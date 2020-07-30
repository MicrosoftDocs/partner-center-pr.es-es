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
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389532"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a><span data-ttu-id="2633d-103">Adición y administración de varios inquilinos en la cuenta del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="2633d-103">Add and manage multiple tenants in your Partner Center account</span></span>

<span data-ttu-id="2633d-104">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="2633d-104">**Applies to**</span></span>

- <span data-ttu-id="2633d-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="2633d-105">Partner Center</span></span>

<span data-ttu-id="2633d-106">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="2633d-106">**Appropriate roles**</span></span>

- <span data-ttu-id="2633d-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="2633d-107">Global admin</span></span>

<span data-ttu-id="2633d-108">Hay muchas razones por las que puede que tenga que administrar varios inquilinos de Azure AD en la cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="2633d-108">There are many reasons why you may need to manage multiple Azure AD tenants in your Partner Center account.</span></span> <span data-ttu-id="2633d-109">Por ejemplo, su empresa puede comprar otra empresa y desea que los empleados de la nueva empresa puedan usar el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="2633d-109">For example, your company may purchase another company, and you want the employees in the new company to be able to use Partner Center.</span></span> <span data-ttu-id="2633d-110">Sin embargo, desea que las dos compañías sigan siendo independientes.</span><span class="sxs-lookup"><span data-stu-id="2633d-110">However, you want the two companies to remain separate.</span></span> <span data-ttu-id="2633d-111">En este caso, debe asociar el inquilino de Azure AD de la compañía a la cuenta global (PNG) del asociado.</span><span class="sxs-lookup"><span data-stu-id="2633d-111">In this case, you'd associate the new company's Azure AD tenant with your Partner global account (PNG).</span></span> <span data-ttu-id="2633d-112">Esta asociación permitiría a los usuarios de ambas empresas trabajar en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="2633d-112">This association would enable users in both companies to work in Partner Center.</span></span>

## <a name="add-another-azure-ad-tenant-to-your-account"></a><span data-ttu-id="2633d-113">Agregar otro inquilino de Azure AD a su cuenta</span><span class="sxs-lookup"><span data-stu-id="2633d-113">Add another Azure AD tenant to your account</span></span>

1. <span data-ttu-id="2633d-114">Como administrador global, inicie sesión en el [Panel](https://partner.microsoft.com/dashboard)del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="2633d-114">As the global admin, sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>
1. <span data-ttu-id="2633d-115">En el icono de **configuración** , seleccione Configuración de la **cuenta** y, a continuación, seleccione **inquilinos**.</span><span class="sxs-lookup"><span data-stu-id="2633d-115">From the **Settings** icon, select **Account settings** and then select **Tenants**.</span></span>
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="asociar inquilinos"::: 

3. <span data-ttu-id="2633d-117">Seleccione **asociar otro inquilino de ad** e indique el inquilino que quiere asociar.</span><span class="sxs-lookup"><span data-stu-id="2633d-117">Select **Associate another AD tenant** and indicate the tenant you want to associate.</span></span>

1. <span data-ttu-id="2633d-118">Como administrador global, inicie sesión en el inquilino que desee asociar y confirme la asociación.</span><span class="sxs-lookup"><span data-stu-id="2633d-118">As global admin, sign into the tenant you want to associate and confirm the association.</span></span> 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="confirmar los inquilinos asociados"::: 

5. <span data-ttu-id="2633d-120">Después de confirmar, verá una notificación de **todos los conjuntos** .</span><span class="sxs-lookup"><span data-stu-id="2633d-120">After you confirm, you will see an **All set** notice.</span></span>  <span data-ttu-id="2633d-121">Seleccione **volver a administración de inquilinos** y verá el inquilino que se acaba de agregar.</span><span class="sxs-lookup"><span data-stu-id="2633d-121">Select **Return to tenant management** and you will see the newly added tenant listed.</span></span>
 
## <a name="next-steps"></a><span data-ttu-id="2633d-122">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="2633d-122">Next steps</span></span>

- [<span data-ttu-id="2633d-123">Incorporación de usuarios</span><span class="sxs-lookup"><span data-stu-id="2633d-123">Add users</span></span>](create-user-accounts-and-set-permissions.md)
