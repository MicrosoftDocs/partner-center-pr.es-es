---
title: Obtención de privilegios de administrador para un cliente
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtén los permisos que necesitas para administrar el servicio o la suscripción de un cliente en su nombre. Obtén información acerca de cómo se conceden, revocan y administran los permisos.
author: LauraBrenner
ms.author: labrenne
ms.custom: SEOAPR.20
keywords: privilegios de administrador delegado, administración en nombre de, quitar privilegios, DAP, AOBO
ms.localizationpriority: high
ms.openlocfilehash: dc56aa2236251c98afa6ffc5b5cc2b3d3f10918b
ms.sourcegitcommit: 093039319fab2a44ab147159bc4be832f1330d57
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/14/2020
ms.locfileid: "83394177"
---
# <a name="obtain-permissions-to-manage-a-customers-service-or-subscription"></a>Obtención de permisos para administrar el servicio o la suscripción de un cliente

**Se aplica a**

- Centro de partners

**Roles adecuados**

- Agente de administrador
- Agente de ventas

Para administrar la suscripción o el servicio de un cliente en su nombre, el cliente debe conceder permisos de administrador para dicho servicio. Para obtener los permisos de administrador de un cliente, envíale un correo electrónico con una solicitud de relación de revendedor. Cuando el cliente apruebe la solicitud, podrás iniciar sesión en el portal de administración del servicio y administrar el servicio en nombre del cliente. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Invitar a un cliente a establecer una relación de revendedor contigo

1.  Selecciona **Clientes** y, a continuación, selecciona **Solicitar una relación de revendedor**.

2.  En la siguiente página, revisa el borrador del mensaje de correo electrónico. Puedes abrir el borrador de mensaje de correo electrónico en la aplicación de mensajería predeterminada o puedes copiar el mensaje en el portapapeles y pegarlo en un correo electrónico. 

    >[!IMPORTANT]
    >Puedes editar el texto en el correo electrónico, pero asegúrate de incluir el vínculo, ya que se trata de un vínculo personalizado que conecta al cliente directamente con tu cuenta. 
    
3.  Selecciona **Listo** cuando hayas completado este paso.

4.  Envía el correo electrónico a tu cliente.

5.  Una vez que el cliente acepte tu invitación, aparecerá en la página **Clientes** y, podrás aprovisionar y administrar el servicio para el cliente desde allí.

6.  Para administrar la cuenta, los servicios, los usuarios y las licencias del cliente, expande el registro del cliente seleccionando la flecha abajo situada junto a su nombre y luego selecciona el portal de administración para el servicio que quieres administrar.

>[!IMPORTANT]  
>Los clientes pueden reasignar o quitar permisos de administrador en el portal de administración del servicio. Sin embargo, a no ser que hayas renegociado tu acuerdo con el cliente, continúas siendo el responsable de proporcionar soporte técnico al cliente y de cumplir con las condiciones del contrato de revendedor en la nube, incluso después de que el cliente reasigne o elimine los permisos de administrador. En esta situación, si el cliente necesita ayuda, puedes ponerte en contacto con el soporte técnico de Microsoft para abrir una solicitud de servicio en nombre del cliente.

Los clientes pueden averiguar cuáles de sus partners tienen privilegios de administrador para su inquilino desde dentro del portal de administración de Office 365. Para ello:

1. El cliente debe iniciar sesión en el portal de administración de Office 365 como administrador global.

2. Selecciona **Configuración** > **Relaciones con los partners**.

3. En la página **Relaciones con los partners**, el cliente verá una lista de los partners con los que trabajan y de los que hayan recibido privilegios de administración delegada para sus inquilinos.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Los clientes pueden administrar los privilegios de administrador delegado de un partner 

El cliente puede decidir retirarte tus privilegios de administrador delegado de su inquilino, pero conservar la relación contigo con fines de suscripción y renovación de licencias. Los clientes administran los derechos y permisos de sus cuentas de Office 365 en la página **Relaciones con los partners** del Centro de administración de Office 365. En esta página, los clientes pueden:

- Consultar los partners con los que tienen una relación y qué partners han delegado privilegios de administrador

- Quitar los privilegios de administrador delegado de un partner para el inquilino

Para quitar los privilegios de administración delegada de un partner:

1. En la página **Relaciones con los partners**, selecciona el partner de interés.
2. En el panel de detalles, selecciona **Remove delegated admin** (Quitar administrador delegado).
3. En el panel de confirmación, selecciona **Quitar**.

>[!IMPORTANT]  
>Las asignaciones de roles de Azure AD al partner son implícitas. Si intentas enumerar los miembros de los roles de Azure AD mediante el portal de Azure AD/PowerShell/Graph, no aparecerá el partner. Para averiguar si los socios están asignados a roles de Azure AD, debes consultar la página de relaciones con los partners del Portal de administración de Office 365, para averiguar si el privilegio de administrador delegado se ha concedido al partner o no.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Privilegios de administrador delegado en Azure AD 

Hay dos grupos de seguridad, agentes de administración y agentes del departamento de soporte técnico, en el inquilino de Azure AD del partner, que se usan para la administración delegada. Cuando un cliente concede el privilegio de administración delegada a un partner:

- El grupo de agentes de administración se asigna al rol de administrador global en el inquilino de Azure AD del cliente.

- El grupo de agentes del departamento de soporte técnico se asigna al rol de administrador del departamento de soporte técnico en el inquilino de Azure AD del cliente.

En función de los roles de directorio asignados, los miembros de ambos grupos pueden iniciar sesión en el inquilino de Azure AD del cliente y en los servicios de O365, con sus credenciales de partner y administrador, en nombre del cliente.

Si el cliente quita privilegios de administrador delegado, se quitan las asignaciones de rol de Azure AD y ya no podrás administrar el inquilino de Azure AD del cliente.

### <a name="azure-subscriptions-and-resource-management"></a>Suscripciones de Azure y administración de recursos

Cada suscripción de Azure tiene su propio conjunto de roles de administración de recursos. Para que un partner de CSP pueda administrar una suscripción de Azure de un cliente, el partner debe estar asignado a uno o más roles en la suscripción de Azure. Específicamente:

- Cuando un cliente acepta una invitación de un revendedor y concede el privilegio de administración delegada a un partner, este último no obtiene automáticamente acceso a las suscripciones de Azure existentes en el inquilino del cliente.

- Cuando el partner CSP aprovisiona una nueva suscripción de Azure para el cliente, al grupo de agentes de administración del inquilino de partner de CSP se le asigna automáticamente el rol de propietario en la suscripción. En función de esta asignación de roles, los miembros del grupo pueden acceder a recursos y administrarlos en la suscripción.

- Cuando un cliente quita privilegios administrativos delegadas de un partner mediante el Portal de Office 365, el partner sigue pudiendo administrar la suscripción de Azure del cliente, en tanto que el partner aún está asignado a uno o más roles en la suscripción. Para que el partner deje de administrar la suscripción de Azure, el cliente debe quitar la asignación de roles.

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

Desde el Centro de partners, los partners de CSP pueden administrar perfiles de Autopilot para sus clientes sin privilegios de administrador delegado en estas circunstancias: 

- Si un cliente quita los privilegios de administración delegada, pero conserva una relación de revendedor contigo, puedes seguir administrando sus perfiles de Autopilot.

- Puedes administrar los dispositivos del cliente que tú u otro partner hayáis agregado. 

- No puedes administrar los dispositivos que ha agregado tu cliente a través de Microsoft Store para Empresas, Microsoft Store para Educación o el portal de Microsoft Intune.

Para más información sobre Autopilot, consulta [Simplificar la configuración de dispositivos con Windows Autopilot](https://docs.microsoft.com/partner-center/autopilot).

>[!IMPORTANT]  
>La experiencia actual de administración de Autopilot en el Centro de partners podría seguir modificando. En el momento de publicar este artículo, se están planteando los siguientes cambios:

- Los partners deben tener privilegios de administración delegada del cliente para poder agregar, actualizar o quitar perfiles y aplicar o quitar perfiles de todos los dispositivos del inquilino del cliente.

- Los partners deben recibir privilegios de administración delegada del cliente para poder quitar los dispositivos agregados por otros partners o por el cliente en el inquilino del cliente. De lo contrario, el partner solo puede quitar los dispositivos agregados anteriormente por el mismo partner.
