---
title: Azure Cost Management de Cloudyn para partners de CSP | Centro de partners
ms.topic: article
ms.date: 10/29/2018
description: Azure Cost Management de Cloudyn requiere acceso aprovisionado a la API del Centro de partners.
author: Janet
ms.author: janet
Keywords: Azure cost management app, manage costs, web apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 586ec2936b8491e91b4f2a56cbc392e4dee350b3
ms.sourcegitcommit: 3871c82c1075206a33eae7cd395a5a36edb2d1fc
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/08/2019
ms.locfileid: "8995799"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a><span data-ttu-id="d756a-103">Aplicación de administración de costos de Azure para partners de CSP de Azure</span><span class="sxs-lookup"><span data-stu-id="d756a-103">Azure cost management app for Azure CSP partners</span></span>  

**<span data-ttu-id="d756a-104">Se aplica a</span><span class="sxs-lookup"><span data-stu-id="d756a-104">Applies to</span></span>**

-  <span data-ttu-id="d756a-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="d756a-105">Partner Center</span></span>

[<span data-ttu-id="d756a-106">Obtener más información sobre Azure Cost Management</span><span class="sxs-lookup"><span data-stu-id="d756a-106">Get More information about Azure Cost Management</span></span>](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a><span data-ttu-id="d756a-107">Antes de comenzar</span><span class="sxs-lookup"><span data-stu-id="d756a-107">Before you begin</span></span>
<span data-ttu-id="d756a-108">Antes de poder usar Azure Cost Management, asegúrate de que cumples los siguientes requisitos:</span><span class="sxs-lookup"><span data-stu-id="d756a-108">Before you can use Azure Cost Management, be sure you meet the following requirements:</span></span>

- <span data-ttu-id="d756a-109">Eres partner en el programa de Proveedor de soluciones en la nube.</span><span class="sxs-lookup"><span data-stu-id="d756a-109">You are a partner in the Cloud Solution Provider program.</span></span>
- <span data-ttu-id="d756a-110">Tienes la capacidad para crear una aplicación web de API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d756a-110">You have the ability to create a Partner Center API web app.</span></span>

## <a name="overview"></a><span data-ttu-id="d756a-111">Introducción</span><span class="sxs-lookup"><span data-stu-id="d756a-111">Overview</span></span>

<span data-ttu-id="d756a-112">Azure Cost Management de Cloudyn es una aplicación web que permite realizar un seguimiento y administrar el número de clientes que están usando Azure y los costos de dicho uso.</span><span class="sxs-lookup"><span data-stu-id="d756a-112">Azure cost management by Cloudyn is a web app that allows you to track and manage how much your customers are using Azure and the costs of that usage.</span></span> <span data-ttu-id="d756a-113">Puedes usarla a través de la API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d756a-113">You use it through the Partner Center API.</span></span>

## <a name="register-your-web-app-in-the-partner-center"></a><span data-ttu-id="d756a-114">Registrar tu aplicación web en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="d756a-114">Register your web app in the Partner Center</span></span>
<span data-ttu-id="d756a-115">Al registrar una aplicación web de Azure Active Directory en el Centro de partners se habilita el acceso a la API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d756a-115">When you register an Azure Active Directory web app in Partner Center you enable access to the the Partner Center API.</span></span> 
1.  <span data-ttu-id="d756a-116">Inicia sesión en el [Centro de partners](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) con una [cuenta de agente de administración o administrador global](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="d756a-116">Sign into [the Partner Center](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) using a [global admin or admin agent account](create-user-accounts-and-set-permissions.md).</span></span>
2.  <span data-ttu-id="d756a-117">Desde el **Centro de partners**, selecciona la **configuración de la cuenta** &gt; **[administración de aplicaciones](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span><span class="sxs-lookup"><span data-stu-id="d756a-117">From the **Partner Center**, select **Account settings** &gt; **[App management](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.</span></span>
3.  <span data-ttu-id="d756a-118">En la sección **Aplicación web**, haz clic en **Agregar nueva aplicación web**.</span><span class="sxs-lookup"><span data-stu-id="d756a-118">In the **Web App** section, click **Add new web app**.</span></span>
<br> <span data-ttu-id="d756a-119">**Nota**: si ya has creado una aplicación web, puedes omitir el paso 3.</span><span class="sxs-lookup"><span data-stu-id="d756a-119">**Note**: If you have previously created a web app, you can skip step 3.</span></span>
4.  <span data-ttu-id="d756a-120">Copia y guarda el GUID de **ID de comercio** y el GUID de **ID de aplicación** para tu aplicación web.</span><span class="sxs-lookup"><span data-stu-id="d756a-120">Copy and save the **Commerce ID** GUID and the **App ID** GUID for your web app.</span></span> <span data-ttu-id="d756a-121">Necesitarás ambos identificadores para usar la versión de evaluación gratuita de 30 días de la aplicación Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="d756a-121">You will need both IDs to use the 30-day free trial of the Azure cost management app.</span></span>

## <a name="add-a-secret-key-to-your-app"></a><span data-ttu-id="d756a-122">Agregar una clave secreta a la aplicación</span><span class="sxs-lookup"><span data-stu-id="d756a-122">Add a secret key to your app</span></span>
1. <span data-ttu-id="d756a-123">En la lista desplegable situada junto al botón **Agregar clave**, selecciona una duración de 1 o 2 años.</span><span class="sxs-lookup"><span data-stu-id="d756a-123">In the drop down next to the **Add key** button, select a duration of 1 or 2 years.</span></span>
2. <span data-ttu-id="d756a-124">Haz clic en **Agregar clave**.</span><span class="sxs-lookup"><span data-stu-id="d756a-124">Click **Add key**.</span></span> 
3. <span data-ttu-id="d756a-125">Copia y guarda el valor de la clave secreta.</span><span class="sxs-lookup"><span data-stu-id="d756a-125">Copy and save the secret key value.</span></span> <span data-ttu-id="d756a-126">Lo necesitarás para la evaluación gratuita de 30 días.</span><span class="sxs-lookup"><span data-stu-id="d756a-126">You will need this for the 30-day free trial.</span></span><br>
   > [!NOTE]  
   > <span data-ttu-id="d756a-127">Las claves secretas de la aplicación son como contraseñas con fechas de caducidad más largas.</span><span class="sxs-lookup"><span data-stu-id="d756a-127">The application secret keys are like passwords with longer expiration dates.</span></span> <span data-ttu-id="d756a-128">Guarda el valor de clave en una ubicación segura para uso futuro.</span><span class="sxs-lookup"><span data-stu-id="d756a-128">Please save the key value in a secure location for future use.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d756a-129">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d756a-129">Next steps</span></span>
<span data-ttu-id="d756a-130">Inicia una [evaluación gratuita de 30 días](https://go.microsoft.com/fwlink/?linkid=857895).</span><span class="sxs-lookup"><span data-stu-id="d756a-130">Start a [30-day free trial](https://go.microsoft.com/fwlink/?linkid=857895).</span></span>
<span data-ttu-id="d756a-131">Necesitas la siguiente información para iniciar la prueba:</span><span class="sxs-lookup"><span data-stu-id="d756a-131">You need the following details to start the trial:</span></span>
- <span data-ttu-id="d756a-132">Credenciales para conectarse al Centro de datos</span><span class="sxs-lookup"><span data-stu-id="d756a-132">Partner Center sign in credentials</span></span>
- <span data-ttu-id="d756a-133">GUID de ID de comercio</span><span class="sxs-lookup"><span data-stu-id="d756a-133">Commerce ID GUID</span></span>
- <span data-ttu-id="d756a-134">GUID de ID de aplicación</span><span class="sxs-lookup"><span data-stu-id="d756a-134">App ID GUID</span></span>
- <span data-ttu-id="d756a-135">Valor de clave secreta de aplicación</span><span class="sxs-lookup"><span data-stu-id="d756a-135">Application secret key value</span></span>
