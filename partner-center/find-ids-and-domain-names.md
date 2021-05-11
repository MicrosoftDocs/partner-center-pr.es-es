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
ms.openlocfilehash: 643b1eeb96a47ee4c438f733efe3be22234d02ff
ms.sourcegitcommit: e462f562e7f26b7d6870c22638a2a841499109d6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/11/2021
ms.locfileid: "109740291"
---
# <a name="locate-important-ids-for-a-user"></a>Buscar los id. importantes de un usuario

**Roles adecuados**

- Administrador global

En este artículo se describe cómo usar el [Azure Portal](https://portal.azure.com/) para buscar la siguiente información para un usuario:

- El Microsoft Azure Active Directory (Azure AD) de inquilino de la organización o empresa del usuario

- El nombre de dominio principal de la organización o empresa asociada al Azure AD inquilino

- El identificador de objeto de usuario

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>Busque el identificador Microsoft Azure AD inquilino y el nombre de dominio principal.

Siga estos pasos para buscar el identificador Azure AD inquilino o el nombre de dominio principal dentro del Azure Portal. (Si desea encontrar un identificador de inquilino mediante programación, consulte Buscar el identificador de inquilino [con PowerShell o la CLI).](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)

> [!NOTE]
> El identificador de inquilino se puede denominar nombres diferentes en diferentes aplicaciones o recursos. Por ejemplo, se puede hacer referencia al identificador de inquilino como el identificador de directorio, el inquilino de Azure Active Directory (Azure AD), el identificador de Microsoft o para determinados informes, incluso el *inquilinoguid*.

1. Inicie sesión en [Azure Portal](https://portal.azure.com/).

2. Seleccione **Azure Active Directory** en el menú.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Muestra Azure Portal seleccionar la Azure Active Directory en el menú.":::

3. Aparece Azure Active Directory **información general.** Para buscar el Azure AD de inquilino o el nombre de dominio principal, busque el campo **Id.** de inquilino y el **campo Dominio** principal. Estos campos aparecen en la sección Información del inquilino.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Muestra la página Información general con dos campos resaltados, el identificador de inquilino y el nombre de dominio principal.":::

4. Puede encontrar el identificador de inquilino en la Azure Portal de otras maneras. Seleccione **Azure Active Directory** en el menú. A continuación, busque **la sección** Administrar en el menú y seleccione **Propiedades.**

   La página Propiedades también muestra el identificador de inquilino asociado del usuario.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Muestra la página Propiedades con el campo Id. de inquilino resaltado.":::

## <a name="find-the-user-object-id"></a>Buscar el identificador de objeto de usuario

Es posible que encontrar el nombre de dominio y el identificador de inquilino no siempre sea suficiente. También es posible que tenga que buscar el identificador de objeto específico asignado a un usuario. Siga estos pasos para buscar el identificador de objeto de un usuario en el Azure Portal:

1. Inicie sesión en [Azure Portal](https://portal.azure.com/).

2. Seleccione **Azure Active Directory** en el menú.

3. Busque la **sección Administrar** en el menú y, a continuación, seleccione **Usuarios.**

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Muestra Azure Active Directory menú con la opción Usuarios resaltada.":::

4. En la página Usuarios, escriba el nombre del usuario en el cuadro de búsqueda.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Muestra la página Usuarios con el cuadro de búsqueda para buscar un usuario específico.":::

5. Seleccione el nombre del usuario donde aparece en la lista.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Muestra la página Usuario que muestra una fila para el usuario buscado.":::

6. Busque la sección Identidad en la página Perfil del usuario. El campo Id. de objeto aparece aquí con el identificador de objeto único del usuario.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Muestra la página Perfil de usuario con la sección Identidad y un campo resaltado para Id. de objeto.":::

## <a name="next-steps"></a>Pasos siguientes

- [Buscar el identificador de inquilino mediante programación con PowerShell o la CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Obtenga más información sobre los perfiles de usuario en Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Descubra cómo los asociados pueden ver o exportar los detalles del cliente en Centro de partners](see-your-customer-list.md)

