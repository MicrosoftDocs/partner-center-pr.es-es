---
title: Migrar de Dynamics 365 y Customer Engagement planear de Basic (ofertas completas) para las versiones más recientes | Centro de partners
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 para Sales / ya no se puede renovar el Plan de Engagement de cliente desde suscripciones Basic (ofrece completo).
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Las ofertas de Dynamics 365, renovar las ofertas, nuevas SKU de Dynamics 365
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134405"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="f5f29-104">Migrar Dynamics 365 y el plan Customer Engagement desde las versiones básicas (ofertas calificados) a versiones más recientes</span><span class="sxs-lookup"><span data-stu-id="f5f29-104">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

<span data-ttu-id="f5f29-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="f5f29-105">**Applies to**</span></span>

-  <span data-ttu-id="f5f29-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="f5f29-106">Partner Center</span></span>

<span data-ttu-id="f5f29-107">Efectivo el 1 de enero de 2019, los clientes con Dynamics 365 para Sales / Customer Engagement Plan desde suscripciones Basic (ofrece completo) ya no se puede renovar estas ofertas heredadas; las suscripciones existentes no se renovarán automáticamente cuando expiran.</span><span class="sxs-lookup"><span data-stu-id="f5f29-107">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="f5f29-108">En la página de detalles de la suscripción, el estado de la suscripción cambiará a "Expira el [fecha]" de "Renueva automáticamente el [fecha]".</span><span class="sxs-lookup"><span data-stu-id="f5f29-108">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="f5f29-109">Para garantizar la continuidad de los clientes, debe realizar la transición aquellos con las suscripciones que van a expirar a una opción admitida, que se enumeran a continuación.</span><span class="sxs-lookup"><span data-stu-id="f5f29-109">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="f5f29-110">Te recomendamos mover los clientes a las nuevas suscripciones antes de la fecha de finalización para evitar interrupciones en el servicio a los clientes.</span><span class="sxs-lookup"><span data-stu-id="f5f29-110">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="f5f29-111">Si usa la API (CREST o centro de partners), puede encontrar la renovación de suscripciones caducadas mediante la evaluación de la fecha de finalización de la suscripción, junto con el auto = False property.</span><span class="sxs-lookup"><span data-stu-id="f5f29-111">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="f5f29-112">Las suscripciones en cuestión se establecerá en auto renovar = False, 1 de enero de 2019.</span><span class="sxs-lookup"><span data-stu-id="f5f29-112">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="f5f29-113">Puedes mover a los clientes a un plan nuevo en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="f5f29-113">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="f5f29-114">El Dynamics 365 ofrece retirará</span><span class="sxs-lookup"><span data-stu-id="f5f29-114">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="f5f29-115">Dynamics 365 para ventas Enterprise Edition CRMOL Basic (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="f5f29-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f5f29-116">Dynamics 365 para ventas Enterprise Edition CRMOL básico (oferta completa) para profesores</span><span class="sxs-lookup"><span data-stu-id="f5f29-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f5f29-117">Dynamics 365 para ventas Enterprise Edition CRMOL básico (oferta completa) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="f5f29-117">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f5f29-118">Dynamics 365 para ventas Enterprise Edition (precios para administración pública) CRMOL Basic (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="f5f29-118">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f5f29-119">Dynamics 365 para ventas Enterprise Edition de SA para CRM Basic (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="f5f29-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f5f29-120">Dynamics 365 para ventas Enterprise Edition de SA para CRM Basic (oferta completa) para profesores</span><span class="sxs-lookup"><span data-stu-id="f5f29-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f5f29-121">Dynamics 365 para ventas Enterprise Edition de SA para CRM Basic (oferta completa) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="f5f29-121">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f5f29-122">Dynamics 365 para ventas de Enterprise Edition (precios para administración pública) de SA para CRM Basic (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="f5f29-122">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f5f29-123">Dynamics 365 para el complemento de edición Enterprise de ventas para CRM Basic (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="f5f29-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f5f29-124">Dynamics 365 para el complemento de edición Enterprise de ventas para CRM Basic (oferta completa) para profesores</span><span class="sxs-lookup"><span data-stu-id="f5f29-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f5f29-125">Dynamics 365 para el complemento de edición Enterprise de ventas para CRM Basic (oferta completa) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="f5f29-125">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f5f29-126">Dynamics 365 para el complemento de ventas de Enterprise Edition (precios para administración pública) para CRM Basic (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="f5f29-126">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f5f29-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL básico (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="f5f29-127">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f5f29-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (precios para administración pública) CRMOL básico (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="f5f29-128">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f5f29-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL básico (oferta completa) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="f5f29-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f5f29-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL básico (oferta completa) para profesores</span><span class="sxs-lookup"><span data-stu-id="f5f29-130">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f5f29-131">Dynamics 365 Customer Engagement Plan Enterprise Edition de SA para CRM Basic (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="f5f29-131">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f5f29-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (precios para administración pública) de SA para CRM Basic (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="f5f29-132">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f5f29-133">Dynamics 365 Customer Engagement Plan Enterprise Edition de SA para CRM Basic (oferta completa) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="f5f29-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f5f29-134">Dynamics 365 Customer Engagement Plan Enterprise Edition de SA para CRM Basic (oferta completa) para profesores</span><span class="sxs-lookup"><span data-stu-id="f5f29-134">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="f5f29-135">Complemento Dynamics 365 Customer Engagement Plan Enterprise Edition para CRM Basic (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="f5f29-135">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f5f29-136">Complemento Dynamics 365 Customer Engagement Plan Enterprise Edition (precios para administración pública) para CRM Basic (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="f5f29-136">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f5f29-137">Dynamics 365 Customer Engagement Plan Enterprise Edition complemento para CRM Basic (oferta completa) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="f5f29-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="f5f29-138">Dynamics 365 Customer Engagement Plan Enterprise Edition complemento CRM Basic (oferta completa) para profesores</span><span class="sxs-lookup"><span data-stu-id="f5f29-138">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="f5f29-139">Dynamics 365 para Sales / planes de Customer Engagement planear de reemplazo de Basic (ofrece completo)</span><span class="sxs-lookup"><span data-stu-id="f5f29-139">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

<span data-ttu-id="f5f29-140">**Ofertas retiradas**</span><span class="sxs-lookup"><span data-stu-id="f5f29-140">**Retired offers**</span></span>   

- <span data-ttu-id="f5f29-141">Dynamics 365 para ventas de CRM Basic o CRMOL Basic (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="f5f29-141">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="f5f29-142">Dynamics 365 Customer Engagement Plan de CRM Basic o CRMOL Basic (oferta completa)</span><span class="sxs-lookup"><span data-stu-id="f5f29-142">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

<span data-ttu-id="f5f29-143">**Opciones de reemplazo**</span><span class="sxs-lookup"><span data-stu-id="f5f29-143">**Replacement options**</span></span>
- <span data-ttu-id="f5f29-144">Dynamics 365 para profesionales de ventas (nuevo)</span><span class="sxs-lookup"><span data-stu-id="f5f29-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="f5f29-145">Dynamics 365 para profesionales de ventas (nuevo)</span><span class="sxs-lookup"><span data-stu-id="f5f29-145">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="f5f29-146">Dynamics 365 para el servicio al cliente</span><span class="sxs-lookup"><span data-stu-id="f5f29-146">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="f5f29-147">Plan de Dynamics 365 Customer Engagement o</span><span class="sxs-lookup"><span data-stu-id="f5f29-147">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="f5f29-148">Miembros del equipo de Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="f5f29-148">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="f5f29-149">Clientes de transición hacia los nuevos planes de productos</span><span class="sxs-lookup"><span data-stu-id="f5f29-149">Transition customers to new product plans</span></span>

<span data-ttu-id="f5f29-150">Mover a los clientes de SKU retiradas a los más recientes requiere los pasos siguientes en este orden:</span><span class="sxs-lookup"><span data-stu-id="f5f29-150">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="f5f29-151">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="f5f29-151">Purchase the new subscription</span></span>
- <span data-ttu-id="f5f29-152">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="f5f29-152">Reassign current user licenses</span></span>
- <span data-ttu-id="f5f29-153">Cancelar suscripción antigua</span><span class="sxs-lookup"><span data-stu-id="f5f29-153">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="f5f29-154">El nuevo plan de compra para su cliente</span><span class="sxs-lookup"><span data-stu-id="f5f29-154">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="f5f29-155">Seleccione **clientes** desde el panel de navegación izquierdo y, a continuación, seleccione el cliente que desea mover a la nueva suscripción.</span><span class="sxs-lookup"><span data-stu-id="f5f29-155">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="f5f29-156">Seleccione **Agregar suscripción**.</span><span class="sxs-lookup"><span data-stu-id="f5f29-156">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="f5f29-157">Selecciona la suscripción que quieras adquirir del catálogo (en este caso, una de las opciones que se indican más arriba), escribe el número de licencias y, a continuación, **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="f5f29-157">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="f5f29-158">El cliente tendrá ahora la suscripción antigua y una nueva.</span><span class="sxs-lookup"><span data-stu-id="f5f29-158">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="f5f29-159">El siguiente paso es volver a asignar licencias a los usuarios del cliente.</span><span class="sxs-lookup"><span data-stu-id="f5f29-159">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="f5f29-160">Seleccione **clientes** desde el panel de navegación izquierdo y, a continuación, seleccione el cliente que está moviendo.</span><span class="sxs-lookup"><span data-stu-id="f5f29-160">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="f5f29-161">Selecciona **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="f5f29-161">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="f5f29-162">Para reasignar una licencia a un usuario, seleccione el usuario y, a continuación, seleccione **administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="f5f29-162">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="f5f29-163">En el **administrar licencias** página, desactive el Dynamics 365 para Sales / Plan de compromiso del cliente de Basic (oferta completo) casilla de verificación de licencia y seleccione un nuevo plan de servicio para la suscripción que el cliente se mueve a.</span><span class="sxs-lookup"><span data-stu-id="f5f29-163">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="f5f29-164">Selecciona **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="f5f29-164">Select **Submit**.</span></span> <span data-ttu-id="f5f29-165">Hará esto para cada usuario que necesita la nueva licencia.</span><span class="sxs-lookup"><span data-stu-id="f5f29-165">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="f5f29-166">Una vez que haya movido las licencias a través a la nueva suscripción puede cancelar la suscripción antigua.</span><span class="sxs-lookup"><span data-stu-id="f5f29-166">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="f5f29-167">Seleccione **clientes** desde el panel de navegación izquierdo y, a continuación, seleccione el cliente que está moviendo.</span><span class="sxs-lookup"><span data-stu-id="f5f29-167">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="f5f29-168">En la página de detalles de suscripción, establezca la suscripción antigua **Suspended** y seleccione **enviar**.</span><span class="sxs-lookup"><span data-stu-id="f5f29-168">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="f5f29-169">Ahora se suspende la suscripción antigua y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="f5f29-169">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="f5f29-170">Se cancelará el aprovisionamiento de la suscripción suspendida automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="f5f29-170">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="f5f29-171">Su cliente no incurrirá en ningún costo adicional para la suscripción antigua.</span><span class="sxs-lookup"><span data-stu-id="f5f29-171">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



