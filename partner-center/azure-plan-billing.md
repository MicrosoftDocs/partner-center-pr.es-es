---
title: 'Facturación del plan de Azure: facturas y archivos de conciliación'
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprende a obtener acceso y a comprender la estructura del archivo de conciliación y facturación relacionado con la facturación del plan de Azure.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: c7c06f5ed7b147625afb5020f63ead411ef58fa8
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551527"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a><span data-ttu-id="82c50-103">Nueva experiencia comercial en CSP: facturación de Azure</span><span class="sxs-lookup"><span data-stu-id="82c50-103">New commerce experience in CSP - Azure billing</span></span> 

<span data-ttu-id="82c50-104">**Roles adecuados**: Agente de administración | Administrador de facturación | Administrador global</span><span class="sxs-lookup"><span data-stu-id="82c50-104">**Appropriate roles**: Admin agent | Billing admin | Global admin</span></span>

<span data-ttu-id="82c50-105">En este artículo se describe cómo acceder a la estructura del archivo de conciliación y facturación relacionado con la facturación del plan de Azure, así cómo comprenderla.</span><span class="sxs-lookup"><span data-stu-id="82c50-105">This article explains how to access and understand the invoice and reconciliation file structure related to billing for the Azure plan.</span></span> <span data-ttu-id="82c50-106">La facturación del plan Azure es una experiencia de facturación simplificada que usa una fecha de facturación única alineada y un período de facturación basado en los meses del calendario.</span><span class="sxs-lookup"><span data-stu-id="82c50-106">Billing under the Azure plan is a simplified billing experience using an aligned single billing date and calendar month-based billing period.</span></span>

## <a name="summary-of-billing-essentials"></a><span data-ttu-id="82c50-107">Resumen de los elementos esenciales de la facturación</span><span class="sxs-lookup"><span data-stu-id="82c50-107">Summary of billing essentials</span></span>

- <span data-ttu-id="82c50-108">**Fecha de facturación**: La factura y el archivo de conciliación estarán disponibles en el panel o API del Centro de partners antes del día 8 (medianoche, UTC).</span><span class="sxs-lookup"><span data-stu-id="82c50-108">**Invoice date**: Invoice and reconciliation file will be available in the Partner Center dashboard/API by the 8th (midnight UTC).</span></span>

- <span data-ttu-id="82c50-109">**Período de facturación**: El período de facturación de la factura coincidirá con el mes natural; por ejemplo, 10/1-10/31, 11/1-11/30.</span><span class="sxs-lookup"><span data-stu-id="82c50-109">**Invoice billing period**: The invoice billing period is aligned to the calendar month, for example,  10/1-10/31, 11/1-11/30.</span></span>

- <span data-ttu-id="82c50-110">**Períodos del servicio de cargos**: Los cargos coincidirán con el mes natural.</span><span class="sxs-lookup"><span data-stu-id="82c50-110">**Charge service periods**: Charges will align to the calendar month.</span></span> <span data-ttu-id="82c50-111">Por ejemplo, si el partner facturado agrega servicios de Azure a través de un plan de Azure el 15/10 y el cliente comienza a consumir los servicios de Azure el mismo 15/10, el partner facturado recibirá la factura o la conciliación el 8/11 referente al consumo del cliente durante el período de servicio del 15/10 al 31/10.</span><span class="sxs-lookup"><span data-stu-id="82c50-111">For example, if billed partner adds Azure services through an Azure plan on 10/15 and the customer begins consumption of Azure services on 10/15, then billed partner will receive invoice/recon on 11/8 for customer consumption for the service period 10/15 - 10/31.</span></span> <span data-ttu-id="82c50-112">La factura del próximo mes que se generará el 8/12 y contendrá todos los cargos del período de servicio del 1/11 al 11/31.</span><span class="sxs-lookup"><span data-stu-id="82c50-112">The next month's invoice that is going to be generated on 12/8 contains all the charges for the service period 11/1- 11/31.</span></span>

- <span data-ttu-id="82c50-113">**Plazo de pago de la factura**: Neto, 60 días.</span><span class="sxs-lookup"><span data-stu-id="82c50-113">**Invoice payment term**: Net 60 days.</span></span>

- <span data-ttu-id="82c50-114">**Moneda de la factura** : A partir del 28 de enero de 2021, se facturará a los partners de la región de la UE/AELC y el Reino Unido que tengan nuevos clientes y clientes de CSP existentes que adquieran nuevas ofertas de comercio por primera vez y cuyos inquilinos se hayan creado antes del 11 de mayo de 2020 por esas compras en la moneda de la ubicación del partner.</span><span class="sxs-lookup"><span data-stu-id="82c50-114">**Invoice currency**: Starting January 28th 2021, partners in the EU/EFTA and UK region who have new customers and existing CSP customers purchasing new commerce offers for the first time whose tenants were created prior to 11 May 2020, will be billed for those purchases in partner location currency.</span></span> <span data-ttu-id="82c50-115">A los partners situados fuera de la región de la UE/AELC y el Reino Unido se les seguirá facturando en la moneda de la ubicación del partner.</span><span class="sxs-lookup"><span data-stu-id="82c50-115">Partners located outside of the EU/EFTA and UK region will continue to be billed in partner location currency.</span></span>

- <span data-ttu-id="82c50-116">**Incentivos de partners**: Pagado a 45 días desde el final del mes de la factura.</span><span class="sxs-lookup"><span data-stu-id="82c50-116">**Partner incentives**: Paid 45 days from the end of the invoice month.</span></span>

## <a name="access-your-invoices-and-reconciliation-files"></a><span data-ttu-id="82c50-117">Acceder a las facturas y los archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="82c50-117">Access your invoices and reconciliation files</span></span>

<span data-ttu-id="82c50-118">El administrador global o el administrador de facturación de tu empresa recibirá un correo electrónico cuando una factura esté lista para ver.</span><span class="sxs-lookup"><span data-stu-id="82c50-118">The global admin or billing admin for your company will receive an email when an invoice is ready to view.</span></span>

<span data-ttu-id="82c50-119">Para acceder a la factura y al archivo de conciliación:</span><span class="sxs-lookup"><span data-stu-id="82c50-119">To access the invoice and reconciliation file:</span></span>

1. <span data-ttu-id="82c50-120">Inicia sesión en el [panel](https://partner.microsoft.com/dashboard/) del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="82c50-120">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="82c50-121">En el menú del Centro de partners, selecciona **Billing** (Facturación).</span><span class="sxs-lookup"><span data-stu-id="82c50-121">From the Partner Center menu, select **Billing**.</span></span>

3. <span data-ttu-id="82c50-122">Selecciona la pestaña de **Periódico** y **Una vez** y la moneda que te interese.</span><span class="sxs-lookup"><span data-stu-id="82c50-122">Select the tab for the **Recurring** and **One-time** and the currency you are interested in.</span></span>

   :::image type="content" source="images/azure/billing3.png" alt-text="Facturación.":::

4. <span data-ttu-id="82c50-124">Selecciona **Factura** o **Archivo de conciliación**.</span><span class="sxs-lookup"><span data-stu-id="82c50-124">Select **Invoice** or **Reconciliation file**.</span></span>  

   <span data-ttu-id="82c50-125">Para ver las facturas históricas y los archivos de conciliación, amplía la fila del historial de facturación a continuación.</span><span class="sxs-lookup"><span data-stu-id="82c50-125">To view historical invoices and recon files expand the Billing history row below.</span></span>

## <a name="understanding-usage-data"></a><span data-ttu-id="82c50-126">Explicación de los datos de uso</span><span class="sxs-lookup"><span data-stu-id="82c50-126">Understanding usage data</span></span> 

1. <span data-ttu-id="82c50-127">El plan de Azure es el contenedor raíz o de nivel superior para el uso.</span><span class="sxs-lookup"><span data-stu-id="82c50-127">Azure plan is the root or top-level container for usage.</span></span> <span data-ttu-id="82c50-128">Todo el uso está vinculado a un único plan de Azure.</span><span class="sxs-lookup"><span data-stu-id="82c50-128">All usage is tied back to a single Azure plan.</span></span>

2. <span data-ttu-id="82c50-129">En un plan, habrá una o varias suscripciones de Azure.</span><span class="sxs-lookup"><span data-stu-id="82c50-129">Within a plan, there will be one or more Azure subscriptions.</span></span> <span data-ttu-id="82c50-130">Estos son los contenedores que se usan para la implementación y la administración de recursos.</span><span class="sxs-lookup"><span data-stu-id="82c50-130">These are containers used for resource management and deployment.</span></span> 

3. <span data-ttu-id="82c50-131">En una suscripción, los grupos de recursos se agregan a recursos de grupo.</span><span class="sxs-lookup"><span data-stu-id="82c50-131">Within a subscription, resource groups add to group resources.</span></span> <span data-ttu-id="82c50-132">Cada recurso se implementa en un grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="82c50-132">Every resource is deployed to one resource group.</span></span> 

4. <span data-ttu-id="82c50-133">Entre los ejemplos de recursos se incluyen las máquinas virtuales y las cuentas de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="82c50-133">Examples of resources include virtual machines and storage accounts.</span></span> 

5. <span data-ttu-id="82c50-134">Los recursos emiten medidores: Los medidores son medidas de consumo de un recurso, y un recurso puede emitir el uso de varios medidores.</span><span class="sxs-lookup"><span data-stu-id="82c50-134">Resource emit meters: Meters are measurements of consumption of a resource, and one resource may emit usage for multiple meters.</span></span> <span data-ttu-id="82c50-135">Los medidores se identifican mediante ProductId, SKUId y AvailabilityId.</span><span class="sxs-lookup"><span data-stu-id="82c50-135">Meters are identified by a ProductId, SKUId, and AvailabilityId.</span></span> 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a><span data-ttu-id="82c50-136">Jerarquía de grupos de recursos de suscripción y medición</span><span class="sxs-lookup"><span data-stu-id="82c50-136">Hierarchy of subscription resource groups and metering</span></span>

<span data-ttu-id="82c50-137">**Cuenta de Azure (inquilino)**</span><span class="sxs-lookup"><span data-stu-id="82c50-137">**Azure account (tenant)**</span></span>

- <span data-ttu-id="82c50-138">Suscripción A</span><span class="sxs-lookup"><span data-stu-id="82c50-138">Subscription A</span></span>
    - <span data-ttu-id="82c50-139">ResourceGroup 1</span><span class="sxs-lookup"><span data-stu-id="82c50-139">ResourceGroup 1</span></span>
        - <span data-ttu-id="82c50-140">Máquina virtual (recurso)</span><span class="sxs-lookup"><span data-stu-id="82c50-140">Virtual machine (resource)</span></span>
            - <span data-ttu-id="82c50-141">Medidor de proceso</span><span class="sxs-lookup"><span data-stu-id="82c50-141">Compute meter</span></span>
        - <span data-ttu-id="82c50-142">Virtual Network (recurso)</span><span class="sxs-lookup"><span data-stu-id="82c50-142">Virtual network (resource)</span></span>
            - <span data-ttu-id="82c50-143">Sin medidor de facturación</span><span class="sxs-lookup"><span data-stu-id="82c50-143">No billing meter</span></span>

    - <span data-ttu-id="82c50-144">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="82c50-144">ResourceGroup 2</span></span>
        - <span data-ttu-id="82c50-145">Máquina virtual (recurso)</span><span class="sxs-lookup"><span data-stu-id="82c50-145">Virtual machine (resource)</span></span>
            - <span data-ttu-id="82c50-146">Medidor de proceso</span><span class="sxs-lookup"><span data-stu-id="82c50-146">Computer meter</span></span>
        - <span data-ttu-id="82c50-147">Disco administrado SSD Premium (recurso)</span><span class="sxs-lookup"><span data-stu-id="82c50-147">Premium SSD-managed disk (resource)</span></span>
            - <span data-ttu-id="82c50-148">Medidor de capacidad de almacenamiento</span><span class="sxs-lookup"><span data-stu-id="82c50-148">Storage capacity meter</span></span>
            - <span data-ttu-id="82c50-149">Medidor de operaciones de almacenamiento</span><span class="sxs-lookup"><span data-stu-id="82c50-149">Storage operations meter</span></span>

- <span data-ttu-id="82c50-150">Suscripción B   -ResourceGroup 1       - Azure SQL (recurso)           - Medidor de DTU       - VPN Gateway (recurso)           - Medidor de VPN Gateway</span><span class="sxs-lookup"><span data-stu-id="82c50-150">Subscription B   -ResourceGroup 1       - Azure SQL (resource)           - DTU meter       - VPN Gateway (resource)           - VPN gateway meter</span></span>

    - <span data-ttu-id="82c50-151">ResourceGroup 2</span><span class="sxs-lookup"><span data-stu-id="82c50-151">ResourceGroup 2</span></span>
        - <span data-ttu-id="82c50-152">Interfaz de Virtual Network (recurso)</span><span class="sxs-lookup"><span data-stu-id="82c50-152">Virtual Network Interface (resource)</span></span>
            - <span data-ttu-id="82c50-153">Sin medidor de facturación</span><span class="sxs-lookup"><span data-stu-id="82c50-153">No billing meter</span></span>

## <a name="read-the-invoice"></a><span data-ttu-id="82c50-154">Leer la factura</span><span class="sxs-lookup"><span data-stu-id="82c50-154">Read the invoice</span></span>

1. <span data-ttu-id="82c50-155">La factura estará disponible el día ocho de cada mes a más tardar.</span><span class="sxs-lookup"><span data-stu-id="82c50-155">Invoice will be available no later than the eighth of each month.</span></span>

2. <span data-ttu-id="82c50-156">Los partners tienen 60 días para remitir el pago.</span><span class="sxs-lookup"><span data-stu-id="82c50-156">Partners have 60 days to remit payment.</span></span>

3. <span data-ttu-id="82c50-157">El período de facturación cubrirá un mes dado del calendario; por ejemplo del 1/10 al 31/10.</span><span class="sxs-lookup"><span data-stu-id="82c50-157">The billing period will cover a given calendar month, for example, 10/1-10/31.</span></span>

4. <span data-ttu-id="82c50-158">Los cargos son netos en cuanto a los ajustes (el importe es el valor neto del "crédito obtenido del partner por los servicios administrados").</span><span class="sxs-lookup"><span data-stu-id="82c50-158">Charges are net of adjustments (amount is net of “Partner earned credit for services managed").</span></span>

5. <span data-ttu-id="82c50-159">Revisa el archivo de conciliación de facturas y el archivo de uso con clasificación diaria para obtener los detalles adicionales de facturación.</span><span class="sxs-lookup"><span data-stu-id="82c50-159">Review the invoice recon file and daily rated usage file for additional billing details.</span></span>

   :::image type="content" source="images/azure/invoice1.png" alt-text="Factura.":::

## <a name="read-the-invoice-reconciliation-file"></a><span data-ttu-id="82c50-161">Lectura del archivo de conciliación de facturas</span><span class="sxs-lookup"><span data-stu-id="82c50-161">Read the invoice reconciliation file</span></span>

1. <span data-ttu-id="82c50-162">Cada combinación de medidor y plan de Azure puede tener hasta dos líneas de facturación en el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="82c50-162">Each Azure plan and meter combination may have up to two billing lines on the recon file.</span></span>

2. <span data-ttu-id="82c50-163">Si el medidor puede tener en cuenta cualquier tipo de descuento o crédito (como los descuentos por nivel o el crédito obtenido del partner por los servicios administrados) durante todo el mes natural, el archivo de conciliación solo contendrá una línea de facturación.</span><span class="sxs-lookup"><span data-stu-id="82c50-163">If the meter qualified for any type of discount or credit (such as tiered discounts or the Partner earned credit for services managed) throughout the entire calendar month, then the recon file will only contain one billing line.</span></span> <span data-ttu-id="82c50-164">La columna **PriceAdjusmentDescription** hará referencia al descuento o al crédito obtenido.</span><span class="sxs-lookup"><span data-stu-id="82c50-164">The column **PriceAdjusmentDescription** will reference the discount or earned credit.</span></span>

3. <span data-ttu-id="82c50-165">Si no existen recursos para un medidor concreto que es apto para el descuento o el crédito obtenido del partner, el archivo de conciliación solo contendrá una línea de facturación y el precio por unidad vigente será el precio de venta al por menor (que es el precio por unidad).</span><span class="sxs-lookup"><span data-stu-id="82c50-165">If there are no resources for a particular meter that qualified for discount or partner earned credit, then the recon file will only contain one billing line and the effective unit price will be the retail price (which is the unit price).</span></span>

4. <span data-ttu-id="82c50-166">Si el medidor (o cualquier recurso que este emita) es apto para el **crédito obtenido del partner para los servicios administrados** durante una parte del mes, el archivo de conciliación contendrá dos líneas de facturación.</span><span class="sxs-lookup"><span data-stu-id="82c50-166">If the meter, or any resources emitting that meter, qualified for **Partner earned credit for services managed** for a part of the month, the recon file will contain two billing lines.</span></span> <span data-ttu-id="82c50-167">Una línea representará los días que el medidor haya calificado y la segunda línea representará los días que el medidor no calificó.</span><span class="sxs-lookup"><span data-stu-id="82c50-167">One line will represent the days the meter qualified and the second line will represent the days the meter did not qualify.</span></span>

>[!NOTE]
><span data-ttu-id="82c50-168">Puede conciliar el consumo de Azure en el archivo de conciliación de una sola compra.</span><span class="sxs-lookup"><span data-stu-id="82c50-168">You can reconcile your Azure consumption in your one-time purchase recon file.</span></span> <span data-ttu-id="82c50-169">Para ello, vaya al archivo de conciliación de uso clasificado diariamente y busque su subscriptionID.</span><span class="sxs-lookup"><span data-stu-id="82c50-169">To do this, go to your daily-rated usage recon file and search for your SubscriptionID.</span></span> <span data-ttu-id="82c50-170">Se mostrarán todos los costos asociados con su identificador del plan de Azure.</span><span class="sxs-lookup"><span data-stu-id="82c50-170">This will display all costs associated with your Azure Plan ID.</span></span> <span data-ttu-id="82c50-171">Su SubscriptionID de Azure se muestra como EntitlementID.</span><span class="sxs-lookup"><span data-stu-id="82c50-171">Your Azure SubscriptionID is shown as the EntitlementID.</span></span>

## <a name="read-the-daily-usage-file"></a><span data-ttu-id="82c50-172">Leer el archivo de uso diario</span><span class="sxs-lookup"><span data-stu-id="82c50-172">Read the daily usage file</span></span>

- <span data-ttu-id="82c50-173">Los medidores de suscripción en un plan de Azure se clasifican y se acumulan diariamente.</span><span class="sxs-lookup"><span data-stu-id="82c50-173">Subscription meters under an Azure plan are rated, and are cumulated, on a daily basis.</span></span>

- <span data-ttu-id="82c50-174">**El crédito obtenido del partner por los servicios administrados**  se determina y se aplica diariamente.</span><span class="sxs-lookup"><span data-stu-id="82c50-174">**Partner earned credit for services managed** is determined and applied on a daily basis.</span></span>

- <span data-ttu-id="82c50-175">Cada medidor de suscripciones tendrá una fila por cada día del mes en el que se haya consumido.</span><span class="sxs-lookup"><span data-stu-id="82c50-175">Every subscription meter will have a row for every day of the month where there was consumption.</span></span>

- <span data-ttu-id="82c50-176">Consulta el ejemplo que aparece a continuación:</span><span class="sxs-lookup"><span data-stu-id="82c50-176">In the example below:</span></span>

  - <span data-ttu-id="82c50-177">El medidor es apto para el **crédito obtenido del partner por los servicios administrados** del 1/7 al 3/7 (ten en cuenta que el precio unitario efectivo es el precio del minorista menos el crédito obtenido del partner).</span><span class="sxs-lookup"><span data-stu-id="82c50-177">Meter qualified for **Partner earned credit for services managed** from 7/1 - 7/3 (note the effective unit price is retail price less partner earned credit.</span></span>

  - <span data-ttu-id="82c50-178">El medidor no es apto para el **crédito obtenido del partner por los servicios administrados** del 4/7 al 7/7 (ten en cuenta que el precio unitario efectivo es el precio del minorista).</span><span class="sxs-lookup"><span data-stu-id="82c50-178">Meter didn't qualify for **Partner earned credit for services managed** from 7/4 - 7/7 (note the effective unit price is retail price).</span></span>

  - <span data-ttu-id="82c50-179">El medidor es apto para el **crédito obtenido del partner por los servicios administrados** del 8/7 al 31/7 (ten en cuenta que el precio unitario efectivo es el precio del minorista menos el crédito obtenido del partner).</span><span class="sxs-lookup"><span data-stu-id="82c50-179">Meter qualified for **Partner earned credit for services managed** from 7/8 - 7/31 (note the effective unit price is retail price less partner earned credit).</span></span>

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-customer-currency"></a><span data-ttu-id="82c50-181">Factura en la moneda del cliente</span><span class="sxs-lookup"><span data-stu-id="82c50-181">Invoice in customer currency</span></span>

<span data-ttu-id="82c50-182">Los servicios de Azure a través de un plan de Azure tendrán un precio de USD y se facturarán en la moneda asignada en el país del cliente.</span><span class="sxs-lookup"><span data-stu-id="82c50-182">Azure services through an Azure plan will be priced in USD and billed in the customer country assigned currency.</span></span> <span data-ttu-id="82c50-183">Si la moneda de facturación no es USD, el tipo de cambio usado se mostrará en la última página de la factura.</span><span class="sxs-lookup"><span data-stu-id="82c50-183">If the billing currency is non-USD, then the Foreign exchange (FX) rate used will be shown on the last page of the invoice.</span></span> <span data-ttu-id="82c50-184">Los tipos de cambio se determinan mensualmente y se aplican a la factura siguiente.</span><span class="sxs-lookup"><span data-stu-id="82c50-184">FX rates are determined monthly and applied to the following invoice.</span></span> <span data-ttu-id="82c50-185">Para obtener una lista completa de las monedas de los países, consulta la [matriz de moneda del cliente y la disponibilidad de los países en cuanto a las nuevas ofertas comerciales](https://go.microsoft.com/fwlink/?linkid=2112354).</span><span class="sxs-lookup"><span data-stu-id="82c50-185">For a full list of country currencies, please view the [new commerce offers country availability and customer currency matrix](https://go.microsoft.com/fwlink/?linkid=2112354).</span></span>

<span data-ttu-id="82c50-186">Microsoft aplica un tipo de cambio predeterminado a los precios en USD base para llegar a los cargos totales en los que se incurre por los servicios de Azure adquiridos o consumidos cada mes natural.</span><span class="sxs-lookup"><span data-stu-id="82c50-186">Microsoft applies a predetermined exchange rate to base USD prices to arrive at total charges incurred for Azure services purchased or consumed each calendar month.</span></span> <span data-ttu-id="82c50-187">El tipo de cambio mensual es el tipo de cambio medio publicado por Thomson Reuters (normalmente) dos días laborables antes del fin de mes anterior a las 16:00 GMT.</span><span class="sxs-lookup"><span data-stu-id="82c50-187">The monthly exchange rate is the mid-rate published by Thomson Reuters (typically) two business days prior to the preceding month-end at 4:00 pm GMT.</span></span> 

<span data-ttu-id="82c50-188">**Por ejemplo,** el tipo de cambio de diciembre de Microsoft sería el tipo de cambio medio de Thomson Reuters el 29 de noviembre o una fecha aproximadamente para una moneda determinada.</span><span class="sxs-lookup"><span data-stu-id="82c50-188">**For example,** Microsoft’s December exchange rate would be the Thomson Reuters mid-rate on or around November 29 for a given currency.</span></span> <span data-ttu-id="82c50-189">Dicho tipo se aplicará a todas las compras en esa moneda del 1 al 31 de diciembre.</span><span class="sxs-lookup"><span data-stu-id="82c50-189">That rate will be applied to all purchases in that currency from December 1 to December 31.</span></span> 

## <a name="azure-reservations"></a><span data-ttu-id="82c50-190">Reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="82c50-190">Azure reservations</span></span>


<span data-ttu-id="82c50-191">Si compra [reservas de Azure](azure-reservations.md) a través de un plan de Azure, puede elegir la facturación única o mensual.</span><span class="sxs-lookup"><span data-stu-id="82c50-191">If purchasing [Azure reservations](azure-reservations.md) through an Azure plan, you can choose either one-time or monthly billing.</span></span>


## <a name="azure-spending"></a><span data-ttu-id="82c50-192">Gastos de Azure</span><span class="sxs-lookup"><span data-stu-id="82c50-192">Azure spending</span></span>

<span data-ttu-id="82c50-193">La experiencia existente de gasto de Azure se ha actualizado para admitir la nueva facturación del plan de Azure en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="82c50-193">The existing Azure spending experience is updated to support the new Azure plan billing in Partner Center.</span></span> <span data-ttu-id="82c50-194">Esto permite a los partners:</span><span class="sxs-lookup"><span data-stu-id="82c50-194">This enables partners to:</span></span>

- <span data-ttu-id="82c50-195">Ver, administrar y recibir alertas del presupuesto establecido en un nivel de cliente.</span><span class="sxs-lookup"><span data-stu-id="82c50-195">View, manage, and receive alerts for budget set at a customer level</span></span> 

- <span data-ttu-id="82c50-196">Ver el total de gastos estimados en un plan de Azure (desglosado por nivel de recurso y medidor).</span><span class="sxs-lookup"><span data-stu-id="82c50-196">View total estimated spending on an Azure plan (broken down by resource and meter level)</span></span>

<span data-ttu-id="82c50-197">Dado que el modelo de facturación para los servicios de Azure a través de un plan de Azure es el consumo de pago posterior, para evitar recibir una factura más grande de lo previsto, los partners pueden aplicar un presupuesto mensual y realizar un seguimiento del porcentaje de uso.</span><span class="sxs-lookup"><span data-stu-id="82c50-197">Because the billing model for Azure services through an Azure plan is post-pay consumption, to avoid a bigger bill than anticipated, partners can apply a monthly budget and track the percentage of usage.</span></span> <span data-ttu-id="82c50-198">Se puede aplicar un presupuesto a un cliente o a varios clientes al mismo tiempo.</span><span class="sxs-lookup"><span data-stu-id="82c50-198">A budget can be applied to one customer or multiple customers at one time.</span></span> 

:::image type="content" source="images/azure/azurespend.png" alt-text="Gastos de Azure.":::

## <a name="next-steps"></a><span data-ttu-id="82c50-200">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="82c50-200">Next steps</span></span>

- <span data-ttu-id="82c50-201">Consulte cómo se calcula el crédito que obtiene el partner (PEC).</span><span class="sxs-lookup"><span data-stu-id="82c50-201">See how the partner earned credit (PEC) is calculated.</span></span> <span data-ttu-id="82c50-202">Inicie sesión en el [panel](https://partner.microsoft.com/dashboard/) del Centro de partners y busque la lista de precios disponible.</span><span class="sxs-lookup"><span data-stu-id="82c50-202">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/) and locate the price list available.</span></span>

- <span data-ttu-id="82c50-203">Obtenga información sobre la [compra del plan de Azure](purchase-azure-plan.md).</span><span class="sxs-lookup"><span data-stu-id="82c50-203">Learn about [purchasing the Azure plan](purchase-azure-plan.md)</span></span>

- <span data-ttu-id="82c50-204">Consulte la [lista de precios para la nueva experiencia comercial en CSP](azure-plan-price-list.md).</span><span class="sxs-lookup"><span data-stu-id="82c50-204">See the [price list for the new commerce experience in CSP](azure-plan-price-list.md)</span></span>
