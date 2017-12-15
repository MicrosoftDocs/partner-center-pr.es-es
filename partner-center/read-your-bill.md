---
title: Leer factura | Centro de partners
description: "La factura mensual es un resumen de todos los cargos (incluidos el programa, los productos y los clientes) para el período mensual actual. Está disponible en el panel del Centro de partners."
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
keywords: "facturación de suscripción, facturación, facturación en el centro de partners, facturación del centro de partners, leer mi factura, factura, factura del centro de partners, factura CSP, ¿dónde está mi factura?"
ms.openlocfilehash: d24c9ad9ac90597c8e56843a25a69b9108c020d2
ms.sourcegitcommit: 2c99458586d7d536f5502317653eb4a43e2fdafc
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/10/2017
---
# <a name="read-your-bill"></a>Leer tu factura

**Se aplica a**

-  Centro de partners
-  Centro de partners para Microsoft Cloud for US Government
-  Centro de partners para Microsoft Cloud Alemania

Para la facturación, ve al menú **Panel** y luego selecciona **Facturación** para tu historial de facturación y las tendencias, vínculos a tu factura y archivo de conciliación y el pago más reciente.

Los partners del programa Proveedor de soluciones en la nube que han elegido la facturación mensual pagan a Microsoft por período vencido de 60 días las suscripciones de sus clientes (basadas en licencia y basadas en el uso).

>**Nota**<br>
La factura mensual es un resumen de todos los cargos (incluidos el programa, los productos y los clientes) para el período de facturación actual y está disponible en el plazo de cuatro (4) días a partir de la fecha de facturación seleccionada.


Para obtener información detallada sobre los cargos, usa los archivos de conciliación correspondientes. Los archivos de conciliación incluyen los identificadores de cliente y de suscripción que usarás para crear facturas de cliente. Para obtener más información, consulta el tema sobre [cómo usar archivos de conciliación](use-the-reconciliation-files.md).

## <a name="invoice-file-definitions"></a>Definiciones de archivo de factura


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Campo</strong></td>
<td><strong>Descripción</strong></td>
</tr>
<tr class="even">
<td>US FEIN</td>
<td>El número de identificación fiscal federal.</td>
</tr>
<tr class="odd">
<td>Customer number</td>
<td>El número de cliente.</td>
</tr>
<tr class="even">
<td>Bill to</td>
<td>La dirección a la que enviamos tu factura. Para cambiar esta dirección, ve a Configuración de la cuenta > Perfil de facturación de partner. </td>
</tr>
<tr class="odd">
<td>Recurring charges</td>
<td>Cargos fijos mensuales (o anuales) para las licencias adquiridas basadas en el uso, facturados previamente al uso del servicio. Este número es la suma de todos los cargos en la columna &quot;Subtotal&quot; del archivo de conciliación basada en licencia (columna T).</td>
</tr>
<tr class="even">
<td>Usage charges</td>
<td>El uso de Azure, incluidos nuevos servicios o aplicaciones habilitados y usados durante el mes de facturación. Este número es la suma de todos los cargos en la columna &quot;PretaxCharges&quot; del archivo de conciliación basada en uso (columna Z).</td>
</tr>
<tr class="odd">
<td>Créditos y ajustes</td>
<td>Crédito o ajustes que corresponden a los cambios realizados en las suscripciones (por ejemplo: aumento o disminución de puestos).</td>
</tr>
<tr class="even">
<td>Other discounts</td>
<td>Por ejemplo, el descuento que el cliente recibe del precio normal de la suscripción. Esto se muestra como un importe fijo, no como un precio por unidad o licencia.</td>
</tr>
<tr class="odd">
<td>Taxes</td>
<td>El total de impuestos para los cargos actuales según se suman en la sección de detalles a partir de la página 2 de la factura. Este número es la suma de todos los cargos de:
<ul>
<li>la columna &quot;TaxAmount&quot; del archivo de conciliación basada en uso (columna AA) y </li>
<li>la columna &quot;Tax&quot; del archivo basado en licencia (columna U).</li>
</ul></td>
</tr>
<tr class="even">
<td>Total current charges</td>
<td>El importe debido en la divisa de facturación para el período de facturación, que se debe abonar antes de la fecha de vencimiento de pago.</td>
</tr>
<tr class="odd">
<td>Payment instructions</td>
<td>Describe cómo pagar la factura, según de tu región. Al realizar un pago, siempre incluye el número de factura.</td>
</tr>
<tr class="even">
<td>Invoice no</td>
<td>El número de la factura.</td>
</tr>
<tr class="odd">
<td>Billing period</td>
<td>A los partners de CSP se les factura mensual o anualmente.</td>
</tr>
<tr class="even">
<td>Invoice date</td>
<td>La fecha en la que recibes tu factura.</td>
</tr>
<tr class="odd">
<td>Payment due date</td>
<td>Fecha en la que debe recibirse tu pago.</td>
</tr>
<tr class="even">
<td>Customer PO</td>
<td>El número de pedido de compra.</td>
</tr>
<tr class="odd">
<td>Customer service</td>
<td>La dirección del sitio web para acceder al servicio de atención al cliente.</td>
</tr>
<tr class="even">
<td>Destinatario del servicio</td>
<td>La dirección en la que se usa el servicio. (Esta es la dirección legal de la compañía asociada al control de la compañía y no se puede cambiar).</td>
</tr>
</tbody>
</table>

 

 

 



