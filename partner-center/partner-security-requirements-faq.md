---
title: Preguntas más frecuentes sobre los requisitos de seguridad para partners | Centro de partners
ms.topic: article
ms.date: 11/09/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Preguntas más frecuentes sobre los requisitos de seguridad para partners
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, Cloud Solution Provider, Cloud Solution Provider program, CSP, Control Panel Vendor, CPV, multi-factor authentication, MFA, secure application model, secure app model, security
ms.localizationpriority: high
ms.openlocfilehash: 1a452b3d67abdfb1eabe4a3e85f458b085cc141d
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004274"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Preguntas más frecuentes sobre los requisitos de seguridad para partners

**Roles adecuados**
-   Administrador global
-   Administrador de usuarios
-   Agente de administración
-   Administrador de facturación
-   Administrador de partners de MPN

En este artículo se incluyen algunas preguntas frecuentes sobre los [requisitos de seguridad para partners](partner-security-requirements.md).

## <a name="partner-security-requirements"></a>Requisitos de seguridad para partners

### <a name="what-are-the-key-timelines-and-milestones"></a>¿Cuáles son las líneas de tiempo e hitos clave?

Los términos asociados con estos requisitos de seguridad se incluyen en el acuerdo entre partners de Microsoft. Tendrás que implementar estos requisitos de seguridad para la conformidad de tu participación en el programa Proveedor de soluciones en la nube.

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>¿Qué sucederá si no hago nada?

Los partners que no se atengan a estas prácticas y obligaciones de seguridad no podrán realizar transacciones en el programa Proveedor de soluciones en la nube ni administrar los inquilinos de cliente que aprovechen los derechos de administrador delegado, una vez que se apliquen estos requisitos de seguridad para partners. Estamos en el proceso de establecer una fecha de aplicación de los requisitos y se la notificaremos a los partners con información detallada.

### <a name="what-will-happen-if-i-do-not-implement-these-partner-security-requirements"></a>¿Qué ocurrirá si no implemento estos requisitos de seguridad de para partners?

El acuerdo entre partners de Microsoft requiere que apliques la autenticación multifactor para las cuentas de usuario y que adoptes el modelo de aplicaciones seguras para interactuar con la API del Centro de partners. Los partners que no cumplan estas prácticas de seguridad pueden perder la capacidad de realizar transacciones en el programa Proveedor de soluciones en la nube o administrar los inquilinos de cliente aprovechando los derechos de administrador delegado.

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>¿Por qué impone Microsoft estos nuevos requisitos?

La seguridad y privacidad de los clientes y partners es la máxima prioridad de Microsoft. Seguimos observando un número creciente y más sofisticado de ataques de seguridad relacionados principalmente con incidentes de riesgo para la identidad. Como los controles preventivos juegan un papel clave en una estrategia de defensa general para frustrar los ataques de seguridad, comenzaremos a aplicar un conjunto de requisitos de seguridad obligatorios para ayudar a proteger a los partners y sus clientes.

### <a name="does-this-apply-to-all-geographies"></a>¿Se aplica a todas las zonas geográficas?

Sí, se aplica a todas las zonas geográficas. Se recomienda encarecidamente a todos los partners que realicen transacciones a través de una nube soberana (21Vianet, gobierno de EE. UU. y Alemania) adopten estos nuevos requisitos de seguridad de inmediato. Sin embargo, no es preciso que estos partners cumplan los nuevos requisitos de seguridad que entran en vigor el 1 de agosto. En el futuro, Microsoft proporcionará más información acerca de la aplicación de estos requisitos de seguridad para las nubes soberanas.

### <a name="is-it-possible-to-get-an-exclusion-for-an-account"></a>¿Es posible obtener una exclusión para una cuenta?

No, no es posible excluir ninguna cuenta de usuario del requisito de aplicación de MFA. Dada la naturaleza altamente privilegiada de los partners, el acuerdo entre partners de Microsoft requiere que se aplique la autenticación multifactor para cada cuenta de usuario en el inquilino de partner.

### <a name="how-do-i-know-if-i-have-met-the-partner-security-requirements"></a>¿Cómo puedo saber si cumplo los requisitos de seguridad del partner?

Debes completar los pasos siguientes.

- Deberás cumplir todos los requisitos descritos en los [requisitos de seguridad del partner](https://docs.microsoft.com/partner-center/partner-security-requirements).
- Debes asegurarte de que todas las cuentas de usuario del inquilino del partner tienen aplicada la autenticación multifactor.

Para ayudar a identificar las áreas principales en las que se pueden realizar acciones, proporcionamos el informe de [estado de los requisitos de seguridad](https://partner.microsoft.com/pcv/security/compliance), que está disponible a través del Centro de partners.

Consulta el [estado de los requisitos de seguridad del partner](https://docs.microsoft.com/partner-center/partner-security-compliance) para obtener más información sobre el informe de estado.

## <a name="required-actions"></a>Acciones necesarias

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>¿Cuáles son las acciones clave que hay que realizar para cumplir los requisitos?

Todos los partners del programa CSP (factura directa, proveedor indirecto y revendedor indirecto), las instancias de Advisor y los proveedores de panel de control deben cumplir los requisitos.

1. **Aplicar MFA a todos los usuarios**

    Todos los partners del programa CSP, las instancias de Advisor y los proveedores de panel de control deben aplicar MFA para todos los usuarios de su inquilino de partner.

    Consideraciones adicionales:

    - Los proveedores indirectos deben trabajar con los revendedores indirectos para incorporarlos al Centro de partners, si aún no lo han hecho, y animar a sus revendedores a que cumplan los requisitos.
    - Azure MFA se pone a disposición de todos los usuarios del inquilino de partner sin coste alguno, a través de los valores predeterminados de seguridad de Azure AD con el único método de comprobación de una aplicación autenticadora que admite contraseñas de un solo uso basadas en el tiempo (TOTP).
    - Existen métodos de comprobación adicionales a través de las SKU de [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium), si se requieren otros métodos, como una llamada telefónica o un mensaje de texto.
    - Los asociados también pueden utilizar una solución de MFA de terceros para cada cuenta al acceder a los servicios en la nube comerciales de Microsoft.

2. **Adoptar el marco de modelo de aplicaciones seguras**

    Todos los partners que hayan desarrollado una integración personalizada con cualquier API (como Azure Resource Manager, Microsoft Graph, Partner Center API, etc.) o que hayan implementado la automatización personalizada mediante herramientas como PowerShell, deberán adoptar el [marco de modelo de aplicaciones seguras](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) para integrarse con los servicios en la nube de Microsoft. Si no lo hacen, puede producirse una interrupción debido a la implementación de MFA. Los siguientes recursos proporcionan información general e instrucciones sobre cómo adoptar el modelo.

    - [Información general sobre el modelo de aplicaciones seguras](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [Centro de partners: guía del modelo de aplicaciones seguras](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Partners del programa CSP: código de ejemplo .NET para habilitar el modelo de aplicaciones seguras](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
    - [Partners del programa CSP: código Java de ejemplo para habilitar el modelo de aplicaciones seguras](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
    - [Documento de autenticación del Centro de partners](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [Documento de Multi-Factor Authentication (MFA) de PowerShell del Centro de partners](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

    Si usas un panel de control, debes consultar al proveedor sobre la adopción del marco de modelo de aplicaciones seguras.

    Los proveedores de panel de control deben [incorporarse](https://docs.microsoft.com/partner-center/enroll-as-cpv) al Centro de partners como proveedores de panel de control y empezar a implementar este requisito inmediatamente. Consulta [Partner Center: Secure Application Model framework](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) (Centro de partners: marco de modelo de aplicaciones seguras). Los proveedores de panel de control deben aceptar y administrar el consentimiento de los partners de CSP en lugar de las credenciales y purgar todas las credenciales existentes de los partners de CSP.

## <a name="multi-factor-authentication"></a>Autenticación multifactor

### <a name="what-is-multi-factor-authentication-mfa"></a>¿Qué es Multi-Factor Authentication (MFA)?

MFA es un mecanismo de seguridad a través del cual los usuarios se autentican con más de un procedimiento obligatorio de seguridad y validación. Funciona al requerir dos o varios de los siguientes métodos de autenticación:

- Un elemento que el usuario conoce (por lo general, una contraseña)
- Un elemento que el usuario posee (un dispositivo de confianza que no puede duplicarse fácilmente como, por ejemplo, un teléfono)
- Un elemento que identifica al usuario personalmente (biométrica)

### <a name="what-is-the-cost-of-enabling-mfa"></a>¿Cuál es el costo de habilitar MFA?

Microsoft proporciona MFA sin coste alguno a través de la implementación de los valores predeterminados de seguridad de Azure AD. La única opción de comprobación disponible a través de esta versión de MFA es una aplicación autenticadora. Si se requiere una llamada telefónica o un mensaje SMS, se deberá adquirir una licencia de [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium). Como alternativa, puedes utilizar una solución de terceros para proporcionar MFA para cada usuario del inquilino de partner: en este caso, es tu responsabilidad asegurarte de que la solución MFA se aplique y que sea compatible.

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>Si ya tengo una solución MFA, ¿qué acciones debo realizar?

Con estos requisitos de seguridad, se requerirá a los usuarios de un inquilino de partner que se autentiquen mediante MFA al acceder a los servicios en la nube comerciales de Microsoft. Se puede usar una solución de terceros para cumplir estos requisitos. Microsoft ya no proporciona pruebas de validación a proveedores de identidades independientes para compatibilidad con Azure Active Directory. Si quieres probar el producto para la interoperabilidad, consulta estas [instrucciones.](https://www.microsoft.com/download/details.aspx?id=56843)

> [!IMPORTANT]
> Si usa una solución de terceros, es importante comprobar que la solución emita la declaración de notificación de referencia del método de autenticación (AMR) que incluye el valor de MFA. Consulte [Testing the Partner Security Requirements](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements) (Prueba de los requisitos de seguridad para partners) para obtener más información sobre cómo validar la solución de terceros que está emitiendo la notificación esperada.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Utilizo varios inquilinos de partner para realizar transacciones. ¿Tengo que implementar MFA en todos ellos?

Sí, tendrás que aplicar MFA para cada inquilino de Azure Active Directory asociado con el programa CSP o el programa Advisor. Si tienes previsto comprar una licencia de Azure Active Directory Premium, debes adquirir una licencia para el usuario en cada inquilino de Azure Active Directory.

### <a name="does-each-user-account-in-my-partner-tenant-need-to-have-mfa-enforced"></a>¿Es necesario aplicar MFA en cada cuenta de usuario de mi inquilino de partner?

Sí, es necesario aplicar MFA en cada usuario. Ten en cuenta que, si usas valores predeterminados de seguridad de Azure AD, no se requiere ninguna acción adicional, ya que esas características aplican MFA para todas las cuentas de usuario. Sin embargo, habilitar los valores predeterminados de seguridad es una forma gratuita y sencilla de asegurarse de que las cuentas de usuario son compatibles con MFA y no se ven afectadas cuando se aplica MFA.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Soy un partner de factura directa con Microsoft. ¿Qué tengo que hacer?

Los partners de Proveedor de soluciones en la nube de factura directa deben aplicar MFA para cada usuario en su inquilino de partner.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>Soy un revendedor indirecto y solo realizo transacciones a través de un distribuidor. ¿También tengo que hacer esto?

Todos los revendedores indirectos tienen que aplicar MFA para cada usuario en su inquilino de partner. Se trata de una acción que el revendedor indirecto debe realizar.

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>No uso Partner Center API. ¿También tengo que implementar MFA?

Sí, este requisito de seguridad es para todos los usuarios, incluidos los usuarios administradores de partner y los usuarios finales de un inquilino de partner.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>¿Qué proveedores de terceros proporcionan soluciones MFA compatibles con Azure Active Directory?

Existe muchas revisiones independientes de las soluciones MFA en línea, como [Gartner](https://www.gartner.com/en/webinars/3881781). Al revisar los proveedores y las soluciones de MFA, los partners deben asegurarse de que la solución que elijan sea compatible con Azure Active Directory.

Microsoft ya no proporciona pruebas de validación a proveedores de identidades independientes para compatibilidad con Azure Active Directory. Si quieres probar el producto para la interoperabilidad, consulta estas [instrucciones.](https://www.microsoft.com/download/details.aspx?id=56843)

Para obtener más información, consulta la [Lista de compatibilidad de federación de Azure AD](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>¿Cómo puedo probar MFA en nuestro espacio aislado de integración?

La característica de valores predeterminados de seguridad de Azure AD debe estar habilitada o, como alternativa, puedes utilizar una solución de terceros que utilice la federación.

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>¿Afectará la habilitación de MFA a cómo interactúo con el inquilino de mi cliente?

No. El cumplimiento de estos requisitos de seguridad no afectará a la forma de administrar los clientes. La capacidad de realizar operaciones administrativas delegadas no se interrumpirá.

### <a name="are-my-customers-subject-to-the-partner-security-requirements"></a>¿Están sujetos mis clientes a los requisitos de seguridad para partners?

No, no es necesario aplicar MFA para cada usuario en los inquilinos de Azure AD de los clientes. Sin embargo, se recomienda que trabajes con cada cliente para determinar la mejor manera de proteger a sus usuarios.

### <a name="can-any-user-be-excluded-from-this-requirement"></a>¿Se puede excluir de este requisito a algún usuario?

No, todos los usuarios, incluidas las cuentas de servicio, del inquilino de partner deberán autenticarse mediante MFA.

### <a name="do-the-partner-security-requirements-apply-to-the-integration-sandbox"></a>¿Se aplican los requisitos de seguridad para partners al espacio aislado de integración?

Sí, los requisitos de seguridad para partners se aplican al espacio aislado de integración. Esto significa que deberás implementar la solución MFA adecuada para los usuarios del inquilino de espacio aislado de integración. Se recomienda implementar los valores predeterminados de seguridad de Azure AD para proporcionar MFA.

### <a name="how-do-i-configure-an-emergency-access-break-glass-account"></a>¿Cómo configuro una cuenta de acceso de emergencia (rotura del cristal)?

Se consideró una práctica recomendada crear una o dos cuentas de acceso de emergencia para evitar bloquear de forma inadvertida el inquilino de Azure AD. Con respecto a los requisitos de seguridad para partners, es necesario que cada usuario se autentique mediante MFA. Por lo tanto, esto significa que tendrás que modificar la definición de una cuenta de acceso de emergencia. Podría tratarse de una cuenta que utiliza una solución de terceros para MFA.

### <a name="if-i-am-using-a-third-party-solution-is-active-directory-federation-service-adfs-required"></a>Si uso una solución de terceros, ¿se necesitan los Servicios de federación de Active Directory (ADFS)?

No, no es necesario tener los Servicios de Federación de Active Directory (ADFS) si usas una solución de terceros. Se recomienda que trabajes con el proveedor de la solución para determinar cuáles son los requisitos de su solución.

### <a name="is-it-a-requirement-to-enable-azure-ad-security-defaults"></a>¿Es necesario habilitar los valores predeterminados de seguridad de Azure AD?

No, no es necesario habilitar los valores predeterminados de seguridad de Azure AD.

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>¿Se puede usar el acceso condicional para cumplir el requisito de MFA?

Sí, se puede usar el acceso condicional para aplicar MFA para cada usuario, incluidas las cuentas de servicio, en el inquilino de partner. Sin embargo, dada la naturaleza de los partners, que tienen privilegios elevados, necesitamos asegurarnos de que cada usuario tenga que usar MFA en todas y cada una de las autenticaciones. Esto significa que no podrás utilizar la característica de acceso condicional para eludir el requisito de MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>¿La cuenta de servicio usada por Azure AD Connect se verá afectada por los requisitos de seguridad para partners?

No, la cuenta de servicio usada por Azure AD Connect no se verá afectada por los requisitos de seguridad para partners. Si experimentas un problema con Azure AD Connect como consecuencia de la aplicación de MFA, abre una solicitud de soporte técnico en el soporte técnico de Microsoft.

## <a name="secure-application-model"></a>Modelo de aplicaciones seguras

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>¿Quién debe adoptar el modelo de aplicaciones seguras para cumplir con los requisitos?

Microsoft está introduciendo un marco seguro y escalable para autenticar los partners de Proveedor de soluciones en la nube (CSP) y Proveedores de panel de control (CPV) que utiliza Multi-Factor Authentication. Para más información, consulta la [guía del modelo de aplicaciones seguras ](https://assetsprod.microsoft.com/secure-application-model-guide.pdf). Todos los partners que hayan desarrollado una integración personalizada con cualquier API (como Azure Resource Manager, Microsoft Graph, Partner Center API, etc.) o que hayan implementado la automatización personalizada mediante herramientas como PowerShell, deberán adoptar el [marco de modelo de aplicaciones seguras](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) para integrarse con los servicios en la nube de Microsoft.

### <a name="what-is-the-secure-application-model"></a>¿Qué es el modelo de aplicaciones seguras?

Microsoft está introduciendo un marco seguro y escalable para autenticar los partners de Proveedor de soluciones en la nube (CSP) y Proveedores de panel de control (CPV) que utiliza Multi-Factor Authentication. Para más información, consulta la [guía del modelo de aplicaciones seguras ](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).  

### <a name="how-do-i-implement-the-secure-application-model"></a>¿Cómo implemento el modelo de aplicaciones seguras?

Todos los partners que hayan desarrollado una integración personalizada con cualquier API (como Azure Resource Manager, Microsoft Graph, Partner Center API, etc.) o que hayan implementado la automatización personalizada mediante herramientas como PowerShell, deberán adoptar el [marco de modelo de aplicaciones seguras](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) para integrarse con los servicios en la nube de Microsoft. Si no lo hacen, puede producirse una interrupción debido a la implementación de MFA. Los siguientes recursos proporcionan información general e instrucciones sobre cómo adoptar el modelo.

- [Información general sobre el modelo de aplicaciones seguras](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Centro de partners: guía del modelo de aplicaciones seguras](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partners del programa CSP: código de ejemplo .NET para habilitar el modelo de aplicaciones seguras](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partners del programa CSP: código Java de ejemplo para habilitar el modelo de aplicaciones seguras](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Documento de autenticación del Centro de partners](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento de Multi-Factor Authentication (MFA) de PowerShell del Centro de partners](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

Si usas un panel de control, debes consultar al proveedor sobre la adopción del marco de modelo de aplicaciones seguras.

Los proveedores de panel de control deben [incorporarse](https://docs.microsoft.com/partner-center/enroll-as-cpv) al Centro de partners como proveedores de panel de control y empezar a implementar este requisito inmediatamente. Consulta [Partner Center: Secure Application Model framework](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) (Centro de partners: marco de modelo de aplicaciones seguras). Los proveedores de panel de control deben aceptar y administrar el consentimiento de los partners de CSP en lugar de las credenciales y purgar todas las credenciales existentes de los partners de CSP.

### <a name="who-is-a-control-panel-vendor-cpv"></a>¿Quién es el proveedor de panel de control (CPV)?

Un proveedor de panel de control es un fabricante de software independiente que desarrolla aplicaciones para que las usen los partners de CSP para la integración con Partner Center API. Un proveedor de panel de control no es un partner de CSP con acceso directo a las API o al panel del Centro de partners. Está disponible una descripción detallada en [Centro de partners: guía del modelo de aplicaciones seguras](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>¿Se tiene que implementar el modelo de aplicaciones seguras para la API/SDK del Centro de partners únicamente?

A través de la aplicación de la autenticación multifactor para todas las cuentas de usuario, cualquier automatización o integración que esté diseñada para ejecutarse de forma no interactiva se verá afectada. Aunque los requisitos de seguridad de partner requieren que habilites el modelo de aplicaciones seguras para la API del Centro de partners, se puede aprovechar para solucionar la necesidad de un segundo factor de autenticación con automatización e integración. Ten en cuenta que el recurso al que se tiene acceso necesitará se compatible con la autenticación basada en tokens de acceso.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Uso herramientas de automatización como PowerShell. ¿Cómo implemento el modelo de aplicaciones seguras?

Si la automatización está pensada para ejecutarse de forma no interactiva y se basa en credenciales de usuario para la autenticación, deberás implementar el modelo de aplicaciones seguras. Consulta [Secure Application Model | Partner Center PowerShell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) (Modelo de aplicaciones seguras | Powershell del Centro de partners) para obtener instrucciones de cómo implementar este marco.  Ten en cuenta que no todas las herramientas de automatización proporcionan la capacidad de autenticación mediante tokens de acceso. Si necesitas ayuda para comprender los cambios que deben hacerse, publica un mensaje en el grupo de [Partner Center Security Guidance](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) (Instrucciones de seguridad del Centro de partners).

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>¿Qué credenciales de usuario debe proporcionar el administrador de aplicaciones al realizar el proceso de consentimiento?

Se recomienda usar una cuenta de servicio que tenga asignados permisos privilegiados mínimos. Con respecto a Partner Center API, significa que debes usar una cuenta que tenga asignado el rol Agente de ventas o Agente de administración.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>¿Por qué el administrador de aplicaciones no debe proporcionar credenciales globales de usuario administrador al realizar el proceso de consentimiento?

Es un procedimiento recomendado usar privilegios mínimos para reducir el riesgo. No se recomienda usar una cuenta que tenga privilegios de administrador globales porque podría proporcionar más permisos de los que se requieren.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Soy un partner de CSP. ¿Cómo sé si mi proveedor de panel de control (CPV) trabaja en la implementación de la solución o no?

En el caso de partners que usan una solución de proveedor de panel de control (CPV) para realizar transacciones en el programa Proveedor de soluciones en la nube (CSP), es tu responsabilidad consultar con el CPV.

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Soy un CPV. ¿Cómo me inscribo?

Para inscribirte como proveedor de panel de control (CPV), sigue las instrucciones que se proporcionan [aquí](https://docs.microsoft.com/partner-center/enroll-as-cpv).

Para recibir el vínculo de inscripción, los CPV deben ponerse en contacto con [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) y proporcionar un patrocinador de empleado de Microsoft que tenga una relación comercial con el CPV o que conozca su negocio. Por ejemplo, un Administrador de desarrollo de partners (PDM).

Una vez inscrito en el Centro de partners y que hayas registrado las aplicaciones, tendrás acceso a las Partner Center API. Si eres un CPV nuevo, recibirás la información del espacio aislado mediante una notificación del Centro de partners. Una vez que hayas completado la inscripción como Microsoft CPV y aceptado el contrato de CPV, puedes:

1. Administrar la aplicación multiinquilino (agregar aplicaciones a Azure Portal, registrar y anular el registro de aplicaciones en el Centro de partners). Nota: Los CPV deben registrar sus aplicaciones en el Centro de partners para que se les autorice para las Partner Center API. Agregar aplicaciones a Azure Portal solo no autoriza a las aplicaciones de CPV para las Partner Center API.
2. Ver y administrar el perfil de CPV.
3. Puedes ver y administrar los usuarios que necesitan acceso a las funcionalidades de CPV. El único rol que puede tener un CPV es el de Administrador global.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Uso el SDK de Centro de partners. ¿Adoptará automáticamente el SDK el modelo de aplicaciones seguras?

No, tendrás que seguir las instrucciones proporcionadas en la [guía del modelo de aplicaciones seguras](https://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>¿Puedo generar un token de actualización para el modelo de aplicaciones seguras con cuentas que no tienen MFA habilitada?

Sí, se puede generar un token de actualización con una cuenta que no tenga MFA aplicada. Sin embargo, no debería hacerse porque los tokens generados con una cuenta que no tiene MFA habilitada no podrán tener acceso a los recursos debido al requisito de MFA.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>¿Cómo debe obtener mi aplicación un token de acceso si se habilita MFA?

Deberá seguir la [guía del modelo de aplicaciones seguras](https://assetsprod.microsoft.com/secure-application-model-guide.pdf), que proporciona detalles sobre cómo hacerlo mientras cumple con los nuevos requisitos de seguridad. Puedes encontrar código .NET de ejemplo [aquí](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) y código Java de ejemplo [aquí](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model).

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Como CPV, ¿creo una aplicación de Azure AD en nuestro inquilino de CPV o en el inquilino del partner de CSP?

El CPV deberá crear la aplicación de Azure Active Directory en el inquilino asociado a su inscripción como CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Soy un CSP que usa la autenticación de solo aplicación. ¿Tengo que realizar algún cambio?

La autenticación de solo aplicación no se ve afectada, ya que las credenciales de usuario no se usan para solicitar un token de acceso. Si se comparten las credenciales de usuario, los proveedores de panel de control (CPV) deben adoptar el [marco del modelo de aplicaciones seguras](https://assetsprod.microsoft.com/secure-application-model-guide.pdf) y purgar las credenciales de partners existentes que tengan.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Como CPV, ¿puedo utilizar el estilo de autenticación de solo aplicación para obtener tokens de acceso?

No, los partners de proveedor de panel de control no pueden utilizar el estilo de autenticación de solo aplicación para solicitar tokens de acceso en nombre del partner. Deben implementar el modelo de aplicaciones seguras, que usa el estilo de autenticación de aplicación más usuario.

## <a name="enforcement"></a>Cumplimiento

### <a name="i-am-using-a-third-party-mfa-solution-and-i-am-being-blocked-what-should-i-do"></a>Estoy usando una solución de MFA de terceros y estoy bloqueado, ¿qué debo hacer?

Para validar la cuenta que tiene acceso a los recursos para la que se solicita la autenticación multifactor, se comprobará la notificación de [referencia del método de autenticación ](https://tools.ietf.org/html/rfc8176) para ver si se muestra MFA. Algunas soluciones de terceros no emiten esta notificación o no incluyen el valor de MFA. Si falta la notificación o el valor de MFA no aparece en la lista, no hay ninguna manera de determinar si se ha solicitado la autenticación multifactor para la cuenta autenticada. Deberá trabajar con el proveedor de la solución de terceros para determinar las acciones que deben realizarse para que la solución emita la notificación de referencia del método de autenticación.

Consulte [Testing the Partner Security Requirements](https://docs.microsoft.com/powershell/partnercenter/test-partner-security-requirements?view=partnercenterps-2.0) (Prueba de los requisitos de seguridad para partners) si no está seguro de que la solución de terceros esté emitiendo la notificación esperada.

### <a name="mfa-is-blocking-me-from-supporting-my-customer-using-aobo-what-should-i-do"></a>MFA impide que ofrezca soporte técnico al cliente mediante AOBO, ¿qué debo hacer?

La aplicación técnica de los requisitos de seguridad del partner comprobará si se ha solicitado la autenticación multifactor para la cuenta autenticada. Si no se ha hecho, se le redirigirá a la página de inicio de sesión y se le pedirá que se autentique de nuevo. Si el dominio no está federado, después de autenticarse correctamente, se le pedirá que configure la autenticación multifactor. Una vez que haya finalizado, podrá administrar los clientes mediante AOBO. Si el dominio está federado, deberá asegurarse de que se ha solicitado la autenticación multifactor para la cuenta autenticada.

## <a name="key-resources"></a>Recursos clave

### <a name="how-to-get-started"></a>Inicio

- [Requisitos de seguridad para partners: guía paso a paso](https://docs.microsoft.com/partner-center/partner-security-requirements).
- Dirija sus preguntas y comentarios a [Partner Center Security Guidance Group](https://aka.ms/MPCSecurityGuidance) (Grupo de instrucciones de seguridad del Centro de partners).
- Asista a los próximos horarios de oficina de partners y seminarios web. Consulte aquí [la programación y los recursos detallados](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance).

### <a name="resources-for-adopting-secure-application-model"></a>Recursos para adoptar el modelo de aplicaciones seguras

- [Información general sobre el modelo de aplicaciones seguras](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Centro de partners: guía del modelo de aplicaciones seguras](https://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Partners del programa CSP: código de ejemplo .NET para habilitar el modelo de aplicaciones seguras](https://docs.microsoft.com/samples/microsoft/partner-center-dotnet-samples/secure-app-model/)
- [Partners del programa CSP: código Java de ejemplo para habilitar el modelo de aplicaciones seguras](https://docs.microsoft.com/samples/microsoft/partner-center-java-samples/secure-app-model/)
- [Documento de autenticación del Centro de partners](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento de Multi-Factor Authentication (MFA) de PowerShell del Centro de partners](https://docs.microsoft.com/powershell/partnercenter/multi-factor-auth)

## <a name="support"></a>Soporte

### <a name="where-can-i-get-support"></a>¿Dónde puedo obtener soporte técnico?

Para que los recursos de soporte técnico cumplan los requisitos de seguridad, si tienes Soporte técnico para socios Avanzado (ASfP), ponte en contacto con el Administrador de cuentas de servicios; para obtener Soporte técnico para socios Premier (PSfP), ponte en contacto con el Administrador de cuentas de servicios y el responsable técnico de cuenta.

### <a name="how-do-i-get-technical-information-and-support-to-help-me-adopt-secure-application-model-framework"></a>¿Cómo obtengo información técnica y soporte técnico que me ayude a adoptar el marco del modelo de aplicaciones seguras?

Las opciones de soporte técnico de productos para Azure Active Directory están disponibles a través de los beneficios de MPN. Los asociados con acceso a una suscripción activa a ASfP o PSfP pueden trabajar con su administrador de cuentas asociado (SAM/TAM) para comprender mejor las opciones disponibles para ellos.

### <a name="how-do-i-contact-support-when-ive-lost-access-to-partner-center"></a>¿Cómo puedo ponerme en contacto con el soporte técnico si he perdido el acceso al Centro de partners?

Ve a [Soporte técnico de partners de Microsoft](https://partner.microsoft.com/support) y elige **Show all support options** (Mostrar todas las opciones de soporte técnico). Verás las opciones disponibles para ponerte en contacto con el soporte técnico de partners de Microsoft. Incluyen un número de teléfono para llamar al soporte técnico y una opción para chatear con el soporte técnico. 

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>¿Dónde puedo encontrar más información sobre los problemas técnicos comunes?

Puedes encontrar información relativa a problemas técnicos comunes [aquí](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues).
