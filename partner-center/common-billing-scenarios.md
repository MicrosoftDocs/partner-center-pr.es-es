---
title: Escenarios comunes de facturación | Centro de partners
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn what you will see on your bill after you add new subscriptions, adjust the number of licenses in a subscription, or cancel a subscription.
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, orders, usage, license-based billing, anniversary date, term, cancellation, renewal, price formula,reconciliation file, recon file
ms.localizationpriority: medium
ms.openlocfilehash: d8afffa1dd11e386b03548c8f10e5490e6db5894
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253394"
---
# <a name="common-billing-scenarios"></a>Escenarios comunes de facturación

**Se aplica a**

-   Cloud Solution Provider program billing

En este tema se explica qué debes esperar ver en tu factura después de agregar nuevas suscripciones, ajustar la cantidad de licencias en una suscripción o cancelar una suscripción. Las suscripciones basadas en licencia y basadas en uso se ven afectadas de forma diferente.

## <a name="in-this-section"></a>En esta sección

-   [Usage-based billing](#usagebased)

-   [License-based billing](#licensebased)

## <a href="" id="usagebased"></a>Usage-based billing

Las suscripciones basadas en uso se facturan mensualmente, por período vencido, el día del aniversario de la suscripción. For example, if the subscription anniversary date is the 15th, you will be charged on January 15 for the service period December 15 - January 14. You will be charged again on February 15 for the service period January 15 - February 14, etc. The charges that are generated on the subscription anniversary day will appear on the following invoice and reconciliation file.

You may occasionally notice that some usage charges are missing from your invoice, or that usage from a previous month is charged in the current month's invoice. This is not an error; it simply means that the service was timestamped after the services occurred. Usage reported within 24 hours of the end of the billing cycle will appear on the next month's bill. 

Usage-based subscriptions may be suspended at any time. 

La lista de precios CSP de Azure se publica mensualmente y se puede encontrar en la página de venta de Centro de partners->Precios y ofertas. Ten en cuenta que los precios pueden cambiar a diario y se reflejan en la pestaña Historial de cambios de la lista de precios.

Los cargos por uso se basan en los precios diarios. Si el precio cambia durante el período de servicio, verás una línea de facturación para cada período de servicio prorrateado y precio aplicable.

## <a href="" id="licensebased"></a>License-based billing

**Facturación:** las suscripciones basadas en licencia se facturan por adelantado el día del aniversario de la suscripción.

**Día de aniversario:** el aniversario es el día del mes en que compraste la suscripción. Por ejemplo, si has comprado la suscripción el 15 de enero, el día de aniversario será el 15 de cada mes.

**Plazo:** todas las suscripciones basadas en licencia tienen un plazo de pago de 12 meses, que comienza en la fecha de compra.

**Cancelación:** las suscripciones suspendidas el mes 1 serán abonadas al 100 %. Las suscripciones suspendidas los meses 2-12 se abonarán de forma prorrateada.

**Renovación:** todas las suscripciones basadas en licencia se renuevan automáticamente 12 meses después de que comience el plazo pagado.

## <a href="" id="licensebasedmonthly"></a>Monthly billing scenarios

**Scenario 1: New subscription**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación mensual. El 15 de enero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tarifa de ciclo   |4,00       |1        |4,00    

El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/2/2018         |12/3/2018    |Tarifa de ciclo   |4,00       |1        |4,00    

**Scenario 2: Change license quantity**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación mensual. El 15 de enero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tarifa de ciclo   |4,00       |1        |4,00    

El 1 de febrero aumentas la cantidad de licencias de una a dos. El 15 de febrero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13/1/2018        |12/2/2018    |Prorrateo de instancia de ciclo   |-4,00       |1        |-4,00    
|13/1/2018         |31/1/2018    | Prorrateo de instancia de ciclo   |2.45       |1        |2.45    
|1/2/2018         |12/2/2018    | Prorrateo de instancia de ciclo   |1.55       |2        |3.10    
|13/2/2018         |12/3/2018    | Prorrateo de instancia de ciclo   |4,00       |2        |8,00    

**Unit Price Formulas:**

The monthly price is 4.00 and there are 31 days in the service period 1/13/2018 - 2/12/2018. Esto equivale a un precio diario de 0,129 (4/31).

There are 19 days in the proration period 1/13/2018 - 1/31/2018.

Precio unitario de prorrateo = 2,451 = 19 x 0,129

There are 12 days in the proration period 2/1/2018 - 2/12/2018.

Precio unitario de prorrateo = 1,54 = 12 x 0,129

**Scenario 3: Suspend before 30 days**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación mensual. El 15 de enero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tarifa de ciclo   |4,00       |1        |4,00    

On February 1 you suspend a subscription. El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/2/2018|Cuota de cancelación|-4,00|1|-4,00

**Scenario 4: Suspend after 30 days**

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

**Unit Price Formulas:**

The monthly price is 4.00 and there are 28 days in the service period 2/13/2018 - 3/12/2018. Esto equivale a un precio diario de 0,143 (4/28).

Precio unitario = días en período de servicio x precio diario x número de licencias.

There are 12 days in the cancellation period 3/1/2018 - 3/12/2018. 

Therefore, the unit price = -1.716 (12 x 0.143 x (-1)).

## <a name="annual-billing-scenarios"></a>Escenarios de facturación anual

**Scenario 1: New subscription**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación anual. El 15 de enero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

**Scenario 2: Add license after subscription anniversary date but before billing date**

Adquieres una nueva suscripción el 11/02/17 con una licencia por 211,20 USD al año. El aniversario de la suscripción está establecido el día 11 de cada mes. El sistema de facturación de Microsoft crea las siguientes líneas de facturación: 

-   $211.20 charge for period 2/11/17 - 2/10/18. 

El 12/02/17 adquieres una segunda licencia. Tu fecha de facturación es el 14/02/17. Se generarán los archivos de factura y de conciliación. El archivo de conciliación contendrá las siguientes líneas de facturación: 

|Fecha de inicio de cargo  |Fecha de fin de cargo  |Tipo de cargo  |Precio unitario |Cantidad | Volumen |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Tarifas prorrateadas al comprar |211,20 |1 | 211,20 |

En el aniversario de la suscripción, 11/03/17, el sistema de facturación de Microsoft crea las siguientes líneas de facturación para el aumento de licencias e 12/02/17: 
-   -$211.20 credit for period 2/11/17 - 2/10/18. 
-   $0.58 prorated charge per license for 1 license for period 2/11/17 - 2/11/17. 
-   $15.62 prorated charge per license for 2 licenses for period 2/12/17 - 3/10/2017. 
-   $195.00 prorated charge per license for 2 licenses for period 3/11/2017 - 2/10/2018. 

El 11/02/17 adquieres una suscripción. El 12/02/17 agregas una licencia. Tu fecha de facturación es el 14/02/17. El 11/02/18 se renueva la suscripción.

La próxima fecha de facturación es el 14/03/17 y se generan los archivos de factura y conciliación. El archivo de conciliación contendrá las siguientes líneas de facturación: 

|Fecha de inicio de cargo  |Fecha de fin de cargo  |Tipo de cargo  |Precio unitario |Cantidad | Volumen |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Prorrateo de instancia de ciclo |-211,20 |1 |-211,20 |
|11/02/2017 |11/02/2017 |Prorrateo de instancia de ciclo |0,58 |1 |0,58 |
|12/02/2017 |10/03/2017 |Prorrateo de instancia de ciclo |15,62 |2 |31,25 |
|11/03/2017 |10/02/2018 |Prorrateo de instancia de ciclo |195,00 |2 |390,00 |

La suscripción se renueva el 11/02/18 por otro período de 12 meses.


**Scenario 3: Change license quantity**

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

**Unit Price Formulas:**

El precio anual es 48,00 que equivale a un precio diario de 0,13 (48,00/365).

Precio unitario = días en período de servicio x precio diario x número de licencias.

There are 19 days in service period 1/13/2018 - 1/31/2018. 

Por lo tanto, el precio unitario = 2,47 (19x0,13x1)

There are 346 days in service period 2/1/2018 - 1/12/2019. 

Por lo tanto, el precio unitario = 44,98 (346x0,13x2)

**Scenario 4: Suspend before 30 days**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación anual. El 15 de enero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

El 1 de febrero suspendes la suscripción. El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Cuota de cancelación|-48,00|1|-48,00

**Scenario 5: Suspend after 30 days**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación anual. El 15 de enero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

El 15 de febrero el archivo de conciliación basado en licencia no contendrá ninguna línea de facturación para esta suscripción.
El 1 de marzo suspendes tu suscripción. El 15 de marzo el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:

|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Volumen |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/1/2019|Cuota de cancelación|-41,34|1|-41,34

**Unit Price Formulas:**

El precio anual es 48,00 que equivale a un precio diario de 0,13 (48,00/365).

Precio unitario = días en período de servicio x precio diario x número de licencias.

There are 318 days in service period 3/1/2018 - 1/12/2019. 

Por lo tanto, el precio unitario = 41,34 (318x0,13x1). Dado que es un crédito, el precio unitario es-41,34.

**Scenario 6: Suspend and reactivate**

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

**Unit Price Formulas:**

El precio anual es 48,00 que equivale a un precio diario de 0,13 (48,00/365).

Precio unitario = días en período de servicio x precio diario x número de licencias.

There are 318 days in service period 3/1/2018 - 1/12/2019. 

Por lo tanto, el precio unitario = 41,34 (318x0,13x1).
