---
title: Archivos de conciliación basada en uso
ms.topic: article
ms.date: 06/08/2020
description: Obtenga información sobre todos los elementos del archivo de conciliación basado en el uso en Centro de partners. Incluye algunos ejemplos.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fc31915660b6a82954daee5fcc8fb2d5292e725c
ms.sourcegitcommit: 837d3c5b52ab056b2b761cd85eb2426f56b62614
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/12/2021
ms.locfileid: "109795013"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Comprender los archivos de conciliación basados en el uso y sus campos específicos en Centro de partners

**Roles adecuados:** administrador de | Administrador de facturación

Para conciliar los cargos con el uso  de un cliente, compare **resellerID**, **ResellerName** y **ResellerBillableAccount** del archivo de conciliación con el nombre del cliente y el identificador de suscripción de Centro de partners. 

## <a name="fields-in-usage-based-reconciliation-files"></a>Campos de los archivos de conciliación basados en el uso

Los siguientes campos explican los servicios usados y la clasificación.

| Columna | Descripción | Valores de ejemplo |
| ------ | ----------- | ------------ |
| PartnerId | Identificador del asociado, en formato GUID. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Nombre del asociado. | *Contoso, Ltd.* |
| PartnerBillableAccountId | Identificador de la cuenta de asociado. | *1010578050* |
| CustomerCompanyName | Nombre de la organización del cliente, según figura en el Centro de partners. *Muy importante para conciliar la factura con la información del sistema.* | *Cliente de prueba* |
| MpnId | Identificador de MPN del asociado de CSP. | *4390934* |
| ResellerMpnId | Identificador de MPN del revendedor del registro de la suscripción.  |
| InvoiceNumber | Número de factura donde aparece la transacción especificada. | *D020001IVK* |
| ChargeStartDate | Fecha de inicio del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latente que no se hayan cobrado anteriormente (de ciclos de facturación anteriores). La hora es siempre el principio del día, 00:00. | *2/1/2019 0:00* |
| ChargeEndDate | Fecha final del ciclo de facturación, excepto cuando se presentan fechas de datos de uso latente que no se hayan cobrado anteriormente (de ciclos de facturación anteriores). La hora siempre corresponde al fin del día, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Identificador único para una suscripción en la plataforma de facturación de Microsoft. Puede ser útil para identificar la suscripción al ponerse en contacto con el soporte técnico. No se usa para la conciliación. *Esto no es lo mismo que el identificador **de suscripción en** la consola de administración de partners.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Alias de la oferta de servicio. | *Microsoft Azure* |
| SubscriptionDescription | Línea de negocio de la oferta de servicio. | *Microsoft Azure* |
| OrderID | Identificador único para un pedido en la plataforma de facturación de Microsoft. Puede ser útil para identificar la suscripción al ponerse en contacto con el soporte técnico. No se usa para la conciliación. | *566890604832738111* |
| ServiceName | Nombre del servicio de Azure en cuestión. | *MÁQUINAS VIRTUALES* |
| ServiceType | Tipo específico del servicio de Azure. | *Service Bus : individual o pack*, base de datos de SQL Azure – Business o Web *Edition* |
| ResourceGuid | Identificador único específico de todos los datos de servicio y de la estructura de precios. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| nombreDelRecurso | El nombre del recurso de Azure. | *Transferencia de datos en (GB)*, *transferencia de datos fuera (GB)* |
| Region (Región) | Región a la que se aplica el uso. Se usa principalmente para asignar tasas a transferencias de datos, ya que las tasas varían según la región. | *Asia Pacífico*, *Europa*, *América Latina*, *Norteamérica* |
| SKU | Identificador único de Microsoft para una oferta. | *7UD-00001* |
| DetailLineItemId | Identificador y cantidad que se deba a las distintas tarifas de un servicio o recurso en un período de facturación determinado. En el caso de los precios por niveles de Azure, puede haber una tarifa para hasta una determinada cantidad de unidades facturables y, a continuación, una tarifa diferente después de esa cantidad. | *1* |
| ConsumedQuantity | Cantidad de servicio consumido (por ejemplo, horas o GB) durante el período de informes. También incluye cualquier uso no facturado de períodos de informes anteriores. | *11* |
| IncludedQuantity | Unidades que se incluye como parte de la oferta. Normalmente no está presente en CSP. | *0* |
| OverageQuantity | Unidades no incluidas como parte de la oferta. El asociado los debe pagar. Igual a **ConsumedQuantity** menos **IncludedQuantity.** | *11* |
| ListPrice | Precio de la oferta en vigor en la fecha de inicio de la suscripción. | *$0,0808* |
| PretaxCharges | Igual a **ListPrist** multiplicado por **OverageQuantity**, redondeado al céntimo más cercano. | *0.085 USD* |
| TaxAmount | Importe de impuestos cobrado. En función de las reglas fiscales del mercado y las circunstancias específicas. | *0,08 USD* |
| PostTaxTotal | Total después de impuestos, cuando correspondan impuestos. | *0,93 USD* |
| Moneda | Tipo de moneda. Cada entidad de facturación tiene solo una moneda. Compruebe que coincide con la primera factura y, a continuación, después de las actualizaciones principales de la plataforma de facturación. | *EUR* |
| PretaxEffectiveRate | Precio unitario antes de impuestos. Igual a **PretaxCharges** dividido por **OverageQuantity**, redondeado al céntimo más cercano. | *0,08 USD* |
| PostTaxEffectiveRate | Precio unitario después de impuestos. Igual a **PostTaxTotal** dividido por **OverageQuantity**, redondeado al céntimo más cercano. O bien, igual a **PretaxEffectiveRate más** el tipo impositivo por importe unitario, redondeado al céntimo más cercano. | *0,08 USD* |
| ChargeType | Tipo [de cargo](recon-file-charge-types.md) o ajuste. | Vea tipos [de cargos](recon-file-charge-types.md). |
| CustomerId | Identificador único de Microsoft para el cliente, en formato GUID. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Nombre de dominio del cliente. Este campo puede aparecer en blanco hasta el segundo ciclo de facturación. | *ejemplo.onmicrosoft.com* |
| BillingCycleType | Frecuencia de facturación de tiempo.| **Mensual**  |
| Unidad | Unidad del recurso **Nombre**. | *GB* u *HOURS* |
| CustomerBillableAccount | Identificador de cuenta único en la plataforma de facturación de Microsoft. | *1280018095* |
| UsageDate | Fecha de implementación del servicio. | *2/1/2019 0:00* |
| MeteredRegion | Identifica la ubicación de un centro de datos dentro de la región (para los servicios donde este valor es aplicable y rellenado). | *Este de Asia*, *Sudeste de Asia*, Norte *de* Europa *,* Oeste de Europa , *Centro-norte de EE. UU.*, *Centro-sur de EE. UU.* |
| MeteredService | Identifica el uso individual del servicio de Azure cuando no se identifica específicamente en la **columna ServiceName.** Por ejemplo, las transferencias de datos se *notifican como Microsoft Azure- Todos los servicios* en la **columna ServiceName.** | *AccessControl,* *CDN,* *Compute,* *Database,* *ServiceBus,* *Storage* |
| MeteredServiceType | Subpartida para **el campo MeteredService** que proporciona una aclaración adicional del uso del servicio de Azure. | *EXTERNAL* |
| Project | Nombre definido por el cliente para su instancia de servicio. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Número de conexiones Azure Service Bus que se aprovisionaron y usaron en un día determinado. | *1,000000 conexiones / 30* días (si tenía una conexión aprovisionada individualmente durante un mes de 30 días), 25 conexiones */ 30 días - Usado: 1,0000000* (si tenía un paquete de 25 conexiones de Service Bus aprovisionadas y usó 1 durante ese día) |

## <a name="next-steps"></a>Pasos siguientes

- [Comprender los campos de los Centro de partners de conciliación basados en licencias](license-based-recon-files.md)