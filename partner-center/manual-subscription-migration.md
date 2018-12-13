---
title: Migrar de Dynamics 365 y el Plan de participación de clientes de Basic (ofertas completos) a versiones más recientes | El centro de partners
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales o ya no se puede renovar el Plan de participación de cliente de suscripciones de Basic (ofrece completo).
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968275"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a><span data-ttu-id="cd04e-103">Migrar de Dynamics 365 y el Plan de participación de clientes de Basic (ofertas completos) a versiones más recientes</span><span class="sxs-lookup"><span data-stu-id="cd04e-103">Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions</span></span>

**<span data-ttu-id="cd04e-104">Se aplica a</span><span class="sxs-lookup"><span data-stu-id="cd04e-104">Applies to</span></span>**

-  <span data-ttu-id="cd04e-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="cd04e-105">Partner Center</span></span>

<span data-ttu-id="cd04e-106">Efectiva el 1 de enero de 2019, los clientes con Dynamics 365 for Sales o Plan de participación de cliente de suscripciones de Basic (ofrece completo) ya no se pueden renovar estas ofertas heredadas; las suscripciones existentes no se renovarán automáticamente cuando expiren.</span><span class="sxs-lookup"><span data-stu-id="cd04e-106">Effective January 1, 2019, customers with Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) subscriptions can no longer renew these legacy offers; existing subscriptions will not renew automatically when they expire.</span></span> <span data-ttu-id="cd04e-107">En la página de detalles de la suscripción, el estado cambiará a "Expira el [fecha]" desde "Se renovará automáticamente en [fecha]".</span><span class="sxs-lookup"><span data-stu-id="cd04e-107">On the subscription’s detail page, the subscription status will change to "Expires on [date]" from "Auto renews on [date]".</span></span> 


<span data-ttu-id="cd04e-108">Para garantizar la continuidad para los clientes, debes pasarlas personas con suscripciones vayan a caducar a una opción compatible, como aparece a continuación.</span><span class="sxs-lookup"><span data-stu-id="cd04e-108">To ensure continuity for customers, you should transition those with expiring subscriptions to a supported option, listed below.</span></span> <span data-ttu-id="cd04e-109">Recomendamos pasar a los clientes a las nuevas suscripciones, antes de la fecha de finalización anual de la suscripción, para evitar interrupciones del servicio a los clientes.</span><span class="sxs-lookup"><span data-stu-id="cd04e-109">We recommend moving customers to new subscriptions before the subscription’s yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="cd04e-110">Si usas la API (CREST o centro de partners), puedes encontrar renovar suscripciones vayan a caducar evaluando la fecha de finalización de la suscripción junto con la automática = False propiedad.</span><span class="sxs-lookup"><span data-stu-id="cd04e-110">If you use the API (either CREST or Partner Center), you can find expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> <span data-ttu-id="cd04e-111">Las suscripciones en cuestión se establecerá automáticamente renovar = False el 1 de enero de 2019.</span><span class="sxs-lookup"><span data-stu-id="cd04e-111">The subscriptions in question will be set to auto renew=False on Jan 1, 2019.</span></span> <span data-ttu-id="cd04e-112">Puedes mover a los clientes a un plan nuevo en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="cd04e-112">You can move customers to a new plan at any time.</span></span> 

### <a name="the-dynamics-365-offers-being-retired"></a><span data-ttu-id="cd04e-113">El de Dynamics 365 ofrece que se retiran</span><span class="sxs-lookup"><span data-stu-id="cd04e-113">The Dynamics 365 offers being retired</span></span>

- <span data-ttu-id="cd04e-114">Dynamics 365 ventas Enterprise Edition CRMOL Basic (calificado oferta)</span><span class="sxs-lookup"><span data-stu-id="cd04e-114">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="cd04e-115">Dynamics 365 ventas Enterprise Edition CRMOL Basic (calificado oferta) para profesores</span><span class="sxs-lookup"><span data-stu-id="cd04e-115">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="cd04e-116">Dynamics 365 ventas Enterprise Edition CRMOL Basic (calificado oferta) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="cd04e-116">Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="cd04e-117">Dynamics 365 ventas Enterprise Edition (Government precios) CRMOL Basic (calificado oferta)</span><span class="sxs-lookup"><span data-stu-id="cd04e-117">Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="cd04e-118">Dynamics 365 para la edición Enterprise de venta de Microsoft software Assurance CRM Basic (calificado oferta)</span><span class="sxs-lookup"><span data-stu-id="cd04e-118">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="cd04e-119">Dynamics 365 para la edición Enterprise de venta de Microsoft software Assurance CRM Basic (calificado oferta) para profesores</span><span class="sxs-lookup"><span data-stu-id="cd04e-119">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="cd04e-120">Dynamics 365 para la edición Enterprise de venta de Microsoft software Assurance CRM Basic (calificado oferta) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="cd04e-120">Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="cd04e-121">Dynamics 365 para Enterprise ventas (Government precios) de Microsoft software Assurance CRM Basic (calificado oferta)</span><span class="sxs-lookup"><span data-stu-id="cd04e-121">Dynamics 365 for Sales Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="cd04e-122">Dynamics 365 para el complemento de ventas de Enterprise Edition CRM Basic (calificado oferta)</span><span class="sxs-lookup"><span data-stu-id="cd04e-122">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="cd04e-123">Dynamics 365 para el complemento de ventas de Enterprise Edition CRM Basic (calificado oferta) para profesores</span><span class="sxs-lookup"><span data-stu-id="cd04e-123">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="cd04e-124">Dynamics 365 para el complemento de ventas de Enterprise Edition CRM Basic (calificado oferta) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="cd04e-124">Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="cd04e-125">Dynamics 365 para el complemento de ventas de Enterprise Edition (Government precios) CRM Basic (calificado oferta)</span><span class="sxs-lookup"><span data-stu-id="cd04e-125">Dynamics 365 for Sales Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="cd04e-126">Dynamics 365 cliente Engagement Plan Enterprise Edition CRMOL Basic (calificado oferta)</span><span class="sxs-lookup"><span data-stu-id="cd04e-126">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="cd04e-127">Dynamics 365 cliente Engagement Plan Enterprise Edition (Government precios) CRMOL Basic (calificado oferta)</span><span class="sxs-lookup"><span data-stu-id="cd04e-127">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="cd04e-128">Dynamics 365 cliente Engagement Plan Enterprise Edition CRMOL Basic (calificado oferta) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="cd04e-128">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="cd04e-129">Dynamics 365 cliente Engagement Plan Enterprise Edition CRMOL Basic (calificado oferta) para profesores</span><span class="sxs-lookup"><span data-stu-id="cd04e-129">Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="cd04e-130">Dynamics 365 cliente Engagement Plan Enterprise Edition desde Microsoft software Assurance CRM Basic (calificado oferta)</span><span class="sxs-lookup"><span data-stu-id="cd04e-130">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="cd04e-131">Dynamics 365 cliente Engagement Plan Enterprise Edition (Government precios) de Microsoft software Assurance CRM Basic (calificado oferta)</span><span class="sxs-lookup"><span data-stu-id="cd04e-131">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="cd04e-132">Dynamics 365 cliente Engagement Plan Enterprise Edition desde Microsoft software Assurance CRM Basic (calificado oferta) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="cd04e-132">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="cd04e-133">Dynamics 365 cliente Engagement Plan Enterprise Edition desde Microsoft software Assurance CRM Basic (calificado oferta) para profesores</span><span class="sxs-lookup"><span data-stu-id="cd04e-133">Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty</span></span>
- <span data-ttu-id="cd04e-134">Dynamics 365 cliente Engagement Plan Enterprise Edition complemento CRM Basic (calificado oferta)</span><span class="sxs-lookup"><span data-stu-id="cd04e-134">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="cd04e-135">Dynamics 365 cliente Engagement Plan Enterprise Edition (Government precios) complemento CRM Basic (calificado oferta)</span><span class="sxs-lookup"><span data-stu-id="cd04e-135">Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)</span></span>
- <span data-ttu-id="cd04e-136">Dynamics 365 cliente Engagement Plan Enterprise Edition complemento CRM Basic (calificado oferta) para estudiantes</span><span class="sxs-lookup"><span data-stu-id="cd04e-136">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students</span></span>
- <span data-ttu-id="cd04e-137">Dynamics 365 cliente Engagement Plan Enterprise Edition complemento CRM Basic (calificado oferta) para profesores</span><span class="sxs-lookup"><span data-stu-id="cd04e-137">Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty</span></span>



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a><span data-ttu-id="cd04e-138">Dynamics 365 for Sales o los planes de participación de cliente previsto de reemplazo de Basic (ofrece completo)</span><span class="sxs-lookup"><span data-stu-id="cd04e-138">Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offers) replacement plans</span></span>

**<span data-ttu-id="cd04e-139">Retirada ofertas</span><span class="sxs-lookup"><span data-stu-id="cd04e-139">Retired offers</span></span>**   

- <span data-ttu-id="cd04e-140">Dynamics 365 para las ventas de CRM Basic o CRMOL Basic (calificado oferta)</span><span class="sxs-lookup"><span data-stu-id="cd04e-140">Dynamics 365 for Sales from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>
- <span data-ttu-id="cd04e-141">Dynamics 365 Customer Engagement Plan de CRM Basic o CRMOL Basic (calificado oferta)</span><span class="sxs-lookup"><span data-stu-id="cd04e-141">Dynamics 365 Customer Engagement Plan from CRM Basic or CRMOL Basic (Qualified Offer)</span></span>

**<span data-ttu-id="cd04e-142">Opciones de reemplazo</span><span class="sxs-lookup"><span data-stu-id="cd04e-142">Replacement options</span></span>**
- <span data-ttu-id="cd04e-143">Dynamics 365 para profesionales de ventas (nuevo)</span><span class="sxs-lookup"><span data-stu-id="cd04e-143">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="cd04e-144">Dynamics 365 para profesionales de ventas (nuevo)</span><span class="sxs-lookup"><span data-stu-id="cd04e-144">Dynamics 365 for Sales Professional (NEW)</span></span>
- <span data-ttu-id="cd04e-145">Dynamics 365 for Customer Service</span><span class="sxs-lookup"><span data-stu-id="cd04e-145">Dynamics 365 for Customer Service</span></span>
- <span data-ttu-id="cd04e-146">Dynamics 365 Customer Engagement Plan o</span><span class="sxs-lookup"><span data-stu-id="cd04e-146">Dynamics 365 Customer Engagement Plan or</span></span>
- <span data-ttu-id="cd04e-147">Miembros del equipo de Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="cd04e-147">Dynamics 365 Team Members</span></span>



## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="cd04e-148">Pasar a los clientes a nuevos planes de producto</span><span class="sxs-lookup"><span data-stu-id="cd04e-148">Transition customers to new product plans</span></span>

<span data-ttu-id="cd04e-149">Mover los clientes desde SKU retiradas a unas más recientes que requiere los pasos siguientes en este orden:</span><span class="sxs-lookup"><span data-stu-id="cd04e-149">Moving customers from retired SKUs to newer ones requires the following steps in this order:</span></span>

- <span data-ttu-id="cd04e-150">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="cd04e-150">Purchase the new subscription</span></span>
- <span data-ttu-id="cd04e-151">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="cd04e-151">Reassign current user licenses</span></span>
- <span data-ttu-id="cd04e-152">Cancelar suscripción antigua</span><span class="sxs-lookup"><span data-stu-id="cd04e-152">Cancel old subscription</span></span>

## <a name="purchase-the-new-plan-for-your-customer"></a><span data-ttu-id="cd04e-153">El nuevo plan de compra para el cliente</span><span class="sxs-lookup"><span data-stu-id="cd04e-153">Purchase the new plan for your customer</span></span>

1. <span data-ttu-id="cd04e-154">Selecciona **los clientes** desde el menú de navegación izquierdo y, a continuación, selecciona al cliente que quieras mover a la nueva suscripción.</span><span class="sxs-lookup"><span data-stu-id="cd04e-154">Select **Customers** from the left nav and then select the customer you want to move to the new subscription.</span></span>
2. <span data-ttu-id="cd04e-155">Selecciona **Agregar suscripción**.</span><span class="sxs-lookup"><span data-stu-id="cd04e-155">Select **Add Subscription**.</span></span>
3. <span data-ttu-id="cd04e-156">Selecciona la suscripción que quieras adquirir del catálogo (en este caso, una de las opciones que se indican más arriba), escribe el número de licencias y, a continuación, **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="cd04e-156">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span> 

<span data-ttu-id="cd04e-157">El cliente ahora tendrá la suscripción antigua y uno nuevo.</span><span class="sxs-lookup"><span data-stu-id="cd04e-157">Your customer will now have both the old subscription and the new one.</span></span> <span data-ttu-id="cd04e-158">El siguiente paso es reasignar licencias a los usuarios del cliente.</span><span class="sxs-lookup"><span data-stu-id="cd04e-158">Your next step is to reassign licenses to the customer's users.</span></span>

1. <span data-ttu-id="cd04e-159">Selecciona **los clientes** desde el menú de navegación izquierdo y, a continuación, selecciona al cliente que se mueve.</span><span class="sxs-lookup"><span data-stu-id="cd04e-159">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="cd04e-160">Selecciona **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="cd04e-160">Select **Users and licenses**.</span></span>
3. <span data-ttu-id="cd04e-161">Para reasignar una licencia a un usuario, selecciona el usuario y, a continuación, selecciona **Administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="cd04e-161">To reassign a license to a user, select the user and then select **Manage licenses**.</span></span> 
4. <span data-ttu-id="cd04e-162">En la página **Administrar licencias** , borrar el Dynamics 365 for Sales / Customer Engagement Plan de Basic (ofrecer calificado) casilla de verificación de licencia y selecciona un nuevo plan de servicio de la suscripción que se cambia el cliente.</span><span class="sxs-lookup"><span data-stu-id="cd04e-162">On the **Manage licenses** page, clear the Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license check box and select a new service plan for the subscription the customer is moving to.</span></span> 
5. <span data-ttu-id="cd04e-163">Selecciona **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="cd04e-163">Select **Submit**.</span></span> <span data-ttu-id="cd04e-164">Para hacer esto para cada usuario que necesita la nueva licencia.</span><span class="sxs-lookup"><span data-stu-id="cd04e-164">You will do this for each user who needs the new license.</span></span> 

<span data-ttu-id="cd04e-165">Una vez que traslades las licencias a la nueva suscripción puede cancelar la suscripción antigua.</span><span class="sxs-lookup"><span data-stu-id="cd04e-165">Once you've moved the licenses over to the new subscription you can cancel the old subscription.</span></span> 

1. <span data-ttu-id="cd04e-166">Selecciona **los clientes** desde el menú de navegación izquierdo y, a continuación, selecciona al cliente que se mueve.</span><span class="sxs-lookup"><span data-stu-id="cd04e-166">Select **Customers** from the left nav and then select the customer you are moving.</span></span>
2. <span data-ttu-id="cd04e-167">En la página de detalles de suscripción, Establece la suscripción antigua a **suspendida** y seleccione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="cd04e-167">On the subscription detail page, set the old subscription to **Suspended** and select **Submit**.</span></span>

<span data-ttu-id="cd04e-168">Ahora se suspende la suscripción antigua y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="cd04e-168">The old subscription is now suspended, and the new subscription is active.</span></span> <span data-ttu-id="cd04e-169">Se cancelará el aprovisionamiento de la suscripción suspendida automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="cd04e-169">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="cd04e-170">El cliente no conllevará ningún coste adicional para la suscripción antigua.</span><span class="sxs-lookup"><span data-stu-id="cd04e-170">Your customer will incur no additional costs for the old subscription.</span></span>
 

 



