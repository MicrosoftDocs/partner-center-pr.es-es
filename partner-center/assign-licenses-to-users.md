---
title: Administración de usuarios para cuentas de cliente
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Administrar usuarios para los clientes de Centro de partners: crear cuentas de usuario, agregar o quitar licencias de usuario, restablecer contraseñas y eliminar o restaurar cuentas de usuario.'
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc896ec3ce16ab0f05a8131de14f573ad96a8141
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149900"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="bc2f9-103">Administración de usuarios y licencias de usuario para cuentas de cliente</span><span class="sxs-lookup"><span data-stu-id="bc2f9-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="bc2f9-104">**Roles adecuados:** administrador global | Administrador de administración de | Agente de administración</span><span class="sxs-lookup"><span data-stu-id="bc2f9-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>


<span data-ttu-id="bc2f9-105">Puede crear y eliminar nuevos usuarios en la cuenta de un cliente.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-105">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="bc2f9-106">También puede restaurar una o varias cuentas de usuario que eliminó anteriormente en un plazo de 30 días a partir de la eliminación.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-106">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="bc2f9-107">Las asignaciones anteriores de la suscripción del usuario también se restaurarán (suponiendo que sus asignaciones anteriores estén disponibles).</span><span class="sxs-lookup"><span data-stu-id="bc2f9-107">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="bc2f9-108">Al comprar nuevas suscripciones para un cliente, el cliente debe proporcionar una lista de todos los usuarios que necesitarán cuentas, sus permisos de usuario y qué servicios necesita cada usuario.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-108">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="bc2f9-109">La sección Usuarios y  licencias de la pestaña Cliente muestra todos los usuarios **creados** en el inquilino de un cliente específico, incluidos los usuarios que tienen licencias adquiridas a otro asociado de CSP o a otro canal de compra.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-109">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="bc2f9-110">Puede asignar [suscripciones a varios usuarios](bulk-license-provisioning-for-multiple-users.md) a la vez importando los nombres mediante un archivo de hoja de cálculo [.csv compatible](adding-multiple-users-to-a-customer-account.md)con Excel .</span><span class="sxs-lookup"><span data-stu-id="bc2f9-110">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="bc2f9-111">Crear cuentas de usuario para un cliente</span><span class="sxs-lookup"><span data-stu-id="bc2f9-111">Create user accounts for a customer</span></span>

1. <span data-ttu-id="bc2f9-112">Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-112">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="bc2f9-113">Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-113">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="bc2f9-114">En el menú del cliente, seleccione **Usuarios y licencias.**</span><span class="sxs-lookup"><span data-stu-id="bc2f9-114">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="bc2f9-115">Para cada usuario que agregue, seleccione **Agregar suscripción** y rellene la información, incluidos los permisos y las licencias.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-115">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="bc2f9-116">Guarde los cambios mediante **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-116">**Save** your changes.</span></span>

5. <span data-ttu-id="bc2f9-117">Asegúrate de registrar el nombre de usuario y la contraseña temporal que enviarás al usuario.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-117">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="bc2f9-118">Si va a agregar varios usuarios de uno en uno, use **Agregar otro usuario.**</span><span class="sxs-lookup"><span data-stu-id="bc2f9-118">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="bc2f9-119">También puede agregar varios usuarios a la vez [importando un archivo de hoja](adding-multiple-users-to-a-customer-account.md)de cálculo .csv compatible con Excel .</span><span class="sxs-lookup"><span data-stu-id="bc2f9-119">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="bc2f9-120">Puede esperar hasta que haya terminado con todo el conjunto antes de enviar por correo electrónico o imprimir los nombres y contraseñas desde la pantalla de confirmación.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-120">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="bc2f9-121">Agregar o quitar licencias de usuario de un cliente</span><span class="sxs-lookup"><span data-stu-id="bc2f9-121">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="bc2f9-122">Los pasos siguientes se aplican a la adición o eliminación de licencias de usuario para productos de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-122">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="bc2f9-123">Para agregar o quitar licencias de usuario para suscripciones de SaaS basadas en licencias en marketplace comercial, consulte Adición o eliminación de licencias [para una suscripción de SaaS.](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)</span><span class="sxs-lookup"><span data-stu-id="bc2f9-123">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="bc2f9-124">Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-124">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="bc2f9-125">Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-125">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="bc2f9-126">En el menú del cliente, seleccione **Usuarios y licencias.**</span><span class="sxs-lookup"><span data-stu-id="bc2f9-126">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="bc2f9-127">Elige uno o varios usuarios de la lista.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-127">Choose one or more users from the list.</span></span> <span data-ttu-id="bc2f9-128">Si, por ejemplo, el cliente acaba de comprar nuevas licencias y quiere asignarlas a personas que aún no las tienen, puede usar la opción Filtrar usuarios **por...** para encontrar el grupo adecuado.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-128">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="bc2f9-129">Selecciona **Administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-129">Select **Manage licenses**.</span></span> <span data-ttu-id="bc2f9-130">Realice los cambios y, a **continuación, guarde**.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-130">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="bc2f9-131">Para [Azure Marketplace,](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)la asignación de licencias y la activación se administran a través del proveedor de software independiente (ISV) que publicó el producto.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-131">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="bc2f9-132">Restablecer la contraseña de un usuario de un cliente</span><span class="sxs-lookup"><span data-stu-id="bc2f9-132">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="bc2f9-133">Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-133">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="bc2f9-134">Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-134">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="bc2f9-135">En el menú del cliente, seleccione **Usuarios y licencias.**</span><span class="sxs-lookup"><span data-stu-id="bc2f9-135">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="bc2f9-136">Elija el usuario de la lista.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-136">Choose the user from the list.</span></span>

4. <span data-ttu-id="bc2f9-137">En la parte inferior de la pantalla, selecciona **Restablecer contraseña**.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-137">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="bc2f9-138">Envía la nueva contraseña temporal al usuario.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-138">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="bc2f9-139">Delete user accounts for a customer (Eliminar cuentas de usuario de un cliente)</span><span class="sxs-lookup"><span data-stu-id="bc2f9-139">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="bc2f9-140">En el **menú Centro de partners,** seleccione **Clientes.**</span><span class="sxs-lookup"><span data-stu-id="bc2f9-140">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="bc2f9-141">Elija el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-141">Choose the customer from the list.</span></span>

2. <span data-ttu-id="bc2f9-142">En el menú del cliente, seleccione **Usuarios y licencias.**</span><span class="sxs-lookup"><span data-stu-id="bc2f9-142">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="bc2f9-143">Elija el usuario de la lista.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-143">Choose the user from the list.</span></span>

3. <span data-ttu-id="bc2f9-144">En la parte inferior de la pantalla, seleccione **Eliminar cuenta de usuario**.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-144">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="bc2f9-145">Si necesita restaurar esta cuenta, puede encontrarla en la pestaña **Usuarios** **eliminados** de la lista Usuarios y licencias del cliente.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-145">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="bc2f9-146">Tiene 30 días para restaurar un usuario eliminado.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-146">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="bc2f9-147">Restaurar cuentas de usuario eliminadas</span><span class="sxs-lookup"><span data-stu-id="bc2f9-147">Restore deleted user accounts</span></span>

1. <span data-ttu-id="bc2f9-148">En el **Centro de partners,** seleccione **Clientes** y, a continuación, elija el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-148">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="bc2f9-149">Seleccione **Usuarios y licencias.**</span><span class="sxs-lookup"><span data-stu-id="bc2f9-149">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="bc2f9-150">Seleccione la **pestaña Usuarios eliminados ( ).** Debe leer **(1)** o superior cuando haya usuarios eliminados que se puedan restaurar.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-150">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="bc2f9-151">Selecciona una o varias de las casillas de los usuarios eliminados y, a continuación, selecciona **Restaurar**.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-151">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="bc2f9-152">Todas las cuentas de usuario seleccionadas volverán a aparecer en la página **Usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="bc2f9-152">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="bc2f9-153">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="bc2f9-153">Next steps</span></span>

- [<span data-ttu-id="bc2f9-154">Asignar o revocar licencias a varios usuarios</span><span class="sxs-lookup"><span data-stu-id="bc2f9-154">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="bc2f9-155">Crear varios usuarios para una cuenta de cliente</span><span class="sxs-lookup"><span data-stu-id="bc2f9-155">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)