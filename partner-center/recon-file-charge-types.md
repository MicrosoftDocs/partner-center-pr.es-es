---
title: Reconciliation file charge types | Partner Center
ms.topic: article
ms.date: 08/26/2019
description: Types of charges (license-based, usage-based and one-time), credits and discounts on Partner Center reconciliation files.
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
# <a name="understand-charge-types"></a><span data-ttu-id="8e4a6-103">Understand charge types</span><span class="sxs-lookup"><span data-stu-id="8e4a6-103">Understand charge types</span></span>

<span data-ttu-id="8e4a6-104">Se aplica a:</span><span class="sxs-lookup"><span data-stu-id="8e4a6-104">Applies to:</span></span>

- <span data-ttu-id="8e4a6-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="8e4a6-105">Partner Center</span></span>
- <span data-ttu-id="8e4a6-106">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="8e4a6-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="8e4a6-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-107">This topic describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="8e4a6-108">Your invoice provides a summary of charges.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-108">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="8e4a6-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-109">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="8e4a6-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="8e4a6-110">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="8e4a6-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span><span class="sxs-lookup"><span data-stu-id="8e4a6-111">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="8e4a6-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-112">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="8e4a6-113">Map charge types to invoice charges</span><span class="sxs-lookup"><span data-stu-id="8e4a6-113">Map charge types to invoice charges</span></span>

<span data-ttu-id="8e4a6-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-114">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="8e4a6-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-115">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="8e4a6-116">Cargos basados en licencias</span><span class="sxs-lookup"><span data-stu-id="8e4a6-116">License-based charges</span></span>

<span data-ttu-id="8e4a6-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-117">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="8e4a6-118">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="8e4a6-118">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="8e4a6-119">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="8e4a6-119">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="8e4a6-120">Tarifa de activación</span><span class="sxs-lookup"><span data-stu-id="8e4a6-120">Activation fee</span></span> | <span data-ttu-id="8e4a6-121">The amount charged to the customer when they use the subscription after purchase.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-121">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="8e4a6-122">Cuota de cancelación</span><span class="sxs-lookup"><span data-stu-id="8e4a6-122">Cancel fee</span></span> | <span data-ttu-id="8e4a6-123">Prorated charges refunded to the customer when associated seats are changed.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-123">Prorated charges refunded to the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="8e4a6-124">Tarifa de ciclo</span><span class="sxs-lookup"><span data-stu-id="8e4a6-124">Cycle fee</span></span> | <span data-ttu-id="8e4a6-125">Periodic charges for a subscription.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-125">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="8e4a6-126">Prorrateo de instancia de ciclo</span><span class="sxs-lookup"><span data-stu-id="8e4a6-126">Cycle instance prorate</span></span> | <span data-ttu-id="8e4a6-127">Prorated charges assessed from the customer when associated seats are changed.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-127">Prorated charges assessed from the customer when associated seats are changed.</span></span> |
| <span data-ttu-id="8e4a6-128">Tarifas prorrateadas al cancelar</span><span class="sxs-lookup"><span data-stu-id="8e4a6-128">Prorate fees when cancel</span></span> | <span data-ttu-id="8e4a6-129">Prorated refund for unused portion of service upon cancellation.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-129">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="8e4a6-130">Tarifas prorrateadas al comprar</span><span class="sxs-lookup"><span data-stu-id="8e4a6-130">Prorate fees when purchase</span></span> | <span data-ttu-id="8e4a6-131">The charge type for a subscription when using annual billing.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-131">The charge type for a subscription when using annual billing.</span></span> |
| <span data-ttu-id="8e4a6-132">Tarifa de compra</span><span class="sxs-lookup"><span data-stu-id="8e4a6-132">Purchase fee</span></span> | <span data-ttu-id="8e4a6-133">The charge type for a subscription when using monthly billing.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-133">The charge type for a subscription when using monthly billing.</span></span> |
| <span data-ttu-id="8e4a6-134">Tarifa prorrateada al renovar</span><span class="sxs-lookup"><span data-stu-id="8e4a6-134">Prorate fee when renew</span></span> | <span data-ttu-id="8e4a6-135">Prorated fees upon subscription renewal.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-135">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="8e4a6-136">Tarifa de renovación</span><span class="sxs-lookup"><span data-stu-id="8e4a6-136">Renew fee</span></span> | <span data-ttu-id="8e4a6-137">Cargo por renovar una suscripción</span><span class="sxs-lookup"><span data-stu-id="8e4a6-137">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="8e4a6-138">Tarifas prorrateadas al activar</span><span class="sxs-lookup"><span data-stu-id="8e4a6-138">Prorate fees when activate</span></span> | <span data-ttu-id="8e4a6-139">>Prorated fees from activation until end of billing period.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-139">>Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="8e4a6-140">One-time charges</span><span class="sxs-lookup"><span data-stu-id="8e4a6-140">One-time charges</span></span>

<span data-ttu-id="8e4a6-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-141">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="8e4a6-142">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="8e4a6-142">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="8e4a6-143">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="8e4a6-143">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="8e4a6-144">Nuevo</span><span class="sxs-lookup"><span data-stu-id="8e4a6-144">New</span></span> | <span data-ttu-id="8e4a6-145">Used when a new purchase is created.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-145">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="8e4a6-146">addQuantity</span><span class="sxs-lookup"><span data-stu-id="8e4a6-146">addQuantity</span></span> | <span data-ttu-id="8e4a6-147">Used in both the refund of the original purchase and the new quantity after an increase.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-147">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="8e4a6-148">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="8e4a6-148">removeQuantity</span></span> | <span data-ttu-id="8e4a6-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-149">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="8e4a6-150">Cancelar</span><span class="sxs-lookup"><span data-stu-id="8e4a6-150">Cancel</span></span> | <span data-ttu-id="8e4a6-151">Used when a subscription is cancelled.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-151">Used when a subscription is cancelled.</span></span> |
| <span data-ttu-id="8e4a6-152">Conversión</span><span class="sxs-lookup"><span data-stu-id="8e4a6-152">Convert</span></span> | <span data-ttu-id="8e4a6-153">Used when a license is upgraded but the number of seats remains unchanged.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-153">Used when a license is upgraded but the number of seats remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="8e4a6-154">Usage charges</span><span class="sxs-lookup"><span data-stu-id="8e4a6-154">Usage charges</span></span>

<span data-ttu-id="8e4a6-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-155">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="8e4a6-156">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="8e4a6-156">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="8e4a6-157">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="8e4a6-157">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="8e4a6-158">Evaluar la tarifa de uso al cancelar</span><span class="sxs-lookup"><span data-stu-id="8e4a6-158">Assess usage fee when cancel</span></span> | <span data-ttu-id="8e4a6-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-159">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="8e4a6-160">Evaluar la tarifa de uso para el ciclo actual</span><span class="sxs-lookup"><span data-stu-id="8e4a6-160">Assess usage fee for current cycle</span></span> | <span data-ttu-id="8e4a6-161">Access usage fee for the current billing period.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-161">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="8e4a6-162">Créditos</span><span class="sxs-lookup"><span data-stu-id="8e4a6-162">Credits</span></span>

<span data-ttu-id="8e4a6-163">To map these credits to your invoice:</span><span class="sxs-lookup"><span data-stu-id="8e4a6-163">To map these credits to your invoice:</span></span>

- <span data-ttu-id="8e4a6-164">Sum the **TotalForCustomer** from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-164">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="8e4a6-165">Sum the **PostTaxTotal** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-165">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="8e4a6-166">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="8e4a6-166">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="8e4a6-167">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="8e4a6-167">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="8e4a6-168">Desplazamiento de un elemento de línea</span><span class="sxs-lookup"><span data-stu-id="8e4a6-168">Offset a line item</span></span> | <span data-ttu-id="8e4a6-169">Partial or whole refund to a line item, including taxes.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-169">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="8e4a6-170">Descuentos basados en uso</span><span class="sxs-lookup"><span data-stu-id="8e4a6-170">Usage-based discounts</span></span>

<span data-ttu-id="8e4a6-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-171">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="8e4a6-172">Charge description (ChargeType column in reconciliation file)</span><span class="sxs-lookup"><span data-stu-id="8e4a6-172">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="8e4a6-173">Charge explanation</span><span class="sxs-lookup"><span data-stu-id="8e4a6-173">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="8e4a6-174">Descuento de activación</span><span class="sxs-lookup"><span data-stu-id="8e4a6-174">Activation discount</span></span> | <span data-ttu-id="8e4a6-175">Discount applied when subscription activated.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-175">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="8e4a6-176">Descuento de ciclo</span><span class="sxs-lookup"><span data-stu-id="8e4a6-176">Cycle discount</span></span> | <span data-ttu-id="8e4a6-177">Discount applied on periodic charges.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-177">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="8e4a6-178">Descuento de renovación</span><span class="sxs-lookup"><span data-stu-id="8e4a6-178">Renew discount</span></span> | <span data-ttu-id="8e4a6-179">Discount applied when subscription renewed.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-179">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="8e4a6-180">Descuento de cancelación</span><span class="sxs-lookup"><span data-stu-id="8e4a6-180">Cancel discount</span></span> | <span data-ttu-id="8e4a6-181">Charges applied when discounts cancelled.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-181">Charges applied when discounts cancelled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="8e4a6-182">Descuentos basados en licencias</span><span class="sxs-lookup"><span data-stu-id="8e4a6-182">License-based discounts</span></span>

<span data-ttu-id="8e4a6-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span><span class="sxs-lookup"><span data-stu-id="8e4a6-183">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="8e4a6-184">*License-based discounts may be applied to multiple charge types.*</span><span class="sxs-lookup"><span data-stu-id="8e4a6-184">*License-based discounts may be applied to multiple charge types.*</span></span>
