---
title: 'Facturación anual: escenarios comunes'
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Centro de partners facturación anual: al agregar nuevas suscripciones, agregar licencias antes de la fecha de facturación, cambiar la cantidad de licencias o suspender o reactivar suscripciones.'
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a6392094e000b899e0545655ecf9ed6117535f7f
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148710"
---
# <a name="common-annual-billing-scenarios-in-partner-center"></a>Escenarios comunes de facturación anual en Centro de partners

**Roles adecuados:** agente de administración | Administrador de facturación | Agente del departamento de soporte técnico | Agente de ventas

Estos [escenarios de facturación comunes de ejemplo](common-billing-scenarios.md) son aplicables si usa facturación anual en Centro de partners.

## <a name="new-annual-subscription"></a>Nueva suscripción anual

La fecha de facturación es el 15 de cada mes. El 13 de enero, comprará una nueva suscripción con una licencia de 4 USD al mes y seleccionará la facturación anual. El archivo de conciliación basado en licencias del 15 de enero contendrá la siguiente línea de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Tarifas prorrateadas al comprar|48.00|1|48.00

## <a name="add-license-after-subscription-anniversary-date-but-before-billing-date"></a>Agregar licencia después de la fecha de aniversario de la suscripción, pero antes de la fecha de facturación

Comprará una nueva suscripción el 11/2/2017 con una licencia por 211,20 USD/año. El aniversario de la suscripción se establece como el 11 de cada mes. El sistema de facturación de Microsoft crea las siguientes líneas de facturación:

- Cargo de 211,20 USD para el período del 11/02/17 al 10/02/18.

El 12/2/17, se adquiere una segunda licencia. La fecha de facturación es el 14/2/17. Se generan una factura y un archivo de conciliación. El archivo de conciliación contendrá las siguientes líneas de facturación:

|Fecha de inicio del cargo  |Fecha de finalización del cargo  |Tipo de cargo  |Unit Price |Cantidad | Amount |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Tarifas prorrateadas al comprar |211.20 |1 | 211.20 |

El 17/3/11/17, el sistema de facturación de Microsoft crea las siguientes líneas de facturación para el aumento de licencias el 17/2/12:

- Crédito de 211,20 USD para el período del 11/17/2/10/18.
- Cargo prorrateado de 0,58 USD por licencia para una licencia durante el período del 11/2/17 al 11/2/17.
- Cargo prorrateado de 15,62 USD por licencia para dos licencias durante el período del 12/2/17 al 10/3/2017.
- Cargo prorrateado de 195,00 USD por licencia para dos licencias durante el período del 11/03/2017 al 10/2018.

El 11/2/17, compra una suscripción. El 12/2/17, agregue una licencia. La fecha de facturación es el 14/2/17. El 11/2/2018 se renueva la suscripción.

La siguiente fecha de facturación es el 14/3/17 y se generan una factura y un archivo de conciliación. El archivo de conciliación contendrá las siguientes líneas de facturación:

|Fecha de inicio del cargo  |Fecha de finalización del cargo  |Tipo de cargo  |Unit Price |Cantidad | Amount |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|2/11/2017 |2/10/2018 |Prorrateo de instancia de ciclo |-211.20 |1 |-211.20 |
|2/11/2017 |2/11/2017 |Prorrateo de instancia de ciclo |0.58 |1 |0.58 |
|2/12/2017 |3/10/2017 |Prorrateo de instancia de ciclo |15.62 |2 |31.25 |
|11/3/2017 |2/10/2018 |Prorrateo de instancia de ciclo |195.00 |2 |390.00 |

El 11/2/18, la suscripción se renueva durante otro período de 12 meses.

## <a name="change-license-quantity"></a>Cambiar cantidad de licencias

La fecha de facturación es el 15 de cada mes. El 13 de enero, comprará una nueva suscripción con una licencia de 4 USD al mes y seleccionará la facturación anual. El archivo de conciliación basado en licencias del 15 de enero contendrá la siguiente línea de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Tarifas prorrateadas al comprar|48.00|1|48.00

El 1 de febrero, aumentará la cantidad de licencias de uno a dos. El archivo de conciliación basado en licencias del 15 de febrero contendrá las siguientes líneas de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Prorrateo de instancia de ciclo|-48.00|1|-48.00
1/13/2018|31/1/2018|Prorrateo de instancia de ciclo|2.47|1|2.47
1/2/2018|1/12/2019|Prorrateo de instancia de ciclo|44.98|2|89.96

El precio anual es 48,00, lo que equivale al precio diario de 0,13 (48,00/365).

Precio unitario = días en el período de servicio x precio diario x número de licencias.

Hay 19 días en el período de servicio 1/13/2018: 31/1/2018.

Por lo tanto, precio unitario = 2,47 (19x0,13x1)

Hay 346 días en el período de servicio 2/1/2018 – 1/12/2019.

Por lo tanto, precio unitario = 44,98 (346x0,13x2)

## <a name="suspend-before-30-days"></a>Suspender antes de 30 días

La fecha de facturación es el 15 de cada mes. El 13 de enero, comprará una nueva suscripción con una licencia de 4 USD al mes y seleccionará la facturación anual. El archivo de conciliación basado en licencias del 15 de enero contendrá la siguiente línea de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Tarifas prorrateadas al comprar|48.00|1|48.00

El 1 de febrero, suspenderá la suscripción. El archivo de conciliación basado en licencias del 15 de febrero contendrá la siguiente línea de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Cuota de cancelación|-48.00|1|-48.00

## <a name="suspend-after-30-days"></a>Suspender después de 30 días

La fecha de facturación es el 15 de cada mes. El 13 de enero, comprará una nueva suscripción con una licencia de 4 USD al mes y seleccionará la facturación anual. El archivo de conciliación basado en licencias del 15 de enero contendrá la siguiente línea de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Tarifas prorrateadas al comprar|48.00|1|48.00

El archivo de conciliación basado en licencias del 15 de febrero no contendrá ninguna línea de facturación para esta suscripción.
El 1 de marzo, suspenderá la suscripción. El archivo de conciliación basado en licencias del 15 de marzo contendrá la siguiente línea de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Cuota de cancelación|-41.34|1|-41.34

El precio anual es 48,00, lo que equivale al precio diario de 0,13 (48,00/365).

Precio unitario = días en el período de servicio x precio diario x número de licencias.

Hay 318 días en el período de servicio 3/1/2018 – 1/12/2019.

Por lo tanto, precio unitario = 41,34 (318x0,13x1). Dado que se trata de un crédito, el precio unitario es -41,34.

## <a name="suspend-and-reactivate"></a>Suspender y reactivar

La fecha de facturación es el 15 de cada mes. El 13 de enero, comprará una nueva suscripción con una licencia de 4 USD al mes y seleccionará la facturación anual. El archivo de conciliación basado en licencias del 15 de enero contendrá la siguiente línea de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Tarifas prorrateadas al comprar|48.00|1|48.00

El 1 de febrero, suspenderá la suscripción. El archivo de conciliación basado en licencias del 15 de febrero contendrá la siguiente línea de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/13/2018|1/12/2019|Cuota de cancelación|-48.00|1|-48.00

El 1 de marzo, reactivará la suscripción. El archivo de conciliación basado en licencias del 15 de marzo contendrá la siguiente línea de facturación:

|Fecha de inicio del cargo |Fecha de finalización del cargo |Tipo de cargo |Unit Price |Cantidad |Amount |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
3/1/2018|1/12/2019|Tarifas prorrateadas al comprar|41.34|1|41.34

El precio anual es 48,00, lo que equivale al precio diario de 0,13 (48,00/365).

Precio unitario = días en el período de servicio x precio diario x número de licencias.

Hay 318 días en el período de servicio 3/1/2018 – 1/12/2019.

Por lo tanto, precio unitario = 41,34 (318x0,13x1).
