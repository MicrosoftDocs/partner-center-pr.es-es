---
title: Escenarios comunes de facturación mensual
ms.topic: article
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Escenarios comunes en el centro de Partners cuando se usa la facturación mensual: incluye la adición de nuevas suscripciones, el cambio de la cantidad de licencias y la suspensión de suscripciones.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4fe5c33fe549604f25500dd333d187e6b70ad73e
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502521"
---
# <a name="sample-monthly-billing-scenarios-for-new-subscriptions-changing-license-amounts-or-suspensions"></a>Ejemplos de escenarios de facturación mensuales para nuevas suscripciones, cambios de cantidades de licencias o suspensiones

**Roles adecuados**

- Agente de administrador
- Administrador de facturación
- Agente del departamento de soporte técnico
- Agente de ventas

Estos ejemplos de [escenarios de facturación comunes](common-billing-scenarios.md) son aplicables si usa la facturación mensual en el centro de Partners.

## <a name="new-monthly-subscription"></a>Nueva suscripción mensual

La fecha de facturación es el 15 de cada mes. El 13 de enero, comprará una suscripción nueva con una licencia de $4/mes y seleccionará la facturación mensual. El archivo de conciliación basado en licencias 15 de enero contendrá las siguientes líneas de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Tarifa de ciclo   |4.00       |1        |4.00 |

El archivo de conciliación basado en licencias del 15 de febrero contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|2/13/2018         |3/12/2018    |Tarifa de ciclo   |4.00       |1        |4.00 |

## <a name="change-license-quantity"></a>Cambiar cantidad de licencias

La fecha de facturación es el 15 de cada mes. El 13 de enero, comprará una suscripción nueva con una licencia de $4/mes y seleccionará la facturación mensual. El archivo de conciliación basado en licencias 15 de enero contendrá las siguientes líneas de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Tarifa de ciclo   |4.00       |1        |4.00    |

En el 1 de febrero, aumentará la cantidad de licencias de uno a dos. El archivo de conciliación basado en licencias del 15 de febrero contendrá las siguientes líneas de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 1/13/2018        |12/2/2018    |Prorrateo de instancia de ciclo   |-4,00       |1        |-4,00   |
|1/13/2018         |31/1/2018    | Prorrateo de instancia de ciclo   |2.45       |1        |2.45    |
|1/2/2018         |12/2/2018    | Prorrateo de instancia de ciclo   |1.55       |2        |3.10    |
|2/13/2018         |3/12/2018    | Prorrateo de instancia de ciclo   |4.00       |2        |8.00    |

El precio mensual es 4,00 y hay 31 días en el período de servicio 1/13/2018 – 2/12/2018. Esto equivale a un precio diario de 0,129 (4/31).

Hay 19 días en el período de proporciones 1/13/2018 a 1/31/2018.

Precio por unidad de proporciones = 2,451 = 19 x 0,129

Hay 12 días en el período de proporciones 2/1/2018 a 2/12/2018.

Precio por unidad de proporciones = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Suspender antes de 30 días

La fecha de facturación es el 15 de cada mes. El 13 de enero, comprará una suscripción nueva con una licencia de $4/mes y seleccionará la facturación mensual. El archivo de conciliación basado en licencias 15 de enero contendrá las siguientes líneas de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|1/13/2018         |12/2/2018    |Tarifa de ciclo   |4.00       |1        |4.00    |

El 1 de febrero se suspende una suscripción. El archivo de conciliación basado en licencias del 15 de febrero contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|12/2/2018|Cuota de cancelación|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Suspender después de 30 días

La fecha de facturación es el 15 de cada mes. El 13 de enero, comprará una suscripción nueva con una licencia de $4/mes y seleccionará la facturación mensual. El archivo de conciliación basado en licencias 15 de enero contendrá las siguientes líneas de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|12/2/2018|Precio del ciclo|4.00|1|4.00

El archivo de conciliación basado en licencias del 15 de febrero contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
2/13/2018|3/12/2018|Precio del ciclo|4.00|1|4.00

El 1 de marzo se suspende la suscripción. El archivo de conciliación basado en licencias 15 de marzo contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Quantity |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|3/12/2018|Cuota de cancelación|-1,72|1|-1,72

El precio mensual es 4,00 y hay 28 días en el período de servicio 2/13/2018 – 3/12/2018. Esto equivale a un precio diario de 0,143 (4/28).

Precio por unidad = días del período de servicio x precio diario x número de licencias.

Hay 12 días en el período de cancelación 3/1/2018 a 3/12/2018.

Por lo tanto, el precio por unidad =-1,716 (12 x 0,143 x (-1)).

## <a name="next-steps"></a>Pasos siguientes

- [Escenarios de facturación para una sola vez y selección de compras periódicas](common-billing-scenarios-onetime-recurring.md)