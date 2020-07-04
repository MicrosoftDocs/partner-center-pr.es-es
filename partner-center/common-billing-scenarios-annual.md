---
title: 'Facturación anual: escenarios comunes'
ms.topic: article
ms.date: 05/05/2020
description: 'Facturación anual del centro de Partners: al agregar nuevas suscripciones, agregar licencias antes de la fecha de facturación, cambiar la cantidad de licencias o suspender o reactivar las suscripciones.'
author: sodeb
ms.author: sodeb
Keywords: facturación, pagos, pedidos, uso, facturación basada en licencias, fecha de aniversario, término, cancelación, renovación, fórmula de precio, archivo de conciliación, archivo de conciliación
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ab6eabf44e5d3811721993e20b78e3038c80e828
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948050"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Escenarios de facturación anuales comunes en el centro de Partners

**Roles adecuados**

- Agente de administrador
- Administrador de facturación
- Agente del departamento de soporte técnico
- Agente de ventas

Estos ejemplos de [escenarios de facturación comunes](common-billing-scenarios.md) son aplicables si usa la facturación anual en el centro de Partners.

## <a name="new-annual-subscription"></a>Nueva suscripción anual

La fecha de facturación es el 15 de cada mes. El 13 de enero adquirirá una suscripción nueva con una licencia de $4/mes y seleccionará la facturación anual. El archivo de conciliación basado en licencias del 15 de enero contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Agregar licencia después de la fecha de aniversario de la suscripción, pero antes de la fecha de facturación

Compre una suscripción nueva en 2/11/17 con una licencia de $211.20/year. El aniversario de la suscripción se establece como el undécimo de cada mes. El sistema de facturación de Microsoft crea las siguientes líneas de facturación:

- Cargo de 211,20 USD para el período del 11/02/17 al 10/02/18.

El 2/12/17 compra una segunda licencia. La fecha de facturación es 2/14/17. Se generan una factura y un archivo de conciliación. El archivo de conciliación contendrá las siguientes líneas de facturación:

|Fecha de inicio de la carga  |Fecha de finalización del cargo  |Tipo de cargo  |Unit Price |Cantidad | Importe |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Tarifas prorrateadas al comprar |211,20 |1 | 211,20 |

En el aniversario de la suscripción, 3/11/17, el sistema de facturación de Microsoft crea las siguientes líneas de facturación para el aumento de la licencia en 2/12/17:

- $211,20 crédito del período 2/11/17 – 2/10/18.
- $0,58 cargo prorrateado por licencia para 1 licencia para el período 2/11/17 – 2/11/17.
- $15,62 cargo prorrateado por licencia para 2 licencias para el período 2/12/17 – 3/10/2017.
- $195,00 cargo prorrateado por licencia para 2 licencias para el período 3/11/2017 – 2/10/2018.

El 2/11/17 compra una suscripción. En 2/12/17, agregará una licencia. La fecha de facturación es 2/14/17. En 2/11/18, su suscripción se renueva.

La siguiente fecha de facturación es 3/14/17 y se genera una factura & archivo de conciliación. El archivo de conciliación contendrá las siguientes líneas de facturación:

|Fecha de inicio de la carga  |Fecha de finalización del cargo  |Tipo de cargo  |Unit Price |Cantidad | Importe |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Prorrateo de instancia de ciclo |-211,20 |1 |-211,20 |
|2/11/2017 |2/11/2017 |Prorrateo de instancia de ciclo |0,58 |1 |0,58 |
|2/12/2017 |3/10/2017 |Prorrateo de instancia de ciclo |15,62 |2 |31,25 |
|11/3/2017 |2/10/2018 |Prorrateo de instancia de ciclo |195,00 |2 |390,00 |

En 2/11/18, la suscripción se renueva para otro período de 12 meses.

## <a name="change-license-quantity"></a>Cambiar cantidad de licencias

La fecha de facturación es el 15 de cada mes. El 13 de enero adquirirá una suscripción nueva con una licencia de $4/mes y seleccionará la facturación anual. El archivo de conciliación basado en licencias del 15 de enero contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

El 1 de febrero aumenta la cantidad de licencias de uno a dos. El archivo de conciliación basado en licencias del 15 de febrero contendrá las siguientes líneas de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Prorrateo de instancia de ciclo|-48,00|1|-48,00
1/13/2018|31/1/2018|Prorrateo de instancia de ciclo|2.47|1|2.47
1/2/2018|1/12/2019|Prorrateo de instancia de ciclo|44,98|2|89,96

El precio anual es 48,00, que equivale al precio diario de 0,13 (48.00/365).

Precio por unidad = días del período de servicio x precio diario x número de licencias.

Hay 19 días en el período de servicio 1/13/2018 – 1/31/2018.

Por lo tanto, precio por unidad = 2,47 (19x 0,13 x1)

Hay 346 días en el período de servicio 2/1/2018 – 1/12/2019.

Por lo tanto, precio por unidad = 44,98 (346x 0,13 x2)

## <a name="suspend-before-30-days"></a>Suspender antes de 30 días

La fecha de facturación es el 15 de cada mes. El 13 de enero adquirirá una suscripción nueva con una licencia de $4/mes y seleccionará la facturación anual. El archivo de conciliación basado en licencias del 15 de enero contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

El 1 de febrero suspende la suscripción. El archivo de conciliación basado en licencias del 15 de febrero contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Cuota de cancelación|-48,00|1|-48,00

## <a name="suspend-after-30-days"></a>Suspender después de 30 días

La fecha de facturación es el 15 de cada mes. El 13 de enero adquirirá una suscripción nueva con una licencia de $4/mes y seleccionará la facturación anual. El archivo de conciliación basado en licencias del 15 de enero contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

El archivo de conciliación basado en licencias del 15 de febrero no contendrá ninguna línea de facturación para esta suscripción.
El 1 de marzo se suspende la suscripción. El archivo de conciliación basado en licencias del 15 de marzo contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Cuota de cancelación|-41,34|1|-41,34

El precio anual es 48,00, que equivale al precio diario de 0,13 (48.00/365).

Precio por unidad = días del período de servicio x precio diario x número de licencias.

Hay 318 días en el período de servicio 3/1/2018 – 1/12/2019.

Por lo tanto, precio por unidad = 41,34 (318x 0,13 x1). Dado que se trata de un crédito, el precio por unidad es-41,34.

## <a name="suspend-and-reactivate"></a>Suspender y reactivar

La fecha de facturación es el 15 de cada mes. El 13 de enero adquirirá una suscripción nueva con una licencia de $4/mes y seleccionará la facturación anual. El archivo de conciliación basado en licencias del 15 de enero contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

El 1 de febrero suspende la suscripción. El archivo de conciliación basado en licencias del 15 de febrero contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Cuota de cancelación|-48,00|1|-48,00

En el 1 de marzo, reactivará la suscripción. El archivo de conciliación basado en licencias del 15 de marzo contendrá la siguiente línea de facturación:

|Fecha de inicio de la carga |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Tarifas prorrateadas al comprar|41,34|1|41,34

El precio anual es 48,00, que equivale al precio diario de 0,13 (48.00/365).

Precio por unidad = días del período de servicio x precio diario x número de licencias.

Hay 318 días en el período de servicio 3/1/2018 – 1/12/2019.

Por lo tanto, precio por unidad = 41,34 (318x 0,13 x1).
