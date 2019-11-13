---
title: Asignar roles y permisos a los usuarios | Centro de partners
ms.topic: article
ms.date: 10/10/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Todos los empleados que necesiten trabajar en el Centro de partners deben tener roles asignados.
author: LauraBrenner
ms.author: labrenne
keywords: roles, permisos, administrador, agente
ms.localizationpriority: high
ms.openlocfilehash: aa2eb2561332f730abedd2416813189abe6dc02d
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/06/2019
ms.locfileid: "73652431"
---
# <a name="assign-users-roles-and-permissions"></a>Asignar roles y permisos de usuarios


Has configurado tu perfil de partner, incluyendo el nombre y la dirección legales, los detalles de soporte técnico, las exenciones fiscales, la información bancaria y el contacto principal de tu empresa. Siguiente paso: configura tus usuarios con contraseñas y roles para que puedan comenzar a trabajar en el Centro de partners contigo.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configura a sus empleados para trabajar en el Centro de partners

Debes determinar los tipos de acceso que tendrán los usuarios en el Centro de partners, en función de los roles y permisos que les otorgues. Los roles están relacionados con los programas en los que participa tu empresa. Por ejemplo, si tu negocio es un Proveedor de soluciones en la nube (CSP), no solo tendrás los roles estándar de administración de inquilinos de Azure AD (como el administrador global), sino que también necesitarás roles específicos para el programa de CSP. Recuerda que cada programa tiene roles específicos.

>[!Note]
> Los roles de inquilino de Azure Active Directory (AAD) incluyen roles de administrador global, administrador de usuarios y CSP. Los roles que no son de AAD son aquellos que no administran al inquilino, e incluyen un administrador de MPN, un administrador de perfil comercial, un administrador de referencias, un administrador de incentivos y un usuario de incentivos. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Administra las transacciones comerciales en el Centro de partners (roles de Azure AD y CSP)

|**Rol**|**Qué puede hacer**|
|----------------------------------|:---------------------------------|
|Administrador global|• Obtener acceso a todas las cuentas o servicios de Microsoft con privilegios completos
|      |• Crear vales de soporte técnico para el Centro de partners
||• Ver contratos, listas de precios y ofertas
||• Ver, crear y administrar los usuarios de partners|
||  • Ver, crear y administrar los archivos de facturación, facturas y conciliación
|Administrador de administración de usuarios   | • Ver, crear y administrar usuarios
||• Ver todos los perfiles de partners
||• Ver, crear y administrar los usuarios de partners  |
|Administrador de facturación | • Ver, crear y administrar los archivos de facturación, facturas y conciliación|
|Usuario predeterminado|  Ver mi perfil   |
|Agente de administración | • Administración de clientes
||• Agregar una lista de dispositivos en el Centro de partners
||• Crear y aplicar los perfiles a los dispositivos
||• Administración de suscripciones
||• Comprobar el estado del servicio y las solicitudes de servicio para clientes
||• Solicitar privilegios de administrador delegado
||• Ver los precios y las ofertas
||• Facturación
||• Administrar contenido en nombre de un cliente
||• Registrar un vendedor de valor agregado|
|Agente de ventas | • Administración de clientes
||• Agregar una lista de dispositivos en el Centro de partners
||• Administración de suscripciones
||• Ver vales de soporte técnico
||• Solicitar la relación con un cliente
||• Administrar clientes potenciales
||• Ver el contrato de cliente
||• Registrar un vendedor de valor agregado|
|Agente del departamento de soporte técnico| • Buscar y ver un cliente
||• Editar detalles del cliente
||• Ayudar a resolver problemas del cliente referentes a la facturación o la administración de las suscripciones
||• Solicitar soporte técnico en nombre de los clientes (Nota: Debes ser un agente de administración para poder completar esta tarea en las suscripciones de Office 365)
||• Administrar los problemas de suscripción y facturación en nombre de los clientes (Nota: Debes ser un agente de administración para poder completar esta tarea en las suscripciones de Office 365)|

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
|Administrador de partners de MPN|• Ver, crear y administrar las solicitudes de servicio de los partners||
||• Ver perfiles legales, de negocios, empresariales y de MPN
||• Ver los detalles de los usuarios y sus datos de habilidades
||• Ver competencias
||• Ver y administrar ventajas
||• Ver y adquirir ofertas de MPN
||• Ver facturas e historial de pedidos de ofertas de MPN
||• Ver datos de los indicadores de contribución de partners
||• Usar la herramienta de validación de comprobantes|
||• Ver el análisis de datos de clientes
|| • Ver otros roles de usuario dentro de la empresa, pero no puede asignar roles
|Administrador de cuentas| • Agregar ubicaciones
|| • Administrar perfiles relacionados con las cuentas para las que es administrador 
||• Asignar roles para usuarios en el inquilino con roles que no sean de AAD 
||• Inscribir ubicaciones en programas


## <a name="manage-referrals"></a>Administrar referencias 

|**Rol**|**Qué puede hacer**|
|-----------------------------|:------------------------|
|Administrador de referencias       |• Ver, crear y administrar los perfiles de negocio
||• Recibir y administrar las referencias
||• Ver, crear y administrar referencias de venta conjunta|
||• Ver, crear y administrar las solicitudes de servicio de los partners
|Administrador del perfil de negocio   |• Ver, crear y administrar el perfil de negocio 
||• Ver, crear y administrar las solicitudes de servicio de los partners|

## <a name="manage-incentives"></a>Administrar incentivos 

|**Rol** | **Qué puede hacer**|
|------------------------------|:-------------------------|
|Administrador de incentivos|• Inicia y administra incentivos 
||• Puede ver y editar todos los aspectos de programas de incentivos
||• Puede ver y editar información bancaria y fiscal
||• Ver ganancias de reembolso y cooperación
||• Acceso a soporte técnico
||• Disputar pagos de incentivos|
|Usuario de incentivos|• Puede ver programas de incentivos
||• Puede ver e iniciar reclamaciones de incentivos
||• Ver ganancias de reembolso y cooperación
||• Acceso a soporte técnico












