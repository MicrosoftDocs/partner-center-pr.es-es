---
title: Migración de suscripciones de Dynamics 365 válidas
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo migrar desde suscripciones básicas de Dynamics 365 a una nueva suscripción antes de que expiren las suscripciones existentes.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 363c97b8c2b62e8d6b62cbe3b2807fb3c0ef3e38
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132747"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="fcf2e-103">Migrar Dynamics 365 y Customer Engagement Plan de las versiones básicas (ofertas aptas) a las versiones más recientes</span><span class="sxs-lookup"><span data-stu-id="fcf2e-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="fcf2e-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="fcf2e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="fcf2e-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="fcf2e-105">Global admin</span></span>
- <span data-ttu-id="fcf2e-106">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="fcf2e-106">User management admin</span></span>
- <span data-ttu-id="fcf2e-107">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="fcf2e-107">Admin agent</span></span>
- <span data-ttu-id="fcf2e-108">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="fcf2e-108">Sales agent</span></span>

<span data-ttu-id="fcf2e-109">A partir del 1 de enero de 2019, los clientes con Dynamics 365 para el plan de participación de ventas y clientes de las suscripciones básicas (ofertas calificadas) ya no podrán renovar estas ofertas heredadas. las suscripciones existentes no se renovarán automáticamente cuando expiren.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-109">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="fcf2e-110">En la página de detalles de la suscripción, el estado de la suscripción cambiará a "expira el [fecha]" de "se renueva automáticamente en [fecha]".</span><span class="sxs-lookup"><span data-stu-id="fcf2e-110">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="fcf2e-111">Para garantizar la continuidad de los clientes, debe realizar la transición de las suscripciones que van a expirar a una opción admitida, que se enumera a continuación.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-111">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="fcf2e-112">Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-112">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="fcf2e-113">Si usa la API (de la cresta o del centro de Partners), puede encontrar suscripciones que van a expirar mediante la evaluación de la fecha de finalización de la suscripción junto con la propiedad auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-113">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="fcf2e-114">Las suscripciones en cuestión se establecerán en renovación automática = false el 1 de enero de 2019.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-114">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="fcf2e-115">Puede trasladar a los clientes a un nuevo plan en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-115">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="fcf2e-116">Se están retirando las ofertas de Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="fcf2e-116">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="fcf2e-117">Dynamics 365 for sales Enterprise Edition CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="fcf2e-118">Dynamics 365 for sales Enterprise Edition CRMOL Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="fcf2e-118">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="fcf2e-119">Dynamics 365 for sales Enterprise Edition CRMOL Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="fcf2e-119">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="fcf2e-120">Dynamics 365 for sales Enterprise Edition (precios de la administración pública) CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="fcf2e-121">Dynamics 365 for sales Enterprise Edition de SA for CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="fcf2e-122">Dynamics 365 for sales Enterprise Edition de SA for CRM Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="fcf2e-122">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="fcf2e-123">Dynamics 365 for sales Enterprise Edition de SA for CRM Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="fcf2e-123">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="fcf2e-124">Dynamics 365 for sales Enterprise Edition (precios de la administración pública) de SA for CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="fcf2e-125">Dynamics 365 for sales Enterprise Edition Add-On para CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="fcf2e-126">Dynamics 365 for sales Enterprise Edition Add-On para CRM Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="fcf2e-126">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="fcf2e-127">Dynamics 365 for sales Enterprise Edition Add-On para CRM Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="fcf2e-127">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="fcf2e-128">Dynamics 365 for sales Enterprise Edition (precios para la administración pública) Add-On para CRM básico (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-128">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="fcf2e-129">Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="fcf2e-130">Dynamics 365 Customer Engagement plan Enterprise Edition (precios para la administración pública) CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="fcf2e-131">Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="fcf2e-131">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="fcf2e-132">Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="fcf2e-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="fcf2e-133">Dynamics 365 Customer Engagement plan Enterprise Edition de SA for CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="fcf2e-134">Dynamics 365 Customer Engagement plan Enterprise Edition (precios de la administración pública) de SA for CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="fcf2e-135">Dynamics 365 Customer Engagement plan Enterprise Edition de SA for CRM Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="fcf2e-135">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="fcf2e-136">Dynamics 365 Customer Engagement plan Enterprise Edition de SA for CRM Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="fcf2e-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="fcf2e-137">Dynamics 365 Customer Engagement plan Enterprise Edition Add-On para CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="fcf2e-138">Dynamics 365 Customer Engagement plan Enterprise Edition (precios para la administración pública) Add-On para CRM básico (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-138">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="fcf2e-139">Dynamics 365 Customer Engagement plan Enterprise Edition Add-On para CRM Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="fcf2e-139">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="fcf2e-140">Dynamics 365 Customer Engagement plan Enterprise Edition Add-On para CRM Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="fcf2e-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="fcf2e-141">Dynamics 365 for sales/Customer Engagement plan from Basic (ofertas calificadas) planes de reemplazo</span><span class="sxs-lookup"><span data-stu-id="fcf2e-141">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="fcf2e-142">**Ofertas retiradas**</span><span class="sxs-lookup"><span data-stu-id="fcf2e-142">**Retired offers**</span></span>   

- <span data-ttu-id="fcf2e-143">Dynamics 365 para ventas de CRM Basic o CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-143">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="fcf2e-144">Plan de Dynamics 365 Customer Engagement de CRM Basic o CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-144">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="fcf2e-145">**Opciones de reemplazo**</span><span class="sxs-lookup"><span data-stu-id="fcf2e-145">**Replacement options**</span></span>
- <span data-ttu-id="fcf2e-146">Dynamics 365 for sales Professional (nuevo)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-146">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="fcf2e-147">Dynamics 365 for sales Professional (nuevo)</span><span class="sxs-lookup"><span data-stu-id="fcf2e-147">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="fcf2e-148">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="fcf2e-148">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="fcf2e-149">Plan de Dynamics 365 Customer Engagement o</span><span class="sxs-lookup"><span data-stu-id="fcf2e-149">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="fcf2e-150">Miembros del equipo de Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="fcf2e-150">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="fcf2e-151">Clientes de transición hacia los nuevos planes de productos</span><span class="sxs-lookup"><span data-stu-id="fcf2e-151">Transition customers to new product plans</span></span>

<span data-ttu-id="fcf2e-152">El traslado de los clientes de las SKU retiradas a otras más recientes requiere los pasos siguientes en este orden:</span><span class="sxs-lookup"><span data-stu-id="fcf2e-152">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="fcf2e-153">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="fcf2e-153">Purchase the new subscription</span></span>
- <span data-ttu-id="fcf2e-154">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="fcf2e-154">Reassign current user licenses</span></span>
- <span data-ttu-id="fcf2e-155">Cancelar suscripción anterior</span><span class="sxs-lookup"><span data-stu-id="fcf2e-155">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="fcf2e-156">Compre el nuevo plan para su cliente</span><span class="sxs-lookup"><span data-stu-id="fcf2e-156">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="fcf2e-157">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que desea desplazar a la nueva suscripción.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-157">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="fcf2e-158">Seleccione **Agregar suscripción**.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-158">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="fcf2e-159">Seleccione la suscripción que desea comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="fcf2e-159">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="fcf2e-160">El cliente tendrá ahora la suscripción antigua y la nueva.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-160">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="fcf2e-161">El siguiente paso consiste en volver a asignar las licencias a los usuarios del cliente.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-161">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="fcf2e-162">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-162">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="fcf2e-163">Seleccione **usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-163">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="fcf2e-164">Para reasignar una licencia a un usuario, seleccione el usuario y, a continuación, seleccione **administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-164">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="fcf2e-165">En la página **administrar licencias** , desactive la casilla Dynamics 365 for sales/Customer Engagement plan from Basic (oferta calificada) y seleccione un nuevo plan de servicio para la suscripción a la que está pasando el cliente.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-165">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="fcf2e-166">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="fcf2e-166">Select **Submit**.</span></span> <span data-ttu-id="fcf2e-167">Lo hará para cada usuario que necesite la nueva licencia.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-167">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="fcf2e-168">Una vez que haya migrado las licencias a la nueva suscripción, puede cancelar la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-168">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="fcf2e-169">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-169">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="fcf2e-170">En la página de detalles de la suscripción, establezca la suscripción antigua en **Suspended** y seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="fcf2e-170">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="fcf2e-171">La suscripción anterior se ha suspendido y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-171">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="fcf2e-172">La suscripción suspendida se desaprovisionará automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-172">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="fcf2e-173">El cliente no incurrirá en costos adicionales por la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="fcf2e-173">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



