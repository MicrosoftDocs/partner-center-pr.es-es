---
title: Cree y administre Azure Marketplace privado en el Azure Portal
description: Obtenga información sobre cómo crear y administrar Azure Marketplace privado (versión preliminar) en el Azure Portal. Azure Marketplace privado (versión preliminar) permite a los administradores regir qué soluciones de terceros pueden usar sus usuarios.
ms.prod: marketplace-customer
ms.topic: how-to
author: msjogarrig
ms.author: jogarrig
ms.date: 02/24/2021
ms.openlocfilehash: 73b9137728fba93704d9b0cb2bc93a3f6498bd90
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756921"
---
# <a name="create-and-manage-private-azure-marketplace-in-the-azure-portal"></a><span data-ttu-id="138b8-104">Cree y administre Azure Marketplace privado en el Azure Portal</span><span class="sxs-lookup"><span data-stu-id="138b8-104">Create and manage Private Azure Marketplace in the Azure portal</span></span>

<span data-ttu-id="138b8-105">Azure Marketplace privado permite a los administradores regir qué soluciones de terceros pueden usar sus usuarios.</span><span class="sxs-lookup"><span data-stu-id="138b8-105">Private Azure Marketplace lets administrators govern which third-party solutions their users can use.</span></span> <span data-ttu-id="138b8-106">Para ello, permite al usuario implementar solo las ofertas aprobadas por el administrador y cumplir con las directivas de su empresa.</span><span class="sxs-lookup"><span data-stu-id="138b8-106">It does this by allowing the user to deploy only offers that are approved by the administrator and comply with your enterprise's policies.</span></span> <span data-ttu-id="138b8-107">Con Azure Marketplace privado, los usuarios pueden buscar ofertas compatibles para comprar e implementar en la tienda en línea.</span><span class="sxs-lookup"><span data-stu-id="138b8-107">With Private Azure Marketplace, users can search the online store for compliant offers to purchase and deploy.</span></span>

<span data-ttu-id="138b8-108">Como administrador de Marketplace (rol asignado), comenzará con un almacén privado deshabilitado y vacío, donde puede Agregar los planes y ofertas aprobados.</span><span class="sxs-lookup"><span data-stu-id="138b8-108">As a Marketplace admin (assigned role), you will start with a disabled and empty Private Store where you can add your approved offers and plans.</span></span> <span data-ttu-id="138b8-109">En este artículo se explica cómo asignar el rol necesario, crear un almacén privado, administrar elementos, aprobar solicitudes de usuario y habilitar Azure Marketplace privado para los usuarios.</span><span class="sxs-lookup"><span data-stu-id="138b8-109">This article explains how to assign the needed role, create a private store, manage items, approve user requests, and enable Private Azure Marketplace for your users.</span></span>

> [!NOTE]
> - <span data-ttu-id="138b8-110">Azure Marketplace privado está en el nivel de inquilino, por lo que todos los usuarios del inquilino verán la misma lista de seleccionada.</span><span class="sxs-lookup"><span data-stu-id="138b8-110">Private Azure Marketplace is at a tenant level, so all users under the tenant will see the same curated list.</span></span>
> - <span data-ttu-id="138b8-111">Todas las soluciones de Microsoft (incluidas las [distribuciones de Linux aprobadas](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) se agregan automáticamente a Azure Marketplace privado.</span><span class="sxs-lookup"><span data-stu-id="138b8-111">All Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) are automatically added to Private Azure Marketplace.</span></span>

## <a name="assign-the-marketplace-admin-role"></a><span data-ttu-id="138b8-112">Asignar el rol de administrador de Marketplace</span><span class="sxs-lookup"><span data-stu-id="138b8-112">Assign the Marketplace admin role</span></span>

<span data-ttu-id="138b8-113">El administrador global del inquilino debe asignar el rol de **Administrador de Marketplace** al administrador privado de Azure Marketplace que va a administrar la tienda privada.</span><span class="sxs-lookup"><span data-stu-id="138b8-113">The tenant Global administrator must assign the **Marketplace admin** role to the Private Azure Marketplace admin who will manage the private store.</span></span>

>[!IMPORTANT]
> <span data-ttu-id="138b8-114">El acceso a la administración privada de Azure Marketplace solo está disponible para los administradores de TI con el rol de administrador de Marketplace asignado.</span><span class="sxs-lookup"><span data-stu-id="138b8-114">Access to Private Azure Marketplace management is only available to IT admins with the Marketplace admin role assigned.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="138b8-115">Requisitos previos</span><span class="sxs-lookup"><span data-stu-id="138b8-115">Prerequisites</span></span>

<span data-ttu-id="138b8-116">Estos requisitos previos son necesarios para poder asignar el rol de administrador de Marketplace a un usuario en el ámbito del inquilino:</span><span class="sxs-lookup"><span data-stu-id="138b8-116">These prerequisites are required before you can assign the Marketplace Admin role to a user on the tenant scope:</span></span>

- <span data-ttu-id="138b8-117">Tiene acceso a un usuario de **administrador global** .</span><span class="sxs-lookup"><span data-stu-id="138b8-117">You have access to a **Global administrator** user.</span></span>
- <span data-ttu-id="138b8-118">El inquilino tiene al menos una suscripción (puede ser cualquier tipo).</span><span class="sxs-lookup"><span data-stu-id="138b8-118">The tenant has at least one subscription (can be any type).</span></span>
- <span data-ttu-id="138b8-119">Al usuario administrador global se le asigna el rol **colaborador** o superior para la suscripción elegida.</span><span class="sxs-lookup"><span data-stu-id="138b8-119">The Global administrator user is assigned the **Contributor** role or higher for the chosen subscription.</span></span>

### <a name="assign-the-marketplace-admin-role-with-access-control-iam"></a><span data-ttu-id="138b8-120">Asignar el rol de administrador de Marketplace con control de acceso (IAM)</span><span class="sxs-lookup"><span data-stu-id="138b8-120">Assign the Marketplace admin role with access control (IAM)</span></span>

1. <span data-ttu-id="138b8-121">Inicie sesión en [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="138b8-121">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
1. <span data-ttu-id="138b8-122">Seleccione **todos los servicios** y, a continuación, **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="138b8-122">Select **All services** and then **Marketplace**.</span></span>
1. <span data-ttu-id="138b8-123">Seleccione **Marketplace privado** en el menú de la izquierda.</span><span class="sxs-lookup"><span data-stu-id="138b8-123">Select **Private Marketplace** from the menu on the left.</span></span>

    <span data-ttu-id="138b8-124">[![Muestra la opción de menú de Marketplace privado en el lado izquierdo de Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="138b8-124">[![Shows the private marketplace menu option on the left side of the Marketplace.](media/private-azure/private-marketplace.png)](media/private-azure/private-marketplace-zoom.png#lightbox)</span></span>

1. <span data-ttu-id="138b8-125">Seleccione **control de acceso (IAM)** para asignar el rol de administrador de Marketplace.</span><span class="sxs-lookup"><span data-stu-id="138b8-125">Select **Access control (IAM)** to assign the Marketplace admin role.</span></span>

    :::image type="content" source="media/private-azure/access-control-iam.png" alt-text="Muestra la pantalla de control de acceso I A M.":::

1. <span data-ttu-id="138b8-127">Seleccione **Agregar** > **Agregar asignación de roles**.</span><span class="sxs-lookup"><span data-stu-id="138b8-127">Select **+ Add** > **Add role assignment**.</span></span>
1. <span data-ttu-id="138b8-128">En **rol**, elija **Administración de Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="138b8-128">Under **Role**, choose **Marketplace Admin**.</span></span>

    :::image type="content" source="media/private-azure/iam-role-assignment.png" alt-text="Muestra el menú de asignación de roles.":::

1. <span data-ttu-id="138b8-130">Seleccione el usuario deseado en la lista desplegable y, a continuación, seleccione **listo**.</span><span class="sxs-lookup"><span data-stu-id="138b8-130">Select the desired user from the dropdown list, then select **Done**.</span></span>

### <a name="assign-the-marketplace-admin-role-with-powershell"></a><span data-ttu-id="138b8-131">Asignación del rol de administrador de Marketplace con PowerShell</span><span class="sxs-lookup"><span data-stu-id="138b8-131">Assign the Marketplace admin role with PowerShell</span></span>

<span data-ttu-id="138b8-132">Use el siguiente script de PowerShell para asignar el rol de administrador de Marketplace. requiere los siguientes parámetros:</span><span class="sxs-lookup"><span data-stu-id="138b8-132">Use the following PowerShell script to assign the Marketplace Admin role; it requires the following parameters:</span></span>

- <span data-ttu-id="138b8-133">**TenantId:** El identificador del inquilino en el ámbito (el rol de administrador de Marketplace es asignable en el ámbito del inquilino).</span><span class="sxs-lookup"><span data-stu-id="138b8-133">**TenantId:** The ID of the tenant in scope (Marketplace admin role is assignable on the tenant scope).</span></span>
- <span data-ttu-id="138b8-134">**SubscriptionId:** Suscripción de la que el administrador global tiene asignado el rol de **colaborador** o superior.</span><span class="sxs-lookup"><span data-stu-id="138b8-134">**SubscriptionId:** A subscription of which the global admin has **Contributor** role or higher assigned.</span></span>
- <span data-ttu-id="138b8-135">**GlobalAdminUsername:** El nombre de usuario del administrador global.</span><span class="sxs-lookup"><span data-stu-id="138b8-135">**GlobalAdminUsername:** The username of the global admin.</span></span>
- <span data-ttu-id="138b8-136">**UsernameToAssignRoleFor:** El nombre de usuario al que se asignará el rol de administrador de Marketplace.</span><span class="sxs-lookup"><span data-stu-id="138b8-136">**UsernameToAssignRoleFor:** The user name to which the Marketplace admin role will be assigned.</span></span>

> [!NOTE]
> <span data-ttu-id="138b8-137">Para los usuarios invitados invitados al inquilino, puede tardar hasta 48 horas hasta que su cuenta esté disponible para asignar el rol de administrador de Marketplace.</span><span class="sxs-lookup"><span data-stu-id="138b8-137">For guest users invited to the tenant, it may take up to 48 hours until their account is available for assigning the Marketplace Admin role.</span></span> <span data-ttu-id="138b8-138">Para obtener más información, consulte [propiedades de un usuario de colaboración de Azure Active Directory B2B](/azure/active-directory/b2b/user-properties).</span><span class="sxs-lookup"><span data-stu-id="138b8-138">For more information, see [Properties of an Azure Active Directory B2B collaboration user](/azure/active-directory/b2b/user-properties).</span></span>

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

<span data-ttu-id="138b8-139">Para obtener más información acerca de los cmdlets incluidos en el Módulo AZ. portal de PowerShell, consulte [Microsoft Azure PowerShell: cmdlets del panel del portal](/powershell/module/az.portal/).</span><span class="sxs-lookup"><span data-stu-id="138b8-139">For more information about the cmdlets contained in the Az.Portal PowerShell module, see [Microsoft Azure PowerShell: Portal Dashboard cmdlets](/powershell/module/az.portal/).</span></span>

## <a name="create-private-azure-marketplace"></a><span data-ttu-id="138b8-140">Creación de Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="138b8-140">Create Private Azure Marketplace</span></span>

1. <span data-ttu-id="138b8-141">Inicie sesión en [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="138b8-141">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="138b8-142">Seleccione **todos los servicios** y, a continuación, **Marketplace**.</span><span class="sxs-lookup"><span data-stu-id="138b8-142">Select **All services** and then **Marketplace**.</span></span>

   :::image type="content" source="media/private-azure/azure-portal-marketplace.png" alt-text="Muestra la ventana principal de Azure Portal.":::

3. <span data-ttu-id="138b8-144">Seleccione **Marketplace privado** en el menú de la izquierda.</span><span class="sxs-lookup"><span data-stu-id="138b8-144">Select **Private Marketplace** from the menu on the left.</span></span>

4. <span data-ttu-id="138b8-145">Seleccione **Introducción** para crear un Azure Marketplace privado (solo tiene que hacerlo una vez).</span><span class="sxs-lookup"><span data-stu-id="138b8-145">Select **Get Started** to create Private Azure Marketplace (you only have to do this once).</span></span>

    :::image type="content" source="media/private-azure/private-marketplace-get-started.png" alt-text="Muestra cómo seleccionar la ventana principal &quot;Introducción a la Azure Portal&quot;.":::

    <span data-ttu-id="138b8-147">Si ya existe un Azure Marketplace privado para este inquilino, **administrar Marketplace** se seleccionará de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="138b8-147">If Private Azure Marketplace already exists for this tenant, **Manage Marketplace** will be selected by default.</span></span>

5. <span data-ttu-id="138b8-148">Una vez completado, tendrá un Azure Marketplace privado vacío y deshabilitado.</span><span class="sxs-lookup"><span data-stu-id="138b8-148">Once completed you will have an empty and disabled Private Azure Marketplace.</span></span>

    :::image type="content" source="media/private-azure/new-private-marketplace.png" alt-text="Muestra la pantalla privada vacía de Azure Marketplace.":::

## <a name="add-items-from-gallery"></a><span data-ttu-id="138b8-150">Agregar elementos de la galería</span><span class="sxs-lookup"><span data-stu-id="138b8-150">Add items from gallery</span></span>

<span data-ttu-id="138b8-151">Un elemento es una combinación de una oferta y un plan.</span><span class="sxs-lookup"><span data-stu-id="138b8-151">An item is a combination of an offer and a plan.</span></span> <span data-ttu-id="138b8-152">Puede buscar y agregar elementos en la página Administrar Marketplace.</span><span class="sxs-lookup"><span data-stu-id="138b8-152">You can search for and add items on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="138b8-153">Seleccione **Agregar elementos**.</span><span class="sxs-lookup"><span data-stu-id="138b8-153">Select **Add items**.</span></span>

2. <span data-ttu-id="138b8-154">Examine la **Galería** o use el campo de búsqueda para buscar el elemento que desee.</span><span class="sxs-lookup"><span data-stu-id="138b8-154">Browse the **Gallery** or use the search field to find the item you want.</span></span>

    <span data-ttu-id="138b8-155">[![Muestra cómo examinar la galería o usar el campo de búsqueda.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="138b8-155">[![Shows how to browse the gallery or use the search field.](media/private-azure/marketplace-gallery.png)](media/private-azure/marketplace-gallery-zoom.png#lightbox)</span></span>

3. <span data-ttu-id="138b8-156">De forma predeterminada, al agregar una nueva oferta, se agregarán todos los planes actuales a la lista aprobada.</span><span class="sxs-lookup"><span data-stu-id="138b8-156">As default, when adding a new offer, all current plans will be added to the approved list.</span></span> <span data-ttu-id="138b8-157">Para modificar la selección del plan antes de agregar los elementos seleccionados, seleccione el menú desplegable en el icono de la oferta y actualice los planes necesarios.</span><span class="sxs-lookup"><span data-stu-id="138b8-157">To modify the plan selection before adding the selected items, select the drop-down menu in the offer’s tile and update the required plans.</span></span>

    :::image type="content" source="media/private-azure/update-plans-400.png" alt-text="Muestra cómo actualizar los planes necesarios.":::

4. <span data-ttu-id="138b8-159">Seleccione **listo** en la parte inferior izquierda después de haber realizado las selecciones.</span><span class="sxs-lookup"><span data-stu-id="138b8-159">Select **Done** at the bottom-left after you've made your selections.</span></span>

>[!Note]
> <span data-ttu-id="138b8-160">**Agregar elementos** a Marketplace solo estará disponible para las ofertas que no sean de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="138b8-160">**Add Items** to the Marketplace will be available for non-Microsoft offers only.</span></span> <span data-ttu-id="138b8-161">Las soluciones de Microsoft (incluidas las [distribuciones de Linux](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)aprobadas) se etiquetarán como "aprobadas de forma predeterminada" y no se pueden administrar en Marketplace privado.</span><span class="sxs-lookup"><span data-stu-id="138b8-161">Microsoft solutions (including [Endorsed Linux Distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) will be tagged as “Approved by default” and cannot be managed in Private Marketplace.</span></span>

## <a name="edit-items-plans"></a><span data-ttu-id="138b8-162">Editar planes del elemento</span><span class="sxs-lookup"><span data-stu-id="138b8-162">Edit item's plans</span></span>

<span data-ttu-id="138b8-163">Puede editar los planes de un elemento en la página Administrar Marketplace.</span><span class="sxs-lookup"><span data-stu-id="138b8-163">You can edit an item's plans on the Manage Marketplace page.</span></span>

1. <span data-ttu-id="138b8-164">En la columna **planes** , revise los planes disponibles en el menú desplegable de ese elemento.</span><span class="sxs-lookup"><span data-stu-id="138b8-164">In the **Plans** column, review the available plans from the dropdown menu for that item.</span></span>
2. <span data-ttu-id="138b8-165">Active o desactive las casillas de verificación para elegir los planes que se van a poner a disposición de los usuarios.</span><span class="sxs-lookup"><span data-stu-id="138b8-165">Select or clear the checkboxes to choose which plans to make available to your users.</span></span>

    :::image type="content" source="media/private-azure/edit-items.png" alt-text="Muestra cómo activar o desactivar la casilla para el elemento requerido.":::

> [!NOTE]
> <span data-ttu-id="138b8-167">Cada oferta necesita al menos un plan seleccionado para que se produzca la actualización.</span><span class="sxs-lookup"><span data-stu-id="138b8-167">Each offer needs at least one plan selected for the update to occur.</span></span> <span data-ttu-id="138b8-168">Para quitar todos los planes relacionados con una oferta, elimine la oferta completa (consulte la sección siguiente).</span><span class="sxs-lookup"><span data-stu-id="138b8-168">To remove all plans related to an offer, delete the entire offer (see next section).</span></span>

## <a name="delete-offers"></a><span data-ttu-id="138b8-169">Eliminación de ofertas</span><span class="sxs-lookup"><span data-stu-id="138b8-169">Delete offers</span></span>

<span data-ttu-id="138b8-170">En la página Administrar Marketplace, active la casilla situada junto al nombre de la oferta (consulte la pantalla anterior) y seleccione **eliminar elementos**.</span><span class="sxs-lookup"><span data-stu-id="138b8-170">In the Manage Marketplace page, select the check box next to the offer name (see screen above) and select **Delete items**.</span></span>

## <a name="enabledisable-private-azure-marketplace"></a><span data-ttu-id="138b8-171">Habilitación o deshabilitación de Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="138b8-171">Enable/disable Private Azure Marketplace</span></span>

<span data-ttu-id="138b8-172">En la página Administrar Marketplace verá uno de estos banners, que muestran el estado actual de Azure Marketplace privado:</span><span class="sxs-lookup"><span data-stu-id="138b8-172">In the Manage Marketplace page you will see one of these banners, which show the current state of Private Azure Marketplace:</span></span>

:::image type="content" source="media/private-azure/state-disable.png" alt-text="Muestra el banner &quot;deshabilitar estado&quot;.":::

:::image type="content" source="media/private-azure/state-enable.png" alt-text="Muestra el banner ' habilitar estado '.":::

<span data-ttu-id="138b8-175">Puede habilitar o deshabilitar Azure Marketplace privado según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="138b8-175">You can enable or disable Private Azure Marketplace as needed.</span></span>

- <span data-ttu-id="138b8-176">Si está deshabilitada, seleccione **Habilitar Marketplace privado** para habilitar.</span><span class="sxs-lookup"><span data-stu-id="138b8-176">If disabled, select **Enable Private Marketplace** to enable.</span></span>
- <span data-ttu-id="138b8-177">Si está habilitada, seleccione Deshabilitar **Marketplace privado** para deshabilitar.</span><span class="sxs-lookup"><span data-stu-id="138b8-177">If enabled, select **Disable Private Marketplace** to disable.</span></span>

## <a name="private-azure-marketplace-notification-center"></a><span data-ttu-id="138b8-178">Centro de notificaciones privado de Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="138b8-178">Private Azure Marketplace notification center</span></span>

<span data-ttu-id="138b8-179">El centro de notificaciones consta de tres tipos de notificaciones y permite que el administrador de Marketplace realice acciones en función de la notificación:</span><span class="sxs-lookup"><span data-stu-id="138b8-179">Notification Center consists of three types of notifications and allows the Marketplace admin to take actions based on the notification:</span></span>

- <span data-ttu-id="138b8-180">Solicitudes de aprobación de los usuarios para los elementos que no están en la lista aprobada (consulte [solicitud para agregar ofertas o planes](#request-to-add-offers-or-plans) a continuación).</span><span class="sxs-lookup"><span data-stu-id="138b8-180">Approval requests from users for items that are not in the approved list (see [Request to add offers or plans](#request-to-add-offers-or-plans) below).</span></span>
- <span data-ttu-id="138b8-181">Nuevas notificaciones del plan para las ofertas que ya tienen uno o más planes en la lista aprobada.</span><span class="sxs-lookup"><span data-stu-id="138b8-181">New plan notifications for offers that already have one or more plans in the approved list.</span></span>
- <span data-ttu-id="138b8-182">Se han quitado las notificaciones del plan para los elementos que se encuentran en la lista aprobada pero que se han quitado de Azure Marketplace global.</span><span class="sxs-lookup"><span data-stu-id="138b8-182">Removed plan notifications for items that are in the approved list but were removed from the global Azure Marketplace.</span></span>

<span data-ttu-id="138b8-183">Para tener acceso al centro de notificaciones:</span><span class="sxs-lookup"><span data-stu-id="138b8-183">To access the notification center:</span></span>

1. <span data-ttu-id="138b8-184">Seleccione **notificaciones** en el menú de la izquierda.</span><span class="sxs-lookup"><span data-stu-id="138b8-184">Select **Notifications** from the left-side menu.</span></span>

    <span data-ttu-id="138b8-185">[![Muestra el menú notificaciones.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="138b8-185">[![Shows the Notifications menu.](media/private-azure/marketplace-notifications-small.png)](media/private-azure/marketplace-notifications.png#lightbox)</span></span>

1. <span data-ttu-id="138b8-186">Seleccione el menú de puntos suspensivos para ver más acciones.</span><span class="sxs-lookup"><span data-stu-id="138b8-186">Select the ellipsis menu for more actions.</span></span>

    :::image type="content" source="media/private-azure/notifications-more-options.png" alt-text="Muestra los resultados del menú más opciones.":::

1. <span data-ttu-id="138b8-188">En el caso de las solicitudes de plan, **Mostrar solicitudes** abre el formulario de solicitud de aprobación, donde puede revisar todas las solicitudes de usuario de la oferta específica.</span><span class="sxs-lookup"><span data-stu-id="138b8-188">For plan requests, **Show requests** opens the approval request form where you can review all user requests for the specific offer.</span></span>
1. <span data-ttu-id="138b8-189">Seleccione **aprobar** o **rechazar**.</span><span class="sxs-lookup"><span data-stu-id="138b8-189">Select **Approve** or **Reject**.</span></span>

    <span data-ttu-id="138b8-190">[![Muestra las opciones de aprobación y rechazo.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="138b8-190">[![Shows the approve and reject options.](media/private-azure/notifications-approve-reject-small.png)](media/private-azure/notifications-approve-reject.png#lightbox)</span></span>

1. <span data-ttu-id="138b8-191">Seleccione el plan que desea aprobar en el menú desplegable.</span><span class="sxs-lookup"><span data-stu-id="138b8-191">Select the plan to approve from the drop-down menu.</span></span>
1. <span data-ttu-id="138b8-192">Agregue un comentario y seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="138b8-192">Add a comment and select **Submit**.</span></span>

## <a name="browsing-private-azure-marketplace"></a><span data-ttu-id="138b8-193">Exploración de Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="138b8-193">Browsing Private Azure Marketplace</span></span>

<span data-ttu-id="138b8-194">Cuando Azure Marketplace privado está habilitado, los usuarios verán qué planes ha aprobado el administrador de Marketplace.</span><span class="sxs-lookup"><span data-stu-id="138b8-194">When Private Azure Marketplace is enabled, users will see which plans the Marketplace admin has approved.</span></span>

- <span data-ttu-id="138b8-195">Un aviso de verde **aprobado** indica que se ha aprobado una oferta de socio comercial (no de Microsoft).</span><span class="sxs-lookup"><span data-stu-id="138b8-195">A green **Approved** notice indicates a Partner (non-Microsoft) offer that is approved.</span></span>
- <span data-ttu-id="138b8-196">Un aviso de azul **aprobado** indica una oferta de Microsoft (incluidas las [distribuciones](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)aprobadas de Linux) que está aprobada.</span><span class="sxs-lookup"><span data-stu-id="138b8-196">A blue **Approved** notice indicates a Microsoft offer (including [Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros)) that is approved.</span></span>

<span data-ttu-id="138b8-197">Los usuarios pueden filtrar entre las ofertas que no están aprobadas:</span><span class="sxs-lookup"><span data-stu-id="138b8-197">Users can filter between offers that are and are not approved:</span></span>

<span data-ttu-id="138b8-198">[![Muestra la opción de filtrado.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="138b8-198">[![Shows the filtering option.](media/private-azure/filter-option-small.png)](media/private-azure/filter-option.png#lightbox)</span></span>

## <a name="buy-or-deploy-in-private-azure-marketplace"></a><span data-ttu-id="138b8-199">Comprar o implementar en Azure Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="138b8-199">Buy or deploy in Private Azure Marketplace</span></span>

<span data-ttu-id="138b8-200">Aunque la experiencia de la página de detalles del producto es similar a la de Azure Marketplace global, hay tres escenarios privados específicos de Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="138b8-200">While the product details page experience is similar to the global Azure Marketplace, there are three Private Azure Marketplace specific scenarios.</span></span>

- <span data-ttu-id="138b8-201">Cuando un usuario selecciona un plan aprobado, se habilita el botón **crear** :</span><span class="sxs-lookup"><span data-stu-id="138b8-201">When a user selects an approved plan, the **Create** button is enabled:</span></span>

    <span data-ttu-id="138b8-202">[![Muestra el banner de la oferta que indica que se puede crear un plan.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="138b8-202">[![Shows the offer banner noting a plan can be created.](media/private-azure/button-create-enabled-small.png)](media/private-azure/button-create-enabled.png#lightbox)</span></span>

- <span data-ttu-id="138b8-203">Si la selección de un plan de producto no aparece en la página de detalles del producto, pero el administrador ha aprobado uno o más planes, un banner anota qué planes están aprobados y el botón **crear** está habilitado:</span><span class="sxs-lookup"><span data-stu-id="138b8-203">If a product plan selection does not appear in the product details page but the admin approved one or more plans, a banner notes which plans are approved and the **Create** button is enabled:</span></span>

    <span data-ttu-id="138b8-204">[![Muestra el banner de la oferta teniendo en cuenta que se puede crear un plan y mostrar los planes disponibles.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="138b8-204">[![Shows the offer banner noting that a plan can be created and showing available plans.](media/private-azure/button-create-enabled-and-plans-small.png)](media/private-azure/button-create-enabled-and-plans.png#lightbox)</span></span>

- <span data-ttu-id="138b8-205">Cuando un usuario selecciona un plan no aprobado, un banner anota el plan como no aprobado y el botón **crear** está deshabilitado.</span><span class="sxs-lookup"><span data-stu-id="138b8-205">When a user selects a non-approved plan, a banner notes the plan as not approved and the **Create** button is disabled.</span></span> <span data-ttu-id="138b8-206">El usuario todavía puede solicitar agregar el plan a la lista aprobada (consulte la sección siguiente).</span><span class="sxs-lookup"><span data-stu-id="138b8-206">The user can still request to add the plan to the approved list (see next section).</span></span>

## <a name="request-to-add-offers-or-plans"></a><span data-ttu-id="138b8-207">Solicitud para agregar ofertas o planes</span><span class="sxs-lookup"><span data-stu-id="138b8-207">Request to add offers or plans</span></span>

<span data-ttu-id="138b8-208">Puede solicitar la adición de una oferta pública o un plan que no está aprobado actualmente en Azure Marketplace privado.</span><span class="sxs-lookup"><span data-stu-id="138b8-208">You can request to add a public offer or plan that is not currently approved in the Private Azure Marketplace.</span></span>

1. <span data-ttu-id="138b8-209">Seleccione **solicitud para agregar** en el banner para abrir el **formulario de solicitud de acceso**.</span><span class="sxs-lookup"><span data-stu-id="138b8-209">Select **Request to add** in the banner to open the **Access request form**.</span></span>

    <span data-ttu-id="138b8-210">[![Muestra el banner con el vínculo "solicitud para agregar".](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="138b8-210">[![Shows the banner with the 'Request to add' link.](media/private-azure/request-banner-small.png)](media/private-azure/request-banner.png#lightbox)</span></span>

    <span data-ttu-id="138b8-211">[![Muestra el formulario de solicitud de acceso para ofertas o planes.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="138b8-211">[![Shows the access request form for offers or plans.](media/private-azure/access-request-form-small.png)](media/private-azure/access-request-form.png#lightbox)</span></span>

1. <span data-ttu-id="138b8-212">Seleccione los planes que se van a agregar a la solicitud (**cualquier plan** indica al administrador de Marketplace que no tiene preferencia para un plan dentro de una oferta).</span><span class="sxs-lookup"><span data-stu-id="138b8-212">Select which plans to add to the request (**Any Plan** tells the Marketplace admin that you don't have a preference for a plan within an offer).</span></span>

1. <span data-ttu-id="138b8-213">Agregue una **justificación** y seleccione **solicitud** para enviar la solicitud.</span><span class="sxs-lookup"><span data-stu-id="138b8-213">Add a **Justification** and select **Request** to submit your request.</span></span>
  
    <span data-ttu-id="138b8-214">[![Muestra el formulario de solicitud de acceso para ofertas o planes con entradas de ejemplo.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="138b8-214">[![Shows the access request form for offers or plans with sample entries.](media/private-azure/access-request-form-filled-small.png)](media/private-azure/access-request-form-filled.png#lightbox)</span></span>

1. <span data-ttu-id="138b8-215">Aparecerá una indicación de una solicitud pendiente en el formulario de solicitud de acceso con una opción para **retirar la solicitud**.</span><span class="sxs-lookup"><span data-stu-id="138b8-215">An indication for a pending request will appear in the Access request form with an option to **Withdraw request**.</span></span>

    <span data-ttu-id="138b8-216">[![Muestra una lista de planes aprobados o pendientes con el vínculo de solicitud de retirada.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="138b8-216">[![Shows a list of approved or pending plans with Withdraw Request link.](media/private-azure/approved-pending-plans-small.png)](media/private-azure/approved-pending-plans.png#lightbox)</span></span>

> [!NOTE]
> <span data-ttu-id="138b8-217">Una vez enviado, el formulario de solicitud de aprobación se enviará al [centro de notificaciones](#private-azure-marketplace-notification-center) para que el administrador de Marketplace Revise la solicitud y tome medidas.</span><span class="sxs-lookup"><span data-stu-id="138b8-217">Once submitted, the approval request form will be sent to the [Notification Center](#private-azure-marketplace-notification-center) for the Marketplace admin to review the request and take action.</span></span>

## <a name="frequently-asked-questions-faqs"></a><span data-ttu-id="138b8-218">Preguntas más frecuentes (P+F)</span><span class="sxs-lookup"><span data-stu-id="138b8-218">Frequently Asked Questions (FAQs)</span></span>

#### <a name="i-am-already-blocking-marketplace-third-party-application-through-azure-policy-how-is-this-different"></a><span data-ttu-id="138b8-219">Ya estoy bloqueando la aplicación de terceros de Marketplace a través de Azure Policy.</span><span class="sxs-lookup"><span data-stu-id="138b8-219">I am already blocking Marketplace third-party application through Azure Policy.</span></span> <span data-ttu-id="138b8-220">¿En qué se diferencia esto?</span><span class="sxs-lookup"><span data-stu-id="138b8-220">How is this different?</span></span>

<span data-ttu-id="138b8-221">Actualmente hay dos maneras de restringir servicios de terceros en Marketplace:</span><span class="sxs-lookup"><span data-stu-id="138b8-221">There are currently two ways to restrict third-party services in Marketplace:</span></span>

1. <span data-ttu-id="138b8-222">A través del portal de EA o el Azure Portal, deshabilite los servicios de terceros o restrinja a "solo SKU de BYOL".</span><span class="sxs-lookup"><span data-stu-id="138b8-222">Through EA portal or the Azure portal, disable third-party services or restrict to “Free or BYOL SKUs only”.</span></span>

    :::image type="content" source="media/private-azure/disable-services.png" alt-text="Muestra cómo restringir los servicios en el Azure Portal.":::

    :::image type="content" source="media/private-azure/disable-services-other-view.png" alt-text="Muestra cómo restringir los servicios en el portal E.":::

2. <span data-ttu-id="138b8-225">Cree una directiva de Azure para permitir solo máquinas virtuales específicas.</span><span class="sxs-lookup"><span data-stu-id="138b8-225">Create an Azure policy to only allow specific VMs.</span></span> <span data-ttu-id="138b8-226">Para más información sobre cómo aplicar directivas a máquinas virtuales Windows, consulte [aplicación de directivas a máquinas virtuales Windows con Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).</span><span class="sxs-lookup"><span data-stu-id="138b8-226">For details on how to enforce policy to Windows VMs, see [Apply policies to Windows VMs with Azure Resource Manager](https://docs.microsoft.com/azure/virtual-machines/windows/policy).</span></span>

<span data-ttu-id="138b8-227">Azure Marketplace privado permite más flexibilidad a la hora de restringir y permitir ofertas y planes específicos.</span><span class="sxs-lookup"><span data-stu-id="138b8-227">Private Azure Marketplace allows more flexibility on restricting and allowing specific offers and plans.</span></span> <span data-ttu-id="138b8-228">Informa a los usuarios finales de la disponibilidad de la implementación en la galería de Marketplace, incluso antes de intentar implementar servicios de terceros.</span><span class="sxs-lookup"><span data-stu-id="138b8-228">It informs end users on the availability for deployment in the marketplace gallery even before they try to deploy third-party services.</span></span> <span data-ttu-id="138b8-229">Para permitir la implementación de servicios de terceros, establezca Azure Marketplace en activado/habilitado en el portal de EA y en el Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="138b8-229">To allow deployment of third-party services, set Azure Marketplace to On/Enabled in EA Portal and the Azure portal.</span></span>

- <span data-ttu-id="138b8-230">Azure Marketplace privado puede ajustar soluciones de asociados no limitadas a las máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="138b8-230">Private Azure Marketplace can curate partner solutions not limited to virtual machines.</span></span>
- <span data-ttu-id="138b8-231">Azure Marketplace privado puede ajustar en el nivel de plan y también puede establecer "plan actual y futuro".</span><span class="sxs-lookup"><span data-stu-id="138b8-231">Private Azure Marketplace can curate at the plan level and can also set “Current and future plan”.</span></span>
- <span data-ttu-id="138b8-232">Azure Marketplace privado puede informar a los usuarios finales sobre lo que puede y no se puede implementar.</span><span class="sxs-lookup"><span data-stu-id="138b8-232">Private Azure Marketplace can inform the end users up front on what can and cannot be deployed.</span></span>

#### <a name="whats-the-difference-between-a-private-offer-and-private-azure-marketplace"></a><span data-ttu-id="138b8-233">¿Cuál es la diferencia entre una oferta privada y un Azure Marketplace privado?</span><span class="sxs-lookup"><span data-stu-id="138b8-233">What's the difference between a Private Offer and Private Azure Marketplace?</span></span>

<span data-ttu-id="138b8-234">Una **oferta privada** permite a los publicadores crear planes que solo son visibles para los clientes de destino.</span><span class="sxs-lookup"><span data-stu-id="138b8-234">A **Private Offer** lets publishers create plans that are only visible to targeted customers.</span></span> <span data-ttu-id="138b8-235">Esto les permite compartir de forma privada soluciones personalizadas con precios negociados, términos y condiciones privados y configuraciones especializadas.</span><span class="sxs-lookup"><span data-stu-id="138b8-235">This lets them privately share customized solutions with negotiated pricing, private terms and conditions, and specialized configurations.</span></span> <span data-ttu-id="138b8-236">Para obtener más información, consulte [ofertas privadas en Marketplace comercial](https://docs.microsoft.com/azure/marketplace/private-offers).</span><span class="sxs-lookup"><span data-stu-id="138b8-236">For details, see [Private offers in the commercial marketplace](https://docs.microsoft.com/azure/marketplace/private-offers).</span></span>

<span data-ttu-id="138b8-237">**Azure Marketplace privado** en el Azure portal permite a los administradores aprobar previamente qué soluciones de terceros pueden implementar sus usuarios.</span><span class="sxs-lookup"><span data-stu-id="138b8-237">**Private Azure Marketplace** in the Azure portal lets administrators pre-approve which third-party solutions their users can deploy.</span></span> <span data-ttu-id="138b8-238">Con un Azure Marketplace privado, los usuarios pueden disfrutar de las ventajas de Azure Marketplace al buscar, comprar e implementar ofertas conformes.</span><span class="sxs-lookup"><span data-stu-id="138b8-238">With a Private Azure Marketplace, users can enjoy the benefits of Azure Marketplace by finding, buying, and deploying compliant offers.</span></span> <span data-ttu-id="138b8-239">Para administrar ofertas privadas basadas en suscripciones en Marketplace privado, el administrador de Marketplace debe tener un rol de "lectura" como mínimo en la suscripción específica.</span><span class="sxs-lookup"><span data-stu-id="138b8-239">To manage subscription-based Private Offers in Private Marketplace, the Marketplace admin must have a minimum of “read” role on the specific subscription.</span></span>

#### <a name="i-added-a-private-offer-to-the-private-azure-marketplace-why-is-it-not-showing-in-the-manage-marketplace-tab"></a><span data-ttu-id="138b8-240">He agregado una oferta privada a Azure Marketplace privado, ¿por qué no aparece en la pestaña administrar Marketplace?</span><span class="sxs-lookup"><span data-stu-id="138b8-240">I added a Private Offer to the Private Azure Marketplace, why is it not showing in the manage marketplace tab?</span></span>

<span data-ttu-id="138b8-241">Las ofertas privadas basadas en suscripciones solo son visibles para las suscripciones enumeradas en la configuración de la oferta privada.</span><span class="sxs-lookup"><span data-stu-id="138b8-241">Subscription-based Private Offers are visible only for the listed subscriptions in the Private Offer settings.</span></span> <span data-ttu-id="138b8-242">Para ver la oferta privada, asegúrese de que el filtro de suscripción global muestra todas las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="138b8-242">To view the Private Offer, ensure the global subscription filter is showing all the subscriptions.</span></span>

<span data-ttu-id="138b8-243">[![Muestra el filtro de Marketplace privado.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span><span class="sxs-lookup"><span data-stu-id="138b8-243">[![Shows the private marketplace filter.](media/private-azure/private-marketplace-filter.png)](media/private-azure/private-marketplace-filter.png#lightbox)</span></span>

#### <a name="can-we-include-custom-images-in-private-azure-marketplace"></a><span data-ttu-id="138b8-244">¿Podemos incluir imágenes personalizadas en Azure Marketplace privado?</span><span class="sxs-lookup"><span data-stu-id="138b8-244">Can we include custom images in Private Azure Marketplace?</span></span>

<span data-ttu-id="138b8-245">No.</span><span class="sxs-lookup"><span data-stu-id="138b8-245">No.</span></span> <span data-ttu-id="138b8-246">Azure Marketplace privado permite que cualquier administrador de TI administre y ajustar soluciones de terceros de Azure Marketplace global.</span><span class="sxs-lookup"><span data-stu-id="138b8-246">Private Azure Marketplace allows any IT administrator to manage and curate third-party solutions from global Azure Marketplace.</span></span> <span data-ttu-id="138b8-247">Dado que las imágenes personalizadas no se encuentran en Azure Marketplace global, el administrador de ti no puede escoger y elegir sus imágenes personalizadas.</span><span class="sxs-lookup"><span data-stu-id="138b8-247">Since custom images are not on global Azure Marketplace, the IT administrator cannot pick and choose your custom images.</span></span> <span data-ttu-id="138b8-248">Si desea compartir imágenes personalizadas, use la galería de [imágenes compartidas](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).</span><span class="sxs-lookup"><span data-stu-id="138b8-248">If you would like to share custom images, use [Shared Image Gallery](https://docs.microsoft.com/azure/virtual-machines/shared-image-galleries).</span></span>

1. <span data-ttu-id="138b8-249">Guía paso a paso: creación de una galería de imágenes compartidas (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).</span><span class="sxs-lookup"><span data-stu-id="138b8-249">Step-by-step guide Create a Shared Image Gallery (SIG) ([CLI](https://docs.microsoft.com/azure/virtual-machines/shared-images-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/shared-images-powershell)).</span></span>
2. <span data-ttu-id="138b8-250">Cree una definición de imagen dentro de un SIG.</span><span class="sxs-lookup"><span data-stu-id="138b8-250">Create an image definition within a SIG.</span></span> <span data-ttu-id="138b8-251">El cliente debe elegir **generalizado** para el campo de estado de so.</span><span class="sxs-lookup"><span data-stu-id="138b8-251">Customer should choose **Generalized** for the OS-state field.</span></span> <span data-ttu-id="138b8-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span><span class="sxs-lookup"><span data-stu-id="138b8-252">([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli#create-an-image-definition), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-vm-powershell#create-an-image-definition)).</span></span>
3. <span data-ttu-id="138b8-253">Incorpore la imagen administrada a la galería de imágenes compartidas ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).</span><span class="sxs-lookup"><span data-stu-id="138b8-253">Bring managed image into the Shared Image Gallery ([CLI](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-cli), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/image-version-managed-image-powershell)).</span></span>
4. <span data-ttu-id="138b8-254">Las imágenes de máquina virtual de SIG residirían en una suscripción.</span><span class="sxs-lookup"><span data-stu-id="138b8-254">The SIG VM images would reside in one subscription.</span></span> <span data-ttu-id="138b8-255">Para que esté disponible para otras suscripciones, use un registro de aplicaciones ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).</span><span class="sxs-lookup"><span data-stu-id="138b8-255">To make it available to other subscriptions, use an app registration ([CLI](https://docs.microsoft.com/azure/virtual-machines/linux/share-images-across-tenants), [PowerShell](https://docs.microsoft.com/azure/virtual-machines/windows/share-images-across-tenants)).</span></span>

#### <a name="why-do-i-see-some-offers-approved-by-default-even-though-the-publisher-is-not-microsoft"></a><span data-ttu-id="138b8-256">¿Por qué veo algunas ofertas **aprobadas de forma predeterminada,** aunque el publicador no es Microsoft?</span><span class="sxs-lookup"><span data-stu-id="138b8-256">Why do I see some offers **Approved by default** even though the publisher is not Microsoft?</span></span>

<span data-ttu-id="138b8-257">Microsoft es compatible con Linux y tecnología de código abierto en Azure.</span><span class="sxs-lookup"><span data-stu-id="138b8-257">Microsoft supports Linux and open-source technology in Azure.</span></span> <span data-ttu-id="138b8-258">Las [distribuciones de Linux aprobadas](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) se admiten en Azure y el precio se integra en las máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="138b8-258">[Endorsed Linux distributions](https://docs.microsoft.com/azure/virtual-machines/linux/endorsed-distros) are supported on Azure and the price is integrated in virtual machines.</span></span> <span data-ttu-id="138b8-259">Dado que el agente de Linux de Azure ya está instalado en Azure Marketplace, se trata como una oferta de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="138b8-259">Because Azure Linux Agent is already pre-installed on Azure Marketplace, it is treated like a Microsoft offer.</span></span> <span data-ttu-id="138b8-260">Como las ofertas de Microsoft están aprobadas de forma predeterminada, las distribuciones de Linux aprobadas no se pueden administrar en Azure Marketplace privado y están aprobadas de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="138b8-260">Since Microsoft offers are approved by default, endorsed Linux distributions cannot be managed in Private Azure Marketplace and are approved by default.</span></span>

## <a name="contact-support"></a><span data-ttu-id="138b8-261">Ponerse en contacto con soporte técnico</span><span class="sxs-lookup"><span data-stu-id="138b8-261">Contact support</span></span>

- <span data-ttu-id="138b8-262">Para obtener soporte técnico de Azure Marketplace, visite [Microsoft Q&A](/answers/products/).</span><span class="sxs-lookup"><span data-stu-id="138b8-262">For Azure Marketplace support, visit [Microsoft Q&A](/answers/products/).</span></span>
