---
title: Cálculo del precio de unidad efectivo
ms.topic: how-to
ms.date: 11/10/2020
description: Obtenga información sobre la unidad de precio efectiva y cómo se calcula. Incluye un cálculo de ejemplo.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7b65a79232656af6ddb69fede7a9ee35fe426a9d
ms.sourcegitcommit: 95a5afdf68d88b6be848729830dcd114e3fb0c0f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/11/2020
ms.locfileid: "94498580"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a><span data-ttu-id="73ce6-104">Cálculo de precio por unidad efectivo para el consumo de planes de Azure</span><span class="sxs-lookup"><span data-stu-id="73ce6-104">Effective unit price calculation for Azure plan consumption</span></span>

## <a name="the-effective-unit-price"></a><span data-ttu-id="73ce6-105">El precio unitario efectivo</span><span class="sxs-lookup"><span data-stu-id="73ce6-105">The effective unit price</span></span>

<span data-ttu-id="73ce6-106">El precio unitario efectivo se calcula en el nivel de medidor (en lugar del nivel de recurso) y se ajusta diariamente según el uso del medidor.</span><span class="sxs-lookup"><span data-stu-id="73ce6-106">The effective unit price is calculated at the meter level (as opposed to the resource level), and is adjusted daily according to meter usage.</span></span>

<span data-ttu-id="73ce6-107">Calculamos el precio unitario efectivo mediante los tres factores siguientes:</span><span class="sxs-lookup"><span data-stu-id="73ce6-107">We calculate the effective unit price using the following three factors:</span></span>

- <span data-ttu-id="73ce6-108">Consumo, que se supervisa diariamente a lo largo del ciclo de facturación</span><span class="sxs-lookup"><span data-stu-id="73ce6-108">Consumption, which is monitored daily throughout the billing cycle</span></span>
- <span data-ttu-id="73ce6-109">Costo facturable del medidor</span><span class="sxs-lookup"><span data-stu-id="73ce6-109">Billable cost for the meter</span></span>
- <span data-ttu-id="73ce6-110">Organización en niveles (si es aplicable)</span><span class="sxs-lookup"><span data-stu-id="73ce6-110">Tiering (if applicable)</span></span>

<span data-ttu-id="73ce6-111">Dado que supervisamos el consumo diariamente a lo largo del ciclo de facturación, el precio de la unidad efectiva fluctuará.</span><span class="sxs-lookup"><span data-stu-id="73ce6-111">Because we monitor consumption daily throughout the billing cycle, the effective unit price will fluctuate.</span></span> <span data-ttu-id="73ce6-112">El precio final de un ciclo de facturación determinado estará disponible después de detener el cálculo de consumo y cerrar el período de facturación.</span><span class="sxs-lookup"><span data-stu-id="73ce6-112">The final price for a given billing cycle will be available after we stop the consumption calculation and close the billing period.</span></span> <span data-ttu-id="73ce6-113">Verá la mayoría de los cambios de consumo después de la cuarta o quinta posición decimal.</span><span class="sxs-lookup"><span data-stu-id="73ce6-113">You’ll see most changes in consumption after the fourth or fifth decimal place.</span></span>

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a><span data-ttu-id="73ce6-114">Averigüe si su medidor usa precios por niveles</span><span class="sxs-lookup"><span data-stu-id="73ce6-114">Find out whether your meter uses tiered pricing</span></span>

<span data-ttu-id="73ce6-115">Si no sabe si el medidor usa precios por niveles, use el procedimiento siguiente para averiguarlo.</span><span class="sxs-lookup"><span data-stu-id="73ce6-115">If you don’t know whether your meter uses tiered pricing, use the procedure below to find out.</span></span> 

1. <span data-ttu-id="73ce6-116">Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="73ce6-116">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>
2. <span data-ttu-id="73ce6-117">Seleccione **vender** , seleccione **precios y ofertas** y, luego, seleccione **precios del plan de Azure**.</span><span class="sxs-lookup"><span data-stu-id="73ce6-117">Select **Sell** , select **Pricing and offers** , and then select **Azure plan pricing**.</span></span>
3. <span data-ttu-id="73ce6-118">Busque el medidor según el identificador y, a continuación, descargue los datos de precios.</span><span class="sxs-lookup"><span data-stu-id="73ce6-118">Locate your meter by ID, and then download your pricing data.</span></span> 

## <a name="sample-calculation"></a><span data-ttu-id="73ce6-119">Cálculo de ejemplo</span><span class="sxs-lookup"><span data-stu-id="73ce6-119">Sample calculation</span></span>

<span data-ttu-id="73ce6-120">En la tabla siguiente se ofrece un ejemplo de cómo se calcula el precio unitario efectivo durante el período abierto.</span><span class="sxs-lookup"><span data-stu-id="73ce6-120">The table below gives an example of how we calculate the effective unit price during the open period.</span></span>

<span data-ttu-id="73ce6-121">En la tabla se aplican los siguientes valores:</span><span class="sxs-lookup"><span data-stu-id="73ce6-121">In the table, the following values apply:</span></span> 

- <span data-ttu-id="73ce6-122">**Up** = precio unitario del recurso/hora = 0,868</span><span class="sxs-lookup"><span data-stu-id="73ce6-122">**UP** = Unit price of the resource/hour = 0.868</span></span>

- <span data-ttu-id="73ce6-123">**BCU** = unidad de consumo facturable para el medidor</span><span class="sxs-lookup"><span data-stu-id="73ce6-123">**BCU** = Billable consumption unit for the meter</span></span>

- <span data-ttu-id="73ce6-124">**BC** = costo facturable para el medidor = BCU \* UP \* 0,85.</span><span class="sxs-lookup"><span data-stu-id="73ce6-124">**BC** = Billable cost for the meter = BCU \* UP \* 0.85.</span></span> <span data-ttu-id="73ce6-125">Esto refleja un ajuste para el 15% de descuento de PEC.</span><span class="sxs-lookup"><span data-stu-id="73ce6-125">This reflects an adjustment for the 15% PEC discount.</span></span> <span data-ttu-id="73ce6-126">A continuación, usamos el límite inferior de la función para limitar el valor a dos dígitos después del separador decimal, con el fin de cobrar la cantidad mínima.</span><span class="sxs-lookup"><span data-stu-id="73ce6-126">We then use the lower limit of the function to limit the value to two digits after the decimal point, in order to charge the minimum amount.</span></span> 

- <span data-ttu-id="73ce6-127">**Precio por unidad vigente** = BCU/BC</span><span class="sxs-lookup"><span data-stu-id="73ce6-127">**Effective unit price** = BCU/BC</span></span>

>[!NOTE]
><span data-ttu-id="73ce6-128">Nota: el medidor de este ejemplo no tiene niveles en los precios.</span><span class="sxs-lookup"><span data-stu-id="73ce6-128">Note: The meter in this example does not have tiers in pricing.</span></span>

| <span data-ttu-id="73ce6-129">Date</span><span class="sxs-lookup"><span data-stu-id="73ce6-129">Date</span></span> | <span data-ttu-id="73ce6-130">BCU (unidad de consumo facturable)</span><span class="sxs-lookup"><span data-stu-id="73ce6-130">BCU (Billable consumption unit)</span></span> | <span data-ttu-id="73ce6-131">BC (costo facturable)</span><span class="sxs-lookup"><span data-stu-id="73ce6-131">BC (Billable cost)</span></span> | <span data-ttu-id="73ce6-132">Precio unitario efectivo</span><span class="sxs-lookup"><span data-stu-id="73ce6-132">Effective unit price</span></span> |
| ------ | ----------- | ----------- | ----------- |  
| <span data-ttu-id="73ce6-133">3-ago</span><span class="sxs-lookup"><span data-stu-id="73ce6-133">3-Aug</span></span> | <span data-ttu-id="73ce6-134">29</span><span class="sxs-lookup"><span data-stu-id="73ce6-134">29</span></span> | <span data-ttu-id="73ce6-135">21,39</span><span class="sxs-lookup"><span data-stu-id="73ce6-135">21.39</span></span> | <span data-ttu-id="73ce6-136">0.737586206896552</span><span class="sxs-lookup"><span data-stu-id="73ce6-136">0.737586206896552</span></span> |
| <span data-ttu-id="73ce6-137">10-ago</span><span class="sxs-lookup"><span data-stu-id="73ce6-137">10-Aug</span></span> | <span data-ttu-id="73ce6-138">210,950039</span><span class="sxs-lookup"><span data-stu-id="73ce6-138">210.950039</span></span> | <span data-ttu-id="73ce6-139">155,63</span><span class="sxs-lookup"><span data-stu-id="73ce6-139">155.63</span></span> | <span data-ttu-id="73ce6-140">0.737757626107858</span><span class="sxs-lookup"><span data-stu-id="73ce6-140">0.737757626107858</span></span> |
| <span data-ttu-id="73ce6-141">25-ago</span><span class="sxs-lookup"><span data-stu-id="73ce6-141">25-Aug</span></span> | <span data-ttu-id="73ce6-142">555,950039</span><span class="sxs-lookup"><span data-stu-id="73ce6-142">555.950039</span></span> | <span data-ttu-id="73ce6-143">410,17</span><span class="sxs-lookup"><span data-stu-id="73ce6-143">410.17</span></span> | <span data-ttu-id="73ce6-144">0.737782122900436</span><span class="sxs-lookup"><span data-stu-id="73ce6-144">0.737782122900436</span></span> |

## <a name="next-steps"></a><span data-ttu-id="73ce6-145">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="73ce6-145">Next steps</span></span>

- [<span data-ttu-id="73ce6-146">Facturación e impuestos</span><span class="sxs-lookup"><span data-stu-id="73ce6-146">Billing and taxes</span></span>](billing.md)
