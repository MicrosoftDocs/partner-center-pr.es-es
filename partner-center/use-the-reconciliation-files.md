---
title: "Usar los archivos de conciliación | Centro de partners"
description: "Para obtener una vista detallada del elemento de línea de cada cargo en un ciclo de facturación, descarga los archivos de conciliación desde el panel del Centro de partners."
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.openlocfilehash: 892204ebcdfe1e1318985f2d50df8af2238bd4c1
ms.sourcegitcommit: 2436cb77fbefc41cc9cb3e62e8a616b6326c557f
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/04/2017
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="a0e23-103">Usar los archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="a0e23-103">Use the reconciliation files</span></span>

**<span data-ttu-id="a0e23-104">Se aplica a</span><span class="sxs-lookup"><span data-stu-id="a0e23-104">Applies to</span></span>**

-  <span data-ttu-id="a0e23-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="a0e23-105">Partner Center</span></span>
-  <span data-ttu-id="a0e23-106">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="a0e23-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="a0e23-107">Centro de partners para Microsoft Cloud Alemania</span><span class="sxs-lookup"><span data-stu-id="a0e23-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="a0e23-108">Para obtener una vista detallada del elemento de línea de cada cargo en un ciclo de facturación, descarga los archivos de conciliación desde el panel del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="a0e23-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="a0e23-109">Los detalles incluyen los cargos para las suscripciones de cada cliente y los eventos detallados (por ejemplo, una adición intermedia de puestos en una suscripción).</span><span class="sxs-lookup"><span data-stu-id="a0e23-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="a0e23-110">Desglosar por partner</span><span class="sxs-lookup"><span data-stu-id="a0e23-110">Itemize by partner</span></span>


<span data-ttu-id="a0e23-111">Los partners del modelo indirecto pueden usar estos campos adicionales en ambos archivos de conciliación basada en uso y en licencia para realizar el desglose por revendedor.</span><span class="sxs-lookup"><span data-stu-id="a0e23-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="a0e23-112">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="a0e23-112">MPN ID</span></span></th>
<th><span data-ttu-id="a0e23-113">Descripción</span><span class="sxs-lookup"><span data-stu-id="a0e23-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="a0e23-114">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="a0e23-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="a0e23-115">Id. de Microsoft Partner Network (MPN) del partner de CSP (directo o indirecto).</span><span class="sxs-lookup"><span data-stu-id="a0e23-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-116">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="a0e23-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="a0e23-117">Solo aparece en los archivos de conciliación de partners en el modelo indirecto.</span><span class="sxs-lookup"><span data-stu-id="a0e23-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="a0e23-118">El Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="a0e23-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="a0e23-119">Corresponde al id. de revendedor indicado para la suscripción específica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="a0e23-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="a0e23-120">Para ver o actualizar el revendedor, en el menú del Centro de partners, selecciona <strong>Clientes</strong> y, después, elige el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="a0e23-120">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="a0e23-121">En el menú del cliente, selecciona <strong>Suscripciones</strong> y elige la suscripción de la lista.</span><span class="sxs-lookup"><span data-stu-id="a0e23-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="a0e23-122">Selecciona <strong>Actualizar</strong> para cambiar el valor de <strong>Revendedor (id. de MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="a0e23-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="a0e23-123">Si un partner CSP vendió la suscripción directamente al cliente, su id. de MPN aparece dos veces, como id. de MPN y como id. de MPN del revendedor.</span><span class="sxs-lookup"><span data-stu-id="a0e23-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="a0e23-124">Si un partner CSP tiene un revendedor sin un id. de MPN, este valor se establece en el id. de MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="a0e23-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="a0e23-125">Si el partner CSP quita un id. de revendedor, este valor se establece en -1.</span><span class="sxs-lookup"><span data-stu-id="a0e23-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="a0e23-126">Campos de archivo basados en licencia</span><span class="sxs-lookup"><span data-stu-id="a0e23-126">License-based file fields</span></span>


<span data-ttu-id="a0e23-127">Para conciliar los cargos en función de los pedidos del cliente, compara el Syndication\_Partner\_Subscription\_Number del archivo de conciliación con el identificador de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="a0e23-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="a0e23-128">Columna</span><span class="sxs-lookup"><span data-stu-id="a0e23-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="a0e23-129">Descripción</span><span class="sxs-lookup"><span data-stu-id="a0e23-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="a0e23-130">Valor de muestra</span><span class="sxs-lookup"><span data-stu-id="a0e23-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-131">PartnerId</span><span class="sxs-lookup"><span data-stu-id="a0e23-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="a0e23-132">Identificador único de una entidad de facturación específica, con formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="a0e23-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="a0e23-133">No es necesario para la reconciliación, pero puede ser información útil.</span><span class="sxs-lookup"><span data-stu-id="a0e23-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="a0e23-134">Igual en todas las filas.</span><span class="sxs-lookup"><span data-stu-id="a0e23-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="a0e23-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="a0e23-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="a0e23-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="a0e23-137">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="a0e23-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="a0e23-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="a0e23-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="a0e23-139">OrderID</span></span></td>
<td><p><span data-ttu-id="a0e23-140">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a0e23-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="a0e23-141">Puede ser útil para identificar al pedido al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="a0e23-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="a0e23-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="a0e23-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="a0e23-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="a0e23-144">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a0e23-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="a0e23-145">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="a0e23-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="a0e23-146">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="a0e23-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="a0e23-147">Consulte Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="a0e23-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="a0e23-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="a0e23-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="a0e23-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="a0e23-150">Identificador único de las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="a0e23-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="a0e23-151">Un cliente puede tener varias suscripciones para el mismo plan, por lo que es importante para el análisis de archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="a0e23-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="a0e23-152">Este campo se asigna al identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="a0e23-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="a0e23-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="a0e23-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="a0e23-154">OfferID</span></span></td>
<td><p><span data-ttu-id="a0e23-155">Identificador único de la oferta.</span><span class="sxs-lookup"><span data-stu-id="a0e23-155">Unique offer ID.</span></span> <span data-ttu-id="a0e23-156">Identificador de la oferta estándar según la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="a0e23-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="a0e23-157"><b>Nota</b>: este valor no coincide con el id. de oferta de la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="a0e23-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="a0e23-158">Consulta DurableOfferID a continuación.</span><span class="sxs-lookup"><span data-stu-id="a0e23-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="a0e23-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="a0e23-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="a0e23-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="a0e23-161">Id. de oferta duradera único, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="a0e23-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="a0e23-162"><b>Nota</b>: este valor coincide con el id. de oferta de la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="a0e23-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="a0e23-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="a0e23-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="a0e23-164">OfferName</span></span></td>
<td><p><span data-ttu-id="a0e23-165">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="a0e23-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="a0e23-166">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="a0e23-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="a0e23-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="a0e23-168">Fecha de finalización de la suscripción, establecida en el día posterior al envío del pedido.</span><span class="sxs-lookup"><span data-stu-id="a0e23-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="a0e23-169">Al consultar la fecha de inicio de la suscripción junto con la fecha de finalización, puedes determinar si el cliente aún está dentro del primer año de la suscripción o si la suscripción se ha renovado para el año siguiente.</span><span class="sxs-lookup"><span data-stu-id="a0e23-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="a0e23-170">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="a0e23-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="a0e23-171">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="a0e23-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="a0e23-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="a0e23-173">La fecha de finalización de la suscripción: 12 meses + x días después de la fecha de inicio (para que se alinee con la fecha de facturación del partner) o 12 meses a partir de la fecha de renovación.</span><span class="sxs-lookup"><span data-stu-id="a0e23-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="a0e23-174">En el momento de la renovación, los precios se actualizan según la lista de precios actual.</span><span class="sxs-lookup"><span data-stu-id="a0e23-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="a0e23-175">Es posible que se necesite una comunicación con el cliente antes de la renovación automatizada.</span><span class="sxs-lookup"><span data-stu-id="a0e23-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="a0e23-176">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="a0e23-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="a0e23-177">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="a0e23-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="a0e23-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="a0e23-179">Día de inicio de los cargos.</span><span class="sxs-lookup"><span data-stu-id="a0e23-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="a0e23-180">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="a0e23-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="a0e23-181">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="a0e23-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="a0e23-182">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="a0e23-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="a0e23-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="a0e23-184">Día de finalización de los cargos.</span><span class="sxs-lookup"><span data-stu-id="a0e23-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="a0e23-185">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="a0e23-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="a0e23-186">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="a0e23-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="a0e23-187">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="a0e23-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="a0e23-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="a0e23-189">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="a0e23-189">The type of charge or adjustment.</span></span> <span data-ttu-id="a0e23-190">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="a0e23-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="a0e23-191">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="a0e23-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="a0e23-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="a0e23-193">Precio por puesto.</span><span class="sxs-lookup"><span data-stu-id="a0e23-193">Price per seat.</span></span> <span data-ttu-id="a0e23-194">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="a0e23-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="a0e23-195">6.82</span><span class="sxs-lookup"><span data-stu-id="a0e23-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-196">Quantity</span><span class="sxs-lookup"><span data-stu-id="a0e23-196">Quantity</span></span></td>
<td><p><span data-ttu-id="a0e23-197">Número de puestos.</span><span class="sxs-lookup"><span data-stu-id="a0e23-197">Number of seats.</span></span> <span data-ttu-id="a0e23-198">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="a0e23-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="a0e23-199">2</span><span class="sxs-lookup"><span data-stu-id="a0e23-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-200">Amount</span><span class="sxs-lookup"><span data-stu-id="a0e23-200">Amount</span></span></td>
<td><p><span data-ttu-id="a0e23-201">Total del precio para la cantidad.</span><span class="sxs-lookup"><span data-stu-id="a0e23-201">Total of price for quantity.</span></span> <span data-ttu-id="a0e23-202">Es de utilidad para comprobar que el cálculo de la cantidad coincide con la manera de calcular este valor para los clientes.</span><span class="sxs-lookup"><span data-stu-id="a0e23-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="a0e23-203">13.32</span><span class="sxs-lookup"><span data-stu-id="a0e23-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="a0e23-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="a0e23-205">Cantidad de descuento que se aplica a estos cargos.</span><span class="sxs-lookup"><span data-stu-id="a0e23-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="a0e23-206">Los IUR o las nuevas suscripciones que puedan optar a un incentivo también incluirán un importe de descuento en esta columna.</span><span class="sxs-lookup"><span data-stu-id="a0e23-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="a0e23-207">2.32</span><span class="sxs-lookup"><span data-stu-id="a0e23-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-208">Subtotal</span><span class="sxs-lookup"><span data-stu-id="a0e23-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="a0e23-209">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="a0e23-209">Total before tax.</span></span> <span data-ttu-id="a0e23-210">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="a0e23-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="a0e23-211">11</span><span class="sxs-lookup"><span data-stu-id="a0e23-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-212">Tax</span><span class="sxs-lookup"><span data-stu-id="a0e23-212">Tax</span></span></td>
<td><p><span data-ttu-id="a0e23-213">Cargo por importe de impuestos, en función de las reglas fiscales de tu mercado y las circunstancias específicas.</span><span class="sxs-lookup"><span data-stu-id="a0e23-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="a0e23-214">0</span><span class="sxs-lookup"><span data-stu-id="a0e23-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="a0e23-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="a0e23-216">Total con impuestos.</span><span class="sxs-lookup"><span data-stu-id="a0e23-216">Total after tax.</span></span> <span data-ttu-id="a0e23-217">Comprueba si se cobran impuestos en la factura.</span><span class="sxs-lookup"><span data-stu-id="a0e23-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="a0e23-218">11</span><span class="sxs-lookup"><span data-stu-id="a0e23-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-219">Currency</span><span class="sxs-lookup"><span data-stu-id="a0e23-219">Currency</span></span></td>
<td><p><span data-ttu-id="a0e23-220">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="a0e23-220">Currency type.</span></span> <span data-ttu-id="a0e23-221">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="a0e23-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="a0e23-222">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="a0e23-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="a0e23-223">EUR</span><span class="sxs-lookup"><span data-stu-id="a0e23-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="a0e23-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="a0e23-225">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="a0e23-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="a0e23-226">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="a0e23-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="a0e23-227">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="a0e23-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="a0e23-228">MPNID</span></span></td>
<td><p><span data-ttu-id="a0e23-229">Id. de MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="a0e23-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="a0e23-230">4390934</span><span class="sxs-lookup"><span data-stu-id="a0e23-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="a0e23-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="a0e23-232">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="a0e23-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="a0e23-233">Ver [Desglosar por partner](#itemizebypartner)</span><span class="sxs-lookup"><span data-stu-id="a0e23-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="a0e23-234">4390934</span><span class="sxs-lookup"><span data-stu-id="a0e23-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="a0e23-235">DomainName</span></span></td>
<td><p><span data-ttu-id="a0e23-236">Nombre de dominio del cliente, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="a0e23-236">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="a0e23-237">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="a0e23-237">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-238">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="a0e23-238">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="a0e23-239">Alias de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="a0e23-239">Subscription nickname.</span></span> <span data-ttu-id="a0e23-240">Si no se especifica ningún alias, el Centro de partners usa OfferName.</span><span class="sxs-lookup"><span data-stu-id="a0e23-240">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="a0e23-241">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="a0e23-241">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-242">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="a0e23-242">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="a0e23-243">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="a0e23-243">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="a0e23-244">(Este es un campo idéntico al nombre de la oferta).</span><span class="sxs-lookup"><span data-stu-id="a0e23-244">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="a0e23-245">PROJECT ONLINE PREMIUM SIN CLIENTE DE PROJECT</span><span class="sxs-lookup"><span data-stu-id="a0e23-245">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="a0e23-246">Campos de archivos basados en el uso</span><span class="sxs-lookup"><span data-stu-id="a0e23-246">Usage-based file fields</span></span>


<span data-ttu-id="a0e23-247">Para conciliar los cargos en función del uso de tu cliente, compara los valores de ResellerID/ResellerName/ResellerBillableAccount del archivo de conciliación, el nombre del cliente y el id. de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="a0e23-247">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="a0e23-248">Los siguientes campos explican los servicios usados y la clasificación.</span><span class="sxs-lookup"><span data-stu-id="a0e23-248">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="a0e23-249">Columna</span><span class="sxs-lookup"><span data-stu-id="a0e23-249">Column</span></span></strong></td>
<td><strong><span data-ttu-id="a0e23-250">Descripción</span><span class="sxs-lookup"><span data-stu-id="a0e23-250">Description</span></span></strong></td>
<td><strong><span data-ttu-id="a0e23-251">Valor de muestra</span><span class="sxs-lookup"><span data-stu-id="a0e23-251">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-252">PartnerID</span><span class="sxs-lookup"><span data-stu-id="a0e23-252">PartnerID</span></span></td>
<td><p><span data-ttu-id="a0e23-253">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="a0e23-253">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="a0e23-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="a0e23-254">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-255">PartnerName</span><span class="sxs-lookup"><span data-stu-id="a0e23-255">PartnerName</span></span></td>
<td><p><span data-ttu-id="a0e23-256">Nombre del partner.</span><span class="sxs-lookup"><span data-stu-id="a0e23-256">Partner Name.</span></span></p></td>
<td><span data-ttu-id="a0e23-257">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="a0e23-257">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-258">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="a0e23-258">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="a0e23-259">Id. de cuenta del partner.</span><span class="sxs-lookup"><span data-stu-id="a0e23-259">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="a0e23-260">1010578050</span><span class="sxs-lookup"><span data-stu-id="a0e23-260">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-261">CustomerName</span><span class="sxs-lookup"><span data-stu-id="a0e23-261">CustomerName</span></span></td>
<td><p><span data-ttu-id="a0e23-262">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="a0e23-262">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="a0e23-263">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="a0e23-263">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="a0e23-264">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="a0e23-264">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-265">MPNID</span><span class="sxs-lookup"><span data-stu-id="a0e23-265">MPNID</span></span></td>
<td><p><span data-ttu-id="a0e23-266">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="a0e23-266">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="a0e23-267">4390934</span><span class="sxs-lookup"><span data-stu-id="a0e23-267">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-268">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="a0e23-268">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="a0e23-269">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="a0e23-269">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="a0e23-270">Ver [Desglosar por partner](#itemizebypartner)</span><span class="sxs-lookup"><span data-stu-id="a0e23-270">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="a0e23-271">4390934</span><span class="sxs-lookup"><span data-stu-id="a0e23-271">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-272">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="a0e23-272">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="a0e23-273">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="a0e23-273">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="a0e23-274">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="a0e23-274">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-275">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="a0e23-275">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="a0e23-276">Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="a0e23-276">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="a0e23-277">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="a0e23-277">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="a0e23-278">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="a0e23-278">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-279">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="a0e23-279">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="a0e23-280">Fecha de finalización del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="a0e23-280">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="a0e23-281">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="a0e23-281">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="a0e23-282">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="a0e23-282">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-283">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="a0e23-283">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="a0e23-284">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a0e23-284">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="a0e23-285">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="a0e23-285">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="a0e23-286">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="a0e23-286">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="a0e23-287">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="a0e23-287">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-288">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="a0e23-288">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="a0e23-289">Alias de la oferta de servicio.</span><span class="sxs-lookup"><span data-stu-id="a0e23-289">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="a0e23-290">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="a0e23-290">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-291">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="a0e23-291">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="a0e23-292">Línea de negocio de la oferta de servicio</span><span class="sxs-lookup"><span data-stu-id="a0e23-292">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="a0e23-293">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="a0e23-293">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-294">OrderID</span><span class="sxs-lookup"><span data-stu-id="a0e23-294">OrderID</span></span></td>
<td><p><span data-ttu-id="a0e23-295">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a0e23-295">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="a0e23-296">Puede ser útil para identificar la suscripción al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="a0e23-296">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="a0e23-297">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="a0e23-297">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-298">ServiceName</span><span class="sxs-lookup"><span data-stu-id="a0e23-298">ServiceName</span></span></td>
<td><p><span data-ttu-id="a0e23-299">Nombre del servicio de Azure en cuestión.</span><span class="sxs-lookup"><span data-stu-id="a0e23-299">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="a0e23-300">MÁQUINAS VIRTUALES</span><span class="sxs-lookup"><span data-stu-id="a0e23-300">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-301">ServiceType</span><span class="sxs-lookup"><span data-stu-id="a0e23-301">ServiceType</span></span></td>
<td><p><span data-ttu-id="a0e23-302">Tipo específico de servicio de Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="a0e23-302">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="a0e23-303">Bus de servicio: individual o paquete</span><span class="sxs-lookup"><span data-stu-id="a0e23-303">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="a0e23-304">Base de datos SQL Azure: edición Business o Web</span><span class="sxs-lookup"><span data-stu-id="a0e23-304">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-305">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="a0e23-305">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="a0e23-306">Identificador único específico para toda la estructura de precios y datos del servicio.</span><span class="sxs-lookup"><span data-stu-id="a0e23-306">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="a0e23-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="a0e23-307">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-308">Nombre de recurso</span><span class="sxs-lookup"><span data-stu-id="a0e23-308">Resource Name</span></span></td>
<td><p><span data-ttu-id="a0e23-309">Nombre del recurso de Azure.</span><span class="sxs-lookup"><span data-stu-id="a0e23-309">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="a0e23-310">Transferencia entrante de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="a0e23-310">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="a0e23-311">Transferencia saliente de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="a0e23-311">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-312">Region</span><span class="sxs-lookup"><span data-stu-id="a0e23-312">Region</span></span></td>
<td><p><span data-ttu-id="a0e23-313">La región a la que se aplica el uso.</span><span class="sxs-lookup"><span data-stu-id="a0e23-313">The region the usage applies to.</span></span> <span data-ttu-id="a0e23-314">Se usa principalmente para asignar tarifas a las transferencias de datos, ya que las tarifas varían según la región.</span><span class="sxs-lookup"><span data-stu-id="a0e23-314">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="a0e23-315">Asia Pacífico, Europa, América Latina, América del Norte</span><span class="sxs-lookup"><span data-stu-id="a0e23-315">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-316">SKU</span><span class="sxs-lookup"><span data-stu-id="a0e23-316">SKU</span></span></td>
<td><p><span data-ttu-id="a0e23-317">Identificador único de MSFT para la oferta</span><span class="sxs-lookup"><span data-stu-id="a0e23-317">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="a0e23-318">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="a0e23-318">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="a0e23-319">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="a0e23-319">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="a0e23-320">Un id. y una cantidad para desglosar las distintas clasificaciones de un servicio o un recurso en un período de facturación determinado.</span><span class="sxs-lookup"><span data-stu-id="a0e23-320">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="a0e23-321">Para clasificación en niveles de Azure, puede haber una clasificación hasta una cantidad determinada de unidades facturables y, posteriormente, una clasificación diferente.</span><span class="sxs-lookup"><span data-stu-id="a0e23-321">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="a0e23-322">1</span><span class="sxs-lookup"><span data-stu-id="a0e23-322">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-323">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="a0e23-323">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="a0e23-324">La cantidad de servicio consumida (horas, GB, etc.) durante el período de notificación.</span><span class="sxs-lookup"><span data-stu-id="a0e23-324">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="a0e23-325">También incluye cualquier uso no facturado de períodos anteriores.</span><span class="sxs-lookup"><span data-stu-id="a0e23-325">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="a0e23-326">11</span><span class="sxs-lookup"><span data-stu-id="a0e23-326">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-327">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="a0e23-327">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="a0e23-328">Unidades que se incluyen como parte de la oferta.</span><span class="sxs-lookup"><span data-stu-id="a0e23-328">Units included as part of the offer.</span></span> <span data-ttu-id="a0e23-329">No suele mostrarse en CSP.</span><span class="sxs-lookup"><span data-stu-id="a0e23-329">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="a0e23-330">0</span><span class="sxs-lookup"><span data-stu-id="a0e23-330">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="a0e23-331">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="a0e23-331">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="a0e23-332">Unidades que no se incluyen como parte de la oferta y que el partner debe abonar.</span><span class="sxs-lookup"><span data-stu-id="a0e23-332">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="a0e23-333">Equivale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="a0e23-333">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="a0e23-334">11</span><span class="sxs-lookup"><span data-stu-id="a0e23-334">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-335">ListPrice</span><span class="sxs-lookup"><span data-stu-id="a0e23-335">ListPrice</span></span></td>
<td><p><span data-ttu-id="a0e23-336">Precio de la oferta en vigor la fecha de inicio de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="a0e23-336">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="a0e23-337">0.0808 USD</span><span class="sxs-lookup"><span data-stu-id="a0e23-337">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-338">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="a0e23-338">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="a0e23-339">ListPrist x OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="a0e23-339">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="a0e23-340">0.085 USD</span><span class="sxs-lookup"><span data-stu-id="a0e23-340">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-341">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="a0e23-341">TaxAmount</span></span></td>
<td><p><span data-ttu-id="a0e23-342">Cargo por importe de impuestos, en función de las reglas fiscales de tu mercado y las circunstancias específicas.</span><span class="sxs-lookup"><span data-stu-id="a0e23-342">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="a0e23-343">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="a0e23-343">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-344">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="a0e23-344">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="a0e23-345">Total con impuestos, si se aplican impuestos.</span><span class="sxs-lookup"><span data-stu-id="a0e23-345">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="a0e23-346">0.93 USD</span><span class="sxs-lookup"><span data-stu-id="a0e23-346">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-347">Currency</span><span class="sxs-lookup"><span data-stu-id="a0e23-347">Currency</span></span></td>
<td><p><span data-ttu-id="a0e23-348">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="a0e23-348">Currency type.</span></span> <span data-ttu-id="a0e23-349">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="a0e23-349">Each billing entity has only one currency.</span></span> <span data-ttu-id="a0e23-350">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="a0e23-350">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="a0e23-351">EUR</span><span class="sxs-lookup"><span data-stu-id="a0e23-351">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-352">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="a0e23-352">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="a0e23-353">Precio sin impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="a0e23-353">Pretax price per unit.</span></span> <span data-ttu-id="a0e23-354">Igual que PretaxCharges/OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="a0e23-354">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="a0e23-355">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="a0e23-355">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-356">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="a0e23-356">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="a0e23-357">Precio después de impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="a0e23-357">Post tax price per unit.</span></span> <span data-ttu-id="a0e23-358">Igual que PostTaxTotal/OverageQuantity o PretaxEffectiveRate + tipo impositivo por importe unitario, redondeado el céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="a0e23-358">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="a0e23-359">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="a0e23-359">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-360">ChargeType</span><span class="sxs-lookup"><span data-stu-id="a0e23-360">ChargeType</span></span></td>
<td><p><span data-ttu-id="a0e23-361">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="a0e23-361">The type of charge or adjustment.</span></span> <span data-ttu-id="a0e23-362">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="a0e23-362">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="a0e23-363">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="a0e23-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-364">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="a0e23-364">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="a0e23-365">Id. de cuenta único en la plataforma de facturación de MSFT.</span><span class="sxs-lookup"><span data-stu-id="a0e23-365">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="a0e23-366">1280018095</span><span class="sxs-lookup"><span data-stu-id="a0e23-366">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-367">UsageDate</span><span class="sxs-lookup"><span data-stu-id="a0e23-367">UsageDate</span></span></td>
<td><p><span data-ttu-id="a0e23-368">Fecha de implementación del servicio.</span><span class="sxs-lookup"><span data-stu-id="a0e23-368">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="a0e23-369">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="a0e23-369">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-370">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="a0e23-370">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="a0e23-371">Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena.</span><span class="sxs-lookup"><span data-stu-id="a0e23-371">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="a0e23-372">Asia Oriental, Asia Suroriental, Norte de Europa, Europa Occidental, Centro-norte de EE.UU., Centro-sur de EE.UU.</span><span class="sxs-lookup"><span data-stu-id="a0e23-372">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-373">MeteredService</span><span class="sxs-lookup"><span data-stu-id="a0e23-373">MeteredService</span></span></td>
<td><p><span data-ttu-id="a0e23-374">Esta columna se usa para hacer un seguimiento de los servicios de Microsoft Azure individuales que quizás no se identifiquen específicamente en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="a0e23-374">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="a0e23-375">Por ejemplo, las transferencias de datos se notifican como &quot;Microsoft Azure: todos los servicios&quot; en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="a0e23-375">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="a0e23-376">En esta columna MeteredService se indicará qué servicio específico pertenece el uso.</span><span class="sxs-lookup"><span data-stu-id="a0e23-376">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="a0e23-377">AccessControl, CDN, Proceso, Base de datos, ServiceBus, Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="a0e23-377">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-378">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="a0e23-378">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="a0e23-379">Subtítulo que aclara el servicio de Microsoft Azure individual más allá del nivel proporcionado por el campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="a0e23-379">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="a0e23-380">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="a0e23-380">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-381">Proyecto</span><span class="sxs-lookup"><span data-stu-id="a0e23-381">Project</span></span></td>
<td><p><span data-ttu-id="a0e23-382">Nombre definido por el cliente para la instancia del servicio</span><span class="sxs-lookup"><span data-stu-id="a0e23-382">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="a0e23-383">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="a0e23-383">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-384">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="a0e23-384">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="a0e23-385">Número de conexiones de Bus de servicio aprovisionadas y usadas en un día determinado.</span><span class="sxs-lookup"><span data-stu-id="a0e23-385">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="a0e23-386">Por ejemplo: si tenías una conexión aprovisionada individualmente durante un mes de 30 días, Service Info 1 contendría 1 "1,000000 conexiones/30 días".</span><span class="sxs-lookup"><span data-stu-id="a0e23-386">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="a0e23-387">Si tenías un paquete de 25 de conexiones de Bus de servicio aprovisionadas y utilizaste 1 durante ese día, la declaración de uso diario de ese día sería "25 conexiones/30 días. Utilizadas: 1,000000".</span><span class="sxs-lookup"><span data-stu-id="a0e23-387">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-388">CustomerID</span><span class="sxs-lookup"><span data-stu-id="a0e23-388">CustomerID</span></span></td>
<td><p><span data-ttu-id="a0e23-389">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="a0e23-389">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="a0e23-390">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="a0e23-390">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="a0e23-391">DomainName</span><span class="sxs-lookup"><span data-stu-id="a0e23-391">DomainName</span></span></td>
<td><p><span data-ttu-id="a0e23-392">Nombre de dominio del cliente, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="a0e23-392">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="a0e23-393">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="a0e23-393">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="a0e23-394">Unidad</span><span class="sxs-lookup"><span data-stu-id="a0e23-394">Unit</span></span></td>
<td><p><span data-ttu-id="a0e23-395">La unidad del nombre del recurso</span><span class="sxs-lookup"><span data-stu-id="a0e23-395">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="a0e23-396">GB u HORAS</span><span class="sxs-lookup"><span data-stu-id="a0e23-396">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>



## <a href="" id="charge_types"></a><span data-ttu-id="a0e23-397">Asignación de cargos entre una factura y el archivo de conciliación</span><span class="sxs-lookup"><span data-stu-id="a0e23-397">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="a0e23-398">La factura proporciona un resumen de los cargos, mientras que el archivo de conciliación proporciona un desglose detallado de las transacciones de elementos de línea, incluidos los tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="a0e23-398">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="a0e23-399">Para hacer referencias cruzadas de cantidades de cargos entre el archivo de conciliación y la factura, puedes usar las opciones de filtro de Microsoft Excel para filtrar por tipo de cargo en el archivo de conciliación con el fin de asignar los cargos de facturación a un conjunto de desgloses de cargos del archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="a0e23-399">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="a0e23-400">Los archivos de conciliación, tanto basados en uso como en licencias, solo muestran cargos y transacciones relacionados con el uso (unidades consumidas y cargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="a0e23-400">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="a0e23-401">En el archivo de conciliación no aparecen devoluciones, descuentos o créditos excepcionales que aparecen en la factura como "Ajustes".</span><span class="sxs-lookup"><span data-stu-id="a0e23-401">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="a0e23-402">La siguiente tabla muestra las asignaciones entre una sección de factura y los tipos de cargo asociados que es posible que se muestren en los archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="a0e23-402">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="a0e23-403">Descripción del cargo de facturación</span><span class="sxs-lookup"><span data-stu-id="a0e23-403">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="a0e23-404">Descripción del cargo del archivo de conciliación (columna ChargeType)</span><span class="sxs-lookup"><span data-stu-id="a0e23-404">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="a0e23-405">¿Qué es este cargo?</span><span class="sxs-lookup"><span data-stu-id="a0e23-405">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="a0e23-406">¿Cómo asigno estos valores de ChargeType a la factura?</span><span class="sxs-lookup"><span data-stu-id="a0e23-406">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><strong><span data-ttu-id="a0e23-407">Cargos periódicos</span><span class="sxs-lookup"><span data-stu-id="a0e23-407">Recurring Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="a0e23-408">Prorrateo de instancia de cancelación</span><span class="sxs-lookup"><span data-stu-id="a0e23-408">Cancel instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-409">Cargos prorrateados reembolsados al cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="a0e23-409">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="a0e23-410">Desde el archivo basado en licencia, suma la columna <strong>Amount</strong>.</span><span class="sxs-lookup"><span data-stu-id="a0e23-410">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a0e23-411">Tarifa de ciclo</span><span class="sxs-lookup"><span data-stu-id="a0e23-411">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-412">Cargos periódicos de una suscripción</span><span class="sxs-lookup"><span data-stu-id="a0e23-412">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a0e23-413">Prorrateo de instancia de ciclo</span><span class="sxs-lookup"><span data-stu-id="a0e23-413">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-414">Cargos prorrateados evaluados del cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="a0e23-414">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a0e23-415">Tarifas prorrateadas al cancelar</span><span class="sxs-lookup"><span data-stu-id="a0e23-415">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-416">Reembolso prorrateado de la parte no usada del servicio tras la cancelación</span><span class="sxs-lookup"><span data-stu-id="a0e23-416">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a0e23-417">Tarifas prorrateadas al comprar</span><span class="sxs-lookup"><span data-stu-id="a0e23-417">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-418">Tarifas prorrateadas tras la compra</span><span class="sxs-lookup"><span data-stu-id="a0e23-418">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a0e23-419">Tarifa de compra</span><span class="sxs-lookup"><span data-stu-id="a0e23-419">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-420">Cargo inicial de una suscripción</span><span class="sxs-lookup"><span data-stu-id="a0e23-420">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a0e23-421">Tarifa prorrateada al renovar</span><span class="sxs-lookup"><span data-stu-id="a0e23-421">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-422">Tarifas prorrateadas tras la renovación de la suscripción</span><span class="sxs-lookup"><span data-stu-id="a0e23-422">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a0e23-423">Tarifa de renovación</span><span class="sxs-lookup"><span data-stu-id="a0e23-423">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-424">Cargo por renovar una suscripción</span><span class="sxs-lookup"><span data-stu-id="a0e23-424">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="a0e23-425">Otros productos y servicios</span><span class="sxs-lookup"><span data-stu-id="a0e23-425">Other Products and Services</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="a0e23-426">Tarifas prorrateadas al activar</span><span class="sxs-lookup"><span data-stu-id="a0e23-426">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-427">Tarifas prorrateadas desde la activación hasta el final del período de facturación</span><span class="sxs-lookup"><span data-stu-id="a0e23-427">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-428">Desde el archivo basado en licencia, suma la columna <strong>Amount</strong>.</span><span class="sxs-lookup"><span data-stu-id="a0e23-428">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="a0e23-429">Cargos de uso</span><span class="sxs-lookup"><span data-stu-id="a0e23-429">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="a0e23-430">Evaluar la tarifa de uso al cancelar</span><span class="sxs-lookup"><span data-stu-id="a0e23-430">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-431">Tarifa de uso de acceso tras la cancelación por uso impagado durante el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="a0e23-431">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="a0e23-432">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="a0e23-432">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a0e23-433">Evaluar la tarifa de uso para el ciclo actual</span><span class="sxs-lookup"><span data-stu-id="a0e23-433">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-434">tarifa de uso de acceso para el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="a0e23-434">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="a0e23-435">Créditos y ajustes</span><span class="sxs-lookup"><span data-stu-id="a0e23-435">Credits &amp; Adjustments</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="a0e23-436">Desplazamiento de un elemento de línea</span><span class="sxs-lookup"><span data-stu-id="a0e23-436">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-437">Reembolso parcial o total de un elemento de línea, incluidos impuestos</span><span class="sxs-lookup"><span data-stu-id="a0e23-437">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-438">Desde el archivo basado en licencia, suma la columna <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="a0e23-438">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="a0e23-439">Desde el archivo basado en uso, suma la columna <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="a0e23-439">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="a0e23-440">Otros descuentos</span><span class="sxs-lookup"><span data-stu-id="a0e23-440">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="a0e23-441">(basado en uso)</span><span class="sxs-lookup"><span data-stu-id="a0e23-441">(usage-based)</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="a0e23-442">Descuento de activación</span><span class="sxs-lookup"><span data-stu-id="a0e23-442">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-443">Descuento que se aplica cuando se activa la suscripción</span><span class="sxs-lookup"><span data-stu-id="a0e23-443">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="a0e23-444">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="a0e23-444">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a0e23-445">Descuento de ciclo</span><span class="sxs-lookup"><span data-stu-id="a0e23-445">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-446">Descuento que se aplica en cargos periódicos</span><span class="sxs-lookup"><span data-stu-id="a0e23-446">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="a0e23-447">Descuento de renovación</span><span class="sxs-lookup"><span data-stu-id="a0e23-447">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-448">Descuento que se aplica cuando se renueva la suscripción</span><span class="sxs-lookup"><span data-stu-id="a0e23-448">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="a0e23-449">Descuento de cancelación</span><span class="sxs-lookup"><span data-stu-id="a0e23-449">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-450">Cargos que se aplican cuando se cancelan los descuentos</span><span class="sxs-lookup"><span data-stu-id="a0e23-450">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="a0e23-451">Otros descuentos</span><span class="sxs-lookup"><span data-stu-id="a0e23-451">Other Discounts</span></span></strong></br>
<em><span data-ttu-id="a0e23-452">(basado en licencia)</span><span class="sxs-lookup"><span data-stu-id="a0e23-452">(license-based)</span></span></em></p>
</td>
<td>
<p><em><span data-ttu-id="a0e23-453">Se pueden aplicar a varios tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="a0e23-453">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="a0e23-454">Desde el archivo basado en licencia, suma la columna <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="a0e23-454">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="a0e23-455"><strong>Impuestos</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="a0e23-455"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="a0e23-456">Se pueden aplicar a varios tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="a0e23-456">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="a0e23-457">Excepción: "Desplazamiento de un elemento de línea" ya incluye impuestos.</span><span class="sxs-lookup"><span data-stu-id="a0e23-457">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="a0e23-458">Consulta Créditos y ajustes, más arriba.</span><span class="sxs-lookup"><span data-stu-id="a0e23-458">See Credits &amp; Adjustments, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="a0e23-459">Impuestos o impuesto de valor añadido (IVA)</span><span class="sxs-lookup"><span data-stu-id="a0e23-459">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="a0e23-460">Desde el archivo basado en licencia, suma la columna <strong>Tax</strong>.</span><span class="sxs-lookup"><span data-stu-id="a0e23-460">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="a0e23-461">Desde el archivo basado en uso, suma la columna <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="a0e23-461">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
