---
title: Asignar roles y permisos a los usuarios | Centro de partners
ms.topic: article
ms.date: 3/5/19
description: Todos los empleados que necesiten trabajar en el centro de Partners deben tener asignado un rol.
author: LauraBrenner
ms.author: labrenne
keywords: roles, permisos, admin, agente
ms.localizationpriority: medium
ms.openlocfilehash: 65a2f7f373fc57f86cfffa73aafd3b7095fe2c04
ms.sourcegitcommit: be8086534ec73937f2be9bcc495c2627423c50f6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/26/2019
ms.locfileid: "67396728"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="12340-104">Asignar roles y permisos de usuarios</span><span class="sxs-lookup"><span data-stu-id="12340-104">Assign users roles and permissions</span></span>


<span data-ttu-id="12340-105">Ha configurado el perfil de socio comercial como nombre legal y dirección, detalles sobre la compatibilidad, exenciones fiscales de archivo, información bancaria y al contacto principal de su empresa.</span><span class="sxs-lookup"><span data-stu-id="12340-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="12340-106">Siguiente paso: los usuarios configurar con las contraseñas y los roles para que pueden empezar a trabajar en el centro de partners con usted.</span><span class="sxs-lookup"><span data-stu-id="12340-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="12340-107">Configuración de sus empleados a trabajar en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="12340-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="12340-108">Determinar los tipos de acceso de los usuarios al centro de partners mediante los roles y permisos que les proporcione.</span><span class="sxs-lookup"><span data-stu-id="12340-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="12340-109">Roles están relacionados con los programas de en que su empresa está implicada.</span><span class="sxs-lookup"><span data-stu-id="12340-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="12340-110">Por ejemplo, si su empresa es una proveedor de soluciones en la nube (CSP) de la empresa, no sólo tendrá el estándar de Azure AD roles de administración como administrador global del inquilino, pero será necesario que las funciones específicas del programa CSP.</span><span class="sxs-lookup"><span data-stu-id="12340-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="12340-111">Cada programa tiene roles específicos a él.</span><span class="sxs-lookup"><span data-stu-id="12340-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="12340-112">Roles de inquilino de Azure Active Directory (AAD) incluyen el administrador global, Administrador de usuarios y roles CSP.</span><span class="sxs-lookup"><span data-stu-id="12340-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="12340-113">Roles de AAD de no son los roles que no administran al inquilino e incluyen administrador MPN, admin de perfil de empresa, Administrador de referencias, incentivo administrador y usuario incentivo.</span><span class="sxs-lookup"><span data-stu-id="12340-113">Non-AAD roles are those roles that do not manage the tenant and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="12340-114">Administrar las transacciones comerciales en el centro de partners (Azure AD y los roles CSP)</span><span class="sxs-lookup"><span data-stu-id="12340-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="12340-115">**Role**</span><span class="sxs-lookup"><span data-stu-id="12340-115">**Role**</span></span>|<span data-ttu-id="12340-116">**¿Qué puede hacer.**</span><span class="sxs-lookup"><span data-stu-id="12340-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="12340-117">Administrador global</span><span class="sxs-lookup"><span data-stu-id="12340-117">Global admin</span></span>|<span data-ttu-id="12340-118">• Puede tener acceso a todos los cuenta de Microsoft y servicios con privilegios completos</span><span class="sxs-lookup"><span data-stu-id="12340-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="12340-119">• Crear incidencias de soporte técnico para el centro de partners</span><span class="sxs-lookup"><span data-stu-id="12340-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="12340-120">• Vista acuerdos, listas de precios y ofertas</span><span class="sxs-lookup"><span data-stu-id="12340-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="12340-121">• Ver, crear y administrar los usuarios del asociado</span><span class="sxs-lookup"><span data-stu-id="12340-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="12340-122">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="12340-122">User Admin</span></span>   | <span data-ttu-id="12340-123">• Ver, crear y administrar usuarios</span><span class="sxs-lookup"><span data-stu-id="12340-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="12340-124">• Ver todos los perfiles de socios comerciales</span><span class="sxs-lookup"><span data-stu-id="12340-124">• View all partner profiles</span></span>
||<span data-ttu-id="12340-125">• Ver, crear y administrar los usuarios del asociado</span><span class="sxs-lookup"><span data-stu-id="12340-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="12340-126">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="12340-126">Billing admin</span></span> | <span data-ttu-id="12340-127">-Ver, crear y administrar la facturación, facturas y archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="12340-127">- View, create, and manage billing, invoices, and recon files</span></span>|
|<span data-ttu-id="12340-128">Usuario predeterminado</span><span class="sxs-lookup"><span data-stu-id="12340-128">Default user</span></span>|  <span data-ttu-id="12340-129">Ver mi perfil</span><span class="sxs-lookup"><span data-stu-id="12340-129">View My profile</span></span>   |
|<span data-ttu-id="12340-130">Agente de administración</span><span class="sxs-lookup"><span data-stu-id="12340-130">Admin agent</span></span> | <span data-ttu-id="12340-131">• Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="12340-131">•    Customer management</span></span>
||<span data-ttu-id="12340-132">• Agregue la lista de dispositivos en el centro de partners <</span><span class="sxs-lookup"><span data-stu-id="12340-132">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="12340-133">• Crear y aplicar los perfiles en dispositivos</span><span class="sxs-lookup"><span data-stu-id="12340-133">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="12340-134">• Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="12340-134">• Subscription management</span></span>
||<span data-ttu-id="12340-135">• Service health y atender solicitudes de clientes</span><span class="sxs-lookup"><span data-stu-id="12340-135">• Service health and service requests for customers</span></span>
||<span data-ttu-id="12340-136">• Solicitud delega privilegios de administrador</span><span class="sxs-lookup"><span data-stu-id="12340-136">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="12340-137">• Ver información sobre precios y ofertas</span><span class="sxs-lookup"><span data-stu-id="12340-137">• View pricing and offers</span></span>
||<span data-ttu-id="12340-138">• La facturación</span><span class="sxs-lookup"><span data-stu-id="12340-138">• Billing</span></span>
||<span data-ttu-id="12340-139">• Administrar parte de un cliente</span><span class="sxs-lookup"><span data-stu-id="12340-139">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="12340-140">• Register un valor agregado reseller</span><span class="sxs-lookup"><span data-stu-id="12340-140">• Register a value added reseller</span></span>|
|<span data-ttu-id="12340-141">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="12340-141">Sales agent</span></span> | <span data-ttu-id="12340-142">• Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="12340-142">•    Customer management</span></span>
||<span data-ttu-id="12340-143">• Agregue la lista de dispositivos en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="12340-143">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="12340-144">• Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="12340-144">• Subscription management</span></span>
||<span data-ttu-id="12340-145">Precio de vista • enumera y ofrece</span><span class="sxs-lookup"><span data-stu-id="12340-145">• View price lists and offers</span></span>
||<span data-ttu-id="12340-146">• Incidencias de soporte técnico de vista</span><span class="sxs-lookup"><span data-stu-id="12340-146">• View support tickets</span></span>
||<span data-ttu-id="12340-147">• Solicitud una relación con un cliente</span><span class="sxs-lookup"><span data-stu-id="12340-147">• Request a relationship with a customer</span></span>
||<span data-ttu-id="12340-148">• Administración de clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="12340-148">• Manage customer leads</span></span>
||<span data-ttu-id="12340-149">• Ver el contrato de cliente</span><span class="sxs-lookup"><span data-stu-id="12340-149">• View the customer agreement</span></span>
||<span data-ttu-id="12340-150">• Register un revendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="12340-150">• Register a value-added reseller</span></span>|
|<span data-ttu-id="12340-151">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="12340-151">Helpdesk agent</span></span>| <span data-ttu-id="12340-152">• Buscar y ver un cliente</span><span class="sxs-lookup"><span data-stu-id="12340-152">•  Search for and view a customer</span></span>
||<span data-ttu-id="12340-153">• Editar detalles de cliente</span><span class="sxs-lookup"><span data-stu-id="12340-153">• Edit customer details</span></span>
||<span data-ttu-id="12340-154">• Ayuda resolver al cliente los problemas con la administración de facturación o suscripción</span><span class="sxs-lookup"><span data-stu-id="12340-154">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="12340-155">• Soporte técnico de solicitud en nombre de los clientes (tenga en cuenta: Debe ser un agente de administración para completar esta tarea para las suscripciones de Office 365)</span><span class="sxs-lookup"><span data-stu-id="12340-155">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="12340-156">• Administración de suscripciones y facturación problemas en el nombre de los clientes (tenga en cuenta: Debe ser un agente de administración para completar esta tarea para las suscripciones de Office 365)</span><span class="sxs-lookup"><span data-stu-id="12340-156">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="12340-157">Proveedor del Panel de control (CPV).</span><span class="sxs-lookup"><span data-stu-id="12340-157">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="12340-158">(Rol CSP y rol sin AAD)</span><span class="sxs-lookup"><span data-stu-id="12340-158">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="12340-159">CPVs desarrollar aplicaciones para su uso por los asociados de proveedor de soluciones en la nube (CSP) que les permite integrar los sistemas con Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="12340-159">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="12340-160">**Role**</span><span class="sxs-lookup"><span data-stu-id="12340-160">**Role**</span></span>   |<span data-ttu-id="12340-161">**¿Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="12340-161">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="12340-162">Administrador global</span><span class="sxs-lookup"><span data-stu-id="12340-162">Global admin</span></span>| <span data-ttu-id="12340-163">Ver y administrar su perfil CPV</span><span class="sxs-lookup"><span data-stu-id="12340-163">View and manage your CPV profile</span></span>|
||<span data-ttu-id="12340-164">Ver y administrar cualquiera de los usuarios que necesitan tener acceso a las funcionalidades de CPV</span><span class="sxs-lookup"><span data-stu-id="12340-164">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="12340-165">Usuario invitado (debe agregarse al inquilino de AAD)</span><span class="sxs-lookup"><span data-stu-id="12340-165">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="12340-166">**Usuario invitado**</span><span class="sxs-lookup"><span data-stu-id="12340-166">**Guest user**</span></span>   | <span data-ttu-id="12340-167">**Roles**</span><span class="sxs-lookup"><span data-stu-id="12340-167">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="12340-168">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="12340-168">MPN partner admin</span></span>|
||<span data-ttu-id="12340-169">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="12340-169">Accounts admin</span></span>|
||<span data-ttu-id="12340-170">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="12340-170">Incentives admin</span></span>|
||<span data-ttu-id="12340-171">Administrador de perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="12340-171">Business profile admin</span></span>|
||<span data-ttu-id="12340-172">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="12340-172">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="12340-173">Administrar la pertenencia a MPN y su empresa (roles no AAD: estos roles de administran el negocio de empresa en lugar de con el inquilino)</span><span class="sxs-lookup"><span data-stu-id="12340-173">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="12340-174">**Role**</span><span class="sxs-lookup"><span data-stu-id="12340-174">**Role**</span></span> | <span data-ttu-id="12340-175">**¿Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="12340-175">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="12340-176">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="12340-176">MPN partner admin</span></span>|<span data-ttu-id="12340-177">•CAN agregar los usuarios que no sean inquilinos</span><span class="sxs-lookup"><span data-stu-id="12340-177">•Can add non-tenant users</span></span>
||<span data-ttu-id="12340-178">• Ver, crear y administrar solicitudes de servicio asociado</span><span class="sxs-lookup"><span data-stu-id="12340-178">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="12340-179">• Vista legal, organización, empresariales y perfiles MPN</span><span class="sxs-lookup"><span data-stu-id="12340-179">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="12340-180">• Ver detalles del usuario y sus datos de conocimientos</span><span class="sxs-lookup"><span data-stu-id="12340-180">• View user details and their skills data</span></span>
||<span data-ttu-id="12340-181">• Competencias de vista</span><span class="sxs-lookup"><span data-stu-id="12340-181">• View competencies</span></span>
||<span data-ttu-id="12340-182">• Ver y administrar las prestaciones</span><span class="sxs-lookup"><span data-stu-id="12340-182">• View and manage benefits</span></span>
||<span data-ttu-id="12340-183">Compra y vista • MPN ofrece</span><span class="sxs-lookup"><span data-stu-id="12340-183">• View and purchase MPN offers</span></span>
||<span data-ttu-id="12340-184">• Vista MPN ofrece facturas e historial de pedidos</span><span class="sxs-lookup"><span data-stu-id="12340-184">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="12340-185">• Ver datos de contribución de asociado</span><span class="sxs-lookup"><span data-stu-id="12340-185">• View partner contribution data</span></span>
||<span data-ttu-id="12340-186">• Puede trabajar en la herramienta de validación del vale</span><span class="sxs-lookup"><span data-stu-id="12340-186">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="12340-187">-Ver análisis de datos de clientes</span><span class="sxs-lookup"><span data-stu-id="12340-187">- View customer data analytics</span></span>
|<span data-ttu-id="12340-188">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="12340-188">Account admin</span></span>| <span data-ttu-id="12340-189">• Puede agregar los usuarios que no sean inquilinos</span><span class="sxs-lookup"><span data-stu-id="12340-189">•   Can add non-tenant users</span></span>
||<span data-ttu-id="12340-190">• Agregar o eliminar las ubicaciones</span><span class="sxs-lookup"><span data-stu-id="12340-190">• Add or delete locations</span></span>
||<span data-ttu-id="12340-191">-Administración de perfiles de las cuentas de para que Administrador</span><span class="sxs-lookup"><span data-stu-id="12340-191">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="12340-192">• Asignación de roles para los usuarios de inquilinos para roles de AAD no</span><span class="sxs-lookup"><span data-stu-id="12340-192">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="12340-193">• Ubicaciones en programas de inscripción</span><span class="sxs-lookup"><span data-stu-id="12340-193">• Enroll locations into programs</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="12340-194">Administrar referencias</span><span class="sxs-lookup"><span data-stu-id="12340-194">Manage referrals</span></span> 

|<span data-ttu-id="12340-195">**Role**</span><span class="sxs-lookup"><span data-stu-id="12340-195">**Role**</span></span>|<span data-ttu-id="12340-196">**¿Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="12340-196">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="12340-197">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="12340-197">Referrals admin</span></span>       |<span data-ttu-id="12340-198">• Ver, crear y administrar perfiles de negocio</span><span class="sxs-lookup"><span data-stu-id="12340-198">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="12340-199">• Recibir y administrar las referencias</span><span class="sxs-lookup"><span data-stu-id="12340-199">• Receive and manage referrals</span></span>
||<span data-ttu-id="12340-200">• Ver, crear y administrar las referencias de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="12340-200">• View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="12340-201">• Ver, crear y administrar solicitudes de servicio asociado</span><span class="sxs-lookup"><span data-stu-id="12340-201">• View, create, and manage partner service requests</span></span>
|<span data-ttu-id="12340-202">Administrador de perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="12340-202">Business profile admin</span></span>   |<span data-ttu-id="12340-203">• Ver, crear y administrar el perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="12340-203">• View, create, and manage business profile</span></span> 
||<span data-ttu-id="12340-204">• Ver, crear y administrar solicitudes de servicio asociado</span><span class="sxs-lookup"><span data-stu-id="12340-204">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="12340-205">Administrar incentivos</span><span class="sxs-lookup"><span data-stu-id="12340-205">Manage incentives</span></span> 

|<span data-ttu-id="12340-206">**Role**</span><span class="sxs-lookup"><span data-stu-id="12340-206">**Role**</span></span> | <span data-ttu-id="12340-207">**¿Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="12340-207">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="12340-208">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="12340-208">Incentives admin</span></span>|<span data-ttu-id="12340-209">• Inicia y administra los incentivos</span><span class="sxs-lookup"><span data-stu-id="12340-209">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="12340-210">Puede ver y editar todos los aspectos de programas de incentivos •</span><span class="sxs-lookup"><span data-stu-id="12340-210">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="12340-211">• Puede ver y editar información bancaria y fiscal</span><span class="sxs-lookup"><span data-stu-id="12340-211">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="12340-212">• Beneficios de descuento y Co-op de vista</span><span class="sxs-lookup"><span data-stu-id="12340-212">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="12340-213">• Compatibilidad con el acceso</span><span class="sxs-lookup"><span data-stu-id="12340-213">• Access support</span></span>
||<span data-ttu-id="12340-214">• Los pagos incentivos de conflictos</span><span class="sxs-lookup"><span data-stu-id="12340-214">• Dispute incentives payments</span></span>|
|<span data-ttu-id="12340-215">Usuario de incentivos</span><span class="sxs-lookup"><span data-stu-id="12340-215">Incentives user</span></span>|<span data-ttu-id="12340-216">• Puede ver los programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="12340-216">•  Can view incentives programs</span></span>
||<span data-ttu-id="12340-217">• Puede ver e iniciar las notificaciones de incentivos</span><span class="sxs-lookup"><span data-stu-id="12340-217">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="12340-218">• Beneficios de descuento y Co-op de vista</span><span class="sxs-lookup"><span data-stu-id="12340-218">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="12340-219">• Beneficios de descuento y Co-op de vista</span><span class="sxs-lookup"><span data-stu-id="12340-219">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="12340-220">• Compatibilidad con el acceso</span><span class="sxs-lookup"><span data-stu-id="12340-220">• Access support</span></span>












