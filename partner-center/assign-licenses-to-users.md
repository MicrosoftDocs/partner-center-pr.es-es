---
title: Administrar usuarios en cuentas de cliente
ms.topic: how-to
ms.date: 05/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información acerca de cómo crear cuentas de usuario para un cliente, agregar o quitar licencias de usuario, restablecer contraseñas de usuario, eliminar cuentas de usuario o restaurarlas.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a3febadda51094d443d83d17b640b1744a130335
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527681"
---
# <a name="user-management-tasks-for-customer-accounts-in-partner-center"></a><span data-ttu-id="e7e46-103">Tareas de administración de usuarios para cuentas de cliente en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="e7e46-103">User management tasks for customer accounts in Partner Center</span></span>

<span data-ttu-id="e7e46-104">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="e7e46-104">**Applies to**</span></span>

- <span data-ttu-id="e7e46-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="e7e46-105">Partner Center</span></span>

<span data-ttu-id="e7e46-106">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="e7e46-106">**Appropriate roles**</span></span>

- <span data-ttu-id="e7e46-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e7e46-107">Global admin</span></span>
- <span data-ttu-id="e7e46-108">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="e7e46-108">User management admin</span></span>
- <span data-ttu-id="e7e46-109">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="e7e46-109">Admin agent</span></span>
- <span data-ttu-id="e7e46-110">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="e7e46-110">Sales agent</span></span>
- <span data-ttu-id="e7e46-111">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="e7e46-111">Helpdesk agent</span></span>

<span data-ttu-id="e7e46-112">Puede crear y eliminar nuevos usuarios en la cuenta de un cliente.</span><span class="sxs-lookup"><span data-stu-id="e7e46-112">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="e7e46-113">También puede restaurar una o más cuentas de usuario que haya eliminado previamente en un plazo de 30 días a partir de la eliminación.</span><span class="sxs-lookup"><span data-stu-id="e7e46-113">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="e7e46-114">Las asignaciones anteriores de la suscripción del usuario también se restaurarán (suponiendo que sus asignaciones anteriores estén disponibles).</span><span class="sxs-lookup"><span data-stu-id="e7e46-114">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="e7e46-115">Al comprar nuevas suscripciones para un cliente, el cliente debe proporcionarle una lista de todos los usuarios que necesitarán cuentas, sus permisos de usuario y los servicios que necesite cada usuario.</span><span class="sxs-lookup"><span data-stu-id="e7e46-115">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

<span data-ttu-id="e7e46-116">Puede [asignar suscripciones a varios usuarios](bulk-license-provisioning-for-multiple-users.md) al mismo tiempo importando los nombres mediante un [archivo de hoja de cálculo. csv compatible con Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="e7e46-116">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="e7e46-117">Crear cuentas de usuario para un cliente</span><span class="sxs-lookup"><span data-stu-id="e7e46-117">Create user accounts for a customer</span></span>

1. <span data-ttu-id="e7e46-118">Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="e7e46-118">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="e7e46-119">Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="e7e46-119">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="e7e46-120">En el menú del cliente, seleccione **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="e7e46-120">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="e7e46-121">Para cada usuario que agregue, seleccione **Agregar suscripción**y, a continuación, rellene la información, incluidos los permisos y las licencias.</span><span class="sxs-lookup"><span data-stu-id="e7e46-121">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="e7e46-122">Guarde los cambios mediante **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="e7e46-122">**Save** your changes.</span></span>

5. <span data-ttu-id="e7e46-123">Asegúrate de registrar el nombre de usuario y la contraseña temporal que enviarás al usuario.</span><span class="sxs-lookup"><span data-stu-id="e7e46-123">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="e7e46-124">Si va a agregar varios usuarios a la vez, use **Agregar otro usuario**.</span><span class="sxs-lookup"><span data-stu-id="e7e46-124">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="e7e46-125">También puede agregar varios usuarios a la vez [importando un archivo de hoja de cálculo. csv compatible con Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="e7e46-125">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="e7e46-126">Puede esperar hasta que termine con todo el conjunto antes de enviar un correo electrónico o imprimir los nombres y las contraseñas en la pantalla de confirmación.</span><span class="sxs-lookup"><span data-stu-id="e7e46-126">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="e7e46-127">Agregar o quitar licencias de usuario de un cliente</span><span class="sxs-lookup"><span data-stu-id="e7e46-127">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="e7e46-128">Los siguientes pasos se aplican a la adición o eliminación de licencias de usuario de productos de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e7e46-128">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="e7e46-129">Para agregar o quitar licencias de usuario para las suscripciones de SaaS basadas en licencias en Marketplace comercial, consulte [adición o eliminación de licencias para una suscripción de SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="e7e46-129">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="e7e46-130">Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="e7e46-130">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="e7e46-131">Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="e7e46-131">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="e7e46-132">En el menú del cliente, seleccione **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="e7e46-132">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="e7e46-133">Elige uno o varios usuarios de la lista.</span><span class="sxs-lookup"><span data-stu-id="e7e46-133">Choose one or more users from the list.</span></span> <span data-ttu-id="e7e46-134">Si, por ejemplo, el cliente acaba de adquirir nuevas licencias y quieres asignarlas a personas que aún no las tienen, puedes usar la opción **Filtrar usuarios por...** para buscar el grupo adecuado.</span><span class="sxs-lookup"><span data-stu-id="e7e46-134">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="e7e46-135">Selecciona **Administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="e7e46-135">Select **Manage licenses**.</span></span> <span data-ttu-id="e7e46-136">Realiza los cambios y haz clic en **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="e7e46-136">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="e7e46-137">En el caso de [los productos de Azure Marketplace](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), la asignación y activación de licencias se administra a través del proveedor de software independiente (ISV) que publicó el producto.</span><span class="sxs-lookup"><span data-stu-id="e7e46-137">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="e7e46-138">Restablecer la contraseña de un usuario de un cliente</span><span class="sxs-lookup"><span data-stu-id="e7e46-138">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="e7e46-139">Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="e7e46-139">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="e7e46-140">Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="e7e46-140">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3.  <span data-ttu-id="e7e46-141">En el menú del cliente, seleccione **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="e7e46-141">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="e7e46-142">Elija el usuario de la lista.</span><span class="sxs-lookup"><span data-stu-id="e7e46-142">Choose the user from the list.</span></span>

4.  <span data-ttu-id="e7e46-143">En la parte inferior de la pantalla, selecciona **Restablecer contraseña**.</span><span class="sxs-lookup"><span data-stu-id="e7e46-143">At the bottom of the screen, select **Reset password**.</span></span> 

5.  <span data-ttu-id="e7e46-144">Envía la nueva contraseña temporal al usuario.</span><span class="sxs-lookup"><span data-stu-id="e7e46-144">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="e7e46-145">Delete user accounts for a customer (Eliminar cuentas de usuario de un cliente)</span><span class="sxs-lookup"><span data-stu-id="e7e46-145">Delete user accounts for a customer</span></span>

1.  <span data-ttu-id="e7e46-146">En el menú del **centro de Partners** , seleccione **clientes**.</span><span class="sxs-lookup"><span data-stu-id="e7e46-146">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="e7e46-147">Elija el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="e7e46-147">Choose the customer from the list.</span></span>

2.  <span data-ttu-id="e7e46-148">En el menú del cliente, seleccione **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="e7e46-148">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="e7e46-149">Elija el usuario de la lista.</span><span class="sxs-lookup"><span data-stu-id="e7e46-149">Choose the user from the list.</span></span>

3.  <span data-ttu-id="e7e46-150">En la parte inferior de la pantalla, seleccione **Eliminar cuenta de usuario**.</span><span class="sxs-lookup"><span data-stu-id="e7e46-150">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="e7e46-151">Si tiene que restaurar esta cuenta, puede encontrarla en la pestaña **usuarios eliminados** de la lista de **usuarios y licencias** del cliente.</span><span class="sxs-lookup"><span data-stu-id="e7e46-151">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="e7e46-152">Tiene 30 días para restaurar un usuario eliminado.</span><span class="sxs-lookup"><span data-stu-id="e7e46-152">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="e7e46-153">Restaurar cuentas de usuario eliminadas</span><span class="sxs-lookup"><span data-stu-id="e7e46-153">Restore deleted user accounts</span></span>

1.  <span data-ttu-id="e7e46-154">En el menú del **centro de Partners** , seleccione **clientes**y, a continuación, elija el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="e7e46-154">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2.  <span data-ttu-id="e7e46-155">Seleccione **usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="e7e46-155">Select **Users and licenses**.</span></span>

3.  <span data-ttu-id="e7e46-156">Seleccione la pestaña **usuarios eliminados ()** . Debe leer **(1)** o superior cuando haya usuarios eliminados que se puedan restaurar.</span><span class="sxs-lookup"><span data-stu-id="e7e46-156">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4.  <span data-ttu-id="e7e46-157">Selecciona una o varias de las casillas de los usuarios eliminados y, a continuación, selecciona **Restaurar**.</span><span class="sxs-lookup"><span data-stu-id="e7e46-157">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="e7e46-158">Todas las cuentas de usuario seleccionadas volverán a aparecer en la página **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="e7e46-158">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="related-topics"></a><span data-ttu-id="e7e46-159">Temas relacionados</span><span class="sxs-lookup"><span data-stu-id="e7e46-159">Related topics</span></span>


[<span data-ttu-id="e7e46-160">Asignar o revocar licencias a varios usuarios</span><span class="sxs-lookup"><span data-stu-id="e7e46-160">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

[<span data-ttu-id="e7e46-161">Crear varios usuarios para una cuenta de cliente</span><span class="sxs-lookup"><span data-stu-id="e7e46-161">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)