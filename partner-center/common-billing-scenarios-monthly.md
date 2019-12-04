---
title: Escenarios comunes de facturación mensual | Centro de Partners
ms.topic: article
ms.date: 11/25/2019
description: Escenarios comunes en el centro de Partners cuando se usa la facturación mensual (como agregar nuevas suscripciones, cambiar la cantidad de licencias y suspender suscripciones).
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
Keywords: facturación, pagos, pedidos, uso, facturación mensual, suscripciones, archivo de conciliación
ms.localizationpriority: medium
ms.openlocfilehash: 9cae4f82e059a2c8258a00ae51a406ca890f7a67
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/03/2019
ms.locfileid: "74722485"
---
# <a name="monthly-billing-scenarios"></a>Escenarios de facturación mensuales

**Roles adecuados**

- Agente de administración
- Administrador de facturación
- Agente del departamento de soporte técnico
- Agente de ventas

Estos ejemplos de [escenarios de facturación comunes](common-billing-scenarios.md) son aplicables si usa la facturación mensual en el centro de Partners.

## <a name="new-monthly-subscription"></a>Nueva suscripción mensual

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación mensual. El 15 de enero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tarifa de ciclo   |4,00       |1        |4,00 |

El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/2/2018         |12/3/2018    |Tarifa de ciclo   |4,00       |1        |4,00 |

## <a name="change-license-quantity"></a>Cambiar la cantidad de licencias

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación mensual. El 15 de enero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tarifa de ciclo   |4,00       |1        |4,00    |

El 1 de febrero aumentas la cantidad de licencias de una a dos. El 15 de febrero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13/1/2018        |12/2/2018    |Prorrateo de instancia de ciclo   |-4,00       |1        |-4,00   |
|13/1/2018         |31/1/2018    | Prorrateo de instancia de ciclo   |2.45       |1        |2.45    |
|1/2/2018         |12/2/2018    | Prorrateo de instancia de ciclo   |1.55       |2        |3.10    |
|13/2/2018         |12/3/2018    | Prorrateo de instancia de ciclo   |4,00       |2        |8,00    |

El precio mensual es 4,00 y hay 31 días en el periodo de servicio 13/1/2018 – 12/2/2018. Esto equivale a un precio diario de 0,129 (4/31).

Hay 19 días en el período de prorrateo 13/1/2018 – 31/1/2018.

Precio unitario de prorrateo = 2,451 = 19 x 0,129

Hay 12 días en el período de prorrateo 1/2/2018 – 12/2/2018.

Precio unitario de prorrateo = 1,54 = 12 x 0,129

## <a name="suspend-before-30-days"></a>Suspender antes de 30 días

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación mensual. El 15 de enero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tarifa de ciclo   |4,00       |1        |4,00    |

El 1 de febrero suspende una suscripción. El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/2/2018|Cuota de cancelación|-4,00|1|-4,00

## <a name="suspend-after-30-days"></a>Suspender después de 30 días

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación mensual. El 15 de enero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/2/2018|Tarifa de ciclo|4,00|1|4,00

El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/2/2018|12/3/2018|Tarifa de ciclo|4,00|1|4,00

El 1 de marzo suspendes la suscripción. El 15 de marzo el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/3/2018|Cuota de cancelación|-1,72|1|-1,72

El precio mensual es 4,00 y hay 28 días en el periodo de servicio 13/2/2018 – 12/3/2018. Esto equivale a un precio diario de 0,143 (4/28).

Precio unitario = días en período de servicio x precio diario x número de licencias.

Hay 12 días en el período de cancelación 1/3/2018 – 12/3/2018.

Por lo tanto, el precio por unidad =-1,716 (12 x 0,143 x (-1)).
