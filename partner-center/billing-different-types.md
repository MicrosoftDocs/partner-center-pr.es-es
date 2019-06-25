---
title: Descripción de los tipos de facturación en el centro de partners | Centro de partners
ms.topic: article
ms.date: 03/01/2019
Description: Información sobre los diferentes tipos de facturación, períodos de facturación y las fechas de facturación
author: MaggiePucciEvans
ms.author: evansma
keywords: la facturación, los pagos, pedidos, archivos de conciliación, archivo de conciliación
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 3e664a8a539125bce21d256c6e6d88d1ab22d14d
ms.sourcegitcommit: 1f9078d422af5f8514d79a6ab9c3444500abfe27
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/24/2019
ms.locfileid: "67343453"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Descripción de los tipos de facturación del Centro de partners

**Se aplica a**

-  Centro de partners
-  Asociados en el programa CSP

Según los tipos de productos que compra para sus clientes, podría tener diferentes períodos de facturación y se facturan en días diferentes del mismo mes. En este artículo se explica qué ha cambiado a partir del 1 de marzo de 2019, y cómo le afectará los cambios.

## <a name="billing-for-recurring-charges"></a>Facturación de cargos periódicos

No cambia la experiencia de facturación para los cargos periódicos de suscripciones basadas en licencias y basada en uso. Vamos a seguir para cobrarle el día del mes que seleccionó como la fecha de facturación y el período de facturación seguirán estando mes antes de esa fecha. Si ha seleccionado el día 15 del mes de su fecha de facturación, le facturará para toda la actividad desde el 15 de un mes de calendario para el día 14 del siguiente mes natural. Las facturas y archivos de conciliación son disponible con carácter general 2-4 días después de la fecha de facturación.

Como antes, se le facturará para estos productos en la moneda del país o región en que se encuentra, independientemente de la ubicación del cliente vende el producto.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Facturación de un solo uso y seleccionadas cargos periódicos

A partir del 1 de marzo de 2019, introdujo una nueva experiencia de facturación para los cargos periódicos y un solo uso para productos de Microsoft y terceros ISV.

Para estos productos, el período de facturación se inicia el primer día del mes del calendario y termina en el último día del mes del calendario. Haremos la factura disponible 8 días del mes siguiente. 

En otras palabras, las transacciones que se realice entre el 1 de mayo y el 31 de mayo de 2019 aparecerá en la factura del 8 de junio. Las transacciones que se realice entre el 1 de junio y el 30 de junio de 2019 aparecerá en la factura del 8 de julio. Es posible que le para compras periódicas y única en la misma factura. 

También puede comprobar su saldo de cuenta/factura cada vez que desee (por ejemplo, entre el 1 de mayo y 7 de junio) y ver la actividad más reciente de la cuenta sin tener que esperar la factura. Tenga en cuenta que cuando se publique la factura en los 8, incluirá los impuestos y otros cargos aplicables y créditos, por lo que la cantidad final podría diferir de lo que se ve durante el período de facturación. 

Tendrá acceso a las facturas del mismo modo que ahora, en el centro de partners, o mediante la API. Aparecerán antes de medianoche UTC de 8 días del mes. 

|**Experiencia de facturación**|**Tipos de producto**|**Fecha de facturación**|**Período de facturación**|**Divisa de facturación**|**¿Actividad actual disponible?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Cargos periódicos para las suscripciones basadas en licencias y basada en uso |Todos los productos desde el [catálogo de servicios en línea](https://partner.microsoft.com/commerce/preferredoffers/list). Algunos ejemplos incluyen Office 365, Microsoft 365, Azure Active Directory, Azure (pago por uso), Dynamics 365, Power BI Pro |La fecha seleccionada cuando creaste la cuenta del centro de partners |El mes anterior a la fecha de facturación. |Se encuentra en la moneda del país o región. Por ejemplo, si su empresa se encuentra en el Reino Unido, se le facturará en libras esterlinas (GBP). Si su empresa se encuentra en la India, le facturaremos en la Rupia India (INR).  |No |
|Cargos periódicos y un solo uso para productos de Microsoft y terceros ISV |Todos los SaaS suscripciones, las reservas de Azure y productos de software (perpetuo y basados en suscripción) que ofrece Microsoft e ISV de terceros. Vea los productos disponibles en el [Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Algunos ejemplos son el software de SUSE Linux (suscripción de software), Windows Server 2019 Essentials (software permanente), suscripción de producto de SaaS de ISV de Azure. |8 días de cada mes |Desde el primer día hasta el último día de cada mes natural |La moneda del país o región que el cliente se encuentra en. Esto significa que recibirá facturas independientes y archivos de conciliación en la moneda del país o región cada cliente que se vende a en el período de facturación. |Sí |

## <a name="billing-scenarios-for-one-time-and-recurring-purchases"></a>Escenarios de facturación para las compras periódicas y únicas
### <a name="scenario-1--purchase-a-subscription-and-then-add-a-seat-on-the-same-day"></a>Escenario 1: adquiera una suscripción y, a continuación, agregue una plaza en el mismo día

En el escenario 1, adquirir una suscripción el 11 de junio a un precio unitario de $4. Más tarde ese mismo día comprar otro de la misma suscripción al mismo precio. 

El archivo de conciliación incluirá lo siguiente: 
-   factura de $4 de 10 de junio, 9 de julio de período de servicio. 
-   $4.00 renovación prorrateada por período de servicio 11 de junio – 11 de junio. Este es el período que tenía 1 licencia. Cálculo = (mensual total del precio días en el período de servicio) x días en prorrateada del servicio período x número de licencias = (30/4) x 30 x 1 = 4.00.
-   $8.00 prorratea renovación para un período de servicio en el 10 de junio, 9 de julio. Este es el período que tenía 2 licencias. Cálculo = (30/4) x 30 x 2 = 8.00.

|**Fecha de compra**   |**Inicio de cargo**  |**Final de cargo**  |**Precio por unidad**  |**Cantidad**  |**Cantidad** |**Tipo de gasto** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |1                 |$4            |Nuevo         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$4       |addQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$8         |addQuantity           |

### <a name="scenario-2--purchase-a-subscription-and-then-add-more-later"></a>Escenario 2: adquiera una suscripción y, a continuación, agregar más posteriormente

En el escenario 2, comprar una suscripción de 11 de junio a un precio unitario de $4 y 12 de junio compra otra suscripción para el mismo producto al mismo precio. 

El archivo de conciliación incluirá lo siguiente: 
-   factura de $4 de 10 de junio, 9 de julio de período de servicio. 
-   $3,87 renovación prorrateada por período de servicio 11 de junio – 12 de junio. Este es el período que tenía 1 licencia. Cálculo = (mensual total del precio días en el período de servicio) x días en prorrateada del servicio período x número de licencias = x (30/4) 29 x 1 = 3,87.
-   $7.74 prorratea renovación por período de servicio del 12 de junio, 9 de julio. Este es el período que tenía 2 licencias. Cálculo = x (30/4) 29 x 2 = 7.74.

|**Fecha de compra**   |**Inicio de cargo**  |**Final de cargo**  |**Precio por unidad**  |**Cantidad**  |**Cantidad** |**Tipo de gasto** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (tiene una licencia)     |6/10/2019   |7/09/2019         |$4         |1        |$4            |Nuevo         |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |1        | -$3.87       |addQuantity           |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        | 2      |$7.74       |addQuantity           |

### <a name="scenario-3--purchase-a-subscription-and-then-remove-a-seat-on-the-same-day"></a>Escenario 3: adquiera una suscripción y, a continuación, quitar una plaza en el mismo día

En el escenario 3, comprar dos suscripciones para el mismo producto el 11 de junio a un precio unitario de $4. Más tarde ese mismo día quite uno de los asientos.  

El archivo de conciliación incluirá lo siguiente: 
-   factura de 8 dólares para dos licencias para el período de servicio el 10 de junio, 9 de julio. 
-   $8.00 renovación prorrateada por período de servicio 11 de junio – 11 de junio. Este es el período que tenía 2 licencias. Cálculo = (mensual total del precio días en el período de servicio) x días en prorrateada del servicio período x número de licencias = (30/4) x 30 x 2 = 8.00.
-   $4.00 prorratea renovación durante el 11 de junio, 9 de julio de período de servicio. Este es el período que tenía 1 licencia. Cálculo = (30/4) x 30 x 1 = 4.00.

|**Fecha de compra**   |**Inicio de cargo**  |**Final de cargo**  |**Precio por unidad**  |**Cantidad**  |**Cantidad** |**Tipo de gasto** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019      |6/10/2019   |7/09/2019         |$4                |2                 |$8            |Nuevo         |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$8       |removeQuantity           |
|6/11/2019     | 6/10/2019    |7/09/2019        |$4        | 1      |$4         |removeQuantity           |

### <a name="scenario-4--purchase-a-subscription-and-then-remove-seats-later"></a>Escenario 4: adquiera una suscripción y, a continuación, quitar puestos posteriormente

En la situación 4, adquiere 2 suscripciones el 11 de junio a un precio unitario de $4 y 12 de junio de quitar uno de los asientos. 

El archivo de conciliación incluirá lo siguiente: 
-   factura de $8 de 10 de junio, 9 de julio de período de servicio. 
-   $7.74 renovación prorrateada por período de servicio 11 de junio – 12 de junio. Este es el período que tenía 2 licencias. Cálculo = (mensual total del precio días en el período de servicio) x días en prorrateada del servicio período x número de licencias = x (30/4) 29 x 2 = 7.74.
-   $3,87 prorratea renovación por período de servicio del 12 de junio, 9 de julio. Este es el período que tenía 1 licencia. Cálculo = x (30/4) 29 x 1 = 3,87.

|**Fecha de compra**   |**Inicio de cargo**  |**Final de cargo**  |**Precio por unidad**  |**Cantidad**  |**Cantidad** |**Tipo de gasto** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|6/11/2019 (tiene 2 licencias)     |6/10/2019   |7/09/2019         |$4         |2        |$8       |Nuevo       |
|6/12/2019     | 6/10/2019    |7/09/2019        |$4        |2        | -$7.74       |removeQuantity           |
|6/12/2019 (tiene 1 licencia)    | 6/10/2019    |7/09/2019   |$4    |1      |$3.87    |removeQuantity |
