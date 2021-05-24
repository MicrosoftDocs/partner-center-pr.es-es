---
title: Restablecer los privilegios de administrador del programa CSP de Azure
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo ayudar a los clientes a restablecer los privilegios de administrador de un partner para que pueda ayudar a administrar las suscripciones del programa CSP de Azure de un cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ad29283001ec542944da4f0cac835c6a5d339251
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855427"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="25aa6-103">Restablecer los privilegios de administrador para las suscripciones de del programa CSP de Azure de un cliente</span><span class="sxs-lookup"><span data-stu-id="25aa6-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="25aa6-104">**Roles adecuados**: Administrador global | Agente de administración</span><span class="sxs-lookup"><span data-stu-id="25aa6-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="25aa6-105">Como partner de CSP, tus clientes suelen esperar que administres el uso que hacen de Azure y sus sistemas por ellos.</span><span class="sxs-lookup"><span data-stu-id="25aa6-105">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="25aa6-106">Para ello, es necesario tener privilegios de administrador.</span><span class="sxs-lookup"><span data-stu-id="25aa6-106">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="25aa6-107">Algunos privilegios se conceden cuando se establece la relación de revendedor con el cliente.</span><span class="sxs-lookup"><span data-stu-id="25aa6-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="25aa6-108">El cliente te concede otros privilegios.</span><span class="sxs-lookup"><span data-stu-id="25aa6-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="25aa6-109">Privilegios de administrador para Azure en CSP</span><span class="sxs-lookup"><span data-stu-id="25aa6-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="25aa6-110">Hay dos niveles de privilegios de administrador para Azure en CSP.</span><span class="sxs-lookup"><span data-stu-id="25aa6-110">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="25aa6-111">**Privilegios de administrador de nivel de inquilino** (**privilegios de administrador delegado**): los partners de CSP obtienen estos privilegios al establecer una relación de revendedor de CSP con los clientes.</span><span class="sxs-lookup"><span data-stu-id="25aa6-111">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="25aa6-112">Los privilegios de administrador delegado proporcionan a los partners de CSP acceso a los inquilinos de sus clientes, lo que les permite desarrollar funciones administrativas, como agregar o administrar usuarios, restablecer contraseñas y administrar licencias de usuario.</span><span class="sxs-lookup"><span data-stu-id="25aa6-112">Delegated admin privileges give CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="25aa6-113">**Privilegios de administrador de nivel de suscripción**: los partners de CSP obtienen estos privilegios al crear suscripciones de Azure CSP para sus clientes.</span><span class="sxs-lookup"><span data-stu-id="25aa6-113">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="25aa6-114">Estos privilegios proporcionan a los partners de CSP acceso completo a estas suscripciones, lo que les permite aprovisionar y administrar los recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="25aa6-114">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="25aa6-115">Restablecer los privilegios de administrador de los partners de CSP</span><span class="sxs-lookup"><span data-stu-id="25aa6-115">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="25aa6-116">El cliente puede volver a crear la asignación de roles de CSP siempre que se le proporcione el identificador de objeto del grupo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="25aa6-116">Your customer can re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="25aa6-117">Para recuperar los privilegios de administrador delegado, debes trabajar con el cliente.</span><span class="sxs-lookup"><span data-stu-id="25aa6-117">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="25aa6-118">Inicie sesión en el panel del Centro de partners y, en el menú del Centro de partners, selecciona **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="25aa6-118">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="25aa6-119">Selecciona el cliente con el que estás trabajando y **solicita una relación de revendedor.**</span><span class="sxs-lookup"><span data-stu-id="25aa6-119">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="25aa6-120">Esta acción genera un vínculo para el cliente que tiene derechos de administrador de inquilinos.</span><span class="sxs-lookup"><span data-stu-id="25aa6-120">This action generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="25aa6-121">El cliente debe seleccionar el vínculo y aprobar la solicitud de relación del revendedor.</span><span class="sxs-lookup"><span data-stu-id="25aa6-121">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Ejemplo de correo electrónico de creación de una relación de revendedor":::

4. <span data-ttu-id="25aa6-123">El asociado, debe conectarse al inquilino del asociado para obtener el identificador de objeto del grupo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="25aa6-123">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="25aa6-124">El cliente que tiene el rol de **propietario o administrador de acceso de usuarios** y tiene permiso para crear la asignación de roles en el nivel de suscripción hace lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="25aa6-124">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="25aa6-125">Se conecta al inquilino donde existe la suscripción de CSP.</span><span class="sxs-lookup"><span data-stu-id="25aa6-125">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="25aa6-126">Se conecta a la suscripción (solo es aplicable si el usuario tiene permisos de asignación de roles en varias suscripciones del inquilino).</span><span class="sxs-lookup"><span data-stu-id="25aa6-126">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="25aa6-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"</span><span class="sxs-lookup"><span data-stu-id="25aa6-127">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="25aa6-128">Crea la asignación de roles.</span><span class="sxs-lookup"><span data-stu-id="25aa6-128">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="25aa6-129">Si quiere conceder el permiso de rol de propietario a nivel del grupo de recursos o a nivel del recurso en lugar del ámbito de la suscripción, pueden funcionar los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="25aa6-129">If you want to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="25aa6-130">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="25aa6-130">Next steps</span></span>

- [<span data-ttu-id="25aa6-131">Administrar suscripciones y recursos en el plan de Azure</span><span class="sxs-lookup"><span data-stu-id="25aa6-131">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
