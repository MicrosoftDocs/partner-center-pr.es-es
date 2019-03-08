---
title: Asignar roles y permisos a los usuarios | Centro de partners
ms.topic: article
ms.date: 10/29/2018
description: Todos los empleados que necesiten trabajar en el centro de Partners deben tener asignado un rol.
author: LauraBrenner
ms.author: labrenne
keywords: roles, permisos, admin, agente
ms.localizationpriority: medium
ms.openlocfilehash: 038a2d6f4d58bbd9a71a2b241ee68982e0e7ef0a
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587748"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="616d8-104">Asignar roles y permisos de usuarios</span><span class="sxs-lookup"><span data-stu-id="616d8-104">Assign users roles and permissions</span></span>


<span data-ttu-id="616d8-105">Ha configurado el perfil de socio comercial como nombre legal y dirección, detalles sobre la compatibilidad, exenciones fiscales de archivo, información bancaria y al contacto principal de su empresa.</span><span class="sxs-lookup"><span data-stu-id="616d8-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="616d8-106">Siguiente paso: los usuarios configurar con las contraseñas y los roles para que pueden empezar a trabajar en el centro de partners con usted.</span><span class="sxs-lookup"><span data-stu-id="616d8-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="616d8-107">Configuración de sus empleados a trabajar en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="616d8-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="616d8-108">Determinar los tipos de acceso de los usuarios al centro de partners mediante los roles y permisos que les proporcione.</span><span class="sxs-lookup"><span data-stu-id="616d8-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="616d8-109">Roles están relacionados con los programas de en que su empresa está implicada.</span><span class="sxs-lookup"><span data-stu-id="616d8-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="616d8-110">Por ejemplo, si su empresa es una proveedor de soluciones en la nube (CSP) de la empresa, no sólo tendrá el estándar de Azure AD roles de administración como administrador global del inquilino, pero será necesario que las funciones específicas del programa CSP.</span><span class="sxs-lookup"><span data-stu-id="616d8-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="616d8-111">Cada programa tiene roles específicos a él.</span><span class="sxs-lookup"><span data-stu-id="616d8-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="616d8-112">Roles de inquilino de Azure Active Directory (AAD) incluyen el administrador global, Administrador de usuarios y roles CSP.</span><span class="sxs-lookup"><span data-stu-id="616d8-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="616d8-113">Roles de AAD de no incluyen MPN admin, admin de perfil de empresa, Administrador de referencias, incentivo administrador y usuario incentivo.</span><span class="sxs-lookup"><span data-stu-id="616d8-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="616d8-114">Administrar las transacciones comerciales en el centro de partners (Azure AD y los roles CSP)</span><span class="sxs-lookup"><span data-stu-id="616d8-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="616d8-115">**Role**</span><span class="sxs-lookup"><span data-stu-id="616d8-115">**Role**</span></span>|<span data-ttu-id="616d8-116">**¿Qué puede hacer.**</span><span class="sxs-lookup"><span data-stu-id="616d8-116">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="616d8-117">Administrador global</span><span class="sxs-lookup"><span data-stu-id="616d8-117">Global admin</span></span>|<span data-ttu-id="616d8-118">• Puede tener acceso a todos los cuenta de Microsoft y servicios con privilegios completos</span><span class="sxs-lookup"><span data-stu-id="616d8-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="616d8-119">• Crear incidencias de soporte técnico para el centro de partners</span><span class="sxs-lookup"><span data-stu-id="616d8-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="616d8-120">• Vista acuerdos, listas de precios y ofertas</span><span class="sxs-lookup"><span data-stu-id="616d8-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="616d8-121">• Ver, crear y administrar los usuarios del asociado</span><span class="sxs-lookup"><span data-stu-id="616d8-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="616d8-122">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="616d8-122">User Admin</span></span>   | <span data-ttu-id="616d8-123">• Ver, crear y administrar usuarios</span><span class="sxs-lookup"><span data-stu-id="616d8-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="616d8-124">• Ver todos los perfiles de socios comerciales</span><span class="sxs-lookup"><span data-stu-id="616d8-124">• View all partner profiles</span></span>
||<span data-ttu-id="616d8-125">• Ver, crear y administrar los usuarios del asociado</span><span class="sxs-lookup"><span data-stu-id="616d8-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="616d8-126">Usuario predeterminado</span><span class="sxs-lookup"><span data-stu-id="616d8-126">Default user</span></span>|  <span data-ttu-id="616d8-127">Ver mi perfil</span><span class="sxs-lookup"><span data-stu-id="616d8-127">View My profile</span></span>   |
|<span data-ttu-id="616d8-128">Agente de administración</span><span class="sxs-lookup"><span data-stu-id="616d8-128">Admin agent</span></span> | <span data-ttu-id="616d8-129">• Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="616d8-129">•    Customer management</span></span>
||<span data-ttu-id="616d8-130">• Agregue la lista de dispositivos en el centro de partners <</span><span class="sxs-lookup"><span data-stu-id="616d8-130">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="616d8-131">• Crear y aplicar los perfiles en dispositivos</span><span class="sxs-lookup"><span data-stu-id="616d8-131">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="616d8-132">• Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="616d8-132">• Subscription management</span></span>
||<span data-ttu-id="616d8-133">• Service health y atender solicitudes de clientes</span><span class="sxs-lookup"><span data-stu-id="616d8-133">• Service health and service requests for customers</span></span>
||<span data-ttu-id="616d8-134">• Solicitud delega privilegios de administrador</span><span class="sxs-lookup"><span data-stu-id="616d8-134">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="616d8-135">• Ver información sobre precios y ofertas</span><span class="sxs-lookup"><span data-stu-id="616d8-135">• View pricing and offers</span></span>
||<span data-ttu-id="616d8-136">• La facturación</span><span class="sxs-lookup"><span data-stu-id="616d8-136">• Billing</span></span>
||<span data-ttu-id="616d8-137">• Administrar parte de un cliente</span><span class="sxs-lookup"><span data-stu-id="616d8-137">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="616d8-138">• Register un valor agregado reseller</span><span class="sxs-lookup"><span data-stu-id="616d8-138">• Register a value added reseller</span></span>|
|<span data-ttu-id="616d8-139">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="616d8-139">Sales agent</span></span> | <span data-ttu-id="616d8-140">• Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="616d8-140">•    Customer management</span></span>
||<span data-ttu-id="616d8-141">• Agregue la lista de dispositivos en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="616d8-141">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="616d8-142">• Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="616d8-142">• Subscription management</span></span>
||<span data-ttu-id="616d8-143">• Incidencias de soporte técnico de vista</span><span class="sxs-lookup"><span data-stu-id="616d8-143">• View support tickets</span></span>
||<span data-ttu-id="616d8-144">• Solicitud una relación con un cliente</span><span class="sxs-lookup"><span data-stu-id="616d8-144">• Request a relationship with a customer</span></span>
||<span data-ttu-id="616d8-145">• Administración de clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="616d8-145">• Manage customer leads</span></span>
||<span data-ttu-id="616d8-146">• Ver el contrato de cliente</span><span class="sxs-lookup"><span data-stu-id="616d8-146">• View the customer agreement</span></span>
||<span data-ttu-id="616d8-147">• Register un revendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="616d8-147">• Register a value-added reseller</span></span>|
|<span data-ttu-id="616d8-148">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="616d8-148">Helpdesk agent</span></span>| <span data-ttu-id="616d8-149">• Buscar y ver un cliente</span><span class="sxs-lookup"><span data-stu-id="616d8-149">•  Search for and view a customer</span></span>
||<span data-ttu-id="616d8-150">• Editar detalles de cliente</span><span class="sxs-lookup"><span data-stu-id="616d8-150">• Edit customer details</span></span>
||<span data-ttu-id="616d8-151">• Ayuda resolver al cliente los problemas con la administración de facturación o suscripción</span><span class="sxs-lookup"><span data-stu-id="616d8-151">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="616d8-152">• Soporte técnico de solicitud en nombre de los clientes (tenga en cuenta: Debe ser un agente de administración para completar esta tarea para las suscripciones de Office 365)</span><span class="sxs-lookup"><span data-stu-id="616d8-152">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="616d8-153">• Administración de suscripciones y facturación problemas en el nombre de los clientes (tenga en cuenta: Debe ser un agente de administración para completar esta tarea para las suscripciones de Office 365)</span><span class="sxs-lookup"><span data-stu-id="616d8-153">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="616d8-154">Proveedor del Panel de control (CPV).</span><span class="sxs-lookup"><span data-stu-id="616d8-154">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="616d8-155">(Rol CSP y rol sin AAD)</span><span class="sxs-lookup"><span data-stu-id="616d8-155">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="616d8-156">CPVs desarrollar aplicaciones para su uso por los asociados de proveedor de soluciones en la nube (CSP) que les permite integrar los sistemas con Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="616d8-156">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="616d8-157">**Role**</span><span class="sxs-lookup"><span data-stu-id="616d8-157">**Role**</span></span>   |<span data-ttu-id="616d8-158">**¿Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="616d8-158">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="616d8-159">Administrador global</span><span class="sxs-lookup"><span data-stu-id="616d8-159">Global admin</span></span>| <span data-ttu-id="616d8-160">Ver y administrar su perfil CPV</span><span class="sxs-lookup"><span data-stu-id="616d8-160">View and manage your CPV profile</span></span>|
||<span data-ttu-id="616d8-161">Ver y administrar cualquiera de los usuarios que necesitan tener acceso a las funcionalidades de CPV</span><span class="sxs-lookup"><span data-stu-id="616d8-161">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="616d8-162">Administrar la pertenencia a MPN y su empresa (roles sin AAD)</span><span class="sxs-lookup"><span data-stu-id="616d8-162">Manage MPN membership and your company (non-AAD roles)</span></span>

|<span data-ttu-id="616d8-163">**Role**</span><span class="sxs-lookup"><span data-stu-id="616d8-163">**Role**</span></span> | <span data-ttu-id="616d8-164">**¿Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="616d8-164">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="616d8-165">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="616d8-165">MPN partner admin</span></span>|<span data-ttu-id="616d8-166">•CAN agregar los usuarios que no sean inquilinos</span><span class="sxs-lookup"><span data-stu-id="616d8-166">•Can add non-tenant users</span></span>
||<span data-ttu-id="616d8-167">• Ver, crear y administrar solicitudes de servicio asociado</span><span class="sxs-lookup"><span data-stu-id="616d8-167">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="616d8-168">• Vista legal, organización, empresariales y perfiles MPN</span><span class="sxs-lookup"><span data-stu-id="616d8-168">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="616d8-169">• Ver detalles del usuario y sus datos de conocimientos</span><span class="sxs-lookup"><span data-stu-id="616d8-169">• View user details and their skills data</span></span>
||<span data-ttu-id="616d8-170">• Competencias de vista</span><span class="sxs-lookup"><span data-stu-id="616d8-170">• View competencies</span></span>
||<span data-ttu-id="616d8-171">• Ver y administrar las prestaciones</span><span class="sxs-lookup"><span data-stu-id="616d8-171">• View and manage benefits</span></span>
||<span data-ttu-id="616d8-172">Compra y vista • MPN ofrece</span><span class="sxs-lookup"><span data-stu-id="616d8-172">• View and purchase MPN offers</span></span>
||<span data-ttu-id="616d8-173">• Vista MPN ofrece facturas e historial de pedidos</span><span class="sxs-lookup"><span data-stu-id="616d8-173">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="616d8-174">• Ver datos de contribución de asociado</span><span class="sxs-lookup"><span data-stu-id="616d8-174">• View partner contribution data</span></span>
||<span data-ttu-id="616d8-175">• Puede trabajar en la herramienta de validación del vale</span><span class="sxs-lookup"><span data-stu-id="616d8-175">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="616d8-176">-Ver análisis de datos de clientes</span><span class="sxs-lookup"><span data-stu-id="616d8-176">- View customer data analytics</span></span>
|<span data-ttu-id="616d8-177">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="616d8-177">Account admin</span></span>| <span data-ttu-id="616d8-178">• Puede agregar los usuarios que no sean inquilinos</span><span class="sxs-lookup"><span data-stu-id="616d8-178">•   Can add non-tenant users</span></span>
||<span data-ttu-id="616d8-179">• Agregar o eliminar las ubicaciones</span><span class="sxs-lookup"><span data-stu-id="616d8-179">• Add or delete locations</span></span>
||<span data-ttu-id="616d8-180">-Administración de perfiles de las cuentas de para que Administrador</span><span class="sxs-lookup"><span data-stu-id="616d8-180">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="616d8-181">• Asignación de roles para los usuarios de inquilinos para roles de AAD no</span><span class="sxs-lookup"><span data-stu-id="616d8-181">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="616d8-182">• Ubicaciones en programas de inscripción</span><span class="sxs-lookup"><span data-stu-id="616d8-182">• Enroll locations into programs</span></span>

## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="616d8-183">Administrar referencias (roles sin AAD)</span><span class="sxs-lookup"><span data-stu-id="616d8-183">Manage referrals (non-AAD roles)</span></span>

|<span data-ttu-id="616d8-184">**Role**</span><span class="sxs-lookup"><span data-stu-id="616d8-184">**Role**</span></span>|<span data-ttu-id="616d8-185">**¿Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="616d8-185">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="616d8-186">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="616d8-186">Referrals admin</span></span>       |<span data-ttu-id="616d8-187">• Ver, crear y administrar perfiles de negocio</span><span class="sxs-lookup"><span data-stu-id="616d8-187">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="616d8-188">• Recibir y administrar las referencias</span><span class="sxs-lookup"><span data-stu-id="616d8-188">• Receive and manage referrals</span></span>
||<span data-ttu-id="616d8-189">• Ver, crear y administrar solicitudes de servicio asociado</span><span class="sxs-lookup"><span data-stu-id="616d8-189">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="616d8-190">Administrador de perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="616d8-190">Business profile admin</span></span>   |<span data-ttu-id="616d8-191">•View, crear y administrar el perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="616d8-191">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="616d8-192">• Ver, crear y administrar solicitudes de servicio asociado</span><span class="sxs-lookup"><span data-stu-id="616d8-192">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="616d8-193">Administrar incentivos (roles sin AAD)</span><span class="sxs-lookup"><span data-stu-id="616d8-193">Manage Incentives  (non-AAD roles)</span></span>

|<span data-ttu-id="616d8-194">**Role**</span><span class="sxs-lookup"><span data-stu-id="616d8-194">**Role**</span></span> | <span data-ttu-id="616d8-195">**¿Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="616d8-195">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="616d8-196">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="616d8-196">Incentives admin</span></span>|<span data-ttu-id="616d8-197">• Inicia y administra los incentivos</span><span class="sxs-lookup"><span data-stu-id="616d8-197">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="616d8-198">Puede ver y editar todos los aspectos de programas de incentivos •</span><span class="sxs-lookup"><span data-stu-id="616d8-198">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="616d8-199">• Puede ver y editar información bancaria y fiscal</span><span class="sxs-lookup"><span data-stu-id="616d8-199">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="616d8-200">• Beneficios de descuento y Co-op de vista</span><span class="sxs-lookup"><span data-stu-id="616d8-200">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="616d8-201">• Compatibilidad con el acceso</span><span class="sxs-lookup"><span data-stu-id="616d8-201">• Access support</span></span>
||<span data-ttu-id="616d8-202">• Los pagos incentivos de conflictos</span><span class="sxs-lookup"><span data-stu-id="616d8-202">• Dispute incentives payments</span></span>|
|<span data-ttu-id="616d8-203">Usuario de incentivos</span><span class="sxs-lookup"><span data-stu-id="616d8-203">Incentives user</span></span>|<span data-ttu-id="616d8-204">• Puede ver los programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="616d8-204">•  Can view incentives programs</span></span>
||<span data-ttu-id="616d8-205">• Puede ver e iniciar las notificaciones de incentivos</span><span class="sxs-lookup"><span data-stu-id="616d8-205">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="616d8-206">• Beneficios de descuento y Co-op de vista</span><span class="sxs-lookup"><span data-stu-id="616d8-206">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="616d8-207">• Beneficios de descuento y Co-op de vista</span><span class="sxs-lookup"><span data-stu-id="616d8-207">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="616d8-208">• Compatibilidad con el acceso</span><span class="sxs-lookup"><span data-stu-id="616d8-208">• Access support</span></span>












