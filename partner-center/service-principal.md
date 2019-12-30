---
title: Entidad de servicio de Azure AD | Centro de partners
ms.topic: article
ms.date: 12/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Incorporación de una entidad de servicio al inquilino de Azure AD
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, Azure plan, service principal, Azure AD application
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 1fe4211879df2063f7b865c249870c49a346f518
ms.sourcegitcommit: 369aceafc54e960ac0bd3a023edc85b06361492b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/12/2019
ms.locfileid: "75010386"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="17b0d-104">Incorporación de una aplicación de Azure AD (entidad de servicio) en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="17b0d-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="17b0d-105">En el programa de Marketplace comercial del Centro de partners, ahora puedes agregar una aplicación de Azure AD (entidad de servicio) como usuario en tu inquilino de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="17b0d-105">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Azure AD tenant.</span></span> <span data-ttu-id="17b0d-106">(Ya podías hacerlo anteriormente en la cuenta de Cloud Partner Portal pero, ahora que has migrado al Centro de partners, esa cuenta es de solo lectura). Ten en cuenta que entidad de servicio es sinónimo de aplicación de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="17b0d-106">(You were able to do this previously in your Cloud Partner Portal (CPP) account, but now that you have migrated to Partner Center, the CPP acount is read-only.) Note that service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="17b0d-107">Incorporación de una aplicación de Azure AD (entidad de servicio)</span><span class="sxs-lookup"><span data-stu-id="17b0d-107">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="17b0d-108">En el panel del Centro de partners, selecciona **Configuración** y, a continuación, selecciona **Configuración de desarrollador**.</span><span class="sxs-lookup"><span data-stu-id="17b0d-108">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="17b0d-109">Selecciona **Usuarios** y, a continuación, **Agregar aplicaciones de Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="17b0d-109">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="17b0d-110">Selecciona una aplicación de Azure AD existente o crea una nueva.</span><span class="sxs-lookup"><span data-stu-id="17b0d-110">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="17b0d-111">Si creas una nueva aplicación de Azure AD, incluye la siguiente información:</span><span class="sxs-lookup"><span data-stu-id="17b0d-111">If you create a new Azure AD Application, include the following information:</span></span>  
<span data-ttu-id="17b0d-112">  
 \*\*Nombre\*\*: Es similar al campo "nombre descriptivo" del portal de CPP.</span><span class="sxs-lookup"><span data-stu-id="17b0d-112">  
\*\*Name\*\*: This is similar to the ‘friendly name’ field in the CPP portal.</span></span>

<span data-ttu-id="17b0d-113">**URL de respuesta**: Esta es la dirección URL en la que los usuarios pueden iniciar sesión para usar la aplicación de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="17b0d-113">**Reply URL**: This is the URL where users can sign in to use your Azure AD application.</span></span> 

<span data-ttu-id="17b0d-114">**URI de identificación de la aplicación**: Se trata de un identificador lógico para la aplicación de Azure AD que se muestra cuando envía una solicitud de inicio de sesión único a Azure AD.</span><span class="sxs-lookup"><span data-stu-id="17b0d-114">**App ID URI**: This is a logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span> 

<span data-ttu-id="17b0d-115">**Roles de seguridad**: Los roles **Administrador** (idéntico al rol "Propietario" en CPP) y **Desarrollador** (el mismo que el rol "Colaborador" en CPP) se aplican al programa de Marketplace comercial del Centro de partners y se pueden asociar a esta aplicación de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="17b0d-115">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

<span data-ttu-id="17b0d-116">Cuando seleccionas **Guardar** para crear esta en el Centro de partners, la información también se vuelve a sincronizar con el sistema de CPP.</span><span class="sxs-lookup"><span data-stu-id="17b0d-116">When you select **Save**,  to create this in Partner Center, the information is also synced back to the CPP system.</span></span>  
