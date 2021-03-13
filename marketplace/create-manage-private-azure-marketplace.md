---
title: Cree y administre Azure Marketplace privado en el Azure Portal
description: Obtenga información sobre cómo crear y administrar Azure Marketplace privado (versión preliminar) en el Azure Portal. Azure Marketplace privado (versión preliminar) permite a los administradores regir qué soluciones de terceros pueden usar sus usuarios.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: dbd67ee1d4e9775d37318ec6389888f03a50b6ec
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412716"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Cree y administre Azure Marketplace privado en el Azure Portal

Azure Marketplace privado permite a los administradores regir qué soluciones de terceros pueden usar sus usuarios. Para ello, permite al usuario implementar solo las ofertas aprobadas por el administrador y cumplir con las directivas de su empresa. Con Azure Marketplace privado, los usuarios pueden buscar ofertas compatibles para comprar e implementar en la tienda en línea.

Como administrador de Marketplace (rol asignado), comenzará con un almacén privado deshabilitado y vacío, donde puede Agregar los planes y ofertas aprobados. En este artículo se explica cómo asignar el rol necesario, crear un almacén privado, administrar elementos, aprobar solicitudes de usuario y habilitar Azure Marketplace privado para los usuarios.

> [!NOTE]
> - Azure Marketplace privado está en el nivel de inquilino, por lo que todos los usuarios del inquilino verán la misma lista de seleccionada.
> - Todas las soluciones de Microsoft (incluidas las [distribuciones de Linux aprobadas](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) se agregan automáticamente a Azure Marketplace privado.

## <a name="assign-the-marketplace-admin-role"></a>Asignar el rol de administrador de Marketplace

El administrador global del inquilino debe asignar el rol de **Administrador de Marketplace** al administrador privado de Azure Marketplace que va a administrar la tienda privada.

>[!IMPORTANT]
> El acceso a la administración privada de Azure Marketplace solo está disponible para los administradores de TI con el rol de administrador de Marketplace asignado.

### <a name="prerequisites"></a>Requisitos previos

Estos requisitos previos son necesarios para poder asignar el rol de administrador de Marketplace a un usuario en el ámbito del inquilino:

- Tiene acceso a un usuario de **administrador global** .
- El inquilino tiene al menos una suscripción (puede ser cualquier tipo).
- Al usuario administrador global se le asigna el rol **colaborador** o superior para la suscripción elegida.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Asignar el rol de administrador de Marketplace con control de acceso (IAM)

1. Inicie sesión en [Azure Portal](https://portal.azure.com/).
1. Seleccione **todos los servicios** y, a continuación, **Marketplace**.
1. Seleccione **Marketplace privado** en el menú de la izquierda.

    [![Muestra la opción de menú de Marketplace privado en el lado izquierdo de Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)

1. Seleccione **control de acceso (IAM)** para asignar el rol de administrador de Marketplace.

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Muestra la pantalla de control de acceso I A M.":::

1. Seleccione **Agregar** > **Agregar asignación de roles**.
1. En **rol**, elija **Administración de Marketplace**.

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Muestra el menú de asignación de roles.":::

1. Seleccione el usuario deseado en la lista desplegable y, a continuación, seleccione **listo**.

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Asignación del rol de administrador de Marketplace con PowerShell

Use el siguiente script de PowerShell para asignar el rol de administrador de Marketplace. requiere los siguientes parámetros:

- **TenantId:** El identificador del inquilino en el ámbito (el rol de administrador de Marketplace es asignable en el ámbito del inquilino).
- **SubscriptionId:** Suscripción de la que el administrador global tiene asignado el rol de **colaborador** o superior.
- **GlobalAdminUsername:** El nombre de usuario del administrador global.
- **UsernameToAssignRoleFor:** El nombre de usuario al que se asignará el rol de administrador de Marketplace.

> [!NOTE]
> Para los usuarios invitados invitados al inquilino, puede tardar hasta 48 horas hasta que su cuenta esté disponible para asignar el rol de administrador de Marketplace. Para obtener más información, consulte [propiedades de un usuario de colaboración de Azure Active Directory B2B](/azure/active-directory/b2b/user-properties).

```PowerShell
function Assign-MarketplaceAdminRole { 
[CmdletBinding()] 
param( 
[Parameter(Mandatory)] 
[string]$TenantId, 
 
[Parameter(Mandatory)] 
[string]$SubscriptionId, 

 

[Parameter(Mandatory)] 
[string]$GlobalAdminUsername, 

 

[Parameter(Mandatory)] 
[string]$UsernameToAssignRoleFor 
) 

$MarketplaceAdminRoleDefinitionName = "Marketplace Admin" 

 

Write-Output "TenantId = $TenantId" 
Write-Output "SubscriptionId = $SubscriptionId" 
Write-Output "GlobalAdminUsername = $GlobalAdminUsername" 
Write-Output "UsernameToAssignRoleFor = $UsernameToAssignRoleFor" 

 

Write-Output "$($GlobalAdminUsername) is about to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)" 

 

$profile = Connect-AzAccount -Tenant $TenantId -SubscriptionId $SubscriptionId

 

 
if($profile -eq $null) 
{ 
Write-Error -Message "Failed to connect to tenant and/or subscription" -ErrorAction Stop 
} 
elseif($profile.Context.Account.Id -ne $GlobalAdminUsername) 
{ 
Write-Error "Connected with $($profile.Context.Account.Id) instead of with the global admin that was specified in the script parameters, which is $($GlobalAdminUsername)" 
} 
else 
{ 
Write-Output "$($GlobalAdminUsername) was connected successfully to Tenant=$($profile.Context.Tenant), Subscription=$($profile.Context.Subscription), AccountId=$($profile.Context.Account.Id), Environment=$($profile.Context.Environment)" 
} 

 

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

 

if($MarketPlaceAdminRole -eq $null) 
{ 
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop 
} 
else 
{ 
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available" 
} 

 

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..." 

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace" 

} 

Assign-MarketplaceAdminRole 
```

Para obtener más información acerca de los cmdlets incluidos en el Módulo AZ. portal de PowerShell, consulte [Microsoft Azure PowerShell: cmdlets del panel del portal](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Creación de Azure Marketplace privado

1. Inicie sesión en [Azure Portal](https://portal.azure.com/).
2. Seleccione **todos los servicios** y, a continuación, **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Muestra la ventana principal de Azure Portal.":::

3. Seleccione **Marketplace privado** en el menú de la izquierda.

4. Seleccione **Introducción** para crear un Azure Marketplace privado (solo tiene que hacerlo una vez).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Muestra cómo seleccionar la ventana principal &quot;Introducción a la Azure Portal&quot;.":::

    Si ya existe un Azure Marketplace privado para este inquilino, **administrar Marketplace** se seleccionará de forma predeterminada.

5. Una vez completado, tendrá un Azure Marketplace privado vacío y deshabilitado.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Muestra la pantalla privada vacía de Azure Marketplace.":::

## <a name="add-items-from-gallery"></a>Agregar elementos de la galería

Un elemento es una combinación de una oferta y un plan. Puede buscar y agregar elementos en la página Administrar Marketplace.

1. Seleccione **Agregar elementos**.

2. Examine la **Galería** o use el campo de búsqueda para buscar el elemento que desee.

    [![Muestra cómo examinar la galería o usar el campo de búsqueda.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)

3. De forma predeterminada, al agregar una nueva oferta, se agregarán todos los planes actuales a la lista aprobada. Para modificar la selección del plan antes de agregar los elementos seleccionados, seleccione el menú desplegable en el icono de la oferta y actualice los planes necesarios.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Muestra cómo actualizar los planes necesarios.":::

4. Seleccione **listo** en la parte inferior izquierda después de haber realizado las selecciones.

>[!Note]
> **Agregar elementos** a Marketplace solo estará disponible para las ofertas que no sean de Microsoft. Las soluciones de Microsoft (incluidas las [distribuciones de Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)aprobadas) se etiquetarán como "aprobadas de forma predeterminada" y no se pueden administrar en Marketplace privado.

## <a name="edit-items-plans"></a>Editar planes del elemento

Puede editar los planes de un elemento en la página Administrar Marketplace.

1. En la columna **planes** , revise los planes disponibles en el menú desplegable de ese elemento.
2. Active o desactive las casillas de verificación para elegir los planes que se van a poner a disposición de los usuarios.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Muestra cómo activar o desactivar la casilla para el elemento requerido.":::

> [!NOTE]
> Cada oferta necesita al menos un plan seleccionado para que se produzca la actualización. Para quitar todos los planes relacionados con una oferta, elimine la oferta completa (consulte la sección siguiente).

## <a name="delete-offers"></a>Eliminación de ofertas

En la página Administrar Marketplace, active la casilla situada junto al nombre de la oferta (consulte la pantalla anterior) y seleccione **eliminar elementos**.

## <a name="enabledisable-private-azure-marketplace"></a>Habilitación o deshabilitación de Azure Marketplace privado

En la página Administrar Marketplace verá uno de estos banners, que muestran el estado actual de Azure Marketplace privado:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Muestra el banner &quot;deshabilitar estado&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Muestra el banner ' habilitar estado '.":::

Puede habilitar o deshabilitar Azure Marketplace privado según sea necesario.

- Si está deshabilitada, seleccione **Habilitar Marketplace privado** para habilitar.
- Si está habilitada, seleccione Deshabilitar **Marketplace privado** para deshabilitar.

## <a name="private-azure-marketplace-notification-center"></a>Centro de notificaciones privado de Azure Marketplace

El centro de notificaciones consta de tres tipos de notificaciones y permite que el administrador de Marketplace realice acciones en función de la notificación:

- Solicitudes de aprobación de los usuarios para los elementos que no están en la lista aprobada (consulte [solicitud para agregar ofertas o planes](#request-to-add-offers-or-plans) a continuación).
- Nuevas notificaciones del plan para las ofertas que ya tienen uno o más planes en la lista aprobada.
- Se han quitado las notificaciones del plan para los elementos que se encuentran en la lista aprobada pero que se han quitado de Azure Marketplace global.

Para tener acceso al centro de notificaciones:

1. Seleccione **notificaciones** en el menú de la izquierda.

    [![Muestra el menú notificaciones.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)

1. Seleccione el menú de puntos suspensivos para ver más acciones.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Muestra los resultados del menú más opciones.":::

1. En el caso de las solicitudes de plan, **Mostrar solicitudes** abre el formulario de solicitud de aprobación, donde puede revisar todas las solicitudes de usuario de la oferta específica.
1. Seleccione **aprobar** o **rechazar**.

    [![Muestra las opciones de aprobación y rechazo.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)

1. Seleccione el plan que desea aprobar en el menú desplegable.
1. Agregue un comentario y seleccione **submit (enviar**).

## <a name="browsing-private-azure-marketplace"></a>Exploración de Azure Marketplace privado

Cuando Azure Marketplace privado está habilitado, los usuarios verán qué planes ha aprobado el administrador de Marketplace.

- Un aviso de verde **aprobado** indica que se ha aprobado una oferta de socio comercial (no de Microsoft).
- Un aviso de azul **aprobado** indica una oferta de Microsoft (incluidas las [distribuciones](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)aprobadas de Linux) que está aprobada.

Los usuarios pueden filtrar entre las ofertas que no están aprobadas:

[![Muestra la opción de filtrado.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Comprar o implementar en Azure Marketplace privado

Aunque la experiencia de la página de detalles del producto es similar a la de Azure Marketplace global, hay tres escenarios privados específicos de Azure Marketplace.

- Cuando un usuario selecciona un plan aprobado, se habilita el botón **crear** :

    [![Muestra el banner de la oferta que indica que se puede crear un plan.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)

- Si la selección de un plan de producto no aparece en la página de detalles del producto, pero el administrador ha aprobado uno o más planes, un banner anota qué planes están aprobados y el botón **crear** está habilitado:

    [![Muestra el banner de la oferta teniendo en cuenta que se puede crear un plan y mostrar los planes disponibles.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)

- Cuando un usuario selecciona un plan no aprobado, un banner anota el plan como no aprobado y el botón **crear** está deshabilitado. El usuario todavía puede solicitar agregar el plan a la lista aprobada (consulte la sección siguiente).

## <a name="request-to-add-offers-or-plans"></a>Solicitud para agregar ofertas o planes

Puede solicitar la adición de una oferta pública o un plan que no está aprobado actualmente en Azure Marketplace privado.

1. Seleccione **solicitud para agregar** en el banner para abrir el **formulario de solicitud de acceso**.

    [![Muestra el banner con el vínculo "solicitud para agregar".](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)

    [![Muestra el formulario de solicitud de acceso para ofertas o planes.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)

1. Seleccione los planes que se van a agregar a la solicitud (**cualquier plan** indica al administrador de Marketplace que no tiene preferencia para un plan dentro de una oferta).

1. Agregue una **justificación** y seleccione **solicitud** para enviar la solicitud.
  
    [![Muestra el formulario de solicitud de acceso para ofertas o planes con entradas de ejemplo.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)

1. Aparecerá una indicación de una solicitud pendiente en el formulario de solicitud de acceso con una opción para **retirar la solicitud**.

    [![Muestra una lista de planes aprobados o pendientes con el vínculo de solicitud de retirada.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)

> [!NOTE]
> Una vez enviado, el formulario de solicitud de aprobación se enviará al [centro de notificaciones](#private-azure-marketplace-notification-center) para que el administrador de Marketplace Revise la solicitud y tome medidas.

## <a name="frequently-asked-questions-faqs"></a>Preguntas más frecuentes (P+F)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Ya estoy bloqueando la aplicación de terceros de Marketplace a través de Azure Policy. ¿En qué se diferencia esto?

Actualmente hay dos maneras de restringir servicios de terceros en Marketplace:

1. A través del portal de EA o el Azure Portal, deshabilite los servicios de terceros o restrinja a "solo SKU de BYOL".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Muestra cómo restringir los servicios en el Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Muestra cómo restringir los servicios en el portal E.":::

2. Cree una directiva de Azure para permitir solo máquinas virtuales específicas. Para más información sobre cómo aplicar directivas a máquinas virtuales Windows, consulte [aplicación de directivas a máquinas virtuales Windows con Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).

Azure Marketplace privado permite más flexibilidad a la hora de restringir y permitir ofertas y planes específicos. Informa a los usuarios finales de la disponibilidad de la implementación en la galería de Marketplace, incluso antes de intentar implementar servicios de terceros. Para permitir la implementación de servicios de terceros, establezca Azure Marketplace en activado/habilitado en el portal de EA y en el Azure Portal.

- Azure Marketplace privado puede ajustar soluciones de asociados no limitadas a las máquinas virtuales.
- Azure Marketplace privado puede ajustar en el nivel de plan y también puede establecer "plan actual y futuro".
- Azure Marketplace privado puede informar a los usuarios finales sobre lo que puede y no se puede implementar.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>¿Cuál es la diferencia entre una oferta privada y un Azure Marketplace privado?

Una **oferta privada** permite a los publicadores crear planes que solo son visibles para los clientes de destino. Esto les permite compartir de forma privada soluciones personalizadas con precios negociados, términos y condiciones privados y configuraciones especializadas. Para obtener más información, consulte [ofertas privadas en Marketplace comercial](https://docs.microsoft.com/azure/marketplace/private-offers).

**Azure Marketplace privado** en el Azure portal permite a los administradores aprobar previamente qué soluciones de terceros pueden implementar sus usuarios. Con un Azure Marketplace privado, los usuarios pueden disfrutar de las ventajas de Azure Marketplace al buscar, comprar e implementar ofertas conformes. Para administrar ofertas privadas basadas en suscripciones en Marketplace privado, el administrador de Marketplace debe tener un rol de "lectura" como mínimo en la suscripción específica.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>He agregado una oferta privada a Azure Marketplace privado, ¿por qué no aparece en la pestaña administrar Marketplace?

Las ofertas privadas basadas en suscripciones solo son visibles para las suscripciones enumeradas en la configuración de la oferta privada. Para ver la oferta privada, asegúrese de que el filtro de suscripción global muestra todas las suscripciones.

[![Muestra el filtro de Marketplace privado.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>¿Podemos incluir imágenes personalizadas en Azure Marketplace privado?

No. Azure Marketplace privado permite que cualquier administrador de TI administre y ajustar soluciones de terceros de Azure Marketplace global. Dado que las imágenes personalizadas no se encuentran en Azure Marketplace global, el administrador de ti no puede escoger y elegir sus imágenes personalizadas. Si desea compartir imágenes personalizadas, use la galería de [imágenes compartidas](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).

1. Guía paso a paso: creación de una galería de imágenes compartidas (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).
2. Cree una definición de imagen dentro de un SIG. El cliente debe elegir **generalizado** para el campo de estado de so. ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Incorpore la imagen administrada a la galería de imágenes compartidas ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).
4. Las imágenes de máquina virtual de SIG residirían en una suscripción. Para que esté disponible para otras suscripciones, use un registro de aplicaciones ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>¿Por qué veo algunas ofertas **aprobadas de forma predeterminada,** aunque el publicador no es Microsoft?

Microsoft es compatible con Linux y tecnología de código abierto en Azure. Las [distribuciones de Linux aprobadas](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) se admiten en Azure y el precio se integra en las máquinas virtuales. Dado que el agente de Linux de Azure ya está instalado en Azure Marketplace, se trata como una oferta de Microsoft. Como las ofertas de Microsoft están aprobadas de forma predeterminada, las distribuciones de Linux aprobadas no se pueden administrar en Azure Marketplace privado y están aprobadas de forma predeterminada.

## <a name="contact-support"></a>Ponerse en contacto con soporte técnico

- Para obtener soporte técnico de Azure Marketplace, visite [Microsoft Q&A](/answers/products/).
