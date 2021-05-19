---
title: Agregar inquilinos a la cuenta Centro de partners cliente
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo agregar, consolidar o administrar varios inquilinos de Azure AD en su cuenta de Centro de partners y saber por qué podría querer hacerlo.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151209"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="7d579-103">Adición y administración de varios inquilinos en la Centro de partners cuenta</span><span class="sxs-lookup"><span data-stu-id="7d579-103">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="7d579-104">**Roles adecuados:** administrador global | Administrador de cuenta</span><span class="sxs-lookup"><span data-stu-id="7d579-104">**Appropriate roles**: Global admin | Account admin</span></span>

<span data-ttu-id="7d579-105">En este artículo se describe cómo consolidar varios inquilinos de Azure Active Directory (Azure AD) para su empresa y, a continuación, agregarlos y administrarlos en su cuenta Centro de partners cliente.</span><span class="sxs-lookup"><span data-stu-id="7d579-105">This article discusses how to consolidate multiple Azure Active Directory (Azure AD) tenants for your company and then add and manage them in your Partner Center account.</span></span> <span data-ttu-id="7d579-106">Hay muchas razones para hacerlo.</span><span class="sxs-lookup"><span data-stu-id="7d579-106">There are many reasons to do so.</span></span> <span data-ttu-id="7d579-107">Por ejemplo:</span><span class="sxs-lookup"><span data-stu-id="7d579-107">For example:</span></span>

- <span data-ttu-id="7d579-108">Supongamos que su empresa, Contoso, ha adquirido otra empresa, Fabrikam.</span><span class="sxs-lookup"><span data-stu-id="7d579-108">Let's say your company, Contoso, has acquired another company, Fabrikam.</span></span> <span data-ttu-id="7d579-109">Quiere que las dos empresas permanezcan independientes, pero quiere que los nuevos empleados puedan usar Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="7d579-109">You want the two companies to remain separate, but you want the new employees to be able to use Partner Center.</span></span> <span data-ttu-id="7d579-110">En este caso, asociará el nuevo inquilino de Azure AD a su cuenta global de asociado (PGA).</span><span class="sxs-lookup"><span data-stu-id="7d579-110">In this case, you associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="7d579-111">Esta asociación permite a los usuarios de ambas empresas trabajar en Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="7d579-111">This association enables users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="7d579-112">Si ejecuta su negocio con más de un inquilino (por ejemplo, *contoso.com*, *contoso.uk* y *contoso.in*), puede usar multiinquilino para agruparlos en la misma cuenta de equipo.</span><span class="sxs-lookup"><span data-stu-id="7d579-112">If you run your business with more than one tenant (for example, *contoso.com*, *contoso.uk*, and *contoso.in*), you can use multitenancy to group them in the same PC account.</span></span>

- <span data-ttu-id="7d579-113">Si las directrices de fusiones y adquisiciones requieren que trabaje  con inquilinos de ambas compañías, usaría los inquilinos constoso.com y *fabrikam.com* inquilinos.</span><span class="sxs-lookup"><span data-stu-id="7d579-113">If mergers and acquisitions guidelines require you to work with tenants of both companies, you would use both the *constoso.com* and *fabrikam.com* tenants.</span></span>

- <span data-ttu-id="7d579-114">Los usuarios de cualquiera de los inquilinos deben poder:</span><span class="sxs-lookup"><span data-stu-id="7d579-114">Users of any of the tenants need to be able to:</span></span>
    * <span data-ttu-id="7d579-115">Acceso Centro de partners para entrenamiento, descargas digitales o asociación de Microsoft Certified Professional (MCP).</span><span class="sxs-lookup"><span data-stu-id="7d579-115">Access Partner Center for training, digital downloads, or Microsoft Certified Professional (MCP) association.</span></span>
    * <span data-ttu-id="7d579-116">Se le Centro de partners roles como administrador de Microsoft Partner Network (MPN) o administrador de incentivos.</span><span class="sxs-lookup"><span data-stu-id="7d579-116">Be assigned Partner Center roles such as Microsoft Partner Network (MPN) admin or incentives admin.</span></span>

## <a name="add-an-azure-ad-tenant-to-your-account"></a><span data-ttu-id="7d579-117">Adición de Azure AD inquilino a la cuenta</span><span class="sxs-lookup"><span data-stu-id="7d579-117">Add an Azure AD tenant to your account</span></span>

1. <span data-ttu-id="7d579-118">Inicie sesión como administrador global en [Microsoft Centro de partners](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="7d579-118">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="7d579-119">En la esquina superior derecha, seleccione **Configuración,** **Configuración de la cuenta** **y, después, Inquilinos.**</span><span class="sxs-lookup"><span data-stu-id="7d579-119">At the upper right, select **Settings**, select **Account settings**, and then select **Tenants**.</span></span>
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Captura de pantalla del botón Asociar del panel Azure AD perfil."::: 

1. <span data-ttu-id="7d579-121">Seleccione **Asociar** y, a continuación, indique el inquilino que desea asociar.</span><span class="sxs-lookup"><span data-stu-id="7d579-121">Select **Associate**, and then indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="7d579-122">En el símbolo del sistema, inicie sesión como administrador global en el inquilino que desea asociar y, a continuación, **seleccione Confirmar**.</span><span class="sxs-lookup"><span data-stu-id="7d579-122">At the prompt, sign in as global admin to the tenant you want to associate, and then select **Confirm**.</span></span> 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Captura de pantalla del botón Confirmar en el panel Confirmar Azure AD asociación."::: 

   <span data-ttu-id="7d579-124">Después de confirmar la asociación, se muestra **un mensaje** All set (Todo el conjunto).</span><span class="sxs-lookup"><span data-stu-id="7d579-124">After you've confirmed the association, an **All set** message is displayed.</span></span> <span data-ttu-id="7d579-125">Para ver el inquilino recién agregado, seleccione **Volver a la administración de inquilinos.**</span><span class="sxs-lookup"><span data-stu-id="7d579-125">To view the newly added tenant, select **Return to tenant management**.</span></span> 
 
>[!NOTE]
><span data-ttu-id="7d579-126">No se puede asociar un inquilino a una cuenta si ya está asociada a otra cuenta Centro de partners cuenta.</span><span class="sxs-lookup"><span data-stu-id="7d579-126">You can't associate a tenant with an account if it's already associated with another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="7d579-127">Eliminación de un inquilino de la cuenta</span><span class="sxs-lookup"><span data-stu-id="7d579-127">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="7d579-128">Inicie sesión como administrador global en [Microsoft Centro de partners](https://partner.microsoft.com/dashboard).</span><span class="sxs-lookup"><span data-stu-id="7d579-128">Sign in as global admin to [Microsoft Partner Center](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="7d579-129">En la esquina superior derecha, seleccione el **icono Configuración** y, a continuación, seleccione Configuración de **la cuenta.**</span><span class="sxs-lookup"><span data-stu-id="7d579-129">At the upper right, select the **Settings** icon, and then select **Account settings**.</span></span>

1. <span data-ttu-id="7d579-130">En el panel izquierdo, seleccione **Inquilinos.**</span><span class="sxs-lookup"><span data-stu-id="7d579-130">On the left pane, select **Tenants**.</span></span> <span data-ttu-id="7d579-131">En **Administrar Azure AD inquilinos,** seleccione la pestaña Partner **(Asociado).**</span><span class="sxs-lookup"><span data-stu-id="7d579-131">Under **Manage Azure AD tenants**, select the **Partner** tab.</span></span>
 
1. <span data-ttu-id="7d579-132">Seleccione **Quitar** junto al inquilino cuya asociación desea quitar.</span><span class="sxs-lookup"><span data-stu-id="7d579-132">Select **Remove** next to the tenant whose association you want to remove.</span></span>

   :::image type="content" source="images/disassociate.png" alt-text="Captura de pantalla de las asociaciones de inquilino actuales y sus vínculos Quitar.":::

   <span data-ttu-id="7d579-134">Como se muestra en la  captura de pantalla anterior, los vínculos Quitar están habilitados para todos los inquilinos asociados, excepto para el inquilino principal y el inquilino en el que ha iniciado sesión actualmente.</span><span class="sxs-lookup"><span data-stu-id="7d579-134">As shown in the preceding screenshot, the **Remove** links are enabled for all associated tenants, except for the primary tenant and the tenant that you're currently signed in to.</span></span> 

   > [!NOTE]   
   > <span data-ttu-id="7d579-135">Cuando se quita un inquilino, los usuarios de ese inquilino ya no tienen acceso a la cuenta de Centro de partners y la eliminación puede afectar a sus competencias.</span><span class="sxs-lookup"><span data-stu-id="7d579-135">When you remove a tenant, the users on that tenant no longer have access to the Partner Center account, and the removal might have an impact on your competencies.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="7d579-136">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="7d579-136">Next steps</span></span>

- [<span data-ttu-id="7d579-137">Crear cuentas de usuario</span><span class="sxs-lookup"><span data-stu-id="7d579-137">Create user accounts</span></span>](create-user-accounts-and-set-permissions.md)






