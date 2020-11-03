---
title: Recepción de pagos en el Marketplace comercial
description: 'Obtenga información sobre cómo recibir los pagos de ganancias en el Marketplace comercial: Azure Marketplace. Incluye la política de pago, el estado de retención de pago y las declaraciones de pago.'
ms.service: marketplace
ms.topic: conceptual
ms.date: 09/28/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: 61730eec204674d7ad095d1fffcd997f65d135ea
ms.sourcegitcommit: 7f595faf952bf2d6cdc229da38bd67ee701b2083
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/02/2020
ms.locfileid: "93189737"
---
# <a name="getting-paid-in-the-commercial-marketplace"></a>Recepción de pagos en el Marketplace comercial

En este artículo se ofrece información importante sobre cómo recibir el pago de las ofertas, los complementos y los ingresos publicitarios. Resume la Directiva de pago, los pasos necesarios antes de recibir el pago y la información general sobre la declaración de pago.

## <a name="commercial-marketplace-payout-policies-and-agreements"></a>Contratos y directivas de pago de Marketplace comercial

Para obtener el pago, es necesario cumplir los acuerdos y la Directiva de pago.

- [Microsoft Azure Marketplace acuerdo del publicador](https://go.microsoft.com/fwlink/p/?LinkID=699560): antes de recibir el pago, debe aceptar este contrato del anunciante. En este contrato se explica la relación entre usted y Microsoft como perteneciente a las ofertas de vendedores en el Marketplace comercial, incluida la cuota de la tienda que Microsoft cobra por cada venta realizada.
- La [Directiva](payout-policy-details.md) de pago muestra las directivas de pago de pago, incluidos los métodos de pago y programación de pago. La Directiva también explica el proceso de los no pagos de clientes.
- [Detalles de impuestos](tax-details-marketplace.md) explica la consideración fiscal de la selección de precios y la responsabilidad fiscal en el contrato de Microsoft [Publisher](https://go.microsoft.com/fwlink/p/?LinkID=699560).
- Las tarifas de la **tienda** se definen oficialmente en el acuerdo del publicador. La tarifa de la tienda se aplica a todas las ventas de ofertas recopiladas por el Marketplace comercial, incluidos los complementos.
- Los **pagos** se realizan mensualmente (siempre que se cumpla el umbral de pago). Normalmente enviamos cualquier pago debido a un mes determinado el día 15 de ese mes. Los pagos suelen tardar entre 3 y 10 días hábiles adicionales en llegar a su cuenta de pago. Para conocer los detalles, consulte [Umbrales de pago, métodos e intervalos de tiempo](payment-thresholds-methods-timeframes.md).

## <a name="prerequisite-steps-before-getting-paid"></a>Pasos de requisitos previos antes de recibir el pago

Antes de que se pague por primera vez, debe configurar la cuenta de pago y completar los formularios de banco y fiscal necesarios. En los formularios bancarios y fiscales, se proporcionarán los métodos de pago preferidos y los formularios fiscales para la retención de impuestos. Los formularios de banco y fiscal son necesarios para que podamos pagarle. Para obtener más información, consulte [configuración de la cuenta de pago y los formularios fiscales](set-up-your-payout-account.md).

### <a name="payout-hold-status"></a>Estado de retención de pagos

De forma predeterminada, enviaremos pagos mensualmente, como se describió anteriormente. Sin embargo, tiene la opción de poner los pagos para un programa en espera y Microsoft no publicará los pagos en su cuenta. Si decide poner los pagos en espera, continuaremos registrando cualquier ganancia en la página de **pagos** . Pero no se le envía ningún pago a la cuenta hasta que quite la retención.

Para colocar los pagos en espera, seleccione el icono de engranaje **configuración** en la parte superior derecha y, a continuación, **configuración del desarrollador** . Seleccione **pago y impuestos** en el menú de la izquierda y, en la sección **asignación de Perfil de pago y impuestos** , busque el programa para el que desea realizar los pagos. Active la casilla **mantener mi pago** para conservar los pagos de este programa. Puede cambiar el estado de la retención de pago en cualquier momento, pero su decisión afectará al siguiente pago mensual. Por ejemplo, si quiere retener los pagos de abril, asegúrese de establecer el estado de retención de pagos en **Activado** antes del final de marzo.

Una vez que haya establecido el estado de retención de pago en **activado** , todos los pagos de este programa estarán en espera hasta que **desactive la casilla.** Al hacerlo, se incluirá durante el siguiente ciclo de pago mensual (siempre que se cumpla el umbral de pago). Si ha tenido los pagos en espera, pero desea tener un pago generado en junio, desactive la casilla para **desactivarla** antes del final de mayo.

>[!Note]
> El estado de la retención de pago se aplica individualmente a cada programa (Microsoft Store, publicidad, Azure Marketplace, etc.). Si desea conservar los pagos de todos los programas, mantenga el pago en cada programa individualmente.

## <a name="payout-statements"></a>Balances de pagos

La declaración de pago muestra los beneficios de las ventas de las ofertas y los complementos en el historial de transacciones. También puede ver los detalles de pago y descargar informes en formato TSV o CSV. Consulte las [declaraciones](payout-statement.md) de pago para obtener más información sobre cómo acceder a la declaración de pago y los detalles del historial de transacciones y los informes de pago. Además, puede usar la [API de pagos de asociados](https://apidocs.microsoft.com/services/partnerpayouts) para extraer sistemáticamente los informes de pago.

## <a name="next-steps"></a>Pasos siguientes

- [API de pagos de asociados](https://apidocs.microsoft.com/services/partnerpayouts)
- [Preguntas más frecuentes sobre los pagos de Marketplace](payout-faq.md)
