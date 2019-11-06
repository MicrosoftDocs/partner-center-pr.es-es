---
title: Requisitos de seguridad para partners | Centro de partners
ms.topic: article
ms.date: 10/11/2019
description: Obtén información acerca los requisitos de seguridad para los asesores y partners que participan en el programa Proveedor de soluciones en la nube.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider program, CSP, Control Panel Vendor, CPV, multi-factor authentication, MFA, secure application model, secure app model, security
ms.localizationpriority: high
ms.openlocfilehash: 4c7f4e61cc249fb51f58e4a94892a2d937cae4e1
ms.sourcegitcommit: 1fe366f787d97c96510cfd409304e7d48af7c286
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/30/2019
ms.locfileid: "73141983"
---
# <a name="partner-security-requirements"></a>Requisitos de seguridad para partners

**Se aplica a**

- Todos los partners que estén en el programa Proveedor de soluciones en la nube
  - Factura directa
  - Proveedor indirecto
  - Revendedor indirecto
- Todos los proveedores de panel de control
- Todos los asesores

Una mayor seguridad y protección de la privacidad se encuentran entre nuestras principales prioridades. Sabemos que la mejor defensa es la prevención y que somos tan seguros como lo sea nuestro vínculo más débil. Esta es la razón por la que necesitamos que todos los usuarios de nuestro ecosistema actúen y se aseguren de que tienen las protecciones de seguridad adecuadas. Para ayudar a proteger a los partners y clientes, presentamos un conjunto de requisitos de seguridad obligatorios para los asesores, proveedores de panel de control y asociados que participen en el programa Proveedor de soluciones en la nube.

## <a name="overview"></a>Introducción

A partir del 1 de agosto de 2019, todos los partners tienen la obligación de aplicar la autenticación multifactor a todas las cuentas de usuario en su inquilino de partner. Los términos asociados a los requisitos de seguridad para partners se han agregado a la [guía del programa Proveedor de soluciones en la nube](https://go.microsoft.com/fwlink/p/?LinkId=617100). En lo que se refiere a los asesores, se aplicarán los mismos requisitos contractuales.

> [!NOTE]
> Se recomienda encarecidamente a todos los partners que realicen transacciones a través de una nube soberana (21Vianet, gobierno de EE. UU. y Alemania) adopten estos requisitos de seguridad de inmediato. Sin embargo, no es preciso que estos partners cumplan los requisitos de seguridad que entran en vigor el 1 de agosto de 2019. En el futuro, Microsoft proporcionará más información acerca de la aplicación de estos requisitos de seguridad para las nubes soberanas.

Los partners que no implementen los requisitos de seguridad obligatorios no podrán realizar transacciones en el programa Proveedor de soluciones en la nube ni administrar los inquilinos del cliente que aprovechen los derechos de administrador delegado, una vez que se apliquen estos requisitos.

## <a name="actions-that-you-need-to-take"></a>Acciones que debes llevar a cabo

Para cumplir los requisitos de seguridad para partners, debes aplicar la autenticación multifactor para cada cuenta de usuario en el inquilino del partner. Para lograrlo, puedes realizar cualquiera de las siguientes acciones.

- Implementar la característica de directivas de protección de línea base de [exigir MFA para los administradores ](/azure/active-directory/conditional-access/howto-baseline-protect-administrators) y [protección del usuario final](/azure/active-directory/conditional-access/howto-baseline-protect-end-users) de Azure Active Directory sin ningún costo adicional.
- Comprar Azure Active Directory Premium para cada cuenta de usuario. Consulta [Planificación de una implementación de Azure Multi-Factor Authentication basada en la nube](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted) para obtener más información.
- Usar una solución de terceros para aplicar la autenticación multifactor para cada cuenta de usuario en el inquilino del partner. Consulta el apartado sobre [cómo se aplicarán los requisitos de seguridad](#how-the-requirements-will-be-enforced) para obtener más detalles y asegurarte de que la solución proporcionará la información esperada.

### <a name="consideration"></a>Consideración

Dado que estos requisitos se aplican a todas las cuentas de usuario del inquilino del partner, deben tenerse en cuenta varias consideraciones para garantizar que la implementación se realiza sin problemas. Entre estas consideraciones se incluye la identificación de cuentas de usuario de Azure Active Directory que no pueden realizar la autenticación multifactor, así como de las aplicaciones y los dispositivos que usa tu organización y que no admiten la autenticación moderna.

Antes de realizar cualquier acción, es aconsejable identificar los siguientes factores

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>¿Hay alguna aplicación o algún dispositivo que no admita el uso de la autenticación moderna?

Cuando apliques la opción de autenticación heredada de la autenticación multifactor, se bloqueará el uso de protocolos como IMAP, POP3, SMTP, etc., ya que no admiten la autenticación multifactor. Para solucionar esta limitación, se puede usar una característica conocida como [contraseñas de aplicación](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) para asegurarse de que la aplicación o el dispositivo se pueden autenticar. Debes examinar las consideraciones acerca del uso de contraseñas, que están documentadas [aquí](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords), aquí para determinar si se pueden usar en su entorno.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>¿Hay usuarios que usen Office 365 proporcionados por licencias asociadas a tu inquilino del partner?

Antes de implementar cualquier solución, es aconsejable determinar qué versión de Microsoft Office utilizan los usuarios de tu inquilino del partner. Examina el [plan para realizar la autenticación multifactor en implementaciones de Office 365](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa) antes de realizar cualquier acción. Existe la posibilidad de que los usuarios tengan problemas de conectividad con aplicaciones como Outlook. Antes de aplicar la autenticación multifactor, es importante asegurarse de que se usa Outlook 2013 SP1, o cualquier versión posterior, y que la organización tiene habilitada la autenticación moderna. Para más información, consulta [Habilitar la autenticación moderna en Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online).

Para habilitar la autenticación moderna en cualquier dispositivo con Windows que tenga Microsoft Office 2013 instalado, es preciso crear dos claves del Registro. Consulta [Habilitar autenticación moderna para Office 2013 en dispositivos Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>¿Hay alguna directiva que impida que los usuarios usen sus dispositivos móviles mientras trabajan?

Es importante identificar las directivas corporativas que impiden que los empleados usen dispositivos móviles mientras trabajan, ya que esto influirá en la solución de autenticación multifactor que implementes. Hay soluciones, como la que se proporciona a través de la implementación de las [directivas de protección de línea base](/azure/active-directory/conditional-access/concept-baseline-protection), que solo permiten el uso de una aplicación de autenticación para la comprobación. Si la organización tiene una directiva que impide el uso de dispositivos móviles, debes tener en cuenta una de las siguientes opciones:

- Implementar una aplicación de contraseñas de un solo uso y duración definida (TOTP) que se pueda ejecutar en un sistema seguro.
- Implementar una solución de terceros que aplique la autenticación multifactor a todas las cuentas de usuario del inquilino del partner que proporcione la opción de verificación más adecuada.
- Comprar licencias de [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) para los usuarios afectados.

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>¿Qué automatización o integración tienes que aproveche las credenciales de usuario para la autenticación?

Como el requisito es aplicar MFA a todos los usuarios, incluidas las cuentas de servicio, del directorio de partners cualquier automatización o integración que aproveche las credenciales de usuario para la autenticación se verá afectada. Por tanto, es importante identificar qué cuentas se usan en estas situaciones. A continuación se muestra una lista de ejemplos de aplicaciones o servicios que se deben tener en cuenta

- Panel de control que se usa usado para aprovisionar recursos en nombre de los clientes
- Integración con todas las plataformas que se utilicen para la facturación (en relación con el programa CSP) y soporte técnico a los clientes
- Scripts de PowerShell que usan los módulos Az, AzureRM, Azure AD, MS Online, etc.

La lista anterior no es completa. Por tanto, es importante que realices una evaluación completa de cualquier aplicación o servicio de tu entorno que aproveche las credenciales de usuario para la autenticación. Para enfrentarte al requisito de la autenticación multifactor, debes implementar las instrucciones del [marco de modelo de aplicaciones seguras](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) siempre que sea posible.

## <a name="accessing-your-environment"></a>Acceso al entorno

Para saber mejor qué o quién realiza la autenticación sin que sea un desafío para la autenticación multifactor, se recomienda revisar la actividad de inicio de sesión. En Azure Active Directory Premium puedes aprovechar el informe de inicios de sesión. Consulta los [informes de actividad de inicio de sesión en el portal de Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins) para obtener más información. Si no tienes Azure Active Directory Premium o estás buscando una manera de obtenerlo a través de PowerShell, deberás utilizar el cmdlet [Get-PartnerUserSignActivity](https://docs.microsoft.com/powershell/module/partnercenter/get-partnerusersigninactivity) del módulo de [PowerShell del Centro de partners](https://www.powershellgallery.com/packages/PartnerCenter/).

## <a name="how-the-requirements-will-be-enforced"></a>Cómo se aplicarán los requisitos

Azure Active Directory y el Centro de partners aplicarán los requisitos de seguridad para partners. Para ello, comprobarán la presencia de la notificación de MFA para identificar que se ha producido la verificación de la autenticación multifactor. Si utilizas Azure Multi-Factor Authentication o las directivas de protección de línea base, no es necesario realizar ninguna acción adicional.

Cuando se usa una solución de autenticación multifactor de terceros, existe la posibilidad de que no se emita la notificación de MFA. Si falta la notificación, Azure Active Directory no podrá determinar si la autenticación multifactor procesó la solicitud de autenticación. Consulta [Testing the Partner Security Requirements](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements) (Prueba de los requisitos de seguridad para partners) para obtener más información sobre cómo comprobar si la solución emite la notificación esperada.

> [!IMPORTANT]
> Si la solución de terceros no emite la notificación esperada, deberás contactar con el proveedor que desarrolló la solución para determinar las acciones que se deben llevar a cabo.

## <a name="resources-and-support"></a>Recursos y soporte técnico

A continuación se muestran los recursos en los que puedes encontrar soporte técnico y código de ejemplo.

- [Comunidad del grupo de instrucciones de seguridad del Centro de partners](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): esta es una comunidad en línea en la que no solo puedes obtener información acerca de los próximos eventos, sino también realizar todas las preguntas que puedas tener.
- [Ejemplos de .NET del Centro de partners](https://github.com/microsoft/partner-center-dotnet-samples): este repositorio de GitHub contiene ejemplos que se han desarrollados mediante .NET y que muestran cómo se puede implementar el marco de modelo de aplicaciones seguras.
- [Ejemplos de Java del Centro de partners](https://github.com/microsoft/partner-center-java-samples): este repositorio de GitHub contiene ejemplos que se han desarrollados mediante Java y que muestran cómo se puede implementar el marco de modelo de aplicaciones seguras.
- [Partner Center PowerShell (autenticación multifactor)](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth): en este artículo se proporcionan datos acerca de cómo implementar el marco de modelo de aplicaciones seguras mediante PowerShell.
