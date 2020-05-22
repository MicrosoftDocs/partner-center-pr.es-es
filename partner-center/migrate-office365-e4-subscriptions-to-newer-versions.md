---
title: Migración de suscripciones de Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 Edition se retirará a partir del 7 de abril de 2017. Obtenga información sobre cómo migrar las suscripciones de clientes a las versiones más recientes de Office 365.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bd9f9effd501846934e1b0b2a86b654dfa14ebbe
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795758"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="ec945-104">Migrar suscripciones de Office 365 E4 a las versiones más recientes de Office 365</span><span class="sxs-lookup"><span data-stu-id="ec945-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="ec945-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="ec945-105">**Applies to**</span></span>

-  <span data-ttu-id="ec945-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ec945-106">Partner Center</span></span>

<span data-ttu-id="ec945-107">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="ec945-107">**Appropriate roles**</span></span>
-   <span data-ttu-id="ec945-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ec945-108">Global admin</span></span>
-   <span data-ttu-id="ec945-109">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="ec945-109">User admin</span></span>
-   <span data-ttu-id="ec945-110">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="ec945-110">Admin agent</span></span>
-   <span data-ttu-id="ec945-111">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="ec945-111">Sales agent</span></span>

<span data-ttu-id="ec945-112">El plan Office 365 Enterprise E4 se ha retirado, en vigor el 7 de abril de 2017.</span><span class="sxs-lookup"><span data-stu-id="ec945-112">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="ec945-113">Ya no se pueden comprar nuevas suscripciones a Office 365 E4 después de esta fecha, y las suscripciones de E4 existentes no se renovarán automáticamente cuando expiren.</span><span class="sxs-lookup"><span data-stu-id="ec945-113">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="ec945-114">Cuando finalicen las suscripciones a E4, se cancelarán.</span><span class="sxs-lookup"><span data-stu-id="ec945-114">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="ec945-115">Para garantizar la continuidad de los clientes, debe realizar la transición de los clientes con suscripciones de E4 que expiren a una opción de SKU admitida, que se enumeran a continuación.</span><span class="sxs-lookup"><span data-stu-id="ec945-115">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="ec945-116">Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes.</span><span class="sxs-lookup"><span data-stu-id="ec945-116">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="ec945-117">Se han retirado las SKU de Office 365 Enterprise E4 Commercial y Government.</span><span class="sxs-lookup"><span data-stu-id="ec945-117">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="ec945-118">En la página de detalles de la suscripción, el estado de la suscripción de E4 ha cambiado a "expira el [fecha]" de "renueve automáticamente en [fecha]".</span><span class="sxs-lookup"><span data-stu-id="ec945-118">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="ec945-119">Si usa la API (de la cresta o del centro de Partners), puede detectar las suscripciones que van a expirar mediante la evaluación de la fecha de finalización de la suscripción junto con la propiedad auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="ec945-119">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="ec945-120">Las suscripciones del plan E4 se establecerán en renovación automática = false en el 7 de abril de 2017.</span><span class="sxs-lookup"><span data-stu-id="ec945-120">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="ec945-121">Puede trasladar a los clientes a un nuevo plan en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="ec945-121">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="ec945-122">Planes de reemplazo de Office 365 Enterprise E4 Edition</span><span class="sxs-lookup"><span data-stu-id="ec945-122">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="ec945-123">Puede optar por mantener la misma funcionalidad con E4 o hacer que los clientes aprovechen las características y funcionalidades más recientes de Office 365 y Skype empresarial online.</span><span class="sxs-lookup"><span data-stu-id="ec945-123">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="ec945-124">Los detalles de precios se encuentran en la lista de precios y en la matriz de lista de ofertas del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="ec945-124">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="ec945-125">Secure Product Enterprise E3 o Secure productiva Enterprise E5 se pueden sustituir en las siguientes opciones para Office 365 Enterprise E3 u Office 365 Enterprise E5, respectivamente.</span><span class="sxs-lookup"><span data-stu-id="ec945-125">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="ec945-126">Opción 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="ec945-126">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="ec945-127">Opción 2: Office 365 Enterprise E3 + PBX en la nube de Skype empresarial</span><span class="sxs-lookup"><span data-stu-id="ec945-127">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="ec945-128">Opción 3: Office 365 Enterprise E3 + CAL de Skype empresarial Plus (paridad de precio y funcionalidad con E4)</span><span class="sxs-lookup"><span data-stu-id="ec945-128">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="ec945-129">Opción 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="ec945-129">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="ec945-130">Característica</span><span class="sxs-lookup"><span data-stu-id="ec945-130">Feature</span></span> | <span data-ttu-id="ec945-131">Opción 1</span><span class="sxs-lookup"><span data-stu-id="ec945-131">Option 1</span></span> | <span data-ttu-id="ec945-132">Opción 2</span><span class="sxs-lookup"><span data-stu-id="ec945-132">Option 2</span></span> | <span data-ttu-id="ec945-133">Opción 3</span><span class="sxs-lookup"><span data-stu-id="ec945-133">Option 3</span></span> | <span data-ttu-id="ec945-134">Opción 4</span><span class="sxs-lookup"><span data-stu-id="ec945-134">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="ec945-135">Obtener todas las características incluidas en Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="ec945-135">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="ec945-136">Sí</span><span class="sxs-lookup"><span data-stu-id="ec945-136">Yes</span></span> | <span data-ttu-id="ec945-137">Sí</span><span class="sxs-lookup"><span data-stu-id="ec945-137">Yes</span></span> | <span data-ttu-id="ec945-138">Sí</span><span class="sxs-lookup"><span data-stu-id="ec945-138">Yes</span></span> | <span data-ttu-id="ec945-139">No</span><span class="sxs-lookup"><span data-stu-id="ec945-139">No</span></span> |
| <span data-ttu-id="ec945-140">Números de teléfono administrados en Office 365</span><span class="sxs-lookup"><span data-stu-id="ec945-140">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="ec945-141">Sí</span><span class="sxs-lookup"><span data-stu-id="ec945-141">Yes</span></span> | <span data-ttu-id="ec945-142">Sí</span><span class="sxs-lookup"><span data-stu-id="ec945-142">Yes</span></span> | <span data-ttu-id="ec945-143">No</span><span class="sxs-lookup"><span data-stu-id="ec945-143">No</span></span> | <span data-ttu-id="ec945-144">No</span><span class="sxs-lookup"><span data-stu-id="ec945-144">No</span></span> |
| <span data-ttu-id="ec945-145">Números de teléfono administrados tanto en el entorno local como en Office 365 (implementación híbrida)</span><span class="sxs-lookup"><span data-stu-id="ec945-145">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="ec945-146">Sí</span><span class="sxs-lookup"><span data-stu-id="ec945-146">Yes</span></span> | <span data-ttu-id="ec945-147">Sí</span><span class="sxs-lookup"><span data-stu-id="ec945-147">Yes</span></span> | <span data-ttu-id="ec945-148">No</span><span class="sxs-lookup"><span data-stu-id="ec945-148">No</span></span> | <span data-ttu-id="ec945-149">No</span><span class="sxs-lookup"><span data-stu-id="ec945-149">No</span></span> |
| <span data-ttu-id="ec945-150">¿Desea agregar un plan de llamada de voz RTC?</span><span class="sxs-lookup"><span data-stu-id="ec945-150">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="ec945-151">Sí</span><span class="sxs-lookup"><span data-stu-id="ec945-151">Yes</span></span> | <span data-ttu-id="ec945-152">Sí</span><span class="sxs-lookup"><span data-stu-id="ec945-152">Yes</span></span> | <span data-ttu-id="ec945-153">No</span><span class="sxs-lookup"><span data-stu-id="ec945-153">No</span></span> | <span data-ttu-id="ec945-154">No</span><span class="sxs-lookup"><span data-stu-id="ec945-154">No</span></span> |
| <span data-ttu-id="ec945-155">¿Conferencias RTC?</span><span class="sxs-lookup"><span data-stu-id="ec945-155">PSTN Conferencing?</span></span> | <span data-ttu-id="ec945-156">Sí</span><span class="sxs-lookup"><span data-stu-id="ec945-156">Yes</span></span> | <span data-ttu-id="ec945-157">No</span><span class="sxs-lookup"><span data-stu-id="ec945-157">No</span></span> | <span data-ttu-id="ec945-158">No</span><span class="sxs-lookup"><span data-stu-id="ec945-158">No</span></span> | <span data-ttu-id="ec945-159">No</span><span class="sxs-lookup"><span data-stu-id="ec945-159">No</span></span> |
| <span data-ttu-id="ec945-160">Herramientas avanzadas para la colaboración, el análisis y la seguridad</span><span class="sxs-lookup"><span data-stu-id="ec945-160">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="ec945-161">Sí</span><span class="sxs-lookup"><span data-stu-id="ec945-161">Yes</span></span> | <span data-ttu-id="ec945-162">No</span><span class="sxs-lookup"><span data-stu-id="ec945-162">No</span></span> | <span data-ttu-id="ec945-163">No</span><span class="sxs-lookup"><span data-stu-id="ec945-163">No</span></span> | <span data-ttu-id="ec945-164">No</span><span class="sxs-lookup"><span data-stu-id="ec945-164">No</span></span> |
| <span data-ttu-id="ec945-165">Informes interactivos, paneles y visualizaciones de datos</span><span class="sxs-lookup"><span data-stu-id="ec945-165">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="ec945-166">Sí</span><span class="sxs-lookup"><span data-stu-id="ec945-166">Yes</span></span> | <span data-ttu-id="ec945-167">No</span><span class="sxs-lookup"><span data-stu-id="ec945-167">No</span></span> | <span data-ttu-id="ec945-168">No</span><span class="sxs-lookup"><span data-stu-id="ec945-168">No</span></span> | <span data-ttu-id="ec945-169">No</span><span class="sxs-lookup"><span data-stu-id="ec945-169">No</span></span> | 
| <span data-ttu-id="ec945-170">¿Más control sobre la seguridad y el cumplimiento de los datos con la privacidad, la transparencia y los controles de usuario mejorados?</span><span class="sxs-lookup"><span data-stu-id="ec945-170">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="ec945-171">Sí</span><span class="sxs-lookup"><span data-stu-id="ec945-171">Yes</span></span> | <span data-ttu-id="ec945-172">No</span><span class="sxs-lookup"><span data-stu-id="ec945-172">No</span></span> | <span data-ttu-id="ec945-173">No</span><span class="sxs-lookup"><span data-stu-id="ec945-173">No</span></span> | <span data-ttu-id="ec945-174">No</span><span class="sxs-lookup"><span data-stu-id="ec945-174">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="ec945-175">Clientes de transición hacia los nuevos planes de productos</span><span class="sxs-lookup"><span data-stu-id="ec945-175">Transition customers to new product plans</span></span>

<span data-ttu-id="ec945-176">Microsoft ofrece continuamente nuevos productos y servicios a nuestros asociados.</span><span class="sxs-lookup"><span data-stu-id="ec945-176">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="ec945-177">En estos casos, es posible que tenga que actualizar los clientes a nuevos servicios o migrar sus suscripciones de SKU que se apagarán finalmente.</span><span class="sxs-lookup"><span data-stu-id="ec945-177">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="ec945-178">La migración de los clientes de SKU retiradas a otras más recientes requiere los siguientes pasos:</span><span class="sxs-lookup"><span data-stu-id="ec945-178">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="ec945-179">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="ec945-179">Purchase the new subscription</span></span>
-   <span data-ttu-id="ec945-180">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="ec945-180">Reassign current user licenses</span></span>
-   <span data-ttu-id="ec945-181">Cancelar la suscripción antigua</span><span class="sxs-lookup"><span data-stu-id="ec945-181">Cancel the old subscription</span></span>

<span data-ttu-id="ec945-182">Siga estos pasos para migrar la suscripción Office 365 Enterprise E4 de un cliente a una de las opciones de la tabla anterior.</span><span class="sxs-lookup"><span data-stu-id="ec945-182">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="ec945-183">Paso 1: compra de la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="ec945-183">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="ec945-184">En el menú del **centro de Partners** , seleccione **clientes**, seleccione el cliente que desea migrar y, a continuación, seleccione **Agregar suscripciones**.</span><span class="sxs-lookup"><span data-stu-id="ec945-184">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="ec945-185">Seleccione la suscripción que desea comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="ec945-185">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="ec945-186">El cliente debería tener ahora suscripciones antiguas y nuevas, la antigua suscripción de Office 365 Enterprise E4 y la nueva suscripción de destino, por ejemplo, la opción 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="ec945-186">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="ec945-187">Paso 2: reasignación de las licencias de los usuarios del cliente</span><span class="sxs-lookup"><span data-stu-id="ec945-187">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="ec945-188">En el menú del **centro de Partners** , seleccione **clientes**, seleccione el cliente que desea migrar y, a continuación, seleccione **usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="ec945-188">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="ec945-189">Se abre la página usuarios y licencias del cliente.</span><span class="sxs-lookup"><span data-stu-id="ec945-189">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="ec945-190">Para reasignar licencias de usuario, selecciona el usuario para reasignar y, a continuación, selecciona **Administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="ec945-190">To re-assign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="ec945-191">En la página **administrar licencias** , desactive la casilla **Office 365 Enterprise E4** License y seleccione un nuevo plan de servicio para la suscripción a la que está pasando el cliente.</span><span class="sxs-lookup"><span data-stu-id="ec945-191">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="ec945-192">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="ec945-192">Select **Submit**.</span></span> <span data-ttu-id="ec945-193">Una página de confirmación enumera las nuevas asignaciones de licencias.</span><span class="sxs-lookup"><span data-stu-id="ec945-193">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="ec945-194">Sigue los mismos pasos con otros usuarios del cliente que necesiten la reasignación de licencias.</span><span class="sxs-lookup"><span data-stu-id="ec945-194">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="ec945-195">Después de mover las licencias de usuario al nuevo servicio, puede cancelar con seguridad la suscripción retirada en el nivel superior del cliente.</span><span class="sxs-lookup"><span data-stu-id="ec945-195">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="ec945-196">Paso 3: cancelar la suscripción anterior</span><span class="sxs-lookup"><span data-stu-id="ec945-196">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="ec945-197">En el menú del **centro de Partners** , seleccione **clientes**.</span><span class="sxs-lookup"><span data-stu-id="ec945-197">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="ec945-198">Seleccione el cliente que desea trasladar y seleccione la suscripción que desea cancelar.</span><span class="sxs-lookup"><span data-stu-id="ec945-198">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="ec945-199">En la página Detalles de la suscripción, establezca el estado de la suscripción en **Suspended**.</span><span class="sxs-lookup"><span data-stu-id="ec945-199">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="ec945-200">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="ec945-200">Select **Submit**.</span></span>

<span data-ttu-id="ec945-201">La suscripción anterior se suspende y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="ec945-201">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="ec945-202">La suscripción suspendida se desaprovisionará automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="ec945-202">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="ec945-203">El cliente no incurre en costos adicionales para la suscripción antigua.</span><span class="sxs-lookup"><span data-stu-id="ec945-203">The customer incurs no additional costs for the old subscription.</span></span>



 



