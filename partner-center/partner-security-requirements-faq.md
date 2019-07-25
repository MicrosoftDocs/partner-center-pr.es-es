---
title: Preguntas más frecuentes sobre los requisitos de seguridad de asociados | Centro de Partners
ms.topic: article
ms.date: 07/18/2019
description: Preguntas más frecuentes sobre los requisitos de seguridad del asociado
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, proveedor de soluciones en la nube, programa del proveedor de soluciones en la nube, CSP, proveedor del panel de control, CPV, autenticación multifactor, MFA, modelo de aplicación segura, modelo de aplicación segura, seguridad
ms.localizationpriority: medium
ms.openlocfilehash: 1a178dc71f8042e6b39a316c6c889b619aaed12c
ms.sourcegitcommit: 5c8ac1b6d29d183d85582d6eb32e37b91dd8c6c1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/18/2019
ms.locfileid: "68315554"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Preguntas más frecuentes sobre los requisitos de seguridad del asociado

Este artículo contiene algunas preguntas frecuentes sobre los [requisitos de seguridad](partner-security-requirements.md)de los asociados. Puede encontrar una lista completa de las preguntas más frecuentes [aquí](http://assetsprod.microsoft.com/security-requirements-faq.pdf).

## <a name="conditional-access"></a>Acceso condicional

### <a name="can-conditional-access-be-used"></a>¿Se puede usar el acceso condicional?

Sí, puede usar el acceso condicional para aplicar MFA a cada usuario, incluidas las cuentas de servicio, en el inquilino del asociado. Sin embargo, dada la naturaleza con privilegios elevados de ser un asociado, es necesario asegurarse de que cada usuario tenga un desafío de MFA para cada autenticación. Esto significa que no podrá aprovechar la característica de acceso condicional que evita el requisito de MFA.

## <a name="multi-factor-authentication"></a>Multi-Factor Authentication

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>¿Los clientes están sujetos a los requisitos de seguridad de los asociados?

No, no es necesario aplicar MFA para cada usuario en los inquilinos de Azure AD del cliente. Sin embargo, se recomienda que trabaje con cada cliente para determinar la mejor manera de proteger a sus usuarios.

### <a name="can-app-passwords-be-used-with-the-baseline-protection-policies"></a>¿Se pueden usar contraseñas de aplicación con las directivas de protección de línea de base?

Sí, se pueden usar las contraseñas de [aplicación](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) . Debe revisar las consideraciones sobre el uso de contraseñas de aplicación que se documentan [aquí](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) para determinar si son compatibles con sus necesidades.

### <a name="can-any-user-be-excluded-from-this-requirement"></a>¿Se puede excluir cualquier usuario de este requisito? 

No, todos los usuarios, incluidas las cuentas de servicio, del inquilino de asociado deberán autenticarse mediante MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>¿Se aplican los requisitos de seguridad del asociado al espacio aislado de integración?

Sí, los requisitos de seguridad del asociado se aplican al espacio aislado de integración. Esto significa que deberá implementar la solución MFA adecuada para los usuarios del inquilino de espacio aislado de integración. Se recomienda implementar las directivas de protección de línea de base para proporcionar MFA.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>¿Cómo configurar una cuenta de acceso de emergencia?

Se consideró una práctica recomendada para crear una o dos cuentas de acceso de emergencia para evitar que se bloquee de forma inadvertida del inquilino de Azure AD. Con respecto a los requisitos de seguridad de los asociados, es necesario que cada usuario se autentique mediante MFA. Por lo tanto, esto significa que tendrá que modificar la definición de una cuenta de acceso de emergencia. Podría tratarse de una cuenta que aprovecha una solución de terceros para MFA.

### <a name="how-will-guest-users-be-impacted-by-the-partner-security-requirements"></a>¿Cómo se verán afectados los usuarios invitados por los requisitos de seguridad del asociado?

Los usuarios invitados deberán autenticarse mediante MFA, al acceder a los recursos de su inquilino de asociado. Los requisitos de seguridad del asociado no tendrán ningún impacto en el usuario invitado para acceder a los recursos de su propio inquilino.

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>Si utilizo una solución de terceros Active Directory Servicio de federación (ADFS) necesario? 

No, no es necesario tener Active Directory Servicio de federación (ADFS) si usa una solución de terceros. Se recomienda que trabaje con el proveedor de la solución para determinar cuáles son los requisitos de su solución.

### <a name="is-it-a-requirement-to-enable-the-baseline-protection-policies"></a>¿Es necesario habilitar las directivas de protección de línea de base?

No, no es necesario habilitar las directivas de protección de línea de base. El único requisito es que aplique MFA para cada usuario, incluidas las cuentas de servicio, en el inquilino del asociado.

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>¿Qué opciones de comprobación se proporcionan a través de la implementación de las directivas de protección de línea de base? 

Con respecto a la versión de MFA que está disponible a través de la implementación de las directivas de protección de línea de base, la única opción de comprobación disponible es una aplicación autenticadora. El uso de un mensaje de llamada de teléfono y mensaje de texto se considera menos seguro. Por lo tanto, estas opciones no están disponibles a través de esta versión de MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>¿La cuenta de servicio usada por Azure AD Connect se verá afectada por los requisitos de seguridad del asociado?

No, la cuenta de servicio usada por Azure AD Connect no se verá afectada por los requisitos de seguridad del asociado. Si experimenta un problema con Azure AD Connect como consecuencia de la aplicación de MFA, abra una solicitud de soporte técnico con el soporte técnico de Microsoft.
