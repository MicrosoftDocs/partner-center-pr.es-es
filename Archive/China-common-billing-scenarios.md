---
title: Escenarios comunes de facturación (centro de partners operado por 21Vianet)
ms.topic: article
ms.date: 10/29/2018
description: En este tema se explica qué debes esperar ver en tu factura después de agregar nuevas suscripciones, ajustar la cantidad de puestos de una suscripción o cancelar una suscripción.
author: MaggiePucciEvans
ms.author: evansma
ms.openlocfilehash: 0da5bbf6a5c3259589973e25f592457da7e3e42e
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132345"
---
# <a name="common-billing-scenarios"></a>Escenarios comunes de facturación

**Se aplica a**

-   Centro de partners operado por 21Vianet


En este tema se explica qué debes esperar ver en tu factura después de agregar nuevas suscripciones, ajustar la cantidad de puestos de una suscripción o cancelar una suscripción. 


## <a name="licence-based-billing"></a>Facturación basada en licencia


Durante meses sin realizar cambios en las suscripciones basadas en certificado, verá un elemento de línea único para cada suscripción de su archivo de conciliación y la factura para el cargo por adelantado para el mes siguiente.

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
<td>Nueva suscripción</td>
<td><p>El período entre la fecha de inicio de la suscripción y la primera fecha de facturación es GRATUITO.</p>
<p>El archivo conciliación contendrá un elemento de línea única:</p>
<ul>
<li>cargo anticipado del mes siguiente</li>
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
<td><p>El archivo conciliación incluirá elementos de varias líneas:</p>
<ul>
<li>cambios de cantidad de licencias, cobrados a un precio unitario de 0 (cero). (No hay ningún costo por cambios de puesto durante el período gratuito)</li>
<li>cargo por adelantado del próximo mes, que refleja la cantidad nueva.</li>
</ul></td>
<td>Uso prorrateado:
<ul>
<li>Del 3 de junio al 7 de junio para 10 puestos = cargo CERO</li>
<li>Del 8 de junio al 11 de junio para 20 puestos = cargo CERO</li>
<li>Del 12 de junio al 14 de junio por 15 puestos = cargo CERO</li>
</ul>
<p>Cortar la facturación: Avance cargo durante el período de mes completo desde el 15 de junio al 14 de julio para 15 puestos. Si el cargo por suscripción mensual es 10 USD, el costo sería 10 USD x 15 puestos = 150 USD.</p></td>
</tr>
<tr class="odd">
<td>Suscripción existente: Aumentar o disminuir la cantidad de licencias</td>
<td><p>El archivo conciliación incluirá elementos de varias líneas:</p>
<ul>
<li>inversión del cargo anticipado</li>
<li>cargos por uso prorrateado</li>
<li>cargo anticipado del mes siguiente</li>
</ul></td>
<td><p>Uso prorrateado:</p>
<ul>
<li>Del 15 de julio al 19 de julio por 15 puestos = 26,61 USD</li>
<li>Del 20 de julio al 30 de julio por 12 puestos = 46,84 USD</li>
<li>Del 31 de julio al 9 de agosto por 18 puestos = 63,87 USD</li>
<li>Del 10 de agosto al 14 de agosto por 10 puestos = 17,74 USD</li>
</ul>
La inversión del cargo anticipado para el período de mes completo desde el 15 de julio hasta el 14 de agosto =-165 USD.
<p>Cortar la facturación: Avanzar cargo durante el período de mes completo desde el 15 de agosto al 14 de septiembre para 10 puestos = 110 USD.</p></td>
</tr>
<tr class="even">
<td>Cancelación: no hay cambios de asientos anteriores</td>
<td><p>El archivo conciliación contendrá un elemento de línea única:</p>
<ul>
<li>Un crédito por los días sin uso, ya que se facturó la totalidad del período de forma anticipada en el extracto de facturación anterior. Esto se calcula según la fecha de finalización de la suscripción.</li>
</ul></td>
<td>Anteriormente se facturan por adelantado cargo: Tiene asientos para el 15 de agosto a 14 de septiembre para 10 = 100 USD.
<p>Parte consumida del cargo anticipado desde el 15 de agosto hasta el 24 de agosto.</p>
<p>Crédito durante días sin usar: Tiene asientos para el 25 de agosto al 14 de septiembre para 10 =-74.51.</p></td>
</tr>
<tr class="odd">
<td>Cancelación: con cambios de puestos anteriores</td>
<td><p>El archivo conciliación incluirá elementos de varias líneas:</p>
<ul>
<li>inversión del cargo anticipado</li>
<li>cargos por uso prorrateado</li>
<li>un crédito por días no usados</li>
</ul></td>
<td>Anteriormente se facturan por adelantado cargo: Tiene asientos para el 15 de agosto a 14 de septiembre para 10 = 100 USD.
<p>Uso prorrateado:</p>
<ul>
<li>Del 15 de agosto al 24 de agosto por 10 puestos</li>
<li>Del 25 de agosto al 14 de septiembre por 5 puestos</li>
</ul>
<p>Crédito durante días sin usar: El 1 de septiembre al 14 de septiembre para 5 usuarios.</p>
<p>La inversión del cargo anticipado para el período de mes completo desde el 15 de agosto hasta el 14 de septiembre =-100 USD.</p></td>
</tr>
</tbody>
</table>
