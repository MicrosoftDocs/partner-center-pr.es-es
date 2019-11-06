---
title: Lista de precios del plan de Azure | Centro de partners
ms.topic: article
ms.date: 11/01/2019
description: Cómo ver la lista de precios de las suscripciones en el plan de Azure
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: 53e5327b505de1c1860e44b477aca21b5aef2d2b
ms.sourcegitcommit: 646536a113584f1572de851e22a212a6f77e64d7
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/01/2019
ms.locfileid: "73428547"
---
# <a name="price-list-for-the-new-commerce-experience-in-csp-for-azure"></a>Lista de precios para la nueva experiencia comercial en CSP para Azure 

La lista de precios para la nueva experiencia comercial de Azure en CSP se publica en el Centro de partners. Asimismo, esta lista de precios se entrega dinámicamente en un archivo preciso en tiempo real y los precios se muestran solo en USD. Sin embargo, la facturación se realiza en la moneda admitida aplicable a la ubicación de la moneda del cliente. Para obtener más información sobre la facturación en la ubicación de la moneda del cliente, consulta [Plan de Azure: facturación](azure-plan-billing.md).

## <a name="see-pricing-for-subscriptions-under-the-azure-plan-pricing"></a>Consulta los precios de las suscripciones en los precios del plan de Azure

1. En el menú del Centro de partners a la izquierda, selecciona **Sell** (Vender) y **Marketplace**.

2. Junto a **Export type** (Tipo de exportación), selecciona **Azure plan consumption pricing** (Precios de consumo del plan de Azure).

3. Junto a **Pricing for date** (Precios en función de la fecha), selecciona la fecha que quieras; por ejemplo, **Current** (Actual). Nota: También puedes seleccionar los **tipos de cambio** para exportar los tipos de cambio actuales.

![Precios de Azure 2](images/azure/pricelist2.jpg)

4. En **Marketplace**, selecciona el **tipo**  y la **categoría**  del producto o busca un producto. Se mostrarán los productos disponibles basados en tu búsqueda.

![pricing](images/azure/Azurepricelist1.jpg)

5. A continuación, selecciona **Export Azure plan price list** (Exportar lista de precios del plan de Azure) para descargar los precios del plan de Azure referentes a los productos que selecciones.


![exportar lista de precios](images/azure/pricelist1.png)



## <a name="azure-price-list-specifics"></a>Detalles de la lista de precios de Azure

- Los precios del plan de Azure estarán disponibles en la página de Marketplace del Centro de partners, en la opción **Sell** (Vender).

- Las exportaciones estarán disponibles para los servicios de consumo del plan de Azure, Azure Reservations y los tipos de cambio.

- Las opciones de exportación incluyen:

    - **Precios de hoy**: Esto incluye todos los medidores y precios desde el día 1 de cada mes hasta la fecha actual del mes actual. Esto incluye precios nuevos, precios modificados o precios eliminados. Todos los precios tendrán fechas de inicio y finalización efectivas para así poder indicar si son nuevos o si se han eliminado.

    - **Precios del mes anterior**: Las descargas de cada tipo de recurso serán mensuales. En cuanto a los archivos de precios, esto incluirá todos los medidores que estuvieron disponibles durante ese mes. Si apareció un nuevo medidor a mediados de mes,se mostrará como un medidor con una fecha de vigencia que refleje su disponibilidad. Esto es similar en precios descontinuados, que se muestran con una fecha de finalización efectiva que describe el momento en el que dejan de estar disponibles.

    - **Tipos de cambio**: Los tipos de cambio estarán disponibles para descargar el día anterior al 1 de cada mes, a las 6 p.m., PST. Por ejemplo, si quieres las tarifas de noviembre, puedes descargarlas el 31 de octubre. El tipo de cambio del mes anterior también estará disponible.

- Recuerda que los precios de las listas de precios son precios directos. Algunos partners pueden optar a los créditos que obtienen los partners. Para obtener información sobre cómo se calcula el crédito que obtienen los partners consulta [Cómo se calcula y paga el crédito que obtiene el partner](partner-earned-credit-explanation.md).

- **Servicios elegibles**: El crédito que obtienen los partners se aplica a los servicios enumerados en los **precios de consumo del plan de Azure** que los partners pueden exportar desde la página de [precios del plan de Azure](https://partner.microsoft.com/commerce/sales). Ten en cuenta que hay excepciones que incluyen, sin limitación, productos de terceros identificados como "Tercero" en la columna Etiquetas de la lista de precios de consumo del plan de Azure y las reservas del plan de Azure.

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

Obtener [información detallada de la lista de precios](https://partner.microsoft.com/commerce/sales?type=Any&category=Any)  
