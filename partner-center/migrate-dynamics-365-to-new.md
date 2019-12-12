---
title: Migración de ofertas de Dynamics 365 Business Edition a versiones más recientes | Centro de Partners
ms.topic: article
ms.date: 12/12/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo migrar las ofertas de Dynamics 365 Business Edition a las versiones más recientes antes de que expiren.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Ofertas de Dynamics 365, renovar ofertas, nuevas SKU de Dynamics 365
ms.openlocfilehash: d4efd051b4d237eac5b766ed1aedc432e8b93ecc
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/11/2019
ms.locfileid: "75005124"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="554e6-104">Migrar ofertas de Dynamics 365 Business Edition a versiones más recientes</span><span class="sxs-lookup"><span data-stu-id="554e6-104">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span> 

<span data-ttu-id="554e6-105">**適用於**</span><span class="sxs-lookup"><span data-stu-id="554e6-105">**Applies to**</span></span>

- <span data-ttu-id="554e6-106">合作夥伴中心</span><span class="sxs-lookup"><span data-stu-id="554e6-106">Partner Center</span></span>

<span data-ttu-id="554e6-107">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="554e6-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="554e6-108">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="554e6-108">Global admin</span></span>
-   <span data-ttu-id="554e6-109">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="554e6-109">User admin</span></span>
-   <span data-ttu-id="554e6-110">Agente de administración</span><span class="sxs-lookup"><span data-stu-id="554e6-110">Admin agent</span></span>
-   <span data-ttu-id="554e6-111">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="554e6-111">Sales agent</span></span>

<span data-ttu-id="554e6-112">A partir del 1 de enero de 2019, los clientes con suscripciones de Dynamics 365 Business Edition ya no podrán renovar en estas ofertas heredadas. las suscripciones existentes no se renovarán automáticamente cuando expiren.</span><span class="sxs-lookup"><span data-stu-id="554e6-112">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="554e6-113">En la página de detalles de la suscripción, el estado de la suscripción cambiará a "expira el [fecha]" de "se renueva automáticamente en [fecha]".</span><span class="sxs-lookup"><span data-stu-id="554e6-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="554e6-114">Para garantizar la continuidad de los clientes, debe realizar la transición de las suscripciones que van a expirar a una opción admitida, que se enumera a continuación.</span><span class="sxs-lookup"><span data-stu-id="554e6-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="554e6-115">Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes.</span><span class="sxs-lookup"><span data-stu-id="554e6-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="554e6-116">Si usa la API (de la cresta o del centro de Partners), puede encontrar suscripciones que van a expirar mediante la evaluación de la fecha de finalización de la suscripción junto con la propiedad auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="554e6-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="554e6-117">Las suscripciones en cuestión se establecerán en renovación automática = false el 1 de enero de 2019.</span><span class="sxs-lookup"><span data-stu-id="554e6-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="554e6-118">Puedes mover a los clientes a un plan nuevo en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="554e6-118">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="554e6-119">Las ediciones Business de Dynamics 365 que se están retirando</span><span class="sxs-lookup"><span data-stu-id="554e6-119">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="554e6-120">Dynamics 365 for Finance and Operations，Business edition</span><span class="sxs-lookup"><span data-stu-id="554e6-120">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="554e6-121">Dynamics 365 的商務小組成員版本</span><span class="sxs-lookup"><span data-stu-id="554e6-121">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="554e6-122">Dynamics Business central: las ofertas nuevas de Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="554e6-122">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="554e6-123">Con las nuevas ofertas de Dynamics Business central, sus clientes pueden conectar sus finanzas, ventas, servicios y operaciones para simplificar los procesos empresariales, mejorar las interacciones de los clientes y tomar mejores decisiones.</span><span class="sxs-lookup"><span data-stu-id="554e6-123">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="554e6-124">Dynamics 365 Business central se basa en la nube y está disponible a través de los asociados de programas del proveedor de soluciones en la nube (CSP).</span><span class="sxs-lookup"><span data-stu-id="554e6-124">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="554e6-125">Los clientes de Dynamics 365 Business Edition pueden recibir precios de transición con descuento para las nuevas ofertas de Business central hasta el 30 de junio de 2020.</span><span class="sxs-lookup"><span data-stu-id="554e6-125">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="554e6-126">Pasar a los clientes a nuevos planes de producto</span><span class="sxs-lookup"><span data-stu-id="554e6-126">Transition customers to new product plans</span></span>

 <span data-ttu-id="554e6-127">El traslado de los clientes de las SKU retiradas a otras más recientes requiere los pasos siguientes en este orden:</span><span class="sxs-lookup"><span data-stu-id="554e6-127">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="554e6-128">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="554e6-128">Purchase the new subscription</span></span>
- <span data-ttu-id="554e6-129">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="554e6-129">Reassign current user licenses</span></span>
- <span data-ttu-id="554e6-130">Cancelar suscripción antigua</span><span class="sxs-lookup"><span data-stu-id="554e6-130">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="554e6-131">Compre el nuevo plan para su cliente</span><span class="sxs-lookup"><span data-stu-id="554e6-131">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="554e6-132">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que desea desplazar a la nueva suscripción.</span><span class="sxs-lookup"><span data-stu-id="554e6-132">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="554e6-133">Seleccione **Agregar suscripción**.</span><span class="sxs-lookup"><span data-stu-id="554e6-133">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="554e6-134">Selecciona la suscripción que quieras adquirir del catálogo (en este caso, una de las opciones que se indican más arriba), escribe el número de licencias y, a continuación, **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="554e6-134">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="554e6-135">El cliente tendrá ahora la suscripción antigua y la nueva.</span><span class="sxs-lookup"><span data-stu-id="554e6-135">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="554e6-136">El siguiente paso consiste en volver a asignar las licencias a los usuarios del cliente.</span><span class="sxs-lookup"><span data-stu-id="554e6-136">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="554e6-137">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="554e6-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="554e6-138">Selecciona **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="554e6-138">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="554e6-139">Para reasignar una licencia a un usuario, seleccione el usuario y, a continuación, seleccione **administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="554e6-139">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="554e6-140">En la página **administrar licencias** , desactive la casilla Dynamics 365 for sales/Customer Engagement plan from Basic (oferta calificada) y seleccione un nuevo plan de servicio para la suscripción a la que está pasando el cliente.</span><span class="sxs-lookup"><span data-stu-id="554e6-140">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="554e6-141">選取 **\[提交\]** 。</span><span class="sxs-lookup"><span data-stu-id="554e6-141">Select **Submit**.</span></span> <span data-ttu-id="554e6-142">Lo hará para cada usuario que necesite la nueva licencia.</span><span class="sxs-lookup"><span data-stu-id="554e6-142">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="554e6-143">Una vez que haya migrado las licencias a la nueva suscripción, puede cancelar la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="554e6-143">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="554e6-144">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="554e6-144">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="554e6-145">En la página de detalles de la suscripción, establezca la suscripción antigua en **Suspended** y seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="554e6-145">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="554e6-146">La suscripción anterior se ha suspendido y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="554e6-146">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="554e6-147">Se cancelará el aprovisionamiento de la suscripción suspendida automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="554e6-147">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="554e6-148">El cliente no incurrirá en costos adicionales por la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="554e6-148">Your customer will incur no additional costs for the old subscription.</span></span>
