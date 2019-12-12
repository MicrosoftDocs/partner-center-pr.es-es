---
title: Archivos de conciliación única y periódica | Centro de Partners
ms.topic: article
ms.date: 11/21/2019
description: Comprenda los archivos de conciliación única y periódica en el centro de Partners.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 51c37c9ea2110b7666c4d1a9bc92a2b01f92209c
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004904"
---
# <a name="one-time-and-recurring-reconciliation-files"></a>Archivos de conciliación única y periódica

**適用於**

- 合作夥伴中心
- Centro de partners para Microsoft Cloud for US Government

**Roles adecuados**
-   全域系統管理員
-   Administrador de usuarios
-   Administrador de facturación
-   Agente de administración
-   Agente de ventas

En este tema se explica cómo leer archivos de conciliación única y periódica en el centro de Partners.

## <a name="fields-in-one-time-and-recurring-reconciliation-files"></a>Campos de archivos de conciliación única y periódica

| Column | Descripción |
| ------ | ----------- |
| PartnerId | Identificador de inquilino de Azure Active Directory único (Azure AD) para una entidad de facturación específica, en formato GUID. No es necesario para la reconciliación. Igual en todas las filas. |
| 客戶識別碼 | Identificador único del inquilino de Azure AD, en formato GUID. 識別客戶。 |
| [客戶名稱] | Nombre de la organización del cliente, según figura en el Centro de partners. |
| CustomerDomainName | Nombre de dominio del cliente. Este campo puede aparecer en blanco hasta el segundo ciclo de facturación. *No utilice este campo como identificador único para el cliente. El cliente o asociado puede actualizar el personal o el dominio predeterminado a través del portal de Office 365.* |
| 客戶國家/地區 | El país donde se encuentra el cliente. |
| 發票號碼 | 交易的指定位置顯示的發票號碼。 |
| MpnId | Identificador de MPN del asociado de CSP. |
| Reseller MpnId | Identificador de MPN del distribuidor de registro de la suscripción. |
| 訂單識別碼 | Identificador único para un pedido en la plataforma de comercio de Microsoft. No se usa para la conciliación. |
| Fecha del pedido | Fecha de realización del pedido. |
| ProductId | Identificador del producto. |
| SkuId | Identificador de una SKU determinada (unidad de mantenimiento de existencias). |
| AvailabilityId | Identificador de la disponibilidad de una SKU determinada. Esto muestra si la SKU está disponible para su compra en el país determinado, la moneda, el segmento del sector, etc. |
| SKU 名稱 | Título para un SKU concreto. |
| [產品名稱] | 產品的名稱。 |
| PublisherName | Nombre del anunciante del producto.
| PublisherID | Identificador único para un publicador determinado. |
| Descripción de la suscripción | Nombre descriptivo de una suscripción. |
| [訂閱識別碼] | Identificador único de una suscripción en la plataforma de comercio de Microsoft. No se usa para la conciliación. *Este identificador no es el mismo que el **identificador de suscripción** en la consola de administración de socios comerciales.* |
| ChargeStartDate | Día de inicio de los cargos. 時間一律是一天的開始時間 (0:00)。 |
| ChargeEndDate | Día de finalización de los cargos. La hora siempre corresponde al fin del día, 23:59. |
| Term y Billingcycle | La duración del período y el ciclo de facturación de la compra (por ejemplo, *1 año, mensualmente*). |
| Tipo de cargo | 費用或調整的類型。 |
| 單價 | El precio unitario publicado en la lista de precios en el momento de la compra. *Asegúrese de que coincide con la información almacenada en el sistema de facturación durante la conciliación.* |
| Precio unitario efectivo | Precio unitario tras realizar los ajustes. |
| 數量 | Número de unidades. *Asegúrese de que coincide con la información almacenada en el sistema de facturación durante la conciliación.* |
| Tipo de unidad | Tipo de unidad que se va a adquirir. |
| DiscountDetails | Explicación de cualquier descuento aplicable. |
| Subtotal | Total sin impuestos. Comprueba si el subtotal coincide con el total esperado, en caso de que se trate de un descuento. |
| Total de impuestos | Cargo del importe de los impuestos. En función de las reglas de impuestos y las circunstancias específicas de su mercado. |
| 總計 | Total con impuestos. Comprueba si se cobran impuestos en la factura. |
| Currency | 貨幣類型。 每一帳單實體都只有一種貨幣。 Asegúrese de que coincide con la primera factura y vuelva a comprobarlo después de cualquier actualización de la plataforma de facturación principal. |
| AlternateID | Un identificador alternativo a un **identificador de pedido**. |
