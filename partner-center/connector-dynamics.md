---
title: El conector de venta conjunta para el centro de Partners de Dynamics 365 CRM
description: Sincronizar las referencias del centro de Partners con el conector de venta conjunta para Dynamics 365 CRM. Después, puede colaborar con Microsoft desde el sistema CRM.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 2082424f8203f0d9c50726e1e5ef7b3e3c39d6c2
ms.sourcegitcommit: 35fe0fdc41886f6f5af71ec74e4a4ebd245dfe1d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/22/2021
ms.locfileid: "104768778"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Introducción al conector de venta conjunta para Dynamics 365 CRM

### <a name="appropriate-roles"></a>Roles adecuados

- Administrador de referencias
- Administrador del sistema o Personalizador del sistema en CRM

Los conectores de la venta conjunta del centro de Partners permiten a los vendedores colaborar en la venta con Microsoft desde los sistemas CRM. No tendrán que estar capacitados para utilizar el centro de partners para administrar las ofertas de venta conjunta. Use los conectores de venta conjunta para crear una nueva referencia de venta conjunta para invitar a un vendedor de Microsoft, recibir referencias del vendedor de Microsoft, aceptar o rechazar referencias y modificar los datos del negocio, como el valor de trato y la fecha de cierre. También puede recibir cualquier actualización de los vendedores de Microsoft en estos acuerdos de venta conjunta. Puede administrar todas las referencias en el CRM de su elección, en lugar de hacerlo en el centro de Partners.

La solución se basa en la automatización y el uso de las API del centro de Partners.

## <a name="prerequisites"></a>Prerrequisitos

Antes de instalar la solución, asegúrese de cumplir los siguientes requisitos previos.

|**Temas**   |**Detalles**   |**Vínculos**   |
|--------------|--------------------|------|
|Identificador de Microsoft Partner Network (MPN) |Necesita un identificador de MPN válido.|[Unirse a la red de asociados](https://partner.microsoft.com/)|
|Listo para la venta conjunta|La solución de IP/servicios debe estar lista para su venta conjunta.|[Venda con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Cuenta de Centro de partners|El identificador de MPN asociado al inquilino del centro de Partners debe ser el mismo que el identificador de MPN asociado a la solución de venta conjunta. Compruebe que puede ver las referencias de venta conjunta en el portal del centro de Partners antes de implementar los conectores.|[Administración de la cuenta](create-user-accounts-and-set-permissions.md)|
|Roles de usuario del Centro de partners|El empleado que va a instalar y usar los conectores debe ser un administrador de referencias.|[Asignar roles y permisos de usuarios](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|El rol de usuario CRM es administrador del sistema o Personalizador del sistema.|[Asignación de roles en Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Cuenta de flujo de automatización de energía|Cree un nuevo entorno de producción con una base de datos para pruebas, ensayo y producción. Si tiene un entorno de producción existente con una base de datos, se puede volver a usar. El usuario que vaya a instalar la solución de conector debe tener una licencia de Power Automatic y acceso a este entorno. Puede supervisar el progreso y obtener más información en [Power Automate](https://flow.microsoft.com/) si se produce un error en la instalación. Seleccione **ver el historial** en **soluciones**.|[Crear o administrar un entorno](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Instalación de la sincronización de referencias del centro de partners para Dynamics 365 (solución de automatización de energía)

1. Vaya a [Power Automatic](https://flow.microsoft.com)y seleccione **entornos** en la esquina superior derecha. Este paso le mostrará las instancias de CRM disponibles.

1. Seleccione la instancia de CRM correspondiente en la lista desplegable de la esquina superior derecha.

1. Seleccione **soluciones** a la izquierda.

1. Seleccione el vínculo **abrir AppSource** en el menú superior.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Captura de pantalla que muestra Open AppSource.":::

1. Busque **conectores de referencias del centro de partners para Dynamics 365** en la pantalla emergente.  

1. Seleccione el botón **obtener ahora** y, después, seleccione **continuar**.

1. Aparece una página donde puede seleccionar el entorno de CRM (Dynamics 365) para instalar la aplicación. Acepte los términos y condiciones.

1. Puede supervisar el progreso y, si se produce un error en la instalación, puede obtener más detalles en Power Automate seleccionando **ver el historial** en **soluciones**.

1. Una vez completada la instalación, vuelva a [Power Automatic](https://flow.microsoft.com) y seleccione **soluciones** a la izquierda. La **sincronización de las referencias del centro de partners para Dynamics 365** ahora está disponible en la lista de **soluciones** .

1. Seleccione la **sincronización de referencias del centro de partners para Dynamics 365**. Están disponibles los siguientes flujos y entidades de automatización.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Captura de pantalla que muestra los CRMs disponibles.":::

## <a name="test-before-you-go-live"></a>Prueba antes de la marcha

Antes de instalar, configurar y personalizar la solución Power Automate en el entorno de producción, asegúrese de probar la solución en una instancia de CRM provisional. Necesitará:

- Instale la solución Power Automate en una instancia de CRM de entorno de ensayo.
- Configurar y personalizar la solución Power Automate en un entorno de ensayo.
- Pruebe la solución en una instancia de CRM de ensayo.
- Después de una prueba correcta, importe como una solución administrada a la instancia de producción.

## <a name="configure-the-solution"></a>Configuración de la solución

1. Después de instalar la solución en la instancia de CRM, vuelva a [Power Automatic](https://flow.microsoft.com/).

1. En la lista desplegable **entornos** en la esquina superior derecha, seleccione la instancia de CRM en la que instaló la solución Power Automate.

1. Deberá crear conexiones que asocien las tres cuentas de usuario:

   - Usuario del centro de Partners con credenciales de administrador de referencias
   - Eventos del Centro de partners
   - Administrador de CRM con la potencia que automatiza los flujos en la solución

   1. Seleccione **conexiones** a la izquierda y, en la lista, seleccione la solución **referencias del centro de Partners** .

   1. Cree una conexión seleccionando **crear una conexión**.

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Captura de pantalla que muestra cómo crear una conexión.":::

   1. Busque **referencias del centro de Partners (versión preliminar)** en la barra de búsqueda de la esquina superior derecha.

   1. Cree una conexión para el usuario del centro de Partners con el rol de credenciales de administrador de referencias.

   1. A continuación, cree una conexión de eventos del centro de partners para el usuario del centro de Partners con las credenciales de administrador de referencias.

   1. Cree una conexión para Common Data Service (entorno actual) para el usuario administrador de CRM.
     
   1. Después de agregar todas las conexiones, debería ver las siguientes conexiones en su entorno.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Captura de pantalla que muestra las conexiones.":::

## <a name="edit-the-connections"></a>Editar las conexiones

1. Vuelva a la página **soluciones** y seleccione **solución predeterminada**. Seleccione **referencia de conexión (vista previa)** seleccionando **todo**.

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Captura de pantalla que muestra la edición de las conexiones.":::

1. Edite cada una de las conexiones de una en una; para ello, seleccione el icono de puntos suspensivos. Agregue las conexiones correspondientes.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Captura de pantalla que muestra las conexiones enumeradas.":::

1.  Vuelva a la página **soluciones** , seleccione la **sincronización de referencias del centro de partners para Dynamics 365** y active el flujo seleccionando el icono de puntos suspensivos junto a cada flujo en la siguiente secuencia. Si encuentra algún problema mientras activa el flujo, consulte [pasos de personalización](connector-dynamics.md#customize-synchronization-steps) y [pasos para la solución de problemas](connectors-troubleshoot.md).

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

Puede usar las API del webhook del centro de partners para registrarse para los eventos de cambio de recursos. Estos eventos de cambio se envían a la dirección URL como publicaciones HTTP.

1. Seleccione **centro de partners para Dynamics 365 (versión preliminar de Insider)**.

1. Seleccione el icono de **edición** y seleccione **cuando se reciba una solicitud HTTP**.

1. Seleccione el icono de **copiar** para copiar la dirección URL http post proporcionada.

   :::image type="content" source="images/webhook-video.gif" alt-text="Captura de pantalla que muestra el uso de webhooks para registrar cambios de recursos.":::

1. Seleccione el flujo de **registro del webhook del centro de Partners (versión preliminar de Insider)** y, a continuación, seleccione **Ejecutar**.

1. Asegúrese de que la ventana **Ejecutar flujo** se abre en el panel derecho y seleccione **continuar**.

1. Escriba la siguiente información:

   - **Punto de conexión de desencadenador http**: esta dirección URL se copió de un paso anterior.
   - **Eventos que se van a registrar**: seleccione todos los eventos disponibles (**referencia-creado**, referencia **-actualizado**, **relacionado-referencia-creado** y **relacionado-referencia-actualizado**).
   - **¿Sobrescribir los puntos de conexión del desencadenador existente si están presentes?**: sí. Solo se puede registrar una dirección URL para un evento de webhook determinado.

1. Seleccione **Ejecutar flujo** y, a continuación, haga clic en **listo.**

El webhook ahora puede escuchar, crear y actualizar eventos.

## <a name="customize-synchronization-steps"></a>Personalizar pasos de sincronización

Los sistemas CRM son muy personalizados y puede personalizar la solución Power Automatic en función de la configuración de CRM. Cuando se sincronizan las referencias de venta conjunta entre el centro de Partners y el sistema CRM, los campos que se sincronizan en el equipo del centro de Partners se enumeran en la [Guía de asignación de campos personalizados](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Siga la guía de asignación de campos y, si es necesario, realice los cambios adecuados en **[personalizar] crear u obtener detalles de las variables de entorno o de flujo de Dynamics 365** . No actualice ningún otro flujo de la solución Power Automate porque puede afectar a las actualizaciones de soluciones futuras.

Están disponibles las siguientes personalizaciones:

- **Mostrar la marca de verificación en el nombre de la oportunidad**: de forma predeterminada, se mostrará una marca de verificación junto al nombre de la oportunidad para indicar que la sincronización entre el centro de Partners y Dynamics 365 CRM se está produciendo correctamente. Del mismo modo, se mostrará una marca cruzada si se produce un error de sincronización. Para evitar agregar una marca de verificación o una marca cruzada en el nombre de la oportunidad, establezca el valor actual de la **marca de verificación de presentación en la variable de entorno nombre de oportunidad** en no.
- **Valor de trato**: de forma predeterminada, el valor de trato del centro de Partners se sincronizará con **estimatedvalue** en CRM. Si tiene un campo diferente en el CRM para el valor del trato que se va a sincronizar desde:

  - Actualice el nombre del campo **Deal Value** de la variable de entorno Dynamics 365 con el nombre de campo de CRM. Asegúrese de que proporciona el nombre del campo, no su nombre para mostrar.
  - Editar **[personalizar] cree u obtenga detalles del flujo de Dynamics 365** y vaya a **crear o actualizar oportunidad** en CRM y actualizar **crear una nueva oportunidad** y actualizar las acciones de la **oportunidad existentes** para asignar el valor de **DealValue** al campo correcto en el CRM. Además, quite la asignación **DealValue** del campo **ingresos estimados** .

- **Código de país** de la cuenta de cliente: es obligatorio proporcionar un código de país de dos letras (ISO 3166) cuando se crea una nueva referencia. De forma predeterminada, el código de país se sincronizará con y desde el campo de **address1_country** de la cuenta en CRM. Si tiene un campo diferente en el CRM para el código de país desde el que se va a realizar la sincronización:

   - Para un campo de código de país que no es de búsqueda en la cuenta que contiene un código de dos letras:
     - Actualice el nombre del campo de código de país de la **cuenta de cliente** en la variable de entorno Dynamics 365 con el nombre de campo de CRM. Asegúrese de que proporciona el nombre del campo, no su nombre para mostrar.
     - Editar **[personalizar] cree u obtenga detalles del flujo de Dynamics 365** y vaya a **crear o a obtener cuenta de cliente** en la acción de CRM para asignar un valor de **país** al campo correcto en CRM. Además, quite la asignación de valores de **país** del campo **Dirección 1: país o región** .

   - Para un campo de código de país basado en búsquedas en la cuenta:
     - Agregue un nuevo campo personalizado en la cuenta y rellénelo automáticamente con un código de país de dos letras (ISO 3166) en función del valor seleccionado en el campo basado en búsquedas y viceversa.
     - Siga los pasos anteriores para el campo de código de país no lookup para sincronizar un nuevo campo personalizado desde el CRM hacia y desde el centro de Partners.

- **Campos de oportunidad**: si hay campos obligatorios en la **oportunidad** que deben rellenarse, edite **[Customize] cree u obtenga detalles del flujo de Dynamics 365** y vaya a **crear o actualizar oportunidad** en CRM y actualice **crear una nueva acción de oportunidad** para asignar valores a los campos obligatorios en función de los requisitos de su empresa.
- **Campos de clientes potenciales**: si hay campos obligatorios en el **cliente potencial** que deben rellenarse, edite **[Customize] cree u obtenga detalles del flujo de Dynamics 365** y vaya a **Create or Update Lead** en CRM y actualice **cree una nueva acción de cliente potencial** para asignar valores a los campos obligatorios en función de los requisitos de su empresa.
- **Cuenta de cliente**: cuando se sincroniza una nueva referencia del centro de Partners con el CRM, la solución Power Automate intenta buscar una cuenta existente en CRM mediante el nombre de la empresa del cliente y el código postal. Si no encuentra ninguna, se creará una nueva cuenta de cliente en CRM. Para actualizar los criterios de búsqueda y los detalles de creación de la cuenta nueva, edite **[Customize] create or get details from Dynamics 365 Flow** y vaya a **Create or get Account Customer** en la acción CRM y **Create Customer Account**.

## <a name="update-environment-variable"></a>Actualizar variable de entorno

Para actualizar un valor de variable de entorno:

1. Vaya a la página **soluciones** y seleccione **solución predeterminada**. Seleccione la **variable de entorno** seleccionando **todo**.

1. Seleccione la variable de entorno para el valor que debe actualizarse y seleccione **Editar** con el icono de puntos suspensivos.

1. Actualice el **valor actual** (no actualice el **valor predeterminado**) mediante la opción **nuevo valor** y proporcione el valor. El valor debe coincidir con el tipo de datos de la variable. Por ejemplo, el tipo de datos sí o no aceptará el valor sí o no.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Captura de pantalla que muestra las variables de entorno de actualización.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Sincronización de referencia de distribución bidireccional de un extremo a otro

Después de instalar, configurar y personalizar la solución Power Automate, puede probar la sincronización de referencias de venta conjunta entre Dynamics 365 y el centro de Partners.

### <a name="prerequisites"></a>Prerrequisitos

Para sincronizar las referencias entre el centro de Partners y Dynamics 365 CRM, la solución Power Automate marca claramente los campos de referencia específicos de Microsoft. Esta identificación proporciona a los equipos de vendedores la capacidad de decidir qué referencias desean compartir con Microsoft para la venta conjunta.

Se agregará un conjunto de campos y objetos personalizados como parte de la instalación de la solución. Un usuario administrador de CRM tendrá que crear una sección de CRM independiente con los campos personalizados de la **oportunidad** .

Los siguientes campos personalizados deben formar parte de la sección CRM:

- **Sincronizar con el centro de Partners**: si se va a sincronizar la oportunidad con el centro de Partners. De forma predeterminada, el valor de este campo es no y el vendedor debe establecerlo explícitamente en sí para compartir una oportunidad con Microsoft. Las nuevas referencias compartidas del centro de partners a CRM tendrán este valor de campo establecido en sí.
- **Identificador de referencia**: un campo de identificador de solo lectura para la referencia del centro de Partners.
- **Vínculo de referencia**: un vínculo de solo lectura a la referencia en el centro de Partners.
- **¿Cómo puede ayudarle Microsoft?**: ayuda de Microsoft para la referencia. Para crear una referencia de venta conjunta, seleccione la ayuda adecuada que necesita Microsoft. Un contacto de cliente debe estar asociado a la oportunidad de crear una referencia de venta conjunta. Para crear una referencia que no sea de venta conjunta, no seleccione este campo. Una referencia que no es de venta conjunta se puede convertir en una referencia de venta conjunta en cualquier momento seleccionando la opción necesaria para la ayuda.
- **Visibilidad** de la referencia del centro de Partners de Microsoft: seleccione visibilidad para la referencia del centro de Partners. Al hacer que sea visible para los vendedores de Microsoft, una referencia que no sea de venta conjunta podría convertirse en una venta conjunta. Cuando se requiere ayuda de Microsoft, la referencia es visible para los vendedores de Microsoft de forma predeterminada. Una vez que este campo está marcado como visible, no se puede revertir.
- **Identificador de Microsoft CRM**: cuando Microsoft crea y acepta una referencia de venta conjunta, este campo se rellenará con el identificador de CRM de Microsoft.
- **Productos: obsoleto**: no use este campo o agréguelo a la sección CRM. Solo está disponible para la compatibilidad con versiones anteriores. En su lugar, use soluciones del centro de Partners.
- **Audit**: una pista de auditoría de solo lectura para la sincronización con las referencias del centro de Partners.
- **Soluciones** para el centro de Partners de Microsoft: un objeto personalizado para asociar soluciones listas para usar de colaboración o soluciones de Microsoft con la oportunidad. Se pueden agregar o quitar una o varias soluciones de la oportunidad. Es obligatorio agregar al menos una solución lista para participar o de Microsoft a la oportunidad antes de compartirla con Microsoft. Para asociar este objeto a la oportunidad, actualice el formulario de la **oportunidad** en CRM.

  Seleccione la pestaña correspondiente en el formulario de la **oportunidad** y agregue una subcuadrícula como se muestra aquí.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Captura de pantalla que muestra el formulario de la oportunidad.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Captura de pantalla que muestra soluciones de Microsoft.":::

- Después de agregar las soluciones de Microsoft, puede rellenar previamente los detalles de la solución de venta conjunta lista para que los vendedores no tengan que agregarlas. Para agregar un nuevo detalle de la solución, vaya al objeto de detalles de la solución de Microsoft en CRM y seleccione **Agregar registro** para agregar una entrada o usar la **carga de Excel** para agregar varias entradas.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Captura de pantalla que muestra los detalles de la nueva solución de Microsoft.":::

### <a name="scenarios"></a>Escenarios

1. Sincronización de referencia cuando se crea o actualiza una referencia en CRM y se sincroniza en el centro de Partners:

   1. Inicie sesión en el entorno de CRM de Dynamics 365 con el usuario que tiene visibilidad en la sección de la **oportunidad** de CRM.

   1. Asegúrese de que la sección **centro de Partners de Microsoft** está presente al crear una nueva oportunidad en el entorno de Dynamics 365.

      :::image type="content" source="images/dynamic-2a.png" alt-text="Captura de pantalla que muestra la nueva oportunidad.":::

   1. Para sincronizar esta oportunidad con el centro de Partners, asegúrese de establecer los campos siguientes en la vista tarjeta:

      - **¿Cómo puede ayudarle Microsoft?**: para crear una referencia de venta conjunta, seleccione una opción de ayuda adecuada.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Captura de pantalla que muestra cómo obtener los campos correspondientes en la vista de tarjeta.":::

      - **Contacto del cliente**: para crear una referencia de venta conjunta, agregue un contacto de cliente a la oportunidad.
      - **Sincronizar con el centro de Partners**: sí.
      - **Soluciones de Microsoft**: para compartir una referencia con Microsoft, agregue una solución válida de venta conjunta preparada o de Microsoft a la oportunidad.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="Captura de pantalla que muestra el identificador de la solución.":::

   1. Una vez creada la oportunidad en Dynamics 365 con la opción **sincronizar con el centro de Partners** establecida en sí, espere 10 minutos. A continuación, inicie sesión en su cuenta del centro de Partners. Las referencias se sincronizarán con Dynamics 365 y el identificador de **referencia**. Se rellenará el **vínculo de referencia** . Si se produce un error, el campo de **Auditoría** se rellenará con la información del error.
     
    1. Del mismo modo, para una oportunidad que tenga la opción **sincronizar con el centro de Partners** establecida en sí, si actualiza la oportunidad en Dynamics 365 CRM, los cambios se sincronizarán en la cuenta del centro de Partners.

    1. Las oportunidades que se sincronizan correctamente con el centro de Partners se identificarán con ✔ icono en Dynamics 365.

1. Sincronización de referencia cuando se crea o actualiza la referencia en el centro de Partners y se sincroniza en el entorno de Dynamics 365:

   1. Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard/home)del centro de Partners.

   1. Seleccione **referencias** en el menú de la izquierda.

   1. Cree una nueva referencia de venta conjunta desde el centro de Partners seleccionando la opción **nuevo contrato** .

   1. Inicie sesión en el entorno de CRM de Dynamics 365.

   1. Vaya a **oportunidades abiertas**. La referencia creada en el centro de Partners ahora está sincronizada en Dynamics 365 CRM.

   1. Al seleccionar una referencia sincronizada, se rellenan los detalles de la vista de tarjeta.

## <a name="next-steps"></a>Pasos siguientes

- [Administrar los clientes potenciales](manage-leads.md)
- [Administrar las oportunidades de venta conjunta](manage-co-sell-opportunities.md)
- [Más información sobre la plataforma Microsoft Power Automate](/power-automate/)
- [Webhooks del Centro de partners](/partner-center/develop/partner-center-webhooks)
