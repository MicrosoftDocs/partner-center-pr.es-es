---
title: Consolidación de los inquilinos de autorización regional de CSP
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usa estas instrucciones para consolidar los inquilinos para diferentes países o regiones. Esto incluye los pasos para migrar las cuentas de cliente y las suscripciones de cliente.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: LauraBrenner
ms.author: labrenne
keywords: migración de clientes, aprovisionamiento, cuentas de inquilinos, consolidación de inquilinos
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: d361a220ce798863eaeec73e6ff093f135bc4ae1
ms.sourcegitcommit: ca6e0d4a9034120dd600c52ac67b9927dc63b7f5
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/05/2020
ms.locfileid: "84453232"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="69d67-105">Instrucciones para la consolidación de inquilinos de autorización regional de CSP</span><span class="sxs-lookup"><span data-stu-id="69d67-105">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="69d67-106">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="69d67-106">**Applies to**</span></span>

-  <span data-ttu-id="69d67-107">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="69d67-107">Partner Center</span></span>
-  <span data-ttu-id="69d67-108">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="69d67-108">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="69d67-109">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="69d67-109">**Appropriate roles**</span></span>

- <span data-ttu-id="69d67-110">Administrador global</span><span class="sxs-lookup"><span data-stu-id="69d67-110">Global admin</span></span>
- <span data-ttu-id="69d67-111">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="69d67-111">Admin agent</span></span>

<span data-ttu-id="69d67-112">\[Algunos datos se relacionan con productos de versiones preliminares que pueden modificarse sustancialmente antes de su lanzamiento comercial.</span><span class="sxs-lookup"><span data-stu-id="69d67-112">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="69d67-113">Microsoft no ofrece ninguna garantía, expresa o implícita, con respecto a la información aquí proporcionada.\]</span><span class="sxs-lookup"><span data-stu-id="69d67-113">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="69d67-114">Usa estas instrucciones para consolidar los inquilinos para diferentes países o regiones.</span><span class="sxs-lookup"><span data-stu-id="69d67-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

<span data-ttu-id="69d67-115">**Nota**: Debes tener en cuenta todas las suscripciones y recuentos de puestos para tus clientes aprovisionados desde las cuentas de transición.</span><span class="sxs-lookup"><span data-stu-id="69d67-115">**Note**  You must be aware of all of the subscriptions and seat counts for your customers provisioned from the transition accounts.</span></span> <span data-ttu-id="69d67-116">Volverá a aprovisionar las mismas suscripciones exactas con los mismos recuentos de puestos en la nueva cuenta central de CSP como parte del proceso de migración.</span><span class="sxs-lookup"><span data-stu-id="69d67-116">You will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process.</span></span> <span data-ttu-id="69d67-117">Usa la característica de lista de exportación para ayudar a crear una lista de clientes que trasladar al inquilino centralizado.</span><span class="sxs-lookup"><span data-stu-id="69d67-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span> <span data-ttu-id="69d67-118">Los partners eligen si consolidar sus inquilinos.</span><span class="sxs-lookup"><span data-stu-id="69d67-118">Partners choose to consolidate their tenants.</span></span> <span data-ttu-id="69d67-119">Una vez completada la consolidación, los partners no pueden volver a su estado anterior.</span><span class="sxs-lookup"><span data-stu-id="69d67-119">Once consolidation is complete, Partners cannot revert to their previous state.</span></span> <span data-ttu-id="69d67-120">Tenga en cuenta que la acción del cliente también puede ser necesaria.</span><span class="sxs-lookup"><span data-stu-id="69d67-120">Note that customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="69d67-121">Preparación para la migración</span><span class="sxs-lookup"><span data-stu-id="69d67-121">Prepare for migration</span></span>

- <span data-ttu-id="69d67-122">Inicie sesión en el **centro de Partners** con la cuenta de **transición** (existente) (aquella en la que va a realizar la transición) y anote todos los clientes y todos los servicios aprovisionados para esos clientes.</span><span class="sxs-lookup"><span data-stu-id="69d67-122">Sign in to your **Partner Center**  with the **Transitioning** (existing) account (the one you will transition)  and take note of all customers and all of the services provisioned for those customers.</span></span>

   :::image type="content" source="images/regionalcustomer1.png" alt-text="lista de clientes regionales":::

## <a name="migrate-customer-accounts"></a><span data-ttu-id="69d67-124">Migración de las cuentas de cliente</span><span class="sxs-lookup"><span data-stu-id="69d67-124">Migrate customer accounts</span></span>

1. <span data-ttu-id="69d67-125">Inicie sesión en el **centro de Partners** con la cuenta de **transición** (nueva) (la que va a migrar) y vaya a la lista de clientes de **clientes**.</span><span class="sxs-lookup"><span data-stu-id="69d67-125">Sign in to your **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning into) and navigate to the Customers list from **Customers**.</span></span>

2. <span data-ttu-id="69d67-126">Seleccione Clientes.</span><span class="sxs-lookup"><span data-stu-id="69d67-126">Select Customers.</span></span>

3. <span data-ttu-id="69d67-127">Haz clic en **Solicitar una relación de revendedor**.</span><span class="sxs-lookup"><span data-stu-id="69d67-127">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="69d67-128">Se te mostrará un mensaje de correo electrónico predeterminado que presentar a tus clientes.</span><span class="sxs-lookup"><span data-stu-id="69d67-128">You are presented with a default email message to present to your customers.</span></span> <span data-ttu-id="69d67-129">Este mensaje contiene una dirección URL con el identificador de organización exclusivo para tu nueva cuenta del centro de partners.</span><span class="sxs-lookup"><span data-stu-id="69d67-129">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="69d67-130">**Acción de cliente:** Asegúrate de que todos los clientes activos que deseas migrar visitan esta dirección URL.</span><span class="sxs-lookup"><span data-stu-id="69d67-130">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="69d67-131">Al abrir la dirección URL, al cliente se le pedirá que inicie sesión en el portal de Office 365.</span><span class="sxs-lookup"><span data-stu-id="69d67-131">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="69d67-132">El cliente iniciará sesión usando el mismo identificador de organización que utilice para acceder a los portales de administración de Azure y de Office 365.</span><span class="sxs-lookup"><span data-stu-id="69d67-132">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="69d67-133">Tras iniciar sesión, al administrador Global de la cuenta del cliente se le pedirá que envíe un contrato para conceder privilegios de administrador delegado a la nueva cuenta de CSP.</span><span class="sxs-lookup"><span data-stu-id="69d67-133">After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="69d67-134">Si acepta, el cliente seleccionará la casilla y autorizará la relación.</span><span class="sxs-lookup"><span data-stu-id="69d67-134">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="69d67-135">Los clientes aparecerán en la lista de clientes del asociado después de haber enviado el contrato, uno por uno.</span><span class="sxs-lookup"><span data-stu-id="69d67-135">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="69d67-136">Migración de suscripciones basadas en uso de Office 365 y que no sean de Azure</span><span class="sxs-lookup"><span data-stu-id="69d67-136">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="69d67-137">Cuando el cliente haya firmado el contrato, puedes volver a crear sus suscripciones en tu inquilino de partner centralizado.</span><span class="sxs-lookup"><span data-stu-id="69d67-137">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="69d67-138">En el **centro de Partners** , seleccione **clientes**.</span><span class="sxs-lookup"><span data-stu-id="69d67-138">From the **Partner Center** select **Customers**.</span></span>

3. <span data-ttu-id="69d67-139">Abre el nombre de la compañía del cliente que deseas migrar.</span><span class="sxs-lookup"><span data-stu-id="69d67-139">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="69d67-140">Haga clic en **Agregar suscripción**.</span><span class="sxs-lookup"><span data-stu-id="69d67-140">Click **Add subscription**.</span></span>

5. <span data-ttu-id="69d67-141">Agrega las suscripciones y el número de puestos correctos desde el catálogo.</span><span class="sxs-lookup"><span data-stu-id="69d67-141">Add the correct subscriptions and seat counts from the catalog.</span></span> <span data-ttu-id="69d67-142">Verifica los datos con la información proporcionada en las cuentas de partner de **Transición desde**.</span><span class="sxs-lookup"><span data-stu-id="69d67-142">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="lista de clientes":::

6. <span data-ttu-id="69d67-144">Haga clic en **enviar.**</span><span class="sxs-lookup"><span data-stu-id="69d67-144">Click **Submit.**</span></span>

   <span data-ttu-id="69d67-145">Ahora los servicios se proporcionan al cliente desde la cuenta de partner de **Transición a**.</span><span class="sxs-lookup"><span data-stu-id="69d67-145">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="69d67-146">Repite estos pasos para migrar las suscripciones de todos los demás clientes.</span><span class="sxs-lookup"><span data-stu-id="69d67-146">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="69d67-147">Antes de pasar a la siguiente sección, asegúrate de todas las suscripciones de cliente existente en las cuentas de partner de **Transición desde** se vuelven a aprovisionar en la cuenta de partner de **Transición a**.</span><span class="sxs-lookup"><span data-stu-id="69d67-147">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="69d67-148">Los asociados deben suspender las suscripciones en la **transición de** la cuenta de inquilino de asociado del centro de Partners el mismo día en que se realiza la transición de esas suscripciones y se configuran en la cuenta de la **transición a** la cuenta de inquilino del asociado en el centro de partners para asegurarse de que no se produce la facturación doble.</span><span class="sxs-lookup"><span data-stu-id="69d67-148">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="69d67-149">Se denegarán las solicitudes de soporte técnico referentes a créditos debidas a cualquier superposición en la facturación que se produzca por no deshabilitar correctamente las suscripciones de **Transición desde**.</span><span class="sxs-lookup"><span data-stu-id="69d67-149">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="69d67-150">Deshabilitar las suscripciones de Office 365 en la cuenta de partner de Transición desde</span><span class="sxs-lookup"><span data-stu-id="69d67-150">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="69d67-151">Deshabilitar la suscripción de CSP de las cuentas de partner de **Transición desde** detiene toda facturación futura.</span><span class="sxs-lookup"><span data-stu-id="69d67-151">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="69d67-152">No es necesario deshabilitar manualmente las suscripciones de Azure, porque las suscripciones de Azure se deshabilitan automáticamente durante el proceso de migración.</span><span class="sxs-lookup"><span data-stu-id="69d67-152">You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="69d67-153">Inicie sesión en el **centro de Partners** con la **transición de** la cuenta de CSP y navegue hasta la lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="69d67-153">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="69d67-154">Abre al cliente cuyas suscripciones quieras deshabilitar y, a continuación, selecciona la primera oferta que deshabilitar.</span><span class="sxs-lookup"><span data-stu-id="69d67-154">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="69d67-155">Establece la suscripción en **suspendida**y, a continuación, haz clic en **enviar**.</span><span class="sxs-lookup"><span data-stu-id="69d67-155">Set the subscription to **suspended**, and then click **submit**.</span></span>

   >[!Note]
   >  <span data-ttu-id="69d67-156">Suspender la suscripción garantiza que no se produzca la facturación.</span><span class="sxs-lookup"><span data-stu-id="69d67-156">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="69d67-157">La suscripción muestra **suspendida** en la lista de suscripciones.</span><span class="sxs-lookup"><span data-stu-id="69d67-157">The Subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="69d67-158">Repite estos pasos para todas las suscripciones del cliente.</span><span class="sxs-lookup"><span data-stu-id="69d67-158">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="69d67-159">Comprueba que todas muestran **suspendida.**</span><span class="sxs-lookup"><span data-stu-id="69d67-159">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="69d67-160">Selecciona al siguiente cliente de la lista y repite el proceso de deshabilitar todas las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="69d67-160">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="69d67-161">Migración de suscripciones basadas en uso de Azure</span><span class="sxs-lookup"><span data-stu-id="69d67-161">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="69d67-162">No es necesario migrar manualmente las suscripciones de CSP basadas en el uso de Azure como sucede con las suscripciones de Office 365 CSP.</span><span class="sxs-lookup"><span data-stu-id="69d67-162">Azure, usage-based CSP subscriptions do not need to be migrated manually as is the case with Office 365 CSP subscriptions.</span></span> <span data-ttu-id="69d67-163">El soporte técnico de Microsoft Azure puede migrar las suscripciones de Azure, así como todos los servicios o los recursos implementados, desde las cuentas de revendedor de CSP de **Transición desde** a la cuenta de revendedor de CSP de **Transición a**.</span><span class="sxs-lookup"><span data-stu-id="69d67-163">Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="69d67-164">Durante esta transición, el cliente no experimentará ninguna interrupción del servicio.</span><span class="sxs-lookup"><span data-stu-id="69d67-164">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="69d67-165">Asegúrate de que las cuentas de cliente que necesitan que se migren las suscripciones de Azure han aceptado el acuerdo que se asociará con la nueva cuenta de CSP de **Transición a**.</span><span class="sxs-lookup"><span data-stu-id="69d67-165">Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="69d67-166">Los asociados notifican a Microsoft qué cuentas de cliente que tienen suscripciones de Azure están listas para su migración y proporciona los nombres de la compañía de los clientes.</span><span class="sxs-lookup"><span data-stu-id="69d67-166">Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer's company names.</span></span>

3. <span data-ttu-id="69d67-167">Microsoft migra las suscripciones basadas en uso de Azure y notifica a los partners cuándo se ha completado la migración.</span><span class="sxs-lookup"><span data-stu-id="69d67-167">Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.</span></span>

4. <span data-ttu-id="69d67-168">El partner confirma que la suscripción de Azure en las cuentas de revendedor de CSP de **Transición desde** ahora muestra suspendida en el Centro de partners, en la sección de suscripciones del cliente.</span><span class="sxs-lookup"><span data-stu-id="69d67-168">The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="69d67-169">El partner confirma que la suscripción de Azure las cuenta de revendedor de CSP de **Transición a** ahora muestra un estado de **activa** en el Centro de partners, en la sección de suscripciones del cliente.</span><span class="sxs-lookup"><span data-stu-id="69d67-169">The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="69d67-170">Deshabilitar las suscripciones en el cliente no cambia la apariencia del cliente en la lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="69d67-170">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="69d67-171">Actualmente no hay ninguna opción para quitar clientes de la lista.</span><span class="sxs-lookup"><span data-stu-id="69d67-171">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="69d67-172">Los partners deben evitar volver a agregar suscripciones a estos clientes en el futuro desde su cuenta de **Transición desde**.</span><span class="sxs-lookup"><span data-stu-id="69d67-172">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="69d67-173">Repite estos pasos para todas las suscripciones de todos tus clientes para detener futuros cargos en las cuentas **Transición desde**.</span><span class="sxs-lookup"><span data-stu-id="69d67-173">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="69d67-174">El partner recibirá una factura final con un crédito por el número de días sin usar entre el día de la cancelación y el último día del período de facturación.</span><span class="sxs-lookup"><span data-stu-id="69d67-174">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="69d67-175">Tras ese período de facturación final, no se generarán más futuras.</span><span class="sxs-lookup"><span data-stu-id="69d67-175">No future invoices will generate after that final billing period.</span></span>

### <a name="notes"></a><span data-ttu-id="69d67-176">Notas</span><span class="sxs-lookup"><span data-stu-id="69d67-176">Notes</span></span>

- <span data-ttu-id="69d67-177">Deshabilitar la suscripción de la cuenta de la **transición de** CSP no afecta al servicio del cliente final, siempre que el servicio se haya aprovisionado desde la cuenta de **transición a** CSP antes de deshabilitar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="69d67-177">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="69d67-178">El cliente no puede usar las suscripciones y no genera cargos cuando se suspende o cancela.</span><span class="sxs-lookup"><span data-stu-id="69d67-178">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="69d67-179">Actualmente no hay ninguna manera de quitar por completo a un cliente de la lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="69d67-179">There is currently no way to remove a customer from the Customers list completely.</span></span>

>[!Note]
> <span data-ttu-id="69d67-180">Los asociados deben suspender las suscripciones en la **transición de** la cuenta de inquilino del asociado en el centro de Partners el mismo día en el que se realiza la transición de esas suscripciones y se configuran en la cuenta de **transición a** inquilino del asociado en el centro de partners para asegurarse de que no se produce la facturación doble.</span><span class="sxs-lookup"><span data-stu-id="69d67-180">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="69d67-181">Microsoft no admitirá solicitudes de créditos debido a cualquier superposición en la facturación que se produce cuando no se establece correctamente la **transición de** las suscripciones a suspendidas.</span><span class="sxs-lookup"><span data-stu-id="69d67-181">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="69d67-182">Simplificación de la migración mediante la exportación</span><span class="sxs-lookup"><span data-stu-id="69d67-182">Simplify migration using Export</span></span>

<span data-ttu-id="69d67-183">Si usas la **Función de exportación**, puedes capturar las suscripciones que necesites usar en tu nueva estructura consolidada:</span><span class="sxs-lookup"><span data-stu-id="69d67-183">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="69d67-184">Haga clic en **clientes** en el centro de partners para ver la lista de clientes de la estructura existente.</span><span class="sxs-lookup"><span data-stu-id="69d67-184">Click **Customers** on Partner Center to see the list of customers in your existing structure.</span></span>

2. <span data-ttu-id="69d67-185">Abre el nombre del cliente deseado.</span><span class="sxs-lookup"><span data-stu-id="69d67-185">Open the desired customer name.</span></span>

3. <span data-ttu-id="69d67-186">En la página **Suscripciones**, haz clic en **Exportar suscripciones** para exportar los detalles de las suscripciones a un archivo de Excel.</span><span class="sxs-lookup"><span data-stu-id="69d67-186">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="69d67-187">Usa esta lista para volver a crear las suscripciones en el nuevo inquilino consolidado.</span><span class="sxs-lookup"><span data-stu-id="69d67-187">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="69d67-188">Registro de API</span><span class="sxs-lookup"><span data-stu-id="69d67-188">API registration</span></span>

<span data-ttu-id="69d67-189">Para obtener más información sobre el registro de API, consulte [configuración del acceso de API en el centro de Partners](https://go.microsoft.com/fwlink/?linkid=847990).</span><span class="sxs-lookup"><span data-stu-id="69d67-189">For more information about API registration, see [Set up API access in Partner Center](https://go.microsoft.com/fwlink/?linkid=847990).</span></span>
