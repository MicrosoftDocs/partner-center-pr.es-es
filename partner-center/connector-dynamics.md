---
title: El conector de venta co-sell para Dynamics 365 CRM Centro de partners
description: Sincronice las referencias Centro de partners con el conector de venta co-sell para Dynamics 365 CRM. A continuación, puede realizar la venta en colaboración con Microsoft desde el sistema CRM.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 03/01/2021
ms.openlocfilehash: 035a819020097ddee2230b5541e1b477d4b34c14
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148472"
---
# <a name="co-sell-connector-for-dynamics-365-crm-overview"></a>Introducción al conector de venta co-venta para Dynamics 365 CRM

**Roles adecuados:** administrador de referencias | Administrador del sistema o personalizador del sistema en CRM

Centro de partners conectores de venta en colaboración permiten a los vendedores vender con Microsoft desde dentro de los sistemas CRM. No tendrán que entrenarse para usar Centro de partners administrar las ofertas de venta en colaboración. Use los conectores de venta co-sell para crear una nueva referencia de venta conjunto para interactuar con un vendedor de Microsoft, recibir referencias del vendedor de Microsoft, aceptar o rechazar referencias y modificar datos de la oferta, como el valor de la oferta y la fecha de cierre. También puede recibir cualquier actualización de los vendedores de Microsoft sobre estas ofertas de venta coventa. Puede administrar todas las referencias en el CRM que prefiera, en lugar de hacerlo Centro de partners.

La solución se basa en Power Automate y usa Centro de partners API.

## <a name="prerequisites"></a>Requisitos previos

Antes de instalar la solución, asegúrese de cumplir los siguientes requisitos previos.

|**Temas**   |**Detalles**   |**Vínculos**   |
|--------------|--------------------|------|
|Identificador de Microsoft Partner Network (MPN) |Necesita un identificador de MPN válido.|[Unirse a La red de asociados](https://partner.microsoft.com/)|
|Listo para la venta conjunta|La solución ip/services debe estar lista para la venta en colaboración.|[Vender con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Cuenta de Centro de partners|El identificador de MPN asociado al inquilino Centro de partners debe ser el mismo que el identificador de MPN asociado a la solución de venta simultánea. Compruebe que puede ver las referencias de venta Centro de partners portal antes de implementar los conectores.|[Administración de la cuenta](create-user-accounts-and-set-permissions.md)|
|Roles de usuario del Centro de partners|El empleado que instalará y usará los conectores debe ser un administrador de referencias.|[Asignar roles y permisos de usuarios](create-user-accounts-and-set-permissions.md)|
|Dynamics 365 CRM|El rol de usuario de CRM es Administrador del sistema o Personalizador del sistema.|[Asignación de roles en Dynamics 365](/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Power Automate de flujo|Cree un nuevo entorno de producción con una base de datos para pruebas, ensayo y producción. Si tiene un entorno de producción existente con una base de datos, se puede reutilizar. El usuario que va a instalar la solución del conector debe tener una Power Automate licencia y acceso a este entorno. Puede supervisar el progreso y obtener más información en [Power Automate](https://flow.microsoft.com/) si se produce un error en la instalación. Seleccione **Ver historial en** **Soluciones.**|[Creación o administración del entorno](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a>Instalar Centro de partners de referencias para Dynamics 365 (Power Automate solución)

1. Vaya a [Power Automate](https://flow.microsoft.com)y seleccione **Entornos** en la esquina superior derecha. Este paso le mostrará las instancias de CRM disponibles.

1. Seleccione la instancia de CRM adecuada en la lista desplegable de la esquina superior derecha.

1. Seleccione **Soluciones** a la izquierda.

1. Seleccione el **vínculo Abrir AppSource** en el menú superior.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Captura de pantalla que muestra Open AppSource.":::

1. Busque **conectores Centro de partners referencias para Dynamics 365** en la pantalla emergente.  

1. Seleccione el **botón Obtenerla ahora** y, a continuación, **seleccione Continuar.**

1. Aparece una página donde puede seleccionar el entorno crm (Dynamics 365) para instalar la aplicación. Acepte los términos y condiciones.

1. Puede supervisar el progreso y, si se produce un error en la instalación, puede obtener más detalles en Power Automate si selecciona **Ver** historial en **Soluciones**.

1. Una vez completada la instalación, vuelva a [Power Automate](https://flow.microsoft.com) seleccione **Soluciones a** la izquierda. **Centro de partners sincronización de referencias para Dynamics 365** ya está disponible en la **lista Soluciones.**

1. Seleccione **Centro de partners de referencias para Dynamics 365.** Las siguientes Power Automate y entidades están disponibles.

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="Captura de pantalla que muestra las CRM disponibles.":::

## <a name="test-before-you-go-live"></a>Prueba antes de empezar a realizar la ejecución

Antes de instalar, configurar y personalizar la solución Power Automate en el entorno de producción, asegúrese de probar la solución en una instancia de CRM de almacenamiento provisional. Necesitará:

- Instale la solución Power Automate en una instancia de CRM del entorno de ensayo.
- Configure y personalice la solución Power Automate en un entorno de ensayo.
- Pruebe la solución en una instancia de CRM de almacenamiento provisional.
- Después de una prueba correcta, importe como una solución administrada a la instancia de producción.

## <a name="configure-the-solution"></a>Configuración de la solución

1. Después de instalar la solución en la instancia de CRM, vuelva a [Power Automate](https://flow.microsoft.com/).

1. En la **lista desplegable Entornos** de la esquina superior derecha, seleccione la instancia de CRM donde instaló la Power Automate solución.

1. Deberá crear conexiones que asocie las tres cuentas de usuario:

   - Centro de partners usuario con credenciales de administrador de referencias
   - Eventos del Centro de partners
   - Administrador de CRM con los flujos Power Automate en la solución

   1. Seleccione **Conexiones** a la izquierda y seleccione la **solución Centro de partners referencias** de la lista.

   1. Para crear una conexión, seleccione **Crear una conexión.**

         :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Captura de pantalla que muestra Creación de una conexión.":::

   1. Busque Centro de partners **referencias (versión preliminar)** en la barra de búsqueda de la esquina superior derecha.

   1. Cree una conexión para el usuario Centro de partners usuario con el rol de credenciales del administrador de referencias.

   1. A continuación, cree una conexión Centro de partners Events para el Centro de partners usuario con las credenciales de administrador de referencias.

   1. Cree una conexión para Common Data Service (entorno actual) para el usuario administrador de CRM.
     
   1. Después de agregar todas las conexiones, debería ver las siguientes conexiones en su entorno.

      :::image type="content" source="images/cosellconnectors/dynamics-2.png" alt-text="Captura de pantalla que muestra las conexiones.":::

## <a name="edit-the-connections"></a>Edición de las conexiones

1. Vuelva a la **página Soluciones** y seleccione **Solución predeterminada.** Seleccione **Connection Reference (preview) (Referencia** de conexión [versión preliminar]) **seleccionando All (Todo).**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Captura de pantalla que muestra Edición de las conexiones.":::

1. Edite cada una de las conexiones individualmente seleccionando el icono de puntos suspensivos. Agregue las conexiones pertinentes.

   :::image type="content" source="images/cosellconnectors/dynamics-4.png" alt-text="Captura de pantalla que muestra las conexiones enumeradas.":::

1.  Vuelva a  la página Soluciones, seleccione sincronización de referencias de Centro de partners para **Dynamics 365** y active el flujo seleccionando el icono de puntos suspensivos junto a cada flujo de la secuencia siguiente. Si encuentra algún problema al activar el flujo, consulte Pasos [de personalización](connector-dynamics.md#customize-synchronization-steps) y [Pasos de solución de problemas.](connectors-troubleshoot.md)

Active los flujos en la secuencia siguiente:

- Centro de partners webhook Registration (Insider Preview)
- Creación de una referencia de venta co-venta: Dynamics 365 Centro de partners (versión preliminar de Insider)
- [Personalizar] Crear u obtener detalles del flujo de Dynamics 365
- Centro de partners a Dynamics 365 - Helper (Insider Preview)
- Centro de partners de referencias de venta co-venta de Microsoft a Dynamics 365 (versión preliminar de Insider)
- Centro de partners a Dynamics 365 (insider preview)
- Dynamics 365 to Centro de partners (Insider Preview)
- Oportunidad de dynamics 365 Centro de partners (versión preliminar de Insider)
- Dynamics 365 Microsoft Solutions to Centro de partners (Insider Preview)
 
## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Uso de api de webhook para registrarse para eventos de cambio de recursos

Puede usar las API Centro de partners webhook para registrarse en eventos de cambio de recursos. Estos eventos de cambio se envían a la dirección URL como publicaciones HTTP.

1. Seleccione **Centro de partners a Dynamics 365 (Insider Preview).**

1. Seleccione el **icono Editar** y seleccione Cuando se recibe una **solicitud HTTP.**

1. Seleccione el **icono Copiar** para copiar la dirección URL de HTTP POST proporcionada.

   :::image type="content" source="images/webhook-video.gif" alt-text="Captura de pantalla que muestra el uso de webhooks para registrar cambios en los recursos.":::

1. Seleccione el **flujo Centro de partners registro de webhook (insider preview Power Automate)** y, a continuación, seleccione **Ejecutar**.

1. Asegúrese de que **se abre la** ventana Ejecutar flujo en el panel derecho y seleccione **Continuar.**

1. Escriba la siguiente información:

   - **Punto de conexión de desencadenador** http: esta dirección URL se copió de un paso anterior.
   - **Eventos que se registrarán:** seleccione todos los eventos disponibles **(creados** por **referencias,** actualizados por referencia, creados **por referencias** relacionadas y **actualizados por referencias relacionadas).**
   - **¿Sobrescribir los puntos de conexión de desencadenador existentes si están presentes?**: Sí. Solo se puede registrar una dirección URL para un evento de webhook determinado.

1. Seleccione **Run flow (Ejecutar** flujo) y, a continuación, **seleccione Done (Listo).**

El webhook ahora puede escuchar, crear y actualizar eventos.

## <a name="customize-synchronization-steps"></a>Personalización de los pasos de sincronización

Los sistemas CRM están muy personalizados y puede personalizar la solución Power Automate en función de la configuración de CRM. Cuando las referencias de venta co-sell se sincronizan entre Centro de partners y el sistema CRM, los campos que se sincronizan en el equipo Centro de partners se muestran en la Guía de asignación de campos [personalizados](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Siga la guía de asignación de campos y, si es necesario, realice los cambios adecuados en [Personalizar] Crear u obtener detalles a partir de variables de entorno o flujo de **Dynamics 365.** No actualice ningún otro flujo de la solución Power Automate porque puede afectar a futuras actualizaciones de la solución.

Están disponibles las siguientes personalizaciones:

- **Mostrar marca** de verificación en el nombre de la oportunidad: de forma predeterminada, se mostrará una marca de verificación junto al nombre de la oportunidad para indicar que la sincronización entre Centro de partners y Dynamics 365 CRM se está produciendo correctamente. De forma similar, se mostrará una marca cruzada si se produce un error en la sincronización. Para evitar agregar una marca de verificación o una marca  cruzada en el nombre de la oportunidad, establezca el valor actual de la marca de verificación Mostrar de la variable de entorno de nombre de oportunidad en No.
- **Valor de** la oferta: de forma predeterminada, el valor de la oferta Centro de partners se sincronizará con y desde **estimatedvalue** en CRM. Si tiene un campo diferente en CRM para el valor de la oferta desde el que se va a sincronizar:

  - Actualice el **nombre del campo Valor** de la oferta en la variable de entorno de Dynamics 365 con el nombre del campo de CRM. Asegúrese de proporcionar el nombre del campo, no su nombre para mostrar.
  - Edite [Personalizar] Cree u obtenga detalles del flujo  de **Dynamics 365** y vaya  **a** Crear o actualizar una oportunidad en CRM y actualice Crear una nueva oportunidad y Actualizar las acciones de oportunidad existentes para asignar el valor **DealValue** al campo correcto en CRM. Además, quite la **asignación DealValue** del **campo Ingresos estimados.**

- **Código de país de la** cuenta de cliente: es obligatorio proporcionar un código de país de dos letras (ISO 3166) al crear una nueva referencia. De forma predeterminada, el código de país se sincronizará con y desde el campo de address1_country **de** la cuenta en CRM. Si tiene un campo diferente en crm para el código de país desde el que se va a sincronizar:

   - Para un campo de código de país que no sealookup de la cuenta que contiene un código de dos letras:
     - Actualice el **nombre del campo Código de** país de la cuenta de cliente en la variable de entorno de Dynamics 365 con el nombre del campo de CRM. Asegúrese de proporcionar el nombre del campo, no su nombre para mostrar.
     - Editar [Personalizar] Cree u obtenga detalles del flujo de  **Dynamics 365** y vaya **a** Crear u obtener cuenta de cliente en la acción CRM para asignar un valor de País al campo correcto en CRM. Además, quite la **asignación de** valor Country del **campo Address 1: Country/Region (Dirección 1: país o** región).

   - Para un campo de código de país basado en búsqueda en la cuenta:
     - Agregue un nuevo campo personalizado en la cuenta y rellene automáticamente con un código de país de dos letras (ISO 3166) basado en el valor seleccionado en el campo basado en búsqueda y viceversa.
     - Siga los pasos anteriores para que el campo de código de país que no eslookup sincronice un nuevo campo personalizado desde CRM hacia y desde Centro de partners.

- **Campos de** oportunidad: si hay  campos obligatorios en Oportunidad que deben rellenarse, edite [Personalizar] Crear  u obtener detalles del flujo de **Dynamics 365** y vaya a Crear o actualizar oportunidad en CRM y actualice La acción Crear una nueva oportunidad para asignar valores **a** los campos obligatorios en función de sus requisitos empresariales.
- Campos **de** clientes potenciales:  si hay campos obligatorios en Clientes potenciales que deben rellenarse, edite  [Personalizar] Crear u obtener detalles del flujo de **Dynamics 365** y vaya a Crear o actualizar cliente potencial en CRM y actualice Crear una nueva acción de cliente potencial para asignar valores **a** los campos obligatorios en función de sus requisitos empresariales.
- **Cuenta de** cliente: cuando se sincroniza una nueva referencia de Centro de partners a CRM, la solución Power Automate intenta buscar una cuenta existente en CRM mediante el nombre de la empresa del cliente y el código postal. Si no encuentra una, se creará una nueva cuenta de cliente en CRM. Para actualizar los criterios de búsqueda y los detalles de creación de nuevas cuentas,  edite [Personalizar] Crear u obtener detalles del flujo de **Dynamics 365** y vaya a Crear u obtener cuenta de cliente en la acción CRM y Crear cuenta de **cliente**.

## <a name="update-environment-variable"></a>Actualización de la variable de entorno

Para actualizar un valor de variable de entorno:

1. Vaya a la **página Soluciones** y seleccione **Solución predeterminada.** Seleccione **Variable de** entorno seleccionando **Todos.**

1. Seleccione la variable de entorno para el valor que debe actualizarse y **seleccione Editar** con el icono de puntos suspensivos.

1. Actualice **el valor actual** (no actualice el valor **predeterminado)** mediante la **opción Nuevo** valor y proporcionando el valor. El valor debe coincidir con el tipo de datos de la variable. Por ejemplo, el tipo de datos Sí o No aceptará el valor Sí o No.

   :::image type="content" source="images/environment-variables-video.gif" alt-text="Captura de pantalla que muestra Actualizar variables de entorno.":::

## <a name="end-to-end-bidirectional-co-sell-referral-synchronization"></a>Sincronización de referencias de venta bidireccional de un extremo a otro

Después de instalar, configurar y personalizar la solución Power Automate, puede probar la sincronización de referencias de venta coexistida entre Dynamics 365 y Centro de partners.

### <a name="prerequisites"></a>Requisitos previos

Para sincronizar las referencias entre Centro de partners y Dynamics 365 CRM, la solución Power Automate delimita claramente los campos de referencia específicos de Microsoft. Esta identificación ofrece a los equipos vendedores la capacidad de decidir qué referencias quieren compartir con Microsoft para la venta en colaboración.

Se agregará un conjunto de campos y objetos personalizados como parte de la instalación de la solución. Un usuario administrador de CRM deberá crear una sección de CRM independiente con los **campos personalizados Oportunidad.**

Los siguientes campos personalizados deben formar parte de la sección CRM:

- **Sincronizar con Centro de partners:** si se debe sincronizar la oportunidad con Centro de partners. De forma predeterminada, el valor de este campo es No y el vendedor debe establecer explícitamente en Sí para compartir una oportunidad con Microsoft. Las nuevas referencias compartidas Centro de partners a CRM tendrán este valor de campo establecido en Sí.
- **Identificador de referencia:** campo de identificador de solo lectura para la Centro de partners referencia.
- **Vínculo de referencia:** vínculo de solo lectura a la referencia en Centro de partners.
- **¿Cómo puede ayudar Microsoft?**: Ayuda necesaria de Microsoft para la referencia. Para crear una referencia de venta en colaboración, seleccione la ayuda adecuada que necesita Microsoft. Un contacto con el cliente debe estar asociado a la oportunidad de crear una referencia de venta co-sell. Para crear una referencia que no sea de venta en colaboración, no seleccione este campo. Una referencia de venta no co-sell se puede convertir en una referencia de venta co-sell en cualquier momento seleccionando la opción adecuada de ayuda necesaria.
- **Visibilidad Centro de partners referencias de Microsoft:** seleccione visibilidad para la Centro de partners referencia. Al hacer que sea visible para los vendedores de Microsoft, una referencia de venta no coventa podría convertirse en venta en colaboración. Cuando se requiere ayuda de Microsoft, la referencia es visible para los vendedores de Microsoft de forma predeterminada. Una vez que este campo está marcado como visible, no se puede revertir.
- **Identificador de Microsoft CRM:** cuando Microsoft crea y acepta una referencia de venta en colaboración, este campo se rellena con el identificador de CRM de Microsoft.
- **Productos: obsoletos:** no use este campo ni agrégrelo a la sección CRM. Solo está disponible por compatibilidad con versiones anteriores. Use Centro de partners soluciones en su lugar.
- **Auditoría:** un registro de auditoría de solo lectura para sincronizar con Centro de partners referencias.
- **Microsoft Centro de partners Solutions:** un objeto personalizado para asociar soluciones listas para la venta en colaboración o soluciones de Microsoft con la oportunidad. Se pueden agregar o quitar una o varias soluciones de la oportunidad. Es obligatorio agregar al menos una solución de Microsoft o lista para la venta compartida a la oportunidad antes de compartirla con Microsoft. Para asociar este objeto a la oportunidad, actualice el **formulario Oportunidad** en CRM.

  Seleccione la pestaña adecuada en el **formulario Oportunidad** y agregue una subcuadrícula como se muestra aquí.

  :::image type="content" source="images/cosellconnectors/dynamics-6.png" alt-text="Captura de pantalla que muestra el formulario Oportunidad.":::

  :::image type="content" source="images/cosellconnectors/dynamics-7.png" alt-text="Captura de pantalla que muestra Soluciones de Microsoft.":::

- Después de agregar soluciones de Microsoft, puede rellenar previamente los detalles de la solución lista para la venta en colaboración para que los vendedores no tengan que agregarlos. Para agregar un nuevo detalle de la solución, vaya  al objeto Detalles de la solución de Microsoft en CRM y seleccione Agregar registro para agregar una entrada o usar la carga de **Excel** para agregar varias entradas.

  :::image type="content" source="images/dynamic-1a.png" alt-text="Captura de pantalla que muestra Los detalles de la nueva solución de Microsoft.":::

### <a name="scenarios"></a>Escenarios

1. Sincronización de referencias cuando se crea o actualiza la referencia en CRM y se sincroniza en Centro de partners:

   1. Inicie sesión en el entorno de Dynamics 365 CRM con el usuario que tenga visibilidad en la **sección Oportunidad** de CRM.

   1. Asegúrese de que **la Centro de partners** microsoft está presente al crear una nueva oportunidad en el entorno de Dynamics 365.

      :::image type="content" source="images/dynamic-2a.png" alt-text="Captura de pantalla que muestra Nueva oportunidad.":::

   1. Para sincronizar esta oportunidad con Centro de partners, asegúrese de establecer los siguientes campos en la vista de tarjeta:

      - **¿Cómo puede ayudar Microsoft?**: para crear una referencia de venta en colaboración, seleccione una opción de ayuda adecuada.

         :::image type="content" source="images/dynamic-3a.png" alt-text="Captura de pantalla que muestra cómo obtener los campos adecuados en la vista de tarjeta.":::

      - **Contacto con el** cliente: para crear una referencia de venta en colaboración, agregue un contacto de cliente a la oportunidad.
      - **Sincronizar con Centro de partners:** Sí.
      - **Soluciones de Microsoft:** para compartir una referencia con Microsoft, agregue una solución válida lista para venta en colaboración o de Microsoft a la oportunidad.
      
        :::image type="content" source="images/dynamic-4a.png" alt-text="Captura de pantalla que muestra el identificador de la solución.":::

   1. Una vez creada la oportunidad en Dynamics 365 con la opción Sincronizar con **Centro de partners** establecida en Sí, espere 10 minutos. A continuación, inicie sesión en Centro de partners cuenta. Las referencias se sincronizarán con Dynamics 365 y el **identificador de referencia.** **El vínculo de** referencia se rellenará. Si se produce un error, el **campo Auditoría** se rellenará con información de error.
     
    1. Del mismo modo, para una oportunidad que tenía la opción Sincronizar con **Centro de partners** establecida en Sí, si actualiza la oportunidad en Dynamics 365 CRM, los cambios se sincronizarán en su cuenta de Centro de partners.

    1. Las oportunidades que se sincronizan correctamente con Centro de partners se identificarán con ✔icono en Dynamics 365.

1. Sincronización de referencias cuando la referencia se crea o actualiza en Centro de partners y se sincroniza en el entorno de Dynamics 365:

   1. Inicie sesión en el panel de Centro de partners [.](https://partner.microsoft.com/dashboard/home)

   1. Seleccione **Referencias en** el menú de la izquierda.

   1. Cree una nueva referencia de venta Centro de partners seleccionando la **opción Nueva oferta.**

   1. Inicie sesión en el entorno de Dynamics 365 CRM.

   1. Vaya a **Open Opportunities (Oportunidades abiertas).** La referencia creada en Centro de partners ahora está sincronizada en Dynamics 365 CRM.

   1. Al seleccionar una referencia sincronizada, se rellenan los detalles de la vista de tarjeta.

## <a name="next-steps"></a>Pasos siguientes

- [Administrar los clientes potenciales](manage-leads.md)
- [Administrar las oportunidades de venta conjunta](manage-co-sell-opportunities.md)
- [Más información sobre la plataforma Power Automate Microsoft](/power-automate/)
- [Webhooks del Centro de partners](/partner-center/develop/partner-center-webhooks)
