---
title: Preguntas más frecuentes sobre el pago para Microsoft Commercial Marketplace
description: Obtenga respuestas a preguntas habituales sobre los pagos en Marketplace comercial. Incluye respuestas sobre el motivo por el que las ganancias son diferentes de las esperadas.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 09/11/2020
ms.openlocfilehash: 5775eb497940870344e0d3da85def7c3e717c65f
ms.sourcegitcommit: cc30a06abe55b9da32177a24e74bfd6fc7d8bbb9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/12/2020
ms.locfileid: "94532028"
---
# <a name="common-questions-about-commercial-marketplace-payouts"></a>Preguntas comunes sobre los pagos comerciales de Marketplace

En este artículo se responden las preguntas más frecuentes sobre los pagos en Marketplace comercial.

## <a name="earnings-incorrect-or-missing"></a>Ganancias incorrectas o ausentes

#### <a name="why-are-my-earnings-missing"></a>¿Por qué faltan mis ganancias?

- Es posible que el pedido del cliente todavía no sea válido para el pago. En el caso de los pedidos de clientes que no sean empresariales, Microsoft debe recibir el pago del cliente antes de que las ganancias del publicador sean válidas. En el caso de los pedidos de clientes empresariales, las ganancias estarán disponibles uno o dos días después de la fecha del pedido de compra. Compruebe el estado del pedido en los [informes de pedidos](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Es posible que las ganancias de las transacciones anteriores a julio de 2019 no se muestren en el informe del historial de transacciones. Consulte los extractos históricos en la [descarga de pagos](https://partner.microsoft.com/dashboard/payouts/reports/incentiveexport).
- Compruebe el período [de tiempo del ciclo de pago](payment-thresholds-methods-timeframes.md) y comprenda Cuándo deben aparecer las ganancias en la declaración de pago.

#### <a name="why-is-my-earnings-amount-different-than-what-i-expected"></a>¿Por qué la cantidad de ganancias es diferente de la esperada?

- Si el cliente pagó parcialmente el pedido, el importe de la ganancia se basará en el importe de pago parcial después de deducir la cuota y el impuesto adecuado.
- Comprobar la responsabilidad de la remisión de impuestos por país. En el caso de los países en los que Microsoft sea responsable del impuesto, Microsoft recauda y descuenta el impuesto de las ganancias del publicador. El importe de la transacción que se muestra en el extracto es posterior al importe del impuesto. Consulte el artículo sobre [datos fiscales](tax-details-marketplace.md).
- Las ofertas de SaaS y IaaS tienen un precio de agencia con descuento al 10% en lugar del 20% estándar, lo que permite una tasa de ganancias del 90%. Esta promoción es efectiva hasta el 30 de junio de 2021.

**Más** información: [contrato de publicador de Marketplace comercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), detalles de la [Directiva de pago](payout-policy-details.md), [umbral de pago, método y](payment-thresholds-methods-timeframes.md)período de tiempo, y se [paga en el Marketplace comercial, los detalles de](marketplace-get-paid.md) [impuestos](tax-details-marketplace.md), las [instrucciones](payout-statement.md)de pago, el [Panel de pedidos en el análisis de Marketplace comercial](/azure/marketplace/partner-center-portal/orders-dashboard) .

## <a name="earnings-reconciliation"></a>Conciliación de ganancias
### <a name="how-do-i-reconcile-payout-statements-to-order-or-usage-reports-in-analytics"></a>¿Cómo concilio los extractos de pago para los informes de pedidos o uso en los análisis?
Use AssetID, orderID y el ID. de elemento de línea que aparecen en el informe de historial de transacciones de pago con pedidos de análisis e informes de uso. Use esta asignación:

- Transacción de pago History.AssetID = order.OrderID
- Transacción de pago History.OrderID & LineItem = Usage.UsageReferenceID [OrderID:LineItemID]

### <a name="how-do-i-know-when-to-expect-payments-for-my-customer-orders"></a>¿Cómo sabe cuándo se deben esperar los pagos de los pedidos de los clientes?
- En primer lugar, mediante AssetID, compruebe los pedidos de clientes en los [informes de pedidos](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/order).
- Compruebe el canal del cliente para la suscripción de cliente en el [Informe de clientes](https://partner.microsoft.com/dashboard/commercial-marketplace/analytics/customer).
- En el caso de los clientes empresariales, los beneficios del publicador aparecen en la declaración 1-2 días después de la fecha del pedido de compra.
- En el caso de los clientes que no son de empresa, los beneficios del publicador aparecen en la declaración 1-2 días después de recibir el pago del cliente.

**Lecturas adicionales** : [declaraciones de pago](payout-statement.md), [Panel de pedidos en el análisis de Marketplace comercial](/azure/marketplace/partner-center-portal/orders-dashboard)

## <a name="payout-policies"></a>Directivas de pago

#### <a name="how-do-i-find-the-current-agency-fee-and-the-payout-rate"></a>¿Cómo encuentro el precio actual de la agencia y la tarifa de pago?

- Consulte el acuerdo de publicador de marketplace comercial. El precio de la agencia estándar es del 20 %. Los Co-Sell las transacciones válidas de SaaS tienen un descuento de un 10%. Compruebe los anuncios de los precios de las agencias promocionales.
- En la declaración de pago, la tarifa de obtención especifica la tasa de pago real de una transacción determinada.

#### <a name="when-can-i-expect-a-payment-from-microsoft-once-earnings-appear-on-my-statement"></a>¿Cuándo se puede esperar un pago de Microsoft una vez que aparezcan ganancias en el extracto?
- Una vez que la ganancia está en estado sin procesar, puede comprobar la fecha de vencimiento del mes en que se procesarán las ganancias para el pago. Una vez preparado el pago, el estado de la ganancia cambiará a "procesado".  Microsoft publica los pagos antes del día 15 del vencimiento.
- En el caso de los pedidos pagados por tarjeta de crédito, Microsoft conserva los pagos de 30 días hasta que se realiza la obtención de un adulto.

 **Lectura adicional** : [contrato de publicador de Marketplace comercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), detalles de la [Directiva de pago](payout-policy-details.md), [detalles de impuestos](tax-details-marketplace.md), [umbral de pago, método y](payment-thresholds-methods-timeframes.md) período de tiempo

## <a name="payments-and-adjustments"></a>Pagos y ajustes

#### <a name="why-is-my-payment-missing"></a>¿Por qué falta mi pago?

- Asegúrese de que el estado de pago y el estado del perfil fiscal se muestran como *válidos* en la [Página de información general](https://partner.microsoft.com/dashboard/commercial-marketplace/overview).
- Es posible que no haya alcanzado el umbral mínimo para un pago. Las ganancias deben ser de al menos 50 USD para recibir un pago.


#### <a name="how-do-i-set-my-account-to-not-receive-payment"></a>Cómo configurar la cuenta para que no reciba el pago?
Puede mantener los pagos en el [Perfil de pago](https://partner.microsoft.com/dashboard/commercial-marketplace/overview); solo tiene que comprobar la **suspensión**. Microsoft le enviará un pago hasta que publique la suspensión.

#### <a name="why-do-i-receive-in-a-different-currency-than-the-purchase-currency"></a>¿Por qué lo recibo en una moneda distinta a la moneda de la compra?

La moneda del pago se basa en la moneda seleccionada en el perfil de pago. La moneda de compra se basa en la moneda que la que pagó el cliente.

#### <a name="how-do-i-reconcile-adjustments"></a>¿Cómo concilio los ajustes?

Los ajustes de pago son correcciones de pago para dar cabida a ajustes compensatorios, como problemas del sistema. En el extracto de pago, ReasonCode especificará el motivo del ajuste. No están diseñados para conciliarse directamente con transacciones individuales.

**Lectura adicional** : [contrato de publicador de Marketplace comercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), detalles de la [Directiva de pago](payout-policy-details.md), [detalles de impuestos](tax-details-marketplace.md), [umbral de pago, método y](payment-thresholds-methods-timeframes.md) período de tiempo

## <a name="taxes"></a>Impuestos

#### <a name="how-do-we-identify-tax-remit-responsibility-between-microsoft-or-publisher-in-the-payout-statement"></a>¿Cómo se identifica la responsabilidad de la remisión de impuestos entre Microsoft o el publicador en el extracto de pagos?

En la descarga del historial de transacciones, busque la columna del modelo de impuestos. Esta columna muestra si está administrado por MS o por ISV. Consulte las reglas de impuestos específicas del país y las implicaciones de pago en el artículo sobre [datos fiscales](tax-details-marketplace.md).

#### <a name="how-do-i-download-service-fee-tax-forms"></a>¿Cómo descargo los formularios fiscales sobre precios de servicio?

Vaya a la página **Payout Payment** (Pagos) y, a continuación, en la sección **List of Payment** (Lista de pagos). Aparece un vínculo al formulario fiscal sobre precios de servicio para un pago que tiene el impuesto sobre precios de servicio.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>¿Cómo descargo un formulario de retención fiscal en PDF?

Vaya a la página *Payout Payment* (Pagos) y, a continuación, en la sección **List of Payment** (Lista de pagos). Aparecerá un vínculo a un formulario de retención fiscal junto a un pago.

#### <a name="where-do-i-find-year-end-tax-forms"></a>¿Dónde encuentro los formularios fiscales de fin de año?

Vaya a la [página del perfil](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) para ver los formularios fiscales de fin de año.

#### <a name="how-do-i-find-withholding-tax-for-a-transaction"></a>¿Cómo busco la retención de impuestos de una transacción?
La retención de impuestos se aplica a los publicadores de EE. UU. que han cumplimentado un formulario W-9. La retención de impuestos se calcula en un pago mensual.

**Lectura adicional** : [contrato de publicador de Marketplace comercial](https://go.microsoft.com/fwlink/p/?LinkID=699560), detalles de la [Directiva de pago](payout-policy-details.md)

## <a name="payout-statement-access"></a>Acceso a la declaración de pago

#### <a name="how-do-i-access-a-payout-statement"></a>¿Cómo se accede a un extracto de pagos?

1. Compruebe sus roles. Para acceder al extracto de pagos debe tener los roles *Colaborador financiero* o *Propietario de la cuenta*.
2. En la navegación superior derecha, seleccione el icono de **pago** para ver el informe de pago. Elija entre el **historial de transacciones** , el **pago** y la **descarga**.

**Lecturas adicionales** : [roles de pago y permisos](payout-statement.md#roles-and-permissions), [instrucciones de pago](payout-statement.md) 

## <a name="payout-statement-report"></a>Informe de la instrucción de pago

#### <a name="what-does-each-field-in-the-transaction-download-mean"></a>¿Qué significa cada campo de la descarga de la transacción?

Consulte las [instrucciones de pago](payout-statement.md) para obtener una lista detallada de los atributos y su significado.

#### <a name="what-is-earning-status"></a>¿Qué es el estado de ganancias?

Esto muestra las ganancias como no procesadas, procesadas o enviadas.

- Sin **procesar** : las ganancias se encuentran en un período de custodia hasta la fecha de vencimiento.
- **Procesado** : las ganancias se han madurado y están preparadas en un pago mensual. Los pagos se liberan el 15 de cada mes.
- **Enviado** : el pago se ha publicado correctamente en el Banco según el perfil de pago.

#### <a name="how-do-i-download-service-fee-tax-forms"></a>¿Cómo descargo los formularios fiscales sobre precios de servicio?

Vaya a la página **Payout Payment** (Pagos) y, a continuación, en la sección **List of Payment** (Lista de pagos). Aparece un vínculo al formulario fiscal sobre precios de servicio para un pago que tiene el impuesto sobre precios de servicio.

#### <a name="how-do-i-download-a-withholding-tax-form-in-pdf"></a>Cómo descargar un formulario de retención de impuestos en PDF?

Vaya a la página **Payout Payment** (Pagos) y, a continuación, en la sección **List of Payment** (Lista de pagos). Aparecerá un vínculo a un formulario de retención fiscal junto a un pago.

#### <a name="where-do-i-find-year-end-tax-forms"></a>¿Dónde encuentro los formularios fiscales de fin de año?

Vaya a la [página del perfil](https://partner.microsoft.com/dashboard/payee/profiles/partner/manage) para ver los formularios fiscales de fin de año.

**Lecturas adicionales** : [instrucciones de pago](payout-statement.md), [descarga de historial de transacciones](payout-statement.md#transaction-history-download)

## <a name="historical-statements"></a>Extractos históricos

#### <a name="how-do-i-view-historical-information"></a>Cómo ver información histórica?

El historial de extractos mostrará la instantánea de los datos de los pagos a partir de octubre de 2019. Desafortunadamente, la información de pago aquí no se actualiza. Para recibir la información más reciente, envíe una incidencia de soporte técnico para los datos más recientes.

**Lecturas adicionales** : [instrucciones de pago](payout-statement.md), [descarga de historial de transacciones](payout-statement.md#transaction-history-download)

## <a name="payout-export-api"></a>API de exportación de pagos

#### <a name="how-do-i-download-payout-data"></a>¿Cómo se descargan los datos de los pagos?

Use la [API de pago de socios comerciales](https://apidocs.microsoft.com/services/partnerpayouts).

## <a name="next-steps"></a>Pasos siguientes

- [Recepción de pagos en el Marketplace comercial](marketplace-get-paid.md)
