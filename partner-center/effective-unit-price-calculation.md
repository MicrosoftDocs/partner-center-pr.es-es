---
title: Cálculo del precio unitario vigente
ms.topic: how-to
ms.date: 04/02/2021
description: Obtenga información sobre el precio unitario efectivo y cómo se calcula. En este artículo también se incluye un cálculo de ejemplo.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147129"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="9aeca-104">Cálculo del precio unitario efectivo para el consumo del plan de Azure</span><span class="sxs-lookup"><span data-stu-id="9aeca-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="9aeca-105">**Roles adecuados:** Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="9aeca-105">**Appropriate roles**: Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="9aeca-106">El precio unitario efectivo</span><span class="sxs-lookup"><span data-stu-id="9aeca-106">The effective unit price</span></span>

<span data-ttu-id="9aeca-107">El precio unitario efectivo se calcula en el nivel de medidor (en lugar del nivel de recurso) y se ajusta diariamente según el uso del medidor.</span><span class="sxs-lookup"><span data-stu-id="9aeca-107">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="9aeca-108">Calculamos el precio unitario efectivo mediante los tres factores siguientes:</span><span class="sxs-lookup"><span data-stu-id="9aeca-108">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="9aeca-109">Consumo, que se supervisa diariamente a lo largo del ciclo de facturación</span><span class="sxs-lookup"><span data-stu-id="9aeca-109">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="9aeca-110">Costo facturable del medidor</span><span class="sxs-lookup"><span data-stu-id="9aeca-110">Billable cost for the meter</span></span>
- <span data-ttu-id="9aeca-111">Niveles (si procede)</span><span class="sxs-lookup"><span data-stu-id="9aeca-111">Tiering (if applicable)</span></span>

<span data-ttu-id="9aeca-112">Dado que supervisamos el consumo diariamente a lo largo del ciclo de facturación, el precio unitario efectivo fluctúa.</span><span class="sxs-lookup"><span data-stu-id="9aeca-112">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="9aeca-113">El precio final de un ciclo de facturación determinado estará disponible después de detener el cálculo de consumo y cerrar el período de facturación.</span><span class="sxs-lookup"><span data-stu-id="9aeca-113">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="9aeca-114">Verá la mayoría de los cambios en el consumo después de la cuarta o la quinta posición decimal.</span><span class="sxs-lookup"><span data-stu-id="9aeca-114">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="9aeca-115">Averiguar si el medidor usa precios por niveles</span><span class="sxs-lookup"><span data-stu-id="9aeca-115">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="9aeca-116">Si no sabe si el medidor usa precios por niveles, use el procedimiento siguiente para averiguarlo.</span><span class="sxs-lookup"><span data-stu-id="9aeca-116">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="9aeca-117">Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="9aeca-117">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="9aeca-118">Seleccione **Vender,** Precios **y ofertas y,** a continuación, seleccione Precios del plan de **Azure.**</span><span class="sxs-lookup"><span data-stu-id="9aeca-118">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="9aeca-119">Busque el medidor por identificador y, a continuación, descargue los datos de precios.</span><span class="sxs-lookup"><span data-stu-id="9aeca-119">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="9aeca-120">Cálculo de ejemplo</span><span class="sxs-lookup"><span data-stu-id="9aeca-120">Sample calculation</span></span>

<span data-ttu-id="9aeca-121">En la tabla siguiente se proporciona un ejemplo de cómo se calcula el precio unitario efectivo durante el período de apertura.</span><span class="sxs-lookup"><span data-stu-id="9aeca-121">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="9aeca-122">En la tabla, se aplican los valores siguientes:</span><span class="sxs-lookup"><span data-stu-id="9aeca-122">In the table, the following values apply:</span></span> 

- <span data-ttu-id="9aeca-123">**UP** = Precio unitario del recurso/hora = 0,868</span><span class="sxs-lookup"><span data-stu-id="9aeca-123">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="9aeca-124">**BCU** = Unidad de consumo facturable para el medidor</span><span class="sxs-lookup"><span data-stu-id="9aeca-124">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="9aeca-125">**BC** = Costo facturable para el medidor = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="9aeca-125">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="9aeca-126">Esto refleja un ajuste para el descuento del 15 % de PEC.</span><span class="sxs-lookup"><span data-stu-id="9aeca-126">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="9aeca-127">A continuación, usamos el límite inferior de la función para limitar el valor a dos dígitos después del separador decimal, con el fin de cobrar la cantidad mínima.</span><span class="sxs-lookup"><span data-stu-id="9aeca-127">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="9aeca-128">**Precio unitario efectivo** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="9aeca-128">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="9aeca-129">Nota: El medidor de este ejemplo no tiene niveles en los precios u otros descuentos: el precio unitario efectivo tiene en cuenta los porcentajes de descuento y otros ajustes.</span><span class="sxs-lookup"><span data-stu-id="9aeca-129">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="9aeca-130">Fecha</span><span class="sxs-lookup"><span data-stu-id="9aeca-130">Date</span></span> | <span data-ttu-id="9aeca-131">BCU (unidad de consumo facturable)</span><span class="sxs-lookup"><span data-stu-id="9aeca-131">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="9aeca-132">BC (costo facturable)</span><span class="sxs-lookup"><span data-stu-id="9aeca-132">BC (Billable cost)</span></span> | <span data-ttu-id="9aeca-133">Precio unitario efectivo</span><span class="sxs-lookup"><span data-stu-id="9aeca-133">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="9aeca-134">3 de agosto</span><span class="sxs-lookup"><span data-stu-id="9aeca-134">3-Aug</span></span> | <span data-ttu-id="9aeca-135">29</span><span class="sxs-lookup"><span data-stu-id="9aeca-135">29</span></span> | <span data-ttu-id="9aeca-136">21.39</span><span class="sxs-lookup"><span data-stu-id="9aeca-136">21.39</span></span> | <span data-ttu-id="9aeca-137">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="9aeca-137">0.737586206896552</span></span> |
| <span data-ttu-id="9aeca-138">10 de agosto</span><span class="sxs-lookup"><span data-stu-id="9aeca-138">10-Aug</span></span> | <span data-ttu-id="9aeca-139">210.950039</span><span class="sxs-lookup"><span data-stu-id="9aeca-139">210.950039</span></span> | <span data-ttu-id="9aeca-140">155.63</span><span class="sxs-lookup"><span data-stu-id="9aeca-140">155.63</span></span> | <span data-ttu-id="9aeca-141">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="9aeca-141">0.737757626107858</span></span> |
| <span data-ttu-id="9aeca-142">25 de agosto</span><span class="sxs-lookup"><span data-stu-id="9aeca-142">25-Aug</span></span> | <span data-ttu-id="9aeca-143">555.950039</span><span class="sxs-lookup"><span data-stu-id="9aeca-143">555.950039</span></span> | <span data-ttu-id="9aeca-144">410.17</span><span class="sxs-lookup"><span data-stu-id="9aeca-144">410.17</span></span> | <span data-ttu-id="9aeca-145">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="9aeca-145">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="9aeca-146">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="9aeca-146">Next steps</span></span>

- [<span data-ttu-id="9aeca-147">Facturación e impuestos</span><span class="sxs-lookup"><span data-stu-id="9aeca-147">Billing and taxes</span></span>](billing.md)
