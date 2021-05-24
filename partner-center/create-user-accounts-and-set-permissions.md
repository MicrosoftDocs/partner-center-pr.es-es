---
title: Creación de cuentas de usuario y asignación de roles
description: Cada empleado debe tener asignado un rol para poder acceder al Centro de partners. Obtén información acerca de cómo crear cuentas de usuario, asignar roles y establecer permisos.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
ms.custom: contperf-fy21q2
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.date: 10/12/2020
ms.openlocfilehash: 9621f0bc3283d7d3b08e2ebac62b4e5d8c95a4d4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148149"
---
# <a name="create-user-accounts"></a>Crear las cuentas de usuario  

**Roles adecuados:** Administrador de cuentas | Administrador global | Administrador de usuarios

Crear cuentas de usuario para los empleados que necesitan acceder al Centro de partners. Estas tareas las debe llevar a cabo el administrador de gestión de usuarios, el administrador de cuentas o el administrador global. El usuario que realiza estas tareas también debe tener asignados los roles Administrador de usuarios o Administrador global de Azure Active Directory (AAD). Para obtener más información, sobre los roles de AAD, consulta [Permisos de roles de administrador en Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).

## <a name="add-a-new-user"></a>Agregar un usuario nuevo

1. En el icono **Configuración** de la parte superior derecha del Centro de partners, seleccione **Configuración de la cuenta** y, luego, **Administración de usuarios**.

2. Selecciona **Agregar usuario**.

3. Escribe el nombre completo y la dirección de correo electrónico única del usuario.

4. Selecciona el tipo de agente o el tipo de administrador que quieres asignar al usuario. El acceso al Centro de partners se basa en roles, por lo que puedes asignar permisos para personalizar la vista del usuario y mostrar solo las características que el usuario necesite para completar las tareas específicas.  Si los usuarios quieren una asignación de roles, para encontrar administradores globales y ponerse en contacto con ellos, deben ir a **Administración de usuarios** y filtrar por administradores globales.

5. Selecciona **Agregar** para crear la cuenta de usuario. Confirma los detalles del usuario en la página siguiente.

> [!IMPORTANT]  
> Anota la nueva información de inicio de sesión del usuario que aparece en esta página. Asegúrate de copiar y enviar esta información al nuevo usuario ya que no volverás a tener acceso a ella. 

El usuario tendrá que iniciar sesión en el Centro de partners con su nombre de usuario y su contraseña temporal. Cuando el usuario inicie sesión en el Centro de partners por primera vez, se le pedirá cambiar la contraseña.

## <a name="assign-user-roles"></a>Asignar roles de usuario

Para trabajar en el Centro de partners, debes tener un rol asignado.  Actualmente, los roles incluyen roles de inquilino de Azure Active Directory, roles de proveedor de soluciones en la nube (CSP) y roles de empresa que no son de AAD. Una empresa individual puede necesitar todos estos roles.

>[!Important]
>Los usuarios deben aparecer en tu inquilino para acceder al Centro de partners. Las asignaciones de roles proporcionan acceso adicional.

## <a name="next-steps"></a>Pasos siguientes

- [Asignación de roles y permisos a los empleados que necesitan trabajar en el Centro de partners](permissions-overview.md)
