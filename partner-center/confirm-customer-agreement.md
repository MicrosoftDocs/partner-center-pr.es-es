---
title: Confirmación de la aceptación por parte del cliente del Contrato de cliente de Microsoft | Centro de partners
ms.topic: article
ms.date: 02/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Obtén información sobre cómo confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft. Puede ser necesario para hacer pedidos de productos y servicios de Microsoft para los clientes.
author: LauraBrenner
ms.author: labrenne
keywords: customer, customers, consent, MCA, Microsoft Cloud Agreement, Microsoft Customer Agreement, customer agreement templates
ms.localizationpriority: high
ms.openlocfilehash: c9445ae24de16d25cf887299521eef8d6d793c6f
ms.sourcegitcommit: 5f31ca4a9bd8fd7e69e019476ac72836606d87da
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/04/2020
ms.locfileid: "77012199"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Confirmación de la aceptación por parte del cliente del Contrato de cliente de Microsoft

**Se aplica a**

- Centro de partners
- Centro de administración de Microsoft 365

**Roles adecuados**

- Agente de administrador
- Agente de ventas

**Tipos de partners adecuados**

- Revendedores indirectos, partners de facturación directa y proveedores indirectos


El 1 de octubre de 2019, Microsoft incorporó el **Contrato de cliente de Microsoft** en el programa CSP para reemplazar el Contrato de Microsoft Cloud. Lee las [instrucciones](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Fpartner-center%2Findirect-reseller-tasks-in-partner-center&data=02%7C01%7CChelsea.Kajs%40microsoft.com%7Cd5e0adc6b10646352ce508d7a4e84251%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637159189767080601&sdata=%2BPAWMBPVbVBkTx25r9CoD7cQxRqRVEYkxWIilrwwxZc%3D&reserved=0) adicionales para los revendedores indirectos.

 Para facilitar la migración de los asociados al nuevo contrato, se admitirá el Contrato de Microsoft Cloud actual en el programa CSP hasta el 31 de enero de 2020. Los partners pueden confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft en el Centro de partners o bien, ahora, pueden optar por invitar al cliente a través de una dirección URL para que revise y acepte el contrato en el Centro de administración de Microsoft 365 autenticado. Para obtener más detalles sobre la línea de tiempo, consulta la tabla siguiente:

| Fecha | Hito | Detalles |
|------------|------------|--------------------------------|
|01 de agosto de 2019|Versión preliminar de la experiencia del usuario disponible en el espacio aislado|Los partners pueden confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft desde el panel del Centro de partners del entorno del espacio aislado de CSP. Los partners con acceso al entorno de espacio aislado de CSP pueden acceder a una versión preliminar de los cambios en la experiencia del usuario. Los partners sin acceso al espacio aislado pueden obtener información sobre los cambios en este tema.|
|03 de septiembre de 2019|Hay una versión preliminar de la API disponible en el espacio aislado.|El partner puede confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft desde la API del Centro de partners del entorno del espacio aislado de CSP. Los partners de la API pueden usar esta oportunidad para acceder a una versión preliminar de los cambios de la API y comenzar a trabajar en la integración de la API para admitir el nuevo contrato.|
|20 de septiembre de 2019|Hay una versión preliminar del SDK de .NET disponible en el espacio aislado.|El asociado puede confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft mediante el SDK de .NET del Centro de partners del entorno del espacio aislado de CSP. Los asociados de la API pueden usar esta oportunidad para acceder a una versión preliminar de los cambios del SDK de .NET y comenzar a trabajar en la integración de la API para admitir el nuevo contrato.|
|01 de octubre de 2019|Contrato de cliente de Microsoft disponible en el entorno de producción|Microsoft introducirá el Contrato de cliente de Microsoft en el programa CSP para reemplazar el Contrato de Microsoft Cloud. Los partners pueden confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft desde la API y el panel del Centro de partners en el entorno de producción. El Contrato de Microsoft Cloud sigue siendo compatible con el programa de partners de CSP. Sin embargo, es recomendable que los partners inicien la migración al Contrato de cliente de Microsoft. Las nuevas compras y los cambios en el recuento de puestos de las suscripciones existentes requerirán la confirmación por parte del partner del Contrato de cliente de Microsoft o del Contrato de Microsoft Cloud. Ciertas ofertas nuevas (por ejemplo, el nuevo plan de Azure) requerirán la confirmación del Contrato de cliente de Microsoft.|
|31 de enero de 2020|El Contrato de Microsoft Cloud se quitó de la producción|El Contrato de Microsoft Cloud ya no se acepta en el programa para partners de CSP. Las nuevas compras y los cambios en el recuento de puestos de las suscripciones existentes requerirán que el partner confirme el Contrato de cliente de Microsoft. Este requisito se aplica a los clientes nuevos y a los clientes existentes que puedan haber aceptado previamente el Contrato de Microsoft Cloud.|
|3 de febrero de 2020|El partner ahora tiene la opción de invitar al cliente a través de una dirección URL para que revise y acepte el contrato en el Centro de administración de Microsoft 365 autenticado. | El cliente puede aceptar el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365. Mediante la aceptación directa del contrato en el Centro de administración de Microsoft 365, el cliente confirma la aprobación de los términos. 

Tienes las dos opciones siguientes para que los clientes acepten el Contrato de cliente de Microsoft.  

**Opción 1**: atestación del partner de la aceptación del cliente; el partner puede confirmar la aceptación del cliente mediante el SDK o la API del Centro de partners o a través del panel del Centro de partners.

**Opción 2**: aceptación directa del cliente; el partner puede invitar al cliente a través de una dirección URL para que revise y acepte el contrato en el Centro de administración de Microsoft 365.

## <a name="access-microsoft-customer-agreement-template"></a>Acceso a la plantilla del Contrato de cliente de Microsoft

Puedes descargar manualmente la versión más reciente de la plantilla del Contrato de cliente de Microsoft desde [aquí](https://aka.ms/customeragreement). Ten en cuenta que el Contrato de cliente de Microsoft es específico para cada país. Al solicitar la plantilla del Contrato de cliente de Microsoft, asegúrate de seleccionar el país correcto en función de la ubicación del cliente. 

## <a name="option-1-confirm-customer-acceptance-using-partner-center-apisdk"></a>Opción 1: Confirmación de la aceptación por parte del cliente mediante el SDK o la API del Centro de partners

Puedes usar el SDK o la API del Centro de partners para confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft. Para obtener más información sobre el SDK o la API, consulta:

- [Obtener los metadatos del acuerdo del Contrato de cliente de Microsoft](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [Confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Obtener confirmación de la aceptación por parte del cliente del Contrato de cliente de Microsoft](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [Obtener un vínculo de descarga para la plantilla del Contrato de cliente de Microsoft](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)

## <a name="confirm-customer-acceptance-in-partner-center"></a>Confirmación de la aceptación por parte del cliente en el Centro de partners

Los partners pueden confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft en el Centro de partners para clientes nuevos y clientes existentes. Los revendedores no pueden dar fe en nombre de sus clientes y deben colaborar con su proveedor indirecto para completar la atestación.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Confirmar la aceptación de los clientes nuevos

Si creas un nuevo inquilino de cliente en el Centro de partners, sigue los pasos que se describen a continuación para confirmar la aceptación del cliente del Contrato de cliente de Microsoft. Para poder seguir estos pasos, debes ser agente de administración o de ventas.

1. Selecciona **Clientes** y, a continuación, **Nuevo cliente**.

2. En **Información de cuenta**, especifica los datos de la empresa y su contacto principal.

3. En **Contrato de Microsoft**, selecciona el cuadro para dar fe de que el cliente ha aceptado el Contrato de cliente de Microsoft. 

4. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.

5. Comprueba que la información de contacto del usuario principal que se muestra sea correcta. Si no lo es, selecciona **Actualizar** y escribe el **Nombre**, los **Apellidos**, la **Dirección de correo electrónico** y el ***Número de teléfono** (opcional) de la persona que ha aceptado el contrato.

6. Selecciona **Siguiente** para continuar con los pasos restantes para crear el inquilino del cliente.

![Cliente nuevo](images/mca/newcustomeragreement.jpg)  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Confirmar la aceptación de los clientes existentes

Debes ser agente de administración o de ventas para poder hacer esto:

1. Selecciona **Clientes**. Busca y selecciona el cliente.

2. Selecciona **Información de cuenta**.

3. En **Contrato de cliente de Microsoft**, selecciona **Actualizar**.

4. Escribe el **Nombre**, los **Apellidos**, la **Dirección de correo electrónico** y el **Número de teléfono** (opcional) de la persona que aceptó el contrato. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.

5. Selecciona **Guardar** y continúa.

![Cliente existente](images/mcua2.png)

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Recuperar la confirmación de la aceptación del cliente

Sigue los pasos que se describen a continuación para recuperar la confirmación de que un cliente existente ha aceptado el Contrato de cliente de Microsoft. Debes ser agente de administración o agente de ventas para poder hacer esto.

1. Selecciona **Clientes** y, a continuación, busca y selecciona el cliente que quieras ver.

2. Selecciona **Información de cuenta**.

3. En **Contrato de cliente de Microsoft**, consulta si el cliente ha proporcionado la confirmación.

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Opción 2: Aceptación del cliente en el Centro de administración de Microsoft 365

Los partners pueden invitar a clientes nuevos y existentes, a través de una dirección URL, para que revisen y acepten el contrato en el Centro de administración de Microsoft 365. En las siguientes secciones se muestra cómo puedes:

- Crear un cliente nuevo e invitarlo para que revise y acepte el contrato.

- Invitar a un cliente nuevo para que revise y acepte la relación y el contrato de revendedor

- Invitar a un cliente existente para que revise y acepte el contrato

## <a name="create-a-net-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Crear un cliente nuevo e invitarlo para que revise y acepte el contrato.

Sigue los pasos que se indican a continuación para crear un cliente nuevo en el Centro de partners e invitarlo para que revise y acepte el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365.

1. En la pestaña **Clientes** del Centro de partners, selecciona **Agregar cliente**.

2. En **Información de la cuenta**, escribe la información sobre el nuevo cliente en todos los campos obligatorios, incluido el nombre de la empresa del cliente y el contacto principal.

3. En **Contrato de cliente**, selecciona la primera opción, que es **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center** (Se pedirá al cliente que acepte el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365). Completa los demás campos obligatorios en la página.

4. Selecciona **Siguiente: revisión** y sigue los pasos para crear el inquilino del cliente. (Nota: Los clientes nuevos no pueden hacer nuevas compras hasta que acepten el Contrato de cliente de Microsoft).  

![Crear un cliente nuevo](images/mca/create-new-customer.jpg)

5. Cuando llegues a la pantalla **Confirmación** del nuevo flujo de trabajo del cliente, guarda las credenciales del cliente. Deberás proporcionar estas credenciales al cliente más adelante.

6. Fuera del Centro de partners, crea y envía un correo electrónico en el que invites al cliente a aceptar el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365. Asegúrate de incluir los elementos siguientes en el correo electrónico:

   - Un vínculo a esta[ dirección URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (inicio de sesión obligatorio)
   - Las credenciales del cliente que guardaste en el paso 5

7. A continuación, el cliente recibirá la invitación por correo electrónico del partner y seleccionará la [dirección URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. El cliente deberá iniciar sesión en el Centro de administración de Microsoft 365 con las credenciales del cliente que recibió previamente del partner.

9. A continuación, el cliente marcará la casilla para aceptar el Contrato de cliente de Microsoft.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Invitación de un cliente nuevo para que revise y acepte la relación de revendedor y el Contrato de cliente de Microsoft 

Usa los pasos siguientes para invitar a un nuevo cliente para que revise y acepte la relación de revendedor y el Contrato de cliente de Microsoft. 

1. En la pestaña **Clientes** en el Centro de partners, selecciona el vínculo **Solicitar una relación de revendedor**. 

2. Se generará una plantilla de correo electrónico automática, que incluirá texto y una dirección URL parametrizada que dirigirá al cliente al Centro de administración de Microsoft 365.

3. Puedes personalizar la plantilla de correo electrónico generada automáticamente y, a continuación, seleccionar **Copiar al portapapeles** o **Abrir en correo**.

4. Usa esta plantilla de correo electrónico para invitar al cliente a aceptar la solicitud de **relación de revendedor** y el **Contrato de cliente de Microsoft**. (Nota: En la invitación por correo electrónico, asegúrate de que el partner también incluye la dirección URL que se proporcionó automáticamente, así como las credenciales del cliente que se crearon recientemente).

![Crear una relación](images/mca/createrelationship.jpg)

5. El cliente recibirá una invitación por correo electrónico y hará clic en la dirección URL parametrizada. 

6. El cliente usará las credenciales proporcionadas por el partner en el correo electrónico para iniciar sesión en el Centro de administración de Microsoft 365.

7. El cliente marcará la casilla para aceptar la **relación de revendedor** y el **Contrato de cliente de Microsoft**. 

8. En la misma dirección URL, el cliente podrá ver una lista consolidada de los diferentes partners con los que trabaja. Podrá seleccionar un partner para ver los detalles.

![Aceptar el contrato](images/mca/accept.jpg)

## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Invitación de un cliente existente para que revise y acepte el contrato

Usa los pasos siguientes para invitar a un cliente existente para que revise y acepte el Contrato de cliente de Microsoft. 

1. Crea el correo electrónico del cliente con la dirección URL incrustada para invitar a tu cliente para que acepte el Contrato de cliente de Microsoft.

2. El cliente recibirá la invitación por correo electrónico y hará clic en la [dirección URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. El cliente escribirá sus credenciales en el Centro de administración de Microsoft 365.

4. El cliente marcará la casilla para aceptar el Contrato de cliente de Microsoft. 

5. En la misma dirección URL, el cliente podrá ver la lista consolidada de los diferentes partners con los que trabaja. Podrá seleccionar un partner para ver los detalles.

![cliente](images/mca/customeraccept.png)

>[!NOTE]
>En determinados escenarios, es posible que los clientes no puedan aceptar directamente el Contrato de cliente de Microsoft. Para obtener más información acerca de estas situaciones, consulta [Dos escenarios en los que es necesario dar fe en nombre de tu cliente](attest-acceptance-customer-agreement.md).
