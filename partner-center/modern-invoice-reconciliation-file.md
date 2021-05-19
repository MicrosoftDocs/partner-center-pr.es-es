---
title: Recon file fields for CSP one-time purchases (Recon file fields for CSP one-time purchases) (Recon file fields for CSP one-time
ms.topic: conceptual
ms.date: 01/29/2021
description: Obtenga información sobre todos los elementos del archivo de conciliación de compras de un solo uso de CSP Centro de partners, incluidos los valores de ejemplo.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.openlocfilehash: 85946f44e1265ad5012faf9d782609904100c80e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146262"
---
# <a name="csp-one-time-purchase-reconciliation-file-fields"></a>Campos de archivo de conciliación de compras únicas de CSP

**Roles adecuados:** Administrador de | Agente de facturación

## <a name="using-the-recon-file"></a>Uso del archivo de conciliación
En la tabla siguiente se muestran las descripciones y los valores de ejemplo de los campos del archivo de conciliación para las compras únicas de CSP.

Para obtener más información sobre los archivos de conciliación, [vea Usar los archivos de conciliación](use-the-reconciliation-files.md).

| Columna | Descripción | Valor de ejemplo |
| ------ | ----------- | ------------ |
| PartnerId | Identificador único en formato GUID para una entidad de facturación específica. No es necesario para la conciliación. Igual en todas las filas. | *0e195b37-4574-4539-bc42-0e539b9684c0* |
| CustomerId | Identificador único de Microsoft para el cliente en formato GUID. | *196e2273-9651-43a3-ba7e-7cbcd918fc40* |
| CustomerName | Nombre de la organización del cliente según figura en el Centro de partners. Esta columna es importante para conciliar la factura con la información del sistema. | *Quer modern cust DE2* |
| CustomerDomainName | Nombre de dominio del cliente. | *testcustomerdomain.onmicrosoft.com* |
| CustomerCountry | El país donde se encuentra el cliente. Consulte la lista [completa de países](./regional-authorization-overview.md) de su región.  | *DE* |
| InvoiceNumber | Número de factura asociado al archivo de conciliación.  | *G002297372* |
| MpnId | Identificador de MPN del asociado de CSP. Para obtener más información, [vea cómo agregar elementos por asociado.](./use-the-reconciliation-files.md#itemize-reconciliation-files-by-partner) | *6034453* |
| ResellerMpnId | Identificador de MPN del revendedor del registro de la suscripción. | *6048879* |
| OrderId | Identificador único para un pedido en la plataforma de facturación de Microsoft. Puede ser útil para identificar el pedido al ponerse en contacto con el soporte técnico. No se usa para la conciliación. | *0ET2qaZvJGfF9wgSKnWzR5JLmhp10lOc1* |
| OrderDate | Fecha en UTC en la que se ha realizado el pedido. | *10/3/2020* |
| ProductId | Identificador único del producto. | *DZH318Z0BNZ5* |
| SkuId | Identificador único de SKU. | *006G* |
| AvailabilityId | Identificador único de disponibilidad. | *DZH318Z08B80* |
| SkuName | Nombre de la SKU. | *Tablas: LRS* |
| ProductName | Nombre del producto. | *Tablas* |
| ChargeType | Tipo [de cargo o](./recon-file-charge-types.md) ajuste. | *Nuevo* |
| UnitPrice | Precio por licencia, tal como se publicó en la lista de precios en el momento de la compra. Asegúrese de que coincide con la información almacenada en el sistema de facturación durante la conciliación. | *0.045* |
| Cantidad | Número de licencias. Asegúrese de que coincide con la información almacenada en el sistema de facturación durante la conciliación. | *1* |
| Subtotal | Total sin impuestos. El subtotal debe ser igual a la cantidad facturable multiplicada por el precio unitario efectivo. | *0* |
| TaxTotal | Cargo por importe de impuestos. En función de las reglas fiscales del mercado y las circunstancias específicas. | *0* |
| Total | El importe total es igual al subtotal más el importe de impuestos. | *0* |
| Moneda | La factura se genera en el contexto de la moneda del cliente. Esto significa que, si eres un partner que está realizando transacciones con clientes con distintas monedas de facturación, recibirás una factura por cada tipo de moneda de cliente.  | *EUR* |
| PriceAdjustmentDescription | Los motivos de los ajustes en el precio unitario. Estas son las razones principales, pero no se limitan a determinar el precio unitario efectivo. | *["15,0 % crédito obtenido del partner por los servicios administrados"]* |
| PublisherName | Publicador del producto.  | *Microsoft* |
| PublisherId | Identificador único que el Centro de partners usa para identificar al publicador. | *Na* |
| SubscriptionDescription | Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios. Esta columna es un campo idéntico a OfferName. | *Plan de Azure* |
| SubscriptionId | Identificador único para una suscripción en la plataforma de facturación de Microsoft. No se usa para la conciliación. Tenga en cuenta que este identificador no es el mismo que el identificador de suscripción en la consola de administración del asociado. | *307628f1-d9d2-f09c-ea1f-4183f0cae308* |
| ChargeStartDate | Fecha en que se inicia el período de facturación de una suscripción. | *9/1/2020* |
| ChargeEndDate | Fecha en que finaliza el período de facturación de una suscripción. | *30/09/2020* |
| TermAndBillingCycle | El compromiso de duración para continuar con la suscripción en el momento de la compra. | *Datos almacenados (GB/mes)* |
| EffectiveUnitPrice | Precio unitario prorrateado para calcular el costo del ciclo de facturación. Los descuentos, los ajustes en los días de facturación y otros factores determinan el precio unitario efectivo. Para obtener más información, vea [Effective Unit Price Calculation](./effective-unit-price-calculation.md).  | *0.03825* |
| UnitType | Tipo de unidad en la que se cobra el medidor. | *1 GB/mes* |
| AlternateId | Identificador alternativo del elemento de línea de pedido al que se hace referencia. | *6dc5c039750a* |
| BillableQuantity | Cantidad total que se está facturando.  | *0.005001* |
| BillingFrequency | Plan de facturación seleccionado en el momento de la compra. | *Na*  |
| PricingCurrency | Moneda de la lista de precios. | *USD* |
| PCToBCExchangeRate | Tipo de cambio aplicado para la moneda de precios a la moneda de facturación. | *0.846202666* |
| PCToBCExchangeRateDate | Fecha en la que se determina la moneda de precios a la moneda de facturación. | *30/09/2020* |
| MeterDescription | Descripción del medidor.  | *Tablas: datos LRS almacenados (GB/mes)* |
| ReservationOrderId | Identificador del pedido de reserva. | *E21A6344E398FFC1C4D7...* |
| CreditReasonCode | Descripción del crédito. | *Crédito de consumo de Azure* |

>[!NOTE]
>Puede conciliar el consumo de Azure en el archivo de conciliación de una sola compra. Para ello, vaya al archivo de conciliación de uso clasificado diariamente y busque subscriptionID. Esto mostrará todos los costos asociados con el identificador del plan de Azure. El Identificador de suscripción de Azure se muestra como EntitlementID.

## <a name="next-steps"></a>Pasos siguientes

- [Facturación e impuestos](billing.md)
