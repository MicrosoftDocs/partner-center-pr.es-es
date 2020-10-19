---
title: Agregar inquilinos adicionales a la cuenta del centro de Partners
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprenda a agregar, consolidar o administrar varios inquilinos de Azure AD en su cuenta del centro de Partners. Obtenga información acerca de algunas de las razones por las que podría querer hacerlo.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175166"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="78664-104">Adición y administración de varios inquilinos en la cuenta del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="78664-104">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="78664-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="78664-105">**Applies to**</span></span>

- <span data-ttu-id="78664-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="78664-106">Partner Center</span></span>

<span data-ttu-id="78664-107">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="78664-107">**Appropriate roles**</span></span>

- <span data-ttu-id="78664-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="78664-108">Global admin</span></span>

<span data-ttu-id="78664-109">Esta característica le permite administrar varios inquilinos para su empresa y consolidarlos en su cuenta del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="78664-109">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="78664-110">Hay muchas razones por las que puede que tenga que administrar varios inquilinos de Azure AD en la cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="78664-110">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="78664-111">Por ejemplo:</span><span class="sxs-lookup"><span data-stu-id="78664-111">For example:</span></span>

- <span data-ttu-id="78664-112">Su empresa puede comprar otra empresa y quiere que los empleados de la nueva empresa puedan usar el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="78664-112">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="78664-113">Sin embargo, desea que las dos compañías sigan siendo independientes.</span><span class="sxs-lookup"><span data-stu-id="78664-113">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="78664-114">En este caso, debe asociar el inquilino de Azure AD de la compañía a su cuenta global de socio comercial (PGA).</span><span class="sxs-lookup"><span data-stu-id="78664-114">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="78664-115">Esta asociación permitiría a los usuarios de ambas empresas trabajar en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="78664-115">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="78664-116">Si tiene más de un inquilino para ejecutar su empresa (por ejemplo, contoso.com, contoso.uk, contoso.in), puede usar multiinquilino para asociarlos con la misma cuenta de equipo.</span><span class="sxs-lookup"><span data-stu-id="78664-116">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="78664-117">Las fusiones y adquisiciones requieren que trabaje con más de un inquilino (por ejemplo, si Contoso adquiere Fabrikam, deberá poder usar los inquilinos respectivos Constoso.com y Fabrikam.com).</span><span class="sxs-lookup"><span data-stu-id="78664-117">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="78664-118">Los usuarios de cualquiera de los inquilinos necesitarán poder:</span><span class="sxs-lookup"><span data-stu-id="78664-118">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="78664-119">Centro de Partners de acceso para cursos, descargas digitales, Asociación de MCP</span><span class="sxs-lookup"><span data-stu-id="78664-119">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="78664-120">Debe tener asignados roles del centro de partners como el administrador de MPN, el administrador de incentivos, etc.</span><span class="sxs-lookup"><span data-stu-id="78664-120">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="78664-121">Agregar otro inquilino de Azure AD a su cuenta</span><span class="sxs-lookup"><span data-stu-id="78664-121">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="78664-122">Como administrador global, inicie sesión en el [Panel](https://partner.microsoft.com/dashboard)del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="78664-122">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="78664-123">En el icono de **configuración** , seleccione Configuración de la **cuenta** y, a continuación, seleccione **inquilinos**.</span><span class="sxs-lookup"><span data-stu-id="78664-123">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="asociar inquilinos"::: 

3. <span data-ttu-id="78664-125">Seleccione **asociar otro inquilino de ad** e indique el inquilino que quiere asociar.</span><span class="sxs-lookup"><span data-stu-id="78664-125">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="78664-126">Como administrador global, inicie sesión en el inquilino que desee asociar y confirme la asociación.</span><span class="sxs-lookup"><span data-stu-id="78664-126">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="asociar inquilinos"::: 

5. <span data-ttu-id="78664-128">Después de confirmar, verá una notificación de **todos los conjuntos** .</span><span class="sxs-lookup"><span data-stu-id="78664-128">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="78664-129">Seleccione **volver a administración de inquilinos** y verá el inquilino que se acaba de agregar.</span><span class="sxs-lookup"><span data-stu-id="78664-129">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="78664-130">No se puede asociar un inquilino a una cuenta si ya está asociado a otra cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="78664-130">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="78664-131">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="78664-131">Next steps</span></span>

- [<span data-ttu-id="78664-132">Incorporación de usuarios</span><span class="sxs-lookup"><span data-stu-id="78664-132">Add users</span></span>](create-user-accounts-and-set-permissions.md)
