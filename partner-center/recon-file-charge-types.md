---
title: Tipos de cargo de archivo de conciliación
ms.topic: article
ms.date: 06/05/2020
description: Descubra los tipos de cargos (como, basado en licencias, basados en el uso, y una sola vez), créditos y descuentos en los archivos de conciliación del centro de Partners.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f1fb7fdcc4ec56f0d5cf0eb26b62294235a5b908
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441609"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a><span data-ttu-id="8af44-103">Comprender los distintos tipos de cargos en los archivos de conciliación del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="8af44-103">Understand the different charge types in Partner Center reconciliation files</span></span>

<span data-ttu-id="8af44-104">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="8af44-104">**Applies to**</span></span>

- <span data-ttu-id="8af44-105">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="8af44-105">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="8af44-106">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="8af44-106">**Appropriate roles**</span></span>

- <span data-ttu-id="8af44-107">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="8af44-107">Admin agent</span></span>
- <span data-ttu-id="8af44-108">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="8af44-108">Billing admin</span></span>
- <span data-ttu-id="8af44-109">Administrador global</span><span class="sxs-lookup"><span data-stu-id="8af44-109">Global admin</span></span>

<span data-ttu-id="8af44-110">En este artículo se describen las asignaciones entre una sección de factura y los tipos de cargos asociados que podrían estar en el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="8af44-110">This article describes the mappings between an invoice section and associated charge types that might be on your reconciliation file.</span></span> <span data-ttu-id="8af44-111">La factura proporciona un resumen de los cargos.</span><span class="sxs-lookup"><span data-stu-id="8af44-111">Your invoice provides a summary of charges.</span></span> <span data-ttu-id="8af44-112">El archivo de conciliación proporciona un desglose detallado de las transacciones de elementos de línea, incluidos los tipos de cargos.</span><span class="sxs-lookup"><span data-stu-id="8af44-112">Your reconciliation file provides a detailed breakdown of line-item transactions, including charge types.</span></span> <span data-ttu-id="8af44-113">Para obtener más información acerca de los archivos de conciliación, consulte [uso de archivos de conciliación](use-the-reconciliation-files.md).</span><span class="sxs-lookup"><span data-stu-id="8af44-113">For more information on reconciliation files, see [how to use reconciliation files](use-the-reconciliation-files.md).</span></span>

<span data-ttu-id="8af44-114">Tanto [los archivos de conciliación basados en el uso](usage-based-recon-files.md) como [los archivos de conciliación basados en licencias](license-based-recon-files.md) solo muestran las transacciones y los cargos relacionados con el uso (unidades consumidas y cargos relacionados).</span><span class="sxs-lookup"><span data-stu-id="8af44-114">Both [usage-based reconciliation files](usage-based-recon-files.md) and [license-based reconciliation files](license-based-recon-files.md) only show usage-related transactions and charges (units consumed and related charges).</span></span>

> [!NOTE]
> <span data-ttu-id="8af44-115">No se muestran en el archivo de conciliación los créditos, descuentos o reembolsos de un solo descuento que aparecen en la factura como **ajustes** .</span><span class="sxs-lookup"><span data-stu-id="8af44-115">One-off credits, discounts or refunds that appear on the invoice as **Adjustments** are not shown in the reconciliation file.</span></span>

## <a name="map-charge-types-to-invoice-charges"></a><span data-ttu-id="8af44-116">Asignación de tipos de cargos a cargos de factura</span><span class="sxs-lookup"><span data-stu-id="8af44-116">Map charge types to invoice charges</span></span>

<span data-ttu-id="8af44-117">Para hacer referencias cruzadas de los importes de los cargos entre su factura y el archivo de conciliación, use las opciones de filtro de Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="8af44-117">To cross-reference charge amounts between your invoice and reconciliation file, use the filter options in Microsoft Excel.</span></span> <span data-ttu-id="8af44-118">Filtre por tipos de carga en el archivo de conciliación para asignar los cargos de la factura a un conjunto de desgloses de gastos en el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="8af44-118">Filter by charge types on your reconciliation file to map the invoice charges to a set of charge breakdowns on the reconciliation file.</span></span>

## <a name="license-based-charges"></a><span data-ttu-id="8af44-119">Cargos basados en licencias</span><span class="sxs-lookup"><span data-stu-id="8af44-119">License-based charges</span></span>

<span data-ttu-id="8af44-120">Para asignar estos cargos basados en licencias a la factura, sume la columna **amount** del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="8af44-120">To map these license-based charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="8af44-121">Descripción de cargos (columna ChargeType en el archivo de conciliación)</span><span class="sxs-lookup"><span data-stu-id="8af44-121">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="8af44-122">Explicación de cargos</span><span class="sxs-lookup"><span data-stu-id="8af44-122">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="8af44-123">Tarifa de activación</span><span class="sxs-lookup"><span data-stu-id="8af44-123">Activation fee</span></span> | <span data-ttu-id="8af44-124">La cantidad que se cobra al cliente cuando usa la suscripción después de la compra.</span><span class="sxs-lookup"><span data-stu-id="8af44-124">The amount charged to the customer when they use the subscription after purchase.</span></span> |
| <span data-ttu-id="8af44-125">Cuota de cancelación</span><span class="sxs-lookup"><span data-stu-id="8af44-125">Cancel fee</span></span> | <span data-ttu-id="8af44-126">Cargos prorrateados reembolsados al cliente cuando se cambian las licencias asociadas.</span><span class="sxs-lookup"><span data-stu-id="8af44-126">Prorated charges refunded to the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="8af44-127">Cancelar prorrateo de instancia</span><span class="sxs-lookup"><span data-stu-id="8af44-127">Cancel instance prorate</span></span> | <span data-ttu-id="8af44-128">Los cargos prorrateados se cancelan cuando el cliente con una suscripción mensual tiene una suscripción suspendida y las licencias asociadas cambian en el mismo mes.</span><span class="sxs-lookup"><span data-stu-id="8af44-128">Prorated charges canceled when customer with monthly subscription has subscription suspended and associated licenses changed within the same month.</span></span> |
| <span data-ttu-id="8af44-129">Tarifa de ciclo</span><span class="sxs-lookup"><span data-stu-id="8af44-129">Cycle fee</span></span> | <span data-ttu-id="8af44-130">Cargos periódicos de una suscripción.</span><span class="sxs-lookup"><span data-stu-id="8af44-130">Periodic charges for a subscription.</span></span> |
| <span data-ttu-id="8af44-131">Prorrateo de instancia de ciclo</span><span class="sxs-lookup"><span data-stu-id="8af44-131">Cycle instance prorate</span></span> | <span data-ttu-id="8af44-132">Cargos prorrateados evaluados por el cliente cuando se cambian las licencias asociadas.</span><span class="sxs-lookup"><span data-stu-id="8af44-132">Prorated charges assessed from the customer when associated licenses are changed.</span></span> |
| <span data-ttu-id="8af44-133">Tarifas de prorrateo al cancelar</span><span class="sxs-lookup"><span data-stu-id="8af44-133">Prorate fees when cancel</span></span> | <span data-ttu-id="8af44-134">Reembolso prorrateado de la parte no utilizada del servicio tras la cancelación.</span><span class="sxs-lookup"><span data-stu-id="8af44-134">Prorated refund for unused portion of service upon cancellation.</span></span> |
| <span data-ttu-id="8af44-135">Tarifas de prorrateo cuando se convierten de la oferta actual</span><span class="sxs-lookup"><span data-stu-id="8af44-135">Prorate fees when convert away from current offering</span></span> | <span data-ttu-id="8af44-136">Cargos prorrateados después de la conversión de la suscripción mensual actual a una suscripción anual.</span><span class="sxs-lookup"><span data-stu-id="8af44-136">Prorated charges after converting away from the current monthly subscription to an annual subscription.</span></span> |
| <span data-ttu-id="8af44-137">Cuotas de protarifas cuando se convierten a una nueva oferta</span><span class="sxs-lookup"><span data-stu-id="8af44-137">Prorate fees when convert to a new offering</span></span> | <span data-ttu-id="8af44-138">Cargos prorrateados después de convertir una suscripción mensual a una nueva suscripción anual.</span><span class="sxs-lookup"><span data-stu-id="8af44-138">Prorated charges after converting a monthly subscription to a new annual subscription.</span></span> |
| <span data-ttu-id="8af44-139">Tarifas prorrateadas al comprar</span><span class="sxs-lookup"><span data-stu-id="8af44-139">Prorate fees when purchase</span></span> | <span data-ttu-id="8af44-140">El tipo de cargo de una suscripción cuando se usa la facturación mensual o anual.</span><span class="sxs-lookup"><span data-stu-id="8af44-140">The charge type for a subscription when using both monthly or annual billing.</span></span> |
| <span data-ttu-id="8af44-141">Cuota de prorrateo al renovar</span><span class="sxs-lookup"><span data-stu-id="8af44-141">Prorate fee when renew</span></span> | <span data-ttu-id="8af44-142">Tarifas prorrateadas tras la renovación de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="8af44-142">Prorated fees upon subscription renewal.</span></span> |
| <span data-ttu-id="8af44-143">Precio de renovación</span><span class="sxs-lookup"><span data-stu-id="8af44-143">Renew fee</span></span> | <span data-ttu-id="8af44-144">Cargo por renovar una suscripción</span><span class="sxs-lookup"><span data-stu-id="8af44-144">Charge for renewing a subscription</span></span> |
| <span data-ttu-id="8af44-145">Tarifas de protarifas al activar</span><span class="sxs-lookup"><span data-stu-id="8af44-145">Prorate fees when activate</span></span> | <span data-ttu-id="8af44-146">Tarifas prorrateadas de la activación hasta el final del período de facturación.</span><span class="sxs-lookup"><span data-stu-id="8af44-146">Prorated fees from activation until end of billing period.</span></span> |

## <a name="one-time-charges"></a><span data-ttu-id="8af44-147">Cargos por única vez</span><span class="sxs-lookup"><span data-stu-id="8af44-147">One-time charges</span></span>

<span data-ttu-id="8af44-148">Para asignar estos cargos de un solo tiempo a la factura, sume la columna **amount** del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="8af44-148">To map these one-time charges to your invoice, sum the **Amount** column from the license-based file.</span></span>

| <span data-ttu-id="8af44-149">Descripción de cargos (columna ChargeType en el archivo de conciliación)</span><span class="sxs-lookup"><span data-stu-id="8af44-149">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="8af44-150">Explicación de cargos</span><span class="sxs-lookup"><span data-stu-id="8af44-150">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="8af44-151">Nuevo</span><span class="sxs-lookup"><span data-stu-id="8af44-151">New</span></span> | <span data-ttu-id="8af44-152">Se usa cuando se crea una nueva compra.</span><span class="sxs-lookup"><span data-stu-id="8af44-152">Used when a new purchase is created.</span></span> |
| <span data-ttu-id="8af44-153">addQuantity</span><span class="sxs-lookup"><span data-stu-id="8af44-153">addQuantity</span></span> | <span data-ttu-id="8af44-154">Se usa tanto en el reembolso de la compra original como en la nueva cantidad después de un aumento.</span><span class="sxs-lookup"><span data-stu-id="8af44-154">Used in both the refund of the original purchase and the new quantity after an increase.</span></span> |
| <span data-ttu-id="8af44-155">removeQuantity</span><span class="sxs-lookup"><span data-stu-id="8af44-155">removeQuantity</span></span> | <span data-ttu-id="8af44-156">Se usa tanto en el reembolso de la compra original como en la nueva cantidad tras una disminución.</span><span class="sxs-lookup"><span data-stu-id="8af44-156">Used in both the refund of the original purchase and the new quantity after a decrease.</span></span> |
| <span data-ttu-id="8af44-157">Cancelar</span><span class="sxs-lookup"><span data-stu-id="8af44-157">Cancel</span></span> | <span data-ttu-id="8af44-158">Se usa cuando se cancela una suscripción.</span><span class="sxs-lookup"><span data-stu-id="8af44-158">Used when a subscription is canceled.</span></span> |
| <span data-ttu-id="8af44-159">Convert</span><span class="sxs-lookup"><span data-stu-id="8af44-159">Convert</span></span> | <span data-ttu-id="8af44-160">Se usa cuando se actualiza una licencia pero el número de licencias permanece inalterado.</span><span class="sxs-lookup"><span data-stu-id="8af44-160">Used when a license is upgraded but the number of licenses remains unchanged.</span></span> |

## <a name="usage-charges"></a><span data-ttu-id="8af44-161">Cargos de uso</span><span class="sxs-lookup"><span data-stu-id="8af44-161">Usage charges</span></span>

<span data-ttu-id="8af44-162">Para asignar estos cargos de uso a la factura, sume la columna **PretaxCharges** del archivo basado en el uso.</span><span class="sxs-lookup"><span data-stu-id="8af44-162">To map these usage charges to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="8af44-163">Descripción de cargos (columna ChargeType en el archivo de conciliación)</span><span class="sxs-lookup"><span data-stu-id="8af44-163">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="8af44-164">Explicación de cargos</span><span class="sxs-lookup"><span data-stu-id="8af44-164">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="8af44-165">Evaluar la cuota de uso al cancelar</span><span class="sxs-lookup"><span data-stu-id="8af44-165">Assess usage fee when cancel</span></span> | <span data-ttu-id="8af44-166">Precio de uso de acceso a la cancelación por el uso no pagado durante el período de facturación actual.</span><span class="sxs-lookup"><span data-stu-id="8af44-166">Access usage fee upon cancellation for unpaid usage during the current billing period.</span></span> |
| <span data-ttu-id="8af44-167">Evaluar la cuota de uso del ciclo actual</span><span class="sxs-lookup"><span data-stu-id="8af44-167">Assess usage fee for current cycle</span></span> | <span data-ttu-id="8af44-168">Precio de uso de acceso para el período de facturación actual.</span><span class="sxs-lookup"><span data-stu-id="8af44-168">Access usage fee for the current billing period.</span></span> |

### <a name="credits"></a><span data-ttu-id="8af44-169">Créditos</span><span class="sxs-lookup"><span data-stu-id="8af44-169">Credits</span></span>

<span data-ttu-id="8af44-170">Para asignar estos créditos a su factura:</span><span class="sxs-lookup"><span data-stu-id="8af44-170">To map these credits to your invoice:</span></span>

- <span data-ttu-id="8af44-171">Sume el **TotalForCustomer** del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="8af44-171">Sum the **TotalForCustomer** from the license-based file.</span></span>
- <span data-ttu-id="8af44-172">Sume la columna **PostTaxTotal** del archivo basado en el uso.</span><span class="sxs-lookup"><span data-stu-id="8af44-172">Sum the **PostTaxTotal** column from the usage-based file.</span></span>

| <span data-ttu-id="8af44-173">Descripción de cargos (columna ChargeType en el archivo de conciliación)</span><span class="sxs-lookup"><span data-stu-id="8af44-173">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="8af44-174">Explicación de cargos</span><span class="sxs-lookup"><span data-stu-id="8af44-174">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="8af44-175">Desplazar un elemento de línea</span><span class="sxs-lookup"><span data-stu-id="8af44-175">Offset a line item</span></span> | <span data-ttu-id="8af44-176">Reembolso completo o parcial a un elemento de línea, incluidos los impuestos.</span><span class="sxs-lookup"><span data-stu-id="8af44-176">Partial or whole refund to a line item, including taxes.</span></span> |

### <a name="usage-based-discounts"></a><span data-ttu-id="8af44-177">Descuentos basados en el uso</span><span class="sxs-lookup"><span data-stu-id="8af44-177">Usage-based discounts</span></span>

<span data-ttu-id="8af44-178">Para asignar estos descuentos basados en el uso a la factura, sume la columna **PretaxCharges** del archivo basado en el uso.</span><span class="sxs-lookup"><span data-stu-id="8af44-178">To map these usage-based discounts to your invoice, sum the **PretaxCharges** column from the usage-based file.</span></span>

| <span data-ttu-id="8af44-179">Descripción de cargos (columna ChargeType en el archivo de conciliación)</span><span class="sxs-lookup"><span data-stu-id="8af44-179">Charge description (ChargeType column in reconciliation file)</span></span> | <span data-ttu-id="8af44-180">Explicación de cargos</span><span class="sxs-lookup"><span data-stu-id="8af44-180">Charge explanation</span></span> |
| ------------------------------------------------------------- | ------------------ |
| <span data-ttu-id="8af44-181">Descuento de activación</span><span class="sxs-lookup"><span data-stu-id="8af44-181">Activation discount</span></span> | <span data-ttu-id="8af44-182">Descuento que se aplica cuando se activa la suscripción.</span><span class="sxs-lookup"><span data-stu-id="8af44-182">Discount applied when subscription activated.</span></span> |
| <span data-ttu-id="8af44-183">Descuento por ciclo</span><span class="sxs-lookup"><span data-stu-id="8af44-183">Cycle discount</span></span> | <span data-ttu-id="8af44-184">Descuento aplicado a los cargos periódicos.</span><span class="sxs-lookup"><span data-stu-id="8af44-184">Discount applied on periodic charges.</span></span> |
| <span data-ttu-id="8af44-185">Renovar descuento</span><span class="sxs-lookup"><span data-stu-id="8af44-185">Renew discount</span></span> | <span data-ttu-id="8af44-186">Descuento que se aplica cuando se renueva la suscripción.</span><span class="sxs-lookup"><span data-stu-id="8af44-186">Discount applied when subscription renewed.</span></span> |
| <span data-ttu-id="8af44-187">Cancelar descuento</span><span class="sxs-lookup"><span data-stu-id="8af44-187">Cancel discount</span></span> | <span data-ttu-id="8af44-188">Cargos que se aplica cuando se cancelan los descuentos.</span><span class="sxs-lookup"><span data-stu-id="8af44-188">Charges applied when discounts are canceled.</span></span> |

### <a name="license-based-discounts"></a><span data-ttu-id="8af44-189">Descuentos basados en licencias</span><span class="sxs-lookup"><span data-stu-id="8af44-189">License-based discounts</span></span>

<span data-ttu-id="8af44-190">Para asignar descuentos basados en licencias a la factura, sume la columna **TotalOtherDiscount** del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="8af44-190">To map license-based discounts to your invoice, sum the **TotalOtherDiscount** column from the license-based file.</span></span>

<span data-ttu-id="8af44-191">*Los descuentos basados en licencias se pueden aplicar a varios tipos de cargos.*</span><span class="sxs-lookup"><span data-stu-id="8af44-191">*License-based discounts may be applied to multiple charge types.*</span></span>
