---
title: Requisitos de seguridad de asociados | Centro de partners
ms.topic: article
ms.date: 06/25/2019
description: Obtenga información sobre los requisitos de seguridad para los asesores y asociados que participan en el programa proveedor de soluciones en la nube.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, el proveedor de soluciones en la nube, Cloud Solution Provider programar, CSP, el proveedor del Panel de Control, CPV, autenticación multifactor, MFA, proteger el modelo de aplicación, modelo de aplicaciones seguro, seguridad
ms.localizationpriority: medium
ms.openlocfilehash: de1452ce14c8343e2e05dcc65a7a6c05259576c5
ms.sourcegitcommit: ca7f000a58575fa9a089693256c095120dde3c5d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/24/2019
ms.locfileid: "67347004"
---
# <a name="partner-security-requirements"></a>Requisitos de seguridad asociados

**Se aplica a**

- Todos los asociados en el programa proveedor de soluciones en la nube
  - Bill directa
  - Proveedor indirecto
  - Revendedor indirecto
- Todos los proveedores de Panel de Control
- Todos los asesores

Seguridad y privacidad de los clientes y asociados son las principales prioridades para Microsoft. Seguimos ver un número creciente de más sofisticados ataques de seguridad, principalmente relacionados con las identidades en peligro. Como los controles preventivos desempeñan un papel clave en una estrategia de defensa global para frustrar los ataques de seguridad, comenzaremos a imponer un conjunto de requisitos de seguridad para ayudar a proteger los socios y sus clientes.

> [!NOTE]
> Se recomienda encarecidamente que todos los asociados de intercambiar a través de una nube soberana (21Vianet, gobierno de Estados Unidos y Alemania) actuarán y adoptarán estos nuevos requisitos de seguridad inmediatamente. Sin embargo, estos asociados no tienen que cumplir los nuevos requisitos de seguridad efectivos el 1 de julio. Microsoft proporcionará detalles adicionales sobre el cumplimiento de estos requisitos de seguridad para las nubes independientes en el futuro.

## <a name="overview-of-the-requirements"></a>Información general de los requisitos

Todos los asociados que participan en el programa proveedor de soluciones en la nube, los proveedores del Panel de Control y socios de Advisor son necesarios para aplicar la autenticación multifactor (MFA) para cada usuario en su inquilino de partner. Esto puede hacerse mediante la habilitación de dos [directivas de línea de base de Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection). Las directivas de línea de base son un conjunto de directivas predefinidas que ayudan a proteger frente a ataques comunes muchas de las organizaciones. Estos ataques comunes pueden incluir "phishing", reproducción y protector de contraseña. Las directivas de línea de base están disponibles en todas las ediciones de Azure Active Directory. Microsoft ha realizado estas directivas de protección de la línea base disponible para todos los usuarios porque los ataques basados en la identidad han ido en aumento durante los últimos años.

Se describen las directivas de línea de base de dos que deben estar habilitadas en la tabla siguiente.

|**Directiva**| |
|-----|-----|
|**Requerir MFA para que los administradores**|La exigencia de MFA para la directiva de administradores, deberá habilitar los usuarios de los roles de administrador deben registrarse en MFA mediante la aplicación de autenticador. Una vez completado el registro de MFA, los administradores deberán realizar MFA cada vez que inicien sesión en.|
|**Protección del usuario final**|Protección del usuario final es una directiva de línea de base MFA basadas en riesgos que protege todos los usuarios en un directorio. Si habilita esta directiva requiere que todos los usuarios deben registrarse en MFA mediante la aplicación de autenticador. Los usuarios pueden omitir el símbolo del sistema de registro MFA durante 14 días, tras el cual se bloqueará de iniciar sesión hasta que se registren en MFA. Una vez registrado para MFA, se pedirá a los usuarios para MFA solo durante los intentos de inicio de sesión de riesgo. Las cuentas de usuario en peligro se bloquean hasta que se restablece su contraseña y los eventos de riesgo se han descartado.|

Cuando se habilitan estas directivas, cada usuario podrá usar Azure MFA sin costo adicional. Si usa una solución de terceros, se deben aplicar MFA para cada usuario al tener acceso a servicios en la nube de Microsoft Commercial.

> [!IMPORTANT]
> Puesto que todos los usuarios en el directorio de asociados, se exige MFA, habrá un impacto en cualquier automatización o integración que utiliza las credenciales de usuario. Para abordar este impacto en que deberá modificar la forma la automatización o la integración se conecta a los servicios comerciales en la nube de Microsoft. Si el servicio se está conectando a admite la autenticación basada en token, a continuación, se recomienda que implemente la [marco de modelo de aplicación Secure](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model).

## <a name="what-actions-do-i-need-to-take"></a>¿Las acciones que es necesario realizar? 

Para asegurarse de que cada usuario en el asociado está protegido, debe habilitar la [exigencia de MFA para que los administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) y [protección del usuario final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) directivas básicas. Antes de habilitar estas directivas, es importante comprender qué hacen y cómo afectan a cualquier cliente de automatización o integración y los usuarios.

### <a name="considerations"></a>Consideraciones

Dado que los requisitos de seguridad se aplican a todos los usuarios en un directorio de socios, varias consideraciones deben realizarse para garantizar una implementación sin problemas. Estas consideraciones son la identificación de los usuarios de Azure Active Directory que no se puede o no se debe realizar la MFA, así como las aplicaciones y los clientes usados por la organización que no admiten la autenticación moderna.

#### <a name="legacy-protocols"></a>Protocolos heredados

Protocolos de autenticación heredados (IMAP, SMTP, POP3, etc.) se usan los clientes de correo para realizar solicitudes de autenticación. Estos protocolos no son compatibles con MFA. La mayoría de las cuentas comprometidas vistos por Microsoft está provocada por los actores no válidos la realización de ataques contra los protocolos heredados intenta omitir MFA. Para asegurarse de que se requiere MFA al iniciar sesión en una cuenta en un directorio de asociados y los actores no válidos no pueden omitir MFA, estos requisitos de seguridad bloqueará todas las solicitudes de autenticación de protocolos heredados.

### <a name="enabling-the-baseline-policies"></a>Habilitar las directivas de línea base

Consulte la [implementar el tutorial de requisitos de seguridad asociado](tutorials/partner-security-requirements.yml) para una experiencia guiada sobre la implementación de las directivas de línea de base.  

#### <a name="require-mfa-for-admins"></a>Requerir MFA para que los administradores

El *exigencia de MFA para la administración* directiva básica requiere MFA para los siguientes roles de directorio, considera que los roles de Azure Active Directory con más privilegios:

- Administrador global
- Administrador de SharePoint
- Administrador de Exchange
- Administrador de acceso condicional
- Administrador de seguridad
- Administrador de soporte técnico o administrador de contraseñas
- Administrador de facturación
- Administrador de usuarios

Tras la habilitación de la exigencia de MFA para los administradores directiva, los roles de nueve administrador anterior deberán registrarse en MFA mediante la aplicación Authenticator. Una vez completado el registro de MFA, los administradores deberán realizar MFA cada vez que inicio de sesión único.

Si su organización tiene estas cuentas en uso en scripts o código, considere la posibilidad de reemplazarlos con [administra identidades](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview).

Para habilitar esta directiva y proteger a los administradores:

1. Inicie sesión en el **portal Azure** como un administrador Global, Administrador de seguridad o administrador de acceso condicional.
2. Vaya a **Azure Active Directory** > **acceso condicional**.
3. En la lista de directivas, seleccione **directiva de línea base: Requerir MFA para que los administradores**.
4. Establecer **Habilitar directiva** a **usar la directiva inmediatamente**.
5. Haga clic en **guardar**.

    ![Requerir MFA para que los administradores](images/security/baseline-policy-require-mfa-for-admins.png)

> [!WARNING]
> Antes de habilitar esta directiva, asegúrese de que los usuarios no usan protocolos de autenticación heredados. Consulte el artículo [Cómo: Autenticación heredados de bloque a Azure Active Directory con acceso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use) para obtener más información.

> [!IMPORTANT]
> Hay un problema conocido, lo que afecta a su capacidad para conectarse a Exchange Online PowerShell con privilegios de administrador delegados. Consulte la [Exchange Online PowerShell](#exchange-online-powershell) conocido problema antes de habilitar esta directiva si usa este módulo de PowerShell.

#### <a name="end-user-protection"></a>Protección del usuario final

La directiva de línea de base de usuarios finales protection protege todos los usuarios en un directorio. Si habilita esta directiva requiere que todos los usuarios se registren para Azure MFA en 14 días. Una vez registrado, se pedirá a los usuarios para MFA solo durante los intentos de inicio de sesión de riesgo. Las cuentas de usuario en peligro se bloquean hasta que el restablecimiento de contraseña y el riesgo de despido.

La directiva **directiva de línea base: Protección del usuario final** viene previamente configurada y se mostrarán en la parte superior cuando vaya a la hoja de acceso condicional en Azure portal.

Para habilitar esta directiva y proteger a los usuarios:

1. Inicie sesión en el **portal Azure** como un administrador Global, Administrador de seguridad o administrador de acceso condicional.
2. Vaya a **Azure Active Directory** > **acceso condicional**.
3. En la lista de directivas, seleccione **directiva de línea base: Protección del usuario final (versión preliminar)** .
4. Establecer **Habilitar directiva** a **usar la directiva inmediatamente**.
5. Haga clic en **guardar**.

    ![Protección del usuario final](images/security/baseline-policy-end-user-protection.png)

> [!WARNING]
> Antes de habilitar esta directiva, asegúrese de que los usuarios no usan protocolos de autenticación heredados. Consulte el artículo [Cómo: Autenticación heredados de bloque a Azure Active Directory con acceso condicional](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-legacy-auth#identify-legacy-authentication-use) para obtener más información.

> [!IMPORTANT]
> No hay problemas conocidos que afectan a la capacidad para conectarse a Exchange Online PowerShell con privilegios de administrador delegados. Consulte la [Exchange Online PowerShell](#exchange-online-powershell) conocido problema antes de habilitar esta directiva si usa este módulo de PowerShell.

## <a name="common-issues"></a>Problemas comunes

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

Después de habilitar las directivas de línea de base, es posible que la automatización o la integración está produciendo una excepción similar al siguiente

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

La razón de esta excepción es que se autentican con credenciales de usuario y MFA ahora es necesario. Para solucionar esta excepción, deberá usar un token de acceso para la autenticación. Consulte la [Guía del modelo de aplicación Secure](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) para obtener más información.

>[!IMPORTANT]
>Módulos de PowerShell y API más modernos admiten la capacidad de utilizar un token de acceso para la autenticación. Sin embargo, hay algunos que actualmente no se admite esta funcionalidad. Si necesita ayuda para determinar si el módulo de PowerShell o de API que intenta aprovechar admite el uso de un token de acceso para la autenticación, a continuación, publicar un mensaje en el [grupo de instrucciones de seguridad de Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) Comunidad.

#### <a name="aadsts700082"></a>AADSTS700082

Cuando haya implementado el marco de trabajo del modelo de aplicación Secure es probable que recibirá la siguiente excepción 90 días después de generar el token de actualización inicial

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

Con respecto a Azure Active Directory la duración máxima para una actualización de token es de 90 días. Para corregir este error, deberá generar y almacenar de forma segura un nuevo token de actualización. Tenga en cuenta que es posible actualizar el token de actualización mediante programación porque con cada solicitud a Azure Active Directory para un token de acceso se devuelve un nuevo token de actualización. Puede implementar la lógica adecuada para actualizar el token de actualización almacenada de forma segura antes de que expire.

Consulte [vigencia de tokens Configurable en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) para obtener más información.

## <a name="known-issues"></a>Problemas conocidos

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

Cuando se habilita MFA asociados no podrá usar sus privilegios de administración delegadas con Exchange Online mediante PowerShell para realizar acciones con sus clientes. Consulte [conectarse a Exchange Online PowerShell mediante la autenticación multifactor](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell) para obtener más información sobre esta limitación.

## <a name="resources-and-support"></a>Recursos y soporte técnico

A través de la [Comunidad de grupo de instrucciones de seguridad de Partner Center](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) se puede encontrar recursos adicionales y obtenga información sobre los próximos eventos tales como el horario de oficina técnica. Consulte la [preguntas más frecuentes](http://assetsprod.microsoft.com/security-requirements-faq.pdf) documento para obtener más información sobre los requisitos.

### <a name="developers"></a>Desarrolladores

- [Habilitar el modelo de aplicaciones seguras](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Ejemplos de .NET de centro de partners](https://github.com/microsoft/partner-center-dotnet-samples)
- [Ejemplos de Java del centro de partners](https://github.com/microsoft/partner-center-java-samples)
- [Implementar el modelo de aplicación segura de PowerShell de centro de partners](https://docs.microsoft.com/powershell/partnercenter/secure-app-model)
