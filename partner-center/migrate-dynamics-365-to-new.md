---
title: Migración de Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo migrar ofertas de Dynamics 365 Business Edition a versiones más recientes antes de que expiren.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151532"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="436f4-103">Migración de ofertas de Dynamics 365 Business Edition a versiones más recientes</span><span class="sxs-lookup"><span data-stu-id="436f4-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="436f4-104">**Roles adecuados:** administrador global | Administrador de administración de | Agente de administración | Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="436f4-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="436f4-105">A partir del 1 de enero de 2019, los clientes con suscripciones de Dynamics 365 Business Edition ya no pueden renovarse en estas ofertas heredadas. Las suscripciones existentes no se renovarán automáticamente cuando expiren.</span><span class="sxs-lookup"><span data-stu-id="436f4-105">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="436f4-106">En la página de detalles de la suscripción, el estado de la suscripción cambiará a "Expira el [fecha]" de "Renovación automática el [fecha]".</span><span class="sxs-lookup"><span data-stu-id="436f4-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="436f4-107">Para garantizar la continuidad de los clientes, debe realizar la transición de los que tienen suscripciones que expiran a una opción compatible, que se muestra a continuación.</span><span class="sxs-lookup"><span data-stu-id="436f4-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="436f4-108">Se recomienda mover clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones del servicio para los clientes.</span><span class="sxs-lookup"><span data-stu-id="436f4-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="436f4-109">Si usa la API (YA SEATE o Centro de partners), puede encontrar suscripciones que expiran evaluando la fecha de finalización de la suscripción junto con la propiedad renovación automática = False.</span><span class="sxs-lookup"><span data-stu-id="436f4-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="436f4-110">Las suscripciones en cuestión se establecerán en auto renew=False el 1 de enero de 2019.</span><span class="sxs-lookup"><span data-stu-id="436f4-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="436f4-111">Puede trasladar clientes a un nuevo plan en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="436f4-111">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="436f4-112">Dynamics 365 Business Edition que se va a retirar</span><span class="sxs-lookup"><span data-stu-id="436f4-112">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="436f4-113">Dynamics 365 for Finance and Operations, Business Edition</span><span class="sxs-lookup"><span data-stu-id="436f4-113">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="436f4-114">Dynamics 365 for Team Members, edición Business</span><span class="sxs-lookup"><span data-stu-id="436f4-114">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="436f4-115">Dynamics Business Central: nuevas ofertas de Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="436f4-115">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="436f4-116">Con las nuevas ofertas de Dynamics Business Central, los clientes pueden conectar sus finanzas, ventas, servicio y operaciones para optimizar los procesos empresariales, mejorar las interacciones de los clientes y tomar mejores decisiones.</span><span class="sxs-lookup"><span data-stu-id="436f4-116">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="436f4-117">Dynamics 365 Business Central está basado en la nube y solo está disponible a través Proveedor de soluciones en la nube asociados del programa csp (CSP).</span><span class="sxs-lookup"><span data-stu-id="436f4-117">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="436f4-118">Los clientes de Dynamics 365 Business Edition pueden recibir precios de transición con descuento para las nuevas ofertas de Business Central hasta el 30 de junio de 2020.</span><span class="sxs-lookup"><span data-stu-id="436f4-118">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="436f4-119">Clientes de transición hacia los nuevos planes de productos</span><span class="sxs-lookup"><span data-stu-id="436f4-119">Transition customers to new product plans</span></span>

 <span data-ttu-id="436f4-120">El traslado de clientes de SKU retiradas a otras más recientes requiere los pasos siguientes en este orden:</span><span class="sxs-lookup"><span data-stu-id="436f4-120">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="436f4-121">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="436f4-121">Purchase the new subscription</span></span>
- <span data-ttu-id="436f4-122">Reasignación de licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="436f4-122">Reassign current user licenses</span></span>
- <span data-ttu-id="436f4-123">Cancelación de una suscripción antigua</span><span class="sxs-lookup"><span data-stu-id="436f4-123">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="436f4-124">Compra del nuevo plan para el cliente</span><span class="sxs-lookup"><span data-stu-id="436f4-124">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="436f4-125">Seleccione **Clientes** en el panel de navegación izquierdo y, a continuación, seleccione el cliente que desea trasladar a la nueva suscripción.</span><span class="sxs-lookup"><span data-stu-id="436f4-125">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="436f4-126">Seleccione **Agregar suscripción.**</span><span class="sxs-lookup"><span data-stu-id="436f4-126">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="436f4-127">Seleccione la suscripción que desea comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, **seleccione Enviar**.</span><span class="sxs-lookup"><span data-stu-id="436f4-127">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="436f4-128">El cliente tendrá ahora la suscripción anterior y la nueva.</span><span class="sxs-lookup"><span data-stu-id="436f4-128">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="436f4-129">El siguiente paso consiste en reasignar licencias a los usuarios del cliente.</span><span class="sxs-lookup"><span data-stu-id="436f4-129">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="436f4-130">Seleccione **Clientes** en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="436f4-130">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="436f4-131">Seleccione **Usuarios y licencias.**</span><span class="sxs-lookup"><span data-stu-id="436f4-131">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="436f4-132">Para reasignar una licencia a un usuario, selecciónelo y, a continuación, **seleccione Administrar licencias.**</span><span class="sxs-lookup"><span data-stu-id="436f4-132">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="436f4-133">En  la página Administrar licencias, desactive la casilla Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license (Plan de Dynamics 365 for Sales/Customer Engagement plan from Basic [Oferta calificada]) y seleccione un nuevo plan de servicio para la suscripción a la que se traslada el cliente.</span><span class="sxs-lookup"><span data-stu-id="436f4-133">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="436f4-134">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="436f4-134">Select **Submit**.</span></span> <span data-ttu-id="436f4-135">Lo hará para cada usuario que necesite la nueva licencia.</span><span class="sxs-lookup"><span data-stu-id="436f4-135">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="436f4-136">Una vez que haya movido las licencias a la nueva suscripción, puede cancelar la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="436f4-136">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="436f4-137">Seleccione **Clientes** en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="436f4-137">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="436f4-138">En la página de detalles de la suscripción, establezca la suscripción antigua en **Suspendido** y seleccione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="436f4-138">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="436f4-139">La suscripción anterior ahora está suspendida y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="436f4-139">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="436f4-140">La suscripción suspendida se desaprovisionará automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="436f4-140">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="436f4-141">El cliente no incurrirá en costos adicionales por la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="436f4-141">Your customer will incur no additional costs for the old subscription.</span></span>
