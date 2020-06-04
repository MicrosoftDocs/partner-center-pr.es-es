---
title: Requerir MFA para el inquilino del asociado
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtén información sobre cómo el requisito de MFA para los inquilinos de partner ayudará a proteger el acceso a los recursos de los clientes. Incluye escenarios de ejemplo.
author: LauraBrenner
ms.author: labrenne
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider program, CSP, Control Panel Vendor, CPV, multi-factor authentication, MFA, secure application model, secure app model, security
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9454e9410e4110fdf3542bde3696d8447d4c90d0
ms.sourcegitcommit: dadc0b112497802db2d8d5e72fc76c95a4dc18d6
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/27/2020
ms.locfileid: "83998311"
---
# <a name="mandating-multi-factor-authentication-mfa-for-your-partner-tenant"></a>Requisito de Multi-Factor Authentication (MFA) para el inquilino de partner

**Se aplica a**

- Todos los partners que estén en el programa Proveedor de soluciones en la nube
  - Factura directa
  - Proveedor indirecto
  - Revendedor indirecto
- Todos los asesores

**Roles afectados**

- Agente de administrador
- Agente de ventas
- Agente del departamento de soporte técnico
- Administrador de facturación
- Administrador global

La intención de esta característica es ayudar a los partners a proteger su acceso a los recursos de clientes frente al riesgo de las credenciales.
Los partners deben aplicar la autenticación multifactor (MFA) para todas las cuentas de usuario de su inquilino de partner, incluido el usuario invitado. Con esta característica, estos roles de partner deberán completar la verificación MFA para las siguientes áreas:

- [Panel del Centro de partners](#partner-center-dashboard) (a partir del 1 de mayo de 2020)
- [API del Centro de partners](#partner-center-api) (a partir del 1 de mayo de 2020)
- [Administración delegada de partner](#partner-delegated-administration)

Las medidas de seguridad y privacidad continuas y en constante crecimiento son una de nuestras principales prioridades, y seguimos ayudando a los partners a proteger a sus clientes e inquilinos. Todos los partners que participan en el programa Proveedor de soluciones en la nube (CSP), los proveedores de panel de control (CPV) y los asesores deben implementar los [requisitos de seguridad para partners](partner-security-requirements.md) para mantener el cumplimiento.

Microsoft ha iniciado la activación de medidas de seguridad adicionales para los inquilinos de partners. Esta activación de medidas de seguridad puede ayudar a los partners a proteger a sus inquilinos y a sus clientes al exigir la verificación mediante autenticación multifactor (MFA) a fin de evitar un acceso no autorizado.

Hemos completado correctamente la activación de las funcionalidades de administración delegada de partners para todos los inquilinos de partners. Para contribuir a proteger aún más a los partners y clientes, a partir del 1 de mayo de 2020, iniciaremos la activación para las transacciones del Centro de partners en CSP a fin de ayudar a los partners a proteger sus negocios y a sus clientes frente a incidentes relacionados con el robo de identidad.

En esta documentación se proporciona a los partners una experiencia detallada e instrucciones sobre la activación de las medidas de seguridad.

## <a name="partner-center-dashboard"></a>Panel del Centro de partners

Ciertas páginas del panel del Centro de partners se protegerán mediante MFA, entre las que se incluyen:

* Todas las páginas de la pestaña **Clientes**; por ejemplo, todas las páginas a las que se puede acceder desde la siguiente dirección URL: https://partner.microsoft.com/commerce/*
* Todas las páginas de la pestaña **Soporte técnico > Solicitudes de clientes**; p. ej., las páginas a las que se accede desde https://partner.microsoft.com/dashboard/support/csp/customers/*
* Página de facturación

Si intentas acceder a cualquiera de estas páginas y aún no has completado la comprobación de MFA, se te pedirá que lo hagas.

> [!NOTE]
> Otras páginas del Centro de partners, como la página Información general o la página Estado de mantenimiento del servicio, no estarán protegidas mediante MFA.

Los siguientes tipos de usuario están autorizados para acceder a estas páginas protegidas por MFA y, por tanto, se ven afectados por esta característica.


| Páginas protegidas con MFA       | Agentes administradores      |  Agentes de ventas     |   Agentes del departamento de soporte técnico     | Administrador global      |  Administrador de facturación     | 
|---    |---    |---    |---    |---    |---    |
| Todas las páginas de la pestaña Clientes      |   x    |    x   |  x     |       |       |
| Todas las páginas de la pestaña Soporte técnico > Solicitudes de clientes     | x      |       |    x   |       |       |
| Página de facturación     |   x    |       |       |    x   |   x    |

**Ejemplos**

Para ilustrar cómo funciona la comprobación, ten en cuenta los dos ejemplos siguientes.

**Ejemplo 1: El partner ha implementado Azure AD MFA**
1.    Julia trabaja para CSP Contoso. Contoso ha implementado MFA para todos los usuarios del inquilino de partner de Contoso mediante Azure Active Directory (Azure AD) MFA.
2.    Julia inicia una nueva sesión de explorador y navega hasta la página de información general del panel del Centro de partners (que no está protegida por MFA). El Centro de partners redirige a Julia a Azure AD para que inicie sesión.
3.    Debido a la instancia existente de Azure AD MFA configurada por Contoso, se requiere a Julia que complete la comprobación de MFA. Después de que el inicio de sesión y la verificación de MFA se hayan realizado correctamente, se redirige a Julia de nuevo a la página de información general del panel del Centro de partners.
4.    Julia intenta acceder a una de las páginas protegidas por MFA del Centro de partners. Puesto que Julia ya ha completado la comprobación de MFA durante el inicio de sesión anterior, puede acceder a la página protegida por MFA sin que sea necesario volver a realizarla.

**Ejemplo 2: El partner ha implementado una instancia de MFA de terceros mediante la federación de identidades**
1. David trabaja para CSP Wingtip. Wingtip implementó MFA para todos sus usuarios en el inquilino de partner de Wingtip mediante una instancia de MFA de terceros que se integra con Azure AD a través de la federación de identidades.
2. David inicia una nueva sesión de explorador y navega hasta la página de información general del panel del Centro de partners (que no está protegida por MFA). El Centro de partners redirige a David a Azure AD para que inicie sesión.
3. Puesto que Wingtip ha configurado la federación de identidades, Azure AD redirige a David al proveedor de identidades federado para que complete el inicio de sesión y la comprobación de MFA. Después de que el inicio de sesión y la verificación de MFA se hayan realizado correctamente, se redirige a David de nuevo a Azure AD y, a continuación, a la página de información general del panel del Centro de partners.
4. David intenta acceder a una de las páginas protegidas por MFA del Centro de partners. Puesto que David ya ha completado la comprobación de MFA durante el inicio de sesión anterior, puede acceder a la página protegida por MFA sin que sea necesario volver a realizarla.

**Ejemplo 3: El partner no ha implementado MFA**
1. Jorge trabaja para CSP Fabrikam. Fabrikam no ha implementado MFA para ningún usuario en el inquilino de partner de Fabrikam.
2. Jorge inicia una nueva sesión de explorador y navega hasta la página de información general del panel del Centro de partners (que no está protegida por MFA). El Centro de partners redirige a Jorge a Azure AD para que inicie sesión.
3. Puesto que Fabrikam no ha implementado MFA, no es necesario que Jorge complete la comprobación de MFA. Después de que el inicio de sesión se haya realizado correctamente, se redirige a Jorge de nuevo a la página de información general del panel del Centro de partners.
4. Jorge intenta acceder a una de las páginas protegidas por MFA del Centro de partners. Puesto que Jorge no ha completado la comprobación de MFA, el Centro de partners le redirige a Azure AD para que la complete. Como es la primera vez que se requiere a Jorge que complete la MFA, también se le pide que se [registre para MFA](#mfa-registration-experience). Tras realizar correctamente el registro de MFA y la comprobación de MFA, Jorge puede acceder a la página protegida por MFA.
5. Otro día, antes de que Fabrikam implemente la MFA para ningún usuario, Jorge inicia una nueva sesión de explorador y navega hasta la página de información general del panel del Centro de partners (que no está protegida por MFA). El Centro de partners redirige a Jorge a Azure AD para que inicie sesión sin que se le pida la confirmación de MFA. 
6. Jorge intenta acceder a una de las páginas protegidas por MFA del Centro de partners. Puesto que Jorge no ha completado la comprobación de MFA, el Centro de partners le redirige a Azure AD para que la complete. Dado que Jorge ha registrado la MFA, esta vez solo se le pide que complete la verificación de MFA.

> [!NOTE]
>Acción: El administrador de empresa debe implementar la MFA ahora con cualquiera de las [opciones](partner-security-requirements.md#actions-that-you-need-to-take) que sugiere el Centro de partners.

## <a name="partner-center-api"></a>API del Centro de partners

La API del Centro de partners admite tanto la autenticación de solo aplicación como la autenticación de aplicación y usuario. 

Cuando se usa la autenticación de aplicación y usuario, el Centro de partners requiere la comprobación de MFA. Más concretamente, cuando una aplicación de partner quiere enviar una solicitud de API al Centro de partners, debe incluir un token de acceso en el encabezado de autorización de la solicitud. 

> [!NOTE]
>El [modelo de aplicaciones seguras](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) es un marco de trabajo seguro y escalable para autenticar partners de CSP y CPV mediante la arquitectura de Microsoft Azure MFA al llamar a la API del Centro de partners. Es necesario implementarlo antes de habilitar MFA en el inquilino. 

Cuando el Centro de partners recibe una solicitud de API con un token de acceso obtenido mediante la autenticación de la aplicación y el usuario, la API del Centro de partners comprueba la presencia del valor *MFA* en la notificación de *referencia de método de autenticación (AMR)* . Puedes usar un descodificador JWT para validar si un token de acceso contiene el valor esperado de referencia de método de autenticación (AMR) o no:

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
  "family_name": "Adminagent",
  "given_name": "CSP",
  "ipaddr": "127.0.0.1",
  "name": "Adminagent CSP",
  "oid": "4988e250-5aee-482a-9136-6d269cb755c0",
  "scp": "user_impersonation",
  "tenant_region_scope": "NA",
  "tid": "df845f1a-7b35-40a2-ba78-6481de91f8ae",
  "unique_name": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "upn": "Adminagent.csp@testtestpartner.onmicrosoft.com",
  "ver": "1.0"
}
```

Si el valor está presente, el Centro de partners concluye que se completó la comprobación de MFA y procesa la solicitud de API. Si el valor no está presente, la API del Centro de partners rechazará la solicitud con la siguiente respuesta:

``` csharp
HTTP/1.1 401 Unauthorized - MFA required
Transfer-Encoding: chunked
Request-Context: appId=cid-v1:03ce8ca8-8373-4021-8f25-d5dd45c7b12f
WWW-Authenticate: Bearer error="invalid_token"
Date: Thu, 14 Feb 2019 21:54:58 GMT
```

Cuando se usa la autenticación de solo aplicación, las API que la admitan funcionarán continuamente sin solicitar la MFA.

## <a name="partner-delegated-administration"></a>Administración delegada de partner

### <a name="using-service-portals"></a>Uso de portales de servicio

Las cuentas de partners, incluidos los agentes de administrador y los agentes del departamento de soporte técnico, pueden usar los privilegios de administrador delegado de partner para administrar los recursos de los clientes a través de los portales de Microsoft Online Services, la interfaz de la línea de comandos (CLI) y las API (mediante la autenticación de aplicación y usuario).

Al acceder a los portales de Microsoft Online Services con los privilegios de administrador delegado de partner (administrador con derechos delegados) para administrar los recursos de los clientes, muchos de estos portales requieren que la cuenta de partner se autentique de forma interactiva, con el inquilino de Azure Active Directory del cliente establecido como el contexto de autenticación: es necesario que la cuenta de partner inicie sesión en el inquilino de cliente.

Cuando Azure Active Directory reciba estas solicitudes de autenticación, requerirá que la cuenta de partner complete la comprobación de MFA. Hay dos experiencias de usuario posibles, en función de si la cuenta de partner es una identidad administrada o federada:

- Si la cuenta de partner es una identidad **administrada**, Azure Active Directory le pedirá directamente al usuario que complete la comprobación de MFA. Si la cuenta de partner no se ha registrado para MFA con Azure Active Directory previamente, se le pedirá al usuario que [complete el registro de MFA](#mfa-registration-experience) en primer lugar.

- Si la cuenta de partner es una identidad **federada**, la experiencia depende de la forma en que el administrador de partners haya configurado la federación en Azure Active Directory. Al configurar la federación en Azure Active Directory, el administrador de partners puede indicar a Azure Active Directory si el proveedor de identidades federado admite MFA o no. Si lo hace, Azure Active Directory redirigirá el usuario al proveedor de identidades federado para completar la comprobación de MFA. En otro caso, Azure Active Directory le pedirá directamente al usuario que complete la comprobación de MFA. Si la cuenta de partner no se ha registrado para MFA con Azure Active Directory previamente, se le pedirá al usuario que [complete el registro de MFA](#mfa-registration-experience) en primer lugar.

La experiencia general es similar al escenario en el que un inquilino de cliente final ha implementado MFA para sus administradores. Por ejemplo, el inquilino de cliente ha habilitado los [valores predeterminados de seguridad de Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), lo que requiere que todas las cuentas con derechos administrativos inicien sesión en el inquilino de cliente con la comprobación de MFA, incluidos los agentes de administrador y los agentes del departamento de soporte técnico. Con fines de prueba, los partners pueden habilitar los [valores predeterminados de seguridad de Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) en el inquilino de cliente y, a continuación, intentar usar los privilegios de administración delegada de partner para acceder al inquilino de cliente.

> [!NOTE]
> No todos los portales de Microsoft Online Services requieren que las cuentas de partners inicien sesión en el inquilino de cliente al acceder a los recursos de los clientes mediante privilegios de administrador delegado de partner. En su lugar, solo requieren que las cuentas de partners inicien sesión en el inquilino de partner. Un ejemplo es el Centro de administración de Exchange. Con el tiempo, esperamos que estos portales requieran que las cuentas de partners inicien sesión en el inquilino de cliente al usar privilegios de administrador delegado de partner.

### <a name="using-service-apis"></a>Uso de las API de servicio
Algunas API de Microsoft Online Services (por ejemplo, Azure Resource Manager, Azure AD Graph, Microsoft Graph, etc.) admiten que los partners con privilegios de administrador delegado de partner administren los recursos del cliente mediante programación. Para sacar provecho de los privilegios de administrador delegado de partner con estas API, la aplicación de partner debe incluir un token de acceso en el encabezado de autorización de solicitud de API, donde el token de acceso se obtiene teniendo una cuenta de usuario de partner para autenticarse con Azure AD, con la instancia de Azure AD del cliente establecida como el contexto de autenticación. Es necesario que la aplicación de partner tenga una cuenta de usuario de partner que inicie sesión en el inquilino de cliente.

Cuando Azure AD reciba esta solicitud de autenticación, requerirá que la cuenta de usuario de partner complete la comprobación de MFA. Si la cuenta de usuario de partner no se ha registrado para MFA previamente, se le pedirá al usuario que complete primero el registro de MFA.

Esta característica afecta a todas las aplicaciones de partner que se integran con estas API con privilegios de administrador delegado de partner. Para asegurarte de que las aplicaciones de partner pueden continuar funcionando con estas API sin interrupción:

- El partner debe evitar el uso de métodos de autenticación de usuarios no interactivos con Azure AD para obtener el token de acceso. Cuando se usa un método de autenticación de usuario no interactivo, como el [flujo de contraseña](https://github.com/AzureAD/azure-activedirectory-library-for-dotnet/wiki/Acquiring-tokens-with-username-and-password), Azure AD no podrá pedir al usuario que complete la comprobación de MFA. El partner debe cambiar al uso del método de autenticación de usuario interactivo, como el [flujo de OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v1-protocols-openid-connect-code) en su lugar.
- Durante el método de autenticación de usuario interactivo, el partner debe usar una cuenta de usuario de partner que ya esté habilitada para MFA. Como alternativa, cuando Azure AD lo pida, el partner puede completar el registro de MFA y la comprobación de MFA durante el inicio de sesión.
- Es similar al escenario en el que un inquilino de cliente final ha implementado MFA para sus administradores. Por ejemplo, el inquilino de cliente ha habilitado los [valores predeterminados de seguridad de Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), lo que requiere que todas las cuentas de usuario con derechos administrativos inicien sesión en el inquilino de cliente con la comprobación de MFA, incluidos los agentes de administrador y los agentes del departamento de soporte técnico. Para la prueba, los partners pueden habilitar los [valores predeterminados de seguridad de Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) en el inquilino de cliente y, a continuación, intentar usar los privilegios de administración delegada de partner para acceder mediante programación al inquilino de cliente.

### <a name="mfa-registration-experience"></a>Experiencia de registro de MFA
Durante la comprobación de MFA, si la cuenta de partner no se ha registrado para MFA previamente, Azure AD le pedirá al usuario que complete primero el registro de MFA:

![Paso 1 del registro de MFA](images/MfaRegistration1.png)

Después de hacer clic en **Siguiente**, se le pedirá al usuario que elija entre una lista de métodos de verificación.

![Paso 2 del registro de MFA](images/MfaRegistration2.png)

Después de que el registro se haya realizado correctamente, es necesario que el usuario complete la comprobación de MFA en función de la comprobación haya elegido.



## <a name="request-for-technical-exception"></a>Solicitud de excepción técnica

Los partners pueden aplicar una excepción técnica para suprimir la comprobación de MFA en caso de que se encuentren problemas técnicos con Microsoft Online Services y no haya ninguna solución o alternativa factible. Antes de hacerlo, revisa las siguientes secciones:

 - [Lista de problemas comunes comunicados por los partners](#list-of-common-issues-reported-by-partners)
 - [Cómo enviar una solicitud de excepción técnica](#how-to-submit-a-request-for-technical-exception)
 
### <a name="list-of-common-issues-reported-by-partners"></a>Lista de problemas comunes comunicados por los partners
Antes de solicitar una excepción técnica, revisa la lista de problemas comunes que han comunicado otros partners para saber si son motivos válidos para la excepción técnica o no.

#### <a name="issue-1-partner-needs-more-time-to-implement-mfa-for-their-partner-agents"></a>Problema 1: El partner necesita más tiempo para implementar MFA para sus agentes de partner
Un partner no se ha iniciado o todavía está en proceso de implementar MFA para sus agentes de partner que requieren acceso a los portales de Microsoft Online Services con privilegios de administración delegada de partner para administrar los recursos de los clientes. El partner necesita más tiempo para completar la implementación de MFA. ¿Es este problema un motivo válido para la excepción técnica?

**Respuesta**: No. El partner debe crear planes para implementar MFA para sus usuarios y evitar las interrupciones.

> [!NOTE]
> Aunque el partner no haya implementado MFA para los agentes de partner, estos pueden seguir accediendo a los portales de Microsoft Online Services con privilegios de administración delegada de partner, siempre que puedan completar el registro de MFA y la comprobación de MFA cuando se les solicite durante el inicio de sesión en el inquilino de cliente. Al completar el registro de MFA no se habilita automáticamente el usuario para MFA.

##### <a name="issue-2-partner-has-not-implemented-mfa-for-user-accounts-not-using-delegated-admin-privileges"></a>Problema 2: El partner no ha implementado MFA para las cuentas de usuario que no usan privilegios de administrador delegado
Un partner tiene varios usuarios en sus inquilinos de partner que no requieren acceder a los portales de Microsoft Online Services para administrar los recursos de los clientes con privilegios de administración delegada de partner. El partner está en proceso de implementar MFA para estos usuarios y necesita más tiempo para que se complete. ¿Es este problema un motivo válido para la excepción técnica?

**Respuesta**: No. Puesto que estas cuentas de usuario no usan privilegios de administración delegada de partner para administrar los recursos de los clientes, no se les pedirá que inicien sesión en el inquilino del cliente. No se verán afectados porque Azure AD requiera la comprobación de MFA durante el inicio de sesión en el inquilino de cliente.

##### <a name="issue-3-partner-has-not-implemented-mfa-for-user-service-accounts"></a>Problema 3: El partner no ha implementado MFA para las cuentas de servicio de usuario
Un partner tiene algunas cuentas de usuario en sus inquilinos de partner, que los dispositivos usan como cuentas de servicio. Son cuentas con pocos privilegios que no requieren acceder al Centro de partners ni a los portales de Microsoft Online Services para administrar los recursos de los clientes con privilegios de administración delegada de partner. ¿Es este problema un motivo válido para la excepción técnica?

**Respuesta**: No. Puesto que estas cuentas de usuario no usan privilegios de administración delegada de partner para administrar los recursos de los clientes, no se les pedirá que inicien sesión en el inquilino del cliente. No se verán afectados porque Azure AD requiera la comprobación de MFA durante el inicio de sesión en el inquilino de cliente.

#### <a name="issue-4-partner-cannot-implement-mfa-using-ms-authenticator-app"></a>Problema 4: El partner no puede implementar MFA con la aplicación autenticadora de MS
Un partner tiene una directiva "dispositivo limpio", que no permite que los empleados traigan sus dispositivos móviles personales a su área de trabajo. Sin acceso a sus dispositivos móviles personales, los empleados no pueden instalar la aplicación MS Authenticator, que es la única verificación de MFA compatible con los valores predeterminados de seguridad de Azure AD. ¿Es este problema un motivo válido para la excepción técnica?

**Respuesta**: No, no es un motivo válido para la excepción técnica. El partner debe tener en cuenta las alternativas siguientes para que sus empleados puedan completar la comprobación de MFA al acceder al Centro de partners:
- El partner también puede registrarse para Azure AD Premium o soluciones de MFA de terceros (compatibles con Azure AD) que pueden proporcionar métodos de verificación adicionales.

#### <a name="issue-5-partner-cannot-implement-mfa-due-to-the-use-of-legacy-authentication-protocols"></a>Problema 5: El partner no puede implementar MFA debido al uso de protocolos de autenticación heredados
Un partner tiene algunos agentes de partner que todavía usan protocolos de autenticación heredados, que no son compatibles con MFA. Por ejemplo, los usuarios siguen usando Outlook 2010, que se basa en protocolos de autenticación heredados. Al habilitar MFA para estos agentes de partner se interrumpirá el uso de protocolos de autenticación heredados.

**Respuesta**: No, no es un motivo válido para la excepción técnica. Se recomienda encarecidamente a los partners que dejen de usar los protocolos de autenticación heredados debido a posibles implicaciones de seguridad, ya que estos protocolos no se pueden proteger con la comprobación de MFA y son mucho más susceptibles a poner en peligro las credenciales. Si no es una opción dejar de usar los protocolos de autenticación heredados, los partners deben considerar la posibilidad de suscribirse a Azure AD Premium, que admite el uso de contraseñas de aplicación. Las contraseñas de aplicación son contraseñas de un solo uso generadas por el sistema y suelen ser más seguras que las contraseñas generadas por personas. Mediante el uso de contraseñas de aplicación, los partners pueden implementar MFA para sus usuarios, mientras recurren a las contraseñas de aplicación solo para los protocolos de autenticación heredados.

Lee la publicación sobre la [autenticación básica y Exchange Online](https://techcommunity.microsoft.com/t5/exchange-team-blog/basic-auth-and-exchange-online-february-2020-update/ba-p/1191282) para comprender el plan más reciente para admitir la autenticación heredada para Outlook y sigue el [blog del equipo de Exchange](https://techcommunity.microsoft.com/t5/exchange-team-blog/bg-p/Exchange) para recibir noticias futuras. 

> [!NOTE]
> Aunque el partner no haya implementado MFA para los agentes de partner, estos pueden seguir accediendo a los portales de Microsoft Online Services con privilegios de administración delegada de partner, siempre que puedan completar el registro de MFA y la comprobación de MFA cuando se les solicite durante el inicio de sesión en el inquilino de cliente. Al completar el registro de MFA no se habilita automáticamente el usuario para MFA.

#### <a name="issue-6-partner-has-implemented-third-party-mfa-that-isnt-recognized-by-azure-ad"></a>Problema 6: El partner ha implementado una instancia de MFA de terceros que Azure AD no reconoce
Un partner ha implementado MFA para sus usuarios mediante una solución de MFA de terceros. Sin embargo, el partner no puede configurar correctamente la solución MFA de terceros para retransmitir a Azure AD que se ha completado la verificación de MFA durante la autenticación del usuario. ¿Es esto un motivo válido para la excepción técnica?

**Respuesta**: Sí, este problema puede considerarse un motivo válido para la excepción técnica. Antes de enviar una solicitud de excepción técnica, confirma con el proveedor de soluciones de MFA de terceros que no se puede configurar la solución MFA para que fluya la notificación *authenticationmethodsreferences* (con el valor *multipleauthn*) a Azure AD para indicar que se ha completado la verificación de MFA durante la autenticación del usuario. Al enviar una solicitud de excepción técnica, debes proporcionar los detalles de la solución de MFA de terceros usada e indicar el método de integración (por ejemplo, a través de la federación de identidades o el uso del control personalizado de Azure AD), además de proporcionar la siguiente información en la solicitud de excepción técnica como documentos complementarios:
* Configuraciones de MFA de terceros. 
* El resultado de [probar los requisitos de seguridad de los partners](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements) que ejecuta la cuenta con MFA de terceros habilitada.
* El pedido de compra de la solución de MFA de terceros que usas o tienes previsto usar.


### <a name="how-to-submit-a-request-for-technical-exception"></a>Cómo enviar una solicitud de excepción técnica

Para enviar una solicitud de excepción técnica:

1. Inicia sesión en el Centro de partners como administrador global o agente de administrador.
2. Crea una nueva solicitud de servicio de partner navegando hasta **Soporte técnico** > **Partner support requests** (Solicitudes de soporte técnico de partners) y haciendo clic en **Nueva solicitud**.
3. Busca **MFA - Request for exception** (MFA: solicitud de excepción) en el cuadro de búsqueda o selecciona **CSP** en Categoría. A continuación, selecciona **Cuentas, Incorporación, Acceso** en Tema. Finalmente, selecciona **MFA - Request for exception** (MFA: solicitud de excepción) en el subtema y, luego, el **paso siguiente**.
4. Proporciona los detalles solicitados para enviar una solicitud de servicio de excepción técnica y haz clic en **Enviar**.

Microsoft puede tardar hasta tres días laborables en proporcionar una respuesta a la solicitud de excepción técnica.
