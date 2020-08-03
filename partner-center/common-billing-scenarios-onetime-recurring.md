---
title: Facturación de una sola vez & compras periódicas
ms.topic: article
ms.date: 05/05/2020
description: Consulte los ejemplos de facturación del centro de partners para una sola vez y seleccione compras periódicas; al adquirir suscripciones, agregar más suscripciones, agregar o quitar licencias.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5349a78b788c060999c98440edf962a64cb43112
ms.sourcegitcommit: e243bc0ef337f5d92c5b208ce6bb9dc5f179b185
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/31/2020
ms.locfileid: "87468399"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Escenarios de facturación del centro de partners para una sola vez y selección de compras periódicas

**Roles adecuados**

- Agente de administrador
- Administrador de facturación
- Agente del departamento de soporte técnico
- Agente de ventas

Estos son [escenarios de facturación habituales](common-billing-scenarios.md). 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Comprar una suscripción y agregar una licencia en el mismo día

En el escenario 1, compras una suscripción el 11 de junio a un precio unitario de 4 USD. Más adelante el mismo día, compras otra unidad de la misma suscripción al mismo precio.

El archivo de conciliación incluirá lo siguiente:

- Factura de 4 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio.
- Renovación prorrateada de 4 USD para el período de servicio comprendido entre el 11 y el 11 de junio. Este era el período cuando tenías una licencia. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 30 x 1 = 4,00.
- Renovación prorrateada de 8 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio. Este era el período cuando tenías 2 licencias. Cálculo = (4/30) x 30 x 2 = 8,00.

|**Fecha de compra**   |**Inicio del cargo** |**Finalización del cargo**  |**Precio por unidad**  |**Cantidad**  |**Importe** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |09/7/2019         |4 USD                |1                 |4 USD            |Nuevo         |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |1        | -4 USD       |addQuantity           |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        | 2      |8 USD         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Comprar una suscripción y agregar más suscripciones más adelante

En el escenario 2, compras una suscripción el 11 de junio a un precio unitario de 4 USD y el 12 de junio compras otra suscripción del mismo producto al mismo precio.

El archivo de conciliación incluirá lo siguiente:

- Factura de 4 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio.
- Renovación prorrateada de -3,87 USD para el período de servicio comprendido entre el 11 y el 12 de junio. Este era el período cuando tenías una licencia. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 29 x 1 = 3,87.
- Renovación prorrateada de 7,74 USD para el período de servicio comprendido entre el 12 de junio y el 9 de julio. Este era el período cuando tenías 2 licencias. Cálculo = (4/30) x 29 x 2 = 7,74.

|**Fecha de compra**   |**Inicio del cargo** |**Finalización del cargo**  |**Precio por unidad**  |**Cantidad**  |**Importe** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (tienes 1 licencia)     |10/6/2019   |09/7/2019         |4 USD         |1        |4 USD            |Nuevo         |
|12/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |1        | -3,87 USD       |addQuantity           |
|12/6/2019     | 10/6/2019    |09/7/2019        |4 USD        | 2      |7,74 USD       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Comprar una suscripción y quitar una licencia en el mismo día

En el escenario 3, compras dos suscripciones del mismo producto el 11 de junio a un precio unitario de 4 USD. Más adelante, el mismo día quitará una de las licencias.  

El archivo de conciliación incluirá lo siguiente:

- Factura de 8 USD por dos licencias para el período de servicio comprendido entre el 10 de junio y el 9 de julio.
- Renovación prorrateada de -8,00 USD para el período de servicio comprendido entre el 11 y el 11 de junio. Este era el período cuando tenías 2 licencias. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 30 x 2 = 8,00.
- Renovación prorrateada de 4,00 USD para el período de servicio comprendido entre el 11 de junio y el 9 de julio. Este era el período cuando tenías una licencia. Cálculo = (4/30) x 30 x 1 = 4,00.

|**Fecha de compra**   |**Inicio del cargo** |**Finalización del cargo**  |**Precio por unidad**  |**Cantidad**  |**Importe** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |09/7/2019         |4 USD                |2                 |8 USD            |Nuevo         |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |2        | -8 USD       |removeQuantity           |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        | 1      |4 USD         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Compra de una suscripción y eliminación de licencias más adelante

En el escenario 4, compra 2 suscripciones el 11 de junio a un precio por unidad de $4 y el 12 de junio quita una de las licencias.

El archivo de conciliación incluirá lo siguiente:

- Factura de 8 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio.
- Renovación prorrateada de -7,74 USD para el período de servicio comprendido entre el 11 y el 12 de junio. Este era el período cuando tenías 2 licencias. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 29 x 2 = 7,74.
- Renovación prorrateada de 3,87 USD para el período de servicio comprendido entre el 12 de junio y el 9 de julio. Este era el período cuando tenías una licencia. Cálculo = (4/30) x 29 x 1 = 3,87.

|**Fecha de compra**   |**Inicio del cargo** |**Finalización del cargo**  |**Precio por unidad**  |**Cantidad**  |**Importe** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (tienes 2 licencias)     |10/6/2019   |09/7/2019         |4 USD         |2        |8 USD       |Nuevo       |
|12/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |2        | -7,74 USD       |removeQuantity           |
|12/6/2019 (tienes 1 licencia)    | 10/6/2019    |09/7/2019   |4 USD    |1      |3,87 USD    |removeQuantity |
