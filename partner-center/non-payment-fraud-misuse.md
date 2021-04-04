---
title: Administración de los impagos, fraudes o usos incorrectos
description: Obtenga información acerca de los diversos riesgos implicados en las transacciones en línea y los procedimientos recomendados para administrar y mitigar estos riesgos en el centro de Partners.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 07/14/2020
ms.openlocfilehash: 75881544097abdfac8d6f96bde37e9700eb28cf7
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132356"
---
# <a name="managing-non-payment-fraud-or-misuse-in-partner-center"></a>Administración de no pago, fraude o uso indebido en el Centro de partners

Se aplica a:

- Centro de partners para la nube de Microsoft Government

**Roles adecuados**

- Administrador global
- Administrador del control de usuarios
- Agente de administrador
- Administrador de facturación

Usted es responsable financieramente de las compras fraudulentas por parte de los clientes y/o el no pago de los servicios adquiridos. Por lo tanto, *se recomienda encarecidamente que ponga en marcha la prevención de fraudes y los controles de mitigación de riesgos de detección*.

Para evitar o tratar la actividad fraudulenta o el uso indebido, es importante comprender los posibles riesgos y desarrollar directivas y prácticas que puedan reducir su exposición.

## <a name="enforcement-of-microsoft-acceptable-use-policy"></a>Aplicación de la Directiva de uso aceptable de Microsoft

Si Microsoft detecta que la actividad de los clientes o asociados que confirmamos o sospechas infringe la Directiva de uso aceptable, se llevará a cabo los pasos de cumplimiento. El cliente podría suspenderse inmediatamente. Microsoft le notificará las acciones de aplicación o las actualizará en sus solicitudes.

## <a name="abuse-of-service-risks"></a>Abuso de riesgos del servicio

El **abuso de riesgos del servicio** significa que los clientes que usan servicios en la nube infringen la Directiva de uso aceptable de Microsoft.

### <a name="examples-of-abuse-of-service"></a>Ejemplos de abuso de servicio

Algunos ejemplos de estas infracciones de la Directiva de uso aceptable de Microsoft son:

- Correo basura
- Piratería
- Ataques por denegación de servicio distribuido (DDoS)
- Minería de Bitcoin
- Distribución de malware
- Reventa de suscripciones pirateadas

## <a name="theft-of-service-risks"></a>Robo de riesgos de servicio

El **robo de riesgos de servicio** implica a los clientes que no tienen intención de pagar por los servicios consumidos. Este robo puede implicar el uso de instrumentos de pago robados, la información de facturación falsa o el valor predeterminado de los saldos pendientes.

### <a name="examples-of-service-theft"></a>Ejemplos de robo de servicio

Algunos ejemplos de estos riesgos de transacciones en línea pueden ser:

- Transacciones que no se producen en la persona ("la tarjeta de crédito no está presente")
- Identidades no representadas
- Servicios aprovisionados y usados antes de recibir el pago inicial
- Mercados emergentes o regiones de alto riesgo para fraude en línea
- Automatización de la creación y compra de cuentas por actores no válidos

## <a name="managing-online-risk"></a>Administración de riesgos en línea

Puede utilizar las siguientes recomendaciones como ayuda para desarrollar directivas y prácticas con el fin de reducir la exposición a los riesgos de transacciones en línea en el ciclo de vida de las relaciones con los clientes.

### <a name="onboarding-new-customers"></a>Incorporación de nuevos clientes

Sugerencias para reducir los riesgos en línea al incorporar nuevos clientes:

- Establezca relaciones personales con los clientes siempre que sea posible (por ejemplo, ponerse en contacto con los clientes por teléfono).
- Compruebe las credenciales y el fondo de los clientes a través de métodos mejores (como el uso de oficinas de crédito o agencias de informes comerciales empresariales).
- Use la autenticación multifactor (como la comprobación de SMS) durante el registro para minimizar la exposición a la creación y compra de cuentas robóticas.
- Administrar y realizar un seguimiento de las identidades mediante servicios (como servicios de identidad digital).
- Evalúe el nivel financiero del cliente a través de rigurosos sistemas de detección de fraudes de tarjetas de crédito.
- Establezca una directiva de recopilación clara. Detalle el proceso de las colecciones y el momento en que el acceso a las suscripciones se verá afectado por no pago. (Puede deshabilitar el acceso o [suspender las suscripciones de un cliente](create-a-new-subscription.md#suspend-a-subscription) para que no sean de pago).

### <a name="managing-customer-accounts"></a>Administración de cuentas de clientes

Las sugerencias para administrar las cuentas de cliente posteriores a la compra incluyen:

- Implemente un proceso para recibir, revisar, actuar y responder rápidamente a las notificaciones de Microsoft.
- Trabaje con los clientes para comprender sus necesidades empresariales de uso de la nube, mientras que la configuración de umbrales de supervisión adecuada. (Por ejemplo, puede [establecer un presupuesto mensual de gastos de Azure en el](set-an-azure-spending-budget-for-your-customers.md) centro de Partners. Esta comprensión le permite supervisar el uso del cliente durante el mes y recibir una notificación cuando los clientes estén cerca de su presupuesto).
- Supervise los [registros de actividad](activity-logs.md) de los clientes con regularidad para ayudar a detectar fraudes pronto.
- Realice una acción rápida cuando se detecten actividades sospechosas.
- Evite ofrecer a los clientes acceso administrativo completo a las suscripciones sin implementar primero los controles de mitigación de riesgos.

### <a name="managing-customer-billing"></a>Administrar la facturación de los clientes

Las sugerencias para administrar la compra posterior a la facturación de clientes incluyen:

- Solicite los pagos por adelantado antes de las transacciones iniciales y la facturación.
- No acepte instrumentos de pago de alto riesgo (como tarjetas de prepago o tarjetas de valor almacenado).
- Supervise los pagos de clientes y los clientes de cuentas de vencimiento. Aplique de forma agresiva procesos normalizados de estiba para los pagos o la no pago.

Para obtener estrategias más detalladas para mitigar los riesgos en línea, consulte la [Guía de administración de riesgos de transacciones en línea.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4Bhtt)
