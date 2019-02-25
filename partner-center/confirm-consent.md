---
title: Confirmar la aceptación del cliente del contrato de Microsoft en la nube | El centro de partners
ms.topic: article
ms.date: 02/22/2019
Description: As a partner, you need to obtain your customer’s acceptance of the Microsoft Cloud Agreement before you can order Microsoft products and services for that customer. To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing certain details regarding the person who accepted the agreement.
author: v-petand
ms.author: v-petand
keywords: cliente, clientes, da su consentimiento, MCA, contrato de Microsoft Cloud, plantillas de acuerdos de cliente
ms.localizationpriority: medium
ms.openlocfilehash: 269647b819dda4c86ae7397dac3504268767abba
ms.sourcegitcommit: 83d2757756ed1ed8f5f7ae06c84e7547174faf9a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 02/25/2019
ms.locfileid: "9099443"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Confirmar la aceptación del cliente del contrato de Microsoft en la nube

**Se aplica a:**
-  Centro de partners

Como partner, debes obtener la aceptación de tu cliente del contrato de Microsoft en la nube antes de que se pueden pedir productos de Microsoft y servicios para que el cliente. Para mejorar la ayuda a los partners cumplan los requisitos de cumplimiento, Microsoft te pide a los partners para confirmar la aceptación al proporcionar la siguiente información relativa a la persona que ha aceptado el acuerdo: 

-   Nombre

-   Apellidos

-   Dirección de correo electrónico

-   Número de teléfono

-   Fecha de aceptación

Para obtener más información, consulta la confirmación de aceptación de cliente del contrato de Microsoft Cloud [Preguntas más frecuentes](https://docs.microsoft.com/en-us/partner-center/confirm-consent-faq).

## <a name="schedule"></a>Programación

**7 de agosto de 2018**

-   Los partners de facturación directa y los proveedores indirectos pueden confirmar aceptación del cliente del contrato de Microsoft en la nube. Confirmación es *opcional*.

-   Confirmación de aceptación de cliente puede hacerse a través del centro de partners o API del centro de partners.

-   Confirmación de aceptación de cliente solo es compatible con la nube pública de Microsoft.


**7 de noviembre de 2018**

-   Los partners de facturación directa y proveedores indirectos **deben** confirmar aceptación del cliente del contrato de Microsoft en la nube cuando transacciones a través del panel del centro de partners. Confirmación es *obligatorio*.

-   Si no se proporciona la confirmación para un cliente determinado:

    -   No podrás crear nuevos pedidos de este cliente.

    -   No podrás cambiar el número de puestos de suscripciones existentes basados en puestos de este cliente.

-   Confirmación de aceptación de cliente puede hacerse a través del centro de partners o API del centro de partners.

-   Confirmación de aceptación de cliente solo es compatible con la nube pública de Microsoft.

-   Esto se aplica a los entornos de producción y espacio aislado.

**11 de marzo de 2018**

- Los partners de facturación directa y Providersmust indirecto confirmar aceptación del cliente del contrato de nube de Microsoft en el entorno de espacio aislado CSP cuando transacciones a través de la API del centro de partners.
- Si no se proporciona la confirmación para un cliente determinado:

    - No podrás crear nuevos pedidos de cliente mediante la API del centro de partners.
 
    - No podrás cambiar el número de puestos de suscripciones existentes basados en puestos para este cliente mediante la API del centro de partners.
- Confirmación de aceptación de cliente solo es compatible con la nube pública de Microsoft. 

**22 de marzo, 12018**

- Los partners de facturación directa y Providersmust indirecto confirmar aceptación del cliente del contrato de nube de Microsoft en el entorno de producción de CSP cuando transacciones a través de la API del centro de partners.

- Si no se proporciona la confirmación para un cliente determinado:
  - No podrás crear nuevos pedidos de cliente mediante la API del centro de partners.

  - No podrás cambiar el número de puestos de suscripciones existentes basados en puestos para este cliente mediante la API del centro de partners.
-  Confirmación de aceptación de cliente solo es compatible con la nube pública de Microsoft.







## <a name="confirming-customer-acceptance-in-partner-center"></a>Confirmar la aceptación del cliente en el centro de partners

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confirmar la aceptación del cliente para un nuevo cliente

Usa el siguiente procedimiento para confirmar la aceptación del cliente mientras creas a un nuevo inquilino del cliente en el centro de partners. Ten en cuenta que debe ser un agente de administración o el agente de ventas para hacer esto.
 
1.  Selecciona **los clientes**y, a continuación, **nuevo cliente** y, a continuación, selecciona **la información de cuenta**.

2.  Escribe la información acerca de la **empresa** y el **contacto principal**.

![Información de la empresa](images/mca/mca1.png)

3.  **Contrato de Microsoft cloud**, selecciona **el cliente ha aceptado el acuerdo de nube de Microsoft más reciente**. 

4.  En **la fecha de aceptación de contrato**, escribe la fecha adecuada. No puedes establecer esto en una fecha futura.

5.  Escribe los detalles del usuario que proporciona la aceptación. 

![Agregar la fecha de aceptación](images/mca/MCA3.png)

De manera predeterminada, se muestra la información de usuario de contacto principal. Si esto no es correcto, selecciona la **actualización** y, a continuación, escribe el **nombre**, **apellido**, **dirección de correo electrónico**, y **número de teléfono* (opcional) de la persona que ha aceptado el acuerdo.

6.  Seleccione **siguiente** para continuar con el resto de los pasos para crear al inquilino del cliente.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confirmar la aceptación del cliente de un cliente existente

Debes ser un agente de administración o el agente de ventas para hacer esto. 

1.  Selecciona **los clientes**y, a continuación, busca y selecciona al cliente que quieres ver. 

2.  Selecciona **la información de cuenta**.

3.  **Contrato de Microsoft cloud**, seleccione la **actualización**.

![Actualizar](images/mca/mca4.png)

4.  Escribe el **nombre**, **apellido**, **dirección de correo electrónico**y **número de teléfono** (opcional del usuario que ha aceptado el acuerdo).

5.  En **la fecha de aceptación de contrato**, escribe la fecha adecuada. No puedes establecer esto en una fecha futura.

6.  Seleccione **Guardar y continuar**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confirmar la aceptación del cliente durante la creación de nuevo pedido de un cliente existente

Si intentas crear un nuevo pedido de un cliente existente que no has confirmado antes, recibirás un símbolo del sistema para completar la confirmación. Usa el siguiente procedimiento para hacer esto. 

1.  Escribe el **nombre**, **apellido**, **dirección de correo electrónico**y **número de teléfono** (opcional del usuario que ha aceptado el acuerdo).

2.  En **la fecha de aceptación de contrato**, escribe la fecha adecuada. No puedes establecer esto en una fecha futura.

3.  Seleccione **Guardar y continuar**.


### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperar la confirmación de aceptación de cliente de un cliente existente

Puedes recuperar la confirmación de aceptación de cliente de un cliente existente que has proporcionado anteriormente con el siguiente procedimiento. Debes ser un agente de administración o el agente de ventas para hacer esto. 

1.  Selecciona **los clientes**y, a continuación, busca y selecciona al cliente que quieres ver. 

2.  Selecciona **la información de cuenta**.

3.  **Contrato de Microsoft cloud**, podrás ver independientemente de si se ha proporcionado confirmación para este cliente.

