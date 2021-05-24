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
# <a name="create-user-accounts"></a><span data-ttu-id="713fd-104">Crear las cuentas de usuario</span><span class="sxs-lookup"><span data-stu-id="713fd-104">Create user accounts</span></span>  

<span data-ttu-id="713fd-105">**Roles adecuados:** Administrador de cuentas | Administrador global | Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="713fd-105">**Appropriate roles**: Account admin | Global admin | User management admin</span></span>

<span data-ttu-id="713fd-106">Crear cuentas de usuario para los empleados que necesitan acceder al Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="713fd-106">Create user accounts for employees who need access to the Partner Center.</span></span> <span data-ttu-id="713fd-107">Estas tareas las debe llevar a cabo el administrador de gestión de usuarios, el administrador de cuentas o el administrador global. El usuario que realiza estas tareas también debe tener asignados los roles Administrador de usuarios o Administrador global de Azure Active Directory (AAD).</span><span class="sxs-lookup"><span data-stu-id="713fd-107">These tasks must be done by the user management admin, accounts admin, or the global admin. The user performing these tasks must also be assigned the Azure Active Directory (AAD) roles of User administrator or Global administrator.</span></span> <span data-ttu-id="713fd-108">Para obtener más información, sobre los roles de AAD, consulta [Permisos de roles de administrador en Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span><span class="sxs-lookup"><span data-stu-id="713fd-108">For more information about AAD roles, see [Administrator role permissions in Azure Active Directory](/azure/active-directory/users-groups-roles/directory-assign-admin-roles).</span></span>

## <a name="add-a-new-user"></a><span data-ttu-id="713fd-109">Agregar un usuario nuevo</span><span class="sxs-lookup"><span data-stu-id="713fd-109">Add a new user</span></span>

1. <span data-ttu-id="713fd-110">En el icono **Configuración** de la parte superior derecha del Centro de partners, seleccione **Configuración de la cuenta** y, luego, **Administración de usuarios**.</span><span class="sxs-lookup"><span data-stu-id="713fd-110">From the **Settings** icon at the top right of the Partner Center, select **Account settings** and then select **User management**.</span></span>

2. <span data-ttu-id="713fd-111">Selecciona **Agregar usuario**.</span><span class="sxs-lookup"><span data-stu-id="713fd-111">Select **Add user**.</span></span>

3. <span data-ttu-id="713fd-112">Escribe el nombre completo y la dirección de correo electrónico única del usuario.</span><span class="sxs-lookup"><span data-stu-id="713fd-112">Enter the user's full name and unique email address.</span></span>

4. <span data-ttu-id="713fd-113">Selecciona el tipo de agente o el tipo de administrador que quieres asignar al usuario.</span><span class="sxs-lookup"><span data-stu-id="713fd-113">Select the type of agent and/or the type of admin you want to assign to the user.</span></span> <span data-ttu-id="713fd-114">El acceso al Centro de partners se basa en roles, por lo que puedes asignar permisos para personalizar la vista del usuario y mostrar solo las características que el usuario necesite para completar las tareas específicas.</span><span class="sxs-lookup"><span data-stu-id="713fd-114">Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks.</span></span>  <span data-ttu-id="713fd-115">Si los usuarios quieren una asignación de roles, para encontrar administradores globales y ponerse en contacto con ellos, deben ir a **Administración de usuarios** y filtrar por administradores globales.</span><span class="sxs-lookup"><span data-stu-id="713fd-115">If users want a role assignment, they can find global admins to contact by going to **User management** and filtering on global admin.</span></span>

5. <span data-ttu-id="713fd-116">Selecciona **Agregar** para crear la cuenta de usuario.</span><span class="sxs-lookup"><span data-stu-id="713fd-116">Select **Add** to create the user account.</span></span> <span data-ttu-id="713fd-117">Confirma los detalles del usuario en la página siguiente.</span><span class="sxs-lookup"><span data-stu-id="713fd-117">Confirm the user's details on the next page.</span></span>

> [!IMPORTANT]  
> <span data-ttu-id="713fd-118">Anota la nueva información de inicio de sesión del usuario que aparece en esta página.</span><span class="sxs-lookup"><span data-stu-id="713fd-118">Make a note of the new user's sign-in information displayed on this page.</span></span> <span data-ttu-id="713fd-119">Asegúrate de copiar y enviar esta información al nuevo usuario ya que no volverás a tener acceso a ella.</span><span class="sxs-lookup"><span data-stu-id="713fd-119">Be sure to copy and send this information to the new user as you will not be able to access it again later.</span></span> 

<span data-ttu-id="713fd-120">El usuario tendrá que iniciar sesión en el Centro de partners con su nombre de usuario y su contraseña temporal.</span><span class="sxs-lookup"><span data-stu-id="713fd-120">The user will need to sign in to the Partner Center with their user name and temporary password.</span></span> <span data-ttu-id="713fd-121">Cuando el usuario inicie sesión en el Centro de partners por primera vez, se le pedirá cambiar la contraseña.</span><span class="sxs-lookup"><span data-stu-id="713fd-121">When the user signs in to the Partner Center for the first time, they are prompted to change their password.</span></span>

## <a name="assign-user-roles"></a><span data-ttu-id="713fd-122">Asignar roles de usuario</span><span class="sxs-lookup"><span data-stu-id="713fd-122">Assign user roles</span></span>

<span data-ttu-id="713fd-123">Para trabajar en el Centro de partners, debes tener un rol asignado.</span><span class="sxs-lookup"><span data-stu-id="713fd-123">To work in the Partner Center, you must have an assigned role.</span></span>  <span data-ttu-id="713fd-124">Actualmente, los roles incluyen roles de inquilino de Azure Active Directory, roles de proveedor de soluciones en la nube (CSP) y roles de empresa que no son de AAD.</span><span class="sxs-lookup"><span data-stu-id="713fd-124">Currently, roles include Azure Active Directory tenant roles, Cloud Solution Provider (CSP) roles, and non-AAD company roles.</span></span> <span data-ttu-id="713fd-125">Una empresa individual puede necesitar todos estos roles.</span><span class="sxs-lookup"><span data-stu-id="713fd-125">An individual company can have a need for all of these roles.</span></span>

>[!Important]
><span data-ttu-id="713fd-126">Los usuarios deben aparecer en tu inquilino para acceder al Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="713fd-126">Individuals must be listed in your tenant to access Partner Center.</span></span> <span data-ttu-id="713fd-127">Las asignaciones de roles proporcionan acceso adicional.</span><span class="sxs-lookup"><span data-stu-id="713fd-127">Role assignments provide additional access.</span></span>

## <a name="next-steps"></a><span data-ttu-id="713fd-128">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="713fd-128">Next steps</span></span>

- [<span data-ttu-id="713fd-129">Asignación de roles y permisos a los empleados que necesitan trabajar en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="713fd-129">Assign users roles and permissions for employees needing to work in Partner Center</span></span>](permissions-overview.md)
