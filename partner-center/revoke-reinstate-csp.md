---
title: Restablecer los privilegios de administrador para las suscripciones de Azure CSP | Centro de partners
ms.topic: article
ms.date: 10/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: En este documento se explica cómo ayudar a los clientes a restablecer los privilegios de administrador de los partners.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.openlocfilehash: 1bcbcf32e3b3f4513ed3e55984b49b090da4a734
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2020
ms.locfileid: "73651706"
---
# <a name="reinstate-admin-privileges-for-azure-csp-subscriptions"></a>Restablecer los privilegios de administrador para las suscripciones de Azure CSP  

**Roles aplicables**

- Administrador global
- Agente de administrador

Como partner de CSP, tus clientes suelen esperar que administres el uso que hacen de Azure y sus sistemas por ellos. Para ello, es necesario disponer de privilegios de administrador. Algunos privilegios se conceden cuando se establece la relación de revendedor con el cliente. El cliente te concede otros privilegios.

## <a name="admin-privileges-for-azure-in-csp"></a>Privilegios de administrador para Azure en CSP 

Hay dos niveles de privilegios de administrador para Azure en CSP. 

**Privilegios de administrador de nivel de inquilino** (**privilegios de administrador delegado**): los partners de CSP obtienen estos privilegios al establecer una relación de revendedor de CSP con los clientes. Esto proporciona a los partners de CSP acceso a los inquilinos de sus clientes, lo que les permite desarrollar funciones administrativas, como agregar o administrar usuarios, restablecer contraseñas y administrar licencias de usuario. 

**Privilegios de administrador de nivel de suscripción**: los partners de CSP obtienen estos privilegios al crear suscripciones de Azure CSP para sus clientes. Esto proporciona a los partners de CSP acceso completo a estas suscripciones, lo que les permite aprovisionar y administrar los recursos de Azure. 


## <a name="reinstate-csp-partners-admin-privileges"></a>Restablecer los privilegios de administrador de los partners de CSP

Para recuperar los privilegios de administrador delegado, debes trabajar con el cliente.
 
 1. Inicia sesión en el panel del Centro de partners y, en el menú del Centro de partners, selecciona **Clientes**.

 2. Selecciona el cliente con el que estás trabajando y **solicita una relación de revendedor.** Esta acción genera un vínculo para el cliente que tiene derechos de administrador de inquilinos.

 3. El usuario debe seleccionar el vínculo y aprobar la solicitud de relación del revendedor.
 
![relación de revendedor](images/azure/revoke4.png)

## <a name="adding-the-admin-agents-group-as-an-owner-for-the-azure-csp-subscription"></a>Adición del grupo de agentes de administrador como un propietario de la suscripción de Azure CSP

 El cliente deberá agregar el grupo de agentes de administrador como el propietario de la suscripción de Azure CSP.

1. Usa la consola de PowerShell o el Entorno de scripting integrado (ISE) de PowerShell. Asegúrate de que los módulos AzureRM y AzureAD están instalados. 

2.  Conéctate a tu inquilino de Azure AD.
Cmdlet de PowerShell: Connect-AzureAD

3.  Obtén el ObjectId de los grupos de agentes de administrador.
Cmdlet de PowerShell: Get-AzureADGroup`1nn

![grupo de agentes de administrador](images/azure/revoke5.png)

El usuario realiza los pasos siguientes en la empresa del cliente que tiene acceso de propietario a la suscripción de Azure CSP.

4. La usuaria con acceso de propietario a la suscripción de Azure CSP inicia sesión en Azure Resource Manager con sus credenciales.

    Cmdlet de PowerShell: Login-AzureRMAccount

5.  A continuación, puede agregar el grupo de agentes de administrador como propietaria a la suscripción de Azure de CSP.

    Cmdlet de PowerShell: New-AzureRMRoleAssignment-ObjectId <id. del objeto que recibió en el paso 3>-RoleDefinitionName-Scope "/subscriptions/<SubscriptionId of CSP subscription>"

![propietarios de agentes de administrador](images/azure/revoke6.png)    

**Para más información**

[Administrar suscripciones y recursos en el plan de Azure](azure-plan-manage.md)
