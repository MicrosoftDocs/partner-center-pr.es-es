---
title: Agregar inquilinos adicionales a la cuenta del centro de Partners
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Administrar varios inquilinos a través de la cuenta del centro de Partners
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf9399f23153f25f319e399c9c327515cd9ed51
ms.sourcegitcommit: 583c792d904cc1b15eda9217a1f21f434564c8e7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/29/2020
ms.locfileid: "87389532"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Adición y administración de varios inquilinos en la cuenta del centro de Partners

**Se aplica a**

- Centro de partners

**Roles adecuados**

- Administrador global

Hay muchas razones por las que puede que tenga que administrar varios inquilinos de Azure AD en la cuenta del centro de Partners. Por ejemplo, su empresa puede comprar otra empresa y desea que los empleados de la nueva empresa puedan usar el centro de Partners. Sin embargo, desea que las dos compañías sigan siendo independientes. En este caso, debe asociar el inquilino de Azure AD de la compañía a la cuenta global (PNG) del asociado. Esta asociación permitiría a los usuarios de ambas empresas trabajar en el centro de Partners.

## <a name="add-another-azure-ad-tenant-to-your-account"></a>Agregar otro inquilino de Azure AD a su cuenta

1. Como administrador global, inicie sesión en el [Panel](https://partner.microsoft.com/dashboard)del centro de Partners.
1. En el icono de **configuración** , seleccione Configuración de la **cuenta** y, a continuación, seleccione **inquilinos**.
 
:::image type="content" source="images/merge-accounts/multitenant.png" alt-text="asociar inquilinos"::: 

3. Seleccione **asociar otro inquilino de ad** e indique el inquilino que quiere asociar.

1. Como administrador global, inicie sesión en el inquilino que desee asociar y confirme la asociación. 

:::image type="content" source="images/merge-accounts/multitenant2.png" alt-text="confirmar los inquilinos asociados"::: 

5. Después de confirmar, verá una notificación de **todos los conjuntos** .  Seleccione **volver a administración de inquilinos** y verá el inquilino que se acaba de agregar.
 
## <a name="next-steps"></a>Pasos siguientes

- [Incorporación de usuarios](create-user-accounts-and-set-permissions.md)
