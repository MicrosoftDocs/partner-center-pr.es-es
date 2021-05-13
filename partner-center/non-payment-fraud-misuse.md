---
title: Administración de los impagos, fraudes o usos incorrectos
description: Obtenga información sobre los distintos riesgos implicados en las transacciones en línea y los procedimientos recomendados para administrar y mitigar esos riesgos en Centro de partners.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 1d8e59ea2d2e8d40163ea06b305845c37a356f16
ms.sourcegitcommit: dc9438475ccc6298bec6a698bf5fc9bd5cf2aa81
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/12/2021
ms.locfileid: "109818667"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Administración de no pago, fraude o uso indebido en el Centro de partners

**Se aplica a**: Centro de partners | Centro de partners para Microsoft Cloud for US Government

**Roles adecuados:** administrador global | Administrador de administración de | Agente de administración | Administrador de facturación

Usted es responsable financieramente de las compras fraudulentas realizadas por sus clientes o por el impago de los servicios adquiridos. Por lo tanto, se recomienda encarecidamente que ponga en marcha controles de prevención de fraudes y *de mitigación de riesgos de detección.*

Para evitar y/o abordar la actividad fraudulenta o el uso indebido, es importante comprender los posibles riesgos y desarrollar directivas y prácticas que puedan reducir la exposición.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Cumplimiento de la directiva de uso aceptable de Microsoft

Si Microsoft detecta una actividad de asociado o cliente que confirmamos o sospechamos que infringe la directiva de uso aceptable, tomaremos medidas de cumplimiento. El cliente podría suspenderse inmediatamente. Microsoft le notificará de las acciones de cumplimiento o se le actualizará en las solicitudes.

## <a name="abuse-of-service-risks"></a>Abuso de los riesgos del servicio

**El uso indebido de** los riesgos del servicio significa que los clientes que usan servicios en la nube infringen la directiva de uso aceptable de Microsoft.

### <a name="examples-of-abuse-of-service"></a>Ejemplos de abuso de servicio

Entre los ejemplos de estas infracciones de la directiva de uso aceptable de Microsoft se incluyen:

- Spam
- Hacking
- Ataques de denegación de servicio distribuido (DDoS)
- Minería de datos de Bitón
- Distribución de malware
- Reventa de suscripciones pirateadas

## <a name="theft-of-service-risks"></a>Robo de riesgos de servicio

**El robo de riesgos** de servicio significa que los clientes que no tienen intención de pagar por los servicios consumidos. Este robo puede implicar el uso de instrumento de pago robados, proporcionar información de facturación falsa o el incumplimiento de saldos pendientes.

### <a name="examples-of-service-theft"></a>Ejemplos de robo de servicio

Algunos ejemplos de estos riesgos de transacción en línea pueden ser:

- Transacciones que no se producen en persona ("las transacciones de tarjeta de crédito no están presentes")
- Identidades mal representadas
- Servicios aprovisionados y usados antes de recibir el pago inicial
- Mercados emergentes o regiones de alto riesgo para fraudes en línea
- Automatización de la creación y compra de cuentas por parte de actores con problemas

## <a name="managing-online-risk"></a>Administración del riesgo en línea

Puede usar las siguientes recomendaciones para ayudarle a desarrollar directivas y prácticas para reducir la exposición a los riesgos de transacciones en línea en el ciclo de vida de las relaciones con los clientes.

### <a name="onboarding-new-customers"></a>Incorporación de nuevos clientes

Entre las sugerencias para reducir los riesgos en línea al incorporar nuevos clientes se incluyen:

- Establezca relaciones personales con los clientes cuando sea posible (por ejemplo, ponerse en contacto con los clientes por teléfono).
- Compruebe las credenciales y los antecedentes de los clientes mediante mejores métodos (como el uso de oficinas de crédito o agencias de informes comerciales empresariales).
- Use la autenticación multifactor (como la verificación por SMS) durante el registro para minimizar la exposición a la creación y compra de cuentas robóticas.
- Administrar y realizar un seguimiento de las identidades mediante servicios (como servicios de identidad digital).
- Evalúe la solidez financiera del cliente a través de sistemas de detección de fraudes de tarjetas de crédito rigurosos.
- Establezca una directiva de recopilaciones clara. Detalle del proceso de recopilación y cuándo se verá afectado el acceso a las suscripciones por impago. (Puede deshabilitar el acceso o [suspender las suscripciones](create-a-new-subscription.md#suspend-a-subscription) de un cliente por impago).

### <a name="managing-customer-accounts"></a>Administración de cuentas de clientes

Entre las sugerencias para administrar las cuentas de cliente después de la compra se incluyen:

- Implemente un proceso para recibir, revisar, actuar y responder rápidamente a las notificaciones de Microsoft.
- Trabaje con los clientes para comprender sus necesidades empresariales de uso de la nube al tiempo que se han configurado los umbrales de supervisión adecuados. (Por ejemplo, puede establecer [un presupuesto de gastos mensual](set-an-azure-spending-budget-for-your-customers.md) de Azure en Centro de partners. Este conocimiento le permite supervisar el uso de los clientes durante el mes y recibir notificaciones cuando los clientes estén cerca de su presupuesto).
- Supervise los [registros de actividad del cliente](activity-logs.md) con regularidad para ayudar a detectar fraudes pronto.
- Tome medidas rápidas cuando se detecten actividades sospechosas.
- Evite dar a los clientes acceso administrativo total a las suscripciones sin implementar primero controles de mitigación de riesgos.

### <a name="managing-customer-billing"></a>Administración de la facturación del cliente

Entre las sugerencias para administrar la facturación posterior a la compra del cliente se incluyen:

- Solicitar prepagos antes de las transacciones iniciales y la facturación.
- No acepte los instrumento de pago de alto riesgo (por ejemplo, tarjetas de pago previo o tarjetas de valor almacenado).
- Supervise los pagos de los clientes y las cuentas de vencimiento por cobrar. Aplique de forma agresiva procesos de reclamación estandarizados para pagos atrasados o impagos.

Para obtener estrategias más detalladas para mitigar el riesgo en línea, consulte la Guía de administración de riesgos [de transacciones en línea.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
