---
title: Agregar inquilinos a la cuenta del centro de Partners
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información acerca de cómo agregar, consolidar o administrar varios inquilinos de Azure AD en la cuenta del centro de Partners y obtener información sobre por qué podría querer hacerlo.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124812"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Adición y administración de varios inquilinos en la cuenta del centro de Partners


**Roles adecuados**

- Administrador global
- Administrador de cuentas

En este artículo se describe cómo consolidar varios inquilinos de Azure Active Directory (Azure AD) para su empresa y, a continuación, agregarlos y administrarlos en su cuenta del centro de Partners. Hay muchas razones para hacerlo. Por ejemplo:

- Supongamos que su empresa, Contoso, ha adquirido otra empresa, fabrikam. Quiere que las dos compañías sigan siendo independientes, pero desea que los nuevos empleados puedan usar el centro de Partners. En este caso, asociará el inquilino de Azure AD de la compañía a su cuenta global de socio comercial (PGA). Esta asociación permite a los usuarios de ambas empresas trabajar en el centro de Partners.

- Si ejecuta su empresa con más de un inquilino (por ejemplo, *contoso.com*, *contoso.uk* y *contoso.in*), puede usar la multiempresa para agruparlos en la misma cuenta de equipo.

- Si los mezcladores y las directrices de adquisiciones requieren que trabaje con los inquilinos de ambas empresas, usaría los inquilinos *constoso.com* y *fabrikam.com* .

- Los usuarios de cualquiera de los inquilinos deben poder:
    * Obtenga acceso al centro de partners para cursos, descargas digitales o asociación de Microsoft Certified Professional (MCP).
    * Debe tener asignados roles del centro de partners como el administrador de Microsoft Partner Network (MPN) o el administrador de incentivos.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Adición de un inquilino de Azure AD a su cuenta

1. Inicie sesión como administrador global en el [centro de Partners de Microsoft](https://partner.microsoft.com/dashboard).

1. En la esquina superior derecha, seleccione **configuración**, seleccione Configuración de la **cuenta** y, a continuación, seleccione **inquilinos**.
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Captura de pantalla del botón asociar en el panel Perfil de Azure AD."::: 

1. Seleccione **asociar** y, a continuación, indique el inquilino que desea asociar.

1. En el símbolo del sistema, inicie sesión como administrador global en el inquilino que desee asociar y, a continuación, seleccione **confirmar**. 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Captura de pantalla del botón confirmar en el panel confirmar nueva asociación de Azure AD."::: 

   Una vez confirmada la asociación, se muestra un mensaje **todo establecido** . Para ver el inquilino recién agregado, seleccione **volver a administración de inquilinos**. 
 
>[!NOTE]
>No se puede asociar un inquilino con una cuenta si ya está asociado a otra cuenta del centro de Partners.


## <a name="remove-a-tenant-from-your-account"></a>Quitar un inquilino de su cuenta
 
1. Inicie sesión como administrador global en el [centro de Partners de Microsoft](https://partner.microsoft.com/dashboard).

1. En la esquina superior derecha, seleccione el icono de **configuración** y, a continuación, seleccione Configuración de la **cuenta**.

1. En el panel izquierdo, seleccione **inquilinos**. En **administrar inquilinos de Azure ad**, seleccione la pestaña **socio comercial** .
 
1. Seleccione **quitar** junto al inquilino cuya asociación desea quitar.

   :::image type="content" source="images/disassociate.png" alt-text="Captura de pantalla de las asociaciones de inquilino actuales y sus vínculos de eliminación.":::

   Como se muestra en la captura de pantalla anterior, los vínculos de **eliminación** están habilitados para todos los inquilinos asociados, excepto para el inquilino principal y el inquilino en el que está conectado actualmente. 

   > [!NOTE]   
   > Cuando se quita un inquilino, los usuarios de ese inquilino ya no tienen acceso a la cuenta del centro de Partners y la eliminación puede afectar a sus competencias. 

## <a name="next-steps"></a>Pasos siguientes

- [Crear cuentas de usuario](create-user-accounts-and-set-permissions.md)






