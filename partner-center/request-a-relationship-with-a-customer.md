---
title: Solicitar relación con un cliente
ms.topic: how-to
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Solicite una relación con un cliente para escenarios multicanal de varios asociados o si es necesario restaurar los privilegios de administrador delegados para un cliente.
author: dineshvu
ms.author: dineshvu
ms.localizationpriority: medium
ms.openlocfilehash: 55f86e6e48b0b897410826e22564e2d27e25258b
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018142"
---
# <a name="how-to-request-a-reseller-relationship-from-a-customer-in-partner-center"></a>Cómo solicitar una relación de revendedor de un cliente en el Centro de partners

**Roles adecuados**

- Agente de administrador
- Administrador global

Si desea administrar el servicio o la suscripción de un cliente en su nombre, el cliente debe concederle permisos de administrador para ese servicio o suscripción y firmar el Contrato de cliente de Microsoft.

Si desea establecer una relación de revendedor con un cliente y administrar solo las suscripciones de Azure que aprovisiona, no es necesario obtener permisos de administrador.

>[!NOTE] 
>La opción de no solicitar permisos no está disponible para los asociados que operan en Microsoft Cloud for US Government o Microsoft Cloud Germany. Para más información, consulte Clientes que [delegan privilegios de administración en asociados.](customers-revoke-admin-privileges.md)

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Invitar a un cliente a establecer una relación de revendedor contigo

Puede solicitar una relación de revendedor con un cliente desde su país o su misma región.

1. Selecciona **Clientes** en el menú **Centro de partners** y, a continuación, selecciona **Solicitar una relación de revendedor**.

2. Para solicitar permisos de administrador a este cliente, seleccione Incluir privilegios de administración **delegados para Azure Active Directory y Office 365.** Para establecer la relación sin solicitar permisos de administrador, desactive esta opción.

3. En la página siguiente, revise el borrador del mensaje de correo electrónico. Puede abrir el borrador del mensaje en la aplicación de correo electrónico predeterminada o puede copiar el mensaje en el portapapeles y pegarlo en un correo electrónico.

   Puedes editar el texto en el correo electrónico, pero asegúrate de incluir el vínculo, ya que se trata de un vínculo personalizado que conecta al cliente directamente con tu cuenta. Selecciona **Listo** cuando hayas completado este paso.

4. Envía el correo electrónico a tu cliente.

5. Una vez que el cliente acepte la  invitación, aparecerá en la página Clientes y podrá aprovisionar y administrar el servicio para el cliente desde allí.

   > [!NOTE]
   > Si el cliente aún no ha aceptado el Contrato de cliente de Microsoft, se le pedirá que lo haga cuando acepte la invitación. El cliente debe ser administrador global para aceptar la invitación.

6. Para administrar la cuenta, los servicios, los usuarios y las licencias del cliente, expande el registro del cliente seleccionando la flecha abajo situada junto a su nombre.

> [!IMPORTANT]  
> Los clientes pueden reasignar o quitar permisos de administrador en el portal de administración del servicio. Sin embargo, a menos que y hasta que renegocie su contrato con el cliente, seguirá siendo responsable de proporcionar soporte técnico al cliente y de cumplir los términos del Contrato microsoft partner, incluso después de que un cliente reasigna o quita los permisos de administrador. En esta situación, si el cliente requiere ayuda, puede llamar al soporte técnico de Microsoft para abrir una solicitud de servicio en nombre del cliente.

## <a name="changes-to-the-customer-invitation-experience"></a>Cambios en la experiencia de invitación del cliente

La experiencia del cliente para aceptar una invitación de relación de revendedor de un Proveedor de soluciones en la nube asociado se hospeda en diferentes portales orientados al cliente. La ubicación del portal depende de si un cliente está en una nube pública de Microsoft o en una nube nacional:

|Tipos de clientes en la nube  | ¿Dónde acepta un cliente una invitación de relación de revendedor? |
|---------|---------
| Clientes en la nube pública | Centro de administración de Microsoft 365 |
| Clientes de Centro de partners para Microsoft Cloud Alemania | Microsoft Office portal de administración |
| Clientes de Centro de partners para Microsoft Cloud for US Government | Microsoft Office portal de administración |
|

## <a name="next-steps"></a>Pasos siguientes

- [Asignar contactos de soporte técnico](assign-support-contacts.md)

- [Eliminación de una relación con un cliente](remove-a-relationship.md)
