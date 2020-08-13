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
ms.openlocfilehash: c87e47efc6c94e4e53a031a983a4a4e528ddc012
ms.sourcegitcommit: 59bdf42f5282262835cb7ee2bd215bbddc7686d7
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/06/2020
ms.locfileid: "87839190"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="b6f13-103">Asignación de roles y permisos a los usuarios de una empresa que necesitan trabajar en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="b6f13-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="b6f13-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="b6f13-104">**Appropriate roles**</span></span>

- <span data-ttu-id="b6f13-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="b6f13-105">Global admin</span></span>
- <span data-ttu-id="b6f13-106">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="b6f13-106">User admin</span></span>
- <span data-ttu-id="b6f13-107">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="b6f13-107">MPN partner admin</span></span>

<span data-ttu-id="b6f13-108">Has configurado tu perfil de partner, incluyendo el nombre y la dirección legales, los detalles de soporte técnico, las exenciones fiscales, la información bancaria y el contacto principal de tu empresa.</span><span class="sxs-lookup"><span data-stu-id="b6f13-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="b6f13-109">Paso siguiente: configura tus usuarios con contraseñas y roles para que puedan comenzar a trabajar en el Centro de partners contigo.</span><span class="sxs-lookup"><span data-stu-id="b6f13-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="b6f13-110">Configura a sus empleados para trabajar en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="b6f13-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="b6f13-111">Debes determinar los tipos de acceso que tendrán los usuarios en el Centro de partners, en función de los roles y permisos que les otorgues.</span><span class="sxs-lookup"><span data-stu-id="b6f13-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="b6f13-112">Los roles están relacionados con los programas en los que participa tu empresa.</span><span class="sxs-lookup"><span data-stu-id="b6f13-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="b6f13-113">Por ejemplo, si tu negocio es un Proveedor de soluciones en la nube (CSP), no solo tendrás los roles estándar de administración de inquilinos de Azure AD (como el administrador global), sino que también necesitarás roles específicos para el programa de CSP.</span><span class="sxs-lookup"><span data-stu-id="b6f13-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="b6f13-114">Recuerda que cada programa tiene roles específicos.</span><span class="sxs-lookup"><span data-stu-id="b6f13-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="b6f13-115">Los roles de inquilino de Azure Active Directory (AAD) incluyen roles de administrador global, administrador de usuarios y CSP.</span><span class="sxs-lookup"><span data-stu-id="b6f13-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="b6f13-116">Los roles que no son de AAD son aquellos que no administran al inquilino, e incluyen un administrador de MPN, un administrador de perfil comercial, un administrador de referencias, un administrador de incentivos y un usuario de incentivos.</span><span class="sxs-lookup"><span data-stu-id="b6f13-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="b6f13-117">Administra las transacciones comerciales en el Centro de partners (roles de Azure AD y CSP)</span><span class="sxs-lookup"><span data-stu-id="b6f13-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="b6f13-118">**Rol**</span><span class="sxs-lookup"><span data-stu-id="b6f13-118">**Role**</span></span>|<span data-ttu-id="b6f13-119">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="b6f13-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="b6f13-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="b6f13-120">Global admin</span></span>|<span data-ttu-id="b6f13-121">\*    Obtener acceso a todos los servicios o cuentas de Microsoft con privilegios completos</span><span class="sxs-lookup"><span data-stu-id="b6f13-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="b6f13-122">\*    Crear vales de soporte técnico para el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="b6f13-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="b6f13-123">\*    Ver contratos, listas de precios y ofertas</span><span class="sxs-lookup"><span data-stu-id="b6f13-123">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="b6f13-124">\*    Ver, crear y administrar usuarios asociados</span><span class="sxs-lookup"><span data-stu-id="b6f13-124">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="b6f13-125">• Ver, crear y administrar los archivos de facturación, facturas y conciliación</span><span class="sxs-lookup"><span data-stu-id="b6f13-125">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="b6f13-126">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="b6f13-126">User management admin</span></span>   | <span data-ttu-id="b6f13-127">\*    Ver, crear y administrar usuarios</span><span class="sxs-lookup"><span data-stu-id="b6f13-127">\*    View, create, and manage users</span></span>
||<span data-ttu-id="b6f13-128">\*    Ver todos los perfiles de asociado</span><span class="sxs-lookup"><span data-stu-id="b6f13-128">\*    View all partner profiles</span></span>
||<span data-ttu-id="b6f13-129">\*    Ver, crear y administrar usuarios asociados</span><span class="sxs-lookup"><span data-stu-id="b6f13-129">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="b6f13-130">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="b6f13-130">Billing admin</span></span> | <span data-ttu-id="b6f13-131">• Ver, crear y administrar los archivos de facturación, facturas y conciliación</span><span class="sxs-lookup"><span data-stu-id="b6f13-131">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="b6f13-132">\*    Ver precios</span><span class="sxs-lookup"><span data-stu-id="b6f13-132">\*    View pricing</span></span>
|<span data-ttu-id="b6f13-133">Usuario predeterminado</span><span class="sxs-lookup"><span data-stu-id="b6f13-133">Default user</span></span>|  <span data-ttu-id="b6f13-134">Ver mi perfil</span><span class="sxs-lookup"><span data-stu-id="b6f13-134">View My profile</span></span>   |
|<span data-ttu-id="b6f13-135">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="b6f13-135">Admin agent</span></span> | <span data-ttu-id="b6f13-136">\*    Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="b6f13-136">\*    Customer management</span></span>
||<span data-ttu-id="b6f13-137">\*    Agregar una lista de dispositivos en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="b6f13-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="b6f13-138">\*    Crear perfiles y aplicarlos a dispositivos</span><span class="sxs-lookup"><span data-stu-id="b6f13-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="b6f13-139">\*    Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="b6f13-139">\*    Subscription management</span></span>
||<span data-ttu-id="b6f13-140">\*    Comprobar el estado del servicio y las solicitudes de servicio para clientes</span><span class="sxs-lookup"><span data-stu-id="b6f13-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="b6f13-141">\*    Solicitar privilegios de administrador delegado</span><span class="sxs-lookup"><span data-stu-id="b6f13-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="b6f13-142">\*    Ver los precios y las ofertas</span><span class="sxs-lookup"><span data-stu-id="b6f13-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="b6f13-143">\*    Facturación</span><span class="sxs-lookup"><span data-stu-id="b6f13-143">\*    Billing</span></span>
||<span data-ttu-id="b6f13-144">\*    Administrar contenido en nombre de un cliente</span><span class="sxs-lookup"><span data-stu-id="b6f13-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="b6f13-145">\*    Registrar un revendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="b6f13-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="b6f13-146">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="b6f13-146">Sales agent</span></span> | <span data-ttu-id="b6f13-147">\*    Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="b6f13-147">\*    Customer management</span></span>
||<span data-ttu-id="b6f13-148">\*    Agregar una lista de dispositivos en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="b6f13-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="b6f13-149">\*    Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="b6f13-149">\*    Subscription management</span></span>
||<span data-ttu-id="b6f13-150">\*    Ver vales de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="b6f13-150">\*    View support tickets</span></span>
||<span data-ttu-id="b6f13-151">\*    Solicitar una relación con un cliente</span><span class="sxs-lookup"><span data-stu-id="b6f13-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="b6f13-152">\*    Ver los precios y las ofertas</span><span class="sxs-lookup"><span data-stu-id="b6f13-152">\*    View pricing and offers</span></span>
||<span data-ttu-id="b6f13-153">\*    Administrar clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="b6f13-153">\*    Manage customer leads</span></span>
||<span data-ttu-id="b6f13-154">\*    Ver el contrato de cliente</span><span class="sxs-lookup"><span data-stu-id="b6f13-154">\*    View the customer agreement</span></span>
||<span data-ttu-id="b6f13-155">\*    Registrar un vendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="b6f13-155">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="b6f13-156">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="b6f13-156">Helpdesk agent</span></span>| <span data-ttu-id="b6f13-157">\*    Buscar y ver un cliente</span><span class="sxs-lookup"><span data-stu-id="b6f13-157">\*    Search for and view a customer</span></span>
||<span data-ttu-id="b6f13-158">\*    Editar detalles del cliente</span><span class="sxs-lookup"><span data-stu-id="b6f13-158">\*    Edit customer details</span></span>
||<span data-ttu-id="b6f13-159">\*    Ayudar a resolver problemas del cliente referentes a la facturación o la administración de las suscripciones</span><span class="sxs-lookup"><span data-stu-id="b6f13-159">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="b6f13-160">\*    Solicitar soporte técnico en nombre de los clientes</span><span class="sxs-lookup"><span data-stu-id="b6f13-160">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="b6f13-161">\*    Administrar los problemas de suscripción y facturación en nombre de los clientes</span><span class="sxs-lookup"><span data-stu-id="b6f13-161">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="b6f13-162">Proveedor del panel de control (CPV).</span><span class="sxs-lookup"><span data-stu-id="b6f13-162">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="b6f13-163">(Rol de CSP y rol que no es de AAD)</span><span class="sxs-lookup"><span data-stu-id="b6f13-163">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="b6f13-164">Los CPV desarrollan aplicaciones para los partners del Proveedor de soluciones en la nube (CSP) y que así puedan integrar sus sistemas con las API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="b6f13-164">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="b6f13-165">**Rol**</span><span class="sxs-lookup"><span data-stu-id="b6f13-165">**Role**</span></span>   |<span data-ttu-id="b6f13-166">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="b6f13-166">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="b6f13-167">Administrador global</span><span class="sxs-lookup"><span data-stu-id="b6f13-167">Global admin</span></span>| <span data-ttu-id="b6f13-168">Ver y administrar el perfil de CPV</span><span class="sxs-lookup"><span data-stu-id="b6f13-168">View and manage your CPV profile</span></span>|
||<span data-ttu-id="b6f13-169">Ver y administrar los usuarios que necesiten acceso a las funcionalidades de CPV</span><span class="sxs-lookup"><span data-stu-id="b6f13-169">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="b6f13-170">Usuario invitado (debe agregarse al inquilino de AAD)</span><span class="sxs-lookup"><span data-stu-id="b6f13-170">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="b6f13-171">**Usuario invitado**</span><span class="sxs-lookup"><span data-stu-id="b6f13-171">**Guest user**</span></span>   | <span data-ttu-id="b6f13-172">**Roles**</span><span class="sxs-lookup"><span data-stu-id="b6f13-172">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="b6f13-173">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="b6f13-173">MPN partner admin</span></span>|
||<span data-ttu-id="b6f13-174">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="b6f13-174">Accounts admin</span></span>|
||<span data-ttu-id="b6f13-175">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="b6f13-175">Incentives admin</span></span>|
||<span data-ttu-id="b6f13-176">Administrador del perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="b6f13-176">Business profile admin</span></span>|
||<span data-ttu-id="b6f13-177">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="b6f13-177">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="b6f13-178">Administrar la pertenencia a MPN y su empresa (roles que no son de AAD: estos roles administran el negocio de la empresa en lugar del inquilino)</span><span class="sxs-lookup"><span data-stu-id="b6f13-178">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="b6f13-179">**Rol**</span><span class="sxs-lookup"><span data-stu-id="b6f13-179">**Role**</span></span> | <span data-ttu-id="b6f13-180">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="b6f13-180">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="b6f13-181">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="b6f13-181">MPN partner admin</span></span>|<span data-ttu-id="b6f13-182">\*    Ver, crear y administrar las solicitudes de servicio de los asociados</span><span class="sxs-lookup"><span data-stu-id="b6f13-182">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="b6f13-183">\*    Ver perfiles legales, de negocios, empresariales y de MPN</span><span class="sxs-lookup"><span data-stu-id="b6f13-183">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="b6f13-184">\*    Ver los detalles de los usuarios y sus datos de aptitudes</span><span class="sxs-lookup"><span data-stu-id="b6f13-184">\*    View user details and their skills data</span></span>
||<span data-ttu-id="b6f13-185">\*    Ver competencias</span><span class="sxs-lookup"><span data-stu-id="b6f13-185">\*    View competencies</span></span>
||<span data-ttu-id="b6f13-186">\*    Ver y administrar ventajas</span><span class="sxs-lookup"><span data-stu-id="b6f13-186">\*    View and manage benefits</span></span>
||<span data-ttu-id="b6f13-187">\*    Ver y adquirir ofertas de MPN</span><span class="sxs-lookup"><span data-stu-id="b6f13-187">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="b6f13-188">\*    Ver las facturas y el historial de pedidos de ofertas de MPN</span><span class="sxs-lookup"><span data-stu-id="b6f13-188">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="b6f13-189">\*    Ver datos de los indicadores de contribución de asociados</span><span class="sxs-lookup"><span data-stu-id="b6f13-189">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="b6f13-190">\*    Usar la herramienta de validación de cupones</span><span class="sxs-lookup"><span data-stu-id="b6f13-190">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="b6f13-191">\*     Ver análisis de datos de clientes</span><span class="sxs-lookup"><span data-stu-id="b6f13-191">\*    View customer data analytics</span></span>
||<span data-ttu-id="b6f13-192">\*    Ver otros roles de usuario dentro de la empresa, pero no puede asignar roles</span><span class="sxs-lookup"><span data-stu-id="b6f13-192">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="b6f13-193">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="b6f13-193">Account admin</span></span>| <span data-ttu-id="b6f13-194">• Agregar ubicaciones</span><span class="sxs-lookup"><span data-stu-id="b6f13-194">Add locations</span></span>
|| <span data-ttu-id="b6f13-195">• Administrar perfiles relacionados con las cuentas para las que es administrador</span><span class="sxs-lookup"><span data-stu-id="b6f13-195">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="b6f13-196">\*    Asignar roles de usuarios del inquilino a roles que no son de AAD</span><span class="sxs-lookup"><span data-stu-id="b6f13-196">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="b6f13-197">\*    Inscribir ubicaciones en programas</span><span class="sxs-lookup"><span data-stu-id="b6f13-197">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="b6f13-198">Administrar referencias</span><span class="sxs-lookup"><span data-stu-id="b6f13-198">Manage referrals</span></span> 

|<span data-ttu-id="b6f13-199">**Rol**</span><span class="sxs-lookup"><span data-stu-id="b6f13-199">**Role**</span></span>|<span data-ttu-id="b6f13-200">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="b6f13-200">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="b6f13-201">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="b6f13-201">Referrals admin</span></span>       |<span data-ttu-id="b6f13-202">\*    Ver, crear y administrar los perfiles de negocio</span><span class="sxs-lookup"><span data-stu-id="b6f13-202">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="b6f13-203">\*    Recibir y administrar referencias</span><span class="sxs-lookup"><span data-stu-id="b6f13-203">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="b6f13-204">\*    Ver, crear y administrar referencias de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="b6f13-204">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="b6f13-205">\*    Ver, crear y administrar las solicitudes de servicio de los asociados</span><span class="sxs-lookup"><span data-stu-id="b6f13-205">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="b6f13-206">Administrador del perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="b6f13-206">Business profile admin</span></span>   |<span data-ttu-id="b6f13-207">\*    Ver, crear y administrar el perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="b6f13-207">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="b6f13-208">\*    Ver, crear y administrar las solicitudes de servicio de los asociados</span><span class="sxs-lookup"><span data-stu-id="b6f13-208">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="b6f13-209">Administrar incentivos</span><span class="sxs-lookup"><span data-stu-id="b6f13-209">Manage incentives</span></span> 

|<span data-ttu-id="b6f13-210">**Rol**</span><span class="sxs-lookup"><span data-stu-id="b6f13-210">**Role**</span></span> | <span data-ttu-id="b6f13-211">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="b6f13-211">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="b6f13-212">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="b6f13-212">Incentives admin</span></span>|<span data-ttu-id="b6f13-213">\*    Iniciar y administrar incentivos</span><span class="sxs-lookup"><span data-stu-id="b6f13-213">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="b6f13-214">\*    Ver y editar todos los aspectos de los programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="b6f13-214">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="b6f13-215">\*    Ver y editar información bancaria y fiscal</span><span class="sxs-lookup"><span data-stu-id="b6f13-215">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="b6f13-216">\*    Ver ganancias de devolución y cooperación</span><span class="sxs-lookup"><span data-stu-id="b6f13-216">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="b6f13-217">\*    Acceder a soporte técnico</span><span class="sxs-lookup"><span data-stu-id="b6f13-217">\*    Access support</span></span>
||<span data-ttu-id="b6f13-218">\*    Disputar pagos de incentivos</span><span class="sxs-lookup"><span data-stu-id="b6f13-218">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="b6f13-219">Usuario de incentivos</span><span class="sxs-lookup"><span data-stu-id="b6f13-219">Incentives user</span></span>|<span data-ttu-id="b6f13-220">\*    Ver programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="b6f13-220">\*    Can view incentives programs</span></span>
||<span data-ttu-id="b6f13-221">\*    Ver e iniciar reclamaciones de incentivos</span><span class="sxs-lookup"><span data-stu-id="b6f13-221">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="b6f13-222">\*    Ver ganancias de devolución y cooperación</span><span class="sxs-lookup"><span data-stu-id="b6f13-222">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="b6f13-223">\*    Acceder a soporte técnico</span><span class="sxs-lookup"><span data-stu-id="b6f13-223">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="b6f13-224">Ver datos de conclusiones del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="b6f13-224">View Partner Center Insights data</span></span>

|<span data-ttu-id="b6f13-225">**Rol**</span><span class="sxs-lookup"><span data-stu-id="b6f13-225">**Role**</span></span> | <span data-ttu-id="b6f13-226">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="b6f13-226">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="b6f13-227">Visor de informes ejecutivos</span><span class="sxs-lookup"><span data-stu-id="b6f13-227">Executive report viewer</span></span>|<span data-ttu-id="b6f13-228">Acceso a todos los conjuntos de datos de informes</span><span class="sxs-lookup"><span data-stu-id="b6f13-228">Access to all reporting datasets</span></span>|
|<span data-ttu-id="b6f13-229">Visor de informes</span><span class="sxs-lookup"><span data-stu-id="b6f13-229">Report viewer</span></span>|<span data-ttu-id="b6f13-230">Acceso a informes de datos, a excepción de los ingresos y los datos personales de clientes y empleados</span><span class="sxs-lookup"><span data-stu-id="b6f13-230">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    
