---
title: Archivos de conciliación basada en licencia
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo leer archivos de conciliación basados en licencias en Centro de partners. En este artículo se explica el significado de cada campo en el archivo de conciliación basado en licencias.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 041f0fadfea107027ae1d9796d235700e66e6834
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146585"
---
# <a name="understand-the-fields-in-partner-center-license-based-reconciliation-files"></a>Comprender los campos de los Centro de partners de conciliación basados en licencias

**Se aplica a**: Centro de partners | Centro de partners para Microsoft Cloud for US Government

**Roles adecuados:** Administrador global | Administrador de administración de | Administración de facturación | Agente de administración

Para conciliar los cambios con los  pedidos de un cliente, compare el Syndication_Partner_Subscription_Number del archivo de conciliación con el identificador de suscripción **de** Centro de partners.

## <a name="fields-in-license-based-reconciliation-files"></a>Campos de los archivos de conciliación basados en licencias

| Columna | Descripción | Valor de ejemplo |
| ------ | ----------- | ------------ |
| PartnerId | Identificador único en formato GUID para una entidad de facturación específica. No es necesario para la conciliación. Igual en todas las filas. | *8ddd03642-test-test-test-46b58d356b4e* |
| CustomerId | Identificador único de Microsoft para el cliente en formato GUID. | *12ABCD34-001A-BCD2-987C-3210ABCD5678* |
| CustomerName | Nombre de la organización del cliente, según figura en el Centro de partners. *Campo muy importante para conciliar la factura con la información del sistema.* | *Cliente de prueba A* |
| MpnId | Identificador de MPN del asociado de CSP. Vea [cómo agregar elementos por asociado.](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *4390934* |
| ResellerMpnId | Identificador de MPN del revendedor del registro de la suscripción.  |
| OrderId | Identificador único para un pedido en la plataforma de facturación de Microsoft. Puede ser útil para identificar el pedido al ponerse en contacto con el soporte técnico. No se usa para la conciliación. | *566890604832738111* |
| SubscriptionId | Identificador único para una suscripción en la plataforma de facturación de Microsoft. Puede ser útil para identificar la suscripción al ponerse en contacto con el soporte técnico. No se usa para la conciliación. *Este valor no es el mismo que el identificador **de suscripción en** la consola de administración de partners. Consulte **SyndicationPartnerSubscriptionNumber en su** lugar.* | *usCBMgAAAAAAAAIA* |
| SyndicationPartnerSubscriptionNumber | Identificador único de las suscripciones. Un cliente puede tener varias suscripciones para el mismo plan. Esta columna es importante para el análisis de archivos de conciliación. Este campo se asigna al identificador **de suscripción en** la consola de administración de partners. | *fb977ab5-test-test-test-24c8d9591708* |
| OfferId | Identificador único de la oferta. Identificador de oferta estándar, tal como se define en la lista de precios. *Este valor no coincide con **el identificador de la oferta** de la lista de precios. Vea **DurableOfferID en su** lugar.* | *FE616D64-E9A8-40EF-843F-152E9 ESTAF3D1* |
| DurableOfferId | Identificador único de la oferta duradera, tal como se define en la lista de precios. *Este valor coincide con el **identificador de la oferta** de la lista de precios.* | *1017D7F3-6D7F-4BFA-BDD8-79BC8F104E0C* |
| OfferName | Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios. | *Microsoft Office 365 (Plan E3)* |
| SubscriptionStartDate | Fecha de inicio de la suscripción en UTC. La hora es siempre el principio del día, 00:00. Este campo se establece en el día después de enviar el pedido. Se usa con **SubscriptionEndDate** para determinar si el cliente todavía está dentro del primer año de la suscripción o si la suscripción se ha renovado para el año siguiente. | *2/1/2019 0:00* |
| SubscriptionEndDate | Fecha de finalización de la suscripción en UTC. La hora es siempre el principio del día, 00:00. *12 meses más x **días*** después de la fecha de inicio para alinearse con la fecha de facturación del asociado o *12* meses a partir de la fecha de renovación . En el momento de la renovación, los precios se actualizan según la lista de precios actual. Es posible que se necesite una comunicación con el cliente antes de la renovación automatizada. | *2/1/2019 0:00* |
| ChargeStartDate | Día de inicio de los cargos. La hora es siempre el principio del día, 00:00. Se usa para calcular los cargos diarios *(cargos pro rata)* cuando un cliente cambia los números de licencia. | *2/1/2019 0:00* |
| ChargeEndDate | Día de finalización de los cargos. La hora siempre corresponde al fin del día, 23:59. Se usa para calcular los cargos diarios *(cargos pro rata)* cuando un cliente cambia los números de licencia. | *2/28/2019 23:59* |
| ChargeType | Tipo [de cargo o](recon-file-charge-types.md) ajuste. | Consulte los [tipos de cargos](recon-file-charge-types.md). |
| UnitPrice | Precio por licencia, tal como se publicó en la lista de precios en el momento de la compra. Asegúrese de que coincide con la información almacenada en el sistema de facturación durante la conciliación. | *6.82* |
| Cantidad | Número de licencias. Asegúrese de que coincide con la información almacenada en el sistema de facturación durante la conciliación. | *2* |
| Amount | Total del precio para la cantidad. Se usa para comprobar si el cálculo de la cantidad coincide con la forma en que calcula este valor para los clientes. | *13.32* |
| TotalOtherDiscount | Cantidad de descuento que se aplica a estos cargos. Las licencias de productos incluidas con una competencia o MAPS, o nuevas suscripciones aptas para un incentivo, también contendrán un importe de descuento en esta columna. | *2.32* |
| Subtotal | Total sin impuestos. Comprueba si el subtotal coincide con el total esperado, en caso de un descuento. | *11* |
| Impuesto | Cargo por importe de impuestos. En función de las reglas fiscales del mercado y las circunstancias específicas. | *0* |
| TotalForCustomer | Total con impuestos. Comprueba si se cobran impuestos en la factura. | *11* |
| Moneda | Tipo de moneda. Cada entidad de facturación tiene solo una moneda. Compruebe si coincide con la primera factura. Vuelva a comprobarlo después de las actualizaciones principales de la plataforma de facturación. | *EUR* |
| DomainName | Nombre de dominio del cliente. Este campo puede aparecer en blanco hasta el segundo ciclo de facturación. *No use este campo como identificador único para el cliente. El cliente o asociado puede actualizar el dominio predeterminado o vanidad a través del portal de Office 365.* | *ejemplo.onmicrosoft.com* |
| SubscriptionName | Alias de suscripción. Si no se especifica ningún alias, Centro de partners la **propiedad OfferName**. | *PROJECT ONLINE* |
| SubscriptionDescription | Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios. (Se trata de un campo idéntico a **OfferName).** | *PROJECT ONLINE PREMIUM SIN CLIENTE DE PROJECT* |
| BillingCycleType | Frecuencia de facturación única.| *Mensual* |
