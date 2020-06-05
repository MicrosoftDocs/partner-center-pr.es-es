---
title: Agregar Servicios compartidos para asociados de Azure
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use los servicios compartidos de asociados de Azure para comprar suscripciones de Azure para su propio uso y para tener un método uniforme de compra, seguimiento y administración de Azure.
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, servicios compartidos, inquilino
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 62989c58284de46834f02abc01041c454e725a81
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/04/2020
ms.locfileid: "84425954"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a><span data-ttu-id="bdfb5-104">Agregue los servicios compartidos de asociados de Azure para que los asociados puedan comprar suscripciones de Azure para su propio uso.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-104">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>

<span data-ttu-id="bdfb5-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="bdfb5-105">**Applies to**</span></span>

- <span data-ttu-id="bdfb5-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="bdfb5-106">Partner Center</span></span>

<span data-ttu-id="bdfb5-107">Los Servicios compartidos para partners de Azure son un nuevo tipo de oferta para partners en el programa CSP que les permite comprar suscripciones de Azure para el uso propio.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-107">Azure Partner Shared Services is a new offer type for partners in the CSP program enabling partners to purchase Azure subscriptions for their own use.</span></span><span data-ttu-id="bdfb5-108">Crea la oportunidad de que los asociados usen un método uniforme para comprar, realizar el seguimiento y administrar Azure, además de la capacidad de consolidar sus contratos de licencia y reventa de Azure con Microsoft.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-108">  It creates the opportunity for partners to use a uniform method for purchasing, tracking, and managing Azure in addition to the ability to consolidate their Azure licensing and reselling agreements with Microsoft.</span></span> <span data-ttu-id="bdfb5-109">Con los servicios compartidos de asociados de Azure, ahora los asociados tienen la misma flexibilidad para usar las suscripciones de Azure en CSP que en los programas de Microsoft Contrato Enterprise y Web Direct, lo que abre escenarios como compilar entornos de desarrollo y pruebas, implementar cargas de trabajo internas y hospedar servicios compartidos o aplicaciones de varios inquilinos.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-109">With Azure Partner Shared Services, partners now have the same flexibility to use Azure subscriptions in CSP as they do in the Microsoft Enterprise Agreement and Web Direct programs, opening up scenarios such as:  build development and test environments, deploy internal workloads, and host shared services or multi-tenant applications.</span></span>  

## <a name="create-the-shared-services-tenant"></a><span data-ttu-id="bdfb5-110">Crear el inquilino de servicios compartidos</span><span class="sxs-lookup"><span data-stu-id="bdfb5-110">Create the shared services tenant</span></span>

1. <span data-ttu-id="bdfb5-111">Vaya a **configuración**  >  **ver toda la configuración**  >  **servicios compartidos**.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-111">Go to **Settings** > **View all settings** > **Shared services**.</span></span>

   ![\* \* Configuración de la cuenta \* \* > \* \* servicios compartidos \* \*](images/sharedservices2.png)

2. <span data-ttu-id="bdfb5-113">Si aún no tiene un inquilino de servicios compartidos, haga clic en **crear servicios compartidos**.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-113">If you don't already have a shared services tenant, click **Create shared services**.</span></span>

   ![Crear servicios compartidos](images/sharedservices3.png)

3. <span data-ttu-id="bdfb5-115">Esto crea un inquilino de servicios compartidos y compra la suscripción de servicios compartidos de CSP de Azure, que se usará para los recursos compartidos y la carga de trabajo interna.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-115">This creates a shared services tenant and purchases the Azure CSP Shared Services subscription, to be used for shared resources and internal workload.</span></span>

   ![Creación del inquilino y compra de la suscripción](images/sharedservices5.png)

## <a name="about-the-azure--internalshared-services-offer"></a><span data-ttu-id="bdfb5-117">Acerca de la oferta de Azure-Carga de trabajo interna/servicios compartidos</span><span class="sxs-lookup"><span data-stu-id="bdfb5-117">About the Azure- Internal/Shared Services offer</span></span>

- <span data-ttu-id="bdfb5-118">El Azure-Carga de trabajo interna/servicios compartidos suscripción es un nuevo tipo de oferta de Azure en CSP al que se tiene acceso a través del centro de partners que los asociados obtienen para su propio uso de Azure.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-118">The Azure - Internal/Shared Services subscription is a new Azure offer type in CSP accessed through Partner Center that partners get for their own use of Azure.</span></span> 

- <span data-ttu-id="bdfb5-119">Azure-Carga de trabajo interna/servicios compartidos oferta no es válida para descuentos e incentivos.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-119">Azure - Internal/Shared Services offer is not eligible for discounts and incentives.</span></span>

- <span data-ttu-id="bdfb5-120">La oferta de Azure-Carga de trabajo interna/servicios compartidos solo se puede aplicar al inquilino de servicios compartidos.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-120">The Azure - Internal/Shared Services offer can only be applied to the shared services tenant.</span></span>

- <span data-ttu-id="bdfb5-121">El uso principal de la suscripción Azure-Carga de trabajo interna/servicios compartidos es para que pueda usar Azure para sus propios propósitos de desarrollo.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-121">The primary use for the Azure - Internal/Shared Services subscription is so that you can use Azure for your own development purposes.</span></span> <span data-ttu-id="bdfb5-122">El inquilino compartido que se usa para aprovisionar esta oferta no se puede usar para otros servicios como Office 365 o Dynamics.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-122">The shared tenant you use to provision this offer cannot be used for other services such as Office 365 or Dynamics seats.</span></span> 

- <span data-ttu-id="bdfb5-123">Puede cancelar la suscripción como cualquier otra suscripción.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-123">You can cancel the subscription like any other subscription.</span></span> <span data-ttu-id="bdfb5-124">Vaya a la **configuración**  >  **vista todos los**  >  **servicios compartidos**.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-124">Go to the **settings** > **View all settings** > **Shared services**.</span></span> <span data-ttu-id="bdfb5-125">Seleccione el Azure-Carga de trabajo interna/servicios compartidos suscripción y cancélelo.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-125">Select the Azure - Internal/Shared Services subscription and cancel it.</span></span>

## <a name="accessing-azure-partner-shared-services-consumption-details"></a><span data-ttu-id="bdfb5-126">Obtener acceso a los detalles de consumo de servicios compartidos de Azure Partner</span><span class="sxs-lookup"><span data-stu-id="bdfb5-126">Accessing Azure Partner Shared Services consumption details</span></span>

<span data-ttu-id="bdfb5-127">Encontrará el consumo de Azure en la factura de CSP y en el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-127">You will find the Azure consumption on your CSP invoice and the reconciliation file.</span></span> <span data-ttu-id="bdfb5-128">Se incluirá como parte de Microsoft Azure elemento de línea de la factura.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-128">It will be included as part of Microsoft Azure line item in the invoice.</span></span> <span data-ttu-id="bdfb5-129">La información detallada sobre el consumo estará disponible en el archivo de conciliación registrado en el inquilino que se creó para esta oferta.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-129">The detailed consumption information will be available in the reconciliation file logged against the tenant that was created for this offer.</span></span> 

## <a name="azure-partner-shared-services-pricing"></a><span data-ttu-id="bdfb5-130">Precios de los servicios compartidos de asociados de Azure</span><span class="sxs-lookup"><span data-stu-id="bdfb5-130">Azure Partner Shared Services pricing</span></span>

<span data-ttu-id="bdfb5-131">Para ver el nuevo archivo de precios de los servicios compartidos de asociados de Azure, vaya a **vender**  >  **precios y ofertas** y seleccione la lista de precios del mes actual.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-131">To see the new pricing file for Azure Partner Shared Services go to **Sell** > **Pricing and offers** and select the current month's price list.</span></span> <span data-ttu-id="bdfb5-132">En las próximas semanas, también se publicará una API de tarjeta de tarifas específica.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-132">In the coming weeks, a specific rate card api will also be released.</span></span>

## <a name="marketplace-offers-and-azure-partner-shared-services"></a><span data-ttu-id="bdfb5-133">Ofertas de Marketplace y servicios compartidos de asociados de Azure</span><span class="sxs-lookup"><span data-stu-id="bdfb5-133">Marketplace offers and Azure Partner Shared Services</span></span>

<span data-ttu-id="bdfb5-134">A partir del 1 de marzo de 2019, los servicios compartidos de asociados de Azure (APSS) ya no admiten ofertas de Marketplace.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-134">As of March 1, 2019, Azure Partner Shared Services (APSS) no longer supports Marketplace offers.</span></span>

|<span data-ttu-id="bdfb5-135">**Soporte técnico de Marketplace**</span><span class="sxs-lookup"><span data-stu-id="bdfb5-135">**Marketplace support**</span></span>   |<span data-ttu-id="bdfb5-136">**APSS admitido antes del 1 de marzo de 2019**</span><span class="sxs-lookup"><span data-stu-id="bdfb5-136">**APSS supported before March 1, 2019**</span></span>|<span data-ttu-id="bdfb5-137">**Después del 1 de marzo de 2019**</span><span class="sxs-lookup"><span data-stu-id="bdfb5-137">**After March 1, 2019**</span></span>|
|---------------------------|:----------------------------|:-------------------|
|<span data-ttu-id="bdfb5-138">Traiga su propia licencia (BYOL) y servicios gratuitos</span><span class="sxs-lookup"><span data-stu-id="bdfb5-138">Bring your own license (BYOL) and free services</span></span>   | <span data-ttu-id="bdfb5-139">Sí</span><span class="sxs-lookup"><span data-stu-id="bdfb5-139">Yes</span></span>   | <span data-ttu-id="bdfb5-140">No</span><span class="sxs-lookup"><span data-stu-id="bdfb5-140">No</span></span>|
|<span data-ttu-id="bdfb5-141">Otras ofertas de Marketplace de terceros</span><span class="sxs-lookup"><span data-stu-id="bdfb5-141">Other third-party marketplace offers</span></span>   | <span data-ttu-id="bdfb5-142">No</span><span class="sxs-lookup"><span data-stu-id="bdfb5-142">No</span></span>   |<span data-ttu-id="bdfb5-143">No</span><span class="sxs-lookup"><span data-stu-id="bdfb5-143">No</span></span>|

<span data-ttu-id="bdfb5-144">Los asociados que tienen servicios BYOL o gratis implementados con APSS no se verán afectados; sin embargo, después del 1 de marzo de 2019, no podrán adquirir nuevos servicios de BYOL o gratis.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-144">Partners who have BYOL or free services deployed using APSS will not be impacted; however after March 1, 2019 they will not be able to purchase new BYOL or free services.</span></span>

<span data-ttu-id="bdfb5-145">Para aprovechar el catálogo completo de ofertas de Marketplace disponibles (no solo BYOL y servicios gratuitos), recomendamos que los asociados de CSP implementen servicios compartidos con suscripciones de Azure directas de Web.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-145">To take advantage of the full catalog of Marketplace offers available (not just BYOL and free services), we recommend CSP partners deploy shared services using web direct Azure subscriptions.</span></span>  <span data-ttu-id="bdfb5-146">Los asociados de CSP que han implementado BYOL de terceros y recursos de servicio gratis desde Marketplace previamente y desean seguir utilizándolos e implementar más ofertas de terceros se recomiendan para migrar la suscripción de APSS a web Direct y [migrar las suscripciones de Azure existentes](https://docs.microsoft.com/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span><span class="sxs-lookup"><span data-stu-id="bdfb5-146">CSP partners who have deployed third-party BYOL and free service resources from the Marketplace previously and wish to continue using them and deploy more third-party offerings are encouraged to migrate the APSS subscription to web direct [Migrating Existing Azure Subscriptions](https://docs.microsoft.com/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span></span>

<span data-ttu-id="bdfb5-147">Los asociados, que planean seguir usando la suscripción a APSS después del 1 de marzo de 2019 y desean implementar nuevos [servicios de BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) de terceros o servicios gratuitos, pueden seguir las instrucciones de los ISV para implementarlos en sus suscripciones de APSS.</span><span class="sxs-lookup"><span data-stu-id="bdfb5-147">Partners, who plan to continue using APSS subscription after the March 1, 2019 and wish to deploy new third-party [BYOL services](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) or free services, can follow the instructions from ISVs to deploy these to their APSS subscriptions.</span></span>

