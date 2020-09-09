---
title: ¿Qué se debe hacer si el único administrador del programa MPN ha abandonado la empresa?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información acerca de qué hacer para buscar un nuevo administrador de MPN u obtener ayuda del administrador global de su empresa. Además, obtenga información sobre cómo agregar un nuevo administrador global del centro de Partners.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1ff6252ce36e68f2f17115460a97fa4928daf029
ms.sourcegitcommit: 3a9318d0de7a159215cb454295125532134ff8de
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/09/2020
ms.locfileid: "89570634"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>¿Qué se debe hacer si el único administrador del programa MPN ha abandonado la empresa?

**Se aplica a**

- Centro de partners

El siguiente artículo le guiará a través de tres escenarios típicos con respecto a qué hacer si su administrador de MPN ha abandonado la empresa.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Escenario 1: el administrador de asociados de MPN/admin de cuenta ha dejado la empresa, pero todavía hay administradores globales en la cuenta

En este caso, se puede asignar a otra persona de la compañía el rol de administrador de asociados de MPN. Para tener asignado el rol de administrador de asociados de MPN específico y el rol de administrador de cuenta:

1. Inicie sesión en su cuenta del centro de Partners con su cuenta profesional (por ejemplo, tom@contoso.com ).
1. En la página **Administración de usuarios** filtro en administrador global para ver quiénes son los administradores globales de su empresa. 
1. Póngase en contacto con uno de los administradores globales y pídale que le asigne el rol específico de MPN que necesita. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Escenario 2: administrador de asociados de MPN/administrador de la cuenta ha abandonado la empresa y no hay administradores globales en la cuenta 

Si va a la página de **Administración de usuarios** y filtra por el administrador global, pero observa que no hay ningún administrador global en su empresa que pueda ayudarle a obtener el rol específico de MPN, siga estos pasos:

1. Vaya a [portal.Azure.com](https://ms.portal.azure.com/), inicie sesión con su cuenta profesional (por ejemplo, tom@contoso.com ). 
1. Seleccione la opción **ayuda y soporte técnico** en la barra de navegación del menú de la izquierda.
1. En la página siguiente, seleccione **nuevo support request** y tipo de **problema técnico** en el menú desplegable, inserte los detalles adicionales y haga clic en **siguiente: soluciones.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Busque administrador en Azure Portal":::

4. Después de revisar las soluciones recomendadas en la página siguiente, seleccione **siguiente: detalles** y complete los campos necesarios.
1. Revise y cree la solicitud de soporte técnico.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Escenario 3: el administrador de asociados de MPN/administrador de la cuenta/Administrador global ha abandonado la empresa y no hay otros usuarios que puedan tener acceso a la Azure AD de la empresa. Se trata de una pérdida completa de acceso.

Siga los pasos de [adquisición del administrador](https://docs.microsoft.com/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) para asumir un directorio no administrado como administrador de Azure Active Directory.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>¿No estás seguro de si tu empresa ya tiene una cuenta profesional?

Si no está seguro de si su empresa tiene una cuenta profesional, siga estos pasos para realizar la comprobación.

1. Inicie sesión en el [portal de administración de Azure](https://ms.portal.azure.com).
2. Seleccione **Azure Active Directory** en el menú de la izquierda y, a continuación, seleccione **nombres de dominio**.
Si ya tienes una cuenta profesional, se mostrará tu nombre de dominio.

>[!Note]
>Si tiene una suscripción activa a Microsoft Azure u Office 365, ya tiene una cuenta profesional y las credenciales de inicio de sesión deben ser las mismas que las usadas para tener acceso a esos servicios.