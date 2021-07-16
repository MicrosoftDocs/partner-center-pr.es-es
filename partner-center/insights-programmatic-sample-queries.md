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
# <a name="sample-queries-for-partner-center-insights-report"></a>Consultas de ejemplo para Centro de partners insights

En este artículo se proporcionan consultas de ejemplo para los informes Ideas asociados. Puede usar estas consultas llamando al punto de conexión de la API de Creación de consultas de informe. Si es necesario, la [llamada API Crear](insights-programmatic-access-paradigm.md#create-report-query-api) consulta de informe se puede modificar para agregar más columnas, ajustar el período de cálculo y agregar condiciones de filtro.

Para obtener más información sobre los nombres de columna, los atributos y las descripciones, consulte [Definiciones de datos](insights-data-definitions.md).

## <a name="customer-details"></a>Detalles del cliente

Estas consultas de ejemplo se aplican al informe de detalles de los clientes:

### <a name="by-geography"></a>Por geografía

Lista de clientes de una ubicación geográfica específica del mes pasado.

```sql
SELECT CustomerName, CustomerTpid, Product 
FROM CustomersAndTenants 
WHERE CustomerMarket='United States' TIMESPAN LAST_MONTH
```

### <a name="by-sku-and-billed-revenue"></a>Por SKU e ingresos facturados

La lista de clientes que usan SKU y ingresos facturados específicos es superior a 20 000 en los últimos 6 meses

```sql
SELECT CustomerName, CustomerTpid, SKU, Month, BilledRevenueUSD 
FROM CustomersAndTenants 
WHERE SKU='MICROSOFT 365 BUSINESS STANDARD' AND BilledRevenueUSD>20000 TIMESPAN LAST_6_MONTHS
```

### <a name="by-available-seats"></a>Por puestos disponibles

10 clientes principales según los puestos disponibles del mes pasado

```sql
SELECT CustomerName, CustomerTpid, Product, AvailableSeats 
FROM CustomersAndTenants ORDER BY AvailableSeats DESC LIMIT 10 TIMESPAN LAST_MONTH
```

## <a name="partner-profile"></a>Perfil de partner

Estas consultas de ejemplo se aplican al informe de perfil de asociado:

### <a name="by-geography"></a>Por geografía

Lista de asociados de una ubicación geográfica específica.

```sql
SELECT MPNId, PartnerName 
FROM Profile 
WHERE Country='United States'
```

### <a name="by-mpn-partner"></a>Por asociado de MPN

Lista de asociados en el mismo asociado de MPN de PGA

```sql
SELECT MPNId, PartnerName, PGAMpnId 
FROM Profile 
WHERE PGAMpnId='1001xx'
```

## <a name="reseller-performance"></a>Rendimiento del revendedor

Estas consultas de ejemplo se aplican al informe de rendimiento del revendedor:

### <a name="by-geography"></a>Por geografía

Lista de revendedores de una ubicación geográfica específica del mes pasado.

```sql
SELECT ResellerMpnId, ResellerName 
FROM ResellerPerformance 
WHERE ResellerMarket='US' TIMESPAN LAST_MONTH
```

### <a name="by-reseller"></a>Por revendedor

Recuento de clientes, número de suscripciones, puestos disponibles totales, puestos asignados totales, ingresos totales de un revendedor específico.

```sql
SELECT ResellerMpnId, ResellerName, CustomerCount, SubscriptionCount, TotalAvailableSeats, TotalAssignedSeats, TotalRevenue 
FROM ResellerPerformance 
WHERE ResellerMpnId='1051xxx'
```

### <a name="top-10-by-revenue"></a>10 principales por ingresos

Los 10 principales revendedores en función de los ingresos totales del mes pasado.

```sql
SELECT ResellerMpnId, ResellerName, TotalRevenue 
FROM ResellerPerformance 
ORDER BY TotalRevenue 
LIMIT 10 
TIMESPAN LAST_MONTH
```

## <a name="subscription-details"></a>Detalles de la suscripción

Estas consultas de ejemplo se aplican al informe de detalles de la suscripción:

### <a name="by-renewal-eligibility"></a>Por elegibilidad de renovación

Lista de suscripciones que no son aptas para la renovación automática en el último mes.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE IsAutoRenew='N' TIMESPAN LAST_MONTH
```

### <a name="by-subscription-state"></a>Por estado de suscripción

Lista de suscripciones que están en estado Deshabilitar en el mes pasado.

```sql
SELECT SubscriptionId, SubscriptionEndDate, CustomerName, CustomerTpid, Product 
FROM SeatsSubscriptionsAndRevenue 
WHERE SubscriptionState='Disabled' TIMESPAN LAST_MONTH
```

### <a name="counts-for-six-months"></a>Recuentos durante seis meses

Recuento de suscripciones, puestos vendidos totales, recuento de clientes de un asociado específico en los últimos seis meses.

```sql
SELECT MPNId, SubscriptionCount, TotalSoldSeats, BilledRevenueUSD, CustomerCount 
FROM SeatsSubscriptionsAndRevenue 
WHERE MPNId=6096xxx TIMESPAN LAST_6_MONTHS
```

## <a name="azure-usage"></a>Uso de Azure

Estas consultas de ejemplo se aplican al informe de uso de Azure:

### <a name="by-meter-category"></a>Por categoría de medidor

Lista de suscripciones de uso de Azure con unidades de uso y ACR para la categoría de medidores específicos en los últimos seis meses.

```sql
SELECT SubscriptionId, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE MeterCategory='Azure DNS' 
TIMESPAN LAST_6_MONTHS
```

### <a name="by-total-acr"></a>Por ACR total

Lista de suscripciones de uso de Azure donde el total de ACR es superior a 20 000 en los últimos seis meses

```sql
SELECT SubscriptionId, ServiceName, CustomerName, Month, UsageUnits, UsageQuantity, TotalACR 
FROM AzureUsage 
WHERE TotalACR>20000 TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a>Pasos siguientes

- [API para acceder a los datos de análisis de Partner Insights](insights-programmatic-analytics-available-api.md)