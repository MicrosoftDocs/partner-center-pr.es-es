---
title: Creación y administración de Azure Marketplace privado en Azure Portal
description: Obtenga información sobre cómo crear y administrar Azure Marketplace privado (versión preliminar) en el Azure Portal. Azure Marketplace privado (versión preliminar) permite a los administradores regir qué soluciones de terceros pueden usar sus usuarios.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 09/18/2020
ms.openlocfilehash: 2459e7841c2c33227ad38f9d6fa1fc139fc0326e
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/01/2020
ms.locfileid: "96439246"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a>Creación y administración de Azure Marketplace privado (versión preliminar) en el Azure Portal

Azure Marketplace privado (versión preliminar) permite a los administradores regir qué soluciones de terceros pueden usar sus usuarios. Esto le permite implementar solo las ofertas que apruebe y que cumplan las directivas de su empresa. Con Azure Marketplace privado, los usuarios pueden buscar ofertas compatibles para comprar e implementar en la tienda en línea. 

Como administrador de Marketplace (rol asignado), comenzará con un almacén privado deshabilitado y vacío, donde puede Agregar los planes y ofertas aprobados. En este artículo se explica cómo crear, administrar y habilitar Azure Marketplace privado para los usuarios.

Notas:

- Azure Marketplace privado está en el nivel de inquilino, por lo que todos los usuarios del inquilino verán la misma lista de seleccionada.
- Todas las soluciones de Microsoft se agregan automáticamente a Azure Marketplace privado.

## <a name="assign-the-marketplace-admin-role"></a>Asignar el rol de administrador de Marketplace

El administrador global del inquilino debe asignar el rol de **Administrador de Marketplace** al administrador privado de Azure Marketplace que va a administrar la tienda privada.

>[!IMPORTANT]
> El acceso a la administración privada de Azure Marketplace solo está disponible para los administradores de TI con el rol de administrador de Marketplace asignado.

### <a name="prerequisites"></a>Requisitos previos

Debe cumplir estos requisitos previos para poder asignar el rol de administrador de Marketplace a un usuario en el ámbito del inquilino:

- Tiene acceso a un usuario de **administrador global** .
- El inquilino tiene al menos una suscripción (puede ser cualquier tipo).
- Al usuario administrador global se le asigna el rol **colaborador** o superior para la suscripción elegida.
- El usuario administrador global tiene el acceso con privilegios elevados establecido en **sí** (consulte [elevación de acceso para administrar todas las suscripciones y grupos de administración de Azure](/azure/role-based-access-control/elevate-access-global-admin)).

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

$MarketPlaceAdminRole = Get-AzRoleDefinition $MarketplaceAdminRoleDefinitionName

if($MarketPlaceAdminRole -eq $null)
{
Write-Error -Message "'$($MarketplaceAdminRoleDefinitionName)' role is not available" -ErrorAction Stop
}
else
{
Write-Output -Message "'$($MarketplaceAdminRoleDefinitionName)' role is available"
}

Write-Output -Message "About to assign '$($MarketplaceAdminRoleDefinitionName)' role for $($UsernameToAssignRoleFor)..."
$elevatedAccessOnRoot = Get-AzRoleAssignment | where {$_.RoleDefinitionName -eq "User Access Administrator" -and $_.Scope -eq "/" -and $_.SignInName.Trim().ToLower() -eq $GlobalAdminUsername.Trim().ToLower() } | ft -Property SignInName

if($elevatedAccessOnRoot.Count -eq 0)
{
Write-Error -Message "$($GlobalAdminUsername) doesn't have permissions to assign '$($MarketplaceAdminRoleDefinitionName)'. Please verify it has elevated access 'On' in portal, https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin" -ErrorAction Stop
}
else
{
Write-Output "$GlobalAdminUsername has elevated access on root"
}

New-AzRoleAssignment -SignInName $UsernameToAssignRoleFor -RoleDefinitionName $MarketplaceAdminRoleDefinitionName -Scope "/providers/Microsoft.Marketplace"

}

Assign-MarketplaceAdminRole
```

Para obtener más información acerca de los cmdlets incluidos en el Módulo AZ. portal de PowerShell, consulte [Microsoft Azure PowerShell: cmdlets del panel del portal](/powershell/module/az.portal/).

## <a name="create-private-azure-marketplace"></a>Creación de Azure Marketplace privado

1. Inicie sesión en [Azure Portal](https://portal.azure.com/).
2. Seleccione **todos los servicios** y, a continuación, **Marketplace**.

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal ventana principal.":::

3. Seleccione **Marketplace privado** en las opciones de la izquierda.

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Seleccionar Marketplace privado en la ventana principal de Azure Portal.":::

4. Seleccione **Introducción** para crear un Azure Marketplace privado (solo tiene que hacerlo una vez).

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Seleccionar introducción en la ventana principal de Azure Portal.":::

    Si ya existe un Azure Marketplace privado para este inquilino, **administrar Marketplace** se seleccionará de forma predeterminada.

5. Una vez completado, tendrá un Azure Marketplace privado vacío y deshabilitado.

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="La pantalla de Azure Marketplace privada vacía.":::

## <a name="add-items-from-gallery"></a>Agregar elementos de la galería

Un elemento es una combinación de una oferta y un plan. Puede buscar y agregar un elemento en la página Administrar Marketplace.

1. Seleccione **Agregar elementos**.

2. Examine la **Galería** o use el campo de búsqueda para buscar el elemento que desee.

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Examinar la galería o usar el campo de búsqueda.":::

3. De forma predeterminada, al agregar una nueva oferta, se agregarán todos los planes actuales a la lista de permitidos. Para modificar la selección del plan antes de agregar los elementos seleccionados, seleccione el menú desplegable en el icono de la oferta y actualice los planes necesarios.

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Actualice los planes necesarios.":::

4. Seleccione **listo** en la parte inferior izquierda después de haber realizado las selecciones.

>[!Note]
> **Agregar elementos** a Marketplace solo estará disponible para las ofertas que no sean de Microsoft. Las ofertas de Microsoft están permitidas de forma predeterminada.

## <a name="edit-item-plans"></a>Editar planes de elementos

Puede editar los planes de un elemento en la página Administrar Marketplace.

1. En la columna **planes** , revise los planes disponibles en el menú desplegable de ese elemento.
2. Active o desactive las casillas de verificación para elegir los planes que se van a poner a disposición de los usuarios.

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Activar o desactivar la casilla para el elemento requerido.":::

> [!NOTE]
> Cada oferta necesita al menos un plan seleccionado para que se produzca la actualización. Para quitar todos los planes relacionados con una oferta, elimine la oferta completa (consulte la sección siguiente).

## <a name="delete-offers"></a>Eliminación de ofertas

En la página Administrar Marketplace, active la casilla situada junto al nombre de la oferta (consulte la pantalla anterior) y seleccione **eliminar elementos**.

## <a name="enabledisable-private-azure-marketplace"></a>Habilitación o deshabilitación de Azure Marketplace privado

En la página Administrar Marketplace verá uno de estos banners, que muestran el estado actual de Azure Marketplace privado:

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Deshabilitar banner de estado":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Habilitar banner de estado":::

Puede habilitar o deshabilitar Azure Marketplace privado según sea necesario.

1. Si está deshabilitada, seleccione **Habilitar Marketplace privado** para habilitar.
2. Si está habilitada, seleccione Deshabilitar **Marketplace privado** para deshabilitar.

## <a name="browsing-private-azure-marketplace"></a>Exploración de Azure Marketplace privado

Cuando Azure Marketplace privado está habilitado, los usuarios verán qué planes ha permitido el administrador de Marketplace.

- Un aviso verde **permitido** indica que se permite una oferta de socio comercial (que no es de Microsoft).
- Un aviso azul **permitido** indica una oferta de Microsoft que está permitida.

Los usuarios pueden filtrar entre las ofertas que son y no están permitidas:

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Opción de filtrado.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a>Comprar o implementar en Azure Marketplace privado

Aunque la experiencia de la página de detalles del producto es similar a la de Azure Marketplace pública, hay tres escenarios particulares específicos de Azure Marketplace.

- Cuando un usuario selecciona un plan permitido, se habilita el botón **crear** :

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="El banner de la oferta indicando que se puede crear un plan.":::

- Cuando un usuario selecciona un plan no permitido, un banner indica que el plan no está permitido y el botón **crear** está deshabilitado.

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="No se puede crear el banner de la oferta con un plan.":::

- Si la selección de un plan de producto no aparece en la página de detalles del producto, pero el administrador ha aprobado uno o más planes, un banner anota qué planes están permitidos y el botón **crear** está habilitado:

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="El banner de la oferta indicando que se puede crear un plan y mostrar los planes disponibles.":::

## <a name="contact-support"></a>Ponerse en contacto con soporte técnico

Para obtener soporte técnico de Azure Marketplace, visite [Microsoft Q&A](/answers/products/). 
