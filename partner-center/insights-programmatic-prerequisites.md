---
title: Requisitos previos para acceder mediante programación a los datos de análisis
description: Requisitos previos para acceder mediante programación a los datos de análisis
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375865"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Requisitos previos para acceder mediante programación a los datos de análisis

**Roles adecuados:** Administrador global | Administrador de MPN

Para poder acceder mediante programación a los datos de análisis de Conclusiones de asociados, debe cumplir los requisitos siguientes.

## <a name="mpn-program-enrollment"></a>Inscripción del programa MPN

Para acceder a los datos de análisis de Partner Insights mediante programación, debe estar inscrito en el programa MPN y tener una Centro de partners asociada. Para obtener información sobre cómo hacerlo, [consulte Creación de una cuenta de MPN en Centro de partners](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>Creación Azure Active Directory aplicación (AAD)

No se pueden usar credenciales de usuario normales para el acceso mediante programación a los datos Ideas Analytics. Es Azure Active Directory una aplicación de acceso compartido (AAD) junto con un secreto (aplicación + acceso de usuario) para acceder a las API de acceso mediante programación. Para obtener información sobre cómo crear una aplicación y un secreto de AAD, consulte Inicio rápido: Registro de una [aplicación con el Plataforma de identidad de Microsoft.](/azure/active-directory/develop/quickstart-register-app)   Se requiere permiso para acceder a Microsoft Partner API. Para obtener información sobre cómo agregar permisos, consulte [Autenticación Partner API asociado](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>Asignación del rol Visor de informes ejecutivos (ERV) al usuario

Para acceder a los datos de análisis de Conclusiones de asociados mediante programación, debe tener el Visor de informes ejecutivos (ERV). Para obtener información sobre cómo asignar el rol ERV al usuario, consulte Centro de partners Ideas acceso basado [en roles: Centro de partners](insights-roles.md)

## <a name="generate-an-aad-token"></a>Generación de un token de AAD

Debe generar un token de AAD mediante el identificador de aplicación (cliente), el secreto de cliente, el identificador de usuario y la contraseña.   [Consulte aquí los](insights-programmatic-first-api-call.md#token-generation) pasos para generar el token de AAD.

> [!Note]
> El token es válido durante una hora.

## <a name="next-steps"></a>Pasos siguientes
[Paradigma del acceso mediante programación](insights-programmatic-access-paradigm.md)