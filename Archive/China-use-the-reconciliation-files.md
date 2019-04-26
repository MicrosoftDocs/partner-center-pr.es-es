---
title: Use los archivos de conciliación (centro de partners operado por 21Vianet)
ms.topic: article
ms.date: 10/29/2018
description: Para obtener una vista detallada del elemento de línea de cada cargo en un ciclo de facturación, descarga los archivos de conciliación desde el panel del Centro de partners.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.openlocfilehash: 30e3b7a7933678c4af079bb86aa1439559387f2b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132085"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="58110-103">Usar los archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="58110-103">Use the reconciliation files</span></span>

<span data-ttu-id="58110-104">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="58110-104">**Applies to**</span></span>

-   <span data-ttu-id="58110-105">Centro de partners operado por 21Vianet</span><span class="sxs-lookup"><span data-stu-id="58110-105">Partner Center operated by 21Vianet</span></span>


<span data-ttu-id="58110-106">Para obtener una vista detallada del elemento de línea de cada cargo en un ciclo de facturación, descarga los archivos de conciliación desde el panel del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="58110-106">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from the Partner Center dashboard.</span></span> <span data-ttu-id="58110-107">Los detalles incluyen los cargos para las suscripciones de cada cliente y los eventos detallados (por ejemplo, una adición intermedia de puestos en una suscripción).</span><span class="sxs-lookup"><span data-stu-id="58110-107">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="58110-108">Detallar asociado</span><span class="sxs-lookup"><span data-stu-id="58110-108">Itemize by partner</span></span>


<span data-ttu-id="58110-109">Los partners del modelo indirecto pueden usar estos campos adicionales en ambos archivos de conciliación basada en uso y en licencia para realizar el desglose por revendedor.</span><span class="sxs-lookup"><span data-stu-id="58110-109">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="58110-110">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="58110-110">MPN ID</span></span></th>
<th><span data-ttu-id="58110-111">Descripción</span><span class="sxs-lookup"><span data-stu-id="58110-111">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="58110-112">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="58110-112">MPN ID</span></span></td>
<td><p><span data-ttu-id="58110-113">Id. de Microsoft Partner Network (MPN) del partner de CSP (directo o indirecto).</span><span class="sxs-lookup"><span data-stu-id="58110-113">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-114">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="58110-114">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="58110-115">Solo aparece en los archivos de conciliación de partners en el modelo indirecto.</span><span class="sxs-lookup"><span data-stu-id="58110-115">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="58110-116">El Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="58110-116">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="58110-117">Corresponde al id. de revendedor indicado para la suscripción específica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="58110-117">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="58110-118">Para ver o actualizar el revendedor, en el menú del Centro de partners, selecciona <strong>Clientes</strong> y, después, elige el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="58110-118">eTo view or update the reseller, in the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="58110-119">En el menú del cliente, selecciona <strong>Suscripciones</strong> y elige la suscripción de la lista.</span><span class="sxs-lookup"><span data-stu-id="58110-119">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="58110-120">Selecciona <strong>Actualizar</strong> para cambiar el valor de <strong>Revendedor (id. de MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="58110-120">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="58110-121">Si un partner CSP vendió la suscripción directamente al cliente, su id. de MPN aparece dos veces, como id. de MPN y como id. de MPN del revendedor.</span><span class="sxs-lookup"><span data-stu-id="58110-121">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="58110-122">Si un partner CSP tiene un revendedor sin un id. de MPN, este valor se establece en el id. de MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="58110-122">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="58110-123">Si el partner CSP quita un id. de revendedor, este valor se establece en -1.</span><span class="sxs-lookup"><span data-stu-id="58110-123">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="58110-124">Campos de archivo de licencia</span><span class="sxs-lookup"><span data-stu-id="58110-124">License-based file fields</span></span>


<span data-ttu-id="58110-125">Para conciliar los cargos en función de los pedidos del cliente, compara el Syndication\_Partner\_Subscription\_Number del archivo de conciliación con el id. de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="58110-125">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="58110-126"><strong>Columna</strong></span><span class="sxs-lookup"><span data-stu-id="58110-126"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="58110-127"><strong>Descripción</strong></span><span class="sxs-lookup"><span data-stu-id="58110-127"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="58110-128"><strong>Valor de ejemplo</strong></span><span class="sxs-lookup"><span data-stu-id="58110-128"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-129">PartnerId</span><span class="sxs-lookup"><span data-stu-id="58110-129">PartnerId</span></span></td>
<td><p><span data-ttu-id="58110-130">Identificador único de una entidad de facturación específica, con formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="58110-130">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="58110-131">No es necesario para la reconciliación, pero puede ser información útil.</span><span class="sxs-lookup"><span data-stu-id="58110-131">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="58110-132">Igual en todas las filas.</span><span class="sxs-lookup"><span data-stu-id="58110-132">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="58110-133">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="58110-133">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-134">CustomerID</span><span class="sxs-lookup"><span data-stu-id="58110-134">CustomerID</span></span></td>
<td><p><span data-ttu-id="58110-135">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="58110-135">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="58110-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="58110-136">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-137">OrderID</span><span class="sxs-lookup"><span data-stu-id="58110-137">OrderID</span></span></td>
<td><p><span data-ttu-id="58110-138">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="58110-138">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="58110-139">Puede ser útil para identificar al pedido al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="58110-139">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="58110-140">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="58110-140">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-141">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="58110-141">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="58110-142">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="58110-142">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="58110-143">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="58110-143">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="58110-144">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="58110-144">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="58110-145">Consulte Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="58110-145">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="58110-146">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="58110-146">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-147">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="58110-147">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="58110-148">Identificador único de las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="58110-148">Unique identifier for subscriptions.</span></span> <span data-ttu-id="58110-149">Un cliente puede tener varias suscripciones para el mismo plan, por lo que es importante para el análisis de archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="58110-149">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="58110-150">Este campo se asigna al identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="58110-150">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="58110-151">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="58110-151">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-152">OfferID</span><span class="sxs-lookup"><span data-stu-id="58110-152">OfferID</span></span></td>
<td><p><span data-ttu-id="58110-153">Identificador único de la oferta.</span><span class="sxs-lookup"><span data-stu-id="58110-153">Unique offer ID.</span></span> <span data-ttu-id="58110-154">Identificador de la oferta estándar según la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="58110-154">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="58110-155"><b>Nota</b>: Este valor no coincide con Id. de oferta desde la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="58110-155"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="58110-156">Consulta DurableOfferID a continuación.</span><span class="sxs-lookup"><span data-stu-id="58110-156">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="58110-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="58110-157">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-158">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="58110-158">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="58110-159">Identificador único de oferta duradera, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="58110-159">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="58110-160"><b>Nota</b>: Este valor coincide con el Id. de oferta desde la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="58110-160"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="58110-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="58110-161">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-162">OfferName</span><span class="sxs-lookup"><span data-stu-id="58110-162">OfferName</span></span></td>
<td><p><span data-ttu-id="58110-163">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="58110-163">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="58110-164">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="58110-164">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-165">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="58110-165">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="58110-166">Fecha de finalización de la suscripción, establecida en el día posterior al envío del pedido.</span><span class="sxs-lookup"><span data-stu-id="58110-166">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="58110-167">Al consultar la fecha de inicio de la suscripción junto con la fecha de finalización, puedes determinar si el cliente aún está dentro del primer año de la suscripción o si la suscripción se ha renovado para el año siguiente.</span><span class="sxs-lookup"><span data-stu-id="58110-167">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="58110-168">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="58110-168">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="58110-169">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="58110-169">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-170">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="58110-170">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="58110-171">La fecha de finalización de la suscripción: 12 meses + x días después de la fecha de inicio (para alinearse con fecha de facturación del asociado) o 12 meses a partir de la fecha de renovación.</span><span class="sxs-lookup"><span data-stu-id="58110-171">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="58110-172">En el momento de la renovación, los precios se actualizan según la lista de precios actual.</span><span class="sxs-lookup"><span data-stu-id="58110-172">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="58110-173">Es posible que se necesite una comunicación con el cliente antes de la renovación automatizada.</span><span class="sxs-lookup"><span data-stu-id="58110-173">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="58110-174">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="58110-174">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="58110-175">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="58110-175">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-176">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="58110-176">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="58110-177">Día de inicio de los cargos.</span><span class="sxs-lookup"><span data-stu-id="58110-177">Start day of the charges.</span></span></p>
<p><span data-ttu-id="58110-178">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="58110-178">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="58110-179">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="58110-179">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="58110-180">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="58110-180">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-181">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="58110-181">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="58110-182">Día de finalización de los cargos.</span><span class="sxs-lookup"><span data-stu-id="58110-182">End day of the charges.</span></span></p>
<p><span data-ttu-id="58110-183">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="58110-183">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="58110-184">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="58110-184">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="58110-185">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="58110-185">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-186">ChargeType</span><span class="sxs-lookup"><span data-stu-id="58110-186">ChargeType</span></span></td>
<td><p><span data-ttu-id="58110-187">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="58110-187">The type of charge or adjustment.</span></span> <span data-ttu-id="58110-188">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="58110-188">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="58110-189">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="58110-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-190">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="58110-190">UnitPrice</span></span></td>
<td><p><span data-ttu-id="58110-191">Precio por puesto.</span><span class="sxs-lookup"><span data-stu-id="58110-191">Price per seat.</span></span> <span data-ttu-id="58110-192">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="58110-192">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="58110-193">6.82</span><span class="sxs-lookup"><span data-stu-id="58110-193">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-194">Cantidad</span><span class="sxs-lookup"><span data-stu-id="58110-194">Quantity</span></span></td>
<td><p><span data-ttu-id="58110-195">Número de puestos.</span><span class="sxs-lookup"><span data-stu-id="58110-195">Number of seats.</span></span> <span data-ttu-id="58110-196">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="58110-196">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="58110-197">2</span><span class="sxs-lookup"><span data-stu-id="58110-197">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-198">Volumen</span><span class="sxs-lookup"><span data-stu-id="58110-198">Amount</span></span></td>
<td><p><span data-ttu-id="58110-199">Total del precio para la cantidad.</span><span class="sxs-lookup"><span data-stu-id="58110-199">Total of price for quantity.</span></span> <span data-ttu-id="58110-200">Es de utilidad para comprobar que el cálculo de la cantidad coincide con la manera de calcular este valor para los clientes.</span><span class="sxs-lookup"><span data-stu-id="58110-200">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="58110-201">13.32</span><span class="sxs-lookup"><span data-stu-id="58110-201">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-202">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="58110-202">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="58110-203">Cantidad de descuento que se aplica a estos cargos.</span><span class="sxs-lookup"><span data-stu-id="58110-203">Amount of discount applied to these charges.</span></span> <span data-ttu-id="58110-204">Los IUR o las nuevas suscripciones que puedan optar a un incentivo también incluirán un importe de descuento en esta columna.</span><span class="sxs-lookup"><span data-stu-id="58110-204">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="58110-205">2.32</span><span class="sxs-lookup"><span data-stu-id="58110-205">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-206">Subtotal</span><span class="sxs-lookup"><span data-stu-id="58110-206">Subtotal</span></span></td>
<td><p><span data-ttu-id="58110-207">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="58110-207">Total before tax.</span></span> <span data-ttu-id="58110-208">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="58110-208">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="58110-209">11</span><span class="sxs-lookup"><span data-stu-id="58110-209">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-210">Impuestos</span><span class="sxs-lookup"><span data-stu-id="58110-210">Tax</span></span></td>
<td><p><span data-ttu-id="58110-211">Cargo por importe de impuestos, en función de las reglas fiscales de tu mercado y las circunstancias específicas.</span><span class="sxs-lookup"><span data-stu-id="58110-211">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="58110-212">0</span><span class="sxs-lookup"><span data-stu-id="58110-212">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-213">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="58110-213">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="58110-214">Total con impuestos.</span><span class="sxs-lookup"><span data-stu-id="58110-214">Total after tax.</span></span> <span data-ttu-id="58110-215">Comprueba si se cobran impuestos en la factura.</span><span class="sxs-lookup"><span data-stu-id="58110-215">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="58110-216">11</span><span class="sxs-lookup"><span data-stu-id="58110-216">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-217">Moneda</span><span class="sxs-lookup"><span data-stu-id="58110-217">Currency</span></span></td>
<td><p><span data-ttu-id="58110-218">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="58110-218">Currency type.</span></span> <span data-ttu-id="58110-219">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="58110-219">Each billing entity has only one currency.</span></span> <span data-ttu-id="58110-220">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="58110-220">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="58110-221">CNY</span><span class="sxs-lookup"><span data-stu-id="58110-221">CNY</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-222">CustomerName</span><span class="sxs-lookup"><span data-stu-id="58110-222">CustomerName</span></span></td>
<td><p><span data-ttu-id="58110-223">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="58110-223">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="58110-224">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="58110-224">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="58110-225">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="58110-225">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-226">MPNID</span><span class="sxs-lookup"><span data-stu-id="58110-226">MPNID</span></span></td>
<td><p><span data-ttu-id="58110-227">Id. de MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="58110-227">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="58110-228">4390934</span><span class="sxs-lookup"><span data-stu-id="58110-228">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-229">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="58110-229">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="58110-230">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="58110-230">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="58110-231">Ver [Desglosar por partner](#itemizebypartner)</span><span class="sxs-lookup"><span data-stu-id="58110-231">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="58110-232">4390934</span><span class="sxs-lookup"><span data-stu-id="58110-232">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-233">DomainName</span><span class="sxs-lookup"><span data-stu-id="58110-233">DomainName</span></span></td>
<td><p><span data-ttu-id="58110-234">Nombre de dominio del cliente, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="58110-234">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="58110-235">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="58110-235">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-236">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="58110-236">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="58110-237">Alias de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="58110-237">Subscription nickname.</span></span> <span data-ttu-id="58110-238">Si no se especifica ningún alias, el Centro de partners usa OfferName.</span><span class="sxs-lookup"><span data-stu-id="58110-238">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="58110-239">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="58110-239">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-240">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="58110-240">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="58110-241">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="58110-241">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="58110-242">(Este es un campo idéntico al nombre de la oferta).</span><span class="sxs-lookup"><span data-stu-id="58110-242">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="58110-243">PROJECT ONLINE PREMIUM SIN CLIENTE DE PROJECT</span><span class="sxs-lookup"><span data-stu-id="58110-243">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="58110-244">Campos de archivo basada en uso</span><span class="sxs-lookup"><span data-stu-id="58110-244">Usage-based file fields</span></span>


<span data-ttu-id="58110-245">Para conciliar los cargos en función del uso de tu cliente, compara los valores de ResellerID/ResellerName/ResellerBillableAccount del archivo de conciliación, el nombre del cliente y el id. de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="58110-245">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="58110-246">Los siguientes campos explican los servicios usados y la clasificación.</span><span class="sxs-lookup"><span data-stu-id="58110-246">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="58110-247"><strong>Columna</strong></span><span class="sxs-lookup"><span data-stu-id="58110-247"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="58110-248"><strong>Descripción</strong></span><span class="sxs-lookup"><span data-stu-id="58110-248"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="58110-249"><strong>Valor de ejemplo</strong></span><span class="sxs-lookup"><span data-stu-id="58110-249"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-250">PartnerID</span><span class="sxs-lookup"><span data-stu-id="58110-250">PartnerID</span></span></td>
<td><p><span data-ttu-id="58110-251">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="58110-251">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="58110-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="58110-252">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-253">PartnerName</span><span class="sxs-lookup"><span data-stu-id="58110-253">PartnerName</span></span></td>
<td><p><span data-ttu-id="58110-254">Nombre del partner.</span><span class="sxs-lookup"><span data-stu-id="58110-254">Partner Name.</span></span></p></td>
<td><span data-ttu-id="58110-255">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="58110-255">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-256">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="58110-256">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="58110-257">Id. de cuenta del partner.</span><span class="sxs-lookup"><span data-stu-id="58110-257">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="58110-258">1010578050</span><span class="sxs-lookup"><span data-stu-id="58110-258">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-259">CustomerName</span><span class="sxs-lookup"><span data-stu-id="58110-259">CustomerName</span></span></td>
<td><p><span data-ttu-id="58110-260">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="58110-260">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="58110-261">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="58110-261">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="58110-262">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="58110-262">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-263">MPNID</span><span class="sxs-lookup"><span data-stu-id="58110-263">MPNID</span></span></td>
<td><p><span data-ttu-id="58110-264">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="58110-264">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="58110-265">4390934</span><span class="sxs-lookup"><span data-stu-id="58110-265">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-266">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="58110-266">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="58110-267">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="58110-267">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="58110-268">Ver [Desglosar por partner](#itemizebypartner)</span><span class="sxs-lookup"><span data-stu-id="58110-268">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="58110-269">4390934</span><span class="sxs-lookup"><span data-stu-id="58110-269">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-270">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="58110-270">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="58110-271">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="58110-271">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="58110-272">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="58110-272">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-273">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="58110-273">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="58110-274">Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="58110-274">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="58110-275">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="58110-275">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="58110-276">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="58110-276">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-277">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="58110-277">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="58110-278">Fecha de finalización del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="58110-278">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="58110-279">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="58110-279">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="58110-280">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="58110-280">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-281">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="58110-281">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="58110-282">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="58110-282">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="58110-283">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="58110-283">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="58110-284">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="58110-284">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="58110-285">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="58110-285">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-286">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="58110-286">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="58110-287">Alias de la oferta de servicio.</span><span class="sxs-lookup"><span data-stu-id="58110-287">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="58110-288">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="58110-288">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-289">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="58110-289">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="58110-290">Línea de negocio de la oferta de servicio</span><span class="sxs-lookup"><span data-stu-id="58110-290">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="58110-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="58110-291">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-292">OrderID</span><span class="sxs-lookup"><span data-stu-id="58110-292">OrderID</span></span></td>
<td><p><span data-ttu-id="58110-293">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="58110-293">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="58110-294">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="58110-294">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="58110-295">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="58110-295">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-296">ServiceName</span><span class="sxs-lookup"><span data-stu-id="58110-296">ServiceName</span></span></td>
<td><p><span data-ttu-id="58110-297">Nombre del servicio de Azure en cuestión.</span><span class="sxs-lookup"><span data-stu-id="58110-297">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="58110-298">MÁQUINAS VIRTUALES</span><span class="sxs-lookup"><span data-stu-id="58110-298">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-299">ServiceType</span><span class="sxs-lookup"><span data-stu-id="58110-299">ServiceType</span></span></td>
<td><p><span data-ttu-id="58110-300">Tipo específico de servicio de Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="58110-300">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="58110-301">Bus de servicio: individual o paquete</span><span class="sxs-lookup"><span data-stu-id="58110-301">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="58110-302">Base de datos SQL Azure: edición Business o Web</span><span class="sxs-lookup"><span data-stu-id="58110-302">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-303">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="58110-303">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="58110-304">Identificador único específico para toda la estructura de precios y datos del servicio.</span><span class="sxs-lookup"><span data-stu-id="58110-304">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="58110-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="58110-305">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-306">Nombre de recurso</span><span class="sxs-lookup"><span data-stu-id="58110-306">Resource Name</span></span></td>
<td><p><span data-ttu-id="58110-307">Nombre del recurso de Azure.</span><span class="sxs-lookup"><span data-stu-id="58110-307">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="58110-308">Transferencia entrante de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="58110-308">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="58110-309">Transferencia saliente de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="58110-309">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-310">Region</span><span class="sxs-lookup"><span data-stu-id="58110-310">Region</span></span></td>
<td><p><span data-ttu-id="58110-311">La región a la que se aplica el uso.</span><span class="sxs-lookup"><span data-stu-id="58110-311">The region the usage applies to.</span></span> <span data-ttu-id="58110-312">Se usa principalmente para asignar tarifas a las transferencias de datos, ya que las tarifas varían según la región.</span><span class="sxs-lookup"><span data-stu-id="58110-312">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="58110-313">Asia Pacífico, Europa, América Latina, América del Norte</span><span class="sxs-lookup"><span data-stu-id="58110-313">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-314">SKU</span><span class="sxs-lookup"><span data-stu-id="58110-314">SKU</span></span></td>
<td><p><span data-ttu-id="58110-315">Identificador único de MSFT para la oferta</span><span class="sxs-lookup"><span data-stu-id="58110-315">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="58110-316">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="58110-316">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="58110-317">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="58110-317">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="58110-318">Un id. y una cantidad para desglosar las distintas clasificaciones de un servicio o un recurso en un período de facturación determinado.</span><span class="sxs-lookup"><span data-stu-id="58110-318">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="58110-319">Para clasificación en niveles de Azure, puede haber una clasificación hasta una cantidad determinada de unidades facturables y, posteriormente, una clasificación diferente.</span><span class="sxs-lookup"><span data-stu-id="58110-319">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="58110-320">1</span><span class="sxs-lookup"><span data-stu-id="58110-320">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-321">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="58110-321">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="58110-322">La cantidad de servicio consumida (horas, GB, etc.) durante el período de notificación.</span><span class="sxs-lookup"><span data-stu-id="58110-322">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="58110-323">También incluye cualquier uso no facturado de períodos anteriores.</span><span class="sxs-lookup"><span data-stu-id="58110-323">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="58110-324">11</span><span class="sxs-lookup"><span data-stu-id="58110-324">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-325">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="58110-325">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="58110-326">Unidades que se incluyen como parte de la oferta.</span><span class="sxs-lookup"><span data-stu-id="58110-326">Units included as part of the offer.</span></span> <span data-ttu-id="58110-327">No suele mostrarse en CSP.</span><span class="sxs-lookup"><span data-stu-id="58110-327">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="58110-328">0</span><span class="sxs-lookup"><span data-stu-id="58110-328">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="58110-329">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="58110-329">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="58110-330">Unidades que no se incluyen como parte de la oferta y que el partner debe abonar.</span><span class="sxs-lookup"><span data-stu-id="58110-330">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="58110-331">Equivale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="58110-331">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="58110-332">11</span><span class="sxs-lookup"><span data-stu-id="58110-332">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-333">ListPrice</span><span class="sxs-lookup"><span data-stu-id="58110-333">ListPrice</span></span></td>
<td><p><span data-ttu-id="58110-334">Precio de la oferta en vigor la fecha de inicio de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="58110-334">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="58110-335">0.0808 USD</span><span class="sxs-lookup"><span data-stu-id="58110-335">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-336">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="58110-336">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="58110-337">ListPrist x OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="58110-337">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="58110-338">0.085 USD</span><span class="sxs-lookup"><span data-stu-id="58110-338">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-339">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="58110-339">TaxAmount</span></span></td>
<td><p><span data-ttu-id="58110-340">Cargo por importe de impuestos, en función de las reglas fiscales de tu mercado y las circunstancias específicas.</span><span class="sxs-lookup"><span data-stu-id="58110-340">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="58110-341">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="58110-341">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-342">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="58110-342">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="58110-343">Total con impuestos, si se aplican impuestos.</span><span class="sxs-lookup"><span data-stu-id="58110-343">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="58110-344">0.93 USD</span><span class="sxs-lookup"><span data-stu-id="58110-344">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-345">Moneda</span><span class="sxs-lookup"><span data-stu-id="58110-345">Currency</span></span></td>
<td><p><span data-ttu-id="58110-346">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="58110-346">Currency type.</span></span> <span data-ttu-id="58110-347">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="58110-347">Each billing entity has only one currency.</span></span> <span data-ttu-id="58110-348">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="58110-348">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="58110-349">CNY</span><span class="sxs-lookup"><span data-stu-id="58110-349">CNY</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-350">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="58110-350">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="58110-351">Precio sin impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="58110-351">Pretax price per unit.</span></span> <span data-ttu-id="58110-352">Igual que PretaxCharges/OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="58110-352">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="58110-353">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="58110-353">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-354">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="58110-354">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="58110-355">Precio después de impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="58110-355">Post tax price per unit.</span></span> <span data-ttu-id="58110-356">Igual que PostTaxTotal/OverageQuantity o PretaxEffectiveRate + tipo impositivo por importe unitario, redondeado el céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="58110-356">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="58110-357">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="58110-357">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-358">ChargeType</span><span class="sxs-lookup"><span data-stu-id="58110-358">ChargeType</span></span></td>
<td><p><span data-ttu-id="58110-359">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="58110-359">The type of charge or adjustment.</span></span> <span data-ttu-id="58110-360">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="58110-360">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="58110-361">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="58110-361">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-362">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="58110-362">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="58110-363">Id. de cuenta único en la plataforma de facturación de MSFT.</span><span class="sxs-lookup"><span data-stu-id="58110-363">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="58110-364">1280018095</span><span class="sxs-lookup"><span data-stu-id="58110-364">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-365">UsageDate</span><span class="sxs-lookup"><span data-stu-id="58110-365">UsageDate</span></span></td>
<td><p><span data-ttu-id="58110-366">Fecha de implementación del servicio.</span><span class="sxs-lookup"><span data-stu-id="58110-366">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="58110-367">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="58110-367">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-368">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="58110-368">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="58110-369">Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena.</span><span class="sxs-lookup"><span data-stu-id="58110-369">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="58110-370">Asia oriental, Sur asiático, Norte de Europa, Europa occidental, Norte central de EE. UU., Sur central de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="58110-370">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-371">MeteredService</span><span class="sxs-lookup"><span data-stu-id="58110-371">MeteredService</span></span></td>
<td><p><span data-ttu-id="58110-372">Esta columna se usa para hacer un seguimiento de los servicios de Microsoft Azure individuales que quizás no se identifiquen específicamente en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="58110-372">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="58110-373">Por ejemplo, las transferencias de datos se notifican como &quot;Microsoft Azure: todos los servicios&quot; en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="58110-373">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="58110-374">En esta columna MeteredService se indicará qué servicio específico pertenece el uso.</span><span class="sxs-lookup"><span data-stu-id="58110-374">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="58110-375">AccessControl, CDN, Proceso, Base de datos, ServiceBus, Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="58110-375">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-376">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="58110-376">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="58110-377">Subtítulo que aclara el servicio de Microsoft Azure individual más allá del nivel proporcionado por el campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="58110-377">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="58110-378">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="58110-378">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-379">Proyecto</span><span class="sxs-lookup"><span data-stu-id="58110-379">Project</span></span></td>
<td><p><span data-ttu-id="58110-380">Nombre definido por el cliente para la instancia del servicio</span><span class="sxs-lookup"><span data-stu-id="58110-380">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="58110-381">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="58110-381">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-382">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="58110-382">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="58110-383">Número de conexiones de Bus de servicio aprovisionadas y usadas en un día determinado.</span><span class="sxs-lookup"><span data-stu-id="58110-383">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="58110-384">Por ejemplo: si tenías una conexión aprovisionada individualmente durante un mes de 30 días, Service Info 1 contendría 1 "1,000000 conexiones/30 días".</span><span class="sxs-lookup"><span data-stu-id="58110-384">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="58110-385">Si tuviera un paquete de 25 de conexiones de bus de servicio aprovisionada y ha utilizado 1 durante ese día, el extracto de uso diario durante ese día indicaría "25 conexiones / 30 días: utilizado: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="58110-385">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="58110-386">CustomerID</span><span class="sxs-lookup"><span data-stu-id="58110-386">CustomerID</span></span></td>
<td><p><span data-ttu-id="58110-387">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="58110-387">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="58110-388">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="58110-388">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="58110-389">DomainName</span><span class="sxs-lookup"><span data-stu-id="58110-389">DomainName</span></span></td>
<td><p><span data-ttu-id="58110-390">Nombre de dominio del cliente, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="58110-390">Customer's domain name, used to help identify the customer.</span></span></p></td>
<td><span data-ttu-id="58110-391">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="58110-391">example.onmicrosoft.com</span></span></td></tr>
</tbody>
</table>



## <a href="" id="charge_types"></a><span data-ttu-id="58110-392">Asignación de cargos entre una factura y el archivo de conciliación</span><span class="sxs-lookup"><span data-stu-id="58110-392">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="58110-393">La factura proporciona un resumen de los cargos, mientras que el archivo de conciliación proporciona un desglose detallado de las transacciones de elementos de línea, incluidos los tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="58110-393">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="58110-394">Para hacer referencias cruzadas de cantidades de cargos entre el archivo de conciliación y la factura, puedes usar las opciones de filtro de Microsoft Excel para filtrar por tipo de cargo en el archivo de conciliación con el fin de asignar los cargos de facturación a un conjunto de desgloses de cargos del archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="58110-394">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="58110-395">La siguiente tabla muestra las asignaciones entre una sección de factura y los tipos de cargo asociados que es posible que se muestren en los archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="58110-395">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="58110-396"><strong>Descripción de cargos de facturación</strong></span><span class="sxs-lookup"><span data-stu-id="58110-396"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-397"><strong>Descripción de cargos del archivo de conciliación (columna ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="58110-397"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-398"><strong>¿Qué es este cargo?</strong></span><span class="sxs-lookup"><span data-stu-id="58110-398"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-399"><strong>¿Cómo se asignan estos ChargeTypes a la factura?</strong></span><span class="sxs-lookup"><span data-stu-id="58110-399"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="8">
<p><span data-ttu-id="58110-400"><strong>Cargos periódicos</strong></span><span class="sxs-lookup"><span data-stu-id="58110-400"><strong>Recurring Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-401">Prorrateo de instancia de cancelación</span><span class="sxs-lookup"><span data-stu-id="58110-401">Cancel instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-402">Cargos prorrateados reembolsados al cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="58110-402">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
<td rowspan="8">
<p><span data-ttu-id="58110-403">Desde el archivo basado en licencia, suma la columna <strong>Amount</strong>.</span><span class="sxs-lookup"><span data-stu-id="58110-403">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58110-404">Tarifa de ciclo</span><span class="sxs-lookup"><span data-stu-id="58110-404">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-405">Cargos periódicos de una suscripción</span><span class="sxs-lookup"><span data-stu-id="58110-405">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58110-406">Prorrateo de instancia de ciclo</span><span class="sxs-lookup"><span data-stu-id="58110-406">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-407">Cargos prorrateados evaluados del cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="58110-407">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58110-408">Tarifas prorrateadas al cancelar</span><span class="sxs-lookup"><span data-stu-id="58110-408">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-409">Reembolso prorrateado de la parte no usada del servicio tras la cancelación</span><span class="sxs-lookup"><span data-stu-id="58110-409">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58110-410">Tarifas prorrateadas al comprar</span><span class="sxs-lookup"><span data-stu-id="58110-410">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-411">Tarifas prorrateadas tras la compra</span><span class="sxs-lookup"><span data-stu-id="58110-411">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58110-412">Tarifa de compra</span><span class="sxs-lookup"><span data-stu-id="58110-412">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-413">Cargo inicial de una suscripción</span><span class="sxs-lookup"><span data-stu-id="58110-413">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58110-414">Tarifa prorrateada al renovar</span><span class="sxs-lookup"><span data-stu-id="58110-414">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-415">Tarifas prorrateadas tras la renovación de la suscripción</span><span class="sxs-lookup"><span data-stu-id="58110-415">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58110-416">Tarifa de renovación</span><span class="sxs-lookup"><span data-stu-id="58110-416">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-417">Cargo por renovar una suscripción</span><span class="sxs-lookup"><span data-stu-id="58110-417">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58110-418"><strong>Otros productos y servicios</strong></span><span class="sxs-lookup"><span data-stu-id="58110-418"><strong>Other Products and Services</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-419">Tarifas prorrateadas al activar</span><span class="sxs-lookup"><span data-stu-id="58110-419">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-420">Tarifas prorrateadas desde la activación hasta el final del período de facturación</span><span class="sxs-lookup"><span data-stu-id="58110-420">Prorated fees from activation until end of billing period</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-421">Desde el archivo basado en licencia, suma la columna <strong>Amount</strong>.</span><span class="sxs-lookup"><span data-stu-id="58110-421">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="58110-422"><strong>Cargos de uso</strong></span><span class="sxs-lookup"><span data-stu-id="58110-422"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-423">Evaluar la tarifa de uso al cancelar</span><span class="sxs-lookup"><span data-stu-id="58110-423">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-424">Tarifa de uso de acceso tras la cancelación por uso impagado durante el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="58110-424">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="58110-425">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="58110-425">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58110-426">Evaluar la tarifa de uso para el ciclo actual</span><span class="sxs-lookup"><span data-stu-id="58110-426">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-427">tarifa de uso de acceso para el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="58110-427">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58110-428"><strong>Créditos &amp; ajustes</strong></span><span class="sxs-lookup"><span data-stu-id="58110-428"><strong>Credits &amp; Adjustments</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-429">Desplazamiento de un elemento de línea</span><span class="sxs-lookup"><span data-stu-id="58110-429">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-430">Reembolso parcial o total de un elemento de línea, incluidos impuestos</span><span class="sxs-lookup"><span data-stu-id="58110-430">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-431">Desde el archivo basado en licencia, suma la columna <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="58110-431">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="58110-432">Desde el archivo basado en uso, suma la columna <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="58110-432">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>


<tr>
<td rowspan="4">
<p><span data-ttu-id="58110-433"><strong>Otros descuentos</strong></span><span class="sxs-lookup"><span data-stu-id="58110-433"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="58110-434">
<em>(usage-based)</em></span><span class="sxs-lookup"><span data-stu-id="58110-434">
<em>(usage-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-435">Descuento de activación</span><span class="sxs-lookup"><span data-stu-id="58110-435">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-436">Descuento que se aplica cuando se activa la suscripción</span><span class="sxs-lookup"><span data-stu-id="58110-436">Discount applied when subscription activated</span></span></p>
</td>
<td rowspan="4">
<p><span data-ttu-id="58110-437">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="58110-437">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58110-438">Descuento de ciclo</span><span class="sxs-lookup"><span data-stu-id="58110-438">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-439">Descuento que se aplica en cargos periódicos</span><span class="sxs-lookup"><span data-stu-id="58110-439">Discount applied on periodic charges</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="58110-440">Descuento de renovación</span><span class="sxs-lookup"><span data-stu-id="58110-440">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-441">Descuento que se aplica cuando se renueva la suscripción</span><span class="sxs-lookup"><span data-stu-id="58110-441">Discount applied when subscription renewed</span></span></p>
</td>
</tr><tr>
<td>
<p><span data-ttu-id="58110-442">Descuento de cancelación</span><span class="sxs-lookup"><span data-stu-id="58110-442">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-443">Cargos que se aplican cuando se cancelan los descuentos</span><span class="sxs-lookup"><span data-stu-id="58110-443">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58110-444"><strong>Otros descuentos</strong></span><span class="sxs-lookup"><span data-stu-id="58110-444"><strong>Other Discounts</strong></span></span></br><span data-ttu-id="58110-445">
<em>(basados en licencias)</em></span><span class="sxs-lookup"><span data-stu-id="58110-445">
<em>(license-based)</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-446"><em>Se pueden aplicar a varios tipos de cargos</em></span><span class="sxs-lookup"><span data-stu-id="58110-446"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p>&nbsp;</p>
</td>
<td>
<p><span data-ttu-id="58110-447">Desde el archivo basado en licencia, suma la columna <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="58110-447">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="58110-448"><strong>Impuestos</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="58110-448"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-449"><em>Se pueden aplicar a varios tipos de cargos</em></span><span class="sxs-lookup"><span data-stu-id="58110-449"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="58110-450"><em>Excepción: Ya se "Compensación de un elemento de la línea" incluye los impuestos. Consulte créditos &amp; ajustes, más arriba.</em></span><span class="sxs-lookup"><span data-stu-id="58110-450"><em>Exception: "Offset a line item" already includes taxes. See Credits &amp; Adjustments, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-451">Impuestos o impuesto de valor añadido (IVA)</span><span class="sxs-lookup"><span data-stu-id="58110-451">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="58110-452">Desde el archivo basado en licencia, suma la columna <strong>Tax</strong>.</span><span class="sxs-lookup"><span data-stu-id="58110-452">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="58110-453">Desde el archivo basado en uso, suma la columna <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="58110-453">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
