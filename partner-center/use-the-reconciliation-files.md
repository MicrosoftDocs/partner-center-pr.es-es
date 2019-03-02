---
title: Usar los archivos de conciliación | Centro de partners
ms.topic: article
ms.date: 10/29/2018
description: Para obtener una vista detallada del elemento de línea de cada cargo en un ciclo de facturación, descarga los archivos de conciliación del centro de partners.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 081afc547a0ff86010e06fcb5224a615a0075e34
ms.sourcegitcommit: 8bfd1358a0ef86e46bee2a1097d86de3c9e969e8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/02/2019
ms.locfileid: "9122282"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="0e03a-103">Usar los archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="0e03a-103">Use the reconciliation files</span></span>

**<span data-ttu-id="0e03a-104">Se aplica a</span><span class="sxs-lookup"><span data-stu-id="0e03a-104">Applies to</span></span>**

-  <span data-ttu-id="0e03a-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="0e03a-105">Partner Center</span></span>
-  <span data-ttu-id="0e03a-106">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="0e03a-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="0e03a-107">Para obtener una vista detallada del elemento de línea de cada cargo en un ciclo de facturación, descarga los archivos de conciliación del centro de partners.</span><span class="sxs-lookup"><span data-stu-id="0e03a-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="0e03a-108">Los detalles incluyen los cargos para las suscripciones de cada cliente y los eventos detallados (por ejemplo, una adición intermedia de puestos en una suscripción).</span><span class="sxs-lookup"><span data-stu-id="0e03a-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="0e03a-109">Desglosar por partner</span><span class="sxs-lookup"><span data-stu-id="0e03a-109">Itemize by partner</span></span>


<span data-ttu-id="0e03a-110">Los partners del modelo indirecto pueden usar estos campos adicionales en ambos archivos de conciliación basada en uso y en licencia para realizar el desglose por revendedor.</span><span class="sxs-lookup"><span data-stu-id="0e03a-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="0e03a-111">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="0e03a-111">MPN ID</span></span></th>
<th><span data-ttu-id="0e03a-112">Descripción</span><span class="sxs-lookup"><span data-stu-id="0e03a-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="0e03a-113">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="0e03a-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="0e03a-114">Id. de Microsoft Partner Network (MPN) del partner de CSP (directo o indirecto).</span><span class="sxs-lookup"><span data-stu-id="0e03a-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-115">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="0e03a-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="0e03a-116">Solo aparece en los archivos de conciliación de partners en el modelo indirecto.</span><span class="sxs-lookup"><span data-stu-id="0e03a-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="0e03a-117">El Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="0e03a-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="0e03a-118">Corresponde al id. de revendedor indicado para la suscripción específica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="0e03a-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="0e03a-119">Para ver o actualizar el revendedor, en el menú del centro de partners, selecciona <strong>los clientes</strong>y luego elige el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="0e03a-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="0e03a-120">En el menú del cliente, selecciona <strong>Suscripciones</strong> y elige la suscripción de la lista.</span><span class="sxs-lookup"><span data-stu-id="0e03a-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="0e03a-121">Selecciona <strong>Actualizar</strong> para cambiar el valor de <strong>Revendedor (id. de MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="0e03a-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="0e03a-122">Si un partner CSP vendió la suscripción directamente al cliente, su id. de MPN aparece dos veces, como id. de MPN y como id. de MPN del revendedor.</span><span class="sxs-lookup"><span data-stu-id="0e03a-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="0e03a-123">Si un partner CSP tiene un revendedor sin un id. de MPN, este valor se establece en el id. de MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="0e03a-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="0e03a-124">Si el partner CSP quita un id. de revendedor, este valor se establece en -1.</span><span class="sxs-lookup"><span data-stu-id="0e03a-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="0e03a-125">Campos de archivo basados en licencia</span><span class="sxs-lookup"><span data-stu-id="0e03a-125">License-based file fields</span></span>


<span data-ttu-id="0e03a-126">Para conciliar los cargos en función de los pedidos del cliente, compara el Syndication\_Partner\_Subscription\_Number del archivo de conciliación con el identificador de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="0e03a-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="0e03a-127">Columna</span><span class="sxs-lookup"><span data-stu-id="0e03a-127">Column</span></span></strong></td>
<td><strong><span data-ttu-id="0e03a-128">Descripción</span><span class="sxs-lookup"><span data-stu-id="0e03a-128">Description</span></span></strong></td>
<td><strong><span data-ttu-id="0e03a-129">Valor de muestra</span><span class="sxs-lookup"><span data-stu-id="0e03a-129">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="0e03a-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="0e03a-131">Identificador único de una entidad de facturación específica, con formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="0e03a-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="0e03a-132">No es necesario para la reconciliación, pero puede ser información útil.</span><span class="sxs-lookup"><span data-stu-id="0e03a-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="0e03a-133">Igual en todas las filas.</span><span class="sxs-lookup"><span data-stu-id="0e03a-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="0e03a-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="0e03a-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="0e03a-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="0e03a-136">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="0e03a-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="0e03a-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="0e03a-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="0e03a-138">OrderID</span></span></td>
<td><p><span data-ttu-id="0e03a-139">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0e03a-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="0e03a-140">Puede ser útil para identificar al pedido al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="0e03a-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="0e03a-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="0e03a-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="0e03a-143">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0e03a-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="0e03a-144">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="0e03a-145">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="0e03a-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="0e03a-146">Consulte Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="0e03a-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="0e03a-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="0e03a-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="0e03a-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="0e03a-149">Identificador único de las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="0e03a-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="0e03a-150">Un cliente puede tener varias suscripciones para el mismo plan, por lo que es importante para el análisis de archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="0e03a-151">Este campo se asigna al identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="0e03a-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="0e03a-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="0e03a-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="0e03a-153">OfferID</span></span></td>
<td><p><span data-ttu-id="0e03a-154">Identificador único de la oferta.</span><span class="sxs-lookup"><span data-stu-id="0e03a-154">Unique offer ID.</span></span> <span data-ttu-id="0e03a-155">Identificador de la oferta estándar según la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="0e03a-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="0e03a-156"><b>Nota</b>: este valor no coincide con el id. de oferta de la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="0e03a-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="0e03a-157">Consulta DurableOfferID a continuación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="0e03a-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="0e03a-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="0e03a-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="0e03a-160">Id. de oferta duradera único, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="0e03a-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="0e03a-161"><b>Nota</b>: este valor coincide con el id. de oferta de la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="0e03a-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="0e03a-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="0e03a-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="0e03a-163">OfferName</span></span></td>
<td><p><span data-ttu-id="0e03a-164">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="0e03a-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="0e03a-165">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="0e03a-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="0e03a-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="0e03a-167">Fecha de finalización de la suscripción, establecida en el día posterior al envío del pedido.</span><span class="sxs-lookup"><span data-stu-id="0e03a-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="0e03a-168">Al consultar la fecha de inicio de la suscripción junto con la fecha de finalización, puedes determinar si el cliente aún está dentro del primer año de la suscripción o si la suscripción se ha renovado para el año siguiente.</span><span class="sxs-lookup"><span data-stu-id="0e03a-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="0e03a-169">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="0e03a-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="0e03a-170">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="0e03a-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="0e03a-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="0e03a-172">La fecha de finalización de la suscripción: 12 meses + x días después de la fecha de inicio (para que se alinee con la fecha de facturación del partner) o 12 meses a partir de la fecha de renovación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="0e03a-173">En el momento de la renovación, los precios se actualizan según la lista de precios actual.</span><span class="sxs-lookup"><span data-stu-id="0e03a-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="0e03a-174">Es posible que se necesite una comunicación con el cliente antes de la renovación automatizada.</span><span class="sxs-lookup"><span data-stu-id="0e03a-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="0e03a-175">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="0e03a-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="0e03a-176">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="0e03a-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="0e03a-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="0e03a-178">Día de inicio de los cargos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="0e03a-179">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="0e03a-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="0e03a-180">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="0e03a-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="0e03a-181">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="0e03a-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="0e03a-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="0e03a-183">Día de finalización de los cargos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="0e03a-184">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="0e03a-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="0e03a-185">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="0e03a-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="0e03a-186">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="0e03a-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="0e03a-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="0e03a-188">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="0e03a-188">The type of charge or adjustment.</span></span> <span data-ttu-id="0e03a-189">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="0e03a-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="0e03a-190">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="0e03a-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="0e03a-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="0e03a-192">Precio por puesto, tal y como se publica en la lista de precios en el momento de compra.</span><span class="sxs-lookup"><span data-stu-id="0e03a-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="0e03a-193">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="0e03a-194">6.82</span><span class="sxs-lookup"><span data-stu-id="0e03a-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-195">Quantity</span><span class="sxs-lookup"><span data-stu-id="0e03a-195">Quantity</span></span></td>
<td><p><span data-ttu-id="0e03a-196">Número de puestos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-196">Number of seats.</span></span> <span data-ttu-id="0e03a-197">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="0e03a-198">2</span><span class="sxs-lookup"><span data-stu-id="0e03a-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-199">Amount</span><span class="sxs-lookup"><span data-stu-id="0e03a-199">Amount</span></span></td>
<td><p><span data-ttu-id="0e03a-200">Total del precio para la cantidad.</span><span class="sxs-lookup"><span data-stu-id="0e03a-200">Total of price for quantity.</span></span> <span data-ttu-id="0e03a-201">Es de utilidad para comprobar que el cálculo de la cantidad coincide con la manera de calcular este valor para los clientes.</span><span class="sxs-lookup"><span data-stu-id="0e03a-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="0e03a-202">13.32</span><span class="sxs-lookup"><span data-stu-id="0e03a-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="0e03a-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="0e03a-204">Cantidad de descuento que se aplica a estos cargos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="0e03a-205">Los IUR o las nuevas suscripciones que puedan optar a un incentivo también incluirán un importe de descuento en esta columna.</span><span class="sxs-lookup"><span data-stu-id="0e03a-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="0e03a-206">2.32</span><span class="sxs-lookup"><span data-stu-id="0e03a-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-207">Subtotal</span><span class="sxs-lookup"><span data-stu-id="0e03a-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="0e03a-208">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-208">Total before tax.</span></span> <span data-ttu-id="0e03a-209">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="0e03a-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="0e03a-210">11</span><span class="sxs-lookup"><span data-stu-id="0e03a-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-211">Tax</span><span class="sxs-lookup"><span data-stu-id="0e03a-211">Tax</span></span></td>
<td><p><span data-ttu-id="0e03a-212">Cargo por importe, en función del market& #39; las reglas fiscales de s y las circunstancias específicas de impuestos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-212">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="0e03a-213">0</span><span class="sxs-lookup"><span data-stu-id="0e03a-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="0e03a-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="0e03a-215">Total con impuestos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-215">Total after tax.</span></span> <span data-ttu-id="0e03a-216">Comprueba si se cobran impuestos en la factura.</span><span class="sxs-lookup"><span data-stu-id="0e03a-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="0e03a-217">11</span><span class="sxs-lookup"><span data-stu-id="0e03a-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-218">Currency</span><span class="sxs-lookup"><span data-stu-id="0e03a-218">Currency</span></span></td>
<td><p><span data-ttu-id="0e03a-219">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="0e03a-219">Currency type.</span></span> <span data-ttu-id="0e03a-220">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="0e03a-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="0e03a-221">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="0e03a-222">EUR</span><span class="sxs-lookup"><span data-stu-id="0e03a-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="0e03a-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="0e03a-224">Customer& #39; nombre de la organización s según se indica en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="0e03a-224">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="0e03a-225">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="0e03a-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="0e03a-226">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="0e03a-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="0e03a-227">MPNID</span></span></td>
<td><p><span data-ttu-id="0e03a-228">Id. de MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="0e03a-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="0e03a-229">4390934</span><span class="sxs-lookup"><span data-stu-id="0e03a-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="0e03a-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="0e03a-231">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="0e03a-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="0e03a-232">Ver <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Desglosar por partner</a></span><span class="sxs-lookup"><span data-stu-id="0e03a-232">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="0e03a-233">4390934</span><span class="sxs-lookup"><span data-stu-id="0e03a-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="0e03a-234">DomainName</span></span></td>
<td><p><span data-ttu-id="0e03a-235">Customer& #39; nombre de dominio de s, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="0e03a-235">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="0e03a-236">No debe usarse para identificar al cliente como el partner o el cliente puede actualizar el dominio cortesía de forma predeterminada a través del portal de O365.</span><span class="sxs-lookup"><span data-stu-id="0e03a-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="0e03a-237">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="0e03a-238">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="0e03a-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="0e03a-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="0e03a-240">Alias de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="0e03a-240">Subscription nickname.</span></span> <span data-ttu-id="0e03a-241">Si no se especifica ningún alias, el Centro de partners usa OfferName.</span><span class="sxs-lookup"><span data-stu-id="0e03a-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="0e03a-242">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="0e03a-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="0e03a-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="0e03a-244">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="0e03a-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="0e03a-245">(Este es un campo idéntico al nombre de la oferta).</span><span class="sxs-lookup"><span data-stu-id="0e03a-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="0e03a-246">PROJECT ONLINE PREMIUM SIN CLIENTE DE PROJECT</span><span class="sxs-lookup"><span data-stu-id="0e03a-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="0e03a-247">Campos de archivos basados en el uso</span><span class="sxs-lookup"><span data-stu-id="0e03a-247">Usage-based file fields</span></span>


<span data-ttu-id="0e03a-248">Para conciliar los cargos en función del uso de tu cliente, compara los valores de ResellerID/ResellerName/ResellerBillableAccount del archivo de conciliación, el nombre del cliente y el id. de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="0e03a-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="0e03a-249">Los siguientes campos explican los servicios usados y la clasificación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="0e03a-250">Columna</span><span class="sxs-lookup"><span data-stu-id="0e03a-250">Column</span></span></strong></td>
<td><strong><span data-ttu-id="0e03a-251">Descripción</span><span class="sxs-lookup"><span data-stu-id="0e03a-251">Description</span></span></strong></td>
<td><strong><span data-ttu-id="0e03a-252">Valor de muestra</span><span class="sxs-lookup"><span data-stu-id="0e03a-252">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="0e03a-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="0e03a-254">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="0e03a-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="0e03a-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="0e03a-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="0e03a-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="0e03a-257">Nombre del partner.</span><span class="sxs-lookup"><span data-stu-id="0e03a-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="0e03a-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="0e03a-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="0e03a-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="0e03a-260">Id. de cuenta del partner.</span><span class="sxs-lookup"><span data-stu-id="0e03a-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="0e03a-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="0e03a-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="0e03a-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="0e03a-263">Customer& #39; nombre de la organización s según se indica en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="0e03a-263">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="0e03a-264">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="0e03a-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="0e03a-265">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="0e03a-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="0e03a-266">MPNID</span></span></td>
<td><p><span data-ttu-id="0e03a-267">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="0e03a-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="0e03a-268">4390934</span><span class="sxs-lookup"><span data-stu-id="0e03a-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="0e03a-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="0e03a-270">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="0e03a-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="0e03a-271">Ver <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Desglosar por partner</a></span><span class="sxs-lookup"><span data-stu-id="0e03a-271">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="0e03a-272">4390934</span><span class="sxs-lookup"><span data-stu-id="0e03a-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="0e03a-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="0e03a-274">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="0e03a-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="0e03a-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="0e03a-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="0e03a-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="0e03a-277">Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="0e03a-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="0e03a-278">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="0e03a-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="0e03a-279">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="0e03a-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="0e03a-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="0e03a-281">Fecha de finalización del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="0e03a-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="0e03a-282">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="0e03a-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="0e03a-283">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="0e03a-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="0e03a-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="0e03a-285">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0e03a-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="0e03a-286">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="0e03a-287">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="0e03a-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="0e03a-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="0e03a-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="0e03a-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="0e03a-290">Alias de la oferta de servicio.</span><span class="sxs-lookup"><span data-stu-id="0e03a-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="0e03a-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="0e03a-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="0e03a-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="0e03a-293">Línea de negocio de la oferta de servicio</span><span class="sxs-lookup"><span data-stu-id="0e03a-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="0e03a-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="0e03a-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="0e03a-295">OrderID</span></span></td>
<td><p><span data-ttu-id="0e03a-296">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0e03a-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="0e03a-297">Puede ser útil para identificar la suscripción al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="0e03a-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="0e03a-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="0e03a-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="0e03a-300">Nombre del servicio de Azure en cuestión.</span><span class="sxs-lookup"><span data-stu-id="0e03a-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="0e03a-301">MÁQUINAS VIRTUALES</span><span class="sxs-lookup"><span data-stu-id="0e03a-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="0e03a-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="0e03a-303">Tipo específico de servicio de Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="0e03a-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="0e03a-304">Bus de servicio: individual o paquete</span><span class="sxs-lookup"><span data-stu-id="0e03a-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="0e03a-305">Base de datos SQL Azure: edición Business o Web</span><span class="sxs-lookup"><span data-stu-id="0e03a-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="0e03a-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="0e03a-307">Identificador único específico para toda la estructura de precios y datos del servicio.</span><span class="sxs-lookup"><span data-stu-id="0e03a-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="0e03a-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="0e03a-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-309">Nombre de recurso</span><span class="sxs-lookup"><span data-stu-id="0e03a-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="0e03a-310">Nombre del recurso de Azure.</span><span class="sxs-lookup"><span data-stu-id="0e03a-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="0e03a-311">Transferencia entrante de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="0e03a-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="0e03a-312">Transferencia saliente de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="0e03a-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-313">Region</span><span class="sxs-lookup"><span data-stu-id="0e03a-313">Region</span></span></td>
<td><p><span data-ttu-id="0e03a-314">La región a la que se aplica el uso.</span><span class="sxs-lookup"><span data-stu-id="0e03a-314">The region the usage applies to.</span></span> <span data-ttu-id="0e03a-315">Se usa principalmente para asignar tarifas a las transferencias de datos, ya que las tarifas varían según la región.</span><span class="sxs-lookup"><span data-stu-id="0e03a-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="0e03a-316">Asia Pacífico, Europa, América Latina, América del Norte</span><span class="sxs-lookup"><span data-stu-id="0e03a-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-317">SKU</span><span class="sxs-lookup"><span data-stu-id="0e03a-317">SKU</span></span></td>
<td><p><span data-ttu-id="0e03a-318">Identificador único de MSFT para la oferta</span><span class="sxs-lookup"><span data-stu-id="0e03a-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="0e03a-319">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="0e03a-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="0e03a-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="0e03a-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="0e03a-321">Un id. y una cantidad para desglosar las distintas clasificaciones de un servicio o un recurso en un período de facturación determinado.</span><span class="sxs-lookup"><span data-stu-id="0e03a-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="0e03a-322">Para clasificación en niveles de Azure, puede haber una clasificación hasta una cantidad determinada de unidades facturables y, posteriormente, una clasificación diferente.</span><span class="sxs-lookup"><span data-stu-id="0e03a-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="0e03a-323">1</span><span class="sxs-lookup"><span data-stu-id="0e03a-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="0e03a-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="0e03a-325">La cantidad de servicio consumida (horas, GB, etc.) durante el período de notificación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="0e03a-326">También incluye cualquier uso no facturado de períodos anteriores.</span><span class="sxs-lookup"><span data-stu-id="0e03a-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="0e03a-327">11</span><span class="sxs-lookup"><span data-stu-id="0e03a-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="0e03a-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="0e03a-329">Unidades que se incluyen como parte de la oferta.</span><span class="sxs-lookup"><span data-stu-id="0e03a-329">Units included as part of the offer.</span></span> <span data-ttu-id="0e03a-330">No suele mostrarse en CSP.</span><span class="sxs-lookup"><span data-stu-id="0e03a-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="0e03a-331">0</span><span class="sxs-lookup"><span data-stu-id="0e03a-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="0e03a-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="0e03a-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="0e03a-333">Unidades que no se incluyen como parte de la oferta y que el partner debe abonar.</span><span class="sxs-lookup"><span data-stu-id="0e03a-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="0e03a-334">Equivale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="0e03a-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="0e03a-335">11</span><span class="sxs-lookup"><span data-stu-id="0e03a-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="0e03a-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="0e03a-337">Precio de la oferta en vigor la fecha de inicio de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="0e03a-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="0e03a-338">0.0808 USD</span><span class="sxs-lookup"><span data-stu-id="0e03a-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="0e03a-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="0e03a-340">ListPrist x OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="0e03a-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="0e03a-341">0.085 USD</span><span class="sxs-lookup"><span data-stu-id="0e03a-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="0e03a-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="0e03a-343">Cargo por importe, en función del market& #39; las reglas fiscales de s y las circunstancias específicas de impuestos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-343">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="0e03a-344">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="0e03a-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="0e03a-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="0e03a-346">Total con impuestos, si se aplican impuestos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="0e03a-347">0.93 USD</span><span class="sxs-lookup"><span data-stu-id="0e03a-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-348">Currency</span><span class="sxs-lookup"><span data-stu-id="0e03a-348">Currency</span></span></td>
<td><p><span data-ttu-id="0e03a-349">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="0e03a-349">Currency type.</span></span> <span data-ttu-id="0e03a-350">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="0e03a-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="0e03a-351">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="0e03a-352">EUR</span><span class="sxs-lookup"><span data-stu-id="0e03a-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="0e03a-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="0e03a-354">Precio sin impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="0e03a-354">Pretax price per unit.</span></span> <span data-ttu-id="0e03a-355">Igual que PretaxCharges/OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="0e03a-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="0e03a-356">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="0e03a-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="0e03a-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="0e03a-358">Precio después de impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="0e03a-358">Post tax price per unit.</span></span> <span data-ttu-id="0e03a-359">Igual que PostTaxTotal/OverageQuantity o PretaxEffectiveRate + tipo impositivo por importe unitario, redondeado el céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="0e03a-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="0e03a-360">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="0e03a-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="0e03a-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="0e03a-362">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="0e03a-362">The type of charge or adjustment.</span></span> <span data-ttu-id="0e03a-363">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="0e03a-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="0e03a-364">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="0e03a-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="0e03a-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="0e03a-366">Id. de cuenta único en la plataforma de facturación de MSFT.</span><span class="sxs-lookup"><span data-stu-id="0e03a-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="0e03a-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="0e03a-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="0e03a-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="0e03a-369">Fecha de implementación del servicio.</span><span class="sxs-lookup"><span data-stu-id="0e03a-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="0e03a-370">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="0e03a-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="0e03a-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="0e03a-372">Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena.</span><span class="sxs-lookup"><span data-stu-id="0e03a-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="0e03a-373">Asia Oriental, Asia Suroriental, Norte de Europa, Europa Occidental, Centro-norte de EE.UU., Centro-sur de EE.UU.</span><span class="sxs-lookup"><span data-stu-id="0e03a-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="0e03a-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="0e03a-375">Esta columna se usa para hacer un seguimiento de los servicios de Microsoft Azure individuales que quizás no se identifiquen específicamente en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="0e03a-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="0e03a-376">Por ejemplo, las transferencias de datos se notifican como &quot;Microsoft Azure: todos los servicios&quot; en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="0e03a-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="0e03a-377">En esta columna MeteredService se indicará qué servicio específico pertenece el uso.</span><span class="sxs-lookup"><span data-stu-id="0e03a-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="0e03a-378">AccessControl, CDN, Proceso, Base de datos, ServiceBus, Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="0e03a-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="0e03a-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="0e03a-380">Subtítulo que aclara el servicio de Microsoft Azure individual más allá del nivel proporcionado por el campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="0e03a-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="0e03a-381">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="0e03a-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-382">Proyecto</span><span class="sxs-lookup"><span data-stu-id="0e03a-382">Project</span></span></td>
<td><p><span data-ttu-id="0e03a-383">Nombre definido por el cliente para la instancia del servicio</span><span class="sxs-lookup"><span data-stu-id="0e03a-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="0e03a-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="0e03a-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="0e03a-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="0e03a-386">Número de conexiones de Bus de servicio aprovisionadas y usadas en un día determinado.</span><span class="sxs-lookup"><span data-stu-id="0e03a-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="0e03a-387">Por ejemplo: si tenías una conexión aprovisionada individualmente durante un mes de 30 días, Service Info 1 contendría 1 "1,000000 conexiones/30 días".</span><span class="sxs-lookup"><span data-stu-id="0e03a-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="0e03a-388">Si tenías un paquete de 25 de conexiones de Bus de servicio aprovisionadas y utilizaste 1 durante ese día, la declaración de uso diario de ese día sería "25 conexiones/30 días. Utilizadas: 1,000000".</span><span class="sxs-lookup"><span data-stu-id="0e03a-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="0e03a-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="0e03a-390">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="0e03a-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="0e03a-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="0e03a-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="0e03a-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="0e03a-392">DomainName</span></span></td>
<td><p><span data-ttu-id="0e03a-393">Customer& #39; nombre de dominio de s, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="0e03a-393">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="0e03a-394">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="0e03a-395">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="0e03a-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="0e03a-396">Unidad</span><span class="sxs-lookup"><span data-stu-id="0e03a-396">Unit</span></span></td>
<td><p><span data-ttu-id="0e03a-397">La unidad del nombre del recurso</span><span class="sxs-lookup"><span data-stu-id="0e03a-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="0e03a-398">GB u HORAS</span><span class="sxs-lookup"><span data-stu-id="0e03a-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="0e03a-399">Campos de archivos de una sola vez y periódicos</span><span class="sxs-lookup"><span data-stu-id="0e03a-399">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="0e03a-400">Columna</span><span class="sxs-lookup"><span data-stu-id="0e03a-400">Column</span></span></th>
<th><span data-ttu-id="0e03a-401">Descripción</span><span class="sxs-lookup"><span data-stu-id="0e03a-401">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="0e03a-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="0e03a-402">PartnerId</span></span></td>
<td><p><span data-ttu-id="0e03a-403">Identificador único del inquilino de Microsoft Azure Active Directory para una entidad de facturación específica, en formato GUID.</span><span class="sxs-lookup"><span data-stu-id="0e03a-403">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="0e03a-404">No es necesario para la reconciliación, pero puede ser información útil.</span><span class="sxs-lookup"><span data-stu-id="0e03a-404">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="0e03a-405">Igual en todas las filas.</span><span class="sxs-lookup"><span data-stu-id="0e03a-405">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-406">Id. de cliente</span><span class="sxs-lookup"><span data-stu-id="0e03a-406">Customer Id</span></span></td>
<td><p><span data-ttu-id="0e03a-407">Microsoft Azure Active Directory inquilino identificador exclusivo, en formato GUID, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="0e03a-407">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-408">Nombre del cliente</span><span class="sxs-lookup"><span data-stu-id="0e03a-408">Customer Name</span></span></td>
<td><p><span data-ttu-id="0e03a-409">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="0e03a-409">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="0e03a-410">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="0e03a-411">Nombre de dominio del cliente, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="0e03a-411">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="0e03a-412">No debe usarse para identificar al cliente como el partner o el cliente puede actualizar el dominio cortesía de forma predeterminada a través del portal de O365.</span><span class="sxs-lookup"><span data-stu-id="0e03a-412">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="0e03a-413">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-413">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-414">País de cliente</span><span class="sxs-lookup"><span data-stu-id="0e03a-414">Customer Country</span></span></td>
<td><p><span data-ttu-id="0e03a-415">El país donde se encuentra el cliente.</span><span class="sxs-lookup"><span data-stu-id="0e03a-415">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-416">Número de factura</span><span class="sxs-lookup"><span data-stu-id="0e03a-416">Invoice number</span></span></td>
<td><p><span data-ttu-id="0e03a-417">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="0e03a-417">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-418">MpnId</span><span class="sxs-lookup"><span data-stu-id="0e03a-418">MpnId</span></span></td>
<td><p><span data-ttu-id="0e03a-419">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="0e03a-419">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-420">MpnId de revendedor</span><span class="sxs-lookup"><span data-stu-id="0e03a-420">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="0e03a-421">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="0e03a-421">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-422">Id. de pedido</span><span class="sxs-lookup"><span data-stu-id="0e03a-422">Order ID</span></span></td>
<td><p><span data-ttu-id="0e03a-423">Identificador único de un pedido en la plataforma de comercio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0e03a-423">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="0e03a-424">Puede ser útil para identificar al pedido al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-424">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-425">Fecha del pedido</span><span class="sxs-lookup"><span data-stu-id="0e03a-425">Order date</span></span></td>
<td><p><span data-ttu-id="0e03a-426">Fecha de realización del pedido.</span><span class="sxs-lookup"><span data-stu-id="0e03a-426">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-427">ProductId</span><span class="sxs-lookup"><span data-stu-id="0e03a-427">ProductId</span></span></td>
<td><p><span data-ttu-id="0e03a-428">Identificador del producto.</span><span class="sxs-lookup"><span data-stu-id="0e03a-428">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-429">SkuId</span><span class="sxs-lookup"><span data-stu-id="0e03a-429">SkuId</span></span></td>
<td><p><span data-ttu-id="0e03a-430">Id. de un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="0e03a-430">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-431">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="0e03a-431">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="0e03a-432">Id. de una disponibilidad concreta.</span><span class="sxs-lookup"><span data-stu-id="0e03a-432">The ID for a particular Availability.</span></span> <span data-ttu-id="0e03a-433">"Disponibilidad" hace referencia a si un SKU concreto está o no disponible para su compra para el país, la moneda, el segmento industrial determinados, etc.</span><span class="sxs-lookup"><span data-stu-id="0e03a-433">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-434">Nombre SKU</span><span class="sxs-lookup"><span data-stu-id="0e03a-434">SKU Name</span></span></td>
<td><p><span data-ttu-id="0e03a-435">Título para un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="0e03a-435">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-436">Nombre del producto</span><span class="sxs-lookup"><span data-stu-id="0e03a-436">Product name</span></span></td>
<td><p><span data-ttu-id="0e03a-437">Nombre del producto.</span><span class="sxs-lookup"><span data-stu-id="0e03a-437">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-438">PublisherName</span><span class="sxs-lookup"><span data-stu-id="0e03a-438">PublisherName</span></span></td>
<td><p><span data-ttu-id="0e03a-439">El nombre del Editor del producto.</span><span class="sxs-lookup"><span data-stu-id="0e03a-439">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-440">PublisherID</span><span class="sxs-lookup"><span data-stu-id="0e03a-440">PublisherID</span></span></td>
<td><p><span data-ttu-id="0e03a-441">Identificador único de este publicador.</span><span class="sxs-lookup"><span data-stu-id="0e03a-441">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-442">Descripción de la suscripción</span><span class="sxs-lookup"><span data-stu-id="0e03a-442">Subscription Description</span></span></td>
<td><p><span data-ttu-id="0e03a-443">Nombre descriptivo de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="0e03a-443">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-444">Id. de suscripción</span><span class="sxs-lookup"><span data-stu-id="0e03a-444">Subscription ID</span></span></td>
<td><p><span data-ttu-id="0e03a-445">Identificador único de una suscripción en la plataforma de comercio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0e03a-445">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="0e03a-446">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-446">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="0e03a-447">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="0e03a-447">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-448">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="0e03a-448">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="0e03a-449">Día de inicio de los cargos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-449">Start day of the charges.</span></span> <span data-ttu-id="0e03a-450">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="0e03a-450">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-451">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="0e03a-451">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="0e03a-452">Día de finalización de los cargos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-452">End day of the charges.</span></span> <span data-ttu-id="0e03a-453">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="0e03a-453">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-454">Término y Billingcycle</span><span class="sxs-lookup"><span data-stu-id="0e03a-454">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="0e03a-455">La longitud del término y el ciclo de facturación de la compra.</span><span class="sxs-lookup"><span data-stu-id="0e03a-455">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="0e03a-456">Por ejemplo, "1 año, mensualmente".</span><span class="sxs-lookup"><span data-stu-id="0e03a-456">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-457">Tipo de cargo</span><span class="sxs-lookup"><span data-stu-id="0e03a-457">Charge Type</span></span></td>
<td><p><span data-ttu-id="0e03a-458">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="0e03a-458">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-459">Precio unitario</span><span class="sxs-lookup"><span data-stu-id="0e03a-459">Unit Price</span></span></td>
<td><p><span data-ttu-id="0e03a-460">El precio de su publicación en la lista de precios en el momento de compra.</span><span class="sxs-lookup"><span data-stu-id="0e03a-460">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="0e03a-461">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-461">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-462">Precio unitario eficaz</span><span class="sxs-lookup"><span data-stu-id="0e03a-462">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="0e03a-463">El precio unitario después de que se han realizado ajustes.</span><span class="sxs-lookup"><span data-stu-id="0e03a-463">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-464">Cantidad</span><span class="sxs-lookup"><span data-stu-id="0e03a-464">Quantity</span></span></td>
<td><p><span data-ttu-id="0e03a-465">Número de unidades.</span><span class="sxs-lookup"><span data-stu-id="0e03a-465">Number of units.</span></span> <span data-ttu-id="0e03a-466">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-466">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-467">Tipo de unidad</span><span class="sxs-lookup"><span data-stu-id="0e03a-467">Unit type</span></span></td>
<td><p><span data-ttu-id="0e03a-468">El tipo de unidad que se va a comprar.</span><span class="sxs-lookup"><span data-stu-id="0e03a-468">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-469">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="0e03a-469">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="0e03a-470">Una explicación de los descuentos aplicables.</span><span class="sxs-lookup"><span data-stu-id="0e03a-470">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-471">Subtotal</span><span class="sxs-lookup"><span data-stu-id="0e03a-471">Sub Total</span></span></td>
<td><p><span data-ttu-id="0e03a-472">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-472">Total before tax.</span></span> <span data-ttu-id="0e03a-473">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="0e03a-473">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-474">Total de impuestos</span><span class="sxs-lookup"><span data-stu-id="0e03a-474">Tax Total</span></span></td>
<td><p><span data-ttu-id="0e03a-475">Cargo por importe de impuestos, en función de las reglas fiscales de tu mercado y las circunstancias específicas.</span><span class="sxs-lookup"><span data-stu-id="0e03a-475">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-476">Total</span><span class="sxs-lookup"><span data-stu-id="0e03a-476">Total</span></span></td>
<td><p><span data-ttu-id="0e03a-477">Total con impuestos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-477">Total after tax.</span></span> <span data-ttu-id="0e03a-478">Comprueba si se cobran impuestos en la factura.</span><span class="sxs-lookup"><span data-stu-id="0e03a-478">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-479">Moneda</span><span class="sxs-lookup"><span data-stu-id="0e03a-479">Currency</span></span></td>
<td><p><span data-ttu-id="0e03a-480">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="0e03a-480">Currency type.</span></span> <span data-ttu-id="0e03a-481">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="0e03a-481">Each billing entity has only one currency.</span></span> <span data-ttu-id="0e03a-482">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-482">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-483">AlternateID</span><span class="sxs-lookup"><span data-stu-id="0e03a-483">AlternateID</span></span></td>
<td><p><span data-ttu-id="0e03a-484">Un identificador alternativo para un identificador.</span><span class="sxs-lookup"><span data-stu-id="0e03a-484">An alternate identifier to an ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="0e03a-485">Campos de archivos de uso prorrateado diarios</span><span class="sxs-lookup"><span data-stu-id="0e03a-485">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="0e03a-486">Columna</span><span class="sxs-lookup"><span data-stu-id="0e03a-486">Column</span></span></th>
<th><span data-ttu-id="0e03a-487">Descripción</span><span class="sxs-lookup"><span data-stu-id="0e03a-487">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="0e03a-488">PartnerId</span><span class="sxs-lookup"><span data-stu-id="0e03a-488">PartnerId</span></span></td>
<td><p><span data-ttu-id="0e03a-489">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="0e03a-489">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-490">PartnerName</span><span class="sxs-lookup"><span data-stu-id="0e03a-490">PartnerName</span></span></td>
<td><p><span data-ttu-id="0e03a-491">Nombre del partner.</span><span class="sxs-lookup"><span data-stu-id="0e03a-491">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-492">CustomerId</span><span class="sxs-lookup"><span data-stu-id="0e03a-492">CustomerId</span></span></td>
<td><p><span data-ttu-id="0e03a-493">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="0e03a-493">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-494">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="0e03a-494">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="0e03a-495">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="0e03a-495">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="0e03a-496">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="0e03a-496">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-497">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="0e03a-497">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="0e03a-498">Nombre de dominio del cliente.</span><span class="sxs-lookup"><span data-stu-id="0e03a-498">The customer’s domain name.</span></span> <span data-ttu-id="0e03a-499">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="0e03a-499">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-500">País de cliente</span><span class="sxs-lookup"><span data-stu-id="0e03a-500">Customer country</span></span></td>
<td><p><span data-ttu-id="0e03a-501">El país donde se encuentra el cliente.</span><span class="sxs-lookup"><span data-stu-id="0e03a-501">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-502">MPNID</span><span class="sxs-lookup"><span data-stu-id="0e03a-502">MPNID</span></span></td>
<td><p><span data-ttu-id="0e03a-503">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="0e03a-503">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-504">Revendedor MPNID</span><span class="sxs-lookup"><span data-stu-id="0e03a-504">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="0e03a-505">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="0e03a-505">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="0e03a-506">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="0e03a-506">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-507">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="0e03a-507">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="0e03a-508">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="0e03a-508">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="0e03a-509">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="0e03a-509">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-510">ProductId</span><span class="sxs-lookup"><span data-stu-id="0e03a-510">ProductId</span></span></td>
<td><p><span data-ttu-id="0e03a-511">Identificador del producto.</span><span class="sxs-lookup"><span data-stu-id="0e03a-511">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-512">SkuId</span><span class="sxs-lookup"><span data-stu-id="0e03a-512">SkuId</span></span></td>
<td><p><span data-ttu-id="0e03a-513">Id. de un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="0e03a-513">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-514">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="0e03a-514">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="0e03a-515">Id. de una disponibilidad concreta.</span><span class="sxs-lookup"><span data-stu-id="0e03a-515">The ID for a particular Availability.</span></span> <span data-ttu-id="0e03a-516">"Disponibilidad" hace referencia a si un SKU concreto está o no disponible para su compra para el país, la moneda, el segmento industrial determinados, etc.</span><span class="sxs-lookup"><span data-stu-id="0e03a-516">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-517">Nombre SKU</span><span class="sxs-lookup"><span data-stu-id="0e03a-517">SKU Name</span></span></td>
<td><p><span data-ttu-id="0e03a-518">Título para un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="0e03a-518">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-519">PublisherName</span><span class="sxs-lookup"><span data-stu-id="0e03a-519">PublisherName</span></span></td>
<td><p><span data-ttu-id="0e03a-520">El nombre del publicador.</span><span class="sxs-lookup"><span data-stu-id="0e03a-520">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-521">PublisherID</span><span class="sxs-lookup"><span data-stu-id="0e03a-521">PublisherID</span></span></td>
<td><p><span data-ttu-id="0e03a-522">El identificador del Editor, en formato GUID.</span><span class="sxs-lookup"><span data-stu-id="0e03a-522">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="0e03a-523">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="0e03a-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="0e03a-524">Descripción de la suscripción</span><span class="sxs-lookup"><span data-stu-id="0e03a-524">Subscription Description</span></span></td>
<td><p><span data-ttu-id="0e03a-525">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="0e03a-525">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="0e03a-526">(Este es un campo idéntico al nombre de la oferta).</span><span class="sxs-lookup"><span data-stu-id="0e03a-526">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-527">Id. de suscripción</span><span class="sxs-lookup"><span data-stu-id="0e03a-527">Subscription ID</span></span></td>
<td><p><span data-ttu-id="0e03a-528">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="0e03a-528">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="0e03a-529">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-529">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="0e03a-530">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="0e03a-530">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-531">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="0e03a-531">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="0e03a-532">Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="0e03a-532">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="0e03a-533">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="0e03a-533">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-534">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="0e03a-534">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="0e03a-535">Fecha de finalización del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="0e03a-535">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="0e03a-536">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="0e03a-536">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-537">Fecha de uso</span><span class="sxs-lookup"><span data-stu-id="0e03a-537">Usage Date</span></span></td>
<td><p><span data-ttu-id="0e03a-538">Fecha de uso del servicio.</span><span class="sxs-lookup"><span data-stu-id="0e03a-538">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-539">Tipo de medidor</span><span class="sxs-lookup"><span data-stu-id="0e03a-539">Meter Type</span></span></td>
<td><p><span data-ttu-id="0e03a-540">El tipo de metros.</span><span class="sxs-lookup"><span data-stu-id="0e03a-540">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-541">Categoría de metro</span><span class="sxs-lookup"><span data-stu-id="0e03a-541">Meter Category</span></span></td>
<td><p><span data-ttu-id="0e03a-542">El servicio de nivel superior para el uso.</span><span class="sxs-lookup"><span data-stu-id="0e03a-542">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-543">Id. de metro</span><span class="sxs-lookup"><span data-stu-id="0e03a-543">Meter Id</span></span></td>
<td><p><span data-ttu-id="0e03a-544">El identificador para el medidor que se usa.</span><span class="sxs-lookup"><span data-stu-id="0e03a-544">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-545">Medidor subcategoría.</span><span class="sxs-lookup"><span data-stu-id="0e03a-545">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="0e03a-546">El tipo de servicio de Azure que puede afectar a la velocidad.</span><span class="sxs-lookup"><span data-stu-id="0e03a-546">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-547">Nombre de metro</span><span class="sxs-lookup"><span data-stu-id="0e03a-547">Meter Name</span></span></td>
<td><p><span data-ttu-id="0e03a-548">La unidad de medida para el medidor está consumiendo.</span><span class="sxs-lookup"><span data-stu-id="0e03a-548">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-549">Región de metro</span><span class="sxs-lookup"><span data-stu-id="0e03a-549">Meter Region</span></span></td>
<td><p><span data-ttu-id="0e03a-550">Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena.</span><span class="sxs-lookup"><span data-stu-id="0e03a-550">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-551">Unidad</span><span class="sxs-lookup"><span data-stu-id="0e03a-551">Unit</span></span></td>
<td><p><span data-ttu-id="0e03a-552">La unidad del nombre del recurso.</span><span class="sxs-lookup"><span data-stu-id="0e03a-552">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-553">Cantidad consumida</span><span class="sxs-lookup"><span data-stu-id="0e03a-553">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="0e03a-554">La cantidad de servicio consumida (horas, GB, etc.) durante el período de notificación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-554">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="0e03a-555">También incluye cualquier uso no facturado de períodos anteriores.</span><span class="sxs-lookup"><span data-stu-id="0e03a-555">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-556">Ubicación de recurso</span><span class="sxs-lookup"><span data-stu-id="0e03a-556">Resource Location</span></span></td>
<td><p><span data-ttu-id="0e03a-557">El centro de datos donde se ejecuta el medidor.</span><span class="sxs-lookup"><span data-stu-id="0e03a-557">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-558">Servicio consumida</span><span class="sxs-lookup"><span data-stu-id="0e03a-558">Consumed Service</span></span></td>
<td><p><span data-ttu-id="0e03a-559">El servicio de plataforma de Azure que usaste.</span><span class="sxs-lookup"><span data-stu-id="0e03a-559">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-560">Grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="0e03a-560">Resource Group</span></span></td>
<td><p><span data-ttu-id="0e03a-561">El grupo de recursos en el que se está ejecutando el medidor implementado.</span><span class="sxs-lookup"><span data-stu-id="0e03a-561">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-562">URI de recurso</span><span class="sxs-lookup"><span data-stu-id="0e03a-562">Resource URI</span></span></td>
<td><p><span data-ttu-id="0e03a-563">El URI del recurso que se usa.</span><span class="sxs-lookup"><span data-stu-id="0e03a-563">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-564">Tipo de cargo</span><span class="sxs-lookup"><span data-stu-id="0e03a-564">Charge type</span></span></td>
<td><p><span data-ttu-id="0e03a-565">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="0e03a-565">The type of charge or adjustment.</span></span> <span data-ttu-id="0e03a-566">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="0e03a-566">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-567">Precio unitario</span><span class="sxs-lookup"><span data-stu-id="0e03a-567">Unit price</span></span></td>
<td><p><span data-ttu-id="0e03a-568">Precio por licencia, ya que publica en la lista de precios en el momento de compra.</span><span class="sxs-lookup"><span data-stu-id="0e03a-568">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="0e03a-569">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-569">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-570">Cantidad</span><span class="sxs-lookup"><span data-stu-id="0e03a-570">Quantity</span></span></td>
<td><p><span data-ttu-id="0e03a-571">Número de licencias.</span><span class="sxs-lookup"><span data-stu-id="0e03a-571">Number of licenses.</span></span> <span data-ttu-id="0e03a-572">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-572">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-573">Tipo de unidad</span><span class="sxs-lookup"><span data-stu-id="0e03a-573">Unit type</span></span></td>
<td><p><span data-ttu-id="0e03a-574">El tipo de unidad el medidor se cargará en.</span><span class="sxs-lookup"><span data-stu-id="0e03a-574">The type of unit the meter is charged in.</span></span> <span data-ttu-id="0e03a-575">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="0e03a-575">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-576">Antes de impuestos de facturación</span><span class="sxs-lookup"><span data-stu-id="0e03a-576">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="0e03a-577">Importe total antes de impuestos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-577">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-578">Divisa de facturación</span><span class="sxs-lookup"><span data-stu-id="0e03a-578">Billing currency</span></span></td>
<td><p><span data-ttu-id="0e03a-579">La divisa en la región geográfica del cliente</span><span class="sxs-lookup"><span data-stu-id="0e03a-579">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-580">Precios total sin impuestos</span><span class="sxs-lookup"><span data-stu-id="0e03a-580">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="0e03a-581">El precio antes de que se agregan los impuestos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-581">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-582">Moneda de precios</span><span class="sxs-lookup"><span data-stu-id="0e03a-582">Pricing currency</span></span></td>
<td><p><span data-ttu-id="0e03a-583">La divisa en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="0e03a-583">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-584">Información de servicio 1</span><span class="sxs-lookup"><span data-stu-id="0e03a-584">Service Info 1</span></span></td>
<td><p><span data-ttu-id="0e03a-585">Número de conexiones de Bus de servicio aprovisionadas y usadas en un día determinado.</span><span class="sxs-lookup"><span data-stu-id="0e03a-585">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-586">Información sobre el servicio 2</span><span class="sxs-lookup"><span data-stu-id="0e03a-586">Service Info 2</span></span></td>
<td><p><span data-ttu-id="0e03a-587">Un campo heredado que captura metadatos específicos del servicio opcional.</span><span class="sxs-lookup"><span data-stu-id="0e03a-587">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="0e03a-588">Etiquetas</span><span class="sxs-lookup"><span data-stu-id="0e03a-588">Tags</span></span></td>
<td><p><span data-ttu-id="0e03a-589">Etiquetas que se asigna al medidor en orden para agrupar registros de facturación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-589">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="0e03a-590">Por ejemplo, puedes usar etiquetas para distribuir los costes por el departamento que usa el medidor.</span><span class="sxs-lookup"><span data-stu-id="0e03a-590">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="0e03a-591">Información adicional</span><span class="sxs-lookup"><span data-stu-id="0e03a-591">Additional Info</span></span></td>
<td><p><span data-ttu-id="0e03a-592">Cualquier información adicional que no se tratan en otras columnas.</span><span class="sxs-lookup"><span data-stu-id="0e03a-592">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="0e03a-593">Asignación de cargos entre una factura y el archivo de conciliación</span><span class="sxs-lookup"><span data-stu-id="0e03a-593">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="0e03a-594">La factura proporciona un resumen de los cargos, mientras que el archivo de conciliación proporciona un desglose detallado de las transacciones de elementos de línea, incluidos los tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="0e03a-594">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="0e03a-595">Para hacer referencias cruzadas de cantidades de cargos entre el archivo de conciliación y la factura, puedes usar las opciones de filtro de Microsoft Excel para filtrar por tipo de cargo en el archivo de conciliación con el fin de asignar los cargos de facturación a un conjunto de desgloses de cargos del archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-595">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="0e03a-596">Los archivos de conciliación, tanto basados en uso como en licencias, solo muestran cargos y transacciones relacionados con el uso (unidades consumidas y cargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="0e03a-596">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="0e03a-597">En el archivo de conciliación no aparecen devoluciones, descuentos o créditos excepcionales que aparecen en la factura como "Ajustes".</span><span class="sxs-lookup"><span data-stu-id="0e03a-597">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="0e03a-598">La siguiente tabla muestra las asignaciones entre una sección de factura y los tipos de cargo asociados que es posible que se muestren en los archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="0e03a-598">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="0e03a-599">Descripción del cargo de facturación</span><span class="sxs-lookup"><span data-stu-id="0e03a-599">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="0e03a-600">Descripción del cargo del archivo de conciliación (columna ChargeType)</span><span class="sxs-lookup"><span data-stu-id="0e03a-600">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="0e03a-601">¿Qué es este cargo?</span><span class="sxs-lookup"><span data-stu-id="0e03a-601">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="0e03a-602">¿Cómo asigno estos valores de ChargeType a la factura?</span><span class="sxs-lookup"><span data-stu-id="0e03a-602">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="0e03a-603">Cargos basado en licencia</span><span class="sxs-lookup"><span data-stu-id="0e03a-603">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="0e03a-604">Tarifa de activación</span><span class="sxs-lookup"><span data-stu-id="0e03a-604">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-605">El importe cobrado al cliente cuando usa la suscripción después de adquirirla</span><span class="sxs-lookup"><span data-stu-id="0e03a-605">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="0e03a-606">Desde el archivo basado en licencia, suma la columna <strong>Amount</strong>.</span><span class="sxs-lookup"><span data-stu-id="0e03a-606">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0e03a-607">Cuota de cancelación</span><span class="sxs-lookup"><span data-stu-id="0e03a-607">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-608">Cargos prorrateados reembolsados al cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="0e03a-608">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0e03a-609">Tarifa de ciclo</span><span class="sxs-lookup"><span data-stu-id="0e03a-609">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-610">Cargos periódicos de una suscripción</span><span class="sxs-lookup"><span data-stu-id="0e03a-610">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0e03a-611">Prorrateo de instancia de ciclo</span><span class="sxs-lookup"><span data-stu-id="0e03a-611">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-612">Cargos prorrateados evaluados del cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="0e03a-612">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0e03a-613">Tarifas prorrateadas al cancelar</span><span class="sxs-lookup"><span data-stu-id="0e03a-613">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-614">Reembolso prorrateado de la parte no usada del servicio tras la cancelación</span><span class="sxs-lookup"><span data-stu-id="0e03a-614">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0e03a-615">Tarifas prorrateadas al comprar</span><span class="sxs-lookup"><span data-stu-id="0e03a-615">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-616">El tipo de cargo de una suscripción cuando se utiliza la facturación anual</span><span class="sxs-lookup"><span data-stu-id="0e03a-616">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0e03a-617">Tarifa de compra</span><span class="sxs-lookup"><span data-stu-id="0e03a-617">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-618">El tipo de cargo de una suscripción cuando se utiliza la facturación mensual</span><span class="sxs-lookup"><span data-stu-id="0e03a-618">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0e03a-619">Tarifa prorrateada al renovar</span><span class="sxs-lookup"><span data-stu-id="0e03a-619">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-620">Tarifas prorrateadas tras la renovación de la suscripción</span><span class="sxs-lookup"><span data-stu-id="0e03a-620">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="0e03a-621">Tarifa de renovación</span><span class="sxs-lookup"><span data-stu-id="0e03a-621">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-622">Cargo por renovar una suscripción</span><span class="sxs-lookup"><span data-stu-id="0e03a-622">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0e03a-623">Tarifas prorrateadas al activar</span><span class="sxs-lookup"><span data-stu-id="0e03a-623">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-624">Tarifas prorrateadas desde la activación hasta el final del período de facturación</span><span class="sxs-lookup"><span data-stu-id="0e03a-624">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="0e03a-625">Cargos de uso</span><span class="sxs-lookup"><span data-stu-id="0e03a-625">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="0e03a-626">Evaluar la tarifa de uso al cancelar</span><span class="sxs-lookup"><span data-stu-id="0e03a-626">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-627">Tarifa de uso de acceso tras la cancelación por uso impagado durante el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="0e03a-627">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="0e03a-628">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="0e03a-628">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0e03a-629">Evaluar la tarifa de uso para el ciclo actual</span><span class="sxs-lookup"><span data-stu-id="0e03a-629">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-630">tarifa de uso de acceso para el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="0e03a-630">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="0e03a-631">Créditos</span><span class="sxs-lookup"><span data-stu-id="0e03a-631">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="0e03a-632">Desplazamiento de un elemento de línea</span><span class="sxs-lookup"><span data-stu-id="0e03a-632">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-633">Reembolso parcial o total de un elemento de línea, incluidos impuestos</span><span class="sxs-lookup"><span data-stu-id="0e03a-633">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-634">Desde el archivo basado en licencia, suma la columna <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="0e03a-634">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="0e03a-635">Desde el archivo basado en uso, suma la columna <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="0e03a-635">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="0e03a-636">Descuentos basados en uso</span><span class="sxs-lookup"><span data-stu-id="0e03a-636">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="0e03a-637">Descuento de activación</span><span class="sxs-lookup"><span data-stu-id="0e03a-637">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-638">Descuento que se aplica cuando se activa la suscripción</span><span class="sxs-lookup"><span data-stu-id="0e03a-638">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="0e03a-639">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="0e03a-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0e03a-640">Descuento de ciclo</span><span class="sxs-lookup"><span data-stu-id="0e03a-640">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-641">Descuento que se aplica en cargos periódicos</span><span class="sxs-lookup"><span data-stu-id="0e03a-641">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0e03a-642">Descuento de renovación</span><span class="sxs-lookup"><span data-stu-id="0e03a-642">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-643">Descuento que se aplica cuando se renueva la suscripción</span><span class="sxs-lookup"><span data-stu-id="0e03a-643">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0e03a-644">Descuento de cancelación</span><span class="sxs-lookup"><span data-stu-id="0e03a-644">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-645">Cargos que se aplican cuando se cancelan los descuentos</span><span class="sxs-lookup"><span data-stu-id="0e03a-645">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="0e03a-646">Descuentos basado en licencia</span><span class="sxs-lookup"><span data-stu-id="0e03a-646">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="0e03a-647">Se pueden aplicar a varios tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="0e03a-647">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="0e03a-648">Desde el archivo basado en licencia, suma la columna <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="0e03a-648">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="0e03a-649"><strong>Impuestos</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="0e03a-649"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="0e03a-650">Se pueden aplicar a varios tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="0e03a-650">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="0e03a-651">Excepción: &quot;desplazamiento de un elemento de línea&quot; ya incluye impuestos.</span><span class="sxs-lookup"><span data-stu-id="0e03a-651">Exception: &quot;Offset a line item&quot; already includes taxes.</span></span> <span data-ttu-id="0e03a-652">Créditos, consulta la sección anterior.</span><span class="sxs-lookup"><span data-stu-id="0e03a-652">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="0e03a-653">Impuestos o impuesto de valor añadido (IVA)</span><span class="sxs-lookup"><span data-stu-id="0e03a-653">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="0e03a-654">Desde el archivo basado en licencia, suma la columna <strong>Tax</strong>.</span><span class="sxs-lookup"><span data-stu-id="0e03a-654">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="0e03a-655">Desde el archivo basado en uso, suma la columna <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="0e03a-655">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
