---
title: Requisitos de seguridad para partners | Centro de partners
ms.topic: article
ms.date: 08/30/2019
description: Obtén información acerca los requisitos de seguridad para los asesores y partners que participan en el programa Proveedor de soluciones en la nube.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider program, CSP, Control Panel Vendor, CPV, multi-factor authentication, MFA, secure application model, secure app model, security
ms.localizationpriority: medium
ms.openlocfilehash: c95ec38f928ca4032ffecebaf25f23e87d10c079
ms.sourcegitcommit: de3cdc792b6b4bbc64d1288d371623d79d535205
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/03/2019
ms.locfileid: "70215646"
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

A partir del 1 de agosto de 2019 todos los partners tienen la obligación de aplicar la autenticación multifactor a todos los usuarios, incluidas las cuentas de servicio, en su inquilino del partner.

> [!NOTE]
> Se recomienda encarecidamente a todos los partners que realicen transacciones a través de una nube soberana (21Vianet, gobierno de EE. UU. y Alemania) adopten estos nuevos requisitos de seguridad de inmediato. Sin embargo, no es preciso que estos partners cumplan los nuevos requisitos de seguridad que entran en vigor el 1 de agosto de 2019. En el futuro, Microsoft proporcionará más información acerca de la aplicación de estos requisitos de seguridad para las nubes soberanas.

Los términos asociados a los requisitos de seguridad para partners se han agregado a la [guía del programa Proveedor de soluciones en la nube](https://go.microsoft.com/fwlink/p/?LinkId=617100). A partir del 1 de agosto de 2019, todos los partners que participen en el programa Proveedor de soluciones en la nube deben cumplir los términos y condiciones. En lo que se refiere a los asesores, se aplicarán los mismos requisitos contractuales.

Los partners que no implementen los requisitos de seguridad obligatorios no podrán realizar transacciones en el programa Proveedor de soluciones en la nube ni administrar los inquilinos del cliente que aprovechen los derechos de administrador delegado, una vez que se apliquen estos requisitos. Estamos en el proceso de establecer una fecha de aplicación técnica de los requisitos y se la notificaremos a los partners con información detallada.

## <a name="what-actions-do-i-need-to-take"></a>¿Qué acciones necesito realizar?

Dada la naturaleza de los partners, que tienen privilegios elevados, necesitamos asegurarnos de que cada usuario tenga que usar la MFA en todas y cada una de las autenticaciones. Esto se puede realizar de cualquiera de estas maneras:

- Mediante la implementación de Azure AD Premium y asegurándose de que se aplica MFA a todos los usuarios.
- Mediante la implementación de las [directivas de protección de línea de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).
- Mediante la implementación de una solución de terceros y asegurándose de que se aplica MFA a todos los usuarios.

> [!IMPORTANT]
> Una vez que estos requisitos se aplican técnicamente, todas y cada una de las autenticaciones deben tener un desafío de MFA. No se podrá usar ninguna característica del acceso condicional para evitar la autenticación mediante MFA al acceder a los servicios en la nube comercial de Microsoft.

### <a name="considerations"></a>Consideraciones

Dado que estos requisitos se aplican a todos los usuarios, incluidas las cuentas de servicio, del inquilino del partner deben hacerse varias consideraciones para garantizar que la implementación se realiza sin problemas. Entre estas consideraciones se incluye la identificación en Azure AD de los usuarios que no pueden realizar MFA, así como de las aplicaciones y los dispositivos usados por una organización que no admiten la autenticación moderna.

Antes de realizar cualquier acción, es aconsejable identificar los siguientes factores

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>¿Hay alguna una aplicación o un dispositivo que no admita el uso de MFA al autenticarse?

Cuando se aplique la autenticación heredada de MFA, se bloqueará el uso de protocolos como IMAP, POP3, SMTP, etc., ya que no admiten MFA. Para solucionar esta limitación, se puede usar una característica conocida como [contraseñas de aplicación](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) para asegurarse de que la aplicación o el dispositivo se pueden autenticar. Debes examinar las consideraciones acerca del uso de contraseñas, que están documentadas [aquí](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords), aquí para determinar si se pueden usar en su entorno.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>¿Hay usuarios que usen Office 365 proporcionados por licencias asociadas a tu inquilino del partner?

Antes de implementar cualquier solución, es aconsejable determinar qué versión de Microsoft Office utilizan los usuarios de tu inquilino del partner. Examina el [plan para realizar la autenticación multifactor en implementaciones de Office 365](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa) antes de realizar cualquier acción. Existe la posibilidad de que los usuarios tengan problemas de conectividad con aplicaciones como Outlook. Antes de aplicar la autenticación multifactor, es importante asegurarse de que se usa Outlook 2013 SP1, o cualquier versión posterior, y que la organización tiene habilitada la autenticación moderna. Para más información, consulta [Habilitar la autenticación moderna en Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online).

Para habilitar la autenticación moderna en cualquier dispositivo con Windows que tenga Microsoft Office 2013 instalado, es preciso crear dos claves del Registro. Consulta [Habilitar autenticación moderna para Office 2013 en dispositivos Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).

> [!IMPORTANT]
> Si has habilitado a los usuarios para Azure AD MFA y tienen dispositivos en los que se ejecuta Office 2013 que no están habilitados para la autenticación moderna, deberán usar contraseñas de aplicaciones en esos dispositivos. Aquí se puede encontrar más información acerca de las contraseñas de aplicaciones y cuándo, dónde y cómo se deben usar: [Contraseñas de aplicaciones con Azure Multi-Factor Authentication](https://go.microsoft.com/fwlink/p/?LinkId=528178).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>¿Hay alguna directiva que impida que los usuarios usen sus dispositivos móviles mientras trabajan?

Es importante identificar las directivas corporativas que impiden que los empleados usen dispositivos móviles mientras trabajan, ya que esto influirá en la solución MFA que implementes. Hay soluciones MFA, como la que se proporciona a través de la implementación de las [directivas de protección de línea de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection), que solo permiten el uso de una aplicación de autenticación para la comprobación. Si la organización tiene una directiva que impide el uso de dispositivos móviles, debes tener en cuenta una de las siguientes opciones:

- Implementar una aplicación de contraseñas de un solo uso y duración definida (TOTP) que se pueda ejecutar en un sistema seguro.
- Implementar una solución de terceros que aplique MFA a todos los usuarios del inquilino del partner que proporcione la opción de comprobación más adecuada.
- Comprar licencias de [Azure AD Premium](https://azure.microsoft.com/pricing/details/active-directory/) para los usuarios afectados.

La compatibilidad con el uso de las claves de seguridad de FIDO se encuentra en el plan de desarrollo de las directivas de protección de línea de base. Una vez agregada la compatibilidad, podrá aprovechar las claves de seguridad de FIDO para el segundo factor de autenticación. Hasta entonces, está limitado al uso de la aplicación de autenticación.

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>¿Qué automatización o integración tienes que aproveche las credenciales de usuario para la autenticación?

Como el requisito es aplicar MFA a todos los usuarios, incluidas las cuentas de servicio, del directorio de partners cualquier automatización o integración que aproveche las credenciales de usuario para la autenticación se verá afectada. Por tanto, es importante identificar qué cuentas se usan en estas situaciones. A continuación se muestra una lista de ejemplos de aplicaciones o servicios que se deben tener en cuenta

- Panel de control que se usa usado para aprovisionar recursos en nombre de los clientes
- Integración con todas las plataformas que se utilicen para la facturación (en relación con el programa CSP) y soporte técnico a los clientes
- Scripts de PowerShell que usan los módulos Az, AzureRM, Azure AD, MS Online, etc.

La lista anterior no es completa. Por tanto, es importante que realices una evaluación completa de cualquier aplicación o servicio de tu entorno que aproveche las credenciales de usuario para la autenticación. Para enfrentarse al requisito de MFA, debes implementar las instrucciones del [marco de modelo de aplicaciones seguras](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) siempre que sea posible. Los siguientes son recursos adicionales que te ayudarán a saber cómo se puede implementar el marco de modelo de aplicaciones seguras

- [Ejemplos de .NET del Centro de partners](https://github.com/microsoft/partner-center-dotnet-samples): este repositorio de GitHub contiene ejemplos que se han desarrollados mediante .NET y que muestran cómo se puede implementar el marco de modelo de aplicaciones seguras.
- [Ejemplos de Java del Centro de partners](https://github.com/microsoft/partner-center-java-samples): este repositorio de GitHub contiene ejemplos que se han desarrollados mediante Java y que muestran cómo se puede implementar el marco de modelo de aplicaciones seguras.
- [Partner Center PowerShell (modelo de aplicaciones seguras)](https://docs.microsoft.com/powershell/partnercenter/secure-app-model): en este artículo se proporcionan datos acerca de cómo implementar el marco de modelo de aplicaciones seguras mediante PowerShell.
- [Comunidad del grupo de instrucciones de seguridad del Centro de partners](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance): esta es una comunidad en línea en la que no solo puedes obtener información acerca de los próximos eventos, sino también realizar todas las preguntas que puedas tener.

### <a name="enforcing-mfa-for-all-users"></a>Aplicación de MFA a todos los usuarios

En esta sección se explica cómo usar las [directivas de protección de línea de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) para aplicar MFA a todos los usuarios, incluidas las cuentas de servicio, del inquilino del partner. Si planeas usar Azure AD Premium, siga los pasos que se documentan [aquí](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).

> [!NOTE]
> Se puede usar una solución de terceros, que sea compatible con Azure AD, para aplicar MFA a todos los usuarios, incluidas las cuentas de servicio. Para obtener más detalles acerca de cómo se debe implementar la solución, consulta la documentación del proveedor.

Las directivas de protección de línea de base son un conjunto de directivas predefinidas que ayudan a proteger las organizaciones frente a muchos ataques comunes. Estos ataques comunes pueden incluir la difusión de contraseña, la reinyección y la suplantación de identidad. Las directivas de protección de línea de base están disponibles en todas las ediciones de Azure Active Directory. Microsoft está poniendo estas directivas de protección de línea de base a disposición de todo el mundo, con el fin de que tanto los clientes como los partners puedan implementar las mejores prácticas de seguridad.

Las dos directivas de protección de línea de base que deben habilitarse se describen en la tabla siguiente.

|**Directiva**| |
|-----|-----|
|**Require MFA for admins** (Requerir MFA a los administradores)|La habilitación de la directiva Require MFA for admins (Requerir MFA a los administradores) requiere que los usuarios que tengan roles de administrador se registren en MFA mediante la aplicación de autenticación. Una vez que se complete el registro de MFA, los administradores deberán realizar la autenticación multifactor cada vez que inicien sesión.|
|**End user protection** (Protección del usuario final)|End user protection (Protección del usuario final) es una directiva de protección de base de MFA basada en el riesgo que protege a todos los usuarios de un directorio. La habilitación de esta directiva requiere que todos los usuarios se registren para MFA mediante la aplicación de autenticación. Los usuarios pueden hacer caso omiso la solicitud de registro en MFA durante 14 días, pero tras ese periodo se les impedirá iniciar sesión hasta que se registren en MFA. Una vez que se hayan registrado, solo se solicitará a los usuarios la autenticación multifactor en los intentos de inicio de sesión peligrosos. Las cuentas de usuario en peligro se bloquean hasta que se restablece su contraseña y han desaparecido los eventos de riesgo.|

Cuando estas directivas están habilitadas, todos los usuarios podrán usar Azure MFA mediante la aplicación de autenticación para realizar la comprobación sin costo adicional.

#### <a name="configure-self-service-password-reset"></a>Configuración del autoservicio de restablecimiento de contraseña

El autoservicio de restablecimiento de contraseña (SSPR) es una característica Azure Active Directory que permite a los usuarios restablecer sus contraseñas sin necesidad de ponerse en contacto con el equipo de soporte técnico. Para poder usar el servicio, los usuarios deben registrarse, o estar registrados, en el autoservicio de restablecimiento de contraseña. Durante el registro, el usuario elige uno o varios métodos de autenticación que ha habilitado su organización.

Cuando la directiva de protección de línea de base [End user protection](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) (Protección del usuario final) está habilitada, todas las cuentas de usuario que corran peligro se bloquearán hasta que se restablezca su contraseña y hayan descartado los eventos de riesgo. Teniendo esto en cuenta, se recomienda que cada usuario, que sea administrador global, realice las siguientes acciones para registrarse en SSPR, para quedarse bloqueado.

1. Vete a la [página de configuración de SSPR](https://aka.ms/ssprsetup).
2. Escribe tu nombre de usuario y contraseña.
3. Configura al menos una de las opciones que se usarán para comprobar tu identidad al restablecer la contraseña.  

Cuando una cuenta haya estado en peligro, el administrador deberá tomar las medidas necesarias para restaurar el acceso del usuario afectado. Para obtener más detalles acerca del proceso de desbloqueo de un usuario, consulta los [pasos necesarios para desbloquear a un usuario](#recovering-compromised-accounts).

#### <a name="require-mfa-for-admins"></a>Require MFA for admins (Requerir MFA a los administradores)

La directiva de línea de base*Require MFA for admins* (Requerir MFA a los administradores) requiere MFA para los siguientes roles de directorio, que se consideran los roles Azure Active Directory con más privilegios:

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
5. Haz clic en **Guardar**.

> [!WARNING]
> Antes de habilitar esta directiva, asegúrese de que los usuarios no usan protocolos de autenticación heredados. Mediante la implementación de esta directiva se bloqueará la autenticación heredada.

> [!IMPORTANT]
> Existe un problema conocido que afecta a la capacidad para conectarse a Exchange Online PowerShell mediante privilegios administrativos delegados. Si usa esta módulo de PowerShell, vea el problema conocido de[Exchange Online PowerShell](#exchange-online-powershell) antes de habilitar esta directiva.

#### <a name="end-user-protection"></a>End user protection (Protección del usuario final)

La directiva de línea de base End user protection (Protección del usuario final) protege a todos los usuarios de un directorio. La habilitación de esta directiva requiere que todos los usuarios se registren para Azure MFA en un plazo máximo de 14 días. Tras el registro solo se solicitará a los usuarios la MFA en los intentos de inicio de sesión peligrosos. Las cuentas de usuario en peligro se bloquean hasta que se restablece la contraseña y el riesgo desaparece.

La directiva **Directiva de línea de base: End user protection (Protección del usuario final)** viene preconfigurada y se mostrará en la parte superior al desplazarse a la hoja Acceso condicional en Azure Portal.

Para habilitar esta directiva y proteger a los usuarios:

1. Inicia sesión en  **Azure Portal** como administrador global, administrador de seguridad o administrador de acceso condicional.
2. Vaya a **Azure Active Directory** > **Acceso condicional**.
3. En la lista de directivas, selecciona **Directiva de línea de base: End user protection (preview) [Protección del usuario final (versión preliminar)]** .
4. En **Habilitar directiva**, selecciona **Usar la directiva inmediatamente**.
5. Haz clic en **Guardar**.

> [!WARNING]
> Antes de habilitar esta directiva, asegúrese de que los usuarios no usan protocolos de autenticación heredados. Mediante la implementación de esta directiva se bloqueará la autenticación heredada.

> [!IMPORTANT]
> Existe un problema conocido que afecta a la capacidad para conectarse a Exchange Online PowerShell mediante privilegios administrativos delegados. Si usa esta módulo de PowerShell, vea el problema conocido de[Exchange Online PowerShell](#exchange-online-powershell) antes de habilitar esta directiva.

## <a name="assessing-your-environment"></a>Evaluación del entorno

Mediante uno de los requisitos de seguridad de partner actuales se obliga a aplicar MFA a todos los usuarios del inquilino del partner. Dado que este requisito se puede cumplir mediante varios métodos diferentes, puede resultar difícil de evaluar si se requieren acciones adicionales. Puedes aprovechar herramientas como los registros de auditoría de Azure Active Directory y [Microsoft Secure Score](https://docs.microsoft.com/office365/securitycompliance/microsoft-secure-score) para evaluar si se requieren más acciones adicional para proteger el inquilino con la autenticación multifactor. Microsoft está trabajando en una experiencia en el Centro de partners para proporcionar una comprobación rápida del cumplimiento de los requisitos de MFA y del modelo de aplicaciones seguras.

Microsoft Secure Score ofrece visualizaciones sólidas, integración con otros productos de Microsoft, comparación de la puntuación con la de otras empresas, filtrado por categoría y mucho más. Con esta herramienta, puedes completar las acciones de mejora de la seguridad dentro de la organización y realizar un seguimiento del historial de la puntuación. La puntuación también puede reflejar si las soluciones de terceros han realizado las acciones de mejora recomendadas.

![Microsoft Secure Score](images/security/secure-score.png)

> [!NOTE]
> Las acciones que puedes llevar a cabo para mejorar Microsoft Secure Score pueden tardar hasta 24 horas en reflejarse.

Microsoft Secure Score solo proporcionará una representación numérica de la postura de seguridad. Para saber mejor qué o quién realiza la autenticación sin que sea un desafío para MFA, se recomienda consultar los registros de auditoría de Azure Active Directory. Esto puede realizarse mediante el módulo [ Azure PowerShell](https://docs.microsoft.com/powershell/azure/overview) y el siguiente script. Se generará un informe que proporciona información acerca de los intentos de autenticación que se han producido durante el último día en los que no se ha usado MFA.

```powershell
Login-AzAccount
$context = Get-AzContext

function Get-SignInEvents
{
    param([string]$userId)

    $content = '{"startDateTime":"' + (Get-Date).AddDays(-1).ToUniversalTime().ToString("yyyy-MM-ddT05:00:00.000Z") + '","endDateTime":"' + (Get-Date).ToUniversalTime().ToString("yyyy-MM-ddTHH:mm:ss.fffZ")  + '","userId":"' + $userId +'","riskState":[],"totalRisk":[],"realtimeRisk":[],"tokenIssuerType":[],"isAdfsEnabled":false}'

    $token = [Microsoft.Azure.Commands.Common.Authentication.AzureSession]::Instance.AuthenticationFactory.Authenticate($context.Account, $context.Environment, $context.Tenant.Id, $null, "Never", $null, "74658136-14ec-4630-ad9b-26e160ff0fc6")

    $headers = @{
    'Authorization' = 'Bearer ' + $token.AccessToken
    'Content-Type' = 'application/json'
        'X-Requested-With'= 'XMLHttpRequest'
        'x-ms-client-request-id'= [guid]::NewGuid()
        'x-ms-correlation-id' = [guid]::NewGuid()
    }

    Invoke-RestMethod -Body $content -Header $headers -Method POST -Uri "https://main.iam.ad.ext.azure.com/api/Reports/SignInEventsV3"
}

$report = $()

Get-AzADUser | foreach {
    $events = Get-SignInEvents $_.Id
    $report += $events.Items
}

$report | Where-Object {$_.mfaRequired -eq $false} | Select-Object userPrincipalName, userDisplayName, createdDateTime, resourceDisplayName, loginSucceeded, failureReason, mfaRequired, mfaAuthMethod, mfaAuthDetail, mfaResult, @{Name='policies'; Expression={[string]::join(',', $($_.conditionalAccessPolicies | Select-Object displayName).displayName )}}, conditionalAccessStatus | Export-Csv report.csv
```

Después de ejecutar el script anterior, los detalles estarán disponibles en el archivo report. csv. Contendrá una lista de los intentos de autenticación que se han producido a lo largo del día anterior en el que el usuario no usó MFA. Tendrás que revisar cada entrada para determinar si es el comportamiento esperado y actuar, en caso de que sea necesario.

![Informe de evaluación](images/security/assessment-report.png)

## <a name="common-issues"></a>Problemas comunes

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

Después de habilitar las directivas de línea de base, es posible que la automatización o la integración encuentren una excepción como la siguiente

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

La razón de esta excepción es que la autenticación se va a realizar mediante las credenciales del usuario y que se necesita MFA. Para solucionar esta excepción, necesitarás utilizar un token de acceso para la autenticación. Para más información, consulta la [guía del modelo de aplicaciones seguras ](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).

>[!IMPORTANT]
>La mayoría de las API y los módulos de PowerShell modernos admiten la posibilidad de utilizar un token de acceso para la autenticación. Sin embargo, hay algunos que no la admiten. Si necesitas ayuda para determinar si la API o el módulo de PowerShell que intenta aprovechar admiten el uso de un token de acceso para la autenticación, publica un mensaje en el [grupo de instrucciones de seguridad del Centro de partners](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

#### <a name="aadsts700082"></a>AADSTS700082

Una vez que hayas implementado el marco del modelo de aplicaciones seguras, es probable que recibas la siguiente excepción 90 días después de generar el token de actualización inicial

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

Con respecto a Azure Active Directory la duración máxima de un token de actualización es de 90 días. Para solucionar este error, debes generar un token de actualización y almacenarlo de forma segura. Ten en cuenta que el token de actualización se puede actualizar mediante programación, ya que cada vez que se solicita un token de acceso a Azure Active Directory se devuelve un nuevo token de actualización. Puedes implementar la lógica apropiada para actualizar el token de actualización almacenado de forma segura antes de que expire.

Para más información, consulta [Vigencia de tokens configurable en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

### <a name="recovering-compromised-accounts"></a>Recuperación de cuentas en peligro

Para ayudar a proteger a nuestros clientes, el servicio de credenciales filtradas de Microsoft busca pares de nombre de usuario y contraseña disponibles públicamente. Si coinciden con las de cualquiera de nuestros usuarios, te ayudaremos a proteger la cuenta de inmediato. Los usuarios identificados como con una credencial filtrada están en peligro de forma confirmada. y se les bloqueará el inicio de sesión hasta que se restablezca su contraseña.

Los usuarios a los que se ha asignado una licencia de Azure AD Premium pueden restaurar el acceso a través del autoservicio de restablecimiento de contraseña (SSPR) si la funcionalidad está habilitada en su directorio. Los usuarios sin una licencia Premium que no puedan iniciar sesión porque estén bloqueados deben ponerse en contacto con un administrador para restablecer manualmente la contraseña y descartar el evento de riesgo de usuario marcado.

#### <a name="steps-to-unblock-a-user"></a>Pasos para desbloquear a un usuario

Comprueba que la directiva ha bloqueado al usuario, para lo que debes examinar sus registros de inicio de sesión.

1. Es preciso que un administrador inicie sesión en **Azure Portal**  y que vaya a **Azure Active Directory** > **Usuarios**, que haga clic en el nombre del usuario y que vaya a Inicios de sesión.
2. Para iniciar el restablecimiento de la contraseña de un usuario bloqueado, el administrador debe ir a **Azure Active Directory** > **Usuarios marcados en riesgo**
3. Haz clic en el usuario cuya cuenta esté bloqueada para ver información acerca de la actividad de inicio de sesión reciente del usuario.
4. Haz clic en Restablecer contraseña para asignar una contraseña temporal, que se debe cambiar en el siguiente inicio de sesión.
5. Haz clic en Descartar todos los eventos para restablecer la puntuación de riesgo del usuario.

El usuario ya puede iniciar sesión, restablecer su contraseña y acceder a la aplicación.

## <a name="known-issues"></a>Problemas conocidos

### <a name="exchange-online-powershell"></a>Exchange Online PowerShell

Si se aplica MFA, los partners no podrán utilizar sus privilegios administrativos delegados con Exchange Online PowerShell para realizar acciones en sus clientes. Para más información acerca de esta limitación, consulta [Conexión con Exchange Online PowerShell mediante autenticación multifactor](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell) .

Para solucionar esta limitación, puedes crear una cuenta y no usarla nunca para realizar una autenticación interactiva. Se recomienda aprovechar [Azure AD PowerShell](https://docs.microsoft.com/powershell/module/azuread/) para crear la nueva cuenta y realizar la configuración inicial. El siguiente código de PowerShell se puede usar para crear y configurar la cuenta

```powershell
Import-Module AzureAD
Connect-AzureAD

$PasswordProfile = New-Object -TypeName Microsoft.Open.AzureAD.Model.PasswordProfile

$PasswordProfile.Password = "Password"
$PasswordProfile.ForceChangePasswordNextLogin = $false

$user = New-AzureADUser -DisplayName "New User" -PasswordProfile $PasswordProfile -UserPrincipalName "NewUser@contoso.com" -AccountEnabled $true

# Uncomment the following two lines if you want the account to have Admin Agent privileges
# $adminAgentsGroup = Get-AzureADGroup -Filter "DisplayName eq 'AdminAgents'"
# Add-AzureADGroupMember -ObjectId $adminAgentsGroup.ObjectId -RefObjectId $user.ObjectId
```

La próxima vez que te conectes a Exchange Online mediante PowerShell usa esta cuenta, ya que funcionará como cabría esperar.

> [!IMPORTANT]
> La capacidad de los partners para utilizar sus privilegios administrativos delegados con Exchange Online PowerShell para realizar acciones en sus clientes, cuando se aplique MFA, estará disponible en el futuro. Hasta entonces, debes aprovechar esta solución alternativa.

## <a name="resources-and-support"></a>Recursos y soporte técnico

Mediante la [comunidad del grupo de instrucciones de seguridad del Centro de partners](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance), puedes encontrar más recursos y obtener información acerca de próximos eventos, como el horario del soporte técnico. Para más información acerca de los requisitos, consulta las [preguntas frecuentes](partner-security-requirements-faq.md).
