---
title: Migrar suscripciones de Office 365 E4 a las versiones más recientes de Office 365 | Centro de partners
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: La edición de Office 365 Enterprise E4 se retirará a partir del 7 de abril de 2017. Obtén información sobre cómo migrar las suscripciones de cliente a las versiones más recientes de Office 365.
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: 314711a3f640ad6a228a437e35fe0d8a543e4da5
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004574"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="2548c-104">Migrar de suscripciones de Office 365 E4 a las versiones más recientes de Office 365</span><span class="sxs-lookup"><span data-stu-id="2548c-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="2548c-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="2548c-105">**Applies to**</span></span>

-  <span data-ttu-id="2548c-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="2548c-106">Partner Center</span></span>

<span data-ttu-id="2548c-107">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="2548c-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="2548c-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="2548c-108">Global admin</span></span>
-   <span data-ttu-id="2548c-109">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="2548c-109">User admin</span></span>
-   <span data-ttu-id="2548c-110">Agente de administración</span><span class="sxs-lookup"><span data-stu-id="2548c-110">Admin agent</span></span>
-   <span data-ttu-id="2548c-111">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="2548c-111">Sales agent</span></span>

<span data-ttu-id="2548c-112">El plan Office 365 Enterprise E4 se retira de forma efectiva el 7 de abril de 2017.</span><span class="sxs-lookup"><span data-stu-id="2548c-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="2548c-113">Ya no se podrán adquirir nuevas suscripciones de Office 365 E4 después de esta fecha, y las suscripciones E4 existentes no se renovarán automáticamente cuando expiren.</span><span class="sxs-lookup"><span data-stu-id="2548c-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="2548c-114">Cuando finalicen suscripciones de E4, se cancelarán.</span><span class="sxs-lookup"><span data-stu-id="2548c-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="2548c-115">Para garantizar la continuidad de los clientes, debes pasar los clientes cuyas suscripciones a E4 vayan a caducar a una opción de SKU compatible, como aparece a continuación.</span><span class="sxs-lookup"><span data-stu-id="2548c-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="2548c-116">Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes.</span><span class="sxs-lookup"><span data-stu-id="2548c-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
>  <span data-ttu-id="2548c-117">Se han retirado las SKU de Office 365 Enterprise E4 Commercial y Government.</span><span class="sxs-lookup"><span data-stu-id="2548c-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="2548c-118">En la página de detalles de la suscripción, el estado de la suscripción a E4 ha cambiado de "Se renovará automáticamente en [fecha]" a "Expira en [fecha]".</span><span class="sxs-lookup"><span data-stu-id="2548c-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="2548c-119">Si usas la API (CREST o el Centro de partners), puedes descubrir suscripciones caducadas mediante la evaluación de la fecha de finalización de la suscripción junto con la renovación automática = False propiedad.</span><span class="sxs-lookup"><span data-stu-id="2548c-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="2548c-120">Las suscripciones E4 se establece como renovación automática = Falso el 7 de abril de 2017.</span><span class="sxs-lookup"><span data-stu-id="2548c-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="2548c-121">Puedes mover a los clientes a un plan nuevo en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="2548c-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="2548c-122">Planes de reemplazo de la edición Office 365 Enterprise E4</span><span class="sxs-lookup"><span data-stu-id="2548c-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="2548c-123">Puedes elegir mantener la misma funcionalidad con E4 o puedes hacer que los clientes saquen provecho de las nuevas características y funciones de Office 365 y Skype Empresarial Online.</span><span class="sxs-lookup"><span data-stu-id="2548c-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="2548c-124">Los detalles de precios se encuentran en la lista de precios y en la matriz de lista de ofertas en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="2548c-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="2548c-125">Secure Productive Enterprise E3 o Secure Productive Enterprise E5 puede sustituirse en las siguientes opciones por Office 365 Enterprise E3 o Office 365 Enterprise E5 respectivamente.</span><span class="sxs-lookup"><span data-stu-id="2548c-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="2548c-126">Opción 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="2548c-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="2548c-127">Opción 2: E3 de Office 365 empresa + Skype Empresarial Cloud PBX</span><span class="sxs-lookup"><span data-stu-id="2548c-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="2548c-128">Opción 3: Office 365 Enterprise E3 + Skype Empresarial + CAL (paridad de precio y la funcionalidad con E4)</span><span class="sxs-lookup"><span data-stu-id="2548c-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="2548c-129">Opción 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="2548c-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="2548c-130">Función</span><span class="sxs-lookup"><span data-stu-id="2548c-130">Feature</span></span> | <span data-ttu-id="2548c-131">Opción 1</span><span class="sxs-lookup"><span data-stu-id="2548c-131">Option 1</span></span> | <span data-ttu-id="2548c-132">Opción 2</span><span class="sxs-lookup"><span data-stu-id="2548c-132">Option 2</span></span> | <span data-ttu-id="2548c-133">Opción 3</span><span class="sxs-lookup"><span data-stu-id="2548c-133">Option 3</span></span> | <span data-ttu-id="2548c-134">Opción 4</span><span class="sxs-lookup"><span data-stu-id="2548c-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="2548c-135">¿Obtener todas las características incluidas en Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="2548c-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="2548c-136">Sí</span><span class="sxs-lookup"><span data-stu-id="2548c-136">Yes</span></span> | <span data-ttu-id="2548c-137">Sí</span><span class="sxs-lookup"><span data-stu-id="2548c-137">Yes</span></span> | <span data-ttu-id="2548c-138">Sí</span><span class="sxs-lookup"><span data-stu-id="2548c-138">Yes</span></span> | <span data-ttu-id="2548c-139">No</span><span class="sxs-lookup"><span data-stu-id="2548c-139">No</span></span> |
| <span data-ttu-id="2548c-140">¿Números de teléfono administrados en Office 365?</span><span class="sxs-lookup"><span data-stu-id="2548c-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="2548c-141">Sí</span><span class="sxs-lookup"><span data-stu-id="2548c-141">Yes</span></span> | <span data-ttu-id="2548c-142">Sí</span><span class="sxs-lookup"><span data-stu-id="2548c-142">Yes</span></span> | <span data-ttu-id="2548c-143">No</span><span class="sxs-lookup"><span data-stu-id="2548c-143">No</span></span> | <span data-ttu-id="2548c-144">No</span><span class="sxs-lookup"><span data-stu-id="2548c-144">No</span></span> |
| <span data-ttu-id="2548c-145">¿Números de teléfono administrados en local y en Office 365 (implementación híbrida)?</span><span class="sxs-lookup"><span data-stu-id="2548c-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="2548c-146">Sí</span><span class="sxs-lookup"><span data-stu-id="2548c-146">Yes</span></span> | <span data-ttu-id="2548c-147">Sí</span><span class="sxs-lookup"><span data-stu-id="2548c-147">Yes</span></span> | <span data-ttu-id="2548c-148">No</span><span class="sxs-lookup"><span data-stu-id="2548c-148">No</span></span> | <span data-ttu-id="2548c-149">No</span><span class="sxs-lookup"><span data-stu-id="2548c-149">No</span></span> |
| <span data-ttu-id="2548c-150">¿Opción para agregar un plan de llamadas de voz RTC?</span><span class="sxs-lookup"><span data-stu-id="2548c-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="2548c-151">Sí</span><span class="sxs-lookup"><span data-stu-id="2548c-151">Yes</span></span> | <span data-ttu-id="2548c-152">Sí</span><span class="sxs-lookup"><span data-stu-id="2548c-152">Yes</span></span> | <span data-ttu-id="2548c-153">No</span><span class="sxs-lookup"><span data-stu-id="2548c-153">No</span></span> | <span data-ttu-id="2548c-154">No</span><span class="sxs-lookup"><span data-stu-id="2548c-154">No</span></span> |
| <span data-ttu-id="2548c-155">¿Conferencias RTC?</span><span class="sxs-lookup"><span data-stu-id="2548c-155">PSTN Conferencing?</span></span> | <span data-ttu-id="2548c-156">Sí</span><span class="sxs-lookup"><span data-stu-id="2548c-156">Yes</span></span> | <span data-ttu-id="2548c-157">No</span><span class="sxs-lookup"><span data-stu-id="2548c-157">No</span></span> | <span data-ttu-id="2548c-158">No</span><span class="sxs-lookup"><span data-stu-id="2548c-158">No</span></span> | <span data-ttu-id="2548c-159">No</span><span class="sxs-lookup"><span data-stu-id="2548c-159">No</span></span> |
| <span data-ttu-id="2548c-160">¿Herramientas avanzadas de colaboración, análisis y seguridad?</span><span class="sxs-lookup"><span data-stu-id="2548c-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="2548c-161">Sí</span><span class="sxs-lookup"><span data-stu-id="2548c-161">Yes</span></span> | <span data-ttu-id="2548c-162">No</span><span class="sxs-lookup"><span data-stu-id="2548c-162">No</span></span> | <span data-ttu-id="2548c-163">No</span><span class="sxs-lookup"><span data-stu-id="2548c-163">No</span></span> | <span data-ttu-id="2548c-164">No</span><span class="sxs-lookup"><span data-stu-id="2548c-164">No</span></span> |
| <span data-ttu-id="2548c-165">¿Visualizaciones interactivas de informes, paneles y datos?</span><span class="sxs-lookup"><span data-stu-id="2548c-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="2548c-166">Sí</span><span class="sxs-lookup"><span data-stu-id="2548c-166">Yes</span></span> | <span data-ttu-id="2548c-167">No</span><span class="sxs-lookup"><span data-stu-id="2548c-167">No</span></span> | <span data-ttu-id="2548c-168">No</span><span class="sxs-lookup"><span data-stu-id="2548c-168">No</span></span> | <span data-ttu-id="2548c-169">No</span><span class="sxs-lookup"><span data-stu-id="2548c-169">No</span></span> | 
| <span data-ttu-id="2548c-170">¿Más control sobre la seguridad de los datos y la conformidad con la privacidad integradas, transparencia y controles de usuario refinados?</span><span class="sxs-lookup"><span data-stu-id="2548c-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="2548c-171">Sí</span><span class="sxs-lookup"><span data-stu-id="2548c-171">Yes</span></span> | <span data-ttu-id="2548c-172">No</span><span class="sxs-lookup"><span data-stu-id="2548c-172">No</span></span> | <span data-ttu-id="2548c-173">No</span><span class="sxs-lookup"><span data-stu-id="2548c-173">No</span></span> | <span data-ttu-id="2548c-174">No</span><span class="sxs-lookup"><span data-stu-id="2548c-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="2548c-175">Pasar a los clientes a nuevos planes de producto</span><span class="sxs-lookup"><span data-stu-id="2548c-175">Transition customers to new product plans</span></span>

<span data-ttu-id="2548c-176">Microsoft ofrece de forma continua nuevos productos y servicios a nuestros partners.</span><span class="sxs-lookup"><span data-stu-id="2548c-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="2548c-177">En estos casos, podrías tener que actualizar a los clientes con los nuevos servicios o migrar sus suscripciones de SKU que finalmente se apagarán.</span><span class="sxs-lookup"><span data-stu-id="2548c-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="2548c-178">Migración de los clientes desde SKU retiradas a unas más recientes que requieren los siguiente pasos:</span><span class="sxs-lookup"><span data-stu-id="2548c-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="2548c-179">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="2548c-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="2548c-180">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="2548c-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="2548c-181">Cancelar la suscripción antigua</span><span class="sxs-lookup"><span data-stu-id="2548c-181">Cancel the old subscription</span></span>

<span data-ttu-id="2548c-182">Sigue estos pasos para migrar la suscripción a Office 365 Enterprise E4 de un cliente a una de las opciones en la tabla anterior.</span><span class="sxs-lookup"><span data-stu-id="2548c-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="2548c-183">Paso 1 - Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="2548c-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="2548c-184">En el menú del **centro de Partners** , seleccione **clientes**, seleccione el cliente que desea migrar y, a continuación, seleccione **Agregar suscripciones**.</span><span class="sxs-lookup"><span data-stu-id="2548c-184">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="2548c-185">Selecciona la suscripción que quieras adquirir del catálogo (en este caso, una de las opciones que se indican más arriba), escribe el número de licencias y, a continuación, **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="2548c-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="2548c-186">El cliente debería tener ahora suscripciones antiguas y nuevas, la antigua suscripción de Office 365 Enterprise E4 y la nueva suscripción de destino, por ejemplo, la opción 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="2548c-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="2548c-187">Paso 2: Reasignar licencias de los usuarios del cliente</span><span class="sxs-lookup"><span data-stu-id="2548c-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="2548c-188">En el menú del **centro de Partners** , seleccione **clientes**, seleccione el cliente que desea migrar y, a continuación, seleccione **usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="2548c-188">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="2548c-189">Se abre la página usuarios y licencias del cliente.</span><span class="sxs-lookup"><span data-stu-id="2548c-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="2548c-190">Para reasignar licencias de usuario, selecciona el usuario para reasignar y, a continuación, selecciona **Administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="2548c-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="2548c-191">En la página **Administrar licencias** desactiva la casilla de verificación de licencia de **Office 365 Enterprise E4**  selecciona un nuevo plan de servicio de la suscripción a la que se cambia el cliente.</span><span class="sxs-lookup"><span data-stu-id="2548c-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="2548c-192">Selecciona **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="2548c-192">Select **Submit**.</span></span> <span data-ttu-id="2548c-193">Una página de confirmación enumera las nuevas asignaciones de licencias.</span><span class="sxs-lookup"><span data-stu-id="2548c-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="2548c-194">Sigue los mismos pasos con otros usuarios del cliente que necesiten la reasignación de licencias.</span><span class="sxs-lookup"><span data-stu-id="2548c-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="2548c-195">Después de mover las licencias de usuario al nuevo servicio, puedes cancelar de forma segura la suscripción retirada al nivel superior del cliente.</span><span class="sxs-lookup"><span data-stu-id="2548c-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="2548c-196">Paso 3 - Cancelar la suscripción antigua</span><span class="sxs-lookup"><span data-stu-id="2548c-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="2548c-197">En el menú del **centro de Partners** , seleccione **clientes**.</span><span class="sxs-lookup"><span data-stu-id="2548c-197">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="2548c-198">Selecciona al cliente que quieres mover y selecciona la suscripción que quieres cancelar.</span><span class="sxs-lookup"><span data-stu-id="2548c-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="2548c-199">En la página de detalles de suscripción, establece el estado de la suscripción a **Suspendida**.</span><span class="sxs-lookup"><span data-stu-id="2548c-199">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="2548c-200">Selecciona **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="2548c-200">Select **Submit**.</span></span>

<span data-ttu-id="2548c-201">Se ha suspendido la suscripción antigua y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="2548c-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="2548c-202">Se cancelará el aprovisionamiento de la suscripción suspendida automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="2548c-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="2548c-203">El cliente no incurre en costos adicionales para la suscripción antigua.</span><span class="sxs-lookup"><span data-stu-id="2548c-203">The customer incurs no additional costs for the old subscription.</span></span>



 



