---
title: Restablecer los privilegios de administrador del programa CSP de Azure
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo ayudar a los clientes a restablecer los privilegios de administrador de un partner para que pueda ayudar a administrar las suscripciones del programa CSP de Azure de un cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ad29283001ec542944da4f0cac835c6a5d339251
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855427"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Restablecer los privilegios de administrador para las suscripciones de del programa CSP de Azure de un cliente  

**Roles adecuados**: Administrador global | Agente de administración

Como partner de CSP, tus clientes suelen esperar que administres el uso que hacen de Azure y sus sistemas por ellos. Para ello, es necesario tener privilegios de administrador. Algunos privilegios se conceden cuando se establece la relación de revendedor con el cliente. El cliente te concede otros privilegios.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilegios de administrador para Azure en CSP

Hay dos niveles de privilegios de administrador para Azure en CSP.

**Privilegios de administrador de nivel de inquilino** (**privilegios de administrador delegado**): los partners de CSP obtienen estos privilegios al establecer una relación de revendedor de CSP con los clientes. Los privilegios de administrador delegado proporcionan a los partners de CSP acceso a los inquilinos de sus clientes, lo que les permite desarrollar funciones administrativas, como agregar o administrar usuarios, restablecer contraseñas y administrar licencias de usuario.

**Privilegios de administrador de nivel de suscripción**: los partners de CSP obtienen estos privilegios al crear suscripciones de Azure CSP para sus clientes. Estos privilegios proporcionan a los partners de CSP acceso completo a estas suscripciones, lo que les permite aprovisionar y administrar los recursos de Azure.

## <a name="reinstate-csp-partners-admin-privileges"></a>Restablecer los privilegios de administrador de los partners de CSP

El cliente puede volver a crear la asignación de roles de CSP siempre que se le proporcione el identificador de objeto del grupo AdminAgents. Para recuperar los privilegios de administrador delegado, debes trabajar con el cliente.

1. Inicie sesión en el panel del Centro de partners y, en el menú del Centro de partners, selecciona **Clientes**.

2. Selecciona el cliente con el que estás trabajando y **solicita una relación de revendedor.** Esta acción genera un vínculo para el cliente que tiene derechos de administrador de inquilinos.

3. El cliente debe seleccionar el vínculo y aprobar la solicitud de relación del revendedor.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Ejemplo de correo electrónico de creación de una relación de revendedor":::

4. El asociado, debe conectarse al inquilino del asociado para obtener el identificador de objeto del grupo AdminAgents.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. El cliente que tiene el rol de **propietario o administrador de acceso de usuarios** y tiene permiso para crear la asignación de roles en el nivel de suscripción hace lo siguiente:


    1. Se conecta al inquilino donde existe la suscripción de CSP.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Se conecta a la suscripción (solo es aplicable si el usuario tiene permisos de asignación de roles en varias suscripciones del inquilino).
   
         PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"


    3. Crea la asignación de roles.
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Si quiere conceder el permiso de rol de propietario a nivel del grupo de recursos o a nivel del recurso en lugar del ámbito de la suscripción, pueden funcionar los siguientes comandos:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Pasos siguientes

- [Administrar suscripciones y recursos en el plan de Azure](azure-plan-manage.md)
