---
title: Asignación de roles y permisos a los usuarios
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtén información sobre qué roles son los más adecuados para los usuarios que administran las transacciones comerciales, las referencias, los incentivos o las suscripciones a MPN de tu empresa.
author: hemas
ms.author: hemas
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: c0e7aecd7d56e1919c7f142312a9090b8ff40bd3
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/17/2020
ms.locfileid: "86434324"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="89c04-103">Asignación de roles y permisos a los usuarios de una empresa que necesitan trabajar en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="89c04-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="89c04-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="89c04-104">**Appropriate roles**</span></span>

- <span data-ttu-id="89c04-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="89c04-105">Global admin</span></span>
- <span data-ttu-id="89c04-106">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="89c04-106">User admin</span></span>
- <span data-ttu-id="89c04-107">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="89c04-107">MPN partner admin</span></span>

<span data-ttu-id="89c04-108">Has configurado tu perfil de partner, incluyendo el nombre y la dirección legales, los detalles de soporte técnico, las exenciones fiscales, la información bancaria y el contacto principal de tu empresa.</span><span class="sxs-lookup"><span data-stu-id="89c04-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="89c04-109">Paso siguiente: configura tus usuarios con contraseñas y roles para que puedan comenzar a trabajar en el Centro de partners contigo.</span><span class="sxs-lookup"><span data-stu-id="89c04-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="89c04-110">Configura a sus empleados para trabajar en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="89c04-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="89c04-111">Debes determinar los tipos de acceso que tendrán los usuarios en el Centro de partners, en función de los roles y permisos que les otorgues.</span><span class="sxs-lookup"><span data-stu-id="89c04-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="89c04-112">Los roles están relacionados con los programas en los que participa tu empresa.</span><span class="sxs-lookup"><span data-stu-id="89c04-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="89c04-113">Por ejemplo, si tu negocio es un Proveedor de soluciones en la nube (CSP), no solo tendrás los roles estándar de administración de inquilinos de Azure AD (como el administrador global), sino que también necesitarás roles específicos para el programa de CSP.</span><span class="sxs-lookup"><span data-stu-id="89c04-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="89c04-114">Recuerda que cada programa tiene roles específicos.</span><span class="sxs-lookup"><span data-stu-id="89c04-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="89c04-115">Los roles de inquilino de Azure Active Directory (AAD) incluyen roles de administrador global, administrador de usuarios y CSP.</span><span class="sxs-lookup"><span data-stu-id="89c04-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="89c04-116">Los roles que no son de AAD son aquellos que no administran al inquilino, e incluyen un administrador de MPN, un administrador de perfil comercial, un administrador de referencias, un administrador de incentivos y un usuario de incentivos.</span><span class="sxs-lookup"><span data-stu-id="89c04-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="89c04-117">Administra las transacciones comerciales en el Centro de partners (roles de Azure AD y CSP)</span><span class="sxs-lookup"><span data-stu-id="89c04-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="89c04-118">**Rol**</span><span class="sxs-lookup"><span data-stu-id="89c04-118">**Role**</span></span>|<span data-ttu-id="89c04-119">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="89c04-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="89c04-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="89c04-120">Global admin</span></span>|<span data-ttu-id="89c04-121">\*    Obtener acceso a todos los servicios o cuentas de Microsoft con privilegios completos</span><span class="sxs-lookup"><span data-stu-id="89c04-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="89c04-122">\*    Crear vales de soporte técnico para el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="89c04-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="89c04-123">\*    Ver contratos, listas de precios y ofertas</span><span class="sxs-lookup"><span data-stu-id="89c04-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="89c04-124">\*    Ver, crear y administrar usuarios asociados</span><span class="sxs-lookup"><span data-stu-id="89c04-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="89c04-125">• Ver, crear y administrar los archivos de facturación, facturas y conciliación</span><span class="sxs-lookup"><span data-stu-id="89c04-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="89c04-126">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="89c04-126">User management admin</span></span>   | <span data-ttu-id="89c04-127">\*    Ver, crear y administrar usuarios</span><span class="sxs-lookup"><span data-stu-id="89c04-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="89c04-128">\*    Ver todos los perfiles de asociado</span><span class="sxs-lookup"><span data-stu-id="89c04-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="89c04-129">\*    Ver, crear y administrar usuarios asociados</span><span class="sxs-lookup"><span data-stu-id="89c04-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="89c04-130">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="89c04-130">Billing admin</span></span> | <span data-ttu-id="89c04-131">• Ver, crear y administrar los archivos de facturación, facturas y conciliación</span><span class="sxs-lookup"><span data-stu-id="89c04-131">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="89c04-132">Usuario predeterminado</span><span class="sxs-lookup"><span data-stu-id="89c04-132">Default user</span></span>|  <span data-ttu-id="89c04-133">Ver mi perfil</span><span class="sxs-lookup"><span data-stu-id="89c04-133">View My profile</span></span>   |
|<span data-ttu-id="89c04-134">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="89c04-134">Admin agent</span></span> | <span data-ttu-id="89c04-135">\*    Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="89c04-135">\*    Customer management</span></span>
||<span data-ttu-id="89c04-136">\*    Agregar una lista de dispositivos en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="89c04-136">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="89c04-137">\*    Crear perfiles y aplicarlos a dispositivos</span><span class="sxs-lookup"><span data-stu-id="89c04-137">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="89c04-138">\*    Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="89c04-138">\*    Subscription management</span></span>
||<span data-ttu-id="89c04-139">\*    Comprobar el estado del servicio y las solicitudes de servicio para clientes</span><span class="sxs-lookup"><span data-stu-id="89c04-139">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="89c04-140">\*    Solicitar privilegios de administrador delegado</span><span class="sxs-lookup"><span data-stu-id="89c04-140">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="89c04-141">\*    Ver los precios y las ofertas</span><span class="sxs-lookup"><span data-stu-id="89c04-141">\*    View pricing and offers</span></span>
||<span data-ttu-id="89c04-142">\*    Facturación</span><span class="sxs-lookup"><span data-stu-id="89c04-142">\*    Billing</span></span>
||<span data-ttu-id="89c04-143">\*    Administrar contenido en nombre de un cliente</span><span class="sxs-lookup"><span data-stu-id="89c04-143">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="89c04-144">\*    Registrar un revendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="89c04-144">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="89c04-145">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="89c04-145">Sales agent</span></span> | <span data-ttu-id="89c04-146">\*    Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="89c04-146">\*    Customer management</span></span>
||<span data-ttu-id="89c04-147">\*    Agregar una lista de dispositivos en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="89c04-147">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="89c04-148">\*    Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="89c04-148">\*    Subscription management</span></span>
||<span data-ttu-id="89c04-149">\*    Ver vales de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="89c04-149">\*    View support tickets</span></span>
||<span data-ttu-id="89c04-150">\*    Solicitar una relación con un cliente</span><span class="sxs-lookup"><span data-stu-id="89c04-150">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="89c04-151">\*    Administrar clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="89c04-151">\*    Manage customer leads</span></span>
||<span data-ttu-id="89c04-152">\*    Ver el contrato de cliente</span><span class="sxs-lookup"><span data-stu-id="89c04-152">\*    View the customer agreement</span></span>
||<span data-ttu-id="89c04-153">\*    Registrar un vendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="89c04-153">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="89c04-154">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="89c04-154">Helpdesk agent</span></span>| <span data-ttu-id="89c04-155">\*    Buscar y ver un cliente</span><span class="sxs-lookup"><span data-stu-id="89c04-155">\*    Search for and view a customer</span></span>
||<span data-ttu-id="89c04-156">\*    Editar detalles del cliente</span><span class="sxs-lookup"><span data-stu-id="89c04-156">\*    Edit customer details</span></span>
||<span data-ttu-id="89c04-157">\*    Ayudar a resolver problemas del cliente referentes a la facturación o la administración de las suscripciones</span><span class="sxs-lookup"><span data-stu-id="89c04-157">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="89c04-158">\*    Solicitar soporte técnico en nombre de los clientes</span><span class="sxs-lookup"><span data-stu-id="89c04-158">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="89c04-159">\*    Administrar los problemas de suscripción y facturación en nombre de los clientes</span><span class="sxs-lookup"><span data-stu-id="89c04-159">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="89c04-160">Proveedor del panel de control (CPV).</span><span class="sxs-lookup"><span data-stu-id="89c04-160">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="89c04-161">(Rol de CSP y rol que no es de AAD)</span><span class="sxs-lookup"><span data-stu-id="89c04-161">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="89c04-162">Los CPV desarrollan aplicaciones para los partners del Proveedor de soluciones en la nube (CSP) y que así puedan integrar sus sistemas con las API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="89c04-162">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="89c04-163">**Rol**</span><span class="sxs-lookup"><span data-stu-id="89c04-163">**Role**</span></span>   |<span data-ttu-id="89c04-164">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="89c04-164">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="89c04-165">Administrador global</span><span class="sxs-lookup"><span data-stu-id="89c04-165">Global admin</span></span>| <span data-ttu-id="89c04-166">Ver y administrar el perfil de CPV</span><span class="sxs-lookup"><span data-stu-id="89c04-166">View and manage your CPV profile</span></span>|
||<span data-ttu-id="89c04-167">Ver y administrar los usuarios que necesiten acceso a las funcionalidades de CPV</span><span class="sxs-lookup"><span data-stu-id="89c04-167">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="89c04-168">Usuario invitado (debe agregarse al inquilino de AAD)</span><span class="sxs-lookup"><span data-stu-id="89c04-168">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="89c04-169">**Usuario invitado**</span><span class="sxs-lookup"><span data-stu-id="89c04-169">**Guest user**</span></span>   | <span data-ttu-id="89c04-170">**Roles**</span><span class="sxs-lookup"><span data-stu-id="89c04-170">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="89c04-171">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="89c04-171">MPN partner admin</span></span>|
||<span data-ttu-id="89c04-172">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="89c04-172">Accounts admin</span></span>|
||<span data-ttu-id="89c04-173">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="89c04-173">Incentives admin</span></span>|
||<span data-ttu-id="89c04-174">Administrador del perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="89c04-174">Business profile admin</span></span>|
||<span data-ttu-id="89c04-175">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="89c04-175">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="89c04-176">Administrar la pertenencia a MPN y su empresa (roles que no son de AAD: estos roles administran el negocio de la empresa en lugar del inquilino)</span><span class="sxs-lookup"><span data-stu-id="89c04-176">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="89c04-177">**Rol**</span><span class="sxs-lookup"><span data-stu-id="89c04-177">**Role**</span></span> | <span data-ttu-id="89c04-178">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="89c04-178">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="89c04-179">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="89c04-179">MPN partner admin</span></span>|<span data-ttu-id="89c04-180">\*    Ver, crear y administrar las solicitudes de servicio de los asociados</span><span class="sxs-lookup"><span data-stu-id="89c04-180">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="89c04-181">\*    Ver perfiles legales, de negocios, empresariales y de MPN</span><span class="sxs-lookup"><span data-stu-id="89c04-181">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="89c04-182">\*    Ver los detalles de los usuarios y sus datos de aptitudes</span><span class="sxs-lookup"><span data-stu-id="89c04-182">\*    View user details and their skills data</span></span>
||<span data-ttu-id="89c04-183">\*    Ver competencias</span><span class="sxs-lookup"><span data-stu-id="89c04-183">\*    View competencies</span></span>
||<span data-ttu-id="89c04-184">\*    Ver y administrar ventajas</span><span class="sxs-lookup"><span data-stu-id="89c04-184">\*    View and manage benefits</span></span>
||<span data-ttu-id="89c04-185">\*    Ver y adquirir ofertas de MPN</span><span class="sxs-lookup"><span data-stu-id="89c04-185">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="89c04-186">\*    Ver las facturas y el historial de pedidos de ofertas de MPN</span><span class="sxs-lookup"><span data-stu-id="89c04-186">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="89c04-187">\*    Ver datos de los indicadores de contribución de asociados</span><span class="sxs-lookup"><span data-stu-id="89c04-187">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="89c04-188">\*    Usar la herramienta de validación de cupones</span><span class="sxs-lookup"><span data-stu-id="89c04-188">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="89c04-189">\*     Ver análisis de datos de clientes</span><span class="sxs-lookup"><span data-stu-id="89c04-189">\*    View customer data analytics</span></span>
||<span data-ttu-id="89c04-190">\*    Ver otros roles de usuario dentro de la empresa, pero no puede asignar roles</span><span class="sxs-lookup"><span data-stu-id="89c04-190">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="89c04-191">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="89c04-191">Account admin</span></span>| <span data-ttu-id="89c04-192">• Agregar ubicaciones</span><span class="sxs-lookup"><span data-stu-id="89c04-192">Add locations</span></span>
|| <span data-ttu-id="89c04-193">• Administrar perfiles relacionados con las cuentas para las que es administrador</span><span class="sxs-lookup"><span data-stu-id="89c04-193">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="89c04-194">\*    Asignar roles de usuarios del inquilino a roles que no son de AAD</span><span class="sxs-lookup"><span data-stu-id="89c04-194">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="89c04-195">\*    Inscribir ubicaciones en programas</span><span class="sxs-lookup"><span data-stu-id="89c04-195">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="89c04-196">Administrar referencias</span><span class="sxs-lookup"><span data-stu-id="89c04-196">Manage referrals</span></span> 

|<span data-ttu-id="89c04-197">**Rol**</span><span class="sxs-lookup"><span data-stu-id="89c04-197">**Role**</span></span>|<span data-ttu-id="89c04-198">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="89c04-198">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="89c04-199">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="89c04-199">Referrals admin</span></span>       |<span data-ttu-id="89c04-200">\*    Ver, crear y administrar los perfiles de negocio</span><span class="sxs-lookup"><span data-stu-id="89c04-200">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="89c04-201">\*    Recibir y administrar referencias</span><span class="sxs-lookup"><span data-stu-id="89c04-201">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="89c04-202">\*    Ver, crear y administrar referencias de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="89c04-202">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="89c04-203">\*    Ver, crear y administrar las solicitudes de servicio de los asociados</span><span class="sxs-lookup"><span data-stu-id="89c04-203">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="89c04-204">Administrador del perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="89c04-204">Business profile admin</span></span>   |<span data-ttu-id="89c04-205">\*    Ver, crear y administrar el perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="89c04-205">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="89c04-206">\*    Ver, crear y administrar las solicitudes de servicio de los asociados</span><span class="sxs-lookup"><span data-stu-id="89c04-206">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="89c04-207">Administrar incentivos</span><span class="sxs-lookup"><span data-stu-id="89c04-207">Manage incentives</span></span> 

|<span data-ttu-id="89c04-208">**Rol**</span><span class="sxs-lookup"><span data-stu-id="89c04-208">**Role**</span></span> | <span data-ttu-id="89c04-209">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="89c04-209">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="89c04-210">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="89c04-210">Incentives admin</span></span>|<span data-ttu-id="89c04-211">\*    Iniciar y administrar incentivos</span><span class="sxs-lookup"><span data-stu-id="89c04-211">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="89c04-212">\*    Ver y editar todos los aspectos de los programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="89c04-212">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="89c04-213">\*    Ver y editar información bancaria y fiscal</span><span class="sxs-lookup"><span data-stu-id="89c04-213">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="89c04-214">\*    Ver ganancias de devolución y cooperación</span><span class="sxs-lookup"><span data-stu-id="89c04-214">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="89c04-215">\*    Acceder a soporte técnico</span><span class="sxs-lookup"><span data-stu-id="89c04-215">\*    Access support</span></span>
||<span data-ttu-id="89c04-216">\*    Disputar pagos de incentivos</span><span class="sxs-lookup"><span data-stu-id="89c04-216">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="89c04-217">Usuario de incentivos</span><span class="sxs-lookup"><span data-stu-id="89c04-217">Incentives user</span></span>|<span data-ttu-id="89c04-218">\*    Ver programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="89c04-218">\*    Can view incentives programs</span></span>
||<span data-ttu-id="89c04-219">\*    Ver e iniciar reclamaciones de incentivos</span><span class="sxs-lookup"><span data-stu-id="89c04-219">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="89c04-220">\*    Ver ganancias de devolución y cooperación</span><span class="sxs-lookup"><span data-stu-id="89c04-220">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="89c04-221">\*    Acceder a soporte técnico</span><span class="sxs-lookup"><span data-stu-id="89c04-221">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="89c04-222">Ver datos de conclusiones del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="89c04-222">View Partner Center Insights data</span></span>

|<span data-ttu-id="89c04-223">**Rol**</span><span class="sxs-lookup"><span data-stu-id="89c04-223">**Role**</span></span> | <span data-ttu-id="89c04-224">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="89c04-224">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="89c04-225">Visor de informes ejecutivos</span><span class="sxs-lookup"><span data-stu-id="89c04-225">Executive report viewer</span></span>|<span data-ttu-id="89c04-226">Acceso a todos los conjuntos de datos de informes</span><span class="sxs-lookup"><span data-stu-id="89c04-226">Access to all reporting datasets</span></span>|
|<span data-ttu-id="89c04-227">Visor de informes</span><span class="sxs-lookup"><span data-stu-id="89c04-227">Report viewer</span></span>|<span data-ttu-id="89c04-228">Acceso a informes de datos, a excepción de los ingresos y los datos personales de clientes y empleados</span><span class="sxs-lookup"><span data-stu-id="89c04-228">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    