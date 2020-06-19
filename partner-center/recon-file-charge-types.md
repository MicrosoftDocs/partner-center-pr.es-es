---
title: Tipos de cargos de archivo de conciliación
ms.topic: article
ms.date: 06/05/2020
description: Descubra los tipos de cargos (como, basado en licencias, basados en el uso, y una sola vez), créditos y descuentos en los archivos de conciliación del centro de Partners.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1ec4f4a483ecfd106f7ec41b85372e136524a046
ms.sourcegitcommit: 1796d3d0ec2e06a3792852377ff81127b4d22fe0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/17/2020
ms.locfileid: "84909113"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="e40df-103">Comprender los distintos tipos de cargos en los archivos de conciliación del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="e40df-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="e40df-104">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="e40df-104">**Applies to**</span></span>

- <span data-ttu-id="e40df-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="e40df-105">Partner Center</span></span>
- <span data-ttu-id="e40df-106">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="e40df-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="e40df-107">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="e40df-107">**Appropriate roles**</span></span>

- <span data-ttu-id="e40df-108">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="e40df-108">Admin agent</span></span>
- <span data-ttu-id="e40df-109">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="e40df-109">Billing admin</span></span>
- <span data-ttu-id="e40df-110">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e40df-110">Global admin</span></span>

<span data-ttu-id="e40df-111">En este tema se describen las asignaciones entre una sección de factura y los tipos de cargos asociados que podrían estar en el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="e40df-111">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="e40df-112">La factura proporciona un resumen de los cargos.</span><span class="sxs-lookup"><span data-stu-id="e40df-112">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="e40df-113">El archivo de conciliación proporciona un desglose detallado de las transacciones de elementos de línea, incluidos los tipos de cargos.</span><span class="sxs-lookup"><span data-stu-id="e40df-113">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="e40df-114">Para obtener más información acerca de los archivos de conciliación, consulte [uso de archivos de conciliación](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="e40df-114">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="e40df-115">Tanto [los archivos de conciliación basados en el uso](usage-based-recon-files.md) como [los archivos de conciliación basados en licencias](license-based-recon-files.md) solo muestran las transacciones y los cargos relacionados con el uso (unidades consumidas y cargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="e40df-115">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="e40df-116">No se muestran en el archivo de conciliación los créditos, descuentos o reembolsos de un solo descuento que aparecen en la factura como **ajustes** .</span><span class="sxs-lookup"><span data-stu-id="e40df-116">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="e40df-117">Asignación de tipos de cargos a cargos de factura</span><span class="sxs-lookup"><span data-stu-id="e40df-117">Map charge types to invoice charges</span></span>

<span data-ttu-id="e40df-118">Para hacer referencias cruzadas de los importes de los cargos entre su factura y el archivo de conciliación, use las opciones de filtro de Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="e40df-118">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="e40df-119">Filtre por tipos de carga en el archivo de conciliación para asignar los cargos de la factura a un conjunto de desgloses de gastos en el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="e40df-119">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="e40df-120">Cargos basados en licencias</span><span class="sxs-lookup"><span data-stu-id="e40df-120">License-based charges</span></span>

<span data-ttu-id="e40df-121">Para asignar estos cargos basados en licencias a la factura, sume la columna **amount** del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="e40df-121">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="e40df-122">Descripción de cargos (columna ChargeType en el archivo de conciliación)</span><span class="sxs-lookup"><span data-stu-id="e40df-122">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e40df-123">Explicación de cargos</span><span class="sxs-lookup"><span data-stu-id="e40df-123">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e40df-124">Tarifa de activación</span><span class="sxs-lookup"><span data-stu-id="e40df-124">Activation fee</span></span> | <span data-ttu-id="e40df-125">La cantidad que se cobra al cliente cuando usa la suscripción después de la compra.</span><span class="sxs-lookup"><span data-stu-id="e40df-125">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="e40df-126">Cuota de cancelación</span><span class="sxs-lookup"><span data-stu-id="e40df-126">Cancel fee</span></span> | <span data-ttu-id="e40df-127">Los cargos prorrateados se reembolsan al cliente cuando se cambian los puestos asociados.</span><span class="sxs-lookup"><span data-stu-id="e40df-127">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="e40df-128">Cancelar prorrateo de instancia</span><span class="sxs-lookup"><span data-stu-id="e40df-128">Cancel instance prorate</span></span> | <span data-ttu-id="e40df-129">Los cargos prorrateados se cancelan cuando el cliente con una suscripción mensual tiene una suscripción suspendida y los puestos asociados cambian en el mismo mes.</span><span class="sxs-lookup"><span data-stu-id="e40df-129">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated seats changed within the same month.</span></span> |
| <span data-ttu-id="e40df-130">Tarifa de ciclo</span><span class="sxs-lookup"><span data-stu-id="e40df-130">Cycle fee</span></span> | <span data-ttu-id="e40df-131">Cargos periódicos de una suscripción.</span><span class="sxs-lookup"><span data-stu-id="e40df-131">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="e40df-132">Prorrateo de instancia de ciclo</span><span class="sxs-lookup"><span data-stu-id="e40df-132">Cycle instance prorate</span></span> | <span data-ttu-id="e40df-133">Cargos prorrateados evaluados por el cliente cuando se cambian los puestos asociados.</span><span class="sxs-lookup"><span data-stu-id="e40df-133">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="e40df-134">Tarifas de prorrateo al cancelar</span><span class="sxs-lookup"><span data-stu-id="e40df-134">Prorate fees when cancel</span></span> | <span data-ttu-id="e40df-135">Reembolso prorrateado de la parte no utilizada del servicio tras la cancelación.</span><span class="sxs-lookup"><span data-stu-id="e40df-135">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="e40df-136">Tarifas de prorrateo cuando se convierten de la oferta actual</span><span class="sxs-lookup"><span data-stu-id="e40df-136">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="e40df-137">Cargos prorrateados después de la conversión de la suscripción mensual actual a una suscripción anual.</span><span class="sxs-lookup"><span data-stu-id="e40df-137">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="e40df-138">Cuotas de protarifas cuando se convierten a una nueva oferta</span><span class="sxs-lookup"><span data-stu-id="e40df-138">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="e40df-139">Cargos prorrateados después de convertir una suscripción mensual a una nueva suscripción anual.</span><span class="sxs-lookup"><span data-stu-id="e40df-139">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="e40df-140">Tarifas prorrateadas al comprar</span><span class="sxs-lookup"><span data-stu-id="e40df-140">Prorate fees when purchase</span></span> | <span data-ttu-id="e40df-141">El tipo de cargo de una suscripción cuando se usa la facturación anual.</span><span class="sxs-lookup"><span data-stu-id="e40df-141">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="e40df-142">Precio de compra</span><span class="sxs-lookup"><span data-stu-id="e40df-142">Purchase fee</span></span> | <span data-ttu-id="e40df-143">El tipo de cargo de una suscripción cuando se usa la facturación mensual.</span><span class="sxs-lookup"><span data-stu-id="e40df-143">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="e40df-144">Cuota de prorrateo al renovar</span><span class="sxs-lookup"><span data-stu-id="e40df-144">Prorate fee when renew</span></span> | <span data-ttu-id="e40df-145">Tarifas prorrateadas tras la renovación de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="e40df-145">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="e40df-146">Precio de renovación</span><span class="sxs-lookup"><span data-stu-id="e40df-146">Renew fee</span></span> | <span data-ttu-id="e40df-147">Cargo por renovar una suscripción</span><span class="sxs-lookup"><span data-stu-id="e40df-147">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="e40df-148">Tarifas de protarifas al activar</span><span class="sxs-lookup"><span data-stu-id="e40df-148">Prorate fees when activate</span></span> | <span data-ttu-id="e40df-149">Tarifas prorrateadas de la activación hasta el final del período de facturación.</span><span class="sxs-lookup"><span data-stu-id="e40df-149">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="e40df-150">Cargos por única vez</span><span class="sxs-lookup"><span data-stu-id="e40df-150">One-time charges</span></span>

<span data-ttu-id="e40df-151">Para asignar estos cargos de un solo tiempo a la factura, sume la columna **amount** del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="e40df-151">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="e40df-152">Descripción de cargos (columna ChargeType en el archivo de conciliación)</span><span class="sxs-lookup"><span data-stu-id="e40df-152">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e40df-153">Explicación de cargos</span><span class="sxs-lookup"><span data-stu-id="e40df-153">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e40df-154">Nuevo</span><span class="sxs-lookup"><span data-stu-id="e40df-154">New</span></span> | <span data-ttu-id="e40df-155">Se usa cuando se crea una nueva compra.</span><span class="sxs-lookup"><span data-stu-id="e40df-155">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="e40df-156">addQuantity</span><span class="sxs-lookup"><span data-stu-id="e40df-156">addQuantity</span></span> | <span data-ttu-id="e40df-157">Se usa tanto en el reembolso de la compra original como en la nueva cantidad después de un aumento.</span><span class="sxs-lookup"><span data-stu-id="e40df-157">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="e40df-158">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="e40df-158">removeQuantity</span></span> | <span data-ttu-id="e40df-159">Se usa tanto en el reembolso de la compra original como en la nueva cantidad tras una disminución.</span><span class="sxs-lookup"><span data-stu-id="e40df-159">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="e40df-160">Cancelar</span><span class="sxs-lookup"><span data-stu-id="e40df-160">Cancel</span></span> | <span data-ttu-id="e40df-161">Se usa cuando se cancela una suscripción.</span><span class="sxs-lookup"><span data-stu-id="e40df-161">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="e40df-162">Convert</span><span class="sxs-lookup"><span data-stu-id="e40df-162">Convert</span></span> | <span data-ttu-id="e40df-163">Se usa cuando se actualiza una licencia pero el número de puestos permanece inalterado.</span><span class="sxs-lookup"><span data-stu-id="e40df-163">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="e40df-164">Cargos de uso</span><span class="sxs-lookup"><span data-stu-id="e40df-164">Usage charges</span></span>

<span data-ttu-id="e40df-165">Para asignar estos cargos de uso a la factura, sume la columna **PretaxCharges** del archivo basado en el uso.</span><span class="sxs-lookup"><span data-stu-id="e40df-165">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="e40df-166">Descripción de cargos (columna ChargeType en el archivo de conciliación)</span><span class="sxs-lookup"><span data-stu-id="e40df-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e40df-167">Explicación de cargos</span><span class="sxs-lookup"><span data-stu-id="e40df-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e40df-168">Evaluar la cuota de uso al cancelar</span><span class="sxs-lookup"><span data-stu-id="e40df-168">Assess usage fee when cancel</span></span> | <span data-ttu-id="e40df-169">Precio de uso de acceso a la cancelación por el uso no pagado durante el período de facturación actual.</span><span class="sxs-lookup"><span data-stu-id="e40df-169">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="e40df-170">Evaluar la cuota de uso del ciclo actual</span><span class="sxs-lookup"><span data-stu-id="e40df-170">Assess usage fee for current cycle</span></span> | <span data-ttu-id="e40df-171">Precio de uso de acceso para el período de facturación actual.</span><span class="sxs-lookup"><span data-stu-id="e40df-171">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="e40df-172">Créditos</span><span class="sxs-lookup"><span data-stu-id="e40df-172">Credits</span></span>

<span data-ttu-id="e40df-173">Para asignar estos créditos a su factura:</span><span class="sxs-lookup"><span data-stu-id="e40df-173">To map these credits to your invoice:</span></span>

- <span data-ttu-id="e40df-174">Sume el **TotalForCustomer** del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="e40df-174">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="e40df-175">Sume la columna **PostTaxTotal** del archivo basado en el uso.</span><span class="sxs-lookup"><span data-stu-id="e40df-175">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="e40df-176">Descripción de cargos (columna ChargeType en el archivo de conciliación)</span><span class="sxs-lookup"><span data-stu-id="e40df-176">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e40df-177">Explicación de cargos</span><span class="sxs-lookup"><span data-stu-id="e40df-177">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e40df-178">Desplazar un elemento de línea</span><span class="sxs-lookup"><span data-stu-id="e40df-178">Offset a line item</span></span> | <span data-ttu-id="e40df-179">Reembolso completo o parcial a un elemento de línea, incluidos los impuestos.</span><span class="sxs-lookup"><span data-stu-id="e40df-179">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="e40df-180">Descuentos basados en el uso</span><span class="sxs-lookup"><span data-stu-id="e40df-180">Usage-based discounts</span></span>

<span data-ttu-id="e40df-181">Para asignar estos descuentos basados en el uso a la factura, sume la columna **PretaxCharges** del archivo basado en el uso.</span><span class="sxs-lookup"><span data-stu-id="e40df-181">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="e40df-182">Descripción de cargos (columna ChargeType en el archivo de conciliación)</span><span class="sxs-lookup"><span data-stu-id="e40df-182">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="e40df-183">Explicación de cargos</span><span class="sxs-lookup"><span data-stu-id="e40df-183">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="e40df-184">Descuento de activación</span><span class="sxs-lookup"><span data-stu-id="e40df-184">Activation discount</span></span> | <span data-ttu-id="e40df-185">Descuento que se aplica cuando se activa la suscripción.</span><span class="sxs-lookup"><span data-stu-id="e40df-185">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="e40df-186">Descuento por ciclo</span><span class="sxs-lookup"><span data-stu-id="e40df-186">Cycle discount</span></span> | <span data-ttu-id="e40df-187">Descuento aplicado a los cargos periódicos.</span><span class="sxs-lookup"><span data-stu-id="e40df-187">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="e40df-188">Renovar descuento</span><span class="sxs-lookup"><span data-stu-id="e40df-188">Renew discount</span></span> | <span data-ttu-id="e40df-189">Descuento que se aplica cuando se renueva la suscripción.</span><span class="sxs-lookup"><span data-stu-id="e40df-189">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="e40df-190">Cancelar descuento</span><span class="sxs-lookup"><span data-stu-id="e40df-190">Cancel discount</span></span> | <span data-ttu-id="e40df-191">Cargos que se aplica cuando se cancelan los descuentos.</span><span class="sxs-lookup"><span data-stu-id="e40df-191">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="e40df-192">Descuentos basados en licencias</span><span class="sxs-lookup"><span data-stu-id="e40df-192">License-based discounts</span></span>

<span data-ttu-id="e40df-193">Para asignar descuentos basados en licencias a la factura, sume la columna **TotalOtherDiscount** del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="e40df-193">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="e40df-194">*Los descuentos basados en licencias se pueden aplicar a varios tipos de cargos.*</span><span class="sxs-lookup"><span data-stu-id="e40df-194">*License-based discounts may be applied to multiple charge types.*</span></span>
