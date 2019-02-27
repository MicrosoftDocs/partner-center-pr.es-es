---
title: Asignar roles a los usuarios y permisos | El centro de partners
ms.topic: article
ms.date: 10/29/2018
description: Todos los empleados que necesitan trabajar en el centro de Partners deben tener asignado un rol.
author: labrenne
ms.author: labrenne
keywords: roles, permisos, administración, agente
ms.localizationpriority: medium
ms.openlocfilehash: cc0e37601b16033bf31faaf5056ca0389d6f5cf6
ms.sourcegitcommit: 7961476a8fed7cd56a09c6edc8dd1e2dd7f46465
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 02/27/2019
ms.locfileid: "9117218"
---
# <a name="assign-users-roles-and-permissions"></a><span data-ttu-id="e9ec7-104">Asignar roles y permisos de usuarios</span><span class="sxs-lookup"><span data-stu-id="e9ec7-104">Assign users roles and permissions</span></span>


<span data-ttu-id="e9ec7-105">Hayas configurado tu perfil de partner incluidos nombre legal y dirección, detalles de soporte técnico, exenciones fiscales, información bancaria y el contacto principal de tu empresa.</span><span class="sxs-lookup"><span data-stu-id="e9ec7-105">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="e9ec7-106">Siguiente paso: Haz que los usuarios configurados con las contraseñas y roles para que puedan comenzar a trabajar en el centro de partners contigo.</span><span class="sxs-lookup"><span data-stu-id="e9ec7-106">Next step: get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="e9ec7-107">Configurar los empleados a trabajar en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="e9ec7-107">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="e9ec7-108">Determinar los tipos de acceso de los usuarios al centro de partners por los roles y permisos que les darías.</span><span class="sxs-lookup"><span data-stu-id="e9ec7-108">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="e9ec7-109">Roles están relacionados con los programas que participa en tu negocio.</span><span class="sxs-lookup"><span data-stu-id="e9ec7-109">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="e9ec7-110">Por ejemplo, si tu empresa es una empresa de proveedor de soluciones en la nube (CSP), no solo tendrá Azure AD estándar de inquilino de funciones de administración como administrador global, pero que las funciones específicas del programa CSP.</span><span class="sxs-lookup"><span data-stu-id="e9ec7-110">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="e9ec7-111">Cada programa tiene roles específicos.</span><span class="sxs-lookup"><span data-stu-id="e9ec7-111">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="e9ec7-112">Roles de inquilino de Azure Active Directory (AAD) incluyen el administrador global, Administrador de usuarios y las funciones CSP.</span><span class="sxs-lookup"><span data-stu-id="e9ec7-112">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="e9ec7-113">Roles de AAD de no incluyen administrador MPN, Administrador de perfil de negocio, Administrador de referencias, Administrador de incentivos y usuario de incentivos.</span><span class="sxs-lookup"><span data-stu-id="e9ec7-113">Non-AAD roles include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="e9ec7-114">Administrar las transacciones comerciales en el centro de partners (Azure AD y roles CSP)</span><span class="sxs-lookup"><span data-stu-id="e9ec7-114">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|**<span data-ttu-id="e9ec7-115">Rol</span><span class="sxs-lookup"><span data-stu-id="e9ec7-115">Role</span></span>**|**<span data-ttu-id="e9ec7-116">Lo que se puede hacer</span><span class="sxs-lookup"><span data-stu-id="e9ec7-116">What they can do</span></span>**|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="e9ec7-117">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e9ec7-117">Global admin</span></span>|<span data-ttu-id="e9ec7-118">• Puede tener acceso a todas las cuentas o servicios Microsoft con privilegios completos</span><span class="sxs-lookup"><span data-stu-id="e9ec7-118">• Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="e9ec7-119">• Crear incidencias de soporte técnico para el centro de partners</span><span class="sxs-lookup"><span data-stu-id="e9ec7-119">•   Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="e9ec7-120">• Ver contratos, listas de precios y ofertas</span><span class="sxs-lookup"><span data-stu-id="e9ec7-120">• View agreements, price lists, and offers</span></span>
||<span data-ttu-id="e9ec7-121">• Ver, crear y administrar usuarios de partners</span><span class="sxs-lookup"><span data-stu-id="e9ec7-121">• View, create, and manage partner users</span></span>|
|<span data-ttu-id="e9ec7-122">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="e9ec7-122">User Admin</span></span>   | <span data-ttu-id="e9ec7-123">• Ver, crear y administrar usuarios</span><span class="sxs-lookup"><span data-stu-id="e9ec7-123">•   View, create, and manage users</span></span>
||<span data-ttu-id="e9ec7-124">• Ver todos los perfiles de partners</span><span class="sxs-lookup"><span data-stu-id="e9ec7-124">• View all partner profiles</span></span>
||<span data-ttu-id="e9ec7-125">• Ver, crear y administrar usuarios de partners</span><span class="sxs-lookup"><span data-stu-id="e9ec7-125">• View, create, and manage partner users</span></span>  |
|<span data-ttu-id="e9ec7-126">Usuario predeterminado</span><span class="sxs-lookup"><span data-stu-id="e9ec7-126">Default user</span></span>|  <span data-ttu-id="e9ec7-127">Ver mi perfil</span><span class="sxs-lookup"><span data-stu-id="e9ec7-127">View My profile</span></span>   |
|<span data-ttu-id="e9ec7-128">Agente de administración</span><span class="sxs-lookup"><span data-stu-id="e9ec7-128">Admin agent</span></span> | <span data-ttu-id="e9ec7-129">• Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="e9ec7-129">•    Customer management</span></span>
||<span data-ttu-id="e9ec7-130">• Agregar la lista de dispositivos a la Center< de partners</span><span class="sxs-lookup"><span data-stu-id="e9ec7-130">• Add device list to the Partner Center<</span></span>
||<span data-ttu-id="e9ec7-131">• Crear y aplicar los perfiles a los dispositivos</span><span class="sxs-lookup"><span data-stu-id="e9ec7-131">• Create and apply profiles to devices</span></span>
||<span data-ttu-id="e9ec7-132">• Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="e9ec7-132">• Subscription management</span></span>
||<span data-ttu-id="e9ec7-133">Solicitudes de servicio y estado del servicio de • para los clientes</span><span class="sxs-lookup"><span data-stu-id="e9ec7-133">• Service health and service requests for customers</span></span>
||<span data-ttu-id="e9ec7-134">• Solicitud privilegios de administrador</span><span class="sxs-lookup"><span data-stu-id="e9ec7-134">• Request delegated administrator privileges</span></span>
||<span data-ttu-id="e9ec7-135">• Ver precios y ofertas</span><span class="sxs-lookup"><span data-stu-id="e9ec7-135">• View pricing and offers</span></span>
||<span data-ttu-id="e9ec7-136">• La facturación</span><span class="sxs-lookup"><span data-stu-id="e9ec7-136">• Billing</span></span>
||<span data-ttu-id="e9ec7-137">• Administrar en nombre de un cliente</span><span class="sxs-lookup"><span data-stu-id="e9ec7-137">• Administer on behalf of a customer</span></span>
||<span data-ttu-id="e9ec7-138">• Registrar un valor agregado revendedor</span><span class="sxs-lookup"><span data-stu-id="e9ec7-138">• Register a value added reseller</span></span>|
|<span data-ttu-id="e9ec7-139">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="e9ec7-139">Sales agent</span></span> | <span data-ttu-id="e9ec7-140">• Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="e9ec7-140">•    Customer management</span></span>
||<span data-ttu-id="e9ec7-141">• Agregar una lista de dispositivos en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="e9ec7-141">• Add device list to the Partner Center</span></span>
||<span data-ttu-id="e9ec7-142">• Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="e9ec7-142">• Subscription management</span></span>
||<span data-ttu-id="e9ec7-143">• Ver incidencias de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="e9ec7-143">• View support tickets</span></span>
||<span data-ttu-id="e9ec7-144">• Solicitar una relación con un cliente</span><span class="sxs-lookup"><span data-stu-id="e9ec7-144">• Request a relationship with a customer</span></span>
||<span data-ttu-id="e9ec7-145">• Administrar clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="e9ec7-145">• Manage customer leads</span></span>
||<span data-ttu-id="e9ec7-146">• Ver el contrato de cliente</span><span class="sxs-lookup"><span data-stu-id="e9ec7-146">• View the customer agreement</span></span>
||<span data-ttu-id="e9ec7-147">• Registrar un revendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="e9ec7-147">• Register a value-added reseller</span></span>|
|<span data-ttu-id="e9ec7-148">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="e9ec7-148">Helpdesk agent</span></span>| <span data-ttu-id="e9ec7-149">• Buscar y ver un cliente</span><span class="sxs-lookup"><span data-stu-id="e9ec7-149">•  Search for and view a customer</span></span>
||<span data-ttu-id="e9ec7-150">• Editar detalles de los clientes</span><span class="sxs-lookup"><span data-stu-id="e9ec7-150">• Edit customer details</span></span>
||<span data-ttu-id="e9ec7-151">• Ayudan a resolver problemas del cliente con la administración de facturación o de suscripción</span><span class="sxs-lookup"><span data-stu-id="e9ec7-151">• Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="e9ec7-152">• Solicitar soporte en nombre de los clientes (Nota: debes ser un agente administrador para completar esta tarea en las suscripciones de Office 365)</span><span class="sxs-lookup"><span data-stu-id="e9ec7-152">• Request support on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>
||<span data-ttu-id="e9ec7-153">• Administrar suscripciones y facturación problemas en nombre de los clientes (Nota: debes ser un agente administrador para completar esta tarea en las suscripciones de Office 365)</span><span class="sxs-lookup"><span data-stu-id="e9ec7-153">• Manage subscriptions and billing issues on behalf of customers (Note: You must be an admin agent to complete this task for Office 365 subscriptions)</span></span>|
|
### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="e9ec7-154">Proveedor de Panel de control (CPV).</span><span class="sxs-lookup"><span data-stu-id="e9ec7-154">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="e9ec7-155">(Las funciones CSP y no AAD)</span><span class="sxs-lookup"><span data-stu-id="e9ec7-155">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="e9ec7-156">CPVs desarrollar aplicaciones para su uso por los partners de proveedor de soluciones en la nube (CSP) para que puedan integrar sus sistemas con las API del centro de partners.</span><span class="sxs-lookup"><span data-stu-id="e9ec7-156">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|**<span data-ttu-id="e9ec7-157">Rol</span><span class="sxs-lookup"><span data-stu-id="e9ec7-157">Role</span></span>**   |**<span data-ttu-id="e9ec7-158">Lo que puedes hacer</span><span class="sxs-lookup"><span data-stu-id="e9ec7-158">What you can do</span></span>**|
|------------------------------|:----------------------------|
|<span data-ttu-id="e9ec7-159">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e9ec7-159">Global admin</span></span>| <span data-ttu-id="e9ec7-160">Ver y administrar tu perfil CPV</span><span class="sxs-lookup"><span data-stu-id="e9ec7-160">View and manage your CPV profile</span></span>|
||<span data-ttu-id="e9ec7-161">Ver y administrar cualquiera de los usuarios que necesitan acceder a las funcionalidades CPV</span><span class="sxs-lookup"><span data-stu-id="e9ec7-161">View and manage any of your users who need access to CPV capabilities</span></span>|

## <a name="manage-mpn-membership-and-your-company-non-aad-roles"></a><span data-ttu-id="e9ec7-162">Administrar tu empresa (funciones que no sean AAD) y la suscripción a MPN</span><span class="sxs-lookup"><span data-stu-id="e9ec7-162">Manage MPN membership and your company (non-AAD roles)</span></span>

|**<span data-ttu-id="e9ec7-163">Rol</span><span class="sxs-lookup"><span data-stu-id="e9ec7-163">Role</span></span>** | **<span data-ttu-id="e9ec7-164">Lo que puedes hacer</span><span class="sxs-lookup"><span data-stu-id="e9ec7-164">What you can do</span></span>**|
|----------------------------|:----------------------------|
|<span data-ttu-id="e9ec7-165">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="e9ec7-165">MPN partner admin</span></span>|<span data-ttu-id="e9ec7-166">•CAN agregar usuarios del inquilino que no sean</span><span class="sxs-lookup"><span data-stu-id="e9ec7-166">•Can add non-tenant users</span></span>
||<span data-ttu-id="e9ec7-167">• Ver, crear y administrar las solicitudes de servicio de partners</span><span class="sxs-lookup"><span data-stu-id="e9ec7-167">• View, create, and manage partner service requests</span></span>
||<span data-ttu-id="e9ec7-168">• Vista legales, organización, empresas y perfiles MPN</span><span class="sxs-lookup"><span data-stu-id="e9ec7-168">• View legal, organization, business, and MPN profiles</span></span>
||<span data-ttu-id="e9ec7-169">• Ver detalles de usuario y sus datos de habilidades</span><span class="sxs-lookup"><span data-stu-id="e9ec7-169">• View user details and their skills data</span></span>
||<span data-ttu-id="e9ec7-170">• Ver competencias</span><span class="sxs-lookup"><span data-stu-id="e9ec7-170">• View competencies</span></span>
||<span data-ttu-id="e9ec7-171">• Ver y administrar ventajas</span><span class="sxs-lookup"><span data-stu-id="e9ec7-171">• View and manage benefits</span></span>
||<span data-ttu-id="e9ec7-172">• Vista y compra de ofertas MPN</span><span class="sxs-lookup"><span data-stu-id="e9ec7-172">• View and purchase MPN offers</span></span>
||<span data-ttu-id="e9ec7-173">Facturas y el historial de pedidos de ofertas • vista MPN</span><span class="sxs-lookup"><span data-stu-id="e9ec7-173">• View MPN offers order history and invoices</span></span>
||<span data-ttu-id="e9ec7-174">• Ver datos de contribución de partners</span><span class="sxs-lookup"><span data-stu-id="e9ec7-174">• View partner contribution data</span></span>
||<span data-ttu-id="e9ec7-175">• Puede trabajar en la herramienta de validación de asientos</span><span class="sxs-lookup"><span data-stu-id="e9ec7-175">• Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="e9ec7-176">-Ver un análisis de datos de cliente</span><span class="sxs-lookup"><span data-stu-id="e9ec7-176">- View customer data analytics</span></span>
|<span data-ttu-id="e9ec7-177">Administrador de la cuenta</span><span class="sxs-lookup"><span data-stu-id="e9ec7-177">Account admin</span></span>| <span data-ttu-id="e9ec7-178">• Agregar usuarios del inquilino que no sean</span><span class="sxs-lookup"><span data-stu-id="e9ec7-178">•   Can add non-tenant users</span></span>
||<span data-ttu-id="e9ec7-179">• Agregar o eliminar ubicaciones</span><span class="sxs-lookup"><span data-stu-id="e9ec7-179">• Add or delete locations</span></span>
||<span data-ttu-id="e9ec7-180">-Administrar perfiles relacionados con las cuentas que eres el Administrador de</span><span class="sxs-lookup"><span data-stu-id="e9ec7-180">- Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="e9ec7-181">• Asignar roles para los usuarios de inquilino a las funciones que no sean de AAD</span><span class="sxs-lookup"><span data-stu-id="e9ec7-181">• Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="e9ec7-182">• Inscribir ubicaciones en los programas</span><span class="sxs-lookup"><span data-stu-id="e9ec7-182">• Enroll locations into programs</span></span>

## <a name="manage-referrals-non-aad-roles"></a><span data-ttu-id="e9ec7-183">Administrar las referencias (funciones que no sean AAD)</span><span class="sxs-lookup"><span data-stu-id="e9ec7-183">Manage referrals (non-AAD roles)</span></span>

|**<span data-ttu-id="e9ec7-184">Rol</span><span class="sxs-lookup"><span data-stu-id="e9ec7-184">Role</span></span>**|**<span data-ttu-id="e9ec7-185">Lo que puedes hacer</span><span class="sxs-lookup"><span data-stu-id="e9ec7-185">What you can do</span></span>**|
|-----------------------------|:------------------------|
|<span data-ttu-id="e9ec7-186">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="e9ec7-186">Referrals admin</span></span>       |<span data-ttu-id="e9ec7-187">• Ver, crear y administrar perfiles de negocio</span><span class="sxs-lookup"><span data-stu-id="e9ec7-187">•   View, create, and manage business profiles</span></span>
||<span data-ttu-id="e9ec7-188">• Recibir y administrar las referencias</span><span class="sxs-lookup"><span data-stu-id="e9ec7-188">• Receive and manage referrals</span></span>
||<span data-ttu-id="e9ec7-189">• Ver, crear y administrar las solicitudes de servicio de partners</span><span class="sxs-lookup"><span data-stu-id="e9ec7-189">• View, create, and manage partner service requests</span></span>|
|<span data-ttu-id="e9ec7-190">Administrador de perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="e9ec7-190">Business profile admin</span></span>   |<span data-ttu-id="e9ec7-191">•View, crear y administrar el perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="e9ec7-191">•View, create, and manage business profile</span></span> 
||<span data-ttu-id="e9ec7-192">• Ver, crear y administrar las solicitudes de servicio de partners</span><span class="sxs-lookup"><span data-stu-id="e9ec7-192">• View, create, and manage partner service requests</span></span>|

## <a name="manage-incentives--non-aad-roles"></a><span data-ttu-id="e9ec7-193">Administrar incentivos (funciones que no sean AAD)</span><span class="sxs-lookup"><span data-stu-id="e9ec7-193">Manage Incentives  (non-AAD roles)</span></span>

|**<span data-ttu-id="e9ec7-194">Rol</span><span class="sxs-lookup"><span data-stu-id="e9ec7-194">Role</span></span>** | **<span data-ttu-id="e9ec7-195">Lo que puedes hacer</span><span class="sxs-lookup"><span data-stu-id="e9ec7-195">What you can do</span></span>**|
|------------------------------|:-------------------------|
|<span data-ttu-id="e9ec7-196">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="e9ec7-196">Incentives admin</span></span>|<span data-ttu-id="e9ec7-197">• Inicia y administra los incentivos</span><span class="sxs-lookup"><span data-stu-id="e9ec7-197">• Initiates and manages incentives</span></span> 
||<span data-ttu-id="e9ec7-198">• Permite ver y editar todos los aspectos de los programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="e9ec7-198">• Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="e9ec7-199">• Permite ver y editar detalles bancarios y fiscales</span><span class="sxs-lookup"><span data-stu-id="e9ec7-199">• Can view and edit bank and tax details</span></span>
||<span data-ttu-id="e9ec7-200">• Ganancias de reembolso y cooperación de vista</span><span class="sxs-lookup"><span data-stu-id="e9ec7-200">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="e9ec7-201">• Soporte de acceso</span><span class="sxs-lookup"><span data-stu-id="e9ec7-201">• Access support</span></span>
||<span data-ttu-id="e9ec7-202">• Los pagos de incentivos disputa</span><span class="sxs-lookup"><span data-stu-id="e9ec7-202">• Dispute incentives payments</span></span>|
|<span data-ttu-id="e9ec7-203">Usuario de incentivos</span><span class="sxs-lookup"><span data-stu-id="e9ec7-203">Incentives user</span></span>|<span data-ttu-id="e9ec7-204">• Ver programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="e9ec7-204">•  Can view incentives programs</span></span>
||<span data-ttu-id="e9ec7-205">• Puede ver e iniciar reclamaciones de incentivos</span><span class="sxs-lookup"><span data-stu-id="e9ec7-205">• Can view and initiate incentives claims</span></span>
||<span data-ttu-id="e9ec7-206">• Ganancias de reembolso y cooperación de vista</span><span class="sxs-lookup"><span data-stu-id="e9ec7-206">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="e9ec7-207">• Ganancias de reembolso y cooperación de vista</span><span class="sxs-lookup"><span data-stu-id="e9ec7-207">• View rebate and co-op earnings</span></span>
||<span data-ttu-id="e9ec7-208">• Soporte de acceso</span><span class="sxs-lookup"><span data-stu-id="e9ec7-208">• Access support</span></span>












