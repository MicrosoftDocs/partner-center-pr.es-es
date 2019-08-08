---
title: Requisitos de seguridad de los asociados | Centro de Partners
ms.topic: article
ms.date: 08/05/2019
description: Obtenga información sobre los requisitos de seguridad para asesores y asociados que participan en el programa proveedor de soluciones en la nube.
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, proveedor de soluciones en la nube, programa del proveedor de soluciones en la nube, CSP, proveedor del panel de control, CPV, autenticación multifactor, MFA, modelo de aplicación segura, modelo de aplicación segura, seguridad
ms.localizationpriority: medium
ms.openlocfilehash: 39081f42c326665bdc30bf25df302d9ae00d9723
ms.sourcegitcommit: fe21430f96e203d279714623888224662d2782a2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/05/2019
ms.locfileid: "68787256"
---
# <a name="partner-security-requirements"></a>Requisitos de seguridad del asociado

**Se aplica a**

- Todos los asociados del programa proveedor de soluciones en la nube
  - Factura directa
  - Proveedor indirecto
  - Revendedor indirecto
- Todos los proveedores del panel de control
- Todos los asesores

Una mayor seguridad y protección de la privacidad se encuentran entre las principales prioridades. Sabemos que la mejor defensa es la prevención y que somos tan seguros como nuestro vínculo más débil. Esta es la razón por la que necesitamos que todos los usuarios de nuestro ecosistema actúen y se aseguren de que tienen las protecciones de seguridad adecuadas. Para ayudar a proteger a los asociados y clientes, presentamos un conjunto de requisitos de seguridad obligatorios para asesores, proveedores del panel de control y asociados que participan en el programa proveedor de soluciones en la nube.

A partir del 1 de agosto de 2019 todos los asociados son necesarios para aplicar la autenticación multifactor a todos los usuarios, incluidas las cuentas de servicio, en su inquilino de asociado.

> [!NOTE]
> Se recomienda encarecidamente que todos los asociados que transaccionen una nube soberano (21Vianet, gobierno de EE. UU. y Alemania) adopten estos nuevos requisitos de seguridad inmediatamente. Sin embargo, no es necesario que estos asociados cumplan los nuevos requisitos de seguridad a partir del 1 de agosto de 2019. Microsoft proporcionará información adicional sobre la aplicación de estos requisitos de seguridad para nubes independientes en el futuro.

Los términos asociados a los requisitos de seguridad del asociado se han agregado a la [Guía del programa del proveedor de soluciones](https://go.microsoft.com/fwlink/p/?LinkId=617100)en la nube. A partir del 1 de agosto de 2019, todos los asociados que participan en el programa proveedor de soluciones en la nube deben cumplir los términos. En lo que se refiere a los asesores, se aplicarán los mismos requisitos contractuales.

Los asociados que no implementen los requisitos de seguridad obligatorios no podrán hacerlo en el programa proveedor de soluciones en la nube ni administrar los inquilinos del cliente que aprovechan los derechos de administrador de delegado, una vez que se aplican estos requisitos. Estamos en proceso de establecer una fecha de aplicación técnica para los requisitos y notificaremos a los asociados de la fecha la información detallada.

## <a name="what-actions-do-i-need-to-take"></a>¿Qué acciones necesito realizar?

Dada la naturaleza con privilegios elevados de ser un asociado, necesitamos asegurarnos de que cada usuario tenga un desafío de MFA para cada autenticación. Esto puede realizarse de una de las siguientes maneras:

- Implementar Azure AD Premium y asegurarse de que se aplica MFA para cada usuario
- Implementar las [directivas de protección de línea de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection)
- Implementar una solución de terceros y asegurarse de que se aplica MFA para cada usuario

> [!IMPORTANT]
> Una vez que estos requisitos se aplican técnicamente, cada autenticación única debe tener un desafío de MFA. No podrá usar ninguna característica del acceso condicional para evitar la autenticación mediante MFA al acceder a los servicios en la nube de Microsoft Commercial.

### <a name="considerations"></a>Consideraciones

Dado que estos requisitos se aplican a todos los usuarios, incluidas las cuentas de servicio, en el inquilino del asociado, hay varias consideraciones que deben realizarse para garantizar una implementación sin problemas. Entre estas consideraciones se incluye la identificación de usuarios en Azure AD que no pueden realizar MFA, así como las aplicaciones y los dispositivos usados por su organización que no admiten la autenticación moderna.

Antes de realizar cualquier acción, se recomienda que identifique lo siguiente

#### <a name="do-you-have-an-application-or-device-that-does-not-support-the-use-of-mfa-when-authenticating"></a>¿Tiene una aplicación o un dispositivo que no admite el uso de MFA al autenticarse?

Cuando se aplica la autenticación heredada de MFA, se bloquearán protocolos de uso como IMAP, POP3, SMTP, etc., ya que estos protocolos no admiten MFA. Para solucionar esta limitación, se puede usar una característica conocida como contraseñas de [aplicación](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#app-passwords) para asegurarse de que la aplicación o el dispositivo todavía se pueden autenticar. Debe revisar las consideraciones sobre el uso de contraseñas de aplicación que se documentan [aquí](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#considerations-about-app-passwords) para determinar si se pueden usar en su entorno.

#### <a name="do-you-have-users-using-office-365-provided-by-licenses-associated-with-your-partner-tenant"></a>¿Tiene usuarios que usan Office 365 que proporcionan licencias asociadas a su inquilino de asociado?

Antes de implementar cualquier solución, se recomienda que determine por qué la versión de Microsoft Office la usan los usuarios de su inquilino de asociado. Revise el [plan para la autenticación multifactor para implementaciones de Office 365](https://docs.microsoft.com/office365/admin/security-and-compliance/multi-factor-authentication-plan#enable-mfa) antes de realizar cualquier acción. Existe la posibilidad de que los usuarios experimenten problemas de conectividad con aplicaciones como Outlook. Antes de aplicar MFA, es importante asegurarse de que se use Outlook 2013 SP1, o una versión posterior, y que la organización tenga habilitada la autenticación moderna. Vea [Habilitar la autenticación moderna en Exchange Online](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/enable-or-disable-modern-authentication-in-exchange-online) para obtener más información.

Para habilitar la autenticación moderna en cualquier dispositivo que ejecute Windows que tenga Microsoft Office 2013 instalado, deberá crear dos claves del registro. Consulte [habilitación de la autenticación moderna para Office 2013 en dispositivos Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).

> [!IMPORTANT]
> Si ha habilitado a los usuarios para Azure AD MFA y tienen dispositivos que ejecutan Office 2013 y que no están habilitados para la autenticación moderna, deberán usar contraseñas de aplicación en esos dispositivos. Puede encontrar más información sobre las contraseñas de aplicación y cuándo y dónde se deben usar aquí: [Contraseñas de aplicación con Azure multi-factor Authentication](https://go.microsoft.com/fwlink/p/?LinkId=528178).

#### <a name="is-there-a-policy-preventing-any-of-your-users-from-using-their-mobile-devices-while-working"></a>¿Hay alguna directiva que impida que los usuarios usen sus dispositivos móviles mientras trabajan?

Es importante identificar las directivas corporativas que impiden que los empleados usen dispositivos móviles mientras trabajan, ya que influirán en la solución MFA que implemente. Hay soluciones MFA, como la que se proporciona a través de la implementación de las [directivas de protección de línea de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection), que solo permiten el uso de una aplicación de autenticador para la comprobación. En caso de que la organización tenga una directiva que impida el uso de dispositivos móviles, debe tener en cuenta una de las siguientes opciones:

- Implementación de un dispositivo Android virtualizado en el que se puede instalar una aplicación autenticadora
- Implementar una solución de terceros que aplique MFA para cada usuario del inquilino del asociado que proporcione la opción de comprobación más adecuada
- Compra de licencias de [Azure ad Premium](https://azure.microsoft.com/pricing/details/active-directory/) para los usuarios afectados

#### <a name="what-automation-or-integration-do-you-have-that-leverages-user-credentials-for-authentication"></a>¿Qué automatización o integración tiene que usa las credenciales de usuario para la autenticación?

Dado que el requisito es aplicar MFA para cada usuario, incluidas las cuentas de servicio, en el directorio de socios comerciales se verá afectada cualquier automatización o integración que aproveche las credenciales de usuario para la autenticación. Por lo tanto, es importante que identifique qué cuentas se usan en estas situaciones. A continuación se muestra una lista de ejemplos de aplicaciones o servicios que se deben tener en cuenta

- Panel de control usado para aprovisionar recursos en nombre de sus clientes
- Integración con cualquier plataforma que se utilice para la facturación (en relación con el programa CSP) y soporte técnico a sus clientes.
- Scripts de PowerShell que usan los módulos AZ, AzureRM, Azure AD, MS online, etc.

La lista anterior no es completa. Por lo tanto, es importante que realice una evaluación completa de cualquier aplicación o servicio de su entorno que saque provecho de las credenciales de usuario para la autenticación. Para competir con el requisito de MFA, debe implementar las instrucciones en el [marco de modelo de aplicación segura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) siempre que sea posible. Los siguientes son recursos adicionales que le ayudarán a entender cómo se puede implementar el marco de modelo de aplicación segura

- [Ejemplos de .net del centro de Partners](https://github.com/microsoft/partner-center-dotnet-samples) : este repositorio de github contiene ejemplos, desarrollados con .net, que muestran cómo se puede implementar el marco de trabajo de modelo de aplicación segura.
- [Ejemplos de Java del centro de Partners](https://github.com/microsoft/partner-center-java-samples) : este repositorio de github contiene ejemplos, desarrollados con Java, que muestran cómo se puede implementar el marco de trabajo de modelo de aplicación segura.
- [Centro de Partners PowerShell: modelo de aplicación seguro](https://docs.microsoft.com/powershell/partnercenter/secure-app-model) . este es un artículo que proporciona detalles sobre cómo implementar el marco de modelo de aplicación segura mediante PowerShell.
- [Guía de seguridad del centro de Partners](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) : esta es la comunidad en línea, donde puede obtener información sobre los próximos eventos y formular las preguntas que pueda tener.

### <a name="enforcing-mfa-for-all-users"></a>Aplicación de MFA para todos los usuarios

En esta sección se explica cómo puede usar las [directivas de protección de línea de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) para aplicar MFA para cada usuario, incluidas las cuentas de servicio, en el inquilino de asociado. Si tiene previsto usar Azure AD Premium, siga los pasos que se describen [aquí](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-getstarted).

> [!NOTE]
> Una solución de terceros, que es compatible con Azure AD, puede usarse para aplicar MFA para todos los usuarios, incluidas las cuentas de servicio de. Consulte la documentación del proveedor para obtener más detalles sobre cómo se debe implementar la solución.

Las directivas de protección de línea de base son un conjunto de directivas predefinidas que ayudan a proteger las organizaciones frente a muchos ataques comunes. Estos ataques comunes pueden incluir la pulverización de contraseñas, la reproducción y la suplantación de identidad. Las directivas de protección de línea de base están disponibles en todas las ediciones de Azure Active Directory. Microsoft está poniendo estas directivas de protección de línea de base a disposición de todo el mundo para que los clientes y asociados puedan implementar las mejores prácticas de seguridad.

Las dos directivas de protección de línea de base que deben habilitarse se describen en la tabla siguiente.

|**Directiva**| |
|-----|-----|
|**Requerir MFA para administradores**|La habilitación de la Directiva requerir MFA para administradores requiere que los usuarios de los roles de administrador se registren en MFA con la aplicación Authenticator. Una vez completado el registro de MFA, los administradores deberán realizar MFA cada vez que inicien sesión.|
|**Protección de usuarios finales**|La protección del usuario final es una directiva de protección de base de MFA basada en riesgo que protege a todos los usuarios de un directorio. La habilitación de esta directiva requiere que todos los usuarios se registren para MFA con la aplicación Authenticator. Los usuarios pueden omitir la solicitud de registro de MFA durante 14 días, tras lo cual se les bloqueará el iniciar sesión hasta que se registren en MFA. Una vez que se haya registrado para MFA, solo se solicitará a los usuarios la MFA durante los intentos de inicio de sesión peligrosos. Las cuentas de usuario en peligro se bloquean hasta que se restablece la contraseña y se descartan los eventos de riesgo.|

Cuando estas directivas están habilitadas, cada usuario podrá usar Azure MFA con la aplicación Authenticator para la comprobación sin costo adicional.

#### <a name="configure-self-service-password-reset"></a>Configurar el autoservicio de restablecimiento de contraseña

El autoservicio de restablecimiento de contraseña (SSPR) es una característica Azure Active Directory que permite a los usuarios restablecer sus contraseñas sin necesidad de ponerse en contacto con el equipo de soporte técnico. Los usuarios deben registrarse o registrarse para el autoservicio de restablecimiento de contraseña antes de usar el servicio. Durante el registro, el usuario elige uno o varios métodos de autenticación habilitados por su organización.

Cuando la Directiva de protección de línea de base de [protección del usuario final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) está habilitada, todas las cuentas de usuario en peligro se bloquearán hasta que se restablezca la contraseña y se hayan descartado los eventos de riesgo. Teniendo en cuenta esto, se recomienda que cada usuario, que es un administrador global, realice lo siguiente para registrarse en SSPR para que no se bloquee.

1. Vaya a la [Página de instalación de SSPR](https://aka.ms/ssprsetup)
2. Escriba su nombre de usuario y contraseña
3. Configure al menos una de las opciones de comprobaciones que se usarán para comprobar quién es el restablecimiento de la contraseña.  

Cuando una cuenta se ve comprometida, un administrador deberá tomar medidas para restaurar el acceso para el usuario afectado. Consulte los [pasos para desbloquear a un usuario](#recovering-compromised-accounts) para obtener más detalles sobre el proceso de desbloqueo del usuario.

#### <a name="require-mfa-for-admins"></a>Requerir MFA para administradores

La directiva *requerir MFA para la línea de base de administrador* requiere MFA para los siguientes roles de directorio, que se consideran los roles Azure Active Directory con más privilegios:

- Administrador global
- Administrador de SharePoint
- Administrador de Exchange
- Administrador de acceso condicional
- Administrador de seguridad
- Administrador de soporte técnico/administrador de contraseñas
- Administrador de facturación
- Administrador de usuarios

Al habilitar la Directiva requerir MFA para administradores, se requerirán los nueve roles de administrador anteriores para registrarse en MFA con la aplicación Authenticator. Una vez completado el registro de MFA, los administradores deberán realizar MFA cada vez que inicien sesión.

Si su organización tiene estas cuentas en uso en scripts o código, considere la posibilidad [](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/overview)de reemplazarlas por identidades administradas.

Para habilitar esta directiva y proteger a los administradores:

1. Inicie sesión en el **Azure portal** como administrador global, administrador de seguridad o administrador de acceso condicional.
2. Vaya a **Azure Active Directory** > **acceso condicional**.
3. En la lista de directivas, seleccione **Directiva de línea base: Requerir MFA para administradores**.
4. Establezca **Habilitar Directiva** para **usar la Directiva inmediatamente**.
5. Haga clic en **Guardar**.

> [!WARNING]
> Antes de habilitar esta Directiva, asegúrese de que los usuarios no utilicen protocolos de autenticación heredados. A través de la implementación de esta Directiva, se bloqueará la autenticación heredada.

> [!IMPORTANT]
> Existe un problema conocido que afecta a la capacidad de conectarse a Exchange Online PowerShell con privilegios administrativos delegados. Vea el problema conocido de [Exchange Online PowerShell](#exchange-online-powershell) antes de habilitar esta Directiva si usa este módulo de PowerShell.

#### <a name="end-user-protection"></a>Protección de usuarios finales

La Directiva de línea de base de protección del usuario final protege a todos los usuarios de un directorio. La habilitación de esta directiva requiere que todos los usuarios se registren en Azure MFA en 14 días. Una vez registrado, solo se solicitará a los usuarios la MFA durante los intentos de inicio de sesión peligrosos. Las cuentas de usuario en peligro se bloquean hasta que el restablecimiento de contraseña y el riesgo se descartan.

Directiva de **línea de base de directiva: La protección** de usuarios finales viene preconfigurada y se mostrará en la parte superior cuando vaya a la hoja de acceso condicional en Azure portal.

Para habilitar esta directiva y proteger a los usuarios:

1. Inicie sesión en el **Azure portal** como administrador global, administrador de seguridad o administrador de acceso condicional.
2. Vaya a **Azure Active Directory** > **acceso condicional**.
3. En la lista de directivas, seleccione **Directiva de línea base: Protección de usuarios finales (versión**preliminar).
4. Establezca **Habilitar Directiva** para **usar la Directiva inmediatamente**.
5. Haga clic en **Guardar**.

> [!WARNING]
> Antes de habilitar esta Directiva, asegúrese de que los usuarios no utilicen protocolos de autenticación heredados. A través de la implementación de esta Directiva, se bloqueará la autenticación heredada.

> [!IMPORTANT]
> Hay problemas conocidos que afectan a la capacidad de conectarse a Exchange Online PowerShell con privilegios de administrador delegados. Vea el problema conocido de [Exchange Online PowerShell](#exchange-online-powershell) antes de habilitar esta Directiva si usa este módulo de PowerShell.

## <a name="common-issues"></a>Problemas comunes

### <a name="azure-active-directory"></a>Azure Active Directory

#### <a name="aadsts50076"></a>AADSTS50076

Después de habilitar las directivas de línea de base, es posible que se produzca una excepción como la siguiente:

    AADSTS50076: Due to a configuration change made by your administrator, or because you moved to a new location, you must use multi-factor authentication to access 'MyApp'.

La razón de esta excepción es que se está autenticando con las credenciales de usuario y que MFA es ahora necesario. Para solucionar esta excepción, deberá utilizar un token de acceso para la autenticación. Vea la [Guía modelo de aplicación segura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) para obtener más información.

>[!IMPORTANT]
>La mayoría de las API modernas y los módulos de PowerShell admiten la posibilidad de utilizar un token de acceso para la autenticación. Sin embargo, hay algunos que actualmente no admiten esta funcionalidad. Si necesita ayuda para determinar si la API o el módulo de PowerShell que está intentando aprovechar admite el uso de un token de acceso para la autenticación, publique un mensaje en la comunidad del [grupo de instrucciones de seguridad del centro de Partners](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) .

#### <a name="aadsts700082"></a>AADSTS700082

Una vez que haya implementado el marco de trabajo de modelo de aplicación segura, es probable que reciba la siguiente excepción 90 días después de generar el token de actualización inicial.

    The refresh token has expired due to inactivity. The token was issued on 2019-01-02T09:19:53.5422744Z and was inactive for 90.00:00:00

Con respecto a Azure Active Directory la duración máxima de un token de actualización es de 90 días. Para solucionar este error, debe generar y almacenar de forma segura un nuevo token de actualización. Tenga en cuenta que es posible actualizar el token de actualización mediante programación, ya que con cada solicitud de Azure Active Directory para un token de acceso se devuelve un nuevo token de actualización. Puede implementar la lógica adecuada para actualizar el token de actualización almacenado de forma segura antes de que expire.

Consulte [vigencias de los tokens configurables en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) para obtener más información.

### <a name="recovering-compromised-accounts"></a>Recuperación de cuentas en peligro

Para ayudar a proteger a nuestros clientes, el servicio de credenciales perdidas de Microsoft busca pares de nombre de usuario y contraseña disponibles públicamente. Si coincide con uno de nuestros usuarios, ayudaremos a proteger esa cuenta inmediatamente. Los usuarios identificados como con una credencial filtrada se confirman en peligro. Se bloqueará el inicio de sesión de estos usuarios hasta que se restablezca la contraseña.

Los usuarios a los que se ha asignado una licencia de Azure AD Premium pueden restaurar el acceso a través del autoservicio de restablecimiento de contraseña (SSPR) si la capacidad está habilitada en su directorio. Los usuarios sin una licencia Premium que estén bloqueados deben ponerse en contacto con un administrador para realizar un restablecimiento de contraseña manual y descartar el evento de riesgo de usuario marcado.

#### <a name="steps-to-unblock-a-user"></a>Pasos para desbloquear un usuario

Compruebe que el usuario ha sido bloqueado por la Directiva examinando los registros de inicio de sesión del usuario.

1. Un administrador debe iniciar sesión en el **Azure portal** y navegar a **Azure Active Directory** > **usuarios** > haga clic en el nombre del usuario y navegue hasta inicios de sesión.
2. Para iniciar el restablecimiento de contraseña en un usuario bloqueado, un administrador debe navegar a **Azure Active Directory** > **usuarios marcados en riesgo** .
3. Haga clic en el usuario cuya cuenta está bloqueada para ver información acerca de la actividad de inicio de sesión reciente del usuario.
4. Haga clic en Restablecer contraseña para asignar una contraseña temporal que se debe cambiar en el siguiente inicio de sesión.
5. Haga clic en descartar todos los eventos para restablecer la puntuación de riesgo del usuario.

Ahora el usuario puede iniciar sesión, restablecer su contraseña y acceder a la aplicación.

## <a name="known-issues"></a>Problemas conocidos

### <a name="exchange-online-powershell"></a>PowerShell en línea de Exchange

Cuando se aplica MFA, los asociados no podrán usar sus privilegios administrativos delegados con Exchange Online PowerShell para realizar acciones con sus clientes. Consulte [conexión a Exchange Online PowerShell mediante multi-factor Authentication](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell) para obtener más información sobre esta limitación.

Para solucionar esta limitación, puede crear una nueva cuenta y nunca usarla para realizar una autenticación interactiva. Se recomienda aprovechar [Azure ad PowerShell](https://docs.microsoft.com/powershell/module/azuread/) para crear la nueva cuenta y realizar la configuración inicial. Se puede usar el siguiente PowerShell para crear y configurar la cuenta.

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

La próxima vez que se conecte a Exchange Online a través de PowerShell use esta cuenta, funcionará según lo esperado.

> [!IMPORTANT]
> La capacidad de los asociados de usar sus privilegios administrativos delegados con Exchange Online PowerShell para realizar acciones en sus clientes, cuando se aplica MFA, estará disponible en el futuro. Hasta entonces, debe aprovechar esta solución alternativa.

## <a name="resources-and-support"></a>Recursos y soporte técnico

A través del [centro de Partners guía de seguridad](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) de la comunidad, puede encontrar recursos adicionales y obtener información sobre próximos eventos, como horas de oficina técnica. Consulte el documento [preguntas](partner-security-requirements-faq.md) más frecuentes para obtener más información sobre los requisitos.
