---
title: Informe de estado de requisitos de seguridad
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información acerca de cómo comprobar el cumplimiento de los requisitos de seguridad con el informe de estado de requisitos de seguridad y el informe de MFA del Centro de partners.
author: isaiahwilliams
ms.author: iswillia
ms.localizationpriority: high
ms.topic: conceptual
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f521e05fbf0b3a6c209a84ed9ab53d2502960a5
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624160"
---
# <a name="security-requirements-status-report"></a>Informe de estado de requisitos de seguridad

**Roles adecuados**
- Proveedores del Panel de control
- Administradores globales

En este artículo se explica el informe de estado de los requisitos de seguridad del Centro de partners. Este informe proporciona métricas sobre el cumplimiento de los [requisitos de seguridad de los partners](partner-security-requirements.md) para la autenticación multifactor (MFA) para los usuarios del inquilino de partner.

Para obtener acceso a este informe en el [Centro de partners](https://partner.microsoft.com/dashboard), vaya a **Configuración** > **Configuración de cuenta** > **Estado de requisitos de seguridad**. El informe se actualiza diariamente y refleja los datos de inicio de sesión de los últimos siete días.

>[!NOTE]
>El informe de estado de los requisitos de seguridad solo se admite en el Centro de partners. No está disponible en Microsoft Cloud for US Government ni en Microsoft Cloud Germany. Se recomienda encarecidamente a todos los partners que realicen transacciones a través de una nube soberana (Gobierno de EE. UU. y Alemania) que adopten estos nuevos requisitos de seguridad de inmediato. Sin embargo, actualmente, no es preciso que estos partners cumplan los nuevos requisitos de seguridad. En el futuro, Microsoft proporcionará más información acerca de la aplicación de estos requisitos de seguridad para las nubes soberanas.

## <a name="security-status-metrics"></a>Métricas de estado de seguridad

El informe de estado de requisitos de seguridad ofrece conclusiones acerca de la implementación de MFA para partners y proporciona métricas sobre la configuración de MFA y las actividades del Centro de partners en los inquilinos de partner. En las siguientes secciones se describen con más detalle estas métricas.

### <a name="mfa-configuration-on-a-partner-tenant"></a>Configuración de MFA en un inquilino de partner

La métrica **Percentage of enabled user accounts with MFA enforced using options listed here:** (Porcentaje de cuentas de usuario habilitadas con MFA aplicada mediante las opciones que se muestran aquí:) muestra el porcentaje de cuentas de usuario habilitadas en el inquilino del partner que tiene MFA aplicada. Puede usar una de estas [opciones de MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) para lograr el cumplimiento. Estos datos se capturan y se registran diariamente. Por ejemplo:

- Contoso es un partner de CSP con 110 cuentas de usuario en el inquilino, 10 de las cuales están deshabilitadas. 
- De las 100 cuentas restantes, en 90 se aplica MFA mediante las [opciones de MFA](/azure/active-directory/fundamentals/concept-fundamentals-mfa-get-started) proporcionadas. Por lo tanto, la métrica muestra un 90 %. 

### <a name="partner-center-requests-with-mfa"></a>Solicitudes del Centro de partners con MFA

Cada vez que los empleados inician sesión en el Centro de partners para trabajar o, mediante las API, obtener o enviar datos a través del Centro de partners, su estado de seguridad recibe un desafío y seguimiento. En el seguimiento del estado de seguridad también se incluyen las aplicaciones y cualquier aplicación del proveedor del panel de control. Estos datos se muestran en métricas en **Porcentaje de solicitudes al Centro de partners con MFA** y reflejan los últimos siete días.

#### <a name="dashboard-mfa-verification"></a>Verificación de MFA del panel

La métrica **Through Partner Center portal** (Mediante el portal del Centro de partners) está relacionada con las actividades del panel del Centro de partners. Mide el porcentaje de operaciones realizadas por los usuarios que han completado la comprobación de MFA. Por ejemplo:

- Contoso es un partner de CSP con dos agentes de administración, Julia y Juan.
- El primer día, Julia inicia sesión en el panel del Centro de partners sin verificación MFA y realiza tres operaciones.
- El segundo día, Juan inicia sesión en el panel del Centro de partners sin verificación MFA y realiza cinco operaciones.
- El tercer día, Julia inicia sesión en el panel del Centro de partners con verificación MFA y realiza dos operaciones.
- Los otros cuatro días, ningún agente realiza operaciones.
- De las 10 operaciones realizadas en el periodo de siete días, dos las realizó un usuario con verificación MFA. Por lo tanto, la métrica muestra un 20 %.

Usa el archivo **Portal requests without MFA** para averiguar qué usuario inició sesión en el panel del Centro de partners sin verificación MFA y la hora de la última visita en el período notificado.

#### <a name="appuser-mfa-verification"></a>Verificación MFA de aplicación y usuario

La métrica **Through API or SDK** (Mediante la API o el SDK) está relacionada con la autenticación de aplicación y usuario mediante solicitudes de la API del Centro de partners. Mide el porcentaje de solicitudes de API realizadas mediante un token de acceso con notificación de MFA. Por ejemplo:

- Fabrikam es un partner de CSP y tiene una aplicación de CSP que usa una combinación de métodos de autenticación de aplicación y usuario y de solo aplicación.
- El primer día, la aplicación realiza tres solicitudes de API respaldadas por un token de acceso obtenido mediante el método de autenticación de aplicación y usuario sin la verificación de MFA.
- El segundo día, la aplicación realiza cinco solicitudes de API respaldadas por un token de acceso obtenido mediante la autenticación de solo aplicación.
- El tercer día, la aplicación realiza dos solicitudes de API respaldadas por un token de acceso obtenido mediante el método de autenticación de aplicación y usuario con verificación MFA.
- Los otros cuatro días, ningún agente realiza operaciones.
- Las cinco solicitudes de API del segundo día, que estaban respaldadas por un token de acceso obtenido mediante la autenticación de solo aplicación, se omiten de la métrica, ya que no hacen uso de las credenciales de usuario. De las cinco operaciones restantes, dos de ellas estaban respaldadas por un token de acceso obtenido con la verificación de MFA. Por lo tanto, la métrica muestra un 40 %.

Para conocer los resultados de las actividades de aplicación y usuario en el valor distinto de 100 % de esta métrica, usa los archivos:

- **API requests summary** para comprender el estado general de MFA por aplicación.
- **All API requests** para comprender los detalles de cada una de las solicitudes de API realizadas por los usuarios del inquilino. El resultado está limitado a un máximo de 10 000 solicitudes más recientes a fin de optimizar la experiencia de descarga.

## <a name="actions-for-mfa-status-below-100"></a>Acciones para un estado de MFA inferior al 100 %

Algunos partners que hayan implementado MFA podrían ver métricas de informe por debajo del 100 %. Para comprender por qué, estos son algunos factores a tener en cuenta.

> [!NOTE]
> Tendrá que trabajar con alguien de la organización que esté familiarizado con la administración de identidades y la implementación de MFA para el inquilino del partner.

### <a name="implemented-mfa-for-your-partner-tenant"></a>Se implementó MFA para el inquilino del partner

Para lograr el cumplimiento, debe implementar MFA para el inquilino del partner. Para obtener información detallada sobre cómo implementar MFA, consulte [Requisitos de seguridad para usar el Centro de partners o las API del Centro de partners](partner-security-requirements.md).

>[!NOTE]
> Las métricas de MFA se calculan cada día y tienen en cuenta las operaciones realizadas en los últimos siete días. Si solo ha completado recientemente la implementación de MFA para el inquilino del partner, puede que las métricas aún no sean del 100 %.

### <a name="verify-mfa-on-all-user-accounts"></a>Verificar MFA en todas las cuentas de usuario

Comprenda si la implementación de MFA actual cubre todas las cuentas de usuario o solo algunas. Algunas soluciones MFA están basadas en directivas y admiten la exclusión de usuarios, mientras que otras pueden requerir que se habilite explícitamente MFA por usuario. Compruebe que no ha excluido ningún usuario de la implementación de MFA actual. Las cuentas de usuario que se excluyan e inicien sesión en el Centro de partners para realizar cualquier actividad relacionada con CSP, CPV o Advisor pueden hacer que las métricas no sean del 100 %.

### <a name="review-your-mfa-conditions"></a>Revisión de las condiciones de MFA

Comprende si la implementación actual solo aplica MFA en condiciones específicas. Algunas soluciones MFA proporcionan flexibilidad para aplicar MFA solo cuando se cumplen ciertas condiciones. Por ejemplo, el usuario obtiene acceso desde un dispositivo desconocido o una ubicación desconocida. Un usuario que esté habilitado para MFA pero que no se requiera que complete la comprobación de MFA al acceder al Centro de partners, puede provocar que las métricas no sean del 100%.

>[!NOTE]
>En el caso de los partners que han implementado MFA con los valores predeterminados de seguridad de Azure AD, es importante tener en cuenta que, para ninguna de las cuentas de usuario de administrador, se aplicará la autenticación multifactor según el riesgo. A los usuarios se les pedirá MFA solo durante los intentos de inicio de sesión de riesgo (por ejemplo, el usuario inicia sesión desde una ubicación diferente). Además, los usuarios tendrán hasta 14 días para registrarse para MFA. A los usuarios que no hayan completado el registro de MFA no se les solicitará la comprobación de MFA durante el período de 14 días. Por lo tanto, se espera que las métricas puede que no sean del 100 % para los partners que han implementado MFA con los valores por defecto de seguridad de Azure AD.

### <a name="review-third-party-mfa-configurations"></a>Revisión de las configuraciones de MFA de terceros

Si usas una solución de MFA de terceros, identifica cómo se integra con Azure AD. En general, hay dos métodos, incluidos los controles personalizados y de federación:

* **Federación de identidades**: cuando Azure AD recibe una solicitud de autenticación, Azure AD redirigirá al usuario al proveedor de identidades federado para la autenticación. Tras una autenticación correcta, el proveedor de identidades federado redirigirá al usuario a Azure AD junto con un token SAML. Para que Azure AD reconozca que el usuario ha completado la comprobación de MFA al autenticarse en el proveedor de identidades federado, el token SAML debe incluir la notificación *authenticationmethodsreferences* (con el valor *multipleauthn*). Compruebe si el proveedor de identidades federado admite la emisión de este tipo de notificaciones. Si es así, compruebe si el proveedor de identidades federado se ha configurado para ello. Si falta la notificación, Azure AD (y, por tanto, el Centro de partners) no sabrá que el usuario ha completado la verificación MFA y esto puede hacer que la métrica no sea del 100 %.

* **Control personalizado**: el control personalizado de Azure AD no se puede usar para identificar si un usuario ha completado la verificación MFA mediante una solución MFA de terceros. Como resultado, cualquier usuario que haya completado la comprobación de MFA a través de un control personalizado aparecerá siempre en Azure AD (y, a su vez, en el Centro de partners) como si no hubiera completado dicha comprobación. Siempre que sea posible, se recomienda usar la Federación de identidades en lugar de un Control personalizado al integrar con Azure AD.

### <a name="identify-which-users-have-signed-in-to-partner-center-without-mfa"></a>Identificar qué usuarios han iniciado sesión en el Centro de partners sin MFA

Puede ser útil identificar los usuarios que inician sesión en el Centro de partners sin comprobación de MFA y comprobarlos con la implementación de MFA actual. Puede usar el [informe de inicio de sesión de Azure AD ](/azure/active-directory/reports-monitoring/concept-sign-ins) para averiguar si un usuario ha completado la comprobación de MFA o no. Actualmente, el informe de inicio de sesión de Azure AD solo está disponible para los partners que se han suscrito a Azure AD Premium o a cualquier SKU de O365, lo que incluye Azure AD Premium (por ejemplo, EMS).

## <a name="next-steps"></a>Pasos siguientes

- [Comunidad de grupos de guías de seguridad del Centro de partners](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)
- [Requisitos de seguridad del Centro de partners](partner-security-requirements.md)
- [Preguntas más frecuentes sobre los requisitos de seguridad del Centro de partners](partner-security-requirements-faq.md)
