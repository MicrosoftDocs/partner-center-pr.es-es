---
title: Migración de suscripciones de Dynamics 365 válidas
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo migrar desde suscripciones básicas de Dynamics 365 a una nueva suscripción antes de que expiren las suscripciones existentes.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Ofertas de Dynamics 365, renovar ofertas, nuevas SKU de Dynamics 365
ms.openlocfilehash: cac5717a1f7b27537faa694dcf665a69a7226483
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795993"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="aa062-104">Migrar Dynamics 365 y Customer Engagement Plan de las versiones básicas (ofertas aptas) a las versiones más recientes</span><span class="sxs-lookup"><span data-stu-id="aa062-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="aa062-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="aa062-105">**Applies to**</span></span>

-  <span data-ttu-id="aa062-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="aa062-106">Partner Center</span></span>

<span data-ttu-id="aa062-107">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="aa062-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="aa062-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="aa062-108">Global admin</span></span>
-   <span data-ttu-id="aa062-109">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="aa062-109">User admin</span></span>
-   <span data-ttu-id="aa062-110">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="aa062-110">Admin agent</span></span>
-   <span data-ttu-id="aa062-111">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="aa062-111">Sales agent</span></span>

<span data-ttu-id="aa062-112">A partir del 1 de enero de 2019, los clientes con Dynamics 365 para el plan de participación de ventas y clientes de las suscripciones básicas (ofertas calificadas) ya no podrán renovar estas ofertas heredadas. las suscripciones existentes no se renovarán automáticamente cuando expiren.</span><span class="sxs-lookup"><span data-stu-id="aa062-112">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="aa062-113">En la página de detalles de la suscripción, el estado de la suscripción cambiará a "expira el [fecha]" de "se renueva automáticamente en [fecha]".</span><span class="sxs-lookup"><span data-stu-id="aa062-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="aa062-114">Para garantizar la continuidad de los clientes, debe realizar la transición de las suscripciones que van a expirar a una opción admitida, que se enumera a continuación.</span><span class="sxs-lookup"><span data-stu-id="aa062-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="aa062-115">Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes.</span><span class="sxs-lookup"><span data-stu-id="aa062-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="aa062-116">Si usa la API (de la cresta o del centro de Partners), puede encontrar suscripciones que van a expirar mediante la evaluación de la fecha de finalización de la suscripción junto con la propiedad auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="aa062-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="aa062-117">Las suscripciones en cuestión se establecerán en renovación automática = false el 1 de enero de 2019.</span><span class="sxs-lookup"><span data-stu-id="aa062-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="aa062-118">Puede trasladar a los clientes a un nuevo plan en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="aa062-118">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="aa062-119">Se están retirando las ofertas de Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="aa062-119">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="aa062-120">Dynamics 365 for sales Enterprise Edition CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="aa062-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="aa062-121">Dynamics 365 for sales Enterprise Edition CRMOL Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="aa062-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="aa062-122">Dynamics 365 for sales Enterprise Edition CRMOL Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="aa062-122">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="aa062-123">Dynamics 365 for sales Enterprise Edition (precios de la administración pública) CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="aa062-123">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="aa062-124">Dynamics 365 for sales Enterprise Edition de SA for CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="aa062-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="aa062-125">Dynamics 365 for sales Enterprise Edition de SA for CRM Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="aa062-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="aa062-126">Dynamics 365 for sales Enterprise Edition de SA for CRM Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="aa062-126">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="aa062-127">Dynamics 365 for sales Enterprise Edition (precios de la administración pública) de SA for CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="aa062-127">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="aa062-128">Dynamics 365 para el complemento sales Enterprise Edition para CRM básico (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="aa062-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="aa062-129">Dynamics 365 para el complemento sales Enterprise Edition para CRM básico (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="aa062-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="aa062-130">Dynamics 365 para el complemento sales Enterprise Edition para CRM básico (oferta completa) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="aa062-130">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="aa062-131">Complemento Dynamics 365 for sales Enterprise Edition (precios para la administración pública) para CRM básico (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="aa062-131">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="aa062-132">Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="aa062-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="aa062-133">Dynamics 365 Customer Engagement plan Enterprise Edition (precios para la administración pública) CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="aa062-133">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="aa062-134">Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="aa062-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="aa062-135">Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="aa062-135">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="aa062-136">Dynamics 365 Customer Engagement plan Enterprise Edition de SA for CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="aa062-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="aa062-137">Dynamics 365 Customer Engagement plan Enterprise Edition (precios de la administración pública) de SA for CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="aa062-137">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="aa062-138">Dynamics 365 Customer Engagement plan Enterprise Edition de SA for CRM Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="aa062-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="aa062-139">Dynamics 365 Customer Engagement plan Enterprise Edition de SA for CRM Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="aa062-139">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="aa062-140">Complemento de Dynamics 365 Customer Engagement plan Enterprise Edition para CRM básico (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="aa062-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="aa062-141">Complemento de Dynamics 365 Customer Engagement plan Enterprise Edition (precios para la administración pública) para CRM básico (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="aa062-141">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="aa062-142">Complemento de Dynamics 365 Customer Engagement plan Enterprise Edition para CRM básico (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="aa062-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="aa062-143">Complemento de Dynamics 365 Customer Engagement plan Enterprise Edition para CRM básico (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="aa062-143">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="aa062-144">Dynamics 365 for sales/Customer Engagement plan from Basic (ofertas calificadas) planes de reemplazo</span><span class="sxs-lookup"><span data-stu-id="aa062-144">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="aa062-145">**Ofertas retiradas**</span><span class="sxs-lookup"><span data-stu-id="aa062-145">**Retired offers**</span></span>   

- <span data-ttu-id="aa062-146">Dynamics 365 para ventas de CRM Basic o CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="aa062-146">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="aa062-147">Plan de Dynamics 365 Customer Engagement de CRM Basic o CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="aa062-147">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="aa062-148">**Opciones de reemplazo**</span><span class="sxs-lookup"><span data-stu-id="aa062-148">**Replacement options**</span></span>
- <span data-ttu-id="aa062-149">Dynamics 365 for sales Professional (nuevo)</span><span class="sxs-lookup"><span data-stu-id="aa062-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="aa062-150">Dynamics 365 for sales Professional (nuevo)</span><span class="sxs-lookup"><span data-stu-id="aa062-150">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="aa062-151">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="aa062-151">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="aa062-152">Plan de Dynamics 365 Customer Engagement o</span><span class="sxs-lookup"><span data-stu-id="aa062-152">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="aa062-153">Miembros del equipo de Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="aa062-153">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="aa062-154">Clientes de transición hacia los nuevos planes de productos</span><span class="sxs-lookup"><span data-stu-id="aa062-154">Transition customers to new product plans</span></span>

<span data-ttu-id="aa062-155">El traslado de los clientes de las SKU retiradas a otras más recientes requiere los pasos siguientes en este orden:</span><span class="sxs-lookup"><span data-stu-id="aa062-155">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="aa062-156">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="aa062-156">Purchase the new subscription</span></span>
- <span data-ttu-id="aa062-157">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="aa062-157">Reassign current user licenses</span></span>
- <span data-ttu-id="aa062-158">Cancelar suscripción anterior</span><span class="sxs-lookup"><span data-stu-id="aa062-158">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="aa062-159">Compre el nuevo plan para su cliente</span><span class="sxs-lookup"><span data-stu-id="aa062-159">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="aa062-160">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que desea desplazar a la nueva suscripción.</span><span class="sxs-lookup"><span data-stu-id="aa062-160">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="aa062-161">Seleccione **Agregar suscripción**.</span><span class="sxs-lookup"><span data-stu-id="aa062-161">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="aa062-162">Seleccione la suscripción que desea comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="aa062-162">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="aa062-163">El cliente tendrá ahora la suscripción antigua y la nueva.</span><span class="sxs-lookup"><span data-stu-id="aa062-163">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="aa062-164">El siguiente paso consiste en volver a asignar las licencias a los usuarios del cliente.</span><span class="sxs-lookup"><span data-stu-id="aa062-164">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="aa062-165">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="aa062-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="aa062-166">Seleccione **usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="aa062-166">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="aa062-167">Para reasignar una licencia a un usuario, seleccione el usuario y, a continuación, seleccione **administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="aa062-167">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="aa062-168">En la página **administrar licencias** , desactive la casilla Dynamics 365 for sales/Customer Engagement plan from Basic (oferta calificada) y seleccione un nuevo plan de servicio para la suscripción a la que está pasando el cliente.</span><span class="sxs-lookup"><span data-stu-id="aa062-168">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="aa062-169">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="aa062-169">Select **Submit**.</span></span> <span data-ttu-id="aa062-170">Lo hará para cada usuario que necesite la nueva licencia.</span><span class="sxs-lookup"><span data-stu-id="aa062-170">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="aa062-171">Una vez que haya migrado las licencias a la nueva suscripción, puede cancelar la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="aa062-171">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="aa062-172">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="aa062-172">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="aa062-173">En la página de detalles de la suscripción, establezca la suscripción antigua en **Suspended** y seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="aa062-173">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="aa062-174">La suscripción anterior se ha suspendido y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="aa062-174">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="aa062-175">La suscripción suspendida se desaprovisionará automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="aa062-175">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="aa062-176">El cliente no incurrirá en costos adicionales por la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="aa062-176">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



