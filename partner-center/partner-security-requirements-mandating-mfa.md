---
title: Requerir MFA para su inquilino de socio | Centro de Partners
ms.topic: article
ms.date: 11/12/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Detalles sobre la obligatoriedad de la autenticación multifactor (MFA) para los requisitos de seguridad del inquilino del asociado
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider program, CSP, Control Panel Vendor, CPV, multi-factor authentication, MFA, secure application model, secure app model, security
ms.localizationpriority: medium
ms.openlocfilehash: 9241e7fd7f9812e2c456eac70065e185a9cf8d61
ms.sourcegitcommit: 0f14e29540c6814f01395924223b495cc5299954
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/13/2019
ms.locfileid: "73983348"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Requerir multi-factor Authentication (MFA) para el inquilino de asociado

**Se aplica a**

- Todos los partners que estén en el programa Proveedor de soluciones en la nube
  - Factura directa
  - Proveedor indirecto
  - Revendedor indirecto
- Todos los asesores

Estos asociados serán necesarios para completar la comprobación de MFA para las siguientes áreas:

- [Panel del centro de Partners](#partner-center-dashboard) (dirigido a H1 CY2020)
- [API del centro de Partners](#partner-center-api) (con el destino H1 CY2020)
- [Administración delegada de asociados](#partner-delegated-administration) (a partir del 18 de noviembre de 2019)

La intención de esta característica es ayudar a los asociados a proteger su acceso a los recursos del cliente frente al riesgo de las credenciales.

## <a name="partner-center-dashboard"></a>Panel del centro de Partners
Ciertas páginas del panel del centro de Partners se protegerán mediante MFA, lo que incluye:

* Todas las páginas en la pestaña **clientes** .
* Todas las páginas de la pestaña **Support > Customer requests** .

Si intenta obtener acceso a cualquiera de estas páginas y aún no ha completado la comprobación de MFA, se le pedirá que lo haga.

Los siguientes tipos de usuario están autorizados para tener acceso a estas páginas protegidas por MFA y, por tanto, se ven afectadas por esta característica, entre las que se incluyen:

* Agentes de administración
* Agentes de ventas
* Agentes del Departamento de soporte técnico

Para ilustrar cómo funciona esto, tenga en cuenta los dos ejemplos siguientes.

**Ejemplo 1: el asociado ha implementado Azure AD MFA**
1.  Julia funciona para CSP contoso. Contoso ha implementado MFA para todos los usuarios del inquilino de Contoso Partner mediante Azure AD MFA.
2.  En su estación de trabajo, Julia inicia una nueva sesión del explorador y se desplaza a la página de información general del panel del centro de Partners (que no está protegida por MFA). El centro de Partners redirige Julia a Azure AD para iniciar sesión.
3.  Debido a la configuración de Azure AD MFA existente por Contoso, se requiere Julia para completar la comprobación de MFA. Cuando el inicio de sesión y la comprobación de MFA se hayan realizado correctamente, Julia se redirige de nuevo a la página de información general del panel del centro de Partners.
4.  Julia intenta tener acceso a una de las páginas protegidas con MFA del centro de Partners. Puesto que Julia ya ha completado la comprobación de MFA durante el inicio de sesión anterior, Julia puede tener acceso a la página protegida por MFA sin que sea necesario volver a realizar la comprobación de MFA.

**Ejemplo 2: el asociado ha implementado MFA de terceros mediante la Federación de identidades**
1. Trent funciona para CSP Wingtip. Wingtip implementó MFA para todos sus usuarios en el inquilino de asociado de Wingtip mediante MFA de terceros que se integra con Azure AD a través de la Federación de identidades.
2. Desde su estación de trabajo, Trent inicia una nueva sesión del explorador y se desplaza a la página de información general del panel del centro de Partners (que no está protegida por MFA). El centro de Partners redirige a Diego a Azure AD para iniciar sesión.
3. Puesto que Wingtip tiene la configuración de la Federación de identidades, Azure AD redirige Trent al proveedor de identidades federado para completar el inicio de sesión y la comprobación de MFA. Una vez que el inicio de sesión y la comprobación de MFA son correctos, Trent se redirige a Azure AD y, a continuación, a la página de información general del panel del centro de Partners
4. Diego intenta acceder a una de las páginas protegidas con MFA del centro de Partners. Dado que Trent ya ha completado la comprobación de MFA durante el inicio de sesión anterior, Trent puede acceder a la página protegida de MFA sin que sea necesario volver a realizar la comprobación de MFA.

**Ejemplo 3: el asociado no ha implementado MFA**
1. Juan trabaja para CSP fabrikam. Fabrikam no implementó MFA para ningún usuario en el inquilino de socio de fabrikam.
2. En su estación de trabajo, Juan inicia una nueva sesión del explorador y se desplaza a la página de información general del panel del centro de Partners (que no está protegida por MFA). El centro de Partners redirige a John a Azure AD para iniciar sesión.
3. Puesto que Fabrikam no ha implementado MFA, no es necesario que John complete la comprobación de MFA. Una vez que el inicio de sesión se realiza correctamente, se redirige a John a la página de información general del panel del centro de Partners.
4. Juan intenta tener acceso a una de las páginas protegidas con MFA del centro de Partners. Puesto que Juan no ha completado la comprobación de MFA, el centro de Partners redirige a John a Azure AD para completar la comprobación de MFA. Como esta es la primera vez que se necesita John para completar MFA, también se solicita a John registrarse para MFA mediante Microsoft Authenticator aplicación. Tras realizar correctamente el registro de MFA y la comprobación de MFA, Juan ahora puede acceder a la página protegida por MFA.

## <a name="partner-center-api"></a>API del centro de Partners

La API del centro de Partners admite tanto la autenticación de aplicación como la autenticación de aplicación y de usuario. Cuando se usa la autenticación de usuario y aplicación, el centro de Partners requiere la comprobación de MFA. Más concretamente, cuando una aplicación asociada desea enviar una solicitud de API al centro de Partners, debe incluir un token de acceso en el encabezado Authorization de la solicitud. Cuando el centro de Partners recibe una solicitud de API con un token de acceso obtenido mediante la autenticación de usuario y aplicación, la API del centro de Partners comprobará la presencia del valor de *MFA* en la declaración de *referencia de método de autenticación (Amr)* . Puede usar un descodificador de JWT para validar si un token de acceso contiene el valor de referencia de método de autenticación esperada (AMR) o no:

``` csharp
{
  "aud": "https://api.partnercenter.microsoft.com",
  "iss": "https://sts.windows.net/df845f1a-7b35-40a2-ba78-6481de91f8ae/",
  "iat": 1549088552,
  "nbf": 1549088552,
  "exp": 1549092452,
  "acr": "1",
  "amr": [
    "pwd",
    "mfa"
  ],
  "appid": "23ec45a3-5127-4185-9eff-c8887839e6ab",
  "appidacr": "0",
  "family_name": "Williams",
  "given_name": "Isaiah",
  "ipaddr": "127.0.0.1",
  "name": "Isaiah Williams",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
  "upn": "Isaiah.Williams@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

Si el valor está presente, el centro de Partners concluye que se completó la comprobación de MFA y procesa la solicitud de API. Si el valor no está presente, la API del centro de Partners rechazará la solicitud con la siguiente respuesta:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

## <a name="partner-delegated-administration"></a>Administración delegada de asociados

### <a name="using-service-portals"></a>Uso de portales de servicio

Las cuentas de asociados, incluidos los agentes de administración y los agentes del Departamento de soporte técnico, pueden usar los privilegios de administrador delegado de sus asociados para administrar los recursos del cliente a través de portales de Microsoft Online Services, la interfaz de la línea de comandos (CLI) y las API (mediante la autenticación de usuario y aplicación).

Al tener acceso a los portales de Microsoft Online Services con los privilegios de administrador delegado de asociados para administrar los recursos del cliente, muchos de estos portales requieren que la cuenta de asociado se autentique de forma interactiva, con el cliente Azure Active Directory conjunto de inquilinos como el contexto de autenticación: la cuenta de asociado es necesaria para iniciar sesión en el inquilino del cliente.

Cuando Azure Active Directory reciba estas solicitudes de autenticación, requerirá que la cuenta del asociado complete la comprobación de MFA. Hay dos experiencias de usuario posibles, en función de si la cuenta de asociado es una identidad administrada o federada:

- Si la cuenta de asociado es una identidad **administrada** , Azure Active Directory le pedirá directamente al usuario que complete la comprobación de MFA. Si la cuenta de socio no se ha registrado para MFA con Azure Active Directory antes, se le pedirá al usuario que complete primero el [registro de MFA](#mfa-registration-experience) .

- Si la cuenta de socio comercial es una identidad **federada** , la experiencia depende de la forma en que el administrador de asociados ha configurado la federación en Azure Active Directory. Al configurar la Federación en Azure Active Directory, el administrador del asociado puede indicar a Azure Active Directory si el proveedor de identidades federado admite MFA o no. En ese caso, Azure Active Directory redirigirá al usuario al proveedor de identidades federado para completar la comprobación de MFA. De lo contrario, Azure Active Directory le pedirá directamente al usuario que complete la comprobación de MFA. Si la cuenta de socio no se ha registrado para MFA con Azure Active Directory antes, se le pedirá al usuario que complete primero el [registro de MFA](#mfa-registration-experience) .

La experiencia general es muy similar a la del escenario en el que un inquilino de cliente final ha implementado MFA para sus administradores. Por ejemplo, el inquilino del cliente ha habilitado [Azure ad Directiva de línea de base: MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators), que requiere que todas las cuentas con derechos administrativos inicien sesión en el inquilino del cliente con la comprobación de MFA, incluidos los agentes de administración y los agentes del Departamento de soporte técnico. Con fines de prueba, los asociados pueden habilitar la [Directiva MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) en el inquilino del cliente y, a continuación, intentar usar los privilegios de administración delegada del asociado para acceder al inquilino del cliente.

> [!NOTE]
> No todos los portales de Microsoft Online Services requieren que las cuentas de asociados inicien sesión en el inquilino del cliente al obtener acceso a los recursos del cliente mediante privilegios de administrador delegados asociados. En su lugar, solo requieren que las cuentas de asociados inicien sesión en el inquilino del asociado. Un ejemplo es el centro de administración de Exchange. Con el tiempo, esperamos que estos portales requieran que las cuentas de asociados inicien sesión en el inquilino del cliente al usar privilegios de administrador delegados asociados.

### <a name="using-service-apis"></a>Uso de las API de servicio
Algunas API de Microsoft Online Services (por ejemplo, Azure Resource Manager, Azure AD Graph, Microsoft Graph, etc.) admiten asociados con privilegios de administrador delegados de asociados para administrar mediante programación los recursos del cliente. Para sacar provecho de los privilegios de administrador delegado de asociados con estas API, la aplicación de asociado debe incluir un token de acceso en el encabezado de autorización de solicitud de API, donde el token de acceso se obtiene al tener una cuenta de usuario del asociado para autenticarse con Azure AD, con el el cliente Azure AD establecer como el contexto de autenticación. La aplicación de socio comercial debe tener una cuenta de usuario de asociado que inicie sesión en el inquilino del cliente.

Cuando Azure AD recibe una solicitud de autenticación, Azure AD requerirá que la cuenta de usuario del asociado complete la comprobación de MFA. Si la cuenta de usuario del asociado no se ha registrado para MFA antes, se le pedirá al usuario que complete primero el registro de MFA.

Esta característica afecta a todas las aplicaciones de asociados que se integran con estas API con privilegios de administrador delegados de asociados. Para asegurarse de que las aplicaciones de asociados pueden continuar funcionando con estas API sin interrupción:

- El asociado debe evitar el uso de métodos de autenticación de usuario no interactivos con Azure AD para obtener el token de acceso. Cuando se usa un método de autenticación de usuario no interactivo como el [flujo de contraseñas](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), Azure ad no podrá pedir al usuario que complete la comprobación de MFA. El asociado debe cambiar al uso del método de autenticación de usuario interactivo, como [OpenID Connect Flow](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-openid-connect-code) en su lugar.
- Durante el método de autenticación interactiva de usuarios, el asociado debe usar una cuenta de usuario de asociado que ya esté habilitada para MFA. Como alternativa, cuando Azure AD, el asociado puede completar el registro de MFA y la comprobación de MFA durante el inicio de sesión.
- Esto es muy similar al escenario en el que un inquilino de cliente final ha implementado MFA para sus administradores. Por ejemplo, el inquilino del cliente ha habilitado [Azure ad Directiva de línea de base-MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators), que requiere que todas las cuentas de usuario con derechos administrativos inicien sesión en el inquilino del cliente con la comprobación de MFA, incluidos los agentes de administración y los agentes del Departamento de soporte técnico. Con fines de prueba, los asociados pueden habilitar la [Directiva MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) en el inquilino del cliente y, a continuación, intentar usar los privilegios de administración delegada del asociado para acceder mediante programación al inquilino del cliente.

### <a name="mfa-registration-experience"></a>Experiencia de registro de MFA
Durante la comprobación de MFA, si la cuenta de socio no se ha registrado previamente para MFA, Azure AD pedirá al usuario que complete primero el registro de MFA:

![Registro de MFA, paso 1](images/MfaRegistration1.png)

Después de hacer clic en **siguiente**, se le pedirá al usuario que elija entre una lista de métodos de comprobación (incluido el teléfono, SMS y la aplicación Authenticator).

![Registro de MFA, paso 2](images/MfaRegistration2.png)

Cuando el registro se realiza correctamente, es necesario que el usuario complete la comprobación de MFA en función de la comprobación elegida por el usuario.



## <a name="request-for-technical-exception"></a>Solicitud de excepción técnica

Los asociados pueden solicitar la excepción técnica para suprimir la comprobación de MFA en caso de que se encuentre con problemas técnicos con Microsoft Online Services y no haya ninguna solución o solución factible. Antes de hacerlo, revise las siguientes secciones:

 - [Lista de problemas comunes comunicados por los asociados](#list-of-common-issues-reported-by-partners)
 - [Cómo enviar una solicitud de excepción técnica](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>Lista de problemas comunes comunicados por los asociados
Antes de aplicar la excepción técnica, revise la lista de problemas comunes que han comunicado otros asociados para saber si son razones válidas para la excepción técnica o no.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problema 1: el asociado necesita más tiempo para implementar MFA para sus agentes de asociados
Un asociado no se ha iniciado o todavía está en proceso de implementar MFA para sus agentes asociados que requieren acceso a los portales de Microsoft Online Services con privilegios de administración delegada de asociados para administrar los recursos del cliente. El asociado necesita más tiempo para completar la implementación de MFA. ¿Es un motivo válido para la excepción técnica?

**Respuesta**: no. El asociado debe crear planes para implementar MFA para que sus usuarios puedan evitar interrupciones.

> [!NOTE]
> Aunque el asociado no ha implementado MFA para sus agentes de asociados, los agentes asociados pueden seguir accediendo a los portales de Microsoft Online Services con privilegios de administración delegada de asociados, siempre que puedan completar el registro de MFA y la comprobación de MFA Cuando se le solicite durante el inicio de sesión en el inquilino del cliente. Al completar el registro de MFA no se habilita automáticamente el usuario para MFA.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problema 2: el asociado no ha implementado MFA para las cuentas de usuario que no usan privilegios de administrador delegado
Un asociado tiene algunos usuarios en sus inquilinos de asociados que no necesitan acceso a los portales de Microsoft Online Services para administrar los recursos del cliente mediante privilegios de administración delegada de asociados. El asociado está en proceso de implementar MFA para estos usuarios y necesita más tiempo para completarse. ¿Es un motivo válido para la excepción técnica?

**Respuesta**: no. Puesto que estas cuentas de usuario no utilizan privilegios de administración delegada de asociados para administrar los recursos del cliente, no se les pedirá que inicien sesión en el inquilino del cliente. No se verán afectados por Azure AD requiere la comprobación de MFA durante el inicio de sesión en el inquilino del cliente.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problema 3: el asociado no ha implementado MFA para las cuentas de servicio de usuario
Un asociado tiene algunas cuentas de usuario en sus inquilinos de asociados que los dispositivos usan como cuentas de servicio. Normalmente, se trata de cuentas con pocos privilegios que no requieren el centro de Partners de acceso ni portales de Microsoft Online Services para administrar los recursos de los clientes mediante privilegios de administración delegada de asociados. ¿Es un motivo válido para la excepción técnica?

**Respuesta**: no. Puesto que estas cuentas de usuario no utilizan privilegios de administración delegada de asociados para administrar los recursos del cliente, no se les pedirá que inicien sesión en el inquilino del cliente. No se verán afectados por Azure AD requiere la comprobación de MFA durante el inicio de sesión en el inquilino del cliente.

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problema 4: el asociado no puede implementar MFA con la aplicación MS Authenticator
Un asociado tiene una directiva de "escritorio limpio" que no permite que los empleados traigan sus dispositivos móviles personales a su área de trabajo. Sin acceso a sus dispositivos móviles personales, los empleados no pueden instalar la aplicación MS Authenticator, que es la única comprobación de MFA compatible con las directivas de línea de base de Azure AD. ¿Es un motivo válido para la excepción técnica?

**Respuesta**: no, no es un motivo válido para la excepción técnica. El asociado debe tener en cuenta las alternativas siguientes, de modo que sus empleados todavía puedan completar la comprobación de MFA al acceder al centro de Partners:
- Aparte de la aplicación MS Authenticator, las directivas de línea de base de Azure AD también se pueden usar con una aplicación de autenticador compatible de terceros, que puede ser compatible con equipos Windows que ejecutan Microsoft Windows.
- El asociado también puede registrarse para Azure AD Premium o soluciones de MFA de terceros (compatibles con Azure AD) que pueden proporcionar métodos de comprobación adicionales.

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problema 5: el asociado no puede implementar MFA debido al uso de protocolos de autenticación heredados
Un asociado tiene algunos agentes asociados que todavía usan protocolos de autenticación heredados, que no son compatibles con MFA. Por ejemplo, los usuarios siguen usando Outlook 2010, que se basa en protocolos de autenticación heredados. Al habilitar MFA para estos agentes de asociados se interrumpirá el uso de protocolos de autenticación heredados.

**Respuesta**: no, no es un motivo válido para la excepción técnica. Se recomienda encarecidamente a los asociados que salgan del uso de los protocolos de autenticación heredados debido a posibles implicaciones de seguridad, ya que estos protocolos no se pueden proteger con la comprobación de MFA y son mucho más susceptibles al riesgo de credenciales. Si no es una opción pasar del uso de los protocolos de autenticación heredados, los asociados deben considerar la posibilidad de suscribirse a Azure AD Premium, que admite el uso de contraseñas de aplicación. Las contraseñas de aplicación son contraseñas generadas por el sistema, que suelen ser más seguras que las contraseñas generadas por el usuario. Mediante el uso de contraseñas de aplicación, los asociados pueden implementar MFA para sus usuarios, al mismo tiempo que recurren a las contraseñas de aplicación solo para los protocolos de autenticación heredados.

> [!NOTE]
> Aunque el asociado no ha implementado MFA para sus agentes de asociados, los agentes asociados pueden seguir accediendo a los portales de Microsoft Online Services con privilegios de administración delegada de asociados, siempre que puedan completar el registro de MFA y la comprobación de MFA Cuando se le solicite durante el inicio de sesión en el inquilino del cliente. Al completar el registro de MFA no se habilita automáticamente el usuario para MFA.

#### <a name="issue-6-partner-is-using-exchange-online-powershell-which-does-not-support-mfa"></a>Problema 6: el asociado está usando Exchange Online PowerShell que no admite MFA
Un asociado está usando Exchange Online PowerShell con privilegios de administración delegados de asociados para administrar el servicio de Exchange online en nombre de sus clientes. Exchange Online PowerShell no es compatible con MFA. Si el asociado implementa MFA para sus usuarios, estos usuarios ya no podrán tener acceso a Exchange Online PowerShell. ¿Es un motivo válido para la excepción técnica?

**Respuesta**: sí, esto se puede considerar como un motivo válido para la excepción técnica. El [módulo de PowerShell de Exchange Online existente que admite la administración delegada de socios comerciales](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) no requiere que el usuario asociado inicie sesión en el inquilino del cliente y, por tanto, no se ve afectado por Azure ad requiere la comprobación de MFA. Sin embargo, no es compatible con MFA. El equipo de Microsoft Exchange Online está desarrollando un nuevo módulo de PowerShell que admite tanto los privilegios de administración delegados de asociados como MFA. Hasta que el nuevo módulo de PowerShell esté disponible, los asociados no podrán implementar MFA para los usuarios que necesiten usar el módulo de PowerShell existente. Si estos usuarios tienen dificultades para acceder a otros servicios de Microsoft Online Services debido a Azure AD requiere la comprobación de MFA durante el inicio de sesión entre inquilinos, los asociados pueden solicitar una excepción técnica para suprimir la comprobación de MFA.

> [!NOTE]
> Aunque el asociado no puede implementar MFA para los usuarios que necesitan tener acceso al módulo de PowerShell de Exchange Online, estos usuarios aún pueden tener acceso a los servicios en línea de Microsoft para administrar los recursos del cliente con privilegios de administración delegada asociados. pueden completar el registro de MFA y la comprobación de MFA cuando se le solicite durante el inicio de sesión en el inquilino del cliente. Al completar el registro de MFA, no se habilita automáticamente el usuario para MFA y, por tanto, no se ve afectado el acceso al módulo de PowerShell de Exchange Online.

#### <a name="issue-7-partner-has-implemented-3rd-party-mfa-which-isnt-recognized-by-azure-ad"></a>Problema 7: el asociado ha implementado MFA de terceros que no reconoce Azure AD
Un asociado ha implementado MFA para sus usuarios mediante una solución de MFA de terceros. Sin embargo, el asociado no puede configurar correctamente la solución MFA de terceros para la retransmisión a Azure AD que se ha completado la comprobación de MFA durante la autenticación del usuario. ¿Es un motivo válido para la excepción técnica?

**Respuesta**: sí, esto se puede considerar como un motivo válido para la excepción técnica. Antes de enviar una solicitud de excepción técnica, confirme con el proveedor de soluciones de MFA de terceros que no se puede configurar la solución MFA para que fluya la solicitud *authenticationmethodsreferences* (con el valor *multipleauthn*) a Azure ad para indicar que se ha completado la comprobación de MFA durante la autenticación del usuario. Al enviar una solicitud de excepción técnica, proporcione los detalles de la solución MFA de terceros utilizada e indique el método de integración (por ejemplo, a través de la Federación de identidades o el uso de Azure AD control personalizado).

### <a name="how-to-submit-a-request-for-technical-exception"></a>Cómo enviar una solicitud de excepción técnica

Para enviar una solicitud de excepción técnica:

1. Inicie sesión en el centro de partners como administrador global o agente de administración.
2. Cree una nueva solicitud de servicio de asociado; para ello, vaya a **soporte técnico** > **solicitudes de soporte técnico de asociados** y haga clic en **nueva solicitud**.
4. En el tema sobre **MFA y modelo de aplicación seguro** , ferentes **Enviar solicitud de excepción técnica** como el tipo de problema.
6. Proporcione los detalles solicitados para enviar una solicitud de servicio de excepción técnica y haga clic en **Enviar**.

Microsoft puede tardar hasta tres días laborables en proporcionar una respuesta a la solicitud de excepción técnica.
