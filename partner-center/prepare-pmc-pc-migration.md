---
title: Preparar para pasar de Partner Membership Center al centro de partners | Centro de partners
ms.topic: article
ms.date: 06/13/2019
description: Aspectos que hay que pensar antes de mover su negocio de PMC al centro de partners
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: fc3b457af07c4433d2b311f066cbeb240243ee0c
ms.sourcegitcommit: 09b3f69db956717e59709ee4c78bc9e879844adc
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/20/2019
ms.locfileid: "67279886"
---
# <a name="prepare-for-your-move-from-partner-membership-center-pmc-to-partner-center"></a>Preparar para la migración desde Partner Membership Center (PMC) al centro de partners

Movemos administración de pertenencia de Partner Membership Center (PMC) para el centro de partners: el único destino para administrar la relación comercial con Microsoft. Queremos pasar a centro de partners para ser lo más eficaz y fácil posible. Hemos identificado algunas áreas donde el centro de partners difiere de PMC; y pensamos que deseará comprenderlas y prepararse para ellos antes de realizar el movimiento.

## <a name="account-and-identity-setup"></a>Programa de instalación de la cuenta y de identidad

**¿Qué es una cuenta de trabajo de Azure Active Directory (Azure AD)?**

Una cuenta profesional de Azure es una representación virtual dedicada y aislada de tu empresa en la nube pública de Azure, creada automáticamente cuando te suscribes a un servicio en la nube de Microsoft como Azure, Microsoft Intune u Office 365.

La cuenta de trabajo hospeda los usuarios de Azure AD y la información sobre ellos: su correo electrónico, contraseñas, datos de perfil, permisos y así sucesivamente. La cuenta de trabajo también contiene grupos, aplicaciones y otra información relativa a una empresa y su seguridad. Para obtener más información, vea...

En el centro de partners usará su correo electrónico profesional para iniciar sesión en su cuenta no es su correo electrónico personal.
- Su cuenta profesional: john@contoso.com
- Su cuenta personal: John@outlook.com

El correo electrónico de trabajo forma parte de su inquilino de Azure active directory. Para tener una cuenta de centro de partners, debe tener un inquilino de AAD. Para obtener más información sobre Azure Active Directory, lea [crear su directorio de Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/fundamentals/add-custom-domain#create-your-directory-in-azure-ad).

**Cuando se mueve al centro de partners de PMC, ¿qué cuenta debe iniciar sesión en Centro de partners con if un inquilino de AAD con Microsoft (para Office 365, por ejemplo) y usted también tiene un inquilino para su negocio CSP?**

Puede iniciar sesión en Partner Center con la cuenta CSP o la cuenta de correo electrónico del trabajo MPN. Si decide iniciar sesión con su correo electrónico profesional CSP, en el panel de navegación izquierdo se mostrará información sobre el programa MPN y CSP. Si inicia sesión con su correo electrónico profesional de inquilino de Azure AD de MPN, verá solo la información del programa MPN. Roles de usuario diferencian de MPN y CSP así que asegúrese de asignar roles de usuario en consecuencia si usa la misma cuenta para la empresa MPN y CSP,. Para obtener información sobre los roles de usuario, lea [asignar permisos y roles de usuario](permissions-overview.md).

**¿Qué es la diferencia entre el rol de administrador global de AAD y el rol de administrador global de PMC MPN?**

Estos son dos roles diferentes completamente con permisos diferentes. El administrador global de inquilino AAD en el centro de partners administra al inquilino: agrega o quita los usuarios, proporciona y administra las contraseñas, roles y permisos y tiene acceso a programas de toda la empresa en el centro de partners. 

El rol de administrador global de MPN en PMC podría hacer lo siguiente:

- Ver y editar todos los datos asociados con la empresa y todas las ubicaciones de la empresa

-  Agregue los administradores en el nivel global o local.  Además, los administradores globales pueden asignar a cualquier persona en cualquier ubicación de acceso de administrador Global que les concede acceso global, independientemente de qué ubicación que están asociados.
-  Lleve a cabo a cualquier socio orientado a la función de la interfaz de usuario incluidas: 

-  Agregar o quitar usuarios

 - Asignar o quitar roles 

 - Agregar, quitar o actualizar ubicaciones 

 - Competencia de compra/asignaciones 

-  Ventajas de la vista

Cuando el administrador global de MPN se mueve al centro de partners la función se llama el administrador del asociado MPN que tiene permisos diferentes y las tareas que el administrador global de centro de partners. Para obtener más información sobre los roles y permisos en el centro de partners, lea [asignar roles a los usuarios y permisos](permissions-overview.md)

**Roles de usuario en el centro de partners**

Centro de partners tiene diferentes tipos de roles según los tipos de trabajo que se debe realizar. Hay funciones como administrador global que son roles de Azure AD. Algunos de los roles son específicos de programas como el proveedor de servicios en la nube o incentivos y hay funciones que son específicas de MPN. Para averiguar cuáles son todos los roles de centro de partners, leer [asignar roles a los usuarios y permisos](permissions-overview.md).

**¿Qué ocurre con los roles Mis usuarios cuando pasan de PMC al centro de partners?**

Excepto para el contacto principal del programa que lleva a cabo la migración o el administrador global de MPN, todos los usuarios en la PMC perderán sus roles de administrador. La persona que se complete la migración debe asignarles roles en el centro de partners. Los roles en el centro de partners diferencian de los de la PMC. Lectura [asignar roles a los usuarios y permisos](permissions-overview) y [mover de PMC al centro de partners](https://docs.microsoft.com/en-us/partner-center/move-pmc-pc-map#user-roles) para obtener más en roles de usuario en el centro de partners.


**¿Qué es la diferencia entre mi perfil de la empresa y mi perfil de negocio?**

Perfil de su empresa es la información acerca de su compañía que incluya la dirección, ubicaciones, contacto principal, información bancaria y fiscal.

El perfil de negocio es cómo presentar usted mismo a los clientes y una página de marketing que muestra su logotipo, obtener más información sobre el foco de su negocio, su experiencia, etcetera.

**¿Qué tiene en cuenta el promedio de consolidación para mi cuenta?**

Si usa al mismo inquilino de Azure AD para migrar varias cuentas de MPN en Centro de partners, el sistema reconocerá automáticamente y pedirle que consolidar las cuentas. Esto es cierto incluso si tiene varios dominios asociados al mismo inquilino de Azure AD. 

Podría decidir migrar al centro de partners mediante independiente de los inquilinos AAD, pero tenga en cuenta que este produce aislado de evaluación de sus competencias y adicional de costos de adquisición. 

**¿Si tengo varios inquilinos AAD y una sola cuenta MPN, es posible crear un vínculo a ellas en el centro de partners?**

Sí, en el centro de partners puede vincular a varios inquilinos de Azure AD a solo cuenta del centro de partners.
Obtenga más información aquí. 


## <a name="microsoft-partner-network-mpn-membership-migration"></a>Migración de suscripción de Microsoft Partner Network (MPN) 

**¿Quién puede realizar el movimiento de PMC al centro de partners?**

El administrador global de MPN de empresa o el contacto de programa principal (estas dos funciones a menudo se mantienen por la misma persona) puede iniciar y realizar el movimiento.

**¿Se convertirá la persona que completa la migración en el contacto principal en el perfil legal de la empresa en el centro de partners?**

No necesariamente, sin embargo, el contacto principal debe ser alguien que tenga autorización para firmar contratos.

**¿Microsoft puede migrar Mis suscripciones MPN para mí?**

No. Microsoft no puede ayudarle a mover la cuenta de pertenencia al centro de partners. Debe mover la cuenta iniciando sesión en PMC con su cuenta profesional (inicio de sesión en las credenciales) comenzar el proceso de migración. Después de haber completado los pasos para mover la cuenta puede empezar a administrar la pertenencia y asignar permisos y roles de usuario a su equipo para que puedan obtener acceso a beneficios y ayudar a administrar la pertenencia. Microsoft migrará automáticamente las competencias actuales, ventajas, información de ubicación, la información bancaria y fiscal de incentivos y las asociaciones de MCP, incluido el acceso de Partner University.

Microsoft migrará automáticamente las competencias actuales, ventajas, información de ubicación, la información bancaria y fiscal de incentivos y las asociaciones de MCP, incluido el acceso de Partner University.

**¿Cómo cambiará la directiva de renovación?**

 En el centro de partners, la ventana de renovación es desde la fecha de aniversario a través de los 30 días siguientes.

**¿Nuestras competencias no cambios después de que se mueven al centro de partners?**

Sí, competencias no se verán afectados por el traslado al centro de partners. Si observa las discrepancias, póngase en contacto con [soporte](https://partner.microsoft.com/support).


 **¿Cambiarán Mis ventajas (incluidas las ventajas de la nube, soporte técnico, ventajas de software, Visual Studio) después de que se mueva?**

 Los beneficios elegibles no cambiará. Si observa las discrepancias, póngase en contacto con [soporte](https://partner.microsoft.com/support).

 **¿Se respetará las cuentas de Microsoft que tienen asignaciones de las ventajas de Visual Studio?**


 Sí. Se respeta y conserva asignados para MSA beneficios de Visual Studio. También se conservarán después de la renovación en el centro de partners. Sin embargo, si quita una asignación de MSA una vez migrado en el centro de partners, no se puede agregar al centro de partners.

En el centro de partners, puede agregar un asociado de cuentas profesionales y las cuentas de usuario invitado que son MSA desde el mismo inquilino donde el asociado es MPN admin en el inquilino de Azure AD. Si el asociado es un administrador global en varios inquilinos de Azure AD y todos los inquilinos de estos están asociados a la misma cuenta de centro de partners, el asociado se permite agregar usuarios en todos estos inquilinos a las ventajas de Visual Studio y las asignaciones según el uso de Azure.

Aunque los usuarios invitados pueden asignarse según el uso de las suscripciones de Visual Studio mediante el administrador MPN o administrador global, los usuarios invitados no pueden iniciar sesión centro de partners usando su MSA. Los usuarios invitados pueden, sin embargo, inicie sesión en Azure y Visual Studio para validar y usar sus beneficios asignados.


 **¿Cómo debemos administramos nuestras asociaciones de MCP y nuestro acceso Partner University?**

 No hay ningún cambio en las asociaciones de MCP mover desde la PMC. Sin embargo, los nuevos empleados nuevo después de mover al centro de partners deberá estar asociados en el centro de partners. Todos los permisos de Partner University para usuarios existentes permanecerán pero los nuevos empleados deben ir a [el centro de aprendizaje](https://partner.microsoft.com/training) para obtener información sobre cómo obtener acceso a Partner University.

 **¿Se usan referencias de clientes en el centro de partners?**

 No, no necesita referencias de clientes para cumplir los requisitos de capacidad en el centro de partners.

 **¿Las asociaciones de socio de registro se moverán al centro de partners?**

 Sí, no hay ningún cambio en el socio de registro. Obtenga más información sobre [vincular su Id. de partner a sus clientes](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).

**¿Hay un impacto a incentivos debido a la migración a centro de partners?**

No, no hay ningún impacto en los incentivos si ha movido la cuenta sin las ubicaciones de consolidación. Si su empresa tiene varias cuentas en PMC y, cuando se mueve al centro de partners, decide consolidar en una cuenta global, no habrá pérdida de incentivos, pero puede haber un retraso en los pagos incentivos. Si no mueve todas las cuentas PMC que se han visto involucradas en programas de incentivos, puede dejar a ganar incentivos que están asociados a esas cuentas.


**¿Cuáles son los roles de usuario incentivos en Centro de partners?** 

Incentivos roles en el centro de partners están basados en ubicación e incluyen Administrador de incentivos y del usuario de incentivos. Para obtener más información sobre lo que pueden hacer en esos roles, consulte [asignar roles a los usuarios y permisos](permissions-overview.md).

**¿Los usuarios de incentivos se pueden asignar en el nivel global y la ubicación?**

 Sí. Puede asignar un administrador incentivos para que sea el Administrador de incentivos para todas las ubicaciones o cada ubicación puede tener su propio administrador de incentivos.

 **¿Pueden pagar incentivos en el nivel global o ubicación?**

 Incentivos se pagan solo en el nivel de ubicación.

**¿Con respecto a las referencias, cuántos perfiles de negocio podemos crear?**

Su empresa puede crear varios perfiles de negocio como la necesidad de representan por completo los intereses de su compañía. En cada perfil de negocio, puede mostrar hasta cinco ubicaciones, una ubicación por país. Cada uno de los perfiles de negocio puede recibir las referencias para cada uno de sus ubicaciones.

**¿Cómo las referencias se asignarán, qué cambios puede esperar? ¿Por ejemplo, si tengo una empresa en un mercado internacional y las ubicaciones en otros mercados, cómo las referencias se asignará?**

Las referencias se asignan en función de los parámetros de búsqueda que define el cliente. Entonces, independientemente de si tiene una ubicación o en varias, si los clientes especifica la ubicación deseada y tendrá que existe una empresa que cumpla con los demás parámetros, a continuación, la referencia iría a esa ubicación.








