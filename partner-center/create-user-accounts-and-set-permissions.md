---
title: Create user accounts and set permissions | Partner Center
description: The admin creates a user account for each partner employee who needs access to Partner Center.
ms.assetid: 75D805AE-9922-4CFD-9427-196047D70963
author: MaggiePucciEvans
ms.openlocfilehash: 6a54dd2a221f38edb2439596ba2637907dad73de
ms.sourcegitcommit: f62ea44fb20c2ada21154e254984413ee2a685f3
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/18/2017
---
# <a name="create-user-accounts-and-assign-permissions"></a>Create user accounts and assign permissions

**Applies to**

-  Partner Center

Create user accounts for employees who need access to Partner Center. These tasks must be done by an admin with user management admin permissions. 

## <a name="add-a-new-user"></a>Add a new user

1. On the **Dashboard** menu, select **Account settings > User management**.

2.  Select **Add user**.

3.  Enter the user’s full name and unique email address.

4.  Select the type of agent and the type of admin. Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks. For more information about what each role can do, see [Assign user permissions](#assignuserpermissions).

5.  Select **Add** to create the user account. Confirm the user's details on the next page.

>**Important**<br>
Make a note of the new user's sign-in information displayed on this page. Be sure to copy and send this information to the new user as you will not be able to access it again later. <br>

>The user will need to sign in to Partner Center with their user name and temporary password. When the user signs in to Partner Center for the first time, they are prompted to change their password.    


### <a href="" id="assignuserpermissions"></a>Assign user permissions

Partner Center access is role-based, so you can assign permissions to customize the user's view to show only the features the user needs to complete specific tasks. 

For each user, you must select two permission levels:

-   Agent permissions control what kind of customer data and account information the user can see and change.

-   Admin permissions control the level of access the user has to Partner Center features. This setting has impact outside of Partner Center -- a billing admin can access bills for all Microsoft services (even those unrelated to CSP), and a global admin can access user accounts and customer accounts beyond CSP as well.

## <a name="assign-permissions-for-incentives-users"></a>Assign permissions for Incentives users
When you set up your incentives users, you can give them either the incentive admin role or incentive user role.  El administrador de incentivos puede inscribir y migrar las inscripciones de incentivos, editar perfiles bancarios y fiscales y ver todos los informes. Los usuarios de incentivos pueden revisar las inscripciones del programa y ver informes. Incentives admins and users can have other roles in Partner Center for your organization but to work on Incentives programs a user must be either incentives admin or user.

>**Important** The default setting should always be **No admin**, unless the user's role requires additional access to complete tasks and support customers.

The following table explains what each role can do in Partner Center.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Role in Partner Center</strong></p></td>
<td><p><strong>What they can do</strong></p></td>
<td><p><strong>What they can't do</strong></p></td>
</tr>
<tr class="even">
<td><p><strong>Admin agent</strong></p></td>
<td><ul>
<li><p>Customer management</p></li>
<li><p>Add device list to Partner Center</p></li>
<p><li>Create and apply profiles to devices</p></li>
<li><p>Subscription management</p></li>
<li><p>Service health and service requests for customers</p></li>
<li><p>Request delegated administrator privileges</p></li>
<li><p>View pricing and offers</p></li>
<li><p>Billing</p></li>
<li><p>Administer on behalf of a customer</p></li>
<li><p>Register a value added reseller</p></li>
</ul></td>
<td><ul>
<li><p>User management</p></li>
<li><p>Service requests for Partner Center</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Sales agent</strong></p></td>
<td><ul>
<li><p>Customer management</p></li>
<li><p>Add device list to Partner Center</p></li>
<li><p>Subscription management</p></li>
<li><p>View support tickets</p></li>
<li><p>Request a relationship with a customer</p></li>
<li><p>Manage customer leads</p></li>
<li><p>View the customer agreement</p></li>
<li><p>Register a value added reseller</p></li>
</ul></td>
<td><ul>
<li><p>Create service requests for problems with Partner Center</p></li>
<li><p>Resolve support tickets</p></li>
<li><p>View service health</p></li>
<li><p>View pricing and offers</p></li>
<li><p>Billing</p></li>
<li><p>Administer on behalf of a customer</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Helpdesk agent</strong></p></td>
<td><ul>
<li><p>Search for and view a customer</p></li>
<li><p>Editar detalles del cliente</p></li>
<li><p>Ayudar a resolver problemas del cliente referentes a la facturación o la administración de las suscripciones</p></li>
<li><p>Solicitar soporte técnico en nombre de los clientes. (Nota: Debes ser un agente administrador para completar esta tarea en las suscripciones de Office 365).</p></li>
<li><p>Administrar los problemas referidos a suscripciones y facturación en nombre de los clientes. (Nota: Debes ser un agente administrador para completar esta tarea en las suscripciones de Office 365).</p></li>
</ul></td>
<td><ul>
<li><p>Ver perfiles de asociados</p></li>
<li><p>Create a new customer account</p></li>
<li><p>Editar la información de facturación del cliente</p></li>
<li><p>Solicitar soporte técnico de Azure</p></li>
<li><p>Manage subscriptions</p></li>
<li><p>Request a relationship with a customer</p></li>
<li><p>Manage customer leads</p></li>
<li><p>View pricing and offers</p></li>
<li><p>View the customer agreement</p></li>
<li><p>Billing</p></li>
<li><p>Register a value added reseller</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Global admin</strong></p></td>
<td><ul>
<li><p>Can access all Microsoft account/services with full privileges</p></li>
<li><p>Create support tickets for Partner Center</p></li>
<li><p>View agreements, price lists, and offers</p></li>
<li><p>Billing</p></li>
<li><p>View, create, and manage partner users</p></li>
</ul></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>Billing admin</strong></p></td>
<td><ul>
<li><p>Can access all bills from Microsoft with full privileges</p></li>
<li><p>View agreements, price lists, and offers</p></li>
<li><p>Billing</p></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>User management admin</strong></p></td>
<td><ul>
<li><p>View, create, and manage users</p></li>
<li><p>View all partner profiles</p></li>
</ul></td>
<td></td>
</tr>
<tr class="even">
<td><p><strong>Administrador de incentivos</strong></p></td>
<td><ul>
<li><p>Inscribirse en programas de incentivos</p></li>
<li><p>Migrar las inscripciones de incentivo al Centro de partners</p></li>
<li><p>Ver y administrar todas las inscripciones</p></li>
<li><p>Editar perfiles bancarios y fiscales de los programas de incentivos</p></li>
<li><p>Ver todos los informes de incentivos</p></li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td><p><strong>Usuario de incentivos</strong></p></td>
<td><ul>
<li><p>Ver inscripciones</p></li>
<li><p>Ver informes</p></li>
</ul></td>
<td></td>
</tr>
</tbody>
</table>

 

 

 



