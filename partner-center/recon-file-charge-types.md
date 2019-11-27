---
title: Tipos de cargos de archivo de conciliación | Centro de Partners
ms.topic: article
ms.date: 08/26/2019
description: Tipos de cargos (basados en licencia, basados en el uso y único), créditos y descuentos en los archivos de conciliación del centro de Partners.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 064ed6dda28f5a8ace64942d55ef2a6327528ff5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389813"
---
# <a name="understand-charge-types"></a><span data-ttu-id="584e7-103">Descripción de los tipos de cargos</span><span class="sxs-lookup"><span data-stu-id="584e7-103">Understand charge types</span></span>

<span data-ttu-id="584e7-104">Se aplica a:</span><span class="sxs-lookup"><span data-stu-id="584e7-104">Applies to:</span></span>

- <span data-ttu-id="584e7-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="584e7-105">Partner Center</span></span>
- <span data-ttu-id="584e7-106">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="584e7-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="584e7-107">En este tema se describen las asignaciones entre una sección de factura y los tipos de cargos asociados que podrían estar en el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="584e7-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="584e7-108">La factura proporciona un resumen de los cargos.</span><span class="sxs-lookup"><span data-stu-id="584e7-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="584e7-109">El archivo de conciliación proporciona un desglose detallado de las transacciones de elementos de línea, incluidos los tipos de cargos.</span><span class="sxs-lookup"><span data-stu-id="584e7-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="584e7-110">Para obtener más información acerca de los archivos de conciliación, consulte [uso de archivos de conciliación](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="584e7-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="584e7-111">Tanto [los archivos de conciliación basados en el uso](usage-based-recon-files.md) como [los archivos de conciliación basados en licencias](license-based-recon-files.md) solo muestran las transacciones y los cargos relacionados con el uso (unidades consumidas y cargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="584e7-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="584e7-112">No se muestran en el archivo de conciliación los créditos, descuentos o reembolsos de un solo descuento que aparecen en la factura como **ajustes** .</span><span class="sxs-lookup"><span data-stu-id="584e7-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="584e7-113">Asignación de tipos de cargos a cargos de factura</span><span class="sxs-lookup"><span data-stu-id="584e7-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="584e7-114">Para hacer referencias cruzadas de los importes de los cargos entre su factura y el archivo de conciliación, use las opciones de filtro de Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="584e7-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="584e7-115">Filtre por tipos de carga en el archivo de conciliación para asignar los cargos de la factura a un conjunto de desgloses de gastos en el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="584e7-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="584e7-116">Cargos basados en licencias</span><span class="sxs-lookup"><span data-stu-id="584e7-116">License-based charges</span></span>

<span data-ttu-id="584e7-117">Para asignar estos cargos basados en licencias a la factura, sume la columna **amount** del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="584e7-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="584e7-118">Descripción de cargos (columna ChargeType en el archivo de conciliación)</span><span class="sxs-lookup"><span data-stu-id="584e7-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="584e7-119">Explicación de cargos</span><span class="sxs-lookup"><span data-stu-id="584e7-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="584e7-120">Tarifa de activación</span><span class="sxs-lookup"><span data-stu-id="584e7-120">Activation fee</span></span> | <span data-ttu-id="584e7-121">La cantidad que se cobra al cliente cuando usa la suscripción después de la compra.</span><span class="sxs-lookup"><span data-stu-id="584e7-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="584e7-122">Cuota de cancelación</span><span class="sxs-lookup"><span data-stu-id="584e7-122">Cancel fee</span></span> | <span data-ttu-id="584e7-123">Los cargos prorrateados se reembolsan al cliente cuando se cambian los puestos asociados.</span><span class="sxs-lookup"><span data-stu-id="584e7-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="584e7-124">Tarifa de ciclo</span><span class="sxs-lookup"><span data-stu-id="584e7-124">Cycle fee</span></span> | <span data-ttu-id="584e7-125">Cargos periódicos de una suscripción.</span><span class="sxs-lookup"><span data-stu-id="584e7-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="584e7-126">Prorrateo de instancia de ciclo</span><span class="sxs-lookup"><span data-stu-id="584e7-126">Cycle instance prorate</span></span> | <span data-ttu-id="584e7-127">Cargos prorrateados evaluados por el cliente cuando se cambian los puestos asociados.</span><span class="sxs-lookup"><span data-stu-id="584e7-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="584e7-128">Tarifas prorrateadas al cancelar</span><span class="sxs-lookup"><span data-stu-id="584e7-128">Prorate fees when cancel</span></span> | <span data-ttu-id="584e7-129">Reembolso prorrateado de la parte no utilizada del servicio tras la cancelación.</span><span class="sxs-lookup"><span data-stu-id="584e7-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="584e7-130">Tarifas prorrateadas al comprar</span><span class="sxs-lookup"><span data-stu-id="584e7-130">Prorate fees when purchase</span></span> | <span data-ttu-id="584e7-131">El tipo de cargo de una suscripción cuando se usa la facturación anual.</span><span class="sxs-lookup"><span data-stu-id="584e7-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="584e7-132">Tarifa de compra</span><span class="sxs-lookup"><span data-stu-id="584e7-132">Purchase fee</span></span> | <span data-ttu-id="584e7-133">El tipo de cargo de una suscripción cuando se usa la facturación mensual.</span><span class="sxs-lookup"><span data-stu-id="584e7-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="584e7-134">Tarifa prorrateada al renovar</span><span class="sxs-lookup"><span data-stu-id="584e7-134">Prorate fee when renew</span></span> | <span data-ttu-id="584e7-135">Tarifas prorrateadas tras la renovación de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="584e7-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="584e7-136">Tarifa de renovación</span><span class="sxs-lookup"><span data-stu-id="584e7-136">Renew fee</span></span> | <span data-ttu-id="584e7-137">Cargo por renovar una suscripción</span><span class="sxs-lookup"><span data-stu-id="584e7-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="584e7-138">Tarifas prorrateadas al activar</span><span class="sxs-lookup"><span data-stu-id="584e7-138">Prorate fees when activate</span></span> | <span data-ttu-id="584e7-139">> tarifas prorrateadas de la activación hasta el final del período de facturación.</span><span class="sxs-lookup"><span data-stu-id="584e7-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="584e7-140">Cargos por única vez</span><span class="sxs-lookup"><span data-stu-id="584e7-140">One-time charges</span></span>

<span data-ttu-id="584e7-141">Para asignar estos cargos de un solo tiempo a la factura, sume la columna **amount** del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="584e7-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="584e7-142">Descripción de cargos (columna ChargeType en el archivo de conciliación)</span><span class="sxs-lookup"><span data-stu-id="584e7-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="584e7-143">Explicación de cargos</span><span class="sxs-lookup"><span data-stu-id="584e7-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="584e7-144">Nuevo</span><span class="sxs-lookup"><span data-stu-id="584e7-144">New</span></span> | <span data-ttu-id="584e7-145">Se usa cuando se crea una nueva compra.</span><span class="sxs-lookup"><span data-stu-id="584e7-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="584e7-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="584e7-146">addQuantity</span></span> | <span data-ttu-id="584e7-147">Se usa tanto en el reembolso de la compra original como en la nueva cantidad después de un aumento.</span><span class="sxs-lookup"><span data-stu-id="584e7-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="584e7-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="584e7-148">removeQuantity</span></span> | <span data-ttu-id="584e7-149">Se usa tanto en el reembolso de la compra original como en la nueva cantidad tras una disminución.</span><span class="sxs-lookup"><span data-stu-id="584e7-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="584e7-150">Cancelar</span><span class="sxs-lookup"><span data-stu-id="584e7-150">Cancel</span></span> | <span data-ttu-id="584e7-151">Se usa cuando se cancela una suscripción.</span><span class="sxs-lookup"><span data-stu-id="584e7-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="584e7-152">Convertir</span><span class="sxs-lookup"><span data-stu-id="584e7-152">Convert</span></span> | <span data-ttu-id="584e7-153">Se usa cuando se actualiza una licencia pero el número de puestos permanece inalterado.</span><span class="sxs-lookup"><span data-stu-id="584e7-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="584e7-154">Usage charges</span><span class="sxs-lookup"><span data-stu-id="584e7-154">Usage charges</span></span>

<span data-ttu-id="584e7-155">Para asignar estos cargos de uso a la factura, sume la columna **PretaxCharges** del archivo basado en el uso.</span><span class="sxs-lookup"><span data-stu-id="584e7-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="584e7-156">Descripción de cargos (columna ChargeType en el archivo de conciliación)</span><span class="sxs-lookup"><span data-stu-id="584e7-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="584e7-157">Explicación de cargos</span><span class="sxs-lookup"><span data-stu-id="584e7-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="584e7-158">Evaluar la tarifa de uso al cancelar</span><span class="sxs-lookup"><span data-stu-id="584e7-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="584e7-159">Cuota de uso de acceso tras la cancelación del uso no pagado durante el período de facturación actual.</span><span class="sxs-lookup"><span data-stu-id="584e7-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="584e7-160">Evaluar la tarifa de uso para el ciclo actual</span><span class="sxs-lookup"><span data-stu-id="584e7-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="584e7-161">Cuota de uso de acceso para el período de facturación actual.</span><span class="sxs-lookup"><span data-stu-id="584e7-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="584e7-162">Créditos</span><span class="sxs-lookup"><span data-stu-id="584e7-162">Credits</span></span>

<span data-ttu-id="584e7-163">Para asignar estos créditos a su factura:</span><span class="sxs-lookup"><span data-stu-id="584e7-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="584e7-164">Sume el **TotalForCustomer** del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="584e7-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="584e7-165">Sume la columna **PostTaxTotal** del archivo basado en el uso.</span><span class="sxs-lookup"><span data-stu-id="584e7-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="584e7-166">Descripción de cargos (columna ChargeType en el archivo de conciliación)</span><span class="sxs-lookup"><span data-stu-id="584e7-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="584e7-167">Explicación de cargos</span><span class="sxs-lookup"><span data-stu-id="584e7-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="584e7-168">Desplazamiento de un elemento de línea</span><span class="sxs-lookup"><span data-stu-id="584e7-168">Offset a line item</span></span> | <span data-ttu-id="584e7-169">Reembolso parcial o completo a un artículo de línea, incluidos los impuestos.</span><span class="sxs-lookup"><span data-stu-id="584e7-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="584e7-170">Descuentos basados en uso</span><span class="sxs-lookup"><span data-stu-id="584e7-170">Usage-based discounts</span></span>

<span data-ttu-id="584e7-171">Para asignar estos descuentos basados en el uso a la factura, sume la columna **PretaxCharges** del archivo basado en el uso.</span><span class="sxs-lookup"><span data-stu-id="584e7-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="584e7-172">Descripción de cargos (columna ChargeType en el archivo de conciliación)</span><span class="sxs-lookup"><span data-stu-id="584e7-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="584e7-173">Explicación de cargos</span><span class="sxs-lookup"><span data-stu-id="584e7-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="584e7-174">Descuento de activación</span><span class="sxs-lookup"><span data-stu-id="584e7-174">Activation discount</span></span> | <span data-ttu-id="584e7-175">Descuento que se aplica cuando se activa la suscripción.</span><span class="sxs-lookup"><span data-stu-id="584e7-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="584e7-176">Descuento de ciclo</span><span class="sxs-lookup"><span data-stu-id="584e7-176">Cycle discount</span></span> | <span data-ttu-id="584e7-177">Descuento aplicado a los cargos periódicos.</span><span class="sxs-lookup"><span data-stu-id="584e7-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="584e7-178">Descuento de renovación</span><span class="sxs-lookup"><span data-stu-id="584e7-178">Renew discount</span></span> | <span data-ttu-id="584e7-179">Descuento que se aplica cuando se renueva la suscripción.</span><span class="sxs-lookup"><span data-stu-id="584e7-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="584e7-180">Descuento de cancelación</span><span class="sxs-lookup"><span data-stu-id="584e7-180">Cancel discount</span></span> | <span data-ttu-id="584e7-181">Cargos aplicados cuando se cancelan los descuentos.</span><span class="sxs-lookup"><span data-stu-id="584e7-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="584e7-182">Descuentos basados en licencias</span><span class="sxs-lookup"><span data-stu-id="584e7-182">License-based discounts</span></span>

<span data-ttu-id="584e7-183">Para asignar descuentos basados en licencias a la factura, sume la columna **TotalOtherDiscount** del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="584e7-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="584e7-184">*Los descuentos basados en licencias se pueden aplicar a varios tipos de cargos.*</span><span class="sxs-lookup"><span data-stu-id="584e7-184">*License-based discounts may be applied to multiple charge types.*</span></span>
