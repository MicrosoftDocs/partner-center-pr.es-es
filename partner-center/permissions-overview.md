---
title: Asignar roles y permisos a los usuarios | Centro de partners
ms.topic: article
ms.date: 3/5/19
description: Todos los empleados que necesiten trabajar en el centro de Partners deben tener asignado un rol.
author: LauraBrenner
ms.author: labrenne
keywords: roles, permisos, admin, agente
ms.localizationpriority: medium
ms.openlocfilehash: 658106548596a5fa7d02d29c0065a23caeacb83d
ms.sourcegitcommit: 59825cb626e12dfe5eb2d28e836b4573368d705e
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/09/2019
ms.locfileid: "67690841"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="7cc08-104">Asignar roles y permisos de usuarios</span><span class="sxs-lookup"><span data-stu-id="7cc08-104">Assign users roles and permissions</span></span>


<span data-ttu-id="7cc08-105">Ha configurado el perfil de socio comercial como nombre legal y dirección, detalles sobre la compatibilidad, exenciones fiscales de archivo, información bancaria y al contacto principal de su empresa.</span><span class="sxs-lookup"><span data-stu-id="7cc08-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="7cc08-106">Siguiente paso: los usuarios configurar con las contraseñas y los roles para que pueden empezar a trabajar en el centro de partners con usted.</span><span class="sxs-lookup"><span data-stu-id="7cc08-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="7cc08-107">Configuración de sus empleados a trabajar en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="7cc08-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="7cc08-108">Determinar los tipos de acceso de los usuarios al centro de partners mediante los roles y permisos que les proporcione.</span><span class="sxs-lookup"><span data-stu-id="7cc08-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="7cc08-109">Roles están relacionados con los programas de en que su empresa está implicada.</span><span class="sxs-lookup"><span data-stu-id="7cc08-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="7cc08-110">Por ejemplo, si su empresa es una proveedor de soluciones en la nube (CSP) de la empresa, no sólo tendrá el estándar de Azure AD roles de administración como administrador global del inquilino, pero será necesario que las funciones específicas del programa CSP.</span><span class="sxs-lookup"><span data-stu-id="7cc08-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="7cc08-111">Cada programa tiene roles específicos a él.</span><span class="sxs-lookup"><span data-stu-id="7cc08-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="7cc08-112">Roles de inquilino de Azure Active Directory (AAD) incluyen el administrador global, Administrador de usuarios y roles CSP.</span><span class="sxs-lookup"><span data-stu-id="7cc08-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="7cc08-113">Roles de AAD de no son los roles que no administran al inquilino, e incluyen administrador MPN, admin de perfil de empresa, Administrador de referencias, incentivo administrador y usuario incentivo.</span><span class="sxs-lookup"><span data-stu-id="7cc08-113">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="7cc08-114">Administrar las transacciones comerciales en el centro de partners (Azure AD y los roles CSP)</span><span class="sxs-lookup"><span data-stu-id="7cc08-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="7cc08-115">**Role**</span><span class="sxs-lookup"><span data-stu-id="7cc08-115">**Role**</span></span>|<span data-ttu-id="7cc08-116">**¿Qué puede hacer.**</span><span class="sxs-lookup"><span data-stu-id="7cc08-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="7cc08-117">Administrador global</span><span class="sxs-lookup"><span data-stu-id="7cc08-117">Global admin</span></span>|<span data-ttu-id="7cc08-118">• Puede tener acceso a todos los cuenta de Microsoft y servicios con privilegios completos</span><span class="sxs-lookup"><span data-stu-id="7cc08-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="7cc08-119">• Crear incidencias de soporte técnico para el centro de partners</span><span class="sxs-lookup"><span data-stu-id="7cc08-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="7cc08-120">• Vista acuerdos, listas de precios y ofertas</span><span class="sxs-lookup"><span data-stu-id="7cc08-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="7cc08-121">• Ver, crear y administrar los usuarios del asociado</span><span class="sxs-lookup"><span data-stu-id="7cc08-121">• View, create, and manage partner users</span></span>|
||  <span data-ttu-id="7cc08-122">Ver, crear y administrar la facturación, facturas y archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="7cc08-122">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="7cc08-123">Administrador de administración de usuarios</span><span class="sxs-lookup"><span data-stu-id="7cc08-123">User management admin</span></span>   | <span data-ttu-id="7cc08-124">• Ver, crear y administrar usuarios</span><span class="sxs-lookup"><span data-stu-id="7cc08-124">•    View, create, and manage users</span></span>
||<span data-ttu-id="7cc08-125">• Ver todos los perfiles de socios comerciales</span><span class="sxs-lookup"><span data-stu-id="7cc08-125">• View all partner profiles</span></span>
||<span data-ttu-id="7cc08-126">• Ver, crear y administrar los usuarios del asociado</span><span class="sxs-lookup"><span data-stu-id="7cc08-126">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="7cc08-127">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="7cc08-127">Billing admin</span></span> | <span data-ttu-id="7cc08-128">-Ver, crear y administrar la facturación, facturas y archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="7cc08-128">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="7cc08-129">Usuario predeterminado</span><span class="sxs-lookup"><span data-stu-id="7cc08-129">Default user</span></span>|  <span data-ttu-id="7cc08-130">Ver mi perfil</span><span class="sxs-lookup"><span data-stu-id="7cc08-130">View My profile</span></span>   |
|<span data-ttu-id="7cc08-131">Agente de administración</span><span class="sxs-lookup"><span data-stu-id="7cc08-131">Admin agent</span></span> | <span data-ttu-id="7cc08-132">• Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="7cc08-132">•    Customer management</span></span>
||<span data-ttu-id="7cc08-133">• Agregue la lista de dispositivos en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="7cc08-133">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="7cc08-134">• Crear y aplicar los perfiles en dispositivos</span><span class="sxs-lookup"><span data-stu-id="7cc08-134">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="7cc08-135">• Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="7cc08-135">• Subscription management</span></span>
||<span data-ttu-id="7cc08-136">• Service health y atender solicitudes de clientes</span><span class="sxs-lookup"><span data-stu-id="7cc08-136">• Service health and service requests for customers</span></span>
||<span data-ttu-id="7cc08-137">• Solicitud delega privilegios de administrador</span><span class="sxs-lookup"><span data-stu-id="7cc08-137">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="7cc08-138">• Ver información sobre precios y ofertas</span><span class="sxs-lookup"><span data-stu-id="7cc08-138">• View pricing and offers</span></span>
||<span data-ttu-id="7cc08-139">• La facturación</span><span class="sxs-lookup"><span data-stu-id="7cc08-139">• Billing</span></span>
||<span data-ttu-id="7cc08-140">• Administrar parte de un cliente</span><span class="sxs-lookup"><span data-stu-id="7cc08-140">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="7cc08-141">• Register un valor agregado reseller</span><span class="sxs-lookup"><span data-stu-id="7cc08-141">• Register a value added reseller</span></span>|
|<span data-ttu-id="7cc08-142">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="7cc08-142">Sales agent</span></span> | <span data-ttu-id="7cc08-143">• Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="7cc08-143">•    Customer management</span></span>
||<span data-ttu-id="7cc08-144">• Agregue la lista de dispositivos en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="7cc08-144">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="7cc08-145">• Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="7cc08-145">• Subscription management</span></span>
||<span data-ttu-id="7cc08-146">Precio de vista • enumera y ofrece</span><span class="sxs-lookup"><span data-stu-id="7cc08-146">• View price lists and offers</span></span>
||<span data-ttu-id="7cc08-147">• Incidencias de soporte técnico de vista</span><span class="sxs-lookup"><span data-stu-id="7cc08-147">• View support tickets</span></span>
||<span data-ttu-id="7cc08-148">• Solicitud una relación con un cliente</span><span class="sxs-lookup"><span data-stu-id="7cc08-148">• Request a relationship with a customer</span></span>
||<span data-ttu-id="7cc08-149">• Administración de clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="7cc08-149">• Manage customer leads</span></span>
||<span data-ttu-id="7cc08-150">• Ver el contrato de cliente</span><span class="sxs-lookup"><span data-stu-id="7cc08-150">• View the customer agreement</span></span>
||<span data-ttu-id="7cc08-151">• Register un revendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="7cc08-151">• Register a value-added reseller</span></span>|
|<span data-ttu-id="7cc08-152">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="7cc08-152">Helpdesk agent</span></span>| <span data-ttu-id="7cc08-153">• Buscar y ver un cliente</span><span class="sxs-lookup"><span data-stu-id="7cc08-153">•  Search for and view a customer</span></span>
||<span data-ttu-id="7cc08-154">• Editar detalles de cliente</span><span class="sxs-lookup"><span data-stu-id="7cc08-154">• Edit customer details</span></span>
||<span data-ttu-id="7cc08-155">• Ayuda resolver al cliente los problemas con la administración de facturación o suscripción</span><span class="sxs-lookup"><span data-stu-id="7cc08-155">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="7cc08-156">• Soporte técnico de solicitud en nombre de los clientes (tenga en cuenta: Debe ser un agente de administración para completar esta tarea para las suscripciones de Office 365)</span><span class="sxs-lookup"><span data-stu-id="7cc08-156">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="7cc08-157">• Administración de suscripciones y facturación problemas en el nombre de los clientes (tenga en cuenta: Debe ser un agente de administración para completar esta tarea para las suscripciones de Office 365)</span><span class="sxs-lookup"><span data-stu-id="7cc08-157">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="7cc08-158">Proveedor del Panel de control (CPV).</span><span class="sxs-lookup"><span data-stu-id="7cc08-158">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="7cc08-159">(Rol CSP y rol sin AAD)</span><span class="sxs-lookup"><span data-stu-id="7cc08-159">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="7cc08-160">CPVs desarrollar aplicaciones para su uso por los asociados de proveedor de soluciones en la nube (CSP) que les permite integrar los sistemas con Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="7cc08-160">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="7cc08-161">**Role**</span><span class="sxs-lookup"><span data-stu-id="7cc08-161">**Role**</span></span>   |<span data-ttu-id="7cc08-162">**¿Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="7cc08-162">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="7cc08-163">Administrador global</span><span class="sxs-lookup"><span data-stu-id="7cc08-163">Global admin</span></span>| <span data-ttu-id="7cc08-164">Ver y administrar su perfil CPV</span><span class="sxs-lookup"><span data-stu-id="7cc08-164">View and manage your CPV profile</span></span>|
||<span data-ttu-id="7cc08-165">Ver y administrar cualquiera de los usuarios que necesitan tener acceso a las funcionalidades de CPV</span><span class="sxs-lookup"><span data-stu-id="7cc08-165">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="7cc08-166">Usuario invitado (debe agregarse al inquilino de AAD)</span><span class="sxs-lookup"><span data-stu-id="7cc08-166">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="7cc08-167">**Usuario invitado**</span><span class="sxs-lookup"><span data-stu-id="7cc08-167">**Guest user**</span></span>   | <span data-ttu-id="7cc08-168">**Roles**</span><span class="sxs-lookup"><span data-stu-id="7cc08-168">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="7cc08-169">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="7cc08-169">MPN partner admin</span></span>|
||<span data-ttu-id="7cc08-170">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="7cc08-170">Accounts admin</span></span>|
||<span data-ttu-id="7cc08-171">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="7cc08-171">Incentives admin</span></span>|
||<span data-ttu-id="7cc08-172">Administrador de perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="7cc08-172">Business profile admin</span></span>|
||<span data-ttu-id="7cc08-173">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="7cc08-173">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="7cc08-174">Administrar la pertenencia a MPN y su empresa (roles no AAD: estos roles de administran el negocio de empresa en lugar de con el inquilino)</span><span class="sxs-lookup"><span data-stu-id="7cc08-174">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="7cc08-175">**Role**</span><span class="sxs-lookup"><span data-stu-id="7cc08-175">**Role**</span></span> | <span data-ttu-id="7cc08-176">**¿Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="7cc08-176">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="7cc08-177">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="7cc08-177">MPN partner admin</span></span>|<span data-ttu-id="7cc08-178">• Ver, crear y administrar solicitudes de servicio asociado</span><span class="sxs-lookup"><span data-stu-id="7cc08-178">•    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="7cc08-179">• Vista legal, empresa, empresariales y perfiles MPN</span><span class="sxs-lookup"><span data-stu-id="7cc08-179">• View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="7cc08-180">• Ver detalles del usuario y sus datos de conocimientos</span><span class="sxs-lookup"><span data-stu-id="7cc08-180">• View user details and their skills data</span></span>
||<span data-ttu-id="7cc08-181">• Competencias de vista</span><span class="sxs-lookup"><span data-stu-id="7cc08-181">• View competencies</span></span>
||<span data-ttu-id="7cc08-182">• Ver y administrar las prestaciones</span><span class="sxs-lookup"><span data-stu-id="7cc08-182">• View and manage benefits</span></span>
||<span data-ttu-id="7cc08-183">Compra y vista • MPN ofrece</span><span class="sxs-lookup"><span data-stu-id="7cc08-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="7cc08-184">• Vista MPN ofrece facturas e historial de pedidos</span><span class="sxs-lookup"><span data-stu-id="7cc08-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="7cc08-185">• Ver datos de indicador de contribución de asociado</span><span class="sxs-lookup"><span data-stu-id="7cc08-185">• View partner contribution indicator data</span></span>
||<span data-ttu-id="7cc08-186">• Puede trabajar en la herramienta de validación del vale</span><span class="sxs-lookup"><span data-stu-id="7cc08-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="7cc08-187">-Ver análisis de datos de clientes</span><span class="sxs-lookup"><span data-stu-id="7cc08-187">- View customer data analytics</span></span>
|| <span data-ttu-id="7cc08-188">Ver otros roles de usuario dentro de la empresa, pero no se puede asignar roles</span><span class="sxs-lookup"><span data-stu-id="7cc08-188">View other user roles within company, but can't assign roles</span></span>
|<span data-ttu-id="7cc08-189">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="7cc08-189">Account admin</span></span>| <span data-ttu-id="7cc08-190">Agregar ubicaciones</span><span class="sxs-lookup"><span data-stu-id="7cc08-190">Add locations</span></span>
|| <span data-ttu-id="7cc08-191">Administrar perfiles de las cuentas de para que Administrador</span><span class="sxs-lookup"><span data-stu-id="7cc08-191">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="7cc08-192">• Asignación de roles para los usuarios de inquilinos para roles de AAD no</span><span class="sxs-lookup"><span data-stu-id="7cc08-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="7cc08-193">• Ubicaciones en programas de inscripción</span><span class="sxs-lookup"><span data-stu-id="7cc08-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="7cc08-194">Administrar referencias</span><span class="sxs-lookup"><span data-stu-id="7cc08-194">Manage referrals</span></span> 

|<span data-ttu-id="7cc08-195">**Role**</span><span class="sxs-lookup"><span data-stu-id="7cc08-195">**Role**</span></span>|<span data-ttu-id="7cc08-196">**¿Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="7cc08-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="7cc08-197">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="7cc08-197">Referrals admin</span></span>       |<span data-ttu-id="7cc08-198">• Ver, crear y administrar perfiles de negocio</span><span class="sxs-lookup"><span data-stu-id="7cc08-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="7cc08-199">• Recibir y administrar las referencias</span><span class="sxs-lookup"><span data-stu-id="7cc08-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="7cc08-200">• Ver, crear y administrar las referencias de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="7cc08-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="7cc08-201">• Ver, crear y administrar solicitudes de servicio asociado</span><span class="sxs-lookup"><span data-stu-id="7cc08-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="7cc08-202">Administrador de perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="7cc08-202">Business profile admin</span></span>   |<span data-ttu-id="7cc08-203">• Ver, crear y administrar el perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="7cc08-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="7cc08-204">• Ver, crear y administrar solicitudes de servicio asociado</span><span class="sxs-lookup"><span data-stu-id="7cc08-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="7cc08-205">Administrar incentivos</span><span class="sxs-lookup"><span data-stu-id="7cc08-205">Manage incentives</span></span> 

|<span data-ttu-id="7cc08-206">**Role**</span><span class="sxs-lookup"><span data-stu-id="7cc08-206">**Role**</span></span> | <span data-ttu-id="7cc08-207">**¿Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="7cc08-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="7cc08-208">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="7cc08-208">Incentives admin</span></span>|<span data-ttu-id="7cc08-209">• Inicia y administra los incentivos</span><span class="sxs-lookup"><span data-stu-id="7cc08-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="7cc08-210">Puede ver y editar todos los aspectos de programas de incentivos •</span><span class="sxs-lookup"><span data-stu-id="7cc08-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="7cc08-211">• Puede ver y editar información bancaria y fiscal</span><span class="sxs-lookup"><span data-stu-id="7cc08-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="7cc08-212">• Beneficios de descuento y Co-op de vista</span><span class="sxs-lookup"><span data-stu-id="7cc08-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="7cc08-213">• Compatibilidad con el acceso</span><span class="sxs-lookup"><span data-stu-id="7cc08-213">• Access support</span></span>
||<span data-ttu-id="7cc08-214">• Los pagos incentivos de conflictos</span><span class="sxs-lookup"><span data-stu-id="7cc08-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="7cc08-215">Usuario de incentivos</span><span class="sxs-lookup"><span data-stu-id="7cc08-215">Incentives user</span></span>|<span data-ttu-id="7cc08-216">• Puede ver los programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="7cc08-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="7cc08-217">• Puede ver e iniciar las notificaciones de incentivos</span><span class="sxs-lookup"><span data-stu-id="7cc08-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="7cc08-218">• Beneficios de descuento y Co-op de vista</span><span class="sxs-lookup"><span data-stu-id="7cc08-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="7cc08-219">• Compatibilidad con el acceso</span><span class="sxs-lookup"><span data-stu-id="7cc08-219">• Access support</span></span>












