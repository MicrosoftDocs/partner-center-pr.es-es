---
title: Agregar inquilinos a la cuenta del centro de Partners
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información acerca de cómo agregar, consolidar o administrar varios inquilinos de Azure AD en la cuenta del centro de Partners y obtener información sobre por qué podría querer hacerlo.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124812"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="231d2-103">Adición y administración de varios inquilinos en la cuenta del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="231d2-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="231d2-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="231d2-104">**Appropriate roles**</span></span>

- <span data-ttu-id="231d2-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="231d2-105">Global admin</span></span>
- <span data-ttu-id="231d2-106">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="231d2-106">Account admin</span></span>

<span data-ttu-id="231d2-107">En este artículo se describe cómo consolidar varios inquilinos de Azure Active Directory (Azure AD) para su empresa y, a continuación, agregarlos y administrarlos en su cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="231d2-107">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="231d2-108">Hay muchas razones para hacerlo.</span><span class="sxs-lookup"><span data-stu-id="231d2-108">There are many reasons to do so.</span></span> <span data-ttu-id="231d2-109">Por ejemplo:</span><span class="sxs-lookup"><span data-stu-id="231d2-109">For example:</span></span>

- <span data-ttu-id="231d2-110">Supongamos que su empresa, Contoso, ha adquirido otra empresa, fabrikam.</span><span class="sxs-lookup"><span data-stu-id="231d2-110">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="231d2-111">Quiere que las dos compañías sigan siendo independientes, pero desea que los nuevos empleados puedan usar el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="231d2-111">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="231d2-112">En este caso, asociará el inquilino de Azure AD de la compañía a su cuenta global de socio comercial (PGA).</span><span class="sxs-lookup"><span data-stu-id="231d2-112">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="231d2-113">Esta asociación permite a los usuarios de ambas empresas trabajar en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="231d2-113">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="231d2-114">Si ejecuta su empresa con más de un inquilino (por ejemplo, *contoso.com*, *contoso.uk* y *contoso.in*), puede usar la multiempresa para agruparlos en la misma cuenta de equipo.</span><span class="sxs-lookup"><span data-stu-id="231d2-114">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="231d2-115">Si los mezcladores y las directrices de adquisiciones requieren que trabaje con los inquilinos de ambas empresas, usaría los inquilinos *constoso.com* y *fabrikam.com* .</span><span class="sxs-lookup"><span data-stu-id="231d2-115">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="231d2-116">Los usuarios de cualquiera de los inquilinos deben poder:</span><span class="sxs-lookup"><span data-stu-id="231d2-116">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="231d2-117">Obtenga acceso al centro de partners para cursos, descargas digitales o asociación de Microsoft Certified Professional (MCP).</span><span class="sxs-lookup"><span data-stu-id="231d2-117">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="231d2-118">Debe tener asignados roles del centro de partners como el administrador de Microsoft Partner Network (MPN) o el administrador de incentivos.</span><span class="sxs-lookup"><span data-stu-id="231d2-118">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="231d2-119">Adición de un inquilino de Azure AD a su cuenta</span><span class="sxs-lookup"><span data-stu-id="231d2-119">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="231d2-120">Inicie sesión como administrador global en el [centro de Partners de Microsoft](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="231d2-120">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="231d2-121">En la esquina superior derecha, seleccione **configuración**, seleccione Configuración de la **cuenta** y, a continuación, seleccione **inquilinos**.</span><span class="sxs-lookup"><span data-stu-id="231d2-121">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Captura de pantalla del botón asociar en el panel Perfil de Azure AD."::: 

1. <span data-ttu-id="231d2-123">Seleccione **asociar** y, a continuación, indique el inquilino que desea asociar.</span><span class="sxs-lookup"><span data-stu-id="231d2-123">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="231d2-124">En el símbolo del sistema, inicie sesión como administrador global en el inquilino que desee asociar y, a continuación, seleccione **confirmar**.</span><span class="sxs-lookup"><span data-stu-id="231d2-124">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Captura de pantalla del botón confirmar en el panel confirmar nueva asociación de Azure AD."::: 

   <span data-ttu-id="231d2-126">Una vez confirmada la asociación, se muestra un mensaje **todo establecido** .</span><span class="sxs-lookup"><span data-stu-id="231d2-126">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="231d2-127">Para ver el inquilino recién agregado, seleccione **volver a administración de inquilinos**.</span><span class="sxs-lookup"><span data-stu-id="231d2-127">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="231d2-128">No se puede asociar un inquilino con una cuenta si ya está asociado a otra cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="231d2-128">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="231d2-129">Quitar un inquilino de su cuenta</span><span class="sxs-lookup"><span data-stu-id="231d2-129">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="231d2-130">Inicie sesión como administrador global en el [centro de Partners de Microsoft](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="231d2-130">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="231d2-131">En la esquina superior derecha, seleccione el icono de **configuración** y, a continuación, seleccione Configuración de la **cuenta**.</span><span class="sxs-lookup"><span data-stu-id="231d2-131">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="231d2-132">En el panel izquierdo, seleccione **inquilinos**.</span><span class="sxs-lookup"><span data-stu-id="231d2-132">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="231d2-133">En **administrar inquilinos de Azure ad**, seleccione la pestaña **socio comercial** .</span><span class="sxs-lookup"><span data-stu-id="231d2-133">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="231d2-134">Seleccione **quitar** junto al inquilino cuya asociación desea quitar.</span><span class="sxs-lookup"><span data-stu-id="231d2-134">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Captura de pantalla de las asociaciones de inquilino actuales y sus vínculos de eliminación.":::

   <span data-ttu-id="231d2-136">Como se muestra en la captura de pantalla anterior, los vínculos de **eliminación** están habilitados para todos los inquilinos asociados, excepto para el inquilino principal y el inquilino en el que está conectado actualmente.</span><span class="sxs-lookup"><span data-stu-id="231d2-136">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="231d2-137">Cuando se quita un inquilino, los usuarios de ese inquilino ya no tienen acceso a la cuenta del centro de Partners y la eliminación puede afectar a sus competencias.</span><span class="sxs-lookup"><span data-stu-id="231d2-137">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="231d2-138">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="231d2-138">Next steps</span></span>

- [<span data-ttu-id="231d2-139">Crear cuentas de usuario</span><span class="sxs-lookup"><span data-stu-id="231d2-139">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






