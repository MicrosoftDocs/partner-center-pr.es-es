---
title: Facturación de compras periódicas & única vez
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Centro de partners ejemplos de facturación de una sola vez y seleccionar compras periódicas: al comprar suscripciones, agregar más suscripciones, agregar o quitar licencias.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a26b6e5299c5186959612e622808161ca0f7f7c2
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148625"
---
# <a name="partner-center-billing-scenarios-for-one-time-and-select-recurring-purchases"></a>Centro de partners escenarios de facturación para una sola vez y seleccionar compras periódicas

**Roles adecuados:** agente de administración | Administrador de facturación | Agente de soporte técnico | Agente de ventas

Estos son [escenarios de facturación comunes.](common-billing-scenarios.md) 

## <a name="purchase-a-subscription-and-add-a-license-on-the-same-day"></a>Compra de una suscripción y adición de una licencia el mismo día

En el escenario 1, compras una suscripción el 11 de junio a un precio unitario de 4 USD. Más adelante el mismo día, compras otra unidad de la misma suscripción al mismo precio.

El archivo de conciliación incluirá lo siguiente:

- Factura de 4 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio.
- Renovación prorrateada de 4 USD para el período de servicio comprendido entre el 11 y el 11 de junio. Este es el período en el que tenía una licencia. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 30 x 1 = 4,00.
- Renovación prorrateada de 8 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio. Este es el período en el que tenía dos licencias. Cálculo = (4/30) x 30 x 2 = 8,00.

|**Fecha de compra**   |**Inicio del cargo** |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Amount** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |09/7/2019         |4 USD                |1                 |4 USD            |Nuevo         |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |1        | -4 USD       |addQuantity           |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        | 2      |8 USD         |addQuantity           |

## <a name="purchase-a-subscription-and-add-more-subscriptions-later"></a>Compra de una suscripción y adición de más suscripciones más adelante

En el escenario 2, compras una suscripción el 11 de junio a un precio unitario de 4 USD y el 12 de junio compras otra suscripción del mismo producto al mismo precio.

El archivo de conciliación incluirá lo siguiente:

- Factura de 4 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio.
- Renovación prorrateada de -3,87 USD para el período de servicio comprendido entre el 11 y el 12 de junio. Este es el período en el que tenía una licencia. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 29 x 1 = 3,87.
- Renovación prorrateada de 7,74 USD para el período de servicio comprendido entre el 12 de junio y el 9 de julio. Este es el período en el que tenía dos licencias. Cálculo = (4/30) x 29 x 2 = 7,74.

|**Fecha de compra**   |**Inicio del cargo** |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Amount** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (tienes 1 licencia)     |10/6/2019   |09/7/2019         |4 USD         |1        |4 USD            |Nuevo         |
|12/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |1        | -3,87 USD       |addQuantity           |
|12/6/2019     | 10/6/2019    |09/7/2019        |4 USD        | 2      |7,74 USD       |addQuantity           |

## <a name="purchase-a-subscription-and-remove-a-license-on-the-same-day"></a>Compra de una suscripción y eliminación de una licencia el mismo día

En el escenario 3, compras dos suscripciones del mismo producto el 11 de junio a un precio unitario de 4 USD. Más adelante ese mismo día quitará una de las licencias.  

El archivo de conciliación incluirá lo siguiente:

- Factura de 8 USD por dos licencias para el período de servicio comprendido entre el 10 de junio y el 9 de julio.
- Renovación prorrateada de -8,00 USD para el período de servicio comprendido entre el 11 y el 11 de junio. Este es el período en el que tenía dos licencias. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 30 x 2 = 8,00.
- Renovación prorrateada de 4,00 USD para el período de servicio comprendido entre el 11 de junio y el 9 de julio. Este es el período en el que tenía una licencia. Cálculo = (4/30) x 30 x 1 = 4,00.

|**Fecha de compra**   |**Inicio del cargo** |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Amount** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019      |10/6/2019   |09/7/2019         |4 USD                |2                 |8 USD            |Nuevo         |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |2        | -8 USD       |removeQuantity           |
|11/6/2019     | 10/6/2019    |09/7/2019        |4 USD        | 1      |4 USD         |removeQuantity           |

## <a name="purchase-a-subscription-and-remove-licenses-later"></a>Compra de una suscripción y eliminación de licencias más adelante

En el escenario 4, comprará dos suscripciones el 11 de junio a un precio unitario de 4 USD y el 12 de junio quitará una de las licencias.

El archivo de conciliación incluirá lo siguiente:

- Factura de 8 USD para el período de servicio comprendido entre el 10 de junio y el 9 de julio.
- Renovación prorrateada de -7,74 USD para el período de servicio comprendido entre el 11 y el 12 de junio. Este es el período en el que tenía dos licencias. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (4/30) x 29 x 2 = 7,74.
- Renovación prorrateada de 3,87 USD para el período de servicio comprendido entre el 12 de junio y el 9 de julio. Este es el período en el que tenía una licencia. Cálculo = (4/30) x 29 x 1 = 3,87.

|**Fecha de compra**   |**Inicio del cargo** |**Finalización del cargo**  |**Precio unitario**  |**Cantidad**  |**Amount** |**Tipo de cargo** |
|:------:|:------:|:------:|:------:|:------:|:------:|:-----:|
|11/6/2019 (tiene dos licencias)     |10/6/2019   |09/7/2019         |4 USD         |2        |8 USD       |Nuevo       |
|12/6/2019     | 10/6/2019    |09/7/2019        |4 USD        |2        | -7,74 USD       |removeQuantity           |
|12/6/2019 (tiene una licencia)    | 10/6/2019    |09/7/2019   |4 USD    |1      |3,87 USD    |removeQuantity |

## <a name="next-steps"></a>Pasos siguientes

- [Escenarios de facturación mensual de ejemplo para nuevas suscripciones, cambio de importes de licencia o suspensiones](common-billing-scenarios-monthly.md)