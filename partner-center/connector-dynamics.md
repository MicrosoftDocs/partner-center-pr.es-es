---
title: El conector de venta conjunta para el centro de Partners de Dynamics 365 CRM
ms.topic: how-to
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronice sus referencias en el centro de Partners con el conector de venta conjunta para Dynamics 365 CRM. A continuación, los vendedores pueden colaborar con Microsoft desde los sistemas CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: c92938bbb4ffa6875419d06a9bbf23010ee60724
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947827"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Conector de venta conjunta para Dynamics 365 CRM: información general

### <a name="appropriate-roles"></a>Roles adecuados

- Administrador de referencias
- Administrador del sistema o Personalizador del sistema en CRM

El conector de la venta conjunta del centro de Partners permite que los vendedores covendan con Microsoft desde los sistemas CRM. No tendrán que estar capacitados para utilizar el centro de partners para administrar las ofertas de venta conjunta. Use los conectores de venta conjunta para crear una nueva referencia de venta conjunta con el fin de invitar a un vendedor de Microsoft, recibir referencias del vendedor de Microsoft, aceptar o rechazar referencias, modificar el trato de los datos, como el valor del trato y la fecha de cierre. También puede recibir cualquier actualización de los vendedores de Microsoft en estos acuerdos de venta conjunta. Puede realizar todas las referencias en el CRM de su elección, en lugar de hacerlo en el centro de Partners. 

La solución se basa en la solución Microsoft Power Automate y usa las API del centro de Partners.

## <a name="before-you-install---pre-requisites"></a>Antes de instalar: requisitos previos

|**Temas**   |**Detalles**   |**Vínculos**   |
|--------------|--------------------|------|
|IDENTIFICADOR de Microsoft Partner Network |Necesita un ID. de MPN válido|Para unirse a [MPN](https://partner.microsoft.com/)|
|Lista de coventas|La solución de IP/servicios debe estar lista para su venta conjunta.|[Venda con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Cuenta de Centro de partners|El identificador de MPN asociado al inquilino del centro de Partners debe ser el mismo que el identificador de MPN asociado a la solución de venta conjunta. Compruebe que puede ver las referencias de venta conjunta en el portal del centro de Partners antes de implementar los conectores.|[Administración de la cuenta](create-user-accounts-and-set-permissions.md)|
|Roles de usuario del Centro de partners|El empleado que va a instalar y usar los conectores debe ser un administrador de referencias.|[Asignar roles y permisos de usuarios](create-user-accounts-and-set-permissions.md)| |Dynamics 365 CRM|El rol de usuario CRM es administrador del sistema o Personalizador del sistema|[Asignación de roles en Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Cuenta de flujo de automatización de energía|Una cuenta activa de [Power Automatic](https://flow.microsoft.com) para el administrador del sistema CRM o el personalizador del sistema. Dicho usuario debe iniciar sesión en [Power automatizate](https://flow.microsoft.com) al menos una vez antes de la instalación.|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Instalación de la sincronización de referencias del centro de partners para Dynamics 365 (solución de automatización de energía)

1. Vaya a [Power Automatic](https://flow.microsoft.com) y seleccione **entornos** en la esquina superior derecha. Este paso le mostrará las instancias de CRM disponibles.

2. Seleccione la instancia de CRM correspondiente en la lista desplegable de la esquina superior derecha.

3. Seleccione **soluciones** en la barra de navegación izquierda.

4. Haga clic en el vínculo **abrir AppSource** en el menú superior.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abrir AppSource":::

5. Busque **conectores de referencias del centro de partners para Dynamics365** en la pantalla emergente.  

6. Haga clic en el botón **obtener ahora** y **continúe**.

7. Se abrirá la página en la que puede seleccionar el entorno de CRM (Dynamics 365) para instalar la aplicación.  Acepte los términos y condiciones.

8. A continuación, se le dirigirá a la página **administrar soluciones** .  Vaya a "referencias del centro de Partners" con los botones de flecha de la parte inferior de la página. La **instalación programada** debe aparecer junto a la solución de referencias del centro de Partners. La instalación tardará 10-15 minutos. 

9. Una vez completada la instalación, vuelva a [Power Automatic](https://flow.microsoft.com) y seleccione **soluciones** en el área de navegación izquierda. Observe que la **sincronización de las referencias del centro de partners para Dynamics 365** está disponible en la lista de soluciones.

10. Seleccione la **sincronización de referencias del centro de partners para Dynamics 365**. Están disponibles los siguientes flujos y entidades:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="CRMS disponibles":::

## <a name="best-practice-test-before-you-go-live"></a>Procedimiento recomendado: prueba antes de la marcha

Antes de instalar, configurar y personalizar la solución Power Automate en el entorno de producción, asegúrese de probar la solución en una instancia de CRM provisional.

- Instale la solución Microsoft Power Automate en un entorno de ensayo o una instancia de CRM.
- Realice una copia de la solución y ejecute la configuración y la automatización de las personalizaciones de flujo en el entorno de ensayo.
- Pruebe la solución en una instancia de ensayo o CRM. 
- En caso de éxito, importe como solución administrada a la instancia de producción. 

## <a name="configure-the-solution"></a>Configuración de la solución

1. Una vez que haya instalado la solución en la instancia de CRM, vuelva a [Power Automatic](https://flow.microsoft.com/).


2. En la lista desplegable de **entornos** de la esquina superior derecha, seleccione la instancia de CRM en la que instaló la solución Power Automatic.

3. Deberá crear conexiones que asocien las tres cuentas de usuario:

   - Usuario del centro de Partners con credenciales de administrador de referencias

   - Eventos del Centro de partners

   - Administrador de CRM con la potencia que automatiza los flujos en la solución.

      1. Seleccione **conexiones** en la barra de navegación izquierda y seleccione la solución "referencias del centro de Partners" en la lista.

      2. Cree una conexión haciendo clic en **crear una conexión**.

         :::image type="content" source="images/cosellconnectors/dynamics1.png" alt-text="Crear conexión":::

      3. Busque **referencias del centro de Partners (versión preliminar)** en la barra de búsqueda en la esquina superior derecha.

      4. Cree una conexión para el usuario del centro de Partners con el rol de credenciales de administrador de referencias.

      5. A continuación, cree una conexión de eventos del centro de partners para el usuario del centro de Partners con las credenciales de administrador de referencias.

      6. Cree una conexión para Common Data Service (entorno actual) para el usuario administrador de CRM.
       
     
      7. Una vez que haya agregado todas las conexiones, debería ver las siguientes conexiones en su entorno:

:::image type="content" source="images/cosellconnectors/dynamics2.png" alt-text="Conexiones":::
   
## <a name="edit-the-connections"></a>Editar las conexiones

1. Vuelva a la página **soluciones** y seleccione **solución predeterminada**. Haga clic en **todo** para seleccionar **referencia de conexión (vista previa)** .

:::image type="content" source="images/cosellconnectors/dynamics3.png" alt-text="Conexión":::

2. Edite cada una de las conexiones de una en una; para ello, seleccione el icono de tres puntos. Agregue las conexiones correspondientes.

:::image type="content" source="images/cosellconnectors/dynamics4.png" alt-text="Conexiones enumeradas"::: 

3.  Active los flujos en la secuencia siguiente:
- Registro del webhook del centro de Partners (versión preliminar de Insider)
- Creación de una referencia de venta conjunta: Dynamics 365 al centro de Partners (versión preliminar de Insider)
- Centro de Partners: actualizaciones de referencia de venta conjunta de Microsoft a Dynamics 365 (versión preliminar de Insider)
- Centro de partners a Dynamics 365 (versión preliminar de Insider)
- Dynamics 365 al centro de Partners (versión preliminar de Insider)
- Oportunidad de Dynamics 365 al centro de Partners (versión preliminar de Insider)
- Dynamics 365 Microsoft Solutions to partner Center (versión preliminar de Insider)
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Uso de las API de webhook para registrar eventos de cambio de recursos

Las API del webhook del centro de Partners le permiten registrarse para los eventos de cambio de recursos. Estos eventos de cambio se envían a la dirección URL como publicaciones HTTP.

1. Para registrar la dirección URL, seleccione **registro de webhook del centro de Partners (versión preliminar de Insider)** flujo de automatización.

2. Agregar conexiones para (a) el usuario del centro de Partners con credenciales de administrador de referencias (b.) eventos del centro de partners como se resaltan a continuación

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Desencadenador":::

3. Cuando realice estas actualizaciones, verá

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. Guarde los cambios y seleccione **Activar**.

   Para permitir que los webhooks del centro de Partners escuchen los cambios de eventos, siga estos pasos:

5. Seleccione **centro de partners para Dynamics 365 (versión preliminar de Insider)**.

6. Seleccione el icono de **edición** y seleccione **cuando se reciba una solicitud HTTP**.

7. Seleccione el icono de **copiar** para copiar la dirección URL http post proporcionada.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copiar la dirección URL":::

8. Ahora, seleccione "registro de webhook del centro de Partners (versión preliminar de Insider)" flujo automático de energía y seleccione **Ejecutar**.

9. Asegúrese de que se abre la ventana "flujo de ejecución" en el panel derecho y haga clic en **continuar**.

10. Escriba la siguiente información:

    1. **Punto de conexión de desencadenador http**: dirección URL copiada del paso anterior

    2. **Eventos para registrar**: "referencia creada" y "referencia-actualizada"

    3. **Sobrescribir puntos de conexión de desencadenador existentes si están presentes**: sí (esto Sobrescribe todos los extremos existentes).

11. Seleccione **Ejecutar** y, a continuación, haga clic en **listo.**

Ahora, el webhook puede escuchar la creación y actualización de eventos.

## <a name="customize-synchronization-steps"></a>Personalizar pasos de sincronización

Cuando se sincronizan las referencias de venta conjunta entre el centro de Partners y el sistema CRM, los campos que se sincronizan en el equipo del centro de Partners se enumeran aquí.

A menudo, los sistemas CRM son muy personalizados. Puede personalizar los flujos de automatización. Siga la guía de asignación de campos y, si es necesario, realice los cambios adecuados en los pasos de la potencia que automatiza los flujos.  Se proporcionan las asignaciones de Microsoft Partner Center a CRM, pero en función de su entorno de CRM, puede optar por personalizar aún más los campos.

Se pueden personalizar varios pasos de cada uno de los flujos de potencia automatizados en función de sus necesidades. Estos son algunos ejemplos de las personalizaciones disponibles:

1. Para personalizar los campos de los eventos de creación o actualización en el centro de partners para la sincronización de referencias de CRM: 

    a. Seleccione centro de partners para Dynamics 365 (versión preliminar de Insider) o centro de partners a Salesforce (versión preliminar de Insider).

    b. Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.

    c. Seleccione **(ámbito) sincronizar el cliente potencial o la oportunidad**.

2. Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para crear eventos, seleccione si se trata de una **nueva oportunidad compartida y, a continuación**, haga clic en. Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda **crear una nueva oportunidad en CRM**. Puede editar las asignaciones en esta sección mediante la guía de asignación de campos.

    d. Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para los eventos de actualización, haga clic en el paso "(ámbito) sincronizar el cliente potencial o la oportunidad".

    e. Seleccione **si se trata de una actualización de una oportunidad**. Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda **si la diferencia entre los objetos de oportunidad del centro de Partners y CRM**.  

    f. Seleccione **si sí** seguido de **Actualizar oportunidad existente** .

3. Para personalizar los campos de la sincronización de referencia de CRM a equipo para eventos de actualización:

    a. Seleccione **Editar**  para editar o personalizar el flujo de Power Automatic.

    b. Seleccione **(ámbito) sincronizar la oportunidad**.

    c. Para personalizar las asignaciones de campos de CRM para los eventos de actualización, seleccione **si hay diferencias entre los objetos de cliente potencial del centro de Partners y CRM y, a continuación, haga clic en**. 

    d. Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda el paso **actualizar una referencia con los datos de oportunidad**.

   Puede editar las asignaciones en esta sección basándose en la guía de asignación de campos.

4. Para personalizar los campos de la sincronización de referencia de CRM a equipo para crear eventos

   a. Seleccione **Editar**  para editar o personalizar el flujo de Power Automatic.

   b. Seleccione **(ámbito) sincronizar referencias.**

   c. Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para crear eventos, seleccione **crear referencia de Microsoft**.

   Puede editar las asignaciones en esta sección basándose en la guía de asignación de campos.

Se han creado dos variables de entorno:

- Marca de verificación: indica si necesitaría un icono de marca de verificación además de las oportunidades que se sincronizan bidireccionalmente entre el centro de Partners y Dynamics 365 CRM.

- Sincronizar solo las oportunidades de venta conjunta: significa si desea sincronizar solo las oportunidades de venta conjunta.

Puede optar por editar el valor predeterminado de las variables de entorno.

:::image type="content" source="images/cosellconnectors/dynamics5.png" alt-text="Cuadro de edición para los valores predeterminados":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronización de referencia de venta conjunta bidireccional de un extremo a otro

Una vez que haya instalado, configurado y personalizado la solución Power Automate, puede probar la sincronización de referencias de venta conjunta entre Dynamics 365 y el centro de Partners.

### <a name="pre-requisites"></a>Requisitos previos

Para sincronizar las referencias entre el centro de Partners y Dynamics 365 CRM, la solución Power Automate marca claramente los campos de referencia específicos de Microsoft. Esta identificación proporciona a los equipos de vendedores la capacidad de decidir qué referencias desean compartir con Microsoft para la venta conjunta.

Un conjunto de campos personalizados está disponible como parte de la entidad de **oportunidad** . Un usuario administrador de CRM tendrá que crear una sección de CRM independiente con los campos personalizados de la **oportunidad** .

Los siguientes campos personalizados deben formar parte de la sección CRM:

- **Sincronizar con el centro de Partners**: si se va a sincronizar la oportunidad con el centro de Partners de Microsoft

- **Identificador de referencia**: un campo de identificador de solo lectura para la referencia del centro de Partners de Microsoft

- **Vínculo de referencia**: un vínculo de solo lectura a la referencia en el centro de Partners de Microsoft

- **¿Cómo puede ayudarle Microsoft?**: ayuda necesaria de Microsoft para la referencia

- **Productos**: lista de productos asociados a esta oportunidad

- **Audit**: una pista de auditoría de solo lectura para la sincronización con las referencias del centro de Partners

Actualice el formulario de la oportunidad en Dynamics 365 CRM para incluir el campo soluciones para productos.

:::image type="content" source="images/cosellconnectors/dynamics6.png" alt-text="Formulario de la oportunidad":::

:::image type="content" source="images/cosellconnectors/dynamics7.png" alt-text="{alt-text}":::

### <a name="scenarios"></a>SITUACIÓN

1. Sincronización de referencia cuando se crea o actualiza una referencia en CRM y se sincroniza en el centro de Partners:

   1. Inicie sesión en el entorno de CRM de Dynamics 365 con un usuario que tenga visibilidad en la sección de **oportunidades** de CRM.

   2. Asegúrese de que la siguiente sección está presente al crear una "nueva oportunidad" en el entorno de Dynamics 365

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Sección de la oportunidad de ejemplo que muestra la información del centro de Partners de Microsoft en Dynamics 365.":::

   3. Para sincronizar esta oportunidad con el centro de Partners de Microsoft, asegúrese de establecer los siguientes campos en la vista tarjeta:

      - **Sincronizar con el centro de Partners**: sí

      - **¿Cómo puede ayudarle Microsoft?**: Seleccione una de las siguientes opciones:

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Sección de la oportunidad de ejemplo en Dynamics 365 que muestra las opciones de ayuda del centro de Partners de Microsoft junto a un campo llamado ¿Cómo puede ayudarle Microsoft?":::

      - **Productos**: identificadores de la solución del producto

   4. Una vez creada la oportunidad en Dynamics 365 con la opción **sincronizar con el centro de Partners** establecida en **sí**, espere 10 minutos y, a continuación, inicie sesión en su cuenta del centro de Partners. Las referencias se sincronizarán con Dynamics 365.

   5. Del mismo modo, para una oportunidad que tuviera la opción "sincronizar con el centro de Partners" establecida en "sí", si actualizas la oportunidad en Dynamics 365 CRM, los cambios se sincronizarán en la cuenta del centro de Partners.

   6. Las oportunidades que se sincronizan correctamente con el centro de Partners se identificarán con ✔ icono en Dynamics 365.

2. Sincronización de referencia cuando se crea o actualiza una referencia en el centro de Partners de Microsoft y se sincroniza en el entorno de Dynamics 365:

   1. Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard/home)del centro de Partners.

   2. Seleccione **referencias** en el menú de la izquierda.

   3. Cree una nueva referencia de venta conjunta desde el centro de partners; para ello, haga clic en la opción "nuevo trato".

   4. Inicie sesión en el entorno de CRM de Dynamics 365.

   5. Vaya a **abrir oportunidades**. La referencia creada en el centro de Partners de Microsoft ya está sincronizada en Dynamics 365 CRM.

   6. Al seleccionar una referencia sincronizada, se rellenan los detalles de la vista de tarjeta.

## <a name="next-steps"></a>Pasos siguientes

- [Administrar los clientes potenciales](manage-leads.md)

- [Administrar las oportunidades de venta conjunta](manage-co-sell-opportunities.md)

- [¿Más información sobre la plataforma Microsoft Power Automate?](/power-automate/)

- [Webhooks del Centro de partners](/partner-center/develop/partner-center-webhooks)