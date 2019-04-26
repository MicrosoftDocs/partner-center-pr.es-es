---
title: Asignar roles y permisos a los usuarios | Centro de partners
ms.topic: article
ms.date: 3/5/19
description: Todos los empleados que necesiten trabajar en el centro de Partners deben tener asignado un rol.
author: LauraBrenner
ms.author: labrenne
keywords: roles, permisos, admin, agente
ms.localizationpriority: medium
ms.openlocfilehash: 66923c8a5d4912d178ef483a883f08f40ed8378b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133905"
---
# <a name="assign-users-roles-and-permissions"></a>Asignar roles y permisos de usuarios


Ha configurado el perfil de socio comercial como nombre legal y dirección, detalles sobre la compatibilidad, exenciones fiscales de archivo, información bancaria y al contacto principal de su empresa. Siguiente paso: los usuarios configurar con las contraseñas y los roles para que pueden empezar a trabajar en el centro de partners con usted.

## <a name="set-up-your-employees-to-work-in-partner-center"></a>Configuración de sus empleados a trabajar en el centro de partners

Determinar los tipos de acceso de los usuarios al centro de partners mediante los roles y permisos que les proporcione. Roles están relacionados con los programas de en que su empresa está implicada. Por ejemplo, si su empresa es una proveedor de soluciones en la nube (CSP) de la empresa, no sólo tendrá el estándar de Azure AD roles de administración como administrador global del inquilino, pero será necesario que las funciones específicas del programa CSP. Cada programa tiene roles específicos a él.

>[!Note]
> Roles de inquilino de Azure Active Directory (AAD) incluyen el administrador global, Administrador de usuarios y roles CSP. Roles de AAD de no incluyen MPN admin, admin de perfil de empresa, Administrador de referencias, incentivo administrador y usuario incentivo. 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a>Administrar las transacciones comerciales en el centro de partners (Azure AD y los roles CSP)

|**Role**|**¿Qué puede hacer.**|
|----------------------------------|:---------------------------------|
|Administrador global|• Puede tener acceso a todos los cuenta de Microsoft y servicios con privilegios completos
|      |• Crear incidencias de soporte técnico para el centro de partners
||• Vista acuerdos, listas de precios y ofertas
||• Ver, crear y administrar los usuarios del asociado|
|Administrador de usuarios   | • Ver, crear y administrar usuarios
||• Ver todos los perfiles de socios comerciales
||• Ver, crear y administrar los usuarios del asociado  |
|Administrador de facturación | -Ver, crear y administrar la facturación, facturas y archivos de conciliación|
|Usuario predeterminado|  Ver mi perfil   |
|Agente de administración | • Administración de clientes
||• Agregue la lista de dispositivos en el centro de partners <
||• Crear y aplicar los perfiles en dispositivos
||• Administración de suscripciones
||• Service health y atender solicitudes de clientes
||• Solicitud delega privilegios de administrador
||• Ver información sobre precios y ofertas
||• La facturación
||• Administrar parte de un cliente
||• Register un valor agregado reseller|
|Agente de ventas | • Administración de clientes
||• Agregue la lista de dispositivos en el centro de partners
||• Administración de suscripciones
||• Incidencias de soporte técnico de vista
||• Solicitud una relación con un cliente
||• Administración de clientes potenciales
||• Ver el contrato de cliente
||• Register un revendedor de valor agregado|
|Agente del departamento de soporte técnico| • Buscar y ver un cliente
||• Editar detalles de cliente
||• Ayuda resolver al cliente los problemas con la administración de facturación o suscripción
||• Soporte técnico de solicitud en nombre de los clientes (tenga en cuenta: Debe ser un agente de administración para completar esta tarea para las suscripciones de Office 365)
||• Administración de suscripciones y facturación problemas en el nombre de los clientes (tenga en cuenta: Debe ser un agente de administración para completar esta tarea para las suscripciones de Office 365)|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a>Proveedor del Panel de control (CPV). (Rol CSP y rol sin AAD)
CPVs desarrollar aplicaciones para su uso por los asociados de proveedor de soluciones en la nube (CSP) que les permite integrar los sistemas con Partner Center API. 

|**Role**   |**¿Qué puede hacer**|
|------------------------------|:----------------------------|
|Administrador global| Ver y administrar su perfil CPV|
||Ver y administrar cualquiera de los usuarios que necesitan tener acceso a las funcionalidades de CPV|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a>Administrar la pertenencia a MPN y su empresa (roles sin AAD)

|**Role** | **¿Qué puede hacer**|
|----------------------------|:----------------------------|
|Administrador de partners de MPN|•CAN agregar los usuarios que no sean inquilinos
||• Ver, crear y administrar solicitudes de servicio asociado
||• Vista legal, organización, empresariales y perfiles MPN
||• Ver detalles del usuario y sus datos de conocimientos
||• Competencias de vista
||• Ver y administrar las prestaciones
||Compra y vista • MPN ofrece
||• Vista MPN ofrece facturas e historial de pedidos
||• Ver datos de contribución de asociado
||• Puede trabajar en la herramienta de validación del vale|
||-Ver análisis de datos de clientes
|Administrador de cuentas| • Puede agregar los usuarios que no sean inquilinos
||• Agregar o eliminar las ubicaciones
||-Administración de perfiles de las cuentas de para que Administrador 
||• Asignación de roles para los usuarios de inquilinos para roles de AAD no 
||• Ubicaciones en programas de inscripción

## <a name="guest-user-must-be-added-to-the-aad-tenant"></a>Usuario invitado (debe agregarse al inquilino de AAD)

|**Usuario invitado**   | **Roles**|
|---------------------------|:--------------------|
||Administrador de partners de MPN|
||Administrador de cuentas|
||Administrador de incentivos|
||Administrador de perfil de negocio|
||Administrador de referencias|


## <a name="manage-referrals-non-aad-roles"></a>Administrar referencias (roles sin AAD)

|**Role**|**¿Qué puede hacer**|
|-----------------------------|:------------------------|
|Administrador de referencias       |• Ver, crear y administrar perfiles de negocio
||• Recibir y administrar las referencias
||• Ver, crear y administrar solicitudes de servicio asociado|
|Administrador de perfil de negocio   |•View, crear y administrar el perfil de negocio 
||• Ver, crear y administrar solicitudes de servicio asociado|

## <a name="manage-incentives--non-aad-roles"></a>Administrar incentivos (roles sin AAD)

|**Role** | **¿Qué puede hacer**|
|------------------------------|:-------------------------|
|Administrador de incentivos|• Inicia y administra los incentivos 
||Puede ver y editar todos los aspectos de programas de incentivos •
||• Puede ver y editar información bancaria y fiscal
||• Beneficios de descuento y Co-op de vista
||• Compatibilidad con el acceso
||• Los pagos incentivos de conflictos|
|Usuario de incentivos|• Puede ver los programas de incentivos
||• Puede ver e iniciar las notificaciones de incentivos
||• Beneficios de descuento y Co-op de vista
||• Beneficios de descuento y Co-op de vista
||• Compatibilidad con el acceso












