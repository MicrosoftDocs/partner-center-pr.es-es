---
title: Los clientes delegan privilegios administrativos en los partners | Centro de partners
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo pedir a los clientes que deleguen permisos de administrador en un revendedor o quite los mismos permisos y cómo usar los permisos.
author: LauraBrenner
ms.author: labrenne
keywords: privilegios de administrador delegado, administrador en nombre de, quitar privilegios, DAP, AOBO
ms.localizationpriority: medium
ms.openlocfilehash: 8f49fa5c4b320d05c6c6a9049b41170457bb394f
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253481"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>Los clientes delegan privilegios administrativos en los partners

**Se aplica a**

-  Centro de partners

Para administrar la suscripción o el servicio de un cliente en su nombre, el cliente debe conceder permisos de administrador de dicho servicio. Para obtener los permisos de administrador de un cliente, envíale un correo electrónico con una solicitud de relación de revendedor. Cuando el cliente apruebe la solicitud, podrás iniciar sesión en el portal de administración del servicio y administrar el servicio en nombre del cliente. 

## <a name="invite-a-customer-to-establish-a-reseller-relationship-with-you"></a>Invitar a un cliente a establecer una relación de revendedor contigo

1.  Seleccione **clientes** y, a continuación, seleccione **solicitar una relación de revendedor**.

2.  En la siguiente página, revisa el borrador del mensaje de correo electrónico. Puedes abrir el borrador de mensaje de correo electrónico en la aplicación de mensajería predeterminada o puedes copiar el mensaje en el portapapeles y pegarlo en un correo electrónico. 

    >[!IMPORTANT]
    >Puedes editar el texto en el correo electrónico, pero asegúrate de incluir el vínculo, ya que se trata de un vínculo personalizado que conecta al cliente directamente con tu cuenta. 
    
3.  Seleccione **listo** cuando haya completado este paso.

4.  Envía el correo electrónico a tu cliente.

5.  Una vez que el cliente acepte tu invitación, aparecerá en la página **Clientes** y, podrás aprovisionar y administrar el servicio para el cliente desde allí.

6.  Para administrar la cuenta del cliente, los servicios, los usuarios y las licencias, expanda el registro del cliente seleccionando la flecha abajo junto a su nombre y, a continuación, seleccione el portal de administración para el servicio que desea administrar.

>[!IMPORTANT]  
>Los clientes pueden reasignar o quitar permisos de administrador en el portal de administración de un servicio. Sin embargo, a no ser que hayas renegociado tu acuerdo con el cliente, continúas siendo el responsable de proporcionar al cliente soporte técnico y de cumplir con los términos del acuerdo de revendedor en la nube, incluso después de que el cliente reasigne o elimine los permisos de administrador. En esta situación, si el cliente necesita ayuda, póngase en contacto con el soporte técnico de Microsoft para abrir una solicitud de servicio en nombre del cliente.

Los clientes pueden averiguar cuál de sus asociados tienen privilegios de administrador en el inquilino desde el portal de administración de Office 365. Para ello:

1. El cliente debe iniciar sesión en el portal de administración de Office 365 como administrador global.

2. Seleccione **configuración** > **relaciones de socio**.

3. En la página **relaciones de socios comerciales** , el cliente verá una lista de los asociados con los que trabajan y aquellos a los que se les han concedido privilegios de administración delegados a su inquilino.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Los clientes pueden administrar los privilegios de administrador delegado de un asociado 

Es posible que el cliente decida quitar los privilegios de administrador delegado de su inquilino, pero conserve la relación con usted para fines de suscripción y renovación de licencias. Los clientes administran los derechos y permisos de sus cuentas de Office 365 en la página **Relaciones con los partners** del Centro de administración de Office 365. En esta página, los clientes pueden:

- Consultar los partners con los que tienen una relación y qué partners han delegado privilegios de administrador

- Quitar los privilegios de administración delegados de un asociado del inquilino

Quitar los privilegios de administración delegados de un partner:

1. En la página **Relaciones de partners**, selecciona el partner de interés.
2. En el panel de detalles, selecciona **Quitar administrador delegado**.
3. En el panel de confirmación, seleccione **Quitar**.

>[!IMPORTANT]  
>Las asignaciones de roles de Azure AD al partner son implícitas. Si intentas enumerar los miembros de los roles de Azure AD mediante Portal/PowerShell/Graph de Azure AD, no aparecerá el partner. Para averiguar si los socios están asignados a roles de Azure AD, debes hacer referencia a la página de relaciones con partners del Portal de administración de Office 365, para averiguar si el privilegio de administrador delegado se ha concedido al partner o no.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Privilegios de administrador delegado en Azure AD 

Hay dos grupos de seguridad, agentes de administración y agentes de soporte técnico, en el inquilino de Azure AD del asociado que se usan para la administración delegada. Cuando un cliente concede el privilegio de administración delegada a un partner:

- El grupo de agentes de administración se asigna al rol de administrador global en el inquilino de Azure AD del cliente.

- El grupo de agentes del Departamento de soporte técnico se asigna al rol de administrador del Departamento de soporte técnico en el inquilino de Azure AD del cliente.

En función de los roles de directorio asignados, los miembros de ambos grupos pueden iniciar sesión en el inquilino de Azure AD del cliente y los servicios de O365 con sus credenciales de asociado y administrador en nombre del cliente.

Si el cliente quita los privilegios de administrador delegados, se quitan las asignaciones de roles Azure AD y ya no podrá administrar el inquilino de Azure AD del cliente.

### <a name="azure-subscriptions-and-resource-management"></a>Suscripciones de Azure y administración de recursos

Cada suscripción de Azure tiene su propio conjunto de roles de administración de recursos. Para que un asociado de CSP pueda administrar una suscripción de Azure de un cliente, el asociado debe estar asignado a uno o varios roles de la suscripción de Azure. Concretamente:

- Cuando un cliente acepta una invitación de un revendedor y concede privilegio de administración delegada a un partner, este último no obtiene automáticamente acceso a las suscripciones de Azure existentes en el inquilino del cliente.

- Cuando el partner CSP aprovisiona una nueva suscripción de Azure para el cliente, al grupo de agentes de administración del inquilino de partner de CSP se le asigna automáticamente el rol de propietario en la suscripción. En función de esta asignación de roles, los miembros del grupo pueden acceder a recursos y administrarlos en la suscripción.

- Cuando un cliente quita los privilegios de administración delegados de un asociado mediante el portal de Office 365, el asociado todavía puede administrar la suscripción de Azure del cliente siempre que el socio todavía esté asignado a uno o varios roles de la suscripción. Para que el partner deje de administrar la suscripción de Azure, el cliente debe quitar la asignación de roles.

## <a name="windows-autopilot"></a>Windows Autopilot

<!--Maggie, 12/5/18 - Removed table showing what different CSP partner types can and can't do because all partner types are now in parity. As per Bhavya Chopra in bug 19841770.-->

Desde el centro de Partners, los asociados de CSP pueden administrar perfiles de AutoPilot para sus clientes sin privilegios de administrador delegados en estas circunstancias: 

- Si un cliente quita los privilegios de administración delegados pero conserva una relación de revendedor con usted, puede seguir administrando los perfiles de AutoPilot para ellos.

- Puede administrar los dispositivos del cliente que usted u otro asociado hayan agregado. 

- No puede administrar los dispositivos que ha agregado su cliente a través de la Microsoft Store para empresas, Microsoft Store para educación o Microsoft Intune portal.

Para obtener más información acerca de AutoPilot, consulte [simplificar la configuración de dispositivos con Windows AutoPilot](https://docs.microsoft.com/partner-center/autopilot).

>[!IMPORTANT]  
>La experiencia actual de administración de AutoPilot en el centro de Partners podría seguir modificando. En el momento en que se publicó este artículo, se están considerando los siguientes cambios:

- Los partners deben tener privilegios de administración delegada del cliente para poder agregar, actualizar o eliminar perfiles y aplicar o quitar perfiles de todos los dispositivos del inquilino del cliente.

- El cliente debe conceder privilegios de administración delegada para que el asociado pueda quitar los dispositivos agregados por otros asociados o por el cliente en el inquilino del cliente. De lo contrario, el asociado puede quitar solo los dispositivos agregados anteriormente por el mismo socio.
