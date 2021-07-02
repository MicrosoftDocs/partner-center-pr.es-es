---
title: Creación y administración de Azure Marketplace privado en la Azure Portal
description: Obtenga información sobre cómo crear y administrar Azure Marketplace privado (versión preliminar) en el Azure Portal. La Azure Marketplace privada (versión preliminar) permite a los administradores controlar qué soluciones de terceros pueden usar sus usuarios.
ms.service: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 8a3ffbe5b57c49004518341d27c785dcd1b9ce87
ms.sourcegitcommit: c4601069340445135b551fa96bee6d9923d8aa97
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/01/2021
ms.locfileid: "113173695"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a>Creación y administración de Azure Marketplace privado en la Azure Portal

La Azure Marketplace permite a los administradores controlar qué soluciones de terceros pueden usar sus usuarios. Para ello, permite al usuario implementar solo las ofertas aprobadas por el administrador y cumplir con las directivas de su empresa. Con private Azure Marketplace, los usuarios pueden buscar en la tienda en línea ofertas compatibles para comprar e implementar.

Como administrador de Marketplace (rol asignado), empezará con una tienda privada deshabilitada y vacía donde puede agregar las ofertas y planes aprobados. En este artículo se explica cómo asignar el rol necesario, crear un almacén privado, administrar elementos, aprobar solicitudes de usuario y habilitar Azure Marketplace privado para los usuarios.

> [!NOTE]
> - La Azure Marketplace privada está en el nivel de inquilino, por lo que todos los usuarios del inquilino verán la misma lista de protección.
> - Todas las soluciones de Microsoft (incluidas [las distribuciones de Linux aprobadas)](/azure/virtual-machines/linux/endorsed-distros)se agregan automáticamente a private Azure Marketplace.

## <a name="assign-the-marketplace-admin-role"></a>Asignación del rol de administrador de Marketplace

El inquilino Administrador global asignar el rol de administrador de **Marketplace** al administrador de Azure Marketplace privado que administrará el almacén privado.

>[!IMPORTANT]
> El acceso a la Azure Marketplace privada solo está disponible para los administradores de TI con el rol de administrador de Marketplace asignado.

### <a name="prerequisites"></a>Requisitos previos

Estos requisitos previos son necesarios para poder asignar el rol de administrador de Marketplace a un usuario en el ámbito del inquilino:

- Tiene acceso a un **usuario Administrador global** usuario.
- El inquilino tiene al menos una suscripción (puede ser cualquier tipo).
- Al Administrador global usuario se le asigna el **rol Colaborador** o superior para la suscripción elegida.

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a>Asignación del rol de administrador de Marketplace con control de acceso (IAM)

1. Inicie sesión en [Azure Portal](https://portal.azure.com/).

1. Seleccione **Todos los servicios** y, a continuación, **Marketplace.**

1. Seleccione **Marketplace privado** en el menú de la izquierda.

   :::image type="content" source="media/private-azure/private-marketplace.png" lightbox="media/private-azure/private-marketplace-zoom.png" alt-text="Muestra la opción de menú Marketplace privado en el lado izquierdo de Marketplace.":::

1. Seleccione **Control de acceso (IAM) para** asignar el rol de administrador de Marketplace.

   :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Muestra la pantalla de control de acceso I A M.":::

1. Seleccione **Agregar** > **Agregar asignación de roles**.

1. En **Rol,** elija **Administrador de Marketplace.**

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Muestra el menú Asignación de roles.":::

1. Seleccione el usuario deseado en la lista desplegable y, a continuación, **seleccione Listo.**

### <a name="assign-the-marketplace-admin-role-with-powershell"></a>Asignación del rol de administrador de Marketplace con PowerShell

Use el siguiente script de PowerShell para asignar el rol de administrador de Marketplace. requiere los parámetros siguientes:

- **TenantId:** Identificador del inquilino en el ámbito (el rol de administrador de Marketplace se puede asignar en el ámbito del inquilino).
- **SubscriptionId:** Una suscripción de la que el administrador global tenga asignado **el rol colaborador** o superior.
- **GlobalAdminUsername:** Nombre de usuario del administrador global.
- **UsernameToAssignRoleFor:** Nombre de usuario al que se asignará el rol de administrador de Marketplace.

> [!NOTE]
> Para los usuarios invitados al inquilino, pueden tardar hasta 48 horas hasta que su cuenta esté disponible para asignar el rol de administrador de Marketplace. Para obtener más información, vea [Propiedades de un Azure Active Directory de colaboración B2B](/azure/active-directory/b2b/user-properties).

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

Para obtener más información sobre los cmdlets incluidos en el módulo az.portal de PowerShell, [vea Microsoft Azure PowerShell: Cmdlets del panel del portal.](/powershell/module/az.portal/)

## <a name="create-private-azure-marketplace"></a>Creación de un Azure Marketplace

1. Inicie sesión en [Azure Portal](https://portal.azure.com/).
2. Seleccione **Todos los servicios** y, a continuación, **Marketplace.**

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Muestra la Azure Portal principal.":::

3. Seleccione **Marketplace privado** en el menú de la izquierda.

4. Seleccione **Introducción** para crear Azure Marketplace privado (solo tiene que hacerlo una vez).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Muestra cómo seleccionar el &quot;Introducción en la Azure Portal principal&quot;.":::

    Si la Azure Marketplace privada ya existe para este inquilino, se seleccionará **Administrar Marketplace** de forma predeterminada.

5. Una vez completado, tendrá una cuenta privada vacía y deshabilitada Azure Marketplace.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Muestra la pantalla de Azure Marketplace privada vacía.":::

## <a name="add-items-from-gallery"></a>Adición de elementos desde la galería

Un elemento es una combinación de una oferta y un plan. Puede buscar y agregar elementos en la página Administrar Marketplace.

1. Seleccione **Agregar elementos.**

2. Examine la **Galería** o use el campo de búsqueda para buscar el elemento que desee.

   :::image type="content" source="media/private-azure/marketplace-gallery.png" lightbox="media/private-azure/marketplace-gallery-zoom.png" alt-text="Muestra cómo examinar la galería o usar el campo de búsqueda.":::

3. De forma predeterminada, al agregar una nueva oferta, todos los planes actuales se agregarán a la lista aprobada. Para modificar la selección del plan antes de agregar los elementos seleccionados, seleccione el menú desplegable del icono de la oferta y actualice los planes necesarios.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Muestra cómo actualizar los planes necesarios.":::

4. Seleccione **Listo** en la parte inferior izquierda después de realizar las selecciones.

>[!Note]
> **Agregar elementos** a Marketplace solo estará disponible para ofertas que no sean de Microsoft. Las soluciones de Microsoft (incluidas las distribuciones [de Linux aprobadas)](/azure/virtual-machines/linux/endorsed-distros)se etiquetarán como "Aprobadas de forma predeterminada" y no se pueden administrar en Marketplace privado.

## <a name="edit-items-plans"></a>Editar planes de elementos

Puede editar los planes de un elemento en la página Administrar Marketplace.

1. En la **columna** Planes, revise los planes disponibles en el menú desplegable de ese elemento.

2. Active o desactive las casillas para elegir qué planes quiere que estén disponibles para los usuarios.

   :::image type="content" source="media/private-azure/edit-items.png" alt-text="Muestra cómo activar o borrar la casilla del elemento necesario.":::

   > [!NOTE]
   > Cada oferta necesita al menos un plan seleccionado para que se produzca la actualización. Para quitar todos los planes relacionados con una oferta, elimine toda la oferta (consulte la sección siguiente).

## <a name="delete-offers"></a>Eliminación de ofertas

En la página Administrar Marketplace, active la casilla situada junto al nombre de la oferta (consulte la pantalla anterior) y **seleccione Eliminar elementos**.

## <a name="enabledisable-private-azure-marketplace"></a>Habilitación o deshabilitación de private Azure Marketplace

En la página Administrar Marketplace verá uno de estos banners, que muestran el estado actual de Private Azure Marketplace:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Muestra el banner &quot;Deshabilitar estado&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Muestra el banner &quot;Habilitar estado&quot;.":::

Puede habilitar o deshabilitar private Azure Marketplace según sea necesario.

- Si está deshabilitado, seleccione **Habilitar Marketplace privado** para habilitarlo.
- Si está habilitada, seleccione **Deshabilitar Marketplace privado** para deshabilitarlo.

## <a name="private-azure-marketplace-notification-center"></a>Centro de Azure Marketplace privado

El Centro de notificaciones consta de tres tipos de notificaciones y permite al administrador de Marketplace realizar acciones basadas en la notificación:

- Solicitudes de aprobación de los usuarios para los elementos que no están en la lista aprobada (consulte Solicitud [para agregar ofertas o planes a](#request-to-add-offers-or-plans) continuación).
- Nuevas notificaciones de plan para ofertas que ya tienen uno o varios planes en la lista aprobada.
- Se han quitado las notificaciones de plan para los elementos que están en la lista aprobada, pero que se han quitado de la Azure Marketplace.

Para acceder al centro de notificaciones:

1. Seleccione **Notificaciones en** el menú de la izquierda.

   :::image type="content" source="media/private-azure/marketplace-notifications-small.png" lightbox="media/private-azure/marketplace-notifications.png" alt-text="Muestra el menú Notificaciones.":::

1. Seleccione el menú de puntos suspensivos para más acciones.

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Muestra los resultados del menú Más opciones.":::

1. Para las solicitudes de plan, **Mostrar** solicitudes abre el formulario de solicitud de aprobación, donde puede revisar todas las solicitudes de usuario para la oferta específica.
1. Seleccione **Aprobar** o **Rechazar.**

   :::image type="content" source="media/private-azure/notifications-approve-reject-small.png" lightbox="media/private-azure/notifications-approve-reject.png" alt-text="Muestra las opciones aprobar y rechazar.":::

1. Seleccione el plan que desea aprobar en el menú desplegable.
1. Agregue un comentario y seleccione **Enviar**.

## <a name="browsing-private-azure-marketplace"></a>Exploración de private Azure Marketplace

Cuando la Azure Marketplace privada está habilitada, los usuarios verán qué planes ha aprobado el administrador de Marketplace.

- Un aviso **verde aprobado** indica una oferta de partner (que no es de Microsoft) que está aprobada.
- Un aviso **azul aprobado** indica una oferta de Microsoft (incluidas las distribuciones de [Linux aprobadas)](/azure/virtual-machines/linux/endorsed-distros)que está aprobada.

Los usuarios pueden filtrar entre ofertas que son y no están aprobadas:

   :::image type="content" source="media/private-azure/filter-option-small.png" lightbox="media/private-azure/filter-option.png" alt-text="Muestra la opción de filtrado.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Compra o implementación en private Azure Marketplace

Aunque la experiencia de la página de detalles del producto es similar a la Azure Marketplace global, hay tres escenarios Azure Marketplace privados.

- Cuando un usuario selecciona un plan aprobado, se **habilita el** botón Crear:

   :::image type="content" source="media/private-azure/button-create-enabled-small.png" lightbox="media/private-azure/button-create-enabled.png" alt-text="Muestra el banner de la oferta que indica que se puede crear un plan.":::

- Si una selección de plan de producto no aparece en la página de detalles del producto pero el administrador ha aprobado uno o varios planes, un banner indica qué planes están aprobados y el **botón** Crear está habilitado:

   :::image type="content" source="media/private-azure/button-create-enabled-and-plans-small.png" lightbox="media/private-azure/button-create-enabled-and-plans.png" alt-text="Muestra el banner de la oferta que indica que se puede crear un plan y mostrar los planes disponibles.":::

- Cuando un usuario selecciona un plan no aprobado, un banner indica que el plan no está aprobado y el **botón** Crear está deshabilitado. El usuario todavía puede solicitar agregar el plan a la lista aprobada (consulte la sección siguiente).

## <a name="request-to-add-offers-or-plans"></a>Solicitud para agregar ofertas o planes

Puede solicitar agregar una oferta o un plan público que no esté aprobado actualmente en la versión privada Azure Marketplace.

1. Seleccione **Solicitud para agregar en** el banner para abrir el formulario solicitud de **acceso.**

   :::image type="content" source="media/private-azure/request-banner-small.png" lightbox="media/private-azure/request-banner.png" alt-text="Muestra el banner con el vínculo &quot;Solicitud para agregar&quot;.":::

   :::image type="content" source="media/private-azure/access-request-form-small.png" lightbox="media/private-azure/access-request-form.png" alt-text="Muestra el formulario de solicitud de acceso para ofertas o planes.":::

1. Seleccione los planes que desea agregar a la solicitud **(Cualquier plan** indica al administrador de Marketplace que no tiene preferencia para un plan dentro de una oferta).

1. Agregue una **justificación** y **seleccione Solicitud** para enviar la solicitud.

   :::image type="content" source="media/private-azure/access-request-form-filled-small.png" lightbox="media/private-azure/access-request-form-filled.png" alt-text="Muestra el formulario de solicitud de acceso para ofertas o planes con entradas de ejemplo.":::

1. Aparecerá una indicación para una solicitud pendiente en el formulario Solicitud de acceso con una opción para **Retirar solicitud**.

   :::image type="content" source="media/private-azure/approved-pending-plans-small.png" lightbox="media/private-azure/approved-pending-plans.png" alt-text="Muestra una lista de planes aprobados o pendientes con el vínculo Solicitud de retirada.":::

> [!NOTE]
> Una vez enviado, el formulario de [](#private-azure-marketplace-notification-center) solicitud de aprobación se enviará al Centro de notificaciones para que el administrador de Marketplace revise la solicitud y tome medidas.

> [!CAUTION]
> La aprobación en Marketplace privado no indica la adquisición de una solución.

## <a name="frequently-asked-questions-faqs"></a>Preguntas más frecuentes (P+F)

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a>Ya estoy bloqueando la aplicación de terceros de Marketplace a través de Azure Policy. ¿En qué se diferencia esto?

Actualmente hay dos maneras de restringir servicios de terceros en Marketplace:

1. A través del portal de EA Azure Portal, deshabilite servicios de terceros o restrinja a "Solo SKU gratuitas o BYOL".

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Muestra cómo restringir los servicios en el Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Muestra cómo restringir los servicios en el portal de E A.":::

2. Cree una directiva de Azure para permitir solo máquinas virtuales específicas. Para obtener más información sobre cómo aplicar la directiva a Windows virtuales, consulte Aplicación de directivas a Windows máquinas virtuales [con Azure Resource Manager](/azure/virtual-machines/windows/policy).

La Azure Marketplace privada permite más flexibilidad en la restricción y la posibilidad de ofertas y planes específicos. Informa a los usuarios finales sobre la disponibilidad para la implementación en la galería de Marketplace incluso antes de intentar implementar servicios de terceros. Para permitir la implementación de servicios de terceros, establezca Azure Marketplace en Activado/Habilitado en EA Portal y el Azure Portal.

- Las Azure Marketplace pueden resociar soluciones de asociados no limitadas a máquinas virtuales.
- Los Azure Marketplace pueden seleccionar en el nivel de plan y también pueden establecer "Plan actual y futuro".
- Los Azure Marketplace pueden informar a los usuarios finales por adelantado sobre qué se puede implementar y qué no.

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a>¿Cuál es la diferencia entre una oferta privada y una oferta Azure Marketplace?

Una **oferta privada permite** a los anunciantes crear planes que solo son visibles para los clientes de destino. Esto les permite compartir de forma privada soluciones personalizadas con precios negociados, términos y condiciones privados y configuraciones especializadas. Para más información, consulte [Ofertas privadas en marketplace comercial.](/azure/marketplace/private-offers)

**Las Azure Marketplace** privadas de la Azure Portal permiten a los administradores aprobar previamente qué soluciones de terceros pueden implementar sus usuarios. Con un Azure Marketplace privado, los usuarios pueden disfrutar de las ventajas de Azure Marketplace mediante la búsqueda, la compra y la implementación de ofertas compatibles. Para administrar ofertas privadas basadas en suscripciones en Marketplace privado, el administrador de Marketplace debe tener un rol mínimo de "lectura" en la suscripción específica.

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a>He agregado una oferta privada a la Azure Marketplace privada, ¿por qué no se muestra en la pestaña Administrar Marketplace?

Las ofertas privadas basadas en suscripciones solo son visibles para las suscripciones enumeradas en la configuración de la oferta privada. Para ver la oferta privada, asegúrese de que el filtro de suscripción global muestra todas las suscripciones.

   :::image type="content" source="media/private-azure/private-marketplace-filter.png" lightbox="media/private-azure/private-marketplace-filter.png" alt-text="Muestra el filtro de Marketplace privado.":::

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a>¿Se pueden incluir imágenes personalizadas en Private Azure Marketplace?

No. La Azure Marketplace permite a cualquier administrador de TI administrar y administrar soluciones de terceros de soluciones Azure Marketplace. Dado que las imágenes personalizadas no están en Azure Marketplace global, el administrador de TI no puede elegir ni elegir las imágenes personalizadas. Si desea compartir imágenes personalizadas, use [Shared Image Gallery](/azure/virtual-machines/shared-image-galleries).

1. Guía paso a paso Creación de una Shared Image Gallery (SIG)[(CLI,](/azure/virtual-machines/shared-images-cli) [PowerShell](/azure/virtual-machines/shared-images-powershell)).
2. Cree una definición de imagen dentro de una SIG. El cliente debe **elegir Generalizado para** el campo Estado del sistema operativo. [(CLI,](/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition) [PowerShell](/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).
3. Lleve la imagen administrada a la Shared Image Gallery[(CLI,](/azure/virtual-machines/image-version-managed-image-cli) [PowerShell).](/azure/virtual-machines/image-version-managed-image-powershell)
4. Las imágenes de máquina virtual SIG residirán en una suscripción. Para que esté disponible para otras suscripciones, use un registro de aplicación[(CLI,](/azure/virtual-machines/linux/share-images-across-tenants) [PowerShell).](/azure/virtual-machines/windows/share-images-across-tenants)

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a>¿Por qué veo algunas ofertas **aprobadas de forma predeterminada** aunque el publicador no sea Microsoft?

Microsoft admite Linux y tecnología de código abierto en Azure. [Las distribuciones de Linux aprobadas](/azure/virtual-machines/linux/endorsed-distros) se admiten en Azure y el precio se integra en máquinas virtuales. Dado que el agente linux de Azure ya está preinstalado en Azure Marketplace, se trata como una oferta de Microsoft. Puesto que las ofertas de Microsoft están aprobadas de forma predeterminada, las distribuciones de Linux aprobadas no se pueden administrar en private Azure Marketplace y se aprueban de forma predeterminada.

## <a name="contact-support"></a>Ponerse en contacto con soporte técnico

- Para Azure Marketplace soporte técnico, visite [Microsoft Q&A](/answers/products/).