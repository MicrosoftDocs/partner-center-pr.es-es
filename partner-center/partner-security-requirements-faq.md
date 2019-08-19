---
title: Preguntas más frecuentes sobre los requisitos de seguridad de asociados | Centro de Partners
ms.topic: article
ms.date: 07/18/2019
description: Preguntas más frecuentes sobre los requisitos de seguridad del asociado
author: isaiahwilliams
ms.author: iswillia
keywords: Azure Active Directory, proveedor de soluciones en la nube, programa del proveedor de soluciones en la nube, CSP, proveedor del panel de control, CPV, autenticación multifactor, MFA, modelo de aplicación segura, modelo de aplicación segura, seguridad
ms.localizationpriority: medium
ms.openlocfilehash: 1f2ae0f07888fdabd16b2eb476af7fac975cd71e
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820591"
---
# <a name="frequently-asked-questions-about-the-partner-security-requirements"></a>Preguntas más frecuentes sobre los requisitos de seguridad del asociado

Este artículo contiene algunas preguntas frecuentes sobre los [requisitos de seguridad](partner-security-requirements.md)de los asociados.

## <a name="partner-security-requirements"></a>Requisitos de seguridad del asociado

### <a name="what-are-the-new-partner-security-requirements"></a>¿Cuáles son los nuevos requisitos de seguridad para asociados?

Para proteger a nuestros asociados y clientes, es necesario que los asociados lleven a cabo las siguientes acciones inmediatamente:  

1. **Habilite multi-factor Authentication (MFA) para todos los usuarios de los inquilinos de asociados**. Todos los usuarios de los inquilinos de socios comerciales deben usar la autenticación multifactor (MFA) al iniciar sesión en los servicios en la nube comerciales de Microsoft o a Transact in CSP a través del centro de Partners o a través de las API. Mediante la habilitación de las directivas de protección de línea de base, MFA está disponible de forma gratuita para todos los usuarios de inquilinos de asociados.

2. **Adopte el marco de trabajo del modelo de aplicación seguro**. Todos los asociados que se integran con una API de Microsoft como Azure Resource Manager, Microsoft Graph y la API del centro de Partners deben adoptar el marco de modelo de aplicación seguro para evitar cualquier interrupción en su integración cuando se habilitan las directivas de línea de base. 
 
La habilitación de la autenticación multifactor (MFA) y la adopción del marco de trabajo de modelo de aplicación segura ayudarán a proteger su infraestructura y a proteger los datos de sus clientes frente a posibles riesgos de seguridad, como identificar robos u otros incidentes de fraude.  

### <a name="which-partners-need-to-meet-the-requirements"></a>¿Qué asociados deben cumplir los requisitos?

Estos requisitos son para los siguientes grupos de socios comerciales:
- Todas las organizaciones asociadas que participan en el programa proveedor de soluciones en la nube (CSP) que están transactuando con los servicios en la nube de Microsoft Commercial
  - Asociados directos de factura
  - Proveedores indirectos
  - Revendedores indirectos
- Todos los proveedores del panel de control
- Todos los asociados del programa Advisor  

No es necesario que todos los asociados que transaccionen a través de una nube soberano (21Vianet, gobierno de EE. UU. y Alemania) cumplan los nuevos requisitos de seguridad a partir del 1 de agosto. Sin embargo, se recomienda encarecidamente que todos los asociados que usen una nube de uso soberano y adopten estos nuevos requisitos de seguridad inmediatamente. Microsoft proporcionará información adicional sobre la aplicación de estos requisitos de seguridad para nubes independientes en el futuro.

### <a name="what-are-the-key-timelines-and-milestones"></a>¿Cuáles son las escalas de tiempo e hitos clave?

Los términos asociados con estos requisitos de seguridad se agregarán inmediatamente a la guía del programa del proveedor de soluciones en la nube. Tendrá que implementar estos requisitos de seguridad para cumplir con su participación en el programa CSP a partir del 1 de agosto de 2019. 

### <a name="what-will-happen-if-i-do-not-take-any-actions"></a>¿Qué ocurrirá si no se realiza ninguna acción?

Los asociados que no cumplan estas prácticas y obligaciones de seguridad no podrán hacerlo en el programa proveedor de soluciones en la nube ni administrar los inquilinos del cliente aprovechando los derechos de administrador delegado, una vez que se apliquen estos requisitos de seguridad del asociado. Estamos en proceso de establecer una fecha de cumplimiento para los requisitos y notificaremos a los asociados de la fecha la información detallada.

### <a name="why-is-microsoft-enforcing-these-new-requirements"></a>¿Por qué impone Microsoft estos nuevos requisitos?
La seguridad y privacidad de los clientes y socios es la prioridad máxima de Microsoft. Seguimos viendo un número más sofisticado y creciente de ataques de seguridad relacionados principalmente con incidentes de riesgo de identidad. Como los controles preventivos juegan un papel clave en una estrategia de defensa general para frustrar los ataques de seguridad, comenzaremos a aplicar un conjunto de requisitos de seguridad obligatorios para ayudar a proteger a los asociados y sus clientes.

### <a name="does-this-apply-to-all-geographies"></a>¿Esto se aplica a todas las zonas geográficas?

Sí, esto se aplica a todas las zonas geográficas. Se recomienda encarecidamente que todos los asociados que transaccionen una nube soberano (21Vianet, gobierno de EE. UU. y Alemania) adopten estos nuevos requisitos de seguridad inmediatamente. Sin embargo, no es necesario que estos asociados cumplan los nuevos requisitos de seguridad a partir del 1 de agosto. Microsoft proporcionará información adicional sobre la aplicación de estos requisitos de seguridad para nubes independientes en el futuro.

## <a name="required-actions"></a>Acciones necesarias

### <a name="what-are-the-key-actions-i-need-to-take-to-meet-the-requirements"></a>¿Cuáles son las acciones clave que hay que realizar para cumplir los requisitos?  
Todos los asociados del programa CSP (factura directa, proveedor indirecto y revendedor indirecto), asesores y proveedores del panel de control deben cumplir los requisitos.

1. **Aplicar MFA para todos los usuarios**

    Todos los asociados del programa CSP, los asesores y los proveedores del panel de control deben aplicar MFA para todos los usuarios de su inquilino de asociados. Esto se puede lograr habilitando el uso de [MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators), la [línea de base de protección de usuarios finales](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users)y cualquier directiva de línea de base futura. La funcionalidad proporcionada por las directivas de línea de base continuará evolucionando para asegurarse de que los asociados y los clientes están protegidos frente a las amenazas de seguridad en constante cambio. Por lo tanto, es importante que revise la [documentación de las directivas de línea de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) para obtener más información.

    - Consulte [Directiva de línea base: Requerir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) para más información sobre cómo habilitar la Directiva requerir MFA para la línea de base de administración.
    - Consulte [Directiva de línea base: Protección](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) del usuario final para más información sobre cómo habilitar la Directiva de línea de base de protección del usuario final.
    - Comprenda el concepto de las [directivas de protección de línea de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).

    Consideraciones adicionales:

    - Los proveedores indirectos necesitan trabajar con revendedores indirectos para incorporarlos al centro de partners si aún no lo han hecho y animar a sus revendedores para que cumplan los requisitos.
    - Azure MFA se pone a disposición de todos los usuarios del inquilino del asociado sin coste alguno a través de las directivas de línea de base con el único método de comprobación del uso de la [aplicación Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview).
    - Los métodos de comprobación adicionales están disponibles a través de las SKU de [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) , si se requieren otros métodos como SMS o correo electrónico.
    - Los asociados también pueden aprovechar una solución de MFA de terceros por cada usuario al acceder a los servicios en la nube de Microsoft Commercial.

2. **Adopción del marco de modelo de aplicación segura**

    Todos los asociados que hayan desarrollado la integración personalizada con cualquier API (como Azure Resource Manager, Microsoft Graph, API del centro de Partners, etc.) o que hayan implementado la automatización personalizada mediante herramientas como PowerShell, deberán adoptar el [modelo de aplicación segura. marco de trabajo](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) para la integración con los servicios en la nube de Microsoft. Si no lo hace, puede producirse una interrupción debido a la implementación de MFA. Los siguientes recursos proporcionan información general e instrucciones sobre cómo adoptar el modelo.

    - [Información general sobre el modelo de aplicación segura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
    - [Centro de Partners: Guía del modelo de aplicación segura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
    - [Asociados en el programa CSP: código de ejemplo de .NET para habilitar el modelo de aplicación segura](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
    - [Asociados en el programa CSP: Código de ejemplo de Java para habilitar el modelo de aplicación segura](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
    - [Documento de autenticación del centro de Partners](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
    - [Documento de autenticación multifactor (MFA) de PowerShell del centro de Partners](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

    Si usa un panel de control, debe consultar al proveedor sobre la adopción del marco de trabajo de modelo de aplicación segura.

    Los proveedores del panel de control deben [incorporarse](https://docs.microsoft.com/partner-center/enroll-as-cpv) al centro de partners como proveedor del panel de control y empezar a implementar este requisito inmediatamente. Consulte el centro [de Partners: Marco](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)de modelo de aplicación segura. Los proveedores del panel de control deben aceptar y administrar el consentimiento de los asociados de CSP en lugar de las credenciales y purgar las credenciales de los asociados de CSP existentes.

## <a name="multi-factor-authentication"></a>Multi-Factor Authentication

### <a name="what-is-mfa"></a>¿Qué es MFA?

Multi-factor Authentication (MFA) es un mecanismo de seguridad a pesar de que los usuarios se autentican a través de más de un procedimiento de validación y seguridad necesario. Funciona mediante la exigencia de dos o más de los siguientes métodos de autenticación:

- Un elemento que el usuario conoce (por lo general, una contraseña)
- Un elemento que el usuario posee (un dispositivo de confianza que no puede duplicarse fácilmente como, por ejemplo, un teléfono)
- Un elemento que identifica al usuario personalmente (biométrica)

### <a name="what-are-baseline-protection-policies"></a>¿Qué son las directivas de protección de línea de base? 

[Directivas de protección de línea de base de Microsoft](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) (actualmente en versión preliminar) son un conjunto de directivas predefinidas que ayudan a proteger las organizaciones frente a muchos ataques comunes. Estos ataques comunes pueden incluir la pulverización de contraseñas, la reproducción y la suplantación de identidad. Las directivas de línea de base están disponibles en todas las ediciones de Azure Active Directory. Microsoft está poniendo estas directivas de protección de línea de base a disposición de todos los usuarios porque los ataques basados en identidad han estado en aumento en los últimos años. El objetivo de estas directivas es asegurarse de que todas las organizaciones tengan un nivel de línea de base de seguridad habilitado sin costo adicional.

> [!NOTE]
> Las directivas de línea de base de Microsoft y las funcionalidades relacionadas seguirán evolucionando para proteger mejor a los asociados y clientes de las amenazas de seguridad en constante cambio. Puede haber algunos cambios de nomenclatura y taxonomía con las directivas de línea de base pronto. Se recomienda encarecidamente que visite las páginas de directivas de línea de base directamente para consultar la información más reciente.

### <a name="what-baseline-policies-must-i-enable"></a>¿Qué directivas de línea base se deben habilitar?

Si tiene previsto emplear las directivas de protección de línea de base actuales para proporcionar MFA a cada usuario en el inquilino de asociado, debe habilitar la Directiva de línea de base [requerir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) y [protección del usuario final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) . Estas directivas de protección de línea de base satisfacen el requisito de MFA para cada usuario del inquilino del asociado sin coste alguno solo para los asociados que usan aplicaciones de Microsoft Authenticator a través de dispositivos móviles.

La [Directiva de línea de base requerir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) se usa para los usuarios administrativos en el directorio de socios comerciales y la Directiva de línea de base de [protección de usuarios finales](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) se usa para proteger a los usuarios no administrativos en el inquilino del asociado. La habilitación de estas directivas requerirá que los usuarios se registren para MFA. Una vez que el usuario se ha registrado correctamente, se le pedirá MFA durante los intentos de inicio de sesión en función de los criterios de la Directiva. La funcionalidad proporcionada por las directivas de línea de base continuará evolucionando para asegurarse de que los asociados y los clientes están protegidos frente a las amenazas de seguridad en constante cambio. Por lo tanto, es importante que revise la [documentación de las directivas de línea de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection) para obtener más información.

### <a name="how-do-i-enable-the-require-mfa-for-admins-policy"></a>Cómo habilitar la Directiva ¿requerir MFA para administradores? 

La Directiva de línea de base requerir MFA para administradores se puede habilitar a través del portal de administración de Azure. Consulte [Directiva de línea base: Requerir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) para más información sobre cómo habilitar esta directiva de línea de base.

### <a name="how-do-i-enable-the-end-user-protection-policy"></a>Cómo habilitar la Directiva de protección del usuario final

La Directiva de línea de base de protección del usuario final se puede habilitar a través del portal de administración de Azure. Consulte [Directiva de línea base: Protección](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) del usuario final para más información sobre cómo habilitar esta directiva de línea de base.

### <a name="will-the-baseline-policies-be-automatically-enabled"></a>¿Se habilitarán automáticamente las directivas de línea de base? 

No, para habilitar estas directivas, un usuario que sea miembro de los roles de administrador global, administrador de seguridad o administrador de acceso condicional tendrá que configurar las directivas para usar la Directiva inmediatamente.

### <a name="what-is-the-cost-of-enabling-mfa"></a>¿Cuál es el costo de habilitar MFA?

Microsoft proporciona MFA de forma gratuita a través de la implementación de las directivas [requerir MFA para administración](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) y [protección de usuarios finales](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) . La única opción de comprobación disponible a través de esta versión de MFA es la [aplicación Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Si se requiere una llamada de teléfono o un mensaje SMS, se deberá adquirir una licencia de [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) . Como alternativa, puede utilizar una solución de terceros para proporcionar MFA a cada usuario en el inquilino del asociado: en este caso, es su responsabilidad asegurarse de que la solución MFA se está aplicando y que es compatible.

### <a name="if-i-already-have-an-mfa-solution-what-actions-do-i-need-to-take"></a>Si ya tengo una solución MFA, ¿qué acciones necesito realizar?

A través de estos requisitos de seguridad, es necesario que los usuarios de un inquilino de asociado se autentiquen mediante MFA al acceder a los servicios en la nube de Microsoft Commercial. Se puede usar una solución de terceros para cumplir estos requisitos. Microsoft ya no proporciona pruebas de validación a proveedores de identidades independientes por compatibilidad con Azure Active Directory. Si desea probar el producto para la interoperabilidad, consulte estas [instrucciones](https://www.microsoft.com/download/details.aspx?id=56843).

### <a name="what-verification-method-can-i-use-to-authenticate-mfa"></a>¿Qué método de comprobación puedo usar para autenticar MFA?

Microsoft proporciona MFA de forma gratuita a través de la implementación de las directivas [requerir MFA para administración](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) y [protección de usuarios finales](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) . La única opción de comprobación disponible a través de esta versión de MFA es la [aplicación Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview). Si se requiere una llamada de teléfono o un mensaje SMS, se deberá adquirir una licencia de [Azure Active Directory Premium](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-get-started-premium) . Como alternativa, puede utilizar una solución de terceros para proporcionar MFA a cada usuario en el inquilino del asociado: en este caso, es su responsabilidad asegurarse de que la solución MFA se está aplicando y que es compatible.

### <a name="i-use-multiple-partner-tenants-to-transact-do-i-need-to-implement-mfa-on-them-all"></a>Utilizo varios inquilinos de asociados para Transact. ¿Es necesario implementar MFA en todos?

Sí, necesitará aplicar MFA para cada inquilino de Azure Active Directory asociado con el programa CSP o el programa Advisor. Si planea comprar una licencia de Azure Active Directory Premium, se debe adquirir una licencia para el usuario en cada inquilino de Azure Active Directory.

### <a name="does-each-user-in-my-partner-tenant-need-to-have-mfa-enforced"></a>¿Es necesario que se aplique MFA a cada usuario del inquilino de mi asociado? 

Las directivas de protección de la línea [de base requerir MFA para administración](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) y [protección de usuarios finales](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) aplicarán MFA para cada usuario del inquilino de asociado. Si está aprovechando estas directivas para proporcionar MFA y usa la aplicación [Microsoft Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-overview) , no es necesario adquirir licencias adicionales. De lo contrario, tendrá que comprar una solución adecuada para proporcionar MFA a cada usuario del inquilino de asociado.

### <a name="i-am-a-direct-bill-partner-with-microsoft-what-do-i-need-to-do"></a>Soy un asociado de factura directo con Microsoft. ¿Qué tengo que hacer?

Los asociados directos de proveedores de soluciones en la nube deben aplicar MFA para cada usuario en su inquilino de asociado.

### <a name="i-am-an-indirect-reseller-and-only-transact-though-a-distributor-do-i-still-have-to-do-this"></a>Soy un revendedor indirecto y solo Transact a través de un distribuidor. ¿Todavía tengo que hacer esto?

Todos los revendedores indirectos son necesarios para aplicar MFA para cada usuario en su inquilino de socio. Se trata de una acción que el revendedor indirecto debe realizar.

### <a name="i-do-not-use-the-partner-center-api-do-i-still-need-to-implement-mfa"></a>No utilizo la API del centro de Partners. ¿Todavía tengo que implementar MFA?

Sí, este requisito de seguridad es para todos los usuarios, incluidos los usuarios de administradores asociados y los usuarios finales de un inquilino de socio.

### <a name="which-third-party-vendors-provide-mfa-solutions-compatible-with-azure-active-directory"></a>¿Qué proveedores de terceros proporcionan soluciones MFA compatibles con Azure Active Directory?

Hay muchas revisiones independientes de soluciones de MFA en línea, como [Gartner](https://www.gartner.com/en/webinars/3881781). Al revisar los proveedores y las soluciones de MFA, los asociados deben asegurarse de que la solución que elijan sea compatible con Azure Active Directory.

Microsoft ya no proporciona pruebas de validación a proveedores de identidades independientes por compatibilidad con Azure Active Directory. Si desea probar el producto para la interoperabilidad, consulte estas [instrucciones](https://www.microsoft.com/download/details.aspx?id=56843).

Para obtener más información, consulte la [lista de compatibilidad de Federación de Azure ad](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-compatibility).

### <a name="how-can-i-test-mfa-in-our-integration-sandbox"></a>¿Cómo puedo probar MFA en nuestro espacio aislado de integración?

Las directivas de línea de base [requerir MFA para administración](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) y [protección de usuario final](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) deben estar habilitadas para el inquilino de espacio aislado de integración. A través de esta Directiva, cada usuario del inquilino tendrá que autenticarse mediante MFA.

### <a name="will-enabling-mfa-effect-how-i-interact-with-my-customers-tenant"></a>¿Permitirá el efecto de MFA cómo interactuamos con el inquilino de mi cliente? 

No. El cumplimiento de estos requisitos de seguridad no afectará a la forma de administrar los clientes. La capacidad de realizar operaciones administrativas delegadas no se interrumpirá.

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

### <a name="can-conditional-access-be-used-to-meet-the-mfa-requirement"></a>¿Se puede usar el acceso condicional para cumplir el requisito de MFA?

Sí, puede usar el acceso condicional para aplicar MFA a cada usuario, incluidas las cuentas de servicio, en el inquilino del asociado. Sin embargo, dada la naturaleza con privilegios elevados de ser un asociado, es necesario asegurarse de que cada usuario tenga un desafío de MFA para cada autenticación. Esto significa que no podrá aprovechar la característica de acceso condicional que evita el requisito de MFA.

### <a name="what-verification-options-are-provided-through-the-implementation-of-the-baseline-protection-policies"></a>¿Qué opciones de comprobación se proporcionan a través de la implementación de las directivas de protección de línea de base? 

Con respecto a la versión de MFA que está disponible a través de la implementación de las directivas de protección de línea de base, la única opción de comprobación disponible es una aplicación autenticadora. El uso de un mensaje de llamada de teléfono y mensaje de texto se considera menos seguro. Por lo tanto, estas opciones no están disponibles a través de esta versión de MFA.

### <a name="will-the-service-account-used-by-azure-ad-connect-be-impacted-by-the-partner-security-requirements"></a>¿La cuenta de servicio usada por Azure AD Connect se verá afectada por los requisitos de seguridad del asociado?

No, la cuenta de servicio usada por Azure AD Connect no se verá afectada por los requisitos de seguridad del asociado. Si experimenta un problema con Azure AD Connect como consecuencia de la aplicación de MFA, abra una solicitud de soporte técnico con el soporte técnico de Microsoft.

## <a name="secure-application-model"></a>Modelo de aplicación segura

### <a name="who-should-adopt-the-secure-application-model-to-meet-the-requirements"></a>¿Quién debe adoptar el modelo de aplicación segura para cumplir los requisitos?

Microsoft está introduciendo un marco de trabajo seguro y escalable para autenticar asociados de proveedor de soluciones en la nube (CSP) y proveedores del panel de control (CPV) que aprovecha la autenticación multifactor. Vea la [Guía modelo de aplicación segura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) para obtener más información. Todos los asociados que hayan desarrollado la integración personalizada con cualquier API (como Azure Resource Manager, Microsoft Graph, API del centro de Partners, etc.) o que hayan implementado la automatización personalizada mediante herramientas como PowerShell, deberán adoptar el [modelo de aplicación segura. marco de trabajo](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) para la integración con los servicios en la nube de Microsoft.

### <a name="what-is-the-secure-application-model"></a>¿Qué es el modelo de aplicación segura?

Microsoft está introduciendo un marco de trabajo seguro y escalable para autenticar asociados de proveedor de soluciones en la nube (CSP) y proveedores del panel de control (CPV) que aprovecha la autenticación multifactor. Vea la [Guía modelo de aplicación segura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) para obtener más información.  

### <a name="how-do-i-implement-the-secure-application-model"></a>Cómo implementar el modelo de aplicación segura?

Todos los asociados que hayan desarrollado la integración personalizada con cualquier API (como Azure Resource Manager, Microsoft Graph, API del centro de Partners, etc.) o que hayan implementado la automatización personalizada mediante herramientas como PowerShell, deberán adoptar el [modelo de aplicación segura. marco de trabajo](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model) para la integración con los servicios en la nube de Microsoft. Si no lo hace, puede producirse una interrupción debido a la implementación de MFA. Los siguientes recursos proporcionan información general e instrucciones sobre cómo adoptar el modelo.

- [Información general sobre el modelo de aplicación segura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Centro de Partners: Guía del modelo de aplicación segura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Asociados en el programa CSP: código de ejemplo de .NET para habilitar el modelo de aplicación segura](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [Asociados en el programa CSP: Código de ejemplo de Java para habilitar el modelo de aplicación segura](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [Documento de autenticación del centro de Partners](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento de autenticación multifactor (MFA) de PowerShell del centro de Partners](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

Si usa un panel de control, debe consultar al proveedor sobre la adopción del marco de trabajo de modelo de aplicación segura.

Los proveedores del panel de control deben [incorporarse](https://docs.microsoft.com/partner-center/enroll-as-cpv) al centro de partners como proveedor del panel de control y empezar a implementar este requisito inmediatamente. Consulte el centro [de Partners: Marco](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)de modelo de aplicación segura. Los proveedores del panel de control deben aceptar y administrar el consentimiento de los asociados de CSP en lugar de las credenciales y purgar las credenciales de los asociados de CSP existentes.

### <a name="who-is-a-control-panel-vendor-cpv"></a>¿Quién es un proveedor del panel de control (CPV)? 
Un proveedor del panel de control es un fabricante de software independiente que desarrolla aplicaciones para que las usen los asociados de CSP para la integración con las API del centro de Partners. Un proveedor del panel de control no es un asociado de CSP con acceso directo al panel o las API del centro de Partners. Una descripción detallada está disponible en el [centro de Partners: Guía](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)del modelo de aplicaciones seguras.

### <a name="does-the-secure-application-model-need-to-be-implemented-for-the-partner-center-apisdk-only"></a>¿Es necesario implementar el modelo de aplicación segura solo para el SDK/API del centro de Partners? 

Una vez que se habilitan las directivas *requerir MFA para administradores* y la línea de base de *protección de usuario final* , cada usuario tendrá que autenticarse con multi-factor Authentication. Esto significa que necesitará implementar el modelo de aplicación seguro para cada API, CLI y módulo de PowerShell (por ejemplo, Azure, Azure AD, MS online, centro de Partners, etc.) diseñado para ejecutarse de forma no interactiva y se basa en el uso de las credenciales de usuario para la autenticación.

### <a name="i-am-using-automation-tools-such-as-powershell-how-do-i-implement-the-secure-application-model"></a>Utilizo herramientas de automatización como PowerShell. Cómo implementar el modelo de aplicación segura?  

Si la automatización está diseñada para ejecutarse de forma no interactiva y se basa en las credenciales de usuario para la autenticación, deberá implementar el modelo de aplicación segura. Vea [modelo de aplicación segura | Centro de Partners PowerShell](https://docs.microsoft.com/powershell/partnercenter/secure-app-model?view=partnercenterps-1.5) para obtener instrucciones sobre cómo implementar este marco de trabajo.  Tenga en cuenta que no todas las herramientas de automatización proporcionan la capacidad de autenticación mediante tokens de acceso. Si necesita ayuda para comprender qué cambios deben realizarse, publique un mensaje en el grupo [Guía de seguridad del centro de Partners](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance) .

### <a name="what-user-credentials-should-the-application-administrator-provide-when-performing-the-consent-process"></a>¿Qué credenciales de usuario debe proporcionar el administrador de la aplicación al realizar el proceso de consentimiento? 

Se recomienda que use una cuenta de servicio a la que se le hayan asignado los permisos con privilegios mínimos. Con respecto a la API del centro de Partners, esto significa que debe usar una cuenta que tenga asignado el rol agente de ventas o agentes de administración.

### <a name="why-should-the-application-administrator-not-provide-global-admin-user-credentials-when-performing-the-consent-process"></a>¿Por qué el administrador de aplicaciones no debe proporcionar credenciales de usuario de administrador global al realizar el proceso de consentimiento?

Se recomienda usar las identificaciones con menos privilegios para reducir el riesgo. No se recomienda usar una cuenta que tenga privilegios de administrador global, ya que esto proporcionaría más permisos de los necesarios.

### <a name="i-am-a-csp-partner-how-do-i-know-if-my-control-panel-vendor-cpv-is-working-on-implementing-the-solution-or-not"></a>Soy asociado de CSP. Cómo saber si el proveedor del panel de control (CPV) está trabajando en la implementación de la solución o no? 

En el caso de los asociados que usan una solución de proveedor de panel de control (CPV) para Transact en el programa proveedor de soluciones en la nube (CSP), es su responsabilidad consultar con el CPV. 

### <a name="i-am-a-cpv-how-do-i-enroll"></a>Soy CPV. ¿Cómo inscribirse? 

Para inscribirse como proveedor del panel de control (CPV), siga las instrucciones que se proporcionan [aquí](https://docs.microsoft.com/partner-center/enroll-as-cpv).

Para recibir el vínculo de inscripción, CPVs debe ponerse en [CPVHelp@microsoft.com](mailto:CPVHelp@microsoft.com) contacto y proporcionar un patrocinador de empleado de Microsoft que tenga una relación de negocio con el CPV o que conozca su negocio. Por ejemplo, un administrador de desarrollo de asociados (PDM).

Una vez que se inscriba en el centro de Partners y registre las aplicaciones, tendrá acceso a las API del centro de Partners. Si es un nuevo CPV, recibirá la información del espacio aislado a través de una notificación del centro de Partners. Una vez que haya completado la inscripción como Microsoft CPV y aceptado el contrato CPV, puede:

1. Administrar la aplicación multiinquilino (agregar aplicaciones a Azure Portal, registrar y anular el registro de aplicaciones en el centro de Partners). Nota: CPVs debe registrar sus aplicaciones en el centro de partners para que se les autorice para las API del centro de Partners. Agregar aplicaciones al Azure Portal por separado no autoriza aplicaciones CPV para las API del centro de Partners.
2. Ver y administrar el perfil de CPV.
3. Vea y administre los usuarios que necesitan acceso a las funcionalidades de CPV. El único rol que puede tener un CPV es el administrador global.

### <a name="i-am-using-the-partner-center-sdk-will-sdk-automatically-adopt-the-secure-application-model"></a>Utilizo el SDK del centro de Partners. ¿Adoptará el SDK automáticamente el modelo de aplicación seguro? 

No, tendrá que seguir las instrucciones proporcionadas en la [Guía modelo de aplicación segura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf).

### <a name="can-i-generate-a-refresh-token-for-the-secure-application-model-with-accounts-that-do-not-have-mfa-enabled"></a>¿Se puede generar un token de actualización para el modelo de aplicación segura con cuentas que no tienen MFA habilitado?

Sí, se puede generar un token de actualización con una cuenta que no tenga MFA aplicada. Sin embargo, esto no debería realizarse porque los tokens generados con una cuenta que no tiene MFA habilitado no podrán tener acceso a los recursos debido a la necesidad de MFA.

### <a name="how-should-my-application-obtain-an-access-token-if-we-enable-mfa"></a>¿Cómo debe obtener mi aplicación un token de acceso si se habilita MFA?

Deberá seguir la [Guía de modelo de aplicación segura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) , que proporciona detalles sobre cómo hacerlo mientras cumple con los nuevos requisitos de seguridad. [Aquí](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model) puede encontrar código de ejemplo de .NET y [aquí](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model) el código de ejemplo de Java.

### <a name="as-a-cpv-do-i-create-an-azure-ad-application-in-our-cpv-tenant-or-the-tenant-of-the-csp-partner"></a>Como CPV, ¿creo una aplicación Azure AD en nuestro inquilino de CPV o en el inquilino del asociado de CSP?

El CPV deberá crear la aplicación Azure Active Directory en el inquilino asociado a su inscripción como CPV.

### <a name="i-am-a-csp-that-is-using-app-only-authentication-do-i-need-to-make-any-changes"></a>Soy un CSP que usa la autenticación de solo aplicación. ¿Es necesario realizar algún cambio?

La autenticación de solo aplicación no se ve afectada, ya que las credenciales de usuario no se usan para solicitar un token de acceso. Si se comparten las credenciales del usuario, los proveedores del panel de control (CPVs) deben adoptar el [marco de trabajo de modelo de aplicación seguro](http://assetsprod.microsoft.com/secure-application-model-guide.pdf) y purgar las credenciales de asociado existentes que tengan.

### <a name="as-a-cpv-can-i-leverage-the-app-only-authentication-style-to-get-access-tokens"></a>Como CPV, ¿puedo aprovechar el estilo de autenticación de solo aplicación para obtener tokens de acceso?

No, los asociados de proveedor del panel de control no pueden emplear el estilo de autenticación de solo aplicación para solicitar tokens de acceso en nombre del asociado. Deben implementar el modelo de aplicación seguro, que emplea el estilo de autenticación de usuario y aplicación.

## <a name="key-resources"></a>Recursos clave

### <a name="how-to-get-started"></a>Inicio

- [Requisitos de seguridad del asociado: guía paso a paso](https://docs.microsoft.com/partner-center/partner-security-requirements).
- Dirija sus preguntas y comentarios a este [grupo guía de seguridad del centro de Partners](https://aka.ms/MPCSecurityGuidance).
- Asista a próximos horarios de oficina y seminarios web. Consulte aquí la [programación y los recursos](https://www.microsoftpartnercommunity.com/t5/Partner-Center-Security-Guidance/ct-p/partner-center-security-guidance)detallados.

### <a name="resources-for-enabling-mfa"></a>Recursos para habilitar MFA

- Comprenda el concepto de las [directivas de protección de línea de base](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-baseline-protection).
- Consulte [Directiva de línea base: Requerir MFA para administradores](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-administrators) para más información sobre cómo habilitar la Directiva requerir MFA para la línea de base de administración.
- Consulte [Directiva de línea base: Protección](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-baseline-protect-end-users) del usuario final para más información sobre cómo habilitar la Directiva de línea de base de protección del usuario final.

### <a name="resources-for-adopting-secure-application-model"></a>Recursos para adoptar el modelo de aplicación segura

- [Información general sobre el modelo de aplicación segura](https://docs.microsoft.com/partner-center/develop/enable-secure-app-model)
- [Centro de Partners: Guía del modelo de aplicación segura](http://assetsprod.microsoft.com/secure-application-model-guide.pdf)
- [Asociados en el programa CSP: código de ejemplo de .NET para habilitar el modelo de aplicación segura](http://github.com/microsoft/Partner-Center-DotNet-Samples/tree/master/secure-app-model)
- [Asociados en el programa CSP: Código de ejemplo de Java para habilitar el modelo de aplicación segura](http://github.com/microsoft/Partner-Center-Java-Samples/tree/master/secure-app-model)
- [Documento de autenticación del centro de Partners](https://docs.microsoft.com/partner-center/develop/partner-center-authentication)
- [Documento de autenticación multifactor (MFA) de PowerShell del centro de Partners](https://docs.microsoft.com/partner-center/develop/multi-factor-auth)

## <a name="support"></a>Soporte técnico

### <a name="where-can-i-ask-get-support"></a>¿Dónde puedo pedir ayuda?

Además, para admitir el uso de recursos para cumplir los requisitos de seguridad, si tiene soporte técnico avanzado para asociados (ASfP), póngase en contacto con su administrador de cuentas de servicio; para obtener soporte técnico Premier del acuerdo de asociados (PSfP), póngase en contacto con el administrador de cuentas de servicio y el administrador de cuentas técnico.

### <a name="how-can-i-get-help-with-enabling-the-baseline-policies"></a>¿Cómo puedo obtener ayuda para habilitar las directivas de línea de base?

- Los asociados pueden aprovechar las horas de consulta de las ventajas de MPN para obtener instrucciones más detalladas sobre cómo implementar los requisitos de seguridad.
- Las opciones de soporte técnico de productos para Azure Active Directory están disponibles a través de las ventajas de MPN. Los asociados con acceso a un contrato de ASfP o PSfP activo pueden trabajar con su administrador de cuentas asociado (SAM/TAM) para comprender mejor las opciones disponibles.
- Se puede tener acceso a la implementación de directivas de línea de base con el centro de partners a través de la [solicitud de servicio del centro de Partners](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp). Seleccione *MFA & modelo de aplicación seguro* como tema.

### <a name="how-do-i-get-technical-information-to-adopt-secure-application-model-framework"></a>Cómo obtener información técnica para adoptar el marco de trabajo de modelo de aplicación seguro? 

Las opciones de soporte técnico de productos para Azure Active Directory están disponibles a través de las ventajas de MPN. Los asociados con acceso a una suscripción activa a ASfP o PSfP pueden trabajar con su administrador de cuentas asociado (SAM/TAM) para comprender mejor las opciones disponibles.

### <a name="where-can-i-find-more-information-about-technical-common-issues"></a>¿Dónde puedo encontrar más información sobre problemas comunes técnicos? 

Puede encontrar información sobre los problemas técnicos comunes [aquí](https://docs.microsoft.com/partner-center/partner-security-requirements#common-issues).
