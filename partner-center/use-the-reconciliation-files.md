---
title: Usar los archivos de conciliación | Centro de partners
ms.topic: article
ms.date: 11/07/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para obtener una vista detallada de los elementos de línea de cada cargo en un ciclo de facturación, descargue los archivos de conciliación del centro de Partners.
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 217d5e9c068a07b51f74333f605daca8ab573c9a
ms.sourcegitcommit: 8425d3435892651e3e6cb1147cd3b268b2b1869b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/07/2019
ms.locfileid: "73753852"
---
# <a name="use-the-reconciliation-files"></a><span data-ttu-id="72ca2-103">Usar los archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="72ca2-103">Use the reconciliation files</span></span>

<span data-ttu-id="72ca2-104">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="72ca2-104">**Applies to**</span></span>

-  <span data-ttu-id="72ca2-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="72ca2-105">Partner Center</span></span>
-  <span data-ttu-id="72ca2-106">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="72ca2-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="72ca2-107">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="72ca2-107">**Appropriate roles**</span></span>

- <span data-ttu-id="72ca2-108">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="72ca2-108">Billing admin</span></span>
- <span data-ttu-id="72ca2-109">Administrador global</span><span class="sxs-lookup"><span data-stu-id="72ca2-109">Global admin</span></span>

<span data-ttu-id="72ca2-110">Para obtener una vista detallada de los elementos de línea de cada cargo en un ciclo de facturación, descargue los archivos de conciliación del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="72ca2-110">For a detailed line-item view of each charge in a billing cycle, download the reconciliation files from Partner Center.</span></span> <span data-ttu-id="72ca2-111">Los detalles incluyen los cargos para las suscripciones de cada cliente y los eventos detallados (por ejemplo, una adición intermedia de puestos en una suscripción).</span><span class="sxs-lookup"><span data-stu-id="72ca2-111">The details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of seats to a subscription).</span></span>

## <a name="formatting-issues"></a><span data-ttu-id="72ca2-112">Problemas de formato</span><span class="sxs-lookup"><span data-stu-id="72ca2-112">Formatting issues</span></span>

<span data-ttu-id="72ca2-113">En ocasiones, es posible que el archivo de conciliación tenga problemas de formato.</span><span class="sxs-lookup"><span data-stu-id="72ca2-113">Occasionally your recon file might have formatting issues.</span></span> <span data-ttu-id="72ca2-114">(Esto puede ocurrir, por ejemplo, si no se usa la configuración regional EN-US). Siga los pasos que se indican a continuación para solucionar estos problemas.</span><span class="sxs-lookup"><span data-stu-id="72ca2-114">(This can happen, for example, if the EN-US locale is not used.) Follow the steps below to fix these issues.</span></span> 

<ol>
<li><span data-ttu-id="72ca2-115">Abra el archivo. csv en Excel y seleccione la primera columna.</span><span class="sxs-lookup"><span data-stu-id="72ca2-115">Open the .csv file in Excel, and select the first column.</span></span> <span data-ttu-id="72ca2-116">En la cinta de opciones, seleccione <strong>datos</strong>y, a continuación, seleccione <strong>texto en columnas</strong>.</span><span class="sxs-lookup"><span data-stu-id="72ca2-116">On the ribbon, select <strong>Data</strong>, and then select <strong>Text to Columns</strong>.</span></span></li>

<li><span data-ttu-id="72ca2-117">En el asistente convertir texto en columnas, seleccione <strong>delimitado tipo de archivo</strong>y, a continuación, seleccione <strong>siguiente</strong>.</span><span class="sxs-lookup"><span data-stu-id="72ca2-117">In the Convert Text to Columns Wizard, select <strong>Delimited file type</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="72ca2-118">En el campo delimitadores, seleccione <strong>coma</strong>.</span><span class="sxs-lookup"><span data-stu-id="72ca2-118">In the Delimeters field, select <strong>Comma</strong>.</span></span> <span data-ttu-id="72ca2-119">Si la <strong>pestaña</strong> ya está seleccionada, puede dejarla.</span><span class="sxs-lookup"><span data-stu-id="72ca2-119">If <strong>Tab</strong> is already selected, you can leave it.</span></span> <span data-ttu-id="72ca2-120">Selecciona <strong>Siguiente</strong>.</span><span class="sxs-lookup"><span data-stu-id="72ca2-120">Select <strong>Next</strong>.</span></span></li>

<li><span data-ttu-id="72ca2-121">En el campo formato de datos de columna, seleccione <strong>Fecha: MDA</strong>y, a continuación, seleccione <strong>siguiente</strong>.</span><span class="sxs-lookup"><span data-stu-id="72ca2-121">In the Column data format field, select <strong>Date: MDY</strong>, and then select <strong>Next</strong>.</span></span></li> 

<li><span data-ttu-id="72ca2-122">En el campo formato de datos de columna, seleccione <strong>texto</strong> para todas las columnas de cantidad y, a continuación, seleccione <strong>Finalizar</strong>.</span><span class="sxs-lookup"><span data-stu-id="72ca2-122">In the Column data format field, select <strong>Text</strong> for all amount columns, and then select <strong>Finish</strong>.</span></span></li>
</ol>

## <a name="downloading-a-large-recon-file"></a><span data-ttu-id="72ca2-123">Descarga de un archivo de conciliación grande</span><span class="sxs-lookup"><span data-stu-id="72ca2-123">Downloading a large recon file</span></span>

<span data-ttu-id="72ca2-124">Los archivos de conciliación pueden llegar a ser muy grandes y a veces son difíciles de descargar.</span><span class="sxs-lookup"><span data-stu-id="72ca2-124">Recon files can grow very large and are sometimes difficult to download.</span></span> <span data-ttu-id="72ca2-125">Para obtener un script de PowerShell que ayude a descargar archivos de conciliación grandes, consulte [obtener artículos de línea de factura](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="72ca2-125">For a PowerShell script to help download large recon files, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a href="" id="itemizebypartner"></a><span data-ttu-id="72ca2-126">Elemento por asociado</span><span class="sxs-lookup"><span data-stu-id="72ca2-126">Itemize by partner</span></span>


<span data-ttu-id="72ca2-127">Los partners del modelo indirecto pueden usar estos campos adicionales en ambos archivos de conciliación basada en uso y en licencia para realizar el desglose por revendedor.</span><span class="sxs-lookup"><span data-stu-id="72ca2-127">Partners in the indirect model can use these additional fields in both license-based and usage-based reconciliation files to itemize by reseller.</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="72ca2-128">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="72ca2-128">MPN ID</span></span></th>
<th><span data-ttu-id="72ca2-129">Descripción</span><span class="sxs-lookup"><span data-stu-id="72ca2-129">Description</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="72ca2-130">Id. de MPN</span><span class="sxs-lookup"><span data-stu-id="72ca2-130">MPN ID</span></span></td>
<td><p><span data-ttu-id="72ca2-131">Id. de Microsoft Partner Network (MPN) del partner de CSP (directo o indirecto).</span><span class="sxs-lookup"><span data-stu-id="72ca2-131">The Microsoft Partner Network (MPN) ID of the CSP partner (direct or indirect).</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-132">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="72ca2-132">Reseller MPN ID</span></span></td>
<td><p><span data-ttu-id="72ca2-133">Solo aparece en los archivos de conciliación de partners en el modelo indirecto.</span><span class="sxs-lookup"><span data-stu-id="72ca2-133">Only appears on reconciliation files for partners in the indirect model.</span></span></p>
<p><span data-ttu-id="72ca2-134">El Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="72ca2-134">The MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="72ca2-135">Corresponde al id. de revendedor indicado para la suscripción específica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="72ca2-135">This corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span></p>
<p><span data-ttu-id="72ca2-136">eTo ver o actualizar el distribuidor, en el menú del centro de Partners, seleccione <strong>clientes</strong>y, a continuación, elija el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="72ca2-136">eTo view or update the reseller, from the Partner Center menu, select <strong>Customers</strong>, then choose the customer from the list.</span></span> <span data-ttu-id="72ca2-137">En el menú del cliente, selecciona <strong>Suscripciones</strong> y elige la suscripción de la lista.</span><span class="sxs-lookup"><span data-stu-id="72ca2-137">In the customer menu, select <strong>Subscriptions</strong>, choose the subscription from the list.</span></span> <span data-ttu-id="72ca2-138">Selecciona <strong>Actualizar</strong> para cambiar el valor de <strong>Revendedor (id. de MPN)</strong>.</span><span class="sxs-lookup"><span data-stu-id="72ca2-138">Select <strong>update</strong> to change the <strong>Reseller (MPN ID)</strong>.</span></span></p>
<p><span data-ttu-id="72ca2-139">Si un partner CSP vendió la suscripción directamente al cliente, su id. de MPN aparece dos veces, como id. de MPN y como id. de MPN del revendedor.</span><span class="sxs-lookup"><span data-stu-id="72ca2-139">If a CSP partner sold the subscription directly to the customer, their MPN ID is listed twice, as both the MPN ID and the Reseller MPN ID.</span></span></p>
<p><span data-ttu-id="72ca2-140">Si un asociado de CSP tiene un revendedor sin identificador de MPN, este valor se establece en el identificador de MPN del asociado en su lugar.</span><span class="sxs-lookup"><span data-stu-id="72ca2-140">If a CSP partner has a reseller with no MPN ID, this value is set to the partner's MPN ID instead.</span></span></p>
<p><span data-ttu-id="72ca2-141">Si el partner CSP quita un id. de revendedor, este valor se establece en -1.</span><span class="sxs-lookup"><span data-stu-id="72ca2-141">If the CSP partner removes a reseller ID, this value will be set to -1.</span></span></p></td>
</tr>
</tbody>
</table>

 

## <a href="" id="licensebasedfiles"></a><span data-ttu-id="72ca2-142">Campos de archivos basados en licencias</span><span class="sxs-lookup"><span data-stu-id="72ca2-142">License-based file fields</span></span>


<span data-ttu-id="72ca2-143">Para conciliar los cargos en función de los pedidos del cliente, compara el Syndication\_Partner\_Subscription\_Number del archivo de conciliación con el id. de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="72ca2-143">To reconcile your charges against your customer's orders, compare the Syndication\_Partner\_Subscription\_Number from the reconciliation file against the Subscription ID from Partner Center.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="72ca2-144"><strong>Artículo</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-144"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="72ca2-145"><strong>Descripción</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-145"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="72ca2-146"><strong>Valor de ejemplo</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-146"><strong>Sample Value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-147">PartnerId</span><span class="sxs-lookup"><span data-stu-id="72ca2-147">PartnerId</span></span></td>
<td><p><span data-ttu-id="72ca2-148">Identificador único de una entidad de facturación específica, con formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="72ca2-148">Unique identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="72ca2-149">No es necesario para la reconciliación, pero puede ser información útil.</span><span class="sxs-lookup"><span data-stu-id="72ca2-149">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="72ca2-150">Igual en todas las filas.</span><span class="sxs-lookup"><span data-stu-id="72ca2-150">Same in all rows.</span></span></p></td>
<td><span data-ttu-id="72ca2-151">8ddd03642-test-test-test-46b58d356b4e</span><span class="sxs-lookup"><span data-stu-id="72ca2-151">8ddd03642-test-test-test-46b58d356b4e</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-152">CustomerID</span><span class="sxs-lookup"><span data-stu-id="72ca2-152">CustomerID</span></span></td>
<td><p><span data-ttu-id="72ca2-153">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="72ca2-153">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="72ca2-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span><span class="sxs-lookup"><span data-stu-id="72ca2-154">12ABCD34-001A-BCD2-987C-3210ABCD5678</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-155">OrderID</span><span class="sxs-lookup"><span data-stu-id="72ca2-155">OrderID</span></span></td>
<td><p><span data-ttu-id="72ca2-156">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="72ca2-156">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="72ca2-157">Puede ser útil para identificar al pedido al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-157">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="72ca2-158">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="72ca2-158">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-159">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="72ca2-159">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="72ca2-160">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="72ca2-160">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="72ca2-161">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-161">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="72ca2-162">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="72ca2-162">This is not the same as the Subscription ID on the Partner Admin Console.</span></span> <span data-ttu-id="72ca2-163">Consulte Syndication_Partner_Subscription_Number.</span><span class="sxs-lookup"><span data-stu-id="72ca2-163">Please see Syndication_Partner_Subscription_Number.</span></span></p></td>
<td><span data-ttu-id="72ca2-164">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="72ca2-164">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-165">SyndicationPartnerSubscriptionNumber</span><span class="sxs-lookup"><span data-stu-id="72ca2-165">SyndicationPartnerSubscriptionNumber</span></span></td>
<td><p><span data-ttu-id="72ca2-166">Identificador único de las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="72ca2-166">Unique identifier for subscriptions.</span></span> <span data-ttu-id="72ca2-167">Un cliente puede tener varias suscripciones para el mismo plan, por lo que es importante para el análisis de archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-167">A customer can have multiple subscriptions for the same plan, so this is important for reconciliation file analysis.</span></span></p>
<p><span data-ttu-id="72ca2-168">Este campo se asigna al identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="72ca2-168">This field maps to the Subscription ID in the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="72ca2-169">fb977ab5-test-test-test-24c8d9591708</span><span class="sxs-lookup"><span data-stu-id="72ca2-169">fb977ab5-test-test-test-24c8d9591708</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-170">OfferID</span><span class="sxs-lookup"><span data-stu-id="72ca2-170">OfferID</span></span></td>
<td><p><span data-ttu-id="72ca2-171">Identificador único de la oferta.</span><span class="sxs-lookup"><span data-stu-id="72ca2-171">Unique offer ID.</span></span> <span data-ttu-id="72ca2-172">Identificador de la oferta estándar según la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="72ca2-172">Standard offer ID as per price list.</span></span></p>
<p><span data-ttu-id="72ca2-173"><b>Nota</b>: este valor no coincide con el id. de oferta de la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="72ca2-173"><b>Note</b>: This value does not match Offer ID from the price list.</span></span> <span data-ttu-id="72ca2-174">Consulta DurableOfferID a continuación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-174">See DurableOfferID below.</span></span></p></td>
<td><span data-ttu-id="72ca2-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span><span class="sxs-lookup"><span data-stu-id="72ca2-175">FE616D64-E9A8-40EF-843F-152E9BBEF3D1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-176">DurableOfferID</span><span class="sxs-lookup"><span data-stu-id="72ca2-176">DurableOfferID</span></span></td>
<td><p><span data-ttu-id="72ca2-177">Id. de oferta duradera único, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="72ca2-177">Unique durable offer ID, as defined in the price list.</span></span></p>
<p><span data-ttu-id="72ca2-178"><b>Nota</b>: este valor coincide con el id. de oferta de la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="72ca2-178"><b>Note</b>: This value matches the Offer ID from the price list.</span></span></p></td>
<td><span data-ttu-id="72ca2-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span><span class="sxs-lookup"><span data-stu-id="72ca2-179">1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-180">OfferName</span><span class="sxs-lookup"><span data-stu-id="72ca2-180">OfferName</span></span></td>
<td><p><span data-ttu-id="72ca2-181">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="72ca2-181">The name of the service offering purchased by the customer, as defined in the price list.</span></span></p></td>
<td><span data-ttu-id="72ca2-182">Microsoft Office 365 (Plan E3)</span><span class="sxs-lookup"><span data-stu-id="72ca2-182">Microsoft Office 365 (Plan E3)</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-183">SubscriptionStartDate</span><span class="sxs-lookup"><span data-stu-id="72ca2-183">SubscriptionStartDate</span></span></td>
<td><p><span data-ttu-id="72ca2-184">Fecha de finalización de la suscripción, establecida en el día posterior al envío del pedido.</span><span class="sxs-lookup"><span data-stu-id="72ca2-184">The subscription start date, set to the day after the order is submitted.</span></span> <span data-ttu-id="72ca2-185">Al consultar la fecha de inicio de la suscripción junto con la fecha de finalización, puedes determinar si el cliente aún está dentro del primer año de la suscripción o si la suscripción se ha renovado para el año siguiente.</span><span class="sxs-lookup"><span data-stu-id="72ca2-185">By looking at the subscription start date in conjunction with the end date, you can determine if the customer is still within the first year of the subscription or if the subscription has been renewed for the following year.</span></span></p>
<p><span data-ttu-id="72ca2-186">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="72ca2-186">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="72ca2-187">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="72ca2-187">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-188">SubscriptionEndDate</span><span class="sxs-lookup"><span data-stu-id="72ca2-188">SubscriptionEndDate</span></span></td>
<td><p><span data-ttu-id="72ca2-189">La fecha de finalización de la suscripción: 12 meses + x días después de la fecha de inicio (para que se alinee con la fecha de facturación del partner) o 12 meses a partir de la fecha de renovación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-189">The subscription end date: 12 months + x days after start date (to align with partner billing date) or 12 months from renewal date.</span></span></p>
<p><span data-ttu-id="72ca2-190">En el momento de la renovación, los precios se actualizan según la lista de precios actual.</span><span class="sxs-lookup"><span data-stu-id="72ca2-190">At renewal, prices are updated to the current price list.</span></span> <span data-ttu-id="72ca2-191">Es posible que se necesite una comunicación con el cliente antes de la renovación automatizada.</span><span class="sxs-lookup"><span data-stu-id="72ca2-191">Customer communication may be required in advance of automated renewal.</span></span></p>
<p><span data-ttu-id="72ca2-192">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="72ca2-192">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="72ca2-193">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="72ca2-193">2/1/2015 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-194">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="72ca2-194">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="72ca2-195">Día de inicio de los cargos.</span><span class="sxs-lookup"><span data-stu-id="72ca2-195">Start day of the charges.</span></span></p>
<p><span data-ttu-id="72ca2-196">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="72ca2-196">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="72ca2-197">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="72ca2-197">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="72ca2-198">1/2/2015 0:00</span><span class="sxs-lookup"><span data-stu-id="72ca2-198">2/1/2015 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-199">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="72ca2-199">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="72ca2-200">Día de finalización de los cargos.</span><span class="sxs-lookup"><span data-stu-id="72ca2-200">End day of the charges.</span></span></p>
<p><span data-ttu-id="72ca2-201">Cuando un cliente cambia los números de puestos, este número se usa para calcular los cargos por día (proporcionales).</span><span class="sxs-lookup"><span data-stu-id="72ca2-201">When a customer changes seat numbers, this number is used to calculate per-day (pro-rata) charges.</span></span></p>
<p><span data-ttu-id="72ca2-202">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="72ca2-202">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="72ca2-203">28/2/2015 23:59</span><span class="sxs-lookup"><span data-stu-id="72ca2-203">2/28/2015 23:59</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-204">ChargeType</span><span class="sxs-lookup"><span data-stu-id="72ca2-204">ChargeType</span></span></td>
<td><p><span data-ttu-id="72ca2-205">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="72ca2-205">The type of charge or adjustment.</span></span> <span data-ttu-id="72ca2-206">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="72ca2-206">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="72ca2-207">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="72ca2-207">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-208">UnitPrice</span><span class="sxs-lookup"><span data-stu-id="72ca2-208">UnitPrice</span></span></td>
<td><p><span data-ttu-id="72ca2-209">Precio por puesto, tal y como se publica en la lista de precios en el momento de compra.</span><span class="sxs-lookup"><span data-stu-id="72ca2-209">Price per seat, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="72ca2-210">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-210">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="72ca2-211">6.82</span><span class="sxs-lookup"><span data-stu-id="72ca2-211">6.82</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-212">Cantidad</span><span class="sxs-lookup"><span data-stu-id="72ca2-212">Quantity</span></span></td>
<td><p><span data-ttu-id="72ca2-213">Número de puestos.</span><span class="sxs-lookup"><span data-stu-id="72ca2-213">Number of seats.</span></span> <span data-ttu-id="72ca2-214">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-214">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
<td><span data-ttu-id="72ca2-215">2</span><span class="sxs-lookup"><span data-stu-id="72ca2-215">2</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-216">Volumen</span><span class="sxs-lookup"><span data-stu-id="72ca2-216">Amount</span></span></td>
<td><p><span data-ttu-id="72ca2-217">Total del precio para la cantidad.</span><span class="sxs-lookup"><span data-stu-id="72ca2-217">Total of price for quantity.</span></span> <span data-ttu-id="72ca2-218">Es de utilidad para comprobar que el cálculo de la cantidad coincide con la manera de calcular este valor para los clientes.</span><span class="sxs-lookup"><span data-stu-id="72ca2-218">Useful to check that the amount calculation matches how you calculate this for your customers.</span></span></p></td>
<td><span data-ttu-id="72ca2-219">13.32</span><span class="sxs-lookup"><span data-stu-id="72ca2-219">13.32</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-220">TotalOtherDiscount</span><span class="sxs-lookup"><span data-stu-id="72ca2-220">TotalOtherDiscount</span></span></td>
<td><p><span data-ttu-id="72ca2-221">Cantidad de descuento que se aplica a estos cargos.</span><span class="sxs-lookup"><span data-stu-id="72ca2-221">Amount of discount applied to these charges.</span></span> <span data-ttu-id="72ca2-222">Las licencias de producto incluidas con una competencia o asignaciones o nuevas suscripciones válidas para un incentivo también incluirán un importe de descuento en esta columna.</span><span class="sxs-lookup"><span data-stu-id="72ca2-222">Product Licenses included with a competency or MAPS or new subscriptions eligible for an incentive will also contain a discount amount in this column.</span></span></p></td>
<td><span data-ttu-id="72ca2-223">2.32</span><span class="sxs-lookup"><span data-stu-id="72ca2-223">2.32</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-224">Subtotal</span><span class="sxs-lookup"><span data-stu-id="72ca2-224">Subtotal</span></span></td>
<td><p><span data-ttu-id="72ca2-225">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="72ca2-225">Total before tax.</span></span> <span data-ttu-id="72ca2-226">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="72ca2-226">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
<td><span data-ttu-id="72ca2-227">11</span><span class="sxs-lookup"><span data-stu-id="72ca2-227">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-228">Impuestos</span><span class="sxs-lookup"><span data-stu-id="72ca2-228">Tax</span></span></td>
<td><p><span data-ttu-id="72ca2-229">Cargo del importe de los impuestos, en&#39;función de las reglas de impuestos del mercado y las circunstancias específicas.</span><span class="sxs-lookup"><span data-stu-id="72ca2-229">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="72ca2-230">0</span><span class="sxs-lookup"><span data-stu-id="72ca2-230">0</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-231">TotalForCustomer</span><span class="sxs-lookup"><span data-stu-id="72ca2-231">TotalForCustomer</span></span></td>
<td><p><span data-ttu-id="72ca2-232">Total con impuestos.</span><span class="sxs-lookup"><span data-stu-id="72ca2-232">Total after tax.</span></span> <span data-ttu-id="72ca2-233">Comprueba si se cobran impuestos en la factura.</span><span class="sxs-lookup"><span data-stu-id="72ca2-233">Checks if you are charged tax in the invoice.</span></span></p></td>
<td><span data-ttu-id="72ca2-234">11</span><span class="sxs-lookup"><span data-stu-id="72ca2-234">11</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-235">Moneda</span><span class="sxs-lookup"><span data-stu-id="72ca2-235">Currency</span></span></td>
<td><p><span data-ttu-id="72ca2-236">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="72ca2-236">Currency type.</span></span> <span data-ttu-id="72ca2-237">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="72ca2-237">Each billing entity has only one currency.</span></span> <span data-ttu-id="72ca2-238">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-238">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="72ca2-239">EUR</span><span class="sxs-lookup"><span data-stu-id="72ca2-239">EUR</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-240">CustomerName</span><span class="sxs-lookup"><span data-stu-id="72ca2-240">CustomerName</span></span></td>
<td><p><span data-ttu-id="72ca2-241">Nombre&#39;de la organización del cliente como se indicó en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="72ca2-241">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="72ca2-242">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="72ca2-242">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="72ca2-243">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="72ca2-243">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-244">MPNID</span><span class="sxs-lookup"><span data-stu-id="72ca2-244">MPNID</span></span></td>
<td><p><span data-ttu-id="72ca2-245">Id. de MPN del partner CSP</span><span class="sxs-lookup"><span data-stu-id="72ca2-245">MPN ID of the CSP partner</span></span></p></td>
<td><span data-ttu-id="72ca2-246">4390934</span><span class="sxs-lookup"><span data-stu-id="72ca2-246">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-247">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="72ca2-247">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="72ca2-248">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="72ca2-248">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="72ca2-249">Ver <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Desglosar por partner</a></span><span class="sxs-lookup"><span data-stu-id="72ca2-249">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="72ca2-250">4390934</span><span class="sxs-lookup"><span data-stu-id="72ca2-250">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-251">DomainName</span><span class="sxs-lookup"><span data-stu-id="72ca2-251">DomainName</span></span></td>
<td><p><span data-ttu-id="72ca2-252">Nombre&#39;de dominio del cliente, que se usa para ayudar a identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="72ca2-252">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="72ca2-253">No debe usarse para identificar de forma exclusiva al cliente como cliente o asociado puede actualizar el dominio de cortesía/predeterminado mediante el portal de O365.</span><span class="sxs-lookup"><span data-stu-id="72ca2-253">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="72ca2-254">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-254">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="72ca2-255">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="72ca2-255">example.onmicrosoft.com</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-256">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="72ca2-256">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="72ca2-257">Alias de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="72ca2-257">Subscription nickname.</span></span> <span data-ttu-id="72ca2-258">Si no se especifica ningún alias, el Centro de partners usa OfferName.</span><span class="sxs-lookup"><span data-stu-id="72ca2-258">If no nickname is specified, Partner Center uses the OfferName.</span></span></p></td>
<td><span data-ttu-id="72ca2-259">PROJECT ONLINE</span><span class="sxs-lookup"><span data-stu-id="72ca2-259">PROJECT ONLINE</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-260">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="72ca2-260">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="72ca2-261">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="72ca2-261">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="72ca2-262">(Este es un campo idéntico al nombre de la oferta).</span><span class="sxs-lookup"><span data-stu-id="72ca2-262">(This is an identical field to Offer name).</span></span></p></td>
<td><span data-ttu-id="72ca2-263">PROJECT ONLINE PREMIUM SIN CLIENTE DE PROJECT</span><span class="sxs-lookup"><span data-stu-id="72ca2-263">PROJECT ONLINE PREMIUM WITHOUT PROJECT CLIENT</span></span></td>
</tr>
</tbody>
</table>


## <a href="" id="usagebasedfiles"></a><span data-ttu-id="72ca2-264">Campos de archivos basados en el uso</span><span class="sxs-lookup"><span data-stu-id="72ca2-264">Usage-based file fields</span></span>


<span data-ttu-id="72ca2-265">Para conciliar los cargos en función del uso de tu cliente, compara los valores de ResellerID/ResellerName/ResellerBillableAccount del archivo de conciliación, el nombre del cliente y el id. de suscripción del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="72ca2-265">To reconcile your charges against your customer's usage, compare the ResellerID/ResellerName/ResellerBillableAccount from the reconciliation file, the customer name, and the Subscription ID from Partner Center.</span></span>

<span data-ttu-id="72ca2-266">Los siguientes campos explican los servicios usados y la clasificación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-266">The following fields explain which services were used and the rate.</span></span>

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><span data-ttu-id="72ca2-267"><strong>Artículo</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-267"><strong>Column</strong></span></span></td>
<td><span data-ttu-id="72ca2-268"><strong>Descripción</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-268"><strong>Description</strong></span></span></td>
<td><span data-ttu-id="72ca2-269"><strong>Valor de ejemplo</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-269"><strong>Sample value</strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-270">PartnerID</span><span class="sxs-lookup"><span data-stu-id="72ca2-270">PartnerID</span></span></td>
<td><p><span data-ttu-id="72ca2-271">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="72ca2-271">Partner ID, in GUID format.</span></span></p></td>
<td><span data-ttu-id="72ca2-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="72ca2-272">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-273">PartnerName</span><span class="sxs-lookup"><span data-stu-id="72ca2-273">PartnerName</span></span></td>
<td><p><span data-ttu-id="72ca2-274">Nombre del partner.</span><span class="sxs-lookup"><span data-stu-id="72ca2-274">Partner Name.</span></span></p></td>
<td><span data-ttu-id="72ca2-275">Acme Incorporated</span><span class="sxs-lookup"><span data-stu-id="72ca2-275">Acme Incorporated</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-276">PartnerBillableAccountID</span><span class="sxs-lookup"><span data-stu-id="72ca2-276">PartnerBillableAccountID</span></span></td>
<td><p><span data-ttu-id="72ca2-277">Id. de cuenta del partner.</span><span class="sxs-lookup"><span data-stu-id="72ca2-277">Partner Account ID.</span></span></p></td>
<td><span data-ttu-id="72ca2-278">1010578050</span><span class="sxs-lookup"><span data-stu-id="72ca2-278">1010578050</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-279">CustomerName</span><span class="sxs-lookup"><span data-stu-id="72ca2-279">CustomerName</span></span></td>
<td><p><span data-ttu-id="72ca2-280">Nombre&#39;de la organización del cliente como se indicó en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="72ca2-280">Customer&#39;s organization name as reported in Partner Center.</span></span> <span data-ttu-id="72ca2-281">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="72ca2-281">This is very important for reconciling the invoice with your system information.</span></span></p></td>
<td><span data-ttu-id="72ca2-282">Cliente de prueba A</span><span class="sxs-lookup"><span data-stu-id="72ca2-282">Test Customer A</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-283">MPNID</span><span class="sxs-lookup"><span data-stu-id="72ca2-283">MPNID</span></span></td>
<td><p><span data-ttu-id="72ca2-284">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="72ca2-284">MPN ID of the CSP partner.</span></span></p></td>
<td><span data-ttu-id="72ca2-285">4390934</span><span class="sxs-lookup"><span data-stu-id="72ca2-285">4390934</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-286">ResellerMPNID</span><span class="sxs-lookup"><span data-stu-id="72ca2-286">ResellerMPNID</span></span></td>
<td><p><span data-ttu-id="72ca2-287">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="72ca2-287">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="72ca2-288">Ver <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Desglosar por partner</a></span><span class="sxs-lookup"><span data-stu-id="72ca2-288">See <a href="#itemizebypartner" data-raw-source="[Itemize by partner](#itemizebypartner)">Itemize by partner</a>.</span></span></p></td>
<td><span data-ttu-id="72ca2-289">4390934</span><span class="sxs-lookup"><span data-stu-id="72ca2-289">4390934</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-290">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="72ca2-290">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="72ca2-291">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="72ca2-291">Invoice number where the specified transaction appears.</span></span></p></td>
<td><span data-ttu-id="72ca2-292">D020001IVK</span><span class="sxs-lookup"><span data-stu-id="72ca2-292">D020001IVK</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-293">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="72ca2-293">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="72ca2-294">Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="72ca2-294">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="72ca2-295">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="72ca2-295">The time is always the beginning of the day, 0:00.</span></span></p></td>
<td><span data-ttu-id="72ca2-296">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="72ca2-296">2/1/2014 0:00</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-297">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="72ca2-297">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="72ca2-298">Fecha de finalización del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="72ca2-298">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span></p>
<p><span data-ttu-id="72ca2-299">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="72ca2-299">The time is always the end of the day, 23:59.</span></span></p></td>
<td><span data-ttu-id="72ca2-300">28/2/2014 23:59</span><span class="sxs-lookup"><span data-stu-id="72ca2-300">2/28/2014 23:59</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-301">SubscriptionID</span><span class="sxs-lookup"><span data-stu-id="72ca2-301">SubscriptionID</span></span></td>
<td><p><span data-ttu-id="72ca2-302">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="72ca2-302">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="72ca2-303">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-303">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p>
<p><span data-ttu-id="72ca2-304">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="72ca2-304">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
<td><span data-ttu-id="72ca2-305">usCBMgAAAAAAAAIA</span><span class="sxs-lookup"><span data-stu-id="72ca2-305">usCBMgAAAAAAAAIA</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-306">SubscriptionName</span><span class="sxs-lookup"><span data-stu-id="72ca2-306">SubscriptionName</span></span></td>
<td><p><span data-ttu-id="72ca2-307">Alias de la oferta de servicio.</span><span class="sxs-lookup"><span data-stu-id="72ca2-307">Nickname of the service offering.</span></span></p></td>
<td><span data-ttu-id="72ca2-308">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="72ca2-308">Microsoft Azure</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-309">SubscriptionDescription</span><span class="sxs-lookup"><span data-stu-id="72ca2-309">SubscriptionDescription</span></span></td>
<td><p><span data-ttu-id="72ca2-310">Línea de negocio de la oferta de servicio</span><span class="sxs-lookup"><span data-stu-id="72ca2-310">Line of business of the service offering</span></span></p></td>
<td><span data-ttu-id="72ca2-311">Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="72ca2-311">Microsoft Azure</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-312">OrderID</span><span class="sxs-lookup"><span data-stu-id="72ca2-312">OrderID</span></span></td>
<td><p><span data-ttu-id="72ca2-313">Identificador único de un pedido en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="72ca2-313">Unique identifier for an order in the Microsoft billing platform.</span></span> <span data-ttu-id="72ca2-314">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-314">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span></p></td>
<td><span data-ttu-id="72ca2-315">566890604832738111</span><span class="sxs-lookup"><span data-stu-id="72ca2-315">566890604832738111</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-316">ServiceName</span><span class="sxs-lookup"><span data-stu-id="72ca2-316">ServiceName</span></span></td>
<td><p><span data-ttu-id="72ca2-317">Nombre del servicio de Azure en cuestión.</span><span class="sxs-lookup"><span data-stu-id="72ca2-317">The name of the Azure service in question.</span></span></p></td>
<td><span data-ttu-id="72ca2-318">MÁQUINAS VIRTUALES</span><span class="sxs-lookup"><span data-stu-id="72ca2-318">VIRTUAL MACHINES</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-319">ServiceType</span><span class="sxs-lookup"><span data-stu-id="72ca2-319">ServiceType</span></span></td>
<td><p><span data-ttu-id="72ca2-320">Tipo específico de servicio de Microsoft Azure.</span><span class="sxs-lookup"><span data-stu-id="72ca2-320">The specific type of Windows Azure service.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="72ca2-321">Service Bus: individual o Pack</span><span class="sxs-lookup"><span data-stu-id="72ca2-321">Service Bus - Individual or Pack</span></span></li>
<li><span data-ttu-id="72ca2-322">Base de datos de SQL Azure: Business o Web Edition</span><span class="sxs-lookup"><span data-stu-id="72ca2-322">SQL Azure database - Business or Web Edition</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-323">ResourceGUID</span><span class="sxs-lookup"><span data-stu-id="72ca2-323">ResourceGUID</span></span></td>
<td><p><span data-ttu-id="72ca2-324">Identificador único específico para toda la estructura de precios y datos del servicio.</span><span class="sxs-lookup"><span data-stu-id="72ca2-324">Specific unique identifier for all the service data and pricing structure.</span></span></p></td>
<td><span data-ttu-id="72ca2-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span><span class="sxs-lookup"><span data-stu-id="72ca2-325">DA41BC5F-C52D-4464-8A8D-8C8DCC43503B</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-326">Nombre del recurso</span><span class="sxs-lookup"><span data-stu-id="72ca2-326">Resource Name</span></span></td>
<td><p><span data-ttu-id="72ca2-327">Nombre del recurso de Azure.</span><span class="sxs-lookup"><span data-stu-id="72ca2-327">The name of the Azure resource.</span></span></p></td>
<td><ul>
<li><span data-ttu-id="72ca2-328">Transferencia entrante de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="72ca2-328">Data Transfer In (GB)</span></span></li>
<li><span data-ttu-id="72ca2-329">Transferencia saliente de datos (GB)</span><span class="sxs-lookup"><span data-stu-id="72ca2-329">Data Transfer Out (GB)</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-330">Región</span><span class="sxs-lookup"><span data-stu-id="72ca2-330">Region</span></span></td>
<td><p><span data-ttu-id="72ca2-331">La región a la que se aplica el uso.</span><span class="sxs-lookup"><span data-stu-id="72ca2-331">The region the usage applies to.</span></span> <span data-ttu-id="72ca2-332">Se usa principalmente para asignar tarifas a las transferencias de datos, ya que las tarifas varían según la región.</span><span class="sxs-lookup"><span data-stu-id="72ca2-332">Primarily used to assign rates to data transfers, as rates vary by region.</span></span></p></td>
<td><span data-ttu-id="72ca2-333">Asia Pacífico, Europa, América Latina, América del Norte</span><span class="sxs-lookup"><span data-stu-id="72ca2-333">Asia Pacific, Europe, Latin America, North America</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-334">SKU</span><span class="sxs-lookup"><span data-stu-id="72ca2-334">SKU</span></span></td>
<td><p><span data-ttu-id="72ca2-335">Identificador único de MSFT para la oferta</span><span class="sxs-lookup"><span data-stu-id="72ca2-335">MSFT unique identifier for offer</span></span></p></td>
<td><span data-ttu-id="72ca2-336">7UD 00001</span><span class="sxs-lookup"><span data-stu-id="72ca2-336">7UD-00001</span></span></td>
</tr>
<tr class="odd">
<td><p><span data-ttu-id="72ca2-337">DetailLineItemId</span><span class="sxs-lookup"><span data-stu-id="72ca2-337">DetailLineItemId</span></span></p></td>
<td><p><span data-ttu-id="72ca2-338">Un id. y una cantidad para desglosar las distintas clasificaciones de un servicio o un recurso en un período de facturación determinado.</span><span class="sxs-lookup"><span data-stu-id="72ca2-338">An ID and quantity for itemizing the different rates for a service or resource in a given billing period.</span></span> <span data-ttu-id="72ca2-339">Para clasificación en niveles de Azure, puede haber una clasificación hasta una cantidad determinada de unidades facturables y, posteriormente, una clasificación diferente.</span><span class="sxs-lookup"><span data-stu-id="72ca2-339">For Azure tiered rating, there may be one rate up to a certain quantity of billable units, then a different rate after that.</span></span></p></td>
<td><span data-ttu-id="72ca2-340">1</span><span class="sxs-lookup"><span data-stu-id="72ca2-340">1</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-341">ConsumedQuantity</span><span class="sxs-lookup"><span data-stu-id="72ca2-341">ConsumedQuantity</span></span></td>
<td><p><span data-ttu-id="72ca2-342">La cantidad de servicio consumida (horas, GB, etc.) durante el período de notificación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-342">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span></p>
<p><span data-ttu-id="72ca2-343">También incluye cualquier uso no facturado de períodos anteriores.</span><span class="sxs-lookup"><span data-stu-id="72ca2-343">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
<td><span data-ttu-id="72ca2-344">11</span><span class="sxs-lookup"><span data-stu-id="72ca2-344">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-345">IncludedQuantity</span><span class="sxs-lookup"><span data-stu-id="72ca2-345">IncludedQuantity</span></span></td>
<td><p><span data-ttu-id="72ca2-346">Unidades que se incluyen como parte de la oferta.</span><span class="sxs-lookup"><span data-stu-id="72ca2-346">Units included as part of the offer.</span></span> <span data-ttu-id="72ca2-347">No suele mostrarse en CSP.</span><span class="sxs-lookup"><span data-stu-id="72ca2-347">Not typically present in CSP.</span></span></p></td>
<td><span data-ttu-id="72ca2-348">0</span><span class="sxs-lookup"><span data-stu-id="72ca2-348">0</span></span></td>
</tr>
<tr class="even">
<td><p><span data-ttu-id="72ca2-349">OverageQuantity</span><span class="sxs-lookup"><span data-stu-id="72ca2-349">OverageQuantity</span></span></p></td>
<td><p><span data-ttu-id="72ca2-350">Unidades que no se incluyen como parte de la oferta y que el partner debe abonar.</span><span class="sxs-lookup"><span data-stu-id="72ca2-350">Units not included as part of the offer, that must be paid for by the partner.</span></span></p>
<p><span data-ttu-id="72ca2-351">Equivale a ConsumedQuantity - IncludedQuantity.</span><span class="sxs-lookup"><span data-stu-id="72ca2-351">Equal to the ConsumedQuantity - IncludedQuantity.</span></span></p></td>
<td><span data-ttu-id="72ca2-352">11</span><span class="sxs-lookup"><span data-stu-id="72ca2-352">11</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-353">ListPrice</span><span class="sxs-lookup"><span data-stu-id="72ca2-353">ListPrice</span></span></td>
<td><p><span data-ttu-id="72ca2-354">Precio de la oferta en vigor la fecha de inicio de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="72ca2-354">Offer price in effect at subscription start date.</span></span></p></td>
<td><span data-ttu-id="72ca2-355">0\.0808 USD</span><span class="sxs-lookup"><span data-stu-id="72ca2-355">$0.0808</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-356">PretaxCharges</span><span class="sxs-lookup"><span data-stu-id="72ca2-356">PretaxCharges</span></span></td>
<td><p><span data-ttu-id="72ca2-357">ListPrist x OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="72ca2-357">ListPrist times OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="72ca2-358">0\.085 USD</span><span class="sxs-lookup"><span data-stu-id="72ca2-358">$0.085</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-359">TaxAmount</span><span class="sxs-lookup"><span data-stu-id="72ca2-359">TaxAmount</span></span></td>
<td><p><span data-ttu-id="72ca2-360">Cargo del importe de los impuestos, en&#39;función de las reglas de impuestos del mercado y las circunstancias específicas.</span><span class="sxs-lookup"><span data-stu-id="72ca2-360">Tax amount charge, based on your market&#39;s tax rules and specific circumstances.</span></span></p></td>
<td><span data-ttu-id="72ca2-361">0\.08 USD</span><span class="sxs-lookup"><span data-stu-id="72ca2-361">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-362">PostTaxTotal</span><span class="sxs-lookup"><span data-stu-id="72ca2-362">PostTaxTotal</span></span></td>
<td><p><span data-ttu-id="72ca2-363">Total con impuestos, si se aplican impuestos.</span><span class="sxs-lookup"><span data-stu-id="72ca2-363">Total after tax, when tax is applicable.</span></span></p></td>
<td><span data-ttu-id="72ca2-364">0\.93 USD</span><span class="sxs-lookup"><span data-stu-id="72ca2-364">$0.93</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-365">Moneda</span><span class="sxs-lookup"><span data-stu-id="72ca2-365">Currency</span></span></td>
<td><p><span data-ttu-id="72ca2-366">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="72ca2-366">Currency type.</span></span> <span data-ttu-id="72ca2-367">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="72ca2-367">Each billing entity has only one currency.</span></span> <span data-ttu-id="72ca2-368">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-368">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
<td><span data-ttu-id="72ca2-369">EUR</span><span class="sxs-lookup"><span data-stu-id="72ca2-369">EUR</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-370">PretaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="72ca2-370">PretaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="72ca2-371">Precio sin impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="72ca2-371">Pretax price per unit.</span></span> <span data-ttu-id="72ca2-372">Igual que PretaxCharges/OverageQuantity, redondeado al céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="72ca2-372">Equal to PretaxCharges / OverageQuantity, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="72ca2-373">0\.08 USD</span><span class="sxs-lookup"><span data-stu-id="72ca2-373">$0.08</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-374">PostTaxEffectiveRate</span><span class="sxs-lookup"><span data-stu-id="72ca2-374">PostTaxEffectiveRate</span></span></td>
<td><p><span data-ttu-id="72ca2-375">Precio después de impuestos por unidad.</span><span class="sxs-lookup"><span data-stu-id="72ca2-375">Post tax price per unit.</span></span> <span data-ttu-id="72ca2-376">Igual que PostTaxTotal/OverageQuantity o PretaxEffectiveRate + tipo impositivo por importe unitario, redondeado el céntimo más próximo.</span><span class="sxs-lookup"><span data-stu-id="72ca2-376">Equal to PostTaxTotal / OverageQuantity, or PretaxEffectiveRate + tax rate per unit amoun, rounded to the nearest cent.</span></span></p></td>
<td><span data-ttu-id="72ca2-377">0\.08 USD</span><span class="sxs-lookup"><span data-stu-id="72ca2-377">$0.08</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-378">ChargeType</span><span class="sxs-lookup"><span data-stu-id="72ca2-378">ChargeType</span></span></td>
<td><p><span data-ttu-id="72ca2-379">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="72ca2-379">The type of charge or adjustment.</span></span> <span data-ttu-id="72ca2-380">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="72ca2-380">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
<td><p><span data-ttu-id="72ca2-381">Consulta <a href="#charge_types">Asignación de cargos entre una factura y el archivo de conciliación</a></span><span class="sxs-lookup"><span data-stu-id="72ca2-381">See <a href="#charge_types">Mapping charges between an invoice and the reconciliation file</a></span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-382">CustomerBillableAccount</span><span class="sxs-lookup"><span data-stu-id="72ca2-382">CustomerBillableAccount</span></span></td>
<td><p><span data-ttu-id="72ca2-383">Id. de cuenta único en la plataforma de facturación de MSFT.</span><span class="sxs-lookup"><span data-stu-id="72ca2-383">Unique account ID in the MSFT billing platform.</span></span></p></td>
<td><span data-ttu-id="72ca2-384">1280018095</span><span class="sxs-lookup"><span data-stu-id="72ca2-384">1280018095</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-385">UsageDate</span><span class="sxs-lookup"><span data-stu-id="72ca2-385">UsageDate</span></span></td>
<td><p><span data-ttu-id="72ca2-386">Fecha de implementación del servicio.</span><span class="sxs-lookup"><span data-stu-id="72ca2-386">Date of service deployment.</span></span></p></td>
<td><span data-ttu-id="72ca2-387">1/2/2014 0:00</span><span class="sxs-lookup"><span data-stu-id="72ca2-387">2/1/2014 0:00</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-388">MeteredRegion</span><span class="sxs-lookup"><span data-stu-id="72ca2-388">MeteredRegion</span></span></td>
<td><p><span data-ttu-id="72ca2-389">Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena.</span><span class="sxs-lookup"><span data-stu-id="72ca2-389">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
<td><span data-ttu-id="72ca2-390">Asia Oriental, Asia Suroriental, Norte de Europa, Europa Occidental, Centro-norte de EE. UU., Centro-sur de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="72ca2-390">East Asia, South East Asia, North Europe, West Europe, North Central US, South Central US</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-391">MeteredService</span><span class="sxs-lookup"><span data-stu-id="72ca2-391">MeteredService</span></span></td>
<td><p><span data-ttu-id="72ca2-392">Esta columna se usa para hacer un seguimiento de los servicios de Microsoft Azure individuales que quizás no se identifiquen específicamente en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="72ca2-392">This column is utilized to track the individual Microsoft Azure service that may not be specifically identified in the Service Name column.</span></span> <span data-ttu-id="72ca2-393">Por ejemplo, las transferencias de datos se notifican como &quot;Microsoft Azure: todos los servicios&quot; en la columna Service Name.</span><span class="sxs-lookup"><span data-stu-id="72ca2-393">For example, data transfers are reported as &quot;Microsoft Azure - All Services&quot; in the Service Name column.</span></span> <span data-ttu-id="72ca2-394">En esta columna MeteredService se indicará qué servicio específico pertenece el uso.</span><span class="sxs-lookup"><span data-stu-id="72ca2-394">This MeteredService column will indicate to which specific service the usage pertains.</span></span></p></td>
<td><span data-ttu-id="72ca2-395">AccessControl, CDN, Proceso, Base de datos, ServiceBus, Almacenamiento</span><span class="sxs-lookup"><span data-stu-id="72ca2-395">AccessControl, CDN, Compute, Database, ServiceBus, Storage</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-396">MeteredServiceType</span><span class="sxs-lookup"><span data-stu-id="72ca2-396">MeteredServiceType</span></span></td>
<td><p><span data-ttu-id="72ca2-397">Subtítulo que aclara el servicio de Microsoft Azure individual más allá del nivel proporcionado por el campo MeteredService.</span><span class="sxs-lookup"><span data-stu-id="72ca2-397">A subheading that further clarifies the individual Microsoft Azure service beyond the level provided by the MeteredService field.</span></span></p></td>
<td><span data-ttu-id="72ca2-398">EXTERNO</span><span class="sxs-lookup"><span data-stu-id="72ca2-398">EXTERNAL</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-399">Proyecto</span><span class="sxs-lookup"><span data-stu-id="72ca2-399">Project</span></span></td>
<td><p><span data-ttu-id="72ca2-400">Nombre definido por el cliente para la instancia del servicio</span><span class="sxs-lookup"><span data-stu-id="72ca2-400">Customer-defined name for their service instance</span></span></p></td>
<td><span data-ttu-id="72ca2-401">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="72ca2-401">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-402">ServiceInfo</span><span class="sxs-lookup"><span data-stu-id="72ca2-402">ServiceInfo</span></span></td>
<td><p><span data-ttu-id="72ca2-403">Número de conexiones de Bus de servicio aprovisionadas y usadas en un día determinado.</span><span class="sxs-lookup"><span data-stu-id="72ca2-403">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
<td><span data-ttu-id="72ca2-404">Por ejemplo: Si tuviera una conexión aprovisionada individualmente durante un mes de 30 días, la información de servicio 1 leería "1,000000 conexiones/30 días".</span><span class="sxs-lookup"><span data-stu-id="72ca2-404">For example: if you had an individually provisioned connection during a 30 day month, Service Info 1 would read “1.000000 Connections / 30 days".</span></span> <span data-ttu-id="72ca2-405">Si tiene un 25 paquete de conexiones de ServiceBus aprovisionadas y usó 1 durante ese día, la instrucción de uso diario de ese día indicaría "25 conexiones/30 días-usado: 1,000000".</span><span class="sxs-lookup"><span data-stu-id="72ca2-405">If you had a 25 pack of ServiceBus connections provisioned and you had utilized 1 during that day, your daily usage statement for that day would indicate “25 Connections / 30 Days - Used: 1.000000".</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-406">CustomerID</span><span class="sxs-lookup"><span data-stu-id="72ca2-406">CustomerID</span></span></td>
<td><p><span data-ttu-id="72ca2-407">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="72ca2-407">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
<td><span data-ttu-id="72ca2-408">ORDDC52E52FDEF405786F0642DD0108BE4</span><span class="sxs-lookup"><span data-stu-id="72ca2-408">ORDDC52E52FDEF405786F0642DD0108BE4</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-409">DomainName</span><span class="sxs-lookup"><span data-stu-id="72ca2-409">DomainName</span></span></td>
<td><p><span data-ttu-id="72ca2-410">Nombre&#39;de dominio del cliente, que se usa para ayudar a identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="72ca2-410">Customer&#39;s domain name, used to help identify the customer.</span></span> <span data-ttu-id="72ca2-411">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-411">This field may appear blank until the second billing cycle.</span></span></p></td>
<td><span data-ttu-id="72ca2-412">ejemplo.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="72ca2-412">example.onmicrosoft.com</span></span></td></tr>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-413">Unidad</span><span class="sxs-lookup"><span data-stu-id="72ca2-413">Unit</span></span></td>
<td><p><span data-ttu-id="72ca2-414">La unidad del nombre del recurso</span><span class="sxs-lookup"><span data-stu-id="72ca2-414">The unit of the resource Name</span></span></p></td>
<td><span data-ttu-id="72ca2-415">GB u HORAS</span><span class="sxs-lookup"><span data-stu-id="72ca2-415">GB or HOURS</span></span></td>
</tr>
</tbody>
</table>

## <a href="" id="marketplacefilefields"></a><span data-ttu-id="72ca2-416">Campos de archivo de una sola vez y periódicos</span><span class="sxs-lookup"><span data-stu-id="72ca2-416">One-time and recurring file fields</span></span>

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="72ca2-417">Column</span><span class="sxs-lookup"><span data-stu-id="72ca2-417">Column</span></span></th>
<th><span data-ttu-id="72ca2-418">Descripción</span><span class="sxs-lookup"><span data-stu-id="72ca2-418">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="72ca2-419">PartnerId</span><span class="sxs-lookup"><span data-stu-id="72ca2-419">PartnerId</span></span></td>
<td><p><span data-ttu-id="72ca2-420">Identificador único del inquilino de Microsoft Azure Active Directory para una entidad de facturación específica, en formato GUID.</span><span class="sxs-lookup"><span data-stu-id="72ca2-420">Unique Microsoft Azure Active Directory tenant identifier for a specific billing entity, in GUID format.</span></span> <span data-ttu-id="72ca2-421">No es necesario para la reconciliación, pero puede ser información útil.</span><span class="sxs-lookup"><span data-stu-id="72ca2-421">Not required for reconciliation, however may be useful information.</span></span> <span data-ttu-id="72ca2-422">Igual en todas las filas.</span><span class="sxs-lookup"><span data-stu-id="72ca2-422">Same in all rows.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-423">Identificador de cliente</span><span class="sxs-lookup"><span data-stu-id="72ca2-423">Customer Id</span></span></td>
<td><p><span data-ttu-id="72ca2-424">IDENTIFICADOR único del inquilino de Microsoft Azure Active Directory, en formato GUID, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="72ca2-424">Unique Microsoft Azure Active Directory tenant ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-425">Nombre del cliente</span><span class="sxs-lookup"><span data-stu-id="72ca2-425">Customer Name</span></span></td>
<td><p><span data-ttu-id="72ca2-426">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="72ca2-426">Customer's organization name as reported in Partner Center.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-427">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="72ca2-427">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="72ca2-428">Nombre de dominio del cliente, que se usa para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="72ca2-428">Customer's domain name, used to help identify the customer.</span></span> <span data-ttu-id="72ca2-429">No debe usarse para identificar de forma exclusiva al cliente como cliente o asociado puede actualizar el dominio de cortesía/predeterminado mediante el portal de O365.</span><span class="sxs-lookup"><span data-stu-id="72ca2-429">This should not be used to uniquely identify the customer as the customer/partner can update the vanity/default domain via the O365 portal.</span></span> <span data-ttu-id="72ca2-430">Este campo puede aparecer en blanco hasta el segundo ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-430">This field may appear blank until the second billing cycle.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-431">País del cliente</span><span class="sxs-lookup"><span data-stu-id="72ca2-431">Customer Country</span></span></td>
<td><p><span data-ttu-id="72ca2-432">El país donde se encuentra el cliente.</span><span class="sxs-lookup"><span data-stu-id="72ca2-432">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-433">Número de factura</span><span class="sxs-lookup"><span data-stu-id="72ca2-433">Invoice number</span></span></td>
<td><p><span data-ttu-id="72ca2-434">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="72ca2-434">Invoice number where the specified transaction appears.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-435">MpnId</span><span class="sxs-lookup"><span data-stu-id="72ca2-435">MpnId</span></span></td>
<td><p><span data-ttu-id="72ca2-436">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="72ca2-436">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-437">Reseller MpnId</span><span class="sxs-lookup"><span data-stu-id="72ca2-437">Reseller MpnId</span></span></td>
<td><p><span data-ttu-id="72ca2-438">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="72ca2-438">MPN ID of the reseller of record for the subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-439">Id. de pedido</span><span class="sxs-lookup"><span data-stu-id="72ca2-439">Order ID</span></span></td>
<td><p><span data-ttu-id="72ca2-440">Identificador único para un pedido en la plataforma de comercio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="72ca2-440">Unique identifier for an order in the Microsoft commerce platform.</span></span> <span data-ttu-id="72ca2-441">Puede ser útil para identificar al pedido al ponerse en contacto con el soporte técnico, pero no para la conciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-441">May be useful to identify the order when contacting support but not for reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-442">Fecha del pedido</span><span class="sxs-lookup"><span data-stu-id="72ca2-442">Order date</span></span></td>
<td><p><span data-ttu-id="72ca2-443">Fecha de realización del pedido.</span><span class="sxs-lookup"><span data-stu-id="72ca2-443">The date the order was placed.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-444">ProductId</span><span class="sxs-lookup"><span data-stu-id="72ca2-444">ProductId</span></span></td>
<td><p><span data-ttu-id="72ca2-445">Identificador del producto.</span><span class="sxs-lookup"><span data-stu-id="72ca2-445">The ID for the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-446">SkuId</span><span class="sxs-lookup"><span data-stu-id="72ca2-446">SkuId</span></span></td>
<td><p><span data-ttu-id="72ca2-447">Id. de un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="72ca2-447">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-448">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="72ca2-448">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="72ca2-449">Id. de una disponibilidad concreta.</span><span class="sxs-lookup"><span data-stu-id="72ca2-449">The ID for a particular Availability.</span></span> <span data-ttu-id="72ca2-450">"Disponibilidad" se refiere a si una SKU determinada está disponible para su compra en el país, la moneda, el segmento del sector, etc.</span><span class="sxs-lookup"><span data-stu-id="72ca2-450">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-451">Nombre de SKU</span><span class="sxs-lookup"><span data-stu-id="72ca2-451">SKU Name</span></span></td>
<td><p><span data-ttu-id="72ca2-452">Título para un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="72ca2-452">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-453">Nombre del producto</span><span class="sxs-lookup"><span data-stu-id="72ca2-453">Product name</span></span></td>
<td><p><span data-ttu-id="72ca2-454">Nombre del producto.</span><span class="sxs-lookup"><span data-stu-id="72ca2-454">The name of the product.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-455">PublisherName</span><span class="sxs-lookup"><span data-stu-id="72ca2-455">PublisherName</span></span></td>
<td><p><span data-ttu-id="72ca2-456">Nombre del publicador del producto.</span><span class="sxs-lookup"><span data-stu-id="72ca2-456">The name of the product's publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-457">PublisherID</span><span class="sxs-lookup"><span data-stu-id="72ca2-457">PublisherID</span></span></td>
<td><p><span data-ttu-id="72ca2-458">IDENTIFICADOR único para este publicador.</span><span class="sxs-lookup"><span data-stu-id="72ca2-458">Unique ID for this publisher.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-459">Descripción de la suscripción</span><span class="sxs-lookup"><span data-stu-id="72ca2-459">Subscription Description</span></span></td>
<td><p><span data-ttu-id="72ca2-460">Nombre descriptivo de una suscripción.</span><span class="sxs-lookup"><span data-stu-id="72ca2-460">Friendly name of a subscription.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-461">Id. de la suscripción</span><span class="sxs-lookup"><span data-stu-id="72ca2-461">Subscription ID</span></span></td>
<td><p><span data-ttu-id="72ca2-462">Identificador único de una suscripción en la plataforma de comercio de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="72ca2-462">Unique identifier for a subscription in the Microsoft commerce platform.</span></span> <span data-ttu-id="72ca2-463">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-463">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="72ca2-464">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="72ca2-464">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-465">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="72ca2-465">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="72ca2-466">Día de inicio de los cargos.</span><span class="sxs-lookup"><span data-stu-id="72ca2-466">Start day of the charges.</span></span> <span data-ttu-id="72ca2-467">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="72ca2-467">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-468">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="72ca2-468">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="72ca2-469">Día de finalización de los cargos.</span><span class="sxs-lookup"><span data-stu-id="72ca2-469">End day of the charges.</span></span> <span data-ttu-id="72ca2-470">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="72ca2-470">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-471">Term y Billingcycle</span><span class="sxs-lookup"><span data-stu-id="72ca2-471">Term and Billingcycle</span></span></td>
<td><p><span data-ttu-id="72ca2-472">La duración del período y el ciclo de facturación de la compra.</span><span class="sxs-lookup"><span data-stu-id="72ca2-472">The term length and billing cycle for the purchase.</span></span> <span data-ttu-id="72ca2-473">Por ejemplo, "1 año, mensualmente".</span><span class="sxs-lookup"><span data-stu-id="72ca2-473">For example, “1 Year, Monthly."</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-474">Tipo de cargo</span><span class="sxs-lookup"><span data-stu-id="72ca2-474">Charge Type</span></span></td>
<td><p><span data-ttu-id="72ca2-475">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="72ca2-475">The type of charge or adjustment.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-476">Precio unitario</span><span class="sxs-lookup"><span data-stu-id="72ca2-476">Unit Price</span></span></td>
<td><p><span data-ttu-id="72ca2-477">El precio publicado en el pricelist en el momento de la compra.</span><span class="sxs-lookup"><span data-stu-id="72ca2-477">The price as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="72ca2-478">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-478">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-479">Precio unitario efectivo</span><span class="sxs-lookup"><span data-stu-id="72ca2-479">Effective Unit Price</span></span></td>
<td><p><span data-ttu-id="72ca2-480">Precio unitario tras realizar los ajustes.</span><span class="sxs-lookup"><span data-stu-id="72ca2-480">The unit price after adjustments have been made.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-481">Cantidad</span><span class="sxs-lookup"><span data-stu-id="72ca2-481">Quantity</span></span></td>
<td><p><span data-ttu-id="72ca2-482">Número de unidades.</span><span class="sxs-lookup"><span data-stu-id="72ca2-482">Number of units.</span></span> <span data-ttu-id="72ca2-483">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-483">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-484">Tipo de unidad</span><span class="sxs-lookup"><span data-stu-id="72ca2-484">Unit type</span></span></td>
<td><p><span data-ttu-id="72ca2-485">Tipo de unidad que se va a adquirir.</span><span class="sxs-lookup"><span data-stu-id="72ca2-485">The type of unit being purchased.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-486">PriceAdjustmentDescription</span><span class="sxs-lookup"><span data-stu-id="72ca2-486">PriceAdjustmentDescription</span></span></td>
<td><p><span data-ttu-id="72ca2-487">Explicación de cualquier descuento aplicable.</span><span class="sxs-lookup"><span data-stu-id="72ca2-487">An explanation of any applicable discount.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-488">Subtotal</span><span class="sxs-lookup"><span data-stu-id="72ca2-488">Sub Total</span></span></td>
<td><p><span data-ttu-id="72ca2-489">Total sin impuestos.</span><span class="sxs-lookup"><span data-stu-id="72ca2-489">Total before tax.</span></span> <span data-ttu-id="72ca2-490">Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento.</span><span class="sxs-lookup"><span data-stu-id="72ca2-490">Checks that your subtotal matches your expected total, in case of a discount.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-491">Total de impuestos</span><span class="sxs-lookup"><span data-stu-id="72ca2-491">Tax Total</span></span></td>
<td><p><span data-ttu-id="72ca2-492">Cargo por importe de impuestos, en función de las reglas fiscales de tu mercado y las circunstancias específicas.</span><span class="sxs-lookup"><span data-stu-id="72ca2-492">Tax amount charge, based on your market's tax rules and specific circumstances.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-493">Total</span><span class="sxs-lookup"><span data-stu-id="72ca2-493">Total</span></span></td>
<td><p><span data-ttu-id="72ca2-494">Total con impuestos.</span><span class="sxs-lookup"><span data-stu-id="72ca2-494">Total after tax.</span></span> <span data-ttu-id="72ca2-495">Comprueba si se cobran impuestos en la factura.</span><span class="sxs-lookup"><span data-stu-id="72ca2-495">Checks if you are charged tax in the invoice.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-496">Moneda</span><span class="sxs-lookup"><span data-stu-id="72ca2-496">Currency</span></span></td>
<td><p><span data-ttu-id="72ca2-497">Tipo de moneda.</span><span class="sxs-lookup"><span data-stu-id="72ca2-497">Currency type.</span></span> <span data-ttu-id="72ca2-498">Cada entidad de facturación tiene una sola moneda.</span><span class="sxs-lookup"><span data-stu-id="72ca2-498">Each billing entity has only one currency.</span></span> <span data-ttu-id="72ca2-499">Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-499">Check that it matches your first invoice and then after any major billing platform update.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-500">AlternateID</span><span class="sxs-lookup"><span data-stu-id="72ca2-500">AlternateID</span></span></td>
<td><p><span data-ttu-id="72ca2-501">Un identificador alternativo a un identificador de pedido.</span><span class="sxs-lookup"><span data-stu-id="72ca2-501">An alternate identifier to an order ID.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-502">BillingFrequency</span><span class="sxs-lookup"><span data-stu-id="72ca2-502">BillingFrequency</span></span></td>
<td><p> <span data-ttu-id="72ca2-503">Muestra mensualmente cuando se habilita la facturación mensual.</span><span class="sxs-lookup"><span data-stu-id="72ca2-503">Displays monthly when monthly billing is enabled.</span></span> <span data-ttu-id="72ca2-504">En caso contrario, en blanco.</span><span class="sxs-lookup"><span data-stu-id="72ca2-504">Otherwise blank.</span></span> </p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-505">BillableQuantity</span><span class="sxs-lookup"><span data-stu-id="72ca2-505">BillableQuantity</span></span></td>
<td><p> <span data-ttu-id="72ca2-506">Representa el total de unidades adquiridas o consumidas.</span><span class="sxs-lookup"><span data-stu-id="72ca2-506">Represents the total units purchased or consumed.</span></span> </p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-507">PricingCurrency</span><span class="sxs-lookup"><span data-stu-id="72ca2-507">PricingCurrency</span></span></td>
<td><p> <span data-ttu-id="72ca2-508">Muestra el precio del recurso u oferta</span><span class="sxs-lookup"><span data-stu-id="72ca2-508">Lists the price for resource or offer</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-509">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="72ca2-509">PCToBCExchangeRate</span></span> </td>
<td><p> <span data-ttu-id="72ca2-510">Tasa de cambio aplicada para la moneda de facturación (clientes) de precios</span><span class="sxs-lookup"><span data-stu-id="72ca2-510">Exchange rate applied for pricing currency to (customers) billing currency</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-511">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="72ca2-511">PCToBCExchangeRateDate</span></span> </td>
<td><p> <span data-ttu-id="72ca2-512">Fecha en la que se determina la tasa de cambio de moneda de facturación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-512">Date at which pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-513">MeterDescription</span><span class="sxs-lookup"><span data-stu-id="72ca2-513">MeterDescription</span></span> </td>
<td><p> <span data-ttu-id="72ca2-514">Descripción del medidor para el artículo de línea de consumo</span><span class="sxs-lookup"><span data-stu-id="72ca2-514">Meter description for consumption line item</span></span></p></td>
</tr>
</tbody>
</table>


## <a href="" id="dailyratedusagefields"></a><span data-ttu-id="72ca2-515">Campos de archivo de uso con clasificación diaria</span><span class="sxs-lookup"><span data-stu-id="72ca2-515">Daily-rated usage file fields</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="72ca2-516">Column</span><span class="sxs-lookup"><span data-stu-id="72ca2-516">Column</span></span></th>
<th><span data-ttu-id="72ca2-517">Descripción</span><span class="sxs-lookup"><span data-stu-id="72ca2-517">Description</span></span></th>
</tr>
</thead>
<tbody>

<tr class="odd">
<td><span data-ttu-id="72ca2-518">PartnerId</span><span class="sxs-lookup"><span data-stu-id="72ca2-518">PartnerId</span></span></td>
<td><p><span data-ttu-id="72ca2-519">Id. de partner, en formato de GUID.</span><span class="sxs-lookup"><span data-stu-id="72ca2-519">Partner ID, in GUID format.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-520">PartnerName</span><span class="sxs-lookup"><span data-stu-id="72ca2-520">PartnerName</span></span></td>
<td><p><span data-ttu-id="72ca2-521">Nombre del partner.</span><span class="sxs-lookup"><span data-stu-id="72ca2-521">Partner Name.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-522">CustomerId</span><span class="sxs-lookup"><span data-stu-id="72ca2-522">CustomerId</span></span></td>
<td><p><span data-ttu-id="72ca2-523">Id. de Microsoft único, en formato GUID, usado para identificar al cliente.</span><span class="sxs-lookup"><span data-stu-id="72ca2-523">Unique Microsoft ID, in GUID format, used to identify the customer.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-524">CustomerCompanyName</span><span class="sxs-lookup"><span data-stu-id="72ca2-524">CustomerCompanyName</span></span></td>
<td><p><span data-ttu-id="72ca2-525">Nombre de la organización del cliente según se indica en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="72ca2-525">Customer's organization name as reported in Partner Center.</span></span> <span data-ttu-id="72ca2-526">Esto es muy importante para conciliar la factura con la información del sistema.</span><span class="sxs-lookup"><span data-stu-id="72ca2-526">This is very important for reconciling the invoice with your system information.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-527">CustomerDomainName</span><span class="sxs-lookup"><span data-stu-id="72ca2-527">CustomerDomainName</span></span></td>
<td><p><span data-ttu-id="72ca2-528">El nombre de dominio del cliente.</span><span class="sxs-lookup"><span data-stu-id="72ca2-528">The customer's domain name.</span></span> <span data-ttu-id="72ca2-529">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="72ca2-529">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-530">País del cliente</span><span class="sxs-lookup"><span data-stu-id="72ca2-530">Customer country</span></span></td>
<td><p><span data-ttu-id="72ca2-531">El país donde se encuentra el cliente.</span><span class="sxs-lookup"><span data-stu-id="72ca2-531">The country in which the customer is located.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-532">MPNID</span><span class="sxs-lookup"><span data-stu-id="72ca2-532">MPNID</span></span></td>
<td><p><span data-ttu-id="72ca2-533">Id. de MPN del partner CSP.</span><span class="sxs-lookup"><span data-stu-id="72ca2-533">MPN ID of the CSP partner.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-534">Reseller MPNID</span><span class="sxs-lookup"><span data-stu-id="72ca2-534">Reseller MPNID</span></span></td>
<td><p><span data-ttu-id="72ca2-535">Id. de MPN del revendedor de registro de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="72ca2-535">MPN ID of the reseller of record for the subscription.</span></span> <span data-ttu-id="72ca2-536">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="72ca2-536">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-537">InvoiceNumber</span><span class="sxs-lookup"><span data-stu-id="72ca2-537">InvoiceNumber</span></span></td>
<td><p><span data-ttu-id="72ca2-538">Número de factura donde aparece la transacción especificada.</span><span class="sxs-lookup"><span data-stu-id="72ca2-538">Invoice number where the specified transaction appears.</span></span> <span data-ttu-id="72ca2-539">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="72ca2-539">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-540">ProductId</span><span class="sxs-lookup"><span data-stu-id="72ca2-540">ProductId</span></span></td>
<td><p><span data-ttu-id="72ca2-541">Identificador del producto.</span><span class="sxs-lookup"><span data-stu-id="72ca2-541">The ID for the product.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-542">SkuId</span><span class="sxs-lookup"><span data-stu-id="72ca2-542">SkuId</span></span></td>
<td><p><span data-ttu-id="72ca2-543">Id. de un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="72ca2-543">The ID for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-544">AvailabilityId</span><span class="sxs-lookup"><span data-stu-id="72ca2-544">AvailabilityId</span></span></td>
<td><p><span data-ttu-id="72ca2-545">Id. de una disponibilidad concreta.</span><span class="sxs-lookup"><span data-stu-id="72ca2-545">The ID for a particular Availability.</span></span> <span data-ttu-id="72ca2-546">"Disponibilidad" se refiere a si una SKU determinada está disponible para su compra en el país, la moneda, el segmento del sector, etc.</span><span class="sxs-lookup"><span data-stu-id="72ca2-546">“Availability" refers to whether or not a particular SKU is available for purchase for the given country, currency, industry segment, etc.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-547">Nombre de SKU</span><span class="sxs-lookup"><span data-stu-id="72ca2-547">SKU Name</span></span></td>
<td><p><span data-ttu-id="72ca2-548">Título para un SKU concreto.</span><span class="sxs-lookup"><span data-stu-id="72ca2-548">The title for a particular SKU.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-549">PublisherName</span><span class="sxs-lookup"><span data-stu-id="72ca2-549">PublisherName</span></span></td>
<td><p><span data-ttu-id="72ca2-550">Nombre del publicador.</span><span class="sxs-lookup"><span data-stu-id="72ca2-550">The name of the publisher.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-551">PublisherID</span><span class="sxs-lookup"><span data-stu-id="72ca2-551">PublisherID</span></span></td>
<td><p><span data-ttu-id="72ca2-552">IDENTIFICADOR del publicador, en formato GUID.</span><span class="sxs-lookup"><span data-stu-id="72ca2-552">The ID of the publisher, in GUID format.</span></span> <span data-ttu-id="72ca2-553">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="72ca2-553">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-554">Descripción de la suscripción</span><span class="sxs-lookup"><span data-stu-id="72ca2-554">Subscription Description</span></span></td>
<td><p><span data-ttu-id="72ca2-555">Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="72ca2-555">The name of the service offering purchased by the customer, as defined in the price list.</span></span> <span data-ttu-id="72ca2-556">(Este es un campo idéntico al nombre de la oferta).</span><span class="sxs-lookup"><span data-stu-id="72ca2-556">(This is an identical field to Offer name).</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-557">Id. de la suscripción</span><span class="sxs-lookup"><span data-stu-id="72ca2-557">Subscription ID</span></span></td>
<td><p><span data-ttu-id="72ca2-558">Identificador único de una suscripción en la plataforma de facturación de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="72ca2-558">Unique identifier for a subscription in the Microsoft billing platform.</span></span> <span data-ttu-id="72ca2-559">Puede ser útil para identificar a la suscripción al ponerse en contacto con el soporte técnico, pero no para la reconciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-559">May be useful to identify the subscription when contacting support but not for reconciliation.</span></span> <span data-ttu-id="72ca2-560">No es el mismo que el identificador de suscripción en la consola de administración de partners.</span><span class="sxs-lookup"><span data-stu-id="72ca2-560">This is not the same as the Subscription ID on the Partner Admin Console.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-561">ChargeStartDate</span><span class="sxs-lookup"><span data-stu-id="72ca2-561">ChargeStartDate</span></span></td>
<td><p><span data-ttu-id="72ca2-562">Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="72ca2-562">Start date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="72ca2-563">La hora siempre corresponde al comienzo del día, 0:00.</span><span class="sxs-lookup"><span data-stu-id="72ca2-563">The time is always the beginning of the day, 0:00.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-564">ChargeEndDate</span><span class="sxs-lookup"><span data-stu-id="72ca2-564">ChargeEndDate</span></span></td>
<td><p><span data-ttu-id="72ca2-565">Fecha de finalización del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latentes no cargados previamente (del ciclo de facturación anterior).</span><span class="sxs-lookup"><span data-stu-id="72ca2-565">End date of billing cycle except when presenting dates of previously uncharged latent usage data (from previous bill cycle).</span></span> <span data-ttu-id="72ca2-566">La hora siempre corresponde al fin del día, 23:59.</span><span class="sxs-lookup"><span data-stu-id="72ca2-566">The time is always the end of the day, 23:59.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-567">Fecha de uso</span><span class="sxs-lookup"><span data-stu-id="72ca2-567">Usage Date</span></span></td>
<td><p><span data-ttu-id="72ca2-568">Fecha del uso del servicio.</span><span class="sxs-lookup"><span data-stu-id="72ca2-568">Date of service usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-569">Tipo de medidor</span><span class="sxs-lookup"><span data-stu-id="72ca2-569">Meter Type</span></span></td>
<td><p><span data-ttu-id="72ca2-570">Tipo de medidor.</span><span class="sxs-lookup"><span data-stu-id="72ca2-570">The type of meter.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-571">Categoría de medidor</span><span class="sxs-lookup"><span data-stu-id="72ca2-571">Meter Category</span></span></td>
<td><p><span data-ttu-id="72ca2-572">El servicio de nivel superior para el uso.</span><span class="sxs-lookup"><span data-stu-id="72ca2-572">The top-level service for the usage.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-573">ID. de medidor</span><span class="sxs-lookup"><span data-stu-id="72ca2-573">Meter Id</span></span></td>
<td><p><span data-ttu-id="72ca2-574">IDENTIFICADOR del medidor que se está usando.</span><span class="sxs-lookup"><span data-stu-id="72ca2-574">The ID for the meter being used.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-575">Subcategoría de medidor</span><span class="sxs-lookup"><span data-stu-id="72ca2-575">Meter Sub-category</span></span></td>
<td><p><span data-ttu-id="72ca2-576">El tipo de servicio de Azure que puede afectar a la tarifa.</span><span class="sxs-lookup"><span data-stu-id="72ca2-576">The type of Azure service that can affect the rate.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-577">Nombre del medidor</span><span class="sxs-lookup"><span data-stu-id="72ca2-577">Meter Name</span></span></td>
<td><p><span data-ttu-id="72ca2-578">Unidad de medida del medidor que se está consumiendo.</span><span class="sxs-lookup"><span data-stu-id="72ca2-578">The unit of measure for the meter being consumed.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-579">Región de medidor</span><span class="sxs-lookup"><span data-stu-id="72ca2-579">Meter Region</span></span></td>
<td><p><span data-ttu-id="72ca2-580">Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena.</span><span class="sxs-lookup"><span data-stu-id="72ca2-580">This column identifies the location of a data center within the region for services where this is applicable and populated.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-581">Unidad</span><span class="sxs-lookup"><span data-stu-id="72ca2-581">Unit</span></span></td>
<td><p><span data-ttu-id="72ca2-582">Unidad del nombre del recurso.</span><span class="sxs-lookup"><span data-stu-id="72ca2-582">The unit of the resource Name.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-583">Cantidad consumida</span><span class="sxs-lookup"><span data-stu-id="72ca2-583">Consumed Quantity</span></span></td>
<td><p><span data-ttu-id="72ca2-584">La cantidad de servicio consumida (horas, GB, etc.) durante el período de notificación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-584">The amount of service consumed (hours, GB, etc.) during the reporting period.</span></span> <span data-ttu-id="72ca2-585">También incluye cualquier uso no facturado de períodos anteriores.</span><span class="sxs-lookup"><span data-stu-id="72ca2-585">Also includes any unbilled usage from previous reporting periods.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-586">Ubicación del recurso</span><span class="sxs-lookup"><span data-stu-id="72ca2-586">Resource Location</span></span></td>
<td><p><span data-ttu-id="72ca2-587">Centro de recursos en el que se está ejecutando el medidor.</span><span class="sxs-lookup"><span data-stu-id="72ca2-587">The datacenter where the meter is running.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-588">Servicio consumido</span><span class="sxs-lookup"><span data-stu-id="72ca2-588">Consumed Service</span></span></td>
<td><p><span data-ttu-id="72ca2-589">El servicio de la plataforma Azure que ha usado.</span><span class="sxs-lookup"><span data-stu-id="72ca2-589">The Azure platform service that you used.</span></span></p></td>
</tr>


<tr class="even">
<td><span data-ttu-id="72ca2-590">URI de recurso</span><span class="sxs-lookup"><span data-stu-id="72ca2-590">Resource URI</span></span></td>
<td><p><span data-ttu-id="72ca2-591">URI del recurso que se va a usar.</span><span class="sxs-lookup"><span data-stu-id="72ca2-591">The URI of the resource being used.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-592">Tipo de cargo</span><span class="sxs-lookup"><span data-stu-id="72ca2-592">Charge type</span></span></td>
<td><p><span data-ttu-id="72ca2-593">Tipo de cargo o ajuste.</span><span class="sxs-lookup"><span data-stu-id="72ca2-593">The type of charge or adjustment.</span></span> <span data-ttu-id="72ca2-594">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="72ca2-594">Not available for current activity.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-595">Precio unitario</span><span class="sxs-lookup"><span data-stu-id="72ca2-595">Unit price</span></span></td>
<td><p><span data-ttu-id="72ca2-596">Precio por licencia, tal y como se publica en el pricelist en el momento de la compra.</span><span class="sxs-lookup"><span data-stu-id="72ca2-596">Price per license, as published in the pricelist at the time of purchase.</span></span> <span data-ttu-id="72ca2-597">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-597">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-598">Cantidad</span><span class="sxs-lookup"><span data-stu-id="72ca2-598">Quantity</span></span></td>
<td><p><span data-ttu-id="72ca2-599">Número de licencias.</span><span class="sxs-lookup"><span data-stu-id="72ca2-599">Number of licenses.</span></span> <span data-ttu-id="72ca2-600">Asegúrate de que coincide con la información almacenada en tu sistema de facturación durante la conciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-600">Ensure this matches the information stored in your billing system during reconciliation.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-601">Tipo de unidad</span><span class="sxs-lookup"><span data-stu-id="72ca2-601">Unit type</span></span></td>
<td><p><span data-ttu-id="72ca2-602">Tipo de unidad en la que se carga el medidor.</span><span class="sxs-lookup"><span data-stu-id="72ca2-602">The type of unit the meter is charged in.</span></span> <span data-ttu-id="72ca2-603">No está disponible para la actividad actual.</span><span class="sxs-lookup"><span data-stu-id="72ca2-603">Not available for current activity.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-604">Impuesto previo de facturación</span><span class="sxs-lookup"><span data-stu-id="72ca2-604">Billing pre tax</span></span></td>
<td><p><span data-ttu-id="72ca2-605">Importe total antes de los impuestos.</span><span class="sxs-lookup"><span data-stu-id="72ca2-605">Total amount before taxes.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-606">Moneda de facturación</span><span class="sxs-lookup"><span data-stu-id="72ca2-606">Billing currency</span></span></td>
<td><p><span data-ttu-id="72ca2-607">La moneda en la región geográfica del cliente</span><span class="sxs-lookup"><span data-stu-id="72ca2-607">The currency in the customer's geographic region</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-608">Precio pretax total</span><span class="sxs-lookup"><span data-stu-id="72ca2-608">Pricing pretax total</span></span></td>
<td><p><span data-ttu-id="72ca2-609">Los precios antes de que se agreguen los impuestos.</span><span class="sxs-lookup"><span data-stu-id="72ca2-609">The pricing before taxes are added.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-610">Moneda de precios</span><span class="sxs-lookup"><span data-stu-id="72ca2-610">Pricing currency</span></span></td>
<td><p><span data-ttu-id="72ca2-611">La moneda en el pricelist.</span><span class="sxs-lookup"><span data-stu-id="72ca2-611">The currency in the pricelist.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-612">Información de servicio 1</span><span class="sxs-lookup"><span data-stu-id="72ca2-612">Service Info 1</span></span></td>
<td><p><span data-ttu-id="72ca2-613">Número de conexiones de Bus de servicio aprovisionadas y usadas en un día determinado.</span><span class="sxs-lookup"><span data-stu-id="72ca2-613">The number of ServiceBus connections that were provisioned and utilized on a given day.</span></span></p></td>
</tr>

<tr class="even">
<td><span data-ttu-id="72ca2-614">Información de servicio 2</span><span class="sxs-lookup"><span data-stu-id="72ca2-614">Service Info 2</span></span></td>
<td><p><span data-ttu-id="72ca2-615">Campo heredado que captura los metadatos específicos del servicio opcionales.</span><span class="sxs-lookup"><span data-stu-id="72ca2-615">A legacy field that captures optional service-specific metadata.</span></span></p></td>
</tr>

<tr class="odd">
<td><span data-ttu-id="72ca2-616">Información adicional</span><span class="sxs-lookup"><span data-stu-id="72ca2-616">Additional Info</span></span></td>
<td><p><span data-ttu-id="72ca2-617">Cualquier información adicional no incluida en otras columnas.</span><span class="sxs-lookup"><span data-stu-id="72ca2-617">Any additional information not covered in other columns.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-618">EffectiveUnitPrice</span><span class="sxs-lookup"><span data-stu-id="72ca2-618">EffectiveUnitPrice</span></span></td>
<td><p> <span data-ttu-id="72ca2-619">Valor real que se cobra por unidad (esto incluye los descuentos, el crédito obtenido, etc.).</span><span class="sxs-lookup"><span data-stu-id="72ca2-619">Actual value charged per unit (this includes discounts, earned credit etc).</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-620">PCToBCExchangeRate</span><span class="sxs-lookup"><span data-stu-id="72ca2-620">PCToBCExchangeRate</span></span> </td>
<td><p><span data-ttu-id="72ca2-621">Tasa de cambio aplicada para la moneda de facturación (clientes) de precios.</span><span class="sxs-lookup"><span data-stu-id="72ca2-621">Exchange rate applied for pricing currency to (customers) billing currency.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-622">PCToBCExchangeRateDate</span><span class="sxs-lookup"><span data-stu-id="72ca2-622">PCToBCExchangeRateDate</span></span> </td>
<td><p><span data-ttu-id="72ca2-623">Fecha en la que se determina la tasa de cambio de moneda de facturación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-623">Date at which the pricing currency to billing currency exchange rate is determined.</span></span></p></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="72ca2-624">EntitlementID</span><span class="sxs-lookup"><span data-stu-id="72ca2-624">EntitlementID</span></span></td>
<td><p><span data-ttu-id="72ca2-625">Representa subscriptionID de Azure.</span><span class="sxs-lookup"><span data-stu-id="72ca2-625">Represents Azure subscriptionID.</span></span></p></td>
</tr>
<tr class="even">
<td><span data-ttu-id="72ca2-626">EntitlementDescription</span><span class="sxs-lookup"><span data-stu-id="72ca2-626">EntitlementDescription</span></span></td>
<td><p><span data-ttu-id="72ca2-627">Representa el nombre de la suscripción de Azure.</span><span class="sxs-lookup"><span data-stu-id="72ca2-627">Represents name of Azure subscription.</span></span></p></td>
</tr>

</tbody>
</table>


## <a href="" id="charge_types"></a><span data-ttu-id="72ca2-628">Asignación de cargos entre una factura y el archivo de conciliación</span><span class="sxs-lookup"><span data-stu-id="72ca2-628">Mapping charges between an invoice and the reconciliation file</span></span>

<span data-ttu-id="72ca2-629">La factura proporciona un resumen de los cargos, mientras que el archivo de conciliación proporciona un desglose detallado de las transacciones de elementos de línea, incluidos los tipos de cargo.</span><span class="sxs-lookup"><span data-stu-id="72ca2-629">Your invoice provides a summary of charges, while your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span>

<span data-ttu-id="72ca2-630">Para hacer referencias cruzadas de cantidades de cargos entre el archivo de conciliación y la factura, puedes usar las opciones de filtro de Microsoft Excel para filtrar por tipo de cargo en el archivo de conciliación con el fin de asignar los cargos de facturación a un conjunto de desgloses de cargos del archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-630">To cross-reference charge amounts between the invoice and reconciliation file, you can use Microsoft Excel's filter options to filter by charge types on the reconciliation file to map the invoice charges to a set of charge breakdowns on reconciliation file.</span></span>

<span data-ttu-id="72ca2-631">Los archivos de conciliación, tanto basados en uso como en licencias, solo muestran cargos y transacciones relacionados con el uso (unidades consumidas y cargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="72ca2-631">Reconciliation files, both usage- and license-based, only show usage related transactions and charges (units consumed and related charges).</span></span> <span data-ttu-id="72ca2-632">No se muestran en el archivo de conciliación los créditos, los descuentos o los reembolsos que aparecen en la factura como "ajustes".</span><span class="sxs-lookup"><span data-stu-id="72ca2-632">One off credits, discounts or refunds which appear on the invoice as “Adjustments" are not shown in the reconciliation file.</span></span>

<span data-ttu-id="72ca2-633">La siguiente tabla muestra las asignaciones entre una sección de factura y los tipos de cargo asociados que es posible que se muestren en los archivos de conciliación.</span><span class="sxs-lookup"><span data-stu-id="72ca2-633">The table below shows the mappings between an invoice section and associated charge types that might show up on the reconciliation files.</span></span> 

<table>
<tbody>
<tr>
<td>
<p><span data-ttu-id="72ca2-634"><strong>Descripción del cargo de la factura</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-634"><strong>Invoice charge description</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-635"><strong>Descripción del cargo del archivo de conciliación (columna ChargeType)</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-635"><strong>Reconciliation file charge description (ChargeType column)</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-636"><strong>¿Qué es este cargo?</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-636"><strong>What is this charge?</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-637"><strong>Cómo asignar estos ChargeTypes a la factura?</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-637"><strong>How do I map these ChargeTypes to the invoice?</strong></span></span></p>
</td>
</tr>
<tr>
<td rowspan="10">
<p><span data-ttu-id="72ca2-638"><strong>Cargos basados en licencias</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-638"><strong>License-based charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-639">Tarifa de activación</span><span class="sxs-lookup"><span data-stu-id="72ca2-639">Activation fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-640">El importe cobrado al cliente cuando usa la suscripción después de adquirirla</span><span class="sxs-lookup"><span data-stu-id="72ca2-640">The amount charged to the customer when they use the subscription after purchasing it</span></span></p>
</td>
<td rowspan="10">
<p><span data-ttu-id="72ca2-641">Desde el archivo basado en licencia, suma la columna <strong>Amount</strong>.</span><span class="sxs-lookup"><span data-stu-id="72ca2-641">From license-based file, sum the <strong>Amount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-642">Cuota de cancelación</span><span class="sxs-lookup"><span data-stu-id="72ca2-642">Cancel fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-643">Cargos prorrateados reembolsados al cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="72ca2-643">Prorated charges refunded to the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-644">Tarifa de ciclo</span><span class="sxs-lookup"><span data-stu-id="72ca2-644">Cycle fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-645">Cargos periódicos de una suscripción</span><span class="sxs-lookup"><span data-stu-id="72ca2-645">Periodic charges for a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-646">Prorrateo de instancia de ciclo</span><span class="sxs-lookup"><span data-stu-id="72ca2-646">Cycle instance prorate</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-647">Cargos prorrateados evaluados del cliente al cambiar los puestos asociados</span><span class="sxs-lookup"><span data-stu-id="72ca2-647">Prorated charges assessed from the customer when associated seats are changed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-648">Tarifas prorrateadas al cancelar</span><span class="sxs-lookup"><span data-stu-id="72ca2-648">Prorate fees when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-649">Reembolso prorrateado de la parte no usada del servicio tras la cancelación</span><span class="sxs-lookup"><span data-stu-id="72ca2-649">Prorated refund for unused portion of service upon cancellation</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-650">Tarifas prorrateadas al comprar</span><span class="sxs-lookup"><span data-stu-id="72ca2-650">Prorate fees when purchase</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-651">El tipo de cargo de una suscripción cuando se usa la facturación anual</span><span class="sxs-lookup"><span data-stu-id="72ca2-651">The charge type for a subscription when using annual billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-652">Tarifa de compra</span><span class="sxs-lookup"><span data-stu-id="72ca2-652">Purchase fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-653">El tipo de cargo de una suscripción cuando se usa la facturación mensual</span><span class="sxs-lookup"><span data-stu-id="72ca2-653">The charge type for a subscription when using monthly billing</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-654">Tarifa prorrateada al renovar</span><span class="sxs-lookup"><span data-stu-id="72ca2-654">Prorate fee when renew</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-655">Tarifas prorrateadas tras la renovación de la suscripción</span><span class="sxs-lookup"><span data-stu-id="72ca2-655">Prorated fees upon subscription renewal</span></span></p>
</td>
</tr>
<tr>

<td>
<p><span data-ttu-id="72ca2-656">Tarifa de renovación</span><span class="sxs-lookup"><span data-stu-id="72ca2-656">Renew fee</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-657">Cargo por renovar una suscripción</span><span class="sxs-lookup"><span data-stu-id="72ca2-657">Charge for renewing a subscription</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-658">Tarifas prorrateadas al activar</span><span class="sxs-lookup"><span data-stu-id="72ca2-658">Prorate fees when activate</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-659">Tarifas prorrateadas desde la activación hasta el final del período de facturación</span><span class="sxs-lookup"><span data-stu-id="72ca2-659">Prorated fees from activation until end of billing period</span></span></p>
</td>
</tr>



<tr>
<td rowspan="5">
<p><span data-ttu-id="72ca2-660"><strong>Cargos por única vez</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-660"><strong>One-time Charges</strong></span></span></p>

</td>
<td>
<p><span data-ttu-id="72ca2-661">Nuevo</span><span class="sxs-lookup"><span data-stu-id="72ca2-661">New</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-662">Se usa cuando se crea una nueva compra</span><span class="sxs-lookup"><span data-stu-id="72ca2-662">Used when a new purchase is created</span></span></p>
</td>

<p></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-663">addQuantity</span><span class="sxs-lookup"><span data-stu-id="72ca2-663">addQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-664">Se usa tanto en el reembolso de la compra original como en la nueva cantidad después del aumento</span><span class="sxs-lookup"><span data-stu-id="72ca2-664">Used in both the refund of the original purchase and the new quantity after increase</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-665">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="72ca2-665">removeQuantity</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-666">Se usa tanto en el reembolso de la compra original como en la nueva cantidad después de la disminución.</span><span class="sxs-lookup"><span data-stu-id="72ca2-666">Used in both the refund of the original purchase and the new quantity after decrease</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-667">Cancelar</span><span class="sxs-lookup"><span data-stu-id="72ca2-667">Cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-668">Se usa cuando se cancela una suscripción</span><span class="sxs-lookup"><span data-stu-id="72ca2-668">Used when a subscription is cancelled</span></span></p>
</td>
</tr>

</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-669">Conversión</span><span class="sxs-lookup"><span data-stu-id="72ca2-669">Convert</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-670">Se usa cuando se actualiza una licencia pero el número de puestos permanece inalterado.</span><span class="sxs-lookup"><span data-stu-id="72ca2-670">Used when a license is upgraded but the number of seats remains unchanged</span></span></p>
</td>
</tr>

<tr>
<td rowspan="2">
<p><span data-ttu-id="72ca2-671"><strong>Cargos de uso</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-671"><strong>Usage Charges</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-672">Evaluar la tarifa de uso al cancelar</span><span class="sxs-lookup"><span data-stu-id="72ca2-672">Assess usage fee when cancel</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-673">Tarifa de uso de acceso tras la cancelación por uso impagado durante el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="72ca2-673">Access usage fee upon cancellation for unpaid usage during the current billing period</span></span></p>
</td>
<td rowspan="2">
<p><span data-ttu-id="72ca2-674">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="72ca2-674">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-675">Evaluar la tarifa de uso para el ciclo actual</span><span class="sxs-lookup"><span data-stu-id="72ca2-675">Assess usage fee for current cycle</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-676">tarifa de uso de acceso para el período de facturación actual</span><span class="sxs-lookup"><span data-stu-id="72ca2-676">Access usage fee for the current billing period</span></span></p>
</td>
</tr>

<tr>
<td>
<p><span data-ttu-id="72ca2-677"><strong>Plaza</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-677"><strong>Credits</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-678">Desplazamiento de un elemento de línea</span><span class="sxs-lookup"><span data-stu-id="72ca2-678">Offset a line item</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-679">Reembolso parcial o total de un elemento de línea, incluidos impuestos</span><span class="sxs-lookup"><span data-stu-id="72ca2-679">Partial or whole refund to a line item, including taxes</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-680">Desde el archivo basado en licencia, suma la columna <strong>TotalForCustomer</strong>.</span><span class="sxs-lookup"><span data-stu-id="72ca2-680">From license-based file, sum the <strong>TotalForCustomer</strong> column</span></span></p>
<p><span data-ttu-id="72ca2-681">Desde el archivo basado en uso, suma la columna <strong>PostTaxTotal</strong>.</span><span class="sxs-lookup"><span data-stu-id="72ca2-681">From usage-based file, sum the <strong>PostTaxTotal</strong> column</span></span></p>
</td>
</tr>
<tr>
<td rowspan="4">
<p><span data-ttu-id="72ca2-682"><strong>Descuentos basados en el uso</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-682"><strong>Usage-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-683">Descuento de activación</span><span class="sxs-lookup"><span data-stu-id="72ca2-683">Activation discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-684">Descuento que se aplica cuando se activa la suscripción</span><span class="sxs-lookup"><span data-stu-id="72ca2-684">Discount applied when subscription activated</span></span></p>
</td>

<td rowspan="4">
<p><span data-ttu-id="72ca2-685">Desde el archivo basado en uso, suma la columna <strong>PretaxCharges</strong>.</span><span class="sxs-lookup"><span data-stu-id="72ca2-685">From usage-based file, sum the <strong>PretaxCharges</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-686">Descuento de ciclo</span><span class="sxs-lookup"><span data-stu-id="72ca2-686">Cycle discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-687">Descuento que se aplica en cargos periódicos</span><span class="sxs-lookup"><span data-stu-id="72ca2-687">Discount applied on periodic charges</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-688">Descuento de renovación</span><span class="sxs-lookup"><span data-stu-id="72ca2-688">Renew discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-689">Descuento que se aplica cuando se renueva la suscripción</span><span class="sxs-lookup"><span data-stu-id="72ca2-689">Discount applied when subscription renewed</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-690">Descuento de cancelación</span><span class="sxs-lookup"><span data-stu-id="72ca2-690">Cancel discount</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-691">Cargos que se aplican cuando se cancelan los descuentos</span><span class="sxs-lookup"><span data-stu-id="72ca2-691">Charges applied when discounts cancelled</span></span></p>
</td>
</tr>


<tr>
<td>
<p><span data-ttu-id="72ca2-692"><strong>Descuentos basados en licencias</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-692"><strong>License-based discounts</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-693"><em>Se puede aplicar a varios tipos de cargos</em></span><span class="sxs-lookup"><span data-stu-id="72ca2-693"><em>May be applied to multiple charge types</em></span></span></p>
</td>
<td>
<p></p>
</td>
<td>
<p><span data-ttu-id="72ca2-694">Desde el archivo basado en licencia, suma la columna <strong>TotalOtherDiscount</strong>.</span><span class="sxs-lookup"><span data-stu-id="72ca2-694">From license-based file, sum the <strong>TotalOtherDiscount</strong> column</span></span></p>
</td>
</tr>
<tr>
<td>
<p><span data-ttu-id="72ca2-695"><strong>Impuestos</strong>&nbsp;o&nbsp;<strong>IVA</strong></span><span class="sxs-lookup"><span data-stu-id="72ca2-695"><strong>Taxes</strong>&nbsp;or&nbsp;<strong>VAT</strong></span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-696"><em>Se puede aplicar a varios tipos de cargos</em></span><span class="sxs-lookup"><span data-stu-id="72ca2-696"><em>May be applied to multiple charge types</em></span></span></p>
<p><span data-ttu-id="72ca2-697"><em>Excepción: &quot;Offset un elemento de línea &quot; ya incluye los impuestos. Consulte créditos, arriba.</em></span><span class="sxs-lookup"><span data-stu-id="72ca2-697"><em>Exception: &quot;Offset a line item&quot; already includes taxes. See Credits, above.</em></span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-698">Impuestos o impuesto de valor añadido (IVA)</span><span class="sxs-lookup"><span data-stu-id="72ca2-698">Taxes or value-added taxes (VAT)</span></span></p>
</td>
<td>
<p><span data-ttu-id="72ca2-699">Desde el archivo basado en licencia, suma la columna <strong>Tax</strong>.</span><span class="sxs-lookup"><span data-stu-id="72ca2-699">From license-based file, sum the <strong>Tax</strong> column</span></span></p>
<p><span data-ttu-id="72ca2-700">Desde el archivo basado en uso, suma la columna <strong>TaxAmount</strong>.</span><span class="sxs-lookup"><span data-stu-id="72ca2-700">From usage-based file, sum the <strong>TaxAmount</strong> column</span></span></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>
