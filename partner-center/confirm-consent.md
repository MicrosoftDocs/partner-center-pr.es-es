---
title: Confirmar la aceptación del cliente del Contrato de Microsoft Cloud | Centro de partners
ms.topic: article
ms.date: 04/16/2019
Description: Como partner, debes obtener la aceptación por parte de tu cliente del Contrato de Microsoft Cloud antes de pedir productos y servicios Microsoft para dicho cliente. Para ayudar mejor a los partners a cumplir con los requisitos de cumplimiento, Microsoft les pide que confirmen la aceptación proporcionando ciertos detalles de la persona que ha aceptado el contrato.
author: LauraBrenner
ms.author: labrenne
keywords: cliente, clientes, consentimiento, MCA, contrato de Microsoft Cloud, plantillas de contrato de cliente
ms.localizationpriority: medium
ms.openlocfilehash: 13bd3ee03a346448ca8131713420cf75e555195b
ms.sourcegitcommit: cb736d4ec766d2af41d8c6102d13563169386438
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/29/2019
ms.locfileid: "73045648"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Confirmar la aceptación del cliente del Contrato de Microsoft Cloud

**Se aplica a**
-  Centro de partners

> [!NOTE]
> Actualmente, el recurso de acuerdo solo es compatible con el centro de Partners en la nube pública de Microsoft. No es aplicable a:
> * Centro de partners operado por 21Vianet
> * Centro de partners para Microsoft Cloud Alemania
> * Centro de partners para Microsoft Cloud for US Government

>[!NOTE]
>Este contrato es válido hasta el 31 de enero de 2020. Después de esa fecha, todos los clientes, existentes y nuevos, deben firmar el nuevo contrato de cliente de Microsoft. Para obtener más información, consulte [confirmar la aceptación del cliente del contrato de cliente de Microsoft](confirm-customer-agreement.md).

Como partner, debes obtener la aceptación por parte de tu cliente del Contrato de Microsoft Cloud antes de pedir productos y servicios Microsoft para dicho cliente. Para ayudar mejor a los partners a cumplir con los requisitos de cumplimiento, Microsoft pide a los partners que confirmen la aceptación proporcionando los siguientes detalles de la persona que haya aceptado el contrato: 

-   Nombre

-   Apellidos

-   Dirección de correo electrónico

-   Número de teléfono (opcional)

-   Fecha de aceptación

Para obtener más información, consulte las [preguntas](https://docs.microsoft.com/partner-center/confirm-consent-faq)más frecuentes sobre la confirmación de aceptación del cliente del contrato de Microsoft Cloud.

Los asociados directos de facturación y los proveedores indirectos deben confirmar la aceptación del cliente del contrato de Microsoft Cloud al actuar a través del centro de Partners o de la API del centro de Partners. La confirmación es *obligatoria*.

Si no se facilita la confirmación para un cliente determinado:

-   No podrás crear nuevos pedidos para este cliente.

-   No podrás cambiar el número de puestos de las suscripciones basadas en puestos existentes para este cliente.

La confirmación de la aceptación del cliente se puede realizar a través del centro de Partners o de la API del centro de Partners. Para hacer esto a través de la API del centro de Partners, consulte los temas siguientes: 

-   [Obtener confirmación del consentimiento del cliente](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [Obtener metadatos del contrato](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [Confirmar el consentimiento del cliente](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


Esto se aplica a los entornos de producción y de espacio aislado.

## <a name="confirming-customer-acceptance-in-partner-center"></a>Confirmar la aceptación del cliente en el centro de Partners

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confirmar la aceptación del cliente para un nuevo cliente

Use el procedimiento siguiente para confirmar la aceptación del cliente mientras crea un nuevo inquilino de cliente en el centro de Partners. Ten en cuenta que debes ser agente de administración o agente de ventas para poder hacer esto.

1. Seleccione **clientes**y, después, **nuevo cliente** y, a continuación, seleccione información de la **cuenta**.
2. Introduce la información sobre la **Empresa** y el **Contacto principal**.

![Información de la compañía](images/mca/mca1.png)

3. En **Contrato de Microsoft Cloud**, selecciona **El cliente ha aceptado el último contrato Microsoft Cloud**.
4. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.
5. Introduce los detalles del usuario que proporciona la aceptación.

![Agregar fecha de aceptación](images/mca/MCA3.png)

De manera predeterminada, se mostrará la información del usuario de contacto principal. Si esto no es correcto, selecciona **Actualizar** y, a continuación, introduce el **Nombre**, los **Apellidos**, la **Dirección de correo** y el **Número de teléfono* (opcional) de la persona que haya aceptado el contrato.

6. Selecciona **Siguiente** para continuar con los pasos restantes para crear el inquilino del cliente.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confirmar la aceptación del cliente para un cliente existente

Debes ser agente de administración o agente de ventas para poder hacer esto.

1. Selecciona **Clientes** y, a continuación, busca y selecciona el cliente que quieras ver.
2. Selecciona **Información de cuenta**.
3. En **Contrato de Microsoft Cloud**, selecciona **Actualizar**.

![Actualizar](images/mca/mca4.png)

4. Escriba el **nombre**, los **apellidos**, la **dirección de correo electrónico**y el **número de teléfono** (opcional) del usuario que aceptó el contrato.
5. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.
6. Selecciona **Guardar y continuar**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confirmar la aceptación del cliente durante la creación de un nuevo pedido para un cliente existente

Si intentas crear un nuevo pedido para un cliente existente para el que no has confirmado antes, recibirás un aviso para completar la confirmación. Utiliza el siguiente procedimiento para hacerlo.

1. Escriba el **nombre**, los **apellidos**, la **dirección de correo electrónico**y el **número de teléfono** (opcional) del usuario que aceptó el contrato.
2. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.
3. Selecciona **Guardar y continuar**.

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperar la aceptación del cliente para un cliente existente

Puedes recuperar la confirmación de aceptación del cliente para un cliente existente que la haya proporcionado anteriormente con el siguiente procedimiento. Debes ser agente de administración o agente de ventas para poder hacer esto.

1. Selecciona **Clientes** y, a continuación, busca y selecciona el cliente que quieras ver.
2. Selecciona **Información de cuenta**.
3. En **Contrato de Microsoft Cloud**, verás si no se ha proporcionado o no la confirmación de este cliente.
