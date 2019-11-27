---
title: Archivos de conciliación única y periódica | Centro de Partners
ms.topic: article
ms.date: 11/21/2019
description: Comprenda los archivos de conciliación única y periódica en el centro de Partners.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 0eae0dac3cbb4991e85e335082e6c5071c62841f
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389683"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>Archivos de conciliación única y periódica

Se aplica a:

- Centro de partners
- Centro de partners para Microsoft Cloud for US Government

En este tema se explica cómo leer archivos de conciliación única y periódica en el centro de Partners.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Campos de archivos de conciliación única y periódica

| Column | Descripción |
| ------ | ----------- |
| PartnerId | Identificador de inquilino de Azure Active Directory único (Azure AD) para una entidad de facturación específica, en formato GUID. No es necesario para la reconciliación. Igual en todas las filas. |
| Identificador de cliente | Identificador único del inquilino de Azure AD, en formato GUID. Identifica al cliente. |
| Nombre del cliente | Nombre de la organización del cliente, tal y como se indicó en el centro de Partners. |
| CustomerDomainName | Nombre de dominio del cliente. Este campo puede aparecer en blanco hasta el segundo ciclo de facturación. *No utilice este campo como identificador único para el cliente. El cliente o asociado puede actualizar el personal o el dominio predeterminado a través del portal de Office 365.* |
| País del cliente | El país donde se encuentra el cliente. |
| Número de factura | Número de factura donde aparece la transacción especificada. |
| MpnId | Identificador de MPN del asociado de CSP. |
| Reseller MpnId | Identificador de MPN del distribuidor de registro de la suscripción. |
| Id. de pedido | Identificador único para un pedido en la plataforma de comercio de Microsoft. No se usa para la conciliación. |
| Fecha del pedido | Fecha de realización del pedido. |
| ProductId | Identificador del producto. |
| SkuId | Identificador de una SKU determinada (unidad de mantenimiento de existencias). |
| AvailabilityId | Identificador de la disponibilidad de una SKU determinada. Esto muestra si la SKU está disponible para su compra en el país determinado, la moneda, el segmento del sector, etc. |
| Nombre de SKU | Título para un SKU concreto. |
| Nombre del producto | Nombre del producto. |
| PublisherName | Nombre del publicador del producto.
| PublisherID | Identificador único para un publicador determinado. |
| Descripción de la suscripción | Nombre descriptivo de una suscripción. |
| Id. de la suscripción | Identificador único de una suscripción en la plataforma de comercio de Microsoft. No se usa para la conciliación. *Este identificador no es el mismo que el **identificador de suscripción** en la consola de administración de socios comerciales.* |
| ChargeStartDate | Día de inicio de los cargos. La hora siempre corresponde al comienzo del día, 0:00. |
| ChargeEndDate | Día de finalización de los cargos. La hora siempre corresponde al fin del día, 23:59. |
| Term y Billingcycle | La duración del período y el ciclo de facturación de la compra (por ejemplo, *1 año, mensualmente*). |
| Tipo de cargo | Tipo de cargo o ajuste. |
| Precio unitario | El precio unitario publicado en la lista de precios en el momento de la compra. *Asegúrese de que coincide con la información almacenada en el sistema de facturación durante la conciliación.* |
| Precio unitario efectivo | Precio unitario tras realizar los ajustes. |
| Cantidad | Número de unidades. *Asegúrese de que coincide con la información almacenada en el sistema de facturación durante la conciliación.* |
| Tipo de unidad | Tipo de unidad que se va a adquirir. |
| DiscountDetails | Explicación de cualquier descuento aplicable. |
| Subtotal | Total sin impuestos. Comprueba si el subtotal coincide con el total esperado, en caso de que se trate de un descuento. |
| Total de impuestos | Cargo del importe de los impuestos. En función de las reglas de impuestos y las circunstancias específicas de su mercado. |
| Total | Total con impuestos. Comprueba si se cobran impuestos en la factura. |
| Currency | Tipo de moneda. Cada entidad de facturación tiene una sola moneda. Asegúrese de que coincide con la primera factura y vuelva a comprobarlo después de cualquier actualización de la plataforma de facturación principal. |
| AlternateID | Un identificador alternativo a un **identificador de pedido**. |
