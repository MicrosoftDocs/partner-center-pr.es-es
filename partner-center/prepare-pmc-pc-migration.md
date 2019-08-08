---
title: Preparar la migración del centro de pertenencia del asociado al centro de Partners | Centro de Partners
ms.topic: article
ms.date: 06/13/2019
description: Aspectos que se deben tener en cuenta antes de trasladar su negocio de PMC al centro de Partners
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: d6db2dcb5ac53e29d907c09ca2b16d123b21c07f
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820572"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Prepárese para pasar del centro de afiliación del asociado (PMC) al centro de Partners

Estamos trasladando la administración de pertenencia del centro de afiliación de asociados (PMC) al centro de Partners: el único destino para administrar su relación de negocio con Microsoft. Queremos que el centro de Partners sea lo más eficaz y sencillo posible. Hemos identificado algunas áreas en las que el centro de Partners difiere de PMC y creemos que le interesará comprender y prepararse antes de realizar el traslado.

## <a name="account-and-identity-setup"></a>Configuración de cuentas e identidades

**¿Qué es una cuenta profesional de Azure Active Directory (Azure AD)?**

Una cuenta profesional de Azure es una representación virtual dedicada y aislada de tu empresa en la nube pública de Azure, creada automáticamente cuando te suscribes a un servicio en la nube de Microsoft como Azure, Microsoft Intune u Office 365.

Su cuenta profesional hospeda su Azure AD usuarios y la información sobre ellos: su correo electrónico, contraseñas, datos de perfil, permisos, etc. La cuenta profesional también contiene grupos, aplicaciones y otra información relativa a una empresa y su seguridad. Para obtener más información, vea...

En el centro de Partners, usará el correo electrónico del trabajo para iniciar sesión en su cuenta, no su correo electrónico personal.
- Su cuenta profesional:john@contoso.com
- Tu cuenta personal:John@outlook.com

El correo electrónico de trabajo forma parte del inquilino de Azure Active Directory. Para tener una cuenta en el centro de Partners, debe tener un inquilino de AAD. Para obtener más información sobre Azure Active Directory, lea [crear el directorio en Azure ad](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

**Al pasar al centro de Partners desde PMC, ¿qué cuenta debe iniciar sesión en el centro de Partners con si tiene un inquilino de AAD con Microsoft (por ejemplo, para Office 365) y también tiene un inquilino para su negocio de CSP?**

Puede iniciar sesión en el centro de Partners con la cuenta de CSP o la cuenta de correo electrónico del trabajo de MPN. Si elige iniciar sesión con el correo electrónico de trabajo de CSP, el panel de navegación izquierdo en el panel mostrará la información de los programas MPN y CSP. Si inicia sesión con el correo electrónico de trabajo del inquilino de MPN Azure AD, solo verá la información del programa MPN. Los roles de usuario difieren entre MPN y CSP, por lo que si usa la misma cuenta para el negocio de MPN y CSP, asegúrese de asignar roles de usuario en consecuencia. Para obtener información sobre los roles de usuario, consulte [asignar roles de usuario y permisos](permissions-overview.md).

**¿Cuál es la diferencia entre el rol de administrador global de AAD y el rol de administrador global de PMC MPN?**

Se trata de dos roles completamente diferentes con permisos diferentes. El administrador global del inquilino de AAD del centro de Partners administra el inquilino: agrega o quita usuarios, proporciona y administra contraseñas, roles y permisos, y tiene acceso a todos los programas de su empresa en el centro de Partners. 

El rol de administrador global MPN en PMC podría hacer lo siguiente:

- Ver y editar todos los datos asociados a la empresa y todas las ubicaciones de la empresa

-  Agregue administradores en el nivel global o local.  Además, los administradores globales pueden asignar cualquier persona en cualquier ubicación acceso de administrador global, que les concede acceso global independientemente de la ubicación a la que estén asociadas.
-  Realice cualquier función de interfaz de usuario orientada a asociados, incluidos: 

-  Agregar o quitar usuarios

 - Asignar o quitar roles 

 - Agregar/quitar/actualizar ubicaciones 

 - Adquirir competencia/Maps 

-  Ver las ventajas

Cuando el administrador global de MPN se mueve al centro de Partners, el rol se denomina administrador de asociados de MPN, que tiene permisos y tareas diferentes que el administrador global del centro de Partners. Para obtener más información sobre roles y permisos en el centro de Partners, lea [asignar roles y permisos a los usuarios](permissions-overview.md).

**Roles de usuario, incluidos los roles de usuario invitado en el centro de Partners**

El centro de Partners tiene distintos tipos de roles en función de los tipos de trabajo que es necesario realizar. Hay roles como el administrador global que se Azure AD roles. Algunos de los roles son específicos de programas como el programa de proveedor de servicios en la nube o los incentivos, y hay roles que son específicos de MPN. Para averiguar qué son todos los roles del centro de Partners, lea [asignar roles y permisos a los usuarios](permissions-overview.md).



**¿Qué ocurre con los roles de mis usuarios cuando pasan de PMC al centro de Partners?**

Excepto en el caso del administrador global de MPN o del programa principal que realiza la migración, todos los usuarios de PMC perderán sus roles de administrador. La persona que complete la migración deberá asignar roles en el centro de Partners. Los roles del centro de Partners son distintos de los de PMC. Lea [asignar roles y permisos de usuarios] (permisos-overview.md y [pasar de PMC al centro de Partners](https://docs.microsoft.com/partner-center/move-pmc-pc-map#user-roles) para obtener más información sobre las funciones de usuario en el centro de Partners.


**¿Cuál es la diferencia entre mi perfil de empresa y mi perfil de negocio?**

El perfil de su empresa es la información sobre su empresa que incluye la dirección, las ubicaciones, el contacto principal, los detalles bancarios y los impuestos.

Su perfil de negocio es la forma en que se presenta a los clientes y es una página de marketing que muestra su logotipo, los detalles sobre su enfoque empresarial, su experiencia, etc.

**¿Qué significa la consolidación de cuentas para mi cuenta?**

Si usa el mismo inquilino de Azure AD para migrar varias cuentas de MPN al centro de Partners, el sistema lo reconocerá automáticamente y le pedirá que consolide sus cuentas. Esto es así incluso si tiene varios dominios asociados al mismo inquilino de Azure AD. 

Todavía puede optar por migrar al centro de partners mediante inquilinos de AAD independientes, pero tenga en cuenta que esto produce una evaluación aislada de sus competencias y costes de compra adicionales. 

**Si tengo varios inquilinos de AAD y una sola cuenta de MPN, ¿es posible vincularlos en el centro de Partners?**

Sí, en el centro de Partners, puede vincular varios inquilinos de Azure AD a una cuenta del centro de Partners.
Obtenga más información aquí. 

**¿Existen restricciones para agregar varios inquilinos de Azure AD a una sola cuenta de centro de Partners?**

Si el inquilino de Azure AD ya está asociado a una cuenta de centro de Partners existente, no se puede asociar a las nuevas cuentas del centro de partners mediante la característica multiinquilino. Otra manera de pensar en esto es que un inquilino de Azure AD solo se puede asociar a una cuenta del centro de Partners, pero una cuenta del centro de Partners puede tener varios inquilinos asociados.

## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migración de pertenencia a Microsoft Partner Network (MPN) 

**¿Quién puede realizar el cambio de PMC al centro de Partners?**

El administrador global de MPN de la empresa o el contacto del programa principal (estos dos roles suelen ser mantenidos por la misma persona) pueden iniciar y realizar el cambio.

**¿La persona que completa la migración se convierte en el contacto principal del perfil legal de la empresa en el centro de Partners?**

Sin embargo, no necesariamente, el contacto principal debe ser un usuario que tenga autorización para firmar los acuerdos.

**¿Puede Microsoft migrar mi suscripción a MPN?**

No. Microsoft no puede ayudarle a migrar su cuenta de pertenencia al centro de Partners. Deberá trasladar su cuenta iniciando sesión en PMC con su cuenta profesional (credenciales de inicio de sesión) para comenzar el proceso de migración. Una vez que haya completado los pasos para migrar su cuenta, puede empezar a administrar la pertenencia y asignar roles de usuario y permisos a su equipo para que puedan acceder a las ventajas y ayudar a administrar la pertenencia. Microsoft migrará automáticamente las competencias actuales, las ventajas, la información de ubicación, la información bancaria o fiscal para incentivos y asociaciones de MCP, incluido el acceso a la Universidad de asociados.

Microsoft migrará automáticamente las competencias actuales, las ventajas, la información de ubicación, la información bancaria o fiscal para incentivos y asociaciones de MCP, incluido el acceso a la Universidad de asociados.

**¿Cómo cambiará la Directiva de renovación?**

 En el centro de Partners, la ventana de renovación procede de la fecha de aniversario hasta los 30 días siguientes.

**¿Las competencias permanecerán sin cambios después de pasar al centro de Partners?**

Sí, Compentencies no se verá afectado por el traslado al centro de Partners. Si observa discrepancias, póngase en contacto [con el soporte técnico](https://partner.microsoft.com/support).


 **¿Las ventajas (incluidas las ventajas en la nube, el soporte técnico, los beneficios de software y Visual Studio) cambian después de moverlas?**

 Las ventajas que pueda elegir no cambiarán. Si observa discrepancias, póngase en contacto [con el soporte técnico](https://partner.microsoft.com/support).

 **¿Se respetan las cuentas de Microsoft con las asignaciones de ventajas de Visual Studio?**


 Sí. Las ventajas de Visual Studio asignadas a MSAs se respetarán y se conservarán. También se conservarán después de la renovación en el centro de Partners. Sin embargo, si quita una asignación de MSA una vez migrada en el centro de Partners, no se puede volver a agregar al centro de Partners.

En el centro de Partners, un asociado puede agregar cuentas profesionales y cuentas de usuario invitado que son MSA del mismo inquilino donde el asociado es administrador de MPN en el inquilino de Azure AD. Si el asociado es un administrador global en varios inquilinos de Azure AD y todos estos inquilinos están asociados a la misma cuenta del centro de Partners, se permite que el asociado Agregue usuarios en todos estos inquilinos a las ventajas de Visual Studio y a las asignaciones basadas en el uso de Azure.

Aunque los usuarios invitados pueden asignar suscripciones basadas en el uso de Visual Studio mediante el administrador de MPN o el administrador global, los usuarios invitados no pueden iniciar sesión en el centro de partners mediante su MSA. Sin embargo, los usuarios invitados pueden iniciar sesión en Azure y Visual Studio para validar y usar sus ventajas asignadas.


 **¿Cómo se debe administrar nuestras asociaciones de MCP y el acceso a la Universidad de asociados?**

 No hay cambios en las asociaciones de MCP que se mueven desde PMC. Sin embargo, todos los nuevos empleados nuevos después de pasar al centro de Partners deberán estar asociados al centro de Partners. Todos los permisos de Universidad de asociados para los usuarios existentes permanecerán, pero los nuevos empleados deben ir al [centro de aprendizaje](https://partner.microsoft.com/training) para obtener información sobre cómo obtener acceso a la Universidad de asociados.

 **Cómo ver información de MCP una vez que se pasa al centro de Partners?**

Seleccione **competencias** en la navegación izquierda en el panel. En la página **competencias** puede descargar el informe de aptitudes. El informe de aptitudes mostrará los usuarios que han adquirido conocimientos pertinentes para las competencias y los programas del centro de Partners. Si los usuarios han adquirido conocimientos, pero no son relevantes para las competencias en las que está trabajando, no se mostrarán en el informe.


 **¿Se usan referencias de cliente en el centro de Partners?**

 No, no es necesario que las referencias de los clientes cumplan los requisitos de competencia del centro de Partners.

 **¿Se va a asociar las asociaciones de registros al centro de Partners?**

 Sí, no hay ningún cambio en el asociado del registro. Obtenga más información sobre cómo [vincular su identificador de socio a sus clientes](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).

**¿Hay algún impacto en los incentivos debido al traslado al centro de Partners?**

No, no hay ningún impacto en los incentivos si ha pasado su cuenta sin consolidar las ubicaciones. Si su empresa tiene varias cuentas en PMC y, al pasar al centro de Partners, decide consolidar en una cuenta global, no habrá ninguna pérdida por incentivos, pero puede haber un retraso en el pago de incentivos. Si no mueve todas las cuentas de PMC que han participado en los programas de incentivos, puede dejar de ganar incentivos que están vinculados a esas cuentas.


**¿Cuáles son las funciones de usuario de estímulo del centro de Partners?** 

Los roles de incentivos del centro de Partners se basan en la ubicación e incluyen el usuario de los incentivos y el administrador de incentivos. Para obtener más información sobre lo que pueden hacer esos roles, consulte [asignación de roles y permisos de usuarios](permissions-overview.md).

**¿Puede incentivar a los usuarios a asignarse en el nivel global y de ubicación?**

 Sí. Puede asignar un administrador de incentivos para que sea el administrador de incentivos para todas las ubicaciones o cada ubicación puede tener su propio administrador de incentivos.

 **¿Se pueden pagar incentivos en el nivel global o de ubicación?**

 Los incentivos solo se pagan en el nivel de ubicación.

**En relación con las referencias, ¿cuántos perfiles de negocio se pueden crear?**

Su empresa puede crear tantos perfiles de negocio como necesite para representar por completo los intereses de su empresa. En cada perfil de negocio, puede mostrar hasta cinco ubicaciones, una ubicación por país. Cada perfil de negocio puede recibir referencias para cada una de sus ubicaciones.

**¿Cómo se asignarán las referencias, qué cambios se pueden esperar? Por ejemplo, si tengo una empresa global en un mercado y ubicaciones en otros mercados, ¿cómo se asignarán las referencias?**

Las referencias se asignan en función de los parámetros de búsqueda que define el cliente. Por tanto, independientemente de si tiene una ubicación o varias, si los clientes especifican una ubicación deseada y tiene una empresa en la que se cumplen los otros parámetros, la referencia irá a esa ubicación.








