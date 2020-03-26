---
title: Asignar roles y permisos a los usuarios | Centro de partners
ms.topic: article
ms.date: 03/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtén información sobre qué roles son los más adecuados para los usuarios que administran las transacciones comerciales, las referencias, los incentivos o las suscripciones a MPN de tu empresa.
author: LauraBrenner
ms.author: labrenne
keywords: roles, permisos, administrador, agente
ms.localizationpriority: high
ms.openlocfilehash: 20930ad547bed2399fd60a5c419d8d5c3be8329e
ms.sourcegitcommit: aa33cbd4b3b2f575afcc71ffbdfdc5b45e372f24
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/24/2020
ms.locfileid: "80226171"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="8fcae-104">Asignar roles y permisos de usuarios</span><span class="sxs-lookup"><span data-stu-id="8fcae-104">Assign users roles and permissions</span></span>

<span data-ttu-id="8fcae-105">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="8fcae-105">**Appropriate roles**</span></span>
-    <span data-ttu-id="8fcae-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="8fcae-106">Global admin</span></span>
-    <span data-ttu-id="8fcae-107">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="8fcae-107">User admin</span></span>
-    <span data-ttu-id="8fcae-108">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="8fcae-108">MPN partner admin</span></span>

<span data-ttu-id="8fcae-109">Has configurado tu perfil de partner, incluyendo el nombre y la dirección legales, los detalles de soporte técnico, las exenciones fiscales, la información bancaria y el contacto principal de tu empresa.</span><span class="sxs-lookup"><span data-stu-id="8fcae-109">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="8fcae-110">Siguiente paso: configura tus usuarios con contraseñas y roles para que puedan comenzar a trabajar en el Centro de partners contigo.</span><span class="sxs-lookup"><span data-stu-id="8fcae-110">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="8fcae-111">Configura a sus empleados para trabajar en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="8fcae-111">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="8fcae-112">Debes determinar los tipos de acceso que tendrán los usuarios en el Centro de partners, en función de los roles y permisos que les otorgues.</span><span class="sxs-lookup"><span data-stu-id="8fcae-112">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="8fcae-113">Los roles están relacionados con los programas en los que participa tu empresa.</span><span class="sxs-lookup"><span data-stu-id="8fcae-113">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="8fcae-114">Por ejemplo, si tu negocio es un Proveedor de soluciones en la nube (CSP), no solo tendrás los roles estándar de administración de inquilinos de Azure AD (como el administrador global), sino que también necesitarás roles específicos para el programa de CSP.</span><span class="sxs-lookup"><span data-stu-id="8fcae-114">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="8fcae-115">Recuerda que cada programa tiene roles específicos.</span><span class="sxs-lookup"><span data-stu-id="8fcae-115">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="8fcae-116">Los roles de inquilino de Azure Active Directory (AAD) incluyen roles de administrador global, administrador de usuarios y CSP.</span><span class="sxs-lookup"><span data-stu-id="8fcae-116">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="8fcae-117">Los roles que no son de AAD son aquellos que no administran al inquilino, e incluyen un administrador de MPN, un administrador de perfil comercial, un administrador de referencias, un administrador de incentivos y un usuario de incentivos.</span><span class="sxs-lookup"><span data-stu-id="8fcae-117">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="8fcae-118">Administra las transacciones comerciales en el Centro de partners (roles de Azure AD y CSP)</span><span class="sxs-lookup"><span data-stu-id="8fcae-118">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="8fcae-119">**Rol**</span><span class="sxs-lookup"><span data-stu-id="8fcae-119">**Role**</span></span>|<span data-ttu-id="8fcae-120">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="8fcae-120">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="8fcae-121">Administrador global</span><span class="sxs-lookup"><span data-stu-id="8fcae-121">Global admin</span></span>|<span data-ttu-id="8fcae-122">\*    Obtener acceso a todos los servicios o cuentas de Microsoft con privilegios completos</span><span class="sxs-lookup"><span data-stu-id="8fcae-122">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="8fcae-123">\*    Crear vales de soporte técnico para el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="8fcae-123">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="8fcae-124">\*    Ver contratos, listas de precios y ofertas</span><span class="sxs-lookup"><span data-stu-id="8fcae-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="8fcae-125">\*    Ver, crear y administrar usuarios asociados</span><span class="sxs-lookup"><span data-stu-id="8fcae-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="8fcae-126">• Ver, crear y administrar los archivos de facturación, facturas y conciliación</span><span class="sxs-lookup"><span data-stu-id="8fcae-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="8fcae-127">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="8fcae-127">User management admin</span></span>   | <span data-ttu-id="8fcae-128">\*    Ver, crear y administrar usuarios</span><span class="sxs-lookup"><span data-stu-id="8fcae-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="8fcae-129">\*    Ver todos los perfiles de asociado</span><span class="sxs-lookup"><span data-stu-id="8fcae-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="8fcae-130">\*    Ver, crear y administrar usuarios asociados</span><span class="sxs-lookup"><span data-stu-id="8fcae-130">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="8fcae-131">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="8fcae-131">Billing admin</span></span> | <span data-ttu-id="8fcae-132">• Ver, crear y administrar los archivos de facturación, facturas y conciliación</span><span class="sxs-lookup"><span data-stu-id="8fcae-132">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="8fcae-133">Usuario predeterminado</span><span class="sxs-lookup"><span data-stu-id="8fcae-133">Default user</span></span>|  <span data-ttu-id="8fcae-134">Ver mi perfil</span><span class="sxs-lookup"><span data-stu-id="8fcae-134">View My profile</span></span>   |
|<span data-ttu-id="8fcae-135">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="8fcae-135">Admin agent</span></span> | <span data-ttu-id="8fcae-136">\*    Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="8fcae-136">\*    Customer management</span></span>
||<span data-ttu-id="8fcae-137">\*    Agregar una lista de dispositivos en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="8fcae-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="8fcae-138">\*    Crear perfiles y aplicarlos a dispositivos</span><span class="sxs-lookup"><span data-stu-id="8fcae-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="8fcae-139">\*    Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="8fcae-139">\*    Subscription management</span></span>
||<span data-ttu-id="8fcae-140">\*    Comprobar el estado del servicio y las solicitudes de servicio para clientes</span><span class="sxs-lookup"><span data-stu-id="8fcae-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="8fcae-141">\*    Solicitar privilegios de administrador delegado</span><span class="sxs-lookup"><span data-stu-id="8fcae-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="8fcae-142">\*    Ver los precios y las ofertas</span><span class="sxs-lookup"><span data-stu-id="8fcae-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="8fcae-143">\*    Facturación</span><span class="sxs-lookup"><span data-stu-id="8fcae-143">\*    Billing</span></span>
||<span data-ttu-id="8fcae-144">\*    Administrar contenido en nombre de un cliente</span><span class="sxs-lookup"><span data-stu-id="8fcae-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="8fcae-145">\*    Registrar un revendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="8fcae-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="8fcae-146">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="8fcae-146">Sales agent</span></span> | <span data-ttu-id="8fcae-147">\*    Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="8fcae-147">\*    Customer management</span></span>
||<span data-ttu-id="8fcae-148">\*    Agregar una lista de dispositivos en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="8fcae-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="8fcae-149">\*    Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="8fcae-149">\*    Subscription management</span></span>
||<span data-ttu-id="8fcae-150">\*    Ver vales de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="8fcae-150">\*    View support tickets</span></span>
||<span data-ttu-id="8fcae-151">\*    Solicitar una relación con un cliente</span><span class="sxs-lookup"><span data-stu-id="8fcae-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="8fcae-152">\*    Administrar clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="8fcae-152">\*    Manage customer leads</span></span>
||<span data-ttu-id="8fcae-153">\*    Ver el contrato de cliente</span><span class="sxs-lookup"><span data-stu-id="8fcae-153">\*    View the customer agreement</span></span>
||<span data-ttu-id="8fcae-154">\*    Registrar un vendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="8fcae-154">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="8fcae-155">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="8fcae-155">Helpdesk agent</span></span>| <span data-ttu-id="8fcae-156">\*    Buscar y ver un cliente</span><span class="sxs-lookup"><span data-stu-id="8fcae-156">\*    Search for and view a customer</span></span>
||<span data-ttu-id="8fcae-157">\*    Editar detalles del cliente</span><span class="sxs-lookup"><span data-stu-id="8fcae-157">\*    Edit customer details</span></span>
||<span data-ttu-id="8fcae-158">\*    Ayudar a resolver problemas del cliente referentes a la facturación o la administración de las suscripciones</span><span class="sxs-lookup"><span data-stu-id="8fcae-158">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="8fcae-159">\*    Solicitar soporte técnico en nombre de los clientes</span><span class="sxs-lookup"><span data-stu-id="8fcae-159">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="8fcae-160">\*    Administrar los problemas de suscripción y facturación en nombre de los clientes</span><span class="sxs-lookup"><span data-stu-id="8fcae-160">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="8fcae-161">Proveedor del panel de control (CPV).</span><span class="sxs-lookup"><span data-stu-id="8fcae-161">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="8fcae-162">(Rol de CSP y rol que no es de AAD)</span><span class="sxs-lookup"><span data-stu-id="8fcae-162">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="8fcae-163">Los CPV desarrollan aplicaciones para los partners del Proveedor de soluciones en la nube (CSP) y que así puedan integrar sus sistemas con las API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="8fcae-163">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="8fcae-164">**Rol**</span><span class="sxs-lookup"><span data-stu-id="8fcae-164">**Role**</span></span>   |<span data-ttu-id="8fcae-165">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="8fcae-165">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="8fcae-166">Administrador global</span><span class="sxs-lookup"><span data-stu-id="8fcae-166">Global admin</span></span>| <span data-ttu-id="8fcae-167">Ver y administrar el perfil de CPV</span><span class="sxs-lookup"><span data-stu-id="8fcae-167">View and manage your CPV profile</span></span>|
||<span data-ttu-id="8fcae-168">Ver y administrar los usuarios que necesiten acceso a las funcionalidades de CPV</span><span class="sxs-lookup"><span data-stu-id="8fcae-168">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="8fcae-169">Usuario invitado (debe agregarse al inquilino de AAD)</span><span class="sxs-lookup"><span data-stu-id="8fcae-169">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="8fcae-170">**Usuario invitado**</span><span class="sxs-lookup"><span data-stu-id="8fcae-170">**Guest user**</span></span>   | <span data-ttu-id="8fcae-171">**Roles**</span><span class="sxs-lookup"><span data-stu-id="8fcae-171">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="8fcae-172">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="8fcae-172">MPN partner admin</span></span>|
||<span data-ttu-id="8fcae-173">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="8fcae-173">Accounts admin</span></span>|
||<span data-ttu-id="8fcae-174">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="8fcae-174">Incentives admin</span></span>|
||<span data-ttu-id="8fcae-175">Administrador del perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="8fcae-175">Business profile admin</span></span>|
||<span data-ttu-id="8fcae-176">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="8fcae-176">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="8fcae-177">Administrar la pertenencia a MPN y su empresa (roles que no son de AAD: estos roles administran el negocio de la empresa en lugar del inquilino)</span><span class="sxs-lookup"><span data-stu-id="8fcae-177">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="8fcae-178">**Rol**</span><span class="sxs-lookup"><span data-stu-id="8fcae-178">**Role**</span></span> | <span data-ttu-id="8fcae-179">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="8fcae-179">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="8fcae-180">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="8fcae-180">MPN partner admin</span></span>|<span data-ttu-id="8fcae-181">\*    Ver, crear y administrar las solicitudes de servicio de los asociados</span><span class="sxs-lookup"><span data-stu-id="8fcae-181">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="8fcae-182">\*    Ver perfiles legales, de negocios, empresariales y de MPN</span><span class="sxs-lookup"><span data-stu-id="8fcae-182">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="8fcae-183">\*    Ver los detalles de los usuarios y sus datos de aptitudes</span><span class="sxs-lookup"><span data-stu-id="8fcae-183">\*    View user details and their skills data</span></span>
||<span data-ttu-id="8fcae-184">\*    Ver competencias</span><span class="sxs-lookup"><span data-stu-id="8fcae-184">\*    View competencies</span></span>
||<span data-ttu-id="8fcae-185">\*    Ver y administrar ventajas</span><span class="sxs-lookup"><span data-stu-id="8fcae-185">\*    View and manage benefits</span></span>
||<span data-ttu-id="8fcae-186">\*    Ver y adquirir ofertas de MPN</span><span class="sxs-lookup"><span data-stu-id="8fcae-186">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="8fcae-187">\*    Ver las facturas y el historial de pedidos de ofertas de MPN</span><span class="sxs-lookup"><span data-stu-id="8fcae-187">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="8fcae-188">\*    Ver datos de los indicadores de contribución de asociados</span><span class="sxs-lookup"><span data-stu-id="8fcae-188">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="8fcae-189">\*    Usar la herramienta de validación de cupones</span><span class="sxs-lookup"><span data-stu-id="8fcae-189">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="8fcae-190">\*     Ver análisis de datos de clientes</span><span class="sxs-lookup"><span data-stu-id="8fcae-190">\*    View customer data analytics</span></span>
||<span data-ttu-id="8fcae-191">\*    Ver otros roles de usuario dentro de la empresa, pero no puede asignar roles</span><span class="sxs-lookup"><span data-stu-id="8fcae-191">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="8fcae-192">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="8fcae-192">Account admin</span></span>| <span data-ttu-id="8fcae-193">• Agregar ubicaciones</span><span class="sxs-lookup"><span data-stu-id="8fcae-193">Add locations</span></span>
|| <span data-ttu-id="8fcae-194">• Administrar perfiles relacionados con las cuentas para las que es administrador</span><span class="sxs-lookup"><span data-stu-id="8fcae-194">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="8fcae-195">\*    Asignar roles de usuarios del inquilino a roles que no son de AAD</span><span class="sxs-lookup"><span data-stu-id="8fcae-195">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="8fcae-196">\*    Inscribir ubicaciones en programas</span><span class="sxs-lookup"><span data-stu-id="8fcae-196">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="8fcae-197">Administrar referencias</span><span class="sxs-lookup"><span data-stu-id="8fcae-197">Manage referrals</span></span> 

|<span data-ttu-id="8fcae-198">**Rol**</span><span class="sxs-lookup"><span data-stu-id="8fcae-198">**Role**</span></span>|<span data-ttu-id="8fcae-199">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="8fcae-199">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="8fcae-200">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="8fcae-200">Referrals admin</span></span>       |<span data-ttu-id="8fcae-201">\*    Ver, crear y administrar los perfiles de negocio</span><span class="sxs-lookup"><span data-stu-id="8fcae-201">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="8fcae-202">\*    Recibir y administrar referencias</span><span class="sxs-lookup"><span data-stu-id="8fcae-202">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="8fcae-203">\*    Ver, crear y administrar referencias de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="8fcae-203">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="8fcae-204">\*    Ver, crear y administrar las solicitudes de servicio de los asociados</span><span class="sxs-lookup"><span data-stu-id="8fcae-204">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="8fcae-205">Administrador del perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="8fcae-205">Business profile admin</span></span>   |<span data-ttu-id="8fcae-206">\*    Ver, crear y administrar el perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="8fcae-206">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="8fcae-207">\*    Ver, crear y administrar las solicitudes de servicio de los asociados</span><span class="sxs-lookup"><span data-stu-id="8fcae-207">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="8fcae-208">Administrar incentivos</span><span class="sxs-lookup"><span data-stu-id="8fcae-208">Manage incentives</span></span> 

|<span data-ttu-id="8fcae-209">**Rol**</span><span class="sxs-lookup"><span data-stu-id="8fcae-209">**Role**</span></span> | <span data-ttu-id="8fcae-210">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="8fcae-210">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="8fcae-211">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="8fcae-211">Incentives admin</span></span>|<span data-ttu-id="8fcae-212">\*    Iniciar y administrar incentivos</span><span class="sxs-lookup"><span data-stu-id="8fcae-212">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="8fcae-213">\*    Ver y editar todos los aspectos de los programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="8fcae-213">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="8fcae-214">\*    Ver y editar información bancaria y fiscal</span><span class="sxs-lookup"><span data-stu-id="8fcae-214">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="8fcae-215">\*    Ver ganancias de devolución y cooperación</span><span class="sxs-lookup"><span data-stu-id="8fcae-215">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="8fcae-216">\*    Acceder a soporte técnico</span><span class="sxs-lookup"><span data-stu-id="8fcae-216">\*    Access support</span></span>
||<span data-ttu-id="8fcae-217">\*    Disputar pagos de incentivos</span><span class="sxs-lookup"><span data-stu-id="8fcae-217">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="8fcae-218">Usuario de incentivos</span><span class="sxs-lookup"><span data-stu-id="8fcae-218">Incentives user</span></span>|<span data-ttu-id="8fcae-219">\*    Ver programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="8fcae-219">\*    Can view incentives programs</span></span>
||<span data-ttu-id="8fcae-220">\*    Ver e iniciar reclamaciones de incentivos</span><span class="sxs-lookup"><span data-stu-id="8fcae-220">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="8fcae-221">\*    Ver ganancias de devolución y cooperación</span><span class="sxs-lookup"><span data-stu-id="8fcae-221">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="8fcae-222">\*    Acceder a soporte técnico</span><span class="sxs-lookup"><span data-stu-id="8fcae-222">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="8fcae-223">Ver datos de conclusiones del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="8fcae-223">View Partner Center Insights data</span></span>

|<span data-ttu-id="8fcae-224">**Rol**</span><span class="sxs-lookup"><span data-stu-id="8fcae-224">**Role**</span></span> | <span data-ttu-id="8fcae-225">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="8fcae-225">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="8fcae-226">Visor de informes ejecutivos</span><span class="sxs-lookup"><span data-stu-id="8fcae-226">Executive report viewer</span></span>|<span data-ttu-id="8fcae-227">Acceso a todos los conjuntos de datos de informes</span><span class="sxs-lookup"><span data-stu-id="8fcae-227">Access to all reporting datasets</span></span>|
|<span data-ttu-id="8fcae-228">Visor de informes</span><span class="sxs-lookup"><span data-stu-id="8fcae-228">Report viewer</span></span>|<span data-ttu-id="8fcae-229">Acceso a informes de datos, a excepción de los ingresos y los datos personales de clientes y empleados</span><span class="sxs-lookup"><span data-stu-id="8fcae-229">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












