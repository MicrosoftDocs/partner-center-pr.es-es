---
title: Restablecer los privilegios de administrador del programa CSP de Azure
ms.topic: article
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo ayudar a los clientes a restablecer los privilegios de administrador de un partner para que pueda ayudar a administrar las suscripciones del programa CSP de Azure de un cliente.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 3bb1f5daf1582c4ca4a67c2813d598567db17f13
ms.sourcegitcommit: 7abdd277c0eea51237c97cbb163a4943fd740356
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/06/2020
ms.locfileid: "84467255"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Restablecer los privilegios de administrador para las suscripciones de del programa CSP de Azure de un cliente  

**Roles aplicables**

- Administrador global
- Agente de administrador

Como partner de CSP, tus clientes suelen esperar que administres el uso que hacen de Azure y sus sistemas por ellos. Para ello, es necesario tener privilegios de administrador. Algunos privilegios se conceden cuando se establece la relación de revendedor con el cliente. El cliente te concede otros privilegios.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilegios de administrador para Azure en CSP

Hay dos niveles de privilegios de administrador para Azure en CSP.

**Privilegios de administrador de nivel de inquilino** (**privilegios de administrador delegado**): los partners de CSP obtienen estos privilegios al establecer una relación de revendedor de CSP con los clientes. Esto proporciona a los partners de CSP acceso a los inquilinos de sus clientes, lo que les permite desarrollar funciones administrativas, como agregar o administrar usuarios, restablecer contraseñas y administrar licencias de usuario.

**Privilegios de administrador de nivel de suscripción**: los partners de CSP obtienen estos privilegios al crear suscripciones de Azure CSP para sus clientes. Estos privilegios proporcionan a los partners de CSP acceso completo a estas suscripciones, lo que les permite aprovisionar y administrar los recursos de Azure.

## <a name="reinstate-csp-partners-admin-privileges"></a>Restablecer los privilegios de administrador de los partners de CSP

Para recuperar los privilegios de administrador delegado, debes trabajar con el cliente.

1. Inicia sesión en el panel del Centro de partners y, en el menú del Centro de partners, selecciona **Clientes**.

2. Selecciona el cliente con el que estás trabajando y **solicita una relación de revendedor.** Esta acción genera un vínculo para el cliente que tiene derechos de administrador de inquilinos.

3. El usuario debe seleccionar el vínculo y aprobar la solicitud de relación del revendedor.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Relación de revendedor":::

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Adición del grupo de agentes de administrador como un propietario de la suscripción de Azure CSP

El cliente deberá agregar el grupo de agentes de administrador como el propietario de la suscripción de Azure CSP.

1. Usa la consola de PowerShell o el Entorno de scripting integrado (ISE) de PowerShell. Asegúrate de que los módulos AzureRM y AzureAD están instalados.

2. Conéctate a tu inquilino de Azure AD.

   ```powershell
   Connect-AzureAD
   ```

3. Obtén el ObjectId de los grupos de agentes de administrador.

   ```powershell
   Get-AzureADGroup
   ```

   :::image type="content" source="images/azure/revoke5.png" alt-text="Grupo de agentes de administrador":::

   El usuario realiza los pasos siguientes en la empresa del cliente que tiene acceso de propietario a la suscripción de Azure CSP.

4. La usuaria con acceso de propietario a la suscripción de Azure CSP inicia sesión en Azure Resource Manager con sus credenciales.

   ```powershell
   Login-AzureRMAccount
   ```

5. A continuación, puede agregar el grupo de agentes de administrador como propietaria a la suscripción de Azure de CSP.

    ```powershell
    New-AzureRMRoleAssignment -ObjectId <Object Id that you got from step 3> -RoleDefinitionName Owner -Scope "/subscriptions/<SubscriptionId of CSP subscription>"
    ```

   :::image type="content" source="images/azure/revoke6.png" alt-text="Propietarios de agentes de administrador":::

## <a name="next-steps"></a>Pasos siguientes

[Administrar suscripciones y recursos en el plan de Azure](azure-plan-manage.md)
