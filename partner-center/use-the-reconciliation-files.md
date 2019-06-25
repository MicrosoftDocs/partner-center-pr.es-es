---
title: Usar los archivos de conciliación | Centro de partners
ms.topic: article
ms.date: 03/15/2019
description: Para obtener una vista detallada del elemento de línea de cada carga de un ciclo de facturación, descargue los archivos de conciliación de centro de partners.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: fca9897720412a77ac39c86ba31db411c58c2cb0
ms.sourcegitcommit: 1f9078d422af5f8514d79a6ab9c3444500abfe27
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/24/2019
ms.locfileid: "67343469"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="61357-103">Usar los archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="61357-103">Use the reconciliation files</span></span>

<span data-ttu-id="61357-104">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="61357-104">**Applies to**</span></span>

-  <span data-ttu-id="61357-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="61357-105">Partner Center</span></span>
-  <span data-ttu-id="61357-106">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="61357-106">Partner Center for Microsoft Cloud for US Government</span></span>


<span data-ttu-id="61357-107">Para obtener una vista detallada del elemento de línea de cada carga de un ciclo de facturación, descargue los archivos de conciliación de centro de partners.</span><span class="sxs-lookup"><span data-stu-id="61357-107">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="61357-108">Los detalles incluyen los cargos para las suscripciones de cada cliente y los eventos detallados (por ejemplo, una adición intermedia de puestos en una suscripción).</span><span class="sxs-lookup"><span data-stu-id="61357-108">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="61357-109">Problemas de formato</span><span class="sxs-lookup"><span data-stu-id="61357-109">Formatting issues</span></span>

<span data-ttu-id="61357-110">En ocasiones, el archivo de conciliación podría tener problemas de formato.</span><span class="sxs-lookup"><span data-stu-id="61357-110">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="61357-111">(Esto puede ocurrir, por ejemplo, si no se usa la configuración regional EN-US). Siga estos pasos para corregir estos problemas.</span><span class="sxs-lookup"><span data-stu-id="61357-111">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="61357-112">Abra el archivo .csv en Excel y seleccione la primera columna.</span><span class="sxs-lookup"><span data-stu-id="61357-112">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="61357-113">En la cinta de opciones, seleccione <strong>datos</strong>y, a continuación, seleccione <strong>texto en columnas</strong>.</span><span class="sxs-lookup"><span data-stu-id="61357-113">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="61357-114">En convertir texto en el Asistente de columnas, seleccione <strong>delimitado por tipo de archivo</strong>y, a continuación, seleccione <strong>siguiente</strong>.</span><span class="sxs-lookup"><span data-stu-id="61357-114">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="61357-115">En el campo delimitadores, seleccione <strong>comas</strong>.</span><span class="sxs-lookup"><span data-stu-id="61357-115">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="61357-116">Si <strong>ficha</strong> está ya seleccionado, puede dejarla.</span><span class="sxs-lookup"><span data-stu-id="61357-116">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="61357-117">Selecciona <strong>Siguiente</strong>.</span><span class="sxs-lookup"><span data-stu-id="61357-117">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="61357-118">En el campo de formato de datos de columna, seleccione <strong>fecha: MDY</strong>y, a continuación, seleccione <strong>siguiente</strong>.</span><span class="sxs-lookup"><span data-stu-id="61357-118">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="61357-119">En el campo de formato de datos de columna, seleccione <strong>texto</strong> para amount, todas las columnas y, a continuación, seleccione <strong>finalizar</strong>.</span><span class="sxs-lookup"><span data-stu-id="61357-119">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="61357-120">Descargar un archivo de conciliación grande</span><span class="sxs-lookup"><span data-stu-id="61357-120">Downloading a large recon file</span></span>

<span data-ttu-id="61357-121">Archivos de conciliación pueden crecer muy grandes y a veces son difíciles de descargar.</span><span class="sxs-lookup"><span data-stu-id="61357-121">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="61357-122">Para que un script de PowerShell ayudar a descargar los archivos de conciliación grandes, consulte [Get factura partidas presupuestarias](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="61357-122">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/en-us/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="61357-123">Detallar asociado</span><span class="sxs-lookup"><span data-stu-id="61357-123">Itemize by partner</span></span>


<span data-ttu-id="61357-124">Los partners del modelo indirecto pueden usar estos campos adicionales en ambos archivos de conciliación basada en uso y en licencia para realizar el desglose por revendedor.</span><span class="sxs-lookup"><span data-stu-id="61357-124">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="61357-125">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="61357-125">MPN ID</span></span></th>
<th><span data-ttu-id="61357-126">Descripción</span><span class="sxs-lookup"><span data-stu-id="61357-126">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="61357-127">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="61357-127">MPN ID</span></span></td>
<td><p><span data-ttu-id="61357-128">Id. de Microsoft Partner Network (MPN) del partner de CSP (directo o indirecto).</span><span class="sxs-lookup"><span data-stu-id="61357-128">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-129">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="61357-129">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="61357-130">Solo aparece en los archivos de conciliación de partners en el modelo indirecto.</span><span class="sxs-lookup"><span data-stu-id="61357-130">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="61357-131">El Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="61357-131">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="61357-132">Corresponde al id. de revendedor indicado para la suscripción específica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="61357-132">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="61357-133">muestra de eTo o actualiza el distribuidor, en el menú del centro de partners, seleccione <strong>clientes</strong>, a continuación, elija el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="61357-133">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="61357-134">En el menú del cliente, selecciona <strong>Suscripciones</strong> y elige la suscripción de la lista.</span><span class="sxs-lookup"><span data-stu-id="61357-134">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="61357-135">Selecciona <strong>Actualizar</strong> para cambiar el valor de <strong>Revendedor (id. de MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="61357-135">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="61357-136">Si un partner CSP vendió la suscripción directamente al cliente, su id. de MPN aparece dos veces, como id. de MPN y como id. de MPN del revendedor.</span><span class="sxs-lookup"><span data-stu-id="61357-136">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="61357-137">Si un partner CSP tiene un revendedor sin un id. de MPN, este valor se establece en el id. de MPN del partner.</span><span class="sxs-lookup"><span data-stu-id="61357-137">If a CSP partner has a reseller with no MPN ID, this value is set to the partner’s MPN ID instead.</span></span></p>
<p><span data-ttu-id="61357-138">Si el partner CSP quita un id. de revendedor, este valor se establece en -1.</span><span class="sxs-lookup"><span data-stu-id="61357-138">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a> <span data-ttu-id="61357-139">Campos de archivo de licencia</span><span class="sxs-lookup"><span data-stu-id="61357-139">License-based file fields</span></span>


<span data-ttu-id="61357-140">Para conciliar los cargos en función de los pedidos del cliente, compara el Syndication\_Partner\_Subscription\_Number del archivo de conciliación con el id. de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="61357-140">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="61357-141"><strong>Columna</strong></span><span class="sxs-lookup"><span data-stu-id="61357-141"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="61357-142"><strong>Descripción</strong></span><span class="sxs-lookup"><span data-stu-id="61357-142"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="61357-143"><strong>Valor de ejemplo</strong></span><span class="sxs-lookup"><span data-stu-id="61357-143"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-144">PartnerId</span><span class="sxs-lookup"><span data-stu-id="61357-144">PartnerId</span></span></td>
<td><p><span data-ttu-id="61357-145">Identificador único de una entidad de facturación específica, con formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="61357-145">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="61357-146">No es necesario para la reconciliación, pero puede ser información útil.</span><span class="sxs-lookup"><span data-stu-id="61357-146">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="61357-147">Igual en todas las filas.</span><span class="sxs-lookup"><span data-stu-id="61357-147">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="61357-148">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="61357-148">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-149">CustomerID</span><span class="sxs-lookup"><span data-stu-id="61357-149">CustomerID</span></span></td>
<td><p><span data-ttu-id="61357-150">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="61357-150">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="61357-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="61357-151">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-152">OrderID</span><span class="sxs-lookup"><span data-stu-id="61357-152">OrderID</span></span></td>
<td><p><span data-ttu-id="61357-153">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="61357-153">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="61357-154">Puede ser útil para identificar al pedido al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-154">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="61357-155">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="61357-155">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-156">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="61357-156">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="61357-157">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="61357-157">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="61357-158">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-158">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="61357-159">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="61357-159">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="61357-160">Consulte Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="61357-160">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="61357-161">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="61357-161">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-162">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="61357-162">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="61357-163">Identificador único de las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="61357-163">Unique identifier for subscriptions.</span></span> <span data-ttu-id="61357-164">Un cliente puede tener varias suscripciones para el mismo plan, por lo que es importante para el análisis de archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-164">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="61357-165">Este campo se asigna al identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="61357-165">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="61357-166">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="61357-166">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-167">OfferID</span><span class="sxs-lookup"><span data-stu-id="61357-167">OfferID</span></span></td>
<td><p><span data-ttu-id="61357-168">Identificador único de la oferta.</span><span class="sxs-lookup"><span data-stu-id="61357-168">Unique offer ID.</span></span> <span data-ttu-id="61357-169">Identificador de la oferta estándar según la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="61357-169">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="61357-170"><b>Nota</b>: Este valor no coincide con Id. de oferta desde la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="61357-170"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="61357-171">Consulta DurableOfferID a continuación.</span><span class="sxs-lookup"><span data-stu-id="61357-171">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="61357-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="61357-172">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-173">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="61357-173">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="61357-174">Identificador único de oferta duradera, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="61357-174">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="61357-175"><b>Nota</b>: Este valor coincide con el Id. de oferta desde la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="61357-175"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="61357-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="61357-176">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-177">OfferName</span><span class="sxs-lookup"><span data-stu-id="61357-177">OfferName</span></span></td>
<td><p><span data-ttu-id="61357-178">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="61357-178">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="61357-179">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="61357-179">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-180">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="61357-180">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="61357-181">Fecha de finalización de la suscripción, establecida en el día posterior al envío del pedido.</span><span class="sxs-lookup"><span data-stu-id="61357-181">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="61357-182">Al consultar la fecha de inicio de la suscripción junto con la fecha de finalización, puedes determinar si el cliente aún está dentro del primer año de la suscripción o si la suscripción se ha renovado para el año siguiente.</span><span class="sxs-lookup"><span data-stu-id="61357-182">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="61357-183">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="61357-183">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="61357-184">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="61357-184">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-185">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="61357-185">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="61357-186">La fecha de finalización de la suscripción: 12 meses + x días después de la fecha de inicio (para alinearse con fecha de facturación del asociado) o 12 meses a partir de la fecha de renovación.</span><span class="sxs-lookup"><span data-stu-id="61357-186">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="61357-187">En el momento de la renovación, los precios se actualizan según la lista de precios actual.</span><span class="sxs-lookup"><span data-stu-id="61357-187">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="61357-188">Es posible que se necesite una comunicación con el cliente antes de la renovación automatizada.</span><span class="sxs-lookup"><span data-stu-id="61357-188">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="61357-189">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="61357-189">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="61357-190">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="61357-190">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-191">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="61357-191">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="61357-192">Día de inicio de los cargos.</span><span class="sxs-lookup"><span data-stu-id="61357-192">Start day of the charges.</span></span></p>
<p><span data-ttu-id="61357-193">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="61357-193">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="61357-194">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="61357-194">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="61357-195">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="61357-195">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-196">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="61357-196">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="61357-197">Día de finalización de los cargos.</span><span class="sxs-lookup"><span data-stu-id="61357-197">End day of the charges.</span></span></p>
<p><span data-ttu-id="61357-198">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="61357-198">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="61357-199">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="61357-199">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="61357-200">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="61357-200">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-201">ChargeType</span><span class="sxs-lookup"><span data-stu-id="61357-201">ChargeType</span></span></td>
<td><p><span data-ttu-id="61357-202">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="61357-202">The type of charge or adjustment.</span></span> <span data-ttu-id="61357-203">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="61357-203">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="61357-204">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="61357-204">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-205">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="61357-205">UnitPrice</span></span></td>
<td><p><span data-ttu-id="61357-206">Precio por puesto, tal y como se publica en la lista de precios en el momento de compra.</span><span class="sxs-lookup"><span data-stu-id="61357-206">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="61357-207">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-207">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="61357-208">6.82</span><span class="sxs-lookup"><span data-stu-id="61357-208">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-209">Cantidad</span><span class="sxs-lookup"><span data-stu-id="61357-209">Quantity</span></span></td>
<td><p><span data-ttu-id="61357-210">Número de puestos.</span><span class="sxs-lookup"><span data-stu-id="61357-210">Number of seats.</span></span> <span data-ttu-id="61357-211">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-211">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="61357-212">2</span><span class="sxs-lookup"><span data-stu-id="61357-212">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-213">Volumen</span><span class="sxs-lookup"><span data-stu-id="61357-213">Amount</span></span></td>
<td><p><span data-ttu-id="61357-214">Total del precio para la cantidad.</span><span class="sxs-lookup"><span data-stu-id="61357-214">Total of price for quantity.</span></span> <span data-ttu-id="61357-215">Es de utilidad para comprobar que el cálculo de la cantidad coincide con la manera de calcular este valor para los clientes.</span><span class="sxs-lookup"><span data-stu-id="61357-215">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="61357-216">13.32</span><span class="sxs-lookup"><span data-stu-id="61357-216">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-217">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="61357-217">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="61357-218">Cantidad de descuento que se aplica a estos cargos.</span><span class="sxs-lookup"><span data-stu-id="61357-218">Amount of discount applied to these charges.</span></span> <span data-ttu-id="61357-219">Los IUR o las nuevas suscripciones que puedan optar a un incentivo también incluirán un importe de descuento en esta columna.</span><span class="sxs-lookup"><span data-stu-id="61357-219">IUR or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="61357-220">2.32</span><span class="sxs-lookup"><span data-stu-id="61357-220">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-221">Subtotal</span><span class="sxs-lookup"><span data-stu-id="61357-221">Subtotal</span></span></td>
<td><p><span data-ttu-id="61357-222">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="61357-222">Total before tax.</span></span> <span data-ttu-id="61357-223">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="61357-223">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="61357-224">11</span><span class="sxs-lookup"><span data-stu-id="61357-224">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-225">Impuestos</span><span class="sxs-lookup"><span data-stu-id="61357-225">Tax</span></span></td>
<td><p><span data-ttu-id="61357-226">Importe de impuestos, según el mercado&#39;reglas s y circunstancias concretas.</span><span class="sxs-lookup"><span data-stu-id="61357-226">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="61357-227">0</span><span class="sxs-lookup"><span data-stu-id="61357-227">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-228">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="61357-228">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="61357-229">Total con impuestos.</span><span class="sxs-lookup"><span data-stu-id="61357-229">Total after tax.</span></span> <span data-ttu-id="61357-230">Comprueba si se cobran impuestos en la factura.</span><span class="sxs-lookup"><span data-stu-id="61357-230">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="61357-231">11</span><span class="sxs-lookup"><span data-stu-id="61357-231">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-232">Currency</span><span class="sxs-lookup"><span data-stu-id="61357-232">Currency</span></span></td>
<td><p><span data-ttu-id="61357-233">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="61357-233">Currency type.</span></span> <span data-ttu-id="61357-234">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="61357-234">Each billing entity has only one currency.</span></span> <span data-ttu-id="61357-235">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="61357-235">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="61357-236">EUR</span><span class="sxs-lookup"><span data-stu-id="61357-236">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-237">CustomerName</span><span class="sxs-lookup"><span data-stu-id="61357-237">CustomerName</span></span></td>
<td><p><span data-ttu-id="61357-238">Cliente&#39;nombre de la organización s notificados en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="61357-238">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="61357-239">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="61357-239">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="61357-240">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="61357-240">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-241">MPNID</span><span class="sxs-lookup"><span data-stu-id="61357-241">MPNID</span></span></td>
<td><p><span data-ttu-id="61357-242">Id. de MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="61357-242">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="61357-243">4390934</span><span class="sxs-lookup"><span data-stu-id="61357-243">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-244">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="61357-244">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="61357-245">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="61357-245">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="61357-246">Ver <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Desglosar por partner</a></span><span class="sxs-lookup"><span data-stu-id="61357-246">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="61357-247">4390934</span><span class="sxs-lookup"><span data-stu-id="61357-247">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-248">DomainName</span><span class="sxs-lookup"><span data-stu-id="61357-248">DomainName</span></span></td>
<td><p><span data-ttu-id="61357-249">Cliente&#39;nombre de dominio de s, que ayuda a identificar el cliente.</span><span class="sxs-lookup"><span data-stu-id="61357-249">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="61357-250">No debe usarse para identificar al cliente como el cliente o socio puede actualizar el dominio personal de forma predeterminada a través del portal de Office 365.</span><span class="sxs-lookup"><span data-stu-id="61357-250">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="61357-251">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="61357-251">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="61357-252">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="61357-252">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-253">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="61357-253">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="61357-254">Alias de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="61357-254">Subscription nickname.</span></span> <span data-ttu-id="61357-255">Si no se especifica ningún alias, el Centro de partners usa OfferName.</span><span class="sxs-lookup"><span data-stu-id="61357-255">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="61357-256">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="61357-256">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-257">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="61357-257">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="61357-258">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="61357-258">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="61357-259">(Este es un campo idéntico al nombre de la oferta).</span><span class="sxs-lookup"><span data-stu-id="61357-259">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="61357-260">PROJECT ONLINE PREMIUM SIN CLIENTE DE PROJECT</span><span class="sxs-lookup"><span data-stu-id="61357-260">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="61357-261">Campos de archivo basada en uso</span><span class="sxs-lookup"><span data-stu-id="61357-261">Usage-based file fields</span></span>


<span data-ttu-id="61357-262">Para conciliar los cargos en función del uso de tu cliente, compara los valores de ResellerID/ResellerName/ResellerBillableAccount del archivo de conciliación, el nombre del cliente y el id. de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="61357-262">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="61357-263">Los siguientes campos explican los servicios usados y la clasificación.</span><span class="sxs-lookup"><span data-stu-id="61357-263">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="61357-264"><strong>Columna</strong></span><span class="sxs-lookup"><span data-stu-id="61357-264"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="61357-265"><strong>Descripción</strong></span><span class="sxs-lookup"><span data-stu-id="61357-265"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="61357-266"><strong>Valor de ejemplo</strong></span><span class="sxs-lookup"><span data-stu-id="61357-266"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-267">PartnerID</span><span class="sxs-lookup"><span data-stu-id="61357-267">PartnerID</span></span></td>
<td><p><span data-ttu-id="61357-268">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="61357-268">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="61357-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="61357-269">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-270">PartnerName</span><span class="sxs-lookup"><span data-stu-id="61357-270">PartnerName</span></span></td>
<td><p><span data-ttu-id="61357-271">Nombre del partner.</span><span class="sxs-lookup"><span data-stu-id="61357-271">Partner Name.</span></span></p></td>
<td><span data-ttu-id="61357-272">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="61357-272">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-273">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="61357-273">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="61357-274">Id. de cuenta del partner.</span><span class="sxs-lookup"><span data-stu-id="61357-274">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="61357-275">1010578050</span><span class="sxs-lookup"><span data-stu-id="61357-275">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-276">CustomerName</span><span class="sxs-lookup"><span data-stu-id="61357-276">CustomerName</span></span></td>
<td><p><span data-ttu-id="61357-277">Cliente&#39;nombre de la organización s notificados en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="61357-277">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="61357-278">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="61357-278">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="61357-279">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="61357-279">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-280">MPNID</span><span class="sxs-lookup"><span data-stu-id="61357-280">MPNID</span></span></td>
<td><p><span data-ttu-id="61357-281">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="61357-281">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="61357-282">4390934</span><span class="sxs-lookup"><span data-stu-id="61357-282">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-283">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="61357-283">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="61357-284">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="61357-284">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="61357-285">Ver <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Desglosar por partner</a></span><span class="sxs-lookup"><span data-stu-id="61357-285">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="61357-286">4390934</span><span class="sxs-lookup"><span data-stu-id="61357-286">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-287">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="61357-287">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="61357-288">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="61357-288">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="61357-289">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="61357-289">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-290">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="61357-290">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="61357-291">Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="61357-291">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="61357-292">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="61357-292">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="61357-293">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="61357-293">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-294">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="61357-294">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="61357-295">Fecha de finalización del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="61357-295">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="61357-296">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="61357-296">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="61357-297">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="61357-297">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-298">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="61357-298">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="61357-299">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="61357-299">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="61357-300">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-300">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="61357-301">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="61357-301">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="61357-302">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="61357-302">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-303">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="61357-303">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="61357-304">Alias de la oferta de servicio.</span><span class="sxs-lookup"><span data-stu-id="61357-304">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="61357-305">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="61357-305">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-306">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="61357-306">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="61357-307">Línea de negocio de la oferta de servicio</span><span class="sxs-lookup"><span data-stu-id="61357-307">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="61357-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="61357-308">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-309">OrderID</span><span class="sxs-lookup"><span data-stu-id="61357-309">OrderID</span></span></td>
<td><p><span data-ttu-id="61357-310">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="61357-310">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="61357-311">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-311">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="61357-312">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="61357-312">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-313">ServiceName</span><span class="sxs-lookup"><span data-stu-id="61357-313">ServiceName</span></span></td>
<td><p><span data-ttu-id="61357-314">Nombre del servicio de Azure en cuestión.</span><span class="sxs-lookup"><span data-stu-id="61357-314">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="61357-315">MÁQUINAS VIRTUALES</span><span class="sxs-lookup"><span data-stu-id="61357-315">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-316">ServiceType</span><span class="sxs-lookup"><span data-stu-id="61357-316">ServiceType</span></span></td>
<td><p><span data-ttu-id="61357-317">Tipo específico de servicio de Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="61357-317">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="61357-318">Bus de servicio: individual o paquete</span><span class="sxs-lookup"><span data-stu-id="61357-318">Service Bus – Individual or Pack</span></span></li>
<li><span data-ttu-id="61357-319">Base de datos SQL Azure: edición Business o Web</span><span class="sxs-lookup"><span data-stu-id="61357-319">SQL Azure database – Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-320">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="61357-320">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="61357-321">Identificador único específico para toda la estructura de precios y datos del servicio.</span><span class="sxs-lookup"><span data-stu-id="61357-321">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="61357-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="61357-322">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-323">Nombre de recurso</span><span class="sxs-lookup"><span data-stu-id="61357-323">Resource Name</span></span></td>
<td><p><span data-ttu-id="61357-324">Nombre del recurso de Azure.</span><span class="sxs-lookup"><span data-stu-id="61357-324">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="61357-325">Transferencia entrante de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="61357-325">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="61357-326">Transferencia saliente de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="61357-326">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-327">Region</span><span class="sxs-lookup"><span data-stu-id="61357-327">Region</span></span></td>
<td><p><span data-ttu-id="61357-328">La región a la que se aplica el uso.</span><span class="sxs-lookup"><span data-stu-id="61357-328">The region the usage applies to.</span></span> <span data-ttu-id="61357-329">Se usa principalmente para asignar tarifas a las transferencias de datos, ya que las tarifas varían según la región.</span><span class="sxs-lookup"><span data-stu-id="61357-329">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="61357-330">Asia Pacífico, Europa, América Latina, América del Norte</span><span class="sxs-lookup"><span data-stu-id="61357-330">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-331">SKU</span><span class="sxs-lookup"><span data-stu-id="61357-331">SKU</span></span></td>
<td><p><span data-ttu-id="61357-332">Identificador único de MSFT para la oferta</span><span class="sxs-lookup"><span data-stu-id="61357-332">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="61357-333">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="61357-333">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="61357-334">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="61357-334">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="61357-335">Un id. y una cantidad para desglosar las distintas clasificaciones de un servicio o un recurso en un período de facturación determinado.</span><span class="sxs-lookup"><span data-stu-id="61357-335">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="61357-336">Para clasificación en niveles de Azure, puede haber una clasificación hasta una cantidad determinada de unidades facturables y, posteriormente, una clasificación diferente.</span><span class="sxs-lookup"><span data-stu-id="61357-336">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="61357-337">1</span><span class="sxs-lookup"><span data-stu-id="61357-337">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-338">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="61357-338">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="61357-339">La cantidad de servicio consumida (horas, GB, etc.) durante el período de notificación.</span><span class="sxs-lookup"><span data-stu-id="61357-339">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="61357-340">También incluye cualquier uso no facturado de períodos anteriores.</span><span class="sxs-lookup"><span data-stu-id="61357-340">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="61357-341">11</span><span class="sxs-lookup"><span data-stu-id="61357-341">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-342">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="61357-342">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="61357-343">Unidades que se incluyen como parte de la oferta.</span><span class="sxs-lookup"><span data-stu-id="61357-343">Units included as part of the offer.</span></span> <span data-ttu-id="61357-344">No suele mostrarse en CSP.</span><span class="sxs-lookup"><span data-stu-id="61357-344">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="61357-345">0</span><span class="sxs-lookup"><span data-stu-id="61357-345">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="61357-346">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="61357-346">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="61357-347">Unidades que no se incluyen como parte de la oferta y que el partner debe abonar.</span><span class="sxs-lookup"><span data-stu-id="61357-347">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="61357-348">Equivale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="61357-348">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="61357-349">11</span><span class="sxs-lookup"><span data-stu-id="61357-349">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-350">ListPrice</span><span class="sxs-lookup"><span data-stu-id="61357-350">ListPrice</span></span></td>
<td><p><span data-ttu-id="61357-351">Precio de la oferta en vigor la fecha de inicio de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="61357-351">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="61357-352">0\.0808 USD</span><span class="sxs-lookup"><span data-stu-id="61357-352">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-353">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="61357-353">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="61357-354">ListPrist x OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="61357-354">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="61357-355">0\.085 USD</span><span class="sxs-lookup"><span data-stu-id="61357-355">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-356">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="61357-356">TaxAmount</span></span></td>
<td><p><span data-ttu-id="61357-357">Importe de impuestos, según el mercado&#39;reglas s y circunstancias concretas.</span><span class="sxs-lookup"><span data-stu-id="61357-357">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="61357-358">0\.08 USD</span><span class="sxs-lookup"><span data-stu-id="61357-358">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-359">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="61357-359">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="61357-360">Total con impuestos, si se aplican impuestos.</span><span class="sxs-lookup"><span data-stu-id="61357-360">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="61357-361">0\.93 USD</span><span class="sxs-lookup"><span data-stu-id="61357-361">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-362">Currency</span><span class="sxs-lookup"><span data-stu-id="61357-362">Currency</span></span></td>
<td><p><span data-ttu-id="61357-363">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="61357-363">Currency type.</span></span> <span data-ttu-id="61357-364">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="61357-364">Each billing entity has only one currency.</span></span> <span data-ttu-id="61357-365">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="61357-365">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="61357-366">EUR</span><span class="sxs-lookup"><span data-stu-id="61357-366">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-367">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="61357-367">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="61357-368">Precio sin impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="61357-368">Pretax price per unit.</span></span> <span data-ttu-id="61357-369">Igual que PretaxCharges/OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="61357-369">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="61357-370">0\.08 USD</span><span class="sxs-lookup"><span data-stu-id="61357-370">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-371">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="61357-371">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="61357-372">Precio después de impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="61357-372">Post tax price per unit.</span></span> <span data-ttu-id="61357-373">Igual que PostTaxTotal/OverageQuantity o PretaxEffectiveRate + tipo impositivo por importe unitario, redondeado el céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="61357-373">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="61357-374">0\.08 USD</span><span class="sxs-lookup"><span data-stu-id="61357-374">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-375">ChargeType</span><span class="sxs-lookup"><span data-stu-id="61357-375">ChargeType</span></span></td>
<td><p><span data-ttu-id="61357-376">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="61357-376">The type of charge or adjustment.</span></span> <span data-ttu-id="61357-377">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="61357-377">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="61357-378">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="61357-378">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-379">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="61357-379">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="61357-380">Id. de cuenta único en la plataforma de facturación de MSFT.</span><span class="sxs-lookup"><span data-stu-id="61357-380">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="61357-381">1280018095</span><span class="sxs-lookup"><span data-stu-id="61357-381">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-382">UsageDate</span><span class="sxs-lookup"><span data-stu-id="61357-382">UsageDate</span></span></td>
<td><p><span data-ttu-id="61357-383">Fecha de implementación del servicio.</span><span class="sxs-lookup"><span data-stu-id="61357-383">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="61357-384">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="61357-384">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-385">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="61357-385">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="61357-386">Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena.</span><span class="sxs-lookup"><span data-stu-id="61357-386">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="61357-387">Asia oriental, Sur asiático, Norte de Europa, Europa occidental, Norte central de EE. UU., Sur central de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="61357-387">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-388">MeteredService</span><span class="sxs-lookup"><span data-stu-id="61357-388">MeteredService</span></span></td>
<td><p><span data-ttu-id="61357-389">Esta columna se usa para hacer un seguimiento de los servicios de Microsoft Azure individuales que quizás no se identifiquen específicamente en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="61357-389">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="61357-390">Por ejemplo, las transferencias de datos se notifican como &quot;Microsoft Azure: todos los servicios&quot; en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="61357-390">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="61357-391">En esta columna MeteredService se indicará qué servicio específico pertenece el uso.</span><span class="sxs-lookup"><span data-stu-id="61357-391">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="61357-392">AccessControl, CDN, Proceso, Base de datos, ServiceBus, Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="61357-392">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-393">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="61357-393">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="61357-394">Subtítulo que aclara el servicio de Microsoft Azure individual más allá del nivel proporcionado por el campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="61357-394">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="61357-395">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="61357-395">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-396">Proyecto</span><span class="sxs-lookup"><span data-stu-id="61357-396">Project</span></span></td>
<td><p><span data-ttu-id="61357-397">Nombre definido por el cliente para la instancia del servicio</span><span class="sxs-lookup"><span data-stu-id="61357-397">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="61357-398">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="61357-398">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-399">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="61357-399">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="61357-400">Número de conexiones de Bus de servicio aprovisionadas y usadas en un día determinado.</span><span class="sxs-lookup"><span data-stu-id="61357-400">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="61357-401">Por ejemplo: si tenías una conexión aprovisionada individualmente durante un mes de 30 días, Service Info 1 contendría 1 "1,000000 conexiones/30 días".</span><span class="sxs-lookup"><span data-stu-id="61357-401">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days”.</span></span> <span data-ttu-id="61357-402">Si tuviera un paquete de 25 de conexiones de bus de servicio aprovisionada y ha utilizado 1 durante ese día, el extracto de uso diario durante ese día indicaría "25 conexiones / 30 días: utilizado: 1.000000”.</span><span class="sxs-lookup"><span data-stu-id="61357-402">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days – Used: 1.000000”.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-403">CustomerID</span><span class="sxs-lookup"><span data-stu-id="61357-403">CustomerID</span></span></td>
<td><p><span data-ttu-id="61357-404">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="61357-404">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="61357-405">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="61357-405">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="61357-406">DomainName</span><span class="sxs-lookup"><span data-stu-id="61357-406">DomainName</span></span></td>
<td><p><span data-ttu-id="61357-407">Cliente&#39;nombre de dominio de s, que ayuda a identificar el cliente.</span><span class="sxs-lookup"><span data-stu-id="61357-407">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="61357-408">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="61357-408">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="61357-409">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="61357-409">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="61357-410">Unidad</span><span class="sxs-lookup"><span data-stu-id="61357-410">Unit</span></span></td>
<td><p><span data-ttu-id="61357-411">La unidad del nombre del recurso</span><span class="sxs-lookup"><span data-stu-id="61357-411">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="61357-412">GB u HORAS</span><span class="sxs-lookup"><span data-stu-id="61357-412">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="61357-413">Campos del archivo periódicas y únicas</span><span class="sxs-lookup"><span data-stu-id="61357-413">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="61357-414">Column</span><span class="sxs-lookup"><span data-stu-id="61357-414">Column</span></span></th>
<th><span data-ttu-id="61357-415">Descripción</span><span class="sxs-lookup"><span data-stu-id="61357-415">Description</span></span></th>
</tr>
</thead>
<tbody>


<tr class="odd">
<td><span data-ttu-id="61357-416">PartnerId</span><span class="sxs-lookup"><span data-stu-id="61357-416">PartnerId</span></span></td>
<td><p><span data-ttu-id="61357-417">Identificador único del inquilino de Microsoft Azure Active Directory para una entidad de facturación específica, en formato GUID.</span><span class="sxs-lookup"><span data-stu-id="61357-417">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="61357-418">No es necesario para la reconciliación, pero puede ser información útil.</span><span class="sxs-lookup"><span data-stu-id="61357-418">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="61357-419">Igual en todas las filas.</span><span class="sxs-lookup"><span data-stu-id="61357-419">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-420">Id. de cliente</span><span class="sxs-lookup"><span data-stu-id="61357-420">Customer Id</span></span></td>
<td><p><span data-ttu-id="61357-421">Microsoft Azure Active Directory inquilino identificador único, en formato GUID, que usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="61357-421">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-422">Nombre del cliente</span><span class="sxs-lookup"><span data-stu-id="61357-422">Customer Name</span></span></td>
<td><p><span data-ttu-id="61357-423">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="61357-423">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-424">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="61357-424">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="61357-425">Nombre de dominio del cliente, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="61357-425">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="61357-426">No debe usarse para identificar al cliente como el cliente o socio puede actualizar el dominio personal de forma predeterminada a través del portal de Office 365.</span><span class="sxs-lookup"><span data-stu-id="61357-426">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="61357-427">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="61357-427">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-428">País del cliente</span><span class="sxs-lookup"><span data-stu-id="61357-428">Customer Country</span></span></td>
<td><p><span data-ttu-id="61357-429">El país donde se encuentra el cliente.</span><span class="sxs-lookup"><span data-stu-id="61357-429">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-430">Número de factura</span><span class="sxs-lookup"><span data-stu-id="61357-430">Invoice number</span></span></td>
<td><p><span data-ttu-id="61357-431">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="61357-431">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-432">MpnId</span><span class="sxs-lookup"><span data-stu-id="61357-432">MpnId</span></span></td>
<td><p><span data-ttu-id="61357-433">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="61357-433">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-434">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="61357-434">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="61357-435">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="61357-435">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-436">Id. de pedido</span><span class="sxs-lookup"><span data-stu-id="61357-436">Order ID</span></span></td>
<td><p><span data-ttu-id="61357-437">Identificador único para un pedido en la plataforma de comercio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="61357-437">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="61357-438">Puede ser útil para identificar al pedido al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-438">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-439">Fecha del pedido</span><span class="sxs-lookup"><span data-stu-id="61357-439">Order date</span></span></td>
<td><p><span data-ttu-id="61357-440">Fecha de realización del pedido.</span><span class="sxs-lookup"><span data-stu-id="61357-440">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-441">ProductId</span><span class="sxs-lookup"><span data-stu-id="61357-441">ProductId</span></span></td>
<td><p><span data-ttu-id="61357-442">Identificador del producto.</span><span class="sxs-lookup"><span data-stu-id="61357-442">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-443">SkuId</span><span class="sxs-lookup"><span data-stu-id="61357-443">SkuId</span></span></td>
<td><p><span data-ttu-id="61357-444">Id. de un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="61357-444">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-445">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="61357-445">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="61357-446">Id. de una disponibilidad concreta.</span><span class="sxs-lookup"><span data-stu-id="61357-446">The ID for a particular Availability.</span></span> <span data-ttu-id="61357-447">"Disponibilidad" hace referencia a si un SKU concreto está o no disponible para su compra para el país, la moneda, el segmento industrial determinados, etc.</span><span class="sxs-lookup"><span data-stu-id="61357-447">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-448">Nombre de SKU</span><span class="sxs-lookup"><span data-stu-id="61357-448">SKU Name</span></span></td>
<td><p><span data-ttu-id="61357-449">Título para un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="61357-449">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-450">Nombre del producto</span><span class="sxs-lookup"><span data-stu-id="61357-450">Product name</span></span></td>
<td><p><span data-ttu-id="61357-451">Nombre del producto.</span><span class="sxs-lookup"><span data-stu-id="61357-451">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-452">PublisherName</span><span class="sxs-lookup"><span data-stu-id="61357-452">PublisherName</span></span></td>
<td><p><span data-ttu-id="61357-453">El nombre del publicador del producto.</span><span class="sxs-lookup"><span data-stu-id="61357-453">The name of the product’s publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-454">PublisherID</span><span class="sxs-lookup"><span data-stu-id="61357-454">PublisherID</span></span></td>
<td><p><span data-ttu-id="61357-455">Identificador único para este publicador.</span><span class="sxs-lookup"><span data-stu-id="61357-455">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-456">Descripción de la suscripción</span><span class="sxs-lookup"><span data-stu-id="61357-456">Subscription Description</span></span></td>
<td><p><span data-ttu-id="61357-457">Nombre descriptivo de una suscripción.</span><span class="sxs-lookup"><span data-stu-id="61357-457">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-458">Id. de la suscripción</span><span class="sxs-lookup"><span data-stu-id="61357-458">Subscription ID</span></span></td>
<td><p><span data-ttu-id="61357-459">Identificador único para una suscripción en la plataforma de comercio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="61357-459">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="61357-460">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-460">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="61357-461">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="61357-461">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-462">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="61357-462">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="61357-463">Día de inicio de los cargos.</span><span class="sxs-lookup"><span data-stu-id="61357-463">Start day of the charges.</span></span> <span data-ttu-id="61357-464">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="61357-464">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-465">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="61357-465">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="61357-466">Día de finalización de los cargos.</span><span class="sxs-lookup"><span data-stu-id="61357-466">End day of the charges.</span></span> <span data-ttu-id="61357-467">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="61357-467">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-468">Término y Billingcycle</span><span class="sxs-lookup"><span data-stu-id="61357-468">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="61357-469">La duración del período y ciclo de facturación para la compra.</span><span class="sxs-lookup"><span data-stu-id="61357-469">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="61357-470">Por ejemplo, "1 año, mes".</span><span class="sxs-lookup"><span data-stu-id="61357-470">For example, “1 Year, Monthly.”</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-471">Tipo de cargo</span><span class="sxs-lookup"><span data-stu-id="61357-471">Charge Type</span></span></td>
<td><p><span data-ttu-id="61357-472">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="61357-472">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-473">Precio unitario</span><span class="sxs-lookup"><span data-stu-id="61357-473">Unit Price</span></span></td>
<td><p><span data-ttu-id="61357-474">El precio publicado en la lista de precios en el momento de la compra.</span><span class="sxs-lookup"><span data-stu-id="61357-474">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="61357-475">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-475">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-476">Precio unitario efectivo</span><span class="sxs-lookup"><span data-stu-id="61357-476">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="61357-477">El precio por unidad una vez realizados los ajustes.</span><span class="sxs-lookup"><span data-stu-id="61357-477">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-478">Cantidad</span><span class="sxs-lookup"><span data-stu-id="61357-478">Quantity</span></span></td>
<td><p><span data-ttu-id="61357-479">Número de unidades.</span><span class="sxs-lookup"><span data-stu-id="61357-479">Number of units.</span></span> <span data-ttu-id="61357-480">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-480">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-481">Tipo de unidad</span><span class="sxs-lookup"><span data-stu-id="61357-481">Unit type</span></span></td>
<td><p><span data-ttu-id="61357-482">El tipo de unidad que se compra.</span><span class="sxs-lookup"><span data-stu-id="61357-482">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-483">DiscountDetails</span><span class="sxs-lookup"><span data-stu-id="61357-483">DiscountDetails</span></span></td>
<td><p><span data-ttu-id="61357-484">Explicación de los descuentos aplicables.</span><span class="sxs-lookup"><span data-stu-id="61357-484">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-485">Subtotal</span><span class="sxs-lookup"><span data-stu-id="61357-485">Sub Total</span></span></td>
<td><p><span data-ttu-id="61357-486">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="61357-486">Total before tax.</span></span> <span data-ttu-id="61357-487">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="61357-487">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-488">Total de impuestos</span><span class="sxs-lookup"><span data-stu-id="61357-488">Tax Total</span></span></td>
<td><p><span data-ttu-id="61357-489">Cargo por importe de impuestos, en función de las reglas fiscales de tu mercado y las circunstancias específicas.</span><span class="sxs-lookup"><span data-stu-id="61357-489">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-490">Total</span><span class="sxs-lookup"><span data-stu-id="61357-490">Total</span></span></td>
<td><p><span data-ttu-id="61357-491">Total con impuestos.</span><span class="sxs-lookup"><span data-stu-id="61357-491">Total after tax.</span></span> <span data-ttu-id="61357-492">Comprueba si se cobran impuestos en la factura.</span><span class="sxs-lookup"><span data-stu-id="61357-492">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-493">Currency</span><span class="sxs-lookup"><span data-stu-id="61357-493">Currency</span></span></td>
<td><p><span data-ttu-id="61357-494">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="61357-494">Currency type.</span></span> <span data-ttu-id="61357-495">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="61357-495">Each billing entity has only one currency.</span></span> <span data-ttu-id="61357-496">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="61357-496">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-497">AlternateID</span><span class="sxs-lookup"><span data-stu-id="61357-497">AlternateID</span></span></td>
<td><p><span data-ttu-id="61357-498">Un identificador alternativo para un identificador de pedido.</span><span class="sxs-lookup"><span data-stu-id="61357-498">An alternate identifier to an order ID.</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="61357-499">Campos del archivo de uso diario calificados</span><span class="sxs-lookup"><span data-stu-id="61357-499">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="61357-500">Column</span><span class="sxs-lookup"><span data-stu-id="61357-500">Column</span></span></th>
<th><span data-ttu-id="61357-501">Descripción</span><span class="sxs-lookup"><span data-stu-id="61357-501">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="61357-502">PartnerId</span><span class="sxs-lookup"><span data-stu-id="61357-502">PartnerId</span></span></td>
<td><p><span data-ttu-id="61357-503">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="61357-503">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-504">PartnerName</span><span class="sxs-lookup"><span data-stu-id="61357-504">PartnerName</span></span></td>
<td><p><span data-ttu-id="61357-505">Nombre del partner.</span><span class="sxs-lookup"><span data-stu-id="61357-505">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-506">CustomerId</span><span class="sxs-lookup"><span data-stu-id="61357-506">CustomerId</span></span></td>
<td><p><span data-ttu-id="61357-507">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="61357-507">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-508">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="61357-508">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="61357-509">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="61357-509">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="61357-510">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="61357-510">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-511">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="61357-511">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="61357-512">Nombre de dominio del cliente.</span><span class="sxs-lookup"><span data-stu-id="61357-512">The customer’s domain name.</span></span> <span data-ttu-id="61357-513">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="61357-513">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-514">País del cliente</span><span class="sxs-lookup"><span data-stu-id="61357-514">Customer country</span></span></td>
<td><p><span data-ttu-id="61357-515">El país donde se encuentra el cliente.</span><span class="sxs-lookup"><span data-stu-id="61357-515">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-516">MPNID</span><span class="sxs-lookup"><span data-stu-id="61357-516">MPNID</span></span></td>
<td><p><span data-ttu-id="61357-517">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="61357-517">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-518">Distribuidor MPNID</span><span class="sxs-lookup"><span data-stu-id="61357-518">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="61357-519">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="61357-519">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="61357-520">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="61357-520">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-521">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="61357-521">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="61357-522">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="61357-522">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="61357-523">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="61357-523">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-524">ProductId</span><span class="sxs-lookup"><span data-stu-id="61357-524">ProductId</span></span></td>
<td><p><span data-ttu-id="61357-525">Identificador del producto.</span><span class="sxs-lookup"><span data-stu-id="61357-525">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-526">SkuId</span><span class="sxs-lookup"><span data-stu-id="61357-526">SkuId</span></span></td>
<td><p><span data-ttu-id="61357-527">Id. de un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="61357-527">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-528">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="61357-528">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="61357-529">Id. de una disponibilidad concreta.</span><span class="sxs-lookup"><span data-stu-id="61357-529">The ID for a particular Availability.</span></span> <span data-ttu-id="61357-530">"Disponibilidad" hace referencia a si un SKU concreto está o no disponible para su compra para el país, la moneda, el segmento industrial determinados, etc.</span><span class="sxs-lookup"><span data-stu-id="61357-530">“Availability” refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-531">Nombre de SKU</span><span class="sxs-lookup"><span data-stu-id="61357-531">SKU Name</span></span></td>
<td><p><span data-ttu-id="61357-532">Título para un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="61357-532">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-533">PublisherName</span><span class="sxs-lookup"><span data-stu-id="61357-533">PublisherName</span></span></td>
<td><p><span data-ttu-id="61357-534">El nombre del publicador.</span><span class="sxs-lookup"><span data-stu-id="61357-534">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-535">PublisherID</span><span class="sxs-lookup"><span data-stu-id="61357-535">PublisherID</span></span></td>
<td><p><span data-ttu-id="61357-536">El identificador del publicador, en formato GUID.</span><span class="sxs-lookup"><span data-stu-id="61357-536">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="61357-537">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="61357-537">Not available for current activity.</span></span></p></td>
</tr>

<tr class=”even">
<td><span data-ttu-id="61357-538">Descripción de la suscripción</span><span class="sxs-lookup"><span data-stu-id="61357-538">Subscription Description</span></span></td>
<td><p><span data-ttu-id="61357-539">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="61357-539">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="61357-540">(Este es un campo idéntico al nombre de la oferta).</span><span class="sxs-lookup"><span data-stu-id="61357-540">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-541">Id. de la suscripción</span><span class="sxs-lookup"><span data-stu-id="61357-541">Subscription ID</span></span></td>
<td><p><span data-ttu-id="61357-542">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="61357-542">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="61357-543">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-543">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="61357-544">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="61357-544">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-545">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="61357-545">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="61357-546">Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="61357-546">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="61357-547">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="61357-547">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-548">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="61357-548">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="61357-549">Fecha de finalización del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="61357-549">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="61357-550">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="61357-550">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-551">Fecha de uso</span><span class="sxs-lookup"><span data-stu-id="61357-551">Usage Date</span></span></td>
<td><p><span data-ttu-id="61357-552">Fecha de uso del servicio.</span><span class="sxs-lookup"><span data-stu-id="61357-552">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-553">Tipo de medidor</span><span class="sxs-lookup"><span data-stu-id="61357-553">Meter Type</span></span></td>
<td><p><span data-ttu-id="61357-554">El tipo de medidor.</span><span class="sxs-lookup"><span data-stu-id="61357-554">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-555">Categoría de medidor</span><span class="sxs-lookup"><span data-stu-id="61357-555">Meter Category</span></span></td>
<td><p><span data-ttu-id="61357-556">El servicio de nivel superior para el uso.</span><span class="sxs-lookup"><span data-stu-id="61357-556">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-557">Id. de medidor</span><span class="sxs-lookup"><span data-stu-id="61357-557">Meter Id</span></span></td>
<td><p><span data-ttu-id="61357-558">El identificador del medidor que se va a usar.</span><span class="sxs-lookup"><span data-stu-id="61357-558">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-559">Subcategoría de medidor</span><span class="sxs-lookup"><span data-stu-id="61357-559">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="61357-560">El tipo de servicio de Azure que puede afectar a la tarifa.</span><span class="sxs-lookup"><span data-stu-id="61357-560">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-561">Nombre de medidor</span><span class="sxs-lookup"><span data-stu-id="61357-561">Meter Name</span></span></td>
<td><p><span data-ttu-id="61357-562">La unidad de medida del medidor consumido.</span><span class="sxs-lookup"><span data-stu-id="61357-562">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-563">Región de medidor</span><span class="sxs-lookup"><span data-stu-id="61357-563">Meter Region</span></span></td>
<td><p><span data-ttu-id="61357-564">Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena.</span><span class="sxs-lookup"><span data-stu-id="61357-564">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-565">Unidad</span><span class="sxs-lookup"><span data-stu-id="61357-565">Unit</span></span></td>
<td><p><span data-ttu-id="61357-566">La unidad del nombre de recurso.</span><span class="sxs-lookup"><span data-stu-id="61357-566">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-567">Cantidad consumida</span><span class="sxs-lookup"><span data-stu-id="61357-567">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="61357-568">La cantidad de servicio consumida (horas, GB, etc.) durante el período de notificación.</span><span class="sxs-lookup"><span data-stu-id="61357-568">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="61357-569">También incluye cualquier uso no facturado de períodos anteriores.</span><span class="sxs-lookup"><span data-stu-id="61357-569">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-570">Ubicación de recursos</span><span class="sxs-lookup"><span data-stu-id="61357-570">Resource Location</span></span></td>
<td><p><span data-ttu-id="61357-571">El centro de datos donde se está ejecutando el medidor.</span><span class="sxs-lookup"><span data-stu-id="61357-571">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-572">Servicio consumido</span><span class="sxs-lookup"><span data-stu-id="61357-572">Consumed Service</span></span></td>
<td><p><span data-ttu-id="61357-573">El servicio de la plataforma Azure que usó.</span><span class="sxs-lookup"><span data-stu-id="61357-573">The Azure platform service that you used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-574">Grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="61357-574">Resource Group</span></span></td>
<td><p><span data-ttu-id="61357-575">El grupo de recursos en el que se está ejecutando el medidor implementado.</span><span class="sxs-lookup"><span data-stu-id="61357-575">The resource group in which the deployed meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-576">URI de recurso</span><span class="sxs-lookup"><span data-stu-id="61357-576">Resource URI</span></span></td>
<td><p><span data-ttu-id="61357-577">El URI del recurso que se va a usar.</span><span class="sxs-lookup"><span data-stu-id="61357-577">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-578">Tipo de cargo</span><span class="sxs-lookup"><span data-stu-id="61357-578">Charge type</span></span></td>
<td><p><span data-ttu-id="61357-579">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="61357-579">The type of charge or adjustment.</span></span> <span data-ttu-id="61357-580">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="61357-580">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-581">Precio unitario</span><span class="sxs-lookup"><span data-stu-id="61357-581">Unit price</span></span></td>
<td><p><span data-ttu-id="61357-582">Precio por licencia, como se publica en la lista de precios en el momento de la compra.</span><span class="sxs-lookup"><span data-stu-id="61357-582">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="61357-583">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-583">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-584">Cantidad</span><span class="sxs-lookup"><span data-stu-id="61357-584">Quantity</span></span></td>
<td><p><span data-ttu-id="61357-585">Número de licencias.</span><span class="sxs-lookup"><span data-stu-id="61357-585">Number of licenses.</span></span> <span data-ttu-id="61357-586">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-586">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-587">Tipo de unidad</span><span class="sxs-lookup"><span data-stu-id="61357-587">Unit type</span></span></td>
<td><p><span data-ttu-id="61357-588">El tipo de unidad que se cobra el medidor.</span><span class="sxs-lookup"><span data-stu-id="61357-588">The type of unit the meter is charged in.</span></span> <span data-ttu-id="61357-589">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="61357-589">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-590">Impuestos de facturación anterior a</span><span class="sxs-lookup"><span data-stu-id="61357-590">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="61357-591">Cantidad total antes de impuestos.</span><span class="sxs-lookup"><span data-stu-id="61357-591">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-592">Divisa de facturación</span><span class="sxs-lookup"><span data-stu-id="61357-592">Billing currency</span></span></td>
<td><p><span data-ttu-id="61357-593">La moneda en la región geográfica del cliente</span><span class="sxs-lookup"><span data-stu-id="61357-593">The currency in the customer’s geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-594">Precio total antes de impuestos</span><span class="sxs-lookup"><span data-stu-id="61357-594">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="61357-595">Los precios antes de que se agregan los impuestos.</span><span class="sxs-lookup"><span data-stu-id="61357-595">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-596">Precios de moneda</span><span class="sxs-lookup"><span data-stu-id="61357-596">Pricing currency</span></span></td>
<td><p><span data-ttu-id="61357-597">La moneda en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="61357-597">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-598">Información de servicio 1</span><span class="sxs-lookup"><span data-stu-id="61357-598">Service Info 1</span></span></td>
<td><p><span data-ttu-id="61357-599">Número de conexiones de Bus de servicio aprovisionadas y usadas en un día determinado.</span><span class="sxs-lookup"><span data-stu-id="61357-599">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-600">Información de servicio 2</span><span class="sxs-lookup"><span data-stu-id="61357-600">Service Info 2</span></span></td>
<td><p><span data-ttu-id="61357-601">Un campo heredado que captura los metadatos específicos del servicio opcional.</span><span class="sxs-lookup"><span data-stu-id="61357-601">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="61357-602">`Tags`</span><span class="sxs-lookup"><span data-stu-id="61357-602">Tags</span></span></td>
<td><p><span data-ttu-id="61357-603">Etiquetas que asigna al medidor en orden para agrupar los registros de facturación.</span><span class="sxs-lookup"><span data-stu-id="61357-603">Tags you assign to the meter in order to group billing records.</span></span> <span data-ttu-id="61357-604">Por ejemplo, puede usar etiquetas para distribuir los costos por el departamento que utiliza el medidor.</span><span class="sxs-lookup"><span data-stu-id="61357-604">For example, you can use tags to distribute costs by the department that uses the meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="61357-605">Información adicional</span><span class="sxs-lookup"><span data-stu-id="61357-605">Additional Info</span></span></td>
<td><p><span data-ttu-id="61357-606">Cualquier información adicional que no se tratan en otras columnas.</span><span class="sxs-lookup"><span data-stu-id="61357-606">Any additional information not covered in other columns.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="61357-607">Asignación de cargos entre una factura y el archivo de conciliación</span><span class="sxs-lookup"><span data-stu-id="61357-607">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="61357-608">La factura proporciona un resumen de los cargos, mientras que el archivo de conciliación proporciona un desglose detallado de las transacciones de elementos de línea, incluidos los tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="61357-608">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="61357-609">Para hacer referencias cruzadas de cantidades de cargos entre el archivo de conciliación y la factura, puedes usar las opciones de filtro de Microsoft Excel para filtrar por tipo de cargo en el archivo de conciliación con el fin de asignar los cargos de facturación a un conjunto de desgloses de cargos del archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-609">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="61357-610">Los archivos de conciliación, tanto basados en uso como en licencias, solo muestran cargos y transacciones relacionados con el uso (unidades consumidas y cargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="61357-610">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="61357-611">En el archivo de conciliación no aparecen devoluciones, descuentos o créditos excepcionales que aparecen en la factura como "Ajustes".</span><span class="sxs-lookup"><span data-stu-id="61357-611">One off credits, discounts or refunds which appear on the invoice as “Adjustments” are not shown in the reconciliation file.</span></span>

<span data-ttu-id="61357-612">La siguiente tabla muestra las asignaciones entre una sección de factura y los tipos de cargo asociados que es posible que se muestren en los archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="61357-612">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="61357-613"><strong>Descripción de cargos de facturación</strong></span><span class="sxs-lookup"><span data-stu-id="61357-613"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-614"><strong>Descripción de cargos del archivo de conciliación (columna ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="61357-614"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-615"><strong>¿Qué es este cargo?</strong></span><span class="sxs-lookup"><span data-stu-id="61357-615"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-616"><strong>¿Cómo se asignan estos ChargeTypes a la factura?</strong></span><span class="sxs-lookup"><span data-stu-id="61357-616"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="61357-617"><strong>Cargos de licencia</strong></span><span class="sxs-lookup"><span data-stu-id="61357-617"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-618">Tarifa de activación</span><span class="sxs-lookup"><span data-stu-id="61357-618">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-619">El importe cobrado al cliente cuando usa la suscripción después de adquirirla</span><span class="sxs-lookup"><span data-stu-id="61357-619">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="61357-620">Desde el archivo basado en licencia, suma la columna <strong>Amount</strong>.</span><span class="sxs-lookup"><span data-stu-id="61357-620">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="61357-621">Cuota de cancelación</span><span class="sxs-lookup"><span data-stu-id="61357-621">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-622">Cargos prorrateados reembolsados al cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="61357-622">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="61357-623">Tarifa de ciclo</span><span class="sxs-lookup"><span data-stu-id="61357-623">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-624">Cargos periódicos de una suscripción</span><span class="sxs-lookup"><span data-stu-id="61357-624">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="61357-625">Prorrateo de instancia de ciclo</span><span class="sxs-lookup"><span data-stu-id="61357-625">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-626">Cargos prorrateados evaluados del cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="61357-626">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="61357-627">Tarifas prorrateadas al cancelar</span><span class="sxs-lookup"><span data-stu-id="61357-627">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-628">Reembolso prorrateado de la parte no usada del servicio tras la cancelación</span><span class="sxs-lookup"><span data-stu-id="61357-628">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="61357-629">Tarifas prorrateadas al comprar</span><span class="sxs-lookup"><span data-stu-id="61357-629">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-630">El tipo de gasto para una suscripción cuando se usa la facturación anual</span><span class="sxs-lookup"><span data-stu-id="61357-630">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="61357-631">Tarifa de compra</span><span class="sxs-lookup"><span data-stu-id="61357-631">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-632">El tipo de gasto para una suscripción cuando se usa la facturación mensual</span><span class="sxs-lookup"><span data-stu-id="61357-632">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="61357-633">Tarifa prorrateada al renovar</span><span class="sxs-lookup"><span data-stu-id="61357-633">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-634">Tarifas prorrateadas tras la renovación de la suscripción</span><span class="sxs-lookup"><span data-stu-id="61357-634">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="61357-635">Tarifa de renovación</span><span class="sxs-lookup"><span data-stu-id="61357-635">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-636">Cargo por renovar una suscripción</span><span class="sxs-lookup"><span data-stu-id="61357-636">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="61357-637">Tarifas prorrateadas al activar</span><span class="sxs-lookup"><span data-stu-id="61357-637">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-638">Tarifas prorrateadas desde la activación hasta el final del período de facturación</span><span class="sxs-lookup"><span data-stu-id="61357-638">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="61357-639"><strong>Cargos de un solo uso</strong></span><span class="sxs-lookup"><span data-stu-id="61357-639"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="61357-640">Nuevo</span><span class="sxs-lookup"><span data-stu-id="61357-640">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-641">Utiliza cuando se crea una nueva compra</span><span class="sxs-lookup"><span data-stu-id="61357-641">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="61357-642">addQuantity</span><span class="sxs-lookup"><span data-stu-id="61357-642">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-643">Utilizar en ambos el reembolso de la compra original y la cantidad nuevo después de aumento</span><span class="sxs-lookup"><span data-stu-id="61357-643">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="61357-644">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="61357-644">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-645">Utilizar en ambos el reembolso de la compra original y la cantidad nuevo después de disminución</span><span class="sxs-lookup"><span data-stu-id="61357-645">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="61357-646">Cancelar</span><span class="sxs-lookup"><span data-stu-id="61357-646">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-647">Usar cuando se cancela una suscripción</span><span class="sxs-lookup"><span data-stu-id="61357-647">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="61357-648">Convertir</span><span class="sxs-lookup"><span data-stu-id="61357-648">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-649">Utilizar cuando se actualiza una licencia pero no cambia el número de puestos</span><span class="sxs-lookup"><span data-stu-id="61357-649">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="61357-650"><strong>Cargos de uso</strong></span><span class="sxs-lookup"><span data-stu-id="61357-650"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-651">Evaluar la tarifa de uso al cancelar</span><span class="sxs-lookup"><span data-stu-id="61357-651">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-652">Tarifa de uso de acceso tras la cancelación por uso impagado durante el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="61357-652">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="61357-653">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="61357-653">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="61357-654">Evaluar la tarifa de uso para el ciclo actual</span><span class="sxs-lookup"><span data-stu-id="61357-654">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-655">tarifa de uso de acceso para el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="61357-655">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="61357-656"><strong>Créditos</strong></span><span class="sxs-lookup"><span data-stu-id="61357-656"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-657">Desplazamiento de un elemento de línea</span><span class="sxs-lookup"><span data-stu-id="61357-657">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-658">Reembolso parcial o total de un elemento de línea, incluidos impuestos</span><span class="sxs-lookup"><span data-stu-id="61357-658">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-659">Desde el archivo basado en licencia, suma la columna <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="61357-659">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="61357-660">Desde el archivo basado en uso, suma la columna <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="61357-660">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="61357-661"><strong>Descuentos basados en uso</strong></span><span class="sxs-lookup"><span data-stu-id="61357-661"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-662">Descuento de activación</span><span class="sxs-lookup"><span data-stu-id="61357-662">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-663">Descuento que se aplica cuando se activa la suscripción</span><span class="sxs-lookup"><span data-stu-id="61357-663">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="61357-664">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="61357-664">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="61357-665">Descuento de ciclo</span><span class="sxs-lookup"><span data-stu-id="61357-665">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-666">Descuento que se aplica en cargos periódicos</span><span class="sxs-lookup"><span data-stu-id="61357-666">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="61357-667">Descuento de renovación</span><span class="sxs-lookup"><span data-stu-id="61357-667">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-668">Descuento que se aplica cuando se renueva la suscripción</span><span class="sxs-lookup"><span data-stu-id="61357-668">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="61357-669">Descuento de cancelación</span><span class="sxs-lookup"><span data-stu-id="61357-669">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-670">Cargos que se aplican cuando se cancelan los descuentos</span><span class="sxs-lookup"><span data-stu-id="61357-670">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="61357-671"><strong>Descuentos de licencias</strong></span><span class="sxs-lookup"><span data-stu-id="61357-671"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-672"><em>Se pueden aplicar a varios tipos de cargos</em></span><span class="sxs-lookup"><span data-stu-id="61357-672"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="61357-673">Desde el archivo basado en licencia, suma la columna <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="61357-673">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="61357-674"><strong>Impuestos</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="61357-674"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-675"><em>Se pueden aplicar a varios tipos de cargos</em></span><span class="sxs-lookup"><span data-stu-id="61357-675"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="61357-676"><em>Excepción: &quot;Desplazamiento de un elemento de línea&quot; ya incluye los impuestos. Consulte los créditos, más arriba.</em></span><span class="sxs-lookup"><span data-stu-id="61357-676"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-677">Impuestos o impuesto de valor añadido (IVA)</span><span class="sxs-lookup"><span data-stu-id="61357-677">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="61357-678">Desde el archivo basado en licencia, suma la columna <strong>Tax</strong>.</span><span class="sxs-lookup"><span data-stu-id="61357-678">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="61357-679">Desde el archivo basado en uso, suma la columna <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="61357-679">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
