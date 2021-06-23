---
title: Agregar Servicios compartidos para asociados de Azure
description: Use Servicios compartidos para asociados de Azure para comprar suscripciones de Azure para su propio uso y para tener un método uniforme para comprar, realizar un seguimiento y administrar Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 40ba485cecce394dc81632d01f8774859690c522
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551612"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a><span data-ttu-id="99a0f-103">Agregue Servicios compartidos para asociados de Azure para que los asociados puedan comprar suscripciones de Azure para su propio uso</span><span class="sxs-lookup"><span data-stu-id="99a0f-103">Add Azure Partner Shared Services so partners can buy Azure subscriptions for their own use</span></span>

<span data-ttu-id="99a0f-104">**Roles adecuados:** Administrador global | Agente de administración | Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="99a0f-104">**Appropriate roles**: Global admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="99a0f-105">Servicios compartidos para asociados de Azure (APSS) es un nuevo tipo de oferta para los asociados del programa Proveedor de soluciones en la nube (CSP), lo que permite a los asociados adquirir suscripciones de Azure para su propio uso.</span><span class="sxs-lookup"><span data-stu-id="99a0f-105">Azure Partner Shared Services (APSS) is a new offer type for partners in the Cloud Solution Provider (CSP) program, enabling partners to purchase Azure subscriptions for their own use.</span></span><span data-ttu-id="99a0f-106">Crea la oportunidad de que los asociados usen un método uniforme para comprar, realizar un seguimiento y administrar Azure, además de la capacidad de consolidar sus contratos de licencias y reventa de Azure con Microsoft.</span><span class="sxs-lookup"><span data-stu-id="99a0f-106">  It creates the opportunity for partners to use a uniform method for purchasing, tracking, and managing Azure in addition to the ability to consolidate their Azure licensing and reselling agreements with Microsoft.</span></span> <span data-ttu-id="99a0f-107">Con APSS, los asociados ahora tienen la misma flexibilidad para usar suscripciones de Azure en CSP que en los programas Microsoft Contrato Enterprise y Web Direct, lo que abre escenarios como: crear entornos de desarrollo y pruebas, implementar cargas de trabajo internas y hospedar servicios compartidos o aplicaciones multiinquilino.</span><span class="sxs-lookup"><span data-stu-id="99a0f-107">With APSS, partners now have the same flexibility to use Azure subscriptions in CSP as they do in the Microsoft Enterprise Agreement and Web Direct programs, opening up scenarios such as:  build development and test environments, deploy internal workloads, and host shared services or multi-tenant applications.</span></span>  

## <a name="create-the-shared-services-tenant"></a><span data-ttu-id="99a0f-108">Creación del inquilino de servicios compartidos</span><span class="sxs-lookup"><span data-stu-id="99a0f-108">Create the shared services tenant</span></span>

1. <span data-ttu-id="99a0f-109">Vaya a **Configuración Configuración** Configuración de  >  **la cuenta** Servicios  >  **compartidos.**</span><span class="sxs-lookup"><span data-stu-id="99a0f-109">Go to **Settings** > **Account settings** > **Shared services**.</span></span>

   :::image type="content" source="images/sharedservices2.png" alt-text="Configuración de la > servicios compartidos":::

2. <span data-ttu-id="99a0f-111">Si aún no tiene un inquilino de servicios compartidos, seleccione **Crear servicios compartidos.**</span><span class="sxs-lookup"><span data-stu-id="99a0f-111">If you don't already have a shared services tenant, select **Create shared services**.</span></span>

   :::image type="content" source="images/sharedservices3.png" alt-text="Cree servicios compartidos.":::

3. <span data-ttu-id="99a0f-113">Esto crea un inquilino de servicios compartidos y adquiere la CSP de Azure de Servicios compartidos, que se usará para los recursos compartidos y la carga de trabajo interna.</span><span class="sxs-lookup"><span data-stu-id="99a0f-113">This creates a shared services tenant and purchases the Azure CSP Shared Services subscription, to be used for shared resources and internal workload.</span></span>

   :::image type="content" source="images/sharedservices5.png" alt-text="Cree el inquilino y compre la suscripción.":::

## <a name="about-the-azure--internalshared-services-offer"></a><span data-ttu-id="99a0f-115">Acerca de la Azure - Carga de trabajo interna/servicios compartidos de datos</span><span class="sxs-lookup"><span data-stu-id="99a0f-115">About the Azure- Internal/Shared Services offer</span></span>

- <span data-ttu-id="99a0f-116">La Azure - Carga de trabajo interna/servicios compartidos es un nuevo tipo de oferta de Azure en CSP al que se accede Centro de partners que los asociados obtienen para su propio uso de Azure.</span><span class="sxs-lookup"><span data-stu-id="99a0f-116">The Azure - Internal/Shared Services subscription is a new Azure offer type in CSP accessed through Partner Center that partners get for their own use of Azure.</span></span>

- <span data-ttu-id="99a0f-117">Servicios compartidos para asociados de Azure suscripciones son aptas y se pueden usar para comprar LAS.</span><span class="sxs-lookup"><span data-stu-id="99a0f-117">Azure Partner Shared Services subscriptions are eligible and can be used to purchase RIs.</span></span>

- <span data-ttu-id="99a0f-118">La Azure - Carga de trabajo interna/servicios compartidos oferta solo se puede aplicar al inquilino de servicios compartidos.</span><span class="sxs-lookup"><span data-stu-id="99a0f-118">The Azure - Internal/Shared Services offer can only be applied to the shared services tenant.</span></span>

- <span data-ttu-id="99a0f-119">El uso principal de la Azure - Carga de trabajo interna/servicios compartidos suscripción es para que pueda usar Azure con fines de desarrollo propios.</span><span class="sxs-lookup"><span data-stu-id="99a0f-119">The primary use for the Azure - Internal/Shared Services subscription is so that you can use Azure for your own development purposes.</span></span> <span data-ttu-id="99a0f-120">El inquilino compartido que usa para aprovisionar esta oferta no se puede usar para otros servicios como Office 365 o licencias de Dynamics.</span><span class="sxs-lookup"><span data-stu-id="99a0f-120">The shared tenant you use to provision this offer cannot be used for other services such as Office 365 or Dynamics licenses.</span></span>

- <span data-ttu-id="99a0f-121">Puede cancelar la suscripción como cualquier otra suscripción.</span><span class="sxs-lookup"><span data-stu-id="99a0f-121">You can cancel the subscription like any other subscription.</span></span> <span data-ttu-id="99a0f-122">Vaya a la **configuración de Ver todo**  >  **servicios**  >  **compartidos.**</span><span class="sxs-lookup"><span data-stu-id="99a0f-122">Go to the **settings** > **View all settings** > **Shared services**.</span></span> <span data-ttu-id="99a0f-123">Seleccione la Azure - Carga de trabajo interna/servicios compartidos suscripción y cancele.</span><span class="sxs-lookup"><span data-stu-id="99a0f-123">Select the Azure - Internal/Shared Services subscription and cancel it.</span></span>

## <a name="accessing-azure-partner-shared-services-consumption-details"></a><span data-ttu-id="99a0f-124">Acceso a Servicios compartidos para asociados de Azure de consumo</span><span class="sxs-lookup"><span data-stu-id="99a0f-124">Accessing Azure Partner Shared Services consumption details</span></span>

<span data-ttu-id="99a0f-125">Encontrará el consumo de Azure en la factura de CSP y el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="99a0f-125">You will find the Azure consumption on your CSP invoice and the reconciliation file.</span></span> <span data-ttu-id="99a0f-126">Se incluirá como parte de Microsoft Azure línea en la factura.</span><span class="sxs-lookup"><span data-stu-id="99a0f-126">It will be included as part of Microsoft Azure line item in the invoice.</span></span> <span data-ttu-id="99a0f-127">La información de consumo detallada estará disponible en el archivo de conciliación registrado en el inquilino que se creó para esta oferta.</span><span class="sxs-lookup"><span data-stu-id="99a0f-127">The detailed consumption information will be available in the reconciliation file logged against the tenant that was created for this offer.</span></span>

## <a name="azure-partner-shared-services-pricing"></a><span data-ttu-id="99a0f-128">Servicios compartidos para asociados de Azure precios</span><span class="sxs-lookup"><span data-stu-id="99a0f-128">Azure Partner Shared Services pricing</span></span>

<span data-ttu-id="99a0f-129">Para ver el nuevo archivo de precios de APSS, vaya a **Precios** de venta y ofertas y seleccione la lista de precios del mes  >   actual.</span><span class="sxs-lookup"><span data-stu-id="99a0f-129">To see the new pricing file for APSS, go to **Sell** > **Pricing and offers** and select the current month's price list.</span></span> <span data-ttu-id="99a0f-130">En las próximas semanas, también se lanzará una API de tarjeta de tarifa específica.</span><span class="sxs-lookup"><span data-stu-id="99a0f-130">In the coming weeks, a specific rate card api will also be released.</span></span>

## <a name="marketplace-offers-and-azure-partner-shared-services"></a><span data-ttu-id="99a0f-131">Ofertas y ofertas de Marketplace Servicios compartidos para asociados de Azure</span><span class="sxs-lookup"><span data-stu-id="99a0f-131">Marketplace offers and Azure Partner Shared Services</span></span>

<span data-ttu-id="99a0f-132">A partir del 1 de marzo de 2019, APSS ya no admite ofertas de Marketplace.</span><span class="sxs-lookup"><span data-stu-id="99a0f-132">As of March 1, 2019, APSS no longer supports Marketplace offers.</span></span>

|<span data-ttu-id="99a0f-133">**Soporte técnico de Marketplace**</span><span class="sxs-lookup"><span data-stu-id="99a0f-133">**Marketplace support**</span></span>   |<span data-ttu-id="99a0f-134">**APSS compatible antes del 1 de marzo de 2019**</span><span class="sxs-lookup"><span data-stu-id="99a0f-134">**APSS supported before March 1, 2019**</span></span>|<span data-ttu-id="99a0f-135">**Después del 1 de marzo de 2019**</span><span class="sxs-lookup"><span data-stu-id="99a0f-135">**After March 1, 2019**</span></span>|
|---------------------------|:----------------------------|:-------------------|
|<span data-ttu-id="99a0f-136">Traiga su propia licencia (BYOL) y servicios gratuitos</span><span class="sxs-lookup"><span data-stu-id="99a0f-136">Bring your own license (BYOL) and free services</span></span>   | <span data-ttu-id="99a0f-137">Sí</span><span class="sxs-lookup"><span data-stu-id="99a0f-137">Yes</span></span>   | <span data-ttu-id="99a0f-138">No</span><span class="sxs-lookup"><span data-stu-id="99a0f-138">No</span></span>|
|<span data-ttu-id="99a0f-139">Otras ofertas de Marketplace de terceros</span><span class="sxs-lookup"><span data-stu-id="99a0f-139">Other third-party marketplace offers</span></span>   | <span data-ttu-id="99a0f-140">No</span><span class="sxs-lookup"><span data-stu-id="99a0f-140">No</span></span>   |<span data-ttu-id="99a0f-141">No</span><span class="sxs-lookup"><span data-stu-id="99a0f-141">No</span></span>|

<span data-ttu-id="99a0f-142">Los asociados que tengan BYOL o servicios gratuitos implementados mediante APSS no se verán afectados; sin embargo, después del 1 de marzo de 2019 no podrán comprar nuevos byol ni servicios gratuitos.</span><span class="sxs-lookup"><span data-stu-id="99a0f-142">Partners who have BYOL or free services deployed using APSS will not be impacted; however after March 1, 2019 they will not be able to purchase new BYOL or free services.</span></span>

<span data-ttu-id="99a0f-143">Para aprovechar el catálogo completo de ofertas de Marketplace disponibles (no solo byol y servicios gratuitos), se recomienda que los asociados de CSP implementen servicios compartidos mediante suscripciones web directas de Azure.</span><span class="sxs-lookup"><span data-stu-id="99a0f-143">To take advantage of the full catalog of Marketplace offers available (not just BYOL and free services), we recommend CSP partners deploy shared services using web direct Azure subscriptions.</span></span>  <span data-ttu-id="99a0f-144">Se recomienda a los asociados de CSP que han implementado byol de terceros y recursos de servicio gratuitos de Marketplace anteriormente y que desean seguir usándolos e implementar más ofertas de terceros para migrar la suscripción de APSS a web directa migrando suscripciones de [Azure](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)existentes.</span><span class="sxs-lookup"><span data-stu-id="99a0f-144">CSP partners who have deployed third-party BYOL and free service resources from the Marketplace previously and wish to continue using them and deploy more third-party offerings are encouraged to migrate the APSS subscription to web direct [Migrating Existing Azure Subscriptions](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).</span></span>

<span data-ttu-id="99a0f-145">Los asociados, que tienen previsto seguir usando la suscripción de APSS después del 1 de marzo de 2019 y desean implementar nuevos servicios [BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) de terceros o servicios gratuitos, pueden seguir las instrucciones de los ISV para implementarlos en sus suscripciones de APSS.</span><span class="sxs-lookup"><span data-stu-id="99a0f-145">Partners, who plan to continue using APSS subscription after the March 1, 2019 and wish to deploy new third-party [BYOL services](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) or free services, can follow the instructions from ISVs to deploy these to their APSS subscriptions.</span></span>

## <a name="next-steps"></a><span data-ttu-id="99a0f-146">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="99a0f-146">Next steps</span></span>

- [<span data-ttu-id="99a0f-147">Venta de suscripciones de software a través de CSP</span><span class="sxs-lookup"><span data-stu-id="99a0f-147">Sell software subscriptions through CSP</span></span>](csp-software-subscriptions.md)