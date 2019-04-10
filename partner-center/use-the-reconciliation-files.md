---
title: Usar los archivos de conciliación | Centro de partners
ms.topic: article
ms.date: 10/29/2018
description: Para obtener una vista detallada del elemento de línea de cada carga de un ciclo de facturación, descargue los archivos de conciliación de centro de partners.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0d986ca81e77578ecbb79b909d8f2a8afc4777e4
ms.sourcegitcommit: 275d3eee5613d52f0ac7b8c78f7a7ddd74f56c9e
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/10/2019
ms.locfileid: "59430204"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="b423a-103">Usar los archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="b423a-103">Use the reconciliation files</span></span>

**<span data-ttu-id="b423a-104">Se aplica a</span><span class="sxs-lookup"><span data-stu-id="b423a-104">Applies to</span></span>**

-  <span data-ttu-id="b423a-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="b423a-105">Partner Center</span></span>
-  <span data-ttu-id="b423a-106">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="b423a-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="b423a-107">Para obtener una vista detallada del elemento de línea de cada carga de un ciclo de facturación, descargue los archivos de conciliación de centro de partners.</span><span class="sxs-lookup"><span data-stu-id="b423a-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="b423a-108">Los detalles incluyen los cargos para las suscripciones de cada cliente y los eventos detallados (por ejemplo, una adición intermedia de puestos en una suscripción).</span><span class="sxs-lookup"><span data-stu-id="b423a-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="b423a-109">Problemas de formato</span><span class="sxs-lookup"><span data-stu-id="b423a-109">Formatting issues</span></span>

<span data-ttu-id="b423a-110">En ocasiones, el archivo de conciliación podría tener problemas de formato.</span><span class="sxs-lookup"><span data-stu-id="b423a-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="b423a-111">(Esto puede ocurrir, por ejemplo, si no se usa la configuración regional EN-US). Siga estos pasos para corregir estos problemas.</span><span class="sxs-lookup"><span data-stu-id="b423a-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="b423a-112">Abra el archivo .csv en Excel y seleccione la primera columna.</span><span class="sxs-lookup"><span data-stu-id="b423a-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="b423a-113">En la cinta de opciones, seleccione <strong>datos</strong>y, a continuación, seleccione <strong>texto en columnas</strong>.</span><span class="sxs-lookup"><span data-stu-id="b423a-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="b423a-114">En convertir texto en el Asistente de columnas, seleccione <strong>delimitado por tipo de archivo</strong>y, a continuación, seleccione <strong>siguiente</strong>.</span><span class="sxs-lookup"><span data-stu-id="b423a-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="b423a-115">En el campo delimitadores, seleccione <strong>comas</strong>.</span><span class="sxs-lookup"><span data-stu-id="b423a-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="b423a-116">Si <strong>ficha</strong> está ya seleccionado, puede dejarla.</span><span class="sxs-lookup"><span data-stu-id="b423a-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="b423a-117">Selecciona <strong>Siguiente</strong>.</span><span class="sxs-lookup"><span data-stu-id="b423a-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="b423a-118">En el campo de formato de datos de columna, seleccione <strong>fecha: MDY</strong>y, a continuación, seleccione <strong>siguiente</strong>.</span><span class="sxs-lookup"><span data-stu-id="b423a-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="b423a-119">En el campo de formato de datos de columna, seleccione <strong>texto</strong> para amount, todas las columnas y, a continuación, seleccione <strong>finalizar</strong>.</span><span class="sxs-lookup"><span data-stu-id="b423a-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="b423a-120">Detallar asociado</span><span class="sxs-lookup"><span data-stu-id="b423a-120">Itemize by partner</span></span>


<span data-ttu-id="b423a-121">Los partners del modelo indirecto pueden usar estos campos adicionales en ambos archivos de conciliación basada en uso y en licencia para realizar el desglose por revendedor.</span><span class="sxs-lookup"><span data-stu-id="b423a-121">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b423a-122">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="b423a-122">MPN ID</span></span></th>
<th><span data-ttu-id="b423a-123">Descripción</span><span class="sxs-lookup"><span data-stu-id="b423a-123">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="b423a-124">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="b423a-124">MPN ID</span></span></td>
<td><p><span data-ttu-id="b423a-125">Id. de Microsoft Partner Network (MPN) del partner de CSP (directo o indirecto).</span><span class="sxs-lookup"><span data-stu-id="b423a-125">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-126">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="b423a-126">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="b423a-127">Solo aparece en los archivos de conciliación de partners en el modelo indirecto.</span><span class="sxs-lookup"><span data-stu-id="b423a-127">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="b423a-128">El Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="b423a-128">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b423a-129">Corresponde al id. de revendedor indicado para la suscripción específica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="b423a-129">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="b423a-130">muestra de eTo o actualiza el distribuidor, en el menú del centro de partners, seleccione <strong>clientes</strong>, a continuación, elija el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="b423a-130">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="b423a-131">En el menú del cliente, selecciona <strong>Suscripciones</strong> y elige la suscripción de la lista.</span><span class="sxs-lookup"><span data-stu-id="b423a-131">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="b423a-132">Selecciona <strong>Actualizar</strong> para cambiar el valor de <strong>Revendedor (id. de MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="b423a-132">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="b423a-133">Si un partner CSP vendió la suscripción directamente al cliente, su id. de MPN aparece dos veces, como id. de MPN y como id. de MPN del revendedor.</span><span class="sxs-lookup"><span data-stu-id="b423a-133">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="b423a-134">Si un partner CSP tiene un revendedor sin un id. de MPN, este valor se establece en el id. de MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="b423a-134">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="b423a-135">Si el partner CSP quita un id. de revendedor, este valor se establece en -1.</span><span class="sxs-lookup"><span data-stu-id="b423a-135">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="b423a-136">Campos de archivo de licencia</span><span class="sxs-lookup"><span data-stu-id="b423a-136">License-based file fields</span></span>


<span data-ttu-id="b423a-137">Para conciliar los cargos en función de los pedidos del cliente, compara el Syndication\_Partner\_Subscription\_Number del archivo de conciliación con el id. de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="b423a-137">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="b423a-138">Column</span><span class="sxs-lookup"><span data-stu-id="b423a-138">Column</span></span></strong></td>
<td><strong><span data-ttu-id="b423a-139">Descripción</span><span class="sxs-lookup"><span data-stu-id="b423a-139">Description</span></span></strong></td>
<td><strong><span data-ttu-id="b423a-140">Valor de muestra</span><span class="sxs-lookup"><span data-stu-id="b423a-140">Sample Value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-141">PartnerId</span><span class="sxs-lookup"><span data-stu-id="b423a-141">PartnerId</span></span></td>
<td><p><span data-ttu-id="b423a-142">Identificador único de una entidad de facturación específica, con formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="b423a-142">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="b423a-143">No es necesario para la reconciliación, pero puede ser información útil.</span><span class="sxs-lookup"><span data-stu-id="b423a-143">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="b423a-144">Igual en todas las filas.</span><span class="sxs-lookup"><span data-stu-id="b423a-144">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="b423a-145">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="b423a-145">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-146">CustomerID</span><span class="sxs-lookup"><span data-stu-id="b423a-146">CustomerID</span></span></td>
<td><p><span data-ttu-id="b423a-147">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="b423a-147">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="b423a-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="b423a-148">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-149">OrderID</span><span class="sxs-lookup"><span data-stu-id="b423a-149">OrderID</span></span></td>
<td><p><span data-ttu-id="b423a-150">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b423a-150">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="b423a-151">Puede ser útil para identificar al pedido al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-151">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="b423a-152">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="b423a-152">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-153">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="b423a-153">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="b423a-154">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b423a-154">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b423a-155">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-155">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="b423a-156">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="b423a-156">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="b423a-157">Consulte Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="b423a-157">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="b423a-158">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="b423a-158">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-159">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="b423a-159">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="b423a-160">Identificador único de las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="b423a-160">Unique identifier for subscriptions.</span></span> <span data-ttu-id="b423a-161">Un cliente puede tener varias suscripciones para el mismo plan, por lo que es importante para el análisis de archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-161">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="b423a-162">Este campo se asigna al identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="b423a-162">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="b423a-163">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="b423a-163">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-164">OfferID</span><span class="sxs-lookup"><span data-stu-id="b423a-164">OfferID</span></span></td>
<td><p><span data-ttu-id="b423a-165">Identificador único de la oferta.</span><span class="sxs-lookup"><span data-stu-id="b423a-165">Unique offer ID.</span></span> <span data-ttu-id="b423a-166">Identificador de la oferta estándar según la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="b423a-166">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="b423a-167"><b>Nota</b>: Este valor no coincide con Id. de oferta desde la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="b423a-167"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="b423a-168">Consulta DurableOfferID a continuación.</span><span class="sxs-lookup"><span data-stu-id="b423a-168">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="b423a-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="b423a-169">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-170">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="b423a-170">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="b423a-171">Identificador único de oferta duradera, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="b423a-171">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="b423a-172"><b>Nota</b>: Este valor coincide con el Id. de oferta desde la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="b423a-172"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="b423a-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="b423a-173">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-174">OfferName</span><span class="sxs-lookup"><span data-stu-id="b423a-174">OfferName</span></span></td>
<td><p><span data-ttu-id="b423a-175">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="b423a-175">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="b423a-176">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="b423a-176">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-177">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="b423a-177">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="b423a-178">Fecha de finalización de la suscripción, establecida en el día posterior al envío del pedido.</span><span class="sxs-lookup"><span data-stu-id="b423a-178">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="b423a-179">Al consultar la fecha de inicio de la suscripción junto con la fecha de finalización, puedes determinar si el cliente aún está dentro del primer año de la suscripción o si la suscripción se ha renovado para el año siguiente.</span><span class="sxs-lookup"><span data-stu-id="b423a-179">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="b423a-180">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="b423a-180">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b423a-181">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b423a-181">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-182">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="b423a-182">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="b423a-183">La fecha de finalización de la suscripción: 12 meses + x días después de la fecha de inicio (para alinearse con fecha de facturación del asociado) o 12 meses a partir de la fecha de renovación.</span><span class="sxs-lookup"><span data-stu-id="b423a-183">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="b423a-184">En el momento de la renovación, los precios se actualizan según la lista de precios actual.</span><span class="sxs-lookup"><span data-stu-id="b423a-184">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="b423a-185">Es posible que se necesite una comunicación con el cliente antes de la renovación automatizada.</span><span class="sxs-lookup"><span data-stu-id="b423a-185">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="b423a-186">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="b423a-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b423a-187">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b423a-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-188">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b423a-188">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b423a-189">Día de inicio de los cargos.</span><span class="sxs-lookup"><span data-stu-id="b423a-189">Start day of the charges.</span></span></p>
<p><span data-ttu-id="b423a-190">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="b423a-190">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="b423a-191">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="b423a-191">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b423a-192">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="b423a-192">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-193">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b423a-193">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b423a-194">Día de finalización de los cargos.</span><span class="sxs-lookup"><span data-stu-id="b423a-194">End day of the charges.</span></span></p>
<p><span data-ttu-id="b423a-195">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="b423a-195">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="b423a-196">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="b423a-196">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="b423a-197">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="b423a-197">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-198">ChargeType</span><span class="sxs-lookup"><span data-stu-id="b423a-198">ChargeType</span></span></td>
<td><p><span data-ttu-id="b423a-199">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="b423a-199">The type of charge or adjustment.</span></span> <span data-ttu-id="b423a-200">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="b423a-200">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="b423a-201">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="b423a-201">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-202">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="b423a-202">UnitPrice</span></span></td>
<td><p><span data-ttu-id="b423a-203">Precio por puesto, tal y como se publica en la lista de precios en el momento de compra.</span><span class="sxs-lookup"><span data-stu-id="b423a-203">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b423a-204">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-204">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="b423a-205">6.82</span><span class="sxs-lookup"><span data-stu-id="b423a-205">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-206">Cantidad</span><span class="sxs-lookup"><span data-stu-id="b423a-206">Quantity</span></span></td>
<td><p><span data-ttu-id="b423a-207">Número de puestos.</span><span class="sxs-lookup"><span data-stu-id="b423a-207">Number of seats.</span></span> <span data-ttu-id="b423a-208">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-208">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="b423a-209">2</span><span class="sxs-lookup"><span data-stu-id="b423a-209">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-210">Volumen</span><span class="sxs-lookup"><span data-stu-id="b423a-210">Amount</span></span></td>
<td><p><span data-ttu-id="b423a-211">Total del precio para la cantidad.</span><span class="sxs-lookup"><span data-stu-id="b423a-211">Total of price for quantity.</span></span> <span data-ttu-id="b423a-212">Es de utilidad para comprobar que el cálculo de la cantidad coincide con la manera de calcular este valor para los clientes.</span><span class="sxs-lookup"><span data-stu-id="b423a-212">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="b423a-213">13.32</span><span class="sxs-lookup"><span data-stu-id="b423a-213">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-214">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="b423a-214">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="b423a-215">Cantidad de descuento que se aplica a estos cargos.</span><span class="sxs-lookup"><span data-stu-id="b423a-215">Amount of discount applied to these charges.</span></span> <span data-ttu-id="b423a-216">Los IUR o las nuevas suscripciones que puedan optar a un incentivo también incluirán un importe de descuento en esta columna.</span><span class="sxs-lookup"><span data-stu-id="b423a-216">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="b423a-217">2.32</span><span class="sxs-lookup"><span data-stu-id="b423a-217">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-218">Subtotal</span><span class="sxs-lookup"><span data-stu-id="b423a-218">Subtotal</span></span></td>
<td><p><span data-ttu-id="b423a-219">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="b423a-219">Total before tax.</span></span> <span data-ttu-id="b423a-220">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="b423a-220">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="b423a-221">11</span><span class="sxs-lookup"><span data-stu-id="b423a-221">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-222">Impuestos</span><span class="sxs-lookup"><span data-stu-id="b423a-222">Tax</span></span></td>
<td><p><span data-ttu-id="b423a-223">Importe de impuestos, según el mercado&#39;reglas s y circunstancias concretas.</span><span class="sxs-lookup"><span data-stu-id="b423a-223">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="b423a-224">0</span><span class="sxs-lookup"><span data-stu-id="b423a-224">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-225">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="b423a-225">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="b423a-226">Total con impuestos.</span><span class="sxs-lookup"><span data-stu-id="b423a-226">Total after tax.</span></span> <span data-ttu-id="b423a-227">Comprueba si se cobran impuestos en la factura.</span><span class="sxs-lookup"><span data-stu-id="b423a-227">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="b423a-228">11</span><span class="sxs-lookup"><span data-stu-id="b423a-228">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-229">Moneda</span><span class="sxs-lookup"><span data-stu-id="b423a-229">Currency</span></span></td>
<td><p><span data-ttu-id="b423a-230">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="b423a-230">Currency type.</span></span> <span data-ttu-id="b423a-231">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="b423a-231">Each billing entity has only one currency.</span></span> <span data-ttu-id="b423a-232">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="b423a-232">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="b423a-233">EUR</span><span class="sxs-lookup"><span data-stu-id="b423a-233">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-234">CustomerName</span><span class="sxs-lookup"><span data-stu-id="b423a-234">CustomerName</span></span></td>
<td><p><span data-ttu-id="b423a-235">Cliente&#39;nombre de la organización s notificados en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="b423a-235">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="b423a-236">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="b423a-236">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="b423a-237">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="b423a-237">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-238">MPNID</span><span class="sxs-lookup"><span data-stu-id="b423a-238">MPNID</span></span></td>
<td><p><span data-ttu-id="b423a-239">Id. de MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="b423a-239">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="b423a-240">4390934</span><span class="sxs-lookup"><span data-stu-id="b423a-240">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-241">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="b423a-241">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="b423a-242">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="b423a-242">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b423a-243">Ver <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Desglosar por partner</a></span><span class="sxs-lookup"><span data-stu-id="b423a-243">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="b423a-244">4390934</span><span class="sxs-lookup"><span data-stu-id="b423a-244">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-245">DomainName</span><span class="sxs-lookup"><span data-stu-id="b423a-245">DomainName</span></span></td>
<td><p><span data-ttu-id="b423a-246">Cliente&#39;nombre de dominio de s, que ayuda a identificar el cliente.</span><span class="sxs-lookup"><span data-stu-id="b423a-246">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="b423a-247">No debe usarse para identificar al cliente como el cliente o socio puede actualizar el dominio personal de forma predeterminada a través del portal de Office 365.</span><span class="sxs-lookup"><span data-stu-id="b423a-247">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="b423a-248">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="b423a-248">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="b423a-249">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b423a-249">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-250">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="b423a-250">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="b423a-251">Alias de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="b423a-251">Subscription nickname.</span></span> <span data-ttu-id="b423a-252">Si no se especifica ningún alias, el Centro de partners usa OfferName.</span><span class="sxs-lookup"><span data-stu-id="b423a-252">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="b423a-253">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="b423a-253">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-254">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="b423a-254">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="b423a-255">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="b423a-255">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="b423a-256">(Este es un campo idéntico al nombre de la oferta).</span><span class="sxs-lookup"><span data-stu-id="b423a-256">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="b423a-257">PROJECT ONLINE PREMIUM SIN CLIENTE DE PROJECT</span><span class="sxs-lookup"><span data-stu-id="b423a-257">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="b423a-258">Campos de archivo basada en uso</span><span class="sxs-lookup"><span data-stu-id="b423a-258">Usage-based file fields</span></span>


<span data-ttu-id="b423a-259">Para conciliar los cargos en función del uso de tu cliente, compara los valores de ResellerID/ResellerName/ResellerBillableAccount del archivo de conciliación, el nombre del cliente y el id. de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="b423a-259">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="b423a-260">Los siguientes campos explican los servicios usados y la clasificación.</span><span class="sxs-lookup"><span data-stu-id="b423a-260">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="b423a-261">Column</span><span class="sxs-lookup"><span data-stu-id="b423a-261">Column</span></span></strong></td>
<td><strong><span data-ttu-id="b423a-262">Descripción</span><span class="sxs-lookup"><span data-stu-id="b423a-262">Description</span></span></strong></td>
<td><strong><span data-ttu-id="b423a-263">Valor de muestra</span><span class="sxs-lookup"><span data-stu-id="b423a-263">Sample value</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-264">PartnerID</span><span class="sxs-lookup"><span data-stu-id="b423a-264">PartnerID</span></span></td>
<td><p><span data-ttu-id="b423a-265">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="b423a-265">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="b423a-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="b423a-266">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-267">PartnerName</span><span class="sxs-lookup"><span data-stu-id="b423a-267">PartnerName</span></span></td>
<td><p><span data-ttu-id="b423a-268">Nombre del partner.</span><span class="sxs-lookup"><span data-stu-id="b423a-268">Partner Name.</span></span></p></td>
<td><span data-ttu-id="b423a-269">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="b423a-269">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-270">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="b423a-270">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="b423a-271">Id. de cuenta del partner.</span><span class="sxs-lookup"><span data-stu-id="b423a-271">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="b423a-272">1010578050</span><span class="sxs-lookup"><span data-stu-id="b423a-272">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-273">CustomerName</span><span class="sxs-lookup"><span data-stu-id="b423a-273">CustomerName</span></span></td>
<td><p><span data-ttu-id="b423a-274">Cliente&#39;nombre de la organización s notificados en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="b423a-274">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="b423a-275">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="b423a-275">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="b423a-276">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="b423a-276">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-277">MPNID</span><span class="sxs-lookup"><span data-stu-id="b423a-277">MPNID</span></span></td>
<td><p><span data-ttu-id="b423a-278">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="b423a-278">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="b423a-279">4390934</span><span class="sxs-lookup"><span data-stu-id="b423a-279">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-280">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="b423a-280">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="b423a-281">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="b423a-281">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b423a-282">Ver <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Desglosar por partner</a></span><span class="sxs-lookup"><span data-stu-id="b423a-282">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="b423a-283">4390934</span><span class="sxs-lookup"><span data-stu-id="b423a-283">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-284">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="b423a-284">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="b423a-285">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="b423a-285">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="b423a-286">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="b423a-286">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-287">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b423a-287">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b423a-288">Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="b423a-288">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="b423a-289">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="b423a-289">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="b423a-290">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="b423a-290">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-291">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b423a-291">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b423a-292">Fecha de finalización del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="b423a-292">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="b423a-293">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="b423a-293">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="b423a-294">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="b423a-294">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-295">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="b423a-295">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="b423a-296">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b423a-296">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b423a-297">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-297">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="b423a-298">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="b423a-298">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="b423a-299">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="b423a-299">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-300">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="b423a-300">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="b423a-301">Alias de la oferta de servicio.</span><span class="sxs-lookup"><span data-stu-id="b423a-301">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="b423a-302">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b423a-302">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-303">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="b423a-303">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="b423a-304">Línea de negocio de la oferta de servicio</span><span class="sxs-lookup"><span data-stu-id="b423a-304">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="b423a-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="b423a-305">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-306">OrderID</span><span class="sxs-lookup"><span data-stu-id="b423a-306">OrderID</span></span></td>
<td><p><span data-ttu-id="b423a-307">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b423a-307">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="b423a-308">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-308">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="b423a-309">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="b423a-309">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-310">ServiceName</span><span class="sxs-lookup"><span data-stu-id="b423a-310">ServiceName</span></span></td>
<td><p><span data-ttu-id="b423a-311">Nombre del servicio de Azure en cuestión.</span><span class="sxs-lookup"><span data-stu-id="b423a-311">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="b423a-312">MÁQUINAS VIRTUALES</span><span class="sxs-lookup"><span data-stu-id="b423a-312">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-313">ServiceType</span><span class="sxs-lookup"><span data-stu-id="b423a-313">ServiceType</span></span></td>
<td><p><span data-ttu-id="b423a-314">Tipo específico de servicio de Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="b423a-314">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="b423a-315">Bus de servicio: individual o paquete</span><span class="sxs-lookup"><span data-stu-id="b423a-315">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="b423a-316">Base de datos SQL Azure: edición Business o Web</span><span class="sxs-lookup"><span data-stu-id="b423a-316">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-317">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="b423a-317">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="b423a-318">Identificador único específico para toda la estructura de precios y datos del servicio.</span><span class="sxs-lookup"><span data-stu-id="b423a-318">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="b423a-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="b423a-319">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-320">Nombre de recurso</span><span class="sxs-lookup"><span data-stu-id="b423a-320">Resource Name</span></span></td>
<td><p><span data-ttu-id="b423a-321">Nombre del recurso de Azure.</span><span class="sxs-lookup"><span data-stu-id="b423a-321">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="b423a-322">Transferencia entrante de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="b423a-322">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="b423a-323">Transferencia saliente de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="b423a-323">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-324">Region</span><span class="sxs-lookup"><span data-stu-id="b423a-324">Region</span></span></td>
<td><p><span data-ttu-id="b423a-325">La región a la que se aplica el uso.</span><span class="sxs-lookup"><span data-stu-id="b423a-325">The region the usage applies to.</span></span> <span data-ttu-id="b423a-326">Se usa principalmente para asignar tarifas a las transferencias de datos, ya que las tarifas varían según la región.</span><span class="sxs-lookup"><span data-stu-id="b423a-326">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="b423a-327">Asia Pacífico, Europa, América Latina, América del Norte</span><span class="sxs-lookup"><span data-stu-id="b423a-327">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-328">SKU</span><span class="sxs-lookup"><span data-stu-id="b423a-328">SKU</span></span></td>
<td><p><span data-ttu-id="b423a-329">Identificador único de MSFT para la oferta</span><span class="sxs-lookup"><span data-stu-id="b423a-329">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="b423a-330">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="b423a-330">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="b423a-331">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="b423a-331">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="b423a-332">Un id. y una cantidad para desglosar las distintas clasificaciones de un servicio o un recurso en un período de facturación determinado.</span><span class="sxs-lookup"><span data-stu-id="b423a-332">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="b423a-333">Para clasificación en niveles de Azure, puede haber una clasificación hasta una cantidad determinada de unidades facturables y, posteriormente, una clasificación diferente.</span><span class="sxs-lookup"><span data-stu-id="b423a-333">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="b423a-334">1</span><span class="sxs-lookup"><span data-stu-id="b423a-334">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-335">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="b423a-335">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="b423a-336">La cantidad de servicio consumida (horas, GB, etc.) durante el período de notificación.</span><span class="sxs-lookup"><span data-stu-id="b423a-336">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="b423a-337">También incluye cualquier uso no facturado de períodos anteriores.</span><span class="sxs-lookup"><span data-stu-id="b423a-337">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="b423a-338">11</span><span class="sxs-lookup"><span data-stu-id="b423a-338">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-339">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="b423a-339">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="b423a-340">Unidades que se incluyen como parte de la oferta.</span><span class="sxs-lookup"><span data-stu-id="b423a-340">Units included as part of the offer.</span></span> <span data-ttu-id="b423a-341">No suele mostrarse en CSP.</span><span class="sxs-lookup"><span data-stu-id="b423a-341">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="b423a-342">0</span><span class="sxs-lookup"><span data-stu-id="b423a-342">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="b423a-343">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="b423a-343">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="b423a-344">Unidades que no se incluyen como parte de la oferta y que el partner debe abonar.</span><span class="sxs-lookup"><span data-stu-id="b423a-344">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="b423a-345">Equivale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="b423a-345">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="b423a-346">11</span><span class="sxs-lookup"><span data-stu-id="b423a-346">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-347">ListPrice</span><span class="sxs-lookup"><span data-stu-id="b423a-347">ListPrice</span></span></td>
<td><p><span data-ttu-id="b423a-348">Precio de la oferta en vigor la fecha de inicio de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="b423a-348">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="b423a-349">0.0808 USD</span><span class="sxs-lookup"><span data-stu-id="b423a-349">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-350">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="b423a-350">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="b423a-351">ListPrist x OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="b423a-351">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b423a-352">0.085 USD</span><span class="sxs-lookup"><span data-stu-id="b423a-352">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-353">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="b423a-353">TaxAmount</span></span></td>
<td><p><span data-ttu-id="b423a-354">Importe de impuestos, según el mercado&#39;reglas s y circunstancias concretas.</span><span class="sxs-lookup"><span data-stu-id="b423a-354">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="b423a-355">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="b423a-355">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-356">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="b423a-356">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="b423a-357">Total con impuestos, si se aplican impuestos.</span><span class="sxs-lookup"><span data-stu-id="b423a-357">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="b423a-358">0.93 USD</span><span class="sxs-lookup"><span data-stu-id="b423a-358">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-359">Moneda</span><span class="sxs-lookup"><span data-stu-id="b423a-359">Currency</span></span></td>
<td><p><span data-ttu-id="b423a-360">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="b423a-360">Currency type.</span></span> <span data-ttu-id="b423a-361">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="b423a-361">Each billing entity has only one currency.</span></span> <span data-ttu-id="b423a-362">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="b423a-362">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="b423a-363">EUR</span><span class="sxs-lookup"><span data-stu-id="b423a-363">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-364">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="b423a-364">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="b423a-365">Precio sin impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="b423a-365">Pretax price per unit.</span></span> <span data-ttu-id="b423a-366">Igual que PretaxCharges/OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="b423a-366">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b423a-367">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="b423a-367">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-368">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="b423a-368">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="b423a-369">Precio después de impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="b423a-369">Post tax price per unit.</span></span> <span data-ttu-id="b423a-370">Igual que PostTaxTotal/OverageQuantity o PretaxEffectiveRate + tipo impositivo por importe unitario, redondeado el céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="b423a-370">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="b423a-371">0.08 USD</span><span class="sxs-lookup"><span data-stu-id="b423a-371">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-372">ChargeType</span><span class="sxs-lookup"><span data-stu-id="b423a-372">ChargeType</span></span></td>
<td><p><span data-ttu-id="b423a-373">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="b423a-373">The type of charge or adjustment.</span></span> <span data-ttu-id="b423a-374">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="b423a-374">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="b423a-375">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="b423a-375">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-376">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="b423a-376">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="b423a-377">Id. de cuenta único en la plataforma de facturación de MSFT.</span><span class="sxs-lookup"><span data-stu-id="b423a-377">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="b423a-378">1280018095</span><span class="sxs-lookup"><span data-stu-id="b423a-378">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-379">UsageDate</span><span class="sxs-lookup"><span data-stu-id="b423a-379">UsageDate</span></span></td>
<td><p><span data-ttu-id="b423a-380">Fecha de implementación del servicio.</span><span class="sxs-lookup"><span data-stu-id="b423a-380">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="b423a-381">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="b423a-381">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-382">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="b423a-382">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="b423a-383">Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena.</span><span class="sxs-lookup"><span data-stu-id="b423a-383">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="b423a-384">Asia oriental, Sur asiático, Norte de Europa, Europa occidental, Norte central de EE. UU., Sur central de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="b423a-384">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-385">MeteredService</span><span class="sxs-lookup"><span data-stu-id="b423a-385">MeteredService</span></span></td>
<td><p><span data-ttu-id="b423a-386">Esta columna se usa para hacer un seguimiento de los servicios de Microsoft Azure individuales que quizás no se identifiquen específicamente en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="b423a-386">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="b423a-387">Por ejemplo, las transferencias de datos se notifican como &quot;Microsoft Azure: todos los servicios&quot; en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="b423a-387">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="b423a-388">En esta columna MeteredService se indicará qué servicio específico pertenece el uso.</span><span class="sxs-lookup"><span data-stu-id="b423a-388">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="b423a-389">AccessControl, CDN, Proceso, Base de datos, ServiceBus, Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="b423a-389">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-390">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="b423a-390">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="b423a-391">Subtítulo que aclara el servicio de Microsoft Azure individual más allá del nivel proporcionado por el campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="b423a-391">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="b423a-392">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="b423a-392">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-393">Proyecto</span><span class="sxs-lookup"><span data-stu-id="b423a-393">Project</span></span></td>
<td><p><span data-ttu-id="b423a-394">Nombre definido por el cliente para la instancia del servicio</span><span class="sxs-lookup"><span data-stu-id="b423a-394">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="b423a-395">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="b423a-395">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-396">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="b423a-396">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="b423a-397">Número de conexiones de Bus de servicio aprovisionadas y usadas en un día determinado.</span><span class="sxs-lookup"><span data-stu-id="b423a-397">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="b423a-398">Por ejemplo: si tenías una conexión aprovisionada individualmente durante un mes de 30 días, Service Info 1 contendría 1 "1,000000 conexiones/30 días".</span><span class="sxs-lookup"><span data-stu-id="b423a-398">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="b423a-399">Si tuviera un paquete de 25 de conexiones de bus de servicio aprovisionada y ha utilizado 1 durante ese día, el extracto de uso diario durante ese día indicaría "25 conexiones / 30 días: utilizado: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="b423a-399">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-400">CustomerID</span><span class="sxs-lookup"><span data-stu-id="b423a-400">CustomerID</span></span></td>
<td><p><span data-ttu-id="b423a-401">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="b423a-401">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="b423a-402">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="b423a-402">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b423a-403">DomainName</span><span class="sxs-lookup"><span data-stu-id="b423a-403">DomainName</span></span></td>
<td><p><span data-ttu-id="b423a-404">Cliente&#39;nombre de dominio de s, que ayuda a identificar el cliente.</span><span class="sxs-lookup"><span data-stu-id="b423a-404">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="b423a-405">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="b423a-405">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="b423a-406">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="b423a-406">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="b423a-407">Unidad</span><span class="sxs-lookup"><span data-stu-id="b423a-407">Unit</span></span></td>
<td><p><span data-ttu-id="b423a-408">La unidad del nombre del recurso</span><span class="sxs-lookup"><span data-stu-id="b423a-408">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="b423a-409">GB u HORAS</span><span class="sxs-lookup"><span data-stu-id="b423a-409">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="b423a-410">Campos del archivo periódicas y únicas</span><span class="sxs-lookup"><span data-stu-id="b423a-410">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b423a-411">Column</span><span class="sxs-lookup"><span data-stu-id="b423a-411">Column</span></span></th>
<th><span data-ttu-id="b423a-412">Descripción</span><span class="sxs-lookup"><span data-stu-id="b423a-412">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="b423a-413">PartnerId</span><span class="sxs-lookup"><span data-stu-id="b423a-413">PartnerId</span></span></td>
<td><p><span data-ttu-id="b423a-414">Identificador único del inquilino de Microsoft Azure Active Directory para una entidad de facturación específica, en formato GUID.</span><span class="sxs-lookup"><span data-stu-id="b423a-414">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="b423a-415">No es necesario para la reconciliación, pero puede ser información útil.</span><span class="sxs-lookup"><span data-stu-id="b423a-415">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="b423a-416">Igual en todas las filas.</span><span class="sxs-lookup"><span data-stu-id="b423a-416">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-417">Id. de cliente</span><span class="sxs-lookup"><span data-stu-id="b423a-417">Customer Id</span></span></td>
<td><p><span data-ttu-id="b423a-418">Microsoft Azure Active Directory inquilino identificador único, en formato GUID, que usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="b423a-418">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-419">Nombre del cliente</span><span class="sxs-lookup"><span data-stu-id="b423a-419">Customer Name</span></span></td>
<td><p><span data-ttu-id="b423a-420">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="b423a-420">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-421">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="b423a-421">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="b423a-422">Nombre de dominio del cliente, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="b423a-422">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="b423a-423">No debe usarse para identificar al cliente como el cliente o socio puede actualizar el dominio personal de forma predeterminada a través del portal de Office 365.</span><span class="sxs-lookup"><span data-stu-id="b423a-423">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="b423a-424">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="b423a-424">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-425">País del cliente</span><span class="sxs-lookup"><span data-stu-id="b423a-425">Customer Country</span></span></td>
<td><p><span data-ttu-id="b423a-426">El país donde se encuentra el cliente.</span><span class="sxs-lookup"><span data-stu-id="b423a-426">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-427">Número de factura</span><span class="sxs-lookup"><span data-stu-id="b423a-427">Invoice number</span></span></td>
<td><p><span data-ttu-id="b423a-428">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="b423a-428">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-429">MpnId</span><span class="sxs-lookup"><span data-stu-id="b423a-429">MpnId</span></span></td>
<td><p><span data-ttu-id="b423a-430">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="b423a-430">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-431">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="b423a-431">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="b423a-432">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="b423a-432">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-433">Id. de pedido</span><span class="sxs-lookup"><span data-stu-id="b423a-433">Order ID</span></span></td>
<td><p><span data-ttu-id="b423a-434">Identificador único para un pedido en la plataforma de comercio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b423a-434">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="b423a-435">Puede ser útil para identificar al pedido al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-435">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-436">Fecha del pedido</span><span class="sxs-lookup"><span data-stu-id="b423a-436">Order date</span></span></td>
<td><p><span data-ttu-id="b423a-437">Fecha de realización del pedido.</span><span class="sxs-lookup"><span data-stu-id="b423a-437">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-438">ProductId</span><span class="sxs-lookup"><span data-stu-id="b423a-438">ProductId</span></span></td>
<td><p><span data-ttu-id="b423a-439">Identificador del producto.</span><span class="sxs-lookup"><span data-stu-id="b423a-439">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-440">SkuId</span><span class="sxs-lookup"><span data-stu-id="b423a-440">SkuId</span></span></td>
<td><p><span data-ttu-id="b423a-441">Id. de un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="b423a-441">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-442">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="b423a-442">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="b423a-443">Id. de una disponibilidad concreta.</span><span class="sxs-lookup"><span data-stu-id="b423a-443">The ID for a particular Availability.</span></span> <span data-ttu-id="b423a-444">"Disponibilidad" hace referencia a si un SKU concreto está o no disponible para su compra para el país, la moneda, el segmento industrial determinados, etc.</span><span class="sxs-lookup"><span data-stu-id="b423a-444">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-445">Nombre de SKU</span><span class="sxs-lookup"><span data-stu-id="b423a-445">SKU Name</span></span></td>
<td><p><span data-ttu-id="b423a-446">Título para un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="b423a-446">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-447">Nombre del producto</span><span class="sxs-lookup"><span data-stu-id="b423a-447">Product name</span></span></td>
<td><p><span data-ttu-id="b423a-448">Nombre del producto.</span><span class="sxs-lookup"><span data-stu-id="b423a-448">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-449">PublisherName</span><span class="sxs-lookup"><span data-stu-id="b423a-449">PublisherName</span></span></td>
<td><p><span data-ttu-id="b423a-450">El nombre del publicador del producto.</span><span class="sxs-lookup"><span data-stu-id="b423a-450">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-451">PublisherID</span><span class="sxs-lookup"><span data-stu-id="b423a-451">PublisherID</span></span></td>
<td><p><span data-ttu-id="b423a-452">Identificador único para este publicador.</span><span class="sxs-lookup"><span data-stu-id="b423a-452">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-453">Descripción de la suscripción</span><span class="sxs-lookup"><span data-stu-id="b423a-453">Subscription Description</span></span></td>
<td><p><span data-ttu-id="b423a-454">Nombre descriptivo de una suscripción.</span><span class="sxs-lookup"><span data-stu-id="b423a-454">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-455">Id. de la suscripción</span><span class="sxs-lookup"><span data-stu-id="b423a-455">Subscription ID</span></span></td>
<td><p><span data-ttu-id="b423a-456">Identificador único para una suscripción en la plataforma de comercio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b423a-456">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="b423a-457">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-457">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="b423a-458">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="b423a-458">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-459">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b423a-459">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b423a-460">Día de inicio de los cargos.</span><span class="sxs-lookup"><span data-stu-id="b423a-460">Start day of the charges.</span></span> <span data-ttu-id="b423a-461">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="b423a-461">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-462">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b423a-462">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b423a-463">Día de finalización de los cargos.</span><span class="sxs-lookup"><span data-stu-id="b423a-463">End day of the charges.</span></span> <span data-ttu-id="b423a-464">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="b423a-464">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-465">Término y Billingcycle</span><span class="sxs-lookup"><span data-stu-id="b423a-465">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="b423a-466">La duración del período y ciclo de facturación para la compra.</span><span class="sxs-lookup"><span data-stu-id="b423a-466">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="b423a-467">Por ejemplo, "1 año, mes".</span><span class="sxs-lookup"><span data-stu-id="b423a-467">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-468">Tipo de cargo</span><span class="sxs-lookup"><span data-stu-id="b423a-468">Charge Type</span></span></td>
<td><p><span data-ttu-id="b423a-469">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="b423a-469">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-470">Precio unitario</span><span class="sxs-lookup"><span data-stu-id="b423a-470">Unit Price</span></span></td>
<td><p><span data-ttu-id="b423a-471">El precio publicado en la lista de precios en el momento de la compra.</span><span class="sxs-lookup"><span data-stu-id="b423a-471">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b423a-472">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-472">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-473">Precio unitario efectivo</span><span class="sxs-lookup"><span data-stu-id="b423a-473">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="b423a-474">El precio por unidad una vez realizados los ajustes.</span><span class="sxs-lookup"><span data-stu-id="b423a-474">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-475">Cantidad</span><span class="sxs-lookup"><span data-stu-id="b423a-475">Quantity</span></span></td>
<td><p><span data-ttu-id="b423a-476">Número de unidades.</span><span class="sxs-lookup"><span data-stu-id="b423a-476">Number of units.</span></span> <span data-ttu-id="b423a-477">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-477">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-478">Tipo de unidad</span><span class="sxs-lookup"><span data-stu-id="b423a-478">Unit type</span></span></td>
<td><p><span data-ttu-id="b423a-479">El tipo de unidad que se compra.</span><span class="sxs-lookup"><span data-stu-id="b423a-479">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-480">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="b423a-480">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="b423a-481">Explicación de los descuentos aplicables.</span><span class="sxs-lookup"><span data-stu-id="b423a-481">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-482">Subtotal</span><span class="sxs-lookup"><span data-stu-id="b423a-482">Sub Total</span></span></td>
<td><p><span data-ttu-id="b423a-483">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="b423a-483">Total before tax.</span></span> <span data-ttu-id="b423a-484">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="b423a-484">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-485">Total de impuestos</span><span class="sxs-lookup"><span data-stu-id="b423a-485">Tax Total</span></span></td>
<td><p><span data-ttu-id="b423a-486">Cargo por importe de impuestos, en función de las reglas fiscales de tu mercado y las circunstancias específicas.</span><span class="sxs-lookup"><span data-stu-id="b423a-486">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-487">Total</span><span class="sxs-lookup"><span data-stu-id="b423a-487">Total</span></span></td>
<td><p><span data-ttu-id="b423a-488">Total con impuestos.</span><span class="sxs-lookup"><span data-stu-id="b423a-488">Total after tax.</span></span> <span data-ttu-id="b423a-489">Comprueba si se cobran impuestos en la factura.</span><span class="sxs-lookup"><span data-stu-id="b423a-489">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-490">Moneda</span><span class="sxs-lookup"><span data-stu-id="b423a-490">Currency</span></span></td>
<td><p><span data-ttu-id="b423a-491">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="b423a-491">Currency type.</span></span> <span data-ttu-id="b423a-492">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="b423a-492">Each billing entity has only one currency.</span></span> <span data-ttu-id="b423a-493">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="b423a-493">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-494">AlternateID</span><span class="sxs-lookup"><span data-stu-id="b423a-494">AlternateID</span></span></td>
<td><p><span data-ttu-id="b423a-495">Un identificador alternativo para un identificador de pedido.</span><span class="sxs-lookup"><span data-stu-id="b423a-495">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="b423a-496">Campos del archivo de uso diario calificados</span><span class="sxs-lookup"><span data-stu-id="b423a-496">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b423a-497">Column</span><span class="sxs-lookup"><span data-stu-id="b423a-497">Column</span></span></th>
<th><span data-ttu-id="b423a-498">Descripción</span><span class="sxs-lookup"><span data-stu-id="b423a-498">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="b423a-499">PartnerId</span><span class="sxs-lookup"><span data-stu-id="b423a-499">PartnerId</span></span></td>
<td><p><span data-ttu-id="b423a-500">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="b423a-500">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-501">PartnerName</span><span class="sxs-lookup"><span data-stu-id="b423a-501">PartnerName</span></span></td>
<td><p><span data-ttu-id="b423a-502">Nombre del partner.</span><span class="sxs-lookup"><span data-stu-id="b423a-502">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-503">CustomerId</span><span class="sxs-lookup"><span data-stu-id="b423a-503">CustomerId</span></span></td>
<td><p><span data-ttu-id="b423a-504">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="b423a-504">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-505">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="b423a-505">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="b423a-506">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="b423a-506">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="b423a-507">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="b423a-507">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-508">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="b423a-508">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="b423a-509">Nombre de dominio del cliente.</span><span class="sxs-lookup"><span data-stu-id="b423a-509">The customer’s domain name.</span></span> <span data-ttu-id="b423a-510">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="b423a-510">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-511">País del cliente</span><span class="sxs-lookup"><span data-stu-id="b423a-511">Customer country</span></span></td>
<td><p><span data-ttu-id="b423a-512">El país donde se encuentra el cliente.</span><span class="sxs-lookup"><span data-stu-id="b423a-512">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-513">MPNID</span><span class="sxs-lookup"><span data-stu-id="b423a-513">MPNID</span></span></td>
<td><p><span data-ttu-id="b423a-514">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="b423a-514">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-515">Distribuidor MPNID</span><span class="sxs-lookup"><span data-stu-id="b423a-515">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="b423a-516">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="b423a-516">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="b423a-517">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="b423a-517">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-518">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="b423a-518">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="b423a-519">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="b423a-519">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="b423a-520">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="b423a-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-521">ProductId</span><span class="sxs-lookup"><span data-stu-id="b423a-521">ProductId</span></span></td>
<td><p><span data-ttu-id="b423a-522">Identificador del producto.</span><span class="sxs-lookup"><span data-stu-id="b423a-522">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-523">SkuId</span><span class="sxs-lookup"><span data-stu-id="b423a-523">SkuId</span></span></td>
<td><p><span data-ttu-id="b423a-524">Id. de un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="b423a-524">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-525">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="b423a-525">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="b423a-526">Id. de una disponibilidad concreta.</span><span class="sxs-lookup"><span data-stu-id="b423a-526">The ID for a particular Availability.</span></span> <span data-ttu-id="b423a-527">"Disponibilidad" hace referencia a si un SKU concreto está o no disponible para su compra para el país, la moneda, el segmento industrial determinados, etc.</span><span class="sxs-lookup"><span data-stu-id="b423a-527">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-528">Nombre de SKU</span><span class="sxs-lookup"><span data-stu-id="b423a-528">SKU Name</span></span></td>
<td><p><span data-ttu-id="b423a-529">Título para un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="b423a-529">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-530">PublisherName</span><span class="sxs-lookup"><span data-stu-id="b423a-530">PublisherName</span></span></td>
<td><p><span data-ttu-id="b423a-531">El nombre del publicador.</span><span class="sxs-lookup"><span data-stu-id="b423a-531">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-532">PublisherID</span><span class="sxs-lookup"><span data-stu-id="b423a-532">PublisherID</span></span></td>
<td><p><span data-ttu-id="b423a-533">El identificador del publicador, en formato GUID.</span><span class="sxs-lookup"><span data-stu-id="b423a-533">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="b423a-534">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="b423a-534">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="b423a-535">Descripción de la suscripción</span><span class="sxs-lookup"><span data-stu-id="b423a-535">Subscription Description</span></span></td>
<td><p><span data-ttu-id="b423a-536">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="b423a-536">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="b423a-537">(Este es un campo idéntico al nombre de la oferta).</span><span class="sxs-lookup"><span data-stu-id="b423a-537">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-538">Id. de la suscripción</span><span class="sxs-lookup"><span data-stu-id="b423a-538">Subscription ID</span></span></td>
<td><p><span data-ttu-id="b423a-539">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="b423a-539">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="b423a-540">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-540">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="b423a-541">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="b423a-541">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-542">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="b423a-542">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="b423a-543">Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="b423a-543">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="b423a-544">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="b423a-544">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-545">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="b423a-545">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="b423a-546">Fecha de finalización del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="b423a-546">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="b423a-547">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="b423a-547">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-548">Fecha de uso</span><span class="sxs-lookup"><span data-stu-id="b423a-548">Usage Date</span></span></td>
<td><p><span data-ttu-id="b423a-549">Fecha de uso del servicio.</span><span class="sxs-lookup"><span data-stu-id="b423a-549">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-550">Tipo de medidor</span><span class="sxs-lookup"><span data-stu-id="b423a-550">Meter Type</span></span></td>
<td><p><span data-ttu-id="b423a-551">El tipo de medidor.</span><span class="sxs-lookup"><span data-stu-id="b423a-551">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-552">Categoría de medidor</span><span class="sxs-lookup"><span data-stu-id="b423a-552">Meter Category</span></span></td>
<td><p><span data-ttu-id="b423a-553">El servicio de nivel superior para el uso.</span><span class="sxs-lookup"><span data-stu-id="b423a-553">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-554">Id. de medidor</span><span class="sxs-lookup"><span data-stu-id="b423a-554">Meter Id</span></span></td>
<td><p><span data-ttu-id="b423a-555">El identificador del medidor que se va a usar.</span><span class="sxs-lookup"><span data-stu-id="b423a-555">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-556">Subcategoría de medidor</span><span class="sxs-lookup"><span data-stu-id="b423a-556">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="b423a-557">El tipo de servicio de Azure que puede afectar a la tarifa.</span><span class="sxs-lookup"><span data-stu-id="b423a-557">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-558">Nombre de medidor</span><span class="sxs-lookup"><span data-stu-id="b423a-558">Meter Name</span></span></td>
<td><p><span data-ttu-id="b423a-559">La unidad de medida del medidor consumido.</span><span class="sxs-lookup"><span data-stu-id="b423a-559">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-560">Región de medidor</span><span class="sxs-lookup"><span data-stu-id="b423a-560">Meter Region</span></span></td>
<td><p><span data-ttu-id="b423a-561">Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena.</span><span class="sxs-lookup"><span data-stu-id="b423a-561">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-562">Unidad</span><span class="sxs-lookup"><span data-stu-id="b423a-562">Unit</span></span></td>
<td><p><span data-ttu-id="b423a-563">La unidad del nombre de recurso.</span><span class="sxs-lookup"><span data-stu-id="b423a-563">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-564">Cantidad consumida</span><span class="sxs-lookup"><span data-stu-id="b423a-564">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="b423a-565">La cantidad de servicio consumida (horas, GB, etc.) durante el período de notificación.</span><span class="sxs-lookup"><span data-stu-id="b423a-565">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="b423a-566">También incluye cualquier uso no facturado de períodos anteriores.</span><span class="sxs-lookup"><span data-stu-id="b423a-566">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-567">Ubicación de recursos</span><span class="sxs-lookup"><span data-stu-id="b423a-567">Resource Location</span></span></td>
<td><p><span data-ttu-id="b423a-568">El centro de datos donde se está ejecutando el medidor.</span><span class="sxs-lookup"><span data-stu-id="b423a-568">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-569">Servicio consumido</span><span class="sxs-lookup"><span data-stu-id="b423a-569">Consumed Service</span></span></td>
<td><p><span data-ttu-id="b423a-570">El servicio de la plataforma Azure que usó.</span><span class="sxs-lookup"><span data-stu-id="b423a-570">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-571">Grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="b423a-571">Resource Group</span></span></td>
<td><p><span data-ttu-id="b423a-572">El grupo de recursos en el que se está ejecutando el medidor implementado.</span><span class="sxs-lookup"><span data-stu-id="b423a-572">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-573">URI de recurso</span><span class="sxs-lookup"><span data-stu-id="b423a-573">Resource URI</span></span></td>
<td><p><span data-ttu-id="b423a-574">El URI del recurso que se va a usar.</span><span class="sxs-lookup"><span data-stu-id="b423a-574">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-575">Tipo de cargo</span><span class="sxs-lookup"><span data-stu-id="b423a-575">Charge type</span></span></td>
<td><p><span data-ttu-id="b423a-576">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="b423a-576">The type of charge or adjustment.</span></span> <span data-ttu-id="b423a-577">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="b423a-577">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-578">Precio unitario</span><span class="sxs-lookup"><span data-stu-id="b423a-578">Unit price</span></span></td>
<td><p><span data-ttu-id="b423a-579">Precio por licencia, como se publica en la lista de precios en el momento de la compra.</span><span class="sxs-lookup"><span data-stu-id="b423a-579">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="b423a-580">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-580">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-581">Cantidad</span><span class="sxs-lookup"><span data-stu-id="b423a-581">Quantity</span></span></td>
<td><p><span data-ttu-id="b423a-582">Número de licencias.</span><span class="sxs-lookup"><span data-stu-id="b423a-582">Number of licenses.</span></span> <span data-ttu-id="b423a-583">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-584">Tipo de unidad</span><span class="sxs-lookup"><span data-stu-id="b423a-584">Unit type</span></span></td>
<td><p><span data-ttu-id="b423a-585">El tipo de unidad que se cobra el medidor.</span><span class="sxs-lookup"><span data-stu-id="b423a-585">The type of unit the meter is charged in.</span></span> <span data-ttu-id="b423a-586">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="b423a-586">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-587">Impuestos de facturación anterior a</span><span class="sxs-lookup"><span data-stu-id="b423a-587">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="b423a-588">Cantidad total antes de impuestos.</span><span class="sxs-lookup"><span data-stu-id="b423a-588">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-589">Divisa de facturación</span><span class="sxs-lookup"><span data-stu-id="b423a-589">Billing currency</span></span></td>
<td><p><span data-ttu-id="b423a-590">La moneda en la región geográfica del cliente</span><span class="sxs-lookup"><span data-stu-id="b423a-590">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-591">Precio total antes de impuestos</span><span class="sxs-lookup"><span data-stu-id="b423a-591">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="b423a-592">Los precios antes de que se agregan los impuestos.</span><span class="sxs-lookup"><span data-stu-id="b423a-592">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-593">Precios de moneda</span><span class="sxs-lookup"><span data-stu-id="b423a-593">Pricing currency</span></span></td>
<td><p><span data-ttu-id="b423a-594">La moneda en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="b423a-594">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-595">Información de servicio 1</span><span class="sxs-lookup"><span data-stu-id="b423a-595">Service Info 1</span></span></td>
<td><p><span data-ttu-id="b423a-596">Número de conexiones de Bus de servicio aprovisionadas y usadas en un día determinado.</span><span class="sxs-lookup"><span data-stu-id="b423a-596">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-597">Información de servicio 2</span><span class="sxs-lookup"><span data-stu-id="b423a-597">Service Info 2</span></span></td>
<td><p><span data-ttu-id="b423a-598">Un campo heredado que captura los metadatos específicos del servicio opcional.</span><span class="sxs-lookup"><span data-stu-id="b423a-598">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="b423a-599">Etiquetas</span><span class="sxs-lookup"><span data-stu-id="b423a-599">Tags</span></span></td>
<td><p><span data-ttu-id="b423a-600">Etiquetas que asigna al medidor en orden para agrupar los registros de facturación.</span><span class="sxs-lookup"><span data-stu-id="b423a-600">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="b423a-601">Por ejemplo, puede usar etiquetas para distribuir los costos por el departamento que utiliza el medidor.</span><span class="sxs-lookup"><span data-stu-id="b423a-601">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="b423a-602">Información adicional</span><span class="sxs-lookup"><span data-stu-id="b423a-602">Additional Info</span></span></td>
<td><p><span data-ttu-id="b423a-603">Cualquier información adicional que no se tratan en otras columnas.</span><span class="sxs-lookup"><span data-stu-id="b423a-603">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="b423a-604">Asignación de cargos entre una factura y el archivo de conciliación</span><span class="sxs-lookup"><span data-stu-id="b423a-604">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="b423a-605">La factura proporciona un resumen de los cargos, mientras que el archivo de conciliación proporciona un desglose detallado de las transacciones de elementos de línea, incluidos los tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="b423a-605">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="b423a-606">Para hacer referencias cruzadas de cantidades de cargos entre el archivo de conciliación y la factura, puedes usar las opciones de filtro de Microsoft Excel para filtrar por tipo de cargo en el archivo de conciliación con el fin de asignar los cargos de facturación a un conjunto de desgloses de cargos del archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-606">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="b423a-607">Los archivos de conciliación, tanto basados en uso como en licencias, solo muestran cargos y transacciones relacionados con el uso (unidades consumidas y cargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="b423a-607">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="b423a-608">En el archivo de conciliación no aparecen devoluciones, descuentos o créditos excepcionales que aparecen en la factura como "Ajustes".</span><span class="sxs-lookup"><span data-stu-id="b423a-608">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="b423a-609">La siguiente tabla muestra las asignaciones entre una sección de factura y los tipos de cargo asociados que es posible que se muestren en los archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="b423a-609">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><strong><span data-ttu-id="b423a-610">Descripción del cargo de facturación</span><span class="sxs-lookup"><span data-stu-id="b423a-610">Invoice charge description</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="b423a-611">Descripción del cargo del archivo de conciliación (columna ChargeType)</span><span class="sxs-lookup"><span data-stu-id="b423a-611">Reconciliation file charge description (ChargeType column)</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="b423a-612">¿Qué es este cargo?</span><span class="sxs-lookup"><span data-stu-id="b423a-612">What is this charge?</span></span></strong></p>
</td>
<td>
<p><strong><span data-ttu-id="b423a-613">¿Cómo asigno estos valores de ChargeType a la factura?</span><span class="sxs-lookup"><span data-stu-id="b423a-613">How do I map these ChargeTypes to the invoice?</span></span></strong></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><strong><span data-ttu-id="b423a-614">Cargos basados en licencias</span><span class="sxs-lookup"><span data-stu-id="b423a-614">License-based charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b423a-615">Tarifa de activación</span><span class="sxs-lookup"><span data-stu-id="b423a-615">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-616">El importe cobrado al cliente cuando usa la suscripción después de adquirirla</span><span class="sxs-lookup"><span data-stu-id="b423a-616">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="b423a-617">Desde el archivo basado en licencia, suma la columna <strong>Amount</strong>.</span><span class="sxs-lookup"><span data-stu-id="b423a-617">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b423a-618">Cuota de cancelación</span><span class="sxs-lookup"><span data-stu-id="b423a-618">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-619">Cargos prorrateados reembolsados al cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="b423a-619">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b423a-620">Tarifa de ciclo</span><span class="sxs-lookup"><span data-stu-id="b423a-620">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-621">Cargos periódicos de una suscripción</span><span class="sxs-lookup"><span data-stu-id="b423a-621">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b423a-622">Prorrateo de instancia de ciclo</span><span class="sxs-lookup"><span data-stu-id="b423a-622">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-623">Cargos prorrateados evaluados del cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="b423a-623">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b423a-624">Tarifas prorrateadas al cancelar</span><span class="sxs-lookup"><span data-stu-id="b423a-624">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-625">Reembolso prorrateado de la parte no usada del servicio tras la cancelación</span><span class="sxs-lookup"><span data-stu-id="b423a-625">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b423a-626">Tarifas prorrateadas al comprar</span><span class="sxs-lookup"><span data-stu-id="b423a-626">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-627">El tipo de gasto para una suscripción cuando se usa la facturación anual</span><span class="sxs-lookup"><span data-stu-id="b423a-627">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b423a-628">Tarifa de compra</span><span class="sxs-lookup"><span data-stu-id="b423a-628">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-629">El tipo de gasto para una suscripción cuando se usa la facturación mensual</span><span class="sxs-lookup"><span data-stu-id="b423a-629">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b423a-630">Tarifa prorrateada al renovar</span><span class="sxs-lookup"><span data-stu-id="b423a-630">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-631">Tarifas prorrateadas tras la renovación de la suscripción</span><span class="sxs-lookup"><span data-stu-id="b423a-631">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="b423a-632">Tarifa de renovación</span><span class="sxs-lookup"><span data-stu-id="b423a-632">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-633">Cargo por renovar una suscripción</span><span class="sxs-lookup"><span data-stu-id="b423a-633">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b423a-634">Tarifas prorrateadas al activar</span><span class="sxs-lookup"><span data-stu-id="b423a-634">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-635">Tarifas prorrateadas desde la activación hasta el final del período de facturación</span><span class="sxs-lookup"><span data-stu-id="b423a-635">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>
<tr>
<td rowspan="2">
<p><strong><span data-ttu-id="b423a-636">Cargos de uso</span><span class="sxs-lookup"><span data-stu-id="b423a-636">Usage Charges</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b423a-637">Evaluar la tarifa de uso al cancelar</span><span class="sxs-lookup"><span data-stu-id="b423a-637">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-638">Tarifa de uso de acceso tras la cancelación por uso impagado durante el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="b423a-638">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="b423a-639">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="b423a-639">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b423a-640">Evaluar la tarifa de uso para el ciclo actual</span><span class="sxs-lookup"><span data-stu-id="b423a-640">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-641">tarifa de uso de acceso para el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="b423a-641">Access usage fee for the current billing period</span></span></p>
</td>
</tr>
<tr>
<td>
<p><strong><span data-ttu-id="b423a-642">Créditos</span><span class="sxs-lookup"><span data-stu-id="b423a-642">Credits</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b423a-643">Desplazamiento de un elemento de línea</span><span class="sxs-lookup"><span data-stu-id="b423a-643">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-644">Reembolso parcial o total de un elemento de línea, incluidos impuestos</span><span class="sxs-lookup"><span data-stu-id="b423a-644">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-645">Desde el archivo basado en licencia, suma la columna <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="b423a-645">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="b423a-646">Desde el archivo basado en uso, suma la columna <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="b423a-646">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><strong><span data-ttu-id="b423a-647">Descuentos basados en uso</span><span class="sxs-lookup"><span data-stu-id="b423a-647">Usage-based discounts</span></span></strong></p>
</td>
<td>
<p><span data-ttu-id="b423a-648">Descuento de activación</span><span class="sxs-lookup"><span data-stu-id="b423a-648">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-649">Descuento que se aplica cuando se activa la suscripción</span><span class="sxs-lookup"><span data-stu-id="b423a-649">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="b423a-650">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="b423a-650">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b423a-651">Descuento de ciclo</span><span class="sxs-lookup"><span data-stu-id="b423a-651">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-652">Descuento que se aplica en cargos periódicos</span><span class="sxs-lookup"><span data-stu-id="b423a-652">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b423a-653">Descuento de renovación</span><span class="sxs-lookup"><span data-stu-id="b423a-653">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-654">Descuento que se aplica cuando se renueva la suscripción</span><span class="sxs-lookup"><span data-stu-id="b423a-654">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b423a-655">Descuento de cancelación</span><span class="sxs-lookup"><span data-stu-id="b423a-655">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-656">Cargos que se aplican cuando se cancelan los descuentos</span><span class="sxs-lookup"><span data-stu-id="b423a-656">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><strong><span data-ttu-id="b423a-657">Descuentos basados en licencias</span><span class="sxs-lookup"><span data-stu-id="b423a-657">License-based discounts</span></span></strong></p>
</td>
<td>
<p><em><span data-ttu-id="b423a-658">Se pueden aplicar a varios tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="b423a-658">May be applied to multiple charge types</span></span></em></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="b423a-659">Desde el archivo basado en licencia, suma la columna <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="b423a-659">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="b423a-660"><strong>Impuestos</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="b423a-660"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><em><span data-ttu-id="b423a-661">Se pueden aplicar a varios tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="b423a-661">May be applied to multiple charge types</span></span></em></p>
<p><em><span data-ttu-id="b423a-662">Excepción: &quot;Desplazamiento de un elemento de línea&quot; ya incluye los impuestos.</span><span class="sxs-lookup"><span data-stu-id="b423a-662">Exception: &quot;Offset a line item&quot; already includes taxes.</span></span> <span data-ttu-id="b423a-663">Consulta Créditos más arriba.</span><span class="sxs-lookup"><span data-stu-id="b423a-663">See Credits, above.</span></span></em></p>
</td>
<td>
<p><span data-ttu-id="b423a-664">Impuestos o impuesto de valor añadido (IVA)</span><span class="sxs-lookup"><span data-stu-id="b423a-664">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="b423a-665">Desde el archivo basado en licencia, suma la columna <strong>Tax</strong>.</span><span class="sxs-lookup"><span data-stu-id="b423a-665">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="b423a-666">Desde el archivo basado en uso, suma la columna <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="b423a-666">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
