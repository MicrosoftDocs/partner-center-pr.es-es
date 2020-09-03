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
ms.openlocfilehash: 3feb4e678381b6fa5398bf3b3d89f6e4286e6ff1
ms.sourcegitcommit: 4feae1ea7fd3077934e3c931a5de801c96a4f995
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/27/2020
ms.locfileid: "89040771"
---
# <a name="assign-users-roles-and-permissions-for-a-companys-users-needing-to-work-in-partner-center"></a><span data-ttu-id="ff3b3-103">Asignación de roles y permisos a los usuarios de una empresa que necesitan trabajar en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ff3b3-103">Assign users roles and permissions for a company's users needing to work in Partner Center</span></span>

<span data-ttu-id="ff3b3-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="ff3b3-104">**Appropriate roles**</span></span>

- <span data-ttu-id="ff3b3-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ff3b3-105">Global admin</span></span>
- <span data-ttu-id="ff3b3-106">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="ff3b3-106">User admin</span></span>
- <span data-ttu-id="ff3b3-107">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="ff3b3-107">MPN partner admin</span></span>

<span data-ttu-id="ff3b3-108">Has configurado tu perfil de partner, incluyendo el nombre y la dirección legales, los detalles de soporte técnico, las exenciones fiscales, la información bancaria y el contacto principal de tu empresa.</span><span class="sxs-lookup"><span data-stu-id="ff3b3-108">You've set up your partner profile including legal name and address, support details, file tax exemptions, bank info, and the primary contact for your company.</span></span> <span data-ttu-id="ff3b3-109">Paso siguiente: configura tus usuarios con contraseñas y roles para que puedan comenzar a trabajar en el Centro de partners contigo.</span><span class="sxs-lookup"><span data-stu-id="ff3b3-109">Next step: Get your users set up with passwords and roles so they can begin working in Partner Center with you.</span></span>

## <a name="set-up-your-employees-to-work-in-partner-center"></a><span data-ttu-id="ff3b3-110">Configura a sus empleados para trabajar en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ff3b3-110">Set up your employees to work in Partner Center</span></span>

<span data-ttu-id="ff3b3-111">Debes determinar los tipos de acceso que tendrán los usuarios en el Centro de partners, en función de los roles y permisos que les otorgues.</span><span class="sxs-lookup"><span data-stu-id="ff3b3-111">You determine the types of access your users have to Partner Center by the roles and permissions you give them.</span></span> <span data-ttu-id="ff3b3-112">Los roles están relacionados con los programas en los que participa tu empresa.</span><span class="sxs-lookup"><span data-stu-id="ff3b3-112">Roles are related to the program(s) your business is involved in.</span></span> <span data-ttu-id="ff3b3-113">Por ejemplo, si tu negocio es un Proveedor de soluciones en la nube (CSP), no solo tendrás los roles estándar de administración de inquilinos de Azure AD (como el administrador global), sino que también necesitarás roles específicos para el programa de CSP.</span><span class="sxs-lookup"><span data-stu-id="ff3b3-113">For example,if your business is a Cloud Solution Provider (CSP) business, you will not only have the standard Azure AD tenant management roles such as global admin, but will need roles specific to the CSP program.</span></span> <span data-ttu-id="ff3b3-114">Recuerda que cada programa tiene roles específicos.</span><span class="sxs-lookup"><span data-stu-id="ff3b3-114">Each program has roles specific to it.</span></span>

>[!Note]
> <span data-ttu-id="ff3b3-115">Los roles de inquilino de Azure Active Directory (AAD) incluyen roles de administrador global, administrador de usuarios y CSP.</span><span class="sxs-lookup"><span data-stu-id="ff3b3-115">Azure Active Directory (AAD) tenant roles include global admin, user admin, and CSP roles.</span></span> <span data-ttu-id="ff3b3-116">Los roles que no son de AAD son aquellos que no administran al inquilino, e incluyen un administrador de MPN, un administrador de perfil comercial, un administrador de referencias, un administrador de incentivos y un usuario de incentivos.</span><span class="sxs-lookup"><span data-stu-id="ff3b3-116">Non-AAD roles are those roles that do not manage the tenant, and they include MPN admin, business profile admin, referral admin, incentive admin, and incentive user.</span></span> 

### <a name="manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles"></a><span data-ttu-id="ff3b3-117">Administra las transacciones comerciales en el Centro de partners (roles de Azure AD y CSP)</span><span class="sxs-lookup"><span data-stu-id="ff3b3-117">Manage commercial transactions in Partner Center (Azure AD and CSP roles)</span></span>

|<span data-ttu-id="ff3b3-118">**Rol**</span><span class="sxs-lookup"><span data-stu-id="ff3b3-118">**Role**</span></span>|<span data-ttu-id="ff3b3-119">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="ff3b3-119">**What they can do**</span></span>|
|----------------------------------|:---------------------------------|
|<span data-ttu-id="ff3b3-120">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ff3b3-120">Global admin</span></span>|<span data-ttu-id="ff3b3-121">\*    Obtener acceso a todos los servicios o cuentas de Microsoft con privilegios completos</span><span class="sxs-lookup"><span data-stu-id="ff3b3-121">\*    Can access all Microsoft account/services with full privileges</span></span>
|      |<span data-ttu-id="ff3b3-122">\*    Crear vales de soporte técnico para el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ff3b3-122">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="ff3b3-123">\*    Ver los vales de soporte técnico para partners que cree</span><span class="sxs-lookup"><span data-stu-id="ff3b3-123">\*    View partner support tickets you create</span></span>
||<span data-ttu-id="ff3b3-124">\*    Ver contratos, listas de precios y ofertas</span><span class="sxs-lookup"><span data-stu-id="ff3b3-124">\*    View agreements, price lists, and offers</span></span>
||<span data-ttu-id="ff3b3-125">\*    Ver, crear y administrar usuarios asociados</span><span class="sxs-lookup"><span data-stu-id="ff3b3-125">\*    View, create, and manage partner users</span></span>|
||  <span data-ttu-id="ff3b3-126">• Ver, crear y administrar los archivos de facturación, facturas y conciliación</span><span class="sxs-lookup"><span data-stu-id="ff3b3-126">View, create, and manage billing, invoices, and recon files</span></span>
|<span data-ttu-id="ff3b3-127">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="ff3b3-127">User management admin</span></span>   | <span data-ttu-id="ff3b3-128">\*    Ver, crear y administrar usuarios</span><span class="sxs-lookup"><span data-stu-id="ff3b3-128">\*    View, create, and manage users</span></span>
||<span data-ttu-id="ff3b3-129">\*    Ver todos los perfiles de asociado</span><span class="sxs-lookup"><span data-stu-id="ff3b3-129">\*    View all partner profiles</span></span>
||<span data-ttu-id="ff3b3-130">\*    Ver, crear y administrar usuarios asociados</span><span class="sxs-lookup"><span data-stu-id="ff3b3-130">\*    View, create, and manage partner users</span></span>  |
||<span data-ttu-id="ff3b3-131">\*    Crear vales de soporte técnico para el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ff3b3-131">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="ff3b3-132">\*    Ver los vales de soporte técnico para partners que cree</span><span class="sxs-lookup"><span data-stu-id="ff3b3-132">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="ff3b3-133">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="ff3b3-133">Billing admin</span></span> | <span data-ttu-id="ff3b3-134">• Ver, crear y administrar los archivos de facturación, facturas y conciliación</span><span class="sxs-lookup"><span data-stu-id="ff3b3-134">- View, create, and manage billing, invoices, and recon files</span></span>|
||<span data-ttu-id="ff3b3-135">\*    Ver precios</span><span class="sxs-lookup"><span data-stu-id="ff3b3-135">\*    View pricing</span></span>
||<span data-ttu-id="ff3b3-136">\*    Crear vales de soporte técnico para el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ff3b3-136">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="ff3b3-137">\*    Ver los vales de soporte técnico para partners que cree</span><span class="sxs-lookup"><span data-stu-id="ff3b3-137">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="ff3b3-138">Usuario predeterminado</span><span class="sxs-lookup"><span data-stu-id="ff3b3-138">Default user</span></span>|  <span data-ttu-id="ff3b3-139">Ver mi perfil</span><span class="sxs-lookup"><span data-stu-id="ff3b3-139">View My profile</span></span>   |
|<span data-ttu-id="ff3b3-140">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="ff3b3-140">Admin agent</span></span> | <span data-ttu-id="ff3b3-141">\*    Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="ff3b3-141">\*    Customer management</span></span>
||<span data-ttu-id="ff3b3-142">\*    Agregar una lista de dispositivos en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ff3b3-142">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="ff3b3-143">\*    Crear perfiles y aplicarlos a dispositivos</span><span class="sxs-lookup"><span data-stu-id="ff3b3-143">\*    Create and apply profiles to devices</span></span>
||<span data-ttu-id="ff3b3-144">\*    Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="ff3b3-144">\*    Subscription management</span></span>
||<span data-ttu-id="ff3b3-145">\*    Comprobar el estado del servicio y las solicitudes de servicio para clientes</span><span class="sxs-lookup"><span data-stu-id="ff3b3-145">\*    Service health and service requests for customers</span></span>
||<span data-ttu-id="ff3b3-146">\*    Solicitar privilegios de administrador delegado</span><span class="sxs-lookup"><span data-stu-id="ff3b3-146">\*    Request delegated administrator privileges</span></span>
||<span data-ttu-id="ff3b3-147">\*    Ver los precios y las ofertas</span><span class="sxs-lookup"><span data-stu-id="ff3b3-147">\*    View pricing and offers</span></span>
||<span data-ttu-id="ff3b3-148">\*    Facturación</span><span class="sxs-lookup"><span data-stu-id="ff3b3-148">\*    Billing</span></span>
||<span data-ttu-id="ff3b3-149">\*    Administrar contenido en nombre de un cliente</span><span class="sxs-lookup"><span data-stu-id="ff3b3-149">\*    Administer on behalf of a customer</span></span>
||<span data-ttu-id="ff3b3-150">\*    Registrar un revendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="ff3b3-150">\*    Register a value added reseller</span></span>
||<span data-ttu-id="ff3b3-151">\*    Crear vales de soporte técnico para el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ff3b3-151">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="ff3b3-152">\*    Ver los vales de soporte técnico para partners que cree</span><span class="sxs-lookup"><span data-stu-id="ff3b3-152">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="ff3b3-153">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="ff3b3-153">Sales agent</span></span> | <span data-ttu-id="ff3b3-154">\*    Administración de clientes</span><span class="sxs-lookup"><span data-stu-id="ff3b3-154">\*    Customer management</span></span>
||<span data-ttu-id="ff3b3-155">\*    Agregar una lista de dispositivos en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ff3b3-155">\*    Add device list to the Partner Center</span></span>
||<span data-ttu-id="ff3b3-156">\*    Administración de suscripciones</span><span class="sxs-lookup"><span data-stu-id="ff3b3-156">\*    Subscription management</span></span>
||<span data-ttu-id="ff3b3-157">\*    Ver vales de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="ff3b3-157">\*    View support tickets</span></span>
||<span data-ttu-id="ff3b3-158">\*    Solicitar una relación con un cliente</span><span class="sxs-lookup"><span data-stu-id="ff3b3-158">\*    Request a relationship with a customer</span></span>
||<span data-ttu-id="ff3b3-159">\*    Ver los precios y las ofertas</span><span class="sxs-lookup"><span data-stu-id="ff3b3-159">\*    View pricing and offers</span></span>
||<span data-ttu-id="ff3b3-160">\*    Administrar clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="ff3b3-160">\*    Manage customer leads</span></span>
||<span data-ttu-id="ff3b3-161">\*    Ver el contrato de cliente</span><span class="sxs-lookup"><span data-stu-id="ff3b3-161">\*    View the customer agreement</span></span>
||<span data-ttu-id="ff3b3-162">\*    Registrar un vendedor de valor agregado</span><span class="sxs-lookup"><span data-stu-id="ff3b3-162">\*    Register a value-added reseller</span></span>
||<span data-ttu-id="ff3b3-163">\*    Crear vales de soporte técnico para el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ff3b3-163">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="ff3b3-164">\*    Ver los vales de soporte técnico para partners que cree</span><span class="sxs-lookup"><span data-stu-id="ff3b3-164">\*    View partner support tickets you create</span></span>|
|<span data-ttu-id="ff3b3-165">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="ff3b3-165">Helpdesk agent</span></span>| <span data-ttu-id="ff3b3-166">\*    Buscar y ver un cliente</span><span class="sxs-lookup"><span data-stu-id="ff3b3-166">\*    Search for and view a customer</span></span>
||<span data-ttu-id="ff3b3-167">\*    Editar detalles del cliente</span><span class="sxs-lookup"><span data-stu-id="ff3b3-167">\*    Edit customer details</span></span>
||<span data-ttu-id="ff3b3-168">\*    Ayudar a resolver problemas del cliente referentes a la facturación o la administración de las suscripciones</span><span class="sxs-lookup"><span data-stu-id="ff3b3-168">\*    Help resolve customer issues with billing or subscription management</span></span>
||<span data-ttu-id="ff3b3-169">\*    Solicitar soporte técnico en nombre de los clientes</span><span class="sxs-lookup"><span data-stu-id="ff3b3-169">\*    Request support on behalf of customers</span></span> 
||<span data-ttu-id="ff3b3-170">\*    Administrar los problemas de suscripción y facturación en nombre de los clientes</span><span class="sxs-lookup"><span data-stu-id="ff3b3-170">\*    Manage subscriptions and billing issues on behalf of customers</span></span>
||<span data-ttu-id="ff3b3-171">\*    Crear vales de soporte técnico para el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ff3b3-171">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="ff3b3-172">\*    Ver los vales de soporte técnico para partners que cree</span><span class="sxs-lookup"><span data-stu-id="ff3b3-172">\*    View partner support tickets you create</span></span>| 

### <a name="control-panel-vendor-cpv-csp-role-and-non-aad-role"></a><span data-ttu-id="ff3b3-173">Proveedor del panel de control (CPV).</span><span class="sxs-lookup"><span data-stu-id="ff3b3-173">Control Panel Vendor (CPV).</span></span> <span data-ttu-id="ff3b3-174">(Rol de CSP y rol que no es de AAD)</span><span class="sxs-lookup"><span data-stu-id="ff3b3-174">(CSP role and non-AAD role)</span></span>
<span data-ttu-id="ff3b3-175">Los CPV desarrollan aplicaciones para los partners del Proveedor de soluciones en la nube (CSP) y que así puedan integrar sus sistemas con las API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="ff3b3-175">CPVs develop apps for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> 

|<span data-ttu-id="ff3b3-176">**Rol**</span><span class="sxs-lookup"><span data-stu-id="ff3b3-176">**Role**</span></span>   |<span data-ttu-id="ff3b3-177">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="ff3b3-177">**What you can do**</span></span>|
|------------------------------|:----------------------------|
|<span data-ttu-id="ff3b3-178">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ff3b3-178">Global admin</span></span>| <span data-ttu-id="ff3b3-179">Ver y administrar el perfil de CPV</span><span class="sxs-lookup"><span data-stu-id="ff3b3-179">View and manage your CPV profile</span></span>|
||<span data-ttu-id="ff3b3-180">Ver y administrar los usuarios que necesiten acceso a las funcionalidades de CPV</span><span class="sxs-lookup"><span data-stu-id="ff3b3-180">View and manage any of your users who need access to CPV capabilities</span></span>|

### <a name="guest-user-must-be-added-to-the-aad-tenant"></a><span data-ttu-id="ff3b3-181">Usuario invitado (debe agregarse al inquilino de AAD)</span><span class="sxs-lookup"><span data-stu-id="ff3b3-181">Guest user (must be added to the AAD tenant)</span></span>

|<span data-ttu-id="ff3b3-182">**Usuario invitado**</span><span class="sxs-lookup"><span data-stu-id="ff3b3-182">**Guest user**</span></span>   | <span data-ttu-id="ff3b3-183">**Roles**</span><span class="sxs-lookup"><span data-stu-id="ff3b3-183">**Roles**</span></span>|
|---------------------------|:--------------------|
||<span data-ttu-id="ff3b3-184">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="ff3b3-184">MPN partner admin</span></span>|
||<span data-ttu-id="ff3b3-185">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="ff3b3-185">Accounts admin</span></span>|
||<span data-ttu-id="ff3b3-186">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="ff3b3-186">Incentives admin</span></span>|
||<span data-ttu-id="ff3b3-187">Administrador del perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="ff3b3-187">Business profile admin</span></span>|
||<span data-ttu-id="ff3b3-188">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="ff3b3-188">Referrals admin</span></span>|


## <a name="manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant"></a><span data-ttu-id="ff3b3-189">Administrar la pertenencia a MPN y su empresa (roles que no son de AAD: estos roles administran el negocio de la empresa en lugar del inquilino)</span><span class="sxs-lookup"><span data-stu-id="ff3b3-189">Manage MPN membership and your company (non-AAD roles: these roles manage the company business rather than the tenant)</span></span>

|<span data-ttu-id="ff3b3-190">**Rol**</span><span class="sxs-lookup"><span data-stu-id="ff3b3-190">**Role**</span></span> | <span data-ttu-id="ff3b3-191">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="ff3b3-191">**What you can do**</span></span>|
|----------------------------|:----------------------------|
|<span data-ttu-id="ff3b3-192">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="ff3b3-192">MPN partner admin</span></span>|<span data-ttu-id="ff3b3-193">\*    Ver, crear y administrar las solicitudes de servicio de los asociados</span><span class="sxs-lookup"><span data-stu-id="ff3b3-193">\*    View, create, and manage partner service requests</span></span>||
||<span data-ttu-id="ff3b3-194">\*    Ver perfiles legales, de negocios, empresariales y de MPN</span><span class="sxs-lookup"><span data-stu-id="ff3b3-194">\*    View legal, company, business, and MPN profiles</span></span>
||<span data-ttu-id="ff3b3-195">\*    Ver los detalles de los usuarios y sus datos de aptitudes</span><span class="sxs-lookup"><span data-stu-id="ff3b3-195">\*    View user details and their skills data</span></span>
||<span data-ttu-id="ff3b3-196">\*    Ver competencias</span><span class="sxs-lookup"><span data-stu-id="ff3b3-196">\*    View competencies</span></span>
||<span data-ttu-id="ff3b3-197">\*    Ver y administrar ventajas</span><span class="sxs-lookup"><span data-stu-id="ff3b3-197">\*    View and manage benefits</span></span>
||<span data-ttu-id="ff3b3-198">\*    Ver y adquirir ofertas de MPN</span><span class="sxs-lookup"><span data-stu-id="ff3b3-198">\*    View and purchase MPN offers</span></span>
||<span data-ttu-id="ff3b3-199">\*    Ver las facturas y el historial de pedidos de ofertas de MPN</span><span class="sxs-lookup"><span data-stu-id="ff3b3-199">\*    View MPN offers order history and invoices</span></span>
||<span data-ttu-id="ff3b3-200">\*    Ver datos de los indicadores de contribución de asociados</span><span class="sxs-lookup"><span data-stu-id="ff3b3-200">\*    View partner contribution indicator data</span></span>
||<span data-ttu-id="ff3b3-201">\*    Usar la herramienta de validación de cupones</span><span class="sxs-lookup"><span data-stu-id="ff3b3-201">\*    Can work in the Voucher Validation tool</span></span>|
||<span data-ttu-id="ff3b3-202">\*     Ver análisis de datos de clientes</span><span class="sxs-lookup"><span data-stu-id="ff3b3-202">\*    View customer data analytics</span></span>
||<span data-ttu-id="ff3b3-203">\*    Ver otros roles de usuario dentro de la empresa, pero no puede asignar roles</span><span class="sxs-lookup"><span data-stu-id="ff3b3-203">\*    View other user roles within company, but can't assign roles</span></span>
||<span data-ttu-id="ff3b3-204">\*    Crear vales de soporte técnico para el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ff3b3-204">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="ff3b3-205">\*    Ver los vales de soporte técnico para partners que cree</span><span class="sxs-lookup"><span data-stu-id="ff3b3-205">\*    View partner support tickets you create</span></span>
|<span data-ttu-id="ff3b3-206">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="ff3b3-206">Account admin</span></span>| <span data-ttu-id="ff3b3-207">• Agregar ubicaciones</span><span class="sxs-lookup"><span data-stu-id="ff3b3-207">Add locations</span></span>
|| <span data-ttu-id="ff3b3-208">• Administrar perfiles relacionados con las cuentas para las que es administrador</span><span class="sxs-lookup"><span data-stu-id="ff3b3-208">Manage profiles related to the accounts you are admin for</span></span> 
||<span data-ttu-id="ff3b3-209">\*    Asignar roles de usuarios del inquilino a roles que no son de AAD</span><span class="sxs-lookup"><span data-stu-id="ff3b3-209">\*    Assign roles for users in tenant to non AAD roles</span></span> 
||<span data-ttu-id="ff3b3-210">\*    Inscribir ubicaciones en programas</span><span class="sxs-lookup"><span data-stu-id="ff3b3-210">\*    Enroll locations into programs</span></span>
||<span data-ttu-id="ff3b3-211">\*    Crear vales de soporte técnico para el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ff3b3-211">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="ff3b3-212">\*    Ver los vales de soporte técnico para partners que cree</span><span class="sxs-lookup"><span data-stu-id="ff3b3-212">\*    View partner support tickets you create</span></span>


## <a name="manage-referrals"></a><span data-ttu-id="ff3b3-213">Administrar referencias</span><span class="sxs-lookup"><span data-stu-id="ff3b3-213">Manage referrals</span></span> 

|<span data-ttu-id="ff3b3-214">**Rol**</span><span class="sxs-lookup"><span data-stu-id="ff3b3-214">**Role**</span></span>|<span data-ttu-id="ff3b3-215">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="ff3b3-215">**What you can do**</span></span>|
|-----------------------------|:------------------------|
|<span data-ttu-id="ff3b3-216">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="ff3b3-216">Referrals admin</span></span>       |<span data-ttu-id="ff3b3-217">\*    Ver, crear y administrar los perfiles de negocio</span><span class="sxs-lookup"><span data-stu-id="ff3b3-217">\*    View, create, and manage business profiles</span></span>
||<span data-ttu-id="ff3b3-218">\*    Recibir y administrar referencias</span><span class="sxs-lookup"><span data-stu-id="ff3b3-218">\*    Receive and manage referrals</span></span>
||<span data-ttu-id="ff3b3-219">\*    Ver, crear y administrar referencias de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="ff3b3-219">\* View, create, and manage co-sell referrals</span></span>|
||<span data-ttu-id="ff3b3-220">\*    Ver, crear y administrar las solicitudes de servicio de los asociados</span><span class="sxs-lookup"><span data-stu-id="ff3b3-220">\*    View, create, and manage partner service requests</span></span>
|<span data-ttu-id="ff3b3-221">Administrador del perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="ff3b3-221">Business profile admin</span></span>   |<span data-ttu-id="ff3b3-222">\*    Ver, crear y administrar el perfil de negocio</span><span class="sxs-lookup"><span data-stu-id="ff3b3-222">\* View, create, and manage business profile</span></span> 
||<span data-ttu-id="ff3b3-223">\*    Ver, crear y administrar las solicitudes de servicio de los asociados</span><span class="sxs-lookup"><span data-stu-id="ff3b3-223">\*    View, create, and manage partner service requests</span></span>
||<span data-ttu-id="ff3b3-224">\*    Crear vales de soporte técnico para el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ff3b3-224">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="ff3b3-225">\*    Ver los vales de soporte técnico para partners que cree</span><span class="sxs-lookup"><span data-stu-id="ff3b3-225">\*    View partner support tickets you create</span></span>|

## <a name="manage-incentives"></a><span data-ttu-id="ff3b3-226">Administrar incentivos</span><span class="sxs-lookup"><span data-stu-id="ff3b3-226">Manage incentives</span></span> 

|<span data-ttu-id="ff3b3-227">**Rol**</span><span class="sxs-lookup"><span data-stu-id="ff3b3-227">**Role**</span></span> | <span data-ttu-id="ff3b3-228">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="ff3b3-228">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="ff3b3-229">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="ff3b3-229">Incentives admin</span></span>|<span data-ttu-id="ff3b3-230">\*    Iniciar y administrar incentivos</span><span class="sxs-lookup"><span data-stu-id="ff3b3-230">\*    Initiates and manages incentives</span></span> 
||<span data-ttu-id="ff3b3-231">\*    Ver y editar todos los aspectos de los programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="ff3b3-231">\*    Can view and edit all aspects of incentives programs</span></span>
||<span data-ttu-id="ff3b3-232">\*    Ver y editar información bancaria y fiscal</span><span class="sxs-lookup"><span data-stu-id="ff3b3-232">\*    Can view and edit bank and tax details</span></span>
||<span data-ttu-id="ff3b3-233">\*    Ver ganancias de devolución y cooperación</span><span class="sxs-lookup"><span data-stu-id="ff3b3-233">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="ff3b3-234">\*    Acceder a soporte técnico</span><span class="sxs-lookup"><span data-stu-id="ff3b3-234">\*    Access support</span></span>
||<span data-ttu-id="ff3b3-235">\*    Disputar pagos de incentivos</span><span class="sxs-lookup"><span data-stu-id="ff3b3-235">\*    Dispute incentives payments</span></span>|
|<span data-ttu-id="ff3b3-236">Usuario de incentivos</span><span class="sxs-lookup"><span data-stu-id="ff3b3-236">Incentives user</span></span>|<span data-ttu-id="ff3b3-237">\*    Ver programas de incentivos</span><span class="sxs-lookup"><span data-stu-id="ff3b3-237">\*    Can view incentives programs</span></span>
||<span data-ttu-id="ff3b3-238">\*    Ver e iniciar reclamaciones de incentivos</span><span class="sxs-lookup"><span data-stu-id="ff3b3-238">\*    Can view and initiate incentives claims</span></span>
||<span data-ttu-id="ff3b3-239">\*    Ver ganancias de devolución y cooperación</span><span class="sxs-lookup"><span data-stu-id="ff3b3-239">\*    View rebate and co-op earnings</span></span>
||<span data-ttu-id="ff3b3-240">\*    Crear vales de soporte técnico para el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ff3b3-240">\*    Create support tickets for the Partner Center</span></span>
||<span data-ttu-id="ff3b3-241">\*    Ver los vales de soporte técnico para partners que cree</span><span class="sxs-lookup"><span data-stu-id="ff3b3-241">\*    View partner support tickets you create</span></span>

## <a name="view-partner-center-insights-data"></a><span data-ttu-id="ff3b3-242">Ver datos de conclusiones del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ff3b3-242">View Partner Center Insights data</span></span>

|<span data-ttu-id="ff3b3-243">**Rol**</span><span class="sxs-lookup"><span data-stu-id="ff3b3-243">**Role**</span></span> | <span data-ttu-id="ff3b3-244">**Qué puede hacer**</span><span class="sxs-lookup"><span data-stu-id="ff3b3-244">**What you can do**</span></span>|
|------------------------------|:-------------------------|
|<span data-ttu-id="ff3b3-245">Visor de informes ejecutivos</span><span class="sxs-lookup"><span data-stu-id="ff3b3-245">Executive report viewer</span></span>|<span data-ttu-id="ff3b3-246">Acceder a todos los conjuntos de datos de informes, crear vales de soporte para partners, ver los vales de soporte técnico para partners que cree</span><span class="sxs-lookup"><span data-stu-id="ff3b3-246">Access to all reporting datasets, create partner support tickets, view partner support tickets you create</span></span>|
|<span data-ttu-id="ff3b3-247">Visor de informes</span><span class="sxs-lookup"><span data-stu-id="ff3b3-247">Report viewer</span></span>|<span data-ttu-id="ff3b3-248">Acceder a los informes de datos, con excepción de los ingresos y de los datos personales de clientes y empleados, crear vales de soporte para partners, ver los vales de soporte técnico para partners que cree</span><span class="sxs-lookup"><span data-stu-id="ff3b3-248">Access to data reports with exception of revenue and customer and employee personal data, create partner support tickets, view partner support tickets you create</span></span>|












                                    
