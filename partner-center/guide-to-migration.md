---
title: Guía para la migración desde PMC al centro de Partners | Centro de Partners
ms.topic: article
ms.date: 04/25/2019
description: Qué debe saber al migrar su empresa de PMC al centro de Partners
author: LauraBrenner
ms.author: labrenne
keywords: PMC, migración, pasar al centro de Partners
ms.localizationpriority: medium
ms.openlocfilehash: f8e0b1fa4b31608ed4031832018c0a003abf0ae9
ms.sourcegitcommit: 9d01fb30eafc523784ecc3568c05da9bbe9a1e8c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/01/2019
ms.locfileid: "68708918"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Guía para la migración de PMC al centro de Partners

El sitio web de Microsoft Partner en partner.microsoft.com es una experiencia digital unificada para asociados. En el sitio web del asociado, podrá explorar sus oportunidades y participar en experiencias guiadas que ayuden a su empresa a crear y vender sus aplicaciones y servicios con Microsoft. Mediante el vínculo del panel que está disponible en el sitio web del asociado, los miembros del Microsoft Partner Network pueden iniciar sesión en el centro de Partners en el que administra su relación con Microsoft, inscribirse en programas y registrarse para obtener ofertas. 

Se está retirando el centro de pertenencia de asociados (PMC). Se ha invitado a su empresa a pasar su Microsoft Partner Network la administración de pertenencia al centro de Partners. Esta guía le preparará para lo que puede esperar a medida que realice el cambio de PMC al centro de Partners.

>[!Note]
>Incluso si su compañía tiene más de una cuenta o una ubicación, el traslado al centro de Partners comienza moviendo una (su primera) cuenta al centro de Partners.

## <a name="get-started"></a>Introducción

El movimiento comienza en PMC. El administrador global recibirá una invitación para comenzar el traslado. 

**Preparación en PMC**
- Comprobar los detalles de la empresa 
- Comprobar contacto principal del programa 
- Comprobar las ubicaciones de negocio
- Actualización de los usuarios aprobados

**Cuando esté listo**

Seleccione **Introducción** a la invitación. Se le dirigirá a la página de inicio de sesión del centro de Partners.

![Introducción](images/migration/getstarted.jpg)

## <a name="start-with-your-work-email"></a>Comience con el correo electrónico del trabajo

Si su empresa no tiene un correo electrónico de trabajo y un inquilino de AAD, podemos ayudarle a configurar uno durante el proceso de inicio de sesión del centro de Partners. Cuando intente iniciar sesión con una cuenta de correo electrónico que no sea un correo electrónico de trabajo como su cuenta personal, se le indicará que proporcione información sobre su empresa para que podamos configurar un inquilino de AAD y un correo electrónico de trabajo.
Estos detalles de la compañía se usarán para finalizar su cuenta en el centro de Partners, por lo que debe asegurarse de que son precisos.

>[!Note]
>Si es un asociado en China y está inscrito en el programa de Microsoft Partner Network y del proveedor de soluciones en la nube (CSP), tendrá un inquilino independiente para cada cuenta. Su cuenta con el programa proveedor de soluciones en la nube se administra en la nube nacional y la cuenta de Microsoft Partner Network se administra en la nube global. Las dos cuentas no se pueden vincular.

![Cuéntenos su empresa](images/migration/newtellusabout.png)

Una vez que haya comprobado o actualizado la información, seleccione **Aceptar y continuar**.
Los términos y condiciones de esta página son **exactamente iguales** que el acuerdo que la compañía ya firmó en PMC.  
Esto iniciará la creación del inquilino de Azure AD y proporcionará la cuenta profesional.

La selección de **Aceptar y continuar** también hace lo siguiente:

• Migra la cuenta junto con todas sus ubicaciones al centro de Partners

• Migra cualquier competencia o mapa que haya adquirido en PMC

• Migra las ventajas (mapas, plata y oro) que tenía en PMC

## <a name="invite-employees-to-join-you"></a>Invitar a los empleados a unirse a usted

Cuando se crea el nuevo inquilino de Azure AD, puede invitar a los empleados a que inicien sesión en el centro de Partners.

![Invitar a los empleados](images/migration/invite.png)


Si ha iniciado sesión con un inquilino de AAD existente, los empleados se moverán con usted. En este caso, asigne los roles de los empleados que determinen lo que pueden hacer en el centro de Partners. Nota: Los roles del centro de Partners son diferentes de los roles en PMC. Para obtener más información, consulte [pasar de PMC al centro de Partners](move-pmc-pc-map.md).

## <a name="verify-your-domain-and-become-a-global-admin"></a>Comprobar el dominio y convertirse en administrador global  

Si el inquilino de AAD es nuevo, nadie tiene asignado el rol de administrador global. Para convertirse en el administrador global, debe comprobar la propiedad del dominio. Es posible que necesite el administrador del dominio para ayudarle con esto. Tenga en cuenta que, aunque puede usar las ofertas que ya ha comprado, no podrá comprar nuevas ofertas hasta que complete el paso de obtener un administrador global. 

![Tomar control](images/migration/takecontrol.png)

Al seleccionar introducción, verá la siguiente pantalla:

![Comprobar la propiedad del dominio](images/migration/verifytxt.png)

El registrador de dominios ya estará rellenado. Solo el propietario del dominio puede actualizar el archivo DNS, por lo que al copiar y agregar el archivo de texto al registro DNS, podemos comprobar que es el propietario. La actualización tardará unos minutos en realizarse. Tendrá que cerrar la sesión del centro de Partners y volver a iniciar sesión. Su rol se habrá cambiado a administrador global. 


## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Familiarícese con el panel y el centro de Partners

Paseo por el panel. Aquí puede administrar su pertenencia, agregar un perfil de negocio para las referencias, inscribirse en el programa proveedor de soluciones en la nube y ver las notificaciones y ofertas relevantes para su empresa en cualquier momento seleccionando **Panel**. También puede administrar incentivos, comprar en Marketplace, registrarse para obtener servicios de comercialización y mucho más.  

![Paseo](images/migration/fre.png)

## <a name="next-steps"></a>Pasos siguientes

- [Crear cuentas de usuario](create-user-accounts-and-set-permissions.md)
- [Asignar roles de usuario y permisos](permissions-overview.md)
- [Administrar los programas de pertenencia](renew-mpn-offers.md)
- [Crear el perfil de negocio de su empresa](create-a-marketing-profile.md)
- [Conexión con los clientes a través de referencias](responding-to-referrals.md)

## <a name="see-also"></a>Vea también

- [Guía para la migración de varias empresas de PMC al centro de Partners](move-multiple-companies.md)
