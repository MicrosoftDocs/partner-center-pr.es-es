---
title: Buscar el identificador de inquilino, el nombre de dominio y el identificador de objeto de usuario
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Obtenga información sobre cómo buscar identificadores en el Azure Portal: el identificador de inquilino de Azure AD, el nombre de dominio o el identificador de objeto de usuario específico de una organización. Algunas tareas necesitan esta información.'
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 5da41cdbfa7aa1780b31e170a2398e8e7c65df27
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150869"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="7e53a-104">Buscar los id. importantes de un usuario</span><span class="sxs-lookup"><span data-stu-id="7e53a-104">Locate important IDs for a user</span></span>

<span data-ttu-id="7e53a-105">**Roles apropiados**: administrador global</span><span class="sxs-lookup"><span data-stu-id="7e53a-105">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="7e53a-106">En este artículo se describe cómo usar el [Azure Portal](https://portal.azure.com/) para buscar la siguiente información para un usuario:</span><span class="sxs-lookup"><span data-stu-id="7e53a-106">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="7e53a-107">El Microsoft Azure Active Directory (Azure AD) de inquilino de la organización o empresa del usuario</span><span class="sxs-lookup"><span data-stu-id="7e53a-107">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="7e53a-108">El nombre de dominio principal de la organización o empresa asociada al Azure AD inquilino</span><span class="sxs-lookup"><span data-stu-id="7e53a-108">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="7e53a-109">El identificador de objeto de usuario</span><span class="sxs-lookup"><span data-stu-id="7e53a-109">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="7e53a-110">Buscar el identificador Microsoft Azure AD inquilino y el nombre de dominio principal</span><span class="sxs-lookup"><span data-stu-id="7e53a-110">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="7e53a-111">Siga estos pasos para buscar el identificador Azure AD inquilino o el nombre de dominio principal dentro del Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="7e53a-111">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="7e53a-112">(Si desea encontrar un identificador de inquilino mediante programación, consulte Buscar el identificador de inquilino [con PowerShell o la CLI).](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="7e53a-112">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="7e53a-113">El identificador de inquilino se puede denominar nombres diferentes en diferentes aplicaciones o recursos.</span><span class="sxs-lookup"><span data-stu-id="7e53a-113">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="7e53a-114">Por ejemplo, se puede hacer referencia al identificador de inquilino como el identificador de directorio, el inquilino de Azure Active Directory (Azure AD), el identificador de Microsoft o para determinados informes, incluso el *inquilinoguid*.</span><span class="sxs-lookup"><span data-stu-id="7e53a-114">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="7e53a-115">Inicie sesión en [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="7e53a-115">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="7e53a-116">Seleccione **Azure Active Directory** en el menú.</span><span class="sxs-lookup"><span data-stu-id="7e53a-116">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Muestra Azure Portal seleccionar la Azure Active Directory en el menú.":::

3. <span data-ttu-id="7e53a-118">Aparece Azure Active Directory **información general.**</span><span class="sxs-lookup"><span data-stu-id="7e53a-118">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="7e53a-119">Para buscar el Azure AD de inquilino o el nombre de dominio principal, busque el campo **Id.** de inquilino y el **campo Dominio** principal.</span><span class="sxs-lookup"><span data-stu-id="7e53a-119">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="7e53a-120">Estos campos aparecen en la sección Información del inquilino.</span><span class="sxs-lookup"><span data-stu-id="7e53a-120">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Muestra la página Información general con dos campos resaltados, el identificador de inquilino y el nombre de dominio principal.":::

4. <span data-ttu-id="7e53a-122">Puede encontrar el identificador de inquilino en el Azure Portal de otras maneras.</span><span class="sxs-lookup"><span data-stu-id="7e53a-122">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="7e53a-123">Seleccione **Azure Active Directory** en el menú.</span><span class="sxs-lookup"><span data-stu-id="7e53a-123">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="7e53a-124">A continuación, busque **la sección** Administrar en el menú y seleccione **Propiedades.**</span><span class="sxs-lookup"><span data-stu-id="7e53a-124">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="7e53a-125">La página Propiedades también muestra el identificador de inquilino asociado del usuario.</span><span class="sxs-lookup"><span data-stu-id="7e53a-125">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Muestra la página Propiedades con el campo Id. de inquilino resaltado.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="7e53a-127">Buscar el identificador de objeto de usuario</span><span class="sxs-lookup"><span data-stu-id="7e53a-127">Find the user object ID</span></span>

<span data-ttu-id="7e53a-128">Es posible que encontrar el nombre de dominio y el identificador de inquilino no siempre sea suficiente.</span><span class="sxs-lookup"><span data-stu-id="7e53a-128">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="7e53a-129">También es posible que tenga que buscar el identificador de objeto específico asignado a un usuario.</span><span class="sxs-lookup"><span data-stu-id="7e53a-129">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="7e53a-130">Siga estos pasos para buscar el identificador de objeto de un usuario en el Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="7e53a-130">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="7e53a-131">Inicie sesión en [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="7e53a-131">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="7e53a-132">Seleccione **Azure Active Directory** en el menú.</span><span class="sxs-lookup"><span data-stu-id="7e53a-132">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="7e53a-133">Busque la **sección Administrar** en el menú y, a continuación, seleccione **Usuarios.**</span><span class="sxs-lookup"><span data-stu-id="7e53a-133">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Muestra Azure Active Directory menú con la opción Usuarios resaltada.":::

4. <span data-ttu-id="7e53a-135">En la página Usuarios, escriba el nombre del usuario en el cuadro de búsqueda.</span><span class="sxs-lookup"><span data-stu-id="7e53a-135">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Muestra la página Usuarios con el cuadro de búsqueda para buscar un usuario específico.":::

5. <span data-ttu-id="7e53a-137">Seleccione el nombre del usuario donde aparece en la lista.</span><span class="sxs-lookup"><span data-stu-id="7e53a-137">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Muestra la página Usuario que muestra una fila para el usuario buscado.":::

6. <span data-ttu-id="7e53a-139">Busque la sección Identidad en la página Perfil del usuario.</span><span class="sxs-lookup"><span data-stu-id="7e53a-139">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="7e53a-140">El campo Id. de objeto aparece aquí con el identificador de objeto único del usuario.</span><span class="sxs-lookup"><span data-stu-id="7e53a-140">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Muestra la página Perfil de usuario con la sección Identidad y un campo resaltado para Id. de objeto.":::

## <a name="next-steps"></a><span data-ttu-id="7e53a-142">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="7e53a-142">Next steps</span></span>

- [<span data-ttu-id="7e53a-143">Buscar el identificador de inquilino mediante programación con PowerShell o la CLI</span><span class="sxs-lookup"><span data-stu-id="7e53a-143">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="7e53a-144">Obtenga más información sobre los perfiles de usuario en Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7e53a-144">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="7e53a-145">Descubra cómo los asociados pueden ver o exportar los detalles del cliente en Centro de partners</span><span class="sxs-lookup"><span data-stu-id="7e53a-145">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)

