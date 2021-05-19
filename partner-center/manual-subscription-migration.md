---
title: Migración de suscripciones de Dynamics 365 calificadas
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo migrar de suscripciones de Dynamics 365 básicas y calificadas a una nueva suscripción antes de que expiren las suscripciones existentes.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151651"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="37673-103">Migrar Dynamics 365 y Customer Engagement Plan de las versiones básicas (ofertas aptas) a las versiones más recientes</span><span class="sxs-lookup"><span data-stu-id="37673-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="37673-104">**Roles adecuados:** administrador global | Administrador de administración de | Agente de administración | Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="37673-104">**Appropriate roles**: Global admin | User management admin | Admin agent | Sales agent</span></span>

<span data-ttu-id="37673-105">A partir del 1 de enero de 2019, los clientes con Dynamics 365 for Sales/Customer Engagement Plan de suscripciones básicas (ofertas calificadas) ya no podrán renovar estas ofertas heredadas. Las suscripciones existentes no se renovarán automáticamente cuando expiren.</span><span class="sxs-lookup"><span data-stu-id="37673-105">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="37673-106">En la página de detalles de la suscripción, el estado de la suscripción cambiará a "Expira el [fecha]" de "Renovación automática el [fecha]".</span><span class="sxs-lookup"><span data-stu-id="37673-106">On the subscription's detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="37673-107">Para garantizar la continuidad de los clientes, debe realizar la transición de los que tienen suscripciones que expiran a una opción compatible, que se muestra a continuación.</span><span class="sxs-lookup"><span data-stu-id="37673-107">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="37673-108">Se recomienda mover clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones del servicio para los clientes.</span><span class="sxs-lookup"><span data-stu-id="37673-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="37673-109">Si usa la API (YA SEATE o Centro de partners), puede encontrar suscripciones que expiran evaluando la fecha de finalización de la suscripción junto con la propiedad renovación automática = False.</span><span class="sxs-lookup"><span data-stu-id="37673-109">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="37673-110">Las suscripciones en cuestión se establecerán en auto renew=False el 1 de enero de 2019.</span><span class="sxs-lookup"><span data-stu-id="37673-110">The subscriptions in question will be set to auto renew=False on January 1, 2019.</span></span> <span data-ttu-id="37673-111">Puede trasladar clientes a un nuevo plan en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="37673-111">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="37673-112">Las ofertas de Dynamics 365 que se retiran</span><span class="sxs-lookup"><span data-stu-id="37673-112">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="37673-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="37673-113">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="37673-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="37673-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="37673-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="37673-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="37673-116">Dynamics 365 for Sales Enterprise Edition (precios gubernamentales) CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="37673-116">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="37673-117">Dynamics 365 for Sales Enterprise Edition from SA for CRM Basic (Oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="37673-117">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="37673-118">Dynamics 365 for Sales Enterprise Edition from SA for CRM Basic (Oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="37673-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="37673-119">Dynamics 365 for Sales Enterprise Edition from SA for CRM Basic (Oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="37673-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="37673-120">Dynamics 365 for Sales Enterprise Edition (precios gubernamentales) de SA para CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="37673-120">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="37673-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="37673-121">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="37673-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="37673-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="37673-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="37673-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="37673-124">Dynamics 365 for Sales Enterprise Edition (precios gubernamentales) Add-On para CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="37673-124">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="37673-125">Plan de Dynamics 365 Customer Engagement Enterprise Edition CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="37673-125">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="37673-126">Plan de Dynamics 365 Customer Engagement Enterprise Edition (precios gubernamentales) CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="37673-126">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="37673-127">Plan de Dynamics 365 Customer Engagement Enterprise Edition CRMOL Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="37673-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="37673-128">Plan de Dynamics 365 Customer Engagement Enterprise Edition CRMOL Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="37673-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="37673-129">Plan de Dynamics 365 Customer Engagement Enterprise Edition de SA para CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="37673-129">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="37673-130">Plan de Dynamics 365 Customer Engagement Enterprise Edition (precios gubernamentales) de SA para CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="37673-130">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="37673-131">Plan de Dynamics 365 Customer Engagement Enterprise Edition de SA for CRM Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="37673-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="37673-132">Plan de Dynamics 365 Customer Engagement Enterprise Edition de SA para CRM Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="37673-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="37673-133">Plan de Dynamics 365 Customer Engagement Enterprise Edition Add-On para CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="37673-133">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="37673-134">Plan de Dynamics 365 Customer Engagement Enterprise Edition (precios gubernamentales) Add-On para CRM Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="37673-134">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="37673-135">Plan de Dynamics 365 Customer Engagement Enterprise Edition Add-On para CRM Basic (oferta calificada) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="37673-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="37673-136">Plan de Dynamics 365 Customer Engagement Enterprise Edition Add-On para CRM Basic (oferta calificada) para profesores</span><span class="sxs-lookup"><span data-stu-id="37673-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="37673-137">Plan de Dynamics 365 for Sales/Customer Engagement de planes de reemplazo básicos (ofertas calificadas)</span><span class="sxs-lookup"><span data-stu-id="37673-137">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="37673-138">**Ofertas retiradas**</span><span class="sxs-lookup"><span data-stu-id="37673-138">**Retired offers**</span></span>   

- <span data-ttu-id="37673-139">Dynamics 365 for Sales de CRM Basic o CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="37673-139">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="37673-140">Plan de Dynamics 365 Customer Engagement de CRM Basic o CRMOL Basic (oferta calificada)</span><span class="sxs-lookup"><span data-stu-id="37673-140">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="37673-141">**Opciones de reemplazo**</span><span class="sxs-lookup"><span data-stu-id="37673-141">**Replacement options**</span></span>
- <span data-ttu-id="37673-142">Dynamics 365 for Sales Professional (NUEVO)</span><span class="sxs-lookup"><span data-stu-id="37673-142">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="37673-143">Dynamics 365 for Sales Professional (NUEVO)</span><span class="sxs-lookup"><span data-stu-id="37673-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="37673-144">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="37673-144">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="37673-145">Plan de Dynamics 365 Customer Engagement o</span><span class="sxs-lookup"><span data-stu-id="37673-145">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="37673-146">Miembros del equipo de Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="37673-146">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="37673-147">Clientes de transición hacia los nuevos planes de productos</span><span class="sxs-lookup"><span data-stu-id="37673-147">Transition customers to new product plans</span></span>

<span data-ttu-id="37673-148">El traslado de clientes de SKU retiradas a otras más recientes requiere los pasos siguientes en este orden:</span><span class="sxs-lookup"><span data-stu-id="37673-148">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="37673-149">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="37673-149">Purchase the new subscription</span></span>
- <span data-ttu-id="37673-150">Reasignación de licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="37673-150">Reassign current user licenses</span></span>
- <span data-ttu-id="37673-151">Cancelación de una suscripción antigua</span><span class="sxs-lookup"><span data-stu-id="37673-151">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="37673-152">Compra del nuevo plan para el cliente</span><span class="sxs-lookup"><span data-stu-id="37673-152">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="37673-153">Seleccione **Clientes** en el panel de navegación izquierdo y, a continuación, seleccione el cliente que desea trasladar a la nueva suscripción.</span><span class="sxs-lookup"><span data-stu-id="37673-153">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="37673-154">Seleccione **Agregar suscripción.**</span><span class="sxs-lookup"><span data-stu-id="37673-154">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="37673-155">Seleccione la suscripción que desea comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, **seleccione Enviar**.</span><span class="sxs-lookup"><span data-stu-id="37673-155">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="37673-156">El cliente tendrá ahora la suscripción anterior y la nueva.</span><span class="sxs-lookup"><span data-stu-id="37673-156">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="37673-157">El siguiente paso consiste en reasignar licencias a los usuarios del cliente.</span><span class="sxs-lookup"><span data-stu-id="37673-157">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="37673-158">Seleccione **Clientes** en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="37673-158">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="37673-159">Seleccione **Usuarios y licencias.**</span><span class="sxs-lookup"><span data-stu-id="37673-159">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="37673-160">Para reasignar una licencia a un usuario, selecciónelo y, a continuación, **seleccione Administrar licencias.**</span><span class="sxs-lookup"><span data-stu-id="37673-160">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="37673-161">En  la página Administrar licencias, desactive la casilla Dynamics 365 for Sales/Customer Engagement Plan from Basic (Qualified Offer) license (Plan de Dynamics 365 for Sales/Customer Engagement plan from Basic [Oferta calificada]) y seleccione un nuevo plan de servicio para la suscripción a la que el cliente va a pasar.</span><span class="sxs-lookup"><span data-stu-id="37673-161">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="37673-162">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="37673-162">Select **Submit**.</span></span> <span data-ttu-id="37673-163">Lo hará para cada usuario que necesite la nueva licencia.</span><span class="sxs-lookup"><span data-stu-id="37673-163">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="37673-164">Una vez que haya movido las licencias a la nueva suscripción, puede cancelar la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="37673-164">Once you've moved the licenses over to the new subscription, you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="37673-165">Seleccione **Clientes** en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.</span><span class="sxs-lookup"><span data-stu-id="37673-165">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="37673-166">En la página de detalles de la suscripción, establezca la suscripción antigua en **Suspendido** y seleccione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="37673-166">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="37673-167">La suscripción anterior ahora está suspendida y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="37673-167">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="37673-168">La suscripción suspendida se desaprovisionará automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="37673-168">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="37673-169">El cliente no incurrirá en costos adicionales por la suscripción anterior.</span><span class="sxs-lookup"><span data-stu-id="37673-169">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



