---
title: Leer factura | Centro de partners
ms.topic: article
ms.date: 03/15/2019
description: La factura mensual es un resumen de todos los cargos (incluidos el programa, los productos y los clientes) para el período mensual actual. Está disponible en el centro de partners.
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: facturación de suscripción, facturación, facturación en el centro de partners, facturación del centro de partners, leer mi factura, factura, factura del centro de partners, factura CSP, ¿dónde está mi factura?
ms.localizationpriority: medium
ms.openlocfilehash: 9754127cf02d8c8a1098d4a3045b8960978483cc
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133965"
---
# <a name="read-your-bill"></a>Leer tu factura

**Se aplica a**

-  Centro de partners
-  Centro de partners para Microsoft Cloud for US Government


Para la factura, vaya a la **centro de partners** menú y, a continuación, seleccione **facturación** ver su historial de facturación y las tendencias, vínculos a su archivo de conciliación y la factura y el pago más reciente.

Los partners del programa Proveedor de soluciones en la nube que han elegido la facturación mensual pagan a Microsoft por período vencido de 60 días las suscripciones de sus clientes (basadas en licencia y basadas en el uso).

> [!NOTE]  
> La factura es un resumen de todos los cargos--en el programa, productos y clientes--para el período de facturación actual y está disponible en dos (2) días de la fecha de facturación seleccionada en hora UTC. Por ejemplo, si tienes un 12 de septiembre fecha de facturación, el proceso de generación de facturas comenzar a las 12:00 A.M. UTC en el 13 y completar por 12:00 A.M. UTC el día 14. Si no ve su factura por hora UTC de 11:59 P.M. el día 15, que está fuera de su contrato de nivel de servicio y debe realizar una solicitud de servicio. 

Recibirás una factura por los cargos basados en licencia (Office365) y basados en uso (Azure) y una factura independiente por cargos de un solo uso (instancias de VM reservadas para Azure).

Para obtener información detallada sobre los cargos, usa los archivos de conciliación correspondiente. Los archivos de conciliación incluyen los identificadores de cliente y de suscripción que usarás para crear facturas de cliente. Para obtener más información, consulta el tema sobre [cómo usar archivos de conciliación](use-the-reconciliation-files.md).

## <a name="invoice-file-definitions"></a>Definiciones de archivo de factura


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Field</strong></td>
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
<td>Facturar a</td>
<td>La dirección a la que enviamos tu factura. Para cambiar el nombre de la empresa o la dirección, edite el perfil de facturación de su centro de partners. </td>
</tr>
<tr class="odd">
<td>Cargos basados en licencias</td>
<td>Cargos fijos mensuales (o anuales) para las licencias adquiridas basadas en el uso, facturados previamente al uso del servicio. Este número es la suma de todos los cargos en la columna &quot;Subtotal&quot; del archivo de conciliación basada en licencia (columna T).</td>
</tr>
<tr class="even">
<td>Cargos basados en uso</td>
<td>El uso de Azure, incluidos nuevos servicios o aplicaciones habilitados y usados durante el mes de facturación. Este número es la suma de todos los cargos en la columna &quot;PretaxCharges&quot; del archivo de conciliación basada en uso (columna Z).</td>
</tr>
<tr class="odd">
<td>Descuentos</td>
<td>Por ejemplo, el descuento que el cliente recibe del precio normal de la suscripción. Esto se muestra como un importe fijo, no como un precio por unidad o licencia.</td>
</tr>
<tr class="odd">
<td>Créditos</td>
<td>Crédito o ajustes que corresponden a los cambios realizados en las suscripciones (por ejemplo: aumento o disminución de puestos).</td>
</tr>
<tr class="even">
<tr class="even">
<td>Subtotal</td>
<td>Total antes de impuestos y créditos y cargos exclusivos de impuestos.</td>
</tr>
<td>Impuestos</td>
<td>El total de impuestos para los cargos actuales según se suman en la sección de detalles a partir de la página 2 de la factura. Este número es la suma de todos los cargos de:
<ul>
<li>la columna &quot;TaxAmount&quot; del archivo de conciliación basada en uso (columna AA) y </li>
<li>la columna &quot;Tax&quot; del archivo basado en licencia (columna U).</li>
</ul></td>
</tr>
<tr class="odd">
<td>Otros créditos</td>
<td>Créditos exclusivos de impuestos.</td>
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
<td>El período mensual que hicieron nacer a la fecha de factura. Este es el período durante el cual se consumen los servicios basados en uso y servicios basados en licencias se han reconciliado de cualquier cambio en el número de licencias o ajustes de crédito.</td>
</tr>
<tr class="even">
<td>Invoice date</td>
<td>La fecha de facturación o la fecha de aniversario en el que se genera la factura cada mes.</td>
</tr>
<tr class="odd">
<td>Condiciones de pago</td>
<td>Para las compras de pago único siempre serán 60 días.</td>
</tr>
<tr class="even">
<td>Payment due date</td>
<td>Fecha en la que debe recibirse tu pago.</td>
</tr>
<tr class="odd">
<td>Customer PO</td>
<td>El número de pedido de compra.</td>
</tr>
<tr class="even">
<td>Customer service</td>
<td>La dirección del sitio web para acceder al servicio de atención al cliente.</td>
</tr>
<tr class="odd">
<td>Destinatario del servicio</td>
<td>La dirección en la que se usa el servicio. (Esta es la dirección de empresa legales asociada con la empresa de investigación.)</td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a>Lista desglosada de los cargos de pago único

|**Field** |**Definición**|
|:----------------|:-----------------------------|
|Fecha |Fecha de compra. |
|Descripción |Nombre del producto. |
|Cantidad |Número de productos (reservas, por ejemplo) adquiridos. |
|Precio unitario |Precio por producto (reserva, por ejemplo). |
|Descuentos |Descuentos aplicables. |
|Importe antes de impuestos |Subtotal de las compras antes de impuestos. |
|Impuesto sobre ventas |Importe de impuestos. |
|Total |Total que se pagará. |
 



