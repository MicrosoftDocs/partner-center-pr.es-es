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
ms.openlocfilehash: f536d975d3c644a7afa29a95a3cb45608f6b2c9f
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315854"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="56051-103">Restablecer los privilegios de administrador para las suscripciones de del programa CSP de Azure de un cliente</span><span class="sxs-lookup"><span data-stu-id="56051-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="56051-104">**Roles aplicables**</span><span class="sxs-lookup"><span data-stu-id="56051-104">**Applicable roles**</span></span>

- <span data-ttu-id="56051-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="56051-105">Global admin</span></span>
- <span data-ttu-id="56051-106">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="56051-106">Admin agent</span></span>

<span data-ttu-id="56051-107">Como partner de CSP, tus clientes suelen esperar que administres el uso que hacen de Azure y sus sistemas por ellos.</span><span class="sxs-lookup"><span data-stu-id="56051-107">As a CSP partner your customers often expect that you will manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="56051-108">Para ello, es necesario tener privilegios de administrador.</span><span class="sxs-lookup"><span data-stu-id="56051-108">Doing so requires you to have admin privileges.</span></span> <span data-ttu-id="56051-109">Algunos privilegios se conceden cuando se establece la relación de revendedor con el cliente.</span><span class="sxs-lookup"><span data-stu-id="56051-109">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="56051-110">El cliente te concede otros privilegios.</span><span class="sxs-lookup"><span data-stu-id="56051-110">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="56051-111">Privilegios de administrador para Azure en CSP</span><span class="sxs-lookup"><span data-stu-id="56051-111">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="56051-112">Hay dos niveles de privilegios de administrador para Azure en CSP.</span><span class="sxs-lookup"><span data-stu-id="56051-112">There are two levels of admin privileges for Azure in CSP.</span></span>

<span data-ttu-id="56051-113">**Privilegios de administrador de nivel de inquilino** (**privilegios de administrador delegado**): los partners de CSP obtienen estos privilegios al establecer una relación de revendedor de CSP con los clientes.</span><span class="sxs-lookup"><span data-stu-id="56051-113">**Tenant level admin privileges** (**Delegated admin privileges**) -  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="56051-114">Los privilegios de administrador delegado proporcionan a los asociados de CSP acceso a los inquilinos de sus clientes, lo que les permite desarrollar funciones administrativas, como agregar o administrar usuarios, restablecer contraseñas y administrar licencias de usuario.</span><span class="sxs-lookup"><span data-stu-id="56051-114">Delegated admin privileges gives CSP partners access to their customers' tenants, which allows them to perform administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>

<span data-ttu-id="56051-115">**Privilegios de administrador de nivel de suscripción**: los partners de CSP obtienen estos privilegios al crear suscripciones de Azure CSP para sus clientes.</span><span class="sxs-lookup"><span data-stu-id="56051-115">**Subscription level admin privileges** - CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="56051-116">Estos privilegios proporcionan a los partners de CSP acceso completo a estas suscripciones, lo que les permite aprovisionar y administrar los recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="56051-116">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-partners-admin-privileges"></a><span data-ttu-id="56051-117">Restablecer los privilegios de administrador de los partners de CSP</span><span class="sxs-lookup"><span data-stu-id="56051-117">Reinstate CSP partners' admin privileges</span></span>

<span data-ttu-id="56051-118">El cliente puede volver a crear la asignación de roles de CSP siempre que se le proporcione el identificador de objeto del grupo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="56051-118">Your customer is able to re-create the CSP role assignment as long as you provide the object ID of the AdminAgents group to your customer.</span></span> <span data-ttu-id="56051-119">Para recuperar los privilegios de administrador delegado, debes trabajar con el cliente.</span><span class="sxs-lookup"><span data-stu-id="56051-119">To regain delegated admin privileges, you need to work with your customer.</span></span>

1. <span data-ttu-id="56051-120">Inicie sesión en el panel del Centro de partners y, en el menú del Centro de partners, selecciona **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="56051-120">Sign into the Partner Center dashboard and from the Partner Center menu, select **Customers**.</span></span>

2. <span data-ttu-id="56051-121">Selecciona el cliente con el que estás trabajando y **solicita una relación de revendedor.**</span><span class="sxs-lookup"><span data-stu-id="56051-121">Select the customer you are working with and **request a reseller relationship.**</span></span> <span data-ttu-id="56051-122">Esta acción genera un vínculo para el cliente que tiene derechos de administrador de inquilinos.</span><span class="sxs-lookup"><span data-stu-id="56051-122">This generates a link to the customer who has tenant admin rights.</span></span>

3. <span data-ttu-id="56051-123">El cliente debe seleccionar el vínculo y aprobar la solicitud de relación del revendedor.</span><span class="sxs-lookup"><span data-stu-id="56051-123">That customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Ejemplo de correo electrónico de creación de una relación de revendedor":::

4. <span data-ttu-id="56051-125">El asociado, debe conectarse al inquilino del asociado para obtener el identificador de objeto del grupo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="56051-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. <span data-ttu-id="56051-126">El cliente que tiene el rol de **propietario o administrador de acceso de usuarios** y tiene permiso para crear la asignación de roles en el nivel de suscripción hace lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="56051-126">Your customer who has the role of **owner or user access administrator** and has permission to create role assignment at the subscription level does the following:</span></span>


    1. <span data-ttu-id="56051-127">Se conecta al inquilino donde existe la suscripción de CSP.</span><span class="sxs-lookup"><span data-stu-id="56051-127">Connects to the tenant where the CSP subscription exists.</span></span>
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. <span data-ttu-id="56051-128">Se conecta a la suscripción (solo es aplicable si el usuario tiene permisos de asignación de roles en varias suscripciones del inquilino).</span><span class="sxs-lookup"><span data-stu-id="56051-128">Connects to the subscription (only applicable if the user has role assignment permissions over multiple subscriptions in the tenant).</span></span>
   
         <span data-ttu-id="56051-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"</span><span class="sxs-lookup"><span data-stu-id="56051-129">PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"\`</span></span>


    3. <span data-ttu-id="56051-130">Crea la asignación de roles.</span><span class="sxs-lookup"><span data-stu-id="56051-130">Creates the role assignment</span></span>
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


<span data-ttu-id="56051-131">Si se desea conceder permiso de rol de propietario en el nivel de grupo de recursos o en el nivel de recurso en lugar del ámbito de la suscripción, pueden funcionar los siguientes comandos:</span><span class="sxs-lookup"><span data-stu-id="56051-131">If the desire is to grant owner role permission at resource group level or resource level instead of subscription scope, the following commands can work:</span></span>


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a><span data-ttu-id="56051-132">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="56051-132">Next steps</span></span>

- [<span data-ttu-id="56051-133">Administrar suscripciones y recursos en el plan de Azure</span><span class="sxs-lookup"><span data-stu-id="56051-133">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
