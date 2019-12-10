---
title: Archivos de conciliación basados en el uso | Centro de Partners
ms.topic: article
ms.date: 11/21/2019
description: Se explican todos los elementos del archivo de conciliación basado en el uso, con ejemplos.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: b73962b1e9d2925b0e61632a18522a1c22e4d346
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943388"
---
# <a name="usage-based-file-fields"></a>Campos de archivos basados en el uso

Se aplica a:

- Centro de partners
- Centro de partners para Microsoft Cloud for US Government

Para conciliar los cargos con el uso de un cliente, compare los **ResellerID**, **ResellerName**y **ResellerBillableAccount** del archivo de conciliación con el **nombre del cliente** y el identificador de la **suscripción** del centro de Partners.

## <a name="fields-in-usage-based-reconciliation-files"></a>Campos en archivos de conciliación basados en el uso

Los siguientes campos explican los servicios usados y la clasificación.

| Column | Descripción | Valores de ejemplo |
| ------ | ----------- | ------------ |
| PartnerID | Identificador del asociado, en formato GUID. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Nombre del asociado. | *Contoso, Ltd.* |
| PartnerBillableAccountID | Identificador de cuenta de asociado. | *1010578050* |
| CustomerName | Nombre de la organización del cliente, según figura en el Centro de partners. *Muy importante para conciliar la factura con la información del sistema.* | *Cliente de prueba* |
| MPNID | Identificador de MPN del asociado de CSP. | *4390934* |
| ResellerMPNID | Identificador de MPN del distribuidor de registro de la suscripción. Para obtener más información, consulte [Cómo elemento por asociado](use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *4390934* |
| InvoiceNumber | Número de factura donde aparece la transacción especificada. | *D020001IVK* |
| ChargeStartDate | Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latente que no se hayan cobrado anteriormente (de ciclos de facturación anteriores). La hora siempre corresponde al comienzo del día, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | Fecha final del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latente que no se hayan cobrado anteriormente (de ciclos de facturación anteriores). La hora siempre corresponde al fin del día, 23:59. | *2/28/2019 23:59* |
| SubscriptionID | Identificador único de una suscripción en la plataforma de facturación de Microsoft. Puede ser útil para identificar la suscripción al ponerse en contacto con el servicio de soporte técnico. No se usa para la conciliación. *No es lo mismo que el **identificador de suscripción** en la consola de administración de socios comerciales.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Alias para la oferta de servicio. | *Microsoft Azure* |
| SubscriptionDescription | Línea de negocio de la oferta de servicio. | *Microsoft Azure* |
| OrderID | Identificador único de un pedido en la plataforma de facturación de Microsoft. Puede ser útil para identificar la suscripción al ponerse en contacto con el servicio de soporte técnico. No se usa para la conciliación. | *566890604832738111* |
| ServiceName | Nombre del servicio de Azure en cuestión. | *MÁQUINAS VIRTUALES* |
| ServiceType | El tipo específico de servicio de Azure. | *Service Bus: individual o Pack*, *SQL Azure base de datos: Business o Web Edition* |
| ResourceGUID | Identificador único específico para toda la estructura de precios y datos del servicio. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| nombreDelRecurso | Nombre del recurso de Azure. | *Transferencia de datos en (GB)* *transferencia de datos de salida (GB)* |
| Región | La región a la que se aplica el uso. Se usa principalmente para asignar tasas a las transferencias de datos, ya que las tarifas varían según la región. | *Asia Pacífico*, *Europa*, *América Latina*, *Norteamérica* |
| SKU | Identificador único de Microsoft para una oferta. | *7UD-00001* |
| DetailLineItemId | Identificador y cantidad para clasificar diferentes tasas para un servicio o recurso en un período de facturación determinado. En el caso de los precios en capas de Azure, puede haber una tasa de hasta una cantidad determinada de unidades facturables y, a continuación, una tarifa diferente después de esa cantidad. | *1* |
| ConsumedQuantity | La cantidad de servicio consumido (como horas o GB) durante el período de notificación. También incluye cualquier uso no facturado de períodos anteriores. | *11* |
| IncludedQuantity | Unidades que se incluyen como parte de la oferta. Normalmente no está presente en CSP. | *0* |
| OverageQuantity | Las unidades no se incluyen como parte de la oferta. Estos deben ser pagados por el asociado. Igual a **ConsumedQuantity** menos **IncludedQuantity**. | *11* |
| ListPrice | Precio de la oferta en vigor a la fecha de inicio de la suscripción. | *$0,0808* |
| PretaxCharges | Igual a **ListPrist** multiplicado por **OverageQuantity**, redondeado al cent más cercano. | *$0,085* |
| TaxAmount | Importe de impuestos aplicado. En función de las reglas de impuestos y las circunstancias específicas de su mercado. | *$0,08* |
| PostTaxTotal | Total con impuestos, si se aplican impuestos. | *$0,93* |
| Moneda | Tipo de moneda. Cada entidad de facturación tiene una sola moneda. Compruebe que coincide con la primera factura y, después, después de cualquier actualización de la plataforma de facturación principal. | *EUR* |
| PretaxEffectiveRate | Precio sin impuestos por unidad. Igual a **PretaxCharges** dividido por **OverageQuantity**, redondeado al cent más cercano. | *$0,08* |
| PostTaxEffectiveRate | Precio después de impuestos por unidad. Igual a **PostTaxTotal** dividido por **OverageQuantity**, redondeado al cent más cercano. O bien, igual a **PretaxEffectiveRate** más el tasa impositiva por unidad Amoun, redondeado al cent más cercano. | *$0,08* |
| ChargeType | [Tipo de cargo](recon-file-charge-types.md) o ajuste. | Consulte [tipos de cargos](recon-file-charge-types.md). |
| CustomerBillableAccount | Identificador de cuenta único en la plataforma de facturación de Microsoft. | *1280018095* |
| UsageDate | Fecha de implementación del servicio. | *2/1/2019 0:00* |
| MeteredRegion | Identifica la ubicación de un centro de datos dentro de la región (para los servicios en los que este valor es aplicable y rellenado). | *Asia oriental*, *Asia suroriental*, *Europa del norte*, *Europa occidental*, *centro-norte de EE. UU.* , *centro-sur de EE. UU.* |
| MeteredService | Identifica el uso individual del servicio de Azure cuando no se identifica específicamente en la columna **ServiceName** . Por ejemplo, las transferencias de datos se muestran como *Microsoft Azure todos los servicios* de la columna **ServiceName** . | *AccessControl*, *CDN*, *Compute*, *Database*, *ServiceBus*, *Storage* |
| MeteredServiceType | Subtítulo del campo **MeteredService** que proporciona una explicación adicional sobre el uso del servicio de Azure. | *EXTERNAL* |
| Proyecto | Nombre definido por el cliente para su instancia de servicio. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | El número de conexiones Azure Service Bus aprovisionadas y utilizadas en un día determinado. | *1,000000 conexiones/30 días* (si tiene una conexión aprovisionada individualmente durante un mes de 30 días), *25 conexiones/30 días – se usa: 1,000000* (si tiene un 25 paquete de conexiones Service Bus aprovisionadas y usó 1 durante ese día) |
| CustomerID | Identificador único de Microsoft para el cliente, en formato GUID. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Nombre de dominio del cliente. Este campo puede aparecer en blanco hasta el segundo ciclo de facturación. | *example.onmicrosoft.com* |
| Unidad | Unidad del **nombre**del recurso. | *GB* o *horas* |
