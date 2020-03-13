---
title: Preparación para el cambio desde Partner Membership Center al Centro de partners | Centro de partners
ms.topic: article
ms.date: 06/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Consulta información útil y revisa las preguntas más frecuentes antes de cambiar tu negocio de PMC al Centro de partners.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: high
ms.openlocfilehash: 06167a667152ddaf65702547783df93726f6cadc
ms.sourcegitcommit: eb4fc25524cc68c10906ccd3392914e805213ee5
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2020
ms.locfileid: "78340112"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Preparación para el cambio desde Partner Membership Center (PMC) al Centro de partners

**Roles adecuados**
-    Administrador global
-    Administrador de usuarios
-    Agente de ventas
-    Agente de administrador

Estamos trasladando la administración de la pertenencia desde Partner Membership Center (PMC) al Centro de partners: el único destino para administrar tu relación de negocio con Microsoft. Queremos que el cambio al Centro de partners sea lo más eficaz y sencillo posible. Hemos identificado algunas áreas en las que el Centro de partners difiere de PMC y creemos que te interesará comprender y prepararte antes de realizar el cambio.

## <a name="account-and-identity-setup"></a>Configuración de cuentas e identidades

**¿Qué es una cuenta profesional de Azure Active Directory (Azure AD)?**

Una cuenta profesional de Azure es una representación virtual dedicada y aislada de tu empresa en la nube pública de Azure, que se crea automáticamente cuando te suscribes a un servicio en la nube de Microsoft como Azure, Microsoft Intune u Office 365.

La cuenta profesional hospeda los usuarios de Azure AD y la información sobre ellos: su correo electrónico, contraseñas, datos de perfil, permisos, etc. La cuenta profesional también contiene grupos, aplicaciones y otra información relativa a una compañía y su seguridad. 

En el Centro de partners, usarás el correo electrónico del trabajo para iniciar sesión en tu cuenta, no tu correo electrónico personal.
- Tu cuenta profesional: john@contoso.com
- Tu cuenta personal: John@outlook.com

El correo electrónico del trabajo forma parte del inquilino de Azure Active Directory. Para tener una cuenta en el Centro de partners, debes tener un inquilino de AAD. Para más información sobre Azure Active Directory, consulta [Creación del directorio en Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

**Al cambiar al Centro de partners desde PMC, ¿con qué cuenta tienes que iniciar sesión en el Centro de partners si tienes un inquilino de AAD con Microsoft (por ejemplo, para Office 365) y también tienes un inquilino para tu negocio de CSP?**

Puedes iniciar sesión en el Centro de partners con la cuenta de CSP o la cuenta de correo electrónico del trabajo de MPN. Si eliges iniciar sesión con el correo electrónico del trabajo de CSP, en el área de navegación izquierda del panel se mostrará la información de los programas MPN y CSP. Si inicias sesión con el correo electrónico del trabajo del inquilino de Azure AD de MPN, solo verás la información del programa MPN. Los roles de usuario difieren entre MPN y CSP, por lo que, si usas la misma cuenta para los negocios de MPN y CSP, asegúrate de asignar roles de usuario en consecuencia. Para más información, consulta [Asignar roles y permisos de usuarios](permissions-overview.md).

**Si no quieres usar el inquilino de Azure AD existente de Office 365 para el Centro de partners, puedes crear un nuevo inquilino antes de la migración desde PMC.**

Puede haber muchos motivos por los que no quieras usar un inquilino de Azure AD existente para configurar la cuenta del Centro de partners. Antes de empezar a migrar al Centro de partners, ve a [Azure Portal](https://ms.portal.azure.com/#home) para crear un nuevo inquilino de Azure AD. Sigue las instrucciones de [Creación de un nuevo inquilino en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant). Una vez creado, usa este nuevo inquilino de AAD para configurar la cuenta del Centro de partners al cambiar desde PMC al Centro de partners. Debes ser un administrador global para crear el inquilino. Usa este nuevo directorio para migrar al Centro de partners.


**¿Cuál es la diferencia entre el rol de administrador global de AAD y el rol de administrador global de MPN en PMC?**

Son dos roles diferentes con distintos permisos. El administrador global del inquilino de AAD del Centro de partners administra el inquilino: agrega o quita usuarios, proporciona y administra contraseñas, roles y permisos, y tiene acceso a todos los programas de la compañía en el Centro de partners. 

El rol de administrador global de MPN en PMC puede hacer lo siguiente:

- Ver y editar todos los datos asociados a la compañía y todas las ubicaciones de la compañía.

-  Agregar administradores en el nivel global o local.  Además, los administradores globales pueden asignar a cualquier persona de cualquier ubicación el acceso de administrador global, que concede acceso global independientemente de la ubicación a la que esté asociada.
-  Realizar cualquier función de interfaz de usuario orientada a partners, incluidas las siguientes: 

-  Agregar o quitar usuarios

 - Asignar o quitar roles 

 - Agregar, quitar o actualizar ubicaciones 

 - Adquirir competencia o mapas 

-  Ver las ventajas

Cuando el administrador global de MPN se cambia al Centro de partners, el rol se denomina administrador de partners de MPN, que tiene permisos y tareas diferentes que el administrador global del Centro de partners. Para más información sobre los roles y los permisos del Centro de partners, consulta [Asignar roles y permisos de usuarios](permissions-overview.md).

**Roles de usuario, incluidos los roles de usuario invitado en el Centro de partners**

El Centro de partners tiene distintos tipos de roles en función de los tipos de trabajo que es necesario realizar. Hay roles, como el administrador global, que son roles de Azure AD. Algunos de los roles son específicos de los programas, como de los programas de proveedor de servicios en la nube o de incentivos, y hay roles que son específicos de MPN. Para averiguar lo que son todos los roles del Centro de partners, consulta [Asignar roles y permisos de usuarios](permissions-overview.md).



**¿Qué ocurre con los roles de mis usuarios cuando pasan de PMC al Centro de partners?**

Excepto en el caso del administrador global de MPN o del contacto principal del programa que realiza la migración, todos los usuarios de PMC perderán sus roles de administrador. La persona que completa la migración tendrá que asignar roles en el Centro de partners. Los roles del Centro de partners difieren de los roles en PMC. Consulta [Asignar roles y permisos de usuarios] (permissions-overview.md y [Cambio de PMC al Centro de partners](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles) para más información sobre los roles de usuario en el Centro de partners.


**¿Cuál es la diferencia entre mi perfil de la compañía y mi perfil de negocio?**

El perfil de la compañía es la información sobre tu compañía que incluye la dirección, las ubicaciones, el contacto principal, el banco y los detalles fiscales.

Tu perfil de negocio es la forma en que te presentas a los clientes y es una página de marketing que muestra tu logotipo, los detalles sobre tu enfoque empresarial, tu experiencia, etc.

**¿Qué significa la consolidación de cuentas para mi cuenta?**

Si usas el mismo inquilino de Azure AD para migrar varias cuentas de MPN al Centro de partners, el sistema lo reconocerá automáticamente y te pedirá que consolides tus cuentas. Esto es así incluso si tienes varios dominios asociados al mismo inquilino de Azure AD. 

También puedes optar por migrar al Centro de partners mediante inquilinos de AAD independientes, pero ten en cuenta que se produce una evaluación aislada de tus competencias, además de costes de compra adicionales. 

**Si tengo varios inquilinos de AAD y una sola cuenta de MPN, ¿es posible vincularlos en el Centro de partners?**

Sí, en el Centro de partners, puedes vincular varios inquilinos de Azure AD a una cuenta del Centro de partners.
Obtén más información aquí. 

**¿Existen restricciones para agregar varios inquilinos de Azure AD a una sola cuenta del Centro de partners?**

Si el inquilino de Azure AD ya está asociado a una cuenta del Centro de partners existente, no se puede asociar a nuevas cuentas del Centro de partners mediante la característica multiinquilino. Otra forma de verlo es pensar que un inquilino de Azure AD solo se puede asociar a una cuenta del Centro de partners, pero una cuenta del Centro de partners puede tener varios inquilinos asociados.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migración de la pertenencia a Microsoft Partner Network (MPN) 

**¿Quién puede realizar el cambio de PMC al Centro de partners?**

El administrador global de MPN de la compañía o el contacto principal del programa (los dos roles suelen coincidir en la misma persona) pueden iniciar y realizar el cambio.

**¿Se convertirá la persona que completa la migración en el contacto principal del perfil legal de la empresa en el Centro de partners?**

No necesariamente, pero el contacto principal debe tener autorización para firmar contratos.

**¿Puede Microsoft migrar mi pertenencia a MPN?**

No. Microsoft no puede ayudarte a migrar tu cuenta de pertenencia al Centro de partners. Tendrás que mover tu cuenta iniciando sesión en PMC con tu cuenta profesional (credenciales de inicio de sesión) para comenzar el proceso de migración. Una vez completados los pasos para mover tu cuenta, puedes empezar a administrar tu pertenencia y asignar roles y permisos de usuario a tu equipo para que puedan acceder a las ventajas y ayudar a administrar la pertenencia. Microsoft migrará automáticamente las competencias actuales, las ventajas, la información de ubicación, la información bancaria o fiscal para incentivos y las asociaciones de MCP, incluido el acceso a Partner University.

Microsoft migrará automáticamente las competencias actuales, las ventajas, la información de ubicación, la información bancaria o fiscal para incentivos y las asociaciones de MCP, incluido el acceso a Partner University.

**¿Cómo cambiará la directiva de renovación?**

 En el Centro de partners, la ventana de renovación abarca los 30 días posteriores desde la fecha de aniversario.

**¿Permanecerán las competencias sin cambios después de cambiar al Centro de partners?**

Sí, las competencias no se verán afectadas por el cambio al Centro de partners. Si observas discrepancias, ponte en contacto con el [soporte técnico](https://partner.microsoft.com/support).


 **¿Cambiarán mis ventajas (incluidas las ventajas en la nube, el soporte técnico, las ventajas de software y Visual Studio) después del cambio?**

 Las ventajas elegibles no cambiarán. Si observas discrepancias, ponte en contacto con el [soporte técnico](https://partner.microsoft.com/support).

 **¿Se respetan nuestras cuentas Microsoft con asignaciones de ventajas de Visual Studio?**


 Sí. Los beneficios de Visual Studio asignados a MSA se respetarán y conservarán. También se conservarán después de la renovación en el Centro de partners. Sin embargo, si quitas una asignación de MSA una vez migrada al Centro de partners, no se puede volver a agregar al Centro de partners.

En el Centro de partners, un partner puede agregar cuentas profesionales y cuentas de usuario invitado, que son MSA del mismo inquilino donde el partner es administrador de MPN en el inquilino de Azure AD. Si el partner es un administrador global en varios inquilinos de Azure AD y todos estos inquilinos están asociados a la misma cuenta del Centro de partners, se permite que el partner agregue usuarios de todos estos inquilinos a los beneficios de Visual Studio y asignaciones basadas en el uso de Azure.

Aunque a los usuarios invitados se les pueden asignar suscripciones basadas en el uso de Visual Studio mediante el administrador de MPN o el administrador global, los usuarios invitados no pueden iniciar sesión en el Centro de partners mediante su MSA. Sin embargo, los usuarios invitados pueden iniciar sesión en Azure y Visual Studio para validar y usar sus beneficios asignados.


 **¿Cómo debemos administrar nuestras asociaciones de MCP y nuestro acceso a Partner University?**

 No hay cambios en las asociaciones de MCP que se mueven desde PMC. Sin embargo, los nuevos empleados después de cambiar al Centro de partners deberán asociarse al Centro de partners. Se conservarán todos los permisos de Partner University de los usuarios existentes, pero los nuevos empleados deben ir al [centro de aprendizaje](https://partner.microsoft.com/training) para obtener información sobre cómo acceder a Partner University.

 **¿Cómo visualizo la información de MCP después de cambiar al Centro de partners?**

Selecciona **Competencias** en el área de navegación izquierda en el panel. En la página **Competencias**, puedes descargar el informe de aptitudes. En el informe de aptitudes se mostrarán los usuarios que han adquirido las aptitudes pertinentes para las competencias y los programas del Centro de partners. Si los usuarios han adquirido aptitudes, pero no son pertinentes para las competencias en las que vas a trabajar, no se mostrarán en el informe.


 **¿Se usan referencias de cliente en el Centro de partners?**

 No, no es necesario que las referencias de los clientes cumplan los requisitos de competencia del Centro de partners.

 **¿Se trasladarán las asociaciones de Partner de registro al Centro de partners?**

 Sí, no hay ningún cambio en Partner de registro. Obtén más información sobre la [vinculación del id. de partner a los clientes](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).

**¿Hay algún impacto en los incentivos debido al cambio al Centro de partners?**

No, no hay ningún impacto en los incentivos si has movido tu cuenta sin consolidar las ubicaciones. Si tu negocio tiene varias cuentas en PMC y, al cambiar al Centro de partners, decides consolidarlas en una cuenta global, no habrá ninguna pérdida de incentivos, pero puede haber un retraso en su pago. Si no mueves todas las cuentas de PMC que han participado en los programas de incentivos, puedes dejar de ganar los incentivos que están vinculados a esas cuentas.


**¿Cuáles son los roles de usuario de incentivos del Centro de partners?** 

Los roles de incentivos del Centro de partners se basan en la ubicación e incluyen al administrador de los incentivos y al usuario de los incentivos. Para más información sobre lo que pueden hacer esos roles, consulta [Asignar roles y permisos de usuarios](permissions-overview.md).

**¿Pueden asignarse los usuarios de incentivos en el nivel global y de ubicación?**

 Sí. Puedes asignar un administrador de incentivos para que sea el administrador de incentivos de todas las ubicaciones o cada ubicación puede tener su propio administrador de incentivos.

 **¿Se pueden pagar incentivos en el nivel global o de ubicación?**

 Los incentivos solo se pagan en el nivel de ubicación.

**En relación con las referencias, ¿cuántos perfiles de negocio se pueden crear?**

Tu compañía puede crear tantos perfiles de negocio como necesite para representar por completo los intereses de tu compañía. En cada perfil de negocio, puedes mostrar hasta cinco ubicaciones, una ubicación por país. Cada perfil de negocio puede recibir referencias para cada una de sus ubicaciones.

**¿Cómo se asignarán las referencias, qué cambios se pueden esperar? Por ejemplo, si tengo una compañía global en un mercado y ubicaciones en otros mercados, ¿cómo se asignarán las referencias?**

Las referencias se asignan en función de los parámetros de búsqueda que define el cliente. Por tanto, independientemente de si tienes una ubicación o varias, si el cliente especifica una ubicación deseada y tienes un negocio allí que cumple con los demás parámetros, la referencia irá a esa ubicación.








