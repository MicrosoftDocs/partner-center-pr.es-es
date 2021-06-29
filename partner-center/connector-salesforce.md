---
title: El conector de venta co-sell para Salesforce CRM Centro de partners
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronice las referencias en Centro de partners con su CRM de Salesforce. A continuación, los vendedores pueden vender en colaboración con Microsoft desde sus sistemas CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.date: 06/28/2021
ms.openlocfilehash: f8cb4cd2488e55ab64cf7b7cdce4a3e950b266de
ms.sourcegitcommit: 6a6e8f9af0a58b32770c7fce9f567dd4795b9797
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/29/2021
ms.locfileid: "113029123"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Conector de venta conjunta para Salesforce CRM: información general

**Roles adecuados:** Administrador de referencias | Administrador del sistema o personalizador del sistema en CRM

Centro de partners conector de venta en colaboración permite a los vendedores realizar una venta en colaboración con Microsoft desde dentro de sus sistemas CRM. No tendrán que entrenarse para usar Centro de partners administrar ofertas de venta co-venta. Con los conectores de venta coventa, puede crear una nueva referencia de venta coventa para atraer a un vendedor de Microsoft, recibir referencias del vendedor de Microsoft, aceptar o rechazar referencias, modificar datos de oferta, como el valor de la oferta y la fecha de cierre.  También puede recibir cualquier actualización de los vendedores de Microsoft sobre estas ofertas de venta coventa. Puede hacer que todas las referencias funcionen mientras trabaja en el CRM de su elección en lugar de en Centro de partners.

La solución se basa en Microsoft Power Automate Solution y usa Centro de partners API.

## <a name="before-you-install---pre-requisites"></a>Antes de instalar: requisitos previos

|**Temas**|**Detalles**|**Vínculos**|
|--------------|--------------------|------|
|Microsoft Partner Network id. |Necesita un identificador de MPN válido.|Para unirse [a MPN](https://partner.microsoft.com/)|
|Listo para la venta conjunta|La solución IP/Services debe estar lista para la venta en colaboración.|[Venta con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)|
|Cuenta de Centro de partners|El identificador de MPN asociado al inquilino Centro de partners debe ser el mismo que el identificador de MPN asociado a la solución de venta simultánea. Compruebe que puede ver las referencias de venta Centro de partners portal antes de implementar los conectores.|[Administración de la cuenta](create-user-accounts-and-set-permissions.md)|
|Roles de usuario del Centro de partners|El empleado que instalará y usará los conectores debe ser un administrador de referencias.|[Asignar roles y permisos de usuarios](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|El rol de usuario de CRM es Administrador del sistema o Personalizador del sistema.|[Asignación de roles en Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow Account|Cree un nuevo entorno de producción con una base de datos para pruebas, ensayo y producción. Si tiene un entorno de producción existente con una base de datos, se puede reutilizar. El usuario que va a instalar la solución del conector debe tener una Power Automate licencia y acceso a este entorno. Puede supervisar el progreso y obtener más información en [Power Automate](https://flow.microsoft.com/) si se produce un error en la instalación. Seleccione **Ver historial en** **Soluciones.**|[Creación o administración del entorno](/power-platform/admin/create-environment#create-an-environment-with-a-database)|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Instalación del paquete de Salesforce para campos personalizados de Microsoft

Para sincronizar las referencias entre Centro de partners y Salesforce CRM, la solución Power Automate debe identificar claramente los campos de referencia específicos de Microsoft. Esta demarcación proporciona a los equipos de vendedores asociados la capacidad de decidir qué referencias quieren compartir con Microsoft para la venta en colaboración.

1. En Salesforce, active **Notes (Notas)** y agrégrélo a la lista de oportunidades relacionadas. [Referencia](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

1. Active **los equipos de oportunidad** siguiendo estos pasos:
    - En Configuración, use el cuadro **Búsqueda rápida para** buscar Configuración del equipo de oportunidades.
    - Defina la configuración según sea necesario. [Referencia](https://help.salesforce.com/articleView?id=sf.opp_team_manage.htm&type=5)

1. En Salesforce, instale campos y objetos personalizados mediante el [instalador de paquetes](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Use este instalador para instalar el paquete en cualquier empresa.

    >[!NOTE]
    >Si va a instalar en un espacio aislado, debe reemplazar la parte inicial de la dirección URL por `http://test.salesforce.com` .

1. En Salesforce, agregue Soluciones de Microsoft a la **lista relacionada** con oportunidades. Una vez agregado, seleccione el icono **de llave inglesa** y actualice las propiedades.

## <a name="best-practice-test-before-you-go-live"></a>Procedimiento recomendado: Prueba antes de empezar a realizar la ejecución

Antes de instalar, configurar y personalizar la solución Power Automate en el entorno de producción, asegúrese de probar la solución en una instancia de CRM de almacenamiento provisional.

- Instale microsoft Power Automate solución en un entorno de ensayo o una instancia de CRM.

- Realice una copia de la solución y ejecute la configuración y Power Automate de flujo en el entorno de ensayo.

- Pruebe la solución en una instancia de almacenamiento provisional o CRM.

- Si se ejecuta correctamente, importe como una solución administrada a la instancia de producción.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Instalación de Centro de partners de referencias para Salesforce CRM

1. Vaya a [Power Automate](https://flow.microsoft.com) seleccione **Entornos** en la esquina superior derecha. Esto le mostrará las instancias de CRM disponibles.

1. Seleccione la instancia de CRM adecuada en la lista desplegable de la esquina superior derecha.

1. Seleccione **Soluciones en** la barra de navegación izquierda.

1. Seleccione el **vínculo Abrir AppSource** en el menú superior.

   :::image type="content" source="images/cosellconnectors/open-appsource.png" alt-text="Abrir AppSource":::

1. Busque **conectores Centro de partners referencias** para Salesforce en la pantalla emergente.  

   :::image type="content" source="images/salesforce/salesforce-get-it-now.png" alt-text="Captura de pantalla de Obtenerla ahora.":::

1. Seleccione el **botón Obtener ahora** y, a continuación, seleccione **Continuar.**

1. En la página siguiente, seleccione el entorno de Salesforce CRM para instalar la aplicación. Acepte los términos y condiciones.

1. A continuación, se le dirigirá a la **página Administrar sus** soluciones.  Vaya a "Centro de partners referencias" mediante los botones de flecha de la parte inferior de la página. **La instalación programada debe** aparecer junto a Centro de partners de referencias. La instalación llevará entre 10 y 15 minutos.

1. Una vez completada la instalación, vuelva a [Power Automate](https://flow.microsoft.com) seleccione **Soluciones en** el área de navegación izquierda. Observe que **Centro de partners sincronización de referencias para Salesforce** ya está disponible en la lista Soluciones.

1. Seleccione **Centro de partners de referencias para Salesforce.** Las siguientes Power Automate y entidades están disponibles:

   :::image type="content" source="images/cosellconnectors/partner-center-referrals-synchronization.png" alt-text="Flujos de Salesforce":::

## <a name="configure-the-solution"></a>Configuración de la solución

1. Después de instalar la solución en la instancia de CRM, vuelva a [Power Automate](https://flow.microsoft.com/).

1. En la **lista desplegable Entornos** de la esquina superior derecha, seleccione la instancia de CRM donde instaló la Power Automate solución.

1. Deberá crear conexiones que asocie las tres cuentas de usuario:

   - Centro de partners usuario con credenciales de administrador de referencias
   - Eventos del Centro de partners
   - Administrador de CRM con los flujos Power Automate en la solución

   1. Seleccione **Conexiones** en la barra de navegación izquierda y seleccione la **solución Centro de partners Referencias** de la lista.

   1. Para crear una conexión, seleccione **Crear una conexión.**

        :::image type="content" source="images/cosellconnectors/dynamics-1.png" alt-text="Captura de pantalla que muestra Creación de una conexión.":::

   1. Busque Centro de partners **referencias (versión preliminar)** en la barra de búsqueda de la esquina superior derecha.

   1. Cree una conexión para el usuario Centro de partners con el rol de credenciales del administrador de referencias.

   1. A continuación, cree una Centro de partners events para el Centro de partners con las credenciales del administrador de referencias.

   1. Cree una conexión para Salesforce para el usuario administrador de CRM.
  
   1. Cree una conexión para Microsoft Dataverse para el usuario administrador de CRM.

   1. Después de agregar todas las conexiones, debería ver las siguientes conexiones en su entorno:

        :::image type="content" source="images/cosellconnectors/salesforce-connections.png" alt-text="Captura de pantalla que muestra cómo observar las conexiones.":::

### <a name="edit-the-connections"></a>Edición de las conexiones

1. Vuelva a la **página Soluciones** y seleccione **Solución predeterminada.** Seleccione **Connection Reference (preview) (Referencia de conexión [versión preliminar])** haciendo clic **en All (Todos).**

   :::image type="content" source="images/connection-reference-video.gif" alt-text="Captura de pantalla que muestra Edición de las conexiones.":::

1. Edite cada una de las conexiones individualmente seleccionando el icono de puntos suspensivos. Agregue las conexiones pertinentes.

   :::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Captura de pantalla que muestra cómo editar conectores.":::

1. Active los flujos en la secuencia siguiente:
   - Centro de partners webhook Registration (Insider Preview)
   - [Personalizar] Crear u obtener detalles de Salesforce
   - Creación de una Referral-Salesforce de venta Centro de partners (versión preliminar de Insider)
   - Centro de partners microsoft co-sell Referral Updates to Salesforce (Insider Preview)  
   - Centro de partners a Salesforce (Insider Preview)
   - Salesforce to Centro de partners (Insider Preview)
   - Salesforce Opportunity to Centro de partners (Insider Preview)
   - Soluciones de Salesforce Microsoft para Centro de partners (versión preliminar de Insider)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Uso de api de webhook para registrarse para eventos de cambio de recursos

Puede usar las API Centro de partners webhook para registrarse para eventos de cambio de recursos. Estos eventos de cambio se envían a la dirección URL como publicaciones HTTP.

1. Seleccione **Centro de partners a Salesforce CRM (Insider Preview).**

1. Seleccione el **icono Editar y** seleccione Cuando se recibe una solicitud **HTTP.**

1. Seleccione el **icono Copiar** para copiar la dirección URL de HTTP **POST proporcionada.**

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Captura de pantalla que muestra cómo copiar la dirección URL.":::

1. Seleccione el **flujo Centro de partners registro de webhooks (versión** preliminar de Insider) Power Automate, a continuación, seleccione **Ejecutar**.

1. Asegúrese de que la **ventana Ejecutar** flujo se abre en el panel derecho y seleccione **Continuar.**

1. Escriba la siguiente información:

   - **Punto de conexión de desencadenador HTTP:** esta dirección URL se copió de un paso anterior.
   - **Eventos para registrar:** seleccione todos los eventos disponibles **(creados** por **referencias,** actualizados por referencia, creados por **referencias** relacionadas y **actualizados por referencias relacionadas).**
   - **¿Sobrescribir los puntos de conexión de desencadenador existentes si están presentes?**: Sí. Solo se puede registrar una dirección URL para un evento de webhook determinado.

1. Seleccione **Run flow (Ejecutar** flujo) y, a continuación, **seleccione Done (Listo).**

El webhook ahora puede escuchar, crear y actualizar eventos.

## <a name="customize-synchronization-steps"></a>Personalización de los pasos de sincronización

Los sistemas CRM están muy personalizados y puede personalizar la solución Power Automate en función de la configuración de CRM. Cuando las referencias de venta co-sell se sincronizan entre Centro de partners y el sistema CRM, los campos que se sincronizan en el equipo Centro de partners se muestran en la Guía de asignación de campos [personalizados](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWxL6S).

Siga la guía de asignación de campos y, si es necesario, realice los cambios adecuados en **[Personalizar] Crear** u obtener detalles de Salesforce o variables de entorno. No actualice ningún otro flujo de la solución Power Automate porque puede afectar a futuras actualizaciones de la solución.

Están disponibles las siguientes personalizaciones:

- **Mostrar marca** de verificación en el nombre de la oportunidad: de forma predeterminada, se mostrará una marca de verificación junto al nombre de la oportunidad para indicar que la sincronización entre Centro de partners y Salesforce CRM se está produciendo correctamente. Del mismo modo, se mostrará una marca cruzada si se produce un error en la sincronización. Para evitar agregar una marca de verificación o una marca  cruzada en el nombre de la oportunidad, establezca el valor actual de la marca de verificación Mostrar de la variable de entorno de nombre de oportunidad en No.

- **Nombre de fase:**

  - **Nombre de fase activo:** esta es la fase de la canalización de ventas de una oportunidad en Salesforce.  Representa una fase activa y es equivalente a una referencia en estado aceptado en Centro de partners. Esta puede ser la siguiente fase de la canalización de ventas después de la fase en espera. Al mover la fase de ventas de La oportunidad de la fase en espera a la fase activa, se aceptará la referencia en Centro de partners y los cambios comenzarán a sincronizarse.

  - **Nombre de la fase en espera:** nombre de la fase en la canalización de ventas de una oportunidad en Salesforce. Representa una fase en espera. Las nuevas referencias de venta compartidas de Microsoft que aún no se han aceptado se establecerán en esta fase en Salesforce. Los cambios realizados en una oportunidad mientras está en fase de espera no se sincronizarán con Centro de partners. Al sacar la fase de ventas de la oportunidad de esta fase en espera, se aceptará la referencia en Centro de partners y los cambios comenzarán a sincronizarse.

- **Código de país de la** cuenta de cliente: es obligatorio proporcionar un código de país de dos letras (ISO 3166) al crear una nueva referencia. De forma predeterminada, el código de país se sincronizará con y desde el campo **BillingCountry** de la cuenta en Salesforce. Si tiene un campo diferente en Salesforce para el código de país desde el que se va a sincronizar:

  - Para un campo de código de país que no sealookup de la cuenta que contiene un código de dos letras:

    - Actualice el nombre **del campo Customer Account Country Code (Código** de país de la cuenta de cliente) en la variable de entorno salesforce con el nombre del campo de CRM. Asegúrese de proporcionar el nombre del campo, no su nombre para mostrar.

    - Edite **[Personalizar]** Cree u obtenga detalles de Salesforce y vaya **a** Crear u obtener una cuenta de cliente en la acción **crm** para asignar un valor de País al campo correcto en CRM. Además, quite la **asignación de** valor Country de **BillingCountry**.

  - Para un campo de código de país basado en búsqueda en la cuenta:

    - Agregue un nuevo campo personalizado en la cuenta y rellene automáticamente con un código de país de dos letras (ISO 3166) basado en el valor seleccionado en el campo basado en búsqueda y viceversa.

    - Siga los pasos anteriores para que el campo de código de país que no eslookup sincronice un nuevo campo personalizado desde CRM hacia y desde Centro de partners.

- **Valor de** la oferta: de forma predeterminada, el valor de la oferta Centro de partners se sincronizará con y desde **Amount** en crm. Si tiene un campo diferente en CRM para el valor de la oferta desde el que se va a sincronizar:

  - Actualice el **nombre del campo Valor** de la oferta en la variable de entorno de Salesforce con el nombre del campo de CRM. Asegúrese de proporcionar el nombre del campo, no su nombre para mostrar.

  - Edite **[Personalizar]** Cree u obtenga  detalles de Salesforce y vaya **a** Crear  o actualizar una oportunidad en CRM y actualice las acciones Crear una nueva oportunidad y Actualizar oportunidad existente para asignar **DealValue** al campo correcto en Salesforce.

- **Código de moneda del valor de la oferta:** nombre del campo de código de moneda del valor de la oferta en Salesforce. Este nombre de API de campo se usará para obtener el código de moneda del valor de oferta de Opportunity al crear o actualizar la referencia en Microsoft Centro de partners. Si el campo de código de moneda del valor de la oferta es diferente del **campo predeterminado CurrencyIsoCode,** actualice el valor actual de esta variable de entorno.

  - Actualice el nombre **del campo deal value currency** en la variable de entorno salesforce con el nombre del campo de CRM. Asegúrese de proporcionar el nombre del campo, no su nombre para mostrar.

  - Edite **[Personalizar]** Cree u obtenga  detalles de Salesforce y vaya **a** Crear  o actualizar una oportunidad en CRM y actualice las acciones Crear una nueva oportunidad y Actualizar oportunidad existente para asignar **DealValueCurrency** al campo correcto en Salesforce.

- **Oportunidad de venta compartida** de sincronización: si se establece en **sí,** solo las oportunidades de venta compartida y uso compartido de canalizaciones se sincronizarán de Centro de partners a Salesforce. Si se establece **en no ,** las oportunidades de uso compartido de clientes potenciales, venta compartida y canalización se sincronizarán de Centro de partners a Salesforce. Esta variable no tiene ningún impacto en las oportunidades sincronizadas entre Salesforce y Centro de partners.

## <a name="update-environment-variable"></a>Actualización de la variable de entorno

Para actualizar un valor de variable de entorno:

1. Vaya a la **página Soluciones** y seleccione **Solución predeterminada.** Seleccione **Variable de entorno** seleccionando **Todos.**

1. Seleccione la variable de entorno para el valor que debe actualizarse y seleccione **Editar** con el icono de puntos suspensivos.

1. Actualice **el valor actual** (no actualice el valor **predeterminado)** mediante la **opción Nuevo** valor y proporcionando el valor. El valor debe coincidir con el tipo de datos de la variable. Por ejemplo, el tipo de datos Sí o No aceptará el valor Sí o No.

   :::image type="content" source="images/cosellconnectors/environment-variables-video.gif" alt-text="Captura de pantalla que muestra Actualizar variables de entorno.":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronización de referencias de venta bidireccional de un extremo a otro

Después de instalar, configurar y personalizar la solución Power Automate, puede probar la sincronización de referencias de venta co-venta entre Salesforce CRM y Centro de partners.

### <a name="pre-requisites"></a>Requisitos previos

Para sincronizar las referencias entre Centro de partners y Salesforce CRM, la solución Power Automate debe delimitar claramente los campos de referencia específicos de Microsoft. Esta identificación proporciona a los equipos vendedores la capacidad de decidir qué referencias quieren compartir con Microsoft para la venta en colaboración.

Un conjunto de campos personalizados está disponible como parte de la Centro de partners sincronización de referencias para la oportunidad de la **solución** Salesforce CRM. Un usuario administrador de CRM deberá crear una sección de CRM independiente con los campos **personalizados oportunidad.**

Los siguientes campos personalizados deben formar parte de la sección CRM:

- **Sincronizar con Centro de partners:** si se debe sincronizar la oportunidad con Centro de partners. De forma predeterminada, el valor de este campo es No y el vendedor debe establecer explícitamente en Sí para compartir una oportunidad con Microsoft. Las nuevas referencias compartidas Centro de partners a CRM tendrán este valor de campo establecido en Sí.

- **Identificador de referencia:** campo de identificador de solo lectura para microsoft Centro de partners referencia.

- **Vínculo de referencia:** vínculo de solo lectura a la referencia en Microsoft Centro de partners.

- **¿Cómo puede ayudar Microsoft?**: Ayuda necesaria de Microsoft para la referencia. Para crear una referencia de venta co-sell, seleccione la ayuda adecuada necesaria de Microsoft. Un contacto con el cliente debe estar asociado a la oportunidad de crear una referencia de venta co-sell. Para crear una referencia que no sea de venta en colaboración, no seleccione este campo. Una referencia de venta no co-sell se puede convertir en una referencia de venta co-sell en cualquier momento seleccionando la opción adecuada de ayuda necesaria.

- **Visibilidad Centro de partners referencias de Microsoft:** seleccione visibilidad para la Centro de partners referencia. Al hacer que sea visible para los vendedores de Microsoft, una referencia de venta no coventa podría convertirse en venta en colaboración. Cuando se requiere ayuda de Microsoft, la referencia es visible para los vendedores de Microsoft de forma predeterminada. Una vez que este campo está marcado como visible, no se puede revertir.

- **Identificador de Microsoft CRM:** cuando Microsoft crea y acepta una referencia de venta en colaboración, este campo se rellena con el identificador de CRM de Microsoft.

- **Microsoft Centro de partners Solutions:** un objeto personalizado para asociar soluciones listas para la venta en colaboración o soluciones de Microsoft con la oportunidad. Se pueden agregar o quitar una o varias soluciones de la oportunidad. Es obligatorio agregar al menos una solución de Microsoft o lista para la venta compartida a la oportunidad antes de compartirla con Microsoft. Para asociar este objeto a la oportunidad, actualice el **formulario Oportunidad** en CRM.

- **Auditoría:** un registro de auditoría de solo lectura para sincronizar con Centro de partners referencias

### <a name="scenarios"></a>Escenarios

1. Sincronización de referencias cuando se crea o actualiza la referencia en CRM y se sincroniza en Centro de partners:

   1. Inicie sesión en el entorno de Salesforce CRM con el usuario que tenga visibilidad en la **sección Oportunidad** de CRM.

   1. Asegúrese de que la sección **Microsoft Centro de partners** presente al crear una nueva **oportunidad en** el entorno de Salesforce CRM.

   1. Las oportunidades que se sincronizan correctamente con Centro de partners se identificarán con ✔ icono en Salesforce CRM.
      :::image type="content" source="images/salesforce/salesforce-environment.png" alt-text="Captura de pantalla del entorno de Salesforce.":::

   1. Para sincronizar esta oportunidad con Microsoft Centro de partners, asegúrese de establecer los siguientes campos en la vista de tarjeta:

      - **¿Cómo puede ayudar Microsoft?**: Para crear una referencia de venta co-sell, seleccione una opción de ayuda adecuada.

        :::image type="content" source="images/salesforce/salesforce-help-option.png" alt-text="Captura de pantalla que muestra cómo obtener los campos adecuados en la vista de tarjeta.":::

      - **Sincronización con Centro de partners:** Sí
      - **Contacto del** cliente: para crear una referencia de venta en colaboración, agregue un contacto de cliente a la oportunidad.
      - **Soluciones de Microsoft:** para compartir una referencia con Microsoft, agregue a la oportunidad una solución válida lista para venta en colaboración o de Microsoft.

   1. Después de establecer la opción Sincronizar con **Centro de partners** en **Sí,** espere 10 minutos, inicie sesión en su cuenta Centro de partners cliente. Las referencias se sincronizarán con Salesforce CRM y se rellenará el vínculo de referencia. Si se produce un error, el campo Auditoría se rellenará con información de error.

   1. Del mismo modo, cuando la opción Sincronizar con **Centro de partners** está establecida en **Sí,** si actualiza la oportunidad en Salesforce CRM, los cambios se sincronizarán con la cuenta Centro de partners cliente.

2. Sincronización de referencias cuando se crea o actualiza la referencia en Microsoft Centro de partners y sincroniza en el entorno de Salesforce CRM:

    1. Inicie sesión en Centro de partners [panel](https://partner.microsoft.com/dashboard/home).

    1. Seleccione **Referencias en** el menú de la izquierda.

    1. Cree una nueva referencia de venta Centro de partners haga clic en la opción "New deal" (Nueva oferta).

    1. Inicie sesión en su entorno de Salesforce CRM.

    1. Vaya a **Open Opportunities (Oportunidades abiertas).** La referencia creada en Microsoft Centro de partners ahora está sincronizada en Salesforce CRM.

    1. Al seleccionar una referencia sincronizada, se rellenan los detalles de la vista de tarjeta.

       :::image type="content" source="images/salesforce/salesforce-casino.png" alt-text="Captura de pantalla de la página de oportunidades de Salesforce.":::

>[!NOTE]
>**¿Necesita ayuda con la implementación?**
>Para obtener ayuda con la implementación del conector de referencia de venta co-venta, puede interactuar con un consultor técnico de asociados. Pueden proporcionar asistencia para la implementación y procedimientos recomendados para una implementación correcta.
>
>Para más información, consulte Envío de una solicitud de servicios de [implementación y preventas técnicas.](technical-benefits.md)

## <a name="next-steps"></a>Pasos siguientes

- [Administrar los clientes potenciales](manage-leads.md)

- [Administrar las oportunidades de venta conjunta](manage-co-sell-opportunities.md)

- [Webhooks del Centro de partners](/partner-center/develop/partner-center-webhooks)
