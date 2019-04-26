---
title: Usar los archivos de conciliación | Centro de partners
ms.topic: article
ms.date: 03/15/2019
description: Para obtener una vista detallada del elemento de línea de cada carga de un ciclo de facturación, descargue los archivos de conciliación de centro de partners.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 8e7b17cb39f266c404d7873dc17e471741d52b32
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132785"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="12995-103">Usar los archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="12995-103">Use the reconciliation files</span></span>

<span data-ttu-id="12995-104">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="12995-104">**Applies to**</span></span>

-  <span data-ttu-id="12995-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="12995-105">Partner Center</span></span>
-  <span data-ttu-id="12995-106">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="12995-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="12995-107">Para obtener una vista detallada del elemento de línea de cada carga de un ciclo de facturación, descargue los archivos de conciliación de centro de partners.</span><span class="sxs-lookup"><span data-stu-id="12995-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="12995-108">Los detalles incluyen los cargos para las suscripciones de cada cliente y los eventos detallados (por ejemplo, una adición intermedia de puestos en una suscripción).</span><span class="sxs-lookup"><span data-stu-id="12995-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="12995-109">Problemas de formato</span><span class="sxs-lookup"><span data-stu-id="12995-109">Formatting issues</span></span>

<span data-ttu-id="12995-110">En ocasiones, el archivo de conciliación podría tener problemas de formato.</span><span class="sxs-lookup"><span data-stu-id="12995-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="12995-111">(Esto puede ocurrir, por ejemplo, si no se usa la configuración regional EN-US). Siga estos pasos para corregir estos problemas.</span><span class="sxs-lookup"><span data-stu-id="12995-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="12995-112">Abra el archivo .csv en Excel y seleccione la primera columna.</span><span class="sxs-lookup"><span data-stu-id="12995-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="12995-113">En la cinta de opciones, seleccione <strong>datos</strong>y, a continuación, seleccione <strong>texto en columnas</strong>.</span><span class="sxs-lookup"><span data-stu-id="12995-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="12995-114">En convertir texto en el Asistente de columnas, seleccione <strong>delimitado por tipo de archivo</strong>y, a continuación, seleccione <strong>siguiente</strong>.</span><span class="sxs-lookup"><span data-stu-id="12995-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="12995-115">En el campo delimitadores, seleccione <strong>comas</strong>.</span><span class="sxs-lookup"><span data-stu-id="12995-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="12995-116">Si <strong>ficha</strong> está ya seleccionado, puede dejarla.</span><span class="sxs-lookup"><span data-stu-id="12995-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="12995-117">Selecciona <strong>Siguiente</strong>.</span><span class="sxs-lookup"><span data-stu-id="12995-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="12995-118">En el campo de formato de datos de columna, seleccione <strong>fecha: MDY</strong>y, a continuación, seleccione <strong>siguiente</strong>.</span><span class="sxs-lookup"><span data-stu-id="12995-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="12995-119">En el campo de formato de datos de columna, seleccione <strong>texto</strong> para amount, todas las columnas y, a continuación, seleccione <strong>finalizar</strong>.</span><span class="sxs-lookup"><span data-stu-id="12995-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="12995-120">Detallar asociado</span><span class="sxs-lookup"><span data-stu-id="12995-120">Itemize by partner</span></span>


<span data-ttu-id="12995-121">Los partners del modelo indirecto pueden usar estos campos adicionales en ambos archivos de conciliación basada en uso y en licencia para realizar el desglose por revendedor.</span><span class="sxs-lookup"><span data-stu-id="12995-121">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="12995-122">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="12995-122">MPN ID</span></span></th>
<th><span data-ttu-id="12995-123">Descripción</span><span class="sxs-lookup"><span data-stu-id="12995-123">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="12995-124">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="12995-124">MPN ID</span></span></td>
<td><p><span data-ttu-id="12995-125">Id. de Microsoft Partner Network (MPN) del partner de CSP (directo o indirecto).</span><span class="sxs-lookup"><span data-stu-id="12995-125">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-126">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="12995-126">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="12995-127">Solo aparece en los archivos de conciliación de partners en el modelo indirecto.</span><span class="sxs-lookup"><span data-stu-id="12995-127">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="12995-128">El Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="12995-128">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="12995-129">Corresponde al id. de revendedor indicado para la suscripción específica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="12995-129">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="12995-130">muestra de eTo o actualiza el distribuidor, en el menú del centro de partners, seleccione <strong>clientes</strong>, a continuación, elija el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="12995-130">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="12995-131">En el menú del cliente, selecciona <strong>Suscripciones</strong> y elige la suscripción de la lista.</span><span class="sxs-lookup"><span data-stu-id="12995-131">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="12995-132">Selecciona <strong>Actualizar</strong> para cambiar el valor de <strong>Revendedor (id. de MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="12995-132">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="12995-133">Si un partner CSP vendió la suscripción directamente al cliente, su id. de MPN aparece dos veces, como id. de MPN y como id. de MPN del revendedor.</span><span class="sxs-lookup"><span data-stu-id="12995-133">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="12995-134">Si un partner CSP tiene un revendedor sin un id. de MPN, este valor se establece en el id. de MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="12995-134">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="12995-135">Si el partner CSP quita un id. de revendedor, este valor se establece en -1.</span><span class="sxs-lookup"><span data-stu-id="12995-135">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="12995-136">Campos de archivo de licencia</span><span class="sxs-lookup"><span data-stu-id="12995-136">License-based file fields</span></span>


<span data-ttu-id="12995-137">Para conciliar los cargos en función de los pedidos del cliente, compara el Syndication\_Partner\_Subscription\_Number del archivo de conciliación con el id. de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="12995-137">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="12995-138"><strong>Columna</strong></span><span class="sxs-lookup"><span data-stu-id="12995-138"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="12995-139"><strong>Descripción</strong></span><span class="sxs-lookup"><span data-stu-id="12995-139"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="12995-140"><strong>Valor de ejemplo</strong></span><span class="sxs-lookup"><span data-stu-id="12995-140"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-141">PartnerId</span><span class="sxs-lookup"><span data-stu-id="12995-141">PartnerId</span></span></td>
<td><p><span data-ttu-id="12995-142">Identificador único de una entidad de facturación específica, con formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="12995-142">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="12995-143">No es necesario para la reconciliación, pero puede ser información útil.</span><span class="sxs-lookup"><span data-stu-id="12995-143">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="12995-144">Igual en todas las filas.</span><span class="sxs-lookup"><span data-stu-id="12995-144">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="12995-145">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="12995-145">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-146">CustomerID</span><span class="sxs-lookup"><span data-stu-id="12995-146">CustomerID</span></span></td>
<td><p><span data-ttu-id="12995-147">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="12995-147">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="12995-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="12995-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-149">OrderID</span><span class="sxs-lookup"><span data-stu-id="12995-149">OrderID</span></span></td>
<td><p><span data-ttu-id="12995-150">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="12995-150">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="12995-151">Puede ser útil para identificar al pedido al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-151">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="12995-152">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="12995-152">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-153">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="12995-153">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="12995-154">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="12995-154">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="12995-155">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-155">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="12995-156">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="12995-156">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="12995-157">Consulte Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="12995-157">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="12995-158">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="12995-158">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-159">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="12995-159">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="12995-160">Identificador único de las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="12995-160">Unique identifier for subscriptions.</span></span> <span data-ttu-id="12995-161">Un cliente puede tener varias suscripciones para el mismo plan, por lo que es importante para el análisis de archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-161">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="12995-162">Este campo se asigna al identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="12995-162">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="12995-163">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="12995-163">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-164">OfferID</span><span class="sxs-lookup"><span data-stu-id="12995-164">OfferID</span></span></td>
<td><p><span data-ttu-id="12995-165">Identificador único de la oferta.</span><span class="sxs-lookup"><span data-stu-id="12995-165">Unique offer ID.</span></span> <span data-ttu-id="12995-166">Identificador de la oferta estándar según la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="12995-166">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="12995-167"><b>Nota</b>: Este valor no coincide con Id. de oferta desde la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="12995-167"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="12995-168">Consulta DurableOfferID a continuación.</span><span class="sxs-lookup"><span data-stu-id="12995-168">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="12995-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="12995-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-170">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="12995-170">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="12995-171">Identificador único de oferta duradera, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="12995-171">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="12995-172"><b>Nota</b>: Este valor coincide con el Id. de oferta desde la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="12995-172"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="12995-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="12995-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-174">OfferName</span><span class="sxs-lookup"><span data-stu-id="12995-174">OfferName</span></span></td>
<td><p><span data-ttu-id="12995-175">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="12995-175">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="12995-176">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="12995-176">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-177">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="12995-177">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="12995-178">Fecha de finalización de la suscripción, establecida en el día posterior al envío del pedido.</span><span class="sxs-lookup"><span data-stu-id="12995-178">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="12995-179">Al consultar la fecha de inicio de la suscripción junto con la fecha de finalización, puedes determinar si el cliente aún está dentro del primer año de la suscripción o si la suscripción se ha renovado para el año siguiente.</span><span class="sxs-lookup"><span data-stu-id="12995-179">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="12995-180">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="12995-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="12995-181">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="12995-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-182">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="12995-182">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="12995-183">La fecha de finalización de la suscripción: 12 meses + x días después de la fecha de inicio (para alinearse con fecha de facturación del asociado) o 12 meses a partir de la fecha de renovación.</span><span class="sxs-lookup"><span data-stu-id="12995-183">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="12995-184">En el momento de la renovación, los precios se actualizan según la lista de precios actual.</span><span class="sxs-lookup"><span data-stu-id="12995-184">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="12995-185">Es posible que se necesite una comunicación con el cliente antes de la renovación automatizada.</span><span class="sxs-lookup"><span data-stu-id="12995-185">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="12995-186">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="12995-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="12995-187">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="12995-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-188">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="12995-188">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="12995-189">Día de inicio de los cargos.</span><span class="sxs-lookup"><span data-stu-id="12995-189">Start day of the charges.</span></span></p>
<p><span data-ttu-id="12995-190">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="12995-190">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="12995-191">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="12995-191">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="12995-192">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="12995-192">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-193">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="12995-193">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="12995-194">Día de finalización de los cargos.</span><span class="sxs-lookup"><span data-stu-id="12995-194">End day of the charges.</span></span></p>
<p><span data-ttu-id="12995-195">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="12995-195">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="12995-196">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="12995-196">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="12995-197">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="12995-197">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-198">ChargeType</span><span class="sxs-lookup"><span data-stu-id="12995-198">ChargeType</span></span></td>
<td><p><span data-ttu-id="12995-199">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="12995-199">The type of charge or adjustment.</span></span> <span data-ttu-id="12995-200">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="12995-200">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="12995-201">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="12995-201">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-202">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="12995-202">UnitPrice</span></span></td>
<td><p><span data-ttu-id="12995-203">Precio por puesto, tal y como se publica en la lista de precios en el momento de compra.</span><span class="sxs-lookup"><span data-stu-id="12995-203">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="12995-204">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-204">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="12995-205">6.82</span><span class="sxs-lookup"><span data-stu-id="12995-205">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-206">Cantidad</span><span class="sxs-lookup"><span data-stu-id="12995-206">Quantity</span></span></td>
<td><p><span data-ttu-id="12995-207">Número de puestos.</span><span class="sxs-lookup"><span data-stu-id="12995-207">Number of seats.</span></span> <span data-ttu-id="12995-208">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-208">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="12995-209">2</span><span class="sxs-lookup"><span data-stu-id="12995-209">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-210">Volumen</span><span class="sxs-lookup"><span data-stu-id="12995-210">Amount</span></span></td>
<td><p><span data-ttu-id="12995-211">Total del precio para la cantidad.</span><span class="sxs-lookup"><span data-stu-id="12995-211">Total of price for quantity.</span></span> <span data-ttu-id="12995-212">Es de utilidad para comprobar que el cálculo de la cantidad coincide con la manera de calcular este valor para los clientes.</span><span class="sxs-lookup"><span data-stu-id="12995-212">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="12995-213">13.32</span><span class="sxs-lookup"><span data-stu-id="12995-213">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-214">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="12995-214">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="12995-215">Cantidad de descuento que se aplica a estos cargos.</span><span class="sxs-lookup"><span data-stu-id="12995-215">Amount of discount applied to these charges.</span></span> <span data-ttu-id="12995-216">Los IUR o las nuevas suscripciones que puedan optar a un incentivo también incluirán un importe de descuento en esta columna.</span><span class="sxs-lookup"><span data-stu-id="12995-216">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="12995-217">2.32</span><span class="sxs-lookup"><span data-stu-id="12995-217">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-218">Subtotal</span><span class="sxs-lookup"><span data-stu-id="12995-218">Subtotal</span></span></td>
<td><p><span data-ttu-id="12995-219">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="12995-219">Total before tax.</span></span> <span data-ttu-id="12995-220">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="12995-220">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="12995-221">11</span><span class="sxs-lookup"><span data-stu-id="12995-221">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-222">Impuestos</span><span class="sxs-lookup"><span data-stu-id="12995-222">Tax</span></span></td>
<td><p><span data-ttu-id="12995-223">Importe de impuestos, según el mercado&#39;reglas s y circunstancias concretas.</span><span class="sxs-lookup"><span data-stu-id="12995-223">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="12995-224">0</span><span class="sxs-lookup"><span data-stu-id="12995-224">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-225">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="12995-225">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="12995-226">Total con impuestos.</span><span class="sxs-lookup"><span data-stu-id="12995-226">Total after tax.</span></span> <span data-ttu-id="12995-227">Comprueba si se cobran impuestos en la factura.</span><span class="sxs-lookup"><span data-stu-id="12995-227">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="12995-228">11</span><span class="sxs-lookup"><span data-stu-id="12995-228">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-229">Moneda</span><span class="sxs-lookup"><span data-stu-id="12995-229">Currency</span></span></td>
<td><p><span data-ttu-id="12995-230">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="12995-230">Currency type.</span></span> <span data-ttu-id="12995-231">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="12995-231">Each billing entity has only one currency.</span></span> <span data-ttu-id="12995-232">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="12995-232">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="12995-233">EUR</span><span class="sxs-lookup"><span data-stu-id="12995-233">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-234">CustomerName</span><span class="sxs-lookup"><span data-stu-id="12995-234">CustomerName</span></span></td>
<td><p><span data-ttu-id="12995-235">Cliente&#39;nombre de la organización s notificados en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="12995-235">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="12995-236">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="12995-236">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="12995-237">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="12995-237">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-238">MPNID</span><span class="sxs-lookup"><span data-stu-id="12995-238">MPNID</span></span></td>
<td><p><span data-ttu-id="12995-239">Id. de MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="12995-239">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="12995-240">4390934</span><span class="sxs-lookup"><span data-stu-id="12995-240">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-241">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="12995-241">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="12995-242">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="12995-242">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="12995-243">Ver <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Desglosar por partner</a></span><span class="sxs-lookup"><span data-stu-id="12995-243">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="12995-244">4390934</span><span class="sxs-lookup"><span data-stu-id="12995-244">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-245">DomainName</span><span class="sxs-lookup"><span data-stu-id="12995-245">DomainName</span></span></td>
<td><p><span data-ttu-id="12995-246">Cliente&#39;nombre de dominio de s, que ayuda a identificar el cliente.</span><span class="sxs-lookup"><span data-stu-id="12995-246">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="12995-247">No debe usarse para identificar al cliente como el cliente o socio puede actualizar el dominio personal de forma predeterminada a través del portal de Office 365.</span><span class="sxs-lookup"><span data-stu-id="12995-247">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="12995-248">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="12995-248">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="12995-249">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="12995-249">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-250">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="12995-250">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="12995-251">Alias de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="12995-251">Subscription nickname.</span></span> <span data-ttu-id="12995-252">Si no se especifica ningún alias, el Centro de partners usa OfferName.</span><span class="sxs-lookup"><span data-stu-id="12995-252">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="12995-253">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="12995-253">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-254">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="12995-254">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="12995-255">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="12995-255">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="12995-256">(Este es un campo idéntico al nombre de la oferta).</span><span class="sxs-lookup"><span data-stu-id="12995-256">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="12995-257">PROJECT ONLINE PREMIUM SIN CLIENTE DE PROJECT</span><span class="sxs-lookup"><span data-stu-id="12995-257">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="12995-258">Campos de archivo basada en uso</span><span class="sxs-lookup"><span data-stu-id="12995-258">Usage-based file fields</span></span>


<span data-ttu-id="12995-259">Para conciliar los cargos en función del uso de tu cliente, compara los valores de ResellerID/ResellerName/ResellerBillableAccount del archivo de conciliación, el nombre del cliente y el id. de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="12995-259">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="12995-260">Los siguientes campos explican los servicios usados y la clasificación.</span><span class="sxs-lookup"><span data-stu-id="12995-260">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="12995-261"><strong>Columna</strong></span><span class="sxs-lookup"><span data-stu-id="12995-261"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="12995-262"><strong>Descripción</strong></span><span class="sxs-lookup"><span data-stu-id="12995-262"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="12995-263"><strong>Valor de ejemplo</strong></span><span class="sxs-lookup"><span data-stu-id="12995-263"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-264">PartnerID</span><span class="sxs-lookup"><span data-stu-id="12995-264">PartnerID</span></span></td>
<td><p><span data-ttu-id="12995-265">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="12995-265">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="12995-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="12995-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-267">PartnerName</span><span class="sxs-lookup"><span data-stu-id="12995-267">PartnerName</span></span></td>
<td><p><span data-ttu-id="12995-268">Nombre del partner.</span><span class="sxs-lookup"><span data-stu-id="12995-268">Partner Name.</span></span></p></td>
<td><span data-ttu-id="12995-269">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="12995-269">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-270">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="12995-270">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="12995-271">Id. de cuenta del partner.</span><span class="sxs-lookup"><span data-stu-id="12995-271">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="12995-272">1010578050</span><span class="sxs-lookup"><span data-stu-id="12995-272">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-273">CustomerName</span><span class="sxs-lookup"><span data-stu-id="12995-273">CustomerName</span></span></td>
<td><p><span data-ttu-id="12995-274">Cliente&#39;nombre de la organización s notificados en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="12995-274">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="12995-275">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="12995-275">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="12995-276">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="12995-276">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-277">MPNID</span><span class="sxs-lookup"><span data-stu-id="12995-277">MPNID</span></span></td>
<td><p><span data-ttu-id="12995-278">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="12995-278">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="12995-279">4390934</span><span class="sxs-lookup"><span data-stu-id="12995-279">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-280">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="12995-280">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="12995-281">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="12995-281">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="12995-282">Ver <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Desglosar por partner</a></span><span class="sxs-lookup"><span data-stu-id="12995-282">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="12995-283">4390934</span><span class="sxs-lookup"><span data-stu-id="12995-283">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-284">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="12995-284">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="12995-285">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="12995-285">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="12995-286">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="12995-286">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-287">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="12995-287">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="12995-288">Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="12995-288">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="12995-289">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="12995-289">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="12995-290">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="12995-290">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-291">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="12995-291">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="12995-292">Fecha de finalización del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="12995-292">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="12995-293">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="12995-293">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="12995-294">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="12995-294">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-295">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="12995-295">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="12995-296">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="12995-296">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="12995-297">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="12995-298">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="12995-298">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="12995-299">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="12995-299">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-300">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="12995-300">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="12995-301">Alias de la oferta de servicio.</span><span class="sxs-lookup"><span data-stu-id="12995-301">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="12995-302">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="12995-302">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-303">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="12995-303">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="12995-304">Línea de negocio de la oferta de servicio</span><span class="sxs-lookup"><span data-stu-id="12995-304">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="12995-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="12995-305">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-306">OrderID</span><span class="sxs-lookup"><span data-stu-id="12995-306">OrderID</span></span></td>
<td><p><span data-ttu-id="12995-307">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="12995-307">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="12995-308">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-308">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="12995-309">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="12995-309">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-310">ServiceName</span><span class="sxs-lookup"><span data-stu-id="12995-310">ServiceName</span></span></td>
<td><p><span data-ttu-id="12995-311">Nombre del servicio de Azure en cuestión.</span><span class="sxs-lookup"><span data-stu-id="12995-311">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="12995-312">MÁQUINAS VIRTUALES</span><span class="sxs-lookup"><span data-stu-id="12995-312">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-313">ServiceType</span><span class="sxs-lookup"><span data-stu-id="12995-313">ServiceType</span></span></td>
<td><p><span data-ttu-id="12995-314">Tipo específico de servicio de Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="12995-314">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="12995-315">Bus de servicio: individual o paquete</span><span class="sxs-lookup"><span data-stu-id="12995-315">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="12995-316">Base de datos SQL Azure: edición Business o Web</span><span class="sxs-lookup"><span data-stu-id="12995-316">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-317">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="12995-317">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="12995-318">Identificador único específico para toda la estructura de precios y datos del servicio.</span><span class="sxs-lookup"><span data-stu-id="12995-318">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="12995-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="12995-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-320">Nombre de recurso</span><span class="sxs-lookup"><span data-stu-id="12995-320">Resource Name</span></span></td>
<td><p><span data-ttu-id="12995-321">Nombre del recurso de Azure.</span><span class="sxs-lookup"><span data-stu-id="12995-321">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="12995-322">Transferencia entrante de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="12995-322">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="12995-323">Transferencia saliente de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="12995-323">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-324">Region</span><span class="sxs-lookup"><span data-stu-id="12995-324">Region</span></span></td>
<td><p><span data-ttu-id="12995-325">La región a la que se aplica el uso.</span><span class="sxs-lookup"><span data-stu-id="12995-325">The region the usage applies to.</span></span> <span data-ttu-id="12995-326">Se usa principalmente para asignar tarifas a las transferencias de datos, ya que las tarifas varían según la región.</span><span class="sxs-lookup"><span data-stu-id="12995-326">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="12995-327">Asia Pacífico, Europa, América Latina, América del Norte</span><span class="sxs-lookup"><span data-stu-id="12995-327">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-328">SKU</span><span class="sxs-lookup"><span data-stu-id="12995-328">SKU</span></span></td>
<td><p><span data-ttu-id="12995-329">Identificador único de MSFT para la oferta</span><span class="sxs-lookup"><span data-stu-id="12995-329">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="12995-330">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="12995-330">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="12995-331">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="12995-331">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="12995-332">Un id. y una cantidad para desglosar las distintas clasificaciones de un servicio o un recurso en un período de facturación determinado.</span><span class="sxs-lookup"><span data-stu-id="12995-332">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="12995-333">Para clasificación en niveles de Azure, puede haber una clasificación hasta una cantidad determinada de unidades facturables y, posteriormente, una clasificación diferente.</span><span class="sxs-lookup"><span data-stu-id="12995-333">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="12995-334">1</span><span class="sxs-lookup"><span data-stu-id="12995-334">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-335">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="12995-335">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="12995-336">La cantidad de servicio consumida (horas, GB, etc.) durante el período de notificación.</span><span class="sxs-lookup"><span data-stu-id="12995-336">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="12995-337">También incluye cualquier uso no facturado de períodos anteriores.</span><span class="sxs-lookup"><span data-stu-id="12995-337">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="12995-338">11</span><span class="sxs-lookup"><span data-stu-id="12995-338">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-339">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="12995-339">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="12995-340">Unidades que se incluyen como parte de la oferta.</span><span class="sxs-lookup"><span data-stu-id="12995-340">Units included as part of the offer.</span></span> <span data-ttu-id="12995-341">No suele mostrarse en CSP.</span><span class="sxs-lookup"><span data-stu-id="12995-341">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="12995-342">0</span><span class="sxs-lookup"><span data-stu-id="12995-342">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="12995-343">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="12995-343">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="12995-344">Unidades que no se incluyen como parte de la oferta y que el partner debe abonar.</span><span class="sxs-lookup"><span data-stu-id="12995-344">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="12995-345">Equivale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="12995-345">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="12995-346">11</span><span class="sxs-lookup"><span data-stu-id="12995-346">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-347">ListPrice</span><span class="sxs-lookup"><span data-stu-id="12995-347">ListPrice</span></span></td>
<td><p><span data-ttu-id="12995-348">Precio de la oferta en vigor la fecha de inicio de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="12995-348">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="12995-349">0.0808 USD</span><span class="sxs-lookup"><span data-stu-id="12995-349">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-350">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="12995-350">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="12995-351">ListPrist x OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="12995-351">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="12995-352">0.085 USD</span><span class="sxs-lookup"><span data-stu-id="12995-352">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-353">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="12995-353">TaxAmount</span></span></td>
<td><p><span data-ttu-id="12995-354">Importe de impuestos, según el mercado&#39;reglas s y circunstancias concretas.</span><span class="sxs-lookup"><span data-stu-id="12995-354">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="12995-355">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="12995-355">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-356">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="12995-356">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="12995-357">Total con impuestos, si se aplican impuestos.</span><span class="sxs-lookup"><span data-stu-id="12995-357">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="12995-358">0.93 USD</span><span class="sxs-lookup"><span data-stu-id="12995-358">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-359">Moneda</span><span class="sxs-lookup"><span data-stu-id="12995-359">Currency</span></span></td>
<td><p><span data-ttu-id="12995-360">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="12995-360">Currency type.</span></span> <span data-ttu-id="12995-361">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="12995-361">Each billing entity has only one currency.</span></span> <span data-ttu-id="12995-362">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="12995-362">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="12995-363">EUR</span><span class="sxs-lookup"><span data-stu-id="12995-363">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-364">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="12995-364">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="12995-365">Precio sin impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="12995-365">Pretax price per unit.</span></span> <span data-ttu-id="12995-366">Igual que PretaxCharges/OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="12995-366">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="12995-367">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="12995-367">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-368">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="12995-368">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="12995-369">Precio después de impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="12995-369">Post tax price per unit.</span></span> <span data-ttu-id="12995-370">Igual que PostTaxTotal/OverageQuantity o PretaxEffectiveRate + tipo impositivo por importe unitario, redondeado el céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="12995-370">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="12995-371">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="12995-371">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-372">ChargeType</span><span class="sxs-lookup"><span data-stu-id="12995-372">ChargeType</span></span></td>
<td><p><span data-ttu-id="12995-373">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="12995-373">The type of charge or adjustment.</span></span> <span data-ttu-id="12995-374">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="12995-374">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="12995-375">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="12995-375">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-376">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="12995-376">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="12995-377">Id. de cuenta único en la plataforma de facturación de MSFT.</span><span class="sxs-lookup"><span data-stu-id="12995-377">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="12995-378">1280018095</span><span class="sxs-lookup"><span data-stu-id="12995-378">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-379">UsageDate</span><span class="sxs-lookup"><span data-stu-id="12995-379">UsageDate</span></span></td>
<td><p><span data-ttu-id="12995-380">Fecha de implementación del servicio.</span><span class="sxs-lookup"><span data-stu-id="12995-380">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="12995-381">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="12995-381">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-382">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="12995-382">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="12995-383">Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena.</span><span class="sxs-lookup"><span data-stu-id="12995-383">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="12995-384">Asia oriental, Sur asiático, Norte de Europa, Europa occidental, Norte central de EE. UU., Sur central de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="12995-384">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-385">MeteredService</span><span class="sxs-lookup"><span data-stu-id="12995-385">MeteredService</span></span></td>
<td><p><span data-ttu-id="12995-386">Esta columna se usa para hacer un seguimiento de los servicios de Microsoft Azure individuales que quizás no se identifiquen específicamente en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="12995-386">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="12995-387">Por ejemplo, las transferencias de datos se notifican como &quot;Microsoft Azure: todos los servicios&quot; en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="12995-387">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="12995-388">En esta columna MeteredService se indicará qué servicio específico pertenece el uso.</span><span class="sxs-lookup"><span data-stu-id="12995-388">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="12995-389">AccessControl, CDN, Proceso, Base de datos, ServiceBus, Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="12995-389">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-390">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="12995-390">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="12995-391">Subtítulo que aclara el servicio de Microsoft Azure individual más allá del nivel proporcionado por el campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="12995-391">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="12995-392">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="12995-392">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-393">Proyecto</span><span class="sxs-lookup"><span data-stu-id="12995-393">Project</span></span></td>
<td><p><span data-ttu-id="12995-394">Nombre definido por el cliente para la instancia del servicio</span><span class="sxs-lookup"><span data-stu-id="12995-394">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="12995-395">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="12995-395">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-396">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="12995-396">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="12995-397">Número de conexiones de Bus de servicio aprovisionadas y usadas en un día determinado.</span><span class="sxs-lookup"><span data-stu-id="12995-397">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="12995-398">Por ejemplo: si tenías una conexión aprovisionada individualmente durante un mes de 30 días, Service Info 1 contendría 1 "1,000000 conexiones/30 días".</span><span class="sxs-lookup"><span data-stu-id="12995-398">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="12995-399">Si tuviera un paquete de 25 de conexiones de bus de servicio aprovisionada y ha utilizado 1 durante ese día, el extracto de uso diario durante ese día indicaría "25 conexiones / 30 días: utilizado: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="12995-399">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-400">CustomerID</span><span class="sxs-lookup"><span data-stu-id="12995-400">CustomerID</span></span></td>
<td><p><span data-ttu-id="12995-401">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="12995-401">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="12995-402">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="12995-402">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="12995-403">DomainName</span><span class="sxs-lookup"><span data-stu-id="12995-403">DomainName</span></span></td>
<td><p><span data-ttu-id="12995-404">Cliente&#39;nombre de dominio de s, que ayuda a identificar el cliente.</span><span class="sxs-lookup"><span data-stu-id="12995-404">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="12995-405">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="12995-405">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="12995-406">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="12995-406">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="12995-407">Unidad</span><span class="sxs-lookup"><span data-stu-id="12995-407">Unit</span></span></td>
<td><p><span data-ttu-id="12995-408">La unidad del nombre del recurso</span><span class="sxs-lookup"><span data-stu-id="12995-408">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="12995-409">GB u HORAS</span><span class="sxs-lookup"><span data-stu-id="12995-409">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="12995-410">Campos del archivo periódicas y únicas</span><span class="sxs-lookup"><span data-stu-id="12995-410">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="12995-411">Column</span><span class="sxs-lookup"><span data-stu-id="12995-411">Column</span></span></th>
<th><span data-ttu-id="12995-412">Descripción</span><span class="sxs-lookup"><span data-stu-id="12995-412">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="12995-413">PartnerId</span><span class="sxs-lookup"><span data-stu-id="12995-413">PartnerId</span></span></td>
<td><p><span data-ttu-id="12995-414">Identificador único del inquilino de Microsoft Azure Active Directory para una entidad de facturación específica, en formato GUID.</span><span class="sxs-lookup"><span data-stu-id="12995-414">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="12995-415">No es necesario para la reconciliación, pero puede ser información útil.</span><span class="sxs-lookup"><span data-stu-id="12995-415">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="12995-416">Igual en todas las filas.</span><span class="sxs-lookup"><span data-stu-id="12995-416">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-417">Id. de cliente</span><span class="sxs-lookup"><span data-stu-id="12995-417">Customer Id</span></span></td>
<td><p><span data-ttu-id="12995-418">Microsoft Azure Active Directory inquilino identificador único, en formato GUID, que usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="12995-418">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-419">Nombre del cliente</span><span class="sxs-lookup"><span data-stu-id="12995-419">Customer Name</span></span></td>
<td><p><span data-ttu-id="12995-420">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="12995-420">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-421">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="12995-421">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="12995-422">Nombre de dominio del cliente, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="12995-422">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="12995-423">No debe usarse para identificar al cliente como el cliente o socio puede actualizar el dominio personal de forma predeterminada a través del portal de Office 365.</span><span class="sxs-lookup"><span data-stu-id="12995-423">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="12995-424">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="12995-424">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-425">País del cliente</span><span class="sxs-lookup"><span data-stu-id="12995-425">Customer Country</span></span></td>
<td><p><span data-ttu-id="12995-426">El país donde se encuentra el cliente.</span><span class="sxs-lookup"><span data-stu-id="12995-426">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-427">Número de factura</span><span class="sxs-lookup"><span data-stu-id="12995-427">Invoice number</span></span></td>
<td><p><span data-ttu-id="12995-428">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="12995-428">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-429">MpnId</span><span class="sxs-lookup"><span data-stu-id="12995-429">MpnId</span></span></td>
<td><p><span data-ttu-id="12995-430">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="12995-430">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-431">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="12995-431">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="12995-432">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="12995-432">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-433">Id. de pedido</span><span class="sxs-lookup"><span data-stu-id="12995-433">Order ID</span></span></td>
<td><p><span data-ttu-id="12995-434">Identificador único para un pedido en la plataforma de comercio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="12995-434">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="12995-435">Puede ser útil para identificar al pedido al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-435">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-436">Fecha del pedido</span><span class="sxs-lookup"><span data-stu-id="12995-436">Order date</span></span></td>
<td><p><span data-ttu-id="12995-437">Fecha de realización del pedido.</span><span class="sxs-lookup"><span data-stu-id="12995-437">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-438">ProductId</span><span class="sxs-lookup"><span data-stu-id="12995-438">ProductId</span></span></td>
<td><p><span data-ttu-id="12995-439">Identificador del producto.</span><span class="sxs-lookup"><span data-stu-id="12995-439">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-440">SkuId</span><span class="sxs-lookup"><span data-stu-id="12995-440">SkuId</span></span></td>
<td><p><span data-ttu-id="12995-441">Id. de un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="12995-441">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-442">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="12995-442">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="12995-443">Id. de una disponibilidad concreta.</span><span class="sxs-lookup"><span data-stu-id="12995-443">The ID for a particular Availability.</span></span> <span data-ttu-id="12995-444">"Disponibilidad" hace referencia a si un SKU concreto está o no disponible para su compra para el país, la moneda, el segmento industrial determinados, etc.</span><span class="sxs-lookup"><span data-stu-id="12995-444">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-445">Nombre de SKU</span><span class="sxs-lookup"><span data-stu-id="12995-445">SKU Name</span></span></td>
<td><p><span data-ttu-id="12995-446">Título para un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="12995-446">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-447">Nombre del producto</span><span class="sxs-lookup"><span data-stu-id="12995-447">Product name</span></span></td>
<td><p><span data-ttu-id="12995-448">Nombre del producto.</span><span class="sxs-lookup"><span data-stu-id="12995-448">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-449">PublisherName</span><span class="sxs-lookup"><span data-stu-id="12995-449">PublisherName</span></span></td>
<td><p><span data-ttu-id="12995-450">El nombre del publicador del producto.</span><span class="sxs-lookup"><span data-stu-id="12995-450">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-451">PublisherID</span><span class="sxs-lookup"><span data-stu-id="12995-451">PublisherID</span></span></td>
<td><p><span data-ttu-id="12995-452">Identificador único para este publicador.</span><span class="sxs-lookup"><span data-stu-id="12995-452">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-453">Descripción de la suscripción</span><span class="sxs-lookup"><span data-stu-id="12995-453">Subscription Description</span></span></td>
<td><p><span data-ttu-id="12995-454">Nombre descriptivo de una suscripción.</span><span class="sxs-lookup"><span data-stu-id="12995-454">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-455">Id. de la suscripción</span><span class="sxs-lookup"><span data-stu-id="12995-455">Subscription ID</span></span></td>
<td><p><span data-ttu-id="12995-456">Identificador único para una suscripción en la plataforma de comercio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="12995-456">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="12995-457">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-457">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="12995-458">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="12995-458">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-459">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="12995-459">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="12995-460">Día de inicio de los cargos.</span><span class="sxs-lookup"><span data-stu-id="12995-460">Start day of the charges.</span></span> <span data-ttu-id="12995-461">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="12995-461">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-462">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="12995-462">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="12995-463">Día de finalización de los cargos.</span><span class="sxs-lookup"><span data-stu-id="12995-463">End day of the charges.</span></span> <span data-ttu-id="12995-464">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="12995-464">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-465">Término y Billingcycle</span><span class="sxs-lookup"><span data-stu-id="12995-465">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="12995-466">La duración del período y ciclo de facturación para la compra.</span><span class="sxs-lookup"><span data-stu-id="12995-466">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="12995-467">Por ejemplo, "1 año, mes".</span><span class="sxs-lookup"><span data-stu-id="12995-467">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-468">Tipo de cargo</span><span class="sxs-lookup"><span data-stu-id="12995-468">Charge Type</span></span></td>
<td><p><span data-ttu-id="12995-469">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="12995-469">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-470">Precio unitario</span><span class="sxs-lookup"><span data-stu-id="12995-470">Unit Price</span></span></td>
<td><p><span data-ttu-id="12995-471">El precio publicado en la lista de precios en el momento de la compra.</span><span class="sxs-lookup"><span data-stu-id="12995-471">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="12995-472">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-472">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-473">Precio unitario efectivo</span><span class="sxs-lookup"><span data-stu-id="12995-473">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="12995-474">El precio por unidad una vez realizados los ajustes.</span><span class="sxs-lookup"><span data-stu-id="12995-474">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-475">Cantidad</span><span class="sxs-lookup"><span data-stu-id="12995-475">Quantity</span></span></td>
<td><p><span data-ttu-id="12995-476">Número de unidades.</span><span class="sxs-lookup"><span data-stu-id="12995-476">Number of units.</span></span> <span data-ttu-id="12995-477">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-477">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-478">Tipo de unidad</span><span class="sxs-lookup"><span data-stu-id="12995-478">Unit type</span></span></td>
<td><p><span data-ttu-id="12995-479">El tipo de unidad que se compra.</span><span class="sxs-lookup"><span data-stu-id="12995-479">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-480">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="12995-480">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="12995-481">Explicación de los descuentos aplicables.</span><span class="sxs-lookup"><span data-stu-id="12995-481">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-482">Subtotal</span><span class="sxs-lookup"><span data-stu-id="12995-482">Sub Total</span></span></td>
<td><p><span data-ttu-id="12995-483">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="12995-483">Total before tax.</span></span> <span data-ttu-id="12995-484">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="12995-484">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-485">Total de impuestos</span><span class="sxs-lookup"><span data-stu-id="12995-485">Tax Total</span></span></td>
<td><p><span data-ttu-id="12995-486">Cargo por importe de impuestos, en función de las reglas fiscales de tu mercado y las circunstancias específicas.</span><span class="sxs-lookup"><span data-stu-id="12995-486">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-487">Total</span><span class="sxs-lookup"><span data-stu-id="12995-487">Total</span></span></td>
<td><p><span data-ttu-id="12995-488">Total con impuestos.</span><span class="sxs-lookup"><span data-stu-id="12995-488">Total after tax.</span></span> <span data-ttu-id="12995-489">Comprueba si se cobran impuestos en la factura.</span><span class="sxs-lookup"><span data-stu-id="12995-489">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-490">Moneda</span><span class="sxs-lookup"><span data-stu-id="12995-490">Currency</span></span></td>
<td><p><span data-ttu-id="12995-491">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="12995-491">Currency type.</span></span> <span data-ttu-id="12995-492">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="12995-492">Each billing entity has only one currency.</span></span> <span data-ttu-id="12995-493">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="12995-493">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-494">AlternateID</span><span class="sxs-lookup"><span data-stu-id="12995-494">AlternateID</span></span></td>
<td><p><span data-ttu-id="12995-495">Un identificador alternativo para un identificador de pedido.</span><span class="sxs-lookup"><span data-stu-id="12995-495">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="12995-496">Campos del archivo de uso diario calificados</span><span class="sxs-lookup"><span data-stu-id="12995-496">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="12995-497">Column</span><span class="sxs-lookup"><span data-stu-id="12995-497">Column</span></span></th>
<th><span data-ttu-id="12995-498">Descripción</span><span class="sxs-lookup"><span data-stu-id="12995-498">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="12995-499">PartnerId</span><span class="sxs-lookup"><span data-stu-id="12995-499">PartnerId</span></span></td>
<td><p><span data-ttu-id="12995-500">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="12995-500">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-501">PartnerName</span><span class="sxs-lookup"><span data-stu-id="12995-501">PartnerName</span></span></td>
<td><p><span data-ttu-id="12995-502">Nombre del partner.</span><span class="sxs-lookup"><span data-stu-id="12995-502">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-503">CustomerId</span><span class="sxs-lookup"><span data-stu-id="12995-503">CustomerId</span></span></td>
<td><p><span data-ttu-id="12995-504">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="12995-504">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-505">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="12995-505">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="12995-506">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="12995-506">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="12995-507">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="12995-507">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-508">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="12995-508">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="12995-509">Nombre de dominio del cliente.</span><span class="sxs-lookup"><span data-stu-id="12995-509">The customer’s domain name.</span></span> <span data-ttu-id="12995-510">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="12995-510">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-511">País del cliente</span><span class="sxs-lookup"><span data-stu-id="12995-511">Customer country</span></span></td>
<td><p><span data-ttu-id="12995-512">El país donde se encuentra el cliente.</span><span class="sxs-lookup"><span data-stu-id="12995-512">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-513">MPNID</span><span class="sxs-lookup"><span data-stu-id="12995-513">MPNID</span></span></td>
<td><p><span data-ttu-id="12995-514">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="12995-514">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-515">Distribuidor MPNID</span><span class="sxs-lookup"><span data-stu-id="12995-515">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="12995-516">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="12995-516">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="12995-517">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="12995-517">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-518">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="12995-518">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="12995-519">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="12995-519">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="12995-520">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="12995-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-521">ProductId</span><span class="sxs-lookup"><span data-stu-id="12995-521">ProductId</span></span></td>
<td><p><span data-ttu-id="12995-522">Identificador del producto.</span><span class="sxs-lookup"><span data-stu-id="12995-522">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-523">SkuId</span><span class="sxs-lookup"><span data-stu-id="12995-523">SkuId</span></span></td>
<td><p><span data-ttu-id="12995-524">Id. de un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="12995-524">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-525">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="12995-525">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="12995-526">Id. de una disponibilidad concreta.</span><span class="sxs-lookup"><span data-stu-id="12995-526">The ID for a particular Availability.</span></span> <span data-ttu-id="12995-527">"Disponibilidad" hace referencia a si un SKU concreto está o no disponible para su compra para el país, la moneda, el segmento industrial determinados, etc.</span><span class="sxs-lookup"><span data-stu-id="12995-527">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-528">Nombre de SKU</span><span class="sxs-lookup"><span data-stu-id="12995-528">SKU Name</span></span></td>
<td><p><span data-ttu-id="12995-529">Título para un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="12995-529">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-530">PublisherName</span><span class="sxs-lookup"><span data-stu-id="12995-530">PublisherName</span></span></td>
<td><p><span data-ttu-id="12995-531">El nombre del publicador.</span><span class="sxs-lookup"><span data-stu-id="12995-531">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-532">PublisherID</span><span class="sxs-lookup"><span data-stu-id="12995-532">PublisherID</span></span></td>
<td><p><span data-ttu-id="12995-533">El identificador del publicador, en formato GUID.</span><span class="sxs-lookup"><span data-stu-id="12995-533">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="12995-534">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="12995-534">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="12995-535">Descripción de la suscripción</span><span class="sxs-lookup"><span data-stu-id="12995-535">Subscription Description</span></span></td>
<td><p><span data-ttu-id="12995-536">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="12995-536">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="12995-537">(Este es un campo idéntico al nombre de la oferta).</span><span class="sxs-lookup"><span data-stu-id="12995-537">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-538">Id. de la suscripción</span><span class="sxs-lookup"><span data-stu-id="12995-538">Subscription ID</span></span></td>
<td><p><span data-ttu-id="12995-539">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="12995-539">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="12995-540">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-540">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="12995-541">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="12995-541">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-542">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="12995-542">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="12995-543">Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="12995-543">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="12995-544">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="12995-544">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-545">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="12995-545">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="12995-546">Fecha de finalización del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="12995-546">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="12995-547">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="12995-547">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-548">Fecha de uso</span><span class="sxs-lookup"><span data-stu-id="12995-548">Usage Date</span></span></td>
<td><p><span data-ttu-id="12995-549">Fecha de uso del servicio.</span><span class="sxs-lookup"><span data-stu-id="12995-549">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-550">Tipo de medidor</span><span class="sxs-lookup"><span data-stu-id="12995-550">Meter Type</span></span></td>
<td><p><span data-ttu-id="12995-551">El tipo de medidor.</span><span class="sxs-lookup"><span data-stu-id="12995-551">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-552">Categoría de medidor</span><span class="sxs-lookup"><span data-stu-id="12995-552">Meter Category</span></span></td>
<td><p><span data-ttu-id="12995-553">El servicio de nivel superior para el uso.</span><span class="sxs-lookup"><span data-stu-id="12995-553">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-554">Id. de medidor</span><span class="sxs-lookup"><span data-stu-id="12995-554">Meter Id</span></span></td>
<td><p><span data-ttu-id="12995-555">El identificador del medidor que se va a usar.</span><span class="sxs-lookup"><span data-stu-id="12995-555">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-556">Subcategoría de medidor</span><span class="sxs-lookup"><span data-stu-id="12995-556">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="12995-557">El tipo de servicio de Azure que puede afectar a la tarifa.</span><span class="sxs-lookup"><span data-stu-id="12995-557">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-558">Nombre de medidor</span><span class="sxs-lookup"><span data-stu-id="12995-558">Meter Name</span></span></td>
<td><p><span data-ttu-id="12995-559">La unidad de medida del medidor consumido.</span><span class="sxs-lookup"><span data-stu-id="12995-559">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-560">Región de medidor</span><span class="sxs-lookup"><span data-stu-id="12995-560">Meter Region</span></span></td>
<td><p><span data-ttu-id="12995-561">Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena.</span><span class="sxs-lookup"><span data-stu-id="12995-561">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-562">Unidad</span><span class="sxs-lookup"><span data-stu-id="12995-562">Unit</span></span></td>
<td><p><span data-ttu-id="12995-563">La unidad del nombre de recurso.</span><span class="sxs-lookup"><span data-stu-id="12995-563">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-564">Cantidad consumida</span><span class="sxs-lookup"><span data-stu-id="12995-564">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="12995-565">La cantidad de servicio consumida (horas, GB, etc.) durante el período de notificación.</span><span class="sxs-lookup"><span data-stu-id="12995-565">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="12995-566">También incluye cualquier uso no facturado de períodos anteriores.</span><span class="sxs-lookup"><span data-stu-id="12995-566">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-567">Ubicación de recursos</span><span class="sxs-lookup"><span data-stu-id="12995-567">Resource Location</span></span></td>
<td><p><span data-ttu-id="12995-568">El centro de datos donde se está ejecutando el medidor.</span><span class="sxs-lookup"><span data-stu-id="12995-568">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-569">Servicio consumido</span><span class="sxs-lookup"><span data-stu-id="12995-569">Consumed Service</span></span></td>
<td><p><span data-ttu-id="12995-570">El servicio de la plataforma Azure que usó.</span><span class="sxs-lookup"><span data-stu-id="12995-570">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-571">Grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="12995-571">Resource Group</span></span></td>
<td><p><span data-ttu-id="12995-572">El grupo de recursos en el que se está ejecutando el medidor implementado.</span><span class="sxs-lookup"><span data-stu-id="12995-572">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-573">URI de recurso</span><span class="sxs-lookup"><span data-stu-id="12995-573">Resource URI</span></span></td>
<td><p><span data-ttu-id="12995-574">El URI del recurso que se va a usar.</span><span class="sxs-lookup"><span data-stu-id="12995-574">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-575">Tipo de cargo</span><span class="sxs-lookup"><span data-stu-id="12995-575">Charge type</span></span></td>
<td><p><span data-ttu-id="12995-576">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="12995-576">The type of charge or adjustment.</span></span> <span data-ttu-id="12995-577">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="12995-577">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-578">Precio unitario</span><span class="sxs-lookup"><span data-stu-id="12995-578">Unit price</span></span></td>
<td><p><span data-ttu-id="12995-579">Precio por licencia, como se publica en la lista de precios en el momento de la compra.</span><span class="sxs-lookup"><span data-stu-id="12995-579">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="12995-580">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-580">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-581">Cantidad</span><span class="sxs-lookup"><span data-stu-id="12995-581">Quantity</span></span></td>
<td><p><span data-ttu-id="12995-582">Número de licencias.</span><span class="sxs-lookup"><span data-stu-id="12995-582">Number of licenses.</span></span> <span data-ttu-id="12995-583">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-584">Tipo de unidad</span><span class="sxs-lookup"><span data-stu-id="12995-584">Unit type</span></span></td>
<td><p><span data-ttu-id="12995-585">El tipo de unidad que se cobra el medidor.</span><span class="sxs-lookup"><span data-stu-id="12995-585">The type of unit the meter is charged in.</span></span> <span data-ttu-id="12995-586">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="12995-586">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-587">Impuestos de facturación anterior a</span><span class="sxs-lookup"><span data-stu-id="12995-587">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="12995-588">Cantidad total antes de impuestos.</span><span class="sxs-lookup"><span data-stu-id="12995-588">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-589">Divisa de facturación</span><span class="sxs-lookup"><span data-stu-id="12995-589">Billing currency</span></span></td>
<td><p><span data-ttu-id="12995-590">La moneda en la región geográfica del cliente</span><span class="sxs-lookup"><span data-stu-id="12995-590">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-591">Precio total antes de impuestos</span><span class="sxs-lookup"><span data-stu-id="12995-591">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="12995-592">Los precios antes de que se agregan los impuestos.</span><span class="sxs-lookup"><span data-stu-id="12995-592">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-593">Precios de moneda</span><span class="sxs-lookup"><span data-stu-id="12995-593">Pricing currency</span></span></td>
<td><p><span data-ttu-id="12995-594">La moneda en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="12995-594">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-595">Información de servicio 1</span><span class="sxs-lookup"><span data-stu-id="12995-595">Service Info 1</span></span></td>
<td><p><span data-ttu-id="12995-596">Número de conexiones de Bus de servicio aprovisionadas y usadas en un día determinado.</span><span class="sxs-lookup"><span data-stu-id="12995-596">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-597">Información de servicio 2</span><span class="sxs-lookup"><span data-stu-id="12995-597">Service Info 2</span></span></td>
<td><p><span data-ttu-id="12995-598">Un campo heredado que captura los metadatos específicos del servicio opcional.</span><span class="sxs-lookup"><span data-stu-id="12995-598">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="12995-599">Etiquetas</span><span class="sxs-lookup"><span data-stu-id="12995-599">Tags</span></span></td>
<td><p><span data-ttu-id="12995-600">Etiquetas que asigna al medidor en orden para agrupar los registros de facturación.</span><span class="sxs-lookup"><span data-stu-id="12995-600">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="12995-601">Por ejemplo, puede usar etiquetas para distribuir los costos por el departamento que utiliza el medidor.</span><span class="sxs-lookup"><span data-stu-id="12995-601">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="12995-602">Información adicional</span><span class="sxs-lookup"><span data-stu-id="12995-602">Additional Info</span></span></td>
<td><p><span data-ttu-id="12995-603">Cualquier información adicional que no se tratan en otras columnas.</span><span class="sxs-lookup"><span data-stu-id="12995-603">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="12995-604">Asignación de cargos entre una factura y el archivo de conciliación</span><span class="sxs-lookup"><span data-stu-id="12995-604">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="12995-605">La factura proporciona un resumen de los cargos, mientras que el archivo de conciliación proporciona un desglose detallado de las transacciones de elementos de línea, incluidos los tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="12995-605">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="12995-606">Para hacer referencias cruzadas de cantidades de cargos entre el archivo de conciliación y la factura, puedes usar las opciones de filtro de Microsoft Excel para filtrar por tipo de cargo en el archivo de conciliación con el fin de asignar los cargos de facturación a un conjunto de desgloses de cargos del archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-606">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="12995-607">Los archivos de conciliación, tanto basados en uso como en licencias, solo muestran cargos y transacciones relacionados con el uso (unidades consumidas y cargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="12995-607">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="12995-608">En el archivo de conciliación no aparecen devoluciones, descuentos o créditos excepcionales que aparecen en la factura como "Ajustes".</span><span class="sxs-lookup"><span data-stu-id="12995-608">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="12995-609">La siguiente tabla muestra las asignaciones entre una sección de factura y los tipos de cargo asociados que es posible que se muestren en los archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="12995-609">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="12995-610"><strong>Descripción de cargos de facturación</strong></span><span class="sxs-lookup"><span data-stu-id="12995-610"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-611"><strong>Descripción de cargos del archivo de conciliación (columna ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="12995-611"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-612"><strong>¿Qué es este cargo?</strong></span><span class="sxs-lookup"><span data-stu-id="12995-612"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-613"><strong>¿Cómo se asignan estos ChargeTypes a la factura?</strong></span><span class="sxs-lookup"><span data-stu-id="12995-613"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="12995-614"><strong>Cargos de licencia</strong></span><span class="sxs-lookup"><span data-stu-id="12995-614"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-615">Tarifa de activación</span><span class="sxs-lookup"><span data-stu-id="12995-615">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-616">El importe cobrado al cliente cuando usa la suscripción después de adquirirla</span><span class="sxs-lookup"><span data-stu-id="12995-616">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="12995-617">Desde el archivo basado en licencia, suma la columna <strong>Amount</strong>.</span><span class="sxs-lookup"><span data-stu-id="12995-617">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="12995-618">Cuota de cancelación</span><span class="sxs-lookup"><span data-stu-id="12995-618">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-619">Cargos prorrateados reembolsados al cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="12995-619">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="12995-620">Tarifa de ciclo</span><span class="sxs-lookup"><span data-stu-id="12995-620">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-621">Cargos periódicos de una suscripción</span><span class="sxs-lookup"><span data-stu-id="12995-621">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="12995-622">Prorrateo de instancia de ciclo</span><span class="sxs-lookup"><span data-stu-id="12995-622">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-623">Cargos prorrateados evaluados del cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="12995-623">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="12995-624">Tarifas prorrateadas al cancelar</span><span class="sxs-lookup"><span data-stu-id="12995-624">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-625">Reembolso prorrateado de la parte no usada del servicio tras la cancelación</span><span class="sxs-lookup"><span data-stu-id="12995-625">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="12995-626">Tarifas prorrateadas al comprar</span><span class="sxs-lookup"><span data-stu-id="12995-626">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-627">El tipo de gasto para una suscripción cuando se usa la facturación anual</span><span class="sxs-lookup"><span data-stu-id="12995-627">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="12995-628">Tarifa de compra</span><span class="sxs-lookup"><span data-stu-id="12995-628">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-629">El tipo de gasto para una suscripción cuando se usa la facturación mensual</span><span class="sxs-lookup"><span data-stu-id="12995-629">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="12995-630">Tarifa prorrateada al renovar</span><span class="sxs-lookup"><span data-stu-id="12995-630">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-631">Tarifas prorrateadas tras la renovación de la suscripción</span><span class="sxs-lookup"><span data-stu-id="12995-631">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="12995-632">Tarifa de renovación</span><span class="sxs-lookup"><span data-stu-id="12995-632">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-633">Cargo por renovar una suscripción</span><span class="sxs-lookup"><span data-stu-id="12995-633">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="12995-634">Tarifas prorrateadas al activar</span><span class="sxs-lookup"><span data-stu-id="12995-634">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-635">Tarifas prorrateadas desde la activación hasta el final del período de facturación</span><span class="sxs-lookup"><span data-stu-id="12995-635">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><span data-ttu-id="12995-636"><strong>Cargos de uso</strong></span><span class="sxs-lookup"><span data-stu-id="12995-636"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-637">Evaluar la tarifa de uso al cancelar</span><span class="sxs-lookup"><span data-stu-id="12995-637">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-638">Tarifa de uso de acceso tras la cancelación por uso impagado durante el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="12995-638">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="12995-639">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="12995-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="12995-640">Evaluar la tarifa de uso para el ciclo actual</span><span class="sxs-lookup"><span data-stu-id="12995-640">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-641">tarifa de uso de acceso para el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="12995-641">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="12995-642"><strong>Créditos</strong></span><span class="sxs-lookup"><span data-stu-id="12995-642"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-643">Desplazamiento de un elemento de línea</span><span class="sxs-lookup"><span data-stu-id="12995-643">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-644">Reembolso parcial o total de un elemento de línea, incluidos impuestos</span><span class="sxs-lookup"><span data-stu-id="12995-644">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-645">Desde el archivo basado en licencia, suma la columna <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="12995-645">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="12995-646">Desde el archivo basado en uso, suma la columna <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="12995-646">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="12995-647"><strong>Descuentos basados en uso</strong></span><span class="sxs-lookup"><span data-stu-id="12995-647"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-648">Descuento de activación</span><span class="sxs-lookup"><span data-stu-id="12995-648">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-649">Descuento que se aplica cuando se activa la suscripción</span><span class="sxs-lookup"><span data-stu-id="12995-649">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="12995-650">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="12995-650">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="12995-651">Descuento de ciclo</span><span class="sxs-lookup"><span data-stu-id="12995-651">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-652">Descuento que se aplica en cargos periódicos</span><span class="sxs-lookup"><span data-stu-id="12995-652">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="12995-653">Descuento de renovación</span><span class="sxs-lookup"><span data-stu-id="12995-653">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-654">Descuento que se aplica cuando se renueva la suscripción</span><span class="sxs-lookup"><span data-stu-id="12995-654">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="12995-655">Descuento de cancelación</span><span class="sxs-lookup"><span data-stu-id="12995-655">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-656">Cargos que se aplican cuando se cancelan los descuentos</span><span class="sxs-lookup"><span data-stu-id="12995-656">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="12995-657"><strong>Descuentos de licencias</strong></span><span class="sxs-lookup"><span data-stu-id="12995-657"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-658"><em>Se pueden aplicar a varios tipos de cargos</em></span><span class="sxs-lookup"><span data-stu-id="12995-658"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="12995-659">Desde el archivo basado en licencia, suma la columna <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="12995-659">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="12995-660"><strong>Impuestos</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="12995-660"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-661"><em>Se pueden aplicar a varios tipos de cargos</em></span><span class="sxs-lookup"><span data-stu-id="12995-661"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="12995-662"><em>Excepción: &quot;Desplazamiento de un elemento de línea&quot; ya incluye los impuestos. Consulte los créditos, más arriba.</em></span><span class="sxs-lookup"><span data-stu-id="12995-662"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-663">Impuestos o impuesto de valor añadido (IVA)</span><span class="sxs-lookup"><span data-stu-id="12995-663">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="12995-664">Desde el archivo basado en licencia, suma la columna <strong>Tax</strong>.</span><span class="sxs-lookup"><span data-stu-id="12995-664">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="12995-665">Desde el archivo basado en uso, suma la columna <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="12995-665">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
