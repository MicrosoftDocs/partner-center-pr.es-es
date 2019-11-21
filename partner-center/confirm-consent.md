---
title: Confirmar la aceptación del cliente del Contrato de Microsoft Cloud | Centro de partners
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Learn how to confirm customer acceptance of the Microsoft Cloud Agreement. This may be needed to order Microsoft products and services for customers.
author: LauraBrenner
ms.author: labrenne
keywords: customer, customers, consent, MCA, Microsoft Cloud Agreement, customer agreement templates
ms.localizationpriority: medium
ms.openlocfilehash: d9b2df8f9cf8795eedb75bc23773942e365c83fe
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252588"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Confirmar la aceptación del cliente del Contrato de Microsoft Cloud

**Se aplica a**
-  Centro de partners

> [!NOTE]
> The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only. It is not applicable to:
> * Centro de partners operado por 21Vianet
> * Centro de partners para Microsoft Cloud Alemania
> * Centro de partners para Microsoft Cloud for US Government

>[!NOTE]
>This agreement is valid until January 31, 2020. After that date, all customers, existing and new, must sign the new Microsoft Customer Agreement. To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).

As a partner, you need to obtain your customer's acceptance of the Microsoft Cloud Agreement before you can order Microsoft products and services for that customer. Para ayudar mejor a los partners a cumplir con los requisitos de cumplimiento, Microsoft pide a los partners que confirmen la aceptación proporcionando los siguientes detalles de la persona que haya aceptado el contrato: 

-   Nombre

-   Apellidos

-   Dirección de correo electrónico

-   Número de teléfono (opcional)

-   Fecha de aceptación

To learn more, see the Microsoft Cloud Agreement customer acceptance confirmation [Frequently Asked Questions](https://docs.microsoft.com/partner-center/confirm-consent-faq).

Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Cloud Agreement when transacting through Partner Center or Partner Center API. La confirmación es *obligatoria*.

Si no se facilita la confirmación para un cliente determinado:

-   You won't be able to create new orders for this customer.

-   You won't be able to change the seat count of existing seat-based subscriptions for this customer.

Confirmation of customer acceptance can be done via Partner Center or the Partner Center API. To do this through the Partner Center API, see the following topics: 

-   [Get confirmation of customer consent](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [Get agreement metadata](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [Confirm customer consent](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


This applies to both production and sandbox environments.

## <a name="confirming-customer-acceptance-in-partner-center"></a>Confirming customer acceptance in Partner Center

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confirmar la aceptación del cliente para un nuevo cliente

Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center. Ten en cuenta que debes ser agente de administración o agente de ventas para poder hacer esto.

1. Select **Customers**, and then **New customer** and then select **Account info**.
2. Introduce la información sobre la **Empresa** y el **Contacto principal**.

![Company information](images/mca/mca1.png)

3. En **Contrato de Microsoft Cloud**, selecciona **El cliente ha aceptado el último contrato Microsoft Cloud**.
4. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.
5. Introduce los detalles del usuario que proporciona la aceptación.

![Add acceptance date](images/mca/MCA3.png)

De manera predeterminada, se mostrará la información del usuario de contacto principal. If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and **Phone number* (optional) of the person who accepted the agreement.

6. Selecciona **Siguiente** para continuar con los pasos restantes para crear el inquilino del cliente.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confirmar la aceptación del cliente para un cliente existente

Debes ser agente de administración o agente de ventas para poder hacer esto.

1. Selecciona **Clientes** y, a continuación, busca y selecciona el cliente que quieras ver.
2. Selecciona **Información de cuenta**.
3. En **Contrato de Microsoft Cloud**, selecciona **Actualizar**.

![Actualizar](images/mca/mca4.png)

4. Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.
5. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.
6. Selecciona **Guardar y continuar**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confirmar la aceptación del cliente durante la creación de un nuevo pedido para un cliente existente

If you try to create a new order for an existing customer which you have not confirmed before, you'll receive a prompt to complete the confirmation. Utiliza el siguiente procedimiento para hacerlo.

1. Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.
2. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.
3. Selecciona **Guardar y continuar**.

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperar la aceptación del cliente para un cliente existente

Puedes recuperar la confirmación de aceptación del cliente para un cliente existente que la haya proporcionado anteriormente con el siguiente procedimiento. Debes ser agente de administración o agente de ventas para poder hacer esto.

1. Selecciona **Clientes** y, a continuación, busca y selecciona el cliente que quieras ver.
2. Selecciona **Información de cuenta**.
3. Under **Microsoft cloud agreement**, you'll see whether or not confirmation has been provided for this customer.
