---
title: Archivos de conciliación de uso con clasificación diaria | Centro de Partners
ms.topic: article
ms.date: 01/14/2020
description: Obtenga información sobre cómo leer archivos de conciliación de uso clasificados diariamente en el centro de Partners.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: a9c7f328cf1a10b4a23aeb775524d5931bdbb703
ms.sourcegitcommit: fc43ee25d405ef3dc673edd884c877bfc62ad6aa
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/15/2020
ms.locfileid: "76021727"
---
# <a name="daily-rated-usage-reconciliation-files"></a>Archivos de conciliación de uso clasificados diariamente

**Se aplica a**

- Centro de partners
- Centro de partners para Microsoft Cloud for US Government

**Roles adecuados**

- Agente de administración
- Administrador de facturación
- Agente de ventas
- Agente del departamento de soporte técnico

En este tema se explica cómo leer archivos de conciliación de uso clasificados diariamente.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Campos en archivos de conciliación de uso clasificados diariamente

| Column | Descripción |
| ------ | ----------- |
| PartnerId | Identificador del asociado en formato GUID. |
| PartnerName | Nombre del asociado. |
| CustomerId | Identificador único de Microsoft para el cliente en formato GUID. |
| CustomerName | Nombre de la organización del cliente según se indica en el Centro de partners. *Esta columna es muy importante para conciliar la factura con la información del sistema.* |
| CustomerDomainName | El nombre de dominio del cliente. |
| CustomerCountry | El país donde se encuentra el cliente. |
| MpnId | Identificador de MPN del asociado de CSP. |
| Tier2MpnId | Identificador de MPN del distribuidor de registro de la suscripción. |
| InvoiceNumber | Número de factura donde aparece la transacción especificada. |
| ProductId | Identificador del producto. |
| SkuId | Identificador de una SKU determinada. |
| AvailabilityId | Identificador de la disponibilidad de una SKU determinada. Esto muestra si la SKU está disponible para su compra en el país determinado, la moneda, el segmento del sector, etc. |
| SkuName | Título para un SKU concreto. |
| ProductName | Nombre del producto. |
| PublisherName | Nombre del publicador. |
| PublisherId | Identificador del publicador en formato GUID. |
| SubscriptionDescription | Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios. (Este campo es idéntico a **nombredeoferta**). |
| SubscriptionId | Identificador único de una suscripción en la plataforma de facturación de Microsoft. No se usa para la conciliación. *Este identificador no es el mismo que el **identificador de suscripción** en la consola de administración de socios comerciales.* |
| ChargeStartDate | Fecha de inicio del ciclo de facturación (excepto cuando se presentan fechas de datos de uso latente previamente no cargados del ciclo de facturación anterior). La hora siempre corresponde al comienzo del día, 0:00. |
| ChargeEndDate | Fecha final del ciclo de facturación (excepto cuando se presentan fechas de datos de uso latente previamente no cargados del ciclo de biling anterior). La hora siempre corresponde al fin del día, 23:59. |
| UsageDate | Fecha del uso del servicio. |
| MeterType | Tipo de medidor. |
| MeterCategory | Identifica el servicio de nivel superior para el uso. |
| MeterId | Identificador del medidor que se está usando. |
| MeterSubCategory | El tipo de servicio de Azure, que puede afectar a la tarifa. |
| MeterName | Unidad de medida del medidor que se está consumiendo. |
| MeterRegion | Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena. |
| Unidad | Unidad del **nombre**del recurso. |
| ResourceLocation | Centro de datos en el que se está ejecutando el medidor. |
| ConsumedService | El servicio de la plataforma Azure que ha usado. |
| ResourceGroup | Representa un contenedor que contiene los recursos relacionados de una solución de Azure. |
| ResourceURI | URI del recurso que se va a usar. |
| ChargeType | Tipo de cargo o ajuste.  |
| UnitPrice | Precio por licencia, tal como se publicó en la lista de precios en el momento de la compra. Asegúrese de que este precio coincida con la información almacenada en el sistema de facturación durante la conciliación. |
| Cantidad | Número de licencias. Asegúrese de que este precio coincida con la información almacenada en el sistema de facturación durante la conciliación. |
| UnitType | Tipo de unidad en la que se carga el medidor.  |
| BillingPreTaxTotal | Importe total de facturación antes de los impuestos. |
| BillingCurrency | La moneda en la región geográfica del cliente. |
| PricingPreTaxTotal | Los precios antes de que se agreguen los impuestos. |
| PricingCurrency | La moneda en la lista de precios. |
| ServiceInfo1 | El número de conexiones Service Bus aprovisionadas y utilizadas en un día determinado. |
| ServiceInfo2 | Campo heredado que captura los metadatos específicos del servicio opcionales. |
| Etiquetas | Representa una organización lógica de recursos de Azure establecida por el usuario. |
| AdditionalInfo | Cualquier información adicional no incluida en otras columnas. |
| EffectiveUnitPrice | El valor real que se cobra por unidad, incluidos los descuentos, el crédito acumulado, etc. |
| PCToBCExchangeRate | Tasa de cambio que se aplica para la moneda de facturación. |
| PCToBCExchangeRateDate | Fecha en la que se determina la moneda de los precios de la moneda de facturación. |
| EntitlementId | Representa el identificador de suscripción de Azure. |
| EntitlementDescription | Representa el nombre del identificador de suscripción de Azure. |
| PartnerEarnedCreditPercentage | Muestra el PartnerEarnedCredit del elemento de línea. El crédito obtenido será 0 o 15 por ciento |
