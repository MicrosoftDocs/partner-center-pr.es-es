---
title: Notificar problemas en nombre de un cliente
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información acerca de cómo remitir un problema de servicio al cliente a Microsoft y cómo archivar una incidencia de soporte técnico para diferentes tipos de servicios de Microsoft.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 12310b8c89f593122cdd9caec0aa74a712953219
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175080"
---
# <a name="report-a-service-problem-on-behalf-of-a-customer---including-when-and-how-to-do-so"></a>Notificar un problema del servicio en nombre de un cliente, lo que incluye Cuándo y cómo hacerlo

**Se aplica a**

- Centro de partners
- Centro de partners para Microsoft Cloud for US Government

**Roles adecuados**

- Proveedor indirecto

Si el cliente tiene un problema de servicio que no puede resolver y cumple los criterios descritos en el nivel de [problemas de escalado a Microsoft](escalate-problems-to-microsoft.md), el proveedor indirecto puede presentar una incidencia de soporte técnico para ellos. Este proceso también es útil para escalar los problemas o conflictos de facturación y cuestiones de fraude.

## <a name="submit-a-service-request-for-a-customer"></a>Enviar una solicitud de servicio para un cliente

1. Desde el menú del **Centro de partners**, selecciona **Solicitudes de servicio** y, después, **Solicitud de cliente**. 

2. En la página de solicitudes de cliente, busca el cliente que quieras.

3. En el menú desplegable **Nueva solicitud**, selecciona **Azure** u **Office 365, Dynamics 365, Enterprise Mobility Suite**. Se le redirigirá al Microsoft Azure Portal o al centro de administración de Office 365.

>[!NOTE]
>Las operaciones de soporte técnico asociados que transaccionan Dynamics 365 en CSP son necesarias para mantener un contrato de soporte técnico de soporte técnico avanzado para el plan de asociados (ASfP) o superior. Este contrato de soporte técnico es necesario para enviar incidentes de Dynamics 365 en nombre de un cliente de CSP. [Obtenga más información](https://partner.microsoft.com/support/partnersupport) sobre las opciones del contrato de soporte técnico.

### <a name="microsoft-azure"></a>Microsoft Azure

> [!IMPORTANT]
> Cuando necesites crear una solicitud de servicio para tu cliente en Azure, ten en cuenta que:
>
>- Para que usted, como revendedor indirecto, cree solicitudes de servicio para su cliente en Azure, el proveedor indirecto debe concederle acceso a la cuenta de Azure del cliente. Esto es diferente de la administración en nombre de los clientes de Office 365.
>
>- Aunque el administrador del departamento de soporte técnico del Centro de partners no puede crear solicitudes de servicio en el portal de servicios de Azure, lo que sí que puede hacer es crear un grupo de soporte técnico en el portal de servicios de Azure y conceder a ese grupo permisos para registrar solicitudes de soporte técnico.

1. Seleccione **Nueva solicitud de soporte técnico**.

2. Rellena la solicitud de soporte técnico con la información adecuada y, después, selecciona **Crear**:

   - En la sección **Conceptos básicos** de la solicitud de soporte técnico, asegúrate de seleccionar **Proveedor de soluciones en la nube** en el campo **Plan de soporte técnico**.

   - En la sección **Información de contacto** de la solicitud de soporte técnico, escribe tu información, no la del cliente.

3. A continuación, revise las solicitudes de servicio del cliente en Microsoft Azure Portal; para ello, seleccione **Administrar solicitudes de soporte técnico**.

Es posible que tenga que crear una solicitud de soporte técnico para un cliente si no tiene permisos de administrador para ese cliente. Esto podría pasar en uno de los siguientes casos:

- No solicitó privilegios de administrador la primera vez que estableció la relación.
- Solo se administran las suscripciones de Azure de un cliente, por lo que no tiene permisos administrativos.
 
En cualquiera de estos casos, puedes usar el procedimiento siguiente para crear una solicitud de soporte técnico. 

1. Copie el nombre de dominio del cliente desde la página de su cuenta en el centro de Partners.

2. Ve a https://portal.azure.com/[customerdomainname]. 

3. Selecciona la suscripción de Azure que requiere soporte técnico.

4. Selecciona **Nueva solicitud de soporte** y, a continuación, sigue las indicaciones para crear la solicitud. 

 
### <a name="office-365-microsoft-dynamics-crm-online-enterprise-mobility-suite"></a>Office 365, Microsoft Dynamics CRM Online, Enterprise Mobility Suite

1. En la sección **crear una solicitud de servicio** , elija la categoría de soporte técnico adecuada. Es posible que deba seleccionar **más...** para ver artículos adicionales.

2. Complete el formulario de solicitud de servicio y seleccione **submit (enviar**).

   > [!TIP]
   > Asegúrate de incluir tu información de contacto, no la del cliente.

3. Después, revise las solicitudes de servicio del cliente. para ello, vaya al centro de administración de Office 365 y seleccione **ver todas las incidencias de soporte técnico**.

### <a name="support-for-commercial-marketplace-products"></a>Compatibilidad con productos de Marketplace comercial

Microsoft no proporciona soporte técnico para productos comerciales de Marketplace. Deberá ponerse en contacto con el fabricante de software independiente (ISV) que publicó el producto para obtener soporte técnico.

Para buscar la información de contacto del ISV:

1.  En la página **Marketplace**, selecciona el producto para el que necesitas ayuda.

2.  En la página del producto, encontrará información de contacto de soporte técnico. Puede ser una o varias de las opciones siguientes:

    - Un vínculo a un punto de entrada de soporte en el sitio web del ISV
    - Un correo electrónico de soporte técnico
    - Un número de teléfono de contacto de soporte técnico

## <a name="faq"></a>Preguntas más frecuentes

Consulte a continuación las preguntas más frecuentes sobre las solicitudes de servicio que puede enviar en nombre de un cliente. 

### <a name="what-is-included-as-part-of-the-support-entitlement"></a>¿Qué se incluye como parte de los derechos de soporte técnico?

Las solicitudes de servicio deben archivarse a través del centro de Partners. Están disponibles para Azure, Microsoft Office 365, Microsoft Dynamics CRM Online y Enterprise Mobility Suite. Como partner que participa en el programa Proveedor de soluciones en la nube, puedes esperar un tiempo de respuesta prioritario para tus problemas más importantes.

La compatibilidad con su propio inquilino de socio no se incluye como parte de la ventaja de soporte técnico de CSP. Sin embargo, Office 365, Microsoft Dynamics CRM Online y Enterprise Mobility Suite no cobran una cuota de suscripción de soporte independiente para asociados o clientes. Azure cobra una cuota, pero si tiene derecho a la firma del soporte técnico de la nube u otras ventajas de Microsoft Partner Network (MPN), puede usarlas para pagar esa cuota.

Esta ventaja se aplica a todos los partners que participan en el programa Proveedor de soluciones en la nube, ya sea de pago o en un período de prueba. El soporte técnico de administración de suscripciones y facturación también se incluye como componente gratuito de este paquete.

### <a name="how-quickly-will-i-get-an-initial-response"></a>¿En cuánto tiempo recibiré una respuesta inicial?

Los tiempos de respuesta inicial dependen de la gravedad del incidente enviado. La gravedad de un problema viene determinada por tu indicación del impacto empresarial cuando envías una solicitud de servicio.

Tiempos de respuesta iniciales de los **incidentes técnicos-corrección**:

- Impacto crítico (gravedad A): 2 horas (degradación o pérdida considerable de los servicios. Servicios de producción inactivos).
- Impacto moderado (gravedad B): cuatro horas (pérdida o degradación moderada de los servicios. Servicios de producción afectados parcialmente).
- Impacto mínimo (gravedad C): ocho horas (pérdida o degradación mínima de servicios). Servicios todavía disponibles o servicios que no son de producción afectados).

Los tiempos de respuesta inicial son solo para soporte técnico en inglés. Se proporciona soporte técnico en el idioma local durante las horas laborables.
En el caso de los incidentes que se encuentran dentro de los límites del derecho de soporte técnico, pero no se consideran incidentes de interrupción de la corrección, el tiempo de respuesta inicial puede ser de hasta un día laborable.

### <a name="can-i-submit-a-service-request-by-phone"></a>¿Puedo enviar una solicitud de servicio por teléfono?

No, no se ofrece soporte telefónico para este programa.

### <a name="what-happens-if-i-sign-into-the-azure-portal-and-bypass-partner-center"></a>¿Qué sucede si inicio sesión en el portal de Azure y omito el Centro de partners?

Si inicia sesión directamente en el Microsoft Azure Portal, está viendo el centro en su propio contexto, no en el contexto de un cliente. Esta es la razón por la que solo debe iniciar sesión directamente en el Microsoft Azure Portal al crear una solicitud de servicio para sus propias suscripciones.

El derecho de soporte técnico del programa CSP no proporciona soporte técnico en su propia suscripción de socio. Por este motivo, debe proporcionar el derecho a un plan de soporte técnico válido al crear una solicitud de servicio que se refiere a su suscripción de socio comercial. Algunos ejemplos son el identificador de contrato de MPN, Premier o un plan de soporte técnico de Azure. Para obtener más información, consulte las [preguntas más frecuentes sobre el soporte técnico de Azure](https://go.microsoft.com/fwlink/?LinkId=717532).

### <a name="what-happens-if-i-sign-into-the-office-365-admin-center-portal-and-bypass-partner-center"></a>¿Qué ocurre si inicio sesión en el portal del centro de administración de Office 365 y omite el centro de Partners?

Si inicia sesión directamente en el centro de administración de Office 365, está viendo el centro en su propio contexto, no en el contexto de un cliente. Por eso solo debe iniciar sesión directamente en el centro de administración de Office 365 al crear una solicitud de servicio para sus propias suscripciones.

### <a name="how-do-i-get-additional-dynamics-365-support"></a>¿Cómo puedo obtener soporte adicional de Dynamics 365?

Si tiene problemas relacionados con: las suscripciones a Dynamics 365 plan, las licencias, la facturación, las operaciones de finanzas &, las licencias de producto de Dynamics 365 o necesita soporte técnico adicional:
 
Ponte en contacto con el [Soporte técnico de Dynamics](/dynamics365/customer-engagement/admin/contact-technical-support)

Lee [Soporte técnico de Microsoft Dynamics](https://support.microsoft.com/help/4052881/faq-microsoft-dynamics-365-for-unified-operations-iur)

## <a name="next-steps"></a>Pasos siguientes

- [Proporcionar soporte técnico a tus clientes](customer-support.md)
- [Comprobar el estado del servicio](check-service-health.md)