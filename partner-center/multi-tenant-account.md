---
title: Agregar inquilinos adicionales a la cuenta del centro de Partners
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprenda a agregar, consolidar o administrar varios inquilinos de Azure AD en su cuenta del centro de Partners. Obtenga información acerca de algunas de las razones por las que podría querer hacerlo.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 22f85bda0a651559da1717ae1e5365da40d62aff
ms.sourcegitcommit: 8cb98de420f6ab5bb4cb3efc9007262c4d7d3327
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/12/2021
ms.locfileid: "98105563"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Adición y administración de varios inquilinos en la cuenta del centro de Partners


**Roles adecuados**

- Administrador global

Esta característica le permite administrar varios inquilinos para su empresa y consolidarlos en su cuenta del Centro de partners. Hay muchas razones por las que puede que tenga que administrar varios inquilinos de Azure AD en la cuenta del centro de Partners. Por ejemplo:

- Su empresa puede comprar otra empresa y quiere que los empleados de la nueva empresa puedan usar el centro de Partners. Sin embargo, desea que las dos compañías sigan siendo independientes. En este caso, debe asociar el inquilino de Azure AD de la compañía a su cuenta global de socio comercial (PGA). Esta asociación permitiría a los usuarios de ambas empresas trabajar en el centro de Partners.

- Si tiene más de un inquilino para ejecutar su empresa (por ejemplo, contoso.com, contoso.uk, contoso.in), puede usar multiinquilino para asociarlos con la misma cuenta de equipo.

- Las fusiones y adquisiciones requieren que trabaje con más de un inquilino (por ejemplo, si Contoso adquiere Fabrikam, deberá poder usar los inquilinos respectivos Constoso.com y Fabrikam.com).

- Los usuarios de cualquiera de los inquilinos necesitarán poder:
    1.  Centro de Partners de acceso para cursos, descargas digitales, Asociación de MCP
    2.  Debe tener asignados roles del centro de partners como el administrador de MPN, el administrador de incentivos, etc.


## <a name="add-another-azure-ad-tenant-to-your-account"></a>Agregar otro inquilino de Azure AD a su cuenta

1. Como administrador global, inicie sesión en el [Panel](https://partner.microsoft.com/dashboard)del centro de Partners.
1. En el icono de **configuración** , seleccione Configuración de la **cuenta** y, a continuación, seleccione **inquilinos**.
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="asociar inquilinos"::: 

3. Seleccione **asociar otro inquilino de ad** e indique el inquilino que quiere asociar.

1. Como administrador global, inicie sesión en el inquilino que desee asociar y confirme la asociación. 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="confirmar los inquilinos asociados"::: 

5. Después de confirmar, verá una notificación de **todos los conjuntos** .  Seleccione **volver a administración de inquilinos** y verá el inquilino recién agregado en la lista. 
 

>[!NOTE]
>No se puede asociar un inquilino a una cuenta si ya está asociado a otra cuenta del centro de Partners.


## <a name="remove-a-tenant-from-your-account"></a>Quitar un inquilino de su cuenta
 
1. Como administrador global, inicie sesión en el [Panel](https://partner.microsoft.com/dashboard)del centro de Partners.

1. En el icono de **configuración** , seleccione Configuración de la **cuenta** -> inquilinos y haga clic en la pestaña **socio comercial** .
 
3. Haga clic en **quitar** para el inquilino que desea desasociar.

4. La desasociación de un inquilino significa que los usuarios de ese inquilino ya no tendrán acceso a la cuenta del centro de Partners y esto podría tener un impacto en sus competencias. 

El botón **quitar** está habilitado para todos los inquilinos asociados, excepto el inquilino principal y el inquilino en el que ha iniciado sesión actualmente.

:::image type="content" source="images/disassociate.png" alt-text="inquilinos con el botón Quitar":::
 

## <a name="next-steps"></a>Pasos siguientes

- [Incorporación de usuarios](create-user-accounts-and-set-permissions.md)






