---
title: Usar los archivos de conciliación | Centro de partners
ms.topic: article
ms.date: 10/29/2018
description: Para obtener una vista detallada del elemento de línea de cada cargo en un ciclo de facturación, descarga los archivos de conciliación del centro de partners.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: KPacquer
ms.author: kenpacq
ms.localizationpriority: medium
ms.openlocfilehash: 4b5fbab84c30743e4d91b32bf4cbd2bb8b950992
ms.sourcegitcommit: b433061dff8f667c81b623c33417fb490d8e3b4a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/04/2018
ms.locfileid: "6022238"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="44be6-103">Usar los archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="44be6-103">Use the reconciliation files</span></span>

**<span data-ttu-id="44be6-104">Se aplica a</span><span class="sxs-lookup"><span data-stu-id="44be6-104">Applies to</span></span>**

-  <span data-ttu-id="44be6-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="44be6-105">Partner Center</span></span>
-  <span data-ttu-id="44be6-106">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="44be6-106">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="44be6-107">Centro de partners para Microsoft Cloud Alemania</span><span class="sxs-lookup"><span data-stu-id="44be6-107">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="44be6-108">Para obtener una vista detallada del elemento de línea de cada cargo en un ciclo de facturación, descarga los archivos de conciliación del centro de partners.</span><span class="sxs-lookup"><span data-stu-id="44be6-108">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="44be6-109">Los detalles incluyen los cargos para las suscripciones de cada cliente y los eventos detallados (por ejemplo, una adición intermedia de puestos en una suscripción).</span><span class="sxs-lookup"><span data-stu-id="44be6-109">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="44be6-110">Desglosar por partner</span><span class="sxs-lookup"><span data-stu-id="44be6-110">Itemize by partner</span></span>


<span data-ttu-id="44be6-111">Los partners del modelo indirecto pueden usar estos campos adicionales en ambos archivos de conciliación basada en uso y en licencia para realizar el desglose por revendedor.</span><span class="sxs-lookup"><span data-stu-id="44be6-111">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="44be6-112">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="44be6-112">MPN ID</span></span></th>
<th><span data-ttu-id="44be6-113">Descripción</span><span class="sxs-lookup"><span data-stu-id="44be6-113">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="44be6-114">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="44be6-114">MPN ID</span></span></td>
<td><p><span data-ttu-id="44be6-115">Id. de Microsoft Partner Network (MPN) del partner de CSP (directo o indirecto).</span><span class="sxs-lookup"><span data-stu-id="44be6-115">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-116">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="44be6-116">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="44be6-117">Solo aparece en los archivos de conciliación de partners en el modelo indirecto.</span><span class="sxs-lookup"><span data-stu-id="44be6-117">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="44be6-118">El Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="44be6-118">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="44be6-119">Corresponde al id. de revendedor indicado para la suscripción específica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="44be6-119">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="44be6-120">Para ver o actualizar el revendedor, en el menú del centro de partners, selecciona <strong>los clientes</strong>y luego elige el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="44be6-120">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="44be6-121">En el menú del cliente, selecciona <strong>Suscripciones</strong> y elige la suscripción de la lista.</span><span class="sxs-lookup"><span data-stu-id="44be6-121">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="44be6-122">Selecciona <strong>Actualizar</strong> para cambiar el valor de <strong>Revendedor (id. de MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="44be6-122">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="44be6-123">Si un partner CSP vendió la suscripción directamente al cliente, su id. de MPN aparece dos veces, como id. de MPN y como id. de MPN del revendedor.</span><span class="sxs-lookup"><span data-stu-id="44be6-123">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="44be6-124">Si un partner CSP tiene un revendedor sin un id. de MPN, este valor se establece en el id. de MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="44be6-124">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="44be6-125">Si el partner CSP quita un id. de revendedor, este valor se establece en -1.</span><span class="sxs-lookup"><span data-stu-id="44be6-125">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="44be6-126">Campos de archivo basados en licencia</span><span class="sxs-lookup"><span data-stu-id="44be6-126">License-based file fields</span></span>


<span data-ttu-id="44be6-127">Para conciliar los cargos en función de los pedidos del cliente, compara el Syndication\_Partner\_Subscription\_Number del archivo de conciliación con el identificador de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="44be6-127">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="44be6-128">Columna</span><span class="sxs-lookup"><span data-stu-id="44be6-128">Column</span></span></strong></td>
<td><strong><span data-ttu-id="44be6-129">Descripción</span><span class="sxs-lookup"><span data-stu-id="44be6-129">Description</span></span></strong></td>
<td><strong><span data-ttu-id="44be6-130">Valor de muestra</span><span class="sxs-lookup"><span data-stu-id="44be6-130">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-131">PartnerId</span><span class="sxs-lookup"><span data-stu-id="44be6-131">PartnerId</span></span></td>
<td><p><span data-ttu-id="44be6-132">Identificador único de una entidad de facturación específica, con formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="44be6-132">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="44be6-133">No es necesario para la reconciliación, pero puede ser información útil.</span><span class="sxs-lookup"><span data-stu-id="44be6-133">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="44be6-134">Igual en todas las filas.</span><span class="sxs-lookup"><span data-stu-id="44be6-134">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="44be6-135">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="44be6-135">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-136">CustomerID</span><span class="sxs-lookup"><span data-stu-id="44be6-136">CustomerID</span></span></td>
<td><p><span data-ttu-id="44be6-137">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="44be6-137">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="44be6-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="44be6-138">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-139">OrderID</span><span class="sxs-lookup"><span data-stu-id="44be6-139">OrderID</span></span></td>
<td><p><span data-ttu-id="44be6-140">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="44be6-140">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="44be6-141">Puede ser útil para identificar al pedido al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="44be6-141">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="44be6-142">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="44be6-142">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-143">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="44be6-143">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="44be6-144">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="44be6-144">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="44be6-145">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="44be6-145">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="44be6-146">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="44be6-146">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="44be6-147">Consulte Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="44be6-147">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="44be6-148">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="44be6-148">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-149">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="44be6-149">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="44be6-150">Identificador único de las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="44be6-150">Unique identifier for subscriptions.</span></span> <span data-ttu-id="44be6-151">Un cliente puede tener varias suscripciones para el mismo plan, por lo que es importante para el análisis de archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="44be6-151">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="44be6-152">Este campo se asigna al identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="44be6-152">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="44be6-153">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="44be6-153">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-154">OfferID</span><span class="sxs-lookup"><span data-stu-id="44be6-154">OfferID</span></span></td>
<td><p><span data-ttu-id="44be6-155">Identificador único de la oferta.</span><span class="sxs-lookup"><span data-stu-id="44be6-155">Unique offer ID.</span></span> <span data-ttu-id="44be6-156">Identificador de la oferta estándar según la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="44be6-156">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="44be6-157"><b>Nota</b>: este valor no coincide con el id. de oferta de la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="44be6-157"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="44be6-158">Consulta DurableOfferID a continuación.</span><span class="sxs-lookup"><span data-stu-id="44be6-158">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="44be6-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="44be6-159">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-160">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="44be6-160">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="44be6-161">Id. de oferta duradera único, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="44be6-161">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="44be6-162"><b>Nota</b>: este valor coincide con el id. de oferta de la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="44be6-162"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="44be6-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="44be6-163">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-164">OfferName</span><span class="sxs-lookup"><span data-stu-id="44be6-164">OfferName</span></span></td>
<td><p><span data-ttu-id="44be6-165">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="44be6-165">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="44be6-166">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="44be6-166">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-167">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="44be6-167">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="44be6-168">Fecha de finalización de la suscripción, establecida en el día posterior al envío del pedido.</span><span class="sxs-lookup"><span data-stu-id="44be6-168">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="44be6-169">Al consultar la fecha de inicio de la suscripción junto con la fecha de finalización, puedes determinar si el cliente aún está dentro del primer año de la suscripción o si la suscripción se ha renovado para el año siguiente.</span><span class="sxs-lookup"><span data-stu-id="44be6-169">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="44be6-170">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="44be6-170">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="44be6-171">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="44be6-171">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-172">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="44be6-172">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="44be6-173">La fecha de finalización de la suscripción: 12 meses + x días después de la fecha de inicio (para que se alinee con la fecha de facturación del partner) o 12 meses a partir de la fecha de renovación.</span><span class="sxs-lookup"><span data-stu-id="44be6-173">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="44be6-174">En el momento de la renovación, los precios se actualizan según la lista de precios actual.</span><span class="sxs-lookup"><span data-stu-id="44be6-174">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="44be6-175">Es posible que se necesite una comunicación con el cliente antes de la renovación automatizada.</span><span class="sxs-lookup"><span data-stu-id="44be6-175">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="44be6-176">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="44be6-176">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="44be6-177">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="44be6-177">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-178">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="44be6-178">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="44be6-179">Día de inicio de los cargos.</span><span class="sxs-lookup"><span data-stu-id="44be6-179">Start day of the charges.</span></span></p>
<p><span data-ttu-id="44be6-180">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="44be6-180">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="44be6-181">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="44be6-181">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="44be6-182">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="44be6-182">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-183">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="44be6-183">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="44be6-184">Día de finalización de los cargos.</span><span class="sxs-lookup"><span data-stu-id="44be6-184">End day of the charges.</span></span></p>
<p><span data-ttu-id="44be6-185">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="44be6-185">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="44be6-186">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="44be6-186">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="44be6-187">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="44be6-187">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-188">ChargeType</span><span class="sxs-lookup"><span data-stu-id="44be6-188">ChargeType</span></span></td>
<td><p><span data-ttu-id="44be6-189">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="44be6-189">The type of charge or adjustment.</span></span> <span data-ttu-id="44be6-190">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="44be6-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="44be6-191">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="44be6-191">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-192">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="44be6-192">UnitPrice</span></span></td>
<td><p><span data-ttu-id="44be6-193">Precio por puesto, tal y como se publica en la lista de precios en el momento de compra.</span><span class="sxs-lookup"><span data-stu-id="44be6-193">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="44be6-194">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="44be6-194">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="44be6-195">6.82</span><span class="sxs-lookup"><span data-stu-id="44be6-195">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-196">Quantity</span><span class="sxs-lookup"><span data-stu-id="44be6-196">Quantity</span></span></td>
<td><p><span data-ttu-id="44be6-197">Número de puestos.</span><span class="sxs-lookup"><span data-stu-id="44be6-197">Number of seats.</span></span> <span data-ttu-id="44be6-198">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="44be6-198">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="44be6-199">2</span><span class="sxs-lookup"><span data-stu-id="44be6-199">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-200">Amount</span><span class="sxs-lookup"><span data-stu-id="44be6-200">Amount</span></span></td>
<td><p><span data-ttu-id="44be6-201">Total del precio para la cantidad.</span><span class="sxs-lookup"><span data-stu-id="44be6-201">Total of price for quantity.</span></span> <span data-ttu-id="44be6-202">Es de utilidad para comprobar que el cálculo de la cantidad coincide con la manera de calcular este valor para los clientes.</span><span class="sxs-lookup"><span data-stu-id="44be6-202">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="44be6-203">13.32</span><span class="sxs-lookup"><span data-stu-id="44be6-203">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-204">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="44be6-204">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="44be6-205">Cantidad de descuento que se aplica a estos cargos.</span><span class="sxs-lookup"><span data-stu-id="44be6-205">Amount of discount applied to these charges.</span></span> <span data-ttu-id="44be6-206">Los IUR o las nuevas suscripciones que puedan optar a un incentivo también incluirán un importe de descuento en esta columna.</span><span class="sxs-lookup"><span data-stu-id="44be6-206">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="44be6-207">2.32</span><span class="sxs-lookup"><span data-stu-id="44be6-207">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-208">Subtotal</span><span class="sxs-lookup"><span data-stu-id="44be6-208">Subtotal</span></span></td>
<td><p><span data-ttu-id="44be6-209">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="44be6-209">Total before tax.</span></span> <span data-ttu-id="44be6-210">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="44be6-210">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="44be6-211">11</span><span class="sxs-lookup"><span data-stu-id="44be6-211">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-212">Tax</span><span class="sxs-lookup"><span data-stu-id="44be6-212">Tax</span></span></td>
<td><p><span data-ttu-id="44be6-213">Cargo por importe de impuestos, en función de las reglas fiscales de tu mercado y las circunstancias específicas.</span><span class="sxs-lookup"><span data-stu-id="44be6-213">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="44be6-214">0</span><span class="sxs-lookup"><span data-stu-id="44be6-214">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-215">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="44be6-215">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="44be6-216">Total con impuestos.</span><span class="sxs-lookup"><span data-stu-id="44be6-216">Total after tax.</span></span> <span data-ttu-id="44be6-217">Comprueba si se cobran impuestos en la factura.</span><span class="sxs-lookup"><span data-stu-id="44be6-217">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="44be6-218">11</span><span class="sxs-lookup"><span data-stu-id="44be6-218">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-219">Currency</span><span class="sxs-lookup"><span data-stu-id="44be6-219">Currency</span></span></td>
<td><p><span data-ttu-id="44be6-220">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="44be6-220">Currency type.</span></span> <span data-ttu-id="44be6-221">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="44be6-221">Each billing entity has only one currency.</span></span> <span data-ttu-id="44be6-222">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="44be6-222">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="44be6-223">EUR</span><span class="sxs-lookup"><span data-stu-id="44be6-223">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-224">CustomerName</span><span class="sxs-lookup"><span data-stu-id="44be6-224">CustomerName</span></span></td>
<td><p><span data-ttu-id="44be6-225">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="44be6-225">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="44be6-226">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="44be6-226">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="44be6-227">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="44be6-227">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-228">MPNID</span><span class="sxs-lookup"><span data-stu-id="44be6-228">MPNID</span></span></td>
<td><p><span data-ttu-id="44be6-229">Id. de MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="44be6-229">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="44be6-230">4390934</span><span class="sxs-lookup"><span data-stu-id="44be6-230">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-231">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="44be6-231">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="44be6-232">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="44be6-232">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="44be6-233">Ver [Desglosar por partner](#itemizebypartner)</span><span class="sxs-lookup"><span data-stu-id="44be6-233">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="44be6-234">4390934</span><span class="sxs-lookup"><span data-stu-id="44be6-234">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-235">DomainName</span><span class="sxs-lookup"><span data-stu-id="44be6-235">DomainName</span></span></td>
<td><p><span data-ttu-id="44be6-236">Nombre de dominio del cliente, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="44be6-236">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="44be6-237">No debe usarse para identificar unívocamente el cliente como el partner o el cliente puede actualizar el dominio cortesía de forma predeterminada a través del portal de O365.</span><span class="sxs-lookup"><span data-stu-id="44be6-237">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="44be6-238">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="44be6-238">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="44be6-239">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="44be6-239">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-240">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="44be6-240">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="44be6-241">Alias de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="44be6-241">Subscription nickname.</span></span> <span data-ttu-id="44be6-242">Si no se especifica ningún alias, el Centro de partners usa OfferName.</span><span class="sxs-lookup"><span data-stu-id="44be6-242">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="44be6-243">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="44be6-243">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-244">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="44be6-244">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="44be6-245">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="44be6-245">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="44be6-246">(Este es un campo idéntico al nombre de la oferta).</span><span class="sxs-lookup"><span data-stu-id="44be6-246">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="44be6-247">PROJECT ONLINE PREMIUM SIN CLIENTE DE PROJECT</span><span class="sxs-lookup"><span data-stu-id="44be6-247">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="44be6-248">Campos de archivos basados en el uso</span><span class="sxs-lookup"><span data-stu-id="44be6-248">Usage-based file fields</span></span>


<span data-ttu-id="44be6-249">Para conciliar los cargos en función del uso de tu cliente, compara los valores de ResellerID/ResellerName/ResellerBillableAccount del archivo de conciliación, el nombre del cliente y el id. de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="44be6-249">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="44be6-250">Los siguientes campos explican los servicios usados y la clasificación.</span><span class="sxs-lookup"><span data-stu-id="44be6-250">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="44be6-251">Columna</span><span class="sxs-lookup"><span data-stu-id="44be6-251">Column</span></span></strong></td>
<td><strong><span data-ttu-id="44be6-252">Descripción</span><span class="sxs-lookup"><span data-stu-id="44be6-252">Description</span></span></strong></td>
<td><strong><span data-ttu-id="44be6-253">Valor de muestra</span><span class="sxs-lookup"><span data-stu-id="44be6-253">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-254">PartnerID</span><span class="sxs-lookup"><span data-stu-id="44be6-254">PartnerID</span></span></td>
<td><p><span data-ttu-id="44be6-255">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="44be6-255">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="44be6-256">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="44be6-256">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-257">PartnerName</span><span class="sxs-lookup"><span data-stu-id="44be6-257">PartnerName</span></span></td>
<td><p><span data-ttu-id="44be6-258">Nombre del partner.</span><span class="sxs-lookup"><span data-stu-id="44be6-258">Partner Name.</span></span></p></td>
<td><span data-ttu-id="44be6-259">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="44be6-259">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-260">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="44be6-260">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="44be6-261">Id. de cuenta del partner.</span><span class="sxs-lookup"><span data-stu-id="44be6-261">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="44be6-262">1010578050</span><span class="sxs-lookup"><span data-stu-id="44be6-262">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-263">CustomerName</span><span class="sxs-lookup"><span data-stu-id="44be6-263">CustomerName</span></span></td>
<td><p><span data-ttu-id="44be6-264">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="44be6-264">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="44be6-265">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="44be6-265">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="44be6-266">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="44be6-266">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-267">MPNID</span><span class="sxs-lookup"><span data-stu-id="44be6-267">MPNID</span></span></td>
<td><p><span data-ttu-id="44be6-268">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="44be6-268">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="44be6-269">4390934</span><span class="sxs-lookup"><span data-stu-id="44be6-269">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-270">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="44be6-270">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="44be6-271">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="44be6-271">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="44be6-272">Ver [Desglosar por partner](#itemizebypartner)</span><span class="sxs-lookup"><span data-stu-id="44be6-272">See [Itemize by partner](#itemizebypartner).</span></span></p></td>
<td><span data-ttu-id="44be6-273">4390934</span><span class="sxs-lookup"><span data-stu-id="44be6-273">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-274">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="44be6-274">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="44be6-275">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="44be6-275">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="44be6-276">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="44be6-276">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-277">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="44be6-277">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="44be6-278">Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="44be6-278">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="44be6-279">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="44be6-279">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="44be6-280">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="44be6-280">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-281">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="44be6-281">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="44be6-282">Fecha de finalización del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="44be6-282">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="44be6-283">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="44be6-283">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="44be6-284">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="44be6-284">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-285">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="44be6-285">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="44be6-286">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="44be6-286">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="44be6-287">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="44be6-287">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="44be6-288">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="44be6-288">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="44be6-289">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="44be6-289">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-290">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="44be6-290">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="44be6-291">Alias de la oferta de servicio.</span><span class="sxs-lookup"><span data-stu-id="44be6-291">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="44be6-292">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="44be6-292">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-293">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="44be6-293">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="44be6-294">Línea de negocio de la oferta de servicio</span><span class="sxs-lookup"><span data-stu-id="44be6-294">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="44be6-295">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="44be6-295">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-296">OrderID</span><span class="sxs-lookup"><span data-stu-id="44be6-296">OrderID</span></span></td>
<td><p><span data-ttu-id="44be6-297">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="44be6-297">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="44be6-298">Puede ser útil para identificar la suscripción al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="44be6-298">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="44be6-299">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="44be6-299">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-300">ServiceName</span><span class="sxs-lookup"><span data-stu-id="44be6-300">ServiceName</span></span></td>
<td><p><span data-ttu-id="44be6-301">Nombre del servicio de Azure en cuestión.</span><span class="sxs-lookup"><span data-stu-id="44be6-301">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="44be6-302">MÁQUINAS VIRTUALES</span><span class="sxs-lookup"><span data-stu-id="44be6-302">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-303">ServiceType</span><span class="sxs-lookup"><span data-stu-id="44be6-303">ServiceType</span></span></td>
<td><p><span data-ttu-id="44be6-304">Tipo específico de servicio de Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="44be6-304">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="44be6-305">Bus de servicio: individual o paquete</span><span class="sxs-lookup"><span data-stu-id="44be6-305">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="44be6-306">Base de datos SQL Azure: edición Business o Web</span><span class="sxs-lookup"><span data-stu-id="44be6-306">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-307">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="44be6-307">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="44be6-308">Identificador único específico para toda la estructura de precios y datos del servicio.</span><span class="sxs-lookup"><span data-stu-id="44be6-308">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="44be6-309">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="44be6-309">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-310">Nombre de recurso</span><span class="sxs-lookup"><span data-stu-id="44be6-310">Resource Name</span></span></td>
<td><p><span data-ttu-id="44be6-311">Nombre del recurso de Azure.</span><span class="sxs-lookup"><span data-stu-id="44be6-311">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="44be6-312">Transferencia entrante de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="44be6-312">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="44be6-313">Transferencia saliente de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="44be6-313">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-314">Region</span><span class="sxs-lookup"><span data-stu-id="44be6-314">Region</span></span></td>
<td><p><span data-ttu-id="44be6-315">La región a la que se aplica el uso.</span><span class="sxs-lookup"><span data-stu-id="44be6-315">The region the usage applies to.</span></span> <span data-ttu-id="44be6-316">Se usa principalmente para asignar tarifas a las transferencias de datos, ya que las tarifas varían según la región.</span><span class="sxs-lookup"><span data-stu-id="44be6-316">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="44be6-317">Asia Pacífico, Europa, América Latina, América del Norte</span><span class="sxs-lookup"><span data-stu-id="44be6-317">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-318">SKU</span><span class="sxs-lookup"><span data-stu-id="44be6-318">SKU</span></span></td>
<td><p><span data-ttu-id="44be6-319">Identificador único de MSFT para la oferta</span><span class="sxs-lookup"><span data-stu-id="44be6-319">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="44be6-320">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="44be6-320">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="44be6-321">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="44be6-321">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="44be6-322">Un id. y una cantidad para desglosar las distintas clasificaciones de un servicio o un recurso en un período de facturación determinado.</span><span class="sxs-lookup"><span data-stu-id="44be6-322">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="44be6-323">Para clasificación en niveles de Azure, puede haber una clasificación hasta una cantidad determinada de unidades facturables y, posteriormente, una clasificación diferente.</span><span class="sxs-lookup"><span data-stu-id="44be6-323">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="44be6-324">1</span><span class="sxs-lookup"><span data-stu-id="44be6-324">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-325">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="44be6-325">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="44be6-326">La cantidad de servicio consumida (horas, GB, etc.) durante el período de notificación.</span><span class="sxs-lookup"><span data-stu-id="44be6-326">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="44be6-327">También incluye cualquier uso no facturado de períodos anteriores.</span><span class="sxs-lookup"><span data-stu-id="44be6-327">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="44be6-328">11</span><span class="sxs-lookup"><span data-stu-id="44be6-328">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-329">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="44be6-329">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="44be6-330">Unidades que se incluyen como parte de la oferta.</span><span class="sxs-lookup"><span data-stu-id="44be6-330">Units included as part of the offer.</span></span> <span data-ttu-id="44be6-331">No suele mostrarse en CSP.</span><span class="sxs-lookup"><span data-stu-id="44be6-331">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="44be6-332">0</span><span class="sxs-lookup"><span data-stu-id="44be6-332">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="44be6-333">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="44be6-333">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="44be6-334">Unidades que no se incluyen como parte de la oferta y que el partner debe abonar.</span><span class="sxs-lookup"><span data-stu-id="44be6-334">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="44be6-335">Equivale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="44be6-335">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="44be6-336">11</span><span class="sxs-lookup"><span data-stu-id="44be6-336">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-337">ListPrice</span><span class="sxs-lookup"><span data-stu-id="44be6-337">ListPrice</span></span></td>
<td><p><span data-ttu-id="44be6-338">Precio de la oferta en vigor la fecha de inicio de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="44be6-338">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="44be6-339">0.0808 USD</span><span class="sxs-lookup"><span data-stu-id="44be6-339">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-340">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="44be6-340">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="44be6-341">ListPrist x OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="44be6-341">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="44be6-342">0.085 USD</span><span class="sxs-lookup"><span data-stu-id="44be6-342">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-343">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="44be6-343">TaxAmount</span></span></td>
<td><p><span data-ttu-id="44be6-344">Cargo por importe de impuestos, en función de las reglas fiscales de tu mercado y las circunstancias específicas.</span><span class="sxs-lookup"><span data-stu-id="44be6-344">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="44be6-345">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="44be6-345">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-346">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="44be6-346">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="44be6-347">Total con impuestos, si se aplican impuestos.</span><span class="sxs-lookup"><span data-stu-id="44be6-347">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="44be6-348">0.93 USD</span><span class="sxs-lookup"><span data-stu-id="44be6-348">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-349">Currency</span><span class="sxs-lookup"><span data-stu-id="44be6-349">Currency</span></span></td>
<td><p><span data-ttu-id="44be6-350">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="44be6-350">Currency type.</span></span> <span data-ttu-id="44be6-351">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="44be6-351">Each billing entity has only one currency.</span></span> <span data-ttu-id="44be6-352">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="44be6-352">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="44be6-353">EUR</span><span class="sxs-lookup"><span data-stu-id="44be6-353">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-354">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="44be6-354">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="44be6-355">Precio sin impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="44be6-355">Pretax price per unit.</span></span> <span data-ttu-id="44be6-356">Igual que PretaxCharges/OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="44be6-356">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="44be6-357">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="44be6-357">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-358">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="44be6-358">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="44be6-359">Precio después de impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="44be6-359">Post tax price per unit.</span></span> <span data-ttu-id="44be6-360">Igual que PostTaxTotal/OverageQuantity o PretaxEffectiveRate + tipo impositivo por importe unitario, redondeado el céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="44be6-360">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="44be6-361">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="44be6-361">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-362">ChargeType</span><span class="sxs-lookup"><span data-stu-id="44be6-362">ChargeType</span></span></td>
<td><p><span data-ttu-id="44be6-363">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="44be6-363">The type of charge or adjustment.</span></span> <span data-ttu-id="44be6-364">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="44be6-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="44be6-365">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="44be6-365">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-366">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="44be6-366">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="44be6-367">Id. de cuenta único en la plataforma de facturación de MSFT.</span><span class="sxs-lookup"><span data-stu-id="44be6-367">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="44be6-368">1280018095</span><span class="sxs-lookup"><span data-stu-id="44be6-368">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-369">UsageDate</span><span class="sxs-lookup"><span data-stu-id="44be6-369">UsageDate</span></span></td>
<td><p><span data-ttu-id="44be6-370">Fecha de implementación del servicio.</span><span class="sxs-lookup"><span data-stu-id="44be6-370">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="44be6-371">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="44be6-371">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-372">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="44be6-372">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="44be6-373">Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena.</span><span class="sxs-lookup"><span data-stu-id="44be6-373">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="44be6-374">Asia Oriental, Asia Suroriental, Norte de Europa, Europa Occidental, Centro-norte de EE.UU., Centro-sur de EE.UU.</span><span class="sxs-lookup"><span data-stu-id="44be6-374">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-375">MeteredService</span><span class="sxs-lookup"><span data-stu-id="44be6-375">MeteredService</span></span></td>
<td><p><span data-ttu-id="44be6-376">Esta columna se usa para hacer un seguimiento de los servicios de Microsoft Azure individuales que quizás no se identifiquen específicamente en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="44be6-376">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="44be6-377">Por ejemplo, las transferencias de datos se notifican como &quot;Microsoft Azure: todos los servicios&quot; en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="44be6-377">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="44be6-378">En esta columna MeteredService se indicará qué servicio específico pertenece el uso.</span><span class="sxs-lookup"><span data-stu-id="44be6-378">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="44be6-379">AccessControl, CDN, Proceso, Base de datos, ServiceBus, Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="44be6-379">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-380">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="44be6-380">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="44be6-381">Subtítulo que aclara el servicio de Microsoft Azure individual más allá del nivel proporcionado por el campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="44be6-381">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="44be6-382">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="44be6-382">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-383">Proyecto</span><span class="sxs-lookup"><span data-stu-id="44be6-383">Project</span></span></td>
<td><p><span data-ttu-id="44be6-384">Nombre definido por el cliente para la instancia del servicio</span><span class="sxs-lookup"><span data-stu-id="44be6-384">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="44be6-385">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="44be6-385">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-386">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="44be6-386">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="44be6-387">Número de conexiones de Bus de servicio aprovisionadas y usadas en un día determinado.</span><span class="sxs-lookup"><span data-stu-id="44be6-387">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="44be6-388">Por ejemplo: si tenías una conexión aprovisionada individualmente durante un mes de 30 días, Service Info 1 contendría 1 "1,000000 conexiones/30 días".</span><span class="sxs-lookup"><span data-stu-id="44be6-388">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="44be6-389">Si tenías un paquete de 25 de conexiones de Bus de servicio aprovisionadas y utilizaste 1 durante ese día, la declaración de uso diario de ese día sería "25 conexiones/30 días. Utilizadas: 1,000000".</span><span class="sxs-lookup"><span data-stu-id="44be6-389">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-390">CustomerID</span><span class="sxs-lookup"><span data-stu-id="44be6-390">CustomerID</span></span></td>
<td><p><span data-ttu-id="44be6-391">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="44be6-391">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="44be6-392">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="44be6-392">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="44be6-393">DomainName</span><span class="sxs-lookup"><span data-stu-id="44be6-393">DomainName</span></span></td>
<td><p><span data-ttu-id="44be6-394">Nombre de dominio del cliente, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="44be6-394">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="44be6-395">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="44be6-395">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="44be6-396">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="44be6-396">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="44be6-397">Unidad</span><span class="sxs-lookup"><span data-stu-id="44be6-397">Unit</span></span></td>
<td><p><span data-ttu-id="44be6-398">La unidad del nombre del recurso</span><span class="sxs-lookup"><span data-stu-id="44be6-398">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="44be6-399">GB u HORAS</span><span class="sxs-lookup"><span data-stu-id="44be6-399">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="onetimefiles"></a><span data-ttu-id="44be6-400">Campos de archivos de compra de pago único</span><span class="sxs-lookup"><span data-stu-id="44be6-400">One-time purchase file fields</span></span>

|**<span data-ttu-id="44be6-401">Campo</span><span class="sxs-lookup"><span data-stu-id="44be6-401">Field</span></span>** |**<span data-ttu-id="44be6-402">Definición</span><span class="sxs-lookup"><span data-stu-id="44be6-402">Definition</span></span>**|
|:----------------|:-----------------------------|
|<span data-ttu-id="44be6-403">PartnerId</span><span class="sxs-lookup"><span data-stu-id="44be6-403">PartnerId</span></span> |<span data-ttu-id="44be6-404">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="44be6-404">Partner ID, in GUID format.</span></span> |
|<span data-ttu-id="44be6-405">CustomerId</span><span class="sxs-lookup"><span data-stu-id="44be6-405">CustomerId</span></span> |<span data-ttu-id="44be6-406">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="44be6-406">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span> |
|<span data-ttu-id="44be6-407">CustomerName</span><span class="sxs-lookup"><span data-stu-id="44be6-407">CustomerName</span></span> |<span data-ttu-id="44be6-408">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="44be6-408">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="44be6-409">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="44be6-409">This is very important for reconciling the invoice with your system information.</span></span> |
|<span data-ttu-id="44be6-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="44be6-410">CustomerDomainName</span></span> |<span data-ttu-id="44be6-411">Nombre de dominio del cliente.</span><span class="sxs-lookup"><span data-stu-id="44be6-411">The customer’s domain name.</span></span> |
|<span data-ttu-id="44be6-412">CustomerCountry</span><span class="sxs-lookup"><span data-stu-id="44be6-412">CustomerCountry</span></span> |<span data-ttu-id="44be6-413">El país donde se encuentra el cliente.</span><span class="sxs-lookup"><span data-stu-id="44be6-413">The country in which the customer is located.</span></span> |
|<span data-ttu-id="44be6-414">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="44be6-414">InvoiceNumber</span></span> |<span data-ttu-id="44be6-415">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="44be6-415">Invoice number where the specified transaction appears.</span></span> |
|<span data-ttu-id="44be6-416">MpnId</span><span class="sxs-lookup"><span data-stu-id="44be6-416">MpnId</span></span> |<span data-ttu-id="44be6-417">Id. de MPN del partner CSP (directo o indirecto).</span><span class="sxs-lookup"><span data-stu-id="44be6-417">MPN ID of the CSP partner (direct or indirect).</span></span> |
|<span data-ttu-id="44be6-418">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="44be6-418">Reseller MPN ID</span></span> |<span data-ttu-id="44be6-419">Solo aparece en los archivos de conciliación de partners en el modelo indirecto.</span><span class="sxs-lookup"><span data-stu-id="44be6-419">Only appears on reconciliation files for partners in the indirect model.</span></span> <span data-ttu-id="44be6-420">Id. de MPN del revendedor de registro de la reserva.</span><span class="sxs-lookup"><span data-stu-id="44be6-420">The MPN ID of the reseller of record for the reservation.</span></span> <span data-ttu-id="44be6-421">Corresponde al id. de revendedor indicado para la reserva específica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="44be6-421">This corresponds to the reseller ID listed for the specific reservation in Partner Center.</span></span> <span data-ttu-id="44be6-422">Si un partner CSP vendió la reserva directamente al cliente, su id. de MPN aparece dos veces, como id. de MPN y como id. de MPN del revendedor.</span><span class="sxs-lookup"><span data-stu-id="44be6-422">If a CSP partner sold the reservation directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span> <span data-ttu-id="44be6-423">Si un partner CSP tiene un revendedor sin un id. de MPN, este valor se establece en el id. de MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="44be6-423">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span> <span data-ttu-id="44be6-424">Si el partner CSP quita un id. de revendedor, este valor se establece en -1.</span><span class="sxs-lookup"><span data-stu-id="44be6-424">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span> |
|<span data-ttu-id="44be6-425">OrderId</span><span class="sxs-lookup"><span data-stu-id="44be6-425">OrderId</span></span> |<span data-ttu-id="44be6-426">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="44be6-426">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="44be6-427">Puede ser útil para identificar la reserva al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="44be6-427">May be useful to identify the Azure reservation when contacting support but not for reconciliation.</span></span> |
|<span data-ttu-id="44be6-428">OrderDate</span><span class="sxs-lookup"><span data-stu-id="44be6-428">OrderDate</span></span> |<span data-ttu-id="44be6-429">Fecha de realización del pedido.</span><span class="sxs-lookup"><span data-stu-id="44be6-429">The date the order was placed.</span></span> |
|<span data-ttu-id="44be6-430">ProductId</span><span class="sxs-lookup"><span data-stu-id="44be6-430">ProductId</span></span> |<span data-ttu-id="44be6-431">Identificador del producto.</span><span class="sxs-lookup"><span data-stu-id="44be6-431">The ID for the product.</span></span> |
|<span data-ttu-id="44be6-432">SkuId</span><span class="sxs-lookup"><span data-stu-id="44be6-432">SkuId</span></span>  |<span data-ttu-id="44be6-433">Id. de un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="44be6-433">The ID for a particular SKU.</span></span> |
|<span data-ttu-id="44be6-434">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="44be6-434">AvailabilityId</span></span> |<span data-ttu-id="44be6-435">Id. de una disponibilidad concreta.</span><span class="sxs-lookup"><span data-stu-id="44be6-435">The ID for a particular Availability.</span></span> <span data-ttu-id="44be6-436">"Disponibilidad" hace referencia a si un SKU concreto está o no disponible para su compra para el país, la moneda, el segmento industrial determinados, etc.</span><span class="sxs-lookup"><span data-stu-id="44be6-436">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span> |
|<span data-ttu-id="44be6-437">SkuName</span><span class="sxs-lookup"><span data-stu-id="44be6-437">SkuName</span></span>  |<span data-ttu-id="44be6-438">Título para un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="44be6-438">The title for a particular SKU.</span></span> |
|<span data-ttu-id="44be6-439">ProductName</span><span class="sxs-lookup"><span data-stu-id="44be6-439">ProductName</span></span> |<span data-ttu-id="44be6-440">Nombre del producto.</span><span class="sxs-lookup"><span data-stu-id="44be6-440">The name of the product.</span></span> |
|<span data-ttu-id="44be6-441">ChargeType</span><span class="sxs-lookup"><span data-stu-id="44be6-441">ChargeType</span></span> |<span data-ttu-id="44be6-442">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="44be6-442">The type of charge or adjustment.</span></span> |
|<span data-ttu-id="44be6-443">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="44be6-443">UnitPrice</span></span> |<span data-ttu-id="44be6-444">Precio por producto pedido.</span><span class="sxs-lookup"><span data-stu-id="44be6-444">Price per product ordered.</span></span> |
|<span data-ttu-id="44be6-445">Quantity</span><span class="sxs-lookup"><span data-stu-id="44be6-445">Quantity</span></span> |<span data-ttu-id="44be6-446">Número de productos pedidos.</span><span class="sxs-lookup"><span data-stu-id="44be6-446">Number of products ordered.</span></span> |
|<span data-ttu-id="44be6-447">Subtotal</span><span class="sxs-lookup"><span data-stu-id="44be6-447">Subtotal</span></span> |<span data-ttu-id="44be6-448">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="44be6-448">Total before tax.</span></span> <span data-ttu-id="44be6-449">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="44be6-449">Checks that your subtotal matches your expected total, in case of a discount.</span></span> |
|<span data-ttu-id="44be6-450">TaxTotal</span><span class="sxs-lookup"><span data-stu-id="44be6-450">TaxTotal</span></span> |<span data-ttu-id="44be6-451">Total de todos los impuestos aplicables.</span><span class="sxs-lookup"><span data-stu-id="44be6-451">The total of all applicable taxes.</span></span> |
|<span data-ttu-id="44be6-452">Total</span><span class="sxs-lookup"><span data-stu-id="44be6-452">Total</span></span> |<span data-ttu-id="44be6-453">Número total de esta compra.</span><span class="sxs-lookup"><span data-stu-id="44be6-453">The total amount of this purchase.</span></span> |
|<span data-ttu-id="44be6-454">Moneda</span><span class="sxs-lookup"><span data-stu-id="44be6-454">Currency</span></span> |<span data-ttu-id="44be6-455">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="44be6-455">Currency type.</span></span> <span data-ttu-id="44be6-456">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="44be6-456">Each billing entity has only one currency.</span></span> <span data-ttu-id="44be6-457">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="44be6-457">Check that it matches your first invoice and then after any major billing platform update.</span></span> |
|<span data-ttu-id="44be6-458">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="44be6-458">DiscountDetails</span></span> |<span data-ttu-id="44be6-459">Lista detallada de los descuentos relevantes.</span><span class="sxs-lookup"><span data-stu-id="44be6-459">Detailed listing of any relevant discounts.</span></span> |



## <a href="" id="charge_types"></a><span data-ttu-id="44be6-460">Asignación de cargos entre una factura y el archivo de conciliación</span><span class="sxs-lookup"><span data-stu-id="44be6-460">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="44be6-461">La factura proporciona un resumen de los cargos, mientras que el archivo de conciliación proporciona un desglose detallado de las transacciones de elementos de línea, incluidos los tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="44be6-461">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="44be6-462">Para hacer referencias cruzadas de cantidades de cargos entre el archivo de conciliación y la factura, puedes usar las opciones de filtro de Microsoft Excel para filtrar por tipo de cargo en el archivo de conciliación con el fin de asignar los cargos de facturación a un conjunto de desgloses de cargos del archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="44be6-462">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="44be6-463">Los archivos de conciliación, tanto basados en uso como en licencias, solo muestran cargos y transacciones relacionados con el uso (unidades consumidas y cargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="44be6-463">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="44be6-464">En el archivo de conciliación no aparecen devoluciones, descuentos o créditos excepcionales que aparecen en la factura como "Ajustes".</span><span class="sxs-lookup"><span data-stu-id="44be6-464">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="44be6-465">La siguiente tabla muestra las asignaciones entre una sección de factura y los tipos de cargo asociados que es posible que se muestren en los archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="44be6-465">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="44be6-466">Descripción del cargo de facturación</span><span class="sxs-lookup"><span data-stu-id="44be6-466">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="44be6-467">Descripción del cargo del archivo de conciliación (columna ChargeType)</span><span class="sxs-lookup"><span data-stu-id="44be6-467">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="44be6-468">¿Qué es este cargo?</span><span class="sxs-lookup"><span data-stu-id="44be6-468">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="44be6-469">¿Cómo asigno estos valores de ChargeType a la factura?</span><span class="sxs-lookup"><span data-stu-id="44be6-469">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="44be6-470">Cargos basado en licencia</span><span class="sxs-lookup"><span data-stu-id="44be6-470">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="44be6-471">Tarifa de activación</span><span class="sxs-lookup"><span data-stu-id="44be6-471">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-472">El importe cobrado al cliente cuando usa la suscripción después de adquirirla</span><span class="sxs-lookup"><span data-stu-id="44be6-472">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="44be6-473">Desde el archivo basado en licencia, suma la columna <strong>Amount</strong>.</span><span class="sxs-lookup"><span data-stu-id="44be6-473">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="44be6-474">Cuota de cancelación</span><span class="sxs-lookup"><span data-stu-id="44be6-474">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-475">Cargos prorrateados reembolsados al cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="44be6-475">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="44be6-476">Tarifa de ciclo</span><span class="sxs-lookup"><span data-stu-id="44be6-476">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-477">Cargos periódicos de una suscripción</span><span class="sxs-lookup"><span data-stu-id="44be6-477">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="44be6-478">Prorrateo de instancia de ciclo</span><span class="sxs-lookup"><span data-stu-id="44be6-478">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-479">Cargos prorrateados evaluados del cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="44be6-479">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="44be6-480">Tarifas prorrateadas al cancelar</span><span class="sxs-lookup"><span data-stu-id="44be6-480">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-481">Reembolso prorrateado de la parte no usada del servicio tras la cancelación</span><span class="sxs-lookup"><span data-stu-id="44be6-481">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="44be6-482">Tarifas prorrateadas al comprar</span><span class="sxs-lookup"><span data-stu-id="44be6-482">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-483">Tarifas prorrateadas tras la compra</span><span class="sxs-lookup"><span data-stu-id="44be6-483">Prorated fees upon purchase</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="44be6-484">Tarifa de compra</span><span class="sxs-lookup"><span data-stu-id="44be6-484">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-485">Cargo inicial de una suscripción</span><span class="sxs-lookup"><span data-stu-id="44be6-485">Initial charge for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="44be6-486">Tarifa prorrateada al renovar</span><span class="sxs-lookup"><span data-stu-id="44be6-486">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-487">Tarifas prorrateadas tras la renovación de la suscripción</span><span class="sxs-lookup"><span data-stu-id="44be6-487">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="44be6-488">Tarifa de renovación</span><span class="sxs-lookup"><span data-stu-id="44be6-488">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-489">Cargo por renovar una suscripción</span><span class="sxs-lookup"><span data-stu-id="44be6-489">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="44be6-490">Tarifas prorrateadas al activar</span><span class="sxs-lookup"><span data-stu-id="44be6-490">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-491">Tarifas prorrateadas desde la activación hasta el final del período de facturación</span><span class="sxs-lookup"><span data-stu-id="44be6-491">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="44be6-492">Cargos de uso</span><span class="sxs-lookup"><span data-stu-id="44be6-492">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="44be6-493">Evaluar la tarifa de uso al cancelar</span><span class="sxs-lookup"><span data-stu-id="44be6-493">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-494">Tarifa de uso de acceso tras la cancelación por uso impagado durante el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="44be6-494">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="44be6-495">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="44be6-495">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="44be6-496">Evaluar la tarifa de uso para el ciclo actual</span><span class="sxs-lookup"><span data-stu-id="44be6-496">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-497">tarifa de uso de acceso para el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="44be6-497">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="44be6-498">Créditos</span><span class="sxs-lookup"><span data-stu-id="44be6-498">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="44be6-499">Desplazamiento de un elemento de línea</span><span class="sxs-lookup"><span data-stu-id="44be6-499">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-500">Reembolso parcial o total de un elemento de línea, incluidos impuestos</span><span class="sxs-lookup"><span data-stu-id="44be6-500">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-501">Desde el archivo basado en licencia, suma la columna <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="44be6-501">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="44be6-502">Desde el archivo basado en uso, suma la columna <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="44be6-502">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="44be6-503">Descuentos basados en uso</span><span class="sxs-lookup"><span data-stu-id="44be6-503">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="44be6-504">Descuento de activación</span><span class="sxs-lookup"><span data-stu-id="44be6-504">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-505">Descuento que se aplica cuando se activa la suscripción</span><span class="sxs-lookup"><span data-stu-id="44be6-505">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="44be6-506">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="44be6-506">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="44be6-507">Descuento de ciclo</span><span class="sxs-lookup"><span data-stu-id="44be6-507">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-508">Descuento que se aplica en cargos periódicos</span><span class="sxs-lookup"><span data-stu-id="44be6-508">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="44be6-509">Descuento de renovación</span><span class="sxs-lookup"><span data-stu-id="44be6-509">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-510">Descuento que se aplica cuando se renueva la suscripción</span><span class="sxs-lookup"><span data-stu-id="44be6-510">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="44be6-511">Descuento de cancelación</span><span class="sxs-lookup"><span data-stu-id="44be6-511">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-512">Cargos que se aplican cuando se cancelan los descuentos</span><span class="sxs-lookup"><span data-stu-id="44be6-512">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="44be6-513">Descuentos basado en licencia</span><span class="sxs-lookup"><span data-stu-id="44be6-513">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="44be6-514">Se pueden aplicar a varios tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="44be6-514">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="44be6-515">Desde el archivo basado en licencia, suma la columna <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="44be6-515">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="44be6-516"><strong>Impuestos</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="44be6-516"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="44be6-517">Se pueden aplicar a varios tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="44be6-517">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="44be6-518">Excepción: "Desplazamiento de un elemento de línea" ya incluye impuestos.</span><span class="sxs-lookup"><span data-stu-id="44be6-518">Exception: "Offset a line item" already includes taxes.</span></span> <span data-ttu-id="44be6-519">Créditos, consulta la sección anterior.</span><span class="sxs-lookup"><span data-stu-id="44be6-519">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="44be6-520">Impuestos o impuesto de valor añadido (IVA)</span><span class="sxs-lookup"><span data-stu-id="44be6-520">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="44be6-521">Desde el archivo basado en licencia, suma la columna <strong>Tax</strong>.</span><span class="sxs-lookup"><span data-stu-id="44be6-521">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="44be6-522">Desde el archivo basado en uso, suma la columna <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="44be6-522">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
