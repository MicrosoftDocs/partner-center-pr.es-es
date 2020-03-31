---
title: Archivos de factura | Centro de Partners
ms.topic: article
ms.date: 08/26/2019
description: Comprenda los campos del archivo de factura para la facturación del centro de Partners.
ms.assetid: ''
author: jasonwhowell
ms.author: jasonh
keywords: facturación, factura
ms.localizationpriority: medium
ms.openlocfilehash: 1307a9a2f95cedde5eda7deefb61cb202597f804
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390914"
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
| Customer number | El número de cliente. |
| Facturar a | La dirección a la que enviamos tu factura. Puede cambiar el nombre o la dirección de la empresa en el perfil de facturación del centro de Partners. |
| Cargos basados en licencias | Los cargos fijos mensuales o anuales de las licencias basadas en uso compradas, facturadas por adelantado del servicio. Este número es la suma de todos los cargos de la columna de **subtotal** (columna **T**) del archivo de conciliación basado en licencias. |
| Cargos basados en uso | El uso de Azure. Esto incluye nuevos servicios o aplicaciones habilitados y usados durante el período de facturación. Este número es la suma de todos los cargos de la columna **PretaxCharges** (columna **Z**) del archivo de conciliación basado en el uso. |
| Descuentos | Descuento que el cliente recibe del precio normal de la suscripción. Este número se muestra como una *cantidad plana*, no como un precio por unidad o licencia. |
| Créditos | Créditos o ajustes para los cambios realizados en las suscripciones (por ejemplo, el asiento aumenta o disminuye). |
| Subtotal | Total antes de impuestos y créditos y cargos exclusivos de impuestos. |
| Impuestos | El impuesto total de los cargos actuales, tal como se ha totalizado en la sección de **detalles** a partir de la página 2 de la factura. Este número es la suma de todos los cargos de la columna **TaxAmount** (columna **AA**) del archivo de conciliación basado en el uso, y la columna de **impuestos** (columna **U**) del archivo de conciliación basado en licencias. |
| Otros créditos | Créditos exclusivos de impuestos. |
| Total current charges | La cantidad debida a la moneda de facturación para el período de facturación. Estos cargos se deben a la fecha de vencimiento del pago. |
| Payment instructions | Descripción de cómo pagar la factura, en función de su región. *Asegúrese de incluir siempre el número de factura al realizar un pago.* |
| Invoice no | El número de la factura. |
| Periodo de facturación | El período mensual que conduce a la fecha de la factura. Este es el período durante el cual se consumen los servicios basados en el uso y se concilian los servicios basados en licencias para los ajustes de crédito o cambios en el recuento de licencias. |
| Invoice date | Fecha de facturación o fecha de aniversario en la que se genera la factura cada mes. |
| Condiciones de pago | El plazo de pago. Para las compras de pago único siempre serán 60 días. |
| Payment due date | Fecha en la que se debe recibir el pago. |
| Customer PO | El pedido del número de compra. |
| Servicio al cliente | Dirección del sitio web al que se puede tener acceso al servicio de atención al cliente. |
| Destinatario del servicio | Dirección en la que se utiliza el servicio. (Se trata de la dirección de la empresa legal asociada a la empresa investigación). |

## <a name="one-time-charges-fields"></a>Campos de cargos por única vez

Los campos siguientes solo se aplican a **cargos** únicos en el centro de Partners:

| Campo | Definición |
| ----- | ---------- |
| Date | Fecha de compra. |
| Descripción | Nombre del producto. |
| Cantidad | El número de productos (como reservas) adquiridos. |
| Precio unitario | Precio por producto (por ejemplo, una reserva). |
| Descuentos | Descuentos aplicables. |
| Importe antes de impuestos | Subtotal de las compras antes de impuestos. |
| Impuesto sobre ventas | Importe de los impuestos. |
| Total | Importe total que se va a pagar. |
