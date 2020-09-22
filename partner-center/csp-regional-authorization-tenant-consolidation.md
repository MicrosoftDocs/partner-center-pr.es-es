---
title: Consolidación de los inquilinos de autorización regional de CSP
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usa estas instrucciones para consolidar los inquilinos para diferentes países o regiones. Esto incluye los pasos para migrar las cuentas de cliente y las suscripciones de cliente.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 232eae10927d8ac38b4cce0842fbb8e4278f8d03
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000379"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="c047a-104">Instrucciones para la consolidación de los inquilinos de autorización regional de CSP</span><span class="sxs-lookup"><span data-stu-id="c047a-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="c047a-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="c047a-105">**Applies to**</span></span>

-  <span data-ttu-id="c047a-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="c047a-106">Partner Center</span></span>
-  <span data-ttu-id="c047a-107">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="c047a-107">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="c047a-108">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="c047a-108">**Appropriate roles**</span></span>

- <span data-ttu-id="c047a-109">Administrador global</span><span class="sxs-lookup"><span data-stu-id="c047a-109">Global admin</span></span>
- <span data-ttu-id="c047a-110">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="c047a-110">Admin agent</span></span>

<span data-ttu-id="c047a-111">\[Algunos datos se relacionan con productos de versiones preliminares que pueden modificarse sustancialmente antes de su lanzamiento comercial.</span><span class="sxs-lookup"><span data-stu-id="c047a-111">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="c047a-112">Microsoft no proporciona ninguna garantía, expresa o implícita, con respecto a la información proporcionada aquí.\]</span><span class="sxs-lookup"><span data-stu-id="c047a-112">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="c047a-113">Puede consolidar los inquilinos para su empresa.</span><span class="sxs-lookup"><span data-stu-id="c047a-113">You can consolidate tenants for your business.</span></span> <span data-ttu-id="c047a-114">Usa estas instrucciones para consolidar los inquilinos para diferentes países o regiones.</span><span class="sxs-lookup"><span data-stu-id="c047a-114">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="c047a-115">Debe tener en cuenta todas las suscripciones y los recuentos de licencias aprovisionados para cada uno de los clientes de la cuenta desde la que va a realizar la transición.</span><span class="sxs-lookup"><span data-stu-id="c047a-115">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="c047a-116">Volverá a aprovisionar las mismas suscripciones exactas con los mismos recuentos de licencias en la nueva cuenta central de CSP como parte del proceso de migración.</span><span class="sxs-lookup"><span data-stu-id="c047a-116">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="c047a-117">Usa la característica de lista de exportación para ayudar a crear una lista de clientes que trasladar al inquilino centralizado.</span><span class="sxs-lookup"><span data-stu-id="c047a-117">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="c047a-118">Una vez completada la consolidación, no se puede revertir al estado anterior del inquilino.</span><span class="sxs-lookup"><span data-stu-id="c047a-118">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="c047a-119">También es posible que se necesiten acciones del cliente.</span><span class="sxs-lookup"><span data-stu-id="c047a-119">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="c047a-120">Preparación para la migración</span><span class="sxs-lookup"><span data-stu-id="c047a-120">Prepare for migration</span></span>

- <span data-ttu-id="c047a-121">Inicie sesión en el **centro de Partners**  mediante la cuenta de **transición** (la que va a pasar a la nueva cuenta) y Revise todos los clientes y todos los servicios aprovisionados para esos clientes.</span><span class="sxs-lookup"><span data-stu-id="c047a-121">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="c047a-122">Cierre la sesión de esta cuenta.</span><span class="sxs-lookup"><span data-stu-id="c047a-122">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="c047a-123">Migración de las cuentas de cliente</span><span class="sxs-lookup"><span data-stu-id="c047a-123">Migrate customer accounts</span></span>

1. <span data-ttu-id="c047a-124">Inicie sesión en el **centro de Partners**  con la cuenta de **transición** (nueva) (aquella en la que va a realizar la transición de los clientes).</span><span class="sxs-lookup"><span data-stu-id="c047a-124">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="c047a-125">Seleccione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="c047a-125">Select **Customers**.</span></span>

3. <span data-ttu-id="c047a-126">Haz clic en **Solicitar una relación de revendedor**.</span><span class="sxs-lookup"><span data-stu-id="c047a-126">Click **Request a reseller relationship**.</span></span> <span data-ttu-id="c047a-127">Se le presentará un mensaje de correo electrónico predeterminado para enviarlo a sus clientes.</span><span class="sxs-lookup"><span data-stu-id="c047a-127">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="c047a-128">Este mensaje contiene una dirección URL con el identificador de organización exclusivo para tu nueva cuenta del centro de partners.</span><span class="sxs-lookup"><span data-stu-id="c047a-128">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="c047a-129">**Acción de cliente:** Asegúrate de que todos los clientes activos que deseas migrar visitan esta dirección URL.</span><span class="sxs-lookup"><span data-stu-id="c047a-129">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="c047a-130">Al abrir la dirección URL, al cliente se le pedirá que inicie sesión en el portal de Office 365.</span><span class="sxs-lookup"><span data-stu-id="c047a-130">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="c047a-131">El cliente iniciará sesión usando el mismo identificador de organización que utilice para acceder a los portales de administración de Azure y de Office 365.</span><span class="sxs-lookup"><span data-stu-id="c047a-131">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="c047a-132">Después de iniciar sesión, se pide al administrador global de la **cuenta de cliente** que envíe un contrato que proporcione privilegios de administrador delegado a la nueva cuenta de CSP.</span><span class="sxs-lookup"><span data-stu-id="c047a-132">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="c047a-133">Si acepta, el cliente seleccionará la casilla y autorizará la relación.</span><span class="sxs-lookup"><span data-stu-id="c047a-133">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="c047a-134">Los clientes aparecerán en la lista de clientes del asociado después de haber enviado el contrato, uno por uno.</span><span class="sxs-lookup"><span data-stu-id="c047a-134">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="c047a-135">Migración de suscripciones basadas en uso de Office 365 y que no sean de Azure</span><span class="sxs-lookup"><span data-stu-id="c047a-135">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="c047a-136">Cuando el cliente haya firmado el contrato, puedes volver a crear sus suscripciones en tu inquilino de partner centralizado.</span><span class="sxs-lookup"><span data-stu-id="c047a-136">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="c047a-137">En **centro de Partners** , seleccione **clientes**.</span><span class="sxs-lookup"><span data-stu-id="c047a-137">From **Partner Center** select **Customers**.</span></span>

3. <span data-ttu-id="c047a-138">Abre el nombre de la compañía del cliente que deseas migrar.</span><span class="sxs-lookup"><span data-stu-id="c047a-138">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="c047a-139">Seleccione **Agregar suscripción**.</span><span class="sxs-lookup"><span data-stu-id="c047a-139">Select **Add subscription**.</span></span>

5. <span data-ttu-id="c047a-140">Agregue las suscripciones y los recuentos de licencias correctos del catálogo.</span><span class="sxs-lookup"><span data-stu-id="c047a-140">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="c047a-141">Verifica los datos con la información proporcionada en las cuentas de partner de **Transición desde**.</span><span class="sxs-lookup"><span data-stu-id="c047a-141">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="lista de clientes":::

6. <span data-ttu-id="c047a-143">Haga clic en **enviar.**</span><span class="sxs-lookup"><span data-stu-id="c047a-143">Click **Submit.**</span></span>

   <span data-ttu-id="c047a-144">Ahora los servicios se proporcionan al cliente desde la cuenta de partner de **Transición a**.</span><span class="sxs-lookup"><span data-stu-id="c047a-144">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="c047a-145">Repite estos pasos para migrar las suscripciones de todos los demás clientes.</span><span class="sxs-lookup"><span data-stu-id="c047a-145">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="c047a-146">Antes de pasar a la siguiente sección, asegúrate de todas las suscripciones de cliente existente en las cuentas de partner de **Transición desde** se vuelven a aprovisionar en la cuenta de partner de **Transición a**.</span><span class="sxs-lookup"><span data-stu-id="c047a-146">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="c047a-147">Los asociados deben suspender las suscripciones en la **transición de** la cuenta de inquilino de asociado del centro de Partners el mismo día en que se realiza la transición de esas suscripciones y se configuran en la cuenta de la **transición a** la cuenta de inquilino del asociado en el centro de partners para asegurarse de que no se produce la facturación doble.</span><span class="sxs-lookup"><span data-stu-id="c047a-147">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="c047a-148">Se denegarán los créditos de las solicitudes de soporte técnico debido a cualquier superposición en la facturación que se produzca cuando no se deshabilite correctamente la **transición de** las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="c047a-148">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="c047a-149">Deshabilitar las suscripciones de Office 365 en la cuenta de partner de Transición desde</span><span class="sxs-lookup"><span data-stu-id="c047a-149">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="c047a-150">Deshabilitar la suscripción de CSP de las cuentas de partner de **Transición desde** detiene toda facturación futura.</span><span class="sxs-lookup"><span data-stu-id="c047a-150">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="c047a-151">No tiene que deshabilitar manualmente las suscripciones de Azure, ya que las suscripciones de Azure se deshabilitan automáticamente durante el proceso de migración.</span><span class="sxs-lookup"><span data-stu-id="c047a-151">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="c047a-152">Inicie sesión en el **centro de Partners** con la **transición de** la cuenta de CSP y navegue hasta la lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="c047a-152">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="c047a-153">Abre al cliente cuyas suscripciones quieras deshabilitar y, a continuación, selecciona la primera oferta que deshabilitar.</span><span class="sxs-lookup"><span data-stu-id="c047a-153">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="c047a-154">Establece la suscripción en **suspendida**y, a continuación, haz clic en **enviar**.</span><span class="sxs-lookup"><span data-stu-id="c047a-154">Set the subscription to **suspended**, and then click **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="c047a-155">Suspender la suscripción garantiza que no se produzca la facturación.</span><span class="sxs-lookup"><span data-stu-id="c047a-155">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="c047a-156">La suscripción muestra **Suspended** en la lista de suscripciones.</span><span class="sxs-lookup"><span data-stu-id="c047a-156">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="c047a-157">Repite estos pasos para todas las suscripciones del cliente.</span><span class="sxs-lookup"><span data-stu-id="c047a-157">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="c047a-158">Comprueba que todas muestran **suspendida.**</span><span class="sxs-lookup"><span data-stu-id="c047a-158">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="c047a-159">Selecciona al siguiente cliente de la lista y repite el proceso de deshabilitar todas las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="c047a-159">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="c047a-160">Migración de suscripciones basadas en uso de Azure</span><span class="sxs-lookup"><span data-stu-id="c047a-160">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="c047a-161">A diferencia de las suscripciones de CSP de Office 365, no es necesario migrar manualmente las suscripciones de CSP basadas en el uso de Azure.</span><span class="sxs-lookup"><span data-stu-id="c047a-161">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="c047a-162">Microsoft Azure soporte técnico migrará las suscripciones de Azure, así como todos los servicios o recursos implementados desde la **transición de** las cuentas de revendedores de CSP **a la cuenta** de revendedor de CSP.</span><span class="sxs-lookup"><span data-stu-id="c047a-162">Microsoft Azure Support will migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="c047a-163">Durante esta transición, el cliente no experimentará ninguna interrupción del servicio.</span><span class="sxs-lookup"><span data-stu-id="c047a-163">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="c047a-164">Asegúrese de que las cuentas de cliente que tendrán las suscripciones de Azure migradas han aceptado el contrato que se va a asociar a la nueva cuenta **de transición a** CSP.</span><span class="sxs-lookup"><span data-stu-id="c047a-164">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="c047a-165">Notificará a Microsoft las cuentas de cliente que están preparadas para la migración y proporcionará los nombres de las compañías de los clientes.</span><span class="sxs-lookup"><span data-stu-id="c047a-165">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="c047a-166">Microsoft migra las suscripciones basadas en el uso de Azure y le notifica cuando se completa la migración.</span><span class="sxs-lookup"><span data-stu-id="c047a-166">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="c047a-167">Debe confirmar que la suscripción de Azure en la que se realiza la **transición de** la cuenta de revendedor de CSP ahora está marcada como **suspendida** en el centro de Partners en la sección suscripciones de clientes.</span><span class="sxs-lookup"><span data-stu-id="c047a-167">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="c047a-168">Confirme que la suscripción de Azure en la cuenta de **transición a** revendedor de CSP muestra ahora el estado **activo** en el centro de Partners en la sección suscripciones de clientes.</span><span class="sxs-lookup"><span data-stu-id="c047a-168">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="c047a-169">Deshabilitar las suscripciones en el cliente no cambia la apariencia del cliente en la lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="c047a-169">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="c047a-170">Actualmente no hay ninguna opción para quitar clientes de la lista.</span><span class="sxs-lookup"><span data-stu-id="c047a-170">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="c047a-171">Los partners deben evitar volver a agregar suscripciones a estos clientes en el futuro desde su cuenta de **Transición desde**.</span><span class="sxs-lookup"><span data-stu-id="c047a-171">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="c047a-172">Repite estos pasos para todas las suscripciones de todos tus clientes para detener futuros cargos en las cuentas **Transición desde**.</span><span class="sxs-lookup"><span data-stu-id="c047a-172">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="c047a-173">El partner recibirá una factura final con un crédito por el número de días sin usar entre el día de la cancelación y el último día del período de facturación.</span><span class="sxs-lookup"><span data-stu-id="c047a-173">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="c047a-174">Tras ese período de facturación final, no se generarán más futuras.</span><span class="sxs-lookup"><span data-stu-id="c047a-174">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="c047a-175">Información adicional</span><span class="sxs-lookup"><span data-stu-id="c047a-175">Additional information</span></span>

- <span data-ttu-id="c047a-176">Deshabilitar la suscripción de la cuenta de la **transición de** CSP no afecta al servicio del cliente final, siempre que el servicio se haya aprovisionado desde la cuenta de **transición a** CSP antes de deshabilitar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="c047a-176">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="c047a-177">El cliente no puede usar las suscripciones y no genera cargos cuando se suspende o cancela.</span><span class="sxs-lookup"><span data-stu-id="c047a-177">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="c047a-178">Actualmente no hay ninguna manera de quitar un cliente completamente de la lista de **clientes** .</span><span class="sxs-lookup"><span data-stu-id="c047a-178">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="c047a-179">Los asociados deben suspender las suscripciones en la **transición de** la cuenta de inquilino del asociado en el centro de Partners el mismo día en que se realiza la transición de las suscripciones y se configuran en la cuenta de **transición** para asegurarse de que no se produce la facturación doble.</span><span class="sxs-lookup"><span data-stu-id="c047a-179">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="c047a-180">Microsoft no admitirá solicitudes de créditos debido a cualquier superposición en la facturación que se produce cuando no se establece correctamente la **transición de** las suscripciones a suspendidas.</span><span class="sxs-lookup"><span data-stu-id="c047a-180">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="c047a-181">Simplificación de la migración mediante la exportación</span><span class="sxs-lookup"><span data-stu-id="c047a-181">Simplify migration using Export</span></span>

<span data-ttu-id="c047a-182">Si usas la **Función de exportación**, puedes capturar las suscripciones que necesites usar en tu nueva estructura consolidada:</span><span class="sxs-lookup"><span data-stu-id="c047a-182">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="c047a-183">Haga clic en **clientes** en el centro de partners para ver la lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="c047a-183">Click **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="c047a-184">Abre el nombre del cliente deseado.</span><span class="sxs-lookup"><span data-stu-id="c047a-184">Open the desired customer name.</span></span>

3. <span data-ttu-id="c047a-185">En la página **Suscripciones**, haz clic en **Exportar suscripciones** para exportar los detalles de las suscripciones a un archivo de Excel.</span><span class="sxs-lookup"><span data-stu-id="c047a-185">On the **Subscriptions** page, click **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="c047a-186">Usa esta lista para volver a crear las suscripciones en el nuevo inquilino consolidado.</span><span class="sxs-lookup"><span data-stu-id="c047a-186">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="c047a-187">Registro de API</span><span class="sxs-lookup"><span data-stu-id="c047a-187">API registration</span></span>

<span data-ttu-id="c047a-188">Para obtener más información sobre el registro de API, consulte [configuración del acceso de API en el centro de Partners](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="c047a-188">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="c047a-189">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="c047a-189">Next steps</span></span>

- [<span data-ttu-id="c047a-190">Configuración y administración de las cuentas de clientes para partners revendedores en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="c047a-190">Customer account setup and management for reseller partners in Partner Center</span></span>](customer-accounts.md)