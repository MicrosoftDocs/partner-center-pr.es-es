---
title: El conector de venta co-sell para Salesforce CRM Centro de partners
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronice las referencias en Centro de partners con salesforce CRM. A continuación, los vendedores pueden vender en colaboración con Microsoft desde dentro de sus sistemas CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 8139f89a37048b1790353e3bdd18ac1b44887219
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284390"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Conector de venta conjunta para Salesforce CRM: información general

**Roles adecuados**

- Administrador de referencias
- Administrador del sistema o personalizador del sistema en CRM

Centro de partners conector de venta en colaboración permite a los vendedores realizar la venta en colaboración con Microsoft desde dentro de los sistemas CRM. No tendrán que entrenarse para usar Centro de partners administrar las ofertas de venta co-venta. Con los conectores de venta coventa, puede crear una nueva referencia de venta conjunto para interactuar con un vendedor de Microsoft, recibir referencias del vendedor de Microsoft, aceptar o rechazar referencias, modificar los datos de la oferta, como el valor de la oferta y la fecha de cierre.  También puede recibir cualquier actualización de los vendedores de Microsoft en estas ofertas de venta coventa. Puede hacer que todas las referencias funcionen mientras trabaja en el CRM que prefiera, en lugar de hacerlo Centro de partners. 

La solución se basa en microsoft Power Automate solución y usa Centro de partners API.

## <a name="before-you-install---pre-requisites"></a>Antes de instalar: requisitos previos

|**Temas**   |**Detalles**   |**Vínculos**   |
|--------------|--------------------|------|
|Microsoft Partner Network id. |Necesita un identificador de MPN válido.|Para unirse [a MPN](https://partner.microsoft.com/)|
|Listo para la venta conjunta|La solución ip/services debe estar lista para la venta en colaboración.|[Vender con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Cuenta de Centro de partners|El identificador de MPN asociado al inquilino Centro de partners debe ser el mismo que el identificador de MPN asociado a la solución de venta simultánea. Compruebe que puede ver las referencias de venta Centro de partners portal antes de implementar los conectores.|[Administración de la cuenta](create-user-accounts-and-set-permissions.md)|
|Roles de usuario del Centro de partners|El empleado que instalará y usará los conectores debe ser un administrador de referencias.|[Asignar roles y permisos de usuarios](create-user-accounts-and-set-permissions.md)|
|Salesforce CRM|El rol de usuario de CRM es Administrador del sistema o Personalizador del sistema.|[Asignación de roles en Salesforce CRM](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|Power Automate Flow Account|Una cuenta [Power Automate](https://flow.microsoft.com) activa para el administrador del sistema CRM o el personalizador del sistema. Ese usuario debe iniciar sesión en [Power Automate](https://flow.microsoft.com) al menos una vez antes de la instalación.|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a>Instalación del paquete de Salesforce para campos personalizados de Microsoft 

Para sincronizar las referencias entre Centro de partners y Salesforce CRM, la solución Power Automate debe identificar claramente los campos de referencia específicos de Microsoft. Esta demarcación proporciona a los equipos de vendedores asociados la capacidad de decidir qué referencias quieren compartir con Microsoft para la venta en colaboración.

1. En Salesforce, active **Notes (Notas)** y agrégrélo a la lista de oportunidades relacionadas. 
[Referencia](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. Active **los equipos de oportunidad** siguiendo estos pasos: 
    - En Configuración, use el cuadro **Búsqueda rápida para** buscar Configuración del equipo de oportunidades.
    - Defina la configuración según sea necesario.
[Referencia](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. En Salesforce, instale campos y objetos personalizados mediante el [instalador de paquetes](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV). Úsese esto para instalar el paquete en cualquier empresa.

>[!NOTE]
>Si va a instalar en un espacio aislado, debe reemplazar la parte inicial de la dirección URL por http://test.salesforce.com

4. En Salesforce, agregue Soluciones de Microsoft a la **lista relacionada** con oportunidades. Una vez agregado, seleccione el icono **de llave inglesa** y actualice las propiedades.

## <a name="best-practice-test-before-you-go-live"></a>Procedimiento recomendado: Prueba antes de empezar a realizar la ejecución

Antes de instalar, configurar y personalizar la solución Power Automate en el entorno de producción, asegúrese de probar la solución en una instancia de CRM de almacenamiento provisional.

- Instale microsoft Power Automate solución en un entorno de ensayo o una instancia de CRM.

- Realice una copia de la solución y ejecute la configuración y Power Automate de flujo en el entorno de ensayo.

- Pruebe la solución en una instancia de almacenamiento provisional o CRM.

- Si se ejecuta correctamente, importe como una solución administrada a la instancia de producción.

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Instalación de Centro de partners de referencias para Salesforce CRM

1. Vaya a [Power Automate](https://flow.microsoft.com) y seleccione **Entornos en** la esquina superior derecha. Esto le mostrará las instancias de CRM disponibles.

2. Seleccione la instancia de CRM adecuada en la lista desplegable de la esquina superior derecha.

3. Seleccione **Soluciones en** la barra de navegación izquierda.

4. Seleccione el **vínculo Abrir AppSource** en el menú superior.

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abrir AppSource":::

5. Busque **conectores Centro de partners referencias** para Salesforce en la pantalla emergente.  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. Seleccione el **botón Obtenerla ahora** y, a continuación, **Continuar.**

7. Se abrirá la página donde puede seleccionar el entorno de Salesforce CRM para instalar la aplicación.  Acepte los términos y condiciones.

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRMS disponibles":::

8. A continuación, se le dirigirá a la **página Administrar sus soluciones.**  Vaya a "Centro de partners referencias" mediante los botones de flecha de la parte inferior de la página. **La instalación programada debe** aparecer junto a Centro de partners Solución de referencias. La instalación llevará de 10 a 15 minutos.

9. Una vez completada la instalación, vuelva a [Power Automate](https://flow.microsoft.com) seleccione **Soluciones en** el área de navegación izquierda. Observe que **Centro de partners sincronización de referencias para Salesforce** está disponible en la lista Soluciones.

10. Seleccione **Centro de partners de referencias para Salesforce.** Las siguientes Power Automate y entidades están disponibles:

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Flujos de Salesforce":::



## <a name="configure-the-solution"></a>Configuración de la solución

1. Una vez que haya instalado la solución en la instancia de CRM, vuelva a [Power Automate](https://flow.microsoft.com/).

2. En la **lista desplegable Entornos** de la esquina superior derecha, seleccione la instancia de CRM donde instaló la Power Automate solución.
3. Deberá crear conexiones que asocie las tres cuentas de usuario:
    - Centro de partners usuario con credenciales de administrador de referencias
    - Eventos del Centro de partners
    - El administrador de CRM con Power Automate flujos de la solución.
4. Seleccione **Conexiones** en la barra de navegación izquierda y seleccione la solución "Centro de partners Referencias" de la lista.

5. Cree una conexión haciendo clic en **Crear una conexión.**

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Crear conexión":::

- Busque Centro de partners referencias (versión preliminar) en la barra de búsqueda de la esquina superior derecha.

- Cree una conexión para el usuario Centro de partners con el rol de credenciales del administrador de referencias.

-  A continuación, cree una Centro de partners events para el Centro de partners con las credenciales del administrador de referencias.

- Cree una conexión para Salesforce para el usuario administrador de CRM.

-  Una vez que haya agregado todas las conexiones, debería ver las siguientes conexiones en su entorno:

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Observar conexiones":::

### <a name="edit-the-connections"></a>Edición de las conexiones

1. Vuelva a la página Soluciones y seleccione **Solución predeterminada.**  Seleccione **Connection Reference (preview) (Referencia de conexión [versión preliminar])** haciendo clic **en All (Todos).**
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Inicio de la edición del conector":::

2. Edite cada una de las conexiones individualmente seleccionando el icono de tres puntos. Agregue las conexiones pertinentes.

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Edición de conectores":::

3. Active los flujos en la secuencia siguiente:

- Centro de partners webhook Registration (Insider Preview)
- Creación de una referencia de venta co-venta: Salesforce Centro de partners (versión preliminar de Insider)
- Centro de partners microsoft co-sell Referral Updates to Salesforce (Insider Preview)
- Centro de partners a Salesforce (Insider Preview)
- Salesforce to Centro de partners (Insider Preview)
- Salesforce Opportunity to Centro de partners (Insider Preview)
- Soluciones de Salesforce microsoft para Centro de partners (versión preliminar de Insider)

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a>Uso de api de webhook para registrarse para eventos de cambio de recursos

Las CENTRO DE PARTNERS webhook permiten registrarse para eventos de cambio de recursos. Estos eventos de cambio se envían a la dirección URL como publicaciones HTTP.

1. Para registrar la dirección URL, **seleccione Centro de partners webhook Registration (Insider Preview) (Registro de webhook [insider preview])** Power Automate flujo.

2. Agregue conexiones para (a.) Centro de partners usuario con credenciales de administrador de referencias (b.) Centro de partners Eventos, como se resalta a continuación.

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Desencadenador":::

3. Al realizar estas actualizaciones, verá

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. Guarde los cambios y seleccione **Activar**.

   Para habilitar Centro de partners webhooks para escuchar los cambios de eventos, realice los pasos siguientes:

5. Seleccione **Centro de partners a Salesforce CRM (Insider Preview).**

6. Seleccione el **icono Editar** y seleccione Cuando se recibe una **solicitud HTTP.**

7. Seleccione el **icono Copiar** para copiar la dirección URL de HTTP POST proporcionada.

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copiar la dirección URL":::

8. Ahora, seleccione el flujo de Centro de partners registro de webhook (insider preview)Power Automate" y seleccione **Ejecutar**.

9. Asegúrese de que se abre la ventana "Flujo de ejecución" en el panel derecho y seleccione **Continuar.**

10. Escriba la siguiente información:

    1. **Punto de conexión de desencadenador http:** dirección URL copiada del paso anterior

    2. **Eventos para registrar:**"creados por referencia" y "actualizados por referencia"

    3. **Sobrescribir los puntos de conexión de desencadenador existentes si están** presentes: Sí (esto sobrescribe los puntos de conexión existentes).

11. Seleccione **Ejecutar y,** a continuación, **seleccione Listo.**

El webhook ahora puede escuchar para crear y actualizar eventos.

## <a name="customize-synchronization-steps"></a>Personalización de los pasos de sincronización

Cuando se sincronizan las referencias de venta Centro de partners y el sistema CRM, los campos que se sincronizan en Centro de partners PC se enumeran aquí.

A menudo, los sistemas CRM están muy personalizados. Puede personalizar los flujos de Power Automate datos. Siga la guía de asignación de campos y, si es necesario, realice los cambios adecuados en los pasos de Power Automate flujos.  Se proporcionan asignaciones de Centros de partners de Microsoft a CRM, pero en función de su entorno crm, puede optar por personalizar aún más los campos.

Varios pasos de cada uno de los Power Automate se pueden personalizar en función de sus necesidades. A continuación se muestran ejemplos de personalizaciones disponibles:

1. Para personalizar los campos de los eventos de creación o actualización en el Centro de partners sincronización de referencias de CRM:

   1. Seleccione Centro de partners a Salesforce CRM (Insider Preview).

   2. Seleccione **Editar** para editar o personalizar el flujo Power Automate datos.

   3. Seleccione **(Ámbito) Sincronizar el cliente potencial o la oportunidad.**

2. Para personalizar las asignaciones de campos de CRM para crear eventos, seleccione Si es una nueva **oportunidad compartida y, a continuación,**. Seleccione el subes paso si **es así y,** a continuación, expanda **Crear una nueva oportunidad en CRM.** Puede editar las asignaciones de esta sección mediante la Guía de asignación de campos.

   1. Para personalizar las asignaciones de campos de CRM para eventos de actualización, seleccione el paso "(Ámbito) Sincronizar el cliente potencial u oportunidad".

   2. Seleccione **Si se trata de una actualización de una oportunidad, a continuación,**. Seleccione el subes paso en caso afirmativo **y,** a continuación, expanda If difference between the opportunity objects in Centro de partners and CRM (Si la diferencia entre los objetos de oportunidad **de Centro de partners y CRM), a continuación, .**  

   3. Seleccione **If yes (Si es así)** seguido de **Update existing opportunity (Actualizar oportunidad existente).**

3. Para personalizar los campos para la sincronización de referencias de CRM a PC para eventos de actualización:

   1. Seleccione **Editar**  para editar o personalizar el flujo Power Automate datos.

   2. Seleccione **(Ámbito) Sincronizar la oportunidad.**

   3. Para personalizar las asignaciones de campos de CRM (basadas en la guía de asignaciones de campos) para eventos de actualización, seleccione Si hay diferencias entre los objetos de cliente potencial **en Centro de partners y CRM y, a continuación,**.

   4. Seleccione el subescalón en **caso afirmativo y,** a continuación, expanda el paso **Actualizar una referencia con datos de oportunidad**.

   Puede editar las asignaciones de esta sección en función de la Guía de asignación de campos.

4. ¿Para personalizar los campos de sincronización de referencia de CRM a PC para crear eventos?

   1. Seleccione **Editar**  para editar o personalizar el flujo Power Automate datos.

   2. Seleccione **(Ámbito) Sincronizar referencias.**

   3. Para personalizar las asignaciones de campos de CRM (basadas en la guía de asignaciones de campos) para crear eventos, seleccione **Crear referencia de Microsoft.**

Puede editar las asignaciones de esta sección en función de la Guía de asignación de campos.


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronización de referencias de venta bidireccional de un extremo a otro

Una vez que haya instalado, configurado y personalizado la solución Power Automate, puede probar la sincronización de referencias de venta co-venta entre Salesforce CRM y Centro de partners.

### <a name="pre-requisites"></a>Requisitos previos

Para sincronizar las referencias entre Centro de partners y Salesforce CRM, la solución Power Automate debe delimitar claramente los campos de referencia específicos de Microsoft. Esta identificación proporciona a los equipos vendedores la capacidad de decidir qué referencias quieren compartir con Microsoft para la venta en colaboración.

Un conjunto de campos personalizados está disponible como parte de la Centro de partners de referencias para la entidad de oportunidad de **la** solución Salesforce CRM. Un usuario administrador de CRM deberá crear una sección de CRM independiente con los **campos personalizados oportunidad.**

Los siguientes campos personalizados deben formar parte de la sección CRM:

- **Sincronización con Centro de partners:** si se debe sincronizar la oportunidad con Microsoft Centro de partners

- **Identificador de referencia:** campo de identificador de solo lectura para microsoft Centro de partners referencia

- **Vínculo de referencia:** vínculo de solo lectura a la referencia en Microsoft Centro de partners

- **Ayuda de Microsoft:** Ayuda necesaria de Microsoft para la referencia

- **Productos:** lista de productos asociados a esta oportunidad

- **Auditoría:** un registro de auditoría de solo lectura para sincronizar con Centro de partners referencias

### <a name="scenarios"></a>Escenarios:

1. Sincronización de referencias cuando se crea o actualiza la referencia en CRM y se sincroniza en Centro de partners:

   1. Inicie sesión en el entorno de Salesforce CRM con el usuario que tenga visibilidad en la **sección Oportunidad** de CRM.

   2. Asegúrese de que la siguiente sección está presente al crear una "nueva oportunidad" en el entorno de Salesforce CRM.

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Entorno de Salesforce":::

   3. Para sincronizar esta oportunidad con Microsoft Centro de partners, asegúrese de establecer los siguientes campos en la vista de tarjeta:

       - "Sincronizar con Centro de partners": Sí
       - "¿Cómo puede ayudar Microsoft?": seleccione una de las siguientes opciones:
       - Productos: los IDs de solución del producto

   4. Una vez que haya establecido la opción  **Sincronizar** con Centro de partners **en** Sí, espere 10 minutos, inicie sesión en Centro de partners cuenta. Las referencias se sincronizarán con Salesforce CRM.

   5. Cuando la opción "Sincronizar con Centro de partners" está establecida en "Sí", si actualiza la oportunidad en Salesforce CRM, los cambios se sincronizarán con la cuenta Centro de partners cliente.

   6. Las oportunidades que se sincronizan correctamente con Centro de partners se identificarán con ✔icono en Salesforce CRM.

2. Sincronización de referencias cuando se crea o actualiza la referencia en Microsoft Centro de partners y sincroniza en el entorno de Salesforce CRM:

    1. Inicie sesión en Centro de partners [panel](https://partner.microsoft.com/dashboard/home).

    2. Seleccione **Referencias en** el menú de la izquierda.

    3. Cree una nueva referencia de venta Centro de partners haga clic en la opción "New deal" (Nueva oferta).

    4. Inicie sesión en su entorno de Salesforce CRM.

    5. Vaya a **Open Opportunities (Oportunidades abiertas).** La referencia creada en Microsoft Centro de partners ahora está sincronizada en Salesforce CRM.

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Pantalla de oportunidades de Salesforce":::

    6. Al seleccionar una referencia sincronizada, se rellenan los detalles de la vista de tarjeta.

## <a name="next-steps"></a>Pasos siguientes

- [Administrar los clientes potenciales](manage-leads.md)

- [Administrar las oportunidades de venta conjunta](manage-co-sell-opportunities.md)

- [Webhooks del Centro de partners](/partner-center/develop/partner-center-webhooks)
