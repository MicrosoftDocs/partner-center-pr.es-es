---
title: Asignar roles y permisos a los usuarios | Centro de partners
ms.topic: article
ms.date: 10/10/2019
description: Todos los empleados que necesiten trabajar en el Centro de partners deben tener roles asignados.
author: LauraBrenner
ms.author: labrenne
keywords: roles, permisos, administrador, agente
ms.localizationpriority: high
ms.openlocfilehash: 0bbc9af84b8a1464f255c17147fdc10a7504eb43
ms.sourcegitcommit: 1ccc27092949deb6f6404e64fd6a628fd7b5fd5c
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/11/2019
ms.locfileid: "72276097"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="f5cef-104">Asignar roles y permisos de usuarios</span><span class="sxs-lookup"><span data-stu-id="f5cef-104">Assign users roles and permissions</span></span>


<span data-ttu-id="f5cef-105">Has configurado tu perfil de partner, incluyendo el nombre y la dirección legales, los detalles de soporte técnico, las exenciones fiscales, la información bancaria y el contacto principal de tu empresa.</span><span class="sxs-lookup"><span data-stu-id="f5cef-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="f5cef-106">Siguiente paso: configura tus usuarios con contraseñas y roles para que puedan comenzar a trabajar en el Centro de partners contigo.</span><span class="sxs-lookup"><span data-stu-id="f5cef-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="f5cef-107">Configura a sus empleados para trabajar en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="f5cef-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="f5cef-108">Debes determinar los tipos de acceso que tendrán los usuarios en el Centro de partners, en función de los roles y permisos que les otorgues.</span><span class="sxs-lookup"><span data-stu-id="f5cef-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="f5cef-109">Los roles están relacionados con los programas en los que participa tu empresa.</span><span class="sxs-lookup"><span data-stu-id="f5cef-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="f5cef-110">Por ejemplo, si tu negocio es un Proveedor de soluciones en la nube (CSP), no solo tendrás los roles estándar de administración de inquilinos de Azure AD (como el administrador global), sino que también necesitarás roles específicos para el programa de CSP.</span><span class="sxs-lookup"><span data-stu-id="f5cef-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="f5cef-111">Recuerda que cada programa tiene roles específicos.</span><span class="sxs-lookup"><span data-stu-id="f5cef-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="f5cef-112">Los roles de inquilino de Azure Active Directory (AAD) incluyen roles de administrador global, administrador de usuarios y CSP.</span><span class="sxs-lookup"><span data-stu-id="f5cef-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="f5cef-113">Los roles que no son de AAD son aquellos que no administran al inquilino, e incluyen un administrador de MPN, un administrador de perfil comercial, un administrador de referencias, un administrador de incentivos y un usuario de incentivos.</span><span class="sxs-lookup"><span data-stu-id="f5cef-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="f5cef-114">Administra las transacciones comerciales en el Centro de partners (roles de Azure AD y CSP)</span><span class="sxs-lookup"><span data-stu-id="f5cef-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="f5cef-115">**Rol**</span><span class="sxs-lookup"><span data-stu-id="f5cef-115">**Role**</span></span>|<span data-ttu-id="f5cef-116">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="f5cef-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="f5cef-117">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f5cef-117">Global admin</span></span>|<span data-ttu-id="f5cef-118">• Obtener acceso a todas las cuentas o servicios de Microsoft con privilegios completos</span><span class="sxs-lookup"><span data-stu-id="f5cef-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="f5cef-119">• Crear vales de soporte técnico para el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="f5cef-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="f5cef-120">• Ver contratos, listas de precios y ofertas</span><span class="sxs-lookup"><span data-stu-id="f5cef-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="f5cef-121">• Ver, crear y administrar los usuarios de partners</span><span class="sxs-lookup"><span data-stu-id="f5cef-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="f5cef-122">• Ver, crear y administrar los archivos de facturación, facturas y conciliación</span><span class="sxs-lookup"><span data-stu-id="f5cef-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="f5cef-123">Administrador de administración de usuarios</span><span class="sxs-lookup"><span data-stu-id="f5cef-123">User management admin</span></span>   | <span data-ttu-id="f5cef-124">• Ver, crear y administrar usuarios</span><span class="sxs-lookup"><span data-stu-id="f5cef-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="f5cef-125">• Ver todos los perfiles de partners</span><span class="sxs-lookup"><span data-stu-id="f5cef-125">• View all partner profiles</span></span>
||<span data-ttu-id="f5cef-126">• Ver, crear y administrar los usuarios de partners</span><span class="sxs-lookup"><span data-stu-id="f5cef-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="f5cef-127">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="f5cef-127">Billing admin</span></span> | <span data-ttu-id="f5cef-128">• Ver, crear y administrar los archivos de facturación, facturas y conciliación</span><span class="sxs-lookup"><span data-stu-id="f5cef-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="f5cef-129">Usuario predeterminado</span><span class="sxs-lookup"><span data-stu-id="f5cef-129">Default user</span></span>|  <span data-ttu-id="f5cef-130">Ver mi perfil</span><span class="sxs-lookup"><span data-stu-id="f5cef-130">View My profile</span></span>   |
|<span data-ttu-id="f5cef-131">Agente de administración</span><span class="sxs-lookup"><span data-stu-id="f5cef-131">Admin agent</span></span> | <span data-ttu-id="f5cef-132">• Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="f5cef-132">•    Customer management</span></span>
||<span data-ttu-id="f5cef-133">• Agregar una lista de dispositivos en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="f5cef-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="f5cef-134">• Crear y aplicar los perfiles a los dispositivos</span><span class="sxs-lookup"><span data-stu-id="f5cef-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="f5cef-135">• Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="f5cef-135">• Subscription management</span></span>
||<span data-ttu-id="f5cef-136">• Comprobar el estado del servicio y las solicitudes de servicio para clientes</span><span class="sxs-lookup"><span data-stu-id="f5cef-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="f5cef-137">• Solicitar privilegios de administrador delegado</span><span class="sxs-lookup"><span data-stu-id="f5cef-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="f5cef-138">• Ver los precios y las ofertas</span><span class="sxs-lookup"><span data-stu-id="f5cef-138">• View pricing and offers</span></span>
||<span data-ttu-id="f5cef-139">• Facturación</span><span class="sxs-lookup"><span data-stu-id="f5cef-139">• Billing</span></span>
||<span data-ttu-id="f5cef-140">• Administrar contenido en nombre de un cliente</span><span class="sxs-lookup"><span data-stu-id="f5cef-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="f5cef-141">• Registrar un vendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="f5cef-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="f5cef-142">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="f5cef-142">Sales agent</span></span> | <span data-ttu-id="f5cef-143">• Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="f5cef-143">•    Customer management</span></span>
||<span data-ttu-id="f5cef-144">• Agregar una lista de dispositivos en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="f5cef-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="f5cef-145">• Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="f5cef-145">• Subscription management</span></span>
||<span data-ttu-id="f5cef-146">• Ver vales de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="f5cef-146">• View support tickets</span></span>
||<span data-ttu-id="f5cef-147">• Solicitar la relación con un cliente</span><span class="sxs-lookup"><span data-stu-id="f5cef-147">• Request a relationship with a customer</span></span>
||<span data-ttu-id="f5cef-148">• Administrar clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="f5cef-148">• Manage customer leads</span></span>
||<span data-ttu-id="f5cef-149">• Ver el contrato de cliente</span><span class="sxs-lookup"><span data-stu-id="f5cef-149">• View the customer agreement</span></span>
||<span data-ttu-id="f5cef-150">• Registrar un vendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="f5cef-150">• Register a value-added reseller</span></span>|
|<span data-ttu-id="f5cef-151">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="f5cef-151">Helpdesk agent</span></span>| <span data-ttu-id="f5cef-152">• Buscar y ver un cliente</span><span class="sxs-lookup"><span data-stu-id="f5cef-152">•  Search for and view a customer</span></span>
||<span data-ttu-id="f5cef-153">• Editar detalles del cliente</span><span class="sxs-lookup"><span data-stu-id="f5cef-153">• Edit customer details</span></span>
||<span data-ttu-id="f5cef-154">• Ayudar a resolver problemas del cliente referentes a la facturación o la administración de las suscripciones</span><span class="sxs-lookup"><span data-stu-id="f5cef-154">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="f5cef-155">• Solicitar soporte técnico en nombre de los clientes (Nota: Debes ser un agente de administración para poder completar esta tarea en las suscripciones de Office 365)</span><span class="sxs-lookup"><span data-stu-id="f5cef-155">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="f5cef-156">• Administrar los problemas de suscripción y facturación en nombre de los clientes (Nota: Debes ser un agente de administración para poder completar esta tarea en las suscripciones de Office 365)</span><span class="sxs-lookup"><span data-stu-id="f5cef-156">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="f5cef-157">Proveedor del panel de control (CPV).</span><span class="sxs-lookup"><span data-stu-id="f5cef-157">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="f5cef-158">(Rol de CSP y rol que no es de AAD)</span><span class="sxs-lookup"><span data-stu-id="f5cef-158">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="f5cef-159">Los CPV desarrollan aplicaciones para los partners del Proveedor de soluciones en la nube (CSP) y que así puedan integrar sus sistemas con las API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="f5cef-159">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="f5cef-160">**Rol**</span><span class="sxs-lookup"><span data-stu-id="f5cef-160">**Role**</span></span>   |<span data-ttu-id="f5cef-161">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="f5cef-161">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="f5cef-162">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f5cef-162">Global admin</span></span>| <span data-ttu-id="f5cef-163">Ver y administrar el perfil de CPV</span><span class="sxs-lookup"><span data-stu-id="f5cef-163">View and manage your CPV profile</span></span>|
||<span data-ttu-id="f5cef-164">Ver y administrar los usuarios que necesiten acceso a las funcionalidades de CPV</span><span class="sxs-lookup"><span data-stu-id="f5cef-164">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="f5cef-165">Usuario invitado (debe agregarse al inquilino de AAD)</span><span class="sxs-lookup"><span data-stu-id="f5cef-165">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="f5cef-166">**Usuario invitado**</span><span class="sxs-lookup"><span data-stu-id="f5cef-166">**Guest user**</span></span>   | <span data-ttu-id="f5cef-167">**Roles**</span><span class="sxs-lookup"><span data-stu-id="f5cef-167">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="f5cef-168">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="f5cef-168">MPN partner admin</span></span>|
||<span data-ttu-id="f5cef-169">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="f5cef-169">Accounts admin</span></span>|
||<span data-ttu-id="f5cef-170">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="f5cef-170">Incentives admin</span></span>|
||<span data-ttu-id="f5cef-171">Administrador del perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="f5cef-171">Business profile admin</span></span>|
||<span data-ttu-id="f5cef-172">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="f5cef-172">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="f5cef-173">Administrar la pertenencia a MPN y su empresa (roles que no son de AAD: estos roles administran el negocio de la empresa en lugar del inquilino)</span><span class="sxs-lookup"><span data-stu-id="f5cef-173">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="f5cef-174">**Rol**</span><span class="sxs-lookup"><span data-stu-id="f5cef-174">**Role**</span></span> | <span data-ttu-id="f5cef-175">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="f5cef-175">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="f5cef-176">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="f5cef-176">MPN partner admin</span></span>|<span data-ttu-id="f5cef-177">• Ver, crear y administrar las solicitudes de servicio de los partners</span><span class="sxs-lookup"><span data-stu-id="f5cef-177">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="f5cef-178">• Ver perfiles legales, de negocios, empresariales y de MPN</span><span class="sxs-lookup"><span data-stu-id="f5cef-178">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="f5cef-179">• Ver los detalles de los usuarios y sus datos de habilidades</span><span class="sxs-lookup"><span data-stu-id="f5cef-179">• View user details and their skills data</span></span>
||<span data-ttu-id="f5cef-180">• Ver competencias</span><span class="sxs-lookup"><span data-stu-id="f5cef-180">• View competencies</span></span>
||<span data-ttu-id="f5cef-181">• Ver y administrar ventajas</span><span class="sxs-lookup"><span data-stu-id="f5cef-181">• View and manage benefits</span></span>
||<span data-ttu-id="f5cef-182">• Ver y adquirir ofertas de MPN</span><span class="sxs-lookup"><span data-stu-id="f5cef-182">• View and purchase MPN offers</span></span>
||<span data-ttu-id="f5cef-183">• Ver facturas e historial de pedidos de ofertas de MPN</span><span class="sxs-lookup"><span data-stu-id="f5cef-183">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="f5cef-184">• Ver datos de los indicadores de contribución de partners</span><span class="sxs-lookup"><span data-stu-id="f5cef-184">• View partner contribution indicator data</span></span>
||<span data-ttu-id="f5cef-185">• Usar la herramienta de validación de comprobantes</span><span class="sxs-lookup"><span data-stu-id="f5cef-185">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="f5cef-186">• Ver el análisis de datos de clientes</span><span class="sxs-lookup"><span data-stu-id="f5cef-186">- View customer data analytics</span></span>
|| <span data-ttu-id="f5cef-187">• Ver otros roles de usuario dentro de la empresa, pero no puede asignar roles</span><span class="sxs-lookup"><span data-stu-id="f5cef-187">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="f5cef-188">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="f5cef-188">Account admin</span></span>| <span data-ttu-id="f5cef-189">• Agregar ubicaciones</span><span class="sxs-lookup"><span data-stu-id="f5cef-189">Add locations</span></span>
|| <span data-ttu-id="f5cef-190">• Administrar perfiles relacionados con las cuentas para las que es administrador</span><span class="sxs-lookup"><span data-stu-id="f5cef-190">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="f5cef-191">• Asignar roles para usuarios en el inquilino con roles que no sean de AAD</span><span class="sxs-lookup"><span data-stu-id="f5cef-191">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="f5cef-192">• Inscribir ubicaciones en programas</span><span class="sxs-lookup"><span data-stu-id="f5cef-192">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="f5cef-193">Administrar referencias</span><span class="sxs-lookup"><span data-stu-id="f5cef-193">Manage referrals</span></span> 

|<span data-ttu-id="f5cef-194">**Rol**</span><span class="sxs-lookup"><span data-stu-id="f5cef-194">**Role**</span></span>|<span data-ttu-id="f5cef-195">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="f5cef-195">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="f5cef-196">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="f5cef-196">Referrals admin</span></span>       |<span data-ttu-id="f5cef-197">• Ver, crear y administrar los perfiles de negocio</span><span class="sxs-lookup"><span data-stu-id="f5cef-197">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="f5cef-198">• Recibir y administrar las referencias</span><span class="sxs-lookup"><span data-stu-id="f5cef-198">• Receive and manage referrals</span></span>
||<span data-ttu-id="f5cef-199">• Ver, crear y administrar referencias de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="f5cef-199">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="f5cef-200">• Ver, crear y administrar las solicitudes de servicio de los partners</span><span class="sxs-lookup"><span data-stu-id="f5cef-200">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="f5cef-201">Administrador del perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="f5cef-201">Business profile admin</span></span>   |<span data-ttu-id="f5cef-202">• Ver, crear y administrar el perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="f5cef-202">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="f5cef-203">• Ver, crear y administrar las solicitudes de servicio de los partners</span><span class="sxs-lookup"><span data-stu-id="f5cef-203">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="f5cef-204">Administrar incentivos</span><span class="sxs-lookup"><span data-stu-id="f5cef-204">Manage incentives</span></span> 

|<span data-ttu-id="f5cef-205">**Rol**</span><span class="sxs-lookup"><span data-stu-id="f5cef-205">**Role**</span></span> | <span data-ttu-id="f5cef-206">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="f5cef-206">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="f5cef-207">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="f5cef-207">Incentives admin</span></span>|<span data-ttu-id="f5cef-208">• Inicia y administra incentivos</span><span class="sxs-lookup"><span data-stu-id="f5cef-208">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="f5cef-209">• Puede ver y editar todos los aspectos de programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="f5cef-209">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="f5cef-210">• Puede ver y editar información bancaria y fiscal</span><span class="sxs-lookup"><span data-stu-id="f5cef-210">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="f5cef-211">• Ver ganancias de reembolso y cooperación</span><span class="sxs-lookup"><span data-stu-id="f5cef-211">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="f5cef-212">• Acceso a soporte técnico</span><span class="sxs-lookup"><span data-stu-id="f5cef-212">• Access support</span></span>
||<span data-ttu-id="f5cef-213">• Disputar pagos de incentivos</span><span class="sxs-lookup"><span data-stu-id="f5cef-213">• Dispute incentives payments</span></span>|
|<span data-ttu-id="f5cef-214">Usuario de incentivos</span><span class="sxs-lookup"><span data-stu-id="f5cef-214">Incentives user</span></span>|<span data-ttu-id="f5cef-215">• Puede ver programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="f5cef-215">•  Can view incentives programs</span></span>
||<span data-ttu-id="f5cef-216">• Puede ver e iniciar reclamaciones de incentivos</span><span class="sxs-lookup"><span data-stu-id="f5cef-216">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="f5cef-217">• Ver ganancias de reembolso y cooperación</span><span class="sxs-lookup"><span data-stu-id="f5cef-217">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="f5cef-218">• Acceso a soporte técnico</span><span class="sxs-lookup"><span data-stu-id="f5cef-218">• Access support</span></span>












