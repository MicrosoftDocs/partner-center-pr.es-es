---
title: Buscar el ID. de inquilino, el nombre de dominio, el ID. de objeto de usuario
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Obtenga información sobre cómo buscar identificadores en el Azure Portal: el identificador de inquilino de Azure AD de una organización, el nombre de dominio o el identificador de objeto de usuario específico. Algunas tareas necesitan esta información.'
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: b88d6e11c7f4d56cf58d136a91b530688b3e5413
ms.sourcegitcommit: fdc32c0afce88f8266f75746ec15bf04745590ad
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/07/2020
ms.locfileid: "94360078"
---
# <a name="locate-important-ids-for-a-user"></a><span data-ttu-id="c9e26-104">Búsqueda de identificadores importantes para un usuario</span><span class="sxs-lookup"><span data-stu-id="c9e26-104">Locate important IDs for a user</span></span>

<span data-ttu-id="c9e26-105">En este artículo se describe cómo usar el [Azure portal](https://portal.azure.com/) para buscar la siguiente información para un usuario:</span><span class="sxs-lookup"><span data-stu-id="c9e26-105">This article describes how to use the [Azure portal](https://portal.azure.com/) to locate the following information for a user:</span></span>

- <span data-ttu-id="c9e26-106">El identificador de inquilino de Microsoft Azure Active Directory (Azure AD) de la organización o la empresa del usuario</span><span class="sxs-lookup"><span data-stu-id="c9e26-106">The Microsoft Azure Active Directory (Azure AD) tenant ID of the user's organization or company</span></span>

- <span data-ttu-id="c9e26-107">El nombre de dominio principal de la organización o compañía asociada al inquilino de Azure AD</span><span class="sxs-lookup"><span data-stu-id="c9e26-107">The primary domain name of the organization or company associated with the Azure AD tenant</span></span>

- <span data-ttu-id="c9e26-108">IDENTIFICADOR de objeto de usuario</span><span class="sxs-lookup"><span data-stu-id="c9e26-108">The user object ID</span></span>

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a><span data-ttu-id="c9e26-109">Busque el identificador de inquilino de Microsoft Azure AD y el nombre de dominio principal</span><span class="sxs-lookup"><span data-stu-id="c9e26-109">Find the Microsoft Azure AD tenant ID and primary domain name</span></span>

<span data-ttu-id="c9e26-110">Siga estos pasos para buscar el identificador de inquilino de Azure AD o el nombre de dominio principal en el Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="c9e26-110">Follow these steps to locate the Azure AD tenant ID or primary domain name within the Azure portal.</span></span> <span data-ttu-id="c9e26-111">(Si desea buscar un identificador de inquilino mediante programación, consulte búsqueda de un [identificador de inquilino con PowerShell o CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)).</span><span class="sxs-lookup"><span data-stu-id="c9e26-111">(If you'd like to find a tenant ID programmatically, see [Find tenant ID with PowerShell or CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell).)</span></span>

> [!NOTE]
> <span data-ttu-id="c9e26-112">El identificador de inquilino puede denominarse nombres diferentes en aplicaciones o recursos diferentes.</span><span class="sxs-lookup"><span data-stu-id="c9e26-112">The tenant ID may be called different names in different applications or resources.</span></span> <span data-ttu-id="c9e26-113">Por ejemplo, se puede hacer referencia al identificador de inquilino como el identificador de directorio, el inquilino de Azure Active Directory (Azure AD), el identificador de Microsoft o para determinados informes, incluso el *tenantguid*.</span><span class="sxs-lookup"><span data-stu-id="c9e26-113">For example, the tenant ID may be referred to as the directory ID, the Azure Active Directory (Azure AD) tenant, Microsoft ID, or for certain reports, even the *tenantguid*.</span></span>

1. <span data-ttu-id="c9e26-114">Inicie sesión en [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="c9e26-114">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="c9e26-115">Seleccione **Azure Active Directory** en el menú.</span><span class="sxs-lookup"><span data-stu-id="c9e26-115">Select **Azure Active Directory** from the menu.</span></span>

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Muestra Azure Portal seleccionar la opción Azure Active Directory en el menú.":::

3. <span data-ttu-id="c9e26-117">Aparece una página de **información general** de Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c9e26-117">An Azure Active Directory **Overview** page appears.</span></span> <span data-ttu-id="c9e26-118">Para buscar el identificador de inquilino de Azure AD o el nombre de dominio principal, busque el campo ID. de **inquilino** y el campo **dominio principal** .</span><span class="sxs-lookup"><span data-stu-id="c9e26-118">To find the Azure AD tenant ID or primary domain name, look for the **Tenant ID** field and the **Primary domain** field.</span></span> <span data-ttu-id="c9e26-119">Estos campos aparecen en la sección información del inquilino.</span><span class="sxs-lookup"><span data-stu-id="c9e26-119">These fields appear in the Tenant information section.</span></span>

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Muestra la página de información general con dos campos resaltados, el ID. de inquilino y el nombre de dominio principal.":::

4. <span data-ttu-id="c9e26-121">Puede encontrar el identificador de inquilino en el Azure Portal de varias maneras.</span><span class="sxs-lookup"><span data-stu-id="c9e26-121">You can find the tenant ID in the Azure portal in a few other ways.</span></span> <span data-ttu-id="c9e26-122">Seleccione **Azure Active Directory** en el menú.</span><span class="sxs-lookup"><span data-stu-id="c9e26-122">Select **Azure Active Directory** from the menu.</span></span> <span data-ttu-id="c9e26-123">A continuación, busque la sección **administrar** en el menú y seleccione **propiedades**.</span><span class="sxs-lookup"><span data-stu-id="c9e26-123">Then, locate the **Manage** section on the menu and select **Properties**.</span></span>

   <span data-ttu-id="c9e26-124">En la página propiedades también se muestra el identificador de inquilino asociado del usuario.</span><span class="sxs-lookup"><span data-stu-id="c9e26-124">The Properties page also displays the user's associated Tenant ID.</span></span>

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Muestra la página de propiedades con el campo ID. de inquilino resaltado.":::

## <a name="find-the-user-object-id"></a><span data-ttu-id="c9e26-126">Buscar el ID. de objeto de usuario</span><span class="sxs-lookup"><span data-stu-id="c9e26-126">Find the user object ID</span></span>

<span data-ttu-id="c9e26-127">Solo se puede encontrar el nombre de dominio y el ID. de inquilino.</span><span class="sxs-lookup"><span data-stu-id="c9e26-127">Just finding the domain name and tenant ID may not always be enough.</span></span> <span data-ttu-id="c9e26-128">También es posible que necesite buscar el identificador de objeto específico asignado a un usuario.</span><span class="sxs-lookup"><span data-stu-id="c9e26-128">You may also need to locate the specific object ID assigned to a user.</span></span> <span data-ttu-id="c9e26-129">Siga estos pasos para buscar el identificador de objeto de un usuario en el Azure Portal:</span><span class="sxs-lookup"><span data-stu-id="c9e26-129">Follow these steps to find a user's object ID in the Azure portal:</span></span>

1. <span data-ttu-id="c9e26-130">Inicie sesión en [Azure Portal](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="c9e26-130">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="c9e26-131">Seleccione **Azure Active Directory** en el menú.</span><span class="sxs-lookup"><span data-stu-id="c9e26-131">Select **Azure Active Directory** from the menu.</span></span>

3. <span data-ttu-id="c9e26-132">Busque la sección **administrar** en el menú y, a continuación, seleccione **usuarios**.</span><span class="sxs-lookup"><span data-stu-id="c9e26-132">Locate the **Manage** section on the menu, then select **Users**.</span></span>

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Muestra Azure Active Directory menú con la opción usuarios resaltados.":::

4. <span data-ttu-id="c9e26-134">En la página usuarios, escriba el nombre del usuario en el cuadro de búsqueda.</span><span class="sxs-lookup"><span data-stu-id="c9e26-134">From the Users page, type the user's name in the search box.</span></span>

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Muestra la página usuarios con el cuadro de búsqueda para buscar un usuario específico.":::

5. <span data-ttu-id="c9e26-136">Seleccione el nombre del usuario en el que aparece en la lista.</span><span class="sxs-lookup"><span data-stu-id="c9e26-136">Select the user's name where it appears on the list.</span></span>  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Muestra una página de usuario que muestra una fila para el usuario buscado.":::

6. <span data-ttu-id="c9e26-138">Busque la sección identidad en la página de perfil del usuario.</span><span class="sxs-lookup"><span data-stu-id="c9e26-138">Locate the Identity section on the user's Profile page.</span></span> <span data-ttu-id="c9e26-139">El campo ID. de objeto aparece aquí con el identificador de objeto único del usuario.</span><span class="sxs-lookup"><span data-stu-id="c9e26-139">The Object ID field appears here with the user's unique object ID.</span></span>

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Muestra la página de Perfil de usuario con la sección de identidad y un campo resaltado para el ID. de objeto.":::

## <a name="next-steps"></a><span data-ttu-id="c9e26-141">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="c9e26-141">Next steps</span></span>

- [<span data-ttu-id="c9e26-142">Busque el identificador de inquilino mediante programación con PowerShell o CLI</span><span class="sxs-lookup"><span data-stu-id="c9e26-142">Find your tenant ID programmatically with PowerShell or CLI</span></span>](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [<span data-ttu-id="c9e26-143">Más información acerca de los perfiles de usuario en Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c9e26-143">Learn more about user profiles in Azure Active Directory</span></span>](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [<span data-ttu-id="c9e26-144">Averigüe cómo los asociados pueden ver o exportar los detalles del cliente en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="c9e26-144">Find out how partners can see or export customer details in Partner Center</span></span>](see-your-customer-list.md)
