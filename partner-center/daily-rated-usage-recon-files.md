---
title: Archivos de conciliación de uso clasificados diariamente
ms.topic: article
ms.date: 06/12/2020
description: Obtenga información sobre cómo leer archivos de conciliación de uso clasificados diariamente en Centro de partners. Incluye descripciones de campos específicos en el archivo de conciliación.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9b5daf91646324a9d4ace92d25736cfd0361ad6c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147282"
---
# <a name="learn-how-to-read-daily-rated-usage-reconciliation-files-in-partner-center"></a>Obtenga información sobre cómo leer archivos de conciliación de uso clasificados diariamente en Centro de partners

**Se aplica a**: Centro de partners | Centro de partners para Microsoft Cloud for US Government

**Roles adecuados:** agente de administración | Administración de facturación | Agente de ventas | Agente del departamento de soporte técnico

En este artículo se explica cómo leer los archivos de conciliación de uso clasificados diariamente.

>[!NOTE]
>Normalmente, el uso con clasificación diaria tarda 24 horas en aparecer en Centro de partners acceso a través de la API.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Campos en archivos de conciliación de uso clasificados diariamente

| Columna | Descripción |
| ------ | ----------- |
| PartnerId | Identificador del asociado en formato GUID. |
| PartnerName | Nombre del asociado. |
| CustomerId | Identificador único de Microsoft para el cliente en formato GUID. |
| CustomerName | Nombre de la organización del cliente según figura en el Centro de partners. *Esta columna es importante para conciliar la factura con la información del sistema.* |
| CustomerDomainName | Nombre de dominio del cliente. |
| CustomerCountry | El país en el que se encuentra el cliente. |
| MpnId | Identificador de MPN del asociado de CSP. |
| Tier2MpnId | Identificador de MPN del revendedor del registro de la suscripción. |
| InvoiceNumber | Número de factura donde aparece la transacción especificada. |
| ProductId | Identificador del producto. |
| SkuId | Identificador de una SKU determinada. |
| AvailabilityId | Identificador de la disponibilidad de una SKU determinada. En esta columna se muestra si la SKU está disponible para su compra en el país, la moneda, el segmento del sector, etc. |
| SkuName | Título de una SKU determinada. |
| ProductName | Nombre del producto. |
| PublisherName | Nombre del publicador. |
| PublisherId | Identificador del publicador en formato GUID. |
| SubscriptionDescription | Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios. (Esta columna es un campo idéntico a **OfferName**). |
| SubscriptionId | Identificador único para una suscripción en la plataforma de facturación de Microsoft. No se usa para la conciliación. *Este identificador no es el mismo que el identificador de **suscripción** en la consola de administración del asociado.* |
| ChargeStartDate | Fecha de inicio del ciclo de facturación (excepto cuando se presentan fechas de datos de uso latente no cobrados previamente del ciclo de facturación anterior). La hora es siempre el principio del día, 00:00. |
| ChargeEndDate | Fecha de finalización del ciclo de facturación (excepto cuando se presentan fechas de datos de uso latente no cobrados previamente del ciclo de facturación anterior). La hora siempre corresponde al fin del día, 23:59. |
| UsageDate | Fecha de uso del servicio. |
| MeterType | Tipo de medidor. |
| MeterCategory | Identifica el servicio de nivel superior para el uso. |
| MeterId | Identificador del medidor que se está utilizando. |
| MeterSubCategory | El tipo de servicio de Azure, que puede afectar a la velocidad. |
| MeterName | Unidad de medida para el medidor que se va a consumir. |
| MeterRegion | Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde MeterRegion es aplicable y rellenado. |
| Unidad | Unidad del nombre del **recurso**. |
| ResourceLocation | Centro de datos donde se ejecuta el medidor. |
| ConsumedService | El servicio de la plataforma Azure que ha usado. |
| ResourceGroup | Representa un contenedor que contiene recursos relacionados para una solución de Azure. |
| ResourceURI | Uri del recurso que se está utilizando. |
| ChargeType | Tipo de cargo o ajuste.  |
| UnitPrice | Precio por licencia, tal como se publica en la lista de precios en el momento de la compra. Asegúrese de que este precio coincide con la información almacenada en el sistema de facturación durante la conciliación. |
| Cantidad | Número de licencias. Asegúrese de que este precio coincide con la información almacenada en el sistema de facturación durante la conciliación. |
| UnitType | Tipo de unidad en la que se cobra el medidor.  |
| BillingPreTaxTotal | Importe total de facturación antes de impuestos.<br/> _**BillingPreTaxTotal** = FLOOR(([ @EffectiveUnitPrice ]*[ @Quantity ]*[ @PCToBCExchangeRate ]), 2)_ |
| BillingCurrency | Moneda en la región geográfica del cliente. |
| PricingPreTaxTotal | Los precios, antes de que se agregan los impuestos. |
| PricingCurrency | Moneda de la lista de precios. |
| ServiceInfo1 | Número de conexiones Service Bus que se aprovisionaron y usaron en un día determinado. |
| ServiceInfo2 | Campo heredado que captura metadatos opcionales específicos del servicio. |
| Etiquetas | Representa una organización lógica de recursos de Azure establecida por el usuario. |
| AdditionalInfo | Cualquier información adicional no incluida en otras columnas. |
| EffectiveUnitPrice | El valor real que se cobra por unidad, incluidos los descuentos, el crédito obtenido, y así sucesivamente. |
| PCToBCExchangeRate | Tipo de cambio aplicado para la moneda de precios a la moneda de facturación. |
| PCToBCExchangeRateDate | Fecha en la que se determina la moneda de precios a la moneda de facturación. |
| EntitlementId | Representa el identificador de suscripción de Azure. |
| EntitlementDescription | Representa el nombre del identificador de suscripción de Azure. |
| PartnerEarnedCreditPercentage | Muestra partnerEarnedCredit para el elemento de línea. El crédito obtenido será del 0 al 15 por ciento |
| CreditPercentage | Muestra el crédito de consumo de Azure. El crédito obtenido será 0 o 100 por ciento. |
| CreditType | Tipo del crédito. Por ejemplo, **Crédito de Azure aplicado.** |
>[!NOTE]
>El uso con clasificación diaria normalmente tarda 24 horas en aparecer en Centro de partners o para que se pueda acceder a través de la API.


