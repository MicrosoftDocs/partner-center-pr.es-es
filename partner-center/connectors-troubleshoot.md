---
title: Solución de problemas de conectores de referencias de venta conjunta
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga respuestas a preguntas comunes sobre el uso de conectores de venta co-sell. Lea estas preguntas más frecuentes sobre cómo solucionar problemas de conectores de venta co-sell.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 49a2b6e5461dacbe87c34b36805a5c240c2e5fd1
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148353"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a>Solución de problemas de conectores de referencias de venta conjunta

**Se aplica a**: Dynamics 365 CRM | Salesforce CRM

**Roles adecuados:** administrador de referencias | Administrador del sistema o personalizador del sistema en CRM

 ## <a name="questions-and-answers-about-pre-requisites"></a>Preguntas y respuestas sobre los requisitos previos

1. ¿Puede usar una solución de conectores de referencia de venta co-venta de prueba para su entorno?

Si se encuentra en el entorno de prueba o ensayo, puede optar por la solución de prueba. La versión de pago de los conectores está disponible en AppSource a 15 USD/mes. Con la conexión de pago, recibirá 10 000 llamadas API al día. Los conectores son contenedores sobre Centro de partners API de referencia. Cada vez que las  soluciones  de conector se ejecutan para un evento de creación o actualización en las oportunidades de Centro de partners o crm, se realiza una llamada API.

2. ¿Qué rol necesita para crear secciones en el entorno crm?

Los usuarios que son administradores del sistema o personalizadores del sistema pueden aplicar cambios para todos los usuarios. Sin embargo, todos los usuarios de la aplicación pueden personalizar el sistema e incluso compartir algunas de sus personalizaciones con otros usuarios. 

3. ¿Los vendedores de asociados necesitan roles especiales para trabajar Centro de partners?
 
Los vendedores de asociados deben tener asignado el rol "Administrador de referencias". Para obtener más información, vea [Información general sobre permisos.](create-user-accounts-and-set-permissions.md)

4. ¿Qué campos se deben configurar primero en el entorno crm? 

• Asegúrese de que la moneda es adecuada para su ubicación y que se encuentra en el entorno de CRM con precisión. • El equipo de ventas debe aparecer en el entorno de CRM como usuarios de CRM.

5. ¿Qué requisitos previos son necesarios para crear Power Automate entorno?

Para usar el Power Automate, necesita:

- Se requiere Power Automate licencia.
- Se requiere un almacenamiento mínimo de 1 GB.

6.  ¿Necesita una suscripción de Dynamics 365 para usar la solución Salesforce Connectors?

La solución Salesforce Connector es de tipo "Dynamics Flow" que admite la sincronización con otros sistemas CRM. La solución no requiere que tenga una instancia de Dynamics 365 o una suscripción. Al instalar la solución salesforce, puede aparecer una lista desplegable con el entorno de CDS existente en su empresa. Debe seleccionar ese entorno. Además, si recibe el error "No se pudo encontrar una organización de Dynamics 365 conectada al usuario que ha iniciado sesión", deberá crear un nuevo entorno para el conector.

## <a name="questions-and-answers-about-configuration"></a>Preguntas y respuestas sobre la configuración

1. ¿Qué debe hacer si se enfrenta al siguiente error al activar flujos en Power Automate Platform?

Error: Error al solicitar Azure Resource Manager error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'. 

Siga estos pasos de solución de problemas:

- Elimine la conexión de CDS y vuelva a crear las conexiones DE CDS.
- Desactivar y activar el flujo secundario 
- Elimine la solución y vuelva a instalarla. 

2.  ¿Qué debe hacer si se encuentra con el error "Iniciar sesión" al agregar un conector Centro de partners en Power Automate Platform?

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Mensaje de error que requiere inicio de sesión":::

Siga este paso de solución de problemas:

- Use sus Centro de partners para iniciar sesión en el entorno de flujo una vez (flow.microsoft.com).


3. ¿Qué debe hacer si recibe el siguiente error al activar el flujo de Centro de partners a CRM en Power Automate Platform?
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Mensaje de error que requiere actualizaciones":::

Siga estos pasos de solución de problemas:

- Active primero los dos flujos secundarios siguientes antes de activar el flujo Centro de partners a CRM.
      - Centro de partners a CRM- Helper (Insider Preview)
      - Centro de partners actualizaciones de referencia de venta co-venta de Microsoft a CRM (versión preliminar de Insider)

4. ¿Qué debe hacer cuando no puede agregar conexiones al flujo al intentar editar el flujo?

Las conexiones se agregan al flujo mientras se ejecuta y se agregan a cada flujo por separado.  Si el cuadro de diálogo para agregar conexiones no se abre automáticamente al editar el flujo, puede editar cada uno de los pasos y sub pasos de los flujos individualmente.

- Seleccione cada flujo y edéelo individualmente.
- Expandir todos los pasos del flujo 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Pasos que necesitan conexiones":::

- Seleccione los pasos en los que verá un icono de advertencia que le pide que asocie conexiones y agregue conexiones. 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Edición del flujo paso a paso":::


5. ¿Qué debe hacer si los flujos de la solución Co-sell Referrals Connectors no se encienden?

A. En Power Automate, deberá editar flujos en el orden siguiente y actualizarlos para usar las conexiones correctas:

- Centro de partners webhook Registration (Insider Preview)
- Creación de una referencia de venta co-venta: Salesforce Centro de partners (versión preliminar de Insider)
- Centro de partners microsoft co-sell Referral Updates to Salesforce (Insider Preview)
- Centro de partners a Salesforce (versión preliminar de Insider)
- Salesforce to Centro de partners (Insider Preview)
- Salesforce Opportunity to Centro de partners (Insider Preview)
- Salesforce Microsoft Solutions to Centro de partners (Insider Preview)

 B. Para cada flujo, seleccione la **opción Ejecutar solo usuarios.** Seleccione **Usar conexión en** lugar de Proporcionado por el usuario de solo **ejecución.**  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Para activar un flujo":::


C. Active estos flujos mencionados a continuación:

 - Centro de partners de referencias de venta co-venta de Microsoft a Salesforce (versión preliminar de Insider)

- Salesforce to Centro de partners (Insider Preview)

    
D. Active todos los flujos restantes.

E. En flow Centro de partners registro de webhook, seleccione **Ejecutar**. Proporcione la **dirección URL http** de la primera acción en Centro de partners flujo de **Salesforce.** Seleccione las cuatro opciones en **Eventos para registrar y** seleccione Sí **en** Sobrescribir.

## <a name="questions-and-answers-about-runmaintenance"></a>Preguntas y respuestas sobre ejecución/mantenimiento

1. ¿Cómo se solucionan los errores durante la Power Automate de flujo?

Para asegurarse de que los flujos de Power Automate se ejecutan según lo previsto y para solucionar los errores durante la ejecución, consulte [Corrección de](/power-automate/fix-flow-failures)errores de flujo .

2. ¿Qué debe hacer si ve referencias que no están sincronizadas correctamente en Centro de partners o crm?
 
Para determinar el estado de la sincronización de referencias, seleccione **Auditar**. 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Sincronización de referencias":::

Asegúrese de que se cumplen las condiciones siguientes:

- El identificador de la solución se proporciona como parte de la oportunidad.

- Se requiere un código de país de dos letras.

- Cuando se selecciona ayuda de Microsoft para la oportunidad, se requiere información de contacto del cliente.

3. ¿Cómo asegurarse de que una referencia se sincronizará bidireccionalmente?

Siga estos pasos:

- Los vendedores asociados deben asegurarse de que han habilitado la opción **Sync with Centro de partners** en la sección CRM.

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Asegúrese de que ha habilitado Synch.":::

- Los vendedores deben proporcionar los ingresos y la fecha de cierre al calificar a un cliente potencial.

- Si el identificador de  CRM  se proporciona en la fase de creación o actualización de la oportunidad de venta en colaboración, pero no se encuentra una oportunidad de cliente potencial con ese identificador en CRM, se omitirá la actualización o la creación.

- Asegúrese de que el campo de moneda de referencia está configurado en el entorno de Salesforce. 

4. ¿Qué debe hacer si el conector se desconecta y se pierde una sincronización de referencias?

Estas son algunas de las opciones que puede probar:

- Compruebe si el nombre de usuario o la contraseña han expirado para Centro de partners usuario con roles de administrador de referencia.

- Puede ir a la oportunidad no sincronizada, realizar una actualización secundaria y observar si la referencia se ha sincronizado.

- Si los flujos se han ejecutado y han dado error, seleccione el flujo y vuelva a enviar la ejecución que ha dado error.

5. ¿Qué debe hacer cuando se producen errores de acceso denegado?

Asegúrese de que existen los roles adecuados.

- Rol administrador de referencias para Centro de partners vendedor 
 
- Rol Administrador del sistema o Personalizador del sistema en la instancia de CRM

- Asegúrese de que el Power Automate usuario de la cuenta de flujo de trabajo inicia sesión al https://flow.microsoft.com menos una vez con antelación.

6. Si ve que falta el **código de país** de la cuenta de cliente al crear una oportunidad de venta en colaboración, ¿qué debe hacer?

Deberá agregar el código de país iso de dos letras a la cuenta de cliente en CRM.

7. ¿Qué debe hacer si ve el error de que el identificador **de solución es necesario** al crear una oportunidad de venta en colaboración?

Para crear una referencia de venta en colaboración, necesita una solución preparada para la venta en colaboración de Microsoft. 

8. ¿Qué debe hacer cuando vea que se crean oportunidades de venta Centro de partners que no están sincronizadas con CRM aunque no haya errores de flujo?

Haga lo siguiente:

- Después de crear una nueva oferta de venta en Centro de partners, compruebe si se invoca Centro de partners al flujo de Dynamics 365 (es posible que se invoque varias veces).

- Si se invoca el flujo, compruebe todos los flujos invocados e identifique la ejecución del flujo que actualizaría el CRM. Puede seguir las acciones y comprobar si ha actualizado crm o ha detectado un problema.

- Active **Nueva oferta** en Centro de partners para ver si se rellena con el identificador de CRM.

- Asegúrese de que la oferta no se cierre accidentalmente como **Ganada** o **Perdida en** Centro de partners.

## <a name="next-steps"></a>Pasos siguientes

- [Administrar los clientes potenciales](manage-leads.md)
 
- [Administrar las oportunidades de venta conjunta](manage-co-sell-opportunities.md)
