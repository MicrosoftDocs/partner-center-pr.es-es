---
title: Transferencia de una suscripción de Azure en un plan de Azure a otro asociado de CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprenda a cambiar el asociado de Proveedor de soluciones en la nube asociado a las suscripciones de Azure de un cliente en un plan de Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: dcacc6da51fe40c7eb05997f5409ef5fadbcf693
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856056"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Transferencia de las suscripciones del plan de Azure de un cliente a otro partner

**Roles adecuados:** administrador de | Agente de ventas | Agente de facturación

En este artículo se describe cómo un cliente puede cambiar sus suscripciones de Azure en un plan de Azure de un Proveedor de soluciones en la nube (CSP) a otro.

Para cambiar las suscripciones de Azure de un cliente de otro asociado, siga estos pasos. Tanto el asociado como el cliente tienen pasos que completar.

>[!Note]  
>Solo los asociados con una relación de facturación directa con Microsoft pueden acceder a las herramientas de transición. Los revendedores indirectos deben trabajar con sus proveedores indirectos para aprovechar esta herramienta de transición.

El cliente debe estar en conversación con ambos asociados (actual y futuro) antes de aprovechar esta herramienta. Es necesario tener una conversación sin conexión para evitar confusiones y abandonos. Además, los partners y clientes deben comprender estas consideraciones y requisitos previos antes de iniciar una transición:

**Consideraciones clave:**

- Azure Reservations no se moverá con la suscripción al asociado futuro
- Los precios de CSP para los servicios de Azure en el asociado actual no realizarán la transición  
- Las responsabilidades de soporte técnico del cliente se trasladarán al asociado futuro
- La facturación y la facturación se moverán al asociado futuro en el momento de la transferencia
- Azure Role-Based Access Control (RBAC) no se ve afectado por la transferencia
- El administrador en nombre de (AOBO) no se concederá de forma predeterminada al asociado futuro
- Los productos de Marketplace de terceros se transferirán siempre y cuando los productos pasen la comprobación de idoneidad de Marketplace.
    - No hay descuentos especiales ni restricciones regionales
    - Los productos no están basados en suscripciones
    - El asociado futuro debe trabajar con el publicador para asegurarse de que están en la lista de permitidos para la implementación del producto.
    - Si no se cumplen todas estas condiciones para transferir los productos de Marketplace, se deben cancelar las suscripciones de Azure y, a continuación, volver a comprar productos de Marketplace con el nuevo asociado.

**Requisitos previos:**

- El cliente interactúa con el asociado de CSP actual en su intención de realizar la transición.
- El futuro asociado de CSP trabaja con el cliente para asegurarse de que se pueden satisfacer las necesidades del cliente.
- El futuro asociado de CSP establece una relación con el cliente y adquiere un plan de Azure antes de que comience la transición.  
- El cliente debe firmar Contrato de cliente de Microsoft asociado de CSP futuro
- El futuro asociado de CSP debe haber firmado el Contrato de asociado de Microsoft para usar esta herramienta.

## <a name="customer-tasks-to-be-completed"></a>Tareas del cliente que se deben completar

Para transferir una suscripción de Azure en un plan de Azure, el cliente debe iniciar el proceso ponerse en contacto con su asociado actual. Deben recopilar el nombre de la compañía y el dominio de su asociado actual para que su asociado futuro pueda completar el formulario de solicitud de transferencia en su nombre.

El cliente también debe identificar las suscripciones que desea transferir desde su asociado actual. No se pueden cambiar los asociados para las suscripciones de Office 365, Enterprise Mobility Suite o Microsoft Dynamics CRM.

>[!Note]  
>Es responsabilidad del asociado futuro completar el formulario de solicitud de transferencia que inicia el proceso de transferencia. Microsoft no puede intervención en nombre del cliente o del asociado actual. El cliente debe planear trabajar estrechamente con su asociado futuro y actual para que la transición se realice sin problemas.

## <a name="future-partner-tasks-to-be-completed"></a>Tareas futuras de asociados que se completarán

El asociado futuro de la suscripción debe completar un formulario de solicitud de transferencia Centro de partners solicitar una transferencia de suscripción:

1.  En el Centro de partners, seleccione **Clientes** y, a continuación, seleccione el cliente del que desea completar un formulario de solicitud de transferencia en nombre de .
2.  En el menú Cliente, seleccione **Suscripciones.**
3.  Seleccione la **sección Solicitud de** transferencia.
4.  En la **sección Solicitud de transferencia,** seleccione **Agregar nueva solicitud.**

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sección Transferencias":::

5.  Complete el **formulario Nueva solicitud de** transferencia.

6.  Seleccione **Send transfer request** Send (Enviar solicitud de  >  **transferencia).**

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formulario de solicitud de transferencia completo":::

7.  Revisión de la confirmación de la solicitud de transferencia

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Revisión de la transferencia pendiente":::

    >[!Note]
    >El asociado futuro puede cancelar la solicitud de transferencia seleccionando **Cancelar** solicitud en la esquina superior derecha solo cuando el estado de la solicitud de transferencia sea "pendiente". Una vez que el estado de la solicitud de transferencia está "en curso" o "completo", las cancelaciones no serán posibles.

## <a name="current-partner-tasks-to-be-completed"></a>Tareas actuales de asociados que se deben completar

El agente de administración del cliente del asociado actual recibirá un correo electrónico en el que el cliente solicita una transferencia de sus suscripciones:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Revisar":::

Revise y acepte el formulario de solicitud de transferencia Centro de partners para completar la transferencia de la suscripción.

>[!Note]  
>Si el asociado actual no hace ninguna acción en un plazo de 30 días, la solicitud expirará y el asociado futuro tendrá una para crear una nueva solicitud de transferencia.

1.  Seleccione **Revisar solicitud de transferencia** desde el correo electrónico O
1.  En el Centro de partners, seleccione **Clientes** y, a continuación, seleccione el cliente del que se ha enviado una solicitud de transferencia en nombre de .
2.  En el menú Cliente, seleccione **Suscripciones.**
3.  Seleccione la **sección Solicitud de** transferencia.
4.  Expanda la información de transferencia seleccionando el identificador de **solicitud de transferencia elegido** en Solicitudes **recibidas.**

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Solicitud de transferencia de revisiones de origen":::

5.  Revise la solicitud de transferencia. Seleccione las suscripciones de Azure solicitadas para transferir.

>[!Note]  
> Antes de continuar, tenga en cuenta que ya no tendrá acceso a las suscripciones seleccionadas.
> No se le facturará por uso adicional.
> Las reservas de Azure no se transfieren con las suscripciones.

6.  A **continuación, seleccione Aceptar y transferir** para completar el proceso de transferencia.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Selección de las suscripciones que se transferirán en los planes de Azure":::

7.  Ver confirmación de aceptación de transferencia.

   En este momento, el asociado futuro, el cliente y el asociado actual recibirán una notificación de la solicitud de transferencia aceptada por correo electrónico.

   Después de que se haya aceptado la transición, el estado de transferencia podría permanecer pendiente durante un máximo de 15 minutos mientras se actualiza el sistema. Si tarda más, el sistema seguirá intentando durante tres días. Si el estado de transferencia sigue siendo Pendiente, el asociado debe enviar una solicitud de servicio.

   Una vez completada la transferencia, las suscripciones incluidas en la solicitud aparecerán en el plan de Azure del asociado futuro y ya no se mostrarán con usted.

>[!Note]  
>Para proveedores indirectos: informe a su revendedor indirecto de que se ha aceptado la solicitud de transferencia.

### <a name="managing-your-transferred-customer-subscriptions"></a>Administración de las suscripciones de cliente transferidas

- El acceso a los usuarios, grupos o entidades de servicio existentes que se asignaron mediante el control de acceso basado en rol de Azure (RBAC) no se ve afectado durante la transición. El control de acceso basado en rol [de Azure (RBAC](/azure/role-based-access-control/overview) de Azure) ayuda al cliente a administrar quién tiene acceso a los recursos de Azure, qué puede hacer con esos recursos y a qué áreas tiene acceso. Como nuevo asociado, no se le proporciona acceso RBAC a los recursos del cliente después de la transferencia de la suscripción. El asociado anterior del cliente conserva su acceso RBAC. Trabaje con el cliente para comprender quién tiene información sobre sus suscripciones y cómo realizar los cambios deseados.

- Por lo tanto, es importante que el cliente quite el acceso RBAC de Azure para su asociado anterior y agregue acceso al nuevo asociado. Para más información sobre el cliente que proporciona nuevo acceso, consulte ¿Qué es el control de acceso basado en [rol de Azure (RBAC de Azure)?](/azure/role-based-access-control/overview) Para obtener más información sobre cómo el cliente quita el acceso RBAC del asociado anterior, consulte [Eliminación de una asignación de roles.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)

- Además, no obtiene automáticamente acceso de administrador en nombre [de (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) a las suscripciones. AOBO es necesario para que los asociados administren las suscripciones de Azure de sus clientes en su nombre. Para más información sobre los privilegios de Azure, consulte [Obtención de permisos para administrar el servicio o](./customers-revoke-admin-privileges.md) la suscripción de un cliente.

## <a name="next-steps"></a>Pasos siguientes:

- [(RBAC de Azure)](/azure/role-based-access-control/overview)
- [Obtenga permisos para administrar el servicio o la suscripción de un cliente.](./customers-revoke-admin-privileges.md)
