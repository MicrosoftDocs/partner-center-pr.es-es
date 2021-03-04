---
title: Procesos y programaciones de pagos
description: Obtenga información sobre los pagos y transacciones, como los planes de pago y los procesos de rerecuperación para el Marketplace comercial y otras transacciones.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 12/04/2020
ms.openlocfilehash: 9c4ad89eb25e811c4bea11e7e7e5d3845ceafee6
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756855"
---
# <a name="payout-schedules-and-processes"></a>Procesos y programaciones de pagos

**Roles adecuados:**

- Administrador de cuentas
- Administrador global

En este artículo se describe la programación de pago de Microsoft, dónde encontrar el estado de un pago y el proceso de no pago del cliente.

## <a name="payment-schedules"></a>Programaciones de pago

En las secciones siguientes se describe el proceso de pago de las transacciones de **contrato Enterprise** y de la **tarjeta de crédito/factura** .

### <a name="enterprise-agreement-transactions"></a>Transacciones de Contrato Enterprise

Cuando un cliente compra un producto desde Microsoft AppSource o Azure Marketplace usando su Contrato Enterprise de Microsoft actual para las transacciones, se emitirán pagos en el siguiente ciclo de pago 30 días después de la factura del cliente. Las transacciones en las que un cliente utiliza una tarjeta de crédito tienen un período de retención de 30 días antes del pago.

A menudo se producirá un pago antes de que Microsoft recopile el pago del cliente. Vea el [proceso de no pago](#process-for-customer-non-payment) a través de los clientes a continuación para las acciones que tomamos si el cliente no paga a Microsoft, pero ya hemos emitido un pago.

| Evento | Descripción | Visibilidad de informes | Agotamiento |
| --- | --- | --- | --- |
| Uso o mes de la transacción | El cliente usa o compra un servicio. | Panel [uso](/azure/marketplace/partner-center-portal/usage-dashboard) u [orden](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mes 1** |
| Microsoft calcula el importe de facturación | Determinar el uso total, total de transacciones | Panel [uso](/azure/marketplace/partner-center-portal/usage-dashboard) u [orden](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mes 2** |
| Pago registrado | Determinar el precio de la Agencia y los ingresos de pago | Marcado como no procesado en el historial de transacciones de la [instrucción de pago](payout-statement.md) | **Mes 3 (primera semana)** |
| Preparación del pago | Los ingresos están preparados para el pago mensual | Marcado como próximo en el historial de transacciones de la [instrucción de pago](payout-statement.md) | **Mes 3 (primera semana)** |
| **Pago enviado** | **El pago se envía al publicador** | **Marcado como enviado en el historial de transacciones y en la sección de pagos de la [instrucción de pago](payout-statement.md)** | **Mes 3 (no posterior al 15)** |
| Factura pagada por el cliente | Microsoft recopila el pago del cliente | Sin cambios | **Mes 4 a 12** |
|

\* La fecha de pago está en hora estándar del Pacífico (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Escala de tiempo de los pagos de los clientes con contrato Enterprise.":::

### <a name="transactions-with-credit-card-or-invoice-checkwire"></a>Transacciones con tarjeta de crédito o factura (comprobación/conexión)

Todas las compras con una tarjeta de crédito o una factura mensual tienen un período de retención de 30 días para garantizar que los fondos se recopilan del cliente.

| Evento | Descripción | Visibilidad de informes | Agotamiento |
| --- | --- | --- | --- |
| Uso o mes de la transacción | El cliente usa o compra un servicio. | Panel [uso](/azure/marketplace/partner-center-portal/usage-dashboard) u [orden](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mes 1** |
| Factura pagada por el cliente | Determinar el uso total, el valor total de la transacción y el cliente paga la factura | Panel [uso](/azure/marketplace/partner-center-portal/usage-dashboard) u [orden](/azure/marketplace/partner-center-portal/orders-dashboard) | **Mes 2** |
| Pago registrado | Determinar el precio de la Agencia y los ingresos de pago | Marcado como no procesado en el historial de transacciones de la [instrucción de pago](payout-statement.md) | **Mes 2** |
| período de retención de 30 días | Garantizar la recopilación de fondos, los posibles contracargos y las solicitudes de reembolso | Marcado como no procesado en el historial de transacciones de la [instrucción de pago](payout-statement.md) | **Mes 3** |
| Preparación del pago | Los ingresos están preparados para el pago mensual | Marcado como próximo en el historial de transacciones de la [instrucción de pago](payout-statement.md) | **Mes 4 (primera semana)** |
| **Pago enviado** | **El pago se envía al publicador** | **Marcado como enviado en el historial de transacciones y en la sección de pagos de la [instrucción de pago](payout-statement.md)** | **Mes 4 (no posterior al 15)** |
|

\* La fecha de pago está en hora estándar del Pacífico (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Escala de tiempo de los pagos de los clientes de la tarjeta de crédito y de la factura.":::

## <a name="process-for-customer-non-payment"></a>Proceso en caso de impago de los clientes

En raras ocasiones, Microsoft no puede cobrar los pagos a los clientes por sus compras en Marketplace comercial. Cuando un cliente no puede pagar a Microsoft según su programación de facturación, comienza el proceso de cobro. Este proceso tarda aproximadamente cuatro meses e implica una comunicación continua con Microsoft. Si al final de este proceso no se recibe el pago, Microsoft cancela los fondos y los considera no cobrados.

Según el proceso de pago articulado aquí, es posible que Microsoft ya haya pagado fondos a los anunciantes (usted) que finalmente no se podrán cobrar. Por lo tanto, tenemos un proceso para conciliar estos importes. Para asegurarse de que tiene la advertencia de que su pago (ya recibido) se puede conciliar, se le avisará cuando un cliente se encuentre en el proceso de cobro y es probable que se cancelen las compras.

Microsoft recuperará los pagos que ya se le hayan pagado a usted con uno de los siguientes métodos: (1) Microsoft puede restar los importes no pagados de los pagos futuros; por ejemplo, si se considera que 1000 dólares USA de los pagos no se pueden cobrar ni cancelar, se retienen los pagos futuros hasta que se recupere este importe; o bien, (2) Microsoft puede solicitar un reembolso o los importes no cobrados a los anunciantes de la factura.

A continuación, se muestra una programación de ejemplo:

| Evento | Fecha aproximada * | Visibilidad de los asociados |
| --- | --- | --- |
| Ejemplo de fecha de pago | 15/10/2020 | Se marca como **Enviado** en el historial de transacciones y en la sección de pagos del panel de pago. |
| <font color="red">Si el cliente no paga a Microsoft</font> | 2/12/2020 – 5/12/2020 | Sin cambios, igual que antes. |
| El cliente recibe el primer correo electrónico de pago atrasado. | 12/6/2020 | None |
| El cliente recibe mensajes de correo electrónico periódicos cada vez más urgentes. | 07/12/2020 – 31/01/2021 | None |
| Es probable que el anunciante reciba una notificación de una probable cancelación. | 07/01/2021 | Notificación por correo electrónico enviada al anunciante de que su cliente aún no ha enviado el pago. Se incluyen el identificador de la transacción y el importe en dólares. |
| El cliente recibe el aviso de cancelación. | 01/02/2021 | None |
| El proceso de cobro finaliza o los fondos se cancelan. | 15/02/2021 | Notificación por correo electrónico enviada al anunciante de que los fondos se han cancelado. Se incluyen el identificador de la transacción y el importe en dólares. |
| El pago se deduce. | 01/03/2021 | El publicador verá una transacción negativa en la declaración de pago del centro de Partners |
| El pago se retiene. | 15/03/2021 | Los pagos futuros se mostrarán en la declaración de pago del centro de Partners. El anunciante no recibirá ningún pago hasta que el saldo deje de ser negativo.  |
|||

\* La fecha de pago está en hora estándar del Pacífico (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Número de días para que los pagos lleguen a la cuenta de pago

Normalmente enviamos todos los pagos con vencimiento en un mes determinado a día 15 de ese mes, aunque el pago tardará más tiempo en llegar a su cuenta. El número de días depende del método de pago que usamos para su cuenta, como se describe a continuación.

> [!NOTE]
> Los días que se muestran a continuación son aproximados; cualquier pago puede tardar más o menos tiempo en llegar a su cuenta.

| Método de pago     | Número de días para que lleguen a la cuenta de pago     |
|--------------------|--------------------------------------------|
| PayPal             | 1 día laborable                             |
| ACH/SEPA           | 2 a 3 días laborables                          |
| Transferencia bancaria      | 7 a 10 días laborables                         |
|

## <a name="next-steps"></a>Pasos siguientes

- [Datos fiscales](tax-details-marketplace.md)
