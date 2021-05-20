---
title: Escenarios comunes de facturación mensual
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Escenarios comunes en Centro de partners cuando se usa la facturación mensual: incluye la adición de nuevas suscripciones, el cambio de la cantidad de licencias y la suspensión de suscripciones.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 66c9ec09f707d87248fdef31e4cf66f4ca927ce1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148659"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Escenarios de facturación mensual de ejemplo para nuevas suscripciones, cambio de importes de licencia o suspensiones

**Roles adecuados:** agente de administración | Administrador de facturación | Agente del departamento de soporte técnico | Agente de ventas

Estos [escenarios de facturación](common-billing-scenarios.md) comunes de ejemplo son aplicables si usa la facturación mensual en Centro de partners.

## <a name="new-monthly-subscription"></a>Nueva suscripción mensual

La fecha de facturación es el 15 de cada mes. El 13 de enero, comprará una nueva suscripción con una licencia de 4 USD al mes y seleccionará la facturación mensual. El archivo de conciliación basado en licencias del 15 de enero contendrá las siguientes líneas de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Tarifa de ciclo   |4.00       |1        |4.00 |

El archivo de conciliación basado en licencias del 15 de febrero contendrá la siguiente línea de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Tarifa de ciclo   |4.00       |1        |4.00 |

## <a name="change-license-quantity"></a>Cambiar cantidad de licencias

La fecha de facturación es el 15 de cada mes. El 13 de enero, comprará una nueva suscripción con una licencia de 4 USD al mes y seleccionará la facturación mensual. El archivo de conciliación basado en licencias del 15 de enero contendrá las siguientes líneas de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Tarifa de ciclo   |4.00       |1        |4.00    |

El 1 de febrero, aumentará la cantidad de licencias de uno a dos. El archivo de conciliación basado en licencias del 15 de febrero contendrá las siguientes líneas de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |12/2/2018    |Prorrateo de instancia de ciclo   |-4.00       |1        |-4.00   |
|1/13/2018         |31/1/2018    | Prorrateo de instancia de ciclo   |2.45       |1        |2.45    |
|1/2/2018         |12/2/2018    | Prorrateo de instancia de ciclo   |1.55       |2        |3.10    |
|2/13/2018         |3/12/2018    | Prorrateo de instancia de ciclo   |4.00       |2        |8.00    |

El precio mensual es 4,00 y hay 31 días en el período de servicio del 1/13/2018 al 12/2018. Esto equivale a un precio diario de 0,129 (4/31).

Hay 19 días en el período de prorización del 1/13/2018 al 31/1/2018.

Precio unitario de proración = 2,451 = 19 x 0,129

Hay 12 días en el período de prorización 2/1/2018 – 2/12/2018.

Precio unitario de proración = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Suspender antes de 30 días

La fecha de facturación es el 15 de cada mes. El 13 de enero, comprará una nueva suscripción con una licencia de 4 USD al mes y seleccionará la facturación mensual. El archivo de conciliación basado en licencias del 15 de enero contendrá las siguientes líneas de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Tarifa de ciclo   |4.00       |1        |4.00    |

El 1 de febrero, suspenderá una suscripción. El archivo de conciliación basado en licencias del 15 de febrero contendrá la siguiente línea de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|12/2/2018|Cuota de cancelación|-4.00|1|-4.00

## <a name="suspend-after-30-days"></a>Suspender después de 30 días

La fecha de facturación es el 15 de cada mes. El 13 de enero, comprará una nueva suscripción con una licencia de 4 USD al mes y seleccionará la facturación mensual. El archivo de conciliación basado en licencias del 15 de enero contendrá las siguientes líneas de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|12/2/2018|Costo del ciclo|4.00|1|4.00

El archivo de conciliación basado en licencias del 15 de febrero contendrá la siguiente línea de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Costo del ciclo|4.00|1|4.00

El 1 de marzo suspenderá la suscripción. El archivo de conciliación basado en licencias del 15 de marzo contendrá la siguiente línea de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Cuota de cancelación|-1.72|1|-1.72

El precio mensual es 4,00 y hay 28 días en el período de servicio del 13/2/2018 al 12/3/2018. Esto equivale a un precio diario de 0,143 (4/28).

Precio unitario = días en el período de servicio x precio diario x número de licencias.

Hay 12 días en el período de cancelación del 1/3/2018 al 12/3/2018.

Por lo tanto, el precio unitario = -1,716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Pasos siguientes

- [Escenarios de facturación para compras periódicas y únicas](common-billing-scenarios-onetime-recurring.md)