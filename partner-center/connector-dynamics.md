---
title: El conector de venta conjunta para el centro de Partners de Dynamics 365 CRM
ms.topic: how-to
ms.date: 03/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizar las referencias del centro de Partners con el conector de venta conjunta para Dynamics 365 CRM. A continuación, los vendedores pueden colaborar con Microsoft desde los sistemas CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 10062fd20e3553856d8b595efd3224ff456c2c49
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756793"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a>Conector de venta conjunta para Dynamics 365 CRM: información general

### <a name="appropriate-roles"></a>Roles adecuados

- Administrador de referencias
- Administrador del sistema o Personalizador del sistema en CRM

El conector de la venta conjunta del centro de Partners permite que los vendedores covendan con Microsoft desde los sistemas CRM. No tendrán que estar capacitados para utilizar el centro de partners para administrar las ofertas de venta conjunta. Use los conectores de venta conjunta para crear una nueva referencia de venta conjunta con el fin de invitar a un vendedor de Microsoft, recibir referencias del vendedor de Microsoft, aceptar o rechazar referencias, modificar el trato de los datos, como el valor del trato y la fecha de cierre. También puede recibir cualquier actualización de los vendedores de Microsoft en estos acuerdos de venta conjunta. Puede administrar todas las referencias en el CRM de su elección, en lugar de hacerlo en el centro de Partners. 

La solución se basa en la solución Microsoft Power Automate y usa las API del centro de Partners.

## <a name="before-you-install---pre-requisites"></a>Antes de instalar: requisitos previos

|**Temas**   |**Detalles**   |**Vínculos**   |
|--------------|--------------------|------|
|IDENTIFICADOR de Microsoft Partner Network |Necesita un ID. de MPN válido|Para unirse a [MPN](https://partner.microsoft.com/)|
|Listo para la venta conjunta|La solución de IP/servicios debe estar lista para su venta conjunta.|[Venda con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Cuenta de Centro de partners|El identificador de MPN asociado al inquilino del centro de Partners debe ser el mismo que el identificador de MPN asociado a la solución de venta conjunta. Compruebe que puede ver las referencias de venta conjunta en el portal del centro de Partners antes de implementar los conectores.|[Administración de la cuenta](create-user-accounts-and-set-permissions.md)|
|Roles de usuario del Centro de partners|El empleado que va a instalar y usar los conectores debe ser un administrador de referencias.|[Asignar roles y permisos de usuarios](create-user-accounts-and-set-permissions.md)| 
|Dynamics 365 CRM|El rol de usuario CRM es administrador del sistema o Personalizador del sistema|[Asignación de roles en Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Cuenta de flujo de automatización de energía|Cree un nuevo entorno de producción con base de datos para pruebas, ensayo y producción. Si tiene un entorno de producción existente con una base de datos, se puede volver a usar. El usuario que vaya a instalar la solución de conector debe tener energía automatizada y obtener acceso a este entorno. Puede supervisar el progreso y obtener más detalles en caso de que se produzca un error en la instalación de [Power Automatic](https://flow.microsoft.com/) ; para ello, haga clic en Ver historial en soluciones.|[Crear o administrar un entorno](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Instalación de la sincronización de referencias del centro de partners para Dynamics 365 (solución de automatización de energía)

1. Vaya a [Power Automatic](https://flow.microsoft.com) y seleccione **entornos** en la esquina superior derecha. Este paso le mostrará las instancias de CRM disponibles.

2. Seleccione la instancia de CRM correspondiente en la lista desplegable de la esquina superior derecha.

3. Seleccione **soluciones** en la barra de navegación izquierda.

4. Haga clic en el vínculo **abrir AppSource** en el menú superior.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abrir AppSource":::

5. Busque **conectores de referencias del centro de partners para Dynamics365** en la pantalla emergente.  

6. Haga clic en el botón **obtener ahora** y **continúe**.

7. Se abrirá la página en la que puede seleccionar el entorno de CRM (Dynamics 365) para instalar la aplicación.  Acepte los términos y condiciones.

8. Puede supervisar el progreso y obtener más detalles en caso de que se produzca un error en la instalación de Power Automatic; para ello, haga clic en **Ver historial** en **soluciones**.
 

9. Una vez completada la instalación, vuelva a [Power Automatic](https://flow.microsoft.com) y seleccione **soluciones** en el área de navegación izquierda. Observe que la **sincronización de las referencias del centro de partners para Dynamics 365** está disponible en la lista de soluciones.

10. Seleccione la **sincronización de referencias del centro de partners para Dynamics 365**. Están disponibles los siguientes flujos y entidades:

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="CRMS disponibles":::

## <a name="best-practice-test-before-you-go-live"></a>Procedimiento recomendado: prueba antes de la marcha

Antes de instalar, configurar y personalizar la solución Power Automate en el entorno de producción, asegúrese de probar la solución en una instancia de CRM provisional.

- Instale la solución Microsoft Power Automate en un entorno de ensayo o una instancia de CRM.
- Configure y personalice la solución Microsoft Power Automate en el entorno de ensayo.
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

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Crear conexión":::

      3. Busque **referencias del centro de Partners (versión preliminar)** en la barra de búsqueda en la esquina superior derecha.

      4. Cree una conexión para el usuario del centro de Partners con el rol de credenciales de administrador de referencias.

      5. A continuación, cree una conexión de eventos del centro de partners para el usuario del centro de Partners con las credenciales de administrador de referencias.

      6. Cree una conexión para Common Data Service (entorno actual) para el usuario administrador de CRM.
     
      7. Una vez que haya agregado todas las conexiones, debería ver las siguientes conexiones en su entorno:

:::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Conexiones":::
   
## <a name="edit-the-connections"></a>Editar las conexiones

1. Vuelva a la página **soluciones** y seleccione **solución predeterminada**. Haga clic en **todo** para seleccionar **referencia de conexión (vista previa)** .

:::image type="content" source="images/connection-reference-video.gif" alt-text="Editar las conexiones":::

2. Edite cada una de las conexiones de una en una; para ello, seleccione el icono de tres puntos. Agregue las conexiones correspondientes.

:::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Conexiones enumeradas"::: 

3.  Vuelva a la página soluciones, seleccione la sincronización de referencias del centro de partners para Dynamics 365 y active el flujo haciendo clic en el icono de tres puntos junto a cada flujo en la siguiente secuencia. Si encuentra algún problema al activar el flujo, consulte pasos de [Personalización](connector-dynamics.md#customize-synchronization-steps) y [pasos para solucionar problemas](connectors-troubleshoot.md). 

Active los flujos en la secuencia siguiente:

- Registro del webhook del centro de Partners (versión preliminar de Insider)
- Creación de una referencia de venta conjunta: Dynamics 365 al centro de Partners (versión preliminar de Insider)
- Personalícela Creación u obtención de detalles del flujo de Dynamics 365 
- Centro de partners a Dynamics 365: Ayudante (versión preliminar de Insider)
- Centro de Partners: actualizaciones de referencia de venta conjunta de Microsoft a Dynamics 365 (versión preliminar de Insider)
- Centro de partners a Dynamics 365 (versión preliminar de Insider)
- Dynamics 365 al centro de Partners (versión preliminar de Insider)
- Oportunidad de Dynamics 365 al centro de Partners (versión preliminar de Insider)
- Dynamics 365 Microsoft Solutions to partner Center (versión preliminar de Insider)
 

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Uso de las API de webhook para registrar eventos de cambio de recursos

Las API del webhook del centro de Partners le permiten registrarse para los eventos de cambio de recursos. Estos eventos de cambio se envían a la dirección URL como publicaciones HTTP.

1. Seleccione **centro de partners para Dynamics 365 (versión preliminar de Insider)**.

2. Seleccione el icono de **edición** y seleccione **cuando se reciba una solicitud HTTP**.

3. Seleccione el icono de **copiar** para copiar la dirección URL http post proporcionada.

 :::image type="content" source="images/webhook-video.gif" alt-text="Uso de webhooks para registrar cambios de recursos":::

4. Seleccione el flujo "registro de webhook del centro de Partners (versión preliminar Insider)" y seleccione **Ejecutar**.

5. Asegúrese de que se abre la ventana "flujo de ejecución" en el panel derecho y haga clic en **continuar**.

6. Escriba la siguiente información:

   - **Punto de conexión de desencadenador http**: dirección URL copiada del paso anterior

   - **Eventos que se van a registrar**: seleccione todos los eventos disponibles ("referencia creada", "referencia-actualizada", "relacionado-referencia creada", "relacionada-referencia-actualizada")

   -**Sobrescribir puntos de conexión de desencadenador existentes si están presentes**: sí es importante tener en cuenta que solo se puede registrar una dirección URL para un evento de webhook determinado. Es importante tener en cuenta que solo se puede registrar una dirección URL para un evento de webhook determinado. 

7. Seleccione **Ejecutar** y, a continuación, haga clic en **listo.**

Ahora, el webhook puede escuchar la creación y actualización de eventos.

## <a name="customize-synchronization-steps"></a>Personalizar pasos de sincronización

Los sistemas CRM son muy personalizados y puede personalizar la solución Power Automatic en función de la configuración de CRM.  Cuando se sincronizan las referencias de venta conjunta entre el centro de Partners y el sistema CRM, los campos que se sincronizan en el equipo del centro de Partners se enumeran en la [Guía de asignación de campos personalizados](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Siga la guía de asignación de campos y, si es necesario, realice los cambios adecuados en **[personalizar] crear u obtener detalles de las variables de entorno o de flujo de Dynamics 365**  . Se recomienda no actualizar ningún otro flujo de la solución Power automatizate, ya que puede afectar a las actualizaciones de soluciones futuras. 

A continuación se enumeran las personalizaciones disponibles:

- Marca de verificación en el nombre de la oportunidad: de forma predeterminada, se mostrará una marca de verificación junto a nombre de la oportunidad para indicar que la sincronización entre el centro de Partners y Dynamics 365 CRM se está produciendo correctamente. Del mismo modo, se mostrará una marca cruzada si se produce un error de sincronización. Para evitar que se agreguen cheques o marcas cruzadas en el nombre de la oportunidad, establezca el valor actual de mostrar marca de verificación en la variable de entorno nombre de oportunidad en no.

- Valor de trato: de forma predeterminada, el valor de trato desde el centro de Partners se sincronizará con **estimatedvalue** en CRM. Si tiene un campo diferente en CRM para el valor de trato que se va a sincronizar desde:

    a.    Actualice el nombre del campo de valor de la variable de entorno de Dynamics 365 con el nombre de campo de CRM. Tenga en cuenta que debe proporcionar el nombre del campo, no su nombre para mostrar.

    b.    Editar **[personalizar] cree u obtenga detalles del flujo de Dynamics 365**  y vaya a **crear o actualizar** oportunidad en CRM y actualizar **crear una nueva oportunidad** y actualizar las acciones de la **oportunidad existentes** para asignar el valor de **DealValue** al campo correcto en CRM. Además, quite la **asignación DealValue** del campo **ingresos estimados** .

- Código de país de la cuenta de cliente: es obligatorio proporcionar un código de país de dos letras (ISO 3166) al crear una nueva referencia. De forma predeterminada, el código de país se sincronizará con el campo address1_country de la cuenta en CRM. Si tiene un campo diferente en CRM para el código de país que se va a sincronizar desde:

   a.    Para un campo de código de país que no sea de búsqueda en la cuenta que contiene el código de dos letras:

   - Actualice el nombre del campo de código de país de la cuenta de cliente en la variable de entorno Dynamics 365 con el nombre de campo de CRM. Tenga en cuenta que debe proporcionar el nombre del campo, no su nombre para mostrar.

   - Editar **[personalizar] cree u obtenga detalles del flujo de Dynamics 365**  y vaya a crear o a obtener cuenta de cliente en CRM acción para asignar el valor de país al campo correcto en CRM. Además, quite la asignación de valores de país de la dirección 1: campo de país o región.

   b.    Para un campo de código de país basado en búsquedas en la cuenta:

   - Agregue un nuevo campo personalizado en la cuenta y rellénelo automáticamente con el código de país de dos letras (ISO 3166) en función del valor seleccionado en campo basado en búsquedas y viceversa.

   - Siga los pasos anteriores para el campo de código de país que no es de búsqueda para sincronizar un nuevo campo personalizado desde CRM hacia y desde el centro de Partners.

- Campos de la oportunidad: si hay campos obligatorios en la oportunidad que deben rellenarse editar **[personalizar], cree u obtenga detalles del flujo de Dynamics 365**  y vaya a **crear o actualizar oportunidad** en CRM y actualizar **crear una nueva acción de oportunidad** para asignar valores a los campos obligatorios en función de los requisitos empresariales.

- Campos de clientes potenciales: si hay campos obligatorios en el cliente potencial que deben rellenarse editar **[personalizar], cree u obtenga detalles del flujo de Dynamics 365**  y vaya a **crear o actualizar clientes potenciales** en CRM y actualice **crear una nueva acción de cliente potencial** para asignar valores a los campos obligatorios en función de los requisitos de su empresa.

- Cuenta de cliente: cuando se sincroniza una nueva referencia desde el centro de partners a CRM, la solución de automatización de energía intenta buscar una cuenta existente en CRM con el nombre de la compañía del cliente y el código postal. Si no encuentra ninguna, se creará una nueva cuenta de cliente en CRM. Para actualizar los criterios de búsqueda y los detalles de creación de la nueva cuenta, edite **[personalizar] cree u obtenga detalles del flujo de Dynamics 365** y vaya a **crear u obtener una cuenta de cliente** en CRM y **crear la acción** de la cuenta de cliente.

## <a name="update-environment-variable"></a>Actualizar variable de entorno

Para actualizar un valor de variable de entorno:

1. Vaya a la página de **soluciones** y seleccione **solución predeterminada**. Seleccione **variable de entorno** haciendo clic en todo.

2. Seleccione la variable de entorno para el valor que debe actualizarse y haga clic en **Editar** con el icono de tres puntos.

3. Actualice el valor **actual** (no actualice el valor predeterminado) con la opción **nuevo valor** y proporcione el valor. El valor debe coincidir con el tipo de datos de la variable; por ejemplo, un tipo de datos sí/no aceptará ningún valor sí o no.

:::image type="content" source="images/environment-variables-video.gif" alt-text="Actualizar variables de entorno":::

- Sincronización de referencia de venta conjunta bidireccional de un extremo a otro

Una vez que haya instalado, configurado y personalizado la solución Power Automate, puede probar la sincronización de referencias de venta conjunta entre Dynamics 365 y el centro de Partners.

### <a name="pre-requisites"></a>Requisitos previos

Para sincronizar las referencias entre el centro de Partners y Dynamics 365 CRM, la solución Power Automate marca claramente los campos de referencia específicos de Microsoft. Esta identificación proporciona a los equipos de vendedores la capacidad de decidir qué referencias desean compartir con Microsoft para la venta conjunta.

Se agregará un conjunto de campos y objetos personalizados como parte de la instalación de la solución. Un usuario administrador de CRM tendrá que crear una sección de CRM independiente con los campos personalizados de la **oportunidad** .

Los siguientes campos personalizados deben formar parte de la sección CRM:

- **Sincronizar con el centro de Partners**: si se va a sincronizar la oportunidad con el centro de Partners de Microsoft. De forma predeterminada, el valor de este campo es no y el vendedor debe establecerlo explícitamente en sí para compartir una oportunidad con Microsoft. Las nuevas referencias compartidas del centro de partners a CRM tendrán este valor de campo establecido en sí.

- **Identificador de referencia**: un campo de identificador de solo lectura para la referencia del centro de Partners de Microsoft

- **Vínculo de referencia**: un vínculo de solo lectura a la referencia en el centro de Partners de Microsoft
- **¿Cómo puede ayudarle Microsoft?**: ayuda de Microsoft para la referencia. Para crear una referencia de venta conjunta, seleccione la ayuda adecuada que necesita Microsoft. Un contacto de cliente debe estar asociado a la oportunidad de crear una referencia de venta conjunta. Para crear una referencia que no sea de venta conjunta, deje este campo anulado de selección. Una referencia que no sea de venta conjunta se puede convertir en una referencia de venta conjunta en cualquier momento seleccionando la opción de ayuda necesaria.

- **Visibilidad** de la referencia del centro de Partners de Microsoft: seleccione visibilidad para la referencia del centro de Partners de Microsoft. Al hacer que sea visible para los vendedores de Microsoft, una referencia que no sea de venta conjunta puede convertirse en una venta conjunta. Cuando se requiere ayuda de Microsoft, la referencia es visible para los vendedores de Microsoft de forma predeterminada. Una vez marcado como visible, este campo no se puede revertir.

- **Identificador de Microsoft CRM**: cuando Microsoft crea y acepta una referencia de venta conjunta, este campo se rellenará con el identificador de CRM de Microsoft.

- **Productos: obsoleto** : no usar este campo o agregarlo a la sección CRM, solo está disponible para compatibilidad con versiones anteriores. En su lugar, use las soluciones del centro de Partners de Microsoft.

- **Audit**: una pista de auditoría de solo lectura para la sincronización con las referencias del centro de Partners

- **Soluciones** para el centro de Partners de Microsoft: un objeto personalizado para asociar soluciones listas para usar de colaboración o soluciones de Microsoft con la oportunidad. Se pueden agregar o quitar una o varias soluciones de la oportunidad. Es obligatorio agregar al menos una solución preparada para la venta conjunta o Microsoft a la oportunidad antes de compartirla con Microsoft. Para asociar este objeto a la oportunidad, actualice el formulario de la oportunidad en CRM:

  Seleccione la pestaña adecuada en formulario de la oportunidad y agregue una subcuadrícula como se muestra a continuación:

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Formulario de la oportunidad":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="{alt-text}":::



- Después de agregar las soluciones de Microsoft, puede rellenar previamente los detalles de la solución de venta conjunta lista para que los vendedores no tengan que agregarlas. Para agregar un nuevo detalle de la solución, vaya al objeto de detalles de la solución de Microsoft en CRM y haga clic en **Agregar registro** para agregar una entrada o usar la **carga de Excel** para agregar varias entradas.

:::image type="content" source="images/dynamic-1a.png" alt-text="Detalles de la solución":::

### <a name="scenarios"></a>SITUACIÓN

1. Sincronización de referencia cuando se crea o actualiza una referencia en CRM y se sincroniza en el centro de Partners:

   1. Inicie sesión en el entorno de CRM de Dynamics 365 con un usuario que tenga visibilidad en la sección de **oportunidades** de CRM.

   2. Asegúrese de que la sección centro de Partners de Microsoft esté presente cuando cree una "nueva oportunidad" en el entorno de Dynamics 365

   :::image type="content" source="images/dynamic-2a.png" alt-text="Nueva oportunidad"::: 

   3. Para sincronizar esta oportunidad con el centro de Partners, asegúrese de establecer los campos siguientes en la vista tarjeta:

      - **¿Cómo puede ayudarle Microsoft?**: para crear una referencia de venta conjunta, seleccione una opción de ayuda adecuada.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Cómo obtener los campos correspondientes en la vista de tarjeta":::

      - **Contacto del cliente**: para crear una referencia de venta conjunta, agregue un contacto de cliente a la oportunidad.
      - **Sincronizar con el centro de Partners**: sí

      - Soluciones de Microsoft: para compartir una referencia con Microsoft, agregue una solución válida de venta conjunta preparada o de Microsoft a la oportunidad.
       
      
      :::image type="content" source="images/dynamic-4a.png" alt-text="Id. de la solución":::

   4. Una vez creada la oportunidad en Dynamics 365 con la opción sincronizar con el centro de Partners establecida en sí, espere 10 minutos y, a continuación, inicie sesión en su cuenta del centro de Partners. Las referencias se sincronizarán con Dynamics 365 y el identificador de referencia. Se rellenará el vínculo de referencia. En caso de error, el campo de auditoría se rellenará con información de error.
     
    5. Del mismo modo, para una oportunidad que tuviera la opción "sincronizar con el centro de Partners" establecida en "sí", si actualizas la oportunidad en Dynamics 365 CRM, los cambios se sincronizarán en la cuenta del centro de Partners.

    6. Las oportunidades que se sincronizan correctamente con el centro de Partners se identificarán con ✔ icono en Dynamics 365.

2. Sincronización de referencia cuando se crea o actualiza una referencia en el centro de Partners de Microsoft y se sincroniza en el entorno de Dynamics 365:

   1. Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard/home)del centro de Partners.

   2. Seleccione **referencias** en el menú de la izquierda.

   3. Cree una nueva referencia de venta conjunta desde el centro de Partners seleccionando la opción  **nuevo contrato** .

   4. Inicie sesión en el entorno de CRM de Dynamics 365.

   5. Vaya a **abrir oportunidades**. La referencia creada en el centro de Partners de Microsoft ya está sincronizada en Dynamics 365 CRM.

   6. Al seleccionar una referencia sincronizada, se rellenan los detalles de la vista de tarjeta.

## <a name="next-steps"></a>Pasos siguientes

- [Administrar los clientes potenciales](manage-leads.md)

- [Administrar las oportunidades de venta conjunta](manage-co-sell-opportunities.md)

- [¿Más información sobre la plataforma Microsoft Power Automate?](/power-automate/)

- [Webhooks del Centro de partners](/partner-center/develop/partner-center-webhooks)
