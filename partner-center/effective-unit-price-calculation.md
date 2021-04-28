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
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172224"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="250e7-104">Cálculo de precios unitarios efectivos para el consumo del plan de Azure</span><span class="sxs-lookup"><span data-stu-id="250e7-104">Effective unit price calculation for Azure plan consumption</span></span>

<span data-ttu-id="250e7-105">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="250e7-105">**Appropriate roles**</span></span>

- <span data-ttu-id="250e7-106">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="250e7-106">Billing admin</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="250e7-107">El precio unitario efectivo</span><span class="sxs-lookup"><span data-stu-id="250e7-107">The effective unit price</span></span>

<span data-ttu-id="250e7-108">El precio unitario efectivo se calcula en el nivel de medidor (en lugar del nivel de recurso) y se ajusta diariamente según el uso del medidor.</span><span class="sxs-lookup"><span data-stu-id="250e7-108">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="250e7-109">Calculamos el precio unitario efectivo mediante los tres factores siguientes:</span><span class="sxs-lookup"><span data-stu-id="250e7-109">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="250e7-110">Consumo, que se supervisa diariamente a lo largo del ciclo de facturación</span><span class="sxs-lookup"><span data-stu-id="250e7-110">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="250e7-111">Costo facturable del medidor</span><span class="sxs-lookup"><span data-stu-id="250e7-111">Billable cost for the meter</span></span>
- <span data-ttu-id="250e7-112">Niveles (si procede)</span><span class="sxs-lookup"><span data-stu-id="250e7-112">Tiering (if applicable)</span></span>

<span data-ttu-id="250e7-113">Dado que supervisamos el consumo diariamente a lo largo del ciclo de facturación, el precio unitario efectivo fluctúa.</span><span class="sxs-lookup"><span data-stu-id="250e7-113">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="250e7-114">El precio final de un ciclo de facturación determinado estará disponible después de detener el cálculo de consumo y cerrar el período de facturación.</span><span class="sxs-lookup"><span data-stu-id="250e7-114">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="250e7-115">Verá la mayoría de los cambios en el consumo después de la cuarta o quinta posición decimal.</span><span class="sxs-lookup"><span data-stu-id="250e7-115">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="250e7-116">Averiguar si el medidor usa precios por niveles</span><span class="sxs-lookup"><span data-stu-id="250e7-116">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="250e7-117">Si no sabe si el medidor usa precios por niveles, use el procedimiento siguiente para averiguarlo.</span><span class="sxs-lookup"><span data-stu-id="250e7-117">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="250e7-118">Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="250e7-118">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="250e7-119">Seleccione **Vender,** seleccione **Precios y ofertas** y, a continuación, seleccione Precios del plan de **Azure.**</span><span class="sxs-lookup"><span data-stu-id="250e7-119">Select **Sell**, select **Pricing and offers**, and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="250e7-120">Busque el medidor por identificador y, a continuación, descargue los datos de precios.</span><span class="sxs-lookup"><span data-stu-id="250e7-120">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="250e7-121">Cálculo de ejemplo</span><span class="sxs-lookup"><span data-stu-id="250e7-121">Sample calculation</span></span>

<span data-ttu-id="250e7-122">En la tabla siguiente se proporciona un ejemplo de cómo se calcula el precio unitario efectivo durante el período de apertura.</span><span class="sxs-lookup"><span data-stu-id="250e7-122">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="250e7-123">En la tabla , se aplican los valores siguientes:</span><span class="sxs-lookup"><span data-stu-id="250e7-123">In the table, the following values apply:</span></span> 

- <span data-ttu-id="250e7-124">**UP** = Precio unitario del recurso/hora = 0,868</span><span class="sxs-lookup"><span data-stu-id="250e7-124">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="250e7-125">**BCU** = Unidad de consumo facturable para el medidor</span><span class="sxs-lookup"><span data-stu-id="250e7-125">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="250e7-126">**BC** = Costo facturable para el medidor = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="250e7-126">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="250e7-127">Esto refleja un ajuste para el descuento del 15 % de PEC.</span><span class="sxs-lookup"><span data-stu-id="250e7-127">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="250e7-128">A continuación, usamos el límite inferior de la función para limitar el valor a dos dígitos después del separador decimal, con el fin de cobrar la cantidad mínima.</span><span class="sxs-lookup"><span data-stu-id="250e7-128">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="250e7-129">**Precio unitario efectivo** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="250e7-129">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]

><span data-ttu-id="250e7-130">Nota: El medidor de este ejemplo no tiene niveles en precios u otros descuentos: los factores de precio unitario efectivo en los porcentajes de descuento y otros ajustes.</span><span class="sxs-lookup"><span data-stu-id="250e7-130">Note: The meter in this example does not have tiers in pricing or other discounts—the Effective Unit Price factors in discount percentages and other adjustments.</span></span>


| <span data-ttu-id="250e7-131">Date</span><span class="sxs-lookup"><span data-stu-id="250e7-131">Date</span></span> | <span data-ttu-id="250e7-132">BCU (unidad de consumo facturable)</span><span class="sxs-lookup"><span data-stu-id="250e7-132">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="250e7-133">BC (costo facturable)</span><span class="sxs-lookup"><span data-stu-id="250e7-133">BC (Billable cost)</span></span> | <span data-ttu-id="250e7-134">Precio unitario efectivo</span><span class="sxs-lookup"><span data-stu-id="250e7-134">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="250e7-135">3 de agosto</span><span class="sxs-lookup"><span data-stu-id="250e7-135">3-Aug</span></span> | <span data-ttu-id="250e7-136">29</span><span class="sxs-lookup"><span data-stu-id="250e7-136">29</span></span> | <span data-ttu-id="250e7-137">21.39</span><span class="sxs-lookup"><span data-stu-id="250e7-137">21.39</span></span> | <span data-ttu-id="250e7-138">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="250e7-138">0.737586206896552</span></span> |
| <span data-ttu-id="250e7-139">10 de agosto</span><span class="sxs-lookup"><span data-stu-id="250e7-139">10-Aug</span></span> | <span data-ttu-id="250e7-140">210.950039</span><span class="sxs-lookup"><span data-stu-id="250e7-140">210.950039</span></span> | <span data-ttu-id="250e7-141">155.63</span><span class="sxs-lookup"><span data-stu-id="250e7-141">155.63</span></span> | <span data-ttu-id="250e7-142">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="250e7-142">0.737757626107858</span></span> |
| <span data-ttu-id="250e7-143">25 de agosto</span><span class="sxs-lookup"><span data-stu-id="250e7-143">25-Aug</span></span> | <span data-ttu-id="250e7-144">555.950039</span><span class="sxs-lookup"><span data-stu-id="250e7-144">555.950039</span></span> | <span data-ttu-id="250e7-145">410.17</span><span class="sxs-lookup"><span data-stu-id="250e7-145">410.17</span></span> | <span data-ttu-id="250e7-146">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="250e7-146">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="250e7-147">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="250e7-147">Next steps</span></span>

- [<span data-ttu-id="250e7-148">Facturación e impuestos</span><span class="sxs-lookup"><span data-stu-id="250e7-148">Billing and taxes</span></span>](billing.md)
