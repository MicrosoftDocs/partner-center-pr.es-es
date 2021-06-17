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
ms.openlocfilehash: 84e5f7f2674e9b2f3c3c26ed2ea49f9bba0e96e0
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276882"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a><span data-ttu-id="7ea66-104">Instrucciones para la consolidación de los inquilinos de autorización regional de CSP</span><span class="sxs-lookup"><span data-stu-id="7ea66-104">Instructions for CSP regional authorization tenant consolidation</span></span>

<span data-ttu-id="7ea66-105">**Se aplica a**: Centro de partners | Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="7ea66-105">**Applies to**: Partner Center | Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="7ea66-106">**Roles adecuados**: Administrador global | Agente de administración</span><span class="sxs-lookup"><span data-stu-id="7ea66-106">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="7ea66-107">\[Parte de la información está relacionada con el producto publicado previamente que se puede modificar considerablemente antes de su lanzamiento comercial.</span><span class="sxs-lookup"><span data-stu-id="7ea66-107">\[Some information relates to pre-released product which may be substantially modified before it's commercially released.</span></span> <span data-ttu-id="7ea66-108">Microsoft no otorga ninguna garantía, explícita o implícita, con respecto a la información proporcionada aquí.\]</span><span class="sxs-lookup"><span data-stu-id="7ea66-108">Microsoft makes no warranties, express or implied, with respect to the information provided here.\]</span></span>

<span data-ttu-id="7ea66-109">Puede consolidar los inquilinos para su negocio.</span><span class="sxs-lookup"><span data-stu-id="7ea66-109">You can consolidate tenants for your business.</span></span> <span data-ttu-id="7ea66-110">Usa estas instrucciones para consolidar los inquilinos para diferentes países o regiones.</span><span class="sxs-lookup"><span data-stu-id="7ea66-110">Use these instructions to consolidate tenants for different country/regions.</span></span>

>[!NOTE]  
><span data-ttu-id="7ea66-111">Debe tener en cuenta todos los recuentos de suscripciones y licencias aprovisionadas para cada uno de los clientes de la cuenta desde la que va a realizar la transición.</span><span class="sxs-lookup"><span data-stu-id="7ea66-111">You must be aware of all of the provisioned subscriptions and license counts for each of your customers in the account you are transitioning from.</span></span> <span data-ttu-id="7ea66-112">Volverá a aprovisionar esas mismas suscripciones exactas con los mismos recuentos de licencias en la nueva cuenta central de CSP como parte del proceso de migración.</span><span class="sxs-lookup"><span data-stu-id="7ea66-112">You will be re-provisioning those same exact subscriptions with the same license counts under the new central CSP account as part of the migration process.</span></span> <span data-ttu-id="7ea66-113">Usa la característica de lista de exportación para ayudar a crear una lista de clientes que trasladar al inquilino centralizado.</span><span class="sxs-lookup"><span data-stu-id="7ea66-113">Use the export list feature to help create a list of customers to move over to the centralized tenant.</span></span>  <span data-ttu-id="7ea66-114">Una vez completada la consolidación, no se puede revertir al estado de inquilino anterior.</span><span class="sxs-lookup"><span data-stu-id="7ea66-114">Once consolidation is complete, you can't revert to the previous tenant state.</span></span> <span data-ttu-id="7ea66-115">También puede ser necesaria una acción del cliente.</span><span class="sxs-lookup"><span data-stu-id="7ea66-115">Customer action may also be required.</span></span>

## <a name="prepare-for-migration"></a><span data-ttu-id="7ea66-116">Preparación para la migración</span><span class="sxs-lookup"><span data-stu-id="7ea66-116">Prepare for migration</span></span>

- <span data-ttu-id="7ea66-117">Inicie sesión en **Centro de partners** con  la cuenta de transición (la que va a realizar la transición a la nueva cuenta) y revise todos los clientes y todos los servicios aprovisionados para esos clientes.</span><span class="sxs-lookup"><span data-stu-id="7ea66-117">Sign in to **Partner Center**  using the **Transitioning** account (the one you will transition to the new account), and review of all customers and all of the services provisioned for those customers.</span></span>

- <span data-ttu-id="7ea66-118">Cerrar sesión en esta cuenta.</span><span class="sxs-lookup"><span data-stu-id="7ea66-118">Sign out of this account.</span></span>

## <a name="migrate-customer-accounts"></a><span data-ttu-id="7ea66-119">Migración de las cuentas de cliente</span><span class="sxs-lookup"><span data-stu-id="7ea66-119">Migrate customer accounts</span></span>

1. <span data-ttu-id="7ea66-120">Inicie sesión **en Centro de partners**  con la cuenta **de** transición (nueva) (a la que va a realizar la transición de los clientes).</span><span class="sxs-lookup"><span data-stu-id="7ea66-120">Sign in to **Partner Center**  with the **Transitioning** (new) account (the one you are transitioning customers into).</span></span>

2. <span data-ttu-id="7ea66-121">Seleccione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="7ea66-121">Select **Customers**.</span></span>

3. <span data-ttu-id="7ea66-122">Seleccione **Solicitar una relación de revendedor.**</span><span class="sxs-lookup"><span data-stu-id="7ea66-122">Select **Request a reseller relationship**.</span></span> <span data-ttu-id="7ea66-123">Aparece un mensaje de correo electrónico predeterminado para enviarlo a los clientes.</span><span class="sxs-lookup"><span data-stu-id="7ea66-123">You are presented with a default email message to send to your customers.</span></span> <span data-ttu-id="7ea66-124">Este mensaje contiene una dirección URL con el identificador de organización exclusivo para tu nueva cuenta del centro de partners.</span><span class="sxs-lookup"><span data-stu-id="7ea66-124">This message contains a URL with the org ID unique to your new Partner Center account.</span></span>

4. <span data-ttu-id="7ea66-125">**Acción de cliente:** Asegúrate de que todos los clientes activos que deseas migrar visitan esta dirección URL.</span><span class="sxs-lookup"><span data-stu-id="7ea66-125">**Customer Action:** Ensure that each of the active customers you want to migrate visits this URL.</span></span> <span data-ttu-id="7ea66-126">Al abrir la dirección URL, al cliente se le pedirá que inicie sesión en el portal de Office 365.</span><span class="sxs-lookup"><span data-stu-id="7ea66-126">When opening the URL, the customer is prompted to sign in to the Office 365 portal.</span></span> <span data-ttu-id="7ea66-127">El cliente iniciará sesión usando el mismo identificador de organización que utilice para acceder a los portales de administración de Azure y de Office 365.</span><span class="sxs-lookup"><span data-stu-id="7ea66-127">The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.</span></span>

5. <span data-ttu-id="7ea66-128">Después de iniciar sesión,  se solicita al administrador global de la cuenta de cliente que envíe un contrato que concede privilegios de administrador delegado a la nueva cuenta de CSP.</span><span class="sxs-lookup"><span data-stu-id="7ea66-128">After signing in, the Global Admin for the **customer account** is prompted to submit an agreement that gives delegated admin privileges to the new CSP account.</span></span> <span data-ttu-id="7ea66-129">Si acepta, el cliente seleccionará la casilla y autorizará la relación.</span><span class="sxs-lookup"><span data-stu-id="7ea66-129">If they agree, the customer selects the checkbox and agrees to authorize the relationship.</span></span>

<span data-ttu-id="7ea66-130">Los clientes aparecerán en la lista de clientes del asociado después de haber enviado el contrato, uno a uno.</span><span class="sxs-lookup"><span data-stu-id="7ea66-130">The customers will appear in the partner's customer list after they have submitted the agreement, one by one.</span></span>

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a><span data-ttu-id="7ea66-131">Migración de suscripciones basadas en uso de Office 365 y que no sean de Azure</span><span class="sxs-lookup"><span data-stu-id="7ea66-131">Migrating Office 365 and non-Azure usage-based subscriptions</span></span>

1. <span data-ttu-id="7ea66-132">Cuando el cliente haya firmado el contrato, puedes volver a crear sus suscripciones en tu inquilino de partner centralizado.</span><span class="sxs-lookup"><span data-stu-id="7ea66-132">Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.</span></span>

2. <span data-ttu-id="7ea66-133">En **Centro de partners**, seleccione **Clientes.**</span><span class="sxs-lookup"><span data-stu-id="7ea66-133">From **Partner Center**, select **Customers**.</span></span>

3. <span data-ttu-id="7ea66-134">Abre el nombre de la compañía del cliente que deseas migrar.</span><span class="sxs-lookup"><span data-stu-id="7ea66-134">Open the company name for the customer you want to migrate.</span></span>

4. <span data-ttu-id="7ea66-135">Seleccione **Agregar suscripción**.</span><span class="sxs-lookup"><span data-stu-id="7ea66-135">Select **Add subscription**.</span></span>

5. <span data-ttu-id="7ea66-136">Agregue las suscripciones y los recuentos de licencias correctos del catálogo.</span><span class="sxs-lookup"><span data-stu-id="7ea66-136">Add the correct subscriptions and license counts from the catalog.</span></span> <span data-ttu-id="7ea66-137">Verifica los datos con la información proporcionada en las cuentas de partner de **Transición desde**.</span><span class="sxs-lookup"><span data-stu-id="7ea66-137">Verify with the information provided in the **Transitioning From** partner accounts.</span></span>

   :::image type="content" source="images/regionalcustomer2.png" alt-text="lista de clientes.":::

6. <span data-ttu-id="7ea66-139">Seleccione **Enviar.**</span><span class="sxs-lookup"><span data-stu-id="7ea66-139">Select **Submit.**</span></span>

   <span data-ttu-id="7ea66-140">Ahora los servicios se proporcionan al cliente desde la cuenta de partner de **Transición a**.</span><span class="sxs-lookup"><span data-stu-id="7ea66-140">The services are now provided to the customer from the **Transitioning To** partner account.</span></span>

7. <span data-ttu-id="7ea66-141">Repite estos pasos para migrar las suscripciones de todos los demás clientes.</span><span class="sxs-lookup"><span data-stu-id="7ea66-141">Repeat these steps to migrate subscriptions for all additional customers.</span></span>

<span data-ttu-id="7ea66-142">Antes de pasar a la siguiente sección, asegúrate de todas las suscripciones de cliente existente en las cuentas de partner de **Transición desde** se vuelven a aprovisionar en la cuenta de partner de **Transición a**.</span><span class="sxs-lookup"><span data-stu-id="7ea66-142">Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.</span></span>

> [!NOTE]
> <span data-ttu-id="7ea66-143">Los asociados deben  suspender las suscripciones de la cuenta Transición desde el inquilino del asociado  en Centro de partners el mismo día en que esas suscripciones se han pasado y configurado en la cuenta Transición al inquilino del asociado del Centro de partners para asegurarse de que no se produce la doble facturación.</span><span class="sxs-lookup"><span data-stu-id="7ea66-143">Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur.</span></span> <span data-ttu-id="7ea66-144">Se denegarán las solicitudes de soporte técnico para los créditos debido a cualquier superposición en la facturación que se produzca al no deshabilitar correctamente las suscripciones **De** transición.</span><span class="sxs-lookup"><span data-stu-id="7ea66-144">Support requests will be denied for credits due to any overlap in billing that occurs from not correctly disabling the **Transitioning From** subscriptions.</span></span>

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a><span data-ttu-id="7ea66-145">Deshabilitar las suscripciones de Office 365 en la cuenta de partner de Transición desde</span><span class="sxs-lookup"><span data-stu-id="7ea66-145">Disabling the Office 365 subscriptions under the Transitioning From partner account</span></span>

<span data-ttu-id="7ea66-146">Deshabilitar la suscripción de CSP de las cuentas de partner de **Transición desde** detiene toda facturación futura.</span><span class="sxs-lookup"><span data-stu-id="7ea66-146">Disabling the CSP subscription under the **Transitioning From** partner accounts stops any future billing.</span></span> <span data-ttu-id="7ea66-147">No tiene que deshabilitar manualmente las suscripciones de Azure, ya que las suscripciones de Azure se deshabilitan automáticamente durante el proceso de migración.</span><span class="sxs-lookup"><span data-stu-id="7ea66-147">You don't have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.</span></span>

1. <span data-ttu-id="7ea66-148">Inicie sesión en el **Centro de partners** con la **cuenta Transitioning From** CSP (Transición desde CSP) y vaya a la lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="7ea66-148">Sign in to the **Partner Center** with the **Transitioning From** CSP account and navigate to the customer list.</span></span>

2. <span data-ttu-id="7ea66-149">Abre al cliente cuyas suscripciones quieras deshabilitar y, a continuación, selecciona la primera oferta que deshabilitar.</span><span class="sxs-lookup"><span data-stu-id="7ea66-149">Open the customer with subscriptions to disable, and then select the first offer to disable.</span></span>

3. <span data-ttu-id="7ea66-150">Establezca la suscripción en **suspendida y,** a continuación, **seleccione Enviar**.</span><span class="sxs-lookup"><span data-stu-id="7ea66-150">Set the subscription to **suspended**, and then select **submit**.</span></span>

   >[!Note]
   ><span data-ttu-id="7ea66-151">La suspensión de la suscripción garantiza que no se produzca la doble facturación.</span><span class="sxs-lookup"><span data-stu-id="7ea66-151">Suspending the subscription ensures double billing does not occur.</span></span>

   <span data-ttu-id="7ea66-152">La suscripción se **muestra suspendida en** la lista de suscripciones.</span><span class="sxs-lookup"><span data-stu-id="7ea66-152">The subscription shows **suspended** on the subscriptions list.</span></span>

4. <span data-ttu-id="7ea66-153">Repite estos pasos para todas las suscripciones del cliente.</span><span class="sxs-lookup"><span data-stu-id="7ea66-153">Repeat these steps for all subscriptions under the customer.</span></span> <span data-ttu-id="7ea66-154">Comprueba que todas muestran **suspendida.**</span><span class="sxs-lookup"><span data-stu-id="7ea66-154">Verify all show **suspended.**</span></span>

5. <span data-ttu-id="7ea66-155">Selecciona al siguiente cliente de la lista y repite el proceso de deshabilitar todas las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="7ea66-155">Select the next customer on the list and repeat the process of disabling all subscriptions.</span></span>

## <a name="migrating-azure-usage-based-subscriptions"></a><span data-ttu-id="7ea66-156">Migración de suscripciones basadas en uso de Azure</span><span class="sxs-lookup"><span data-stu-id="7ea66-156">Migrating Azure usage-based subscriptions</span></span>

<span data-ttu-id="7ea66-157">A diferencia de las suscripciones de CSP de Office 365, no es necesario migrar manualmente las suscripciones de CSP basadas en el uso de Azure.</span><span class="sxs-lookup"><span data-stu-id="7ea66-157">Unlike the Office 365 CSP subscriptions, Azure, usage-based CSP subscriptions do not need to be migrated manually.</span></span> <span data-ttu-id="7ea66-158">Microsoft Azure soporte técnico migrará las suscripciones de Azure y todos los servicios o recursos implementados desde la transición de las cuentas de revendedor de **CSP** a la cuenta de revendedor de **Transición** a CSP.</span><span class="sxs-lookup"><span data-stu-id="7ea66-158">Microsoft Azure Support will migrate the Azure subscriptions and all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account.</span></span> <span data-ttu-id="7ea66-159">Durante esta transición, el cliente no experimentará ninguna interrupción del servicio.</span><span class="sxs-lookup"><span data-stu-id="7ea66-159">There will be no disruption of service to the customer during this transition.</span></span>

1. <span data-ttu-id="7ea66-160">Asegúrese de que las cuentas de cliente que tendrán suscripciones de Azure migradas hayan aceptado el contrato para asociarse a la nueva cuenta de CSP **de** transición a .</span><span class="sxs-lookup"><span data-stu-id="7ea66-160">Ensure that the customer accounts that will have Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.</span></span>

2. <span data-ttu-id="7ea66-161">Notificará a Microsoft qué cuentas de cliente están listas para migrar y proporcionará los nombres de la empresa de esos clientes.</span><span class="sxs-lookup"><span data-stu-id="7ea66-161">You will notify Microsoft of which customer accounts are ready to migrate, and provide those customer's company names.</span></span>

3. <span data-ttu-id="7ea66-162">Microsoft migra las suscripciones basadas en el uso de Azure y le notifica cuando se completa la migración.</span><span class="sxs-lookup"><span data-stu-id="7ea66-162">Microsoft migrates the Azure usage-based subscriptions and notifies you when the migration is complete.</span></span>

4. <span data-ttu-id="7ea66-163">Debe confirmar que la suscripción de Azure en la cuenta  de revendedor de **Transición** desde CSP ahora está marcada como suspendida en Centro de partners en la sección suscripciones del cliente.</span><span class="sxs-lookup"><span data-stu-id="7ea66-163">You need to confirm that the Azure subscription under the **Transitioning From** CSP reseller account now is marked **suspended** in Partner Center under the customer subscriptions section.</span></span>

5. <span data-ttu-id="7ea66-164">Confirme que la suscripción de Azure en la cuenta  de revendedor de **Transición** a CSP ahora muestra el estado activo en Centro de partners en la sección suscripciones de cliente.</span><span class="sxs-lookup"><span data-stu-id="7ea66-164">Confirm that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in Partner Center under the customer subscriptions section.</span></span>

   >[!Note]
   > <span data-ttu-id="7ea66-165">Deshabilitar las suscripciones en el cliente no cambia la apariencia del cliente en la lista Clientes.</span><span class="sxs-lookup"><span data-stu-id="7ea66-165">Disabling the subscriptions under the customer does not change the appearance of the customer in the Customers list.</span></span> <span data-ttu-id="7ea66-166">Actualmente no hay ninguna opción para quitar clientes de la lista.</span><span class="sxs-lookup"><span data-stu-id="7ea66-166">There is currently no option to remove customers from the list.</span></span> <span data-ttu-id="7ea66-167">Los partners deben evitar volver a agregar suscripciones a estos clientes en el futuro desde su cuenta de **Transición desde**.</span><span class="sxs-lookup"><span data-stu-id="7ea66-167">Partners should avoid adding subscriptions back to these customers from their **Transitioning From** account in the future.</span></span>

6. <span data-ttu-id="7ea66-168">Repite estos pasos para todas las suscripciones de todos tus clientes para detener futuros cargos en las cuentas **Transición desde**.</span><span class="sxs-lookup"><span data-stu-id="7ea66-168">Repeat these steps for all subscriptions under all of your customers to stop future charges on the **Transitioning From** account(s).</span></span> <span data-ttu-id="7ea66-169">El partner recibirá una factura final con un crédito por el número de días sin usar entre el día de la cancelación y el último día del período de facturación.</span><span class="sxs-lookup"><span data-stu-id="7ea66-169">The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period.</span></span> <span data-ttu-id="7ea66-170">Tras ese período de facturación final, no se generarán más futuras.</span><span class="sxs-lookup"><span data-stu-id="7ea66-170">No future invoices will generate after that final billing period.</span></span>

### <a name="additional-information"></a><span data-ttu-id="7ea66-171">Información adicional</span><span class="sxs-lookup"><span data-stu-id="7ea66-171">Additional information</span></span>

- <span data-ttu-id="7ea66-172">Deshabilitar la suscripción de la cuenta de **CSP** de transición desde no afecta al servicio del cliente final, siempre y cuando el servicio se aprovisionó desde la cuenta de **CSP** de transición a antes de deshabilitar la suscripción.</span><span class="sxs-lookup"><span data-stu-id="7ea66-172">Disabling the subscription from the **Transitioning From** CSP account does not impact end customer's service as long as the service was provisioned from the **Transitioning To** CSP account prior to disabling the subscription.</span></span>

- <span data-ttu-id="7ea66-173">El cliente no puede usar las suscripciones y no generan cargos cuando se suspenden o cancelan.</span><span class="sxs-lookup"><span data-stu-id="7ea66-173">Subscriptions cannot be used by the customer and do not generate charges when suspended or canceled.</span></span>

- <span data-ttu-id="7ea66-174">Actualmente no hay ninguna manera de quitar un cliente por completo de la **lista** De clientes.</span><span class="sxs-lookup"><span data-stu-id="7ea66-174">There is currently no way to remove a customer completely from the **Customers** list.</span></span>
- 
    >[!Note]
    > <span data-ttu-id="7ea66-175">Los asociados deben  suspender las suscripciones en la cuenta de inquilino de transición desde el  asociado en Centro de partners el mismo día en que esas suscripciones se transiciónn a la cuenta de transición a y configurarse en ella para asegurarse de que no se produce la doble facturación.</span><span class="sxs-lookup"><span data-stu-id="7ea66-175">Partners must suspend subscriptions on the **Transitioning From** partner tenant account in Partner Center the same day those subscriptions are transitioned to and set up under the **Transitioning To** account to ensure double billing does not occur.</span></span> <span data-ttu-id="7ea66-176">Microsoft no admitirá solicitudes de crédito debido a cualquier superposición en  la facturación que se produzca al no establecer correctamente la transición de suscripciones a suspendidas.</span><span class="sxs-lookup"><span data-stu-id="7ea66-176">Microsoft will not support requests for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to suspended.</span></span>

### <a name="simplify-migration-using-export"></a><span data-ttu-id="7ea66-177">Simplificación de la migración mediante la exportación</span><span class="sxs-lookup"><span data-stu-id="7ea66-177">Simplify migration using Export</span></span>

<span data-ttu-id="7ea66-178">Si usas la **Función de exportación**, puedes capturar las suscripciones que necesites usar en tu nueva estructura consolidada:</span><span class="sxs-lookup"><span data-stu-id="7ea66-178">Using the **Export Function**, you can capture the subscriptions you need to use in your new consolidated structure:</span></span>

1. <span data-ttu-id="7ea66-179">Seleccione **Clientes** en Centro de partners para ver la lista de clientes.</span><span class="sxs-lookup"><span data-stu-id="7ea66-179">Select **Customers** on Partner Center to see the list of customers.</span></span> 

2. <span data-ttu-id="7ea66-180">Abre el nombre del cliente deseado.</span><span class="sxs-lookup"><span data-stu-id="7ea66-180">Open the desired customer name.</span></span>

3. <span data-ttu-id="7ea66-181">En la **página Suscripciones,** seleccione **Exportar suscripciones para** exportar los detalles de las suscripciones a un archivo de Excel.</span><span class="sxs-lookup"><span data-stu-id="7ea66-181">On the **Subscriptions** page, select **Export Subscriptions** to export details of subscriptions to an Excel file.</span></span>

4. <span data-ttu-id="7ea66-182">Usa esta lista para volver a crear las suscripciones en el nuevo inquilino consolidado.</span><span class="sxs-lookup"><span data-stu-id="7ea66-182">Use this list to recreate the subscriptions in your new consolidated tenant.</span></span>

### <a name="api-registration"></a><span data-ttu-id="7ea66-183">Registro de API</span><span class="sxs-lookup"><span data-stu-id="7ea66-183">API registration</span></span>

<span data-ttu-id="7ea66-184">Para obtener más información sobre el registro de API, consulte [Configuración del acceso de API en Centro de partners](/partner-center/develop/set-up-api-access-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="7ea66-184">For more information about API registration, see [Set up API access in Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).</span></span>

## <a name="next-steps"></a><span data-ttu-id="7ea66-185">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="7ea66-185">Next steps</span></span>

- [<span data-ttu-id="7ea66-186">Proveedor de soluciones en la nube mercados regionales y monedas del programa en los que puede vender ofertas de CSP</span><span class="sxs-lookup"><span data-stu-id="7ea66-186">Cloud Solution Provider program regional markets and currencies where you can sell CSP offers</span></span>](regional-authorization-overview.md)
