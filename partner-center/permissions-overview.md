---
title: Asignación de roles y permisos a los usuarios
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtén información sobre qué roles son los más adecuados para los usuarios que administran las transacciones comerciales, las referencias, los incentivos o las suscripciones a MPN de tu empresa.
author: hemas
ms.author: hemas
keywords: roles, permisos, administrador, agente
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 4f4ec3a1a14e6845f7b6079e286876d9bb1f3dd5
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/03/2020
ms.locfileid: "85948599"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a>Asignación de roles y permisos a los usuarios de una empresa que necesitan trabajar en el Centro de partners

**Roles adecuados**

- Administrador global
- Administrador de usuarios
- Administrador de partners de MPN

Has configurado tu perfil de partner, incluyendo el nombre y la dirección legales, los detalles de soporte técnico, las exenciones fiscales, la información bancaria y el contacto principal de tu empresa. Paso siguiente: configura tus usuarios con contraseñas y roles para que puedan comenzar a trabajar en el Centro de partners contigo.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configura a sus empleados para trabajar en el Centro de partners

Debes determinar los tipos de acceso que tendrán los usuarios en el Centro de partners, en función de los roles y permisos que les otorgues. Los roles están relacionados con los programas en los que participa tu empresa. Por ejemplo, si tu negocio es un Proveedor de soluciones en la nube (CSP), no solo tendrás los roles estándar de administración de inquilinos de Azure AD (como el administrador global), sino que también necesitarás roles específicos para el programa de CSP. Recuerda que cada programa tiene roles específicos.

>[!Note]
> Los roles de inquilino de Azure Active Directory (AAD) incluyen roles de administrador global, administrador de usuarios y CSP. Los roles que no son de AAD son aquellos que no administran al inquilino, e incluyen un administrador de MPN, un administrador de perfil comercial, un administrador de referencias, un administrador de incentivos y un usuario de incentivos. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Administra las transacciones comerciales en el Centro de partners (roles de Azure AD y CSP)

|**Rol**|**Qué puede hacer**|
|----------------------------------|:---------------------------------|
|Administrador global|*    Obtener acceso a todos los servicios o cuentas de Microsoft con privilegios completos
|      |*    Crear vales de soporte técnico para el Centro de partners
||*    Ver contratos, listas de precios y ofertas
||*    Ver, crear y administrar usuarios asociados|
||  • Ver, crear y administrar los archivos de facturación, facturas y conciliación
|Administrador del control de usuarios   | *    Ver, crear y administrar usuarios
||*    Ver todos los perfiles de asociado
||*    Ver, crear y administrar usuarios asociados  |
|Administrador de facturación | • Ver, crear y administrar los archivos de facturación, facturas y conciliación|
|Usuario predeterminado|  Ver mi perfil   |
|Agente de administrador | *    Administración de clientes
||*    Agregar una lista de dispositivos en el Centro de partners
||*    Crear perfiles y aplicarlos a dispositivos
||*    Administración de suscripciones
||*    Comprobar el estado del servicio y las solicitudes de servicio para clientes
||*    Solicitar privilegios de administrador delegado
||*    Ver los precios y las ofertas
||*    Facturación
||*    Administrar contenido en nombre de un cliente
||*    Registrar un revendedor de valor agregado|
|Agente de ventas | *    Administración de clientes
||*    Agregar una lista de dispositivos en el Centro de partners
||*    Administración de suscripciones
||*    Ver vales de soporte técnico
||*    Solicitar una relación con un cliente
||*    Administrar clientes potenciales
||*    Ver el contrato de cliente
||*    Registrar un vendedor de valor agregado|
|Agente del departamento de soporte técnico| *    Buscar y ver un cliente
||*    Editar detalles del cliente
||*    Ayudar a resolver problemas del cliente referentes a la facturación o la administración de las suscripciones
||*    Solicitar soporte técnico en nombre de los clientes 
||*    Administrar los problemas de suscripción y facturación en nombre de los clientes| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Proveedor del panel de control (CPV). (Rol de CSP y rol que no es de AAD)
Los CPV desarrollan aplicaciones para los partners del Proveedor de soluciones en la nube (CSP) y que así puedan integrar sus sistemas con las API del Centro de partners. 

|**Rol**   |**Qué puede hacer**|
|------------------------------|:----------------------------|
|Administrador global| Ver y administrar el perfil de CPV|
||Ver y administrar los usuarios que necesiten acceso a las funcionalidades de CPV|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a>Usuario invitado (debe agregarse al inquilino de AAD)

|**Usuario invitado**   | **Roles**|
|---------------------------|:--------------------|
||Administrador de partners de MPN|
||Administrador de cuentas|
||Administrador de incentivos|
||Administrador del perfil de negocio|
||Administrador de referencias|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a>Administrar la pertenencia a MPN y su empresa (roles que no son de AAD: estos roles administran el negocio de la empresa en lugar del inquilino)

|**Rol** | **Qué puede hacer**|
|----------------------------|:----------------------------|
|Administrador de partners de MPN|*    Ver, crear y administrar las solicitudes de servicio de los asociados||
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
|Administrador de cuentas| • Agregar ubicaciones
|| • Administrar perfiles relacionados con las cuentas para las que es administrador 
||*    Asignar roles de usuarios del inquilino a roles que no son de AAD 
||*    Inscribir ubicaciones en programas


## <a name="manage-referrals"></a>Administrar referencias 

|**Rol**|**Qué puede hacer**|
|-----------------------------|:------------------------|
|Administrador de referencias       |*    Ver, crear y administrar los perfiles de negocio
||*    Recibir y administrar referencias
||*    Ver, crear y administrar referencias de venta conjunta|
||*    Ver, crear y administrar las solicitudes de servicio de los asociados
|Administrador del perfil de negocio   |*    Ver, crear y administrar el perfil de negocio 
||*    Ver, crear y administrar las solicitudes de servicio de los asociados|

## <a name="manage-incentives"></a>Administrar incentivos 

|**Rol** | **Qué puede hacer**|
|------------------------------|:-------------------------|
|Administrador de incentivos|*    Iniciar y administrar incentivos 
||*    Ver y editar todos los aspectos de los programas de incentivos
||*    Ver y editar información bancaria y fiscal
||*    Ver ganancias de devolución y cooperación
||*    Acceder a soporte técnico
||*    Disputar pagos de incentivos|
|Usuario de incentivos|*    Ver programas de incentivos
||*    Ver e iniciar reclamaciones de incentivos
||*    Ver ganancias de devolución y cooperación
||*    Acceder a soporte técnico

## <a name="view-partner-center-insights-data"></a>Ver datos de conclusiones del Centro de partners

|**Rol** | **Qué puede hacer**|
|------------------------------|:-------------------------|
|Visor de informes ejecutivos|Acceso a todos los conjuntos de datos de informes|
|Visor de informes|Acceso a informes de datos, a excepción de los ingresos y los datos personales de clientes y empleados|












                                    