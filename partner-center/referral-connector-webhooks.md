---
title: Uso de webhooks para obtener eventos de cambio de recursos
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use las API del webhook del centro de partners para saber cuándo se producen cambios en los recursos de las referencias en Dynamics 365 CRM o en CRM de Salesforce.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: referencias, API de webhook, eventos de cambio de recursos
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 43874556b5f3fd355f5c315bf06ca7daee0a699e
ms.sourcegitcommit: 7abdd277c0eea51237c97cbb163a4943fd740356
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/06/2020
ms.locfileid: "84467475"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events-for-dynamics-365-crm-and-salesforce-crm"></a>Uso de las API de webhook para registrar eventos de cambio de recursos para Dynamics 365 CRM y el CRM de Salesforce

### <a name="appropriate-roles"></a>Roles adecuados

- Administrador de referencias
- Administrador del sistema o Personalizador del sistema para Dynamics 365 CRM o CRM de Salesforce

Las API del webhook del centro de Partners le permiten registrarse para los eventos de cambio de recursos. Estos eventos de cambio se envían a la dirección URL como publicaciones HTTP.

>[!NOTE]
>En este tema se explican las API de webhook para Dynamics 365 CRM y el CRM de Salesforce.

## <a name="configure-the-webhook"></a>Configuración del webhook

1. Para registrar la dirección URL, seleccione **registro de webhook del centro de Partners (versión preliminar de Insider)** flujo de automatización.

2. Agregar conexiones para () Usuario del centro de Partners con credenciales de administrador de referencias (b.) Eventos del centro de Partners, tal y como se resalta

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Desencadenador":::

3. Cuando realice estas actualizaciones, verá

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. Guarde los cambios y seleccione **Activar**.

   Para permitir que los webhooks del centro de Partners escuchen los cambios de eventos en los objetos de coexistencia o de referencia independiente IP en el centro de Partners y en los sistemas CRM, realice los pasos siguientes:

5. Seleccione **centro de partners para Dynamics 365 (versión preliminar de Insider)** o **centro de partners a Salesforce (versión preliminar de Insider)**.

6. Seleccione el icono de **edición** y seleccione **cuando se reciba una solicitud HTTP**.

7. Seleccione el icono de **copiar** para copiar la dirección URL http post proporcionada.

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copiar la dirección URL":::

8. Ahora, seleccione "registro de webhook del centro de Partners (versión preliminar de Insider)" flujo automático de energía y seleccione **Ejecutar**.

9. Asegúrese de que se abre la ventana "flujo de ejecución" en el panel derecho y haga clic en **continuar**.

10. Escriba la siguiente información:

    1. **Punto de conexión de desencadenador http**: dirección URL copiada del paso anterior

    2. **Eventos para registrar**: "referencia creada" y "referencia-actualizada"

    3. **Sobrescribir puntos de conexión de desencadenador existentes si están presentes**: sí (esto Sobrescribe todos los extremos existentes).

    El webhook ahora puede escuchar cambios (crear y actualizar eventos).

11. Seleccione **Ejecutar** y, a continuación, haga clic en **listo.**

## <a name="customize-synchronization-steps"></a>Personalizar pasos de sincronización

Cuando se sincronizan las referencias de venta conjunta entre el centro de Partners y el sistema CRM, los campos que se sincronizan en el equipo del centro de Partners se enumeran aquí.

A menudo, los sistemas CRM son muy personalizados. Puede personalizar los flujos de automatización. Siga la guía de asignación de campos y, si es necesario, realice los cambios adecuados en los pasos de la potencia que automatiza los flujos.  Se proporcionan asignaciones del centro de Partners de Microsoft a CRM, pero en función de su entorno de CRM, puede optar por personalizar aún más los campos.

Se pueden personalizar varios pasos de cada uno de los flujos de potencia automatizados en función de sus necesidades. Estos son algunos ejemplos de las personalizaciones disponibles:

1. Para personalizar los campos de los eventos de creación o actualización en el centro de partners para la sincronización de referencias de CRM:

   1. Seleccione centro de partners para Dynamics 365 (versión preliminar de Insider) o centro de partners a Salesforce (versión preliminar de Insider).

   2. Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.

   3. Seleccione **(ámbito) sincronizar el cliente potencial o la oportunidad**.

2. Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para crear eventos, seleccione si se trata de una **nueva oportunidad compartida y, a continuación**, haga clic en. Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda **crear una nueva oportunidad en CRM**. Puede editar las asignaciones en esta sección mediante la guía de asignación de campos.

   1. Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para los eventos de actualización, haga clic en el paso "(ámbito) sincronizar el cliente potencial o la oportunidad".

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

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a>Sincronización de referencia de venta conjunta bidireccional de un extremo a otro

Una vez que haya instalado, configurado y personalizado la solución Power Automate, puede probar la sincronización de referencias de venta conjunta entre Dynamics 365 o Salesforce y Partner Center.

### <a name="pre-requisites"></a>Requisitos previos

Para sincronizar las referencias entre el centro de Partners y Dynamics 365 CRM o entre el centro de Partners y el CRM de Salesforce, la solución Power Automate debe delimitar claramente los campos de referencia específicos de Microsoft. Esto proporciona a los equipos de los vendedores la capacidad de decidir qué referencias desean compartir con Microsoft para la venta conjunta.

Un conjunto de campos personalizados está disponible como parte de la sincronización de referencias del centro de partners para la entidad de la **oportunidad** de la solución Dynamics 365. Un usuario administrador de CRM tendrá que crear una sección de CRM independiente con los campos personalizados de la **oportunidad** .

Los siguientes campos personalizados deben formar parte de la sección CRM:

- **Sincronizar con el centro de Partners**: si se va a sincronizar la oportunidad con el centro de Partners de Microsoft

- **Identificador de referencia**: un campo de identificador de solo lectura para la referencia del centro de Partners de Microsoft

- **Vínculo de referencia**: un vínculo de solo lectura a la referencia en el centro de Partners de Microsoft

- **¿Cómo puede ayudarle Microsoft?**: ayuda necesaria de Microsoft para la referencia

- **Productos**: lista de productos asociados a esta oportunidad

- **Audit**: una pista de auditoría de solo lectura para la sincronización con las referencias del centro de Partners

### <a name="scenarios"></a>SITUACIÓN

1. Sincronización de referencia cuando se crea o actualiza una referencia en CRM y se sincroniza en el centro de Partners:

   1. Inicie sesión en el entorno de CRM de Dynamics 365 con un usuario que tenga visibilidad en la sección de **oportunidades** de CRM.

   2. Asegúrese de que la siguiente sección está presente al crear una "nueva oportunidad" en el entorno de Dynamics 365

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Oportunidad":::

   3. Para sincronizar esta oportunidad con el centro de Partners de Microsoft, asegúrese de establecer los siguientes campos en la vista tarjeta:

      - **Sincronizar con el centro de Partners**: sí

      - **¿Cómo puede ayudarle Microsoft?**: Seleccione una de las siguientes opciones:

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Selecciones de la ayuda":::

      - **Productos**: identificadores de la solución del producto

   4. Una vez creada la oportunidad en Dynamics 365 con la opción **sincronizar con el centro de Partners** establecida en **sí**, espere 10 minutos, inicie sesión en su cuenta del centro de Partners. Las referencias se sincronizarán con Dynamics 365.

   5. Por lo tanto, para una oportunidad que tuviera la opción "sincronizar con el centro de Partners" establecida en "sí", si actualizas la oportunidad en Dynamics 365 CRM, los cambios se sincronizarán en la cuenta del centro de Partners.

   6. Las oportunidades que se sincronizan correctamente con el centro de Partners se identificarán con ✔ icono en Dynamics 365.

2. Sincronización de referencia cuando se crea o actualiza una referencia en el centro de Partners de Microsoft y se sincroniza en el entorno de Dynamics 365:

   1. Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard/home)del centro de Partners.

   2. Seleccione **referencias** en el menú de la izquierda.

   3. Cree una nueva referencia de venta conjunta desde el centro de partners; para ello, haga clic en la opción "nuevo trato".

   4. Inicie sesión en el entorno de CRM de Dynamics 365.

   5. Vaya a **abrir oportunidades**. La referencia creada en el centro de Partners de Microsoft ya está sincronizada en Dynamics 365 CRM.

   6. Al seleccionar una referencia sincronizada, se rellenan los detalles de la vista de tarjeta.

## <a name="next-steps"></a>Pasos siguientes

- [¿Más información sobre la plataforma Microsoft Power Automate?](https://docs.microsoft.com/power-automate/)

- [Eventos del webhook del centro de Partners](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [Administrar los clientes potenciales](manage-leads.md)

- [Administrar las oportunidades de venta conjunta](manage-co-sell-opportunities.md)
