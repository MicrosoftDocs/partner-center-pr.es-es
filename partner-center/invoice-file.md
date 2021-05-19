---
title: Información sobre Centro de partners facturas de facturación
ms.topic: article
ms.date: 05/18/2020
description: Comprenda los campos del archivo de factura para Centro de partners facturación. Se incluyen campos y definiciones para todos los campos de factura y campos de cargos únicos.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5cb60c775bd8de38b8d7ca69c4dd97cf11b919fd
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146619"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Información sobre Centro de partners facturación de facturación

**Roles adecuados:** Administrador global | Administrador de administración de | Administración de facturación | Agente del departamento de soporte técnico

Puede usar las tablas siguientes para comprender los campos de los Centro de partners de factura.

## <a name="invoice-file-fields"></a>Campos de archivo de factura

Los siguientes campos aparecen en los archivos de factura.

| Campo | Definición |
| ----- | ---------- |
| US FEIN | Número de identificación del patrón federal (FEIN). Este es el número Estados Unidos identificador fiscal federal. |
| Número de cliente | Su número de cliente. |
| Dirección de facturación | La dirección a la que enviamos tu factura. Puede cambiar el nombre y la dirección de la empresa en el perfil Centro de partners facturación. |
| Cargos basados en licencias | Los cargos mensuales o anuales planos de las licencias adquiridas basadas en el uso, que se facturan por adelantado del servicio. Este número es la suma de todos los cargos de la **columna Subtotal** (columna **T)** del archivo de conciliación basado en licencias. |
| Cargos basados en el uso | Uso de Azure. Esto incluye nuevos servicios o aplicaciones habilitados y usados durante el período de facturación. Este número es la suma de todos los cargos de la columna **PretaxCharges** (columna **Z)** del archivo de conciliación basado en el uso. |
| Descuentos | Descuento que el cliente recibe del precio normal de la suscripción. Este número se muestra como una *cantidad plana,* no como un precio por unidad o licencia. |
| Créditos | Créditos o ajustes para los cambios realizados en las suscripciones (por ejemplo, aumentos o disminuciones de licencias). |
| Subtotal | Total antes de impuestos y cargos y créditos exclusivos de impuestos. |
| Impuesto | El impuesto total de los cargos actuales, tal y como se muestra en la **sección Detalles** que comienza en la página 2 de la factura. Este número es la suma de todos los cargos de la columna **TaxAmount** (columna  **AA**) del archivo de conciliación basado en uso y de la columna Impuestos (columna **U**) del archivo de conciliación basado en licencia. |
| Otros créditos | Créditos exclusivos para impuestos. |
| Cargos actuales totales | Importe a pagar en la moneda de facturación para el período de facturación. Estos cargos se deben a la fecha de vencimiento del pago. |
| Instrucciones de pago | Descripción de cómo pagar la factura en función de su región. *Asegúrese siempre de incluir el número de factura al realizar un pago.* |
| Invoice no | El número de la factura. |
| Período de facturación | Período mensual que conduce a la fecha de factura. Este es el período durante el cual se consumen los servicios basados en el uso y los servicios basados en licencias se concilian para cualquier ajuste de crédito o cambio en el recuento de licencias. |
| Fecha de la factura | Fecha de facturación o fecha de aniversario en la que se genera la factura cada mes. |
| Condiciones de pago | Período de pago. Para las compras únicas, siempre será de 60 días. |
| Fecha de vencimiento del pago | Fecha en la que se debe recibir el pago. |
| OC del cliente | Su pedido de número de compra. |
| Servicio al cliente | Dirección del sitio web donde puede acceder al servicio de atención al cliente. |
| Destinatario del servicio | Dirección en la que se usa el servicio. (Esta es la dirección legal de la empresa asociada con la investigación de la empresa). |

## <a name="one-time-charges-fields"></a>Campos de cargos únicos

Los siguientes campos solo se aplican **a los cargos únicos** en Centro de partners:

| Campo | Definición |
| ----- | ---------- |
| Date | Fecha de compra. |
| Descripción | Nombre de producto. |
| Cantidad | Número de productos (por ejemplo, reservas) adquiridos. |
| Precio unitario | Precio por producto (por ejemplo, una reserva). |
| Descuentos | Los descuentos aplicables. |
| Importe antes de impuestos | Subtotal de las compras antes de impuestos. |
| Impuestos de ventas | Importe de los impuestos. |
| Total | Importe total que se va a pagar. |
