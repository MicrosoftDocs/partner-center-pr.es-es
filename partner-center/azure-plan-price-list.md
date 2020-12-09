---
title: Lista de precios del plan de Azure para partners de CSP
ms.topic: how-to
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtén información sobre cómo los partners del programa CSP pueden usar el Centro de partners para ver la lista de precios de las suscripciones en el plan de Azure.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 02cea980626ec32d3dd60f646b1f8744130792ea
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534733"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Lista de precios para la nueva experiencia comercial en CSP para Azure

**Roles adecuados**

- Agente de administrador
- Administrador de facturación
- Administrador global
- Agente del departamento de soporte técnico
- Agente de ventas
- Administrador del control de usuarios

La lista de precios para la nueva experiencia comercial de Azure en CSP se publica en el Centro de partners. Asimismo, esta lista de precios se entrega dinámicamente en un archivo preciso en tiempo real y los precios se muestran solo en USD. Sin embargo, la facturación se realiza en la moneda admitida aplicable a la ubicación de la moneda del cliente. Para obtener más información sobre la facturación en la ubicación de la moneda del cliente, consulta [Plan de Azure: facturación](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Consulta los precios de las suscripciones en los precios del plan de Azure

1. En el menú del Centro de partners a la izquierda, selecciona **Sell** (Vender) y **Marketplace**.

2. En los precios del plan de Azure, selecciona el país para el que quieres obtener los precios.

3. Junto a **Tipo de exportación**, selecciona **Precios del consumo del plan de Azure**, **Precios de las reservas del plan de Azure** o **Tipos de cambio**. 

>[!NOTE] 
>Los **Tipos de cambio** no son específicos del país.

4. Junto a **Pricing for date** (Precios en función de la fecha), selecciona la fecha que quieras; por ejemplo, **Current** (Actual).

   :::image type="content" source="images/azure/pricingnew.png" alt-text="Específico del país":::

>[!NOTE] 
>Puedes exportar dos listas de precios diferentes: precios del plan de Azure y precios de terceros de Marketplace.

## <a name="azure-price-list-specifics"></a>Detalles de la lista de precios de Azure

- Los precios del plan de Azure estarán disponibles en la página de Marketplace del Centro de partners, en la opción **Sell** (Vender).

- Las exportaciones estarán disponibles para los servicios de consumo del plan de Azure, Azure Reservations y los tipos de cambio.

- Las opciones de exportación incluyen:

  - **Precios de hoy**: Esto incluye todos los medidores y precios desde el día 1 de cada mes hasta la fecha actual del mes actual. Esto incluye precios nuevos, precios modificados o precios eliminados. Todos los precios tendrán fechas de inicio y finalización efectivas para así poder indicar si son nuevos o si se han eliminado.

  - **Precios del mes anterior**: Las descargas de cada tipo de recurso serán mensuales. En cuanto a los archivos de precios, esto incluirá todos los medidores que estuvieron disponibles durante ese mes. Si apareció un nuevo medidor a mediados de mes, se mostrará como un medidor con una fecha de vigencia que refleje su disponibilidad. Esto es similar en precios descontinuados, que se muestran con una fecha de finalización efectiva que describe el momento en el que dejan de estar disponibles.

  - **Tipos de cambio**: Los tipos de cambio estarán disponibles para descargar el día anterior al 1 de cada mes, a las 6 p.m., PST. Por ejemplo, si quieres las tarifas de noviembre, puedes descargarlas el 31 de octubre. El tipo de cambio del mes anterior también estará disponible.

- Recuerda que los precios de las listas de precios son precios directos. Algunos partners pueden optar a los créditos que obtienen los partners. Para obtener información sobre cómo se calcula el crédito que obtienen los partners consulta [Cómo se calcula y paga el crédito que obtiene el partner](partner-earned-credit-explanation.md).

- **Servicios elegibles**: El crédito que obtienen los partners se aplica a los servicios enumerados en los **precios de consumo del plan de Azure** que los partners pueden exportar desde la página de [precios del plan de Azure](https://partner.microsoft.com/commerce/sales). Ten en cuenta que hay excepciones que incluyen, sin limitación, productos de terceros identificados como "Tercero" en la columna Etiquetas de la lista de precios del consumo del plan de Azure y las reservas del plan de Azure.

## <a name="price-list-data"></a>Datos de la lista de precios

|**Campo**   |**Descripción**   |
|--------------------------|:---------------------------|
|ProductTitle  |Título o nombre del producto|
|ProductID   |Id. de producto|
|SKuId|Id. de SKU|
|SkuTitle|Título o nombre de la SKU|
|Publicador|Microsoft siempre será la parte principal|
|SkuDescription|Descripción de la SKU|
|UnitOfMeasure|Las unidades que se cobrarán o facturarán|
|TermDuration|En el caso de los productos basados en períodos, esta es la duración del período que es aplicable a las reservas|
|Mercado|Mercado de precios|
|Moneda|Moneda de los precios|
|UnitPrice|Precio por unidad|
|PricingTierRangeMin|En cuanto a los planes de tarifa, se aplica el precio mínimo|
|PricingTierRangeMax|En cuanto a los planes de tarifa, se aplica el precio máximo|
|EffectiveStartDate|Fecha de inicio del precio|
|EffectiveEndDate|Fecha de finalización del precio|
|MeterIds|Id. del medidor de la SKU de producto|
|MeterType|Tipo de medidor|
|Etiquetas|Propiedades del producto; en cuanto al precio del plan de Azure, este será Azure o Azure y reservas (para reservas específicamente)|

Las listas de precios del plan de Azure se pueden exportar desde la [página de precios y ofertas](https://partner.microsoft.com/dashboard/sell/pricingandoffers) del Centro de partners.

## <a name="tiered-pricing"></a>Planes de tarifa

Algunos servicios de consumo de plan de Azure admiten los planes de tarifa. Los partners pueden encontrar estos productos y SKU en la lista de precios del plan de Azure. Los elementos que tienen valores en las columnas de rango de plan de tarifa permiten a los partners comprender el precio según el uso. En el siguiente ejemplo en el que se usan datos de ejemplo tenemos una SKU de producto con tres planes de tarifa.

|**ProductId**   |**SkuId**   |**UnitPrice**   |**PricingTierRangeMin**   |**PricingTierRangeMax**   |
|:---------------|:-----------|:---------------|:-------------------------|:-------------------------|
|DDD123456ABC|01AB|0,50|100001|9223372036854780000|
|DDD123456ABC|01AB|0,80|101|100000|
|DDD123456ABC|01AB|1|1|100|

En este ejemplo, si se usan 101 unidades, el cargo sería 100,80. Las 100 primeras unidades son a 1 cada una y la siguiente unidad se cobra a 0,80.

## <a name="pricing-api-for-azure-plan"></a>API de precios para el plan de Azure

Puedes usar la [API de precios](/partner/develop/pricing) a fin de recuperar los precios del plan de Azure para el consumo y las reservas mediante programación. También puedes recuperar tasas de cambio de divisas.

La API de precios se encuentra en un punto de conexión diferente del de las otras API del Centro de partners. La información de precios incluye los precios en USD de los medidores de los recursos del plan de Azure y los precios de las reservas aplicados a las suscripciones al plan de Azure.

Esta API también permite a los partners recuperar las tasas de cambio mensuales, ya que los precios del plan de Azure solo se ofrecen en USD. Puedes usar las API para recuperar los precios y las tasas de cambio de divisas del mes actual o los meses anteriores.

>[!NOTE]
> La API de precios es específica de los precios del plan de Azure. En el caso de los recursos o las reservas de Azure implementadas en suscripciones a planes que no son de Azure, igualmente debes usar la API de RateCard existente y las listas de precios publicadas en la página "Precios y ofertas" del Centro de partners. La API de precios del plan de Azure no admite precios basados en software, Marketplace o licencias, como Microsoft 365 o Dynamics 365.

Para obtener más información sobre los precios del plan de Azure y las API de tasas de cambio de divisas, consulta la [documentación de la API de precios](/partner/develop/pricing) completa.

## <a name="next-steps"></a>Pasos siguientes

- [Administrar suscripciones y recursos en el plan de Azure](azure-plan-manage.md)