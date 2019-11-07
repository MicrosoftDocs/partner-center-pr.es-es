---
title: Azure Cost Management de Cloudyn para partners de CSP | Centro de partners
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Azure Cost Management de Cloudyn requiere acceso aprovisionado a la API del Centro de partners.
author: Janet
ms.author: janet
Keywords: Aplicación de administración de costos de Azure, administración de costos, Web Apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: a746522d3470a8b97b845ed723fae87455e33e5e
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653867"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="6eb15-104">Aplicación de administración de costos de Azure para partners de CSP de Azure</span><span class="sxs-lookup"><span data-stu-id="6eb15-104">Azure cost management app for Azure CSP partners</span></span>  

<span data-ttu-id="6eb15-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="6eb15-105">**Applies to**</span></span>

-  <span data-ttu-id="6eb15-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="6eb15-106">Partner Center</span></span>

[<span data-ttu-id="6eb15-107">Obtener más información sobre Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="6eb15-107">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="6eb15-108">Antes de comenzar</span><span class="sxs-lookup"><span data-stu-id="6eb15-108">Before you begin</span></span>
<span data-ttu-id="6eb15-109">Antes de poder usar Azure Cost Management, asegúrate de que cumples los siguientes requisitos:</span><span class="sxs-lookup"><span data-stu-id="6eb15-109">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="6eb15-110">Eres partner en el programa de Proveedor de soluciones en la nube.</span><span class="sxs-lookup"><span data-stu-id="6eb15-110">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="6eb15-111">Tienes la capacidad para crear una aplicación web de API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="6eb15-111">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="6eb15-112">Introducción</span><span class="sxs-lookup"><span data-stu-id="6eb15-112">Overview</span></span>

<span data-ttu-id="6eb15-113">Cloudyn es una aplicación web que le permite realizar un seguimiento y administrar la cantidad de clientes que usan Azure y los costos de ese uso.</span><span class="sxs-lookup"><span data-stu-id="6eb15-113">Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="6eb15-114">Puedes usarla a través de la API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="6eb15-114">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="6eb15-115">Registrar tu aplicación web en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="6eb15-115">Register your web app in the Partner Center</span></span>
<span data-ttu-id="6eb15-116">Al registrar una aplicación web de Azure Active Directory en el Centro de partners se habilita el acceso a la API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="6eb15-116">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="6eb15-117">Inicia sesión en el [Centro de partners](https://partnercenter.microsoft.com/pcv/dashboard/overview) con una [cuenta de agente de administración o administrador global](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="6eb15-117">Sign into [the Partner Center](https://partnercenter.microsoft.com/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="6eb15-118">En el **centro de Partners**, seleccione Configuración de la **cuenta** &gt; **[Administración de aplicaciones](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .</span><span class="sxs-lookup"><span data-stu-id="6eb15-118">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="6eb15-119">En la sección **Aplicación web**, haz clic en **Agregar nueva aplicación web**.</span><span class="sxs-lookup"><span data-stu-id="6eb15-119">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="6eb15-120">**Nota**: si ya has creado una aplicación web, puedes omitir el paso 3.</span><span class="sxs-lookup"><span data-stu-id="6eb15-120">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="6eb15-121">Copia y guarda el GUID de **ID de comercio** y el GUID de **ID de aplicación** para tu aplicación web.</span><span class="sxs-lookup"><span data-stu-id="6eb15-121">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="6eb15-122">Necesitarás ambos identificadores para usar la versión de evaluación gratuita de 30 días de la aplicación Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="6eb15-122">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="6eb15-123">Agregar una clave secreta a la aplicación</span><span class="sxs-lookup"><span data-stu-id="6eb15-123">Add a secret key to your app</span></span>
1. <span data-ttu-id="6eb15-124">En la lista desplegable situada junto al botón **Agregar clave**, selecciona una duración de 1 o 2 años.</span><span class="sxs-lookup"><span data-stu-id="6eb15-124">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="6eb15-125">Haz clic en **Agregar clave**.</span><span class="sxs-lookup"><span data-stu-id="6eb15-125">Click **Add key**.</span></span> 
3. <span data-ttu-id="6eb15-126">Copia y guarda el valor de la clave secreta.</span><span class="sxs-lookup"><span data-stu-id="6eb15-126">Copy and save the secret key value.</span></span> <span data-ttu-id="6eb15-127">Lo necesitarás para la evaluación gratuita de 30 días.</span><span class="sxs-lookup"><span data-stu-id="6eb15-127">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="6eb15-128">Las claves secretas de aplicación son similares a las contraseñas con fechas de expiración más largas.</span><span class="sxs-lookup"><span data-stu-id="6eb15-128">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="6eb15-129">Guarda el valor de clave en una ubicación segura para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="6eb15-129">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6eb15-130">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="6eb15-130">Next steps</span></span>
<span data-ttu-id="6eb15-131">Inicia una [evaluación gratuita de 30 días](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="6eb15-131">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="6eb15-132">Necesitas la siguiente información para iniciar la prueba:</span><span class="sxs-lookup"><span data-stu-id="6eb15-132">You need the following details to start the trial:</span></span>
- <span data-ttu-id="6eb15-133">Credenciales para conectarse al Centro de datos</span><span class="sxs-lookup"><span data-stu-id="6eb15-133">Partner Center sign in credentials</span></span>
- <span data-ttu-id="6eb15-134">GUID de ID de comercio</span><span class="sxs-lookup"><span data-stu-id="6eb15-134">Commerce ID GUID</span></span>
- <span data-ttu-id="6eb15-135">GUID de ID de aplicación</span><span class="sxs-lookup"><span data-stu-id="6eb15-135">App ID GUID</span></span>
- <span data-ttu-id="6eb15-136">Valor de clave secreta de aplicación</span><span class="sxs-lookup"><span data-stu-id="6eb15-136">Application secret key value</span></span>
