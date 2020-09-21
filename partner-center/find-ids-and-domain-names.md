---
title: Buscar el ID. de inquilino, el nombre de dominio, el ID. de objeto de usuario
ms.topic: how-to
ms.date: 09/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Obtenga información sobre cómo buscar identificadores en el Azure Portal: el identificador de inquilino de Azure AD de una organización, el nombre de dominio o el identificador de objeto de usuario específico. Algunas tareas necesitan esta información.'
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4a3695079a9d5b0b3c66b7c2eda52a31888a6660
ms.sourcegitcommit: 3158b0de261539694e37e433c763afa4067e36fb
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/17/2020
ms.locfileid: "90740437"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="7495d-104">Búsqueda de identificadores importantes para un usuario</span><span class="sxs-lookup"><span data-stu-id="7495d-104">Locate important IDs for a user</span></span>

<span data-ttu-id="7495d-105">En este artículo se describe cómo usar el [Azure portal](https://portal.azure.com/) para buscar la siguiente información para un usuario:</span><span class="sxs-lookup"><span data-stu-id="7495d-105">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="7495d-106">El identificador de inquilino de Microsoft Azure Active Directory (Azure AD) de la organización o la empresa del usuario</span><span class="sxs-lookup"><span data-stu-id="7495d-106">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="7495d-107">El nombre de dominio principal de la organización o compañía asociada al inquilino de Azure AD</span><span class="sxs-lookup"><span data-stu-id="7495d-107">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="7495d-108">IDENTIFICADOR de objeto de usuario</span><span class="sxs-lookup"><span data-stu-id="7495d-108">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="7495d-109">Busque el identificador de inquilino de Microsoft Azure AD y el nombre de dominio principal</span><span class="sxs-lookup"><span data-stu-id="7495d-109">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="7495d-110">Siga estos pasos para buscar el identificador de inquilino de Azure AD o el nombre de dominio principal en el Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="7495d-110">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span>

> [!NOTE]
> <span data-ttu-id="7495d-111">El identificador de inquilino puede denominarse nombres diferentes en aplicaciones o recursos diferentes.</span><span class="sxs-lookup"><span data-stu-id="7495d-111">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="7495d-112">Por ejemplo, se puede hacer referencia al identificador de inquilino como el identificador de directorio, el inquilino de Azure Active Directory (Azure AD), el identificador de Microsoft o para determinados informes, incluso el *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="7495d-112">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="7495d-113">Inicie sesión en [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="7495d-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="7495d-114">Seleccione **Azure Active Directory** en el menú.</span><span class="sxs-lookup"><span data-stu-id="7495d-114">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Muestra Azure Portal seleccionar la opción Azure Active Directory en el menú.":::

3. <span data-ttu-id="7495d-116">Aparece una página de **información general** de Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7495d-116">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="7495d-117">Para buscar el identificador de inquilino de Azure AD o el nombre de dominio principal, busque el campo ID. de **inquilino** y el campo **dominio principal** .</span><span class="sxs-lookup"><span data-stu-id="7495d-117">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="7495d-118">Estos campos aparecen en la sección información del inquilino.</span><span class="sxs-lookup"><span data-stu-id="7495d-118">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Muestra la página de información general con dos campos resaltados, el ID. de inquilino y el nombre de dominio principal.":::

4. <span data-ttu-id="7495d-120">Puede encontrar el identificador de inquilino en el Azure Portal de varias maneras.</span><span class="sxs-lookup"><span data-stu-id="7495d-120">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="7495d-121">Seleccione **Azure Active Directory** en el menú.</span><span class="sxs-lookup"><span data-stu-id="7495d-121">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="7495d-122">A continuación, busque la sección **administrar** en el menú y seleccione **propiedades**.</span><span class="sxs-lookup"><span data-stu-id="7495d-122">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="7495d-123">En la página propiedades también se muestra el identificador de inquilino asociado del usuario.</span><span class="sxs-lookup"><span data-stu-id="7495d-123">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Muestra la página de propiedades con el campo ID. de inquilino resaltado.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="7495d-125">Buscar el ID. de objeto de usuario</span><span class="sxs-lookup"><span data-stu-id="7495d-125">Find the user object ID</span></span>

<span data-ttu-id="7495d-126">Solo se puede encontrar el nombre de dominio y el ID. de inquilino.</span><span class="sxs-lookup"><span data-stu-id="7495d-126">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="7495d-127">También es posible que necesite buscar el identificador de objeto específico asignado a un usuario.</span><span class="sxs-lookup"><span data-stu-id="7495d-127">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="7495d-128">Siga estos pasos para buscar el identificador de objeto de un usuario en el Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="7495d-128">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="7495d-129">Inicie sesión en [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="7495d-129">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="7495d-130">Seleccione **Azure Active Directory** en el menú.</span><span class="sxs-lookup"><span data-stu-id="7495d-130">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="7495d-131">Busque la sección **administrar** en el menú y, a continuación, seleccione **usuarios**.</span><span class="sxs-lookup"><span data-stu-id="7495d-131">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Muestra Azure Active Directory menú con la opción usuarios resaltados.":::

4. <span data-ttu-id="7495d-133">En la página usuarios, escriba el nombre del usuario en el cuadro de búsqueda.</span><span class="sxs-lookup"><span data-stu-id="7495d-133">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Muestra la página usuarios con el cuadro de búsqueda para buscar un usuario específico.":::

5. <span data-ttu-id="7495d-135">Seleccione el nombre del usuario en el que aparece en la lista.</span><span class="sxs-lookup"><span data-stu-id="7495d-135">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Muestra una página de usuario que muestra una fila para el usuario buscado.":::

6. <span data-ttu-id="7495d-137">Busque la sección identidad en la página de perfil del usuario.</span><span class="sxs-lookup"><span data-stu-id="7495d-137">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="7495d-138">El campo ID. de objeto aparece aquí con el identificador de objeto único del usuario.</span><span class="sxs-lookup"><span data-stu-id="7495d-138">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Muestra la página de Perfil de usuario con la sección de identidad y un campo resaltado para el ID. de objeto.":::

## <a name="next-steps"></a><span data-ttu-id="7495d-140">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="7495d-140">Next steps</span></span>

- [<span data-ttu-id="7495d-141">Más información acerca de los perfiles de usuario en Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7495d-141">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="7495d-142">Averigüe cómo los asociados pueden ver o exportar los detalles del cliente en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="7495d-142">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)