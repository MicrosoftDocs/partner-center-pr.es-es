---
title: Creación y administración de Azure Marketplace privado en Azure Portal
description: Obtenga información sobre cómo crear y administrar Azure Marketplace privado (versión preliminar) en el Azure Portal.
ms.prod: marketplace-customer
ms.topic: article
author: keferna
ms.author: keferna
ms.date: 09/18/2020
ms.openlocfilehash: 31179d9fd4068348e689d8b426b7a0307112501a
ms.sourcegitcommit: af4726de429d2b9b7c3656d5cac7d542b0d4af74
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/06/2020
ms.locfileid: "93414865"
---
# <a name="create-and-manage-private-azure-marketplace-preview-in-the-azure-portal"></a><span data-ttu-id="e172d-103">Creación y administración de Azure Marketplace privado (versión preliminar) en el Azure Portal</span><span class="sxs-lookup"><span data-stu-id="e172d-103">Create and manage Private Azure Marketplace (preview) in the Azure portal</span></span>

<span data-ttu-id="e172d-104">Azure Marketplace privado (versión preliminar) permite a los administradores regir qué soluciones de terceros pueden usar sus usuarios.</span><span class="sxs-lookup"><span data-stu-id="e172d-104">Private Azure Marketplace (preview) lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="e172d-105">Esto le permite implementar solo las ofertas que apruebe y que cumplan las directivas de su empresa.</span><span class="sxs-lookup"><span data-stu-id="e172d-105">It does this by allowing you to deploy only offers that you approve and that comply with your enterprise's policies.</span></span> <span data-ttu-id="e172d-106">Con Azure Marketplace privado, los usuarios pueden buscar ofertas compatibles para comprar e implementar en la tienda en línea.</span><span class="sxs-lookup"><span data-stu-id="e172d-106">With Private Azure Marketplace, your users can search the online store for compliant offers to purchase and deploy.</span></span> 

<span data-ttu-id="e172d-107">Como administrador de Marketplace (rol asignado), comenzará con un almacén privado deshabilitado y vacío, donde puede Agregar los planes y ofertas aprobados.</span><span class="sxs-lookup"><span data-stu-id="e172d-107">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="e172d-108">En este artículo se explica cómo crear, administrar y habilitar Azure Marketplace privado para los usuarios.</span><span class="sxs-lookup"><span data-stu-id="e172d-108">This article explains how to create, manage, and enable Private Azure Marketplace for your users.</span></span>

<span data-ttu-id="e172d-109">Notas:</span><span class="sxs-lookup"><span data-stu-id="e172d-109">Notes:</span></span>

- <span data-ttu-id="e172d-110">Azure Marketplace privado está en el nivel de inquilino, por lo que todos los usuarios del inquilino verán la misma lista de seleccionada.</span><span class="sxs-lookup"><span data-stu-id="e172d-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
- <span data-ttu-id="e172d-111">Todas las soluciones de Microsoft se agregan automáticamente a Azure Marketplace privado.</span><span class="sxs-lookup"><span data-stu-id="e172d-111">All Microsoft solutions are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="e172d-112">Asignar el rol de administrador de Marketplace</span><span class="sxs-lookup"><span data-stu-id="e172d-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="e172d-113">El administrador global del inquilino debe asignar el rol de **Administrador de Marketplace** al administrador privado de Azure Marketplace que va a administrar la tienda privada.</span><span class="sxs-lookup"><span data-stu-id="e172d-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="e172d-114">El acceso a la administración privada de Azure Marketplace solo está disponible para los administradores de TI con el rol de administrador de Marketplace asignado.</span><span class="sxs-lookup"><span data-stu-id="e172d-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="e172d-115">Requisitos previos</span><span class="sxs-lookup"><span data-stu-id="e172d-115">Prerequisites</span></span>

<span data-ttu-id="e172d-116">Debe cumplir estos requisitos previos para poder asignar el rol de administrador de Marketplace a un usuario en el ámbito del inquilino:</span><span class="sxs-lookup"><span data-stu-id="e172d-116">You must meet these prerequisites before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="e172d-117">Tiene acceso a un usuario de **administrador global** .</span><span class="sxs-lookup"><span data-stu-id="e172d-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="e172d-118">El inquilino tiene al menos una suscripción (puede ser cualquier tipo).</span><span class="sxs-lookup"><span data-stu-id="e172d-118">The tenant has at least one Subscription (can be any type).</span></span>
- <span data-ttu-id="e172d-119">Al usuario administrador global se le asigna el rol **colaborador** o superior para la suscripción elegida en el paso 2.</span><span class="sxs-lookup"><span data-stu-id="e172d-119">The Global administrator user is assigned the **Contributor** role or higher for the subscription chosen in step 2.</span></span>
- <span data-ttu-id="e172d-120">El usuario administrador global tiene el acceso con privilegios elevados establecido en **sí** (consulte [Elevate-Access-global-admin](/azure/role-based-access-control/elevate-access-global-admin)).</span><span class="sxs-lookup"><span data-stu-id="e172d-120">The Global administrator user has elevated access set to **Yes** (see [elevate-access-global-admin](/azure/role-based-access-control/elevate-access-global-admin)).</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="e172d-121">Asignación del rol de administrador de Marketplace con PowerShell</span><span class="sxs-lookup"><span data-stu-id="e172d-121">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="e172d-122">Use el siguiente script de PowerShell para asignar el rol de administrador de Marketplace. requiere los siguientes parámetros:</span><span class="sxs-lookup"><span data-stu-id="e172d-122">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="e172d-123">**TenantId:** El identificador del inquilino en el ámbito (el rol de administrador de Marketplace es asignable en el ámbito del inquilino).</span><span class="sxs-lookup"><span data-stu-id="e172d-123">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="e172d-124">**SubscriptionId:** Suscripción de la que el administrador global tiene asignado el rol de **colaborador** o superior.</span><span class="sxs-lookup"><span data-stu-id="e172d-124">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="e172d-125">**GlobalAdminUsername:** El nombre de usuario del administrador global.</span><span class="sxs-lookup"><span data-stu-id="e172d-125">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="e172d-126">**UsernameToAssignRoleFor:** El nombre de usuario al que se asignará el rol de administrador de Marketplace.</span><span class="sxs-lookup"><span data-stu-id="e172d-126">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="e172d-127">Para los usuarios invitados invitados al inquilino, puede tardar hasta 48 horas hasta que su cuenta esté disponible para asignar el rol de administrador de Marketplace.</span><span class="sxs-lookup"><span data-stu-id="e172d-127">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace admin role.</span></span> <span data-ttu-id="e172d-128">Para obtener más información, consulte [propiedades de un usuario de colaboración de Azure Active Directory B2B](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="e172d-128">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="e172d-129">Para obtener más información acerca de los cmdlets incluidos en el Módulo AZ. portal de PowerShell, consulte [Microsoft Azure PowerShell: cmdlets del panel del portal](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="e172d-129">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="e172d-130">Creación de Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="e172d-130">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="e172d-131">Inicie sesión en [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="e172d-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="e172d-132">Seleccione **todos los servicios** y, a continuación, **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="e172d-132">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Azure Portal ventana principal.":::

3. <span data-ttu-id="e172d-134">Seleccione **Marketplace privado** en las opciones de la izquierda.</span><span class="sxs-lookup"><span data-stu-id="e172d-134">Select **Private Marketplace** from the options on the left.</span></span>

    :::image type="content" source="media/private-azure/private-marketplace.png" alt-text="Seleccionar Marketplace privado en la ventana principal de Azure Portal.":::

4. <span data-ttu-id="e172d-136">Seleccione **Introducción** para crear un Azure Marketplace privado (solo tiene que hacerlo una vez).</span><span class="sxs-lookup"><span data-stu-id="e172d-136">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Seleccionar introducción en la ventana principal de Azure Portal.":::

    <span data-ttu-id="e172d-138">Si ya existe un Azure Marketplace privado para este inquilino, **administrar Marketplace** se seleccionará de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="e172d-138">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="e172d-139">Una vez completado, tendrá un Azure Marketplace privado vacío y deshabilitado.</span><span class="sxs-lookup"><span data-stu-id="e172d-139">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="La pantalla de Azure Marketplace privada vacía.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="e172d-141">Agregar elementos de la galería</span><span class="sxs-lookup"><span data-stu-id="e172d-141">Add items from gallery</span></span>

<span data-ttu-id="e172d-142">Un elemento es una combinación de una oferta y un plan.</span><span class="sxs-lookup"><span data-stu-id="e172d-142">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="e172d-143">Puede buscar y agregar un elemento en la página Administrar Marketplace.</span><span class="sxs-lookup"><span data-stu-id="e172d-143">You can search for and add item in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="e172d-144">Seleccione **Agregar elementos**.</span><span class="sxs-lookup"><span data-stu-id="e172d-144">Select **Add items**.</span></span>

2. <span data-ttu-id="e172d-145">Examine la **Galería** o use el campo de búsqueda para buscar el elemento que desee.</span><span class="sxs-lookup"><span data-stu-id="e172d-145">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    :::image type="content" source="media/private-azure/marketplace-gallery.png" alt-text="Examinar la galería o usar el campo de búsqueda.":::

3. <span data-ttu-id="e172d-147">De forma predeterminada, al agregar una nueva oferta, se agregarán todos los planes actuales a la lista de permitidos.</span><span class="sxs-lookup"><span data-stu-id="e172d-147">As default, when adding a new offer, all current plans will be added to the allowed list.</span></span> <span data-ttu-id="e172d-148">Para modificar la selección del plan antes de agregar los elementos seleccionados, seleccione el menú desplegable en el icono de la oferta y actualice los planes necesarios.</span><span class="sxs-lookup"><span data-stu-id="e172d-148">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Actualice los planes necesarios.":::

4. <span data-ttu-id="e172d-150">Seleccione **listo** en la parte inferior izquierda después de haber realizado las selecciones.</span><span class="sxs-lookup"><span data-stu-id="e172d-150">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="e172d-151">**Agregar elementos** a Marketplace solo estará disponible para las ofertas que no sean de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e172d-151">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="e172d-152">Las ofertas de Microsoft están permitidas de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="e172d-152">Microsoft offers are allowed by default.</span></span>

## <a name="edit-item-plans"></a><span data-ttu-id="e172d-153">Editar planes de elementos</span><span class="sxs-lookup"><span data-stu-id="e172d-153">Edit item plans</span></span>

<span data-ttu-id="e172d-154">Puede editar los planes de un elemento en la página Administrar Marketplace.</span><span class="sxs-lookup"><span data-stu-id="e172d-154">You can edit an item's plans in the Manage Marketplace page.</span></span>

1. <span data-ttu-id="e172d-155">En la columna **planes** , revise los planes disponibles en el menú desplegable de ese elemento.</span><span class="sxs-lookup"><span data-stu-id="e172d-155">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="e172d-156">Active o desactive las casillas de verificación para elegir los planes que se van a poner a disposición de los usuarios.</span><span class="sxs-lookup"><span data-stu-id="e172d-156">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Activar o desactivar la casilla para el elemento requerido.":::

> [!NOTE]
> <span data-ttu-id="e172d-158">Cada oferta necesita al menos un plan seleccionado para que se produzca la actualización.</span><span class="sxs-lookup"><span data-stu-id="e172d-158">Each offer needs at least one plan selected in order for the update to occur.</span></span> <span data-ttu-id="e172d-159">Para quitar todos los planes relacionados con una oferta, elimine la oferta completa (consulte la sección siguiente).</span><span class="sxs-lookup"><span data-stu-id="e172d-159">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="e172d-160">Eliminación de ofertas</span><span class="sxs-lookup"><span data-stu-id="e172d-160">Delete offers</span></span>

<span data-ttu-id="e172d-161">En la página Administrar Marketplace, active la casilla situada junto al nombre de la oferta (consulte la pantalla anterior) y seleccione **eliminar elementos**.</span><span class="sxs-lookup"><span data-stu-id="e172d-161">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="e172d-162">Habilitación o deshabilitación de Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="e172d-162">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="e172d-163">En la página Administrar Marketplace verá uno de estos banners, que muestran el estado actual de Azure Marketplace privado:</span><span class="sxs-lookup"><span data-stu-id="e172d-163">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Deshabilitar banner de estado":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Habilitar banner de estado":::

<span data-ttu-id="e172d-166">Puede habilitar o deshabilitar Azure Marketplace privado según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="e172d-166">You can enable or disable Private Azure Marketplace as needed.</span></span>

1. <span data-ttu-id="e172d-167">Si está deshabilitada, seleccione **Habilitar Marketplace privado** para habilitar.</span><span class="sxs-lookup"><span data-stu-id="e172d-167">If disabled, select **Enable Private Marketplace** to enable.</span></span>
2. <span data-ttu-id="e172d-168">Si está habilitada, seleccione Deshabilitar **Marketplace privado** para deshabilitar.</span><span class="sxs-lookup"><span data-stu-id="e172d-168">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="e172d-169">Exploración de Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="e172d-169">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="e172d-170">Cuando Azure Marketplace privado está habilitado, los usuarios verán qué planes ha permitido el administrador de Marketplace.</span><span class="sxs-lookup"><span data-stu-id="e172d-170">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has allowed.</span></span>

- <span data-ttu-id="e172d-171">Un aviso verde **permitido** indica que se permite una oferta de socio comercial (que no es de Microsoft).</span><span class="sxs-lookup"><span data-stu-id="e172d-171">A green **Allowed** notice indicates a Partner (non-Microsoft) offer that is allowed.</span></span>
- <span data-ttu-id="e172d-172">Un aviso azul **permitido** indica una oferta de Microsoft que está permitida.</span><span class="sxs-lookup"><span data-stu-id="e172d-172">A blue **Allowed** notice indicates a Microsoft offer that is allowed.</span></span>

<span data-ttu-id="e172d-173">Los usuarios pueden filtrar entre las ofertas que son y no están permitidas:</span><span class="sxs-lookup"><span data-stu-id="e172d-173">Users can filter between offers that are and are not allowed:</span></span>

:::image type="content" source="media/private-azure/filter-option.png" alt-text="Opción de filtrado.":::

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="e172d-175">Comprar o implementar en Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="e172d-175">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="e172d-176">Aunque la experiencia de la página de detalles del producto es similar a la de Azure Marketplace pública, hay tres escenarios particulares específicos de Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="e172d-176">While the product details page experience is similar to the public Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="e172d-177">Cuando un usuario selecciona un plan permitido, se habilita el botón **crear** :</span><span class="sxs-lookup"><span data-stu-id="e172d-177">When a user selects an allowed plan, the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled.png" alt-text="El banner de la oferta indicando que se puede crear un plan.":::

- <span data-ttu-id="e172d-179">Cuando un usuario selecciona un plan no permitido, un banner indica que el plan no está permitido y el botón **crear** está deshabilitado.</span><span class="sxs-lookup"><span data-stu-id="e172d-179">When a user selects a non-allowed plan, a banner notes that the plan is not allowed and the **Create** button is disabled.</span></span>

   :::image type="content" source="media/private-azure/button-create-disabled.png" alt-text="No se puede crear el banner de la oferta con un plan.":::

- <span data-ttu-id="e172d-181">Si la selección de un plan de producto no aparece en la página de detalles del producto, pero el administrador ha aprobado uno o más planes, un banner anota qué planes están permitidos y el botón **crear** está habilitado:</span><span class="sxs-lookup"><span data-stu-id="e172d-181">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are allowed and the **Create** button is enabled:</span></span>

    :::image type="content" source="media/private-azure/button-create-enabled-and-plans.png" alt-text="El banner de la oferta indicando que se puede crear un plan y mostrar los planes disponibles.":::

## <a name="contact-support"></a><span data-ttu-id="e172d-183">Póngase en contacto con el soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="e172d-183">Contact support</span></span>

<span data-ttu-id="e172d-184">Para obtener soporte técnico de Azure Marketplace, visite [Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="e172d-184">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span> 
