---
title: Agregar inquilinos a la cuenta Centro de partners cliente
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo agregar, consolidar o administrar varios inquilinos de Azure AD en su cuenta de Centro de partners y saber por qué podría querer hacerlo.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151209"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Adición y administración de varios inquilinos en la Centro de partners cuenta


**Roles adecuados:** administrador global | Administrador de cuenta

En este artículo se describe cómo consolidar varios inquilinos de Azure Active Directory (Azure AD) para su empresa y, a continuación, agregarlos y administrarlos en su cuenta Centro de partners cliente. Hay muchas razones para hacerlo. Por ejemplo:

- Supongamos que su empresa, Contoso, ha adquirido otra empresa, Fabrikam. Quiere que las dos empresas permanezcan independientes, pero quiere que los nuevos empleados puedan usar Centro de partners. En este caso, asociará el nuevo inquilino de Azure AD a su cuenta global de asociado (PGA). Esta asociación permite a los usuarios de ambas empresas trabajar en Centro de partners.

- Si ejecuta su negocio con más de un inquilino (por ejemplo, *contoso.com*, *contoso.uk* y *contoso.in*), puede usar multiinquilino para agruparlos en la misma cuenta de equipo.

- Si las directrices de fusiones y adquisiciones requieren que trabaje  con inquilinos de ambas compañías, usaría los inquilinos constoso.com y *fabrikam.com* inquilinos.

- Los usuarios de cualquiera de los inquilinos deben poder:
    * Acceso Centro de partners para entrenamiento, descargas digitales o asociación de Microsoft Certified Professional (MCP).
    * Se le Centro de partners roles como administrador de Microsoft Partner Network (MPN) o administrador de incentivos.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Adición de Azure AD inquilino a la cuenta

1. Inicie sesión como administrador global en [Microsoft Centro de partners](https://partner.microsoft.com/dashboard).

1. En la esquina superior derecha, seleccione **Configuración,** **Configuración de la cuenta** **y, después, Inquilinos.**
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Captura de pantalla del botón Asociar del panel Azure AD perfil."::: 

1. Seleccione **Asociar** y, a continuación, indique el inquilino que desea asociar.

1. En el símbolo del sistema, inicie sesión como administrador global en el inquilino que desea asociar y, a continuación, **seleccione Confirmar**. 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Captura de pantalla del botón Confirmar en el panel Confirmar Azure AD asociación."::: 

   Después de confirmar la asociación, se muestra **un mensaje** All set (Todo el conjunto). Para ver el inquilino recién agregado, seleccione **Volver a la administración de inquilinos.** 
 
>[!NOTE]
>No se puede asociar un inquilino a una cuenta si ya está asociada a otra cuenta Centro de partners cuenta.


## <a name="remove-a-tenant-from-your-account"></a>Eliminación de un inquilino de la cuenta
 
1. Inicie sesión como administrador global en [Microsoft Centro de partners](https://partner.microsoft.com/dashboard).

1. En la esquina superior derecha, seleccione el **icono Configuración** y, a continuación, seleccione Configuración de **la cuenta.**

1. En el panel izquierdo, seleccione **Inquilinos.** En **Administrar Azure AD inquilinos,** seleccione la pestaña Partner **(Asociado).**
 
1. Seleccione **Quitar** junto al inquilino cuya asociación desea quitar.

   :::image type="content" source="images/disassociate.png" alt-text="Captura de pantalla de las asociaciones de inquilino actuales y sus vínculos Quitar.":::

   Como se muestra en la  captura de pantalla anterior, los vínculos Quitar están habilitados para todos los inquilinos asociados, excepto para el inquilino principal y el inquilino en el que ha iniciado sesión actualmente. 

   > [!NOTE]   
   > Cuando se quita un inquilino, los usuarios de ese inquilino ya no tienen acceso a la cuenta de Centro de partners y la eliminación puede afectar a sus competencias. 

## <a name="next-steps"></a>Pasos siguientes

- [Crear cuentas de usuario](create-user-accounts-and-set-permissions.md)






