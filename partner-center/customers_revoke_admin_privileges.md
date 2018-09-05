---
title: Los clientes delegan privilegios administrativos en los partners | Centro de partners
description: Como partner revendedor, los clientes pueden delegar en ti para que seas su administrador. También pueden quitar privilegios.
author: labrenne
keywords: privilegios de administrador delegados, administración en nombre de, quitar privilegios
ms.localizationpriority: medium
ms.openlocfilehash: 7209917a92eb2cd9ae86c31f3126bdbac402a04e
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/31/2018
ms.locfileid: "2877175"
---
# <a name="customers-delegate-administration-privileges-to-partners"></a>Los clientes delegan privilegios administrativos en los partners

**Aplicable a**

-  Centro de partners

Como partner de CSP y asesor de confianza de tus clientes, estos podrán delegar en ti para que seas el administrador de su inquilino de Azure AD y de Office 365. Puedes iniciar esa relación a través del Panel de partners, enviándoles una invitación. 

1. En el menú **Panel**, selecciona **Clientes** y entonces selecciona **Solicitar una relación con un cliente**.
2. Aparecerá un correo electrónico de formulario que contendrá tu dirección url. Puedes copiar y pegar el formulario en un correo electrónico para enviarlo a tu cliente. No dudes en agregar cualquier información adicional, pero asegúrate de incluir la dirección url. El cliente usará esa dirección url para responder a la solicitud.  
3. Cuando el cliente acepte la invitación, pasarás a ser el administrador de sus servicios.

Los clientes pueden averiguar cuáles de sus partners tienen privilegios de administrador para su inquilino desde dentro del portal de servicio de Office 365. Para ello:

1. Inicia sesión en el [portal de administración de Office 365](https://portal.office.com/adminportal) como administrador global.
2. Selecciona **Configuración** → **Relaciones con partners**.
3. En la página **Relaciones con partners**, verán una lista de los partners con los que trabajan y de los que hayan recibido privilegios de administración delegados para sus inquilinos.

## <a name="customers-can-manage-a-partners-delegated-admin-privileges"></a>Los clientes pueden administrar los privilegios de administrador delegados en un partner 

El cliente puede decidir retirarte tus privilegios de administrador de su inquilino, pero conservar la relación contigo con fines de suscripción y renovación de licencias. Los clientes administran los derechos y permisos de sus cuentas de Office 365 en la página **Relaciones con los partners** del Centro de administración de Office 365. En esta página, los clientes pueden:

- Consultar los partners con los que tienen una relación y qué partners han delegado privilegios de administrador

- Quitar los privilegios de administrador delegado de un partner para el inquilino

Quitar los privilegios de administración delegados de un partner:

1. En la página **Relaciones de partners**, selecciona el partner de interés.
2. En el panel de detalles, selecciona **Quitar administrador delegado**.
3. En el panel de confirmación, seleccione **Quitar**.

>**Importante**<br>
Las asignaciones de roles de Azure AD al partner son implícitas. Si intentas enumerar los miembros de los roles de Azure AD mediante Portal/PowerShell/Graph de Azure AD, no aparecerá el partner. Para averiguar si los socios están asignados a roles de Azure AD, debes hacer referencia a la página de relaciones con partners del Portal de administración de Office 365, para averiguar si el privilegio de administrador delegado se ha concedido al partner o no.

## <a name="delegated-admin-privileges-in-azure-ad"></a>Privilegios de administrador delegado en Azure AD 

Hay dos grupos de seguridad, agentes de administración y agentes del departamento de soporte técnico, en el inquilino de Azure AD, que se usan para administración delegada. Cuando un cliente concede el privilegio de administración delegada a un partner:

- El grupo de agentes de administración se asigna a la función de administrador global en el inquilino de Azure AD del cliente.

- El grupo de agentes del departamento de soporte técnico se asigna a la función de administrador del departamento de soporte técnico en el inquilino de Azure AD del cliente.

En función de los roles de directorio asignados, los miembros de ambos grupos pueden iniciar sesión en el inquilino de Azure AD del cliente y en los servicios de O365, con sus credenciales de partner y administrador, en nombre del cliente.

Si el cliente quita privilegios de administrador delegado, se quitan las asignaciones de rol de Azure AD y ya no podrás administrar el inquilino de Azure AD del cliente.

### <a name="azure-subscriptions-and-resource-management"></a>Suscripciones de Azure y administración de recursos

Cada suscripción de Azure tiene su propio conjunto de roles de administración de recursos. Para que un partner de CSP pueda administrar una suscripción de Azure de un cliente, el partner debe estar asignado a uno o más roles en la suscripción de Azure. Concretamente:

- Cuando un cliente acepta una invitación de un revendedor y concede privilegio de administración delegada a un partner, este último no obtiene automáticamente acceso a las suscripciones de Azure existentes en el inquilino del cliente.

- Cuando el partner CSP aprovisiona una nueva suscripción de Azure para el cliente, al grupo de agentes de administración del inquilino de partner de CSP se le asigna automáticamente el rol de propietario en la suscripción. En función de esta asignación de roles, los miembros del grupo pueden acceder a recursos y administrarlos en la suscripción.

- Cuando un cliente quita privilegios administrativos delegadas de un asociado con el Portal de Office 365, el partner sigue pudiendo administrar la suscripción de Azure del cliente, en tanto que el partner aún está asignado a una o más funciones en la suscripción. Para que el partner deje de administrar la suscripción de Azure, el cliente debe quitar la asignación de roles.

## <a name="windows-autopilot"></a>WindowsAutoPilot 

Desde el Panel de partners, los partners de CSP pueden administrar la configuración de AutoPilot para sus clientes, incluso sin privilegios de administrador delegado. Obtén más información sobre [Simplificar la configuración de dispositivos con Windows Autopilot.](https://docs.microsoft.com/partner-center/autopilot)

Lo que puedes hacer depende de si eres un revendedor indirecto o directo.

|**Operación**   |**Revendedor directo o revendedor indirecto**   |**Revendedor indirecto**   |
|-----------------|-----------------------------------| -----------------------------|
|Agregar dispositivos (con un archivo csv)  |Sí      |No|
|Quitar dispositivos   |Sí   |No|
|Agregar perfil   |Sí   | Sí   |
|Actualizar perfil   |Sí    |Sí   |
|Quitar perfil   |Sí   |Sí   |
|Aplicar un perfil a dispositivos   |Sí   |Sí   |
|Quitar perfil desde dispositivos   |Sí   |Sí   | 

- Los partners de CSP pueden seguir administrando la configuración de AutoPilot para los clientes existentes con relación de revendedor, incluso si los clientes han quitado lo privilegios de administración delegada a sus partners.

- Puedes administrar los dispositivos existentes para los clientes que ya hayas agregado o que los haya agregado otro partner de CSP.

- No puedes administrar dispositivos que haya cargado tu cliente (a través de Microsoft Store para Empresas o el Portal de Microsoft Intune).

>**Importante** La experiencia de administración de AutoPilot en el Centro de partners de Microsoft no es definitiva y está sujeta a cambios en el futuro. En el momento de redactar este artículo, se están planteando los siguientes cambios:

  - Los partners deben tener privilegios de administración delegada del cliente para poder agregar, actualizar o eliminar perfiles y aplicar o quitar perfiles de todos los dispositivos del inquilino del cliente.

- Los partners deben recibir privilegios de administración delegada del cliente para poder quitar dispositivos cargados por otros partners o por el cliente en el inquilino del cliente. De lo contrario, el partner solo puede quitar los dispositivos agregados anteriormente por el mismo partner.
