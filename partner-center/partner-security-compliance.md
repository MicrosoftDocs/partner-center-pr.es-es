---
title: Estado de los requisitos de seguridad para partners | Centro de partners
ms.date: 10/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtén información sobre los nuevos requisitos obligatorios que aumentan la seguridad para asesores, proveedores del panel de control y partners en el programa Proveedor de soluciones en la nube.
author: LauraBrenner
ms.author: labrenne
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider program, CSP, Control Panel Vendor, CPV, multi-factor authentication, MFA, secure application model, secure app model, security
ms.localizationpriority: high
ms.topic: conceptual
ms.openlocfilehash: 2fc0926f2277cea8eebd7157af44338aabfaa94c
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2020
ms.locfileid: "80136319"
---
# <a name="partner-security-requirements-status"></a>Estado de los requisitos de seguridad para partners

**Se aplica a**

- Todos los partners que estén en el programa Proveedor de soluciones en la nube
  - Factura directa
  - Proveedor indirecto
  - Revendedor indirecto
- Todos los proveedores de panel de control
- Todos los asesores

**Usuarios adecuados**
-    Todos los usuarios habilitados, incluidos los invitados

Una mayor seguridad y protección de la privacidad se encuentran entre nuestras principales prioridades. Sabemos que la mejor defensa es la prevención y que somos tan seguros como lo sea nuestro vínculo más débil. Esta es la razón por la que necesitamos que todos los usuarios de nuestro ecosistema actúen y se aseguren de que tienen las protecciones de seguridad adecuadas. Para ayudar a proteger a los partners y clientes, presentamos un conjunto de requisitos de seguridad obligatorios para los asesores, proveedores de panel de control y partners que participan en el programa Proveedor de soluciones en la nube.

A partir del 1 de agosto de 2019, todos los partners tienen la obligación de aplicar la autenticación multifactor a todos los usuarios, incluidas las cuentas de servicio, en su inquilino de partner. Para obtener información más detallada sobre las nuevas directivas de seguridad, consulte [Requisitos de seguridad para partners](partner-security-requirements.md).

Queremos asegurarnos de que cada usuario tenga un desafío de MFA para cada autenticación. Esto se puede realizar de cualquiera de estas maneras:

- Mediante la implementación de Azure AD Premium para asegurarse de que se aplica MFA a todos los usuarios.
- Implementar los [valores predeterminados de seguridad Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Mediante la implementación de una solución de terceros para asegurarse de que se aplica MFA a todos los usuarios.

## <a name="partner-security-requirements-status"></a>Estado de los requisitos de seguridad para partners

Este informe puede ayudarle a comprobar el estado de los requisitos de seguridad al proporcionar una manera de ver dónde puede que no los cumpla. El seguimiento se actualiza periódicamente.

>[!NOTE]
>El informe de estado de los requisitos de seguridad para partners solo se admite en el Centro de partners. No está disponible en Microsoft Cloud for US Government ni en Microsoft Cloud Germany. Se recomienda encarecidamente a todos los partners que realicen transacciones a través de una nube soberana (21Vianet, gobierno de EE. UU. y Alemania) que adopten estos nuevos requisitos de seguridad de inmediato. Sin embargo, no es preciso que estos partners cumplan los nuevos requisitos de seguridad que entran en vigor el 1 de agosto de 2019. En el futuro, Microsoft proporcionará más información acerca de la aplicación de estos requisitos de seguridad para las nubes soberanas.

## <a name="multi-factor-authentication-mfa-report"></a>Informe de Multi-Factor Authentication ("MFA")

El informe de MFA del Centro de partners ofrece información sobre la implementación de MFA para asociados, para lo cual proporciona dos tipos de métricas basadas en la configuración de MFA y en las actividades del Centro de partners del inquilino del CSP: 

### <a name="mfa-configuration-on-a-csp-tenant"></a>Configuración de MFA en un inquilino del CSP

Esta métrica está relacionada con la configuración de MFA en un inquilino del CSP, que se captura y se notifica diariamente. Mide el porcentaje de cuentas de usuario habilitadas en las que se aplica MFA mediante cualquiera de esas [opciones de MFA](https://aka.ms/partner-mfa-get-started). Por ejemplo:

- Contoso es un CSP asociado con 110 cuentas de usuario en el inquilino, 10 de las cuales están deshabilitadas. 
- De las 100 cuentas restantes, en 90 se aplica MFA mediante las [opciones de MFA](https://aka.ms/partner-mfa-get-started) proporcionadas. Por lo tanto, la métrica muestra un 90 %. 

### <a name="partner-center-activities-with-mfa"></a>Actividades del Centro de partners con MFA

Cada vez que los empleados inician sesión en el Centro de partners para trabajar o, mediante las API, obtener o enviar datos a través del Centro de partners, su estado de seguridad recibe un desafío y seguimiento. En el seguimiento del estado de seguridad también se incluyen las aplicaciones y cualquier aplicación del proveedor del panel de control. El estado que se muestra corresponde a los siete días anteriores.

#### <a name="mfa-verification-completed-by-users"></a>Comprobación de MFA realizada por los usuarios

Esta métrica está relacionada con actividades del panel del Centro de partners. Mide el porcentaje de operaciones realizadas por los usuarios que han completado la comprobación de MFA. Por ejemplo:

- Contoso es un partner de CSP con dos agentes de administración, Julia y Juan.
- El primer día, Julia inicia sesión en el panel del Centro de partners sin la comprobación de MFA y realiza tres operaciones.
- El segundo día, Juan inicia sesión en el panel del Centro de partners sin la comprobación de MFA y realiza cinco operaciones.
- El tercer día, Julia inicia sesión en el panel del Centro de partners con la comprobación de MFA y realiza dos operaciones.
- Los otros cuatro días, ningún agente realiza operaciones.
- De las 10 operaciones realizadas en el periodo de siete días, dos las realizó un usuario con la comprobación de MFA. Por lo tanto, la métrica muestra un 20 %.

#### <a name="appuser-authentication"></a>Autenticación de aplicación y usuario

Esta métrica está relacionada con el uso de solicitudes de API del Centro de partners realizadas con la autenticación de aplicación y usuario. Mide el porcentaje de solicitudes de API realizadas mediante un token de acceso con notificación de MFA. Por ejemplo:

- Fabrikam es un partner de CSP y tiene una aplicación de CSP que usa una combinación de métodos de autenticación de aplicación y usuario y de solo aplicación.
- El primer día, la aplicación realiza tres solicitudes de API respaldadas por un token de acceso obtenido mediante el método de autenticación de aplicación y usuario sin la verificación de MFA.
- El segundo día, la aplicación realiza cinco solicitudes de API respaldadas por un token de acceso obtenido mediante la autenticación de solo aplicación.
- El tercer día, la aplicación realiza dos solicitudes de API respaldadas por un token de acceso obtenido mediante el método de autenticación de aplicación y usuario con la verificación de MFA.
- Los otros cuatro días, ningún agente realiza operaciones.
- Las cinco solicitudes de API del segundo día que estaban respaldadas por un token de acceso obtenido a través de la autenticación de solo aplicación se omiten de la métrica, ya que no hacen uso de las credenciales de usuario. De las cinco operaciones restantes, dos de ellas estaban respaldadas por un token de acceso obtenido con la verificación de MFA. Por lo tanto, la métrica muestra un 40 %.

## <a name="what-should-i-do-if-the-metrics-under-mfa-report-arent-100"></a>¿Qué debo hacer si las métricas del informe de MFA no corresponde al 100 %?

Es posible que las métricas del informe de MFA del Centro de partners no sean del 100 % para los partners que han implementado MFA. Para comprender por qué, estos son algunos factores a tener en cuenta.

> [!NOTE]
> Tendrá que trabajar con alguien de la organización que esté familiarizado con la administración de identidades y la implementación de MFA para el inquilino del partner.

### <a name="have-you-implemented-mfa-for-your-partner-tenant"></a>¿Ha implementado MFA para el inquilino del partner?

Si no es así, primero debe implementar MFA para el inquilino del partner. Para más información sobre cómo implementar MFA, consulte el artículo [Requisitos de seguridad para partners](partner-security-requirements.md).

### <a name="have-you-only-recently-completed-mfa-implementation"></a>¿Solo ha completado la implementación de MFA recientemente?

Las métricas se calculan cada día y tienen en cuenta las operaciones realizadas en los últimos siete días. Si solo ha completado recientemente la implementación de MFA para el inquilino del partner, las métricas pueden no ser del 100 %.

### <a name="have-some-user-accounts-been-excluded-from-mfa-implementation"></a>¿Algunas cuentas de usuario se han excluido de la implementación de MFA?

Comprenda si la implementación de MFA actual cubre todas las cuentas de usuario o solo algunas. Algunas soluciones MFA están basadas en directivas y admiten la exclusión de usuarios, mientras que otras pueden requerir que se habilite explícitamente MFA por usuario. Compruebe que no ha excluido ningún usuario de la implementación de MFA actual. Las cuentas de usuario que se excluyan e inicien sesión en el Centro de partners para realizar cualquier actividad relacionada con CSP pueden hacer que las métricas no sean del 100 %.

### <a name="is-mfa-only-required-when-certain-conditions-are-met"></a>¿Solo se requiere MFA cuando se cumplen ciertas condiciones?

Comprenda si la implementación actual solo aplica MFA en condiciones específicas. Algunas soluciones MFA proporcionan flexibilidad para aplicar MFA solo cuando se cumplen ciertas condiciones. Por ejemplo, el usuario obtiene acceso desde un dispositivo desconocido o una ubicación desconocida. Un usuario que esté habilitado para MFA pero que no se requiera que complete la comprobación de MFA al acceder al Centro de partners, puede provocar que las métricas no sean del 100%.

>[!NOTE]
>En el caso de los partners que han implementado MFA con los valores predeterminados de seguridad de Azure AD, es importante tener en cuenta que, para ninguna de las cuentas de usuario de administrador, se aplicará la autenticación multifactor según el riesgo. A los usuarios se les pedirá MFA solo durante los intentos de inicio de sesión de riesgo (por ejemplo, el usuario inicia sesión desde una ubicación diferente). Además, los usuarios tendrán hasta 14 días para registrarse para MFA. A los usuarios que no hayan completado el registro de MFA no se les solicitará la comprobación de MFA durante el período de 14 días. Por lo tanto, se espera que las métricas puede que no sean del 100 % para los partners que han implementado MFA con los valores por defecto de seguridad de Azure AD.

### <a name="are-you-using-3rd-party-mfa-solution"></a>¿Usa una solución MFA de terceros?

Si usa una solución MFA de terceros, identifique cómo se integra con Azure AD. En general, hay dos métodos, incluidos los controles personalizados y de federación:

* **Federación de identidades**: cuando Azure AD recibe una solicitud de autenticación, Azure AD redirigirá al usuario al proveedor de identidades federado para la autenticación. Tras una autenticación correcta, el proveedor de identidades federado redirigirá al usuario a Azure AD junto con un token SAML. Para que Azure AD reconozca que el usuario ha completado la comprobación de MFA al autenticarse en el proveedor de identidades federado, el token SAML debe incluir la notificación *authenticationmethodsreferences* (con el valor *multipleauthn*). Compruebe si el proveedor de identidades federado admite la emisión de este tipo de notificaciones. Si es así, compruebe si el proveedor de identidades federado se ha configurado para ello. Si falta la notificación, Azure AD (y, por tanto, el Centro de partners) no sabrá que el usuario ha completado la comprobación de MFA y esto puede hacer que la métrica no sea del 100 %.

* **Control personalizado**: el control personalizado de Azure AD no se puede usar para identificar si un usuario ha completado la comprobación de MFA a través de una solución MFA de terceros. Como resultado, cualquier usuario que haya completado la comprobación de MFA a través de un control personalizado aparecerá siempre en Azure AD (y, a su vez, en el Centro de partners) como si no hubiera completado dicha comprobación. Siempre que sea posible, se recomienda usar la Federación de identidades en lugar de un Control personalizado al integrar con Azure AD.

### <a name="identify-which-users-have-logged-into-partner-center-without-mfa"></a>Identificar qué usuarios han iniciado sesión en el Centro de partners sin usar MFA

Puede ser útil identificar los usuarios que inician sesión en el Centro de partners sin comprobación de MFA y comprobarlos con la implementación de MFA actual. Puede usar el [informe de inicio de sesión de Azure AD ](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins) para averiguar si un usuario ha completado la comprobación de MFA o no. El informe de inicio de sesión de Azure AD solo está disponible actualmente para los partners que se han suscrito a Azure AD Premium o a cualquier SKU de O365 que incluye Azure AD Premium (por ejemplo, EMS).

**Para más información**

- [Comunidad de grupos de guías de seguridad del Centro de partners](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Requisitos de seguridad del Centro de partners](partner-security-requirements.md)
- [Preguntas más frecuentes sobre los requisitos de seguridad del Centro de partners](partner-security-requirements-faq.md)
