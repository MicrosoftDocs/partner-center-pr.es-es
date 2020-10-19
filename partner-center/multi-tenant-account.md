---
title: Agregar inquilinos adicionales a la cuenta del centro de Partners
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprenda a agregar, consolidar o administrar varios inquilinos de Azure AD en su cuenta del centro de Partners. Obtenga información acerca de algunas de las razones por las que podría querer hacerlo.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175166"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Adición y administración de varios inquilinos en la cuenta del centro de Partners

**Se aplica a**

- Centro de partners

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

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="asociar inquilinos"::: 

5. Después de confirmar, verá una notificación de **todos los conjuntos** .  Seleccione **volver a administración de inquilinos** y verá el inquilino que se acaba de agregar. 
 

>[!NOTE]
>No se puede asociar un inquilino a una cuenta si ya está asociado a otra cuenta del centro de Partners.

 
## <a name="next-steps"></a>Pasos siguientes

- [Incorporación de usuarios](create-user-accounts-and-set-permissions.md)
