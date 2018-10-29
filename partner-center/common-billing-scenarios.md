---
title: Escenarios comunes de facturación | Centro de partners
ms.topic: article
ms.date: 10/29/2018
description: En este tema se explica qué debes esperar ver en tu factura después de agregar nuevas suscripciones, ajustar la cantidad de licencias de una suscripción o cancelar una suscripción. Las suscripciones basadas en licencia y basadas en uso se verán afectadas de forma diferente.
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.author: evansma
Keywords: billing, payments, orders, usage, license-based billing, anniversary date, term, cancellation, renewal, price formula,reconciliation file, recon file
ms.localizationpriority: medium
ms.openlocfilehash: df555040c02f3317445efd391d84684f1a7e6dac
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/29/2018
ms.locfileid: "5795638"
---
# <a name="common-billing-scenarios"></a>Escenarios comunes de facturación

**Se aplica a**

-   Facturación de programa de proveedor de soluciones en la nube

En este tema se explica qué debes esperar ver en tu factura después de agregar nuevas suscripciones, ajustar la cantidad de licencias en una suscripción o cancelar una suscripción. Las suscripciones basadas en licencia y basadas en uso se ven afectadas de forma diferente.

## <a name="in-this-section"></a>En esta sección

-   [Facturación basada en uso](#usagebased)

-   [Facturación basada en licencia](#licensebased)

## <a href="" id="usagebased"></a>Facturación basada en uso

Las suscripciones basadas en uso se facturan mensualmente, por período vencido, el día del aniversario de la suscripción. Por ejemplo, si la fecha de aniversario de suscripción es el día 15, se te cobrará el 15 de enero por el período de servicio del 15 de diciembre al 14 de enero. Se te hará un cargo de nuevo el 15 de febrero durante el período de servicio del 15 de enero al 14 de febrero, etc. Los cargos que se generan el día del aniversario de la suscripción aparecerán en el siguiente archivo de conciliación y factura.

La suscripción basada en uso se puede suspender en cualquier momento. 

La lista de precios CSP de Azure se publica mensualmente y se puede encontrar en la página de venta de Centro de partners->Precios y ofertas. Ten en cuenta que los precios pueden cambiar a diario y se reflejan en la pestaña Historial de cambios de la lista de precios.

Los cargos por uso se basan en los precios diarios. Si el precio cambia durante el período de servicio, verás una línea de facturación para cada período de servicio prorrateado y precio aplicable.

## <a href="" id="licensebased"></a>Facturación basada en licencia

**Facturación:** las suscripciones basadas en licencia se facturan por adelantado el día del aniversario de la suscripción.

**Día de aniversario:** el aniversario es el día del mes en que compraste la suscripción. Por ejemplo, si has comprado la suscripción el 15 de enero, el día de aniversario será el 15 de cada mes.

**Plazo:** todas las suscripciones basadas en licencia tienen un plazo de pago de 12meses, que comienza en la fecha de compra.

**Cancelación:** las suscripciones suspendidas el mes 1 serán abonadas al 100%. Las suscripciones suspendidas los meses 2-12 se abonarán de forma prorrateada.

**Renovación:** todas las suscripciones basadas en licencia se renuevan automáticamente 12meses después de que comience el plazo pagado.

## <a href="" id="licensebasedmonthly"></a>Escenarios comunes mensuales

**Escenario 1: Nueva suscripción**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación mensual. El 15 de enero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tarifa de ciclo   |4,00       |1        |4,00    

El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/2/2018         |12/3/2018    |Tarifa de ciclo   |4,00       |1        |4,00    

**Escenario 2: Cambiar cantidad de licencias**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación mensual. El 15 de enero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tarifa de ciclo   |4,00       |1        |4,00    

El 1 de febrero aumentas la cantidad de licencias de una a dos. El 15 de febrero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 13/1/2018        |12/2/2018    |Prorrateo de instancia de ciclo   |-4,00       |1        |-4,00    
|13/1/2018         |31/1/2018    | Prorrateo de instancia de ciclo   |2.45       |1        |2.45    
|1/2/2018         |12/2/2018    | Prorrateo de instancia de ciclo   |1.55       |2        |3.10    
|13/2/2018         |12/3/2018    | Prorrateo de instancia de ciclo   |4,00       |2        |8,00    

**Fórmulas de precio unitario:**

El precio mensual es 4,00 y hay 31 días en el periodo de servicio 13/1/2018 – 12/2/2018. Esto equivale a un precio diario de 0,129 (4/31).

Hay 19 días en el período de prorrateo 13/1/2018 – 31/1/2018.

Precio unitario de prorrateo = 2,451 = 19 x 0,129

Hay 12 días en el período de prorrateo 1/2/2018 – 12/2/2018.

Precio unitario de prorrateo = 1,54 = 12 x 0,129

**Escenario 3: Suspensión antes de 30 días**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación mensual. El 15 de enero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |12/2/2018    |Tarifa de ciclo   |4,00       |1        |4,00    

El 1 de febrero suspendes la suscripción. El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/2/2018|Cuota de cancelación|-4,00|1|-4,00

**Escenario 4: Suspensión después de 30 días**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación mensual. El 15 de enero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/2/2018|Tarifa de ciclo|4,00|1|4,00

El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/2/2018|12/3/2018|Tarifa de ciclo|4,00|1|4,00

El 1 de marzo suspendes la suscripción. El 15 de marzo el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/3/2018|Cuota de cancelación|-1,72|1|-1,72

**Fórmulas de precio unitario:**

El precio mensual es 4,00 y hay 28 días en el periodo de servicio 13/2/2018 – 12/3/2018. Esto equivale a un precio diario de 0,143 (4/28).

Precio unitario = días en período de servicio x precio diario x número de licencias.

Hay 12 días en el período de cancelación 1/3/2018 – 12/3/2018. 

Por lo tanto, el precio unitario = -1,716 (12 x 0,143 x (-1)).

## <a name="annual-billing-scenarios"></a>Escenarios de facturación anual

**Escenario 1: Nueva suscripción**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación anual. El 15 de enero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

**Escenario 2: Agregar una licencia después de la fecha del aniversario de la suscripción, pero antes de la fecha de facturación**

Adquieres una nueva suscripción el 11/02/17 con una licencia por 211,20USD al año. El aniversario de la suscripción está establecido el día 11 de cada mes. El sistema de facturación de Microsoft crea las siguientes líneas de facturación: 

-   Cargo de 211,20USD para el período del 11/02/17 al 10/02/18. 

El 12/02/17 adquieres una segunda licencia. Tu fecha de facturación es el 14/02/17. Se generarán los archivos de factura y de conciliación. El archivo de conciliación contendrá las siguientes líneas de facturación: 
|Fecha de inicio de cargo  |Fecha de fin de cargo  |Tipo de cargo  |Precio unitario |Cantidad | Importe |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Tarifas prorrateadas al comprar |211,20 |1 | 211,20 |
 
En el aniversario de la suscripción, 11/03/17, el sistema de facturación de Microsoft crea las siguientes líneas de facturación para el aumento de licencias e 12/02/17: 
-   Crédito de –211,20USD para el período del 11/02/17 al 10/02/18. 
-   Cargo prorrateado de 0,58USD por licencia para 1 licencia para el período del 11/02/17 al 11/02/17. 
-   Cargo prorrateado de 15,62USD por licencia para 2 licencias para el período del 12/02/17 al 10/03/2017. 
-   Cargo prorrateado de 195,00USD por licencia para 2 licencias para el período del 11/03/2017 al 10/02/2018. 
 
El 11/02/17 adquieres una suscripción. El 12/02/17 agregas una licencia. Tu fecha de facturación es el 14/02/17. El 11/02/18 se renueva la suscripción.

La próxima fecha de facturación es el 14/03/17 y se generan los archivos de factura y conciliación. El archivo de conciliación contendrá las siguientes líneas de facturación: 
|Fecha de inicio de cargo  |Fecha de fin de cargo  |Tipo de cargo  |Precio unitario |Cantidad | Importe |
|      :---:   |      :---:   |      :---:   |      :---:   |:---:   |:---:   |
|11/02/2017 |10/02/2018 |Prorrateo de instancia de ciclo |-211,20 |1 |-211,20 |
|11/02/2017 |11/02/2017 |Prorrateo de instancia de ciclo |0,58 |1 |0,58 |
|12/02/2017 |10/03/2017 |Prorrateo de instancia de ciclo |15,62 |2 |31,25 |
|11/03/2017 |10/02/2018 |Prorrateo de instancia de ciclo |195,00 |2 |390,00 |
 
La suscripción se renueva el 11/02/18 por otro período de 12 meses.


**Escenario 3: Cambiar cantidad de licencias**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación anual. El 15 de enero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

El 1 de febrero aumentas la cantidad de licencias de una a dos. El 15 de febrero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  | 
13/1/2018|12/1/2019|Prorrateo de instancia de ciclo|-48,00|1|-48,00
13/1/2018|31/1/2018|Prorrateo de instancia de ciclo|2,47|1|2,47
1/2/2018|12/1/2019|Prorrateo de instancia de ciclo|44,98|2|89,96

**Fórmulas de precio unitario:**

El precio anual es 48,00 que equivale a un precio diario de 0,13 (48,00/365).

Precio unitario = días en período de servicio x precio diario x número de licencias.

Hay 19 días en el período de servicio 13/1/2018 – 31/1/2018. 

Por lo tanto, el precio unitario = 2,47 (19x0,13x1)

Hay 346 días en el período de servicio 1/2/2018 – 12/1/2019. 

Por lo tanto, el precio unitario = 44,98 (346x0,13x2)

**Escenario 4: Suspensión antes de 30 días**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación anual. El 15 de enero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

El 1 de febrero suspendes la suscripción. El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Cuota de cancelación|-48,00|1|-48,00

**Escenario 5: Suspensión después de 30 días**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación anual. El 15 de enero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

El 15 de febrero el archivo de conciliación basado en licencia no contendrá ninguna línea de facturación para esta suscripción.
El 1 de marzo suspendes tu suscripción. El 15 de marzo el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/1/2019|Cuota de cancelación|-41,34|1|-41,34

**Fórmulas de precio unitario:**

El precio anual es 48,00 que equivale a un precio diario de 0,13 (48,00/365).

Precio unitario = días en período de servicio x precio diario x número de licencias.

Hay 318 días en el período de servicio 1/3/2018 – 12/1/2019. 

Por lo tanto, el precio unitario = 41,34 (318x0,13x1). Dado que es un crédito, el precio unitario es-41,34.

**Escenario 6: Suspender y reactivar**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación anual. El 15 de enero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Tarifas prorrateadas al comprar|48,00|1|48,00

El 1 de febrero suspendes la suscripción. El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|12/1/2019|Cuota de cancelación|-48,00|1|-48,00

El 1 de marzo vuelves a activar tu suscripción. El 15 de marzo el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|12/1/2019|Tarifas prorrateadas al comprar|41,34|1|41,34

**Fórmulas de precio unitario:**

El precio anual es 48,00 que equivale a un precio diario de 0,13 (48,00/365).

Precio unitario = días en período de servicio x precio diario x número de licencias.

Hay 318 días en el período de servicio 1/3/2018 – 12/1/2019. 

Por lo tanto, el precio unitario = 41,34 (318x0,13x1).
