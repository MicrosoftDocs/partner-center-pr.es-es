---
title: Azure Cost Management de Cloudyn para CSP
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo registrar la aplicación Web de Cloudyn y usar una clave secreta para ella en el centro de partners para que pueda usar la aplicación para realizar un seguimiento del uso y los costos de Azure de los clientes.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: defa691a3bc70cbda45f01cb447d89364a49e3b8
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/02/2020
ms.locfileid: "96535002"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a><span data-ttu-id="a53c0-103">Realice un seguimiento del uso y los costos de Azure de los clientes con la aplicación Azure cost Management para asociados de CSP</span><span class="sxs-lookup"><span data-stu-id="a53c0-103">Track customer Azure usage and costs with the Azure cost management app for CSP partners</span></span>  

<span data-ttu-id="a53c0-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="a53c0-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a53c0-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="a53c0-105">Global admin</span></span>
- <span data-ttu-id="a53c0-106">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="a53c0-106">Admin agent</span></span>

[<span data-ttu-id="a53c0-107">Obtener más información sobre Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="a53c0-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="a53c0-108">Antes de empezar</span><span class="sxs-lookup"><span data-stu-id="a53c0-108">Before you begin</span></span>
<span data-ttu-id="a53c0-109">Antes de poder usar Azure Cost Management, asegúrese de cumplir los siguientes requisitos:</span><span class="sxs-lookup"><span data-stu-id="a53c0-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="a53c0-110">Usted es un asociado en el programa proveedor de soluciones en la nube.</span><span class="sxs-lookup"><span data-stu-id="a53c0-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="a53c0-111">Tiene la capacidad de crear una aplicación Web de API del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="a53c0-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="a53c0-112">Información general</span><span class="sxs-lookup"><span data-stu-id="a53c0-112">Overview</span></span>

<span data-ttu-id="a53c0-113">Cloudyn es una aplicación web que le permite realizar un seguimiento y administrar la cantidad de clientes que usan Azure y los costos de ese uso.</span><span class="sxs-lookup"><span data-stu-id="a53c0-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="a53c0-114">Se usa a través de la API del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="a53c0-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="a53c0-115">Registro de la aplicación web en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="a53c0-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="a53c0-116">Al registrar una aplicación Web de Azure Active Directory en el centro de Partners, se habilita el acceso a la API del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="a53c0-116">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="a53c0-117">Inicie sesión en el [centro de Partners](https://partnercenter.microsoft.com/pcv/dashboard/overview) con una [cuenta de administrador global o de agente de administración](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="a53c0-117">Sign into [Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="a53c0-118">En el **centro de Partners**, seleccione Configuración de la **cuenta** &gt; **[Administración de aplicaciones](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="a53c0-118">From **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="a53c0-119">En la sección **aplicación web** , haga clic en **Agregar nueva aplicación web**.</span><span class="sxs-lookup"><span data-stu-id="a53c0-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="a53c0-120">**Nota**: Si ya ha creado una aplicación Web, puede omitir el paso 3.</span><span class="sxs-lookup"><span data-stu-id="a53c0-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="a53c0-121">Copie y guarde el GUID de ID. de **Commerce** y el GUID de ID. de **aplicación** para la aplicación Web.</span><span class="sxs-lookup"><span data-stu-id="a53c0-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="a53c0-122">Necesitará ambos identificadores para usar la evaluación gratuita de 30 días de la aplicación Azure cost Management.</span><span class="sxs-lookup"><span data-stu-id="a53c0-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="a53c0-123">Agregar una clave secreta a la aplicación</span><span class="sxs-lookup"><span data-stu-id="a53c0-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="a53c0-124">En el menú desplegable situado junto al botón **Agregar clave** , seleccione una duración de 1 o 2 años.</span><span class="sxs-lookup"><span data-stu-id="a53c0-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="a53c0-125">Haga clic en **Agregar clave**.</span><span class="sxs-lookup"><span data-stu-id="a53c0-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="a53c0-126">Copie y guarde el valor de la clave secreta.</span><span class="sxs-lookup"><span data-stu-id="a53c0-126">Copy and save the secret key value.</span></span> <span data-ttu-id="a53c0-127">Lo necesitará para la evaluación gratuita de 30 días.</span><span class="sxs-lookup"><span data-stu-id="a53c0-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="a53c0-128">Las claves secretas de aplicación son similares a las contraseñas con fechas de expiración más largas.</span><span class="sxs-lookup"><span data-stu-id="a53c0-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="a53c0-129">Guarde el valor de clave en una ubicación segura para su uso futuro.</span><span class="sxs-lookup"><span data-stu-id="a53c0-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a53c0-130">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="a53c0-130">Next steps</span></span>
<span data-ttu-id="a53c0-131">Inicie una [evaluación gratuita de 30 días](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="a53c0-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="a53c0-132">Necesita los siguientes detalles para iniciar la versión de prueba:</span><span class="sxs-lookup"><span data-stu-id="a53c0-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="a53c0-133">Credenciales de inicio de sesión del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="a53c0-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="a53c0-134">GUID de ID. de Commerce</span><span class="sxs-lookup"><span data-stu-id="a53c0-134">Commerce ID GUID</span></span>
- <span data-ttu-id="a53c0-135">GUID de ID. de aplicación</span><span class="sxs-lookup"><span data-stu-id="a53c0-135">App ID GUID</span></span>
- <span data-ttu-id="a53c0-136">Valor de clave secreta de aplicación</span><span class="sxs-lookup"><span data-stu-id="a53c0-136">Application secret key value</span></span>
