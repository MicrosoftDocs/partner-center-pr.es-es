---
title: Configurar los usuarios con la autenticación multifactor
ms.topic: how-to
ms.date: 10/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Obtenga información sobre cómo configurar a los empleados con MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 5e31fe8f65d8d676b7e0745f7747865493bbe3ee
ms.sourcegitcommit: 4a88db7e9e90b4fbb2ba82af38d7f77b016977f3
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/24/2020
ms.locfileid: "92526010"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Configurar los usuarios con la autenticación multifactor

**Roles adecuados**

- Administrador global

Una mayor seguridad y protección de la privacidad se encuentran entre nuestras principales prioridades. Sabemos que la mejor defensa es la prevención y que somos tan seguros como lo sea nuestro vínculo más débil. Esta es la razón por la que necesitamos que todos los usuarios de nuestro ecosistema actúen y se aseguren de tener las protecciones de seguridad adecuadas. Para ayudar a proteger a los partners y clientes, presentamos un conjunto de requisitos de seguridad obligatorios para los asesores, proveedores de panel de control y asociados que participen en el programa Proveedor de soluciones en la nube.

Los partners tienen la obligación de aplicar la autenticación multifactor (MFA) a todas las cuentas de usuario en su inquilino de partner. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Adición de la autenticación multifactor para los usuarios

Debe ser el administrador global de su empresa para poder completar esta tarea.

Es más fácil habilitar la MFA para los usuarios a medida que los agrega a su inquilino de Azure AD.

1. Inicie sesión en [Azure Portal](https://portal.azure.com) y, a continuación, vaya a **Administración de usuarios** .
1. Seleccione **Autenticación multifactor** .
1. Seleccione el usuario que desea habilitar y, a continuación, seleccione **Habilitar** .

Esto habilitará la MFA para este usuario. Estar habilitado significa que al usuario se le pedirá que configure la comprobación de MFA cuando inicie sesión por primera vez. A partir de ese momento, al iniciar sesión, se le pedirá que proporcione un código que se le enviará por correo electrónico o mensaje de texto.  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Especificación de cómo comprobar":::

Para obligar a los usuarios a usar MFA, puede **aplicar** siguiendo los mismos pasos descritos anteriormente y seleccionar **Forzar** . Para obtener más información, lea [Habilitación de Azure Multi-Factor Authentication por usuario para proteger los eventos de inicio de sesión](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates). 

Todos los usuarios comienzan con un estado  **Deshabilitado** . Cuando inscribe usuarios en Azure Multi-Factor Authentication por usuario, su estado cambia a  **Habilitado** . Cuando los usuarios habilitados inician sesión y completan el proceso de registro, su estado cambia a  **Forzado** . 

## <a name="next-steps"></a>Pasos siguientes

- [Asignación de roles y permisos a los usuarios](permissions-overview.md)



