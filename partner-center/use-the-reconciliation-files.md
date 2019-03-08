---
title: Usar los archivos de conciliación | Centro de partners
ms.topic: article
ms.date: 10/29/2018
description: Para obtener una vista detallada del elemento de línea de cada carga de un ciclo de facturación, descargue los archivos de conciliación de centro de partners.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 5ce9b7cd9ead08b7709c68a0e967d64e9f2a32bd
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2019
ms.locfileid: "57585138"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="f2a43-103">Usar los archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="f2a43-103">Use the reconciliation files</span></span>

<span data-ttu-id="f2a43-104">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="f2a43-104">**Applies to**</span></span>

-  <span data-ttu-id="f2a43-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="f2a43-105">Partner Center</span></span>
-  <span data-ttu-id="f2a43-106">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="f2a43-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="f2a43-107">Para obtener una vista detallada del elemento de línea de cada carga de un ciclo de facturación, descargue los archivos de conciliación de centro de partners.</span><span class="sxs-lookup"><span data-stu-id="f2a43-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="f2a43-108">Los detalles incluyen los cargos para las suscripciones de cada cliente y los eventos detallados (por ejemplo, una adición intermedia de puestos en una suscripción).</span><span class="sxs-lookup"><span data-stu-id="f2a43-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="f2a43-109">Detallar asociado</span><span class="sxs-lookup"><span data-stu-id="f2a43-109">Itemize by partner</span></span>


<span data-ttu-id="f2a43-110">Los partners del modelo indirecto pueden usar estos campos adicionales en ambos archivos de conciliación basada en uso y en licencia para realizar el desglose por revendedor.</span><span class="sxs-lookup"><span data-stu-id="f2a43-110">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f2a43-111">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="f2a43-111">MPN ID</span></span></th>
<th><span data-ttu-id="f2a43-112">Descripción</span><span class="sxs-lookup"><span data-stu-id="f2a43-112">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="f2a43-113">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="f2a43-113">MPN ID</span></span></td>
<td><p><span data-ttu-id="f2a43-114">Id. de Microsoft Partner Network (MPN) del partner de CSP (directo o indirecto).</span><span class="sxs-lookup"><span data-stu-id="f2a43-114">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-115">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="f2a43-115">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="f2a43-116">Solo aparece en los archivos de conciliación de partners en el modelo indirecto.</span><span class="sxs-lookup"><span data-stu-id="f2a43-116">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="f2a43-117">El Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="f2a43-117">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f2a43-118">Corresponde al id. de revendedor indicado para la suscripción específica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="f2a43-118">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="f2a43-119">muestra de eTo o actualiza el distribuidor, en el menú del centro de partners, seleccione <strong>clientes</strong>, a continuación, elija el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="f2a43-119">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="f2a43-120">En el menú del cliente, selecciona <strong>Suscripciones</strong> y elige la suscripción de la lista.</span><span class="sxs-lookup"><span data-stu-id="f2a43-120">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="f2a43-121">Selecciona <strong>Actualizar</strong> para cambiar el valor de <strong>Revendedor (id. de MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="f2a43-121">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="f2a43-122">Si un partner CSP vendió la suscripción directamente al cliente, su id. de MPN aparece dos veces, como id. de MPN y como id. de MPN del revendedor.</span><span class="sxs-lookup"><span data-stu-id="f2a43-122">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="f2a43-123">Si un partner CSP tiene un revendedor sin un id. de MPN, este valor se establece en el id. de MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="f2a43-123">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="f2a43-124">Si el partner CSP quita un id. de revendedor, este valor se establece en -1.</span><span class="sxs-lookup"><span data-stu-id="f2a43-124">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="f2a43-125">Campos de archivo de licencia</span><span class="sxs-lookup"><span data-stu-id="f2a43-125">License-based file fields</span></span>


<span data-ttu-id="f2a43-126">Para conciliar los cargos en función de los pedidos del cliente, compara el Syndication\_Partner\_Subscription\_Number del archivo de conciliación con el id. de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="f2a43-126">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="f2a43-127"><strong>Columna</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-127"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="f2a43-128"><strong>Descripción</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-128"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="f2a43-129"><strong>Valor de ejemplo</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-129"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-130">PartnerId</span><span class="sxs-lookup"><span data-stu-id="f2a43-130">PartnerId</span></span></td>
<td><p><span data-ttu-id="f2a43-131">Identificador único de una entidad de facturación específica, con formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="f2a43-131">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="f2a43-132">No es necesario para la reconciliación, pero puede ser información útil.</span><span class="sxs-lookup"><span data-stu-id="f2a43-132">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="f2a43-133">Igual en todas las filas.</span><span class="sxs-lookup"><span data-stu-id="f2a43-133">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="f2a43-134">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="f2a43-134">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-135">CustomerID</span><span class="sxs-lookup"><span data-stu-id="f2a43-135">CustomerID</span></span></td>
<td><p><span data-ttu-id="f2a43-136">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="f2a43-136">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="f2a43-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="f2a43-137">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-138">OrderID</span><span class="sxs-lookup"><span data-stu-id="f2a43-138">OrderID</span></span></td>
<td><p><span data-ttu-id="f2a43-139">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f2a43-139">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="f2a43-140">Puede ser útil para identificar al pedido al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-140">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="f2a43-141">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="f2a43-141">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-142">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="f2a43-142">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="f2a43-143">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f2a43-143">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="f2a43-144">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-144">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="f2a43-145">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="f2a43-145">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="f2a43-146">Consulte Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="f2a43-146">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="f2a43-147">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="f2a43-147">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-148">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="f2a43-148">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="f2a43-149">Identificador único de las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="f2a43-149">Unique identifier for subscriptions.</span></span> <span data-ttu-id="f2a43-150">Un cliente puede tener varias suscripciones para el mismo plan, por lo que es importante para el análisis de archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-150">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="f2a43-151">Este campo se asigna al identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="f2a43-151">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="f2a43-152">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="f2a43-152">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-153">OfferID</span><span class="sxs-lookup"><span data-stu-id="f2a43-153">OfferID</span></span></td>
<td><p><span data-ttu-id="f2a43-154">Identificador único de la oferta.</span><span class="sxs-lookup"><span data-stu-id="f2a43-154">Unique offer ID.</span></span> <span data-ttu-id="f2a43-155">Identificador de la oferta estándar según la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="f2a43-155">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="f2a43-156"><b>Nota</b>: Este valor no coincide con Id. de oferta desde la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="f2a43-156"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="f2a43-157">Consulta DurableOfferID a continuación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-157">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="f2a43-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="f2a43-158">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-159">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="f2a43-159">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="f2a43-160">Identificador único de oferta duradera, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="f2a43-160">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="f2a43-161"><b>Nota</b>: Este valor coincide con el Id. de oferta desde la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="f2a43-161"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="f2a43-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="f2a43-162">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-163">OfferName</span><span class="sxs-lookup"><span data-stu-id="f2a43-163">OfferName</span></span></td>
<td><p><span data-ttu-id="f2a43-164">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="f2a43-164">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="f2a43-165">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="f2a43-165">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-166">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="f2a43-166">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="f2a43-167">Fecha de finalización de la suscripción, establecida en el día posterior al envío del pedido.</span><span class="sxs-lookup"><span data-stu-id="f2a43-167">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="f2a43-168">Al consultar la fecha de inicio de la suscripción junto con la fecha de finalización, puedes determinar si el cliente aún está dentro del primer año de la suscripción o si la suscripción se ha renovado para el año siguiente.</span><span class="sxs-lookup"><span data-stu-id="f2a43-168">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="f2a43-169">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="f2a43-169">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f2a43-170">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="f2a43-170">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-171">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="f2a43-171">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="f2a43-172">La fecha de finalización de la suscripción: 12 meses + x días después de la fecha de inicio (para alinearse con fecha de facturación del asociado) o 12 meses a partir de la fecha de renovación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-172">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="f2a43-173">En el momento de la renovación, los precios se actualizan según la lista de precios actual.</span><span class="sxs-lookup"><span data-stu-id="f2a43-173">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="f2a43-174">Es posible que se necesite una comunicación con el cliente antes de la renovación automatizada.</span><span class="sxs-lookup"><span data-stu-id="f2a43-174">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="f2a43-175">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="f2a43-175">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f2a43-176">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="f2a43-176">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-177">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f2a43-177">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f2a43-178">Día de inicio de los cargos.</span><span class="sxs-lookup"><span data-stu-id="f2a43-178">Start day of the charges.</span></span></p>
<p><span data-ttu-id="f2a43-179">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="f2a43-179">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="f2a43-180">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="f2a43-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f2a43-181">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="f2a43-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-182">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f2a43-182">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f2a43-183">Día de finalización de los cargos.</span><span class="sxs-lookup"><span data-stu-id="f2a43-183">End day of the charges.</span></span></p>
<p><span data-ttu-id="f2a43-184">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="f2a43-184">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="f2a43-185">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="f2a43-185">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="f2a43-186">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="f2a43-186">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-187">ChargeType</span><span class="sxs-lookup"><span data-stu-id="f2a43-187">ChargeType</span></span></td>
<td><p><span data-ttu-id="f2a43-188">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="f2a43-188">The type of charge or adjustment.</span></span> <span data-ttu-id="f2a43-189">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="f2a43-189">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="f2a43-190">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="f2a43-190">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-191">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="f2a43-191">UnitPrice</span></span></td>
<td><p><span data-ttu-id="f2a43-192">Precio por puesto, tal y como se publica en la lista de precios en el momento de compra.</span><span class="sxs-lookup"><span data-stu-id="f2a43-192">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="f2a43-193">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-193">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="f2a43-194">6.82</span><span class="sxs-lookup"><span data-stu-id="f2a43-194">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-195">Cantidad</span><span class="sxs-lookup"><span data-stu-id="f2a43-195">Quantity</span></span></td>
<td><p><span data-ttu-id="f2a43-196">Número de puestos.</span><span class="sxs-lookup"><span data-stu-id="f2a43-196">Number of seats.</span></span> <span data-ttu-id="f2a43-197">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-197">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="f2a43-198">2</span><span class="sxs-lookup"><span data-stu-id="f2a43-198">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-199">Volumen</span><span class="sxs-lookup"><span data-stu-id="f2a43-199">Amount</span></span></td>
<td><p><span data-ttu-id="f2a43-200">Total del precio para la cantidad.</span><span class="sxs-lookup"><span data-stu-id="f2a43-200">Total of price for quantity.</span></span> <span data-ttu-id="f2a43-201">Es de utilidad para comprobar que el cálculo de la cantidad coincide con la manera de calcular este valor para los clientes.</span><span class="sxs-lookup"><span data-stu-id="f2a43-201">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="f2a43-202">13.32</span><span class="sxs-lookup"><span data-stu-id="f2a43-202">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-203">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="f2a43-203">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="f2a43-204">Cantidad de descuento que se aplica a estos cargos.</span><span class="sxs-lookup"><span data-stu-id="f2a43-204">Amount of discount applied to these charges.</span></span> <span data-ttu-id="f2a43-205">Los IUR o las nuevas suscripciones que puedan optar a un incentivo también incluirán un importe de descuento en esta columna.</span><span class="sxs-lookup"><span data-stu-id="f2a43-205">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="f2a43-206">2.32</span><span class="sxs-lookup"><span data-stu-id="f2a43-206">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-207">Subtotal</span><span class="sxs-lookup"><span data-stu-id="f2a43-207">Subtotal</span></span></td>
<td><p><span data-ttu-id="f2a43-208">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="f2a43-208">Total before tax.</span></span> <span data-ttu-id="f2a43-209">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="f2a43-209">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="f2a43-210">11</span><span class="sxs-lookup"><span data-stu-id="f2a43-210">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-211">Impuestos</span><span class="sxs-lookup"><span data-stu-id="f2a43-211">Tax</span></span></td>
<td><p><span data-ttu-id="f2a43-212">Importe de impuestos, según el mercado&#39;reglas s y circunstancias concretas.</span><span class="sxs-lookup"><span data-stu-id="f2a43-212">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="f2a43-213">0</span><span class="sxs-lookup"><span data-stu-id="f2a43-213">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-214">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="f2a43-214">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="f2a43-215">Total con impuestos.</span><span class="sxs-lookup"><span data-stu-id="f2a43-215">Total after tax.</span></span> <span data-ttu-id="f2a43-216">Comprueba si se cobran impuestos en la factura.</span><span class="sxs-lookup"><span data-stu-id="f2a43-216">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="f2a43-217">11</span><span class="sxs-lookup"><span data-stu-id="f2a43-217">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-218">Moneda</span><span class="sxs-lookup"><span data-stu-id="f2a43-218">Currency</span></span></td>
<td><p><span data-ttu-id="f2a43-219">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="f2a43-219">Currency type.</span></span> <span data-ttu-id="f2a43-220">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="f2a43-220">Each billing entity has only one currency.</span></span> <span data-ttu-id="f2a43-221">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-221">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="f2a43-222">EUR</span><span class="sxs-lookup"><span data-stu-id="f2a43-222">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-223">CustomerName</span><span class="sxs-lookup"><span data-stu-id="f2a43-223">CustomerName</span></span></td>
<td><p><span data-ttu-id="f2a43-224">Cliente&#39;nombre de la organización s notificados en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="f2a43-224">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="f2a43-225">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="f2a43-225">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="f2a43-226">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="f2a43-226">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-227">MPNID</span><span class="sxs-lookup"><span data-stu-id="f2a43-227">MPNID</span></span></td>
<td><p><span data-ttu-id="f2a43-228">Id. de MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="f2a43-228">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="f2a43-229">4390934</span><span class="sxs-lookup"><span data-stu-id="f2a43-229">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-230">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="f2a43-230">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="f2a43-231">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="f2a43-231">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f2a43-232">Ver <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Desglosar por partner</a></span><span class="sxs-lookup"><span data-stu-id="f2a43-232">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="f2a43-233">4390934</span><span class="sxs-lookup"><span data-stu-id="f2a43-233">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-234">DomainName</span><span class="sxs-lookup"><span data-stu-id="f2a43-234">DomainName</span></span></td>
<td><p><span data-ttu-id="f2a43-235">Cliente&#39;nombre de dominio de s, que ayuda a identificar el cliente.</span><span class="sxs-lookup"><span data-stu-id="f2a43-235">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="f2a43-236">No debe usarse para identificar al cliente como el cliente o socio puede actualizar el dominio personal de forma predeterminada a través del portal de Office 365.</span><span class="sxs-lookup"><span data-stu-id="f2a43-236">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="f2a43-237">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-237">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="f2a43-238">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="f2a43-238">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-239">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="f2a43-239">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="f2a43-240">Alias de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="f2a43-240">Subscription nickname.</span></span> <span data-ttu-id="f2a43-241">Si no se especifica ningún alias, el Centro de partners usa OfferName.</span><span class="sxs-lookup"><span data-stu-id="f2a43-241">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="f2a43-242">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="f2a43-242">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-243">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="f2a43-243">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="f2a43-244">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="f2a43-244">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="f2a43-245">(Este es un campo idéntico al nombre de la oferta).</span><span class="sxs-lookup"><span data-stu-id="f2a43-245">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="f2a43-246">PROJECT ONLINE PREMIUM SIN CLIENTE DE PROJECT</span><span class="sxs-lookup"><span data-stu-id="f2a43-246">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="f2a43-247">Campos de archivo basada en uso</span><span class="sxs-lookup"><span data-stu-id="f2a43-247">Usage-based file fields</span></span>


<span data-ttu-id="f2a43-248">Para conciliar los cargos en función del uso de tu cliente, compara los valores de ResellerID/ResellerName/ResellerBillableAccount del archivo de conciliación, el nombre del cliente y el id. de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="f2a43-248">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="f2a43-249">Los siguientes campos explican los servicios usados y la clasificación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-249">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="f2a43-250"><strong>Columna</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-250"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="f2a43-251"><strong>Descripción</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-251"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="f2a43-252"><strong>Valor de ejemplo</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-252"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-253">PartnerID</span><span class="sxs-lookup"><span data-stu-id="f2a43-253">PartnerID</span></span></td>
<td><p><span data-ttu-id="f2a43-254">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="f2a43-254">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="f2a43-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="f2a43-255">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-256">PartnerName</span><span class="sxs-lookup"><span data-stu-id="f2a43-256">PartnerName</span></span></td>
<td><p><span data-ttu-id="f2a43-257">Nombre del partner.</span><span class="sxs-lookup"><span data-stu-id="f2a43-257">Partner Name.</span></span></p></td>
<td><span data-ttu-id="f2a43-258">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="f2a43-258">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-259">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="f2a43-259">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="f2a43-260">Id. de cuenta del partner.</span><span class="sxs-lookup"><span data-stu-id="f2a43-260">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="f2a43-261">1010578050</span><span class="sxs-lookup"><span data-stu-id="f2a43-261">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-262">CustomerName</span><span class="sxs-lookup"><span data-stu-id="f2a43-262">CustomerName</span></span></td>
<td><p><span data-ttu-id="f2a43-263">Cliente&#39;nombre de la organización s notificados en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="f2a43-263">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="f2a43-264">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="f2a43-264">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="f2a43-265">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="f2a43-265">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-266">MPNID</span><span class="sxs-lookup"><span data-stu-id="f2a43-266">MPNID</span></span></td>
<td><p><span data-ttu-id="f2a43-267">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="f2a43-267">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="f2a43-268">4390934</span><span class="sxs-lookup"><span data-stu-id="f2a43-268">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-269">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="f2a43-269">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="f2a43-270">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="f2a43-270">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f2a43-271">Ver <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Desglosar por partner</a></span><span class="sxs-lookup"><span data-stu-id="f2a43-271">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="f2a43-272">4390934</span><span class="sxs-lookup"><span data-stu-id="f2a43-272">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-273">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="f2a43-273">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="f2a43-274">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="f2a43-274">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="f2a43-275">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="f2a43-275">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-276">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f2a43-276">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f2a43-277">Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="f2a43-277">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="f2a43-278">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="f2a43-278">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="f2a43-279">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="f2a43-279">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-280">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f2a43-280">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f2a43-281">Fecha de finalización del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="f2a43-281">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="f2a43-282">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="f2a43-282">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="f2a43-283">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="f2a43-283">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-284">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="f2a43-284">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="f2a43-285">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f2a43-285">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="f2a43-286">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-286">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="f2a43-287">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="f2a43-287">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="f2a43-288">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="f2a43-288">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-289">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="f2a43-289">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="f2a43-290">Alias de la oferta de servicio.</span><span class="sxs-lookup"><span data-stu-id="f2a43-290">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="f2a43-291">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="f2a43-291">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-292">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="f2a43-292">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="f2a43-293">Línea de negocio de la oferta de servicio</span><span class="sxs-lookup"><span data-stu-id="f2a43-293">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="f2a43-294">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="f2a43-294">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-295">OrderID</span><span class="sxs-lookup"><span data-stu-id="f2a43-295">OrderID</span></span></td>
<td><p><span data-ttu-id="f2a43-296">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f2a43-296">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="f2a43-297">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="f2a43-298">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="f2a43-298">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-299">ServiceName</span><span class="sxs-lookup"><span data-stu-id="f2a43-299">ServiceName</span></span></td>
<td><p><span data-ttu-id="f2a43-300">Nombre del servicio de Azure en cuestión.</span><span class="sxs-lookup"><span data-stu-id="f2a43-300">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="f2a43-301">MÁQUINAS VIRTUALES</span><span class="sxs-lookup"><span data-stu-id="f2a43-301">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-302">ServiceType</span><span class="sxs-lookup"><span data-stu-id="f2a43-302">ServiceType</span></span></td>
<td><p><span data-ttu-id="f2a43-303">Tipo específico de servicio de Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="f2a43-303">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="f2a43-304">Bus de servicio: individual o paquete</span><span class="sxs-lookup"><span data-stu-id="f2a43-304">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="f2a43-305">Base de datos SQL Azure: edición Business o Web</span><span class="sxs-lookup"><span data-stu-id="f2a43-305">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-306">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="f2a43-306">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="f2a43-307">Identificador único específico para toda la estructura de precios y datos del servicio.</span><span class="sxs-lookup"><span data-stu-id="f2a43-307">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="f2a43-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="f2a43-308">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-309">Nombre de recurso</span><span class="sxs-lookup"><span data-stu-id="f2a43-309">Resource Name</span></span></td>
<td><p><span data-ttu-id="f2a43-310">Nombre del recurso de Azure.</span><span class="sxs-lookup"><span data-stu-id="f2a43-310">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="f2a43-311">Transferencia entrante de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="f2a43-311">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="f2a43-312">Transferencia saliente de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="f2a43-312">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-313">Region</span><span class="sxs-lookup"><span data-stu-id="f2a43-313">Region</span></span></td>
<td><p><span data-ttu-id="f2a43-314">La región a la que se aplica el uso.</span><span class="sxs-lookup"><span data-stu-id="f2a43-314">The region the usage applies to.</span></span> <span data-ttu-id="f2a43-315">Se usa principalmente para asignar tarifas a las transferencias de datos, ya que las tarifas varían según la región.</span><span class="sxs-lookup"><span data-stu-id="f2a43-315">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="f2a43-316">Asia Pacífico, Europa, América Latina, América del Norte</span><span class="sxs-lookup"><span data-stu-id="f2a43-316">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-317">SKU</span><span class="sxs-lookup"><span data-stu-id="f2a43-317">SKU</span></span></td>
<td><p><span data-ttu-id="f2a43-318">Identificador único de MSFT para la oferta</span><span class="sxs-lookup"><span data-stu-id="f2a43-318">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="f2a43-319">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="f2a43-319">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="f2a43-320">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="f2a43-320">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="f2a43-321">Un id. y una cantidad para desglosar las distintas clasificaciones de un servicio o un recurso en un período de facturación determinado.</span><span class="sxs-lookup"><span data-stu-id="f2a43-321">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="f2a43-322">Para clasificación en niveles de Azure, puede haber una clasificación hasta una cantidad determinada de unidades facturables y, posteriormente, una clasificación diferente.</span><span class="sxs-lookup"><span data-stu-id="f2a43-322">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="f2a43-323">1</span><span class="sxs-lookup"><span data-stu-id="f2a43-323">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-324">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="f2a43-324">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="f2a43-325">La cantidad de servicio consumida (horas, GB, etc.) durante el período de notificación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-325">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="f2a43-326">También incluye cualquier uso no facturado de períodos anteriores.</span><span class="sxs-lookup"><span data-stu-id="f2a43-326">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="f2a43-327">11</span><span class="sxs-lookup"><span data-stu-id="f2a43-327">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-328">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="f2a43-328">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="f2a43-329">Unidades que se incluyen como parte de la oferta.</span><span class="sxs-lookup"><span data-stu-id="f2a43-329">Units included as part of the offer.</span></span> <span data-ttu-id="f2a43-330">No suele mostrarse en CSP.</span><span class="sxs-lookup"><span data-stu-id="f2a43-330">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="f2a43-331">0</span><span class="sxs-lookup"><span data-stu-id="f2a43-331">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="f2a43-332">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="f2a43-332">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="f2a43-333">Unidades que no se incluyen como parte de la oferta y que el partner debe abonar.</span><span class="sxs-lookup"><span data-stu-id="f2a43-333">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="f2a43-334">Equivale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="f2a43-334">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="f2a43-335">11</span><span class="sxs-lookup"><span data-stu-id="f2a43-335">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-336">ListPrice</span><span class="sxs-lookup"><span data-stu-id="f2a43-336">ListPrice</span></span></td>
<td><p><span data-ttu-id="f2a43-337">Precio de la oferta en vigor la fecha de inicio de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="f2a43-337">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="f2a43-338">0.0808 USD</span><span class="sxs-lookup"><span data-stu-id="f2a43-338">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-339">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="f2a43-339">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="f2a43-340">ListPrist x OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="f2a43-340">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="f2a43-341">0.085 USD</span><span class="sxs-lookup"><span data-stu-id="f2a43-341">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-342">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="f2a43-342">TaxAmount</span></span></td>
<td><p><span data-ttu-id="f2a43-343">Importe de impuestos, según el mercado&#39;reglas s y circunstancias concretas.</span><span class="sxs-lookup"><span data-stu-id="f2a43-343">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="f2a43-344">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="f2a43-344">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-345">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="f2a43-345">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="f2a43-346">Total con impuestos, si se aplican impuestos.</span><span class="sxs-lookup"><span data-stu-id="f2a43-346">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="f2a43-347">0.93 USD</span><span class="sxs-lookup"><span data-stu-id="f2a43-347">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-348">Moneda</span><span class="sxs-lookup"><span data-stu-id="f2a43-348">Currency</span></span></td>
<td><p><span data-ttu-id="f2a43-349">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="f2a43-349">Currency type.</span></span> <span data-ttu-id="f2a43-350">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="f2a43-350">Each billing entity has only one currency.</span></span> <span data-ttu-id="f2a43-351">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-351">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="f2a43-352">EUR</span><span class="sxs-lookup"><span data-stu-id="f2a43-352">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-353">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="f2a43-353">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="f2a43-354">Precio sin impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="f2a43-354">Pretax price per unit.</span></span> <span data-ttu-id="f2a43-355">Igual que PretaxCharges/OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="f2a43-355">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="f2a43-356">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="f2a43-356">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-357">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="f2a43-357">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="f2a43-358">Precio después de impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="f2a43-358">Post tax price per unit.</span></span> <span data-ttu-id="f2a43-359">Igual que PostTaxTotal/OverageQuantity o PretaxEffectiveRate + tipo impositivo por importe unitario, redondeado el céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="f2a43-359">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="f2a43-360">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="f2a43-360">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-361">ChargeType</span><span class="sxs-lookup"><span data-stu-id="f2a43-361">ChargeType</span></span></td>
<td><p><span data-ttu-id="f2a43-362">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="f2a43-362">The type of charge or adjustment.</span></span> <span data-ttu-id="f2a43-363">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="f2a43-363">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="f2a43-364">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="f2a43-364">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-365">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="f2a43-365">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="f2a43-366">Id. de cuenta único en la plataforma de facturación de MSFT.</span><span class="sxs-lookup"><span data-stu-id="f2a43-366">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="f2a43-367">1280018095</span><span class="sxs-lookup"><span data-stu-id="f2a43-367">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-368">UsageDate</span><span class="sxs-lookup"><span data-stu-id="f2a43-368">UsageDate</span></span></td>
<td><p><span data-ttu-id="f2a43-369">Fecha de implementación del servicio.</span><span class="sxs-lookup"><span data-stu-id="f2a43-369">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="f2a43-370">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="f2a43-370">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-371">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="f2a43-371">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="f2a43-372">Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena.</span><span class="sxs-lookup"><span data-stu-id="f2a43-372">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="f2a43-373">Asia oriental, Sur asiático, Norte de Europa, Europa occidental, Norte central de EE. UU., Sur central de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="f2a43-373">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-374">MeteredService</span><span class="sxs-lookup"><span data-stu-id="f2a43-374">MeteredService</span></span></td>
<td><p><span data-ttu-id="f2a43-375">Esta columna se usa para hacer un seguimiento de los servicios de Microsoft Azure individuales que quizás no se identifiquen específicamente en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="f2a43-375">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="f2a43-376">Por ejemplo, las transferencias de datos se notifican como &quot;Microsoft Azure: todos los servicios&quot; en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="f2a43-376">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="f2a43-377">En esta columna MeteredService se indicará qué servicio específico pertenece el uso.</span><span class="sxs-lookup"><span data-stu-id="f2a43-377">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="f2a43-378">AccessControl, CDN, Proceso, Base de datos, ServiceBus, Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="f2a43-378">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-379">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="f2a43-379">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="f2a43-380">Subtítulo que aclara el servicio de Microsoft Azure individual más allá del nivel proporcionado por el campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="f2a43-380">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="f2a43-381">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="f2a43-381">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-382">Proyecto</span><span class="sxs-lookup"><span data-stu-id="f2a43-382">Project</span></span></td>
<td><p><span data-ttu-id="f2a43-383">Nombre definido por el cliente para la instancia del servicio</span><span class="sxs-lookup"><span data-stu-id="f2a43-383">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="f2a43-384">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="f2a43-384">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-385">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="f2a43-385">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="f2a43-386">Número de conexiones de Bus de servicio aprovisionadas y usadas en un día determinado.</span><span class="sxs-lookup"><span data-stu-id="f2a43-386">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="f2a43-387">Por ejemplo: si tenías una conexión aprovisionada individualmente durante un mes de 30 días, Service Info 1 contendría 1 "1,000000 conexiones/30 días".</span><span class="sxs-lookup"><span data-stu-id="f2a43-387">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="f2a43-388">Si tuviera un paquete de 25 de conexiones de bus de servicio aprovisionada y ha utilizado 1 durante ese día, el extracto de uso diario durante ese día indicaría "25 conexiones / 30 días: utilizado: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="f2a43-388">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-389">CustomerID</span><span class="sxs-lookup"><span data-stu-id="f2a43-389">CustomerID</span></span></td>
<td><p><span data-ttu-id="f2a43-390">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="f2a43-390">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="f2a43-391">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="f2a43-391">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="f2a43-392">DomainName</span><span class="sxs-lookup"><span data-stu-id="f2a43-392">DomainName</span></span></td>
<td><p><span data-ttu-id="f2a43-393">Cliente&#39;nombre de dominio de s, que ayuda a identificar el cliente.</span><span class="sxs-lookup"><span data-stu-id="f2a43-393">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="f2a43-394">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-394">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="f2a43-395">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="f2a43-395">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="f2a43-396">Unidad</span><span class="sxs-lookup"><span data-stu-id="f2a43-396">Unit</span></span></td>
<td><p><span data-ttu-id="f2a43-397">La unidad del nombre del recurso</span><span class="sxs-lookup"><span data-stu-id="f2a43-397">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="f2a43-398">GB u HORAS</span><span class="sxs-lookup"><span data-stu-id="f2a43-398">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="f2a43-399">Campos del archivo periódicas y únicas</span><span class="sxs-lookup"><span data-stu-id="f2a43-399">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f2a43-400">Column</span><span class="sxs-lookup"><span data-stu-id="f2a43-400">Column</span></span></th>
<th><span data-ttu-id="f2a43-401">Descripción</span><span class="sxs-lookup"><span data-stu-id="f2a43-401">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="f2a43-402">PartnerId</span><span class="sxs-lookup"><span data-stu-id="f2a43-402">PartnerId</span></span></td>
<td><p><span data-ttu-id="f2a43-403">Identificador único del inquilino de Microsoft Azure Active Directory para una entidad de facturación específica, en formato GUID.</span><span class="sxs-lookup"><span data-stu-id="f2a43-403">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="f2a43-404">No es necesario para la reconciliación, pero puede ser información útil.</span><span class="sxs-lookup"><span data-stu-id="f2a43-404">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="f2a43-405">Igual en todas las filas.</span><span class="sxs-lookup"><span data-stu-id="f2a43-405">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-406">Id. de cliente</span><span class="sxs-lookup"><span data-stu-id="f2a43-406">Customer Id</span></span></td>
<td><p><span data-ttu-id="f2a43-407">Microsoft Azure Active Directory inquilino identificador único, en formato GUID, que usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="f2a43-407">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-408">Nombre del cliente</span><span class="sxs-lookup"><span data-stu-id="f2a43-408">Customer Name</span></span></td>
<td><p><span data-ttu-id="f2a43-409">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="f2a43-409">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-410">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="f2a43-410">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="f2a43-411">Nombre de dominio del cliente, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="f2a43-411">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="f2a43-412">No debe usarse para identificar al cliente como el cliente o socio puede actualizar el dominio personal de forma predeterminada a través del portal de Office 365.</span><span class="sxs-lookup"><span data-stu-id="f2a43-412">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="f2a43-413">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-413">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-414">País del cliente</span><span class="sxs-lookup"><span data-stu-id="f2a43-414">Customer Country</span></span></td>
<td><p><span data-ttu-id="f2a43-415">El país donde se encuentra el cliente.</span><span class="sxs-lookup"><span data-stu-id="f2a43-415">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-416">Número de factura</span><span class="sxs-lookup"><span data-stu-id="f2a43-416">Invoice number</span></span></td>
<td><p><span data-ttu-id="f2a43-417">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="f2a43-417">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-418">MpnId</span><span class="sxs-lookup"><span data-stu-id="f2a43-418">MpnId</span></span></td>
<td><p><span data-ttu-id="f2a43-419">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="f2a43-419">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-420">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="f2a43-420">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="f2a43-421">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="f2a43-421">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-422">Id. de pedido</span><span class="sxs-lookup"><span data-stu-id="f2a43-422">Order ID</span></span></td>
<td><p><span data-ttu-id="f2a43-423">Identificador único para un pedido en la plataforma de comercio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f2a43-423">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="f2a43-424">Puede ser útil para identificar al pedido al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-424">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-425">Fecha del pedido</span><span class="sxs-lookup"><span data-stu-id="f2a43-425">Order date</span></span></td>
<td><p><span data-ttu-id="f2a43-426">Fecha de realización del pedido.</span><span class="sxs-lookup"><span data-stu-id="f2a43-426">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-427">ProductId</span><span class="sxs-lookup"><span data-stu-id="f2a43-427">ProductId</span></span></td>
<td><p><span data-ttu-id="f2a43-428">Identificador del producto.</span><span class="sxs-lookup"><span data-stu-id="f2a43-428">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-429">SkuId</span><span class="sxs-lookup"><span data-stu-id="f2a43-429">SkuId</span></span></td>
<td><p><span data-ttu-id="f2a43-430">Id. de un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="f2a43-430">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-431">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="f2a43-431">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="f2a43-432">Id. de una disponibilidad concreta.</span><span class="sxs-lookup"><span data-stu-id="f2a43-432">The ID for a particular Availability.</span></span> <span data-ttu-id="f2a43-433">"Disponibilidad" hace referencia a si un SKU concreto está o no disponible para su compra para el país, la moneda, el segmento industrial determinados, etc.</span><span class="sxs-lookup"><span data-stu-id="f2a43-433">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-434">Nombre de SKU</span><span class="sxs-lookup"><span data-stu-id="f2a43-434">SKU Name</span></span></td>
<td><p><span data-ttu-id="f2a43-435">Título para un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="f2a43-435">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-436">Nombre del producto</span><span class="sxs-lookup"><span data-stu-id="f2a43-436">Product name</span></span></td>
<td><p><span data-ttu-id="f2a43-437">Nombre del producto.</span><span class="sxs-lookup"><span data-stu-id="f2a43-437">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-438">PublisherName</span><span class="sxs-lookup"><span data-stu-id="f2a43-438">PublisherName</span></span></td>
<td><p><span data-ttu-id="f2a43-439">El nombre del publicador del producto.</span><span class="sxs-lookup"><span data-stu-id="f2a43-439">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-440">PublisherID</span><span class="sxs-lookup"><span data-stu-id="f2a43-440">PublisherID</span></span></td>
<td><p><span data-ttu-id="f2a43-441">Identificador único para este publicador.</span><span class="sxs-lookup"><span data-stu-id="f2a43-441">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-442">Descripción de la suscripción</span><span class="sxs-lookup"><span data-stu-id="f2a43-442">Subscription Description</span></span></td>
<td><p><span data-ttu-id="f2a43-443">Nombre descriptivo de una suscripción.</span><span class="sxs-lookup"><span data-stu-id="f2a43-443">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-444">Id. de la suscripción</span><span class="sxs-lookup"><span data-stu-id="f2a43-444">Subscription ID</span></span></td>
<td><p><span data-ttu-id="f2a43-445">Identificador único para una suscripción en la plataforma de comercio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f2a43-445">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="f2a43-446">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-446">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="f2a43-447">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="f2a43-447">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-448">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f2a43-448">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f2a43-449">Día de inicio de los cargos.</span><span class="sxs-lookup"><span data-stu-id="f2a43-449">Start day of the charges.</span></span> <span data-ttu-id="f2a43-450">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="f2a43-450">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-451">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f2a43-451">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f2a43-452">Día de finalización de los cargos.</span><span class="sxs-lookup"><span data-stu-id="f2a43-452">End day of the charges.</span></span> <span data-ttu-id="f2a43-453">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="f2a43-453">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-454">Término y Billingcycle</span><span class="sxs-lookup"><span data-stu-id="f2a43-454">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="f2a43-455">La duración del período y ciclo de facturación para la compra.</span><span class="sxs-lookup"><span data-stu-id="f2a43-455">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="f2a43-456">Por ejemplo, "1 año, mes".</span><span class="sxs-lookup"><span data-stu-id="f2a43-456">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-457">Tipo de cargo</span><span class="sxs-lookup"><span data-stu-id="f2a43-457">Charge Type</span></span></td>
<td><p><span data-ttu-id="f2a43-458">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="f2a43-458">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-459">Precio unitario</span><span class="sxs-lookup"><span data-stu-id="f2a43-459">Unit Price</span></span></td>
<td><p><span data-ttu-id="f2a43-460">El precio publicado en la lista de precios en el momento de la compra.</span><span class="sxs-lookup"><span data-stu-id="f2a43-460">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="f2a43-461">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-461">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-462">Precio unitario efectivo</span><span class="sxs-lookup"><span data-stu-id="f2a43-462">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="f2a43-463">El precio por unidad una vez realizados los ajustes.</span><span class="sxs-lookup"><span data-stu-id="f2a43-463">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-464">Cantidad</span><span class="sxs-lookup"><span data-stu-id="f2a43-464">Quantity</span></span></td>
<td><p><span data-ttu-id="f2a43-465">Número de unidades.</span><span class="sxs-lookup"><span data-stu-id="f2a43-465">Number of units.</span></span> <span data-ttu-id="f2a43-466">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-466">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-467">Tipo de unidad</span><span class="sxs-lookup"><span data-stu-id="f2a43-467">Unit type</span></span></td>
<td><p><span data-ttu-id="f2a43-468">El tipo de unidad que se compra.</span><span class="sxs-lookup"><span data-stu-id="f2a43-468">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-469">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="f2a43-469">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="f2a43-470">Explicación de los descuentos aplicables.</span><span class="sxs-lookup"><span data-stu-id="f2a43-470">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-471">Subtotal</span><span class="sxs-lookup"><span data-stu-id="f2a43-471">Sub Total</span></span></td>
<td><p><span data-ttu-id="f2a43-472">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="f2a43-472">Total before tax.</span></span> <span data-ttu-id="f2a43-473">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="f2a43-473">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-474">Total de impuestos</span><span class="sxs-lookup"><span data-stu-id="f2a43-474">Tax Total</span></span></td>
<td><p><span data-ttu-id="f2a43-475">Cargo por importe de impuestos, en función de las reglas fiscales de tu mercado y las circunstancias específicas.</span><span class="sxs-lookup"><span data-stu-id="f2a43-475">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-476">Total</span><span class="sxs-lookup"><span data-stu-id="f2a43-476">Total</span></span></td>
<td><p><span data-ttu-id="f2a43-477">Total con impuestos.</span><span class="sxs-lookup"><span data-stu-id="f2a43-477">Total after tax.</span></span> <span data-ttu-id="f2a43-478">Comprueba si se cobran impuestos en la factura.</span><span class="sxs-lookup"><span data-stu-id="f2a43-478">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-479">Moneda</span><span class="sxs-lookup"><span data-stu-id="f2a43-479">Currency</span></span></td>
<td><p><span data-ttu-id="f2a43-480">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="f2a43-480">Currency type.</span></span> <span data-ttu-id="f2a43-481">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="f2a43-481">Each billing entity has only one currency.</span></span> <span data-ttu-id="f2a43-482">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-482">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-483">AlternateID</span><span class="sxs-lookup"><span data-stu-id="f2a43-483">AlternateID</span></span></td>
<td><p><span data-ttu-id="f2a43-484">Un identificador alternativo para un identificador.</span><span class="sxs-lookup"><span data-stu-id="f2a43-484">An alternate identifier to an ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="f2a43-485">Campos del archivo de uso diario calificados</span><span class="sxs-lookup"><span data-stu-id="f2a43-485">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="f2a43-486">Column</span><span class="sxs-lookup"><span data-stu-id="f2a43-486">Column</span></span></th>
<th><span data-ttu-id="f2a43-487">Descripción</span><span class="sxs-lookup"><span data-stu-id="f2a43-487">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="f2a43-488">PartnerId</span><span class="sxs-lookup"><span data-stu-id="f2a43-488">PartnerId</span></span></td>
<td><p><span data-ttu-id="f2a43-489">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="f2a43-489">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-490">PartnerName</span><span class="sxs-lookup"><span data-stu-id="f2a43-490">PartnerName</span></span></td>
<td><p><span data-ttu-id="f2a43-491">Nombre del partner.</span><span class="sxs-lookup"><span data-stu-id="f2a43-491">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-492">CustomerId</span><span class="sxs-lookup"><span data-stu-id="f2a43-492">CustomerId</span></span></td>
<td><p><span data-ttu-id="f2a43-493">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="f2a43-493">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-494">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="f2a43-494">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="f2a43-495">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="f2a43-495">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="f2a43-496">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="f2a43-496">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-497">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="f2a43-497">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="f2a43-498">Nombre de dominio del cliente.</span><span class="sxs-lookup"><span data-stu-id="f2a43-498">The customer’s domain name.</span></span> <span data-ttu-id="f2a43-499">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="f2a43-499">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-500">País del cliente</span><span class="sxs-lookup"><span data-stu-id="f2a43-500">Customer country</span></span></td>
<td><p><span data-ttu-id="f2a43-501">El país donde se encuentra el cliente.</span><span class="sxs-lookup"><span data-stu-id="f2a43-501">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-502">MPNID</span><span class="sxs-lookup"><span data-stu-id="f2a43-502">MPNID</span></span></td>
<td><p><span data-ttu-id="f2a43-503">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="f2a43-503">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-504">Distribuidor MPNID</span><span class="sxs-lookup"><span data-stu-id="f2a43-504">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="f2a43-505">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="f2a43-505">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="f2a43-506">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="f2a43-506">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-507">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="f2a43-507">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="f2a43-508">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="f2a43-508">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="f2a43-509">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="f2a43-509">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-510">ProductId</span><span class="sxs-lookup"><span data-stu-id="f2a43-510">ProductId</span></span></td>
<td><p><span data-ttu-id="f2a43-511">Identificador del producto.</span><span class="sxs-lookup"><span data-stu-id="f2a43-511">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-512">SkuId</span><span class="sxs-lookup"><span data-stu-id="f2a43-512">SkuId</span></span></td>
<td><p><span data-ttu-id="f2a43-513">Id. de un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="f2a43-513">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-514">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="f2a43-514">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="f2a43-515">Id. de una disponibilidad concreta.</span><span class="sxs-lookup"><span data-stu-id="f2a43-515">The ID for a particular Availability.</span></span> <span data-ttu-id="f2a43-516">"Disponibilidad" hace referencia a si un SKU concreto está o no disponible para su compra para el país, la moneda, el segmento industrial determinados, etc.</span><span class="sxs-lookup"><span data-stu-id="f2a43-516">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-517">Nombre de SKU</span><span class="sxs-lookup"><span data-stu-id="f2a43-517">SKU Name</span></span></td>
<td><p><span data-ttu-id="f2a43-518">Título para un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="f2a43-518">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-519">PublisherName</span><span class="sxs-lookup"><span data-stu-id="f2a43-519">PublisherName</span></span></td>
<td><p><span data-ttu-id="f2a43-520">El nombre del publicador.</span><span class="sxs-lookup"><span data-stu-id="f2a43-520">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-521">PublisherID</span><span class="sxs-lookup"><span data-stu-id="f2a43-521">PublisherID</span></span></td>
<td><p><span data-ttu-id="f2a43-522">El identificador del publicador, en formato GUID.</span><span class="sxs-lookup"><span data-stu-id="f2a43-522">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="f2a43-523">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="f2a43-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="f2a43-524">Descripción de la suscripción</span><span class="sxs-lookup"><span data-stu-id="f2a43-524">Subscription Description</span></span></td>
<td><p><span data-ttu-id="f2a43-525">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="f2a43-525">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="f2a43-526">(Este es un campo idéntico al nombre de la oferta).</span><span class="sxs-lookup"><span data-stu-id="f2a43-526">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-527">Id. de la suscripción</span><span class="sxs-lookup"><span data-stu-id="f2a43-527">Subscription ID</span></span></td>
<td><p><span data-ttu-id="f2a43-528">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f2a43-528">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="f2a43-529">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-529">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="f2a43-530">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="f2a43-530">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-531">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="f2a43-531">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="f2a43-532">Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="f2a43-532">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="f2a43-533">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="f2a43-533">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-534">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="f2a43-534">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="f2a43-535">Fecha de finalización del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="f2a43-535">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="f2a43-536">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="f2a43-536">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-537">Fecha de uso</span><span class="sxs-lookup"><span data-stu-id="f2a43-537">Usage Date</span></span></td>
<td><p><span data-ttu-id="f2a43-538">Fecha de uso del servicio.</span><span class="sxs-lookup"><span data-stu-id="f2a43-538">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-539">Tipo de medidor</span><span class="sxs-lookup"><span data-stu-id="f2a43-539">Meter Type</span></span></td>
<td><p><span data-ttu-id="f2a43-540">El tipo de medidor.</span><span class="sxs-lookup"><span data-stu-id="f2a43-540">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-541">Categoría de medidor</span><span class="sxs-lookup"><span data-stu-id="f2a43-541">Meter Category</span></span></td>
<td><p><span data-ttu-id="f2a43-542">El servicio de nivel superior para el uso.</span><span class="sxs-lookup"><span data-stu-id="f2a43-542">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-543">Id. de medidor</span><span class="sxs-lookup"><span data-stu-id="f2a43-543">Meter Id</span></span></td>
<td><p><span data-ttu-id="f2a43-544">El identificador del medidor que se va a usar.</span><span class="sxs-lookup"><span data-stu-id="f2a43-544">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-545">Subcategoría de medidor</span><span class="sxs-lookup"><span data-stu-id="f2a43-545">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="f2a43-546">El tipo de servicio de Azure que puede afectar a la tarifa.</span><span class="sxs-lookup"><span data-stu-id="f2a43-546">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-547">Nombre de medidor</span><span class="sxs-lookup"><span data-stu-id="f2a43-547">Meter Name</span></span></td>
<td><p><span data-ttu-id="f2a43-548">La unidad de medida del medidor consumido.</span><span class="sxs-lookup"><span data-stu-id="f2a43-548">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-549">Región de medidor</span><span class="sxs-lookup"><span data-stu-id="f2a43-549">Meter Region</span></span></td>
<td><p><span data-ttu-id="f2a43-550">Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena.</span><span class="sxs-lookup"><span data-stu-id="f2a43-550">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-551">Unidad</span><span class="sxs-lookup"><span data-stu-id="f2a43-551">Unit</span></span></td>
<td><p><span data-ttu-id="f2a43-552">La unidad del nombre de recurso.</span><span class="sxs-lookup"><span data-stu-id="f2a43-552">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-553">Cantidad consumida</span><span class="sxs-lookup"><span data-stu-id="f2a43-553">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="f2a43-554">La cantidad de servicio consumida (horas, GB, etc.) durante el período de notificación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-554">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="f2a43-555">También incluye cualquier uso no facturado de períodos anteriores.</span><span class="sxs-lookup"><span data-stu-id="f2a43-555">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-556">Ubicación de recursos</span><span class="sxs-lookup"><span data-stu-id="f2a43-556">Resource Location</span></span></td>
<td><p><span data-ttu-id="f2a43-557">El centro de datos donde se está ejecutando el medidor.</span><span class="sxs-lookup"><span data-stu-id="f2a43-557">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-558">Servicio consumido</span><span class="sxs-lookup"><span data-stu-id="f2a43-558">Consumed Service</span></span></td>
<td><p><span data-ttu-id="f2a43-559">El servicio de la plataforma Azure que usó.</span><span class="sxs-lookup"><span data-stu-id="f2a43-559">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-560">Grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="f2a43-560">Resource Group</span></span></td>
<td><p><span data-ttu-id="f2a43-561">El grupo de recursos en el que se está ejecutando el medidor implementado.</span><span class="sxs-lookup"><span data-stu-id="f2a43-561">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-562">URI de recurso</span><span class="sxs-lookup"><span data-stu-id="f2a43-562">Resource URI</span></span></td>
<td><p><span data-ttu-id="f2a43-563">El URI del recurso que se va a usar.</span><span class="sxs-lookup"><span data-stu-id="f2a43-563">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-564">Tipo de cargo</span><span class="sxs-lookup"><span data-stu-id="f2a43-564">Charge type</span></span></td>
<td><p><span data-ttu-id="f2a43-565">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="f2a43-565">The type of charge or adjustment.</span></span> <span data-ttu-id="f2a43-566">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="f2a43-566">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-567">Precio unitario</span><span class="sxs-lookup"><span data-stu-id="f2a43-567">Unit price</span></span></td>
<td><p><span data-ttu-id="f2a43-568">Precio por licencia, como se publica en la lista de precios en el momento de la compra.</span><span class="sxs-lookup"><span data-stu-id="f2a43-568">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="f2a43-569">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-569">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-570">Cantidad</span><span class="sxs-lookup"><span data-stu-id="f2a43-570">Quantity</span></span></td>
<td><p><span data-ttu-id="f2a43-571">Número de licencias.</span><span class="sxs-lookup"><span data-stu-id="f2a43-571">Number of licenses.</span></span> <span data-ttu-id="f2a43-572">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-572">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-573">Tipo de unidad</span><span class="sxs-lookup"><span data-stu-id="f2a43-573">Unit type</span></span></td>
<td><p><span data-ttu-id="f2a43-574">El tipo de unidad que se cobra el medidor.</span><span class="sxs-lookup"><span data-stu-id="f2a43-574">The type of unit the meter is charged in.</span></span> <span data-ttu-id="f2a43-575">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="f2a43-575">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-576">Impuestos de facturación anterior a</span><span class="sxs-lookup"><span data-stu-id="f2a43-576">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="f2a43-577">Cantidad total antes de impuestos.</span><span class="sxs-lookup"><span data-stu-id="f2a43-577">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-578">Divisa de facturación</span><span class="sxs-lookup"><span data-stu-id="f2a43-578">Billing currency</span></span></td>
<td><p><span data-ttu-id="f2a43-579">La moneda en la región geográfica del cliente</span><span class="sxs-lookup"><span data-stu-id="f2a43-579">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-580">Precio total antes de impuestos</span><span class="sxs-lookup"><span data-stu-id="f2a43-580">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="f2a43-581">Los precios antes de que se agregan los impuestos.</span><span class="sxs-lookup"><span data-stu-id="f2a43-581">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-582">Precios de moneda</span><span class="sxs-lookup"><span data-stu-id="f2a43-582">Pricing currency</span></span></td>
<td><p><span data-ttu-id="f2a43-583">La moneda en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="f2a43-583">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-584">Información de servicio 1</span><span class="sxs-lookup"><span data-stu-id="f2a43-584">Service Info 1</span></span></td>
<td><p><span data-ttu-id="f2a43-585">Número de conexiones de Bus de servicio aprovisionadas y usadas en un día determinado.</span><span class="sxs-lookup"><span data-stu-id="f2a43-585">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-586">Información de servicio 2</span><span class="sxs-lookup"><span data-stu-id="f2a43-586">Service Info 2</span></span></td>
<td><p><span data-ttu-id="f2a43-587">Un campo heredado que captura los metadatos específicos del servicio opcional.</span><span class="sxs-lookup"><span data-stu-id="f2a43-587">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="f2a43-588">Etiquetas</span><span class="sxs-lookup"><span data-stu-id="f2a43-588">Tags</span></span></td>
<td><p><span data-ttu-id="f2a43-589">Etiquetas que asigna al medidor en orden para agrupar los registros de facturación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-589">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="f2a43-590">Por ejemplo, puede usar etiquetas para distribuir los costos por el departamento que utiliza el medidor.</span><span class="sxs-lookup"><span data-stu-id="f2a43-590">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="f2a43-591">Información adicional</span><span class="sxs-lookup"><span data-stu-id="f2a43-591">Additional Info</span></span></td>
<td><p><span data-ttu-id="f2a43-592">Cualquier información adicional que no se tratan en otras columnas.</span><span class="sxs-lookup"><span data-stu-id="f2a43-592">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="f2a43-593">Asignación de cargos entre una factura y el archivo de conciliación</span><span class="sxs-lookup"><span data-stu-id="f2a43-593">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="f2a43-594">La factura proporciona un resumen de los cargos, mientras que el archivo de conciliación proporciona un desglose detallado de las transacciones de elementos de línea, incluidos los tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="f2a43-594">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="f2a43-595">Para hacer referencias cruzadas de cantidades de cargos entre el archivo de conciliación y la factura, puedes usar las opciones de filtro de Microsoft Excel para filtrar por tipo de cargo en el archivo de conciliación con el fin de asignar los cargos de facturación a un conjunto de desgloses de cargos del archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-595">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="f2a43-596">Los archivos de conciliación, tanto basados en uso como en licencias, solo muestran cargos y transacciones relacionados con el uso (unidades consumidas y cargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="f2a43-596">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="f2a43-597">En el archivo de conciliación no aparecen devoluciones, descuentos o créditos excepcionales que aparecen en la factura como "Ajustes".</span><span class="sxs-lookup"><span data-stu-id="f2a43-597">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="f2a43-598">La siguiente tabla muestra las asignaciones entre una sección de factura y los tipos de cargo asociados que es posible que se muestren en los archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="f2a43-598">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="f2a43-599"><strong>Descripción de cargos de facturación</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-599"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-600"><strong>Descripción de cargos del archivo de conciliación (columna ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-600"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-601"><strong>¿Qué es este cargo?</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-601"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-602"><strong>¿Cómo se asignan estos ChargeTypes a la factura?</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-602"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="f2a43-603"><strong>Cargos de licencia</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-603"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-604">Tarifa de activación</span><span class="sxs-lookup"><span data-stu-id="f2a43-604">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-605">El importe cobrado al cliente cuando usa la suscripción después de adquirirla</span><span class="sxs-lookup"><span data-stu-id="f2a43-605">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="f2a43-606">Desde el archivo basado en licencia, suma la columna <strong>Amount</strong>.</span><span class="sxs-lookup"><span data-stu-id="f2a43-606">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f2a43-607">Cuota de cancelación</span><span class="sxs-lookup"><span data-stu-id="f2a43-607">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-608">Cargos prorrateados reembolsados al cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="f2a43-608">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f2a43-609">Tarifa de ciclo</span><span class="sxs-lookup"><span data-stu-id="f2a43-609">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-610">Cargos periódicos de una suscripción</span><span class="sxs-lookup"><span data-stu-id="f2a43-610">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f2a43-611">Prorrateo de instancia de ciclo</span><span class="sxs-lookup"><span data-stu-id="f2a43-611">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-612">Cargos prorrateados evaluados del cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="f2a43-612">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f2a43-613">Tarifas prorrateadas al cancelar</span><span class="sxs-lookup"><span data-stu-id="f2a43-613">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-614">Reembolso prorrateado de la parte no usada del servicio tras la cancelación</span><span class="sxs-lookup"><span data-stu-id="f2a43-614">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f2a43-615">Tarifas prorrateadas al comprar</span><span class="sxs-lookup"><span data-stu-id="f2a43-615">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-616">El tipo de gasto para una suscripción cuando se usa la facturación anual</span><span class="sxs-lookup"><span data-stu-id="f2a43-616">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f2a43-617">Tarifa de compra</span><span class="sxs-lookup"><span data-stu-id="f2a43-617">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-618">El tipo de gasto para una suscripción cuando se usa la facturación mensual</span><span class="sxs-lookup"><span data-stu-id="f2a43-618">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f2a43-619">Tarifa prorrateada al renovar</span><span class="sxs-lookup"><span data-stu-id="f2a43-619">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-620">Tarifas prorrateadas tras la renovación de la suscripción</span><span class="sxs-lookup"><span data-stu-id="f2a43-620">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="f2a43-621">Tarifa de renovación</span><span class="sxs-lookup"><span data-stu-id="f2a43-621">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-622">Cargo por renovar una suscripción</span><span class="sxs-lookup"><span data-stu-id="f2a43-622">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f2a43-623">Tarifas prorrateadas al activar</span><span class="sxs-lookup"><span data-stu-id="f2a43-623">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-624">Tarifas prorrateadas desde la activación hasta el final del período de facturación</span><span class="sxs-lookup"><span data-stu-id="f2a43-624">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="f2a43-625"><strong>Cargos de uso</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-625"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-626">Evaluar la tarifa de uso al cancelar</span><span class="sxs-lookup"><span data-stu-id="f2a43-626">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-627">Tarifa de uso de acceso tras la cancelación por uso impagado durante el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="f2a43-627">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="f2a43-628">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="f2a43-628">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f2a43-629">Evaluar la tarifa de uso para el ciclo actual</span><span class="sxs-lookup"><span data-stu-id="f2a43-629">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-630">tarifa de uso de acceso para el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="f2a43-630">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f2a43-631"><strong>Créditos</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-631"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-632">Desplazamiento de un elemento de línea</span><span class="sxs-lookup"><span data-stu-id="f2a43-632">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-633">Reembolso parcial o total de un elemento de línea, incluidos impuestos</span><span class="sxs-lookup"><span data-stu-id="f2a43-633">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-634">Desde el archivo basado en licencia, suma la columna <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="f2a43-634">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="f2a43-635">Desde el archivo basado en uso, suma la columna <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="f2a43-635">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="f2a43-636"><strong>Descuentos basados en uso</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-636"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-637">Descuento de activación</span><span class="sxs-lookup"><span data-stu-id="f2a43-637">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-638">Descuento que se aplica cuando se activa la suscripción</span><span class="sxs-lookup"><span data-stu-id="f2a43-638">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="f2a43-639">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="f2a43-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f2a43-640">Descuento de ciclo</span><span class="sxs-lookup"><span data-stu-id="f2a43-640">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-641">Descuento que se aplica en cargos periódicos</span><span class="sxs-lookup"><span data-stu-id="f2a43-641">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f2a43-642">Descuento de renovación</span><span class="sxs-lookup"><span data-stu-id="f2a43-642">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-643">Descuento que se aplica cuando se renueva la suscripción</span><span class="sxs-lookup"><span data-stu-id="f2a43-643">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f2a43-644">Descuento de cancelación</span><span class="sxs-lookup"><span data-stu-id="f2a43-644">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-645">Cargos que se aplican cuando se cancelan los descuentos</span><span class="sxs-lookup"><span data-stu-id="f2a43-645">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="f2a43-646"><strong>Descuentos de licencias</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-646"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-647"><em>Se pueden aplicar a varios tipos de cargos</em></span><span class="sxs-lookup"><span data-stu-id="f2a43-647"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="f2a43-648">Desde el archivo basado en licencia, suma la columna <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="f2a43-648">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="f2a43-649"><strong>Impuestos</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="f2a43-649"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-650"><em>Se pueden aplicar a varios tipos de cargos</em></span><span class="sxs-lookup"><span data-stu-id="f2a43-650"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="f2a43-651"><em>Excepción: &quot;Desplazamiento de un elemento de línea&quot; ya incluye los impuestos. Consulte los créditos, más arriba.</em></span><span class="sxs-lookup"><span data-stu-id="f2a43-651"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-652">Impuestos o impuesto de valor añadido (IVA)</span><span class="sxs-lookup"><span data-stu-id="f2a43-652">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="f2a43-653">Desde el archivo basado en licencia, suma la columna <strong>Tax</strong>.</span><span class="sxs-lookup"><span data-stu-id="f2a43-653">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="f2a43-654">Desde el archivo basado en uso, suma la columna <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="f2a43-654">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
