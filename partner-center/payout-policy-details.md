---
title: Procesos y programaciones de pagos
description: Obtenga información sobre pagos y transacciones, como programaciones de pago y procesos de recuperación para Azure Marketplace y otras transacciones.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
author: eunjkim520
ms.author: eunjkim
ms.date: 05/25/2021
ms.openlocfilehash: bcecd4c31d80a4130331c652491e7951af180c67
ms.sourcegitcommit: f1255fb65eac6ee2e0ff0cb95cc16a02dc57fc1a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/27/2021
ms.locfileid: "110582430"
---
# <a name="payout-schedules-and-processes"></a>Procesos y programaciones de pagos

**Roles adecuados:** Administrador de | Administrador global

En este artículo se describe la programación de pago de Microsoft, dónde encontrar el estado de un pago y el proceso de impago del cliente.

## <a name="payment-schedules"></a>Programaciones de pago

En las secciones siguientes se describe el proceso de pago **para Contrato Enterprise** transacciones Contrato de cliente de Microsoft **o CSP.**

### <a name="transactions-when-customer-has-an-enterprise-agreement"></a>Transacciones cuando el cliente tiene una Contrato Enterprise

Cuando un cliente compra un producto de Microsoft AppSource o Azure Marketplace mediante su microsoft Contrato Enterprise existente para transacciones, emitiremos pagos en el siguiente ciclo de pago 30 días después de la factura del cliente. Las transacciones en las que un cliente usa una tarjeta de crédito tienen un período de retención de 30 días antes del pago.

A menudo se producirá un pago antes de que Microsoft recopile el pago del cliente. Consulte [Proceso de impago](#process-for-customer-non-payment) del cliente a continuación para conocer las acciones que se llevan a cabo si el cliente no puede pagar a Microsoft, pero ya hemos emitido un pago.

| Evento | Descripción | Visibilidad de informes | Tiempo* |
| --- | --- | --- | --- |
| Uso o mes de transacción | El cliente usa o compra un servicio. | [Panel de](/azure/marketplace/partner-center-portal/usage-dashboard) uso [u](/azure/marketplace/partner-center-portal/orders-dashboard) pedido | **Mes 1** |
| Microsoft calcula el importe de facturación | Determinación del uso total, total de transacciones | [Panel de](/azure/marketplace/partner-center-portal/usage-dashboard) uso [u](/azure/marketplace/partner-center-portal/orders-dashboard) pedido | **Mes 2** |
| Pago publicado | Determinación de la cuota de la agencia y las ganancias de pago | Marcado como Sin procesar en el historial de transacciones en el [extracto de pago](payout-statement.md) | **Mes 3 (primera semana)** |
| Preparación del pago | Las ganancias se preparan para el pago mensual | Marcado como Próximo en el historial de transacciones en el [extracto de pago](payout-statement.md) | **Mes 3 (primera semana)** |
| **Pago enviado** | **El pago se envía al publicador** | **Marcado como Enviado en el historial de transacciones y en la sección Pagos del [extracto de pago](payout-statement.md)** | **Mes 3 (no posterior al 15)** |
| Factura pagada por el cliente | Microsoft recopila el pago del cliente | Sin cambios | **Mes 4 a 12** |
|

\* La fecha de pago está en hora estándar del Pacífico (PST).

:::image type="content" source="images/payouts/timeline-enterprise.png" alt-text="Escala de tiempo de los pagos para los clientes del contrato Enterprise.":::

### <a name="transactions-when-customer-has-a-microsoft-customer-agreement-or-csp"></a>Transacciones cuando el cliente tiene un Contrato de cliente de Microsoft o CSP

Todas las compras con una tarjeta de crédito o una factura mensual tienen un período de retención de 30 días para asegurarse de que los fondos se recopilan del cliente.

| Evento | Descripción | Visibilidad de informes | Tiempo* |
| --- | --- | --- | --- |
| Uso o mes de transacción | El cliente usa o compra un servicio. | [Panel de](/azure/marketplace/partner-center-portal/usage-dashboard) uso [u](/azure/marketplace/partner-center-portal/orders-dashboard) pedido | **Mes 1** |
| Factura pagada por el cliente | Determinación del uso total, el valor total de la transacción y el cliente paga la factura | [Panel de](/azure/marketplace/partner-center-portal/usage-dashboard) uso [u](/azure/marketplace/partner-center-portal/orders-dashboard) pedido | **Mes 2** |
| Pago publicado | Determinación de los honorarios de la agencia y las ganancias de pago | Marcado como Sin procesar en el historial de transacciones en el [extracto de pago](payout-statement.md) | **Mes 2** |
| Período de retención de 30 días | Garantizar la recopilación de fondos, posibles contra reembolsos y solicitudes de reembolso | Marcado como Sin procesar en el historial de transacciones en el [extracto de pago](payout-statement.md) | **Mes 3** |
| Preparación del pago | Las ganancias se preparan para el pago mensual | Marcado como Próximo en el historial de transacciones en el [extracto de pago](payout-statement.md) | **Mes 4 (primera semana)** |
| **Pago enviado** | **El pago se envía al publicador** | **Marcado como Enviado en el historial de transacciones y en la sección Pagos del [extracto de pago](payout-statement.md)** | **Mes 4 (no posterior al 15)** |
|

\* La fecha de pago está en hora estándar del Pacífico (PST).

:::image type="content" source="images/payouts/timeline-credit-card-invoice.png" alt-text="Escala de tiempo de pagos para clientes con tarjeta de crédito y factura.":::

## <a name="process-for-customer-non-payment"></a>Proceso en caso de impago de los clientes

En raras ocasiones, Microsoft no puede cobrar los pagos a los clientes por sus compras en Marketplace comercial. Cuando un cliente no puede pagar a Microsoft según su programación de facturación, comienza el proceso de cobro. Este proceso tarda aproximadamente cuatro meses e implica una comunicación continua con Microsoft. Si el pago no se recibe al final de este proceso, Microsoft escribe los fondos como no recuperables.

Según el proceso de pago articulado aquí, es posible que Microsoft ya haya pagado fondos a los anunciantes (usted) que finalmente no se podrán cobrar. Por lo tanto, tenemos un proceso para conciliar estos importes.

Microsoft recuperará los pagos que ya se le hayan pagado a usted con uno de los siguientes métodos: (1) Microsoft puede restar los importes no pagados de los pagos futuros; por ejemplo, si se considera que 1000 dólares USA de los pagos no se pueden cobrar ni cancelar, se retienen los pagos futuros hasta que se recupere este importe; o bien, (2) Microsoft puede solicitar un reembolso o los importes no cobrados a los anunciantes de la factura.

La siguiente programación es un ejemplo:

| Evento | Fecha aproximada* | Visibilidad de los asociados |
| --- | --- | --- |
| Ejemplo de fecha de pago | 15/10/2020 | Se marca como **Enviado** en el historial de transacciones y en la sección de pagos del panel de pago. |
| <font color="red">Si el cliente no paga a Microsoft</font> | 2/12/2020 – 5/12/2020 | Sin cambios, igual que antes. |
| El cliente recibe el primer correo electrónico de pago atrasado. | 12/6/2020 | None |
| El cliente recibe mensajes de correo electrónico periódicos cada vez más urgentes. | 07/12/2020 – 31/01/2021 | None |
| Es probable que el anunciante reciba una notificación de una probable cancelación. | 07/01/2021 | - |
| El cliente recibe el aviso de cancelación. | 01/02/2021 | None |
| El proceso de cobro finaliza o los fondos se cancelan. | 15/02/2021 | Notificación por correo electrónico enviada al anunciante de que los fondos se han cancelado. |
| El pago se deduce. | 01/03/2021 | El publicador verá una transacción negativa en Centro de partners de pago |
| El pago se retiene. | 15/03/2021 | Los pagos futuros se mostrarán en Centro de partners de pago. El anunciante no recibirá ningún pago hasta que el saldo deje de ser negativo.  |
|||

\* La fecha de pago está en hora estándar del Pacífico (PST).

## <a name="number-of-days-for-payments-to-reach-a-payout-account"></a>Número de días para que los pagos lleguen a la cuenta de pago

Normalmente, se envía cualquier pago que se deba en un mes determinado el día 15 de ese mes, pero el pago tarda otro tiempo en llegar a su cuenta. El número de días depende del método de pago que usemos para su cuenta, como se describe a continuación.

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
