---
title: Migración desde Partner Sales Connect (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo los asociados de Microsoft pueden migrar de Partner Sales Connect (PSC) a Centro de partners crear o administrar ofertas enviadas por vendedores de Microsoft.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: 5be1c09a26cfcc0d038663e5814ccda7e535d4d1
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551442"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Guía para la venta Centro de partners asociados que migran desde Partner Sales Connect (PSC)

**Roles adecuados:** Administrador de | Administrador de referencias | Partner Sales Connect (PSC) seller | Administrador de Partner Sales Connect (PSC) | Administrador de contratos de Partner Sales Connect (PSC)

En este artículo se proporcionan instrucciones para los asociados que migran de Partner Sales Connect (PSC) a Centro de partners (PC) para que puedan seguir con la creación y administración de ofertas de venta Centro de partners.

>[!Note]
> Si está aquí porque ha visto un banner en PSC sobre la migración, está en el lugar correcto. Esta guía no es aplicable a la evaluación de soluciones (SA) y a los asociados comerciales de licencias de OEM que administran sus ofertas en PSC.

>[!Important]
> A partir del 1 de abril de 2021, su empresa no podrá crear ni editar ofertas en PSC. **Todavía podrá descargar los datos de ofertas existentes mediante la funcionalidad de exportación masiva en PSC. También puede migrar [ofertas abiertas](psc-to-pc.md#psc-deals-migration) de PSC a Centro de partners después de esta fecha.** <br><br> Si hay ofertas en las que esté trabajando activamente que contengan soluciones aptas para incentivos de venta co-venta de IP, tiene dos opciones: <br><br> 1. Marque la oferta como ganada y complete el registro de la oferta en PSC antes del 31 de marzo de 2021. <br> 2. [Migre las ofertas](psc-to-pc.md#psc-deals-migration) a Centro de partners para que obtenga más tiempo para trabajar en la oferta e iniciar el registro de la oferta.

Como sabe, la empresa perderá el acceso a PSC después del **30 de abril de 2021.** Sin embargo, todavía encontrará todo lo que quiere hacer en Centro de partners, como crear ofertas de venta coventa, administrar las ofertas y actuar sobre las ofertas que le envían los vendedores de Microsoft.

Sin embargo, habrá diferencias. La siguiente guía puede ayudar a que la transición a Centro de partners sea más sencilla y sencilla.

## <a name="before-you-move-things-you-need-to-know"></a>Antes de moverse, lo que necesita saber

### <a name="if-you-are-a-psc-admin"></a>Si es administrador de PSC

- Necesita un correo electrónico de trabajo para iniciar sesión en [Centro de partners](https://partner.microsoft.com/).
- Configure su cuenta con la ayuda del administrador de Centro de partners [cuenta.](permissions-overview.md)
- Obtenga información sobre cómo vender en Centro de partners este documento.
- Configure cuentas de usuario en Centro de partners para todos los usuarios de PSC (roles administrador, administrador de contratos y vendedor) y asígneles roles de administrador [de referencias](permissions-overview.md).

>[!IMPORTANT]
> Asegúrese de que el Microsoft Partner Network (MPN) que se muestra en el banner de PSC esté disponible en la lista de ubicaciones de MPN en Centro de partners.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Imagen en la que se muestra el banner de PSC donde los asociados pueden encontrar el identificador de MPN.":::

 Para comprobar que el identificador de MPN aparece como una ubicación de [](https://partner.microsoft.com/dashboard)MPN de Centro de partners, inicie sesión en el panel de Centro de partners y seleccione Configuración **(el** icono de engranaje) en la parte superior derecha de la pantalla, seguido de Configuración de la **cuenta.** En el menú de navegación izquierdo  del segundo nivel, seleccione Ubicaciones para ver la lista de todos los IDs y ubicaciones de MPN asociados a la cuenta Centro de partners usuario.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Si es un vendedor o administrador de contratos de PSC

- Necesita un correo electrónico de trabajo para iniciar sesión en el panel Centro de partners [trabajo.](https://partner.microsoft.com/dashboard)
- Si usa una cuenta que no es de trabajo en PSC o su correo electrónico de trabajo es para una empresa diferente de la empresa asociada, póngase en contacto con el administrador de PSC para obtener ayuda para la configuración de la cuenta.
- Consulte con el administrador de PSC si la configuración de Centro de partners cuenta está completa, independientemente de la cuenta que use para iniciar sesión en PSC.
- Compruebe si tiene acceso a Centro de partners y a la sección Referencias.
- Lea este documento para comprender los flujos de trabajo y los cambios en Centro de partners.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Como administrador en PSC, estos son los pasos siguientes

En el Centro de partners menú de navegación izquierdo, seleccione la **opción Referencias.** Confirme que puede acceder a las páginas Referencias.

  >[!Note]
  > Es posible que tenga que cerrar sesión Centro de partners iniciar sesión de nuevo para actualizar las credenciales de acceso a las páginas de referencias.

Si no ve la opción Referencias en el menú Centro de partners o en las páginas relacionadas [](permissions-overview.md) con referencias, póngase en contacto  con el administrador de la cuenta de su empresa y pídale que le dé acceso a la opción Referencias y al área relacionada. 

Para buscar el administrador de la cuenta de la empresa:

1. Seleccione **Configuración de la** cuenta en el icono de engranaje situado en la parte superior derecha del Centro de partners panel.

1. Seleccione **Administración de usuarios** en el menú de navegación izquierdo del segundo nivel.

1. En la parte superior de la lista de usuarios, seleccione **el** menú desplegable Filtro. Cambie la opción a Administrador **de cuenta.**

   La página mostrará todos los administradores de cuenta con sus respectivas direcciones de correo electrónico. Envíe un correo electrónico a uno de ellos y pídale que asigne el rol de administrador de referencias para su cuenta de trabajo.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="Imagen que muestra los administradores de cuenta en la página de administración de usuarios de configuración de asociados.":::

>[!Important]
>- Si el rol solo implica la administración de usuarios en PSC, pida al administrador de la cuenta de su empresa que le asigne el rol de administrador de cuenta en Centro de partners. [](permissions-overview.md#manage-mpn-membership-and-your-company) 
>- Si su rol también incluye la administración de oportunidades de venta en colaboración, pida que se le asigne el rol [de administrador de referencias.](permissions-overview.md#manage-referrals)
> - Es una buena idea designar también un cliente potencial de administración de cambios entre los administradores de PSC. Si lo hace, impedirá que todos los administradores de PSC tengan que comunicarse individualmente con Centro de partners administradores de cuentas. En su lugar, el responsable de administración de cambios puede ser la persona principal que trabaja con el administrador Centro de partners cuenta.

## <a name="user-migration"></a>Migración de usuarios

Después de configurar la cuenta en Centro de partners, use el Asistente para migración de usuarios en la página oportunidades de venta conjunto para asignar automáticamente roles de Centro de partners a los empleados de su empresa.

>[!Note]
> La migración de usuarios solo la pueden realizar [los administradores de cuentas](permissions-overview.md#manage-mpn-membership-and-your-company) de su empresa. Si no tiene el rol de administrador de cuenta, busque un administrador de cuenta que pueda ayudar a configurar las cuentas de usuario con la ayuda del Asistente para migración de usuarios.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Imagen que muestra el Asistente para migración de usuarios.":::

Los administradores de cuentas verán un vínculo del Asistente para migración de usuarios de PSC en la página oportunidades de venta en colaboración junto a la guía de referencias. Puede iniciar la migración del usuario seleccionando el vínculo. Para iniciar la migración de usuarios, los administradores pueden seleccionar el vínculo. Pueden realizar este paso de migración de usuarios varias veces hasta que a todos los usuarios se les asignen roles adecuados en Centro de partners.

La tabla de migración de usuarios tiene los detalles siguientes:

- Cuenta de usuario: identificador de correo electrónico del empleado
- Cuenta de asociado de PSC: la cuenta a la que está asociado el empleado en PSC
- Rol de usuario de PSC: uno de los tres roles asignados a en PSC.
- Ubicación de MPN de PC: la ubicación para la que se le darán roles de Centro de partners (PC) pertinentes al usuario. El MPN de la cuenta de asociado de PSC se usa para buscar la ubicación de MPN equivalente Centro de partners asignar permisos. Toda la organización denota el identificador de MPN de vOrg.
- Rol de usuario de PC: a los empleados se les asignan roles en función de sus roles de usuario de PSC. A los administradores de PSC se les asignarán roles de administrador de referencias Centro de partners. Al vendedor se le asignará el rol de usuario de referencias Centro de partners. Obtenga más información sobre los Centro de partners y lo que los usuarios con estos roles pueden hacer en Centro de partners [aquí](permissions-overview.md#manage-referrals)
- Inquilino de AAD de PC: el Microsoft Azure Active Directory (Azure AD) al que se asignan los usuarios en Centro de partners
- Estado: hay tres estados posibles para el estado de la migración.
    - **No migrado:** el usuario no tiene asignado ningún rol Centro de partners referencias
    - **Migrado:** el usuario se ha migrado correctamente con el rol pertinente asignado, como se muestra en la tabla.
    - **Error:** no se puede completar la migración debido a algún error

A veces, la migración puede producir errores y producir errores. Estas son algunas de las razones por las que una migración puede provocar un error y algunas de las formas de resolver el problema:

1. Es posible que los usuarios de PSC usen una cuenta que no sea de trabajo.

2. El usuario de PSC puede estar usando una cuenta de un dominio diferente de la que se usa en Centro de partners.

   Para resolver errores relacionados con los escenarios 1 y 2, pida al usuario que inicie sesión en Centro de partners con su cuenta de trabajo asociada a su Azure AD inquilino. El [administrador global](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) puede ayudarle.
   
   Para buscar el administrador global: 
   - Inicie sesión en Centro de partners [panel y](https://partner.microsoft.com/dashboard) seleccione Configuración de **la cuenta** en el icono de engranaje de la parte superior derecha.
   - Seleccione **Administración de usuarios** en la barra de navegación izquierda del segundo nivel.
   - En la parte superior de  la lista de usuarios, seleccione el menú desplegable Filtro y cambie la opción a **Administrador global.** A continuación, la página muestra todos los administradores globales con sus respectivas direcciones de correo electrónico. Pida a uno de ellos que asigne el rol de administrador de referencias para su cuenta de trabajo.
   
      El administrador global puede crear una nueva cuenta de usuario en el inquilino de Azure AD o asignar acceso de usuario invitado a los demás usuarios de la cuenta de dominio. Una vez **configuradas** las cuentas para todos los administradores de contratos y usuarios de PSC, deben iniciar sesión en Centro de partners, seleccionar Referencias en el menú de navegación izquierdo y confirmar que pueden ver la página Referencias.

3. El usuario ya tiene asignado un rol de referencia en Centro de partners.
    - Puede comprobar el rol existente del usuario. En la esquina superior derecha de la Centro de partners, seleccione **Configuración** (el icono de engranaje) y, a continuación, **Configuración de la cuenta.** Cuando vea un segundo menú de navegación izquierdo, seleccione **Administración de usuarios** y busque el usuario.

## <a name="psc-deals-migration"></a>Migración de PSC Deals

Una vez completada la migración de usuarios, use el Asistente para migración de ofertas en la página de oportunidades de venta en colaboración para llevar todas las ofertas abiertas aptas de PSC a Centro de partners. **El vínculo de migración de ofertas solo será visible para los administradores de referencias con todo el ámbito de la organización Centro de partners.** Habrá un vínculo denominado "Migración de contratos **PSC"** en la parte superior derecha de la página Oportunidades de venta masiva, que abrirá el Asistente para migración de contratos.

Lea esta sección antes de iniciar la migración de la oferta.

**Apto para la migración**

Solo algunas ofertas son aptas para la migración de PSC a Centro de partners. Este asistente para migración se ha creado para ayudar a los asociados a llevar sus ofertas a Centro de partners donde siguen trabajando activamente con sus clientes para cerrar el acuerdo. **Solo las ofertas que están en estado abierto creadas a partir del 1 de enero de 2020 con detalles válidos de la cuenta de asociado (id. de MPN válido) y que no están en proceso de registro de la oferta son aptas para la migración.**

**No apto para la migración**

- Las ofertas de evaluación de soluciones no son aptas para la migración de ofertas
- Las ofertas empresariales de licencias de OEM no son aptas para la migración de ofertas
- Cualquier oferta que se haya marcado como ganada en PSC no es apta para la migración. El registro de la oferta si es apto para las ofertas marcadas como ganadas debe completarse en PSC.

## <a name="pre-requisites-for-deal-migration"></a>Requisitos previos para la migración de contratos

Antes de iniciar la migración de ofertas Centro de partners, siga las instrucciones siguientes para configurar las ofertas en PSC para una migración correcta.

1. Todos los miembros del equipo de ventas de su empresa que trabajan en las ofertas abiertas están informados sobre esta migración.
2. Los miembros del equipo de ventas están entrenados para usar Centro de partners administración de contratos.
3. Las ofertas tienen toda la información necesaria como se describe a continuación.
    - Detalles de la empresa del cliente, incluido el nombre y la dirección
    - Detalles de contacto del cliente si se trata de una oferta de venta en colaboración
    - Al menos una solución
    - Al menos un miembro del equipo con todos los detalles: nombre, apellidos, identificador de correo electrónico y número de teléfono
    - Valor de la oferta
    - Fecha de cierre de la oferta estimada
    - Notas del asociado

Puede usar las funcionalidades de carga y descarga masiva en PSC para agregar todos los detalles que faltan en la oferta para todas las ofertas aptas.

>[!Note]
> La migración de la oferta se realizará correctamente aunque no se cumplen los requisitos previos anteriores. Sin embargo, no puede cambiar el estado de la oferta si alguno de los campos obligatorios mencionados anteriormente Centro de partners no están disponibles. A continuación, tendrá que escribir toda la información necesaria que falta en las ofertas de Centro de partners para empezar a trabajar en ellas. **Se recomienda encarecidamente limpiar las ofertas aptas en PSC antes de migrarlas a Centro de partners.**

La migración de la oferta Centro de partners se ha creado como una experiencia con un solo clic. Todo lo que necesita hacer es seleccionar el botón **"Migrar ofertas"** una vez que la empresa esté lista para migrar las ofertas aptas. **No puede elegir las ofertas que desea migrar desde PSC. Si no desea migrar ninguna de las ofertas a Centro de partners, muévenlas al estado cerrado en PSC antes de iniciar la migración.**

>[!Note]
> Después de iniciar la migración, las ofertas pueden tardar hasta **24 horas en migrarse.**

Una vez completada la migración, el mensaje del banner tendrá el estado cambiado para completarse con un vínculo al informe de migración. Descargue el informe para ver los detalles de las ofertas que se migraron de PSC a Centro de partners.

El informe incluye los detalles siguientes.

1. **Centro de partners de interacción:** identificador único de Centro de partners para todas las ofertas de una interacción. Hay dos ofertas: una para el asociado y otra para Microsoft en una interacción de venta Centro de partners.
2. **Centro de partners de referencia:** identificador único de Centro de partners para la oferta que pertenece al asociado.
3. **Nombre de la** oferta: identificador dado a la oferta en PSC.
4. **Id. de oferta de PSC:** identificador único de PSC para la oferta.
5. **Errores:** para indicar si hay algún error al migrar una oferta específica.

Todas las ofertas que se hayan migrado correctamente no estarán visibles en PSC. Puede seguir trabajando en las ofertas migradas en Centro de partners incluida la finalización del registro de ofertas en Centro de partners. No habrá ningún cambio en las interacciones con los vendedores de Microsoft para las ofertas de venta coventa.

Las ofertas migradas desde PSC estarán disponibles en las pestañas Entrante y Saliente en función del origen de la oferta. Todas las ofertas compartidas por su empresa estarán disponibles en la pestaña Salida y las ofertas iniciadas por Microsoft estarán disponibles en la pestaña Entrada de Centro de partners. Habrá dos tipos de ofertas que se crearán después de la migración.

1. **Ofertas de venta** co-venta: las ofertas que están marcadas como venta en colaboración en PSC se crearán como ofertas de venta Centro de partners.
2. **Ofertas dirigidas por** asociados: las ofertas que no están marcadas como venta en colaboración se crearán como ofertas dirigidas por asociados en Centro de partners. Las ofertas dirigidas por asociados son visibles para los vendedores de Microsoft y se pueden actualizar a ofertas de venta coventa antes de alcanzar el estado terminal (ganado, perdido). Además, las ofertas dirigidas por asociados son aptas para el registro de ofertas si hay una solución apta para incentivos en la oferta.

>[!Important]
> Si hay errores debidos a los cuales no se pudieron migrar algunas ofertas, puede volver a iniciar la migración de la oferta haciendo clic en el botón **"Migrar ofertas".** Solo se habilitará si todavía hay algunas ofertas aptas que se deben migrar. Esto también será útil si se encuentra en la fase de transición en la que se crean nuevas ofertas en PSC después de iniciar la migración de ofertas.

Una vez que todas las ofertas se migren correctamente, aparecerá un banner que muestra **"No hay** ofertas para migrar" con el botón **"Migrar ofertas"** **que** se deshabilita.

Después de completar la migración de usuarios o la migración de la oferta, use las instrucciones siguientes para decidir la estrategia de migración:

Si su empresa tiene un administrador de desarrollo de partners (CARGO): cuando se configura la cuenta de Centro de partners y los usuarios se han movido y tienen roles y permisos, puede mover las actividades de venta Centro de partners. Informe al ARCHIVO DE SEGURIDAD para que realice el cambio en lugar de esperar hasta que se complete la fecha límite de la migración, lo que permitirá que todas las nuevas ofertas fluyan a Centro de partners.

>[!Note]
>Una vez que haya realizado este cambio, solo podrá actuar sobre las ofertas activas existentes en PSC. No puede crear nuevas ofertas ni recibir ofertas de vendedores de Microsoft en PSC.

Si su empresa no tiene un VALOR DEC: asegúrese de que todos los usuarios configuren y comprueben todas las cuentas de usuario. Se le notificará a través de un correo electrónico y un banner en PSC con respecto a la fecha exacta en la que puede iniciar la venta Centro de partners. Recuerde que todavía tendrá que administrar las ofertas activas existentes en PSC.

>[!Important]
> Tiene hasta el 30 de abril de 2021 para registrar las ofertas marcadas como ganadas.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Pasos siguientes para administradores de PSC, administradores de contratos de PSC y vendedores de PSC

Obtenga información sobre cómo vender de forma Centro de partners.
Este es un paso importante, que le ayudará a prepararse para la venta Centro de partners. Comprenda los flujos de trabajo y los cambios en Centro de partners para que pueda realizar la venta de forma efectiva de inmediato. Empiece por leer este documento por completo. También hay disponible un buen conjunto de recursos en la galería [de experiencia de venta co-sell](https://aka.ms/cosellexperience).

## <a name="major-differences-between-psc-and-partner-center-workflows"></a>Principales diferencias entre psc y flujos Centro de partners trabajo

|**Escenario**|**Partner Sales Connect**|**Centro de partners**|
|-----|:-----|:-----|
|Roles de usuario|PSC tiene roles de administrador, administrador de contratos y vendedor.|Centro de partners solo tiene un [rol de administrador de](permissions-overview.md#manage-referrals) referencias que concede permiso de lectura y escritura para todas las ofertas.|
|Invitación a Microsoft en una oferta de venta co-venta|Iniciado por el vendedor de Microsoft, no hay ninguna pregunta explícita por parte del asociado.|El partner tendrá que realizar una [solicitud explícita si](manage-co-sell-opportunities.md#add-solutions) se necesita ayuda del vendedor de Microsoft para un contrato. El vendedor de Microsoft tiene la opción de rechazar la solicitud.|
|Expiry|No hay ningún concepto de expiración de una oferta.|Las ofertas entrantes de asociado expiran en 14 días si el asociado no las acepta. Lo mismo sucede con las ofertas salientes de asociados en las que pueden pasar a un estado expirado si el vendedor de Microsoft no actúa en ellos en 14 días.|
|Detalles del vendedor de Microsoft|Visible en cuanto se crea una oferta.|Los detalles del vendedor de Microsoft se comparten con el partner solo si el vendedor acepta explícitamente la invitación para la venta compartida del partner.|
|[Canalización privada](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|No disponible.|Los asociados pueden compartir su canalización sin dar visibilidad a los vendedores de Microsoft.|
|Soluciones|Las soluciones que pertenecen a una sola lista de precios se pueden agregar a una oferta.|El asociado puede [agregar soluciones](manage-co-sell-opportunities.md#add-solutions) que pertenezcan a las listas siguientes. a) Sus propias soluciones b) Soluciones del catálogo de microsoft propio (similar al rol de transacción de transacción en PSC) y c) Soluciones de venta co-venta de otros asociados de terceros (similar al rol Desaprobaciones de ISV en PSC).|
|Asignación de contratos|Solo los vendedores asignados pueden ver y actuar sobre las ofertas.|Los miembros del equipo se pueden agregar a un acuerdo para especificar las personas que trabajan en un acuerdo; no hay ningún bloqueo para que otros administradores de referencias puedan ver esas ofertas o actuar sobre ellas.|
|Organización del cliente|Entrada de texto de forma libre.|Puede buscar la organización [del cliente en](manage-co-sell-opportunities.md#select-your-customer) la base de datos D&[B](https://www.dnb.com/) escribiendo solo unos caracteres. El nombre legal y la dirección se rellenan automáticamente en función de la elección.|
|Contacto del cliente|No es obligatorio.|No es obligatorio para el uso compartido de canalizaciones privadas. Obligatorio si se invita al vendedor de Microsoft a participar en una solicitud de venta coventa.|
|API pública|No disponible.|[API pública](/partner/develop/referrals) para administrar mediante programación Centro de partners referencias.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>Asigne los campos de PSC a los campos correspondientes de Centro de partners

En esta sección se comparan (o "mapas") las capturas de pantalla seleccionadas que se muestran para PSC con la vista correspondiente de la Centro de partners oportunidades de venta conjunto.

Verá círculos numerados, amarillos o rojos en cada par de capturas de pantalla:

- **¿Qué significan los círculos amarillos?** Los círculos amarillos numerados aparecen primero en cada captura de pantalla de PSC. A continuación, encontrará un Centro de partners captura de pantalla debajo de él con muchos de los mismos números.

   Para ver cómo cada campo o atributo de PSC se asigna a su homólogo de Centro de partners, haga coincidir los círculos numerados en las dos capturas de pantalla relacionadas. Por ejemplo, haga coincidir el "1" de color amarillo numerado de la primera captura de pantalla de PSC con el "1" numerado y amarillo en el segundo, Centro de partners captura de pantalla debajo.

- **¿Qué significa un círculo rojo?** Si ve un círculo rojo en una captura de pantalla, eso indica que el campo PSC no está disponible en Centro de partners.

Las asignaciones de campos de psc a Centro de partners se muestran para las áreas siguientes:

1. Página principal de PSC asignada a la Centro de partners predeterminada de oportunidades de venta
1. Vista de cuadrícula de PSC asignada a la Centro de partners de la oferta
1. Vista de detalles de la oferta de PSC asignada a la Centro de partners detalles de la oferta
1. Vista Agregar productos de PSC asignada a la Centro de partners Agregar soluciones
1. Vista de administración de usuarios de PSC asignada a la Centro de partners de administración de usuarios
1. Vista de asignación de roles de usuario de PSC asignada a la Centro de partners asignación de roles
1. Vista de notificaciones de PSC asignada a la Centro de partners de notificaciones

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1 - Página principal de PSC asignada a la Centro de partners predeterminada de oportunidades de venta

Compare los círculos numerados y de coincidencia entre la captura de pantalla de PSC superior y Centro de partners captura de pantalla que hay debajo. Los números correspondientes muestran dónde puede encontrar la característica o el atributo relacionados con PSC en Centro de partners. Los círculos rojos indican que no hay ningún campo Centro de partners coincidencia.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Imagen que muestra las asignaciones de campos entre la página principal de Partner Sales Connect y la vista predeterminada de las oportunidades de venta Centro de partners." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 - Vista de cuadrícula de PSC asignada a la Centro de partners de la oferta

Compare los círculos numerados y de coincidencia entre la captura de pantalla de PSC superior y Centro de partners captura de pantalla que hay debajo. Los números correspondientes muestran dónde puede encontrar la característica o el atributo relacionados con PSC en Centro de partners. Los círculos rojos indican que no hay ningún campo Centro de partners coincidencia.  

> [!NOTE]
> Otras consideraciones aparecen debajo de las capturas de pantalla.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Imagen que muestra las asignaciones de campos entre la vista de cuadrícula Partner Sales Connect (PSC) y la Centro de partners de la oferta." lightbox="images/pscmigration/grid-view-expanded.png":::

**Consideraciones especiales:**

- No hay ninguna vista de lista en Centro de partners como la de PSC.  Todas las ofertas se enumeran en función de la fecha más reciente recibida o creada con la información del cliente y el tipo de la oferta. La primera oferta de la vista está seleccionada de forma predeterminada. La mayoría de los valores que se muestran en el formato de tabla PSC están disponibles en la vista de detalles de la oferta en Centro de partners.
- El rol de oferta no es un campo obligatorio en Centro de partners. No se muestra ni captura en ninguno de los flujos de trabajo. Se deriva automáticamente en el lado del vendedor de Microsoft en función de las soluciones agregadas a la oferta.
- La fecha de última modificación no se muestra en la página de detalles de referencia de Centro de partners. Los asociados pueden usar la funcionalidad de ordenación para ordenar las ofertas en función de la fecha de última actualización.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3 - Vista de detalles de la oferta de PSC asignada a Centro de partners

Compare los círculos numerados y de coincidencia de la parte superior (PSC) con la Centro de partners siguiente. Los números correspondientes muestran dónde puede encontrar la característica o el atributo relacionados con PSC en Centro de partners. Los círculos rojos indican que no hay ningún campo o área que coincida en Centro de partners.

> [!NOTE]
> Otras consideraciones aparecen debajo de las capturas de pantalla.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Imagen que muestra las asignaciones de campos entre la vista de detalles de la oferta de Partner Sales Connect (PSC) y la Centro de partners detalles de la oferta." lightbox="images/pscmigration/deal-details-expanded.png":::

**Consideraciones especiales:**

- Los partners pueden editar una oferta seleccionando el botón Editar en la vista de detalles de la oferta del asociado (6). Una vez seleccionado el botón Editar, todos los campos se podrán editar. A continuación, tiene la opción de guardar o cancelar las modificaciones realizadas en la oferta.
- No hay ninguna opción para cerrar la oferta como duplicada en Centro de partners.
- El resultado del cliente no está disponible en Centro de partners. Todos los detalles relacionados con las interacciones de los clientes se pueden actualizar en la sección Notas de Centro de partners.
- La fecha de cierre de la solución estimada solo está disponible para las ofertas de IOT de OEM Centro de partners. Esta información no se muestra para ningún otro tipo de oferta.
- El programa de licencias no es necesario en Centro de partners. Esta información se deduce automáticamente en función de las soluciones seleccionadas en la oferta.

>[!Note]
>Cualquier oferta marcada como ganada o perdida no se puede editar posteriormente. Tenga cuidado al mover una oferta a uno de estos estados terminales.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4 - Vista "Agregar productos" de PSC asignada a la Centro de partners "Agregar soluciones"

Compare los círculos numerados y de coincidencia de la parte superior (PSC) con la Centro de partners siguiente. Los números correspondientes muestran dónde puede encontrar la característica o el atributo relacionados con PSC en Centro de partners. Los círculos rojos indican que no hay ningún campo o área que coincida en Centro de partners.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Imagen que muestra las asignaciones de campos entre la vista agregar productos de Partner Sales Connect (PSC) y la Centro de partners agregar soluciones." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5 - Administración de usuarios en PSC frente a Centro de partners

Compare los círculos numerados y de coincidencia de la parte superior (PSC) con la Centro de partners siguiente. Los números correspondientes muestran dónde puede encontrar la característica o el atributo relacionados con PSC en Centro de partners. Los círculos rojos indican que no hay ningún campo o área que coincida en Centro de partners.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Imagen en la que se muestran las asignaciones de campos entre la página principal de administración de usuarios de Partner Sales Connect (PSC) y la Centro de partners de la página Administración de usuarios en el área Configuración de la cuenta."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6 - Asignación de roles de usuario en PSC frente a Centro de partners

Compare los círculos numerados y de coincidencia de la parte superior (PSC) con la Centro de partners siguiente. Los números correspondientes muestran dónde puede encontrar la característica o el atributo relacionados con PSC en Centro de partners. Los círculos rojos indican que no hay ningún campo o área que coincida en Centro de partners.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Imagen que muestra las asignaciones de campos entre la vista de asignación de roles de Partner Sales Connect (PSC) y la Centro de partners asignación de roles." lightbox="images/pscmigration/roles-expanded.png":::

**Consideraciones especiales:**

- El rol equivalente para el administrador de PSC es el rol de administrador de cuenta Centro de partners.
- Solo hay un rol en el Centro de partners administración de contratos de venta co-venta. Este rol es el rol de administrador de referencias.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 - Notificaciones en PSC frente a Centro de partners

Compare los círculos numerados y de coincidencia de la parte superior (PSC) con la Centro de partners siguiente. Los números correspondientes muestran dónde puede encontrar la característica o el atributo relacionados con PSC en Centro de partners. Los círculos rojos indican que no hay ningún campo o área que coincida en Centro de partners.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Imagen que muestra la asignación entre las notificaciones de Partner Sales Connect (PSC) y la Centro de partners de notificaciones."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Traslado de PSC a Centro de partners: preguntas más frecuentes

En las secciones siguientes se responden preguntas frecuentes sobre la migración.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1 - ¿Qué debo hacer si no tengo acceso a Centro de partners?

Puede ponerse en contacto con los administradores que aparecen en la página "Sin acceso" para obtener los roles asignados. Necesitará el rol de [administrador de referencias](permissions-overview.md#manage-referrals) para el permiso de lectura y escritura en la sección de referencias. Si solo administra perfiles de negocio, necesitará el rol de administrador de perfiles de negocio en el Centro de partners.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Imagen que muestra la experiencia sin acceso en Centro de partners.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2 - ¿Quién puede concederme acceso a la sección Referencias de Centro de partners?

El [administrador de la](permissions-overview.md#manage-mpn-membership-and-your-company) cuenta puede concederle acceso a la pestaña Referencias. Para buscar el administrador de la cuenta, seleccione **Configuración de la** cuenta en el icono de engranaje situado en la parte superior derecha de la Centro de partners [panel](https://partner.microsoft.com/dashboard). A continuación, **seleccione Administración de** usuarios en la barra de navegación izquierda de segundo nivel. En la parte superior de  la lista de usuarios, seleccione el menú desplegable Filtro y cambie la opción a **administrador de la cuenta.** La página mostrará todos los administradores de cuenta con sus respectivas direcciones de correo electrónico. Pida a uno de ellos que asigne el rol de administrador de referencias para su cuenta de trabajo.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3 - El botón +new deal (+nueva oferta) está en gris para nuestra cuenta. ¿Qué debo hacer para empezar a crear ofertas?

Esto solo ocurre si no hay soluciones preparadas para venta co-sell asociadas a la organización de MPN que se usan en Centro de partners. Póngase en contacto con el ADMINISTRADOR de servicios de seguridad para obtener el identificador de MPN de las soluciones corregido o cree una vale de soporte técnico que mencione el problema: "Botón Nueva oferta en gris después de la migración de PSC".

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 - ¿Puedo asignar ofertas a una persona específica de nuestra organización como PSC?

Puede asignar miembros del equipo a una oferta específica. No bloquea que otros administradores de referencias vea o actúe en esas ofertas.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 - ¿Hay una vista de todas las ofertas que me han asignado?

Puede usar la característica favoritos, que es una pestaña de nivel de usuario. Puede marcar todas las ofertas que se le asignan como favoritas para obtener un acceso rápido a las ofertas.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 - ¿Hay una vista de solo lectura para las ofertas?

No, no hay ninguna vista de solo lectura de las ofertas en la sección de referencias. Todos los administradores de referencias tendrán acceso completo de lectura y escritura a todas las ofertas.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 - ¿Cómo puedo registrar una oferta después de marcarla como ganada?

Si la oferta cumple los criterios siguientes, se mostrará un menú emergente para iniciar el [registro de la oferta.](./register-deals.md)

- Hay una solución apta para incentivos asociada a la oferta.
- El vendedor de Microsoft está invitado a participar en la oferta o le ha invitado a la oferta.
- La tarjeta de Microsoft está en los estados Aceptado o Ganado en Centro de partners.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8 - Aparece un mensaje de error al seleccionar el botón "+New deal registration" (+Nuevo registro de oferta) en la sección Registro de la oferta. ¿Cómo puedo registrar mis ofertas?

El **botón +New deal registration** (+Nuevo registro de oferta) solo lo van a usar los asociados que están registrados en el programa de conexión de ISV para registrar una oferta sin ninguna oportunidad de venta Centro de partners. Para registrar ofertas con una oportunidad de venta en colaboración, se mostrará una ventana emergente cuando la oferta se marque como ganada y si cumple los criterios para el registro de la oferta.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 - ¿Es obligatorio agregar una organización de clientes?

Sí, es obligatorio [agregar una organización](./manage-co-sell-opportunities.md#select-your-customer) de clientes en Centro de partners. En primer lugar, busque la ubicación donde se encuentra el cliente. En función de los detalles que tenga; puede ser específico, incluido el nombre exacto del edificio o simplemente proporcionar detalles de la ciudad. La búsqueda de la organización capturará todas las entidades legales que coincidan con el nombre que escriba para que no tenga que escribir ningún detalle de dirección. Todos los detalles se rellenan automáticamente en función de la organización seleccionada.

### <a name="10---are-customer-contact-details-mandatory"></a>10 - ¿Son obligatorios los detalles de contacto del cliente?

Depende del [tipo de oferta](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) que cree. Si solo comparte la canalización y no necesita ayuda de la organización de ventas de Microsoft, puede optar por no proporcionar los detalles de contacto del cliente. Si va a vender de forma co-venta donde busca activamente ayuda del vendedor de Microsoft, tendrá que proporcionar los detalles de contacto del cliente. Debe obtener el consentimiento explícito del cliente antes de crear una solicitud de venta co-sell en el Centro de partners.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11 - ¿Cuántas soluciones puedo agregar a un contrato?

Puede agregar hasta 50 soluciones (análogas a "productos" en PSC) a un acuerdo. A diferencia de PSC, puede combinar soluciones de sus propias soluciones aptas para la venta co-venta, SKU de Microsoft propias y otras soluciones aptas para venta co-venta de terceros. No hay ningún rol de oferta que se seleccione o esté disponible en el Centro de partners. En el caso de las SKU de Microsoft, opcionalmente puede agregar cantidad y precio para cada SKU que se agregue a la oferta.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12 - ¿Cuándo conoceré los detalles del vendedor de Microsoft después de crear un contrato?

Los vendedores de Microsoft solo se asignan después de que coincidan con el requisito de ayuda exacto indicado al crear el contrato con el rol de vendedor pertinente en el lado de Microsoft. Incluso después de la asignación, los vendedores de Microsoft tendrán la opción de aceptar o rechazar la invitación de venta coventa. Solo si un vendedor acepta una invitación de venta en colaboración, el contrato se actualizará con los detalles de contacto del vendedor de Microsoft. El Acuerdo de Nivel de Servicio para que los vendedores de Microsoft actúen sobre el acuerdo es de 14 días. Es el mismo Acuerdo de Nivel de Servicio que los asociados tienen que actuar sobre el acuerdo antes de que entre en estado expirado.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13 - ¿Dónde puedo encontrar el identificador de oportunidad?

El identificador de oportunidad en PSC es el mismo que el identificador de la oferta en Centro de partners. Puede encontrar el identificador de la oferta junto al nombre de la oferta al abrir cualquier oferta.

### <a name="14---how-can-my-pdm-get-access-to-partner-center"></a>14 - ¿Cómo puede obtener acceso mi ARCHIVO DE SEGURIDAD a Centro de partners?

Centro de partners los PDU no pueden acceder a ellos directamente a diferencia de PSC. Hay varias opciones para habilitar esa funcionalidad, que se mencionan a continuación.

- Información de OCP: si los PDU solo ven las ofertas y el progreso relacionados con ellos, pueden usar el portal de Información de one commercial partner (OCP) para obtener la vista de la organización. Se trata de una herramienta interna y solo está disponible para los PDM. La información de OCP no está disponible para los usuarios de la empresa.
- Usuario invitado en Centro de partners: puede agregar su cuenta de CARGO como usuario invitado en el Centro de partners y asignarle un rol de administrador de referencias para que pueda ver y actuar sobre las @microsoft.com referencias.
- Creación [](./create-user-accounts-and-set-permissions.md#add-a-new-user) de un nuevo usuario en el inquilino: puede crear un nuevo usuario en su propio inquilino y compartir esos detalles con el ARCHIVO DE SEGURIDAD para que pueda ver y actuar sobre referencias similares a las de otros usuarios de referencia de su cuenta.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>Búsqueda del identificador de MPN correcto si la cuenta de PSC no está asociada a un MPN válido

Si está aquí porque ha visto un banner en PSC que menciona "PsC invalid MPN ID association problem" (Problema de asociación de id. de MPN no válido de PSC), se encuentra en el lugar correcto. Es posible que la cuenta se haya vinculado a un identificador de MPN no válido debido a los siguientes motivos

- Su empresa no tiene una cuenta Centro de partners cliente.
- El ARCHIVO DE SEGURIDAD ha cometido un error al escribir el identificador de MPN de su cuenta en los sistemas internos que vinculan la cuenta de PSC a su cuenta de Centro de partners (id. de MPN).
- Su empresa no ha completado la migración de Partner Membership Center (PMC) a Centro de partners.

En primer lugar, busque el identificador de MPN correcto siguiendo los pasos siguientes.

- Inicie sesión en su cuenta Centro de partners cliente
- Use las instrucciones que se proporcionan en la documentación [de configuración de la cuenta](./partner-center-account-setup.md#locate-your-mpn-id) para buscar el identificador de MPN.

A continuación se muestra una captura de pantalla que muestra la ubicación exacta donde puede encontrar el identificador Centro de partners MPN.

:::image type="content" source="images/pscmigration/findingMPNID.png" alt-text="Imagen que muestra la configuración de la cuenta donde el asociado puede encontrar su identificador de MPN."  lightbox="images/pscmigration/findingMPNID.png":::

Después,

- Si tiene un ARCHIVO DE SEGURIDAD, pídales que se corrija el identificador de MPN con el identificador de MPN correcto de la cuenta del Centro de partners.
- Si no tiene un ARCHIVO POSTAL, envíe un correo electrónico a la dirección indicada en el banner de PSC con la información de la cuenta de PSC que se muestra en el banner de PSC y el identificador de MPN correcto de la cuenta del centro de partners.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Recursos que le ayudarán a crear y administrar sus ofertas en Centro de partners

Si aún no ha leído los temas de ayuda de venta en colaboración, los siguientes recursos le ayudarán a administrar las ofertas en el Centro de partners.

|**Para**   |**Lee esto**   |
|-----------------------|:-----------------------|
|Descripción de las pestañas y la navegación en la página de oportunidades de venta en colaboración|[Navegación por la sección de venta en colaboración](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|Selección de una organización de clientes en la lista D&B |[Selección del cliente](./manage-co-sell-opportunities.md#select-your-customer)|
|Modificación de los campos en la sección de detalles de la oferta|[Detalles de la oferta](./manage-co-sell-opportunities.md#deal-details)|
|Adición de miembros del equipo a un equipo de oferta|[Adición de los empleados](./manage-co-sell-opportunities.md#add-team-members)|
|Respuesta a una oferta de venta co-venta|[Administración de ofertas de venta en colaboración](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Registre las ofertas que ha ganado en Centro de partners |[Registrar una nueva oferta](./register-deals.md)
|Obtenga información de referencia y descubra cómo funcionan las referencias. |[Información de referencia](./referral-insights.md)
|Creación y administración de perfiles de negocio|[Administrar el perfil de negocio](./create-a-marketing-profile.md)
|Administración de clientes potenciales para el perfil de negocio |[Administrar los clientes potenciales](./manage-leads.md)|

## <a name="next-steps"></a>Pasos siguientes


- [Partner Sales Connect to Centro de partners workbook :libro](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) para alinear los procesos y roles de ventas de asociados con nuevos procesos de ventas a través de Centro de partners frente a Partner Sales Connect.
- [Centro de partners de operaciones](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) de venta en colaboración: guía para identificar un modelo operativo a través de Centro de partners para administrar clientes potenciales o oportunidades de venta en colaboración y registrar ofertas.
- [Presentación de administración de](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) referencias: se han visualizado instrucciones paso a paso para administrar clientes potenciales y oportunidades de venta Centro de partners.
- [Publicación y administración](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) en marketplace comercial: se han visualizado instrucciones paso a paso para crear, administrar y publicar ofertas a través de Centro de partners en el marketplace comercial.