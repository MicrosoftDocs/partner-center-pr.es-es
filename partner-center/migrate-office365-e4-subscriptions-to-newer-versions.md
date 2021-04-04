---
title: Migración de suscripciones de Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 Edition se retirará a partir del 7 de abril de 2017. Obtenga información sobre cómo migrar las suscripciones de clientes a las versiones más recientes de Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132628"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a><span data-ttu-id="b8e9b-104">Migrar suscripciones de Office 365 E4 a las versiones más recientes de Office 365</span><span class="sxs-lookup"><span data-stu-id="b8e9b-104">Migrate Office 365 E4 subscriptions to newer Office 365 versions</span></span>

<span data-ttu-id="b8e9b-105">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="b8e9b-105">**Appropriate roles**</span></span>

- <span data-ttu-id="b8e9b-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="b8e9b-106">Global admin</span></span>
- <span data-ttu-id="b8e9b-107">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="b8e9b-107">User management admin</span></span>
- <span data-ttu-id="b8e9b-108">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="b8e9b-108">Admin agent</span></span>
- <span data-ttu-id="b8e9b-109">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="b8e9b-109">Sales agent</span></span>

<span data-ttu-id="b8e9b-110">El plan Office 365 Enterprise E4 se ha retirado, en vigor el 7 de abril de 2017.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-110">The Office 365 Enterprise E4 plan is retired, effective April 7, 2017.</span></span> <span data-ttu-id="b8e9b-111">Ya no se pueden comprar nuevas suscripciones a Office 365 E4 después de esta fecha, y las suscripciones de E4 existentes no se renovarán automáticamente cuando expiren.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-111">You can no longer purchase new Office 365 E4 subscriptions after this date, and existing E4 subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="b8e9b-112">Cuando finalicen las suscripciones a E4, se cancelarán.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-112">When E4 subscriptions end, they will be canceled.</span></span> <span data-ttu-id="b8e9b-113">Para garantizar la continuidad de los clientes, debe realizar la transición de los clientes con suscripciones de E4 que expiren a una opción de SKU admitida, que se enumeran a continuación.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-113">To ensure continuity for customers, you should transition customers with expiring E4 subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="b8e9b-114">Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-114">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span> 

> [!NOTE]  
> <span data-ttu-id="b8e9b-115">Se han retirado las SKU de Office 365 Enterprise E4 Commercial y Government.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-115">Both Office 365 Enterprise E4 commercial and government SKUs are retired.</span></span>
 
<span data-ttu-id="b8e9b-116">En la página de detalles de la suscripción, el estado de la suscripción de E4 ha cambiado a "expira el [fecha]" de "renueve automáticamente en [fecha]".</span><span class="sxs-lookup"><span data-stu-id="b8e9b-116">On the subscription's detail page, the E4 subscription status has changed to "Expires on [date]" from "Auto renews on [date]".</span></span> 

<span data-ttu-id="b8e9b-117">Si usa la API (de la cresta o del centro de Partners), puede detectar las suscripciones que van a expirar mediante la evaluación de la fecha de finalización de la suscripción junto con la propiedad auto Renew = false.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-117">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew = False property.</span></span> 

<span data-ttu-id="b8e9b-118">Las suscripciones del plan E4 se establecerán en renovación automática = false en el 7 de abril de 2017.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-118">The E4 subscriptions will be set to auto renew=False in April 7, 2017.</span></span> <span data-ttu-id="b8e9b-119">Puede trasladar a los clientes a un nuevo plan en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-119">You can move customers to a new plan at any time.</span></span> 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a><span data-ttu-id="b8e9b-120">Planes de reemplazo de Office 365 Enterprise E4 Edition</span><span class="sxs-lookup"><span data-stu-id="b8e9b-120">Office 365 Enterprise E4 edition replacement plans</span></span>

<span data-ttu-id="b8e9b-121">Puede optar por mantener la misma funcionalidad con E4 o hacer que los clientes aprovechen las características y funcionalidades más recientes de Office 365 y Skype empresarial online.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-121">You can choose to maintain the same functionality with E4 or have your customers take advantage of newer features and functionality in Office 365 and Skype for Business Online.</span></span> <span data-ttu-id="b8e9b-122">Los detalles de precios se encuentran en la lista de precios y en la matriz de lista de ofertas del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-122">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span> <span data-ttu-id="b8e9b-123">Secure Product Enterprise E3 o Secure productiva Enterprise E5 se pueden sustituir en las siguientes opciones para Office 365 Enterprise E3 u Office 365 Enterprise E5, respectivamente.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-123">Secure Product Enterprise E3 or Secure Productive Enterprise E5 may be substituted in the following options for Office 365 Enterprise E3 or Office 365 Enterprise E5 respectively.</span></span>

- <span data-ttu-id="b8e9b-124">Opción 1: Office 365 Enterprise E5</span><span class="sxs-lookup"><span data-stu-id="b8e9b-124">Option 1: Office 365 Enterprise E5</span></span>

- <span data-ttu-id="b8e9b-125">Opción 2: Office 365 Enterprise E3 + PBX en la nube de Skype empresarial</span><span class="sxs-lookup"><span data-stu-id="b8e9b-125">Option 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX</span></span>

- <span data-ttu-id="b8e9b-126">Opción 3: Office 365 Enterprise E3 + CAL de Skype empresarial Plus (paridad de precio y funcionalidad con E4)</span><span class="sxs-lookup"><span data-stu-id="b8e9b-126">Option 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (price and functionality parity with E4)</span></span>

- <span data-ttu-id="b8e9b-127">Opción 4: Office 365 Enterprise E3</span><span class="sxs-lookup"><span data-stu-id="b8e9b-127">Option 4: Office 365 Enterprise E3</span></span>


| <span data-ttu-id="b8e9b-128">Característica</span><span class="sxs-lookup"><span data-stu-id="b8e9b-128">Feature</span></span> | <span data-ttu-id="b8e9b-129">Opción 1</span><span class="sxs-lookup"><span data-stu-id="b8e9b-129">Option 1</span></span> | <span data-ttu-id="b8e9b-130">Opción 2</span><span class="sxs-lookup"><span data-stu-id="b8e9b-130">Option 2</span></span> | <span data-ttu-id="b8e9b-131">Opción 3</span><span class="sxs-lookup"><span data-stu-id="b8e9b-131">Option 3</span></span> | <span data-ttu-id="b8e9b-132">Opción 4</span><span class="sxs-lookup"><span data-stu-id="b8e9b-132">Option 4</span></span> |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| <span data-ttu-id="b8e9b-133">Obtener todas las características incluidas en Office 365 Enterprise E4?</span><span class="sxs-lookup"><span data-stu-id="b8e9b-133">Get all the features included in Office 365 Enterprise E4?</span></span> | <span data-ttu-id="b8e9b-134">Sí</span><span class="sxs-lookup"><span data-stu-id="b8e9b-134">Yes</span></span> | <span data-ttu-id="b8e9b-135">Sí</span><span class="sxs-lookup"><span data-stu-id="b8e9b-135">Yes</span></span> | <span data-ttu-id="b8e9b-136">Sí</span><span class="sxs-lookup"><span data-stu-id="b8e9b-136">Yes</span></span> | <span data-ttu-id="b8e9b-137">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-137">No</span></span> |
| <span data-ttu-id="b8e9b-138">Números de teléfono administrados en Office 365</span><span class="sxs-lookup"><span data-stu-id="b8e9b-138">Phone numbers managed in Office 365?</span></span> | <span data-ttu-id="b8e9b-139">Sí</span><span class="sxs-lookup"><span data-stu-id="b8e9b-139">Yes</span></span> | <span data-ttu-id="b8e9b-140">Sí</span><span class="sxs-lookup"><span data-stu-id="b8e9b-140">Yes</span></span> | <span data-ttu-id="b8e9b-141">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-141">No</span></span> | <span data-ttu-id="b8e9b-142">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-142">No</span></span> |
| <span data-ttu-id="b8e9b-143">Números de teléfono administrados tanto en el entorno local como en Office 365 (implementación híbrida)</span><span class="sxs-lookup"><span data-stu-id="b8e9b-143">Phone numbers managed both on-premises and in Office 365 (hybrid deployment)?</span></span> | <span data-ttu-id="b8e9b-144">Sí</span><span class="sxs-lookup"><span data-stu-id="b8e9b-144">Yes</span></span> | <span data-ttu-id="b8e9b-145">Sí</span><span class="sxs-lookup"><span data-stu-id="b8e9b-145">Yes</span></span> | <span data-ttu-id="b8e9b-146">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-146">No</span></span> | <span data-ttu-id="b8e9b-147">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-147">No</span></span> |
| <span data-ttu-id="b8e9b-148">¿Desea agregar un plan de llamada de voz RTC?</span><span class="sxs-lookup"><span data-stu-id="b8e9b-148">Option to add a PSTN voice calling plan?</span></span> | <span data-ttu-id="b8e9b-149">Sí</span><span class="sxs-lookup"><span data-stu-id="b8e9b-149">Yes</span></span> | <span data-ttu-id="b8e9b-150">Sí</span><span class="sxs-lookup"><span data-stu-id="b8e9b-150">Yes</span></span> | <span data-ttu-id="b8e9b-151">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-151">No</span></span> | <span data-ttu-id="b8e9b-152">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-152">No</span></span> |
| <span data-ttu-id="b8e9b-153">¿Conferencias RTC?</span><span class="sxs-lookup"><span data-stu-id="b8e9b-153">PSTN Conferencing?</span></span> | <span data-ttu-id="b8e9b-154">Sí</span><span class="sxs-lookup"><span data-stu-id="b8e9b-154">Yes</span></span> | <span data-ttu-id="b8e9b-155">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-155">No</span></span> | <span data-ttu-id="b8e9b-156">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-156">No</span></span> | <span data-ttu-id="b8e9b-157">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-157">No</span></span> |
| <span data-ttu-id="b8e9b-158">Herramientas avanzadas para la colaboración, el análisis y la seguridad</span><span class="sxs-lookup"><span data-stu-id="b8e9b-158">Advanced tools for collaboration, analytics, and security?</span></span> | <span data-ttu-id="b8e9b-159">Sí</span><span class="sxs-lookup"><span data-stu-id="b8e9b-159">Yes</span></span> | <span data-ttu-id="b8e9b-160">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-160">No</span></span> | <span data-ttu-id="b8e9b-161">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-161">No</span></span> | <span data-ttu-id="b8e9b-162">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-162">No</span></span> |
| <span data-ttu-id="b8e9b-163">Informes interactivos, paneles y visualizaciones de datos</span><span class="sxs-lookup"><span data-stu-id="b8e9b-163">Interactive reports, dashboards, and data visualizations?</span></span> | <span data-ttu-id="b8e9b-164">Sí</span><span class="sxs-lookup"><span data-stu-id="b8e9b-164">Yes</span></span> | <span data-ttu-id="b8e9b-165">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-165">No</span></span> | <span data-ttu-id="b8e9b-166">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-166">No</span></span> | <span data-ttu-id="b8e9b-167">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-167">No</span></span> | 
| <span data-ttu-id="b8e9b-168">¿Más control sobre la seguridad y el cumplimiento de los datos con la privacidad, la transparencia y los controles de usuario mejorados?</span><span class="sxs-lookup"><span data-stu-id="b8e9b-168">More control over data security and compliance with built-in privacy, transparency, and refined user controls?</span></span> | <span data-ttu-id="b8e9b-169">Sí</span><span class="sxs-lookup"><span data-stu-id="b8e9b-169">Yes</span></span> | <span data-ttu-id="b8e9b-170">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-170">No</span></span> | <span data-ttu-id="b8e9b-171">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-171">No</span></span> | <span data-ttu-id="b8e9b-172">No</span><span class="sxs-lookup"><span data-stu-id="b8e9b-172">No</span></span> | 

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="b8e9b-173">Clientes de transición hacia los nuevos planes de productos</span><span class="sxs-lookup"><span data-stu-id="b8e9b-173">Transition customers to new product plans</span></span>

<span data-ttu-id="b8e9b-174">Microsoft ofrece continuamente nuevos productos y servicios a nuestros asociados.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-174">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="b8e9b-175">En estos casos, es posible que tenga que actualizar los clientes a nuevos servicios o migrar sus suscripciones de SKU que se apagarán finalmente.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-175">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="b8e9b-176">La migración de los clientes de SKU retiradas a otras más recientes requiere los siguientes pasos:</span><span class="sxs-lookup"><span data-stu-id="b8e9b-176">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

-   <span data-ttu-id="b8e9b-177">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="b8e9b-177">Purchase the new subscription</span></span>
-   <span data-ttu-id="b8e9b-178">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="b8e9b-178">Reassign current user licenses</span></span>
-   <span data-ttu-id="b8e9b-179">Cancelar la suscripción antigua</span><span class="sxs-lookup"><span data-stu-id="b8e9b-179">Cancel the old subscription</span></span>

<span data-ttu-id="b8e9b-180">Siga estos pasos para migrar la suscripción Office 365 Enterprise E4 de un cliente a una de las opciones de la tabla anterior.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-180">Follow these steps to migrate a customer's Office 365 Enterprise E4 subscription to one of the options in the table above.</span></span>

### <a name="step-1---purchase-the-new-subscription"></a><span data-ttu-id="b8e9b-181">Paso 1: compra de la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="b8e9b-181">Step 1 - Purchase the new subscription</span></span>

1. <span data-ttu-id="b8e9b-182">En el menú del **centro de Partners** , seleccione **clientes**, seleccione el cliente que desea migrar y, a continuación, seleccione **Agregar suscripciones**.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-182">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="b8e9b-183">Seleccione la suscripción que desea comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="b8e9b-183">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

   <span data-ttu-id="b8e9b-184">El cliente debería tener ahora suscripciones antiguas y nuevas, la antigua suscripción de Office 365 Enterprise E4 y la nueva suscripción de destino, por ejemplo, la opción 1-Office 365 Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-184">Your customer should now have both old and new subscriptions, the old Office 365 Enterprise E4 subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise E5.</span></span>

### <a name="step-2---reassign-the-customers-users-licenses"></a><span data-ttu-id="b8e9b-185">Paso 2: reasignación de las licencias de los usuarios del cliente</span><span class="sxs-lookup"><span data-stu-id="b8e9b-185">Step 2 - Reassign the customer's users' licenses</span></span>

1. <span data-ttu-id="b8e9b-186">En el menú del **centro de Partners** , seleccione **clientes**, seleccione el cliente que desea migrar y, a continuación, seleccione **usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-186">From the **Partner Center** menu, select **Customers**, select the customer you wish to move, and then select **Users and licenses**.</span></span> <span data-ttu-id="b8e9b-187">Se abre la página usuarios y licencias del cliente.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-187">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="b8e9b-188">Para reasignar licencias de usuario, seleccione el usuario que desea reasignar y, a continuación, seleccione **administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-188">To reassign user licenses, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="b8e9b-189">En la página **administrar licencias** , desactive la casilla **Office 365 Enterprise E4** License y seleccione un nuevo plan de servicio para la suscripción a la que está pasando el cliente.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-189">On the **Manage licenses** page, clear the **Office 365 Enterprise E4** license check box and select a new service plan for the subscription the customer is moving to.</span></span>

4. <span data-ttu-id="b8e9b-190">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="b8e9b-190">Select **Submit**.</span></span> <span data-ttu-id="b8e9b-191">Una página de confirmación enumera las nuevas asignaciones de licencias.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-191">A confirmation page lists the new license assignments.</span></span>

5. <span data-ttu-id="b8e9b-192">Sigue los mismos pasos con otros usuarios del cliente que necesiten la reasignación de licencias.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-192">Continue the same steps with any other customer users that need license reassignment.</span></span>

<span data-ttu-id="b8e9b-193">Después de mover las licencias de usuario al nuevo servicio, puede cancelar con seguridad la suscripción retirada en el nivel superior del cliente.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-193">After moving the user licenses to the new service, you can safely cancel the retired subscription at the top Customer level.</span></span>

### <a name="step-3---cancel-the-old-subscription"></a><span data-ttu-id="b8e9b-194">Paso 3: cancelar la suscripción anterior</span><span class="sxs-lookup"><span data-stu-id="b8e9b-194">Step 3 - Cancel the old subscription</span></span>

1. <span data-ttu-id="b8e9b-195">En el menú del **centro de Partners** , seleccione **clientes**.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-195">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="b8e9b-196">Seleccione el cliente que desea trasladar y seleccione la suscripción que desea cancelar.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-196">Select the customer you want to move, and select the subscription you want to cancel.</span></span>

2. <span data-ttu-id="b8e9b-197">En la página Detalles de la suscripción, establezca el estado de la suscripción en **Suspended**.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-197">In the subscription details page, set the subscription status to **Suspended**.</span></span>

3. <span data-ttu-id="b8e9b-198">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="b8e9b-198">Select **Submit**.</span></span>

<span data-ttu-id="b8e9b-199">La suscripción anterior se suspende y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-199">The old subscription is suspended and the new subscription is active.</span></span> <span data-ttu-id="b8e9b-200">La suscripción suspendida se desaprovisionará automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-200">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="b8e9b-201">El cliente no incurre en costos adicionales para la suscripción antigua.</span><span class="sxs-lookup"><span data-stu-id="b8e9b-201">The customer incurs no additional costs for the old subscription.</span></span>



 



