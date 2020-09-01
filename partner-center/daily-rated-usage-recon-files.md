---
title: Archivos de conciliación de uso clasificados diariamente
ms.topic: article
ms.date: 06/12/2020
description: Obtenga información sobre cómo leer archivos de conciliación de uso clasificados diariamente en el centro de Partners.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bff2c66e7efd05631de7d7643a780cbe5f726103
ms.sourcegitcommit: 3670c6e7f22e4f56545886052b68b9d5b6b3092c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/01/2020
ms.locfileid: "89281317"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Obtenga información sobre cómo leer archivos de conciliación de uso clasificados diariamente en el centro de Partners

**Se aplica a**

- Centro de partners
- Centro de partners para Microsoft Cloud for US Government

**Roles adecuados**

- Agente de administrador
- Administrador de facturación
- Agente de ventas
- Agente del departamento de soporte técnico

En este artículo se explica cómo leer archivos de conciliación de uso clasificados diariamente.

>[!NOTE]
>Normalmente, el uso con clasificación diaria tarda 24 horas en aparecer en el centro de Partners o en el acceso a través de la API.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Campos en archivos de conciliación de uso clasificados diariamente

| Columna | Descripción |
| ------ | ----------- |
| PartnerId | Identificador del asociado en formato GUID. |
| PartnerName | Nombre del asociado. |
| CustomerId | Identificador único de Microsoft para el cliente en formato GUID. |
| CustomerName | Nombre de la organización del cliente según figura en el Centro de partners. *Esta columna es importante para conciliar la factura con la información del sistema.* |
| CustomerDomainName | El nombre de dominio del cliente. |
| CustomerCountry | País en el que se encuentra el cliente. |
| MpnId | Identificador de MPN del asociado de CSP. |
| Tier2MpnId | Identificador de MPN del distribuidor de registro de la suscripción. |
| InvoiceNumber | Número de factura donde aparece la transacción especificada. |
| ProductId | Identificador del producto. |
| SkuId | Identificador de una SKU determinada. |
| AvailabilityId | Identificador de la disponibilidad de una SKU determinada. Esta columna muestra si la SKU está disponible para su compra en el país determinado, la moneda, el segmento de la industria, etc. |
| SkuName | Título de una SKU determinada. |
| ProductName | Nombre del producto. |
| PublisherName | Nombre del publicador. |
| PublisherId | Identificador del publicador en formato GUID. |
| SubscriptionDescription | Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios. (Esta columna es un campo idéntico a **nombredeoferta**). |
| SubscriptionId | Identificador único para una suscripción en la plataforma de facturación de Microsoft. No se usa para la conciliación. *Este identificador no es el mismo que el **identificador de suscripción** en la consola de administración de socios comerciales.* |
| ChargeStartDate | Fecha de inicio del ciclo de facturación (excepto cuando se presentan fechas de datos de uso latente previamente no cargados del ciclo de facturación anterior). La hora es siempre el principio del día, 00:00. |
| ChargeEndDate | Fecha final del ciclo de facturación (excepto cuando se presentan fechas de datos de uso latente previamente no cargados del ciclo de facturación anterior). La hora siempre corresponde al fin del día, 23:59. |
| UsageDate | Fecha del uso del servicio. |
| MeterType | Tipo de medidor. |
| MeterCategory | Identifica el servicio de nivel superior para el uso. |
| Id. del medidor | Identificador del medidor que se está usando. |
| MeterSubCategory | El tipo de servicio de Azure, que puede afectar a la tarifa. |
| MeterName | Unidad de medida del medidor que se está consumiendo. |
| MeterRegion | Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios en los que MeterRegion es aplicable y rellenado. |
| Unidad | Unidad del **nombre**del recurso. |
| ResourceLocation | Centro de datos en el que se está ejecutando el medidor. |
| ConsumedService | El servicio de la plataforma Azure que ha usado. |
| ResourceGroup | Representa un contenedor que contiene los recursos relacionados de una solución de Azure. |
| ResourceURI | URI del recurso que se va a usar. |
| ChargeType | Tipo de cargo o ajuste.  |
| UnitPrice | Precio por licencia, tal como se publicó en la lista de precios en el momento de la compra. Asegúrese de que este precio coincida con la información almacenada en el sistema de facturación durante la conciliación. |
| Cantidad | Número de licencias. Asegúrese de que este precio coincida con la información almacenada en el sistema de facturación durante la conciliación. |
| UnitType | Tipo de unidad en la que se carga el medidor.  |
| BillingPreTaxTotal | Importe total de facturación antes de los impuestos.<br/> _**BillingPreTaxTotal** = Floor (([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | La moneda en la región geográfica del cliente. |
| PricingPreTaxTotal | Los precios, antes de que se agreguen los impuestos. |
| PricingCurrency | Moneda de la lista de precios. |
| ServiceInfo1 | El número de conexiones Service Bus aprovisionadas y utilizadas en un día determinado. |
| ServiceInfo2 | Campo heredado que captura los metadatos específicos del servicio opcionales. |
| Etiquetas | Representa una organización lógica de recursos de Azure establecida por el usuario. |
| AdditionalInfo | Cualquier información adicional no incluida en otras columnas. |
| EffectiveUnitPrice | El valor real que se cobra por unidad, incluidos los descuentos, el crédito obtenido, etc. |
| PCToBCExchangeRate | Tasa de cambio que se aplica para la moneda de facturación. |
| PCToBCExchangeRateDate | Fecha en la que se determina la moneda de los precios de la moneda de facturación. |
| EntitlementId | Representa el identificador de suscripción de Azure. |
| EntitlementDescription | Representa el nombre del identificador de suscripción de Azure. |
| PartnerEarnedCreditPercentage | Muestra el PartnerEarnedCredit del elemento de línea. El crédito obtenido será 0 o 15 por ciento |

>[!NOTE]
>Normalmente, el uso con clasificación diaria tarda 24 horas en aparecer en el centro de Partners o en el acceso a través de la API.


