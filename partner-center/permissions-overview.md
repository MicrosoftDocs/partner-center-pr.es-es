---
title: Asignación de roles y permisos a los usuarios
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtén información sobre qué roles son los más adecuados para los usuarios que administran las transacciones comerciales, las referencias, los incentivos o las suscripciones a MPN de tu empresa.
author: LauraBrenner
ms.author: labrenne
keywords: roles, permisos, administrador, agente
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 0858340c6965ac932f0d4694f6f21be89ca5f817
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795882"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="96850-104">Asignación de roles y permisos a los usuarios de una empresa que necesitan trabajar en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="96850-104">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="96850-105">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="96850-105">**Appropriate roles**</span></span>

- <span data-ttu-id="96850-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="96850-106">Global admin</span></span>
- <span data-ttu-id="96850-107">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="96850-107">User admin</span></span>
- <span data-ttu-id="96850-108">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="96850-108">MPN partner admin</span></span>

<span data-ttu-id="96850-109">Has configurado tu perfil de partner, incluyendo el nombre y la dirección legales, los detalles de soporte técnico, las exenciones fiscales, la información bancaria y el contacto principal de tu empresa.</span><span class="sxs-lookup"><span data-stu-id="96850-109">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="96850-110">Paso siguiente: configura tus usuarios con contraseñas y roles para que puedan comenzar a trabajar en el Centro de partners contigo.</span><span class="sxs-lookup"><span data-stu-id="96850-110">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="96850-111">Configura a sus empleados para trabajar en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="96850-111">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="96850-112">Debes determinar los tipos de acceso que tendrán los usuarios en el Centro de partners, en función de los roles y permisos que les otorgues.</span><span class="sxs-lookup"><span data-stu-id="96850-112">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="96850-113">Los roles están relacionados con los programas en los que participa tu empresa.</span><span class="sxs-lookup"><span data-stu-id="96850-113">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="96850-114">Por ejemplo, si tu negocio es un Proveedor de soluciones en la nube (CSP), no solo tendrás los roles estándar de administración de inquilinos de Azure AD (como el administrador global), sino que también necesitarás roles específicos para el programa de CSP.</span><span class="sxs-lookup"><span data-stu-id="96850-114">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="96850-115">Recuerda que cada programa tiene roles específicos.</span><span class="sxs-lookup"><span data-stu-id="96850-115">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="96850-116">Los roles de inquilino de Azure Active Directory (AAD) incluyen roles de administrador global, administrador de usuarios y CSP.</span><span class="sxs-lookup"><span data-stu-id="96850-116">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="96850-117">Los roles que no son de AAD son aquellos que no administran al inquilino, e incluyen un administrador de MPN, un administrador de perfil comercial, un administrador de referencias, un administrador de incentivos y un usuario de incentivos.</span><span class="sxs-lookup"><span data-stu-id="96850-117">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="96850-118">Administra las transacciones comerciales en el Centro de partners (roles de Azure AD y CSP)</span><span class="sxs-lookup"><span data-stu-id="96850-118">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="96850-119">**Rol**</span><span class="sxs-lookup"><span data-stu-id="96850-119">**Role**</span></span>|<span data-ttu-id="96850-120">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="96850-120">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="96850-121">Administrador global</span><span class="sxs-lookup"><span data-stu-id="96850-121">Global admin</span></span>|<span data-ttu-id="96850-122">\*    Obtener acceso a todos los servicios o cuentas de Microsoft con privilegios completos</span><span class="sxs-lookup"><span data-stu-id="96850-122">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="96850-123">\*    Crear vales de soporte técnico para el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="96850-123">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="96850-124">\*    Ver contratos, listas de precios y ofertas</span><span class="sxs-lookup"><span data-stu-id="96850-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="96850-125">\*    Ver, crear y administrar usuarios asociados</span><span class="sxs-lookup"><span data-stu-id="96850-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="96850-126">• Ver, crear y administrar los archivos de facturación, facturas y conciliación</span><span class="sxs-lookup"><span data-stu-id="96850-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="96850-127">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="96850-127">User management admin</span></span>   | <span data-ttu-id="96850-128">\*    Ver, crear y administrar usuarios</span><span class="sxs-lookup"><span data-stu-id="96850-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="96850-129">\*    Ver todos los perfiles de asociado</span><span class="sxs-lookup"><span data-stu-id="96850-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="96850-130">\*    Ver, crear y administrar usuarios asociados</span><span class="sxs-lookup"><span data-stu-id="96850-130">\*    View, create, and manage partner users</span></span>  |
|<span data-ttu-id="96850-131">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="96850-131">Billing admin</span></span> | <span data-ttu-id="96850-132">• Ver, crear y administrar los archivos de facturación, facturas y conciliación</span><span class="sxs-lookup"><span data-stu-id="96850-132">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="96850-133">Usuario predeterminado</span><span class="sxs-lookup"><span data-stu-id="96850-133">Default user</span></span>|  <span data-ttu-id="96850-134">Ver mi perfil</span><span class="sxs-lookup"><span data-stu-id="96850-134">View My profile</span></span>   |
|<span data-ttu-id="96850-135">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="96850-135">Admin agent</span></span> | <span data-ttu-id="96850-136">\*    Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="96850-136">\*    Customer management</span></span>
||<span data-ttu-id="96850-137">\*    Agregar una lista de dispositivos en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="96850-137">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="96850-138">\*    Crear perfiles y aplicarlos a dispositivos</span><span class="sxs-lookup"><span data-stu-id="96850-138">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="96850-139">\*    Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="96850-139">\*    Subscription management</span></span>
||<span data-ttu-id="96850-140">\*    Comprobar el estado del servicio y las solicitudes de servicio para clientes</span><span class="sxs-lookup"><span data-stu-id="96850-140">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="96850-141">\*    Solicitar privilegios de administrador delegado</span><span class="sxs-lookup"><span data-stu-id="96850-141">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="96850-142">\*    Ver los precios y las ofertas</span><span class="sxs-lookup"><span data-stu-id="96850-142">\*    View pricing and offers</span></span>
||<span data-ttu-id="96850-143">\*    Facturación</span><span class="sxs-lookup"><span data-stu-id="96850-143">\*    Billing</span></span>
||<span data-ttu-id="96850-144">\*    Administrar contenido en nombre de un cliente</span><span class="sxs-lookup"><span data-stu-id="96850-144">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="96850-145">\*    Registrar un revendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="96850-145">\*    Register a value added reseller</span></span>|
|<span data-ttu-id="96850-146">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="96850-146">Sales agent</span></span> | <span data-ttu-id="96850-147">\*    Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="96850-147">\*    Customer management</span></span>
||<span data-ttu-id="96850-148">\*    Agregar una lista de dispositivos en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="96850-148">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="96850-149">\*    Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="96850-149">\*    Subscription management</span></span>
||<span data-ttu-id="96850-150">\*    Ver vales de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="96850-150">\*    View support tickets</span></span>
||<span data-ttu-id="96850-151">\*    Solicitar una relación con un cliente</span><span class="sxs-lookup"><span data-stu-id="96850-151">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="96850-152">\*    Administrar clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="96850-152">\*    Manage customer leads</span></span>
||<span data-ttu-id="96850-153">\*    Ver el contrato de cliente</span><span class="sxs-lookup"><span data-stu-id="96850-153">\*    View the customer agreement</span></span>
||<span data-ttu-id="96850-154">\*    Registrar un vendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="96850-154">\*    Register a value-added reseller</span></span>|
|<span data-ttu-id="96850-155">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="96850-155">Helpdesk agent</span></span>| <span data-ttu-id="96850-156">\*    Buscar y ver un cliente</span><span class="sxs-lookup"><span data-stu-id="96850-156">\*    Search for and view a customer</span></span>
||<span data-ttu-id="96850-157">\*    Editar detalles del cliente</span><span class="sxs-lookup"><span data-stu-id="96850-157">\*    Edit customer details</span></span>
||<span data-ttu-id="96850-158">\*    Ayudar a resolver problemas del cliente referentes a la facturación o la administración de las suscripciones</span><span class="sxs-lookup"><span data-stu-id="96850-158">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="96850-159">\*    Solicitar soporte técnico en nombre de los clientes</span><span class="sxs-lookup"><span data-stu-id="96850-159">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="96850-160">\*    Administrar los problemas de suscripción y facturación en nombre de los clientes</span><span class="sxs-lookup"><span data-stu-id="96850-160">\*    Manage subscriptions and billing issues on behalf of customers</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="96850-161">Proveedor del panel de control (CPV).</span><span class="sxs-lookup"><span data-stu-id="96850-161">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="96850-162">(Rol de CSP y rol que no es de AAD)</span><span class="sxs-lookup"><span data-stu-id="96850-162">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="96850-163">Los CPV desarrollan aplicaciones para los partners del Proveedor de soluciones en la nube (CSP) y que así puedan integrar sus sistemas con las API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="96850-163">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="96850-164">**Rol**</span><span class="sxs-lookup"><span data-stu-id="96850-164">**Role**</span></span>   |<span data-ttu-id="96850-165">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="96850-165">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="96850-166">Administrador global</span><span class="sxs-lookup"><span data-stu-id="96850-166">Global admin</span></span>| <span data-ttu-id="96850-167">Ver y administrar el perfil de CPV</span><span class="sxs-lookup"><span data-stu-id="96850-167">View and manage your CPV profile</span></span>|
||<span data-ttu-id="96850-168">Ver y administrar los usuarios que necesiten acceso a las funcionalidades de CPV</span><span class="sxs-lookup"><span data-stu-id="96850-168">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="96850-169">Usuario invitado (debe agregarse al inquilino de AAD)</span><span class="sxs-lookup"><span data-stu-id="96850-169">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="96850-170">**Usuario invitado**</span><span class="sxs-lookup"><span data-stu-id="96850-170">**Guest user**</span></span>   | <span data-ttu-id="96850-171">**Roles**</span><span class="sxs-lookup"><span data-stu-id="96850-171">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="96850-172">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="96850-172">MPN partner admin</span></span>|
||<span data-ttu-id="96850-173">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="96850-173">Accounts admin</span></span>|
||<span data-ttu-id="96850-174">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="96850-174">Incentives admin</span></span>|
||<span data-ttu-id="96850-175">Administrador del perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="96850-175">Business profile admin</span></span>|
||<span data-ttu-id="96850-176">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="96850-176">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="96850-177">Administrar la pertenencia a MPN y su empresa (roles que no son de AAD: estos roles administran el negocio de la empresa en lugar del inquilino)</span><span class="sxs-lookup"><span data-stu-id="96850-177">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="96850-178">**Rol**</span><span class="sxs-lookup"><span data-stu-id="96850-178">**Role**</span></span> | <span data-ttu-id="96850-179">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="96850-179">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="96850-180">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="96850-180">MPN partner admin</span></span>|<span data-ttu-id="96850-181">\*    Ver, crear y administrar las solicitudes de servicio de los asociados</span><span class="sxs-lookup"><span data-stu-id="96850-181">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="96850-182">\*    Ver perfiles legales, de negocios, empresariales y de MPN</span><span class="sxs-lookup"><span data-stu-id="96850-182">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="96850-183">\*    Ver los detalles de los usuarios y sus datos de aptitudes</span><span class="sxs-lookup"><span data-stu-id="96850-183">\*    View user details and their skills data</span></span>
||<span data-ttu-id="96850-184">\*    Ver competencias</span><span class="sxs-lookup"><span data-stu-id="96850-184">\*    View competencies</span></span>
||<span data-ttu-id="96850-185">\*    Ver y administrar ventajas</span><span class="sxs-lookup"><span data-stu-id="96850-185">\*    View and manage benefits</span></span>
||<span data-ttu-id="96850-186">\*    Ver y adquirir ofertas de MPN</span><span class="sxs-lookup"><span data-stu-id="96850-186">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="96850-187">\*    Ver las facturas y el historial de pedidos de ofertas de MPN</span><span class="sxs-lookup"><span data-stu-id="96850-187">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="96850-188">\*    Ver datos de los indicadores de contribución de asociados</span><span class="sxs-lookup"><span data-stu-id="96850-188">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="96850-189">\*    Usar la herramienta de validación de cupones</span><span class="sxs-lookup"><span data-stu-id="96850-189">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="96850-190">\*     Ver análisis de datos de clientes</span><span class="sxs-lookup"><span data-stu-id="96850-190">\*    View customer data analytics</span></span>
||<span data-ttu-id="96850-191">\*    Ver otros roles de usuario dentro de la empresa, pero no puede asignar roles</span><span class="sxs-lookup"><span data-stu-id="96850-191">\*    View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="96850-192">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="96850-192">Account admin</span></span>| <span data-ttu-id="96850-193">• Agregar ubicaciones</span><span class="sxs-lookup"><span data-stu-id="96850-193">Add locations</span></span>
|| <span data-ttu-id="96850-194">• Administrar perfiles relacionados con las cuentas para las que es administrador</span><span class="sxs-lookup"><span data-stu-id="96850-194">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="96850-195">\*    Asignar roles de usuarios del inquilino a roles que no son de AAD</span><span class="sxs-lookup"><span data-stu-id="96850-195">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="96850-196">\*    Inscribir ubicaciones en programas</span><span class="sxs-lookup"><span data-stu-id="96850-196">\*    Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="96850-197">Administrar referencias</span><span class="sxs-lookup"><span data-stu-id="96850-197">Manage referrals</span></span> 

|<span data-ttu-id="96850-198">**Rol**</span><span class="sxs-lookup"><span data-stu-id="96850-198">**Role**</span></span>|<span data-ttu-id="96850-199">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="96850-199">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="96850-200">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="96850-200">Referrals admin</span></span>       |<span data-ttu-id="96850-201">\*    Ver, crear y administrar los perfiles de negocio</span><span class="sxs-lookup"><span data-stu-id="96850-201">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="96850-202">\*    Recibir y administrar referencias</span><span class="sxs-lookup"><span data-stu-id="96850-202">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="96850-203">\*    Ver, crear y administrar referencias de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="96850-203">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="96850-204">\*    Ver, crear y administrar las solicitudes de servicio de los asociados</span><span class="sxs-lookup"><span data-stu-id="96850-204">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="96850-205">Administrador del perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="96850-205">Business profile admin</span></span>   |<span data-ttu-id="96850-206">\*    Ver, crear y administrar el perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="96850-206">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="96850-207">\*    Ver, crear y administrar las solicitudes de servicio de los asociados</span><span class="sxs-lookup"><span data-stu-id="96850-207">\*    View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="96850-208">Administrar incentivos</span><span class="sxs-lookup"><span data-stu-id="96850-208">Manage incentives</span></span> 

|<span data-ttu-id="96850-209">**Rol**</span><span class="sxs-lookup"><span data-stu-id="96850-209">**Role**</span></span> | <span data-ttu-id="96850-210">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="96850-210">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="96850-211">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="96850-211">Incentives admin</span></span>|<span data-ttu-id="96850-212">\*    Iniciar y administrar incentivos</span><span class="sxs-lookup"><span data-stu-id="96850-212">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="96850-213">\*    Ver y editar todos los aspectos de los programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="96850-213">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="96850-214">\*    Ver y editar información bancaria y fiscal</span><span class="sxs-lookup"><span data-stu-id="96850-214">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="96850-215">\*    Ver ganancias de devolución y cooperación</span><span class="sxs-lookup"><span data-stu-id="96850-215">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="96850-216">\*    Acceder a soporte técnico</span><span class="sxs-lookup"><span data-stu-id="96850-216">\*    Access support</span></span>
||<span data-ttu-id="96850-217">\*    Disputar pagos de incentivos</span><span class="sxs-lookup"><span data-stu-id="96850-217">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="96850-218">Usuario de incentivos</span><span class="sxs-lookup"><span data-stu-id="96850-218">Incentives user</span></span>|<span data-ttu-id="96850-219">\*    Ver programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="96850-219">\*    Can view incentives programs</span></span>
||<span data-ttu-id="96850-220">\*    Ver e iniciar reclamaciones de incentivos</span><span class="sxs-lookup"><span data-stu-id="96850-220">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="96850-221">\*    Ver ganancias de devolución y cooperación</span><span class="sxs-lookup"><span data-stu-id="96850-221">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="96850-222">\*    Acceder a soporte técnico</span><span class="sxs-lookup"><span data-stu-id="96850-222">\*    Access support</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="96850-223">Ver datos de conclusiones del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="96850-223">View Partner Center Insights data</span></span>

|<span data-ttu-id="96850-224">**Rol**</span><span class="sxs-lookup"><span data-stu-id="96850-224">**Role**</span></span> | <span data-ttu-id="96850-225">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="96850-225">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="96850-226">Visor de informes ejecutivos</span><span class="sxs-lookup"><span data-stu-id="96850-226">Executive report viewer</span></span>|<span data-ttu-id="96850-227">Acceso a todos los conjuntos de datos de informes</span><span class="sxs-lookup"><span data-stu-id="96850-227">Access to all reporting datasets</span></span>|
|<span data-ttu-id="96850-228">Visor de informes</span><span class="sxs-lookup"><span data-stu-id="96850-228">Report viewer</span></span>|<span data-ttu-id="96850-229">Acceso a informes de datos, a excepción de los ingresos y los datos personales de clientes y empleados</span><span class="sxs-lookup"><span data-stu-id="96850-229">Access to data reports with exception of revenue and customer and employee personal data</span></span>|












                                    