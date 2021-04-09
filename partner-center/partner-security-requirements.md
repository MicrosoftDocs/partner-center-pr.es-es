---
title: Requisitos de seguridad para partners
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Presenta los requisitos de seguridad de los partners para habilitar Multi-Factor Authentication (MFA) y adoptar el marco del modelo de aplicaciones seguras.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: b7fa76999d2e071f80c0175a8dfcbc1afe527bfc
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087066"
---
# <a name="security-requirements-for-using-partner-center-or-partner-center-apis"></a>Requisitos de seguridad para usar el Centro de partners o las API del Centro de partners

**Roles adecuados**

- Todos los usuarios del Centro de partners

En este artículo se explican los requisitos de seguridad obligatorios para asesores, proveedores de panel de control y partners participantes en el programa Proveedor de soluciones en la nube, así como las opciones de autenticación y otras consideraciones de seguridad. La seguridad y la protección de la privacidad se encuentran entre nuestras principales prioridades. Sabemos que la mejor defensa es la prevención y que somos tan seguros como lo sea nuestro vínculo más débil. Esta es la razón por la que necesitamos que todos los usuarios de nuestro ecosistema actúen y se aseguren de tener las protecciones de seguridad adecuadas.

## <a name="mandatory-security-requirements"></a>Requisitos de seguridad obligatorios

Los asociados que no implementen los requisitos de seguridad obligatorios no podrán realizar transacciones en el programa Proveedor de soluciones en la nube ni administrar los inquilinos del cliente que usen los derechos de administrador delegado. Además, los partners que no implementen los requisitos de seguridad pueden poner en peligro su participación en los programas. Los términos asociados a los requisitos de seguridad para partners se han agregado al acuerdo entre partners de Microsoft. En lo que se refiere a los asesores, se aplicarán los mismos requisitos contractuales.

Para protegerte a ti y a tus clientes, es necesario que los partners lleven a cabo inmediatamente las siguientes acciones:  

1. **Habilitar la autenticación multifactor (MFA) para todas las cuentas de usuario del inquilino de partner**. Debe aplicar MFA en todas las cuentas de usuario de los inquilinos de partner. MFA presentará un desafío a los usuarios al iniciar sesión en los servicios en la nube comerciales de Microsoft o cuando realicen transacciones en el programa Proveedor de soluciones en la nube a través del Centro de partners o de las API.

2. **Adoptar el marco de modelo de aplicaciones seguras**. Todos los partners que se integran con las API del Centro de partners deben adoptar el [marco del modelo de aplicaciones seguras](/partner-center/develop/enable-secure-app-model) para las aplicaciones con cualquier modelo de autenticación de aplicación y usuario.

    > [!IMPORTANT]
    > Se recomienda encarecidamente que los partners implementen el modelo de aplicaciones seguras para la integración con una API de Microsoft, como Azure Resource Manager o Microsoft Graph o al usar la automatización, como PowerShell con credenciales de usuario, para evitar interrupciones cuando se aplica MFA.

Estos requisitos de seguridad le ayudarán a proteger su infraestructura y a proteger los datos de sus clientes de posibles riesgos de seguridad, como el robo de identidad u otros incidentes de fraude.  

## <a name="implementing-multi-factor-authentication"></a>Implementación de la autenticación multifactor

Para cumplir los requisitos de seguridad para partners, debe implementar y aplicar MFA para cada cuenta de usuario del inquilino del partner. Esto se puede lograr de una de las siguientes maneras:

- Implemente los [valores predeterminados de seguridad de Azure Active Directory (Azure AD)](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults). Obtenga más información en la [sección siguiente](#security-defaults).

- Compre Azure Active Directory Premium para cada cuenta de usuario. Para obtener más información, consulte [Planificación de una implementación de Azure AD Multi-Factor Authentication](/azure/active-directory/authentication/howto-mfa-getstarted).

- Use una solución de terceros para aplicar MFA a cada cuenta de usuario en el inquilino del partner. Para asegurarte de que la solución proporcionará la solución esperada, consulta el apartado sobre [cómo se aplicarán los requisitos de seguridad](#how-the-requirements-are-enforced).

> [!NOTE]
> Aunque la autenticación multifactor no se requiere contractualmente para una nube soberana (Gobierno de EE. UU. y Alemania), es muy recomendable que adopte estos requisitos de seguridad.

### <a name="security-defaults"></a>Valores predeterminados de seguridad

Una de las opciones que los partners pueden elegir para implementar los requisitos de MFA es la habilitación de los valores predeterminados de seguridad en Azure AD. Los valores predeterminados de seguridad ofrecen un nivel básico de seguridad sin ningún costo adicional. Revise cómo habilitar MFA para la organización con Azure AD y las consideraciones clave siguientes antes de habilitar los valores predeterminados de seguridad.

- Los partners que ya han adoptado las directivas de línea de base deben tomar medidas para realizar la transición a los valores predeterminados de seguridad.

- Los valores predeterminados de seguridad son el reemplazo de disponibilidad general de las directivas de línea de base de la versión preliminar. Una vez que un asociado habilite los valores predeterminados de seguridad, ya no podrá habilitar las directivas de línea de base.

- Con los valores predeterminados de seguridad, todas las directivas se habilitarán a la vez.

- En el caso de los asociados que usan el [acceso condicional](/azure/active-directory/conditional-access/concept-conditional-access-policy-common), los [valores predeterminados de seguridad no estarán disponibles](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults#disabling-security-defaults).

- En este momento, no bloqueamos la autenticación heredada. Sin embargo, dado que la mayoría de los eventos relacionados con identidades comprometidas provienen de intentos de inicio de sesión mediante la autenticación heredada, se recomienda a los asociados apartarse de estos protocolos antiguos.

- La cuenta de sincronización de Azure AD Connect se excluye de los valores predeterminados de seguridad.

Para obtener información detallada, lea [Introducción a Azure AD Multi-Factor Authentication en una organización](/azure/active-directory/authentication/concept-mfa-get-started) y [¿Cuáles son los valores de seguridad predeterminados?](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

> [!NOTE]
> Los valores predeterminados de seguridad de Azure AD es la evolución simplificada de las directivas de protección de línea base. Si ya ha habilitado las directivas de protección de la base de referencia, es muy recomendable habilitar los [valores predeterminados de seguridad](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults).

## <a name="implementation-considerations"></a>Consideraciones de implementación

Dado que estos requisitos se aplican a todas las cuentas de usuario del inquilino del partner, debe tener en cuenta varios factores para garantizar una implementación sin problemas. Por ejemplo, identifique las cuentas de usuario de Azure AD que no puedan usar MFA, así como las aplicaciones y los dispositivos de la organización que no admiten la autenticación moderna.

Antes de realizar cualquier acción, se recomienda completar las validaciones siguientes. 

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-modern-authentication"></a>¿Hay alguna aplicación o algún dispositivo que no admita el uso de la autenticación moderna?

Cuando se aplique MFA, se bloquearán los protocolos de uso de autenticación heredados, como IMAP, POP3, SMTP y otros, ya que no admiten MFA. Para solucionar esta limitación, puede usar las [contraseñas de aplicación](/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) para asegurarse de que la aplicación o el dispositivo se seguirán autenticando. Revise las [consideraciones acerca del uso de contraseñas de aplicación](/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) para determinar si se pueden usar en su entorno.

#### <a name="do-you-have-office-365-users-with-licenses-associated-with-your-partner-tenant"></a>¿Tiene usuarios de Office 365 con licencias asociadas con su inquilino de partner?

Antes de implementar cualquier solución, aconsejamos determinar qué versión de Microsoft Office utilizan los usuarios del inquilino del asociado. Existe la posibilidad de que los usuarios tengan problemas de conectividad con aplicaciones como Outlook. Antes de aplicar MFA, es importante asegurarse de que usa Outlook 2013 SP1 o posterior y de que la organización tiene habilitada la autenticación moderna. Para obtener más información, consulta [Habilitación de la autenticación moderna en Exchange Online](/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online). 

Para habilitar la autenticación moderna en los dispositivos con Windows que tengan Microsoft Office 2013 instalado, es preciso crear dos claves del Registro. Consulta [Habilitar autenticación moderna para Office 2013 en dispositivos Windows](/office365/admin/security-and-compliance/enable-modern-authentication).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>¿Hay alguna directiva que impida que los usuarios usen sus dispositivos móviles mientras trabajan?

Es importante identificar las directivas corporativas que impiden que los empleados usen dispositivos móviles mientras trabajan, ya que esto influirá en la solución MFA que implementes. Hay soluciones, como la que se proporciona a través de la implementación de las [directivas de seguridad de Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults), que solo permiten el uso de una aplicación de autenticación para la comprobación. Si la organización tiene una directiva que impide el uso de dispositivos móviles, debes tener en cuenta una de las siguientes opciones:

- Implementar una aplicación de contraseñas de un solo uso y duración definida (TOTP) que se pueda ejecutar en un sistema seguro.

- Implementar una solución de terceros que aplique MFA a todas las cuentas de usuario del inquilino del partner que proporcione la opción de verificación más adecuada.

- Comprar licencias de [Azure Active Directory Premium](https://azure.microsoft.com/pricing/details/active-directory/) para los usuarios afectados.

#### <a name="what-automation-or-integration-do-you-have-to-leverage-user-credentials-for-authentication"></a>¿Qué automatización o integración tienes que aproveche las credenciales de usuario para la autenticación?

Dado que aplicamos MFA a todos los usuarios, incluidas las cuentas de servicio, del directorio de asociados, esto afecta a cualquier automatización o integración que utilice las credenciales de usuario para la autenticación. Por tanto, es importante identificar qué cuentas se usan en estas situaciones. Consulta la siguiente lista de aplicaciones o servicios de ejemplo que debes tener en cuenta:

- Panel de control que se usa usado para aprovisionar recursos en nombre de los clientes

- Integración con todas las plataformas que se utilicen para la facturación (en relación con el programa CSP) y soporte técnico a los clientes

- Scripts de PowerShell que usan los módulos Az, AzureRM, Azure AD, MS Online y otros

La lista anterior no es completa. Por tanto, es importante que realice una evaluación completa de cualquier aplicación o servicio de su entorno que use las credenciales de usuario para la autenticación. Para enfrentarse al requisito de MFA, debes implementar las instrucciones del [marco de modelo de aplicaciones seguras](/partner-center/develop/enable-secure-app-model) siempre que sea posible.

## <a name="accessing-your-environment"></a>Acceso al entorno

Para saber mejor qué o quién realiza la autenticación sin un desafío para MFA, es recomendable revisar la actividad de inicio de sesión. En Azure Active Directory Premium, puede usar el informe de inicio de sesión. Para obtener más información sobre este tema, consulte los [Informes de actividad de inicio de sesión en el portal de Azure Active Directory](/azure/active-directory/reports-monitoring/concept-sign-ins). Si no tiene Azure Active Directory Premium o está buscando una manera de obtener la actividad de inicio de sesión mediante PowerShell, deberá utilizar el cmdlet [Get-PartnerUserSignActivity](/powershell/module/partnercenter/get-partnerusersigninactivity) del módulo de [PowerShell del Centro de partners](https://www.powershellgallery.com/packages/PartnerCenter/).

## <a name="how-the-requirements-are-enforced"></a>Cómo se aplican los requisitos

Azure AD y el Centro de partners aplican los requisitos de seguridad para partners. Para ello, comprueban la presencia de la notificación de MFA para identificar que se ha producido. A partir del 18 de noviembre de 2019, Microsoft activó medidas de seguridad adicionales (conocidas anteriormente como de "aplicación técnica") para los inquilinos de partner.

Tras la activación, se solicita a los usuarios del inquilino de partner que completen la verificación MFA al realizar cualquier operación de administración delegada (AOBO), acceder al portal del Centro de partners o llamar a las API del Centro de partners. Para obtener más información, consulte [Requisito de Multi-Factor Authentication (MFA) para el inquilino de partner](partner-security-requirements-mandating-mfa.md). 

Los partners que no han cumplido los requisitos deben implementar estas medidas lo antes posible para evitar interrupciones empresariales. Si utiliza Azure Active Directory Multi-Factor Authentication o los valores predeterminados de seguridad de Azure AD, no es necesario realizar ninguna acción adicional.

Si usa una solución de MFA de terceros, existe la posibilidad de que no se emita la notificación de MFA. Si falta la notificación, Azure AD no podrá determinar si MFA generó un desafío para la solicitud de autenticación. Para obtener más información sobre cómo comprobar si la solución emite la notificación esperada, consulta [Prueba de los requisitos de seguridad para partners](/powershell/partnercenter/test-partner-security-requirements). 

> [!IMPORTANT]
> Si la solución de terceros no emite la notificación esperada, deberás contactar con el proveedor que desarrolló la solución para determinar las acciones que se deben llevar a cabo.

## <a name="resources-and-samples"></a>Recursos y muestras

Consulta los siguientes recursos para obtener soporte y el código de ejemplo:

- [Comunidad del grupo de instrucciones de seguridad del Centro de partners](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): la comunidad del grupo de instrucciones de seguridad del Centro de partners es una comunidad en línea en la que puedes obtener información acerca de los próximos eventos y realizar todas las preguntas que puedas tener.
- [Ejemplos de .NET del Centro de partners](https://github.com/microsoft/partner-center-dotnet-samples): este repositorio de GitHub contiene ejemplos que se han desarrollado mediante .NET y que muestran cómo se puede implementar el marco de modelo de aplicaciones seguras.
- [Ejemplos de Java del Centro de partners](https://github.com/microsoft/partner-center-java-samples): este repositorio de GitHub contiene ejemplos que se han desarrollado mediante Java y que muestran cómo se puede implementar el marco de modelo de aplicaciones seguras.
- [Multi-Factor Authentication de PowerShell del Centro de partners](/powershell/partnercenter/multi-factor-auth): en este artículo de Multi-Factor Authentication se proporcionan datos acerca de cómo implementar el marco de modelo de aplicaciones seguras mediante PowerShell.

## <a name="next-steps"></a>Pasos siguientes

- [Requisito de Multi-Factor Authentication (MFA) para el inquilino de partner](partner-security-requirements-mandating-mfa.md)