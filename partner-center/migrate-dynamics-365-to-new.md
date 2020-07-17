---
title: Migración de Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo migrar ofertas de Dynamics 365 Business Edition calificadas a versiones más recientes antes de que expiren.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d441d121c28c2762d1f1c71d6f6a1e81d089f99c
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436834"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="73e30-103">Migración de ofertas de Dynamics 365 Business Edition a versiones más recientes</span><span class="sxs-lookup"><span data-stu-id="73e30-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="73e30-104">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="73e30-104">**Applies to**</span></span>

- <span data-ttu-id="73e30-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="73e30-105">Partner Center</span></span>

<span data-ttu-id="73e30-106">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="73e30-106">**Appropriate roles**</span></span>
- <span data-ttu-id="73e30-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="73e30-107">Global admin</span></span>
- <span data-ttu-id="73e30-108">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="73e30-108">User admin</span></span>
- <span data-ttu-id="73e30-109">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="73e30-109">Admin agent</span></span>
- <span data-ttu-id="73e30-110">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="73e30-110">Sales agent</span></span>

<span data-ttu-id="73e30-111">A partir del 1 de enero de 2019, los clientes con suscripciones de Dynamics 365 Business Edition ya no podrán renovar en estas ofertas heredadas. las suscripciones existentes no se renovarán automáticamente cuando expiren.</span><span class="sxs-lookup"><span data-stu-id="73e30-111">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="73e30-112">En la página de detalles de la suscripción, el estado de la suscripción cambiará a "expira el [fecha]" de "se renueva automáticamente en [fecha]".</span><span class="sxs-lookup"><span data-stu-id="73e30-112">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="73e30-113">Para garantizar la continuidad de los clientes, debe realizar la transición de las suscripciones que van a expirar a una opción admitida, que se enumera a continuación.</span><span class="sxs-lookup"><span data-stu-id="73e30-113">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="73e30-114">Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes.</span><span class="sxs-lookup"><span data-stu-id="73e30-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="73e30-115">Si usa la API (de la cresta o del centro de Partners), puede encontrar suscripciones que van a expirar mediante la evaluación de la fecha de finalización de la suscripción junto con la propiedad auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="73e30-115">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="73e30-116">Las suscripciones en cuestión se establecerán en renovación automática = false el 1 de enero de 2019.</span><span class="sxs-lookup"><span data-stu-id="73e30-116">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="73e30-117">Puede trasladar a los clientes a un nuevo plan en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="73e30-117">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="73e30-118">Las ediciones Business de Dynamics 365 que se están retirando</span><span class="sxs-lookup"><span data-stu-id="73e30-118">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="73e30-119">Dynamics 365 for Finance and Operations, Business Edition</span><span class="sxs-lookup"><span data-stu-id="73e30-119">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="73e30-120">Dynamics 365 for Team Members, edición Business</span><span class="sxs-lookup"><span data-stu-id="73e30-120">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="73e30-121">Dynamics Business central: las ofertas nuevas de Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="73e30-121">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="73e30-122">Con las nuevas ofertas de Dynamics Business central, sus clientes pueden conectar sus finanzas, ventas, servicios y operaciones para simplificar los procesos empresariales, mejorar las interacciones de los clientes y tomar mejores decisiones.</span><span class="sxs-lookup"><span data-stu-id="73e30-122">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="73e30-123">Dynamics 365 Business central se basa en la nube y está disponible a través de los asociados de programas del proveedor de soluciones en la nube (CSP).</span><span class="sxs-lookup"><span data-stu-id="73e30-123">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="73e30-124">Los clientes de Dynamics 365 Business Edition pueden recibir precios de transición con descuento para las nuevas ofertas de Business central hasta el 30 de junio de 2020.</span><span class="sxs-lookup"><span data-stu-id="73e30-124">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="73e30-125">Clientes de transición hacia los nuevos planes de productos</span><span class="sxs-lookup"><span data-stu-id="73e30-125">Transition customers to new product plans</span></span>

 <span data-ttu-id="73e30-126">El traslado de los clientes de las SKU retiradas a otras más recientes requiere los pasos siguientes en este orden:</span><span class="sxs-lookup"><span data-stu-id="73e30-126">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="73e30-127">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="73e30-127">Purchase the new subscription</span></span>
- <span data-ttu-id="73e30-128">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="73e30-128">Reassign current user licenses</span></span>
- <span data-ttu-id="73e30-129">Cancelar suscripción anterior</span><span class="sxs-lookup"><span data-stu-id="73e30-129">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="73e30-130">Compre el nuevo plan para su cliente</span><span class="sxs-lookup"><span data-stu-id="73e30-130">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="73e30-131">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que desea desplazar a la nueva suscripción.</span><span class="sxs-lookup"><span data-stu-id="73e30-131">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="73e30-132">Seleccione **Agregar suscripción**.</span><span class="sxs-lookup"><span data-stu-id="73e30-132">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="73e30-133">Seleccione la suscripción que desea comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="73e30-133">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="73e30-134">El cliente tendrá ahora la suscripción antigua y la nueva.</span><span class="sxs-lookup"><span data-stu-id="73e30-134">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="73e30-135">El siguiente paso consiste en volver a asignar las licencias a los usuarios del cliente.</span><span class="sxs-lookup"><span data-stu-id="73e30-135">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="73e30-136">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="73e30-136">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="73e30-137">Seleccione **usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="73e30-137">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="73e30-138">Para reasignar una licencia a un usuario, seleccione el usuario y, a continuación, seleccione **administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="73e30-138">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="73e30-139">En la página **administrar licencias** , desactive la casilla Dynamics 365 for sales/Customer Engagement plan from Basic (oferta calificada) y seleccione un nuevo plan de servicio para la suscripción a la que está pasando el cliente.</span><span class="sxs-lookup"><span data-stu-id="73e30-139">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="73e30-140">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="73e30-140">Select **Submit**.</span></span> <span data-ttu-id="73e30-141">Lo hará para cada usuario que necesite la nueva licencia.</span><span class="sxs-lookup"><span data-stu-id="73e30-141">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="73e30-142">Una vez que haya migrado las licencias a la nueva suscripción, puede cancelar la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="73e30-142">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="73e30-143">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="73e30-143">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="73e30-144">En la página de detalles de la suscripción, establezca la suscripción antigua en **Suspended** y seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="73e30-144">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="73e30-145">La suscripción anterior se ha suspendido y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="73e30-145">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="73e30-146">La suscripción suspendida se desaprovisionará automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="73e30-146">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="73e30-147">El cliente no incurrirá en costos adicionales por la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="73e30-147">Your customer will incur no additional costs for the old subscription.</span></span>
