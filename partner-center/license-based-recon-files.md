---
title: Archivos de conciliación basados en licencias | Centro de Partners
ms.topic: article
ms.date: 11/21/2019
description: Comprender los archivos de conciliación basados en licencias en el centro de Partners.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 60ab5404f3cc2d825a110e61bd7c6bf5744bb786
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004604"
---
# <a name="license-based-reconciliation-files"></a>Archivos de conciliación basada en licencia

**Se aplica a**

- Centro de partners
- Centro de partners para Microsoft Cloud for US Government

**Roles adecuados**
-   Administrador global
-   Administrador de usuarios
-   Administrador de facturación
-   Agente de administración

Para conciliar los cambios con los pedidos de un cliente, compare el **Syndication_Partner_Subscription_Number** del archivo de conciliación con el **identificador de suscripción** del centro de Partners.

## <a name="fields-in-license-based-reconciliation-files"></a>Campos en archivos de conciliación basados en licencias

| Column | Descripción | Valor de muestra |
| ------ | ----------- | ------------ |
| PartnerId | Identificador único en formato GUID para una entidad de facturación específica. No es necesario para la reconciliación. Igual en todas las filas. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerID | Identificador único de Microsoft para el cliente en formato GUID. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| OrderID | Identificador único de un pedido en la plataforma de facturación de Microsoft. Puede ser útil para identificar el orden al ponerse en contacto con el servicio de soporte técnico. No se usa para la conciliación. | *566890604832738111* |
| SubscriptionID | Identificador único de una suscripción en la plataforma de facturación de Microsoft. Puede ser útil para identificar la suscripción al ponerse en contacto con el servicio de soporte técnico. No se usa para la conciliación. *Este valor no es el mismo que el **identificador de suscripción** en la consola de administración de socios comerciales. Consulte **SyndicationPartnerSubscriptionNumber** en su lugar.* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Identificador único de las suscripciones. Un cliente puede tener varias suscripciones para el mismo plan. Esta columna es importante para el análisis de archivos de conciliación. Este campo se asigna al **identificador de suscripción** en la consola de administración de socios comerciales. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferID | Identificador único de la oferta. Identificador de la oferta estándar, tal como se define en la lista de precios. *Este valor no coincide con el identificador de la **oferta** de la lista de precios. Vea **DurableOfferID** en su lugar.* | *FE616D64-E9A8-40EF-843F-152E9BBEF3D1* |
| DurableOfferID | Identificador único de la oferta durable, tal como se define en la lista de precios. *Este valor coincide con el identificador de la **oferta** de la lista de precios.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios. | *Microsoft Office 365 (plan E3)* |
| SubscriptionStartDate | Fecha de inicio de la suscripción. La hora siempre corresponde al comienzo del día, 0:00. Este campo se establece en el día después de enviar el pedido. Se usa junto con **SubscriptionEndDate** para determinar: Si el cliente sigue en el primer año de la suscripción, o si la suscripción se ha renovado durante el año siguiente. | *2/1/2019 0:00* |
| SubscriptionEndDate | Fecha de finalización de la suscripción. La hora siempre corresponde al comienzo del día, 0:00. *12 meses más **x** días después de la fecha de inicio* para alinearse con la fecha de facturación del socio o *12 meses a partir de la fecha de renovación*. En el momento de la renovación, los precios se actualizan según la lista de precios actual. Es posible que se necesite una comunicación con el cliente antes de la renovación automatizada. | *2/1/2019 0:00* |
| ChargeStartDate | Día de inicio de los cargos. La hora siempre corresponde al comienzo del día, 0:00. Se usa para calcular los cargos diarios (cargos*prorrateados* ) cuando un cliente cambia los números de asiento. | *2/1/2019 0:00* |
| ChargeEndDate | Día de finalización de los cargos. La hora siempre corresponde al fin del día, 23:59. Se usa para calcular los cargos diarios (cargos*prorrateados* ) cuando un cliente cambia los números de asiento. | *2/28/2019 23:59* |
| ChargeType | [Tipo de cargo](recon-file-charge-types.md) o ajuste. | Consulte [tipos de cargos](recon-file-charge-types.md). |
| UnitPrice | Precio por puesto, tal y como se publica en la lista de precios en el momento de compra. Asegúrese de que coincide con la información almacenada en el sistema de facturación durante la conciliación. | *6,82* |
| Cantidad | Número de puestos. Asegúrese de que coincide con la información almacenada en el sistema de facturación durante la conciliación. | *2* |
| Volumen | Total del precio para la cantidad. Se usa para comprobar si el cálculo de cantidad coincide con la forma de calcular este valor para los clientes. | *13,32* |
| TotalOtherDiscount | Cantidad de descuento que se aplica a estos cargos. Las licencias de producto incluidas en una competencia o en MAPS, o en nuevas suscripciones para un incentivo, también contendrán un importe de descuento en esta columna. | *2,32* |
| Subtotal | Total sin impuestos. Comprueba si el subtotal coincide con el total esperado, en caso de que se trate de un descuento. | *11* |
| Impuestos | Cargo del importe de los impuestos. En función de las reglas de impuestos y las circunstancias específicas de su mercado. | *0* |
| TotalForCustomer | Total con impuestos. Comprueba si se cobran impuestos en la factura. | *11* |
| Moneda | Tipo de moneda. Cada entidad de facturación tiene una sola moneda. Compruebe si coincide con la primera factura. Vuelva a comprobarlo después de las actualizaciones principales de la plataforma de facturación. | *EUR* |
| CustomerName | Nombre de la organización del cliente, según figura en el Centro de partners. *Campo muy importante para conciliar la factura con la información del sistema.* | *Cliente de prueba A* |
| MPNID | Identificador de MPN del asociado de CSP. Vea [Cómo elemento por asociado](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| ResellerMPNID | Identificador de MPN del distribuidor de registro de la suscripción. Vea [Cómo elemento por asociado](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| DomainName | Nombre de dominio del cliente. Este campo puede aparecer en blanco hasta el segundo ciclo de facturación. *No utilice este campo como identificador único para el cliente. El cliente o asociado puede actualizar el personal o el dominio predeterminado a través del portal de Office 365.* | *example.onmicrosoft.com* |
| SubscriptionName | Alias de la suscripción. Si no se especifica ningún alias, el centro de Partners usa **nombredeoferta**. | *PROYECTO EN LÍNEA* |
| SubscriptionDescription | Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios. (Este campo es idéntico a **nombredeoferta**). | *PROJECT ONLINE PREMIUM SIN CLIENTE DE PROYECTO* |
