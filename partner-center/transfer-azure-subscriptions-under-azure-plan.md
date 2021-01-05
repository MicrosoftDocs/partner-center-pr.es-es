---
title: Transferencia de una suscripción de Azure a un plan de Azure a otro asociado de CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo cambiar el asociado del programa proveedor de soluciones en la nube asociado a las suscripciones de Azure de un cliente en un plan de Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: e792e4af2999924ba8be77ec0517ce56c1db7a27
ms.sourcegitcommit: ed5c873d19f0464cc986fe6e852383cd4280daf6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/05/2021
ms.locfileid: "97893213"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>Transfiera las suscripciones del plan de Azure de un cliente a un asociado diferente

**Roles adecuados**

- Partners del programa Proveedor de soluciones en la nube (CSP)

En este artículo se describe cómo un cliente puede cambiar sus suscripciones de Azure en un plan de Azure de un proveedor de soluciones en la nube (CSP) a otro.

Para cambiar las suscripciones de Azure de un cliente de un asociado diferente, siga estos pasos. Tanto el socio como el cliente tienen que completar los pasos.

>[!Note]  
>Solo los asociados con una relación de facturación directa con Microsoft pueden acceder a las herramientas de transición. Los revendedores indirectos deben trabajar con sus proveedores indirectos para aprovechar esta herramienta de transición.

El cliente debe estar en conversación con ambos asociados (actuales y futuros) antes de que se aproveche esta herramienta. Es necesario tener una conversación sin conexión para evitar la confusión y la renovación. Además, los asociados y los clientes deben comprender estas consideraciones y requisitos previos antes de iniciar una transición:

**Consideraciones clave:**

- Azure Reservations no se moverá con la suscripción a un socio comercial futuro
- Los precios de CSP para los servicios de Azure en el socio actual no se transfieren  
- Las responsabilidades de soporte técnico del cliente se trasladarán al asociado futuro
- La facturación y la facturación se trasladarán al asociado futuro en el momento de la transferencia
- El Access Control de Role-Based de Azure (RBAC) no se ve afectado por la transferencia
- El administrador en nombre de (AOBO) no se concederá de forma predeterminada al socio comercial futuro
- Los productos de Marketplace de terceros se transferirán siempre que los productos superen la comprobación de elegibilidad del Marketplace.
    - No hay descuentos especiales ni restricciones regionales
    - Los productos no están basados en la suscripción
    - El asociado futuro debe trabajar con el publicador para asegurarse de que se encuentran en la lista de permitidos para la implementación del producto.
    - Si no se cumplen todas estas condiciones para transferir los productos de Marketplace, se deben cancelar las suscripciones de Azure y, después, volver a comprar los productos de Marketplace con el nuevo socio comercial.

**Requisitos previos:**

- El cliente contrata al asociado de CSP actual en su intención de transición
- El asociado de CSP futuro funciona con el cliente para garantizar que se puedan satisfacer las necesidades del cliente
- El asociado de CSP futuro establece una relación con el cliente y compra un plan de Azure antes de comenzar la transición  
- El cliente debe firmar el acuerdo de cliente de Microsoft con el asociado de CSP futuro
- El asociado de CSP futuro debe haber firmado el acuerdo de asociado de Microsoft para usar esta herramienta

## <a name="customer-tasks-to-be-completed"></a>Tareas del cliente que se van a completar

Para transferir una suscripción de Azure en un plan de Azure, el cliente debe iniciar el proceso poniéndose en contacto con su asociado actual. Deben recopilar el dominio y el nombre de la empresa de su socio actual para que su asociado futuro pueda completar el formulario de solicitud de transferencia en su nombre.

El cliente también debe identificar las suscripciones que desean transferir desde su socio actual. No se pueden cambiar los asociados de las suscripciones a Office 365, Enterprise Mobility Suite o Microsoft Dynamics CRM.

>[!Note]  
>Es responsabilidad del asociado futuro completar el formulario de solicitud de transferencia que inicia el proceso de transferencia. Microsoft no puede intervenir en nombre del cliente o del socio actual. El cliente debe planear trabajar en estrecha colaboración con sus asociados futuros y actuales para que la transición se lleve a cabo sin problemas.

## <a name="future-partner-tasks-to-be-completed"></a>Futuras tareas de asociados que se van a completar

El socio comercial de la suscripción debe completar un formulario de solicitud de transferencia desde el centro de partners para solicitar una transferencia de suscripción:

1.  En el menú del centro de Partners, seleccione **clientes** y, a continuación, seleccione el cliente en nombre del que desea completar un formulario de solicitud de transferencia.
2.  En el menú del cliente, seleccione **suscripciones**.
3.  Seleccione la sección **solicitud de transferencia** .
4.  En la **sección solicitud de transferencia**, seleccione **Agregar nueva solicitud**.

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sección transferencias":::

5.  Complete el formulario **nueva solicitud de transferencia** .

6.  Seleccione **Enviar solicitud de transferencia** de  >  **envío**.

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formulario completar solicitud de transferencia":::

7.  Revisar confirmación de solicitud de transferencia

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Revisión de la transferencia pendiente":::

    >[!Note]
    >El asociado futuro puede cancelar la solicitud de transferencia seleccionando **Cancelar solicitud** en la esquina superior derecha solo cuando el estado de la solicitud de transferencia es "pendiente". Una vez que el estado de la solicitud de transferencia es "en curso" o "completo", no se podrán realizar las cancelaciones.

## <a name="current-partner-tasks-to-be-completed"></a>Tareas de asociados actuales para completar

El agente de administración del asociado actual del cliente recibirá un correo electrónico que solicitará a su cliente una transferencia de sus suscripciones:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Revisar":::

Revise y acepte el formulario de solicitud de transferencia del centro de partners para completar la transferencia de la suscripción.

>[!Note]  
>Si el asociado actual no realiza ninguna acción en un plazo de 30 días, la solicitud expirará y el asociado futuro tendrá un para crear una nueva solicitud de transferencia.

1.  Seleccione **revisar solicitud de transferencia** desde el correo electrónico o
1.  En el menú del centro de Partners, seleccione **clientes** y, a continuación, seleccione el cliente al que se ha enviado una solicitud de transferencia en nombre de.
2.  En el menú del cliente, seleccione **suscripciones**.
3.  Seleccione la sección **solicitud de transferencia** .
4.  Expanda transferir información seleccionando el **identificador de solicitud de transferencia** elegido en **solicitudes recibidas** .

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Solicitud de transferencia de revisiones de origen":::

5.  Revise la solicitud de transferencia. Seleccione las suscripciones de Azure solicitadas que se van a transferir.

>[!Note]  
> Antes de continuar, tenga en cuenta que ya no tendrá acceso a las suscripciones seleccionadas.
> No se le facturará para su uso adicional.
> Las reservas de Azure no se transfieren con las suscripciones.

6.  A continuación, seleccione **Aceptar y transferir** para completar el proceso de transferencia.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Seleccione las suscripciones que se van a transferir en sus planes de Azure":::

7.  Permite ver la confirmación de aceptación de transferencia.

   En este momento, el socio comercial, el cliente y el socio actual recibirán una notificación de la solicitud de transferencia aceptada por correo electrónico.

   Después de, se ha aceptado la transición el estado de la transferencia podría permanecer pendiente hasta 15 minutos mientras se actualiza el sistema. Si tarda más, el sistema seguirá intentando tres días. Si el estado de la transferencia sigue siendo pendiente, el asociado debe enviar una solicitud de servicio.

   Una vez completada la transferencia, las suscripciones incluidas en la solicitud aparecerán en el plan de Azure del asociado futuro y ya no aparecerán en la lista.

>[!Note]  
>Para los proveedores indirectos: informe a su revendedor indirecto de que se ha aceptado la solicitud de transferencia.

### <a name="managing-your-transferred-customer-subscriptions"></a>Administración de las suscripciones de clientes transferidas
- El acceso a los usuarios, grupos o entidades de servicio existentes que se asignaron mediante el control de acceso basado en rol de Azure (RBAC) no se ve afectado durante la transición. El control de acceso basado en roles [(RBAC de Azure)](/azure/role-based-access-control/overview) de Azure ayuda a su cliente a administrar quién tiene acceso a los recursos de Azure, lo que puede hacer con esos recursos y a qué áreas tienen acceso. Como el nuevo asociado, no se le concede ningún acceso RBAC a los recursos de su cliente después de la transferencia de la suscripción. El socio anterior del cliente conserva su acceso RBAC. Trabaje con su cliente para conocer quién tiene conocimiento de sus suscripciones y cómo realizar los cambios deseados.

- Por lo tanto, es importante que el cliente Quite el acceso RBAC de Azure para su asociado anterior y agregue acceso para el nuevo socio. Para más información sobre el cliente que otorga nuevo acceso, consulte [¿Qué es el control de acceso basado en roles de Azure (RBAC de Azure)?](/azure/role-based-access-control/overview) Para obtener más información sobre el cliente que quita el acceso RBAC del asociado anterior, consulte [quitar una asignación de roles](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).

- Además, no obtiene automáticamente acceso [de administrador en nombre de (Aobo)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) a las suscripciones. AOBO es necesario para que los asociados administren las suscripciones de Azure de su cliente en su nombre. Para obtener más información sobre los privilegios de Azure, consulte [obtención de permisos para administrar el servicio o la suscripción de un cliente.](./customers-revoke-admin-privileges.md)

## <a name="next-steps"></a>Pasos siguientes:

- [(RBAC de Azure)](/azure/role-based-access-control/overview)
- [Obtener permisos para administrar el servicio o la suscripción de un cliente.](./customers-revoke-admin-privileges.md)
