---
title: Crear cuentas de usuario y establecer permisos | Centro de partners
description: El administrador crea una cuenta de usuario para cada empleado del partner que necesite acceder al Centro de partners.
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
ms.openlocfilehash: 337100db2ee89fcb92b040db52b62383cef37aeb
ms.sourcegitcommit: d5ce1bf171e535b0236bcd1e6dfbc4ef01ebd209
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 11/22/2017
---
# <a name="create-user-accounts-and-assign-permissions"></a>Crear cuentas de usuario y asignar permisos

**Se aplica a**

-  Centro de partners

Crear cuentas de usuario para los empleados que necesitan acceder al Centro de partners. Estas tareas las debe hacer un administrador con los permisos de administrador de administración de usuarios. 

## <a name="add-a-new-user"></a>Agregar un usuario nuevo

1. En el menú **Panel**, selecciona **Configuración de la cuenta > Administración de usuarios**.

2.  Selecciona **Agregar usuario**.

3.  Escribe el nombre completo y la dirección de correo electrónico del usuario.

4.  Selecciona el tipo de agente y el tipo de administrador. El acceso al Centro de partners se basa en roles, por lo que puedes asignar permisos para personalizar la vista del usuario y mostrar solo las características que el usuario necesite para completar las tareas específicas. Para obtener más información sobre lo que puede hacer cada rol, consulta la sección [Asignar permisos de usuario](#assignuserpermissions).

5.  Selecciona **Agregar** para crear la cuenta de usuario. Confirma los detalles del usuario en la página siguiente.

>**Importante**<br>
Anota la nueva información de inicio de sesión del usuario se muestra en esta página. Asegúrate de copiar y enviar esta información al nuevo usuario ya que no volverás a tener acceso a dicha información. <br>

>El usuario tendrá que iniciar sesión en el Centro de partners con su nombre de usuario y su contraseña temporal. Cuando el usuario inicie sesión en el Centro de partners por primera vez, se le pedirá cambiar la contraseña.    


### <a href="" id="assignuserpermissions"></a>Asignar permisos de usuario

El acceso al Centro de partners se basa en roles, por lo que puedes asignar permisos para personalizar la vista del usuario y mostrar solo las características que el usuario necesite para completar las tareas específicas. 

Para cada usuario, tienes que seleccionar dos niveles de permisos:

-   Los permisos de agente controlan qué tipo de datos de cliente e información de la cuenta pueden ser vistas y cambiadas por el usuario.

-   Los permisos de administrador controlan el nivel de acceso que el usuario tiene a las características del Centro de partners. Esta configuración influye fuera del Centro de partners: un administrador de facturación puede acceder a todas las facturas de todos los servicios Microsoft (incluso los que no estén relacionados con CSP) y un administrador global también puede acceder a las cuentas de usuario y cuentas de cliente más allá de CSP.

>**Importante** El valor predeterminado siempre debe ser **No admin**, a menos que el rol del usuario necesite acceso adicional para completar las tareas y brindar soporte a los clientes.

La siguiente tabla explica lo que puede hacer cada rol en el Centro de partners.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Rol en el Centro de partners</strong></p></td>
<td><p><strong>Lo que se puede hacer</strong></p></td>
<td><p><strong>Lo que no se puede hacer</strong></p></td>
</tr>
<tr class="even">
<td><p><strong>Agente de administración</strong></p></td>
<td><ul>
<li><p>Administración de clientes</p></li>
<li><p>Agregar una lista de dispositivos en el Centro de partners</p></li>
<p><li>Crear y aplicar los perfiles a los dispositivos</p></li>
<li><p>Administración de suscripciones</p></li>
<li><p>Estado del servicio y solicitudes de servicio para clientes</p></li>
<li><p>Solicitar privilegios de administrador delegado</p></li>
<li><p>Ver precios y ofertas</p></li>
<li><p>Facturación</p></li>
<li><p>Administrar en nombre de un cliente</p></li>
<li><p>Registrar un revendedor de valor agregado</p></li>
</ul></td>
<td><ul>
<li><p>Administración de usuarios</p></li>
<li><p>Solicitudes de servicio para el Centro de partners</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Agente de ventas</strong></p></td>
<td><ul>
<li><p>Administración de clientes</p></li>
<li><p>Agregar una lista de dispositivos en el Centro de partners</p></li>
<li><p>Administración de suscripciones</p></li>
<li><p>Ver incidencias de soporte técnico</p></li>
<li><p>Solicitar relación con un cliente</p></li>
<li><p>Administrar clientes potenciales</p></li>
<li><p>Ver el contrato de cliente</p></li>
<li><p>Registrar un revendedor de valor agregado</p></li>
</ul></td>
<td><ul>
<li><p>Crear solicitudes de servicio para los problemas con el Centro de partners</p></li>
<li><p>Resolver incidencias de soporte técnico</p></li>
<li><p>Ver el estado del servicio</p></li>
<li><p>Ver precios y ofertas</p></li>
<li><p>Facturación</p></li>
<li><p>Administrar en nombre de un cliente</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Agente del departamento de soporte técnico</strong></p></td>
<td><ul>
<li><p>Buscar y ver un cliente</p></li>
<li><p>Editar detalles del cliente</p></li>
<li><p>Ayudar a resolver problemas del cliente referentes a la facturación o la administración de las suscripciones</p></li>
<li><p>Solicitar soporte técnico en nombre de los clientes. (Nota: Debes ser un agente administrador para completar esta tarea en las suscripciones de Office 365).</p></li>
<li><p>Administrar los problemas referidos a suscripciones y facturación en nombre de los clientes. (Nota: Debes ser un agente administrador para completar esta tarea en las suscripciones de Office 365).</p></li>
</ul></td>
<td><ul>
<li><p>Ver perfiles de asociados</p></li>
<li><p>Crear una nueva cuenta de cliente</p></li>
<li><p>Editar la información de facturación del cliente</p></li>
<li><p>Solicitar soporte técnico de Azure</p></li>
<li><p>Administrar las suscripciones</p></li>
<li><p>Solicitar relación con un cliente</p></li>
<li><p>Administrar clientes potenciales</p></li>
<li><p>Ver precios y ofertas</p></li>
<li><p>Ver el contrato de cliente</p></li>
<li><p>Facturación</p></li>
<li><p>Registrar un revendedor de valor agregado</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Administrador global</strong></p></td>
<td><ul>
<li><p>Puede acceder a todas las cuentas o servicios Microsoft con privilegios completos</p></li>
<li><p>Crear incidencias de soporte técnico para el Centro de partners</p></li>
<li><p>Ver contratos, listas de precios y ofertas</p></li>
<li><p>Facturación</p></li>
<li><p>Ver, crear y administrar los usuarios de partners</p></li>
</ul></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>Administrador de facturación</strong></p></td>
<td><ul>
<li><p>Puede acceder a todas las facturas de Microsoft con privilegios completos</p></li>
<li><p>Ver contratos, listas de precios y ofertas</p></li>
<li><p>Facturación</p></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>Administrador de administración de usuarios</strong></p></td>
<td><ul>
<li><p>Ver, crear y administrar usuarios</p></li>
<li><p>Ver todos los perfiles de socios</p></li>
</ul></td>
<td></td>
</tr>


 

 

 



