---
title: Crear cuentas de usuario y establecer permisos (centro de partners operado por 21Vianet)
ms.topic: article
ms.date: 10/29/2018
description: Cómo crear cuentas de usuario para los empleados que necesitan tener acceso al centro de partners.
author: MaggiePucciEvans
ms.author: evansma
ms.openlocfilehash: a96c7fedacbb177c93ae19c5ff4f1a241905be4b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132381"
---
# <a name="create-user-accounts-and-set-permissions"></a>Crear cuentas de usuario y establecer permisos


**Se aplica a**

-   Centro de partners operado por 21Vianet


Crear cuentas de usuario para los empleados que necesitan para realizar tareas en el centro de partners. Solo global o pueden agregar usuarios y asignar roles de usuario administradores de administración. En **configuración de la cuenta** &gt; **administración de usuarios**, puede agregar cuentas de usuario y asignar o cambiar los permisos.

**Agregar un nuevo usuario**

1.  En el centro de partners, vaya al menú panel &gt; **configuración de la cuenta** &gt; **administración de usuarios**.

2.  Selecciona **Agregar usuario**.

3.  Escriba el nombre completo y la dirección de correo electrónico única del usuario.

4.  Seleccione el rol y el nivel de acceso del empleado. Los permisos y acceso a partner Center se basan en roles, que le permite controlar las tareas específicas que puede llevar a cabo cada empleado. Para obtener más información sobre lo que puede hacer cada rol, consulte [establecer permisos de usuario](#setuserpermissions).

5.  Selecciona **Agregar** para crear la cuenta de usuario. Aparece la página de confirmación, mostrar los permisos y la información de inicio de sesión, incluida una contraseña temporal al usuario nuevo.

    >**Importante**<br>Cuando los nuevos usuarios inician sesión en Partner Center por primera vez, debe iniciar sesión con su contraseña temporal. Asegúrese de anotar la nueva contraseña del usuario temporal para poder enviarlo más tarde. No podrá tener acceso a esta información de nuevo. 

### <a href="" id="setuserpermissions"></a>Establecer permisos de usuario

Acceso de centro de partners está basado en roles, lo que significa que puede restringir la vista de usuario para mostrar solo las características y funciones que un usuario necesita para completar tareas específicas. Para cada usuario, tienes que seleccionar dos opciones:

-   El **agente** configuración determina qué tipo de datos del cliente y la empresa puede ver el usuario.

-   El **admin** configuración determina cuánto acceso a las características del centro de partners, funciones y datos del usuario. 

    >**Nota:**<br>El valor predeterminado debe ser **ningún administrador** en la mayoría de los casos, a menos que el empleado requiere permisos para completar tareas administrativas específicas.

####<a name="partner-center-roles-and-associated-permissions"></a>Centro de partners roles y permisos asociados

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Rol en el centro de partners</strong></p></td>
<td><p><strong>¿Qué puede hacer.</strong></p></td>
<td><p><strong>¿Qué no se puede hacer.</strong></p></td>
</tr>
<tr class="even">
<td><p><strong>Agente de administración</strong></p></td>
<td><ul>
<li><p>Administración de clientes</p></li>
<li><p>Administración de suscripciones</p></li>
<li><p>Estado del servicio de acceso para los clientes</p></li>
<li><p>Solicitar privilegios de administrador delegados</p></li>
<li><p>Ver precios y ofertas</p></li>
<li><p>Ver y descargar facturas y archivos de conciliación</p></li>
<li><p>Administrar en nombre de un cliente</p></li>
<li><p>Registrar un revendedor de valor agregado</p></li>
</ul></td>
<td><ul>
<li><p>Administración de usuarios</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Agente de ventas</strong></p></td>
<td><ul>
<li><p>Administración de clientes</p></li>
<li><p>Administración de suscripciones</p></li>
<li><p>Solicitar una relación de revendedor con un cliente</p></li>
<li><p>Ver el contrato de cliente</p></li>
<li><p>Registrar un revendedor de valor agregado</p></li>
</ul></td>
<td><ul>
<li><p>Creación de solicitudes de soporte técnico con 21Vianet para problemas con los servicios o el centro de partners</p></li>
<li><p>Ver el estado del servicio</p></li>
<li><p>Ver precios y ofertas</p></li>
<li><p>Ver y descargar facturas y archivos de conciliación</p></li>
<li><p>Administrar en nombre de un cliente</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Agente de soporte técnico</strong></p></td>
<td><ul>
<li><p>Búsqueda de clientes y ver los detalles de cliente</p></li>
<li><p>Editar detalles del cliente</p></li>
<li><p>Estado del servicio de acceso para los clientes</p></li>
<li><p>Administrar en nombre de un cliente</p></li>
</ul></td>
<td><ul>
<li><p>Ver perfiles de asociados</p></li>
<li><p>Crear una nueva cuenta de cliente</p></li>
<li><p>Editar información de facturación del cliente</p></li>
<li><p>Administración de suscripciones</p></li>
<li><p>Solicitar una relación de revendedor con un cliente</p></li>
<li><p>Ver precios y ofertas</p></li>
<li><p>Ver el contrato de cliente</p></li>
<li><p>Ver y descargar facturas y archivos de conciliación</p></li>
<li><p>Registrar un revendedor de valor agregado</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Administrador global</strong></p></td>
<td><ul>
<li><p>Puede tener acceso a todas las cuentas y los servicios con privilegios completos</p></li>
<li><p>Creación de solicitudes de soporte técnico con 21Vianet para los problemas del centro de partners</p></li>
<li><p>Ver contratos, listas de precios y ofertas</p></li>
<li><p>Ver y descargar facturas y archivos de conciliación</p></li>
<li><p>Ver, crear y administrar los usuarios de su empresa</p></li>
</ul></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>Administrador de facturación</strong></p></td>
<td><ul>
<li><p>Puede tener acceso a todas las facturas y archivos de conciliación con privilegios completos</p></li>
<li><p>Ver contratos, listas de precios y ofertas</p></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>Administrador de usuarios</strong></p></td>
<td><ul>
<li><p>Ver, crear y administrar los usuarios de su empresa</p></li>
<li><p>Ver todos los perfiles de socios</p></li>
</ul></td>
<td></td>
</tr>
</tbody>
</table>

