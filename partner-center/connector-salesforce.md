---
title: El conector de venta conjunta para el centro de Partners de Salesforce CRM
ms.topic: article
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizar las referencias en el centro de Partners con el CRM de Salesforce
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: e51ddc8ec3ea568a20404801802548f79cae43d0
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991624"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Conector de venta conjunta para Salesforce CRM: información general

### <a name="appropriate-roles"></a>Roles adecuados

- Administrador de referencias
- Administrador del sistema o Personalizador del sistema en CRM

El conector de la venta conjunta del centro de Partners permite que los vendedores covendan con Microsoft desde los sistemas CRM. No tendrán que estar capacitados para utilizar el centro de partners para administrar las ofertas de venta conjunta. Mediante el uso de conectores de venta conjunta, puede crear una nueva referencia de venta conjunta para participar en un vendedor de Microsoft, recibir referencias del vendedor de Microsoft, aceptar o rechazar las referencias, modificar los datos del negocio, como el valor del negocio y la fecha de cierre.  También puede recibir cualquier actualización de los vendedores de Microsoft en estos acuerdos de venta conjunta. Puede hacer que todas las referencias funcionen mientras trabaja en el CRM de su elección, en lugar de hacerlo en el centro de Partners. 

La solución se basa en la solución Microsoft Power Automate y usa las API del centro de Partners.

## <a name="before-you-install---pre-requisites"></a>Antes de instalar: requisitos previos

|**Temas**   |**Detalles**   |**Vínculos**   |
|--------------|--------------------|------|
|IDENTIFICADOR de Microsoft Partner Network |Necesita un ID. de MPN válido|Para unirse a [MPN](https://partner.microsoft.com/)|
|Venta conjunta lista|La solución de IP/servicios debe estar lista para su venta conjunta.|[Venda con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Cuenta del Centro de partners|El identificador de MPN asociado al inquilino del centro de Partners debe ser el mismo que el identificador de MPN asociado a la solución de venta conjunta. Compruebe que puede ver las referencias de venta conjunta en el portal del centro de Partners antes de implementar los conectores.|[Administración de la cuenta](create-user-accounts-and-set-permissions.md)|
|Roles de usuario del Centro de partners|El empleado que va a instalar y usar los conectores debe ser un administrador de referencias.|[Asignar roles y permisos de usuarios](create-user-accounts-and-set-permissions.md)|
|CRM de Salesforce|El rol de usuario CRM es administrador del sistema o Personalizador del sistema|[Asignación de roles en el CRM de Salesforce](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|Cuenta de flujo de automatización de energía|Una cuenta activa de [Power Automatic](https://flow.microsoft.com) para el administrador del sistema CRM o el personalizador del sistema. Dicho usuario debe iniciar sesión en [Power automatizate](https://flow.microsoft.com) al menos una vez antes de la instalación.|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Instalación de la sincronización de referencias del centro de partners para Salesforce CRM

1. Vaya a [Power Automatic](https://flow.microsoft.com) y seleccione **entornos** en la esquina superior derecha. Se mostrarán las instancias de CRM disponibles.

2. Seleccione la instancia de CRM correspondiente en la lista desplegable de la esquina superior derecha.

3. Seleccione **soluciones** en la barra de navegación izquierda.

4. Haga clic en el vínculo **abrir AppSource** en el menú superior.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abrir AppSource":::

5. Busque **conectores de referencias del centro de partners para Salesforce** en la pantalla emergente.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. Haga clic en el botón **obtener ahora** y **continúe**.

7. Se abrirá la página en la que puede seleccionar el entorno de Salesforce CRM para instalar la aplicación.  Acepte los términos y condiciones.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRMS disponibles":::

8. A continuación, se le dirigirá a la página **administrar soluciones** .  Vaya a "referencias del centro de Partners" con los botones de flecha de la parte inferior de la página. La **instalación programada** debe aparecer junto a la solución de referencias del centro de Partners. La instalación tardará 10-15 minutos.

9. Una vez completada la instalación, vuelva a [Power Automatic](https://flow.microsoft.com) y seleccione **soluciones** en el área de navegación izquierda. Observe que la **sincronización de referencias del centro de partners para Salesforce** está disponible en la lista de soluciones.

10. Seleccione la **sincronización de referencias del centro de partners para Salesforce**. Están disponibles los siguientes flujos y entidades:

    :::image type="content" source="images/salesforce/salesforce-flows.png" alt-text="Flujos de Salesforce":::

## <a name="best-practice-test-before-you-go-live"></a>Procedimiento recomendado: prueba antes de la marcha

Antes de instalar, configurar y personalizar la solución Power Automate en el entorno de producción, asegúrese de probar la solución en una instancia de CRM provisional.

- Instale la solución Microsoft Power Automate en un entorno de ensayo o una instancia de CRM.

- Realice una copia de la solución y ejecute la configuración y la automatización de las personalizaciones de flujo en el entorno de ensayo.

- Pruebe la solución en una instancia de ensayo o CRM.

- En caso de éxito, importe como solución administrada a la instancia de producción.

## <a name="configure-the-solution"></a>Configuración de la solución

1. Una vez que haya instalado la solución en la instancia de CRM, vuelva a [Power Automatic](https://flow.microsoft.com/).

2. En la lista desplegable de **entornos** de la esquina superior derecha, seleccione la instancia de CRM en la que instaló la solución Power Automatic.

3. Tendrá que crear conexiones que asocien las tres cuentas de usuario:

   - Usuario del centro de Partners con credenciales de administrador de referencias
   - Eventos del Centro de partners
   - Administrador de CRM con la potencia que automatiza los flujos en la solución.

   1. Seleccione **conexiones** en la barra de navegación izquierda y seleccione la solución "referencias del centro de Partners" en la lista.

   2. Cree una conexión haciendo clic en **crear una conexión**.

       :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Crear conexión":::

   3. Busque **referencias del centro de Partners (versión preliminar)** en la barra de búsqueda de la esquina superior derecha.

   4. Cree una conexión para el usuario del centro de Partners con el rol de credenciales de administrador de referencias.

   5. A continuación, cree una conexión de eventos del centro de partners para el usuario del centro de Partners con las credenciales de administrador de referencias.

   6. Cree una conexión para Common Data Service (entorno actual) para el usuario administrador de CRM.

4. Para asociar los flujos de alimentación automatizada con las conexiones, edite cada uno de los flujos de Power Automatic para conectarse a Common Data Service y a las referencias del centro de Partners. Guarde los cambios.

5. **Encienda** los flujos automatizar energía.

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Uso de las API de webhook para registrar eventos de cambio de recursos

Las API del webhook del centro de Partners le permiten registrarse para los eventos de cambio de recursos. Estos eventos de cambio se envían a la dirección URL como publicaciones HTTP.

1. Para registrar la dirección URL, seleccione **registro de webhook del centro de Partners (versión preliminar de Insider)** flujo de automatización.

2. Agregar conexiones para () Usuario del centro de Partners con credenciales de administrador de referencias (b.) Eventos del centro de Partners, tal y como se resalta

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Desencadenador":::

3. Cuando realice estas actualizaciones, verá

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. Guarde los cambios y seleccione **Activar**.

   Para permitir que los webhooks del centro de Partners escuchen los cambios de eventos, realice los pasos siguientes:

5. Seleccione **centro de partners para Salesforce CRM (versión preliminar de Insider)**.

6. Seleccione el icono de **edición** y seleccione **cuando se reciba una solicitud HTTP**.

7. Seleccione el icono de **copiar** para copiar la dirección URL http post proporcionada.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copiar la dirección URL":::

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

   1. Seleccione centro de partners para Salesforce CRM (versión preliminar de Insider).

   2. Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.

   3. Seleccione **(ámbito) sincronizar el cliente potencial o la oportunidad**.

2. Para personalizar las asignaciones de campos de CRM para crear eventos, seleccione **si es nueva oportunidad compartida y, a continuación**, haga clic en. Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda **la sección creación de una nueva oportunidad en CRM**. Puede editar las asignaciones en esta sección mediante la guía de asignación de campos.

   1. Para personalizar las asignaciones de campos de CRM para los eventos de actualización, haga clic en el paso "(ámbito) sincronizar el cliente potencial o la oportunidad".

   2. Seleccione **si se trata de una actualización de una oportunidad**. Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda **si la diferencia entre los objetos de oportunidad del centro de Partners y CRM**.  

   3. Seleccione **si sí** seguido de **Actualizar oportunidad existente** .

3. Para personalizar los campos de la sincronización de referencia de CRM a equipo para eventos de actualización:

   1. Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.

   2. Seleccione **(ámbito) sincronizar la oportunidad**.

   3. Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para eventos de actualización, seleccione **si hay diferencias entre los objetos de cliente potencial del centro de Partners y CRM y, a continuación, haga clic en**.

   4. Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda el paso **actualizar una referencia con los datos de oportunidad**.

   Puede editar las asignaciones en esta sección basándose en la guía de asignación de campos.

4. Para personalizar los campos de la sincronización de referencia de CRM a equipo para crear eventos

   1. Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.

   2. Seleccione **(ámbito) sincronizar referencias.**

   3. Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para crear eventos, seleccione **crear referencia de Microsoft**.

Puede editar las asignaciones en esta sección basándose en la guía de asignación de campos.

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a>Crear una sección independiente en el diseño de oportunidades de Salesforce CRM

Para sincronizar las referencias entre el centro de Partners y el CRM de Salesforce, la solución Power Automate debe delimitar claramente los campos de referencia específicos de Microsoft. Esto proporciona a los equipos de los vendedores la capacidad de decidir qué referencias desean compartir con Microsoft para la venta conjunta.

Un conjunto de campos personalizados está disponible como parte de la sincronización de referencias del centro de partners para la entidad de **oportunidad** de CRM de Salesforce. Un usuario administrador de CRM tendrá que crear una sección de CRM independiente con los campos personalizados de la **oportunidad** .
El usuario administrador de Salesforce CRM deberá crear una sección de CRM independiente.

Los siguientes campos personalizados deben formar parte de la sección CRM:

- **Sincronizar con el centro de Partners**: si se va a sincronizar la oportunidad con el centro de Partners de Microsoft

- **Identificador de referencia**: un campo de identificador de solo lectura para la referencia del centro de Partners de Microsoft

- **Vínculo de referencia**: un vínculo de solo lectura a la referencia en el centro de Partners de Microsoft

- **¿Cómo puede ayudarle Microsoft?** Ayuda necesaria de Microsoft para la referencia

- **Productos**: lista de productos asociados a esta oportunidad

- **Audit**: una pista de auditoría de solo lectura para la sincronización con la referencia del centro de Partners de Microsoft

### <a name="set-up-fields-and-relationships"></a>Configurar campos y relaciones

1. Inicie sesión en su cuenta de Salesforce y vaya a la **oportunidad**.

2. Haga clic en las opciones de **configuración** y **Editar objeto** para agregar los campos necesarios.

3. Seleccionar **campos & relaciones** en el panel de navegación izquierdo

   :::image type="content" source="images/salesforce/fields1.png" alt-text="Fields":::

4. Agregue los campos siguientes en los **campos &** tabla de relaciones:

   |**Etiqueta de campo**   |**Nombre del campo**|**Tipo de datos**|**Indizó**|
   |---------------------|:-------------------|:--------------|:----------------|
   |Auditoría| Audit__c|Área de texto largo (100.000) (línea visible 4)||
   |¿Cómo puede ayudarle Microsoft?|How_can_Microsoft_help_c|Lista desplegable|
   |Productos|Products_c|texto (255)||
   |Referral | Referral_Identfier_c|Texto (100) (ID. externo)|sí|
   |Vínculo de referencia| Referral_Link_c_|URL (255)||
   |Sincronizar con el centro de Partners|sync_with_partner_center_c|CheckBox (valor predeterminado desactivado)||

   * Valores de lista desplegable:

   - Propuesta de valor específico de carga de trabajo
   - Arquitectura técnica del cliente
   - Prueba de concepto o demostración
   - Comillas o licencias
   - Éxito del cliente de ventas
   - General u otro

5. Los campos se crearían en **campos & relaciones**

   :::image type="content" source="images/salesforce/fields2.png" alt-text="Campos creados":::

6. En el diseño de la oportunidad, cree una sección independiente con los campos indicados anteriormente.

   - Esta sección debe estar disponible para los vendedores en el diseño de la oportunidad.

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="Diseño de campos del centro de Partners":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronización de referencia de venta conjunta bidireccional de un extremo a otro

Una vez que haya instalado, configurado y personalizado la solución Power Automate, puede probar la sincronización de referencias de venta conjunta entre el centro de Partners y el CRM de Salesforce.

### <a name="pre-requisites"></a>Requisitos previos

Para sincronizar las referencias entre el centro de Partners y el CRM de Salesforce, la solución Power Automate debe delimitar claramente los campos de referencia específicos de Microsoft. Esta identificación proporciona a los equipos de los vendedores la capacidad de decidir qué referencias desean compartir con Microsoft para la venta conjunta.

Un conjunto de campos personalizados está disponible como parte de la sincronización de referencias del centro de partners para la entidad de **oportunidad** de la solución CRM de Salesforce. Un usuario administrador de CRM tendrá que crear una sección de CRM independiente con los campos personalizados de la **oportunidad** .

Los siguientes campos personalizados deben formar parte de la sección CRM:

- **Sincronizar con el centro de Partners**: si se va a sincronizar la oportunidad con el centro de Partners de Microsoft

- **Identificador de referencia**: un campo de identificador de solo lectura para la referencia del centro de Partners de Microsoft

- **Vínculo de referencia**: un vínculo de solo lectura a la referencia en el centro de Partners de Microsoft

- **Ayuda de Microsoft**: ayuda de Microsoft para la referencia

- **Productos**: lista de productos asociados a esta oportunidad

- **Audit**: una pista de auditoría de solo lectura para la sincronización con las referencias del centro de Partners

### <a name="scenarios"></a>SITUACIÓN

1. Sincronización de referencia cuando se crea o actualiza una referencia en CRM y se sincroniza en el centro de Partners:

   1. Inicie sesión en el entorno de Salesforce CRM con un usuario que tenga visibilidad en la sección de **oportunidades** de CRM.

   2. Asegúrese de que la siguiente sección está presente al crear una "nueva oportunidad" en el entorno de CRM de Salesforce.

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Entorno de Salesforce":::

   3. Para sincronizar esta oportunidad con el centro de Partners de Microsoft, asegúrese de establecer los siguientes campos en la vista tarjeta:

       - "Sincronizar con el centro de Partners": sí
       - "¿Cómo puede ayuda de Microsoft?": Seleccione una de las siguientes opciones:
       - Productos: identificadores de la solución del producto

   4. Una vez que haya establecido la opción de sincronización de oportunidades **con el centro de Partners** en **sí**, espere 10 minutos, inicie sesión en su cuenta del centro de Partners. Las referencias se sincronizarán con el CRM de Salesforce.

   5. Cuando la opción "sincronizar con el centro de Partners" está establecida en "sí", si actualiza la oportunidad en el CRM de Salesforce, los cambios se sincronizarán con la cuenta del centro de Partners.

   6. Las oportunidades que se sincronizan correctamente con el centro de Partners se identificarán con ✔ icono en la CRM de Salesforce.

2. Sincronización de referencia cuando se crea o actualiza una referencia en el centro de Partners de Microsoft y se sincroniza en el entorno de Salesforce CRM:

    1. Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard/home)del centro de Partners.

    2. Seleccione **referencias** en el menú de la izquierda.

    3. Cree una nueva referencia de venta conjunta desde el centro de partners; para ello, haga clic en la opción "nuevo trato".

    4. Inicie sesión en el entorno de Salesforce CRM.

    5. Vaya a **abrir oportunidades**. La referencia creada en el centro de Partners de Microsoft ya está sincronizada en el CRM de Salesforce.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Pantalla de oportunidad de Salesforce":::

    6. Al seleccionar una referencia sincronizada, se rellenan los detalles de la vista de tarjeta.

## <a name="next-steps"></a>Pasos siguientes

- [¿Más información sobre la plataforma Microsoft Power Automate?](https://docs.microsoft.com/-automate/)

- [Administrar los clientes potenciales](manage-leads.md)

- [Administrar las oportunidades de venta conjunta](manage-co-sell-opportunities.md)

- [Webhooks del Centro de partners](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)