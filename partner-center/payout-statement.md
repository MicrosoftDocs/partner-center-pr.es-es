---
title: Extractos de pagos
description: Obtenga información sobre los extractos y resúmenes de pago y cómo ver y exportar los datos de pago de Microsoft Centro de partners
ms.subservice: partnercenter-marketplace-publisher
ms.service: marketplace
ms.topic: article
author: eunjkim520
ms.author: eunjkim
ms.date: 3/22/2021
ms.openlocfilehash: dc0c720544f4a8a3c95e5b91ec656e65dbce7c80
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276117"
---
# <a name="payout-statements"></a>Extractos de pagos

**Roles adecuados:** administrador de | Administrador global

El **extracto de pago** presenta información general de los pagos de las ofertas vendidas a través del marketplace comercial. Muestra el historial transaccional de las ganancias, calcula el siguiente pago y muestra las tendencias de pago. También puede descargar el historial de transacciones y los extractos de pago. En este artículo se explica cómo acceder a su extracto de pago y a las distintas páginas y descargas de pago a las que puede acceder Centro de partners.

>[!NOTE]
>Solo verá los datos de los IDs y programas de MPN a los que está asociado. Si desea ver datos adicionales, trabaje con el administrador de la cuenta para obtener permisos. 

## <a name="roles-and-permissions"></a>Roles y permisos

Para acceder a un extracto de pago, debe tener asignado el rol Propietario de **la** cuenta o Colaborador **financiero.**

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

## <a name="access-your-payout-statement"></a>Acceso al extracto de pago

Inicie sesión en [Centro de partners](https://partner.microsoft.com/dashboard/home) seleccione el icono de pago en la esquina superior derecha de la pantalla para acceder a estos resúmenes diferentes:

- Historial de transacciones
- Pagos
- Exportar datos

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Se muestra el icono Pago en la esquina superior derecha del portal del Centro de partners.":::

También puede usar partner [payout API](https://apidocs.microsoft.com/services/partnerpayouts) para conectarse y obtener datos de transacción y pago directamente.


## <a name="transaction-history"></a>Historial de transacciones

La **página Historial de** transacciones muestra el resumen de las ganancias, el próximo pago estimado y la tendencia de ganancias y pagos de los últimos 36 meses. También puede descargar los detalles de la transacción de esta sección.<br><br>En este informe se muestran todas las ganancias aptas para el pago, incluidos los pagos que aún no se han enviado. Las ganancias son aptas para el pago cuando un ISV ha completado toda la información bancaria y fiscal de Centro de partners, ha ganado >50 USD, la cuenta de ISV está activa y se ha facturado al cliente (para transacciones ea) o se ha recibido el pago (para transacciones que no son de EA).

:::image type="content" source="images/payouts/transaction-overview.png" alt-text="Introducción a la transacción.":::

- **Ganancias enviadas este año:** las ganancias totales y el desglose de las ganancias que se han pagado y se pagarán en el próximo mes.
- **Mes de pago estimado:** ganancias totales esperadas en los próximos meses.
- **Tendencia de ganancias y pago:** ganancias mensuales y importes de pago de los últimos 36 meses.
- **Descargar:** descargue los detalles de la transacción .csv o .tsv.

Use la selección de intervalo de fechas en la esquina superior derecha de la página para filtrar la salida de la página para mostrar los últimos 3, 6, 12 o 36 meses. O bien, seleccione un intervalo de fechas personalizado de hasta 36 meses. El intervalo de fechas predeterminado es de 12 meses. También puede filtrar por identificador de inscripción, programa, identificador de pago, tipo de ganancia, maneta y estado. Los datos están disponibles para el año fiscal actual (del 1 de julio al 30 de junio) y los dos años fiscales anteriores.

:::image type="content" source="images/payouts/search-filter.png" alt-text="Filtro de búsqueda en la parte superior derecha de la página.":::

Para ver más detalles sobre una ganancia, seleccione la flecha abajo que se encuentra en el lado derecho de la página. Si lo hace, se mostrará el beneficio, el importe de los ingresos, el producto y el cliente. Si por algún motivo alguno de estos datos no está disponible, pero necesita acceder a ellos, póngase en contacto con el soporte técnico. Si la ganancia es el resultado de un ajuste y no de una transacción, no se mostrarán los campos Producto y Cliente.

### <a name="transaction-history-summary"></a>Resumen del historial de transacciones

Esta vista muestra los detalles de la ganancia, incluido el origen de la ganancia de las fechas de ganancias de ventas del producto, el estado y el mes de pago estimado.

:::image type="content" source="images/payouts/transaction-history.png" alt-text="Historial de transacciones.":::

- **Fecha de adquisición:** la fecha de compra.
- **Tipo de ganancia:** el tipo de ganancia, como Venta, Reembolso o Cooperación.
- **Importe total:** el importe neto de la ganancia. En el marketplace comercial, esto significa después de deducir la tarifa estándar de Marketplace.
- **Estado:** tiene tres opciones:
    - **Próximamente:** las ganancias están en un período de refrigeración pendiente.
    - **Procesado: las** ganancias se preparan para el siguiente pago.
    - **Enviado:** se han pagado las ganancias.
- **Mes de pago estimado:** mes en el que se espera que se paguen las ganancias. Consulte la [sección siguiente](#estimated-payment-month) para obtener más información.

Las transacciones de ganancias se muestran una vez que la transacción cumple los requisitos de pago. Para entender por qué puede que le falten ganancias o inesperadas, consulte [Preguntas comunes sobre los pagos del marketplace comercial.](payout-faq.md#why-are-my-earnings-missing)

#### <a name="estimated-payment-month"></a>Mes de pago estimado

La página Historial de transacciones ahora incluye una tabla que muestra los importes de pago estimados para los próximos meses. También puede ver y descargar esta información en las exportaciones del historial de transacciones y del informe Resumen. Esta información facilita las conciliaciones y las proyecciones de pago.

El mes de pago estimado se calcula en función de las reglas de configuración del programa y las escalas de tiempo, y se procesa en el siguiente ciclo de pago o en el próximo.

El mes de pago estimado está disponible actualmente para todos los tipos de ganancias, excepto la cooperación, que se mostrará como **No aplicable.** Para las ganancias anteriores al 1 de julio de 2020, el mes de pago estimado aparecerá **como No disponible.**

En la tabla siguiente se muestra un ejemplo de mes de pago estimado.

| Month (Mes) | Amount |
| ------ | :-----------: |
|  Sep-2020 |  7 273,99 USD   |
|  Octubre de 2020 | 8692,30 USD  |
|  Noviembre de 2020 | 107,89 USD  |

La cantidad estimada puede variar de la cantidad real por diversos motivos:

- Reestado de ganancias: si se vuelven a calcular las ganancias, el importe real será diferente.
- Ajustes: la cantidad real varía en función de los ajustes que se produjeron o se enviaron.
- Cambio de reglas: un cambio en las reglas puede reflejar el recálculo en el importe real pagado
- Pago por pagar: si se produce un error de pago, el importe real podría ser diferente.

Tenga en cuenta que el pago solo se libera en el mes proyectado si se cumplen las reglas de elegibilidad de pago y el umbral del programa. Estas reglas incluyen, entre otras, la lista siguiente:

- El perfil fiscal debe estar actualizado
- Las ganancias deben cumplir o superar el umbral mínimo de ganancia definido en la guía del programa.
- Pago en espera: si selecciona la opción "Mantener mi pago" en la página de asignación de perfiles.
- Instrumento de pago no disponible: el perfil de pago o de impuestos no se ha completado.

### <a name="transaction-history-download"></a>Descarga del historial de transacciones

Para ver más detalles sobre una ganancia, seleccione **Descargar** en la parte superior de la página. En la tabla siguiente se explica cada columna del informe.

>[!NOTE]
>La exportación de descarga del historial de transacciones tiene dos nuevos campos a partir de agosto de 2020:
>
>- **lastPaymentCurrency**  Moneda en la que se recibió el pago más reciente, en todos los MPN a los que tiene acceso el asociado que ha iniciado sesión actualmente. Si no se recibe ningún pago, la última moneda de pago será dólares estadounidenses.
>- **earningAmountInLastPaymentCurrency**  Importe de la ganancia en la moneda del último pago.

| Nombre de la columna | Descripción | Aplicabilidad para programas de incentivos o marketplaces |
| --- | --- | --- |
| agreementEndDate | Fecha de finalización del acuerdo. | Incentivos: solo algunos programas |
| agreementNumber | Número de acuerdo. | Incentivos: solo algunos programas |
| agreementStartDate | Fecha de inicio del acuerdo. | Incentivos: solo algunos programas |
| calculationDate | Fecha en que se calculó la ganancia en el sistema. | All |
| claimId | Identificador único de una notificación. | Incentivos: solo algunos programas |
| customerCountry | País o región del cliente. | marketplaces |
| customerEmail |  |  |
| customerName | Puede estar en blanco | Programas de incentivos solo (excepción: OEM) y marketplaces. En el caso de las transacciones de CSP, marketplaces mostrará el nombre del CSP. |
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
| externalReferenceId | Identificador único del programa. | Programas de pago directo (incentivos y marketplaces) |
| externalReferenceIdLabel | Etiqueta del identificador único. | Programas de pago directo (incentivos y marketplaces) |
| instantRebateAmount |  |  |
| invoiceDate |  |  |
| invoiceNumber | Número de factura (aplicable solo para empresas) | Incentivos y marketplaces: solo algunos programas |
| lastPaymentCurrency | Moneda del último pago (el campo estará vacío si no ha habido ningún pago anterior). |  |
| lever | Indica la regla de negocios de la ganancia. | All |
| LicensingProgramName | Nombre del programa de licencias. |  |
| LineItemId | Línea individual en la factura de un cliente. |  |
| localProviderSeller | Proveedor o vendedor local del registro. |  |
| Mes de madurez | Mes de pago estimado | Todo |
| OrderId | Se relaciona con la factura de un cliente.  | marketplaces |
| parentProductId | Identificador único del producto principal. Si no hay un producto principal para la transacción, el identificador del producto principal es igual al identificador del producto. | marketplaces |
| parentProductName | Nombre del producto principal. Si no hay un producto principal para la transacción, el nombre del producto principal es igual al nombre del producto. | marketplaces |
| participantId | Identidad principal del asociado que gana con el programa. | All |
| participantIdType | Identificador de programa principalmente para programas de incentivos y Seller IF para marketplaces | All |
| participantName | Nombre del asociado que gana. | All |
| partnerCountryCode | Ubicación, país o región del asociado que gana. | All |
| partNumber | Siempre estará en blanco. | Algunos programas de incentivos y marketplaces |
| paymentId | Identificador único para correlacionar todas las transacciones del informe de transacciones con un pago específico en el informe de pago | Todo |
| paymentStatus | Estado del pago. | All |
| paymentStatusDescription | Descripción detallada del estado del pago. | All |
| productId | Identificador único del producto. | marketplaces |
| ProductName | Nombre del producto vinculado a la transacción. | Todo |
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
| tpan | Indica la red de anuncios de terceros. | Solo anuncios de marketplaces |
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

### <a name="transaction-adjustment-codes"></a>Códigos de ajuste de transacción

En la tabla siguiente se enumeran los códigos de motivo para los ajustes y sus descripciones.

|**Código de motivo**   |**Descripción**   |
|------------------|:-------------------------------------|
| Cumplimiento de AR | Ajuste que reduce las ganancias cuando el partner no paga las facturas de Microsoft a tiempo. |
| Suversión de cooperación | Ajuste que transfiere las ganancias de cooperación a otro período o convierte las ganancias de cooperación en ganancias. |
| Ajuste de operaciones | Ajuste que corrige los errores de cálculo del sistema de Microsoft. |
| Cálculo incorrecto de Ajuste de operaciones de Microsoft | Ajuste que corrige cálculos erróneos. |
| Ajuste de operaciones Inscripción incorrecta de Microsoft | Ajuste de cálculos erróneos relacionados con la inscripción. |
| MCI/CSP de asignación de asociados (suscripción) | Ajuste que corrige el desajuste de la suscripción. |
| Excepción de directiva | Ajuste que invalida una regla de programa.  |
| Ganancias del período anterior | Ajuste de ganancias fuera del período de ganancias actual. |

## <a name="payments"></a>Pagos

En **la página** Pagos se detalla el dinero que ha ganado con Microsoft. También muestra cuándo y cuánto se le pagará.

>[!Note]
> Para poder acceder a esta opción, sus ganancias deben alcanzar el [umbral de pago](payment-thresholds-methods-timeframes.md) de 50 USD. Para obtener más información, vea El [Contrato del publicador de Microsoft](/legal/marketplace/msft-publisher-agreement).

:::image type="content" source="images/payouts/payments-overview.png" alt-text="Pantalla de información general de pagos.":::

- **Total pagado este año:** el total combinado que se le ha pagado este año, en dólares estadounidenses, para todos los programas.
- **Siguiente pago estimado:** el siguiente pago único que le llega (aunque pronto haya otros), en dólares estadounidenses.
- **Último pago:** el importe (en dólares estadounidenses), el nombre del programa y el programa del pago más reciente.
- **Pago por origen:** cantidad de pagos (en dólares estadounidenses) por programa durante los últimos 12 meses.

### <a name="payments-list"></a>Lista de pagos

La **tabla Lista de pagos** muestra los pagos pagados y pendientes. Puede descargar la información fiscal de los honorarios del servicio en formato PDF y ver los detalles de ganancias de un pago determinado.

:::image type="content" source="images/payouts/list-of-payments.png" alt-text="Exportar historial de transacciones.":::

- **Pagado:** todos los pagos enviados correctamente. Elija el año en el menú desplegable para filtrar por los pagos publicados en ese año.
- **Pendiente:** próximos pagos.
- **Impuesto sobre los honorarios del servicio (formulario PDF):** disponible para los pagos sujetos a impuestos sobre los honorarios del servicio. Los impuestos de tarifas de servicio se muestran **en Otros impuestos.**
- **Ver:** redirige al historial de transacciones con una lista de ganancias incluidas en el pago.

Para entender por qué puede que le falten ganancias o inesperadas, consulte [Preguntas comunes sobre los pagos del marketplace comercial.](payout-faq.md#why-are-my-earnings-missing)

### <a name="payment-status"></a>Estado del pago.

En la tabla siguiente se explican los distintos estados de ganancia.

| Estado de la ganancia | Motivo | ¿Se requiere una acción del asociado? |
| --- | --- | --- |
| Sin procesar | La ganancia es válida para el pago. Permanece en este estado durante un período de refrigeración, tal como se define en la guía del programa para el Programa Incentivos. | No |
| Próximamente | El pedido de pago generó revisiones internas pendientes antes de procesar el pago. | No |
| Factura de impuestos pendiente | La factura fiscal está incompleta o no es válida. | Debe actualizar su factura de impuestos antes de recibir el pago. |
| Rechazado durante la revisión | El pago se rechazó durante la revisión. | Para obtener información, póngase en contacto con el servicio de soporte técnico de Microsoft. |
| Con error | Error en el pago debido a un error del sistema de Microsoft. | Póngase en contacto con el soporte técnico de Microsoft para obtener más información. |
| En curso | El pago está en curso. | No |
| Pago incorrecto | La recuperación del pago está en curso. | No |
| Enviado | El pago se ha enviado al banco. | No |
| Reprocesamiento | El pago encontró un error del sistema de Microsoft y se está reprocesado. | No |
| Reversed | El banco revirtió el pago y se enviará de nuevo en el siguiente ciclo de pago. | No |
| Factura de impuestos rechazada | Se rechazó su factura de impuestos durante la revisión. Todos los pagos pendientes se pondrán en espera hasta que se complete la revisión de la factura de impuestos. | Póngase en contacto con el soporte técnico de Microsoft para obtener más información. |
| Factura de impuestos en revisión | Se está revisando su factura de impuestos. El pago se publicará una vez que se haya aprobado la factura de impuestos. | No |
| Rechazada | El banco rechazó el pago. | Póngase en contacto con su banco para obtener información. |
|

### <a name="payments-download"></a>Descarga de pagos

 En la tabla siguiente se explica cada columna del informe. Para ver más detalles sobre los pagos, seleccione **Descargar en** la parte superior de la página Pagos.

| Nombre de la columna | Descripción |
| --- | --- |
| participantID | Identidad principal del asociado que gana con el programa. |
| participantIDType | Normalmente, el identificador del programa para los programas de incentivos y el identificador de vendedor para los programas de la Tienda |
| participantName | Nombre del asociado que gana. |
| programName | Nombre del programa de incentivos/tienda |
| earned | Importe obtenido en la moneda del destinatario del pago para ese programa/participantID. |
| earnedUSD | Importe obtenido para el programa/identificador de participante, en dólares estadounidenses. |
| withheldTax | Importe de los impuestos retenidos en la moneda del destinatario del pago para el programa/participantID. |
| salesTax | Importe total de los impuestos de ventas en la moneda de pago a para el programa o participantID (aplicable solo para programas de incentivos) |
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

La **página Exportar** datos no se actualiza por sí sola. Es posible que tenga que actualizar la página manualmente para ver los datos más recientes. Seleccione una de las tres pestañas para exportar **el** historial de transacciones, **pagos,** **resumen de transacciones** o **instrucción histórica.**

El filtro podría producir un error **No hay datos disponibles.** Esto puede ocurrir si deja el período de tiempo predeterminado seleccionado en tres meses y, a continuación, selecciona un identificador de pago de una ganancia que está fuera de ese período. Si esto sucede, expanda el período de tiempo e inténtelo de nuevo.

Esta es una exportación de pagos de ejemplo:

:::image type="content" source="images/payouts/pc-export-payments.png" alt-text="Exportar informe de pagos.":::

### <a name="historical-statements"></a>Extractos históricos

El **resumen Exportar** datos también proporciona acceso a las instrucciones históricas.

> [!NOTE]
> Una instrucción histórica es una instantánea y no se actualiza. Póngase en contacto [con el soporte](https://partner.microsoft.com/support/v2/?stage=1) técnico y solicite los datos más recientes si es necesario.

:::image type="content" source="images/payouts/pc-export-statements.png" alt-text="Exportar instrucciones históricas.":::

- El historial de transacciones anterior al 1 de julio de 2019 se controla por separado y usa campos diferentes de los informes de historial posteriores.
- El historial de transacciones heredadas tiene una columna denominada "Reservado" que corresponde a la columna "Ganancias" del historial moderno, salvo que excluye todas las ganancias con un estado igual a "Pago enviado".
- Filtros como 3 M, 6 M o 12 M no se aplicarán a la sección Extractos históricos.

### <a name="historical-statement-downloads"></a>Descargas de instrucciones históricas

En la tabla siguiente se explica cada columna de una instrucción histórica.

| Nombre del campo | Descripción |
| --- | --- |
| Origen de ingresos | El origen de los ingresos en función de dónde se ha producido la transacción, como, por ejemplo, Microsoft Store, la Tienda Windows Phone, la Tienda Windows 8 o publicidad. |
| Identificador del pedido | Identificador único del pedido. Este identificador permite identificar las transacciones de compra con sus transacciones que no son de compra correspondientes, como, por ejemplo, reembolsos o contracargos. El identificador del pedido será el mismo en ambos casos. Además, si hay un cargo dividido en el que se usaron varios métodos de pago para una sola compra, permite vincular las transacciones de compra. |
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

- [Partner Payout API](https://apidocs.microsoft.com/services/partnerpayouts)
- [Detalles de directiva de pagos](payout-policy-details.md)
- Para obtener soporte técnico sobre facturación, póngase en contacto con el [soporte técnico al editor](https://partner.microsoft.com/support/v2/?stage=1) en el marketplace comercial.