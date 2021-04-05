---
title: Procedimiento de confirmación de que el cliente ha aceptado el Contrato de cliente de Microsoft para el programa CSP
description: Los asociados del Proveedor de soluciones en la nube (CSP) deben confirmar la aceptación del cliente del Contrato de cliente de Microsoft antes de solicitar servicios Microsoft para los clientes.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633785"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Procedimiento de confirmación de que el cliente ha aceptado el Contrato de cliente de Microsoft para el programa CSP

**Roles adecuados**

- Agente de administrador
- Agente de ventas


Los clientes tienen dos opciones para aceptar el Contrato de cliente de Microsoft.

**Opción 1**: atestación del partner de la aceptación del cliente; el partner puede confirmar la aceptación del cliente mediante el SDK o la API del Centro de partners o a través del panel del Centro de partners.

**Opción 2**: aceptación directa del cliente; el asociado puede invitar al cliente a través de una dirección URL para que revise y acepte el contrato en el Centro de administración de Microsoft 365.

## <a name="access-microsoft-customer-agreement-template"></a>Acceso a la plantilla del Contrato de cliente de Microsoft

Puedes descargar manualmente la versión más reciente de la plantilla del Contrato de cliente de Microsoft desde [aquí](https://aka.ms/customeragreement). El Contrato de cliente de Microsoft es específico para cada país o región. Al solicitar la plantilla del Contrato de cliente de Microsoft, asegúrate de seleccionar el país o región correcto en función de la ubicación del cliente.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Opción 1: Confirmación de la aceptación por parte del cliente en el Centro de partners

Los partners de facturación directa pueden confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft en el Centro de partners para clientes nuevos y clientes existentes. Los revendedores indirectos no pueden dar fe en nombre de sus clientes y deben colaborar con su proveedor indirecto para completar la atestación.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Confirmar la aceptación de los clientes nuevos

Si creas un nuevo inquilino de cliente en el Centro de partners, sigue los pasos que se describen a continuación para confirmar la aceptación del cliente del Contrato de cliente de Microsoft. Para poder seguir estos pasos, debes ser agente de administración o de ventas.

1. Selecciona **Clientes** y, a continuación, **Nuevo cliente**.

2. En **Información de cuenta**, especifica los datos de la empresa y su contacto principal.

3. En **Contrato de Microsoft**, selecciona el cuadro para dar fe de que el cliente ha aceptado el Contrato de cliente de Microsoft.

4. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.

5. Comprueba que la información de contacto del usuario principal que se muestra sea correcta. Si no es correcta, selecciona **Actualizar** y escribe la información exacta de la persona que aceptó el contrato.

6. Selecciona **Siguiente** para continuar con la creación del inquilino del cliente.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Cliente nuevo":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Confirmar la aceptación de los clientes existentes

Debes ser agente de administración o de ventas para poder hacer esto:

1. Selecciona **Clientes**. Busca y selecciona el cliente.

2. Selecciona **Información de cuenta**.

3. En **Contrato de cliente de Microsoft**, selecciona **Actualizar**.

4. Escribe el **Nombre**, los **Apellidos**, la **Dirección de correo electrónico** y el **Número de teléfono** (opcional) de la persona que aceptó el contrato. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.

5. Selecciona **Guardar** y continúa.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Cliente existente":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Recuperar la confirmación de la aceptación del cliente

Siga los pasos que se describen a continuación para recuperar la confirmación de que un cliente existente ha aceptado el Contrato de cliente de Microsoft. Debes ser agente de administración o agente de ventas para poder hacer esto.

1. Selecciona **Clientes** y, a continuación, busca y selecciona el cliente que quieras ver.

2. Selecciona **Información de cuenta**.

3. En **Contrato de cliente de Microsoft**, consulta si el cliente ha proporcionado la confirmación.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Confirmación de la aceptación por parte del cliente mediante el SDK o la API del Centro de partners

Puedes usar el SDK o la API del Centro de partners para confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft. Para obtener más información sobre la API o el SDK, consulta:

- [Obtener los metadatos del acuerdo del Contrato de cliente de Microsoft](/partner-center/develop/get-customer-agreement-metadata)

- [Confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Obtener la confirmación de la aceptación por parte del cliente del Contrato de cliente de Microsoft](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Obtener un vínculo de descarga para la plantilla del Contrato de cliente de Microsoft](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Opción 2: Aceptación del cliente en el Centro de administración de Microsoft 365

Los partners pueden invitar a clientes nuevos y existentes, a través de una dirección URL, para que revisen y acepten el contrato en el Centro de administración de Microsoft 365. En las siguientes secciones se muestra cómo puedes:

- Crear un cliente nuevo e invitarlo para que revise y acepte el contrato.

- Invitar a un cliente nuevo para que revise y acepte la relación y el contrato de revendedor.

- Invitar a un cliente existente para que revise y acepte el contrato.

>[!NOTE]
> Puedes usar el [SDK o la API del Centro de partners](/partner-center/develop/get-direct-sign-status-of-customer-agreement) para obtener el estado de la aceptación directa por parte de un cliente del Contrato de cliente de Microsoft.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Crear un cliente nuevo e invitarlo para que revise y acepte el contrato

Sigue los pasos que se indican a continuación para crear un cliente nuevo en el Centro de partners e invitarlo para que revise y acepte el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365.

1. En la pestaña **Clientes** del Centro de partners, selecciona **Agregar cliente**.

2. En **Información de la cuenta**, escribe la información sobre el nuevo cliente en todos los campos obligatorios, incluido el nombre de la empresa del cliente y el contacto principal.

3. En **Contrato de cliente**, seleccione **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center** (Se pedirá al cliente que acepte el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365). Completa los demás campos obligatorios en la página.

4. Selecciona **Siguiente: revisión** y sigue los pasos para crear el inquilino del cliente. 

>[!NOTE] 
>Los clientes nuevos no pueden hacer compras hasta que acepten el Contrato de cliente de Microsoft.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Crear un cliente nuevo":::

5. Cuando llegues a la pantalla **Confirmación** del nuevo flujo de trabajo del cliente, guarda las credenciales del cliente. Deberás proporcionar estas credenciales al cliente más adelante.

6. Fuera del Centro de partners, crea y envía un correo electrónico en el que invites al cliente a aceptar el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365. Asegúrate de incluir los elementos siguientes en el correo electrónico:

   - Un vínculo a esta[ dirección URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (inicio de sesión obligatorio)

   - Las credenciales del cliente que guardó en el paso 5.

7. A continuación, el cliente recibirá la invitación por correo electrónico del partner y seleccionará la [dirección URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. El cliente deberá iniciar sesión en el Centro de administración de Microsoft 365 con las credenciales del cliente que recibió.

9. El cliente marcará la casilla para aceptar el Contrato de cliente de Microsoft.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Invitación de un cliente nuevo para que revise y acepte la relación de revendedor y el Contrato de cliente de Microsoft 

Usa los pasos siguientes para invitar a un nuevo cliente para que revise y acepte la relación de revendedor y el Contrato de cliente de Microsoft. 

1. En la pestaña **Clientes** en el Centro de partners, selecciona el vínculo **Solicitar una relación de revendedor**. 

2. Se generará una plantilla de correo electrónico automático, que incluirá texto y una dirección URL parametrizada que dirigirá al cliente al Centro de administración de Microsoft 365.

3. Puedes personalizar la plantilla de correo electrónico generada automáticamente y, a continuación, seleccionar **Copiar al portapapeles** o **Abrir en correo**.

4. Usa esta plantilla de correo electrónico para invitar al cliente a aceptar la solicitud de **relación de revendedor** y el **Contrato de cliente de Microsoft**. (Nota: En la invitación por correo electrónico, asegúrate de que el partner también incluye la dirección URL que se proporcionó automáticamente, así como las credenciales del cliente que se crearon recientemente).

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Crear una relación":::

5. El cliente recibirá una invitación por correo electrónico y hará clic en la dirección URL parametrizada. 

6. El cliente usará las credenciales proporcionadas en el correo electrónico para iniciar sesión en el Centro de administración de Microsoft 365.

7. El cliente marcará la casilla para aceptar la **relación de revendedor** y el **Contrato de cliente de Microsoft**. 

8. En la misma dirección URL, el cliente podrá ver una lista consolidada de los diferentes partners con los que trabaja. Podrá seleccionar un partner para ver los detalles.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Aceptar el contrato":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Invitación de un cliente existente para que revise y acepte el contrato

Usa los pasos siguientes para invitar a un cliente existente para que revise y acepte el Contrato de cliente de Microsoft. 

1. Crea el correo electrónico del cliente con la dirección URL incrustada para invitar a tu cliente para que acepte el Contrato de cliente de Microsoft.

2. El cliente recibe la invitación por correo electrónico y hace clic en la [dirección URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. El cliente escribe sus credenciales en el Centro de administración de Microsoft 365.

4. El cliente marcará la casilla para aceptar el Contrato de cliente de Microsoft. 

5. En la misma dirección URL, el cliente podrá ver la lista consolidada de los diferentes partners con los que trabaja. Podrá seleccionar un partner para ver los detalles.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Cliente":::

>[!NOTE]
>En determinados escenarios, es posible que los clientes no puedan aceptar directamente el Contrato de cliente de Microsoft. Para obtener más información sobre estas situaciones, consulte Dos escenarios en los que es necesario dar fe en nombre del cliente, a continuación.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Dos escenarios en los que es necesario dar fe en nombre de tu cliente

Hay dos escenarios en los que es posible que los clientes no puedan aceptar directamente el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365.

**Escenario 1**: un cliente existente que ha comprado cualquier de los productos siguientes a través de una relación de partner existente: ofertas, software o suscripciones de software, instancias reservadas o plan de Azure. Dicho cliente ahora intenta realizar una nueva compra (esta no incluye la renovación automática). Cuando el cliente haga clic en la dirección URL, recibirá el mensaje "Póngase en contacto con su partner para confirmar que acepta el Contrato de cliente de Microsoft".  

**Para resolverlo**: debes dar fe en nombre del cliente.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Captura de pantalla de la página del centro de administración de Microsoft 365 que le pide que se una a su partner para confirmar la aceptación del Contrato de cliente de Microsoft.":::

**Escenario 2**: un cliente existente que ha adquirido cualquiera de las siguientes ofertas, software y suscripciones de software, instancias reservadas y plan de Azure. Dicho cliente ahora intenta realizar una nueva compra con un nuevo partner.

Cuando el cliente haga clic en la dirección URL del Centro de administración de Microsoft 365 para aceptar la nueva relación del partner y el contrato, recibirá el mensaje "Póngase en contacto con su partner para confirmar que acepta el Contrato de cliente de Microsoft".  

**Para resolverlo**: debes dar fe en nombre del cliente.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Confirmación de que un cliente ha aceptado el contrato

Si intenta crear un nuevo pedido para un cliente existente al que no has confirmado con anterioridad, recibirá un aviso para completar la confirmación. Usa el siguiente procedimiento para hacerlo.

1. Escribe el **Nombre**, los **Apellidos**, la **Dirección de correo electrónico** y el **Número de teléfono** (opcional) del usuario que aceptó el contrato.

2. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.

3. Selecciona **Guardar y continuar**. 

## <a name="next-steps"></a>Pasos siguientes

- [Comprobar o actualizar la información del perfil de empresa](update-your-partner-profile.md)
- [Contratos de cliente de Microsoft (por región, idioma)](Agreements.md)
