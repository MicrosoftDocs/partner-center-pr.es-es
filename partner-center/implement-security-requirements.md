---
title: Implementar los requisitos de seguridad para partners
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtener información sobre cómo implementar los requisitos de seguridad necesarios para los usuarios
author: LauraBrenner
ms.author: labrenne
keywords: security
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: d162e8c5fd3cfd335920e4cc5fc826c3622f633c
ms.sourcegitcommit: 562535a4b16a8217c1e1945b7663ca3735e1ee27
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/22/2020
ms.locfileid: "85133274"
---
# <a name="implement-the-partner-security-requirements"></a>Implementar los requisitos de seguridad para partners

**Roles adecuados**

- Administrador global

La seguridad y privacidad de los clientes y asociados son las máximas prioridades de Microsoft. Seguimos observando un número creciente de ataques de seguridad más sofisticado, que están relacionados principalmente con identidades en riesgo. Como los controles preventivos juegan un papel clave en una estrategia de defensa general para frustrar los ataques de seguridad, comenzaremos a aplicar un conjunto de requisitos de seguridad obligatorios para ayudar a proteger a los partners y sus clientes.

A través de este tutorial, obtendrás más información sobre los requisitos de seguridad de los asociados, cómo cumplirlos y el impacto para los usuarios de tu directorio de asociados.

Todos los asociados que participan en el programa Proveedor de soluciones en la nube, los proveedores de panel de control y los asociados de Advisor deben aplicar Multi-Factor Authentication (MFA) para cada usuario en su inquilino de asociado. Para aplicar este servicio, se pueden habilitar dos [directivas de base de referencia de Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection). Las directivas de línea de base son un conjunto de directivas predefinidas que ayudan a proteger las organizaciones frente a muchos ataques comunes. Estos ataques comunes pueden incluir la difusión de contraseña, la reinyección y la suplantación de identidad. Las directivas de base de referencia están disponibles en todas las ediciones de Azure Active Directory. Microsoft está poniendo estas directivas de protección de base de referencia a disposición de todo el mundo porque los ataques basados en la identidad han aumentado en los últimos años.

En los procedimientos siguientes se describe el proceso de habilitación de las dos directivas de base de referencia necesarias:

- **Requerir MFA a los administradores**  La habilitación de la directiva Requerir MFA a los administradores requiere que los usuarios que tengan roles de administrador se registren en MFA mediante la aplicación de autenticación. Una vez que se complete el registro de MFA, los administradores deberán realizar la autenticación multifactor cada vez que inicien sesión.

- **End user protection** End user protection (Protección del usuario final) es una directiva de base de MFA basada en el riesgo que protege a todos los usuarios de un directorio. La habilitación de esta directiva requiere que todos los usuarios se registren para MFA mediante la aplicación de autenticación. Los usuarios pueden hacer caso omiso la solicitud de registro en MFA durante 14 días, pero tras ese periodo se les impedirá iniciar sesión hasta que se registren en MFA. Una vez que se hayan registrado, solo se solicitará a los usuarios la autenticación multifactor en los intentos de inicio de sesión peligrosos. Las cuentas de usuario en peligro se bloquean hasta que se restablece su contraseña y han desaparecido los eventos de riesgo.

Cuando estas directivas están habilitadas, todos los usuarios pueden usar Azure MFA sin ningún costo adicional. Si usas una solución de terceros, debes aplicar MFA para cada usuario al acceder a los servicios en la nube comerciales de Microsoft.

>[!NOTE]
>Puesto que se aplicará MFA para todos los usuarios del directorio de asociados, se producirá un impacto en cualquier automatización o integración que use las credenciales de usuario. Para abordar este impacto, tendrás que modificar la forma en que la automatización o integración se conecta a los servicios en la nube comerciales de Microsoft. Si el servicio al que te estás conectando admite la autenticación basada en tokens, se recomienda que implementes el [marco del modelo de aplicaciones seguras](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).

## <a name="step-one-block-any-existing-legacy-authentication-protocols"></a>Paso uno: Bloquear los protocolos de autenticación heredados existentes

Antes de habilitar las directivas Requerir MFA a los administradores y protección de usuarios finales, asegúrese de que los usuarios no utilicen protocolos de autenticación heredados. Consulta el artículo [Procedimientos para: Bloqueo de la autenticación heredada en Azure AD con acceso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection#identify-legacy-authentication-use) para obtener más información.

## <a name="step-two-enable-the-require-mfa-for-admins-baseline-policy"></a>Segundo paso: Habilitar la directiva de base de referencia Requerir MFA a los administradores?

La directiva de base de referencia Requerir MFA a los administradores requiere MFA para los siguientes roles de directorio, que se consideran los roles de Azure AD con más privilegios:

- Administrador global
- Administrador de SharePoint
- Administrador de Exchange
- Administrador de acceso condicional
- Administrador de seguridad
- Administrador de soporte técnico/administrador de contraseñas
- Administrador de facturación
- Administrador de usuarios

Tras la habilitación de la directiva Requerir MFA a los administradores los nueve roles de administrador anteriores tendrán que registrarse en MFA mediante la aplicación de autenticación. Una vez que se complete el registro de MFA, los administradores deberán realizar la autenticación multifactor cada vez que inicien sesión.

Si tu organización tiene estas cuentas en uso en scripts o código, considera la posibilidad de reemplazarlas por [identidades administradas](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).

Para habilitar esta directiva y proteger a los administradores:

1. Inicia sesión en  **Azure Portal** como administrador global, administrador de seguridad o administrador de acceso condicional.

2. Vaya a **Azure Active Directory** > **Acceso condicional**.

3. En la lista de directivas, selecciona **Directiva de línea de base: Requerir MFA a los administradores**.

4. En **Habilitar directiva**, selecciona **Usar la directiva inmediatamente**.

5. Seleccione  **Guardar**.

Una vez habilitada esta directiva, se solicitará a los usuarios de los roles de administrador anteriores que inicien sesión para proporcionar información de seguridad adicional y configurar la aplicación móvil. Una vez completado, podrán iniciar sesión en el servicio en la nube adecuado.

## <a name="step-three-enable-the-end-user-protection-baseline-policy"></a>Tercer paso: Habilitar la directiva Protección del usuario final

La directiva de línea de base End user protection (Protección del usuario final) protege a todos los usuarios de un directorio. La habilitación de esta directiva requiere que todos los usuarios se registren para Azure MFA en un plazo máximo de 14 días. Una vez registrado, solo se solicitará a los usuarios que ejecuten MFA durante los intentos de inicio de sesión peligrosos. Este comportamiento cambiará en el futuro para los inquilinos asociados. Las cuentas de usuario en peligro se bloquean hasta que se restablece la contraseña y el riesgo desaparece.

La directiva Directiva de base de referencia: End user protection (Protección del usuario final) viene preconfigurada y se mostrará en la parte superior al desplazarse a la hoja Acceso condicional en Azure Portal.

Para habilitar esta directiva y proteger a los usuarios:

1. Inicia sesión en  **Azure Portal** como administrador global, administrador de seguridad o administrador de acceso condicional.

2. Vaya a **Azure Active Directory** > **Acceso condicional**.

3. En la lista de directivas, selecciona **Directiva de línea de base: End user protection (preview) [Protección del usuario final (versión preliminar)]** .

4. En **Habilitar directiva**, selecciona **Usar la directiva inmediatamente**.

5. Seleccione  **Guardar**.

Una vez habilitada esta directiva, se solicitará a todos los usuarios que inicien sesión para proporcionar información de seguridad adicional y configurar la aplicación móvil. Una vez completado, podrán iniciar sesión en el servicio en la nube adecuado.

>[!NOTE]
>Hasta que se apliquen los requisitos de seguridad para asociados, a los usuarios que no estén cubiertos por la directiva de base de referencia Requerir MFA a los administradores solo se les pedirá MFA en función del riesgo.