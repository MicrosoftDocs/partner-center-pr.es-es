---
title: 'Facturación del plan de Azure: facturas y archivos de conciliación'
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprende a obtener acceso y a comprender la estructura del archivo de conciliación y facturación relacionado con la facturación del plan de Azure.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: e230cc0d8ff3afea4bf2cc7b55d3847814696af6
ms.sourcegitcommit: f99424919f0d77bbe4f44293d84f9ea1e3317f13
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/21/2021
ms.locfileid: "98658440"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="bc7c1-103">Nueva experiencia comercial en CSP: facturación de Azure</span><span class="sxs-lookup"><span data-stu-id="bc7c1-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="bc7c1-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="bc7c1-104">**Appropriate roles**</span></span>

- <span data-ttu-id="bc7c1-105">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="bc7c1-105">Admin agent</span></span>
- <span data-ttu-id="bc7c1-106">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="bc7c1-106">Billing admin</span></span>
- <span data-ttu-id="bc7c1-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="bc7c1-107">Global admin</span></span>

<span data-ttu-id="bc7c1-108">En este artículo se describe cómo acceder a la estructura del archivo de conciliación y facturación relacionado con la facturación del plan de Azure, así cómo comprenderla.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-108">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="bc7c1-109">La facturación del plan Azure es una experiencia de facturación simplificada que usa una fecha de facturación única alineada y un período de facturación basado en los meses del calendario.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-109">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="bc7c1-110">Resumen de los elementos esenciales de la facturación</span><span class="sxs-lookup"><span data-stu-id="bc7c1-110">Summary of billing essentials</span></span>

- <span data-ttu-id="bc7c1-111">**Fecha de facturación**: La factura y el archivo de conciliación estarán disponibles en el panel o API del Centro de partners antes del día 8 (medianoche, UTC).</span><span class="sxs-lookup"><span data-stu-id="bc7c1-111">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="bc7c1-112">**Período de facturación**: El período de facturación de la factura coincidirá con el mes natural; por ejemplo, 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-112">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="bc7c1-113">**Períodos del servicio de cargos**: Los cargos coincidirán con el mes natural.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-113">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="bc7c1-114">Por ejemplo, si el partner facturado agrega servicios de Azure a través de un plan de Azure el 15/10 y el cliente comienza a consumir los servicios de Azure el mismo 15/10, el partner facturado recibirá la factura o la conciliación el 8/11 referente al consumo del cliente durante el período de servicio del 15/10 al 31/10.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-114">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="bc7c1-115">La factura del próximo mes que se generará el 8/12 y contendrá todos los cargos del período de servicio del 1/11 al 11/31.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-115">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="bc7c1-116">**Plazo de pago de la factura**: Neto, 60 días.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-116">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="bc7c1-117">**Moneda de la factura** : Los partners seguirán siendo facturados en la moneda asignada del país del cliente.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-117">**Invoice currency**: Partners will continue to be billed in the customer's country's assigned currency.</span></span> <span data-ttu-id="bc7c1-118">Por ejemplo, si el partner facturado está en Irlanda y tiene clientes en el Reino Unido, Noruega y Alemania, entonces el partner facturado recibirá una factura o conciliación en GBP, NOK y EUR.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-118">For example, if the billed partner is in Ireland with customers in the UK, Norway, and Germany, then the billed partner will receive a GBP, NOK, and EUR invoice/recon.</span></span>

- <span data-ttu-id="bc7c1-119">**Incentivos de partners**: Pagado a 45 días desde el final del mes de la factura.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-119">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="bc7c1-120">Acceder a las facturas y los archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="bc7c1-120">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="bc7c1-121">El administrador global o el administrador de facturación de tu empresa recibirá un correo electrónico cuando una factura esté lista para ver.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-121">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="bc7c1-122">Para acceder a la factura y al archivo de conciliación:</span><span class="sxs-lookup"><span data-stu-id="bc7c1-122">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="bc7c1-123">Inicia sesión en el [panel](https://partner.microsoft.com/dashboard/) del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-123">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="bc7c1-124">En el menú del Centro de partners, selecciona **Billing** (Facturación).</span><span class="sxs-lookup"><span data-stu-id="bc7c1-124">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="bc7c1-125">Selecciona la pestaña de **Periódico** y **Una vez** y la moneda que te interese.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-125">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="facturación":::

4. <span data-ttu-id="bc7c1-127">Selecciona **Factura** o **Archivo de conciliación**.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-127">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="bc7c1-128">Para ver las facturas históricas y los archivos de conciliación, amplía la fila del historial de facturación a continuación.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-128">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="bc7c1-129">Explicación de los datos de uso</span><span class="sxs-lookup"><span data-stu-id="bc7c1-129">Understanding usage data</span></span> 

1. <span data-ttu-id="bc7c1-130">El plan de Azure es el contenedor raíz o de nivel superior para el uso.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-130">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="bc7c1-131">Todo el uso está vinculado a un único plan de Azure.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-131">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="bc7c1-132">En un plan, habrá una o varias suscripciones de Azure.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-132">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="bc7c1-133">Estos son los contenedores que se usan para la implementación y la administración de recursos.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-133">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="bc7c1-134">En una suscripción, los grupos de recursos se agregan a recursos de grupo.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-134">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="bc7c1-135">Cada recurso se implementa en un grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-135">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="bc7c1-136">Entre los ejemplos de recursos se incluyen las máquinas virtuales y las cuentas de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-136">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="bc7c1-137">Los recursos emiten medidores: Los medidores son medidas de consumo de un recurso, y un recurso puede emitir el uso de varios medidores.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-137">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="bc7c1-138">Los medidores se identifican mediante ProductId, SKUId y AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-138">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="bc7c1-139">Jerarquía de grupos de recursos de suscripción y medición</span><span class="sxs-lookup"><span data-stu-id="bc7c1-139">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="bc7c1-140">**Cuenta de Azure (inquilino)**</span><span class="sxs-lookup"><span data-stu-id="bc7c1-140">**Azure account (tenant)**</span></span>

- <span data-ttu-id="bc7c1-141">Suscripción A</span><span class="sxs-lookup"><span data-stu-id="bc7c1-141">Subscription A</span></span>
    - <span data-ttu-id="bc7c1-142">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="bc7c1-142">ResourceGroup 1</span></span>
        - <span data-ttu-id="bc7c1-143">Máquina virtual (recurso)</span><span class="sxs-lookup"><span data-stu-id="bc7c1-143">Virtual machine (resource)</span></span>
            - <span data-ttu-id="bc7c1-144">Medidor de proceso</span><span class="sxs-lookup"><span data-stu-id="bc7c1-144">Compute meter</span></span>
        - <span data-ttu-id="bc7c1-145">Virtual Network (recurso)</span><span class="sxs-lookup"><span data-stu-id="bc7c1-145">Virtual network (resource)</span></span>
            - <span data-ttu-id="bc7c1-146">Sin medidor de facturación</span><span class="sxs-lookup"><span data-stu-id="bc7c1-146">No billing meter</span></span>

    - <span data-ttu-id="bc7c1-147">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="bc7c1-147">ResourceGroup 2</span></span>
        - <span data-ttu-id="bc7c1-148">Máquina virtual (recurso)</span><span class="sxs-lookup"><span data-stu-id="bc7c1-148">Virtual machine (resource)</span></span>
            - <span data-ttu-id="bc7c1-149">Medidor de proceso</span><span class="sxs-lookup"><span data-stu-id="bc7c1-149">Computer meter</span></span>
        - <span data-ttu-id="bc7c1-150">Disco administrado SSD Premium (recurso)</span><span class="sxs-lookup"><span data-stu-id="bc7c1-150">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="bc7c1-151">Medidor de capacidad de almacenamiento</span><span class="sxs-lookup"><span data-stu-id="bc7c1-151">Storage capacity meter</span></span>
            - <span data-ttu-id="bc7c1-152">Medidor de operaciones de almacenamiento</span><span class="sxs-lookup"><span data-stu-id="bc7c1-152">Storage operations meter</span></span>

- <span data-ttu-id="bc7c1-153">Suscripción B   -ResourceGroup 1       - Azure SQL (recurso)           - Medidor de DTU       - VPN Gateway (recurso)           - Medidor de VPN Gateway</span><span class="sxs-lookup"><span data-stu-id="bc7c1-153">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="bc7c1-154">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="bc7c1-154">ResourceGroup 2</span></span>
        - <span data-ttu-id="bc7c1-155">Interfaz de Virtual Network (recurso)</span><span class="sxs-lookup"><span data-stu-id="bc7c1-155">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="bc7c1-156">Sin medidor de facturación</span><span class="sxs-lookup"><span data-stu-id="bc7c1-156">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="bc7c1-157">Leer la factura</span><span class="sxs-lookup"><span data-stu-id="bc7c1-157">Read the invoice</span></span>

1. <span data-ttu-id="bc7c1-158">La factura estará disponible el día ocho de cada mes a más tardar.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-158">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="bc7c1-159">Los partners tienen 60 días para remitir el pago.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-159">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="bc7c1-160">El período de facturación cubrirá un mes dado del calendario; por ejemplo del 1/10 al 31/10.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-160">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="bc7c1-161">Los cargos son netos en cuanto a los ajustes (el importe es el valor neto del "crédito obtenido del partner por los servicios administrados").</span><span class="sxs-lookup"><span data-stu-id="bc7c1-161">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="bc7c1-162">Revisa el archivo de conciliación de facturas y el archivo de uso con clasificación diaria para obtener los detalles adicionales de facturación.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-162">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="factura":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="bc7c1-164">Lectura del archivo de conciliación de facturas</span><span class="sxs-lookup"><span data-stu-id="bc7c1-164">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="bc7c1-165">Cada combinación de medidor y plan de Azure puede tener hasta dos líneas de facturación en el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-165">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="bc7c1-166">Si el medidor puede tener en cuenta cualquier tipo de descuento o crédito (como los descuentos por nivel o el crédito obtenido del partner por los servicios administrados) durante todo el mes natural, el archivo de conciliación solo contendrá una línea de facturación.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-166">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="bc7c1-167">La columna **PriceAdjusmentDescription** hará referencia al descuento o al crédito obtenido.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-167">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="bc7c1-168">Si no existen recursos para un medidor concreto que es apto para el descuento o el crédito obtenido del partner, el archivo de conciliación solo contendrá una línea de facturación y el precio por unidad vigente será el precio de venta al por menor (que es el precio por unidad).</span><span class="sxs-lookup"><span data-stu-id="bc7c1-168">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="bc7c1-169">Si el medidor (o cualquier recurso que este emita) es apto para el **crédito obtenido del partner para los servicios administrados** durante una parte del mes, el archivo de conciliación contendrá dos líneas de facturación.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-169">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="bc7c1-170">Una línea representará los días que el medidor haya calificado y la segunda línea representará los días que el medidor no calificó.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-170">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="bc7c1-171">Leer el archivo de uso diario</span><span class="sxs-lookup"><span data-stu-id="bc7c1-171">Read the daily usage file</span></span>

- <span data-ttu-id="bc7c1-172">Los medidores de suscripción en un plan de Azure se clasifican y se acumulan diariamente.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-172">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="bc7c1-173">**El crédito obtenido del partner por los servicios administrados**  se determina y se aplica diariamente.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-173">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="bc7c1-174">Cada medidor de suscripciones tendrá una fila por cada día del mes en el que se haya consumido.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-174">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="bc7c1-175">Consulta el ejemplo que aparece a continuación:</span><span class="sxs-lookup"><span data-stu-id="bc7c1-175">In the example below:</span></span>

  - <span data-ttu-id="bc7c1-176">El medidor es apto para el **crédito obtenido del partner por los servicios administrados** del 1/7 al 3/7 (ten en cuenta que el precio unitario efectivo es el precio del minorista menos el crédito obtenido del partner).</span><span class="sxs-lookup"><span data-stu-id="bc7c1-176">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="bc7c1-177">El medidor no es apto para el **crédito obtenido del partner por los servicios administrados** del 4/7 al 7/7 (ten en cuenta que el precio unitario efectivo es el precio del minorista).</span><span class="sxs-lookup"><span data-stu-id="bc7c1-177">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="bc7c1-178">El medidor es apto para el **crédito obtenido del partner por los servicios administrados** del 8/7 al 31/7 (ten en cuenta que el precio unitario efectivo es el precio del minorista menos el crédito obtenido del partner).</span><span class="sxs-lookup"><span data-stu-id="bc7c1-178">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="bc7c1-180">Factura en la moneda del cliente</span><span class="sxs-lookup"><span data-stu-id="bc7c1-180">Invoice in customer currency</span></span>

<span data-ttu-id="bc7c1-181">Los servicios de Azure a través de un plan de Azure tendrán un precio de USD y se facturarán en la moneda asignada en el país del cliente.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-181">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="bc7c1-182">Si la moneda de facturación no es USD, el tipo de cambio usado se mostrará en la última página de la factura.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-182">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="bc7c1-183">Los tipos de cambio se determinan mensualmente y se aplican a la factura siguiente.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-183">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="bc7c1-184">Para obtener una lista completa de las monedas de los países, consulta la [matriz de moneda del cliente y la disponibilidad de los países en cuanto a las nuevas ofertas comerciales](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="bc7c1-184">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="bc7c1-185">Microsoft realiza la conversión de acuerdo con la Bolsa de Londres.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-185">Microsoft follows the London Stock Exchange for conversion.</span></span> <span data-ttu-id="bc7c1-186">El tipo de cambio usado equivale al tipo de cambio capturado el último segundo del último día laborable del mes en la Bolsa de Londres.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-186">We use the exchange rate, which is equal to the exchange rate captured on the last second of the last business day of the month on the London Stock Exchange.</span></span> <span data-ttu-id="bc7c1-187">Los tipos de cambio se actualizarán y estarán disponible el día anterior al primer día del mes para el que se aplican.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-187">The FX rates will be refreshed and available on the day before the first of the month for which they apply.</span></span>

## <a name="azure-reservations"></a><span data-ttu-id="bc7c1-188">Reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="bc7c1-188">Azure reservations</span></span>


<span data-ttu-id="bc7c1-189">Si compra [reservas de Azure](azure-reservations.md) a través de un plan de Azure, puede elegir la facturación única o mensual.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-189">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="bc7c1-190">Gastos de Azure</span><span class="sxs-lookup"><span data-stu-id="bc7c1-190">Azure spending</span></span>

<span data-ttu-id="bc7c1-191">La experiencia existente de gasto de Azure se ha actualizado para admitir la nueva facturación del plan de Azure en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-191">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="bc7c1-192">Esto permite a los partners:</span><span class="sxs-lookup"><span data-stu-id="bc7c1-192">This enables partners to:</span></span>

- <span data-ttu-id="bc7c1-193">Ver, administrar y recibir alertas del presupuesto establecido en un nivel de cliente.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-193">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="bc7c1-194">Ver el total de gastos estimados en un plan de Azure (desglosado por nivel de recurso y medidor).</span><span class="sxs-lookup"><span data-stu-id="bc7c1-194">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="bc7c1-195">Dado que el modelo de facturación para los servicios de Azure a través de un plan de Azure es el consumo de pago posterior, para evitar recibir una factura más grande de lo previsto, los partners pueden aplicar un presupuesto mensual y realizar un seguimiento del porcentaje de uso.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-195">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="bc7c1-196">Se puede aplicar un presupuesto a un cliente o a varios clientes al mismo tiempo.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-196">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Gastos de Azure":::

## <a name="next-steps"></a><span data-ttu-id="bc7c1-198">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="bc7c1-198">Next steps</span></span>

- <span data-ttu-id="bc7c1-199">Consulte cómo se calcula el crédito que obtiene el partner (PEC).</span><span class="sxs-lookup"><span data-stu-id="bc7c1-199">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="bc7c1-200">Inicie sesión en el [panel](https://partner.microsoft.com/dashboard/) del Centro de partners y busque la lista de precios disponible.</span><span class="sxs-lookup"><span data-stu-id="bc7c1-200">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="bc7c1-201">Obtenga información sobre la [compra del plan de Azure](purchase-azure-plan.md).</span><span class="sxs-lookup"><span data-stu-id="bc7c1-201">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="bc7c1-202">Consulte la [lista de precios para la nueva experiencia comercial en CSP](azure-plan-price-list.md).</span><span class="sxs-lookup"><span data-stu-id="bc7c1-202">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
