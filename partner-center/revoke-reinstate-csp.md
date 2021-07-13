---
title: Restablecer los privilegios de administrador del programa CSP de Azure
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo ayudar a los clientes a restablecer los privilegios de administrador de un partner para que pueda ayudar a administrar las suscripciones del programa Proveedor de soluciones en la nube (CSP) de Azure de un cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 196b38d30942278beb00096529f5965db7dfb96c
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510183"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="33448-103">Restablecer los privilegios de administrador para las suscripciones de del programa CSP de Azure de un cliente</span><span class="sxs-lookup"><span data-stu-id="33448-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="33448-104">**Roles adecuados**: Administrador global | Agente de administración</span><span class="sxs-lookup"><span data-stu-id="33448-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="33448-105">Como partner del programa Proveedor de soluciones en la nube (CSP), sus clientes suelen esperar que administre el uso que hacen de Azure y sus sistemas por ellos.</span><span class="sxs-lookup"><span data-stu-id="33448-105">As a Cloud Solution Provider (CSP) partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="33448-106">Debe tener privilegios de administrador para hacerlo.</span><span class="sxs-lookup"><span data-stu-id="33448-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="33448-107">Algunos privilegios se conceden cuando se establece la relación de revendedor con el cliente.</span><span class="sxs-lookup"><span data-stu-id="33448-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="33448-108">El cliente te concede otros privilegios.</span><span class="sxs-lookup"><span data-stu-id="33448-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="33448-109">Privilegios de administrador para Azure en CSP</span><span class="sxs-lookup"><span data-stu-id="33448-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="33448-110">Hay dos niveles de privilegios de administrador para Azure en CSP.</span><span class="sxs-lookup"><span data-stu-id="33448-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="33448-111">**Privilegios de administrador de nivel de inquilino (privilegios de administrador delegado)** : los partners de CSP obtienen estos privilegios al establecer una relación de revendedor de CSP con los clientes.</span><span class="sxs-lookup"><span data-stu-id="33448-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="33448-112">Los privilegios de administrador delegados proporcionan a los partners de CSP acceso a los inquilinos de sus clientes.</span><span class="sxs-lookup"><span data-stu-id="33448-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="33448-113">Este acceso les permite realizar funciones administrativas, como agregar o administrar usuarios, restablecer contraseñas y administrar licencias de usuario.</span><span class="sxs-lookup"><span data-stu-id="33448-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="33448-114">**Privilegios de administrador de nivel de suscripción**: los partners de CSP obtienen estos privilegios al crear suscripciones de CSP de Azure para sus clientes.</span><span class="sxs-lookup"><span data-stu-id="33448-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="33448-115">Estos privilegios proporcionan a los partners de CSP acceso completo a estas suscripciones, lo que les permite aprovisionar y administrar los recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="33448-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="33448-116">Restablecer los privilegios de administrador de un partner en CSP</span><span class="sxs-lookup"><span data-stu-id="33448-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="33448-117">El cliente puede volver a crear la asignación de roles de CSP siempre que se le proporcione el identificador `object ID` del grupo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="33448-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="33448-118">Para recuperar los privilegios de administrador delegado, debe trabajar con el cliente y completar los pasos que se indican a continuación.</span><span class="sxs-lookup"><span data-stu-id="33448-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="33448-119">Inicia sesión en el panel del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="33448-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="33448-120">En el menú del Centro de partners, seleccione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="33448-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="33448-121">Seleccione el cliente con el que está trabajando y **solicite una relación de revendedor**.</span><span class="sxs-lookup"><span data-stu-id="33448-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="33448-122">Esta acción genera un vínculo para el cliente que tiene derechos de administrador de inquilinos.</span><span class="sxs-lookup"><span data-stu-id="33448-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="33448-123">El cliente debe seleccionar el vínculo y aprobar la solicitud de relación de revendedor.</span><span class="sxs-lookup"><span data-stu-id="33448-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Ejemplo de correo electrónico de creación de una relación de revendedor.":::

5. <span data-ttu-id="33448-125">El asociado, debe conectarse al inquilino del asociado para obtener el identificador de objeto del grupo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="33448-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="33448-126">A continuación, el cliente debe realizar los pasos siguientes mediante PowerShell o la CLI de Azure.</span><span class="sxs-lookup"><span data-stu-id="33448-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="33448-127">El cliente debe tener lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="33448-127">Your customer must have:</span></span>

- <span data-ttu-id="33448-128">El rol de **propietario** o **administrador de acceso de usuario**.</span><span class="sxs-lookup"><span data-stu-id="33448-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="33448-129">Permisos para crear asignaciones de roles en el nivel de suscripción.</span><span class="sxs-lookup"><span data-stu-id="33448-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="33448-130">a.</span><span class="sxs-lookup"><span data-stu-id="33448-130">a.</span></span> <span data-ttu-id="33448-131">Solo para PowerShell, el cliente debe actualizar el módulo `Az.Resources`.</span><span class="sxs-lookup"><span data-stu-id="33448-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="33448-132">b.</span><span class="sxs-lookup"><span data-stu-id="33448-132">b.</span></span> <span data-ttu-id="33448-133">El cliente se conecta al inquilino donde existe la suscripción de CSP.</span><span class="sxs-lookup"><span data-stu-id="33448-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="33448-134">c.</span><span class="sxs-lookup"><span data-stu-id="33448-134">c.</span></span> <span data-ttu-id="33448-135">El cliente se conecta a la suscripción.</span><span class="sxs-lookup"><span data-stu-id="33448-135">The customer connects to the subscription.</span></span> <span data-ttu-id="33448-136">Este paso *solo* es aplicable si el usuario tiene permisos de asignación de roles en varias suscripciones del inquilino.</span><span class="sxs-lookup"><span data-stu-id="33448-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="33448-137">d.</span><span class="sxs-lookup"><span data-stu-id="33448-137">d.</span></span> <span data-ttu-id="33448-138">A continuación, el cliente crea la asignación de roles.</span><span class="sxs-lookup"><span data-stu-id="33448-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="33448-139">En lugar de conceder permisos de propietario en el ámbito de la suscripción, puede concederlos en el nivel de recurso o de grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="33448-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="33448-140">En el nivel de grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="33448-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="33448-141">En el nivel de recurso</span><span class="sxs-lookup"><span data-stu-id="33448-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

<span data-ttu-id="33448-142">Si los pasos anteriores no funcionan o se producen errores al intentarlos, pruebe el siguiente procedimiento "comodín" para restablecer los derechos de administrador del cliente.</span><span class="sxs-lookup"><span data-stu-id="33448-142">If the above steps don't work or you get errors when attempting them, try the following "catch-all" procedure to reinstate admin rights for your customer.</span></span>

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a><span data-ttu-id="33448-143">Solución de problemas</span><span class="sxs-lookup"><span data-stu-id="33448-143">Troubleshooting</span></span>

<span data-ttu-id="33448-144">Si el cliente no puede completar el paso 6 anterior, indíquele que pruebe el siguiente comando:</span><span class="sxs-lookup"><span data-stu-id="33448-144">If the customer is unable to complete step 6 above, have the customer try the following command:</span></span>

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

<span data-ttu-id="33448-145">Proporcione el archivo `newRoleAssignment.log` resultante a Microsoft para su posterior análisis.</span><span class="sxs-lookup"><span data-stu-id="33448-145">Provide the resulting `newRoleAssignment.log` file to Microsoft for further analysis.</span></span>

<span data-ttu-id="33448-146">Si se produce un error en el procedimiento "comodín" durante la ejecución de `Import-Module`, pruebe los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="33448-146">If the "catch-all" procedure fails during the `Import-Module`, try the following steps:</span></span>
- <span data-ttu-id="33448-147">Si se produce un error en la importación porque el módulo está en uso, cierre y vuelva a abrir todas las ventanas para reiniciar la sesión de PowerShell.</span><span class="sxs-lookup"><span data-stu-id="33448-147">If the import fails because the module is in use, restart the PowerShell session by closing and reopening all windows.</span></span>
- <span data-ttu-id="33448-148">Compruebe la versión de `Az.Resources` con `Get-Module Az.Resources -ListAvailable`.</span><span class="sxs-lookup"><span data-stu-id="33448-148">Check version of `Az.Resources` with `Get-Module Az.Resources -ListAvailable`.</span></span>
- <span data-ttu-id="33448-149">Si la versión 4.1.1 no está en la lista disponible, debe usar `Update-Module Az.Resources -Force`.</span><span class="sxs-lookup"><span data-stu-id="33448-149">If version 4.1.1 is not within the available list, you must use `Update-Module Az.Resources -Force`.</span></span>
- <span data-ttu-id="33448-150">Si el error indica que `Az.Accounts` debe ser de una versión específica, actualice también ese módulo y reemplace `Az.Resources` por `Az.Accounts`.</span><span class="sxs-lookup"><span data-stu-id="33448-150">If the error states that `Az.Accounts` needs to be a specific version, update that module as well, replacing `Az.Resources` with `Az.Accounts`.</span></span> <span data-ttu-id="33448-151">A continuación, debe reiniciar la sesión de PowerShell.</span><span class="sxs-lookup"><span data-stu-id="33448-151">You must then restart the PowerShell session.</span></span>


## <a name="next-steps"></a><span data-ttu-id="33448-152">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="33448-152">Next steps</span></span>

- [<span data-ttu-id="33448-153">Administrar suscripciones y recursos en el plan de Azure</span><span class="sxs-lookup"><span data-stu-id="33448-153">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
