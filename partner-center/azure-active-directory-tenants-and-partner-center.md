---
title: Centro de partners e inquilinos de Azure Active Directory | Centro de partners
description: "Para crear una cuenta del Centro de partners, tu empresa debe tener un inquilino de Azure Active Directory (Azure AD). Azure AD es el servicio de administración de identidades y directorios basados en la nube de Microsoft."
author: labrenne
robots: 
ms.openlocfilehash: 9a9a3c3aa239017fe8ecf655f79acbfab6ff8a0b
ms.sourcegitcommit: d7c4ca62acd1ef1026c7d322e40f55a83a80e72a
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/28/2017
---
# <a name="azure-active-directory-tenants-and-partner-center"></a>Centro de partners e inquilinos de Azure Active Directory  

**Se aplica a**

-  Centro de partners

## <a name="why-you-need-an-azure-ad-tenant"></a>¿Por qué necesitas un inquilino de Azure AD?

Necesitamos vincular un inquilino de Azure AD de tu organización a tu nueva cuenta de Centro de partners para que los usuarios del inquilino puedan conectarse al Centro de partners con sus nombres de usuario y contraseñas de Azure AD (cuenta de Microsoft).

Si tu empresa ya tiene un inquilino de Azure AD, puedes vincularlo a tu cuenta del Centro de partners. 

>**Nota**<br> Antes de decidir si usar un inquilino de Azure AD existente, piensa en cuántos usuarios del inquilino necesitarán trabajar en el Centro de partners. Si tienes usuarios en el inquilino que no tendrán que trabajar en el Centro de partners, piensa en crear a un nuevo inquilino para solo aquellos usuarios que tendrán que trabajar en el Centro de partners.

Si tu empresa aún no tiene un inquilino de Azure AD, puedes crear uno de forma gratuita durante el proceso de inscripción. Selecciona **Crear un inquilino** en la página **Iniciar sesión en Azure Active Directory**. 

### <a name="not-sure-if-your-company-already-has-an-azure-ad-tenant"></a>¿No estás seguro de si tu empresa ya tiene un inquilino de Azure AD?

Si no estás seguro de si tu empresa tiene un inquilino de Azure AD, sigue estos pasos para comprobarlo. Ten en cuenta que si tienes una suscripción activa a Microsoft Azure u Office 365, ya tienes un inquilino de Azure AD.
1.  Inicia sesión en el portal de administración de Azure en https://ms.portal.azure.com
2.  Selecciona Azure Active Directory en el menú y luego selecciona Nombres de dominio.
3.  Si ya tienes un inquilino, se mostrará el nombre de dominio.

### <a name="using-an-existing-tenant"></a>¿Quieres usar un inquilino existente?

Si quieres usar un inquilino existente de Azure AD, pero tienes problemas para iniciar sesión, busca el escenario en el siguiente diagrama que mejor se adapte a tu situación y sigue los pasos recomendados. 

![¿Tienes un inquilino de Azure AD o necesitas crear uno?](images/onboardingAADFlow.png)

Para obtener más información sobre cómo agregar dominios a Azure AD, consulta [Agregar o asociar un dominio de Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain)

## <a name="about-microsoft-azure"></a>Acerca de Microsoft Azure

Microsoft Azure es una plataforma de nube pública que las empresas pueden usar para compilar, implementar y administrar aplicaciones a través de una red global de centros de datos administrados por Microsoft. Las empresas usan Azure para crear una infraestructura de TI virtual con funciones virtuales o servicios, en lugar de equipos físicos. 

Al comprar una suscripción de Azure, esencialmente estás alquilando un espacio dedicado y seguro en la nube pública de Azure, no es demasiado distinto de alquilar una planta de un edificio de oficinas para albergar tu empresa física. Para el propietario del edificio de oficinas, tu empresa es un inquilino. 

Un inquilino de Azure AD es una representación virtual dedicada y aislada de tu empresa en la nube pública de Azure, creada automáticamente cuando te suscribes a un servicio en la nube de Microsoft como Azure, Microsoft Intune u Office 365. 

El inquilino hospeda los usuarios de Azure AD y la información sobre ellos: sus contraseñas, datos de perfil, permisos, etc. El inquilino también incluye grupos, aplicaciones y otra información relativa a una empresa y su seguridad. 

Para obtener más información sobre Azure AD, consulta la [Documentación de Azure Active Directory](https://docs.microsoft.com/ azure/active-directory/). 