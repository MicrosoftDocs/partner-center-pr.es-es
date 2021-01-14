---
title: Agregar inquilinos adicionales a la cuenta del centro de Partners
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprenda a agregar, consolidar o administrar varios inquilinos de Azure AD en su cuenta del centro de Partners. Obtenga información acerca de algunas de las razones por las que podría querer hacerlo.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f9852b4e1c3997b82f744555db25fe64e1afc8ad
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182445"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="db6d1-104">Adición y administración de varios inquilinos en la cuenta del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="db6d1-104">Add and manage multiple tenants in your Partner Center account</span></span>


<span data-ttu-id="db6d1-105">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="db6d1-105">**Appropriate roles**</span></span>

- <span data-ttu-id="db6d1-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="db6d1-106">Global admin</span></span>
- <span data-ttu-id="db6d1-107">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="db6d1-107">Account admin</span></span>

<span data-ttu-id="db6d1-108">Esta característica le permite administrar varios inquilinos para su empresa y consolidarlos en su cuenta del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="db6d1-108">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="db6d1-109">Hay muchas razones por las que puede que tenga que administrar varios inquilinos de Azure AD en la cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="db6d1-109">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="db6d1-110">Por ejemplo:</span><span class="sxs-lookup"><span data-stu-id="db6d1-110">For example:</span></span>

- <span data-ttu-id="db6d1-111">Su empresa puede comprar otra empresa y quiere que los empleados de la nueva empresa puedan usar el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="db6d1-111">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="db6d1-112">Sin embargo, desea que las dos compañías sigan siendo independientes.</span><span class="sxs-lookup"><span data-stu-id="db6d1-112">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="db6d1-113">En este caso, debe asociar el inquilino de Azure AD de la compañía a su cuenta global de socio comercial (PGA).</span><span class="sxs-lookup"><span data-stu-id="db6d1-113">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="db6d1-114">Esta asociación permitiría a los usuarios de ambas empresas trabajar en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="db6d1-114">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="db6d1-115">Si tiene más de un inquilino para ejecutar su empresa (por ejemplo, contoso.com, contoso.uk, contoso.in), puede usar multiinquilino para asociarlos con la misma cuenta de equipo.</span><span class="sxs-lookup"><span data-stu-id="db6d1-115">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="db6d1-116">Las fusiones y adquisiciones requieren que trabaje con más de un inquilino (por ejemplo, si Contoso adquiere Fabrikam, deberá poder usar los inquilinos respectivos Constoso.com y Fabrikam.com).</span><span class="sxs-lookup"><span data-stu-id="db6d1-116">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="db6d1-117">Los usuarios de cualquiera de los inquilinos necesitarán poder:</span><span class="sxs-lookup"><span data-stu-id="db6d1-117">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="db6d1-118">Centro de Partners de acceso para cursos, descargas digitales, Asociación de MCP</span><span class="sxs-lookup"><span data-stu-id="db6d1-118">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="db6d1-119">Debe tener asignados roles del centro de partners como el administrador de MPN, el administrador de incentivos, etc.</span><span class="sxs-lookup"><span data-stu-id="db6d1-119">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="db6d1-120">Agregar otro inquilino de Azure AD a su cuenta</span><span class="sxs-lookup"><span data-stu-id="db6d1-120">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="db6d1-121">Como administrador global, inicie sesión en el [Panel](https://partner.microsoft.com/dashboard)del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="db6d1-121">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="db6d1-122">En el icono de **configuración** , seleccione Configuración de la **cuenta** y, a continuación, seleccione **inquilinos**.</span><span class="sxs-lookup"><span data-stu-id="db6d1-122">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="asociar inquilinos"::: 

3. <span data-ttu-id="db6d1-124">Seleccione **asociar otro inquilino de ad** e indique el inquilino que quiere asociar.</span><span class="sxs-lookup"><span data-stu-id="db6d1-124">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="db6d1-125">Como administrador global, inicie sesión en el inquilino que desee asociar y confirme la asociación.</span><span class="sxs-lookup"><span data-stu-id="db6d1-125">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="confirmar los inquilinos asociados"::: 

5. <span data-ttu-id="db6d1-127">Después de confirmar, verá una notificación de **todos los conjuntos** .</span><span class="sxs-lookup"><span data-stu-id="db6d1-127">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="db6d1-128">Seleccione **volver a administración de inquilinos** y verá el inquilino recién agregado en la lista.</span><span class="sxs-lookup"><span data-stu-id="db6d1-128">Select **Return to tenant management** and you'll see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="db6d1-129">No se puede asociar un inquilino a una cuenta si ya está asociado a otra cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="db6d1-129">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>


## <a name="remove-a-tenant-from-your-account"></a><span data-ttu-id="db6d1-130">Quitar un inquilino de su cuenta</span><span class="sxs-lookup"><span data-stu-id="db6d1-130">Remove a tenant from your account</span></span>
 
1. <span data-ttu-id="db6d1-131">Como administrador global, inicie sesión en el [Panel](https://partner.microsoft.com/dashboard)del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="db6d1-131">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

1. <span data-ttu-id="db6d1-132">En el icono de **configuración** , seleccione Configuración de la **cuenta** -> inquilinos y haga clic en la pestaña **socio comercial** .</span><span class="sxs-lookup"><span data-stu-id="db6d1-132">From the **Settings** icon, select **Account settings** -> Tenants and click on the **Partner** tab.</span></span>
 
3. <span data-ttu-id="db6d1-133">Haga clic en **quitar** para el inquilino que desea desasociar.</span><span class="sxs-lookup"><span data-stu-id="db6d1-133">Click **Remove** for the tenant you want to dissociate.</span></span>

4. <span data-ttu-id="db6d1-134">La desasociación de un inquilino significa que los usuarios de ese inquilino ya no tendrán acceso a la cuenta del centro de Partners y esto podría tener un impacto en sus competencias.</span><span class="sxs-lookup"><span data-stu-id="db6d1-134">Dissociating a tenant means that the users on that tenant will no longer have access to the Partner Center account, and this could have an impact on your competencies.</span></span> 

<span data-ttu-id="db6d1-135">El botón **quitar** está habilitado para todos los inquilinos asociados, excepto el inquilino principal y el inquilino en el que ha iniciado sesión actualmente.</span><span class="sxs-lookup"><span data-stu-id="db6d1-135">The **Remove** button is enabled for all associated tenants, except the primary tenant and the tenant which you are currently signed into.</span></span>

:::image type="content" source="images/disassociate.png" alt-text="inquilinos con el botón Quitar":::
 

## <a name="next-steps"></a><span data-ttu-id="db6d1-137">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="db6d1-137">Next steps</span></span>

- [<span data-ttu-id="db6d1-138">Incorporación de usuarios</span><span class="sxs-lookup"><span data-stu-id="db6d1-138">Add users</span></span>](create-user-accounts-and-set-permissions.md)






