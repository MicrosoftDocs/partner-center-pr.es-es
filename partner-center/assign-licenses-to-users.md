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
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Administración de usuarios y licencias de usuario para cuentas de cliente 

**Roles adecuados:** administrador global | Administrador de administración de | Agente de administración


Puede crear y eliminar nuevos usuarios en la cuenta de un cliente. También puede restaurar una o varias cuentas de usuario que eliminó anteriormente en un plazo de 30 días a partir de la eliminación. Las asignaciones anteriores de la suscripción del usuario también se restaurarán (suponiendo que sus asignaciones anteriores estén disponibles).

Al comprar nuevas suscripciones para un cliente, el cliente debe proporcionar una lista de todos los usuarios que necesitarán cuentas, sus permisos de usuario y qué servicios necesita cada usuario.  

>[!NOTE]
>La sección Usuarios y  licencias de la pestaña Cliente muestra todos los usuarios **creados** en el inquilino de un cliente específico, incluidos los usuarios que tienen licencias adquiridas a otro asociado de CSP o a otro canal de compra.

Puede asignar [suscripciones a varios usuarios](bulk-license-provisioning-for-multiple-users.md) a la vez importando los nombres mediante un archivo de hoja de cálculo [.csv compatible](adding-multiple-users-to-a-customer-account.md)con Excel .

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Crear cuentas de usuario para un cliente

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

2. Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.

3. En el menú del cliente, seleccione **Usuarios y licencias.**

4. Para cada usuario que agregue, seleccione **Agregar suscripción** y rellene la información, incluidos los permisos y las licencias. Guarde los cambios mediante **Guardar**.

5. Asegúrate de registrar el nombre de usuario y la contraseña temporal que enviarás al usuario.

6. Si va a agregar varios usuarios de uno en uno, use **Agregar otro usuario.**

7. También puede agregar varios usuarios a la vez [importando un archivo de hoja](adding-multiple-users-to-a-customer-account.md)de cálculo .csv compatible con Excel . Puede esperar hasta que haya terminado con todo el conjunto antes de enviar por correo electrónico o imprimir los nombres y contraseñas desde la pantalla de confirmación.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Agregar o quitar licencias de usuario de un cliente

Los pasos siguientes se aplican a la adición o eliminación de licencias de usuario para productos de Microsoft. Para agregar o quitar licencias de usuario para suscripciones de SaaS basadas en licencias en marketplace comercial, consulte Adición o eliminación de licencias [para una suscripción de SaaS.](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

2. Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.

3. En el menú del cliente, seleccione **Usuarios y licencias.**

4. Elige uno o varios usuarios de la lista. Si, por ejemplo, el cliente acaba de comprar nuevas licencias y quiere asignarlas a personas que aún no las tienen, puede usar la opción Filtrar usuarios **por...** para encontrar el grupo adecuado.

5. Selecciona **Administrar licencias**. Realice los cambios y, a **continuación, guarde**.

> [!NOTE]
> Para [Azure Marketplace,](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)la asignación de licencias y la activación se administran a través del proveedor de software independiente (ISV) que publicó el producto.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Restablecer la contraseña de un usuario de un cliente

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

2. Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.

3. En el menú del cliente, seleccione **Usuarios y licencias.** Elija el usuario de la lista.

4. En la parte inferior de la pantalla, selecciona **Restablecer contraseña**. 

5. Envía la nueva contraseña temporal al usuario.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Delete user accounts for a customer (Eliminar cuentas de usuario de un cliente)

1. En el **menú Centro de partners,** seleccione **Clientes.** Elija el cliente de la lista.

2. En el menú del cliente, seleccione **Usuarios y licencias.** Elija el usuario de la lista.

3. En la parte inferior de la pantalla, seleccione **Eliminar cuenta de usuario**.

Si necesita restaurar esta cuenta, puede encontrarla en la pestaña **Usuarios** **eliminados** de la lista Usuarios y licencias del cliente. Tiene 30 días para restaurar un usuario eliminado.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Restaurar cuentas de usuario eliminadas

1. En el **Centro de partners,** seleccione **Clientes** y, a continuación, elija el cliente de la lista.

2. Seleccione **Usuarios y licencias.**

3. Seleccione la **pestaña Usuarios eliminados ( ).** Debe leer **(1)** o superior cuando haya usuarios eliminados que se puedan restaurar.

4. Selecciona una o varias de las casillas de los usuarios eliminados y, a continuación, selecciona **Restaurar**.

    Todas las cuentas de usuario seleccionadas volverán a aparecer en la página **Usuarios y licencias**.

## <a name="next-steps"></a>Pasos siguientes

- [Asignar o revocar licencias a varios usuarios](bulk-license-provisioning-for-multiple-users.md)

- [Crear varios usuarios para una cuenta de cliente](adding-multiple-users-to-a-customer-account.md)