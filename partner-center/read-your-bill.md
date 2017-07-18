---
title: Leer factura | Centro de partners
description: "La factura mensual es un resumen de todos los cargos (incluidos el programa, los productos y los clientes) para el período mensual actual. Está disponible en el panel del Centro de partners."
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.openlocfilehash: 65c3777c0bd35933f2622fc0de105c051001974e
ms.sourcegitcommit: e8b504fa98b3ec4c7c8fd954f63ea81299791906
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/01/2017
---
# <a name="read-your-bill"></a><span data-ttu-id="853a4-104">Leer tu factura</span><span class="sxs-lookup"><span data-stu-id="853a4-104">Read your bill</span></span>

**<span data-ttu-id="853a4-105">Se aplica a</span><span class="sxs-lookup"><span data-stu-id="853a4-105">Applies to</span></span>**

-  <span data-ttu-id="853a4-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="853a4-106">Partner Center</span></span>
-  <span data-ttu-id="853a4-107">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="853a4-107">Partner Center for Microsoft Cloud for US Government</span></span>
-  <span data-ttu-id="853a4-108">Centro de partners para Microsoft Cloud Alemania</span><span class="sxs-lookup"><span data-stu-id="853a4-108">Partner Center for Microsoft Cloud Germany</span></span>

<span data-ttu-id="853a4-109">La factura mensual es un resumen de todos los cargos (incluidos el programa, los productos y los clientes) para el período mensual actual.</span><span class="sxs-lookup"><span data-stu-id="853a4-109">Your invoice is a summary of all charges (across the program, products, and customers) for the current monthly period.</span></span> <span data-ttu-id="853a4-110">Está disponible en el panel del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="853a4-110">It is available on the Partner Center Dashboard.</span></span>

<span data-ttu-id="853a4-111">Para obtener información detallada sobre los cargos, usa los archivos de conciliación correspondiente.</span><span class="sxs-lookup"><span data-stu-id="853a4-111">For itemized details about the charges, use the accompanying reconciliation files.</span></span> <span data-ttu-id="853a4-112">Los archivos de conciliación incluyen los identificadores de cliente y de suscripción que usarás para crear facturas de cliente.</span><span class="sxs-lookup"><span data-stu-id="853a4-112">The reconciliation files include the customer IDs and subscription IDs that you will use to create customer invoices.</span></span> <span data-ttu-id="853a4-113">Para obtener más información, consulta el tema sobre [cómo usar archivos de conciliación](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="853a4-113">For more information, see [How to use the reconciliation files](use-the-reconciliation-files.md).</span></span>

## <a name="invoice-file-definitions"></a><span data-ttu-id="853a4-114">Definiciones de archivo de factura</span><span class="sxs-lookup"><span data-stu-id="853a4-114">Invoice file definitions</span></span>


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong><span data-ttu-id="853a4-115">Campo</span><span class="sxs-lookup"><span data-stu-id="853a4-115">Field</span></span></strong></td>
<td><strong><span data-ttu-id="853a4-116">Descripción</span><span class="sxs-lookup"><span data-stu-id="853a4-116">Description</span></span></strong></td>
</tr>
<tr class="even">
<td><span data-ttu-id="853a4-117">US FEIN</span><span class="sxs-lookup"><span data-stu-id="853a4-117">US FEIN</span></span></td>
<td><span data-ttu-id="853a4-118">El número de identificación fiscal federal.</span><span class="sxs-lookup"><span data-stu-id="853a4-118">Your Federal Tax ID Number.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="853a4-119">Customer number</span><span class="sxs-lookup"><span data-stu-id="853a4-119">Customer number</span></span></td>
<td><span data-ttu-id="853a4-120">El número de cliente.</span><span class="sxs-lookup"><span data-stu-id="853a4-120">Your customer number.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="853a4-121">Bill to</span><span class="sxs-lookup"><span data-stu-id="853a4-121">Bill to</span></span></td>
<td><span data-ttu-id="853a4-122">La dirección a la que enviamos tu factura.</span><span class="sxs-lookup"><span data-stu-id="853a4-122">The address where we send your invoice.</span></span> <span data-ttu-id="853a4-123">Para cambiar esta dirección, edita tu perfil de cuenta del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="853a4-123">To change this address, edit your Partner Center account profile.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="853a4-124">Recurring charges</span><span class="sxs-lookup"><span data-stu-id="853a4-124">Recurring charges</span></span></td>
<td><span data-ttu-id="853a4-125">Cargos fijos mensuales (o anuales) para las licencias adquiridas basadas en el uso, facturados previamente al uso del servicio.</span><span class="sxs-lookup"><span data-stu-id="853a4-125">The flat monthly (or annual) charges for the purchased usage-based licenses, billed in advance of the service.</span></span> <span data-ttu-id="853a4-126">Este número es la suma de todos los cargos en la columna &quot;Subtotal&quot; del archivo de conciliación basada en licencia (columna T).</span><span class="sxs-lookup"><span data-stu-id="853a4-126">This number is the sum of all charges in the &quot;Subtotal&quot; column in the License-based reconciliation file (column T).</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="853a4-127">Usage charges</span><span class="sxs-lookup"><span data-stu-id="853a4-127">Usage charges</span></span></td>
<td><span data-ttu-id="853a4-128">El uso de Azure, incluidos nuevos servicios o aplicaciones habilitados y usados durante el mes de facturación.</span><span class="sxs-lookup"><span data-stu-id="853a4-128">Azure usage, including new services or applications enabled and used during the billing month.</span></span> <span data-ttu-id="853a4-129">Este número es la suma de todos los cargos en la columna &quot;PretaxCharges&quot; del archivo de conciliación basada en uso (columna Z).</span><span class="sxs-lookup"><span data-stu-id="853a4-129">This number is the sum of all charges in the &quot;PretaxCharges&quot; column in the Usage-based reconciliation file (column Z).</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="853a4-130">Créditos y ajustes</span><span class="sxs-lookup"><span data-stu-id="853a4-130">Credits &amp; adjustments</span></span></td>
<td><span data-ttu-id="853a4-131">Crédito o ajustes que corresponden a los cambios realizados en las suscripciones (por ejemplo: aumento o disminución de puestos).</span><span class="sxs-lookup"><span data-stu-id="853a4-131">Credits or adjustments for changes made to subscriptions (example: seat increases or decreases).</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="853a4-132">Other discounts</span><span class="sxs-lookup"><span data-stu-id="853a4-132">Other discounts</span></span></td>
<td><span data-ttu-id="853a4-133">Por ejemplo, el descuento que el cliente recibe del precio normal de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="853a4-133">For example, the discount that the customer receives from the normal price of the subscription.</span></span> <span data-ttu-id="853a4-134">Esto se muestra como un importe fijo, no como un precio por unidad o licencia.</span><span class="sxs-lookup"><span data-stu-id="853a4-134">This is shown as a flat amount, not as a price per unit or license.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="853a4-135">Taxes</span><span class="sxs-lookup"><span data-stu-id="853a4-135">Taxes</span></span></td>
<td><span data-ttu-id="853a4-136">El total de impuestos para los cargos actuales según se suman en la sección de detalles a partir de la página 2 de la factura.</span><span class="sxs-lookup"><span data-stu-id="853a4-136">The total tax for the current charges as totaled in the details section beginning on page 2 of the invoice.</span></span> <span data-ttu-id="853a4-137">Este número es la suma de todos los cargos de:</span><span class="sxs-lookup"><span data-stu-id="853a4-137">This number is the sum of all the charges in:</span></span>
<ul>
<li><span data-ttu-id="853a4-138">la columna &quot;TaxAmount&quot; del archivo de conciliación basada en uso (columna AA) y </span><span class="sxs-lookup"><span data-stu-id="853a4-138">the &quot;TaxAmount&quot; column of the Usage-based reconciliation file (column AA), and</span></span></li>
<li><span data-ttu-id="853a4-139">la columna &quot;Tax&quot; del archivo basado en licencia (columna U).</span><span class="sxs-lookup"><span data-stu-id="853a4-139">the &quot;Tax&quot; column of the License-based file (column U).</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="853a4-140">Total current charges</span><span class="sxs-lookup"><span data-stu-id="853a4-140">Total current charges</span></span></td>
<td><span data-ttu-id="853a4-141">El importe debido en la divisa de facturación para el período de facturación, que se debe abonar antes de la fecha de vencimiento de pago.</span><span class="sxs-lookup"><span data-stu-id="853a4-141">The amount due in your billing currency for the billing period, due by the payment due date.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="853a4-142">Payment instructions</span><span class="sxs-lookup"><span data-stu-id="853a4-142">Payment instructions</span></span></td>
<td><span data-ttu-id="853a4-143">Describe cómo pagar la factura, según de tu región.</span><span class="sxs-lookup"><span data-stu-id="853a4-143">Describes how to pay your invoice, based on your region.</span></span> <span data-ttu-id="853a4-144">Al realizar un pago, siempre incluye el número de factura.</span><span class="sxs-lookup"><span data-stu-id="853a4-144">Always include your invoice number when making a payment.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="853a4-145">Invoice no</span><span class="sxs-lookup"><span data-stu-id="853a4-145">Invoice no</span></span></td>
<td><span data-ttu-id="853a4-146">El número de la factura.</span><span class="sxs-lookup"><span data-stu-id="853a4-146">The number of your invoice.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="853a4-147">Billing period</span><span class="sxs-lookup"><span data-stu-id="853a4-147">Billing period</span></span></td>
<td><span data-ttu-id="853a4-148">A los partners de CSP se les factura mensual o anualmente.</span><span class="sxs-lookup"><span data-stu-id="853a4-148">CSP partners are billed either monthly or annually.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="853a4-149">Invoice date</span><span class="sxs-lookup"><span data-stu-id="853a4-149">Invoice date</span></span></td>
<td><span data-ttu-id="853a4-150">La fecha en la que recibes tu factura.</span><span class="sxs-lookup"><span data-stu-id="853a4-150">The date you receive your invoice.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="853a4-151">Payment due date</span><span class="sxs-lookup"><span data-stu-id="853a4-151">Payment due date</span></span></td>
<td><span data-ttu-id="853a4-152">Fecha en la que debe recibirse tu pago.</span><span class="sxs-lookup"><span data-stu-id="853a4-152">Your payment must be received by this date.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="853a4-153">Customer PO</span><span class="sxs-lookup"><span data-stu-id="853a4-153">Customer PO</span></span></td>
<td><span data-ttu-id="853a4-154">El número de pedido de compra.</span><span class="sxs-lookup"><span data-stu-id="853a4-154">Your purchase order number.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="853a4-155">Customer service</span><span class="sxs-lookup"><span data-stu-id="853a4-155">Customer service</span></span></td>
<td><span data-ttu-id="853a4-156">La dirección del sitio web para acceder al servicio de atención al cliente.</span><span class="sxs-lookup"><span data-stu-id="853a4-156">The website address to access customer service.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="853a4-157">Destinatario del servicio</span><span class="sxs-lookup"><span data-stu-id="853a4-157">Service recipient</span></span></td>
<td><span data-ttu-id="853a4-158">La dirección en la que se usa el servicio.</span><span class="sxs-lookup"><span data-stu-id="853a4-158">The address where the service is used.</span></span> <span data-ttu-id="853a4-159">(Esta es la dirección legal de la compañía asociada al control de la compañía y no se puede cambiar).</span><span class="sxs-lookup"><span data-stu-id="853a4-159">(This is the legal company address associated with company vetting and cannot be changed.)</span></span></td>
</tr>
</tbody>
</table>

 

 

 



