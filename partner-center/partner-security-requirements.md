---
title: Requisitos de seguridad para partners
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Presenta los requisitos que deben cumplir los partners para habilitar Multi-Factor Authentication (MFA) y adoptar el marco de modelo de aplicaciones seguras.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider program, CSP, Control Panel Vendor, CPV, multi-factor authentication, MFA, secure application model, secure app model, security
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 43febea2a5eb78d983c620bcc6ec155ba49a7c5e
ms.sourcegitcommit: e68e7ab63b6e7807f0aa797680e9b2e0315ecc97
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/11/2020
ms.locfileid: "86265098"
---
# <a name="partner-security-requirements-for-partners-using-partner-center-or-partner-center-apis"></a>Requisitos de seguridad para partners que usan el Centro de partners o las API del Centro de partners

**Se aplica a**

- Todos los partners que estén en el programa Proveedor de soluciones en la nube
  - Factura directa
  - Proveedor indirecto
  - Revendedor indirecto
- Todos los proveedores de panel de control
- Todos los asesores

**Usuarios adecuados**

- Todos los usuarios habilitados, incluidos los invitados

Una mayor seguridad y protección de la privacidad se encuentran entre nuestras principales prioridades. Sabemos que la mejor defensa es la prevención y que somos tan seguros como lo sea nuestro vínculo más débil. Esta es la razón por la que necesitamos que todos los usuarios de nuestro ecosistema actúen y se aseguren de tener las protecciones de seguridad adecuadas. Para ayudar a proteger a los partners y clientes, presentamos un conjunto de requisitos de seguridad obligatorios para los asesores, proveedores de panel de control y asociados que participen en el programa Proveedor de soluciones en la nube.

## <a name="overview"></a>Introducción

Los partners tienen la obligación de aplicar la autenticación multifactor a todas las cuentas de usuario en su inquilino de partner. Los términos asociados a los requisitos de seguridad para partners se han agregado al acuerdo entre partners de Microsoft. En lo que se refiere a los asesores, se aplicarán los mismos requisitos contractuales.

Los partners que no implementen los requisitos de seguridad obligatorios no podrán realizar transacciones en el programa Proveedor de soluciones en la nube ni administrar los inquilinos del cliente que aprovechen los derechos de administrador delegado, una vez que se apliquen estos requisitos. Además, los partners que no implementen los requisitos de seguridad pueden poner en peligro su participación en los programas.  

Para protegerte a ti y a tus clientes, es necesario que los partners lleven a cabo inmediatamente las siguientes acciones:  

1. **Habilitar Multi-Factor Authentication (MFA) para todas las cuentas de usuario del inquilino de partner**. Multi-Factor Authentication (MFA) se debe aplicar a todas las cuentas de usuario de los inquilinos de partner al iniciar sesión en los servicios en la nube comerciales de Microsoft o cuando realicen transacciones en el Proveedor de soluciones en la nube a través del Centro de partners o de las API.

2. **Adoptar el marco de modelo de aplicaciones seguras**. Adoptar el marco de modelo de aplicaciones seguras. Todos los partners que se integran con la API del Centro de partners deben adoptar el marco de modelo de aplicaciones seguras para las aplicaciones del modelo aplicación + autenticación de usuario.

    > [!IMPORTANT]
    > Se recomienda encarecidamente que los partners implementen el modelo de aplicaciones seguras para la integración con una API de Microsoft, como Azure Resource Manager, Microsoft Graph o el uso de la automatización, como PowerShell con credenciales de usuario, para evitar interrupciones cuando se aplica MFA.

La habilitación de Multi-Factor Authentication (MFA) y la adopción del marco de modelo de aplicaciones seguras ayudarán a proteger la infraestructura y los datos de tus clientes frente a posibles riesgos de seguridad, como la identificación de robos u otros incidentes de fraude.  

## <a name="actions-that-you-need-to-take"></a>Acciones que debes llevar a cabo

Para cumplir los requisitos de seguridad para partners, debes aplicar la autenticación multifactor para cada cuenta de usuario en el inquilino del partner. Esto se puede lograr de una de las siguientes maneras:

- Implementar los [valores predeterminados de seguridad Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

- Comprar Azure Active Directory Premium para cada cuenta de usuario. Para más información, consulta [Planificación de una implementación de Azure Multi-Factor Authentication basada en la nube](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).

- Usar una solución de terceros para aplicar la autenticación multifactor para cada cuenta de usuario en el inquilino del partner. Para asegurarte de que la solución proporcionará la solución esperada, consulta el apartado sobre [cómo se aplicarán los requisitos de seguridad](#how-the-requirements-will-be-enforced).

> [!NOTE]
> Aunque la autenticación multifactor no se requiere contractualmente para una nube soberana (21Vianet, Gobierno de EE. UU. y Alemania), se recomienda encarecidamente que adoptes estos requisitos de seguridad.

## <a name="security-defaults"></a>Valores predeterminados de seguridad

La directiva de valores predeterminados de seguridad es una de las [opciones ](#actions-that-you-need-to-take) que los asociados pueden elegir para implementar MFA para cumplir con los requisitos de seguridad en función de sus necesidades empresariales. Ofrece un nivel básico de seguridad habilitado sin costo adicional. Revisa cómo habilitar MFA para tu organización con Azure AD y las consideraciones clave siguientes antes de habilitar los valores predeterminados de seguridad.

- Las directivas de base de referencia seguirán presentes durante un par de meses y quedarán obsoletas a finales de febrero de 2020.

- Los partners que ya han adoptado las directivas de línea de base deben tomar medidas para realizar la transición a los valores predeterminados de seguridad.

- Los valores predeterminados de seguridad son el reemplazo de disponibilidad general de las directivas de línea de base de la versión preliminar. Una vez que un asociado habilite los valores predeterminados de seguridad, ya no podrá habilitar las directivas de línea de base.

- Con los valores predeterminados de seguridad, todas las directivas se habilitarán a la vez.

- En el caso de los asociados que usan el [acceso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-policy-common), los [valores predeterminados de seguridad no estarán disponibles](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- El bloqueo de la autenticación heredada no se aplicará a los asociados en este momento. Sin embargo, dado que la mayoría de los eventos relacionados con identidades comprometidas provienen de intentos de inicio de sesión mediante la autenticación heredada, se recomienda a los asociados a apartarse de estos protocolos antiguos.

- La cuenta de sincronización de Azure AD Connect se excluye de los valores predeterminados de seguridad.

- Para obtener información detallada, consulta [Habilitar la autenticación multifactor para la organización](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-get-started) y [Valores predeterminados de seguridad de Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Los valores predeterminados de seguridad de Azure AD es la evolución simplificada de las directivas de protección de línea base. Si ya has habilitado las directivas de protección de línea de base, se recomienda encarecidamente que habilites los valores predeterminados de seguridad.

Para pasar de las directivas de línea de base a los valores predeterminados de seguridad, lee [¿Cuáles son los valores de seguridad predeterminados?](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

### <a name="consideration"></a>Consideración

Dado que estos requisitos se aplican a todas las cuentas de usuario del inquilino de partner, debes tener en cuenta varias cosas para garantizar una implementación sin problemas, incluida la identificación de las cuentas de usuario en Azure Active Directory que no pueden realizar la autenticación multifactor, así como las aplicaciones y los dispositivos usados por tu organización que no admiten la autenticación moderna.

Antes de realizar cualquier acción, es aconsejable identificar lo siguiente:

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>¿Hay alguna aplicación o algún dispositivo que no admita el uso de la autenticación moderna?

Cuando apliques la opción de autenticación heredada de la autenticación multifactor, se bloqueará el uso de protocolos como IMAP, POP3, SMTP, etc., ya que no admiten la autenticación multifactor. Para solucionar esta limitación, puedes usar una característica conocida como [contraseñas de aplicación](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) para asegurarte de que la aplicación o el dispositivo se seguirán autenticando. Debes examinar las consideraciones acerca del uso de contraseñas, que están documentadas [aquí](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords), aquí para determinar si se pueden usar en su entorno.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>¿Hay usuarios que usen Office 365 proporcionados por licencias asociadas a tu inquilino del partner?

Antes de implementar cualquier solución, aconsejamos determinar qué versión de Microsoft Office utilizan los usuarios de tu inquilino de partner. Examina el [plan para realizar la autenticación multifactor en implementaciones de Office 365](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa) antes de realizar cualquier acción. Existe la posibilidad de que los usuarios tengan problemas de conectividad con aplicaciones como Outlook. Antes de aplicar la autenticación multifactor, es importante asegurarse de que se usa Outlook 2013 SP1, o cualquier versión posterior, y que la organización tiene habilitada la autenticación moderna. Para más información, consulta [Habilitar la autenticación moderna en Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online).

Para habilitar la autenticación moderna en cualquier dispositivo con Windows que tenga Microsoft Office 2013 instalado, es preciso crear dos claves del Registro. Consulta [Habilitar autenticación moderna para Office 2013 en dispositivos Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>¿Hay alguna directiva que impida que los usuarios usen sus dispositivos móviles mientras trabajan?

Es importante identificar las directivas corporativas que impiden que los empleados usen dispositivos móviles mientras trabajan, ya que esto influirá en la solución de autenticación multifactor que implementes. Hay soluciones, como la que se proporciona a través de la implementación de las [directivas de seguridad de Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), que solo permiten el uso de una aplicación de autenticación para la comprobación. Si la organización tiene una directiva que impide el uso de dispositivos móviles, debes tener en cuenta una de las siguientes opciones:

- Implementar una aplicación de contraseñas de un solo uso y duración definida (TOTP) que se pueda ejecutar en un sistema seguro.

- Implementar una solución de terceros que aplique la autenticación multifactor a todas las cuentas de usuario del inquilino del partner que proporcione la opción de verificación más adecuada.

- Comprar licencias de [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) para los usuarios afectados.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>¿Qué automatización o integración tienes que aproveche las credenciales de usuario para la autenticación?

Como el requisito es aplicar MFA a todos los usuarios, incluidas las cuentas de servicio, del directorio de partners cualquier automatización o integración que aproveche las credenciales de usuario para la autenticación se verá afectada. Por tanto, es importante identificar qué cuentas se usan en estas situaciones. Consulta la siguiente lista de aplicaciones o servicios de ejemplo que debes tener en cuenta:

- Panel de control que se usa usado para aprovisionar recursos en nombre de los clientes

- Integración con todas las plataformas que se utilicen para la facturación (en relación con el programa CSP) y soporte técnico a los clientes

- Scripts de PowerShell que usan los módulos Az, AzureRM, Azure AD, MS Online, etc.

La lista anterior no es completa. Por tanto, es importante que realices una evaluación completa de cualquier aplicación o servicio de tu entorno que aproveche las credenciales de usuario para la autenticación. Para enfrentarte al requisito de la autenticación multifactor, debes implementar las instrucciones del [marco de modelo de aplicaciones seguras](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) siempre que sea posible.

## <a name="accessing-your-environment"></a>Acceso al entorno

Para saber mejor qué o quién realiza la autenticación sin que sea un desafío para la autenticación multifactor, te recomendamos revisar la actividad de inicio de sesión. En Azure Active Directory Premium puedes aprovechar el informe de inicio de sesión. Consulta los [informes de actividad de inicio de sesión en el portal de Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins) para obtener más información. Si no tienes Azure Active Directory Premium o estás buscando una manera de obtenerlo a través de PowerShell, deberás utilizar el cmdlet [Get-PartnerUserSignActivity](https://docs.microsoft.com/powershell/module/partnercenter/get-partnerusersigninactivity) del módulo de [PowerShell del Centro de partners](https://www.powershellgallery.com/packages/PartnerCenter/).

## <a name="how-the-requirements-will-be-enforced"></a>Cómo se aplicarán los requisitos

Azure Active Directory y el Centro de partners aplicarán los requisitos de seguridad para partners. Para ello, comprobarán la presencia de la notificación de MFA para identificar que se ha producido la verificación de la autenticación multifactor. A partir del 18 de noviembre de 2019, Microsoft activará medidas de seguridad adicionales (conocidas anteriormente como "aplicación técnica") para los inquilinos de partner. 

Tras la activación, se solicitará a los usuarios del inquilino de partner que completen la comprobación Multi-Factor Authentication (MFA) al realizar cualquier operación de administrar en nombre de (AOBO). Seguiremos ampliando el ámbito de las medidas de seguridad a otros escenarios y roles de usuario, enviando un aviso previo a los partners. Para obtener más información, consulta este documento, que se actualizará con frecuencia. Los partners que no han cumplido los requisitos deben implementar estas medidas lo antes posible para evitar interrupciones empresariales. 

Si utilizas Azure Multi-Factor Authentication o las directivas de seguridad de Azure AD, no es necesario realizar ninguna acción adicional.

Cuando se usa una solución de autenticación multifactor de terceros, existe la posibilidad de que no se emita la notificación de MFA. Si falta la notificación, Azure Active Directory no podrá determinar si la autenticación multifactor procesó la solicitud de autenticación. Para obtener más información sobre cómo comprobar si la solución emite la notificación esperada, consulta [Prueba de los requisitos de seguridad para partners](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Si la solución de terceros no emite la notificación esperada, deberás contactar con el proveedor que desarrolló la solución para determinar las acciones que se deben llevar a cabo.

## <a name="resources-and-support"></a>Recursos y soporte técnico

Consulta los siguientes recursos para obtener soporte y el código de ejemplo:

- [Comunidad del grupo de instrucciones de seguridad del Centro de partners](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): la comunidad del grupo de instrucciones de seguridad del Centro de partners es una comunidad en línea en la que puedes obtener información acerca de los próximos eventos y realizar todas las preguntas que puedas tener.
- [Ejemplos de .NET del Centro de partners](https://github.com/microsoft/partner-center-dotnet-samples): este repositorio de GitHub contiene ejemplos que se han desarrollado mediante .NET y que muestran cómo se puede implementar el marco de modelo de aplicaciones seguras.
- [Ejemplos de Java del Centro de partners](https://github.com/microsoft/partner-center-java-samples): este repositorio de GitHub contiene ejemplos que se han desarrollado mediante Java y que muestran cómo se puede implementar el marco de modelo de aplicaciones seguras.
- [Multi-Factor Authentication de PowerShell del Centro de partners](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth): en este artículo de Multi-Factor Authentication se proporcionan datos acerca de cómo implementar el marco de modelo de aplicaciones seguras mediante PowerShell.
