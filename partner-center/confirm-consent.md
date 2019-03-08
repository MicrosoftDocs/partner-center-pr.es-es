---
title: Confirmar la aceptación del cliente del Contrato de Microsoft Cloud | Centro de partners
ms.topic: article
ms.date: 02/22/2019
Description: Como partner, debes obtener la aceptación por parte de tu cliente del Contrato de Microsoft Cloud antes de pedir productos y servicios Microsoft para dicho cliente. Mejor ayuda asociados requisitos de cumplimiento, Microsoft le pide a los asociados para confirmar la aceptación al proporcionar determinados detalles relacionados con la persona que ha aceptado el contrato.
author: LauraBrenner
ms.author: v-petand
keywords: cliente, clientes, da su consentimiento, MCA, contrato de Microsoft en la nube, las plantillas de contrato de cliente
ms.localizationpriority: medium
ms.openlocfilehash: e8c4b66027eeb9e285bd09a4b77aaf9bb6574188
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587568"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Confirmar la aceptación del cliente del Contrato de Microsoft Cloud

**Se aplica a**
-  Centro de partners

Como partner, debes obtener la aceptación por parte de tu cliente del Contrato de Microsoft Cloud antes de pedir productos y servicios Microsoft para dicho cliente. Para ayudar mejor a los partners a cumplir con los requisitos de cumplimiento, Microsoft pide a los partners que confirmen la aceptación proporcionando los siguientes detalles de la persona que haya aceptado el contrato: 

-   Nombre

-   Apellidos

-   Dirección de correo electrónico

-   Número de teléfono

-   Fecha de aceptación

Para obtener más información, vea la confirmación de aceptación del cliente de contrato en la nube de Microsoft [preguntas más frecuentes](https://docs.microsoft.com/en-us/partner-center/confirm-consent-faq).

## <a name="schedule"></a>Programa

**7 de agosto de 2018**

-   Los partners de factura directa y los proveedores indirectos pueden confirmar la aceptación del cliente del Contrato de Microsoft Cloud. La Confirmación es *opcional*.

-   Confirmación de aceptación del cliente puede realizarse a través del centro de partners o Partner Center API.

-   La confirmación de la aceptación del cliente es compatible solo con la nube pública de Microsoft.


**7 de noviembre de 2018**

-   Dirigir factura asociados y proveedores indirectos **debe** confirme la aceptación del cliente del contrato en la nube de Microsoft al intercambiar a través del panel de centro de partners. La confirmación es *obligatoria*.

-   Si no se facilita la confirmación para un cliente determinado:

    -   No podrás crear nuevos pedidos para este cliente.

    -   No podrás cambiar el número de puestos de suscripciones existentes en función de puestos para este cliente.

-   Confirmación de aceptación del cliente puede realizarse a través del centro de partners o Partner Center API.

-   La confirmación de la aceptación del cliente es compatible solo con la nube pública de Microsoft.

-   Esto se aplica a los entornos de producción y espacio aislado.

**11 de marzo de 2018**

- Socios directo de facturas y Providersmust indirecta confirmación la aceptación del cliente del contrato en la nube de Microsoft en el entorno de espacio aislado CSP al intercambiar a través de Partner Center API.
- Si no se facilita la confirmación para un cliente determinado:

    - No podrá crear nuevos pedidos para este cliente mediante la API del centro de partners.
 
    - No podrá cambiar el número de puestos de suscripciones basadas en puestos existentes para este cliente mediante la API del centro de partners.
- La confirmación de la aceptación del cliente es compatible solo con la nube pública de Microsoft. 

**22 de marzo, 12018**

- Socios directo de facturas y Providersmust indirecta confirmación la aceptación del cliente del contrato en la nube de Microsoft en el entorno de producción de CSP al intercambiar a través de Partner Center API.

- Si no se facilita la confirmación para un cliente determinado:
  - No podrá crear nuevos pedidos para este cliente mediante la API del centro de partners.

  - No podrá cambiar el número de puestos de suscripciones basadas en puestos existentes para este cliente mediante la API del centro de partners.
-  La confirmación de la aceptación del cliente es compatible solo con la nube pública de Microsoft.







## <a name="confirming-customer-acceptance-in-partner-center"></a>Confirmar la aceptación del cliente en el centro de partners

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confirmar la aceptación del cliente para un nuevo cliente

Utilice el procedimiento siguiente para confirmar la aceptación del cliente al crear a un nuevo inquilino de cliente en el centro de partners. Ten en cuenta que debes ser agente de administración o agente de ventas para poder hacer esto.
 
1.  Seleccione **clientes**y, a continuación, **nuevo cliente** y, a continuación, seleccione **información de la cuenta**.

2.  Introduce la información sobre la **Empresa** y el **Contacto principal**.

![Información de la empresa](images/mca/mca1.png)

3.  En **Contrato de Microsoft Cloud**, selecciona **El cliente ha aceptado el último contrato Microsoft Cloud**. 

4.  En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.

5.  Introduce los detalles del usuario que proporciona la aceptación. 

![Agregar la fecha de aceptación](images/mca/MCA3.png)

De manera predeterminada, se mostrará la información del usuario de contacto principal. Si esto no es correcto, selecciona **Actualizar** y, a continuación, introduce el **Nombre**, los **Apellidos**, la **Dirección de correo** y el **Número de teléfono* (opcional) de la persona que haya aceptado el contrato.

6.  Selecciona **Siguiente** para continuar con los pasos restantes para crear el inquilino del cliente.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confirmar la aceptación del cliente para un cliente existente

Debes ser agente de administración o agente de ventas para poder hacer esto. 

1.  Selecciona **Clientes**y, a continuación, busca y selecciona el cliente que quieras ver. 

2.  Seleccione **información de la cuenta**.

3.  En **Contrato de Microsoft Cloud**, selecciona **Actualizar**.

![Actualización](images/mca/mca4.png)

4.  Escriba el **nombre**, **apellidos**, **dirección de correo electrónico**, y **número de teléfono** (opcional) del usuario que ha aceptado el contrato.

5.  En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.

6.  Selecciona **Guardar y continuar**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confirmar la aceptación del cliente durante la creación de un nuevo pedido para un cliente existente

Si intentas crear un nuevo pedido para un cliente existente para el que no has confirmado antes, recibirás un aviso para completar la confirmación. Utiliza el siguiente procedimiento para hacerlo. 

1.  Escriba el **nombre**, **apellidos**, **dirección de correo electrónico**, y **número de teléfono** (opcional) del usuario que ha aceptado el contrato.

2.  En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.

3.  Selecciona **Guardar y continuar**.


### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperar la aceptación del cliente para un cliente existente

Puedes recuperar la confirmación de aceptación del cliente para un cliente existente que la haya proporcionado anteriormente con el siguiente procedimiento. Debes ser agente de administración o agente de ventas para poder hacer esto. 

1.  Selecciona **Clientes**y, a continuación, busca y selecciona el cliente que quieras ver. 

2.  Seleccione **información de la cuenta**.

3.  En **Contrato de Microsoft Cloud**, verás si no se ha proporcionado o no la confirmación de este cliente.

