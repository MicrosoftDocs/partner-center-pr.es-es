---
title: Administrar usuarios para cuentas de cliente
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Administrar usuarios para sus clientes en el centro de Partners: crear cuentas de usuario, agregar o quitar licencias de usuario, restablecer contraseñas y eliminar o restaurar cuentas de usuario.'
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0e2bb4ceb146174da83e9c08a9ff030380298bd0
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756086"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="d0be0-103">Administrar usuarios y licencias de usuario para cuentas de cliente</span><span class="sxs-lookup"><span data-stu-id="d0be0-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="d0be0-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="d0be0-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d0be0-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d0be0-105">Global admin</span></span>
- <span data-ttu-id="d0be0-106">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="d0be0-106">User management admin</span></span>
- <span data-ttu-id="d0be0-107">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="d0be0-107">Admin agent</span></span>


<span data-ttu-id="d0be0-108">Puede crear y eliminar nuevos usuarios en la cuenta de un cliente.</span><span class="sxs-lookup"><span data-stu-id="d0be0-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="d0be0-109">También puede restaurar una o más cuentas de usuario que haya eliminado previamente en un plazo de 30 días a partir de la eliminación.</span><span class="sxs-lookup"><span data-stu-id="d0be0-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="d0be0-110">Las asignaciones anteriores de la suscripción del usuario también se restaurarán (suponiendo que sus asignaciones anteriores estén disponibles).</span><span class="sxs-lookup"><span data-stu-id="d0be0-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="d0be0-111">Al comprar nuevas suscripciones para un cliente, el cliente debe proporcionarle una lista de todos los usuarios que necesitarán cuentas, sus permisos de usuario y los servicios que necesite cada usuario.</span><span class="sxs-lookup"><span data-stu-id="d0be0-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="d0be0-112">La sección **usuarios y licencias** de la pestaña **cliente** muestra todos los usuarios creados en el inquilino de un cliente específico, incluidos los usuarios que tienen licencias adquiridas de otro asociado de CSP o de otro canal de compra.</span><span class="sxs-lookup"><span data-stu-id="d0be0-112">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="d0be0-113">Puede [asignar suscripciones a varios usuarios](bulk-license-provisioning-for-multiple-users.md) al mismo tiempo importando los nombres mediante un [archivo de hoja de cálculo. csv compatible con Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="d0be0-113">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="d0be0-114">Crear cuentas de usuario para un cliente</span><span class="sxs-lookup"><span data-stu-id="d0be0-114">Create user accounts for a customer</span></span>

1. <span data-ttu-id="d0be0-115">Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d0be0-115">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d0be0-116">Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="d0be0-116">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d0be0-117">En el menú del cliente, seleccione **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="d0be0-117">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="d0be0-118">Para cada usuario que agregue, seleccione **Agregar suscripción** y, a continuación, rellene la información, incluidos los permisos y las licencias.</span><span class="sxs-lookup"><span data-stu-id="d0be0-118">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="d0be0-119">Guarde los cambios mediante **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="d0be0-119">**Save** your changes.</span></span>

5. <span data-ttu-id="d0be0-120">Asegúrate de registrar el nombre de usuario y la contraseña temporal que enviarás al usuario.</span><span class="sxs-lookup"><span data-stu-id="d0be0-120">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="d0be0-121">Si va a agregar varios usuarios a la vez, use **Agregar otro usuario**.</span><span class="sxs-lookup"><span data-stu-id="d0be0-121">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="d0be0-122">También puede agregar varios usuarios a la vez [importando un archivo de hoja de cálculo. csv compatible con Excel](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="d0be0-122">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="d0be0-123">Puede esperar hasta que termine con todo el conjunto antes de enviar un correo electrónico o imprimir los nombres y las contraseñas en la pantalla de confirmación.</span><span class="sxs-lookup"><span data-stu-id="d0be0-123">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="d0be0-124">Agregar o quitar licencias de usuario de un cliente</span><span class="sxs-lookup"><span data-stu-id="d0be0-124">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="d0be0-125">Los siguientes pasos se aplican a la adición o eliminación de licencias de usuario de productos de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d0be0-125">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="d0be0-126">Para agregar o quitar licencias de usuario para las suscripciones de SaaS basadas en licencias en Marketplace comercial, consulte [adición o eliminación de licencias para una suscripción de SaaS](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span><span class="sxs-lookup"><span data-stu-id="d0be0-126">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="d0be0-127">Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d0be0-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d0be0-128">Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="d0be0-128">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d0be0-129">En el menú del cliente, seleccione **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="d0be0-129">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="d0be0-130">Elige uno o varios usuarios de la lista.</span><span class="sxs-lookup"><span data-stu-id="d0be0-130">Choose one or more users from the list.</span></span> <span data-ttu-id="d0be0-131">Si, por ejemplo, el cliente acaba de adquirir nuevas licencias y quieres asignarlas a personas que aún no las tienen, puedes usar la opción **Filtrar usuarios por...** para buscar el grupo adecuado.</span><span class="sxs-lookup"><span data-stu-id="d0be0-131">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="d0be0-132">Selecciona **Administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="d0be0-132">Select **Manage licenses**.</span></span> <span data-ttu-id="d0be0-133">Realiza los cambios y haz clic en **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="d0be0-133">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="d0be0-134">En el caso de [los productos de Azure Marketplace](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), la asignación y activación de licencias se administra a través del proveedor de software independiente (ISV) que publicó el producto.</span><span class="sxs-lookup"><span data-stu-id="d0be0-134">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="d0be0-135">Restablecer la contraseña de un usuario de un cliente</span><span class="sxs-lookup"><span data-stu-id="d0be0-135">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="d0be0-136">Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d0be0-136">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="d0be0-137">Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="d0be0-137">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="d0be0-138">En el menú del cliente, seleccione **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="d0be0-138">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="d0be0-139">Elija el usuario de la lista.</span><span class="sxs-lookup"><span data-stu-id="d0be0-139">Choose the user from the list.</span></span>

4. <span data-ttu-id="d0be0-140">En la parte inferior de la pantalla, selecciona **Restablecer contraseña**.</span><span class="sxs-lookup"><span data-stu-id="d0be0-140">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="d0be0-141">Envía la nueva contraseña temporal al usuario.</span><span class="sxs-lookup"><span data-stu-id="d0be0-141">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="d0be0-142">Delete user accounts for a customer (Eliminar cuentas de usuario de un cliente)</span><span class="sxs-lookup"><span data-stu-id="d0be0-142">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="d0be0-143">En el menú del **centro de Partners** , seleccione **clientes**.</span><span class="sxs-lookup"><span data-stu-id="d0be0-143">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="d0be0-144">Elija el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="d0be0-144">Choose the customer from the list.</span></span>

2. <span data-ttu-id="d0be0-145">En el menú del cliente, seleccione **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="d0be0-145">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="d0be0-146">Elija el usuario de la lista.</span><span class="sxs-lookup"><span data-stu-id="d0be0-146">Choose the user from the list.</span></span>

3. <span data-ttu-id="d0be0-147">En la parte inferior de la pantalla, seleccione **Eliminar cuenta de usuario**.</span><span class="sxs-lookup"><span data-stu-id="d0be0-147">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="d0be0-148">Si tiene que restaurar esta cuenta, puede encontrarla en la pestaña **usuarios eliminados** de la lista de **usuarios y licencias** del cliente.</span><span class="sxs-lookup"><span data-stu-id="d0be0-148">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="d0be0-149">Tiene 30 días para restaurar un usuario eliminado.</span><span class="sxs-lookup"><span data-stu-id="d0be0-149">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="d0be0-150">Restaurar cuentas de usuario eliminadas</span><span class="sxs-lookup"><span data-stu-id="d0be0-150">Restore deleted user accounts</span></span>

1. <span data-ttu-id="d0be0-151">En el menú del **centro de Partners** , seleccione **clientes** y, a continuación, elija el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="d0be0-151">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="d0be0-152">Seleccione **usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="d0be0-152">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="d0be0-153">Seleccione la pestaña **usuarios eliminados ()** . Debe leer **(1)** o superior cuando haya usuarios eliminados que se puedan restaurar.</span><span class="sxs-lookup"><span data-stu-id="d0be0-153">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="d0be0-154">Selecciona una o varias de las casillas de los usuarios eliminados y, a continuación, selecciona **Restaurar**.</span><span class="sxs-lookup"><span data-stu-id="d0be0-154">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="d0be0-155">Todas las cuentas de usuario seleccionadas volverán a aparecer en la página **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="d0be0-155">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d0be0-156">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d0be0-156">Next steps</span></span>

- [<span data-ttu-id="d0be0-157">Asignar o revocar licencias a varios usuarios</span><span class="sxs-lookup"><span data-stu-id="d0be0-157">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="d0be0-158">Crear varios usuarios para una cuenta de cliente</span><span class="sxs-lookup"><span data-stu-id="d0be0-158">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)