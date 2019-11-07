---
title: Leer factura | Centro de partners
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: La factura mensual es un resumen de todos los cargos (incluidos el programa, los productos y los clientes) para el período mensual actual. Está disponible en el centro de Partners.
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: facturación de suscripción, facturación, facturación en el centro de partners, facturación del centro de partners, leer mi factura, factura, factura del centro de partners, factura CSP, ¿dónde está mi factura?
ms.localizationpriority: medium
ms.openlocfilehash: 37469a72137d5bc399f5ab765c49c8accd36808d
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/06/2019
ms.locfileid: "73652173"
---
# <a name="read-your-bill"></a>Leer tu factura

**Se aplica a**

-  Centro de partners
-  Centro de partners para Microsoft Cloud for US Government


Para su factura, vaya al menú del **centro de Partners** y seleccione **facturación** para ver el historial de facturación y las tendencias, los vínculos a su archivo de conciliación y de conciliación y el pago más reciente.

Los partners del programa Proveedor de soluciones en la nube que han elegido la facturación mensual pagan a Microsoft por período vencido de 60 días las suscripciones de sus clientes (basadas en licencia y basadas en el uso).

> [!NOTE]  
> La factura es un resumen de todos los cargos, en el programa, los productos y los clientes, para el período de facturación actual y está disponible en un plazo de dos (2) días a partir de la fecha de facturación seleccionada en la hora UTC. Por ejemplo, si tiene una fecha de facturación del 12 de septiembre, el proceso de generación de la factura comenzará en 12: A.M. UTC en el decimotercer y terminará en 12: A.M. UTC en el 14. Si no ve la factura en 11:59PM UTC el día 15, ya no tiene el Acuerdo de Nivel de Servicio y debe archivar una solicitud de servicio. 

Recibirás una factura por los cargos basados en licencia (Office365) y basados en uso (Azure) y una factura independiente por cargos de un solo uso (instancias de VM reservadas para Azure).

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
<td>Facturar a</td>
<td>La dirección a la que enviamos tu factura. Para cambiar el nombre o la dirección de la empresa, edite el perfil de facturación del centro de Partners. </td>
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
<li>la columna &quot;TaxAmount&quot; del archivo de conciliación basada en uso (columna AA) y</li>
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
<td>El período mensual que conduce a la fecha de la factura. Este es el período durante el cual se consumen los servicios basados en el uso y se concilian los servicios basados en licencias para los ajustes de crédito o cambios en el recuento de licencias.</td>
</tr>
<tr class="even">
<td>Invoice date</td>
<td>La fecha de facturación o la fecha de aniversario en la que se genera la factura cada mes.</td>
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
<td>La dirección en la que se usa el servicio. (Se trata de la dirección de la empresa legal asociada a la empresa investigación).</td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a>Lista desglosada de los cargos de pago único

|**Campo** |**Definición**|
|:----------------|:-----------------------------|
|Date |Fecha de compra. |
|Descripción |Nombre del producto. |
|Cantidad |Número de productos (reservas, por ejemplo) adquiridos. |
|Precio unitario |Precio por producto (reserva, por ejemplo). |
|Descuentos |Descuentos aplicables. |
|Importe antes de impuestos |Subtotal de las compras antes de impuestos. |
|Impuesto sobre ventas |Importe de impuestos. |
|Total |Total que se pagará. |
 



