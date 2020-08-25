---
title: Agregar inquilinos adicionales a la cuenta del centro de Partners
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Administrar varios inquilinos a través de la cuenta del centro de Partners
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ecdfcbd4801bee34be298030016d7366b12d7db3
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/25/2020
ms.locfileid: "88846973"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="d37a1-103">Adición y administración de varios inquilinos en la cuenta del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="d37a1-103">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="d37a1-104">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="d37a1-104">**Applies to**</span></span>

- <span data-ttu-id="d37a1-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="d37a1-105">Partner Center</span></span>

<span data-ttu-id="d37a1-106">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="d37a1-106">**Appropriate roles**</span></span>

- <span data-ttu-id="d37a1-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d37a1-107">Global admin</span></span>

<span data-ttu-id="d37a1-108">Esta característica le permite administrar varios inquilinos para su empresa y consolidarlos en su cuenta del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d37a1-108">This feature allows you to manage multiple tenants for your company and to consolidate them into your Partner Center account.</span></span> <span data-ttu-id="d37a1-109">Hay muchas razones por las que puede que tenga que administrar varios inquilinos de Azure AD en la cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="d37a1-109">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="d37a1-110">Por ejemplo:</span><span class="sxs-lookup"><span data-stu-id="d37a1-110">For example:</span></span>

- <span data-ttu-id="d37a1-111">Su empresa puede comprar otra empresa y quiere que los empleados de la nueva empresa puedan usar el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="d37a1-111">Your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="d37a1-112">Sin embargo, desea que las dos compañías sigan siendo independientes.</span><span class="sxs-lookup"><span data-stu-id="d37a1-112">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="d37a1-113">En este caso, debe asociar el inquilino de Azure AD de la compañía a su cuenta global de socio comercial (PGA).</span><span class="sxs-lookup"><span data-stu-id="d37a1-113">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PGA).</span></span> <span data-ttu-id="d37a1-114">Esta asociación permitiría a los usuarios de ambas empresas trabajar en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="d37a1-114">This association would enable users in both companies to work in Partner Center.</span></span>

- <span data-ttu-id="d37a1-115">Si tiene más de un inquilino para ejecutar su empresa (por ejemplo, contoso.com, contoso.uk, contoso.in), puede usar multiinquilino para asociarlos con la misma cuenta de equipo.</span><span class="sxs-lookup"><span data-stu-id="d37a1-115">If you have more than one tenant to run your business (e.g. contoso.com, contoso.uk, contoso.in) you can use multi-tenancy to tie them under the same PC account.</span></span>

- <span data-ttu-id="d37a1-116">Las fusiones y adquisiciones requieren que trabaje con más de un inquilino (por ejemplo, si Contoso adquiere Fabrikam, deberá poder usar los inquilinos respectivos Constoso.com y Fabrikam.com).</span><span class="sxs-lookup"><span data-stu-id="d37a1-116">Mergers and acquisitions requires you to work with more than one tenant (e.g. If Contoso acquires Fabrikam, you would need to be able to use both Constoso.com and Fabrikam.com respective tenants).</span></span>

- <span data-ttu-id="d37a1-117">Los usuarios de cualquiera de los inquilinos necesitarán poder:</span><span class="sxs-lookup"><span data-stu-id="d37a1-117">Users from any of the tenants would need to be able to:</span></span>
    1.  <span data-ttu-id="d37a1-118">Centro de Partners de acceso para cursos, descargas digitales, Asociación de MCP</span><span class="sxs-lookup"><span data-stu-id="d37a1-118">Access Partner Center for training, digital downloads, MCP association</span></span>
    2.  <span data-ttu-id="d37a1-119">Debe tener asignados roles del centro de partners como el administrador de MPN, el administrador de incentivos, etc.</span><span class="sxs-lookup"><span data-stu-id="d37a1-119">Be assigned Partner Center roles like MPN Admin, Incentives Admin etc.</span></span>


## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="d37a1-120">Agregar otro inquilino de Azure AD a su cuenta</span><span class="sxs-lookup"><span data-stu-id="d37a1-120">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="d37a1-121">Como administrador global, inicie sesión en el [Panel](https://partner.microsoft.com/dashboard)del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="d37a1-121">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="d37a1-122">En el icono de **configuración** , seleccione Configuración de la **cuenta** y, a continuación, seleccione **inquilinos**.</span><span class="sxs-lookup"><span data-stu-id="d37a1-122">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="asociar inquilinos"::: 

3. <span data-ttu-id="d37a1-124">Seleccione **asociar otro inquilino de ad** e indique el inquilino que quiere asociar.</span><span class="sxs-lookup"><span data-stu-id="d37a1-124">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="d37a1-125">Como administrador global, inicie sesión en el inquilino que desee asociar y confirme la asociación.</span><span class="sxs-lookup"><span data-stu-id="d37a1-125">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="confirmar los inquilinos asociados"::: 

5. <span data-ttu-id="d37a1-127">Después de confirmar, verá una notificación de **todos los conjuntos** .</span><span class="sxs-lookup"><span data-stu-id="d37a1-127">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="d37a1-128">Seleccione **volver a administración de inquilinos** y verá el inquilino que se acaba de agregar.</span><span class="sxs-lookup"><span data-stu-id="d37a1-128">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span> 
 

>[!NOTE]
><span data-ttu-id="d37a1-129">No se puede asociar un inquilino a una cuenta si ya está asociado a otra cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="d37a1-129">You can't associate a tenant to an account if it is already associated to another Partner Center account.</span></span>

 
## <a name="next-steps"></a><span data-ttu-id="d37a1-130">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d37a1-130">Next steps</span></span>

- [<span data-ttu-id="d37a1-131">Incorporación de usuarios</span><span class="sxs-lookup"><span data-stu-id="d37a1-131">Add users</span></span>](create-user-accounts-and-set-permissions.md)
