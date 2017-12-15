---
title: "Consolidación de los inquilinos de autorización regional de CSP | Centro de partners"
description: "Usa estas instrucciones para consolidar los inquilinos para diferentes países o regiones."
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.openlocfilehash: 655bcee32824f0a2a8859951edea35b2d56922a8
ms.sourcegitcommit: 6215068443504ee777880bffcb1e85fea3b3bfeb
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/16/2017
---
# <a name="csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="5ba06-103">Consolidación de los inquilinos de autorización regional de CSP</span><span class="sxs-lookup"><span data-stu-id="5ba06-103">CSP regional authorization tenant consolidation</span></span>

**<span data-ttu-id="5ba06-104">Se aplica a</span><span class="sxs-lookup"><span data-stu-id="5ba06-104">Applies to</span></span>**

-  <span data-ttu-id="5ba06-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="5ba06-105">Partner Center</span></span>
-  <span data-ttu-id="5ba06-106">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="5ba06-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="5ba06-107">Centro de partners para Microsoft Cloud Alemania</span><span class="sxs-lookup"><span data-stu-id="5ba06-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="5ba06-108">\[Parte de la información hace referencia a la versión preliminar del producto, que puede sufrir modificaciones importantes antes de que se publique la versión comercial.</span><span class="sxs-lookup"><span data-stu-id="5ba06-108">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="5ba06-109">Microsoft no ofrece ninguna garantía, expresa o implícita, respecto a la información que se ofrece aquí.\]</span><span class="sxs-lookup"><span data-stu-id="5ba06-109">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="5ba06-110">Usa estas instrucciones para consolidar los inquilinos para diferentes países o regiones.</span><span class="sxs-lookup"><span data-stu-id="5ba06-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="5ba06-111">**Nota**: Debes tener en cuenta todas las suscripciones y recuentos de puestos para tus clientes aprovisionados desde las cuentas de transición.</span><span class="sxs-lookup"><span data-stu-id="5ba06-111">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="5ba06-112">Se te volverá a aprovisionar esas mismas suscripciones exactas con la misma cantidad de puestos en la nueva cuenta de Central CSP como parte del proceso de migración.</span><span class="sxs-lookup"><span data-stu-id="5ba06-112">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="5ba06-113">Usa la característica de lista de exportación para ayudar a crear una lista de clientes que trasladar al inquilino centralizado.</span><span class="sxs-lookup"><span data-stu-id="5ba06-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="5ba06-114">Los partners eligen si consolidar sus inquilinos.</span><span class="sxs-lookup"><span data-stu-id="5ba06-114">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="5ba06-115">Una vez completada la consolidación, los partners no pueden volver a su estado anterior.</span><span class="sxs-lookup"><span data-stu-id="5ba06-115">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="5ba06-116">Ten en cuenta que es posible que también sean necesarias ciertas acciones por parte del cliente.</span><span class="sxs-lookup"><span data-stu-id="5ba06-116">Note that customer action may also be required.</span></span>

 

## <a name="prepare-for-migration"></a><span data-ttu-id="5ba06-117">Preparación para la migración</span><span class="sxs-lookup"><span data-stu-id="5ba06-117">Prepare for migration</span></span>


-   <span data-ttu-id="5ba06-118">Inicia sesión en <https://partnercenter.microsoft.com> con la cuenta de transición (la cuenta existente) y tome nota de todos los clientes y todos los servicios aprovisionados para dichos clientes.</span><span class="sxs-lookup"><span data-stu-id="5ba06-118">Log on to <https://partnercenter.microsoft.com> with the Transitioning (existing) account and take note of all customers and all of the services provisioned for those customers.</span></span>

![lista de clientes regionales](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a><span data-ttu-id="5ba06-120">Migración de las cuentas de cliente</span><span class="sxs-lookup"><span data-stu-id="5ba06-120">Migrate customer accounts</span></span>


1.  <span data-ttu-id="5ba06-121">Inicia sesión en <https://partnercenter.microsoft.com> con la cuenta de transición (la nueva cuenta) y navega hasta la lista de clientes desde el panel del centro de partners.</span><span class="sxs-lookup"><span data-stu-id="5ba06-121">Log on to <https://partnercenter.microsoft.com> with the Transitioning (new) account and navigate to the Customers list from the Partner Center dashboard.</span></span>

2.  <span data-ttu-id="5ba06-122">Selecciona Clientes.</span><span class="sxs-lookup"><span data-stu-id="5ba06-122">Select Customers.</span></span>

3.  <span data-ttu-id="5ba06-123">Haz clic en **Solicitar una relación de revendedor**.</span><span class="sxs-lookup"><span data-stu-id="5ba06-123">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="5ba06-124">Se te mostrará un mensaje de correo electrónico predeterminado que presentar a tus clientes.</span><span class="sxs-lookup"><span data-stu-id="5ba06-124">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="5ba06-125">Este mensaje contiene una dirección URL con el identificador de organización exclusivo para tu nueva cuenta del centro de partners.</span><span class="sxs-lookup"><span data-stu-id="5ba06-125">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4.  <span data-ttu-id="5ba06-126">**Acción de cliente:** Asegúrate de que todos los clientes activos que deseas migrar visitan esta dirección URL.</span><span class="sxs-lookup"><span data-stu-id="5ba06-126">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="5ba06-127">Al abrir la dirección URL, al cliente se le pedirá que inicie sesión en el portal de Office 365.</span><span class="sxs-lookup"><span data-stu-id="5ba06-127">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="5ba06-128">El cliente iniciará sesión usando el mismo identificador de organización que utilice para acceder a los portales de administración de Azure y de Office 365.</span><span class="sxs-lookup"><span data-stu-id="5ba06-128">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5.  <span data-ttu-id="5ba06-129">Tras iniciar sesión, al administrador Global de la cuenta del cliente se le pedirá que envíe un contrato para conceder privilegios de administrador delegado a la nueva cuenta de CSP.</span><span class="sxs-lookup"><span data-stu-id="5ba06-129">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="5ba06-130">Si acepta, el cliente seleccionará la casilla y autorizará la relación.</span><span class="sxs-lookup"><span data-stu-id="5ba06-130">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="5ba06-131">Los clientes aparecerán en la lista de clientes del partner después de enviar el acuerdo, uno por uno.</span><span class="sxs-lookup"><span data-stu-id="5ba06-131">The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="5ba06-132">Migración de suscripciones basadas en uso de Office 365 y que no sean de Azure</span><span class="sxs-lookup"><span data-stu-id="5ba06-132">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>


1.  <span data-ttu-id="5ba06-133">Cuando el cliente haya firmado el contrato, puedes volver a crear sus suscripciones en tu inquilino de partner centralizado.</span><span class="sxs-lookup"><span data-stu-id="5ba06-133">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2.  <span data-ttu-id="5ba06-134">En el panel del centro de partners, haz clic en **Clientes** en la barra de navegación izquierda.</span><span class="sxs-lookup"><span data-stu-id="5ba06-134">On the Partner Center Dashboard click on **Customers** in the left navigation</span></span>

3.  <span data-ttu-id="5ba06-135">Abre el nombre de la compañía del cliente que deseas migrar.</span><span class="sxs-lookup"><span data-stu-id="5ba06-135">Open the company name for the customer you want to migrate.</span></span>

4.  <span data-ttu-id="5ba06-136">Haz clic en **Agregar suscripción**.</span><span class="sxs-lookup"><span data-stu-id="5ba06-136">Click **Add subscription**.</span></span>

5.  <span data-ttu-id="5ba06-137">Agrega las suscripciones y el número de puestos correctos desde el catálogo.</span><span class="sxs-lookup"><span data-stu-id="5ba06-137">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="5ba06-138">Verifica los datos con la información proporcionada en las cuentas de partner de **Transición desde**.</span><span class="sxs-lookup"><span data-stu-id="5ba06-138">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

    ![captura de pantalla de la lista de clientes](images/regionalcustomer2.png)

6.  <span data-ttu-id="5ba06-140">Haz clic en **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="5ba06-140">Click **Submit.**</span></span>

<span data-ttu-id="5ba06-141">Ahora los servicios se proporcionan al cliente desde la cuenta de partner de **Transición a**.</span><span class="sxs-lookup"><span data-stu-id="5ba06-141">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

<span data-ttu-id="5ba06-142">Repite estos pasos para migrar las suscripciones de todos los demás clientes.</span><span class="sxs-lookup"><span data-stu-id="5ba06-142">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="5ba06-143">Antes de pasar a la siguiente sección, asegúrate de todas las suscripciones de cliente existente en las cuentas de partner de **Transición desde** se vuelven a aprovisionar en la cuenta de partner de **Transición a**.</span><span class="sxs-lookup"><span data-stu-id="5ba06-143">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

<span data-ttu-id="5ba06-144">**Nota** Los partners deben suspender las suscripciones en la cuenta de inquilino de partner de **Transición desde** en el Centro de partners el mismo día que se realice la transición de dichas suscripciones y configurarlas en la cuenta de inquilino de partner de **Transición a** en el Centro de partners para asegurarse de que no se produce una facturación doble.</span><span class="sxs-lookup"><span data-stu-id="5ba06-144">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="5ba06-145">Se denegarán las solicitudes de soporte técnico referentes a créditos debidas a cualquier superposición en la facturación que se produzca por no deshabilitar correctamente las suscripciones de **Transición desde**.</span><span class="sxs-lookup"><span data-stu-id="5ba06-145">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="5ba06-146">Deshabilitar las suscripciones de Office 365 en la cuenta de partner de Transición desde</span><span class="sxs-lookup"><span data-stu-id="5ba06-146">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>


<span data-ttu-id="5ba06-147">Deshabilitar la suscripción de CSP de las cuentas de partner de **Transición desde** detiene toda facturación futura.</span><span class="sxs-lookup"><span data-stu-id="5ba06-147">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="5ba06-148">No es necesario deshabilitar manualmente las suscripciones de Azure, porque las suscripciones de Azure se deshabilitan automáticamente durante el proceso de migración.</span><span class="sxs-lookup"><span data-stu-id="5ba06-148">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1.  <span data-ttu-id="5ba06-149">Inicia sesión en <https://partnercenter.microsoft.com> con la cuenta de CSP de **Transición desde** y navega hasta la lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="5ba06-149">Log on to <https://partnercenter.microsoft.com> with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2.  <span data-ttu-id="5ba06-150">Abre al cliente cuyas suscripciones quieras deshabilitar y, a continuación, selecciona la primera oferta que deshabilitar.</span><span class="sxs-lookup"><span data-stu-id="5ba06-150">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>
3.  <span data-ttu-id="5ba06-151">Establece la suscripción en **suspendida**y, a continuación, haz clic en **enviar**.</span><span class="sxs-lookup"><span data-stu-id="5ba06-151">Set the subscription to **suspended**, and then click **submit**.</span></span>

    <span data-ttu-id="5ba06-152">**Nota**: Suspender la suscripción garantiza que no se produce una facturación doble.</span><span class="sxs-lookup"><span data-stu-id="5ba06-152">**Note**  Suspending the subscription ensures double billing does not occur.</span></span>

     

    <span data-ttu-id="5ba06-153">La suscripción muestra **suspendida** en la lista de suscripciones.</span><span class="sxs-lookup"><span data-stu-id="5ba06-153">The Subscription shows **suspended** on the subscriptions list.</span></span>

4.  <span data-ttu-id="5ba06-154">Repite estos pasos para todas las suscripciones del cliente.</span><span class="sxs-lookup"><span data-stu-id="5ba06-154">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="5ba06-155">Comprueba que todas muestran **suspendida.**</span><span class="sxs-lookup"><span data-stu-id="5ba06-155">Verify all show **suspended.**</span></span>

5.  <span data-ttu-id="5ba06-156">Selecciona al siguiente cliente de la lista y repite el proceso de deshabilitar todas las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="5ba06-156">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="5ba06-157">Migración de suscripciones basadas en uso de Azure</span><span class="sxs-lookup"><span data-stu-id="5ba06-157">Migrating Azure usage-based subscriptions</span></span>


<span data-ttu-id="5ba06-158">Ten en cuenta que no es necesario migrar las suscripciones de CSP basadas en el uso de Azure de forma manual, como sucede con las suscripciones de CSP de Office 365.</span><span class="sxs-lookup"><span data-stu-id="5ba06-158">Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="5ba06-159">El soporte técnico de Microsoft Azure puede migrar las suscripciones de Azure, así como todos los servicios o los recursos implementados, desde las cuentas de revendedor de CSP de **Transición desde** a la cuenta de revendedor de CSP de **Transición a**.</span><span class="sxs-lookup"><span data-stu-id="5ba06-159">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="5ba06-160">Durante esta transición, el cliente no experimentará ninguna interrupción del servicio.</span><span class="sxs-lookup"><span data-stu-id="5ba06-160">There will be no disruption of service to the customer during this transition.</span></span>

1.  <span data-ttu-id="5ba06-161">Asegúrate de que las cuentas de cliente que necesitan que se migren las suscripciones de Azure han aceptado el acuerdo que se asociará con la nueva cuenta de CSP de **Transición a**.</span><span class="sxs-lookup"><span data-stu-id="5ba06-161">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>
2.  <span data-ttu-id="5ba06-162">Los partners notifican a Microsoft qué cuentas de cliente que tienen suscripciones de Azure están listas para migrar y proporciona los nombres de compañía de dichos clientes.</span><span class="sxs-lookup"><span data-stu-id="5ba06-162">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.</span></span>
3.  <span data-ttu-id="5ba06-163">Microsoft migra las suscripciones basadas en uso de Azure y notifica a los partners cuándo se ha completado la migración.</span><span class="sxs-lookup"><span data-stu-id="5ba06-163">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>
4.  <span data-ttu-id="5ba06-164">El partner confirma que la suscripción de Azure en las cuentas de revendedor de CSP de **Transición desde** ahora muestra suspendida en el Centro de partners, en la sección de suscripciones del cliente.</span><span class="sxs-lookup"><span data-stu-id="5ba06-164">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>
5.  <span data-ttu-id="5ba06-165">El partner confirma que la suscripción de Azure las cuenta de revendedor de CSP de **Transición a** ahora muestra un estado de **activa** en el Centro de partners, en la sección de suscripciones del cliente.</span><span class="sxs-lookup"><span data-stu-id="5ba06-165">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

    <span data-ttu-id="5ba06-166">**Nota**: Deshabilitar las suscripciones en el cliente no modifica la apariencia de dicho cliente en la lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="5ba06-166">**Note**  Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="5ba06-167">Actualmente no hay ninguna opción para quitar clientes de la lista.</span><span class="sxs-lookup"><span data-stu-id="5ba06-167">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="5ba06-168">Los partners deben evitar volver a agregar suscripciones a estos clientes en el futuro desde su cuenta de **Transición desde**.</span><span class="sxs-lookup"><span data-stu-id="5ba06-168">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

     

6.  <span data-ttu-id="5ba06-169">Repite estos pasos para todas las suscripciones de todos tus clientes para detener futuros cargos en las cuentas **Transición desde**.</span><span class="sxs-lookup"><span data-stu-id="5ba06-169">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="5ba06-170">El partner recibirá una factura final con un crédito por el número de días sin usar entre el día de la cancelación y el último día del período de facturación.</span><span class="sxs-lookup"><span data-stu-id="5ba06-170">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="5ba06-171">Tras ese período de facturación final, no se generarán más futuras.</span><span class="sxs-lookup"><span data-stu-id="5ba06-171">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="5ba06-172">Notas</span><span class="sxs-lookup"><span data-stu-id="5ba06-172">Notes</span></span>

-   <span data-ttu-id="5ba06-173">Deshabilitar la suscripción desde la cuenta de CSP de **Transición desde** no afecta a servicio del cliente final, siempre que el servicio se haya aprovisionado desde la cuenta de CSP **Transición a** antes de la deshabilitación.</span><span class="sxs-lookup"><span data-stu-id="5ba06-173">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.</span></span>

-   <span data-ttu-id="5ba06-174">El cliente no puede usar las suscripciones y estas no generarán cargos cuando se suspendan o se cancelen.</span><span class="sxs-lookup"><span data-stu-id="5ba06-174">Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.</span></span>

-   <span data-ttu-id="5ba06-175">Actualmente no hay ninguna manera de quitar por completo a un cliente de la lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="5ba06-175">There is currently no way to remove a customer from the Customers list completely.</span></span>

-   <span data-ttu-id="5ba06-176">**Nota** Los partners deben suspender las suscripciones en la cuenta de inquilino de partner de **Transición desde** en el Centro de partners el mismo día que se realice la transición de dichas suscripciones y configurarlas en la cuenta de inquilino de partner de **Transición a** en el Centro de partners para asegurarse de que no se produce una facturación doble.</span><span class="sxs-lookup"><span data-stu-id="5ba06-176">**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="5ba06-177">Microsoft no admitirá las solicitudes de soporte técnico referentes a créditos debidas a cualquier superposición en la facturación que se produzca por no deshabilitar correctamente las suscripciones de **Transición desde**.</span><span class="sxs-lookup"><span data-stu-id="5ba06-177">Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

     

### <a name="simplify-migration-using-export"></a><span data-ttu-id="5ba06-178">Simplificación de la migración mediante la exportación</span><span class="sxs-lookup"><span data-stu-id="5ba06-178">Simplify migration using Export</span></span>

<span data-ttu-id="5ba06-179">Si usas la **Función de exportación**, puedes capturar las suscripciones que necesites usar en tu nueva estructura consolidada:</span><span class="sxs-lookup"><span data-stu-id="5ba06-179">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1.  <span data-ttu-id="5ba06-180">Haz clic en **Clientes** en el panel para ver la lista de clientes de la estructura existente.</span><span class="sxs-lookup"><span data-stu-id="5ba06-180">Click **Customers** on your Dashboard to see the list of customers in your existing structure.</span></span>

2.  <span data-ttu-id="5ba06-181">Abre el nombre del cliente deseado.</span><span class="sxs-lookup"><span data-stu-id="5ba06-181">Open the desired customer name.</span></span>

3.  <span data-ttu-id="5ba06-182">En la página **Suscripciones**, haz clic en **Exportar suscripciones** para exportar los detalles de las suscripciones a un archivo de Excel.</span><span class="sxs-lookup"><span data-stu-id="5ba06-182">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4.  <span data-ttu-id="5ba06-183">Usa esta lista para volver a crear las suscripciones en el nuevo inquilino consolidado.</span><span class="sxs-lookup"><span data-stu-id="5ba06-183">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="5ba06-184">Registro de API</span><span class="sxs-lookup"><span data-stu-id="5ba06-184">API registration</span></span>

<span data-ttu-id="5ba06-185">Para obtener más información acerca del registro de API, visita esta [página web](https://go.microsoft.com/fwlink/?linkid=847990) (en inglés).</span><span class="sxs-lookup"><span data-stu-id="5ba06-185">For more information about API registration, [see this page](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>

## <a name="partner-center-activity-log"></a><span data-ttu-id="5ba06-186">Registro de actividades del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="5ba06-186">Partner Center Activity log</span></span>


<span data-ttu-id="5ba06-187">Con el registro de actividades, los partners pueden ver un registro de todos los cambios que afectan a los clientes en su inquilino.</span><span class="sxs-lookup"><span data-stu-id="5ba06-187">With the Activity log, partners can view a record of all customer-affecting changes made on their tenant.</span></span> <span data-ttu-id="5ba06-188">Esto ayuda a los partners a realizar un seguimiento de los cambios en un inquilino del cliente.</span><span class="sxs-lookup"><span data-stu-id="5ba06-188">This helps partners track changes on a customer tenant.</span></span>

**<span data-ttu-id="5ba06-189">Ver el registro de actividades</span><span class="sxs-lookup"><span data-stu-id="5ba06-189">View the Activity log</span></span>**

1.  <span data-ttu-id="5ba06-190">En el panel del Centro de partners, haz clic en el vínculo **Registro de actividades**.</span><span class="sxs-lookup"><span data-stu-id="5ba06-190">From the Partner Center Dashboard, click the **Activity Log** link.</span></span>
2.  <span data-ttu-id="5ba06-191">En la página **Registro de actividades**, mira los cambios realizados en las cuentas de cliente.</span><span class="sxs-lookup"><span data-stu-id="5ba06-191">On the **Activity Log** page, view the changes made to customer accounts.</span></span> <span data-ttu-id="5ba06-192">Para filtrar el registro de actividades por fecha, elige las fechas **Desde** y **A** para restringir los registros seleccionados en el registro.</span><span class="sxs-lookup"><span data-stu-id="5ba06-192">To filter the Activity log by date, pick **from** and **to** dates to narrow the selected records in the log.</span></span> <span data-ttu-id="5ba06-193">Para filtrar por cliente en el **Registro de actividades**, usa el cuadro de búsqueda.</span><span class="sxs-lookup"><span data-stu-id="5ba06-193">To filter by customer in the **Activity log**, use the search box.</span></span>

**<span data-ttu-id="5ba06-194">Exportación del registro de actividades</span><span class="sxs-lookup"><span data-stu-id="5ba06-194">Export the Activity log</span></span>**

-   <span data-ttu-id="5ba06-195">Haz clic en **Exportar registro** para exportar los datos del registro de actividades a un archivo CSV.</span><span class="sxs-lookup"><span data-stu-id="5ba06-195">Click **Export log** to export your Activity log data to a CSV file.</span></span>

    <span data-ttu-id="5ba06-196">También puedes exportar la lista de clientes y la lista de suscripciones de un cliente individual (desde la página de suscripción de dicho cliente).</span><span class="sxs-lookup"><span data-stu-id="5ba06-196">You can also export the customer list and the subscription list of a single customer (from the customer’s subscription page).</span></span>

 

 



