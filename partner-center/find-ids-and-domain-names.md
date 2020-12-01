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
ms.openlocfilehash: cb0325aae30fe57a4be2be3e37bca1ee6aa1eab8
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/01/2020
ms.locfileid: "96439234"
---
# <a name="locate-important-ids-for-a-user"></a>Búsqueda de identificadores importantes para un usuario

En este artículo se describe cómo usar el [Azure portal](https://portal.azure.com/) para buscar la siguiente información para un usuario:

- El identificador de inquilino de Microsoft Azure Active Directory (Azure AD) de la organización o la empresa del usuario

- El nombre de dominio principal de la organización o compañía asociada al inquilino de Azure AD

- IDENTIFICADOR de objeto de usuario

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Busque el identificador de inquilino de Microsoft Azure AD y el nombre de dominio principal

Siga estos pasos para buscar el identificador de inquilino de Azure AD o el nombre de dominio principal en el Azure Portal. (Si desea buscar un identificador de inquilino mediante programación, consulte búsqueda de un [identificador de inquilino con PowerShell o CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant.md#find-tenant-id-with-powershell)).

> [!NOTE]
> El identificador de inquilino puede denominarse nombres diferentes en aplicaciones o recursos diferentes. Por ejemplo, se puede hacer referencia al identificador de inquilino como el identificador de directorio, el inquilino de Azure Active Directory (Azure AD), el identificador de Microsoft o para determinados informes, incluso el *tenantguid*.

1. Inicie sesión en [Azure Portal](https://portal.azure.com/).

2. Seleccione **Azure Active Directory** en el menú.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Muestra Azure Portal seleccionar la opción Azure Active Directory en el menú.":::

3. Aparece una página de **información general** de Azure Active Directory. Para buscar el identificador de inquilino de Azure AD o el nombre de dominio principal, busque el campo ID. de **inquilino** y el campo **dominio principal** . Estos campos aparecen en la sección información del inquilino.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Muestra la página de información general con dos campos resaltados, el ID. de inquilino y el nombre de dominio principal.":::

4. Puede encontrar el identificador de inquilino en el Azure Portal de varias maneras. Seleccione **Azure Active Directory** en el menú. A continuación, busque la sección **administrar** en el menú y seleccione **propiedades**.

   En la página propiedades también se muestra el identificador de inquilino asociado del usuario.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Muestra la página de propiedades con el campo ID. de inquilino resaltado.":::

## <a name="find-the-user-object-id"></a>Buscar el ID. de objeto de usuario

Solo se puede encontrar el nombre de dominio y el ID. de inquilino. También es posible que necesite buscar el identificador de objeto específico asignado a un usuario. Siga estos pasos para buscar el identificador de objeto de un usuario en el Azure Portal:

1. Inicie sesión en [Azure Portal](https://portal.azure.com/).

2. Seleccione **Azure Active Directory** en el menú.

3. Busque la sección **administrar** en el menú y, a continuación, seleccione **usuarios**.

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Muestra Azure Active Directory menú con la opción usuarios resaltados.":::

4. En la página usuarios, escriba el nombre del usuario en el cuadro de búsqueda.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Muestra la página usuarios con el cuadro de búsqueda para buscar un usuario específico.":::

5. Seleccione el nombre del usuario en el que aparece en la lista.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Muestra una página de usuario que muestra una fila para el usuario buscado.":::

6. Busque la sección identidad en la página de perfil del usuario. El campo ID. de objeto aparece aquí con el identificador de objeto único del usuario.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Muestra la página de Perfil de usuario con la sección de identidad y un campo resaltado para el ID. de objeto.":::

## <a name="next-steps"></a>Pasos siguientes

- [Busque el identificador de inquilino mediante programación con PowerShell o CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Más información acerca de los perfiles de usuario en Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Averigüe cómo los asociados pueden ver o exportar los detalles del cliente en el centro de Partners](see-your-customer-list.md)

