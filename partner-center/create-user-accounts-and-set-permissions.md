---
title: Crear cuentas de usuario y establecer permisos | Centro de partners
description: El administrador crea una cuenta de usuario para cada empleado del partner que necesite acceder al Centro de partners.
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
ms.openlocfilehash: a755c9375c7bd5e61345d7d7e1ab27e00af3fe4d
ms.sourcegitcommit: 772577c0538a5d5b05d45f0e669697209761ab03
translationtype: HT
---
# <a name="create-user-accounts-and-set-permissions"></a>Crear cuentas de usuario y establecer permisos

**Se aplica a**

-  Centro de partners

El administrador crea una cuenta de usuario para cada empleado del partner que necesite acceder al Centro de partners. Estas tareas las debe hacer un administrador con los permisos **Administrador global** o **Administrador de administración de usuarios**. En **Configuración de la cuenta** &gt; **Administración de usuarios**, puedes agregar cuentas y establecer o actualizar los permisos.

**Agregar un usuario nuevo**

1.  En el Centro de partners, ve al menú Panel &gt; **Configuración de la cuenta** &gt; **Administración de usuarios**.
2.  Elige **Agregar usuario**.

3.  Escribe el nombre completo del usuario y crea una dirección de correo única para él.

4.  Selecciona el tipo de agente y el tipo de administrador. El acceso al Centro de partners se basa en roles, por lo que las selecciones que hagas en este paso personalizan la vista de usuario para mostrar solamente la funcionalidad necesaria. Para obtener más información sobre lo que puede hacer cada rol, consulta la sección [Establecer permisos de usuario](#setuserpermissions).

5.  Agrega el usuario. Verás una pantalla de confirmación con una contraseña temporal para el inicio de sesión nuevo. Tienes que copiar esta información y enviarla al nuevo usuario: no es accesible después de salir de la pantalla. Cuando el usuario inicie sesión por primera vez, se le pedirá que actualice la contraseña.

### <a href="" id="setuserpermissions"></a>Establecer permisos de usuario

El acceso al Centro de partners se basa en roles, lo que significa que puedes personalizar la vista de usuario para mostrar solamente la funcionalidad que este último necesita para su función de trabajo. Para cada usuario, tienes que seleccionar dos opciones:

-   El ajuste **agente** controla el tipo de datos de cliente y la información de Microsoft que el usuario puede ver.

-   El ajuste **admin** determina el grado de control que el usuario posee sobre el entorno del Centro de partners y todos los demás servicios Microsoft (cuentas, perfiles e incidencias de soporte técnico). Esta configuración influye fuera del Centro de partners: un administrador de facturación puede acceder a todas las facturas de todos los servicios Microsoft (incluso los que no estén relacionados con CSP) y un administrador global también puede acceder a las cuentas de usuario y cuentas de cliente más allá de CSP.

    El valor predeterminado siempre debe ser **No admin**, a menos que el rol del usuario necesite acceso adicional para completar las tareas y brindar soporte a los clientes.

En la siguiente tabla se explica el conjunto completo de actividades que cada rol puede hacer en el Centro de partners.

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
<li><p>Administración de suscripciones</p></li>
<li><p>Estado del servicio y solicitudes de servicio para clientes</p></li>
<li><p>Solicitar privilegios de administrador delegado</p></li>
<li><p>Ver precios y ofertas</p></li>
<li><p>Facturación</p></li>
<li><p>Administración en nombre de</p></li>
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
<li><p>Administración de suscripciones</p></li>
<li><p>Ver incidencias de soporte técnico</p></li>
<li><p>Solicitar una relación</p></li>
<li><p>Administrar clientes potenciales</p></li>
<li><p>Ver el contrato de cliente</p></li>
<li><p>Registrar un revendedor de valor agregado</p></li>
</ul></td>
<td><ul>
<li><p>Crear incidencias de soporte técnico para los servicios o el Centro de partners</p></li>
<li><p>Resolver incidencias de soporte técnico</p></li>
<li><p>Ver el estado del servicio</p></li>
<li><p>Ver precios y ofertas</p></li>
<li><p>Facturación</p></li>
<li><p>Administración en nombre de</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Agente del departamento de soporte técnico</strong></p></td>
<td><ul>
<li><p>Buscar y ver un cliente</p></li>
<li><p>Editar detalles del cliente</p></li>
<li><p>Estado del servicio</p></li>
<li><p>Crear vales de soporte para los clientes</p></li>
<li><p>Administrar servicios en nombre de clientes</p></li>
</ul></td>
<td><ul>
<li><p>Ver perfiles de asociados</p></li>
<li><p>Crear una nueva lista de clientes</p></li>
<li><p>Editar la información de facturación del cliente</p></li>
<li><p>Administración de suscripciones</p></li>
<li><p>Solicitar una relación</p></li>
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
</tbody>
</table>

 

 

 



