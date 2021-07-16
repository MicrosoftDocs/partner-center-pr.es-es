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
# <a name="prerequisites-to-programmatically-access-analytics-data"></a><span data-ttu-id="70a22-103">Requisitos previos para acceder mediante programación a los datos de análisis</span><span class="sxs-lookup"><span data-stu-id="70a22-103">Prerequisites to programmatically access analytics data</span></span>

<span data-ttu-id="70a22-104">**Roles adecuados:** Administrador global | Administrador de MPN</span><span class="sxs-lookup"><span data-stu-id="70a22-104">**Appropriate roles:** Global admin | MPN admin</span></span>

<span data-ttu-id="70a22-105">Para poder acceder mediante programación a los datos de análisis de Conclusiones de asociados, debe cumplir los requisitos siguientes.</span><span class="sxs-lookup"><span data-stu-id="70a22-105">Before you can programmatically access partner insights analytics data, you need to meet the following requirements.</span></span>

## <a name="mpn-program-enrollment"></a><span data-ttu-id="70a22-106">Inscripción del programa MPN</span><span class="sxs-lookup"><span data-stu-id="70a22-106">MPN Program enrollment</span></span>

<span data-ttu-id="70a22-107">Para acceder a los datos de análisis de Partner Insights mediante programación, debe estar inscrito en el programa MPN y tener una Centro de partners asociada.</span><span class="sxs-lookup"><span data-stu-id="70a22-107">To access partner insights analytics data programmatically, you need to be enrolled in the MPN program and have a Partner Center account.</span></span> <span data-ttu-id="70a22-108">Para obtener información sobre cómo hacerlo, [consulte Creación de una cuenta de MPN en Centro de partners](mpn-create-a-partner-center-account.md)</span><span class="sxs-lookup"><span data-stu-id="70a22-108">To learn how, see [Create an MPN account in Partner Center](mpn-create-a-partner-center-account.md)</span></span>

## <a name="create-azure-active-directory-aad-application"></a><span data-ttu-id="70a22-109">Creación Azure Active Directory aplicación (AAD)</span><span class="sxs-lookup"><span data-stu-id="70a22-109">Create Azure Active Directory (AAD) application</span></span>

<span data-ttu-id="70a22-110">No se pueden usar credenciales de usuario normales para el acceso mediante programación a los datos Ideas Analytics.</span><span class="sxs-lookup"><span data-stu-id="70a22-110">Regular user credentials cannot be used for programmatic access of Partner Insights Analytics data.</span></span> <span data-ttu-id="70a22-111">Es Azure Active Directory una aplicación de acceso compartido (AAD) junto con un secreto (aplicación + acceso de usuario) para acceder a las API de acceso mediante programación.</span><span class="sxs-lookup"><span data-stu-id="70a22-111">An Azure Active Directory (AAD) application needs to be created along with a secret (application + user access) to access the programmatic access APIs.</span></span> <span data-ttu-id="70a22-112">Para obtener información sobre cómo crear una aplicación y un secreto de AAD, consulte Inicio rápido: Registro de una [aplicación con el Plataforma de identidad de Microsoft.](/azure/active-directory/develop/quickstart-register-app)   Se requiere permiso para acceder a Microsoft Partner API.</span><span class="sxs-lookup"><span data-stu-id="70a22-112">To learn how to create an AAD application and secret, see [Quickstart: Register an application with the Microsoft identity platform.](/azure/active-directory/develop/quickstart-register-app) Permission is required to access Microsoft Partner API.</span></span> <span data-ttu-id="70a22-113">Para obtener información sobre cómo agregar permisos, consulte [Autenticación Partner API asociado](/partner/develop/api-authentication#application-and-user-access)</span><span class="sxs-lookup"><span data-stu-id="70a22-113">To learn how to add permission, see [Partner API authentication - Partner](/partner/develop/api-authentication#application-and-user-access)</span></span>

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a><span data-ttu-id="70a22-114">Asignación del rol Visor de informes ejecutivos (ERV) al usuario</span><span class="sxs-lookup"><span data-stu-id="70a22-114">Assign Executive Report Viewer (ERV) role to the user</span></span>

<span data-ttu-id="70a22-115">Para acceder a los datos de análisis de Conclusiones de asociados mediante programación, debe tener el Visor de informes ejecutivos (ERV).</span><span class="sxs-lookup"><span data-stu-id="70a22-115">To access partner insights analytics data programmatically, you should have Executive Report Viewer (ERV).</span></span> <span data-ttu-id="70a22-116">Para obtener información sobre cómo asignar el rol ERV al usuario, consulte Centro de partners Ideas acceso basado [en roles: Centro de partners](insights-roles.md)</span><span class="sxs-lookup"><span data-stu-id="70a22-116">To learn how to assign ERV role to the user, see [Partner Center Insights role-based access - Partner Center](insights-roles.md)</span></span>

## <a name="generate-an-aad-token"></a><span data-ttu-id="70a22-117">Generación de un token de AAD</span><span class="sxs-lookup"><span data-stu-id="70a22-117">Generate an AAD token</span></span>

<span data-ttu-id="70a22-118">Debe generar un token de AAD mediante el identificador de aplicación (cliente), el secreto de cliente, el identificador de usuario y la contraseña.   [Consulte aquí los](insights-programmatic-first-api-call.md#token-generation) pasos para generar el token de AAD.</span><span class="sxs-lookup"><span data-stu-id="70a22-118">You need to Generate an AAD token using the Application (client) ID, client secret, your user ID and password.  [Check here](insights-programmatic-first-api-call.md#token-generation) for steps to generate AAD token.</span></span>

> [!Note]
> <span data-ttu-id="70a22-119">El token es válido durante una hora.</span><span class="sxs-lookup"><span data-stu-id="70a22-119">The token is valid for one hour.</span></span>

## <a name="next-steps"></a><span data-ttu-id="70a22-120">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="70a22-120">Next steps</span></span>
[<span data-ttu-id="70a22-121">Paradigma del acceso mediante programación</span><span class="sxs-lookup"><span data-stu-id="70a22-121">Programmatic access paradigm</span></span>](insights-programmatic-access-paradigm.md)