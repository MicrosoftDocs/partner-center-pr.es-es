---
title: Asignación de roles y permisos a los usuarios
ms.topic: article
ms.date: 10/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtén información sobre qué roles son los más adecuados para los usuarios que administran las transacciones comerciales, las referencias, los incentivos o las suscripciones a MPN de tu empresa.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20, contperf-fy21q1
ms.openlocfilehash: b1ac34bbb92d600805465ca5f6d1b28af54cd5e1
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855138"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Asignación de roles y permisos a los usuarios de una empresa que necesitan trabajar en el Centro de partners

**Roles adecuados:** Administrador global | Administrador de usuarios | Administrador de partners de MPN

Has configurado tu perfil de partner, incluyendo el nombre y la dirección legales, los detalles de soporte técnico, las exenciones fiscales, la información bancaria y el contacto principal de tu empresa. Paso siguiente: configura tus usuarios con contraseñas y roles para que puedan comenzar a trabajar en el Centro de partners contigo.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configura a sus empleados para trabajar en el Centro de partners

Debes determinar los tipos de acceso que tendrán los usuarios en el Centro de partners, en función de los roles y permisos que les otorgues. Los roles están relacionados con los programas en los que participa tu empresa. Por ejemplo, si su empresa es un Proveedor de soluciones en la nube (CSP), no solo tendrá los roles estándar de administración de inquilinos de Azure Active Directory (como el administrador global), sino que también necesitarás roles específicos para el programa CSP. Recuerda que cada programa tiene roles específicos.

>[!Note]
> Los roles de inquilino de Azure Active Directory incluyen roles de administrador global, administrador de usuarios y CSP. Los roles que no son de Azure Active Directory son aquellos que no administran al inquilino, e incluyen un administrador de MPN, un administrador de perfil comercial, un administrador de referencias, un administrador de incentivos y un usuario de incentivos. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Administra las transacciones comerciales en el Centro de partners (roles de Azure AD y CSP)

|**Rol**|**Qué puede hacer**|**Más información**|
|----------------------------------|---|:---------------------------------|
|Administrador global|*    Obtener acceso a todos los servicios o cuentas de Microsoft con privilegios completos|[Administrar la cuenta del Centro de partners](partner-center-account-setup.md)
|      |*    Crear vales de soporte técnico para el Centro de partners
||*    Ver los vales de soporte técnico para partners que cree
||*    Ver contratos, listas de precios y ofertas
||*    Ver, crear y administrar usuarios asociados|
||  • Ver, crear y administrar los archivos de facturación, facturas y conciliación
|Administrador del control de usuarios   | *    Ver, crear y administrar usuarios|[Administración de las ventajas y ofertas de la suscripción a Microsoft Partner Network en el Centro de partners](manage-your-partner-network-benefits.md)
||*    Ver todos los perfiles de asociado
||*    Crear vales de soporte técnico para el Centro de partners
||*    Ver los vales de soporte técnico para partners que cree
|Administrador de facturación | • Ver, crear y administrar los archivos de facturación, facturas y conciliación|[Lectura de la factura](billing.md)
||*    Ver precios
||*    Crear vales de soporte técnico para el Centro de partners
||*    Ver los vales de soporte técnico para partners que cree
|Usuario predeterminado|  Ver mi perfil   |[Restablecimiento de la contraseña](reset-my-pasword.md)
|Agente de administrador | *    Administración de clientes|[Conectar con sus clientes](connect-with-your-customers.md)
||*    Agregar una lista de dispositivos en el Centro de partners
||*    Crear perfiles y aplicarlos a dispositivos
||*    Administración de suscripciones
||*    Comprobar el estado del servicio y las solicitudes de servicio para clientes
||*    Solicitar privilegios de administrador delegado
||*    Ver los precios y las ofertas
||*    Facturación
||*    Administrar contenido en nombre de un cliente
||*    Registrar un revendedor de valor agregado
||*    Crear vales de soporte técnico para el Centro de partners
||*    Ver los vales de soporte técnico para partners que cree|
|Agente de ventas | *    Administración de clientes|[Proporcionar soporte de facturación para sus clientes y ayudar a responder sus preguntas de facturación](provide-billing-support.md)
||*    Agregar una lista de dispositivos en el Centro de partners
||*    Administración de suscripciones
||*    Ver vales de soporte técnico
||*    Solicitar una relación con un cliente
||*    Ver los precios y las ofertas
||*    Administrar clientes potenciales
||*    Ver el contrato de cliente
||*    Registrar un vendedor de valor agregado
||*    Crear vales de soporte técnico para el Centro de partners
||*    Ver los vales de soporte técnico para partners que cree|
|Agente del departamento de soporte técnico| *    Buscar y ver un cliente|[Escalar los problemas a Microsoft y saber qué problemas son más adecuados para escalar a Microsoft.](escalate-problems-to-microsoft.md)
||*    Editar detalles del cliente
||*    Ayudar a resolver problemas del cliente referentes a la facturación o la administración de las suscripciones
||*    Solicitar soporte técnico en nombre de los clientes 
||*    Administrar los problemas de suscripción y facturación en nombre de los clientes
||*    Crear vales de soporte técnico para el Centro de partners
||*    Ver los vales de soporte técnico para partners que cree| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-azure-ad-role"></a>Proveedor del panel de control (CPV). (Rol de CSP y rol que no es de Azure AD)

Los CPV desarrollan aplicaciones para los partners del Proveedor de soluciones en la nube (CSP) y que así puedan integrar sus sistemas con las API del Centro de partners. 

|**Rol**   |**Qué puede hacer**|**Más información**|
|------------------------------|:----------------------------|----|
|Administrador global| Ver y administrar el perfil de CPV|[Inscribirse como proveedor de panel de control para facilitar la integración de sistemas de partners de CSP con las API del Centro de partners](enroll-as-cpv.md)
||Ver y administrar los usuarios que necesiten acceso a las funcionalidades de CPV|

### <a name="guest-user-must-be-added-to-the-azure-active-directory-tenant"></a>Usuario invitado (debe agregarse al inquilino de Azure Active Directory)

|**Usuario invitado**   | **Roles**|
|---------------------------|:--------------------|
||Administrador de partners de MPN|
||Administrador del perfil de negocio|
||Administrador de referencias|


## <a name="manage-mpn-membership-and-your-company"></a>Administración de la pertenencia a MPN y su empresa 

Estos no son roles de Azure Active Directory. Estos roles administran el negocio de la empresa en lugar del inquilino.

|**Rol** | **Qué puede hacer**|**Más información**|
|----------------------------|:----------------------------|-----|
|Administrador de partners de MPN|*    Ver, crear y administrar las solicitudes de servicio de los asociados|[Compra o renueva una suscripción a Microsoft Action Pack o las competencias Silver o Gold.](mpn-get-action-pack.md)
||*    Ver perfiles legales, de negocios, empresariales y de MPN
||*    Ver los detalles de los usuarios y sus datos de aptitudes
||*    Ver competencias
||*    Ver y administrar ventajas
||*    Ver y adquirir ofertas de MPN
||*    Ver las facturas y el historial de pedidos de ofertas de MPN
||*    Ver datos de los indicadores de contribución de asociados
||*    Usar la herramienta de validación de cupones|
||*     Ver análisis de datos de clientes
||*    Ver otros roles de usuario dentro de la empresa, pero no puede asignar roles
||*    Crear vales de soporte técnico para el Centro de partners
||*    Ver los vales de soporte técnico para partners que cree
|Administrador de cuentas| • Agregar ubicaciones|[Administrar ubicaciones](manage-locations.md)
|| • Administrar perfiles relacionados con las cuentas para las que es administrador 
||*    Asignar roles para los usuarios en el inquilino a roles que no son de Azure Active Directory 
||*    Inscribir ubicaciones en programas
||*    Crear vales de soporte técnico para el Centro de partners
||*    Ver los vales de soporte técnico para partners que cree

## <a name="manage-referrals"></a>Administrar referencias

|**Rol** | **Qué puede hacer**|**Más información**
|------------------------------|:-------------------------|---|
|Administrador de referencias|Crear y administrar todo el contenido de la pestaña Referencias del Centro de partners|[Administrar oportunidades de venta conjunta en el Centro de partners para definir acuerdos y satisfacer mejor las necesidades de los clientes](manage-co-sell-opportunities.md)
||    Puede ver y editar todos los clientes potenciales y oportunidades de venta conjunta
||    Puede asignar miembros del equipo para una oferta
||    Puede ver y editar perfiles de negocio
||    Puede ver y registrar ofertas de oportunidades que se han marcado como ganadas y aptas para registrar la oferta
||    Puede crear y ver incidencias de soporte técnico
|Usuario de Referencias|Crear y administrar oportunidades de venta conjunta solo si forman parte del equipo |[Administrar oportunidades de venta conjunta en el Centro de partners para definir acuerdos y satisfacer mejor las necesidades de los clientes](manage-co-sell-opportunities.md)
||    Puede crear oportunidades de venta conjunta para las ubicaciones en las que se les ha asignado el rol
||    Puede ver y registrar ofertas para las oportunidades que se han marcado como ganadas y aptas para registrar la oferta si son miembros del equipo
||    Puede crear y ver incidencias de soporte técnico
|Administrador del perfil de negocio|Crear y administrar perfiles de negocio | [Administrar perfiles de negocio](create-a-marketing-profile.md)
||    Puede crear y ver incidencias de soporte técnico

Junto con el nuevo rol de usuario Referencias, también se introduce el ámbito de ubicación para las ofertas. En la tabla siguiente se explica el acceso a las ofertas basado en la ubicación.

|**Scope** | **Qué puede hacer** |
|------------------------------|:-------------------------|
|Toda la compañía | Tanto los administradores como los usuarios tienen acceso para crear ofertas para cualquier ubicación de su compañía|
|| El administrador de referencias tiene acceso para ver y editar todas las ofertas |
|| Los usuarios de referencias tienen acceso para ver y editar todas las ofertas solo si forman parte del equipo |
|Una o varias ubicaciones | Tanto los administradores como los usuarios tienen acceso para crear ofertas para la ubicación asignada en su compañía|
|| El administrador de referencias tiene acceso para ver y editar todas las ofertas que pertenecen a las ubicaciones asignadas|
|| Los usuarios de referencias tienen acceso para ver y editar todas las ofertas que pertenecen a las ubicaciones asignadas si forman parte del equipo|

## <a name="manage-incentives"></a>Administrar incentivos

|**Rol** | **Qué puede hacer**|**Más información**
|------------------------------|:-------------------------|---|
|Administrador de incentivos|*    Iniciar y administrar incentivos |[Usar estos recursos para ayudarle a empezar a trabajar con incentivos](incentives-get-started-intro.md)
||*    Ver y editar todos los aspectos de los programas de incentivos
||*    Ver y editar información bancaria y fiscal
||*    Ver ganancias de devolución y cooperación
||*    Acceder a soporte técnico
||*    Disputar pagos de incentivos|
|Usuario de incentivos|*    Ver programas de incentivos
||*    Ver e iniciar reclamaciones de incentivos
||*    Ver ganancias de devolución y cooperación
||*    Crear vales de soporte técnico para el Centro de partners
||*    Ver los vales de soporte técnico para partners que cree

## <a name="view-partner-center-insights-data"></a>Ver datos de conclusiones del Centro de partners

|**Rol** | **Qué puede hacer**|**Más información**|
|------------------------------|:-------------------------|---|
|Visor de informes ejecutivos|Acceder a todos los conjuntos de datos de informes, crear vales de soporte para partners, ver los vales de soporte técnico para partners que cree|[Revisar los informes del panel disponibles en la Información acerca del Centro de partners](pci-overview-report.md)
|Visor de informes|Acceder a los informes de datos, con excepción de los ingresos y de los datos personales de clientes y empleados, crear vales de soporte para partners, ver los vales de soporte técnico para partners que cree|

## <a name="next-steps"></a>Pasos siguientes

- [Creación de cuentas de usuario y asignación de roles y permisos](create-user-accounts-and-set-permissions.md)
- [Comprobación de la información de la cuenta al inscribirse en un nuevo programa del Centro de partners](verification-responses.md)
