---
title: Restablecer los privilegios de administrador del programa CSP de Azure
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo ayudar a los clientes a restablecer los privilegios de administrador de un partner para que pueda ayudar a administrar las suscripciones del programa Proveedor de soluciones en la nube (CSP) de Azure de un cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 5d784aef33cce2a722583a77e73c35d5fc8136b1
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551595"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Restablecer los privilegios de administrador para las suscripciones de del programa CSP de Azure de un cliente  

**Roles adecuados**: Administrador global | Agente de administración

Como partner del programa Proveedor de soluciones en la nube (CSP), sus clientes suelen esperar que administre el uso que hacen de Azure y sus sistemas por ellos. Debe tener privilegios de administrador para hacerlo. Algunos privilegios se conceden cuando se establece la relación de revendedor con el cliente. El cliente te concede otros privilegios.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilegios de administrador para Azure en CSP

Hay dos niveles de privilegios de administrador para Azure en CSP.

- **Privilegios de administrador de nivel de inquilino (privilegios de administrador delegado)** : los partners de CSP obtienen estos privilegios al establecer una relación de revendedor de CSP con los clientes. Los privilegios de administrador delegados proporcionan a los partners de CSP acceso a los inquilinos de sus clientes. Este acceso les permite realizar funciones administrativas, como agregar o administrar usuarios, restablecer contraseñas y administrar licencias de usuario.
- **Privilegios de administrador de nivel de suscripción**: los partners de CSP obtienen estos privilegios al crear suscripciones de CSP de Azure para sus clientes. Estos privilegios proporcionan a los partners de CSP acceso completo a estas suscripciones, lo que les permite aprovisionar y administrar los recursos de Azure.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>Restablecer los privilegios de administrador de un partner en CSP

El cliente puede volver a crear la asignación de roles de CSP siempre que se le proporcione el identificador `object ID` del grupo AdminAgents. Para recuperar los privilegios de administrador delegado, debe trabajar con el cliente y completar los pasos que se indican a continuación.

1. Inicia sesión en el panel del Centro de partners.

2. En el menú del Centro de partners, seleccione **Clientes**.

3. Seleccione el cliente con el que está trabajando y **solicite una relación de revendedor**. Esta acción genera un vínculo para el cliente que tiene derechos de administrador de inquilinos.

4. El cliente debe seleccionar el vínculo y aprobar la solicitud de relación de revendedor.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Ejemplo de correo electrónico de creación de una relación de revendedor.":::

5. El asociado, debe conectarse al inquilino del asociado para obtener el identificador de objeto del grupo AdminAgents.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. A continuación, el cliente debe realizar los pasos siguientes mediante PowerShell o la CLI de Azure. El cliente debe tener lo siguiente:

- El rol de **propietario** o **administrador de acceso de usuario**. 
- Permisos para crear asignaciones de roles en el nivel de suscripción.

   a. Solo para PowerShell, el cliente debe actualizar el módulo `Az.Resources`.
   ```powershell
   Update-Module Az.Resources
   ```

   b. El cliente se conecta al inquilino donde existe la suscripción de CSP.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. El cliente se conecta a la suscripción. Este paso *solo* es aplicable si el usuario tiene permisos de asignación de roles en varias suscripciones del inquilino.

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. A continuación, el cliente crea la asignación de roles.
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

En lugar de conceder permisos de propietario en el ámbito de la suscripción, puede concederlos en el nivel de recurso o de grupo de recursos. 

- En el nivel de grupo de recursos

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- En el nivel de recurso

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

Si los pasos anteriores no funcionan o se producen errores al intentarlos, pruebe el siguiente procedimiento "comodín" para restablecer los derechos de administrador del cliente.

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>Solución de problemas

Si el cliente no puede completar el paso 6 anterior, indíquele que pruebe el siguiente comando:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Proporcione el archivo `newRoleAssignment.log` resultante a Microsoft para su posterior análisis.

Si se produce un error en el procedimiento "comodín" durante la ejecución de `Import-Module`, pruebe los pasos siguientes:
- Si se produce un error en la importación porque el módulo está en uso, cierre y vuelva a abrir todas las ventanas para reiniciar la sesión de PowerShell.
- Compruebe la versión de `Az.Resources` con `Get-Module Az.Resources -ListAvailable`.
- Si la versión 4.1.1 no está en la lista disponible, debe usar `Update-Module Az.Resources -Force`.
- Si el error indica que `Az.Accounts` debe ser de una versión específica, actualice también ese módulo y reemplace `Az.Resources` por `Az.Accounts`. A continuación, debe reiniciar la sesión de PowerShell.


## <a name="next-steps"></a>Pasos siguientes

- [Administrar suscripciones y recursos en el plan de Azure](azure-plan-manage.md)
