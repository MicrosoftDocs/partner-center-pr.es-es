---
title: ¿Qué hacer si el único administrador del programa MPN ha dejado la empresa?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre qué hacer para encontrar un nuevo administrador de MPN u obtener ayuda del administrador global de su empresa. Además, obtenga información sobre cómo agregar un nuevo administrador Centro de partners global.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21042169a33d9a413f17f951c4daad0c5fc86a17
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277681"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>¿Qué hacer si el único administrador del programa MPN ha dejado la empresa?

**Roles adecuados:** administrador de asociados de MPN | Administrador de cuenta | Administrador global

El siguiente artículo le guía por tres escenarios típicos relacionados con lo que debe hacer si el administrador de MPN ha dejado la empresa.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Escenario 1: Administrador de asociados de MPN/Administrador de cuentas ha dejado la empresa, pero todavía hay administradores globales en la cuenta.

En este caso, a otra persona de la empresa se le puede asignar el rol de administrador de asociados de MPN. Para que se le asigne el rol de administrador de asociados de MPN específico o de administrador de cuenta:

1. Inicie sesión en Centro de partners cuenta con su cuenta de trabajo (por ejemplo, tom@contoso.com ).
1. En la **página Administración de** usuarios, filtre por Administrador global para ver quiénes son los administradores globales de su empresa. 
1. Póngase en contacto con uno de los administradores globales y pídale que le asigne el rol específico de MPN que necesita. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Escenario 2: Administrador de asociados de MPN/Administrador de cuentas ha dejado la empresa y no hay administradores globales en la cuenta. 

Si va a  la página Administración de usuarios y filtra por Administrador global, pero descubre que no hay ningún administrador global en su empresa que pueda ayudarle a obtener el rol específico de MPN, siga estos pasos:

1. Vaya a [portal.azure.com](https://ms.portal.azure.com/), inicie sesión con su cuenta de trabajo (por ejemplo, tom@contoso.com ). 
1. Seleccione la opción **Ayuda y soporte técnico** en la barra de navegación del menú izquierdo.
1. En la página siguiente, seleccione Nuevo  **Support Request** tipo de problema técnico en el menú desplegable, inserte los detalles adicionales y haga clic en **Siguiente: Soluciones.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Busque admin en Azure Portal.":::

4. Después de revisar las soluciones recomendadas en la página siguiente, seleccione **Siguiente: Detalles** y complete los campos necesarios.
1. Revise y cree la solicitud de soporte técnico.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Escenario 3: El administrador de asociados de MPN, el administrador de cuentas o el administrador global han dejado la empresa y no hay otros usuarios que puedan acceder a los servicios de la Azure AD. Se trata de una pérdida completa de acceso.

Siga los [pasos de la toma de control](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) de administrador para asumir un directorio no administrado como Azure Active Directory administrador.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>¿No estás seguro de si tu empresa ya tiene una cuenta profesional?

Si no está seguro de si su empresa tiene una cuenta de trabajo, siga estos pasos para comprobarlo.

1. Inicie sesión en el [portal de administración de Azure.](https://ms.portal.azure.com)
2. Seleccione **Azure Active Directory** en el menú izquierdo y, a continuación, seleccione **Nombres de dominio.**
Si ya tienes una cuenta profesional, se mostrará tu nombre de dominio.

>[!Note]
>Si tiene una suscripción activa a Microsoft Azure u Office 365, ya tiene una cuenta de trabajo y sus credenciales de inicio de sesión deben ser las mismas que las usadas para acceder a esos servicios.