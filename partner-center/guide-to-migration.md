---
title: Migración de PMC al Centro de partners
ms.topic: article
ms.date: 05/20/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprende a migrar tu empresa de Partner Membership Center (PMC) al Centro de partners.
author: LauraBrenner
ms.author: labrenne
keywords: PMC, migration, moving to Partner Center
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 773466a1c7bfb8a091be11f8e825dae6cc90b765
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679092"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Guía para la migración de PMC al Centro de partners

**Roles adecuados**

- Administrador global

El sitio web para partners de Microsoft en partner.microsoft.com es una experiencia digital unificada para los partners. En el sitio web para partners, podrás explorar tus oportunidades y participar en experiencias guiadas que ayuden a tu empresa a compilar y vender tus aplicaciones y servicios con Microsoft. Mediante el vínculo del panel que está disponible en el sitio web para partners, los miembros de Microsoft Partner Network pueden iniciar sesión en el Centro de partners donde administras tu relación con Microsoft, inscribirse en programas y registrarse para obtener ofertas.

La oferta Partner Membership Center (PMC) se está retirando. Tu empresa ha recibido una invitación para migrar la administración de su pertenencia a Microsoft Partner Network al Centro de partners. Esta guía te preparará para las expectativas durante la migración de PMC al Centro de partners.

>[!NOTE]
>Aunque tu empresa tenga más de una cuenta o ubicación, la migración al Centro de partners comienza con el cambio de una (tu primera) cuenta al Centro de partners.

## <a name="get-started"></a>Introducción

La migración comienza en PMC. Tu administrador global recibirá una invitación para iniciar la migración.

### <a name="prepare-in-pmc"></a>Preparativos en PMC

- Comprobar los detalles de la empresa
- Comprobar el contacto principal del programa
- Comprobar las ubicaciones de la empresa
- Actualizar los usuarios aprobados

### <a name="when-youre-ready"></a>Después de realizar los preparativos

Selecciona **Introducción** en la invitación. Se te dirigirá a la página de inicio de sesión del Centro de partners.

:::image type="content" source="images/migration/getstarted.jpg" alt-text="Introducción":::

## <a name="start-with-your-work-email"></a>Empezar con el correo electrónico del trabajo

Si tu empresa no tiene un correo electrónico del trabajo ni un inquilino de AAD, podemos ayudarte a configurarlos durante el proceso de inicio de sesión en del Centro de partners. Si intentas iniciar sesión con una cuenta de correo electrónico que no es del trabajo (por ejemplo, una cuenta personal), se te indicará que proporciones información sobre la empresa para que podamos configurar un inquilino de AAD y un correo electrónico del trabajo. Estos detalles de la empresa se usarán para finalizar la cuenta en Centro de partners, por lo que debes asegurarte de que sean correctos.

>[!NOTE]
>Si eres un partner de China y estás inscrito en Microsoft Partner Network y en el programa Proveedor de soluciones en la nube (CSP), tendrás un inquilino diferente para cada cuenta. Tu cuenta con el programa Proveedor de soluciones en la nube se administra en la nube nacional y la cuenta de Microsoft Partner Network se administra en la nube global. Las dos cuentas no pueden estar vinculadas.

:::image type="content" source="images/migration/newtellusabout.png" alt-text="Háblenos de su empresa":::

Una vez que hayas comprobado o actualizado la información, selecciona **Aceptar y continuar**.
Los términos y condiciones de esta página son **exactamente los mismos** que los del acuerdo que la empresa firmó en PMC.  
Este paso inicia la creación del inquilino de Azure AD y te proporciona la cuenta profesional.

Al seleccionar **Aceptar y continuar** también sucede lo siguiente:

- Migra tu cuenta junto con todas sus ubicaciones al Centro de partners.

- Migra todas las competencias o instancias de MAP que has adquirido en PMC.

- Migra todos los recursos, ofertas y programas de marketing (MAP, Silver y Gold) que tenías en PMC.

## <a name="invite-employees-to-join-you"></a>Invitar a empleados a unirse a ti

Cuando se crea tu nuevo inquilino de Azure AD, puedes invitar a los empleados a iniciar sesión en el Centro de partners.

:::image type="content" source="images/migration/invite.png" alt-text="Invitar a empleados":::

Si has iniciado sesión con un inquilino de AAD existente, los empleados se habrán migrado contigo. En este caso, asigna a tus empleados roles que determinen lo que pueden hacer en el Centro de partners. 

>[!NOTE] 
>Los roles del Centro de partners son diferentes de los roles de PMC. Para obtener más información, consulta [Migración de PMC al Centro de partners](move-pmc-pc-map.md).

## <a name="verify-your-domain-and-become-a-global-admin"></a>Comprobar el dominio y convertirse en administrador global  

Si el inquilino de AAD es nuevo, no se asigna a nadie el rol de administrador global. Para convertirse en el administrador global, debes comprobar la propiedad del dominio. Es posible que necesites la ayuda del administrador del dominio.

Aunque puede usar las ofertas que ya ha comprado, no podrá comprar nuevas ofertas hasta que complete el paso de asignación de un administrador global.

:::image type="content" source="images/migration/takecontrol.png" alt-text="Tomar el control":::

Al seleccionar Introducción, verás la siguiente pantalla:

:::image type="content" source="images/migration/verifytxt.png" alt-text="Comprobar la propiedad del dominio":::

El registrador de dominios aparecerá rellenado automáticamente. Solo el propietario del dominio puede actualizar el archivo DNS, de modo que al copiar y agregar el archivo de texto al registro DNS, podamos comprobar que eres el propietario. La actualización tardará unos minutos en producirse. Tendrás que cerrar la sesión del Centro de partners y volver a iniciarla. Tu rol habrá cambiado a administrador global.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Familiarízate con el panel y el Centro de partners

Visita el panel. Aquí puedes administrar tu pertenencia, agregar un perfil de negocio para las referencias, inscribirse en el programa Proveedor de soluciones en la nube, y ver las notificaciones y ofertas importantes para tu empresa en cualquier momento. Para ello, selecciona **Panel**. También puedes administrar incentivos, comprar en Marketplace, registrarte para obtener servicios de comercialización y mucho más.  

:::image type="content" source="images/migration/fre.png" alt-text="Visítelo":::

## <a name="next-steps"></a>Pasos siguientes

- [Crear cuentas de usuario](create-user-accounts-and-set-permissions.md)

- [Asignación de roles y permisos de usuario](permissions-overview.md)

- [Administración de programas de suscripción](renew-mpn-offers.md)

- [Creación del perfil de negocio de una empresa](create-a-marketing-profile.md)

- [Conexión con los clientes a través de referencias](responding-to-referrals.md)

- [Guía para la migración de varias empresas de PMC al Centro de partners](move-multiple-companies.md)
