---
title: Campos de archivo de conciliación para compras de un solo tiempo de CSP
ms.topic: conceptual
ms.date: 11/10/2020
description: Obtenga información sobre todos los elementos del archivo de conciliación de compra de un solo tiempo de CSP en el centro de Partners, incluidos los valores de ejemplo.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 29574dad6c3dd5eedbcf93dd555509cb04144ef5
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182586"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Campos de archivo de conciliación de compra única de CSP

## <a name="using-the-recon-file"></a>Uso del archivo de conciliación
En la tabla siguiente se proporcionan descripciones y valores de ejemplo de los campos del archivo de conciliación para las compras de un solo tiempo de CSP.

Para obtener más información sobre los archivos de conciliación, vea [usar los archivos de conciliación](use-the-reconciliation-files.md).

| Columna | Descripción | Valor de ejemplo |
| ------ | ----------- | ------------ |
| PartnerId | Identificador único en formato GUID para una entidad de facturación específica. No es necesario para la reconciliación. Igual en todas las filas. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Identificador único de Microsoft para el cliente en formato GUID. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Nombre de la organización del cliente según figura en el Centro de partners. Esta columna es importante para conciliar la factura con la información del sistema. | *Johnny moderno DE2* |
| CustomerDomainName | Nombre de dominio del cliente. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | País en el que se encuentra el cliente. Consulte la [lista completa de países](./regional-authorization-overview.md) de su región.  | *RESGUARDO* |
| InvoiceNumber | Número de factura asociado al archivo de conciliación.  | *G002297372* |
| MpnId | Identificador de MPN del asociado de CSP. Para obtener más información, consulte [Cómo elemento por asociado](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner). | *6034453* |
| ResellerMpnId | Identificador de MPN del distribuidor de registro de la suscripción. | *6048879* |
| OrderId | Identificador único para un pedido en la plataforma de facturación de Microsoft. Puede ser útil para identificar el orden al ponerse en contacto con el servicio de soporte técnico. No se usa para la conciliación. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Fecha en que se realizó el pedido. | *10/3/2020* |
| ProductId | Identificador único del producto. | *DZH318Z0BNZ5* |
| SkuId | Identificador único de la SKU. | *006G* |
| AvailabilityId | Identificador único de disponibilidad. | *DZH318Z08B80* |
| SkuName | Nombre de la SKU. | *Tablas: LRS* |
| ProductName | Nombre del producto. | *Tablas* |
| ChargeType | [Tipo de cargo](./recon-file-charge-types.md) o ajuste. | *Nuevo* |
| UnitPrice | Precio por licencia, tal como se publicó en la lista de precios en el momento de la compra. Asegúrese de que coincide con la información almacenada en el sistema de facturación durante la conciliación. | *0,045* |
| Cantidad | El número de licencias. Asegúrese de que coincide con la información almacenada en el sistema de facturación durante la conciliación. | *1* |
| Subtotal | Total sin impuestos. El subtotal debe ser igual a la cantidad facturable multiplicada por el precio unitario efectivo. | *0* |
| TaxTotal | Cargo del importe de los impuestos. En función de las reglas de impuestos y las circunstancias específicas de su mercado. | *0* |
| Total | La cantidad total es igual al subtotal más la cantidad de impuestos. | *0* |
| Moneda | La factura se genera en el contexto de la moneda del cliente. Esto significa que, si eres un partner que está realizando transacciones con clientes con distintas monedas de facturación, recibirás una factura por cada tipo de moneda de cliente.  | *EUR* |
| PriceAdjustmentDescription | Los motivos por los que se han realizado los ajustes en el precio por unidad. Estas son las razones principales, pero no se limitan a determinar el precio por unidad vigente. | *["15,0% de crédito obtenido por el socio comercial para servicios administrados"]* |
| PublisherName | Publicador del producto.  | *Microsoft* |
| PublisherId | Identificador único que usa el centro de partners para identificar al publicador. | *NA* |
| SubscriptionDescription | Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios. Esta columna es un campo idéntico a Nombredeoferta. | *Plan de Azure* |
| SubscriptionId | Identificador único para una suscripción en la plataforma de facturación de Microsoft. No se usa para la conciliación. Tenga en cuenta que este identificador no es el mismo que el identificador de suscripción en la consola de administración de socios comerciales. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | La fecha en que el centro de Partners cobra la cuota de suscripción. Si la suscripción se compra con un período de facturación anual y un plan de facturación mensual, en el primer archivo de conciliación, este es el día en el que se adquiere la suscripción. A partir del siguiente archivo de conciliación, se incrementará en 30 días. | *9/1/2020* |
| ChargeEndDate | Final del ciclo de facturación de la suscripción. Si la suscripción se compra con un período de facturación anual y un plan de facturación mensual, en el primer archivo de conciliación, este es el trigésimo día después de la compra de la suscripción. A partir del siguiente archivo de conciliación, se incrementará en 30 días. | *30/09/2020* |
| TermAndBillingCycle | El compromiso de duración para continuar con la suscripción en el momento de la compra. | *Datos almacenados (GB/mes)* |
| EffectiveUnitPrice | El precio unitario prorrateado para calcular el costo del ciclo de facturación. Los descuentos, los ajustes de los días de facturación y otros factores determinan el precio por unidad vigente. Para obtener más información, consulte [cálculo del precio unitario en vigor](./effective-unit-price-calculation.md).  | *0,03825* |
| UnitType | Tipo de unidad en la que se carga el medidor. | *1 GB/mes* |
| AlternateId | El ID. alternativo del elemento de línea de pedido al que se hace referencia. | *6dc5c039750a* |
| BillableQuantity | La cantidad total que se va a facturar.  | *0,005001* |
| BillingFrequency | Plan de facturación seleccionado en el momento de la compra. | *NA*  |
| PricingCurrency | Moneda de la lista de precios. | *USD* |
| PCToBCExchangeRate | La tasa de cambio que se aplica para la moneda de facturación. | *0,846202666* |
| PCToBCExchangeRateDate | Fecha en la que se determina la moneda de los precios de la moneda de facturación. | *30/09/2020* |
| MeterDescription | Descripción del medidor.  | *Tablas: datos LRS almacenados (GB/mes)* |
| ReservationOrderId | Identificador del pedido de reserva. | *E21A6344E398FFC1C4D7...* |

## <a name="next-steps"></a>Pasos siguientes

- [Facturación e impuestos](billing.md)