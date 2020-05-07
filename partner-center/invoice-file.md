---
title: Archivos de factura | Centro de Partners
ms.topic: article
ms.date: 08/26/2019
description: Comprenda los campos del archivo de factura para la facturación del centro de Partners.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
keywords: facturación, factura
ms.localizationpriority: medium
ms.openlocfilehash: bcbb784ceda9e4b8cbddf61e0b5380ad18d3f264
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798903"
---
# <a name="invoice-files"></a>Archivos de factura

**Roles adecuados**
-   Administrador global
-   Administrador de usuarios
-   Administrador de facturación
-   Agente del departamento de soporte técnico

Puede usar las tablas siguientes para comprender los campos de los archivos de factura del centro de Partners.

## <a name="invoice-file-fields"></a>Campos de archivo de factura

Los siguientes campos aparecen en los archivos de factura.

| Campo | Definición |
| ----- | ---------- |
| US FEIN | El número de identificación de la empresa federal (FEIN). Este es el número de identificación de impuesto federal de Estados Unidos. |
| Número de cliente | Su número de cliente. |
| Dirección de facturación | La dirección a la que enviamos tu factura. Puede cambiar el nombre o la dirección de la empresa en el perfil de facturación del centro de Partners. |
| Cargos basados en licencias | Los cargos fijos mensuales o anuales de las licencias basadas en uso compradas, facturadas por adelantado del servicio. Este número es la suma de todos los cargos de la columna de **subtotal** (columna **T**) del archivo de conciliación basado en licencias. |
| Cargos basados en el uso | El uso de Azure. Esto incluye nuevos servicios o aplicaciones habilitados y usados durante el período de facturación. Este número es la suma de todos los cargos de la columna **PretaxCharges** (columna **Z**) del archivo de conciliación basado en el uso. |
| Descuentos | Descuento que el cliente recibe del precio normal de la suscripción. Este número se muestra como una *cantidad plana*, no como un precio por unidad o licencia. |
| Créditos | Créditos o ajustes para los cambios realizados en las suscripciones (por ejemplo, el asiento aumenta o disminuye). |
| Subtotal | Total antes de impuestos y cargos y créditos exclusivos de impuestos. |
| Impuesto | El impuesto total de los cargos actuales, tal como se ha totalizado en la sección de **detalles** a partir de la página 2 de la factura. Este número es la suma de todos los cargos de la columna **TaxAmount** (columna **AA**) del archivo de conciliación basado en el uso, y la columna de **impuestos** (columna **U**) del archivo de conciliación basado en licencias. |
| Otros créditos | Créditos de impuestos exclusivos. |
| Cargos actuales totales | La cantidad debida a la moneda de facturación para el período de facturación. Estos cargos se deben a la fecha de vencimiento del pago. |
| Instrucciones de pago | Descripción de cómo pagar la factura, en función de su región. *Asegúrese de incluir siempre el número de factura al realizar un pago.* |
| Invoice no | El número de la factura. |
| Período de facturación | El período mensual que conduce a la fecha de la factura. Este es el período durante el cual se consumen los servicios basados en el uso y se concilian los servicios basados en licencias para los ajustes de crédito o cambios en el recuento de licencias. |
| Fecha de la factura | Fecha de facturación o fecha de aniversario en la que se genera la factura cada mes. |
| Condiciones de pago | El plazo de pago. En el caso de las compras de un solo tiempo, siempre será de 60 días. |
| Fecha de vencimiento del pago | Fecha en la que se debe recibir el pago. |
| OC del cliente | El pedido del número de compra. |
| Servicio al cliente | Dirección del sitio web al que se puede tener acceso al servicio de atención al cliente. |
| Destinatario del servicio | Dirección en la que se utiliza el servicio. (Se trata de la dirección de la empresa legal asociada a la empresa investigación). |

## <a name="one-time-charges-fields"></a>Campos de cargos por única vez

Los campos siguientes solo se aplican a **cargos** únicos en el centro de Partners:

| Campo | Definición |
| ----- | ---------- |
| Fecha | Fecha de compra. |
| Descripción | Nombre de producto. |
| Cantidad | El número de productos (como reservas) adquiridos. |
| Precio unitario | Precio por producto (por ejemplo, una reserva). |
| Descuentos | Cualquier descuento aplicable. |
| Importe de impuestos previos | Subtotal de las compras antes de los impuestos. |
| Impuestos de ventas | Importe de los impuestos. |
| Total | Importe total que se va a pagar. |
