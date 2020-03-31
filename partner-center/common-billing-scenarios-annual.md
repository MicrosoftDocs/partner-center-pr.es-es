---
title: Escenarios comunes de facturación | Centro de partners
ms.topic: article
ms.date: 11/25/2019
description: 'Consulte facturación anual del centro de Partners: cuando se agregan suscripciones nuevas, se agregan licencias antes de la fecha de facturación, se cambian la cantidad de licencias, se suspenden o reactivan las suscripciones.'
ms.assetid: ''
author: jasonwhowell
ms.author: jasonh
Keywords: facturación, pagos, pedidos, uso, facturación basada en licencias, fecha de aniversario, término, cancelación, renovación, fórmula de precio, archivo de conciliación, archivo de conciliación
ms.localizationpriority: medium
ms.openlocfilehash: fdfb242f51556ce924d06d7a35f32cf726803fe3
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390164"
---
# <a name="annual-billing-scenarios"></a>Escenarios de facturación anuales

**Roles adecuados**

- Agente de administración
- Administrador de facturación
- Agente del departamento de soporte técnico
- Agente de ventas

Estos ejemplos de [escenarios de facturación comunes](common-billing-scenarios.md) son aplicables si usa la facturación anual en el centro de Partners.

## <a name="new-annual-subscription"></a>Nueva suscripción anual

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación anual. El 15 de enero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Agregar licencia después de la fecha de aniversario de la suscripción, pero antes de la fecha de facturación

Adquieres una nueva suscripción el 11/02/17 con una licencia por 211,20 USD al año. El aniversario de la suscripción está establecido el día 11 de cada mes. El sistema de facturación de Microsoft crea las siguientes líneas de facturación:

- Cargo de 211,20 USD para el período del 11/02/17 al 10/02/18.

El 12/02/17 adquieres una segunda licencia. Tu fecha de facturación es el 14/02/17. Se generarán los archivos de factura y de conciliación. El archivo de conciliación contendrá las siguientes líneas de facturación:

|Fecha de inicio de cargo  |Fecha de fin de cargo  |Tipo de cargo  |Precio unitario |Cantidad | Volumen |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Tarifas prorrateadas al comprar |211,20 |1 | 211,20 |

En el aniversario de la suscripción, 11/03/17, el sistema de facturación de Microsoft crea las siguientes líneas de facturación para el aumento de licencias e 12/02/17:

- $211,20 crédito del período 2/11/17 – 2/10/18.
- Cargo prorrateado de 0,58 USD por licencia para 1 licencia para el período del 11/02/17 al 11/02/17.
- Cargo prorrateado de 15,62 USD por licencia para 2 licencias para el período del 12/02/17 al 10/03/2017.
- Cargo prorrateado de 195,00 USD por licencia para 2 licencias para el período del 11/03/2017 al 10/02/2018.

El 11/02/17 adquieres una suscripción. El 12/02/17 agregas una licencia. Tu fecha de facturación es el 14/02/17. El 11/02/18 se renueva la suscripción.

La próxima fecha de facturación es el 14/03/17 y se generan los archivos de factura y conciliación. El archivo de conciliación contendrá las siguientes líneas de facturación:

|Fecha de inicio de cargo  |Fecha de fin de cargo  |Tipo de cargo  |Precio unitario |Cantidad | Volumen |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Prorrateo de instancia de ciclo |-211,20 |1 |-211,20 |
|11/02/2017 |11/02/2017 |Prorrateo de instancia de ciclo |0,58 |1 |0,58 |
|12/02/2017 |10/03/2017 |Prorrateo de instancia de ciclo |15,62 |2 |31,25 |
|11/03/2017 |10/02/2018 |Prorrateo de instancia de ciclo |195,00 |2 |390,00 |

La suscripción se renueva el 11/02/18 por otro período de 12 meses.

## <a name="change-license-quantity"></a>Cambiar la cantidad de licencias

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación anual. El 15 de enero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

El 1 de febrero aumentas la cantidad de licencias de una a dos. El 15 de febrero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Prorrateo de instancia de ciclo|-48,00|1|-48,00
13/1/2018|31/1/2018|Prorrateo de instancia de ciclo|2,47|1|2,47
1/2/2018|12/1/2019|Prorrateo de instancia de ciclo|44,98|2|89,96

El precio anual es 48,00 que equivale a un precio diario de 0,13 (48,00/365).

Precio unitario = días en período de servicio x precio diario x número de licencias.

Hay 19 días en el período de servicio 13/1/2018 – 31/1/2018.

Por lo tanto, el precio unitario = 2,47 (19x0,13x1)

Hay 346 días en el período de servicio 1/2/2018 – 12/1/2019.

Por lo tanto, el precio unitario = 44,98 (346x0,13x2)

## <a name="suspend-before-30-days"></a>Suspender antes de 30 días

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación anual. El 15 de enero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

El 1 de febrero suspendes la suscripción. El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Cuota de cancelación|-48,00|1|-48,00

## <a name="suspend-after-30-days"></a>Suspender después de 30 días

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación anual. El 15 de enero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

El 15 de febrero el archivo de conciliación basado en licencia no contendrá ninguna línea de facturación para esta suscripción.
El 1 de marzo suspendes tu suscripción. El 15 de marzo el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/1/2019|Cuota de cancelación|-41,34|1|-41,34

El precio anual es 48,00 que equivale a un precio diario de 0,13 (48,00/365).

Precio unitario = días en período de servicio x precio diario x número de licencias.

Hay 318 días en el período de servicio 1/3/2018 – 12/1/2019.

Por lo tanto, el precio unitario = 41,34 (318x0,13x1). Dado que es un crédito, el precio unitario es-41,34.

## <a name="suspend-and-reactivate"></a>Suspender y reactivar

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación anual. El 15 de enero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

El 1 de febrero suspendes la suscripción. El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Cuota de cancelación|-48,00|1|-48,00

El 1 de marzo vuelves a activar tu suscripción. El 15 de marzo el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/1/2019|Tarifas prorrateadas al comprar|41,34|1|41,34

El precio anual es 48,00 que equivale a un precio diario de 0,13 (48,00/365).

Precio unitario = días en período de servicio x precio diario x número de licencias.

Hay 318 días en el período de servicio 1/3/2018 – 12/1/2019.

Por lo tanto, el precio unitario = 41,34 (318x0,13x1).
