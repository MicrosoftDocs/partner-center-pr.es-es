---
title: Entidad de servicio de Azure AD
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Averigüe cómo agregar una entidad de servicio al inquilino de Azure AD. Esta acción implica la incorporación de una aplicación de Azure AD (entidad de servicio) en el Centro de partners.
author: dhirajgandhi
ms.author: dhgandhi
Keywords: Azure, Azure plan, service principal, Azure AD application
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: bd2880f57d1ccb3c3675fef4fae7499f7ac02f4b
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949623"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="288e1-105">Incorporación de una aplicación de Azure AD (entidad de servicio) en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="288e1-105">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="288e1-106">En el programa de Marketplace comercial del Centro de partners, ahora puedes agregar una aplicación de Azure AD (entidad de servicio) como usuario en tu cuenta del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="288e1-106">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="288e1-107">(Antes podía hacerlo en la cuenta de Cloud Partner Portal, o CPP.</span><span class="sxs-lookup"><span data-stu-id="288e1-107">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="288e1-108">Ahora que ha migrado al Centro de partners, la cuenta de CPP es de solo lectura).</span><span class="sxs-lookup"><span data-stu-id="288e1-108">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="288e1-109">La entidad de servicio es sinónimo de aplicación de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="288e1-109">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="288e1-110">Incorporación de una aplicación de Azure AD (entidad de servicio)</span><span class="sxs-lookup"><span data-stu-id="288e1-110">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="288e1-111">En el panel del Centro de partners, selecciona **Configuración** y, a continuación, selecciona **Configuración de desarrollador**.</span><span class="sxs-lookup"><span data-stu-id="288e1-111">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="288e1-112">Selecciona **Usuarios** y, a continuación, **Agregar aplicaciones de Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="288e1-112">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="288e1-113">Selecciona una aplicación de Azure AD existente o crea una nueva.</span><span class="sxs-lookup"><span data-stu-id="288e1-113">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="288e1-114">Si creas una nueva aplicación de Azure AD, incluye la siguiente información:</span><span class="sxs-lookup"><span data-stu-id="288e1-114">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="288e1-115">**URL de respuesta**: dirección URL en la que los usuarios pueden iniciar sesión para usar la aplicación de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="288e1-115">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="288e1-116">**URI de identificación de la aplicación**: identificador lógico para la aplicación de Azure AD que se muestra cuando envía una solicitud de inicio de sesión único a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="288e1-116">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="288e1-117">**Roles de seguridad**: Los roles **Administrador** (idéntico al rol "Propietario" en CPP) y **Desarrollador** (el mismo que el rol "Colaborador" en CPP) se aplican al programa de Marketplace comercial del Centro de partners y se pueden asociar a esta aplicación de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="288e1-117">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  
