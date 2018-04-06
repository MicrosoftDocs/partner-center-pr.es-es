---
title: Escenarios comunes de facturación | Centro de partners
description: En este tema se explica qué debes esperar ver en tu factura después de agregar nuevas suscripciones, ajustar la cantidad de licencias de una suscripción o cancelar una suscripción. Las suscripciones basadas en licencia y basadas en uso se verán afectadas de forma diferente.
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
Keywords: billing, payments, orders, usage, license-based billing, anniversary date, term, cancellation, renewal, price formula,reconciliation file, recon file
ms.openlocfilehash: 92c253bb7d73a48eb9b6acc36f54d7f33482c1ad
ms.sourcegitcommit: ec00affdfc79c1346cf8df482ce39dae98e20772
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/28/2018
---
# <a name="common-billing-scenarios"></a>Escenarios comunes de facturación

**Se aplica a**

-  Centro de partners
-  Centro de partners para Microsoft Cloud for US Government
-  Centro de partners para Microsoft Cloud Alemania

En este tema se explica qué debes esperar ver en tu factura después de agregar nuevas suscripciones, ajustar la cantidad de licencias en una suscripción o cancelar una suscripción. Las suscripciones basadas en licencia y basadas en uso se ven afectadas de forma diferente.

## <a name="in-this-section"></a>En esta sección

-   [Facturación basada en uso](#usagebased)

-   [Facturación basada en licencia](#licensebased)

## <a href="" id="usagebased"></a>Facturación basada en uso

Solo se te facturarán los servicios que usaste en el período de facturación anterior. La factura incluye cualquier servicio o aplicación de Azure habilitado que se use durante el período de facturación.

-   Las tarifas de servicio de uso medido pueden cambiar durante el ciclo de facturación.
    -   Aumentos de precio: se proporciona un aviso de 30 días.
    -   Disminuciones de precio: se reflejan el día en que tiene lugar el cambio.
    -   Las suscripciones existentes se facturan según la tarifa en vigor al comienzo del ciclo de facturación.
    -   Las nuevas suscripciones (aquellas que se crearon durante el ciclo de facturación) se facturan según la tarifa en vigor en el momento en que las agregaste.
-   Si cancelas una suscripción durante el primer ciclo de facturación, los cargos por uso aparecerán en el archivo de conciliación correspondiente al período en el que estuvo activa la suscripción.

## <a href="" id="licensebased"></a>Facturación basada en licencia

**Facturación:** las suscripciones basadas en licencia se facturan por adelantado el día del aniversario de la suscripción.

**Día de aniversario:** las suscripciones con facturación mensual se alinean con la fecha de facturación de partner y las suscripciones con facturación anual se alinean con la fecha de compra.

**Plazo:** todas las suscripciones basadas en licencia tienen un plazo de pago de 12meses. El plazo pagado comienza en la fecha de compra para suscripciones de facturación anual y en la fecha de facturación siguiente a la fecha de compra para suscripciones de facturación mensual.

**Cancelación:** si se cancelan suscripciones en los primeros 30 días del plazo pagado, se abonara el 100%. Las suscripciones canceladas después de 30 días se abonará de forma prorrateada.

**Renovación:** todas las suscripciones basadas en licencia se renuevan automáticamente 12meses después de que comience el plazo pagado.

## <a href="" id="licensebasedmonthly"></a>Escenarios comunes mensuales

**Escenario 1: Nueva suscripción**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación mensual. El 15 de enero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         | 14/1/2018   |Tarifa de compra   |0,00       |1       |0,00    
|15/1/2018         |14/2/2018    |Tarifa de ciclo   |4,00       |1        |4,00    

El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|15/2/2018         |14/3/2018    |Tarifa de ciclo   |4,00       |1        |4,00    
Seguirá facturándose el día 15 de cada mes hasta que se suspenda la suscripción.

**Escenario 2: Cambiar cantidad de licencias**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación mensual. El 15 de enero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |14/1/2018    |Tarifa de compra   |0,00       |1        |0,00    
|15/1/2018         |14/2/2018    |Tarifa de ciclo   |4,00       |1        |4,00    

El 1 de febrero aumentas la cantidad de licencias de una a dos. El 15 de febrero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
| 15/1/2018        |14/2/2018    |Prorrateo de instancia de ciclo   |-4,00       |1        |4,00    
|15/1/2018         |31/1/2018    | Prorrateo de instancia de ciclo   |2,21       |1        |2,21    
|1/2/2018         |14/2/2018    | Prorrateo de instancia de ciclo   |1,82       |2        |3,64    
|15/2/2018         |14/3/2018    | Prorrateo de instancia de ciclo   |4,00       |2        |8,00    

**Fórmulas de precio unitario:**

El precio mensual es 4,00 y hay 31 días en el periodo de servicio 15/1/2018 – 14/2/2018. Esto equivale a un precio diario de 0,13 (4/31).

Hay 17 días en el período de prorrateo 15/1/2018 – 31/1/2018.

Precio unitario de prorrateo = 2,21 = 17 x 0,13

Hay 14 días en el período de prorrateo 1/2/2018 – 14/2/2018.

Precio unitario de prorrateo = 1,82 = 14 x 0,13

**Escenario 3: Suspensión antes de 30 días**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación mensual. El 15 de enero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
|13/1/2018         |14/1/2018    |Tarifa de compra   |0,00       |1        |0,00    
|15/1/2018         |14/2/2018    |Tarifa de ciclo   |4,00       |1        |4,00    

1 de febrero suspendes la suscripción. El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
15/1/2018|14/2/2018|Cuota de cancelación|-4,00|1|4,00

**Escenario 4: Suspensión después de 30 días**

La fecha de facturación es el 15 de cada mes. El 13 de enero compras una nueva suscripción con una licencia por 4 USD al mes y seleccionas facturación mensual. El 15 de enero el archivo de conciliación basado en licencia contendrá las siguientes líneas de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
13/1/2018|14/1/2018|Tarifa de compra|0,00|1|0,00
15/1/2018|14/2/2018|Tarifa de ciclo|4,00|1|4,00

El 15 de febrero el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
15/2/2018|14/3/2018|Tarifa de ciclo|4,00|1|4,00

El 1 de marzo suspendes la suscripción. El 15 de marzo el archivo de conciliación basado en licencia contendrá la siguiente línea de facturación:
|Fecha de inicio de cargo |Fecha de fin de cargo |Tipo de cargo |Precio unitario |Cantidad |Importe |
|       :---:      |    :---:       | :---:      |:---:      |:---:    |:---:  |
1/3/2018|14/3/2018|Cuota de cancelación|-1,96|1|-1,96

**Fórmulas de precio unitario:**

El precio mensual es 4,00 y hay 28 días en el periodo de servicio 15/2/2018 – 14/3/2018. Esto equivale a un precio diario de 0,14 (4/28).

Precio unitario = días en período de servicio x precio diario x número de licencias.

Hay 14 días en el período de cancelación 1/3/2018 – 14/3/2018. 

Por lo tanto, el precio unitario =-1,96 (14x0,14 x(-1)).

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
