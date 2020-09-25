---
title: Declaración de pago para el Marketplace comercial en el centro de Partners
description: Obtenga información acerca de las instrucciones de pago y resúmenes, y cómo ver y exportar los datos de pago del Marketplace comercial
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: mingshen-ms
ms.author: mingshen
ms.date: 09/23/2020
ms.openlocfilehash: 460a7b1992d7db40e0f45d3aeb7e2236e9495e07
ms.sourcegitcommit: a84812b650ec8b6d0513c46c04840e4bbb0c8460
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/25/2020
ms.locfileid: "91335782"
---
# <a name="payout-statements"></a>Instrucciones de pago

La **declaración de pago** presenta una visión general de los pagos de ofertas vendidas a través del Marketplace comercial. Muestra el historial transaccional de los ingresos, calcula el siguiente pago y muestra las tendencias de pago. También puede descargar el historial de transacciones y las instrucciones de pago. En este artículo se explica cómo acceder a la declaración de pago y las distintas páginas de pago y descargas a las que se puede acceder en el centro de Partners.

## <a name="roles-and-permissions"></a>Roles y permisos

Para tener acceso a una declaración de pago, debe tener asignado el rol propietario de la **cuenta** o **colaborador financiero** .

| Informes/páginas | Propietario de cuenta | Manager | Desarrollador | Colaborador empresarial | Colaborador financiero | Vendedor |
| --- | --- | --- | --- | --- | --- | --- |
| Informe de adquisición (incluidos los datos casi en tiempo real) | Puede ver | Puede ver | Sin acceso | Sin acceso | Puede ver | Sin acceso |
| Respuesta/informe de comentarios | Puede ver y enviar comentarios | Puede ver y enviar comentarios | Puede ver y enviar comentarios | Sin acceso | Sin acceso | Puede ver y enviar comentarios |
| Informe de mantenimiento (incluidos los datos casi en tiempo real) | Puede ver | Puede ver | Puede ver | Puede ver | Sin acceso | Sin acceso |
| Informe de uso | Puede ver | Puede ver | Puede ver | Puede ver | Sin acceso | Sin acceso |
| Cuenta de pago | Puede actualizar | Sin acceso | Sin acceso | Sin acceso | Puede actualizar | Sin acceso |
| Perfil fiscal | Puede actualizar | Sin acceso | Sin acceso | Sin acceso | Puede actualizar | Sin acceso |
| Resumen de pagos | Puede ver | Sin acceso | Sin acceso | Sin acceso | Puede ver | Sin acceso |
|

## <a name="access-your-payout-statement"></a>Acceder a su declaración de pago

Inicie sesión en el [centro de Partners](https://partner.microsoft.com/dashboard/home) y seleccione el icono de pago en la esquina superior derecha de la pantalla para obtener acceso a los distintos resúmenes:

- Historial de transacciones
- Pagos
- Exportar datos

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Muestra el icono de pago en la esquina superior derecha del portal del centro de Partners.":::

También puede usar la [API de pago de socios comerciales](https://apidocs.microsoft.com/services/partnerpayouts) para conectarse y obtener datos de pagos y transacciones de pago directamente.


## <a name="transaction-history"></a>Historial de transacciones

La página **historial de transacciones** muestra el Resumen de los ingresos, el siguiente pago estimado y la tendencia de ganancias y pagos en los últimos 36 meses. También puede descargar los detalles de las transacciones en esta sección.

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Información general sobre transacciones.":::

- **Ganancias enviadas este año** : ingresos totales y desglose de los ingresos que se han pagado y se pagarán en el próximo mes.
- **Mes de pago estimado** : total de ganancias esperadas en los próximos meses.
- **Ingresos y tendencias de pago** : importes de pago y de ganancias mensuales durante los últimos 36 meses.
- **Descargar** : Descargue los detalles de la transacción en formato. csv o. TSV.

Use la selección de intervalo de fechas en la esquina superior derecha de la página para filtrar el resultado de la página para mostrar los últimos 3, 6, 12 o 36 meses. O bien, seleccione un intervalo de fechas personalizado hasta 36 meses. El intervalo de fechas predeterminado es de 12 meses.

:::image type="content" source="images/payouts/search-filter.png" alt-text="El filtro de búsqueda en la parte superior derecha de la página.":::

### <a name="transaction-history-summary"></a>Resumen de historial de transacciones

Esto muestra la obtención de detalles, incluido el origen de la obtención del producto vendido de fechas, Estados y meses de pago estimados.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Historial de transacciones.":::

- **Fecha acumulada** : la fecha de compra.
- **Tipo de ganancia** : el tipo de ganancia, como la venta, el descuento o la Co-op.
- **Importe total** : la cantidad neta ganada. En el Marketplace comercial, esto significa que, después de deducir la cuota de mercado estándar.
- **Estado** : tiene tres opciones:
    - **Próximos** : las ganancias se encuentran en un período de enfriamiento pendiente.
    - **Procesado** : las ganancias están preparadas para el siguiente pago.
    - **Enviado** : se han pagado las ganancias.
- **Mes de pago estimado** : el mes en el que se espera que se paguen los ingresos.

Las transacciones de obtención se muestran una vez que la transacción cumple la elegibilidad del pago. Para comprender por qué es posible que haya ganancias inesperadas o inesperadas, consulte [preguntas comunes sobre los pagos comerciales de Marketplace](payout-faq.md#why-are-my-earnings-missing).

### <a name="transaction-history-download"></a>Descarga del historial de transacciones

Para ver más detalles sobre una ganancia, seleccione **Descargar** en la parte superior de la página. En la tabla siguiente se explica cada columna del informe.

| Nombre de la columna | Descripción | Aplicabilidad de programas de incentivos/Marketplace |
| --- | --- | --- |
| agreementEndDate | Fecha de finalización del acuerdo. | Incentivos: solo algunos programas |
| agreementNumber | Número de acuerdo. | Incentivos: solo algunos programas |
| agreementStartDate | Fecha de inicio del acuerdo. | Incentivos: solo algunos programas |
| calculationDate | Fecha en que se calculó la ganancia en el sistema. | All |
| claimId | Identificador único de una notificación. | Incentivos: solo algunos programas |
| customerCountry | País o región del cliente. | marketplaces |
| customerEmail |  |  |
| customerName | Siempre estará en blanco. | Solo programas de incentivos (excepción: OEM) y Marketplaces |
| customerTenantId |  |  |
| distributorId | Identificador de distribuidor. | Incentivos: solo algunos programas |
| distributorName | Nombre del distribuidor. | Incentivos: solo algunos programas |
| earningAmount | Importe de la ganancia en la moneda original de la transacción. | All |
| earningAmountInLastPaymentCurrency | Importe de la ganancia en la moneda del último pago (el campo estará vacío si no ha habido ningún pago anterior). |  |
| earningAmountUSD | Importe de la ganancia en USD. | All |
| earningDate | Fecha de la ganancia. | All |
| earningExchangeRate | Tipo de cambio usado para mostrar el importe en USD correspondiente. | All |
| earningId | Identificador único de cada ganancia. | All |
| earningRate | Tasa de incentivos aplicada en el importe de la transacción para generar una ganancia | All |
| earningType | Indica si se trata de honorarios, devolución, cooperativo, venta, etc. | All |
| exchangeRateDate | Fecha del tipo de cambio usada para calcular earningAmountUSD. | All |
| externalReferenceId | Identificador único del programa. | Programas de pago directo (incentivos y Marketplace) |
| externalReferenceIdLabel | Etiqueta del identificador único. | Programas de pago directo (incentivos y Marketplace) |
| instantRebateAmount |  |  |
| Fechafactura |  |  |
| invoiceNumber | Número de factura (aplicable solo para empresas) | Incentivos y Marketplace: solo algunos programas |
| lastPaymentCurrency | Moneda del último pago (el campo estará vacío si no ha habido ningún pago anterior). |  |
| lever | Indica la regla de negocios de la ganancia. | All |
| LicensingProgramName | Nombre del programa de licencias. |  |
| LineItemId | Línea individual en la factura de un cliente. |  |
| localProviderSeller | Proveedor o vendedor local del registro. |  |
| Mes de madurez | El mes de pago estimado | All |
| OrderId | Se relaciona con la factura de un cliente.  | marketplaces |
| parentProductId | Identificador único del producto principal. Si no hay un producto principal para la transacción, el identificador del producto principal es igual al identificador del producto. | marketplaces |
| parentProductName | Nombre del producto principal. Si no hay un producto principal para la transacción, el nombre del producto principal es igual al nombre del producto. | marketplaces |
| participantId | Identidad principal del asociado que gana con el programa. | All |
| participantIdType | Principalmente el identificador de programa para los programas de incentivos y el vendedor si se trata de Marketplace | All |
| participantName | Nombre del asociado que gana. | All |
| partnerCountryCode | Ubicación, país o región del asociado que gana. | All |
| partNumber | Siempre estará en blanco. | Algunos programas de incentivos y Marketplace |
| paymentId | Identificador único del pago. Este número suele aparecer en el extracto del banco. | Solo pagos de SAP |
| paymentStatus | Estado del pago. | All |
| paymentStatusDescription | Descripción detallada del estado del pago. | All |
| productId | Identificador único del producto. | marketplaces |
| ProductName | Nombre del producto vinculado a la transacción. | All |
| productType | Tipo de producto, como, por ejemplo, aplicación, complemento o juego. | marketplaces |
| Código de programa. | Cadena que se va a asignar con el nombre del programa. |  |
| programName | Nombre del programa de incentivos/tienda. | All |
| purchaseOrderCoverageEndDate | Siempre estará en blanco. | Programa de incentivos: CRI |
| purchaseOrderCoverageStartDate | Siempre estará en blanco. | Programa de incentivos: CRI |
| purchaseOrderType | Siempre estará en blanco. | Programa de incentivos: CRI |
| purchaseTypeCode | Siempre estará en blanco. | Programa de incentivos: CRI |
| quantity | Varía en función del programa. Indica la cantidad facturada en los programas de transacción. | All |
| reasonCode |  |  |
| resellerCountry |  |  |
| resellerId | Identificador del revendedor. | Incentivos: solo algunos programas |
| resellerName | Nombre del revendedor. |  |
| SkuId | Identificador de la SKU definida durante la publicación. Una oferta puede tener muchas SKU, pero una SKU solo puede asociarse a una única oferta. Incentivos: solo algunos programas |  |
| storeFee | El importe retenido por Microsoft como honorarios por hacer que la aplicación o el complemento estén disponibles en la Tienda. | marketplaces |
| subscriptionEndDate | Fecha de finalización de la suscripción. | Incentivos: solo algunos programas |
| subscriptionId | Identificador de suscripción asociado al cliente. | Incentivos: solo algunos programas |
| subscriptionStartDate | Fecha de inicio de la suscripción. | Incentivos: solo algunos programas |
| taxCity |  |  |
| taxCountry |  |  |
| taxRemitModel | Entidad responsable de la emisión de impuestos (ventas, uso o impuestos de IVA/GST). | marketplaces |
| taxRemitted | Importe del impuesto remitido (ventas, uso o impuestos de IVA/GST). | marketplaces |
| taxState | Estado del cliente. |  |
| taxZipCode | Código postal del cliente. |  |
| tpan | Indica la red de anuncios de terceros. | solo anuncios de Marketplace |
| transactionAmount | Importe de la transacción en la moneda original de la transacción en función de la ganancia generada. | All |
| transactionAmountUSD | Importe de la transacción en USD. | All |
| transactionCountryCode | Código de país o región en el que se ha producido la transacción. |  |
| transactionCurrency | Moneda en la que se produjo la transacción original del cliente (no es la moneda de la ubicación del asociado). | All |
| transactionDate | Fecha de la transacción. Útil para programas en los que muchas transacciones contribuyen a una ganancia. | All |
| transactionExchangeRate | Tipo de cambio usado para mostrar el importe en USD correspondiente de la transacción. | All |
| transactionId | Identificador único de la transacción. | All |
| transactionPaymentMethod | Instrumento de pago del cliente usado para la transacción, como, por ejemplo, tarjeta, facturación del operador móvil o PayPal. | marketplaces |
| transactionType | Tipo de transacción, como, por ejemplo, compra, reembolso, revocación o contracargo. | marketplaces |
| carga de trabajo | Carga de trabajo | Incentivos: solo algunos programas |
|

## <a name="payments"></a>Pagos

En la página **pagos** se detalla el dinero que ha obtenido con Microsoft. También muestra Cuándo y cuánto se pagará.

>[!Note]
> Para poder acceder a esta opción, sus ganancias deben alcanzar el [umbral de pago](payment-thresholds-methods-timeframes.md) de 50 USD. Para obtener más información, vea el [contrato de Microsoft Publisher](https://go.microsoft.com/fwlink/?LinkID=699560).

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Pantalla de información general de pagos.":::

- **Total de pago de este año** : el total combinado abonado a su año, en dólares estadounidenses, para todos sus programas.
- **Siguiente pago estimado** : el siguiente pago que le llega (aunque haya otros que estén disponibles próximamente), en dólares estadounidenses.
- **Último pago** : la cantidad (en dólares estadounidenses), el nombre del programa y el programa del pago más reciente.
- **Pago por origen** : cantidad de pagos (en dólares estadounidenses), por programa, en los últimos 12 meses.

### <a name="payments-list"></a>Lista de pagos

La tabla **de la lista de pagos** muestra pagos pendientes y de pago. Puede descargar la información fiscal de tarifas de servicio en formato PDF y ver los detalles de obtención de un pago determinado.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Exportar historial de transacciones":::

- **Pagado** : todos los pagos se enviaron correctamente. Elija el año en el menú desplegable para filtrar los pagos liberados en ese año.
- **Pendiente** : próximos pagos.
- **Impuesto de la cuota de servicio (formulario pdf)** : disponible para los pagos que se someten a impuestos sobre la tarifa de servicio. Los impuestos de la cuota de servicio se muestran en **otros impuestos**.
- **Ver** : redirige al historial de transacciones con una lista de ganancias incluidas en el pago.

Para comprender por qué es posible que haya ganancias inesperadas o inesperadas, consulte [preguntas comunes sobre los pagos comerciales de Marketplace](payout-faq.md#why-are-my-earnings-missing).

### <a name="payment-status"></a>Estado del pago.

En la tabla siguiente se explican los distintos Estados de la ganancia.

| Estado de la ganancia | Motivo | ¿Se requiere una acción del asociado? |
| --- | --- | --- |
| Sin procesar | La ganancia es válida para el pago. Permanece en este estado durante un período de enfriamiento, tal y como se define en la guía de programas para el programa incentivos. | No |
| Próximamente | El pedido de pago generó revisiones internas pendientes antes de que se procese el pago. | No |
| Factura de impuestos pendiente | La factura de impuestos está incompleta o no es válida. | Debe actualizar su factura de impuestos antes de recibir el pago. |
| Rechazado durante la revisión | Se rechazó el pago durante la revisión. | Para obtener información, póngase en contacto con el servicio de soporte técnico de Microsoft. |
| Con error | No se pudo realizar el pago debido a un error del sistema de Microsoft. | Póngase en contacto con el soporte técnico de Microsoft para obtener detalles |
| En curso | El pago está en curso. | No |
| Pago incorrecto | La regresión del pago está en curso. | No |
| Enviado | El pago se ha enviado al banco. | No |
| Reprocesamiento | El pago encontró un error del sistema de Microsoft y se está reprocesando. | No |
| Reversed | El banco invirtió el pago y se enviará de nuevo en el siguiente ciclo de pago. | No |
| Factura de impuestos rechazada | Se rechazó su factura de impuestos durante la revisión. Todos los pagos pendientes se pondrán en espera hasta que se complete la revisión de la factura de impuestos. | Póngase en contacto con el soporte técnico de Microsoft para obtener detalles |
| Factura de impuestos en revisión | Se está revisando su factura de impuestos. El pago se publicará una vez que se haya aprobado la factura de impuestos. | No |
| Rechazada | El Banco rechazó el pago. | Póngase en contacto con su banco para obtener información. |
|

### <a name="payments-download"></a>Descarga de pagos

Para ver más detalles sobre los pagos, seleccione **Descargar** en la parte superior de la página. En la tabla siguiente se explica cada columna del informe.

| Nombre de la columna | Descripción |
| --- | --- |
| participantID | Identidad principal del asociado que gana con el programa. |
| participantIDType | Normalmente, el ID. de programa para los programas de incentivos y el identificador de vendedor para los programas de tienda |
| participantName | Nombre del asociado que gana. |
| programName | Incentivos/nombre del programa de tienda |
| earned | Importe obtenido en la moneda del destinatario del pago para ese programa/participantID. |
| earnedUSD | Importe obtenido para el programa/identificador de participante, en dólares estadounidenses. |
| withheldTax | Importe de los impuestos retenidos en la moneda del destinatario del pago para el programa/participantID. |
| salesTax | Importe total del impuesto de ventas en el pago por moneda para el programa/participantID (aplicable solo a los programas de incentivos) |
| serviceFeeTax | Importe total de serviceFeeTax en la moneda del destinatario del pago para el programa/participantID (aplicable solo para programas de la Tienda y Azure Marketplace). |
| totalPayment | Pago total en la moneda local que excluye la retención de impuestos e incluye el impuesto sobre las ventas (si es necesario) para el programa/participantID. |
| currencyCode | Código de la moneda del destinatario del pago. |
| paymentMethod | El método que se usa para pagar al asociado, como, por ejemplo, transferencia bancaria electrónica o nota de crédito. |
| paymentID | Identificador único del pago. Este número suele aparecer en el extracto del banco (aplicable solo para pagos de SAP). |
| paymentStatus | Estado del pago. |
| paymentStatusDescription | Descripción detallada del estado del pago. |
| paymentDate | Fecha en que Microsoft envió el pago. |
|

## <a name="export-data"></a>Exportar datos

La página **exportar datos** no se actualiza por sí misma. Es posible que tenga que actualizar la página manualmente para ver los datos más recientes. Seleccione una de las tres pestañas para exportar el **historial de transacciones**, los **pagos**, el **Resumen de transacciones**o la **instrucción histórica**.

El filtro podría producir un error **no hay datos disponibles** . Esto puede ocurrir si se deja el período de tiempo predeterminado seleccionado en tres meses y después se selecciona un ID. de pago de una ganancia que está fuera de ese período. Si esto ocurre, expanda el período de tiempo y vuelva a intentarlo.

A continuación se muestra un ejemplo de exportación de pagos:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Informe de los pagos exportados.":::

### <a name="historical-statements"></a>Extractos históricos

El Resumen **exportar datos** también proporciona acceso a las instrucciones históricas.

> [!NOTE]
> Una instrucción histórica es una instantánea y no se actualiza. Póngase en contacto [con el soporte técnico](https://partner.microsoft.com/support/v2/?stage=1) y solicite los datos más recientes, si es necesario.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Exportar instrucciones históricas.":::

- El historial de transacciones desde antes del 1 de julio de 2019 se administra por separado y usa distintos campos de informes de historial posteriores.
- El historial de transacciones heredadas tiene una columna denominada "reservada" que corresponde a la columna "beneficios" del historial moderno, con la salvedad de que excluye todas las ganancias cuyo estado es "pago enviado".
- Filtros como 3 M, 6 M o 12 M no se aplicarán a la sección Extractos históricos.

### <a name="historical-statement-downloads"></a>Descargas de instrucciones históricas

En la tabla siguiente se explica cada columna de una instrucción histórica.

| Nombre del campo | Descripción |
| --- | --- |
| Origen de ingresos | El origen de los ingresos en función de dónde se ha producido la transacción, como, por ejemplo, Microsoft Store, la Tienda Windows Phone, la Tienda Windows 8 o publicidad. |
| Identificador del pedido | Identificador único del pedido. Este identificador permite identificar las transacciones de compra con sus transacciones que no son de compra correspondientes, como, por ejemplo, reembolsos o contracargos. El identificador del pedido será el mismo en ambos casos. Además, si hay un cargo dividido en el que se usaron varios métodos de pago para una sola compra, le permite vincular las transacciones de compra. |
| Transaction ID | Identificador único de la transacción. |
| Fecha y hora de la transacción | La fecha y la hora de la transacción (UTC). |
| Id. del producto principal | Identificador único del producto principal. Si no hay un producto principal para la transacción, el identificador del producto principal es igual al identificador del producto. |
| Product ID | Identificador único del producto. |
| Nombre del producto principal | Nombre del producto principal. Si no hay un producto principal para la transacción, el nombre del producto principal es igual al nombre del producto. |
| Nombre de producto | Nombre del producto. |
| Tipo de producto | Tipo de producto, como, por ejemplo, aplicación, complemento o juego. |
| Cantidad | Cuando el origen de ingresos es Microsoft Store para Empresas, la cantidad representa el número de licencias adquiridas. En el caso del resto de orígenes de ingresos, la cantidad siempre será 1. Incluso cuando una sola transacción se divida en dos elementos de línea al haberse usado dos métodos de pago diferentes, la cantidad de cada elemento de línea será 1. |
| Tipo de transacción | Tipo de transacción, como, por ejemplo, compra, reembolso, revocación o contracargo. |
| Método de pago | Instrumento de pago del cliente usado para la transacción, como, por ejemplo, tarjeta, facturación del operador móvil o PayPal. |
| País o región | País o región donde se ha producido la transacción. |
| Proveedor o vendedor local | Proveedor o vendedor local del registro. |
| Moneda de transacción | Moneda de la transacción. |
| Importe de transacción | Importe de la transacción. |
| Impuestos remitidos | Importe del impuesto remitido (ventas, uso o impuestos de IVA/GST). |
| Recibos netos | Importe de la transacción menos el impuesto remitido. |
| Honorarios de la Tienda | El porcentaje de recibos netos retenido por Microsoft como honorarios por hacer que la aplicación o el complemento estén disponibles en la Tienda. |
| Ganancias por la aplicación | Recibos netos menos los honorarios de la Tienda. |
| Impuestos retenidos | Importe de los impuestos retenidos (no se incluye en el archivo CSV **Reserved**). |
| Payment | Ganancias por la aplicación menos la retención de impuestos aplicable (el importe se muestra en la moneda de la transacción). No se incluye en el archivo CSV **Reserved**. |
| Tipo de cambio | Tipo de cambio usado para convertir la moneda de la transacción a la moneda del pago. |
| Moneda del pago | Moneda en la que se realiza el pago. |
| Pago convertido | Importe del pago convertido a la moneda del pago mediante el tipo de cambio. |
| Modelo de remisión de impuestos | Entidad responsable de la emisión de impuestos (ventas, uso o impuestos de IVA/GST). |
| Fecha y hora de la idoneidad | La fecha y la hora en que las ganancias por la transacción se vuelven aptas para el pago (UTC). Cuando se crea un pago, incluye ganancias por la transacción con una fecha y hora de la idoneidad anterior a la fecha de creación del pago (solo se incluye en el archivo CSV **Reserved**). |
| Charges | Muestra un desglose de todos los detalles de los cargos agregados en la columna Importe de transacción (solo se incluye para Azure Marketplace; no se incluye en el archivo CSV **Reserved**). |
|||

## <a name="next-steps"></a>Pasos siguientes

- [API de pago de asociados](https://apidocs.microsoft.com/services/partnerpayouts)
- [Detalles de directiva de pagos](payout-policy-details.md)
- Para obtener soporte técnico sobre facturación, póngase en contacto con el [soporte técnico al editor](https://partner.microsoft.com/support/v2/?stage=1) en el marketplace comercial.