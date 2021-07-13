---
title: Obtener el pago en Centro de partners
description: Obtenga información sobre cómo recibir pagos de ganancias como asociado de Microsoft, por ejemplo, a través de ofertas de marketplace comercial, programas de incentivos y el Proveedor de soluciones en la nube cliente. Incluye la directiva de pago, el estado de retención de pago y los extractos de pago.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 11/25/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: cc01a1aada6c6665d3fd8f6efc6e5ef873736bdc
ms.sourcegitcommit: a09a5f893e876de23a8aa5c0d637e50c5be84941
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/13/2021
ms.locfileid: "113684396"
---
# <a name="getting-paid-in-partner-center"></a>Obtener el pago en Centro de partners

**Roles adecuados:** Administrador de | Administrador global

En este artículo se proporciona información importante sobre cómo recibir el pago de las ofertas, complementos y ganancias de publicidad. Resume la directiva de pago, los pasos necesarios antes de recibir el pago y la información general del extracto de pago.

## <a name="payout-policies-and-agreements"></a>Directivas y contratos de pago

La obtención del pago requiere que se cumplan los contratos y la directiva de pago.

- [Microsoft Azure marketplace Publisher:](/legal/marketplace/msft-publisher-agreement)antes de recibir el pago, debe aceptar este contrato de publicador. En este contrato se explica la relación entre usted y Microsoft en lo que se refiere a las ofertas de vendedores del marketplace comercial, incluida la cuota de tienda que Microsoft cobra por cada venta realizada.
- [La directiva de pago](payout-policy-details.md) muestra las directivas de pago, incluida la programación de pago y los métodos de pago. La directiva también explica el proceso de impagos del cliente.
- [En Los detalles fiscales](tax-details-marketplace.md) se explica la consideración fiscal de la selección de precios y la responsabilidad fiscal en el Contrato Publisher [Microsoft](/legal/marketplace/msft-publisher-agreement).
- **Las tarifas** de la tienda se definen oficialmente en el Publisher de almacenamiento. El precio de la tienda se aplica a todas las ventas de ofertas recopiladas por el marketplace comercial, incluidos los complementos.
- **Los** pagos se realizan mensualmente (siempre que se haya cumplido el umbral de pago). Normalmente, los pagos que se deben pagar en un mes determinado se envían el día 15 de ese mes. Los pagos suelen tardar entre 3 y 10 días laborables adicionales en llegar a su cuenta de pago. Para conocer los detalles, consulte [Umbrales de pago, métodos e intervalos de tiempo](payment-thresholds-methods-timeframes.md).

## <a name="prerequisite-steps-before-getting-paid"></a>Pasos previos antes de recibir el pago

Antes de recibir el pago por primera vez, debe configurar la cuenta de pago y completar los formularios bancarios y fiscales necesarios. En los formularios bancarios y fiscales, proporcionará los métodos de pago preferidos y los formularios fiscales para la retención de impuestos. Los formularios bancarios y fiscales son necesarios para poder pagarle. Para más información, consulte [Configuración de la cuenta de pago y los formularios fiscales.](set-up-your-payout-account.md)

### <a name="payout-hold-status"></a>Estado de retención de pagos

De forma predeterminada, enviaremos pagos mensualmente, como se describió anteriormente. Sin embargo, puede poner en espera los pagos de un programa y Microsoft no liberará los pagos a su cuenta. Si decide mantener los pagos en espera, seguiremos registrando las **ganancias** en la página Pagos. Pero no se le envía ningún pago a la cuenta hasta que quite la retención.

Para mantener los pagos en espera, seleccione el **icono Configuración** engranaje en la parte superior derecha y, a continuación, Configuración de **la cuenta.** Seleccione **Pago e impuestos en** el  menú de la izquierda y, en la sección Asignación de perfiles de pago y impuestos, busque el programa para el que desea que se retenan los pagos. Active la **casilla Mantener** mi pago para contener los pagos de este programa. Puede cambiar el estado de retención de pago en cualquier momento, pero su decisión afectará al siguiente pago mensual. Por ejemplo, si quiere retener los pagos de abril, asegúrese de establecer el estado de retención de pagos en **Activado** antes del final de marzo.

Una vez que haya establecido el estado de retención de pago en **En**, todos los pagos de este programa estarán en espera hasta que desactive la casilla **en Desactivado.** Al hacerlo, se le incluirá durante el siguiente ciclo de pago mensual (siempre que se haya cumplido el umbral de pago). Si ha tenido sus pagos en espera, pero le gustaría que se generara un pago en junio, desactive la casilla en **Desactivado** antes de finales de mayo.

>[!Note]
> El estado de retención de pago se aplica individualmente a cada programa (Microsoft Store, publicidad, Azure Marketplace, y así sucesivamente). Si desea mantener los pagos de todos los programas, mantenga el pago en cada programa individualmente.

## <a name="payout-statements"></a>Extractos de pagos

El extracto de pago muestra las ganancias de las ventas de las ofertas y complementos en el historial de transacciones. También puede ver los detalles de pago y descargar informes en formato tsv o csv. Consulte [Declaraciones de pago para](payout-statement.md) obtener más información sobre cómo acceder al extracto de pago y los detalles del historial de transacciones y los informes de pago. Además, puede usar partner [payouts API](https://apidocs.microsoft.com/services/partnerpayouts) para extraer sistemáticamente los informes de pago.

## <a name="next-steps"></a>Pasos siguientes

- [API de pagos de asociados](https://apidocs.microsoft.com/services/partnerpayouts)
- [Preguntas frecuentes sobre pagos](payout-faq.yml)