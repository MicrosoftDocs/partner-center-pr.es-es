---
title: Lista de consultas de ejemplo
description: Use las consultas de ejemplo para acceder mediante programación a los datos de análisis de Conclusiones de asociados.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: e25784585a1ac505db99e58265939a8851edcbad
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375853"
---
# <a name="sample-queries-for-partner-center-insights-report"></a><span data-ttu-id="f961e-103">Consultas de ejemplo para Centro de partners insights</span><span class="sxs-lookup"><span data-stu-id="f961e-103">Sample queries for Partner Center insights report</span></span>

<span data-ttu-id="f961e-104">En este artículo se proporcionan consultas de ejemplo para los informes Ideas asociados.</span><span class="sxs-lookup"><span data-stu-id="f961e-104">This article provides sample queries for the Partner Insights reports.</span></span> <span data-ttu-id="f961e-105">Puede usar estas consultas llamando al punto de conexión de la API de Creación de consultas de informe.</span><span class="sxs-lookup"><span data-stu-id="f961e-105">You can use these queries by calling the Create Report Query API endpoint.</span></span> <span data-ttu-id="f961e-106">Si es necesario, la [llamada API Crear](insights-programmatic-access-paradigm.md#create-report-query-api) consulta de informe se puede modificar para agregar más columnas, ajustar el período de cálculo y agregar condiciones de filtro.</span><span class="sxs-lookup"><span data-stu-id="f961e-106">If necessary, the [Create Report Query API](insights-programmatic-access-paradigm.md#create-report-query-api) call can be modified to add more columns, adjust the computation period, and add filter conditions.</span></span>

<span data-ttu-id="f961e-107">Para obtener más información sobre los nombres de columna, los atributos y las descripciones, consulte [Definiciones de datos](insights-data-definitions.md).</span><span class="sxs-lookup"><span data-stu-id="f961e-107">For details about the column names, attributes, and descriptions, refer to the [Data Definitions](insights-data-definitions.md).</span></span>

## <a name="customer-details"></a><span data-ttu-id="f961e-108">Detalles del cliente</span><span class="sxs-lookup"><span data-stu-id="f961e-108">Customer details</span></span>

<span data-ttu-id="f961e-109">Estas consultas de ejemplo se aplican al informe de detalles de los clientes:</span><span class="sxs-lookup"><span data-stu-id="f961e-109">These sample queries apply to the customers details report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="f961e-110">Por geografía</span><span class="sxs-lookup"><span data-stu-id="f961e-110">By geography</span></span>

<span data-ttu-id="f961e-111">Lista de clientes de una ubicación geográfica específica del mes pasado.</span><span class="sxs-lookup"><span data-stu-id="f961e-111">List of customers from a specific geography in last month.</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a><span data-ttu-id="f961e-112">Por SKU e ingresos facturados</span><span class="sxs-lookup"><span data-stu-id="f961e-112">By SKU and billed revenue</span></span>

<span data-ttu-id="f961e-113">La lista de clientes que usan SKU y ingresos facturados específicos es superior a 20 000 en los últimos 6 meses</span><span class="sxs-lookup"><span data-stu-id="f961e-113">List of customers using specific SKU and Billed Revenue is more than 20,000 in the last 6 months</span></span>

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a><span data-ttu-id="f961e-114">Por puestos disponibles</span><span class="sxs-lookup"><span data-stu-id="f961e-114">By available seats</span></span>

<span data-ttu-id="f961e-115">10 clientes principales según los puestos disponibles del mes pasado</span><span class="sxs-lookup"><span data-stu-id="f961e-115">Top 10 customers based on Available seats in last month</span></span>

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a><span data-ttu-id="f961e-116">Perfil de partner</span><span class="sxs-lookup"><span data-stu-id="f961e-116">Partner Profile</span></span>

<span data-ttu-id="f961e-117">Estas consultas de ejemplo se aplican al informe de perfil de asociado:</span><span class="sxs-lookup"><span data-stu-id="f961e-117">These sample queries apply to the partner profile report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="f961e-118">Por geografía</span><span class="sxs-lookup"><span data-stu-id="f961e-118">By geography</span></span>

<span data-ttu-id="f961e-119">Lista de asociados de una ubicación geográfica específica.</span><span class="sxs-lookup"><span data-stu-id="f961e-119">List of partners from a specific geography.</span></span>

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a><span data-ttu-id="f961e-120">Por asociado de MPN</span><span class="sxs-lookup"><span data-stu-id="f961e-120">By MPN partner</span></span>

<span data-ttu-id="f961e-121">Lista de asociados en el mismo asociado de MPN de PGA</span><span class="sxs-lookup"><span data-stu-id="f961e-121">List of partners under same PGA MPN Partner</span></span>

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a><span data-ttu-id="f961e-122">Rendimiento del revendedor</span><span class="sxs-lookup"><span data-stu-id="f961e-122">Reseller Performance</span></span>

<span data-ttu-id="f961e-123">Estas consultas de ejemplo se aplican al informe de rendimiento del revendedor:</span><span class="sxs-lookup"><span data-stu-id="f961e-123">These sample queries apply to the reseller performance report:</span></span>

### <a name="by-geography"></a><span data-ttu-id="f961e-124">Por geografía</span><span class="sxs-lookup"><span data-stu-id="f961e-124">By geography</span></span>

<span data-ttu-id="f961e-125">Lista de revendedores de una ubicación geográfica específica del mes pasado.</span><span class="sxs-lookup"><span data-stu-id="f961e-125">List of resellers from a specific geography in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a><span data-ttu-id="f961e-126">Por revendedor</span><span class="sxs-lookup"><span data-stu-id="f961e-126">By reseller</span></span>

<span data-ttu-id="f961e-127">Recuento de clientes, número de suscripciones, puestos disponibles totales, puestos asignados totales, ingresos totales de un revendedor específico.</span><span class="sxs-lookup"><span data-stu-id="f961e-127">Customer count, subscription count, total available seats, total assigned seats, total revenue for a specific reseller.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a><span data-ttu-id="f961e-128">10 principales por ingresos</span><span class="sxs-lookup"><span data-stu-id="f961e-128">Top 10 by revenue</span></span>

<span data-ttu-id="f961e-129">Los 10 principales revendedores en función de los ingresos totales del mes pasado.</span><span class="sxs-lookup"><span data-stu-id="f961e-129">Top 10 resellers based on total revenue in last month.</span></span>

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a><span data-ttu-id="f961e-130">Detalles de la suscripción</span><span class="sxs-lookup"><span data-stu-id="f961e-130">Subscription Details</span></span>

<span data-ttu-id="f961e-131">Estas consultas de ejemplo se aplican al informe de detalles de la suscripción:</span><span class="sxs-lookup"><span data-stu-id="f961e-131">These sample queries apply to the subscription details report:</span></span>

### <a name="by-renewal-eligibility"></a><span data-ttu-id="f961e-132">Por elegibilidad de renovación</span><span class="sxs-lookup"><span data-stu-id="f961e-132">By renewal eligibility</span></span>

<span data-ttu-id="f961e-133">Lista de suscripciones que no son aptas para la renovación automática en el último mes.</span><span class="sxs-lookup"><span data-stu-id="f961e-133">List of subscriptions who are not eligible for auto renewal in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a><span data-ttu-id="f961e-134">Por estado de suscripción</span><span class="sxs-lookup"><span data-stu-id="f961e-134">By subscription state</span></span>

<span data-ttu-id="f961e-135">Lista de suscripciones que están en estado Deshabilitar en el mes pasado.</span><span class="sxs-lookup"><span data-stu-id="f961e-135">List of subscriptions who are in Disable state in last month.</span></span>

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a><span data-ttu-id="f961e-136">Recuentos durante seis meses</span><span class="sxs-lookup"><span data-stu-id="f961e-136">Counts for six months</span></span>

<span data-ttu-id="f961e-137">Recuento de suscripciones, puestos vendidos totales, recuento de clientes de un asociado específico en los últimos seis meses.</span><span class="sxs-lookup"><span data-stu-id="f961e-137">Subscription count, total sold seats, customer count for a specific partner in last six months.</span></span>

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a><span data-ttu-id="f961e-138">Uso de Azure</span><span class="sxs-lookup"><span data-stu-id="f961e-138">Azure Usage</span></span>

<span data-ttu-id="f961e-139">Estas consultas de ejemplo se aplican al informe de uso de Azure:</span><span class="sxs-lookup"><span data-stu-id="f961e-139">These sample queries apply to the Azure usage report:</span></span>

### <a name="by-meter-category"></a><span data-ttu-id="f961e-140">Por categoría de medidor</span><span class="sxs-lookup"><span data-stu-id="f961e-140">By meter category</span></span>

<span data-ttu-id="f961e-141">Lista de suscripciones de uso de Azure con unidades de uso y ACR para la categoría de medidores específicos en los últimos seis meses.</span><span class="sxs-lookup"><span data-stu-id="f961e-141">List of Azure usage subscriptions with usage units and ACR for specific meter category in last six months.</span></span>

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a><span data-ttu-id="f961e-142">Por ACR total</span><span class="sxs-lookup"><span data-stu-id="f961e-142">By total ACR</span></span>

<span data-ttu-id="f961e-143">Lista de suscripciones de uso de Azure donde el total de ACR es superior a 20 000 en los últimos seis meses</span><span class="sxs-lookup"><span data-stu-id="f961e-143">List of Azure usage subscriptions where total ACR is greater than 20,000 in last six months</span></span>

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="f961e-144">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="f961e-144">Next steps</span></span>

- [<span data-ttu-id="f961e-145">API para acceder a los datos de análisis de Partner Insights</span><span class="sxs-lookup"><span data-stu-id="f961e-145">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)