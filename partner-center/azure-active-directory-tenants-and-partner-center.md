---
title: Vinculación de la cuenta profesional para acceder al Centro de partners
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Crea una cuenta profesional que vincule tu empresa con tu cuenta del Centro de partners. Esto permite a los empleados de la empresa obtener acceso al Centro de partners.
author: LauraBrenner
ms.author: labrenne
ms.custom: SEOAPR.20
Keywords: cuenta profesional, correo electrónico, inquilino, inquilino de Azure, crear cuenta, nombre de dominio
ms.localizationpriority: high
ms.date: 11/25/2019
ms.openlocfilehash: e46be80cb39233e7632a97fd511232d5ff762499
ms.sourcegitcommit: 093039319fab2a44ab147159bc4be832f1330d57
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/14/2020
ms.locfileid: "83394217"
---
# <a name="create-a-work-account-that-links-your-company-to-your-partner-center-account"></a>Crea una cuenta profesional que vincule tu empresa con tu cuenta del Centro de partners.

**Se aplica a**

- Centro de partners

**Roles adecuados**

- Administrador global
- Administrador del control de usuarios

## <a name="why-you-need-a-work-account"></a>¿Por qué se necesitas una cuenta profesional?

Microsoft requiere que vincules la cuenta profesional de tu empresa a tu nueva cuenta del Centro de partners. El vínculo permite a los usuarios de la cuenta iniciar sesión en el Centro de partners con sus nombres de usuario y contraseñas de la cuenta profesional.

## <a name="the-work-account-email-address"></a>Dirección de correo electrónico de la cuenta profesional

Tu cuenta profesional o correo electrónico del trabajo es la dirección de correo electrónico que te proporcionó la empresa. El correo electrónico de una cuenta profesional suele tener el formato `you@yourcompany.com`. Las direcciones de correo electrónico personales, como las de Hotmail, Gmail o Yahoo, no se consideran correos electrónicos del trabajo y no se pueden usar para la cuenta del Centro de partners.

Si tienes más de una dirección de correo electrónico del trabajo válida, usa la que esté asociada a tu sede corporativa en lugar de al departamento regional. Por ejemplo, usa el correo electrónico `contoso.com` en lugar de la dirección `contoso.uk`.

> [!NOTE]  
> Antes de decidir si usar una cuenta profesional existente, piensa en cuántos usuarios de la cuenta necesitarán trabajar en el Centro de partners. Si tienes usuarios en la cuenta que no tendrán que trabajar en el Centro de partners, piensa en crear una nueva cuenta para solo aquellos usuarios que tendrán que trabajar en el Centro de partners.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>¿No estás seguro de si tu empresa ya tiene una cuenta profesional?

Si no estás seguro de si tu empresa tiene una cuenta profesional, sigue estos pasos para comprobarlo. Si tienes una suscripción activa a Microsoft Azure u Office 365, ya tienes una cuenta profesional.

1. Inicie sesión en [Azure Portal](https://portal.azure.com).

2. Selecciona Azure Active Directory en el menú y luego selecciona Nombres de dominio.

3. Si ya tienes una cuenta profesional, se mostrará tu nombre de dominio.

Si tu empresa aún no tiene una cuenta profesional, puedes crear una durante el proceso de inscripción.

En el diagrama siguiente se proporcionan los pasos para varios escenarios típicos:

- determinar si tienes una cuenta profesional
- determinar cómo iniciar sesión en tu cuenta profesional
- determinar si necesitas crear una nueva cuenta profesional

:::image type="content" source="images/onboardingAADFlow.png" lightbox="images/onboardingAADFlow.png" alt-text="¿Tienes una cuenta profesional o necesitas crear una?":::

Para obtener más información sobre cómo agregar dominios en Azure AD, consulta el artículo sobre cómo [agregar o asociar un dominio en Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-add-domain).

## <a name="about-microsoft-azure"></a>Acerca de Microsoft Azure

Microsoft Azure es una plataforma de nube pública que las empresas pueden usar para compilar, implementar y administrar aplicaciones a través de una red global de centros de datos administrados por Microsoft. Las empresas usan Azure para crear una infraestructura de TI virtual con funciones o servicios virtuales, en lugar de equipos físicos.

Al comprar una suscripción de Azure, esencialmente estás alquilando un espacio dedicado y seguro en la nube pública de Azure. No es demasiado distinto a alquilar una planta de un edificio de oficinas para albergar tu empresa física. Para el propietario del edificio de oficinas, tu empresa es un inquilino.

Una cuenta profesional de Azure es una representación virtual dedicada y aislada de tu empresa en la nube pública de Azure, que se crea automáticamente cuando te suscribes a un servicio en la nube de Microsoft como Azure, Microsoft Intune u Office 365.

La cuenta profesional hospeda los usuarios de Azure AD y la información sobre ellos: sus contraseñas, datos de perfil, permisos, etc. La cuenta profesional también contiene grupos, aplicaciones y otra información relativa a una compañía y su seguridad.
