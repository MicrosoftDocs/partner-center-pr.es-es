---
title: Creación de cuentas de usuario y asignación de roles
description: Cada empleado debe tener asignado un rol para poder acceder al Centro de partners. Obtén información acerca de cómo crear cuentas de usuario, asignar roles y establecer permisos.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: parthpandyaMSFT
ms.author: parthp
ms.custom: SEOAPR.20
ms.localizationpriority: high
ms.date: 02/26/2020
ms.openlocfilehash: 637e88205d9944f7220e227b5101220d94ed42db
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000439"
---
# <a name="create-user-accounts-and-assign-roles-and-permissions"></a>Creación de cuentas de usuario y asignación de roles y permisos

**Roles adecuados**

- Administrador de cuentas
- Administrador global
- Administrador del control de usuarios

Crear cuentas de usuario para los empleados que necesitan acceder al Centro de partners. Estas tareas las debe llevar a cabo el administrador de gestión de usuarios, el administrador de cuentas o el administrador global. El usuario que realiza estas tareas también debe tener asignados los roles Administrador de usuarios o Administrador global de Azure Active Directory (AAD). Para obtener más información, sobre los roles de AAD, consulta [Permisos de roles de administrador en Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).


## <a name="add-a-new-user"></a>Agregar un usuario nuevo

1. En el icono **Configuración** de la parte superior derecha del Centro de partners, selecciona **Administración de usuarios**.

2. Selecciona **Agregar usuario**.

3. Escribe el nombre completo y la dirección de correo electrónico única del usuario.

4. Selecciona el tipo de agente o el tipo de administrador que quieres asignar al usuario. El acceso al Centro de partners se basa en roles, por lo que puedes asignar permisos para personalizar la vista del usuario y mostrar solo las características que el usuario necesite para completar las tareas específicas.  Si los usuarios quieren una asignación de roles, para encontrar administradores globales y ponerse en contacto con ellos, deben ir a **Administración de usuarios** y filtrar por administradores globales.

5. Selecciona **Agregar** para crear la cuenta de usuario. Confirma los detalles del usuario en la página siguiente.

> [!IMPORTANT]  
> Anota la nueva información de inicio de sesión del usuario que aparece en esta página. Asegúrate de copiar y enviar esta información al nuevo usuario ya que no volverás a tener acceso a ella. 


El usuario tendrá que iniciar sesión en el Centro de partners con su nombre de usuario y su contraseña temporal. Cuando el usuario inicie sesión en el Centro de partners por primera vez, se le pedirá cambiar la contraseña. 

## <a name="find-the-role-youve-been-assigned"></a>Buscar el rol que se le ha asignado

Si el administrador global no se lo ha indicado, puede averiguar qué rol tiene en el Centro de partners mediante el siguiente procedimiento:

1. Inicie sesión en el [panel] del Centro de partners https://partner.microsoft.com/dashboard/home).

1. Seleccione el icono de **Configuración de la cuenta** y, a continuación, seleccione **Mi perfil**.
 
1. Seleccione la pestaña **Roles y permisos**. Verá sus roles y permisos.
 

>[!Note]
>Si no ve un programa cuando inicia sesión, normalmente significa que no tiene los permisos correctos para trabajar en ese programa. Por lo tanto, por ejemplo, si no ve la página Incentivos cuando inicia sesión, no tiene permisos para el programa Incentivos. El administrador global puede proporcionarle los permisos necesarios.


## <a name="find-your-global-admin"></a>Buscar el administrador global

En ocasiones, es posible que un usuario tenga que cambiar su rol o que un usuario nuevo quiera una asignación de rol específica.  
Para buscar un administrador global que pueda realizar cambios de rol o asignar roles a un nuevo usuario, en el **icono de Configuración de la cuenta** de la parte superior derecha del Centro de partners, seleccione **Administración de usuarios** y filtre por el administrador global, o bien diríjase a **Mi perfil**, seleccione **Roles y permisos** y consulte una lista de los diferentes administradores que pueden ayudarle a elevar sus permisos. 


## <a name="new-global-admin"></a>Nuevo administrador global

Si el administrador global deja la organización y alguien debe ocupar su rol, puedes enviar una incidencia al equipo de Azure o de Office 365. Para averiguar cómo hacerlo, selecciona una de las opciones siguientes.

[Nuevo administrador global para Azure](https://support.microsoft.com/help/4505981/what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company)

[Nuevo administrador global para Office 365](https://admin.microsoft.com/)


## <a name="assign-user-roles"></a>Asignar roles de usuario

Para trabajar en el Centro de partners, debes tener un rol asignado.  Actualmente, los roles incluyen roles de inquilino de Azure Active Directory, roles de proveedor de soluciones en la nube (CSP) y roles de empresa que no son de AAD. Una empresa individual puede necesitar todos estos roles.

>[!Important]
>Los usuarios deben aparecer en tu inquilino para acceder al Centro de partners. Las asignaciones de roles proporcionan acceso adicional.


**Los roles de inquilino de AAD incluyen**:
- Administrador global
- Administrador de usuarios

**Los roles de CSP incluyen**:
- Agente de administrador
- Administrador de facturación
- Agente de ventas
- Agente del departamento de soporte técnico

**Roles que administran la pertenencia a MPN y la empresa (no AAD)**
- Administrador de partners de MPN
- Administrador de cuentas
- Administrador de referencias
- Administrador del perfil de negocio
- Administrador y usuario de incentivos

**Proveedor de panel de control es un rol de CSP y no de AAD**.
- Administrador global

El rol **Usuario invitado** debe formar parte del inquilino de AAD y puede tener cualquier rol que no sea de AAD.

Para obtener información específica sobre los roles y lo que puede hacer cada rol, consulta [Asignar permisos de usuario](permissions-overview.md).

## <a name="associate-a-users-microsoft-learn-account-in-partner-center"></a>Asociar la cuenta de Microsoft Learn de un usuario en el Centro de partners

Para poder ver las rutas de entrenamiento y aprendizaje que siguen tus usuarios para sus competencias, deben asociar su identificador de MCP a su cuenta del Centro de partners. Como administrador global, al agregar nuevos usuarios, asegúrate de recordarles que asocien su identificador de MCP a su cuenta. 

### <a name="how-to-associate-your-mcp-id-to-your-partner-center-account"></a>Cómo asociar el identificador de MCP a tu cuenta del Centro de partners

1. En el panel del Centro de partners, selecciona el icono de **Tu cuenta** en la esquina derecha del panel y, a continuación, selecciona **Mi perfil**.

2. En **Your learning** (Tu aprendizaje), podrás asociar tu cuenta de Microsoft Learning y conectar tu cuenta de Microsoft a Partner University.

## <a name="next-steps"></a>Pasos siguientes

- [Asignación de roles y permisos a los usuarios de una empresa que necesitan trabajar en el Centro de partners](permissions-overview.md)