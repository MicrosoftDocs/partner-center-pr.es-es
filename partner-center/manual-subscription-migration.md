---
title: Migre Dynamics 365 y el plan de participación del cliente de las ofertas básicas (calificadas) a las versiones más recientes | Centro de Partners
ms.topic: article
ms.date: 12/12/2018
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo comprar una suscripción nueva antes de que expiren los existentes, reasigne licencias de usuario y, a continuación, cancele la suscripción anterior.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Ofertas de Dynamics 365, renovar ofertas, nuevas SKU de Dynamics 365
ms.openlocfilehash: 466f954af05a266fccba587007565e5d19d3af15
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004597"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="d5dea-104">Migrar Dynamics 365 y el plan Customer Engagement desde las versiones básicas (ofertas calificados) a versiones más recientes</span><span class="sxs-lookup"><span data-stu-id="d5dea-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="d5dea-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="d5dea-105">**Applies to**</span></span>

-  <span data-ttu-id="d5dea-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="d5dea-106">Partner Center</span></span>

<span data-ttu-id="d5dea-107">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="d5dea-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="d5dea-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d5dea-108">Global admin</span></span>
-   <span data-ttu-id="d5dea-109">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="d5dea-109">User admin</span></span>
-   <span data-ttu-id="d5dea-110">Agente de administración</span><span class="sxs-lookup"><span data-stu-id="d5dea-110">Admin agent</span></span>
-   <span data-ttu-id="d5dea-111">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="d5dea-111">Sales agent</span></span>

<span data-ttu-id="d5dea-112">A partir del 1 de enero de 2019, los clientes con Dynamics 365 para el plan de participación de ventas y clientes de las suscripciones básicas (ofertas calificadas) ya no podrán renovar estas ofertas heredadas. las suscripciones existentes no se renovarán automáticamente cuando expiren.</span><span class="sxs-lookup"><span data-stu-id="d5dea-112">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="d5dea-113">En la página de detalles de la suscripción, el estado de la suscripción cambiará a "expira el [fecha]" de "se renueva automáticamente en [fecha]".</span><span class="sxs-lookup"><span data-stu-id="d5dea-113">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="d5dea-114">Para garantizar la continuidad de los clientes, debe realizar la transición de las suscripciones que van a expirar a una opción admitida, que se enumera a continuación.</span><span class="sxs-lookup"><span data-stu-id="d5dea-114">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="d5dea-115">Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes.</span><span class="sxs-lookup"><span data-stu-id="d5dea-115">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="d5dea-116">Si usa la API (de la cresta o del centro de Partners), puede encontrar suscripciones que van a expirar mediante la evaluación de la fecha de finalización de la suscripción junto con la propiedad auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="d5dea-116">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="d5dea-117">Las suscripciones en cuestión se establecerán en renovación automática = false el 1 de enero de 2019.</span><span class="sxs-lookup"><span data-stu-id="d5dea-117">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="d5dea-118">Puedes mover a los clientes a un plan nuevo en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="d5dea-118">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="d5dea-119">Se están retirando las ofertas de Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="d5dea-119">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="d5dea-120">Dynamics 365 for sales Enterprise Edition CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="d5dea-120">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d5dea-121">Dynamics 365 for sales Enterprise Edition CRMOL Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="d5dea-121">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d5dea-122">Dynamics 365 for sales Enterprise Edition CRMOL Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="d5dea-122">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d5dea-123">Dynamics 365 for sales Enterprise Edition (precios de la administración pública) CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="d5dea-123">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d5dea-124">Dynamics 365 for sales Enterprise Edition de SA for CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="d5dea-124">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d5dea-125">Dynamics 365 for sales Enterprise Edition de SA for CRM Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="d5dea-125">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d5dea-126">Dynamics 365 for sales Enterprise Edition de SA for CRM Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="d5dea-126">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d5dea-127">Dynamics 365 for sales Enterprise Edition (precios de la administración pública) de SA for CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="d5dea-127">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d5dea-128">Dynamics 365 para el complemento sales Enterprise Edition para CRM básico (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="d5dea-128">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d5dea-129">Dynamics 365 para el complemento sales Enterprise Edition para CRM básico (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="d5dea-129">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d5dea-130">Dynamics 365 para el complemento sales Enterprise Edition para CRM básico (oferta completa) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="d5dea-130">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d5dea-131">Complemento Dynamics 365 for sales Enterprise Edition (precios para la administración pública) para CRM básico (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="d5dea-131">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d5dea-132">Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="d5dea-132">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d5dea-133">Dynamics 365 Customer Engagement plan Enterprise Edition (precios para la administración pública) CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="d5dea-133">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d5dea-134">Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="d5dea-134">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d5dea-135">Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="d5dea-135">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d5dea-136">Dynamics 365 Customer Engagement plan Enterprise Edition de SA for CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="d5dea-136">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d5dea-137">Dynamics 365 Customer Engagement plan Enterprise Edition (precios de la administración pública) de SA for CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="d5dea-137">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d5dea-138">Dynamics 365 Customer Engagement plan Enterprise Edition de SA for CRM Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="d5dea-138">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d5dea-139">Dynamics 365 Customer Engagement plan Enterprise Edition de SA for CRM Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="d5dea-139">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="d5dea-140">Complemento de Dynamics 365 Customer Engagement plan Enterprise Edition para CRM básico (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="d5dea-140">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d5dea-141">Complemento de Dynamics 365 Customer Engagement plan Enterprise Edition (precios para la administración pública) para CRM básico (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="d5dea-141">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d5dea-142">Complemento de Dynamics 365 Customer Engagement plan Enterprise Edition para CRM básico (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="d5dea-142">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="d5dea-143">Complemento de Dynamics 365 Customer Engagement plan Enterprise Edition para CRM básico (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="d5dea-143">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="d5dea-144">Dynamics 365 for sales/Customer Engagement plan from Basic (ofertas calificadas) planes de reemplazo</span><span class="sxs-lookup"><span data-stu-id="d5dea-144">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="d5dea-145">**Ofertas retiradas**</span><span class="sxs-lookup"><span data-stu-id="d5dea-145">**Retired offers**</span></span>   

- <span data-ttu-id="d5dea-146">Dynamics 365 para ventas de CRM Basic o CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="d5dea-146">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="d5dea-147">Plan de Dynamics 365 Customer Engagement de CRM Basic o CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="d5dea-147">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="d5dea-148">**Opciones de reemplazo**</span><span class="sxs-lookup"><span data-stu-id="d5dea-148">**Replacement options**</span></span>
- <span data-ttu-id="d5dea-149">Dynamics 365 for sales Professional (nuevo)</span><span class="sxs-lookup"><span data-stu-id="d5dea-149">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="d5dea-150">Dynamics 365 for sales Professional (nuevo)</span><span class="sxs-lookup"><span data-stu-id="d5dea-150">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="d5dea-151">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="d5dea-151">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="d5dea-152">Plan de Dynamics 365 Customer Engagement o</span><span class="sxs-lookup"><span data-stu-id="d5dea-152">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="d5dea-153">Miembros del equipo de Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="d5dea-153">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="d5dea-154">Pasar a los clientes a nuevos planes de producto</span><span class="sxs-lookup"><span data-stu-id="d5dea-154">Transition customers to new product plans</span></span>

<span data-ttu-id="d5dea-155">El traslado de los clientes de las SKU retiradas a otras más recientes requiere los pasos siguientes en este orden:</span><span class="sxs-lookup"><span data-stu-id="d5dea-155">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="d5dea-156">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="d5dea-156">Purchase the new subscription</span></span>
- <span data-ttu-id="d5dea-157">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="d5dea-157">Reassign current user licenses</span></span>
- <span data-ttu-id="d5dea-158">Cancelar suscripción antigua</span><span class="sxs-lookup"><span data-stu-id="d5dea-158">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="d5dea-159">Compre el nuevo plan para su cliente</span><span class="sxs-lookup"><span data-stu-id="d5dea-159">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="d5dea-160">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que desea desplazar a la nueva suscripción.</span><span class="sxs-lookup"><span data-stu-id="d5dea-160">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="d5dea-161">Seleccione **Agregar suscripción**.</span><span class="sxs-lookup"><span data-stu-id="d5dea-161">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="d5dea-162">Selecciona la suscripción que quieras adquirir del catálogo (en este caso, una de las opciones que se indican más arriba), escribe el número de licencias y, a continuación, **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="d5dea-162">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="d5dea-163">El cliente tendrá ahora la suscripción antigua y la nueva.</span><span class="sxs-lookup"><span data-stu-id="d5dea-163">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="d5dea-164">El siguiente paso consiste en volver a asignar las licencias a los usuarios del cliente.</span><span class="sxs-lookup"><span data-stu-id="d5dea-164">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="d5dea-165">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="d5dea-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="d5dea-166">Selecciona **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="d5dea-166">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="d5dea-167">Para reasignar una licencia a un usuario, seleccione el usuario y, a continuación, seleccione **administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="d5dea-167">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="d5dea-168">En la página **administrar licencias** , desactive la casilla Dynamics 365 for sales/Customer Engagement plan from Basic (oferta calificada) y seleccione un nuevo plan de servicio para la suscripción a la que está pasando el cliente.</span><span class="sxs-lookup"><span data-stu-id="d5dea-168">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="d5dea-169">Selecciona **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="d5dea-169">Select **Submit**.</span></span> <span data-ttu-id="d5dea-170">Lo hará para cada usuario que necesite la nueva licencia.</span><span class="sxs-lookup"><span data-stu-id="d5dea-170">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="d5dea-171">Una vez que haya migrado las licencias a la nueva suscripción, puede cancelar la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="d5dea-171">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="d5dea-172">Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="d5dea-172">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="d5dea-173">En la página de detalles de la suscripción, establezca la suscripción antigua en **Suspended** y seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="d5dea-173">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="d5dea-174">La suscripción anterior se ha suspendido y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="d5dea-174">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="d5dea-175">Se cancelará el aprovisionamiento de la suscripción suspendida automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="d5dea-175">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="d5dea-176">El cliente no incurrirá en costos adicionales por la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="d5dea-176">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



