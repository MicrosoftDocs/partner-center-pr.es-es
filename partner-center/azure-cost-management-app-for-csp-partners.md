---
title: Azure Cost Management de Cloudyn para partners de CSP | Centro de partners
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo registrar la aplicación Web de Cloudyn y usar una clave secreta para ella en el centro de partners para que pueda usar la aplicación para realizar un seguimiento del uso y los costos de Azure de los clientes.
author: Janet
ms.author: janet
Keywords: Aplicación de administración de costos de Azure, administración de costos, Web Apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: b05f2085aad63f8a0e23fa44de97550d13053f86
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253294"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="6ccbd-104">Aplicación de administración de costos de Azure para partners de CSP de Azure</span><span class="sxs-lookup"><span data-stu-id="6ccbd-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="6ccbd-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="6ccbd-105">**Applies to**</span></span>

- <span data-ttu-id="6ccbd-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="6ccbd-106">Partner Center</span></span>
- <span data-ttu-id="6ccbd-107">Partners del programa Proveedor de soluciones en la nube</span><span class="sxs-lookup"><span data-stu-id="6ccbd-107">Cloud Solution Provider program partners</span></span>

<span data-ttu-id="6ccbd-108">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="6ccbd-108">**Appropriate roles**</span></span>

- <span data-ttu-id="6ccbd-109">Administrador global</span><span class="sxs-lookup"><span data-stu-id="6ccbd-109">Global admin</span></span>
- <span data-ttu-id="6ccbd-110">Agente de administración</span><span class="sxs-lookup"><span data-stu-id="6ccbd-110">Admin agent</span></span>

[<span data-ttu-id="6ccbd-111">Obtener más información sobre Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="6ccbd-111">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="6ccbd-112">Antes de empezar</span><span class="sxs-lookup"><span data-stu-id="6ccbd-112">Before you begin</span></span>
<span data-ttu-id="6ccbd-113">Antes de poder usar Azure Cost Management, asegúrate de que cumples los siguientes requisitos:</span><span class="sxs-lookup"><span data-stu-id="6ccbd-113">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="6ccbd-114">Eres partner en el programa de Proveedor de soluciones en la nube.</span><span class="sxs-lookup"><span data-stu-id="6ccbd-114">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="6ccbd-115">Tienes la capacidad para crear una aplicación web de API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="6ccbd-115">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="6ccbd-116">Información general</span><span class="sxs-lookup"><span data-stu-id="6ccbd-116">Overview</span></span>

<span data-ttu-id="6ccbd-117">Cloudyn es una aplicación web que le permite realizar un seguimiento y administrar la cantidad de clientes que usan Azure y los costos de ese uso.</span><span class="sxs-lookup"><span data-stu-id="6ccbd-117">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="6ccbd-118">Puedes usarla a través de la API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="6ccbd-118">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="6ccbd-119">Registrar tu aplicación web en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="6ccbd-119">Register your web app in the Partner Center</span></span>
<span data-ttu-id="6ccbd-120">Al registrar una aplicación web de Azure Active Directory en el Centro de partners se habilita el acceso a la API del centro de partners.</span><span class="sxs-lookup"><span data-stu-id="6ccbd-120">When you register an Azure Active Directory web app in Partner Center you enable access to the Partner Center API.</span></span> 
1.  <span data-ttu-id="6ccbd-121">Inicia sesión en el [Centro de partners](https://partnercenter.microsoft.com/pcv/dashboard/overview) con una [cuenta de agente de administración o administrador global](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="6ccbd-121">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="6ccbd-122">En el **centro de Partners**, seleccione Configuración de la **cuenta** &gt; **[Administración de aplicaciones](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .</span><span class="sxs-lookup"><span data-stu-id="6ccbd-122">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="6ccbd-123">En la sección **Aplicación web**, haz clic en **Agregar nueva aplicación web**.</span><span class="sxs-lookup"><span data-stu-id="6ccbd-123">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="6ccbd-124">**Nota**: si ya has creado una aplicación web, puedes omitir el paso 3.</span><span class="sxs-lookup"><span data-stu-id="6ccbd-124">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="6ccbd-125">Copia y guarda el GUID de **ID de comercio** y el GUID de **ID de aplicación** para tu aplicación web.</span><span class="sxs-lookup"><span data-stu-id="6ccbd-125">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="6ccbd-126">Necesitarás ambos identificadores para usar la versión de evaluación gratuita de 30 días de la aplicación Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="6ccbd-126">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="6ccbd-127">Agregar una clave secreta a la aplicación</span><span class="sxs-lookup"><span data-stu-id="6ccbd-127">Add a secret key to your app</span></span>
1. <span data-ttu-id="6ccbd-128">En la lista desplegable situada junto al botón **Agregar clave**, selecciona una duración de 1 o 2 años.</span><span class="sxs-lookup"><span data-stu-id="6ccbd-128">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="6ccbd-129">Haz clic en **Agregar clave**.</span><span class="sxs-lookup"><span data-stu-id="6ccbd-129">Click **Add key**.</span></span> 
3. <span data-ttu-id="6ccbd-130">Copia y guarda el valor de la clave secreta.</span><span class="sxs-lookup"><span data-stu-id="6ccbd-130">Copy and save the secret key value.</span></span> <span data-ttu-id="6ccbd-131">Lo necesitarás para la evaluación gratuita de 30 días.</span><span class="sxs-lookup"><span data-stu-id="6ccbd-131">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="6ccbd-132">Las claves secretas de aplicación son similares a las contraseñas con fechas de expiración más largas.</span><span class="sxs-lookup"><span data-stu-id="6ccbd-132">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="6ccbd-133">Guarda el valor de clave en una ubicación segura para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="6ccbd-133">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6ccbd-134">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="6ccbd-134">Next steps</span></span>
<span data-ttu-id="6ccbd-135">Inicia una [evaluación gratuita de 30 días](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="6ccbd-135">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="6ccbd-136">Necesitas la siguiente información para iniciar la prueba:</span><span class="sxs-lookup"><span data-stu-id="6ccbd-136">You need the following details to start the trial:</span></span>
- <span data-ttu-id="6ccbd-137">Credenciales para conectarse al Centro de datos</span><span class="sxs-lookup"><span data-stu-id="6ccbd-137">Partner Center sign in credentials</span></span>
- <span data-ttu-id="6ccbd-138">GUID de ID de comercio</span><span class="sxs-lookup"><span data-stu-id="6ccbd-138">Commerce ID GUID</span></span>
- <span data-ttu-id="6ccbd-139">GUID de ID de aplicación</span><span class="sxs-lookup"><span data-stu-id="6ccbd-139">App ID GUID</span></span>
- <span data-ttu-id="6ccbd-140">Valor de clave secreta de aplicación</span><span class="sxs-lookup"><span data-stu-id="6ccbd-140">Application secret key value</span></span>
