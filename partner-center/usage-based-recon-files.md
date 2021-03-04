---
title: Archivos de conciliación basada en uso
ms.topic: article
ms.date: 06/08/2020
description: Obtenga información sobre todos los elementos del archivo de conciliación basado en el uso en el centro de Partners. Incluye algunos ejemplos.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d3941d09d6ec808f3d188521c4f0c51c9a6d0222
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/03/2021
ms.locfileid: "101755756"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Comprender los archivos de conciliación basados en el uso y sus campos específicos en el centro de Partners

Se aplica a:

- Centro de partners
- Centro de partners para Microsoft Cloud for US Government

**Roles adecuados**

- Administrador de cuentas
- Administrador de facturación

Para conciliar los cargos con el uso de un cliente, compare los **ResellerID**, **ResellerName** y **ResellerBillableAccount** del archivo de conciliación con el **nombre del cliente** y el identificador de la **suscripción** del centro de Partners.

## <a name="fields-in-usage-based-reconciliation-files"></a>Campos en archivos de conciliación basados en el uso

Los siguientes campos explican los servicios usados y la clasificación.

| Columna | Descripción | Valores de ejemplo |
| ------ | ----------- | ------------ |
| PartnerId | Identificador del asociado, en formato GUID. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Nombre del asociado. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Identificador de cuenta de asociado. | *1010578050* |
| CustomerCompanyName | Nombre de la organización del cliente, según figura en el Centro de partners. *Muy importante para conciliar la factura con la información del sistema.* | *Cliente de prueba* |
| MpnId | Identificador de MPN del asociado de CSP. | *4390934* |
| ResellerMpnId | Identificador de MPN del distribuidor de registro de la suscripción.  |
| InvoiceNumber | Número de factura donde aparece la transacción especificada. | *D020001IVK* |
| ChargeStartDate | Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latente que no se hayan cobrado anteriormente (de ciclos de facturación anteriores). La hora es siempre el principio del día, 00:00. | *2/1/2019 0:00* |
| ChargeEndDate | Fecha final del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latente que no se hayan cobrado anteriormente (de ciclos de facturación anteriores). La hora siempre corresponde al fin del día, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Identificador único para una suscripción en la plataforma de facturación de Microsoft. Puede ser útil para identificar la suscripción al ponerse en contacto con el servicio de soporte técnico. No se usa para la conciliación. *No es lo mismo que el **identificador de suscripción** en la consola de administración de socios comerciales.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Alias para la oferta de servicio. | *Microsoft Azure* |
| SubscriptionDescription | Línea de negocio de la oferta de servicio. | *Microsoft Azure* |
| OrderID | Identificador único para un pedido en la plataforma de facturación de Microsoft. Puede ser útil para identificar la suscripción al ponerse en contacto con el servicio de soporte técnico. No se usa para la conciliación. | *566890604832738111* |
| ServiceName | Nombre del servicio de Azure en cuestión. | *MÁQUINAS VIRTUALES* |
| ServiceType | El tipo específico de servicio de Azure. | *Service Bus: individual o Pack*, *SQL Azure base de datos: Business o Web Edition* |
| ResourceGuid | Identificador único específico de todos los datos de servicio y de la estructura de precios. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| nombreDelRecurso | El nombre del recurso de Azure. | *Transferencia de datos en (GB)* *transferencia de datos de salida (GB)* |
| Region | La región a la que se aplica el uso. Se usa principalmente para asignar tasas a las transferencias de datos, ya que las tarifas varían según la región. | *Asia Pacífico*, *Europa*, *América Latina*, *Norteamérica* |
| SKU | Identificador único de Microsoft para una oferta. | *7UD-00001* |
| DetailLineItemId | Identificador y cantidad para clasificar diferentes tasas para un servicio o recurso en un período de facturación determinado. En el caso de los precios en capas de Azure, puede haber una tasa de hasta una cantidad determinada de unidades facturables y, a continuación, una tarifa diferente después de esa cantidad. | *1* |
| ConsumedQuantity | La cantidad de servicio consumido (como horas o GB) durante el período de notificación. También incluye cualquier uso no facturado de períodos de informes anteriores. | *11* |
| IncludedQuantity | Unidades que se incluye como parte de la oferta. Normalmente no está presente en CSP. | *0* |
| OverageQuantity | Las unidades no se incluyen como parte de la oferta. Estos deben ser pagados por el asociado. Igual a **ConsumedQuantity** menos **IncludedQuantity**. | *11* |
| ListPrice | Precio de la oferta en vigor a la fecha de inicio de la suscripción. | *$0,0808* |
| PretaxCharges | Igual a **ListPrist** multiplicado por **OverageQuantity**, redondeado al cent más cercano. | *0.085 USD* |
| TaxAmount | Importe de impuestos aplicado. En función de las reglas de impuestos y las circunstancias específicas de su mercado. | *$0,08* |
| PostTaxTotal | Total después de impuestos, cuando correspondan impuestos. | *$0,93* |
| Moneda | Tipo de moneda. Cada entidad de facturación tiene solo una moneda. Compruebe que coincide con la primera factura y, después, después de cualquier actualización de la plataforma de facturación principal. | *EUR* |
| PretaxEffectiveRate | Precio unitario antes de impuestos. Igual a **PretaxCharges** dividido por **OverageQuantity**, redondeado al cent más cercano. | *$0,08* |
| PostTaxEffectiveRate | Precio unitario después de impuestos. Igual a **PostTaxTotal** dividido por **OverageQuantity**, redondeado al cent más cercano. O bien, es igual a **PretaxEffectiveRate** más la tasa impositiva por unidad, redondeada al cent más cercano. | *$0,08* |
| ChargeType | [Tipo de cargo](recon-file-charge-types.md) o ajuste. | Consulte [tipos de cargos](recon-file-charge-types.md). |
| CustomerId | Identificador único de Microsoft para el cliente, en formato GUID. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Nombre de dominio del cliente. Este campo puede aparecer en blanco hasta el segundo ciclo de facturación. | *ejemplo.onmicrosoft.com* |
| BillingCycleType | Frecuencia de facturación de tiempo.| **Mensual**  |
| Unidad | Unidad del **nombre** del recurso. | *GB* o *horas* |
| CustomerBillableAccount | Identificador de cuenta único en la plataforma de facturación de Microsoft. | *1280018095* |
| UsageDate | Fecha de implementación del servicio. | *2/1/2019 0:00* |
| MeteredRegion | Identifica la ubicación de un centro de datos dentro de la región (para los servicios en los que este valor es aplicable y rellenado). | *Asia oriental*, *Asia suroriental*, *Europa del norte*, *Europa occidental*, *centro-norte de EE. UU.*, *centro-sur de EE. UU.* |
| MeteredService | Identifica el uso individual del servicio de Azure cuando no se identifica específicamente en la columna **ServiceName** . Por ejemplo, las transferencias de datos se muestran como *Microsoft Azure todos los servicios* de la columna **ServiceName** . | *AccessControl*, *CDN*, *Compute*, *Database*, *ServiceBus*, *Storage* |
| MeteredServiceType | Subtítulo del campo **MeteredService** que proporciona una explicación adicional sobre el uso del servicio de Azure. | *EXTERNAL* |
| Project | Nombre definido por el cliente para su instancia de servicio. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | El número de conexiones Azure Service Bus aprovisionadas y utilizadas en un día determinado. | *1,000000 conexiones/30 días* (si tiene una conexión aprovisionada individualmente durante un mes de 30 días), *25 conexiones/30 días – se usa: 1,000000* (si tiene un 25 paquete de conexiones Service Bus aprovisionadas y usó 1 durante ese día) |

## <a name="next-steps"></a>Pasos siguientes

- [Descripción de los campos de los archivos de conciliación basados en licencias del centro de Partners](license-based-recon-files.md)