---
title: "Escenarios comunes de facturación | Centro de partners"
description: "En este tema se explica qué debes esperar ver en tu factura después de agregar nuevas suscripciones, ajustar la cantidad de licencias de una suscripción o cancelar una suscripción. Las suscripciones basadas en licencia y basadas en uso se verán afectadas de forma diferente."
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.openlocfilehash: 92805672975e319b53c2cd89063442df2feb1267
ms.sourcegitcommit: e8b504fa98b3ec4c7c8fd954f63ea81299791906
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/01/2017
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

En los meses que no haya cambios en las suscripciones basadas en licencia,se mostrará un elemento de una línea única para cada suscripción en tu factura. Esto es para el cargo anticipado del mes siguiente.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td>Escenario</td>
<td>Descripción</td>
<td>Ejemplo</td>
</tr>
<tr class="even">
<td>Nueva suscripción agregada</td>
<td><p>El período entre la fecha de inicio de la suscripción y la primera fecha de facturación es GRATUITO.</p>
<p>El archivo de conciliación incluirá un elemento de línea única:</p>
<ul>
<li>El cargo anticipado para el mes siguiente</li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td>Nueva suscripción: cancelada antes del corte de facturación</td>
<td>Los cargos no se aplicarán a la cuenta. La suscripción no aparecerá en el archivo conciliación. Esto es útil si quieres realizar pruebas sin incurrir en gastos de suscripción.</td>
<td></td>
</tr>
<tr class="even">
<td>Nueva suscripción: con ajustes de cantidad de licencias durante el período gratuito</td>
<td><p>El archivo de conciliación incluirá elementos de varias líneas:</p>
<ul>
<li>Cambios de cantidad de licencias, cobrados a un precio unitario de 0 (cero). (No hay ningún coste por cambios de licencia durante el período gratuito)</li>
<li>Cargo por adelantado del próximo mes, que refleja la cantidad nueva.</li>
</ul></td>
<td>Uso prorrateado:
<ul>
<li>Del 3 de junio al 7 de junio para 10 licencias = cargo CERO</li>
<li>Del 8 de junio al 11 de junio para 20 licencias = cargo CERO</li>
<li>Del 12 de junio al 14 de junio por 15 licencias = cargo CERO</li>
</ul>
<p>Fecha límite de facturación: cargo anticipado para el período de mes completo desde el 15 de junio hasta el 14 de julio para 15 licencias. Si el cargo por suscripción mensual es 10USD, el coste sería 10USD x 15 licencias = 150USD.</p></td>
</tr>
<tr class="odd">
<td>Suscripción existente: aumento o reducción de la cantidad de licencias</td>
<td><p>El archivo de conciliación incluirá elementos de varias líneas:</p>
<ul>
<li>Inversión del cargo anticipado</li>
<li>Cargos por uso prorrateado</li>
<li>Cargo anticipado del mes siguiente</li>
</ul></td>
<td><p>Uso prorrateado:</p>
<ul>
<li>Del 15 de julio al 19 de julio por 15 licencias = 26,61USD</li>
<li>Del 20 de julio al 30 de julio por 12 licencias = 46,84USD</li>
<li>Del 31 de julio al 9 de agosto por 18 licencias = 63,87USD</li>
<li>Del 10 de agosto al 14 de agosto por 10 licencias = 17,74USD</li>
</ul>
La inversión del cargo anticipado para el período de mes completo desde el 15 de julio hasta el 14 de agosto =-165USD.
<p>Fecha límite de facturación: cargo anticipado para el período de mes completo desde el 15 de agosto hasta el 14 de septiembre para 10 licencias = 110USD.</p></td>
</tr>
<tr class="even">
<td>Cancelación: no hay cambios de licencias anteriores</td>
<td><p>El archivo de conciliación incluirá un elemento de línea única:</p>
<ul>
<li>Un crédito por los días sin uso, ya que se facturó la totalidad del período de forma anticipada en el extracto de facturación anterior. Esto se calcula según la fecha de finalización de la suscripción.</li>
</ul></td>
<td>Cargo anticipado facturado anteriormente: del 15 de agosto al 14 de septiembre por 10 licencias = 100USD.
<p>Parte consumida del cargo anticipado desde el 15 de agosto hasta el 24 de agosto.</p>
<p>Crédito por días sin usar: del 25 de agosto al 14 de septiembre por 10 licencias =-74,51USD.</p></td>
</tr>
<tr class="odd">
<td>Cancelación: con cambios de licencias anteriores</td>
<td><p>El archivo de conciliación incluirá elementos de varias líneas:</p>
<ul>
<li>Inversión del cargo anticipado</li>
<li>Cargos por uso prorrateado</li>
<li>Un crédito por días no usados</li>
</ul></td>
<td>Cargo anticipado facturado anteriormente: del 15 de agosto al 14 de septiembre por 10 licencias = 100USD.
<p>Uso prorrateado:</p>
<ul>
<li>Del 15 de agosto al 24 de agosto por 10 licencias</li>
<li>Del 25 de agosto al 14 de septiembre por 5 licencias</li>
</ul>
<p>Crédito por días sin usar: del 1 de septiembre al 14 de septiembre por 5 licencias.</p>
<p>La inversión del cargo anticipado para el período de mes completo desde el 15 de agosto hasta el 14 de septiembre =-100USD.</p></td>
</tr>
</tbody>
</table>




 



