---
title: Asignar roles y permisos a los usuarios | Centro de partners
ms.topic: article
ms.date: 3/5/2019
description: A todos los empleados que necesiten trabajar en el centro de Partners se les debe asignar un rol.
author: LauraBrenner
ms.author: labrenne
keywords: roles, permisos, admin, agente
ms.localizationpriority: medium
ms.openlocfilehash: 744ce84c47d3adaf21d8f7b790001737d6489cdb
ms.sourcegitcommit: 9d01fb30eafc523784ecc3568c05da9bbe9a1e8c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/01/2019
ms.locfileid: "68708867"
---
# <a name="assign-users-roles-and-permissions"></a>Asignar roles y permisos de usuarios


Ha configurado el perfil de socio comercial, incluidos el nombre y la dirección legales, los detalles de soporte técnico, las exenciones de impuestos de archivo, la información bancaria y el contacto principal de su empresa. Siguiente paso: conseguir que los usuarios configuren con contraseñas y roles para que puedan empezar a trabajar en el centro de Partners con usted.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configurar los empleados para que trabajen en el centro de Partners

Puede determinar los tipos de acceso que los usuarios tienen al centro de Partners por los roles y permisos que les proporciona. Los roles están relacionados con los programas en los que participa su empresa. Por ejemplo, si su empresa es una empresa de proveedor de soluciones en la nube (CSP), no solo tendrá roles de administración de inquilinos de Azure AD estándar, como el administrador global, pero necesitará roles específicos para el programa CSP. Cada programa tiene roles específicos.

>[!Note]
> Los roles de inquilino de Azure Active Directory (AAD) incluyen roles de administrador global, administrador de usuarios y CSP. Los roles que no son de AAD son aquellos que no administran el inquilino e incluyen el administrador de MPN, el administrador del perfil de negocio, el administrador de referencias, el administrador de incentivos y el usuario de incentivos. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Administrar transacciones comerciales en el centro de Partners (roles de Azure AD y CSP)

|**Role**|**Qué pueden hacer**|
|----------------------------------|:---------------------------------|
|Administrador global|• Puede acceder a todos los cuenta de Microsoft/servicios con privilegios completos
|      |• Crear incidencias de soporte técnico para el centro de Partners
||• Ver contratos, listas de precios y ofertas
||• Ver, crear y administrar usuarios asociados|
||  Ver, crear y administrar los archivos de facturación, facturas y concil.
|Administrador de administración de usuarios   | • Ver, crear y administrar usuarios
||• Ver todos los perfiles de socios comerciales
||• Ver, crear y administrar usuarios asociados  |
|Administrador de facturación | -Ver, crear y administrar los archivos de facturación, facturas y concil.|
|Usuario predeterminado|  Ver mi perfil   |
|Agente de administración | • Administración de clientes
||• Agregar lista de dispositivos al centro de Partners
||• Crear y aplicar perfiles a los dispositivos
||• Administración de suscripciones
||• Mantenimiento del servicio y solicitudes de servicio para los clientes
||• Solicitar privilegios de administrador delegado
||• Ver precios y ofertas
||• Facturación
||• Administrar en nombre de un cliente
||• Registrar un revendedor de valor agregado|
|Agente de ventas | • Administración de clientes
||• Agregar lista de dispositivos al centro de Partners
||• Administración de suscripciones
||• Ver listas de precios y ofertas
||• Ver vales de soporte técnico
||• Solicitar una relación con un cliente
||• Administración de clientes potenciales
||• Ver el contrato del cliente
||• Registro de un revendedor de valor agregado|
|Agente del departamento de soporte técnico| • Buscar y ver un cliente
||• Editar los detalles del cliente
||• Ayude a resolver problemas de clientes con la administración de suscripciones o facturación
||• Solicite soporte técnico en nombre de los clientes (tenga en cuenta lo siguiente: Debe ser un agente de administración para completar esta tarea para las suscripciones de Office 365).
||• Administrar suscripciones y problemas de facturación en nombre de los clientes (tenga en cuenta lo siguiente: Debe ser un agente de administración para completar esta tarea para las suscripciones de Office 365).|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Proveedor del panel de control (CPV). (Rol de CSP y rol que no es de AAD)
CPVs desarrollar aplicaciones para que las usen los asociados del proveedor de soluciones en la nube (CSP) para permitirles integrar sus sistemas con las API del centro de Partners. 

|**Role**   |**Qué puede hacer**|
|------------------------------|:----------------------------|
|Administrador global| Ver y administrar el perfil de CPV|
||Ver y administrar a los usuarios que necesiten acceder a las funcionalidades de CPV|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a>Usuario invitado (debe agregarse al inquilino de AAD)

|**Usuario invitado**   | **Roles**|
|---------------------------|:--------------------|
||Administrador de partners de MPN|
||Administrador de cuentas|
||Administrador de incentivos|
||Administrador de perfil de negocio|
||Administrador de referencias|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a>Administrar la pertenencia a MPN y su empresa (roles que no son de AAD: estos roles administran el negocio de la empresa en lugar del inquilino)

|**Role** | **Qué puede hacer**|
|----------------------------|:----------------------------|
|Administrador de partners de MPN|• Ver, crear y administrar solicitudes de servicio de asociados||
||• Visualización de perfiles legales, de empresa, empresariales y MPN
||• Visualización de los detalles del usuario y sus conocimientos
||• Ver competencias
||• Ver y administrar las ventajas
||• Vea y compre ofertas de MPN
||• Ver MPN ofrece el historial de pedidos y las facturas
||• Ver los datos del indicador de contribución del socio
||• Puede trabajar en la herramienta de validación de asientos|
||-Visualización de análisis de datos de clientes
|| Ver otros roles de usuario dentro de la empresa, pero no puede asignar roles
|Administrador de cuentas| Agregar ubicaciones
|| Administrar perfiles relacionados con las cuentas para las que es administrador 
||• Asignar roles para usuarios en roles de inquilino a no AAD 
||• Inscribir ubicaciones en programas


## <a name="manage-referrals"></a>Administrar referencias 

|**Role**|**Qué puede hacer**|
|-----------------------------|:------------------------|
|Administrador de referencias       |• Ver, crear y administrar perfiles de negocio
||• Recibir y administrar referencias
||• Ver, crear y administrar referencias de venta conjunta|
||• Ver, crear y administrar solicitudes de servicio de asociados
|Administrador de perfil de negocio   |• Ver, crear y administrar perfiles de negocio 
||• Ver, crear y administrar solicitudes de servicio de asociados|

## <a name="manage-incentives"></a>Administrar incentivos 

|**Role** | **Qué puede hacer**|
|------------------------------|:-------------------------|
|Administrador de incentivos|• Inicia y administra incentivos 
||• Puede ver y editar todos los aspectos de los programas de incentivos
||• Puede ver y editar la información bancaria y fiscal
||• Visualización de ingresos y beneficios de la Co-op
||• Soporte de acceso
||• Pagos de incentivos de controversias|
|Usuario de incentivos|• Puede ver los programas de incentivos
||• Puede ver e iniciar notificaciones de incentivos
||• Visualización de ingresos y beneficios de la Co-op
||• Soporte de acceso












