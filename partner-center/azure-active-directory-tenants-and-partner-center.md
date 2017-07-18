---
title: Centro de partners e inquilinos de Azure Active Directory | Centro de partners
description: "Para crear una cuenta del Centro de partners, tu empresa debe tener un inquilino de Azure Active Directory (Azure AD). Azure AD es el servicio de administración de identidades y directorios basados en la nube de Microsoft."
author: labrenne
robots: 
ms.openlocfilehash: 9a9a3c3aa239017fe8ecf655f79acbfab6ff8a0b
ms.sourcegitcommit: d7c4ca62acd1ef1026c7d322e40f55a83a80e72a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/28/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a><span data-ttu-id="df18c-104">Centro de partners e inquilinos de Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="df18c-104">Azure Active Directory tenants and Partner Center</span></span>  

**<span data-ttu-id="df18c-105">Se aplica a</span><span class="sxs-lookup"><span data-stu-id="df18c-105">Applies to</span></span>**

-  <span data-ttu-id="df18c-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="df18c-106">Partner Center</span></span>

## <a name="why-you-need-an-azure-ad-tenant"></a><span data-ttu-id="df18c-107">¿Por qué necesitas un inquilino de Azure AD?</span><span class="sxs-lookup"><span data-stu-id="df18c-107">Why you need an Azure AD tenant</span></span>

<span data-ttu-id="df18c-108">Necesitamos vincular un inquilino de Azure AD de tu organización a tu nueva cuenta de Centro de partners para que los usuarios del inquilino puedan conectarse al Centro de partners con sus nombres de usuario y contraseñas de Azure AD (cuenta de Microsoft).</span><span class="sxs-lookup"><span data-stu-id="df18c-108">We need to link your organization’s Azure AD tenant to your new Partner Center account, so your tenant users can sign in to Partner Center with their Azure AD (Microsoft account) user names and passwords.</span></span>

<span data-ttu-id="df18c-109">Si tu empresa ya tiene un inquilino de Azure AD, puedes vincularlo a tu cuenta del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="df18c-109">If your company already has an Azure AD tenant, you can link it to your Partner Center account.</span></span> 

>**<span data-ttu-id="df18c-110">Nota</span><span class="sxs-lookup"><span data-stu-id="df18c-110">Note</span></span>**<br> <span data-ttu-id="df18c-111">Antes de decidir si usar un inquilino de Azure AD existente, piensa en cuántos usuarios del inquilino necesitarán trabajar en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="df18c-111">Before you decide to use an existing Azure AD tenant, think about how many users in the tenant will need to work in Partner Center.</span></span> <span data-ttu-id="df18c-112">Si tienes usuarios en el inquilino que no tendrán que trabajar en el Centro de partners, piensa en crear a un nuevo inquilino para solo aquellos usuarios que tendrán que trabajar en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="df18c-112">If you have users in the tenant who won’t need to work in Partner Center, consider creating a new tenant for only those users who will need to work in Partner Center.</span></span>

<span data-ttu-id="df18c-113">Si tu empresa aún no tiene un inquilino de Azure AD, puedes crear uno de forma gratuita durante el proceso de inscripción.</span><span class="sxs-lookup"><span data-stu-id="df18c-113">If your company doesn’t already have an Azure AD tenant, you can create one for free during the enrollment process.</span></span> <span data-ttu-id="df18c-114">Selecciona **Crear un inquilino** en la página **Iniciar sesión en Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="df18c-114">Select **Create new tenant** on the **Sign in to Azure Active Directory** page.</span></span> 

### <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a><span data-ttu-id="df18c-115">¿No estás seguro de si tu empresa ya tiene un inquilino de Azure AD?</span><span class="sxs-lookup"><span data-stu-id="df18c-115">Not sure if your company already has an Azure AD tenant?</span></span>

<span data-ttu-id="df18c-116">Si no estás seguro de si tu empresa tiene un inquilino de Azure AD, sigue estos pasos para comprobarlo.</span><span class="sxs-lookup"><span data-stu-id="df18c-116">If you’re not sure whether your company has an Azure AD tenant, follow these steps to check.</span></span> <span data-ttu-id="df18c-117">Ten en cuenta que si tienes una suscripción activa a Microsoft Azure u Office 365, ya tienes un inquilino de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="df18c-117">Note that If you have an active subscription to Microsoft Azure or Office 365, you already have an Azure AD tenant.</span></span>
1.  <span data-ttu-id="df18c-118">Inicia sesión en el portal de administración de Azure en https://ms.portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="df18c-118">Sign in to the Azure admin portal at https://ms.portal.azure.com</span></span>
2.  <span data-ttu-id="df18c-119">Selecciona Azure Active Directory en el menú y luego selecciona Nombres de dominio.</span><span class="sxs-lookup"><span data-stu-id="df18c-119">Select Azure Active Directory from the menu and then select Domain Names.</span></span>
3.  <span data-ttu-id="df18c-120">Si ya tienes un inquilino, se mostrará el nombre de dominio.</span><span class="sxs-lookup"><span data-stu-id="df18c-120">If you already have a tenant, your domain name will be listed.</span></span>

### <a name="using-an-existing-tenant"></a><span data-ttu-id="df18c-121">¿Quieres usar un inquilino existente?</span><span class="sxs-lookup"><span data-stu-id="df18c-121">Using an existing tenant?</span></span>

<span data-ttu-id="df18c-122">Si quieres usar un inquilino existente de Azure AD, pero tienes problemas para iniciar sesión, busca el escenario en el siguiente diagrama que mejor se adapte a tu situación y sigue los pasos recomendados.</span><span class="sxs-lookup"><span data-stu-id="df18c-122">If you want to use an existing Azure AD tenant but you’re having trouble signing in, find the scenario on the diagram below that best matches your situation and follow the recommended steps.</span></span> 

![¿Tienes un inquilino de Azure AD o necesitas crear uno?](images/onboardingAADFlow.png)

<span data-ttu-id="df18c-124">Para obtener más información sobre cómo agregar dominios a Azure AD, consulta [Agregar o asociar un dominio de Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)</span><span class="sxs-lookup"><span data-stu-id="df18c-124">For more information about adding domains in Azure AD, see [Add or associate a domain in Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)</span></span>

## <a name="about-microsoft-azure"></a><span data-ttu-id="df18c-125">Acerca de Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="df18c-125">About Microsoft Azure</span></span>

<span data-ttu-id="df18c-126">Microsoft Azure es una plataforma de nube pública que las empresas pueden usar para compilar, implementar y administrar aplicaciones a través de una red global de centros de datos administrados por Microsoft.</span><span class="sxs-lookup"><span data-stu-id="df18c-126">Microsoft Azure is a public cloud platform that companies can use to build, deploy, and manage applications across a global network of Microsoft-managed datacenters.</span></span> <span data-ttu-id="df18c-127">Las empresas usan Azure para crear una infraestructura de TI virtual con funciones virtuales o servicios, en lugar de equipos físicos.</span><span class="sxs-lookup"><span data-stu-id="df18c-127">Companies use Azure to build a virtual IT infrastructure with virtual functions, or services, instead of physical machines.</span></span> 

<span data-ttu-id="df18c-128">Al comprar una suscripción de Azure, esencialmente estás alquilando un espacio dedicado y seguro en la nube pública de Azure, no es demasiado distinto de alquilar una planta de un edificio de oficinas para albergar tu empresa física.</span><span class="sxs-lookup"><span data-stu-id="df18c-128">When you purchase an Azure subscription, you’re essentially renting a dedicated, secure space in the Azure public cloud, not too different from renting a floor in an office building to house your company’s physical business.</span></span> <span data-ttu-id="df18c-129">Para el propietario del edificio de oficinas, tu empresa es un inquilino.</span><span class="sxs-lookup"><span data-stu-id="df18c-129">To the office building’s owner, your company is a tenant.</span></span> 

<span data-ttu-id="df18c-130">Un inquilino de Azure AD es una representación virtual dedicada y aislada de tu empresa en la nube pública de Azure, creada automáticamente cuando te suscribes a un servicio en la nube de Microsoft como Azure, Microsoft Intune u Office 365.</span><span class="sxs-lookup"><span data-stu-id="df18c-130">An Azure AD tenant is a dedicated and isolated virtual representation of your company in the Azure public cloud, created for you when you subscribe to a Microsoft cloud service such as Azure, Microsoft Intune, or Office 365.</span></span> 

<span data-ttu-id="df18c-131">El inquilino hospeda los usuarios de Azure AD y la información sobre ellos: sus contraseñas, datos de perfil, permisos, etc.</span><span class="sxs-lookup"><span data-stu-id="df18c-131">Your tenant hosts your Azure AD users and the information about them - their passwords, profile data, permissions, and so on.</span></span> <span data-ttu-id="df18c-132">El inquilino también incluye grupos, aplicaciones y otra información relativa a una empresa y su seguridad.</span><span class="sxs-lookup"><span data-stu-id="df18c-132">The tenant also contains groups,applications, and other information pertaining to a company and its security.</span></span> 

<span data-ttu-id="df18c-133">Para obtener más información sobre Azure AD, consulta la [Documentación de Azure Active Directory](https://docs.microsoft.com/ azure/active-directory/).</span><span class="sxs-lookup"><span data-stu-id="df18c-133">To learn more about Azure AD, see the [Azure Active Directory Documentation](https://docs.microsoft.com/ azure/active-directory/).</span></span> 