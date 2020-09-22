---
title: Solución de problemas de conectores de referencias de venta conjunta
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Preguntas más frecuentes sobre cómo solucionar problemas de conectores de venta conjunta.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: ad09d7c805ce5a1138d7546fd041ae1eda77b00c
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/22/2020
ms.locfileid: "91003003"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Solución de problemas de conectores de referencias de venta conjunta

**Se aplica a:**

- Centro de partners
- Dynamics 365 CRM
- CRM de Salesforce

**Roles adecuados**

- Administrador de referencias
- Administrador del sistema o Personalizador del sistema en CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Preguntas y respuestas sobre los requisitos previos

1. ¿Puede usar una solución de conectores de referencias de venta conjunta de prueba para su entorno?

Si está en el entorno de prueba o ensayo, puede optar por la solución de prueba. La versión de pago de los conectores está disponible en AppSource en US $15/month. Con la conexión de pago, obtendrá 10 000 llamadas API al día. Los conectores son contenedores que se encuentran en la parte superior de las API de referencia del centro de Partners. Cada vez que se ejecutan las soluciones de conector para un evento de **creación** o **actualización** sobre las oportunidades en el centro de Partners o en el lado de CRM, se realiza una llamada API.

2. ¿Qué rol necesita para crear secciones en el entorno de CRM?

Los usuarios que son administradores del sistema o personalizadores del sistema pueden aplicar cambios para todos. Sin embargo, todos los usuarios de la aplicación pueden personalizar el sistema e incluso compartir algunas de sus personalizaciones con otras personas. 

3. ¿Los vendedores de asociados necesitan roles especiales para trabajar en el centro de Partners?
 
A los vendedores asociados se les debe asignar el rol de administrador de referencias. Para obtener más información, consulte la siguiente [información general sobre los permisos] (Create-User-accounts-and-set-permissions).

4. ¿Cuáles son los campos que deben configurarse en primer lugar en el entorno de CRM? 

• Asegúrese de que la moneda sea adecuada para su ubicación y que se encuentra en el entorno de CRM con precisión. • El equipo de ventas debe aparecer en el entorno de CRM como usuarios de CRM.

5.  ¿Cuáles son los requisitos previos necesarios para automatizar la creación de entornos?

Para usar el entorno de automatización de energía, necesita:

- Se necesita una licencia de Power Automatic.
- Se requiere un mínimo de 1 GB de almacenamiento.

6.  ¿Necesita una suscripción a Dynamics 365 para usar la solución de conectores de Salesforce?

La solución de conector de Salesforce es de tipo "flujo de Dynamics" que admite la sincronización con otros sistemas CRM. La solución no requiere que tenga una instancia de Dynamics 365 o una suscripción. Al instalar la solución Salesforce, puede aparecer una lista desplegable con el entorno de CDS existente en la empresa. Debe seleccionar ese entorno. Además, si obtiene el error no encontramos una organización de Dynamics 365 conectada al usuario que inició sesión, deberá crear un nuevo entorno para el conector.

## <a name="questions-and-answers-about-configuration"></a>Preguntas y respuestas acerca de la configuración

1. ¿Qué debe hacer si se plantea el siguiente error al activar los flujos en Power automatization Platform?

Error: no se pudo realizar la solicitud a Azure Resource Manager: "{" error ": {" Code ":" WorkflowTriggerNotFound "," message ":" no se encontró el desencadenador "e14d00f1-1fdf-4b1b-AAAC-54a5064093d3" del flujo de trabajo "manual". "}}". 

Siga estos pasos de solución de problemas:

- Elimine la conexión de CDS y, a continuación, vuelva a crear las conexiones de CDS.
- Activar y desactivar el flujo secundario 
- Elimine la solución y, a continuación, vuelva a instalar la solución. 

2.  ¿Qué debe hacer si se plantea el siguiente error al agregar un conector del centro de Partners en Power automatization Platform?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Mensaje de error que requiere inicio de sesión":::

Siga este paso de solución de problemas:

- Use el inicio de sesión del centro de partners para iniciar sesión en el entorno de Flow (flow.microsoft.com).


3. ¿Qué debe hacer si recibe el siguiente error al activar el flujo del centro de partners a CRM en la plataforma de automatización de energía?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Mensaje de error que requiere actualizaciones":::

Siga estos pasos de solución de problemas:

- Active los dos flujos secundarios siguientes antes de activar el flujo de CRM al centro de Partners.
      - Centro de partners a CRM: Ayudante (versión preliminar de Insider)
      - Centro de Partners: actualizaciones de referencia de venta conjunta de Microsoft a CRM (versión preliminar de Insider)

4. ¿Qué debe hacer si no puede agregar conexiones al flujo al intentar editar el flujo?

Puede agregar conexiones al flujo mientras el flujo se está ejecutando y agregar cada flujo por separado.  Si el cuadro de diálogo para agregar conexiones no se abre automáticamente mientras se edita el flujo, puede editar cada uno de los pasos y subpasos de los flujos para agregar las conexiones.

- Seleccione cada flujo y edítelo de forma individual.
- Expanda todos los pasos del flujo 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Pasos que necesitan conexiones":::

- Seleccione los pasos en los que verá un icono de advertencia pidiéndole asociar conexiones y agregue conexiones. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Editar flujo paso a paso":::


5. ¿Qué debe hacer si los flujos de la solución de conectores de las referencias de venta conjunta no se activan (activar)?

    A. En Power Automate, tendrá que editar los flujos en el siguiente orden y actualizarlos para que usen las conexiones correspondientes:

    - Registro del webhook del centro de Partners (versión preliminar de Insider)
    - Creación de una referencia de venta conjunta: Salesforce al centro de Partners (versión preliminar de Insider)
    - Centro de Partners: actualizaciones de referencia de venta conjunta de Microsoft en Salesforce (versión preliminar de Insider)
    - Centro de partners a Salesforce (versión preliminar de Insider)
    - Salesforce a Partner Center (versión preliminar de Insider)
    - Oportunidad de Salesforce para el centro de Partners (versión preliminar de Insider)
    - Soluciones de Salesforce de Microsoft para el centro de Partners (versión preliminar de Insider)

    B. Para cada flujo, seleccione la opción **ejecutar solo usuarios** . Seleccione **Usar conexión** en lugar de **proporcionados por el usuario de solo ejecución**.  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Para activar un flujo":::

C. Active estos flujos que se indican a continuación:

- Centro de Partners: actualizaciones de referencia de venta conjunta de Microsoft en Salesforce (versión preliminar de Insider)

- Salesforce a Partner Center (versión preliminar de Insider)


D. Active todos los flujos restantes.

E. En el registro del webhook del centro de Partners de Flow, seleccione **Ejecutar**. Proporcione la **dirección URL http** de la primera acción del **centro de Partners al flujo de Salesforce** . Seleccione las cuatro opciones en **eventos para registrarse** y seleccione **sí** para sobrescribir.

## <a name="questions-and-answers-about-runmaintenance"></a>Preguntas y respuestas sobre la ejecución/mantenimiento

1. ¿Cómo se solucionan los problemas en caso de que se produzcan errores durante la ejecución del flujo de energía automatizada?

Para asegurarse de que los flujos de energía automatizada se ejecutan como se espera y para solucionar errores durante la ejecución, consulte [solucionar errores de flujo](/power-automate/fix-flow-failures).

2. ¿Qué debe hacer si ve referencias que no están sincronizadas correctamente en el centro de Partners o en el entorno de CRM?
 
Para determinar el estado de la sincronización de referencias, seleccione **Auditoría**. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Cómo sincronizar referencias":::

Asegúrese de que se cumplen las condiciones siguientes:

- El identificador de la solución se proporciona como parte de la oportunidad.

- Se requiere código de país de dos letras.

- Cuando se selecciona ayuda de Microsoft para la oportunidad, se requiere la información de contacto del cliente.

3. En qué condiciones una referencia no se sincroniza de bidireccional

Asegúrese de lo siguiente:

- Los vendedores asociados deben asegurarse de que tienen habilitada la opción **sincronizar con el centro de Partners** en la sección CRM.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Asegúrese de que ha habilitado la sincronización":::

- Los vendedores deben proporcionar los ingresos y la fecha de cierre al calificar a un cliente potencial.

- Si se proporciona el identificador de CRM en la creación o la actualización de la oportunidad de venta conjunta y si un cliente potencial/oportunidad con ese identificador no se encuentra en CRM, se omitirá la actualización o la creación para esa oportunidad.

- Asegúrese de que el campo de moneda de referencia está configurado en el entorno de Salesforce. 

4. ¿Qué debe hacer si el conector se desconecta y se pierde la sincronización de una referencia. 

A continuación se muestran algunas de las opciones que puede probar:

- Compruebe si el nombre de usuario o la contraseña han expirado para el usuario del centro de Partners con roles de administrador de referencias.

- Puede ir a la oportunidad no sincronizada, realizar una actualización menor y observar si la referencia se ha sincronizado.

- Si los flujos se han ejecutado y han dado error, seleccione el flujo y vuelva a enviar la ejecución que ha producido un error.

5. ¿Qué debe hacer cuando se produce un error de acceso denegado?

Asegúrese de que existen los roles adecuados

- Rol de administrador de referencias para el vendedor del centro de Partners 
 
- Rol de administrador del sistema o del Personalizador del sistema en la instancia de CRM

- Asegúrese de que el usuario de la cuenta de flujo de Power Automate inicia sesión https://flow.microsoft.com al menos una vez de antemano.

6. Si ve que falta el código de país de la **cuenta de cliente** al crear una oportunidad de venta conjunta, ¿qué debe hacer?

Tendrá que agregar el código de país de dos letras ISO a la cuenta de cliente en CRM.

7. ¿Qué debe hacer si ve el error el identificador de la **solución es necesario** al crear una oportunidad de venta conjunta?

Con el fin de crear una referencia de venta conjunta, necesita una solución lista para participar de Microsoft. 

8. ¿Qué debe hacer cuando vea oportunidades de venta conjunta creadas en el centro de partners que no se sincronizan con CRM aunque no se produzcan errores de flujo:

Siga estos pasos:

- Una vez que haya creado un nuevo trato de venta conjunta en el centro de Partners, compruebe si se invoca el flujo del centro de partners a Dynamics 365 (es posible que se invoque varias veces).

- Si se invoca el flujo, compruebe todos los flujos invocados e identifique la ejecución de flujo que actualizaría el CRM. Puede seguir las acciones y comprobar si se ha actualizado el CRM o si se ha producido un problema.

- Consulte *nuevo trato** en el centro de partners para ver si se rellena con el identificador de CRM.

- Asegúrese de que el trato no se cierra accidentalmente como "ganada" o "perdida" en el centro de Partners.

## <a name="next-steps"></a>Pasos siguientes

- [Administrar los clientes potenciales](manage-leads.md)
 
- [Administrar las oportunidades de venta conjunta](manage-co-sell-opportunities.md)