---
title: Descripción de los tipos de facturación del Centro de partners | Centro de partners
ms.topic: article
ms.date: 03/01/2019
Description: Información sobre los tipos de facturación, los períodos de facturación y las fechas de facturación diferentes
author: MaggiePucciEvans
ms.author: evansma
keywords: facturación, pagos, pedidos, archivos de conciliación, archivo de conciliación
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 38ad28fb74968d351d6031e21446f02d22f7e4fa
ms.sourcegitcommit: ba0b0eea3dbc028ec162f58b841ba9e3588f1dca
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/29/2019
ms.locfileid: "70134623"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Descripción de los tipos de facturación del Centro de partners

**Se aplica a**

-  Centro de partners
-  Partners del programa CSP

En función de los tipos de productos que compres para tus clientes, es posible que tengas períodos de facturación diferentes y que se te facture en distintos días del mismo mes. En este artículo se explica qué ha cambiado desde el 1 de marzo de 2019 y cómo te afectarán los cambios.

## <a name="billing-for-recurring-charges"></a>Facturación de cargos periódicos

La experiencia de facturación para los cargos periódicos de las suscripciones basadas en licencias y en el uso no cambia. Seguiremos emitiendo tu factura el día del mes que has seleccionado como fecha de facturación y el período de facturación seguirá siendo el mes anterior a esa fecha. Si has seleccionado el día 15 del mes de la fecha de facturación, se te facturará toda la actividad desde el 15 de un mes natural hasta el día 14 del mes natural siguiente. Las facturas y los archivos de conciliación están disponibles con carácter general entre 2 y 4 días después de la fecha de facturación.

Como antes, te facturaremos estos productos en la divisa del país o la región donde resides, independientemente de la ubicación del cliente al que has vendido el producto.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Facturación de cargos únicos y determinados cargos periódicos

A partir del 1 de marzo de 2019, se introdujo una nueva experiencia de facturación para cargos periódicos y únicos para productos de ISV de Microsoft y de terceros.

Para estos productos, el período de facturación comienza el primer día del mes natural y finaliza el último día del mismo mes natural. La factura estará disponible en el octavo día del mes siguiente. 

En otras palabras, todas las transacciones que realices entre el 1 de mayo y el 31 de mayo de 2019 aparecerán en la factura del 8 de junio. Todas las transacciones que realices entre el 1 de junio y el 30 de junio de 2019 aparecerán en la factura del 8 de julio. Es posible que se te facturen las compras periódicas y únicas en la misma factura. 

También puedes comprobar el saldo de la cuenta o la factura siempre que lo desees (por ejemplo, entre el 1 de mayo y el 7 de junio) y ver la actividad más reciente de la cuenta sin tener que esperar a recibir la factura. Ten en cuenta que, cuando publiquemos tu factura el día 8, se incluirán los impuestos y otros cargos y créditos aplicables, por lo que la cantidad final podría diferir de la que ves durante el período de facturación. 

Tendrás acceso a las facturas igual que ahora, ya sea en el Centro de partners o a través de la API. Aparecerán antes de la medianoche, hora UTC, el octavo día del mes. 

|**Experiencia de facturación**|**Tipos de productos**|**Fecha de facturación**|**Periodo de facturación**|**Divisa de facturación**|**¿Existe actividad disponible actualmente?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Cargos periódicos para suscripciones basadas en licencia y en el uso. |Todos los productos del [Catálogo de servicios en línea](https://partner.microsoft.com/commerce/preferredoffers/list). Algunos ejemplos son Office 365, Microsoft 365, Azure Active Directory, Azure (pago por uso), Dynamics 365 y PowerBI Pro. |Fecha seleccionada al crear la cuenta del Centro de partners |Mes anterior a la fecha de facturación. |Divisa del país o la región donde te encuentras. Por ejemplo, si tu empresa se encuentra en el Reino Unido, te facturaremos en libras esterlinas (GBP). Si tu empresa se encuentra en la India, te facturaremos en rupias indias (INR).  |No |
|Cargos periódicos y únicos para productos de ISV de Microsoft y de terceros. |Todas las suscripciones de SaaS, Azure Reservations y productos de software (perpetuos y de suscripción) que ofrecen los ISV de Microsoft y de terceros. Consulta los productos disponibles en [Marketplace](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Los ejemplos incluyen software de SUSE Linux (suscripción de software), Windows Server 2019 Essentials (software perpetuo), suscripción de productos SaaS de Azure ISV. |Octavo día de cada mes. |Desde el primero hasta el último día de cada mes natural. |Divisa del país o la región donde se encuentra el cliente. Esto significa que recibirás facturas y archivos de conciliación independientes en la moneda del país o la región de cada cliente al que has realizado ventas durante el período de facturación. |Sí |

## <a name="billing-scenarios-for-one-time-and-recurring-purchases"></a>Escenarios de facturación para compras únicas y periódicas
### <a name="scenario-1--purchase-a-subscription-and-then-add-a-seat-on-the-same-day"></a>Escenario 1: Compra de una suscripción y posterior adición de un puesto el mismo día

En el escenario 1, compras una suscripción el 11 de junio a un precio unitario de 4 USD. Más adelante el mismo día, compras otra unidad de la misma suscripción al mismo precio. 

El archivo de conciliación incluirá lo siguiente: 
-   Factura de 4 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio. 
-   Renovación prorrateada de 4 USD para el período de servicio comprendido entre el 11 y el 11 de junio. Este era el período cuando tenías una licencia. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 30 x 1 = 4,00.
-   Renovación prorrateada de 8 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio. Este era el período cuando tenías 2 licencias. Cálculo = (4/30) x 30 x 2 = 8,00.

|**Fecha de compra**   |**Inicio del cargo**  |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Volumen** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |09/7/2019         |4 USD                |1                 |4 USD            |Nuevo         |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |1        | -4 USD       |addQuantity           |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        | 2      |8 USD         |addQuantity           |

### <a name="scenario-2--purchase-a-subscription-and-then-add-more-later"></a>Escenario 2: Compra de una suscripción y adición de otras más adelante

En el escenario 2, compras una suscripción el 11 de junio a un precio unitario de 4 USD y el 12 de junio compras otra suscripción del mismo producto al mismo precio. 

El archivo de conciliación incluirá lo siguiente: 
-   Factura de 4 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio. 
-   Renovación prorrateada de -3,87 USD para el período de servicio comprendido entre el 11 y el 12 de junio. Este era el período cuando tenías una licencia. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 29 x 1 = 3,87.
-   Renovación prorrateada de 7,74 USD para el período de servicio comprendido entre el 12 de junio y el 9 de julio. Este era el período cuando tenías 2 licencias. Cálculo = (4/30) x 29 x 2 = 7,74.

|**Fecha de compra**   |**Inicio del cargo**  |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Volumen** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (tienes 1 licencia)     |10/6/2019   |09/7/2019         |4 USD         |1        |4 USD            |Nuevo         |
|12/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |1        | -3,87 USD       |addQuantity           |
|12/6/2019     | 10/6/2019    |09/7/2019        |4 USD        | 2      |7,74 USD       |addQuantity           |

### <a name="scenario-3--purchase-a-subscription-and-then-remove-a-seat-on-the-same-day"></a>Escenario 3: Compra de una suscripción y posterior eliminación de un puesto el mismo día

En el escenario 3, compras dos suscripciones del mismo producto el 11 de junio a un precio unitario de 4 USD. Más adelante el mismo día, quitas uno de los puestos.  

El archivo de conciliación incluirá lo siguiente: 
-   Factura de 8 USD por dos licencias para el período de servicio comprendido entre el 10 de junio y el 9 de julio. 
-   Renovación prorrateada de -8,00 USD para el período de servicio comprendido entre el 11 y el 11 de junio. Este era el período cuando tenías 2 licencias. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 30 x 2 = 8,00.
-   Renovación prorrateada de 4,00 USD para el período de servicio comprendido entre el 11 de junio y el 9 de julio. Este era el período cuando tenías una licencia. Cálculo = (4/30) x 30 x 1 = 4,00.

|**Fecha de compra**   |**Inicio del cargo**  |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Volumen** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |09/7/2019         |4 USD                |2                 |8 USD            |Nuevo         |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |2        | -8 USD       |removeQuantity           |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        | 1      |4 USD         |removeQuantity           |

### <a name="scenario-4--purchase-a-subscription-and-then-remove-seats-later"></a>Escenario 4: Compra de una suscripción y eliminación de puestos más adelante

En el escenario 4, compras 2 suscripciones el 11 de junio a un precio unitario de 4 USD y el 12 de junio quitas uno de los puestos. 

El archivo de conciliación incluirá lo siguiente: 
-   Factura de 8 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio. 
-   Renovación prorrateada de -7,74 USD para el período de servicio comprendido entre el 11 y el 12 de junio. Este era el período cuando tenías 2 licencias. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 29 x 2 = 7,74.
-   Renovación prorrateada de 3,87 USD para el período de servicio comprendido entre el 12 de junio y el 9 de julio. Este era el período cuando tenías una licencia. Cálculo = (4/30) x 29 x 1 = 3,87.

|**Fecha de compra**   |**Inicio del cargo**  |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Volumen** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (tienes 2 licencias)     |10/6/2019   |09/7/2019         |4 USD         |2        |8 USD       |Nuevo       |
|12/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |2        | -7,74 USD       |removeQuantity           |
|12/6/2019 (tienes 1 licencia)    | 10/6/2019    |09/7/2019   |4 USD    |1      |3,87 USD    |removeQuantity |

## <a name="billing-scenarios-for-free-trial-license-based-saas-transactions"></a>Escenarios de facturación para transacciones de SaaS basadas en licencias de evaluación gratuitas
### <a name="scenario-5--renew-a-license-based-free-trial-saas-subscription-to-a-paid-subscription-at-the-end-of-the-free-trial-period"></a>Escenario 5: Renovación de una suscripción de SaaS de evaluación gratuita basada en licencias a una suscripción de pago al final del período de evaluación gratuita

En este escenario, compras una suscripción de SaaS (software como servicio) basada en licencias de evaluación gratuitas el 10 de junio y se renueva automáticamente como una suscripción de pago cuando finaliza el período de evaluación gratuita. 

Los archivos de conciliación incluirán lo siguiente: 
- Factura de 0 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio. 
- Factura de 2 USD para el período de servicio comprendido entre el 10 de julio y el 9 de agosto.

|**Fecha de compra**   |**Inicio del cargo**  |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Volumen** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|10/6/2019 (tienes 1 licencia)      |10/6/2019   |09/7/2019         |0 USD                |1                 |0 USD            |Nuevo         |
|10/7/2019 (tienes 1 licencia)     | 10/7/2019    |09/8/2019        |2 USD        |1        | 2 USD       |Renovación           |

### <a name="scenario-6--cancel-a-license-based-free-trial-saas-subscription"></a>Escenario 6: Cancelación de una suscripción de SaaS de evaluación gratuita basada en licencias

Puedes cancelar una suscripción de SaaS (software como servicio) de evaluación gratuita basada en licencias en cualquier momento, incluso durante el período de evaluación gratuita. 

En este escenario, compras una suscripción e SaaS de evaluación gratuita basada en licencias el 1 de julio y la cancelas inmediatamente después en el Centro de partners. 

El archivo de conciliación incluirá lo siguiente: 
- Factura de 0 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio para la nueva compra.
- Factura de 0 USD para el período de servicio comprendido entre el 10 de julio y el 9 de julio para la cancelación.

|**Fecha de compra**   |**Inicio del cargo**  |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Volumen** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|10/6/2019 (tienes 11 licencias)      |10/6/2019   |09/7/2019         |0 USD                |11                |0 USD            |Nuevo         |
|10/6/2019 (no tienes ninguna licencia)     | 10/6/2019    |09/7/2019        |0 USD        |11       | 0 USD       |Cancelación           |

### <a name="scenario-7--convert-a-custom-meter-saas-subscription-from-one-sku-to-another-for-the-same-product-on-the-same-day"></a>Escenario 7: Convertir una suscripción de SaaS de medidor personalizado de una SKU a otra del mismo producto el mismo día

En este escenario, compras una SKU (Silver) bajo un producto y la conviertes en otra SKU disponible (Bronce) en este producto el mismo día. 

El archivo de conciliación incluirá lo siguiente: 
- Factura de 20 USD de Plata para el período de servicio comprendido entre el 10 de junio de 2019 y el 9 de julio de 2020
- Renovación prorrateada de 20 USD de Plata para el período de servicio comprendido entre el 10 de junio de 2019 y el 9 de julio de 2020
- Factura de 10 USD de Bronce para el período de servicio comprendido entre el 10 de junio de 2019 y el 9 de julio de 2020

|**Fecha de compra**   |**SKU**   |**Inicio del cargo**   |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Volumen** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|10/6/2019 (tienes 1 licencia) |Plata     |10/6/2019   |10/6/2019         |20 USD        |1         |20 USD            |Nuevo      |
|10/6/2019 (tienes 1 licencia) |Plata    | 10/6/2019    |10/6/2019        |20 USD        |1       | -20 USD       |Convertir           |
|10/6/2019 (tienes 1 licencia) |Bronce    | 10/6/2019    |10/6/2019        |10 USD        |1       | 10 USD       |Convertir           |

### <a name="scenario-8--purchase-and-cancel-a-custom-meter-saas-subscription-from-the-azure-portal-on-the-same-day"></a>Escenario 8: Compra y cancelación de una suscripción de SaaS de medidor personalizado desde Azure Portal el mismo día 

En este escenario, se compra una suscripción de SaaS de medidor personalizado en Azure Portal, que se cancela posteriormente el mismo día. 

|**Fecha de compra**   |**SKU**   |**Inicio del cargo**   |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Volumen** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|:-----:|
|10/6/2019 (tienes 1 licencia) |Bronce     |10/6/2019   |10/6/2019         |10 USD        |1         |10 USD            |Nuevo      |
|10/6/2019 (no tienes ninguna licencia) |Bronce    | 10/6/2019    |10/6/2019        |10 USD        |1       | -10 USD       |CancelImmediate  |
