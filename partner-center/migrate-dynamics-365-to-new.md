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
ms.openlocfilehash: e83c06c11638bdde508fd27904038bcb6d8c9e9c
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132645"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a><span data-ttu-id="62219-103">Migración de ofertas de Dynamics 365 Business Edition a versiones más recientes</span><span class="sxs-lookup"><span data-stu-id="62219-103">Migrate Dynamics 365 Business Edition Offers to newer versions</span></span>

<span data-ttu-id="62219-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="62219-104">**Appropriate roles**</span></span>

- <span data-ttu-id="62219-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="62219-105">Global admin</span></span>
- <span data-ttu-id="62219-106">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="62219-106">User management admin</span></span>
- <span data-ttu-id="62219-107">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="62219-107">Admin agent</span></span>
- <span data-ttu-id="62219-108">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="62219-108">Sales agent</span></span>

<span data-ttu-id="62219-109">A partir del 1 de enero de 2019, los clientes con suscripciones de Dynamics 365 Business Edition ya no podrán renovar en estas ofertas heredadas. las suscripciones existentes no se renovarán automáticamente cuando expiren.</span><span class="sxs-lookup"><span data-stu-id="62219-109">Effective January 1, 2019, customers with Dynamics 365 Business Edition subscriptions can no longer renew into these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="62219-110">En la página de detalles de la suscripción, el estado de la suscripción cambiará a "expira el [fecha]" de "se renueva automáticamente en [fecha]".</span><span class="sxs-lookup"><span data-stu-id="62219-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span>

<span data-ttu-id="62219-111">Para garantizar la continuidad de los clientes, debe realizar la transición de las suscripciones que van a expirar a una opción admitida, que se enumera a continuación.</span><span class="sxs-lookup"><span data-stu-id="62219-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="62219-112">Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes.</span><span class="sxs-lookup"><span data-stu-id="62219-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="62219-113">Si usa la API (de la cresta o del centro de Partners), puede encontrar suscripciones que van a expirar mediante la evaluación de la fecha de finalización de la suscripción junto con la propiedad auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="62219-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="62219-114">Las suscripciones en cuestión se establecerán en renovación automática = false el 1 de enero de 2019.</span><span class="sxs-lookup"><span data-stu-id="62219-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="62219-115">Puede trasladar a los clientes a un nuevo plan en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="62219-115">You can move customers to a new plan at any time.</span></span> 

## <a name="the-dynamics-365-business-editions-being-retired"></a><span data-ttu-id="62219-116">Las ediciones Business de Dynamics 365 que se están retirando</span><span class="sxs-lookup"><span data-stu-id="62219-116">The Dynamics 365 Business Editions being retired</span></span>

- <span data-ttu-id="62219-117">Dynamics 365 for Finance and Operations, Business Edition</span><span class="sxs-lookup"><span data-stu-id="62219-117">Dynamics 365 for Finance and Operations, Business edition</span></span>
- <span data-ttu-id="62219-118">Dynamics 365 for Team Members, edición Business</span><span class="sxs-lookup"><span data-stu-id="62219-118">Dynamics 365 for Team Members, Business edition</span></span>

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a><span data-ttu-id="62219-119">Dynamics Business central: las ofertas nuevas de Dynamics 365 Business Edition</span><span class="sxs-lookup"><span data-stu-id="62219-119">Dynamics Business Central - the Dynamics 365 Business Edition new offers</span></span>

<span data-ttu-id="62219-120">Con las nuevas ofertas de Dynamics Business central, sus clientes pueden conectar sus finanzas, ventas, servicios y operaciones para simplificar los procesos empresariales, mejorar las interacciones de los clientes y tomar mejores decisiones.</span><span class="sxs-lookup"><span data-stu-id="62219-120">With the new Dynamics Business Central offers, your customers can connect their financials, sales, service, and operations to streamline business processes, improve customer interactions, and make better decisions.</span></span> <span data-ttu-id="62219-121">Dynamics 365 Business central se basa en la nube y está disponible a través de los asociados de programas del proveedor de soluciones en la nube (CSP).</span><span class="sxs-lookup"><span data-stu-id="62219-121">Dynamics 365 Business Central is cloud-based and available through Cloud Solution Provider (CSP) program partners only.</span></span>
<span data-ttu-id="62219-122">Los clientes de Dynamics 365 Business Edition pueden recibir precios de transición con descuento para las nuevas ofertas de Business central hasta el 30 de junio de 2020.</span><span class="sxs-lookup"><span data-stu-id="62219-122">Dynamics 365 Business Edition customers are eligible to receive discounted transition pricing for the new Business Central offers until June 30, 2020.</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="62219-123">Clientes de transición hacia los nuevos planes de productos</span><span class="sxs-lookup"><span data-stu-id="62219-123">Transition customers to new product plans</span></span>

 <span data-ttu-id="62219-124">El traslado de los clientes de las SKU retiradas a otras más recientes requiere los pasos siguientes en este orden:</span><span class="sxs-lookup"><span data-stu-id="62219-124">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="62219-125">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="62219-125">Purchase the new subscription</span></span>
- <span data-ttu-id="62219-126">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="62219-126">Reassign current user licenses</span></span>
- <span data-ttu-id="62219-127">Cancelar suscripción anterior</span><span class="sxs-lookup"><span data-stu-id="62219-127">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="62219-128">Compre el nuevo plan para su cliente</span><span class="sxs-lookup"><span data-stu-id="62219-128">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="62219-129">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que desea desplazar a la nueva suscripción.</span><span class="sxs-lookup"><span data-stu-id="62219-129">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="62219-130">Seleccione **Agregar suscripción**.</span><span class="sxs-lookup"><span data-stu-id="62219-130">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="62219-131">Seleccione la suscripción que desea comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="62219-131">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="62219-132">El cliente tendrá ahora la suscripción antigua y la nueva.</span><span class="sxs-lookup"><span data-stu-id="62219-132">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="62219-133">El siguiente paso consiste en volver a asignar las licencias a los usuarios del cliente.</span><span class="sxs-lookup"><span data-stu-id="62219-133">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="62219-134">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="62219-134">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="62219-135">Seleccione **usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="62219-135">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="62219-136">Para reasignar una licencia a un usuario, seleccione el usuario y, a continuación, seleccione **administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="62219-136">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="62219-137">En la página **administrar licencias** , desactive la casilla Dynamics 365 for sales/Customer Engagement plan from Basic (oferta calificada) y seleccione un nuevo plan de servicio para la suscripción a la que está pasando el cliente.</span><span class="sxs-lookup"><span data-stu-id="62219-137">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="62219-138">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="62219-138">Select **Submit**.</span></span> <span data-ttu-id="62219-139">Lo hará para cada usuario que necesite la nueva licencia.</span><span class="sxs-lookup"><span data-stu-id="62219-139">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="62219-140">Una vez que haya migrado las licencias a la nueva suscripción, puede cancelar la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="62219-140">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="62219-141">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="62219-141">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="62219-142">En la página de detalles de la suscripción, establezca la suscripción antigua en **Suspended** y seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="62219-142">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="62219-143">La suscripción anterior se ha suspendido y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="62219-143">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="62219-144">La suscripción suspendida se desaprovisionará automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="62219-144">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="62219-145">El cliente no incurrirá en costos adicionales por la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="62219-145">Your customer will incur no additional costs for the old subscription.</span></span>
