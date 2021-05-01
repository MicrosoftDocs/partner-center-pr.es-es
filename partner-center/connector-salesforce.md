---
title: El conector de venta co-sell para Salesforce CRM Centro de partners
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronice las referencias en Centro de partners con salesforce CRM. A continuación, los vendedores pueden vender en colaboración con Microsoft desde dentro de sus sistemas CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 8139f89a37048b1790353e3bdd18ac1b44887219
ms.sourcegitcommit: 1899307642f057070b1bdd647594fc46ba61fb08
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/30/2021
ms.locfileid: "108284390"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="5cfef-104">Conector de venta conjunta para Salesforce CRM: información general</span><span class="sxs-lookup"><span data-stu-id="5cfef-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="5cfef-105">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="5cfef-105">**Appropriate roles**</span></span>

- <span data-ttu-id="5cfef-106">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="5cfef-106">Referrals admin</span></span>
- <span data-ttu-id="5cfef-107">Administrador del sistema o personalizador del sistema en CRM</span><span class="sxs-lookup"><span data-stu-id="5cfef-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="5cfef-108">Centro de partners conector de venta en colaboración permite a los vendedores realizar la venta en colaboración con Microsoft desde dentro de los sistemas CRM.</span><span class="sxs-lookup"><span data-stu-id="5cfef-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="5cfef-109">No tendrán que entrenarse para usar Centro de partners administrar las ofertas de venta co-venta.</span><span class="sxs-lookup"><span data-stu-id="5cfef-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="5cfef-110">Con los conectores de venta coventa, puede crear una nueva referencia de venta conjunto para interactuar con un vendedor de Microsoft, recibir referencias del vendedor de Microsoft, aceptar o rechazar referencias, modificar los datos de la oferta, como el valor de la oferta y la fecha de cierre.</span><span class="sxs-lookup"><span data-stu-id="5cfef-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="5cfef-111">También puede recibir cualquier actualización de los vendedores de Microsoft en estas ofertas de venta coventa.</span><span class="sxs-lookup"><span data-stu-id="5cfef-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="5cfef-112">Puede hacer que todas las referencias funcionen mientras trabaja en el CRM que prefiera, en lugar de hacerlo Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="5cfef-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="5cfef-113">La solución se basa en microsoft Power Automate solución y usa Centro de partners API.</span><span class="sxs-lookup"><span data-stu-id="5cfef-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="5cfef-114">Antes de instalar: requisitos previos</span><span class="sxs-lookup"><span data-stu-id="5cfef-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="5cfef-115">**Temas**</span><span class="sxs-lookup"><span data-stu-id="5cfef-115">**Topics**</span></span>   |<span data-ttu-id="5cfef-116">**Detalles**</span><span class="sxs-lookup"><span data-stu-id="5cfef-116">**Details**</span></span>   |<span data-ttu-id="5cfef-117">**Vínculos**</span><span class="sxs-lookup"><span data-stu-id="5cfef-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="5cfef-118">Microsoft Partner Network id.</span><span class="sxs-lookup"><span data-stu-id="5cfef-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="5cfef-119">Necesita un identificador de MPN válido.</span><span class="sxs-lookup"><span data-stu-id="5cfef-119">You need a valid MPN ID</span></span>|<span data-ttu-id="5cfef-120">Para unirse [a MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="5cfef-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="5cfef-121">Listo para la venta conjunta</span><span class="sxs-lookup"><span data-stu-id="5cfef-121">Co-sell ready</span></span>|<span data-ttu-id="5cfef-122">La solución ip/services debe estar lista para la venta en colaboración.</span><span class="sxs-lookup"><span data-stu-id="5cfef-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="5cfef-123">Vender con Microsoft</span><span class="sxs-lookup"><span data-stu-id="5cfef-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="5cfef-124">Cuenta de Centro de partners</span><span class="sxs-lookup"><span data-stu-id="5cfef-124">Partner Center account</span></span>|<span data-ttu-id="5cfef-125">El identificador de MPN asociado al inquilino Centro de partners debe ser el mismo que el identificador de MPN asociado a la solución de venta simultánea.</span><span class="sxs-lookup"><span data-stu-id="5cfef-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="5cfef-126">Compruebe que puede ver las referencias de venta Centro de partners portal antes de implementar los conectores.</span><span class="sxs-lookup"><span data-stu-id="5cfef-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="5cfef-127">Administración de la cuenta</span><span class="sxs-lookup"><span data-stu-id="5cfef-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="5cfef-128">Roles de usuario del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="5cfef-128">Partner Center user roles</span></span>|<span data-ttu-id="5cfef-129">El empleado que instalará y usará los conectores debe ser un administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="5cfef-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="5cfef-130">Asignar roles y permisos de usuarios</span><span class="sxs-lookup"><span data-stu-id="5cfef-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="5cfef-131">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="5cfef-131">Salesforce CRM</span></span>|<span data-ttu-id="5cfef-132">El rol de usuario de CRM es Administrador del sistema o Personalizador del sistema.</span><span class="sxs-lookup"><span data-stu-id="5cfef-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="5cfef-133">Asignación de roles en Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="5cfef-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="5cfef-134">Power Automate Flow Account</span><span class="sxs-lookup"><span data-stu-id="5cfef-134">Power Automate Flow Account</span></span>|<span data-ttu-id="5cfef-135">Una cuenta [Power Automate](https://flow.microsoft.com) activa para el administrador del sistema CRM o el personalizador del sistema.</span><span class="sxs-lookup"><span data-stu-id="5cfef-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="5cfef-136">Ese usuario debe iniciar sesión en [Power Automate](https://flow.microsoft.com) al menos una vez antes de la instalación.</span><span class="sxs-lookup"><span data-stu-id="5cfef-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="5cfef-137">Instalación del paquete de Salesforce para campos personalizados de Microsoft</span><span class="sxs-lookup"><span data-stu-id="5cfef-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="5cfef-138">Para sincronizar las referencias entre Centro de partners y Salesforce CRM, la solución Power Automate debe identificar claramente los campos de referencia específicos de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5cfef-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="5cfef-139">Esta demarcación proporciona a los equipos de vendedores asociados la capacidad de decidir qué referencias quieren compartir con Microsoft para la venta en colaboración.</span><span class="sxs-lookup"><span data-stu-id="5cfef-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="5cfef-140">En Salesforce, active **Notes (Notas)** y agrégrélo a la lista de oportunidades relacionadas.</span><span class="sxs-lookup"><span data-stu-id="5cfef-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="5cfef-141">Referencia</span><span class="sxs-lookup"><span data-stu-id="5cfef-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="5cfef-142">Active **los equipos de oportunidad** siguiendo estos pasos:</span><span class="sxs-lookup"><span data-stu-id="5cfef-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="5cfef-143">En Configuración, use el cuadro **Búsqueda rápida para** buscar Configuración del equipo de oportunidades.</span><span class="sxs-lookup"><span data-stu-id="5cfef-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="5cfef-144">Defina la configuración según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="5cfef-144">Define the settings as needed.</span></span>
[<span data-ttu-id="5cfef-145">Referencia</span><span class="sxs-lookup"><span data-stu-id="5cfef-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="5cfef-146">En Salesforce, instale campos y objetos personalizados mediante el [instalador de paquetes](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span><span class="sxs-lookup"><span data-stu-id="5cfef-146">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="5cfef-147">Úsese esto para instalar el paquete en cualquier empresa.</span><span class="sxs-lookup"><span data-stu-id="5cfef-147">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="5cfef-148">Si va a instalar en un espacio aislado, debe reemplazar la parte inicial de la dirección URL por http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="5cfef-148">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="5cfef-149">En Salesforce, agregue Soluciones de Microsoft a la **lista relacionada** con oportunidades.</span><span class="sxs-lookup"><span data-stu-id="5cfef-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="5cfef-150">Una vez agregado, seleccione el icono **de llave inglesa** y actualice las propiedades.</span><span class="sxs-lookup"><span data-stu-id="5cfef-150">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="5cfef-151">Procedimiento recomendado: Prueba antes de empezar a realizar la ejecución</span><span class="sxs-lookup"><span data-stu-id="5cfef-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="5cfef-152">Antes de instalar, configurar y personalizar la solución Power Automate en el entorno de producción, asegúrese de probar la solución en una instancia de CRM de almacenamiento provisional.</span><span class="sxs-lookup"><span data-stu-id="5cfef-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="5cfef-153">Instale microsoft Power Automate solución en un entorno de ensayo o una instancia de CRM.</span><span class="sxs-lookup"><span data-stu-id="5cfef-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="5cfef-154">Realice una copia de la solución y ejecute la configuración y Power Automate de flujo en el entorno de ensayo.</span><span class="sxs-lookup"><span data-stu-id="5cfef-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="5cfef-155">Pruebe la solución en una instancia de almacenamiento provisional o CRM.</span><span class="sxs-lookup"><span data-stu-id="5cfef-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="5cfef-156">Si se ejecuta correctamente, importe como una solución administrada a la instancia de producción.</span><span class="sxs-lookup"><span data-stu-id="5cfef-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="5cfef-157">Instalación de Centro de partners de referencias para Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="5cfef-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="5cfef-158">Vaya a [Power Automate](https://flow.microsoft.com) y seleccione **Entornos en** la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="5cfef-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="5cfef-159">Esto le mostrará las instancias de CRM disponibles.</span><span class="sxs-lookup"><span data-stu-id="5cfef-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="5cfef-160">Seleccione la instancia de CRM adecuada en la lista desplegable de la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="5cfef-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="5cfef-161">Seleccione **Soluciones en** la barra de navegación izquierda.</span><span class="sxs-lookup"><span data-stu-id="5cfef-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="5cfef-162">Seleccione el **vínculo Abrir AppSource** en el menú superior.</span><span class="sxs-lookup"><span data-stu-id="5cfef-162">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abrir AppSource":::

5. <span data-ttu-id="5cfef-164">Busque **conectores Centro de partners referencias** para Salesforce en la pantalla emergente.</span><span class="sxs-lookup"><span data-stu-id="5cfef-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="5cfef-166">Seleccione el **botón Obtenerla ahora** y, a continuación, **Continuar.**</span><span class="sxs-lookup"><span data-stu-id="5cfef-166">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="5cfef-167">Se abrirá la página donde puede seleccionar el entorno de Salesforce CRM para instalar la aplicación.</span><span class="sxs-lookup"><span data-stu-id="5cfef-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="5cfef-168">Acepte los términos y condiciones.</span><span class="sxs-lookup"><span data-stu-id="5cfef-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRMS disponibles":::

8. <span data-ttu-id="5cfef-170">A continuación, se le dirigirá a la **página Administrar sus soluciones.**</span><span class="sxs-lookup"><span data-stu-id="5cfef-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="5cfef-171">Vaya a "Centro de partners referencias" mediante los botones de flecha de la parte inferior de la página.</span><span class="sxs-lookup"><span data-stu-id="5cfef-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="5cfef-172">**La instalación programada debe** aparecer junto a Centro de partners Solución de referencias.</span><span class="sxs-lookup"><span data-stu-id="5cfef-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="5cfef-173">La instalación llevará de 10 a 15 minutos.</span><span class="sxs-lookup"><span data-stu-id="5cfef-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="5cfef-174">Una vez completada la instalación, vuelva a [Power Automate](https://flow.microsoft.com) seleccione **Soluciones en** el área de navegación izquierda.</span><span class="sxs-lookup"><span data-stu-id="5cfef-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="5cfef-175">Observe que **Centro de partners sincronización de referencias para Salesforce** está disponible en la lista Soluciones.</span><span class="sxs-lookup"><span data-stu-id="5cfef-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="5cfef-176">Seleccione **Centro de partners de referencias para Salesforce.**</span><span class="sxs-lookup"><span data-stu-id="5cfef-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="5cfef-177">Las siguientes Power Automate y entidades están disponibles:</span><span class="sxs-lookup"><span data-stu-id="5cfef-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Flujos de Salesforce":::



## <a name="configure-the-solution"></a><span data-ttu-id="5cfef-179">Configuración de la solución</span><span class="sxs-lookup"><span data-stu-id="5cfef-179">Configure the solution</span></span>

1. <span data-ttu-id="5cfef-180">Una vez que haya instalado la solución en la instancia de CRM, vuelva a [Power Automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="5cfef-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="5cfef-181">En la **lista desplegable Entornos** de la esquina superior derecha, seleccione la instancia de CRM donde instaló la Power Automate solución.</span><span class="sxs-lookup"><span data-stu-id="5cfef-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="5cfef-182">Deberá crear conexiones que asocie las tres cuentas de usuario:</span><span class="sxs-lookup"><span data-stu-id="5cfef-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="5cfef-183">Centro de partners usuario con credenciales de administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="5cfef-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="5cfef-184">Eventos del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="5cfef-184">Partner Center Events</span></span>
    - <span data-ttu-id="5cfef-185">El administrador de CRM con Power Automate flujos de la solución.</span><span class="sxs-lookup"><span data-stu-id="5cfef-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="5cfef-186">Seleccione **Conexiones** en la barra de navegación izquierda y seleccione la solución "Centro de partners Referencias" de la lista.</span><span class="sxs-lookup"><span data-stu-id="5cfef-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="5cfef-187">Cree una conexión haciendo clic en **Crear una conexión.**</span><span class="sxs-lookup"><span data-stu-id="5cfef-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Crear conexión":::

- <span data-ttu-id="5cfef-189">Busque Centro de partners referencias (versión preliminar) en la barra de búsqueda de la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="5cfef-189">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="5cfef-190">Cree una conexión para el usuario Centro de partners con el rol de credenciales del administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="5cfef-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="5cfef-191">A continuación, cree una Centro de partners events para el Centro de partners con las credenciales del administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="5cfef-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="5cfef-192">Cree una conexión para Salesforce para el usuario administrador de CRM.</span><span class="sxs-lookup"><span data-stu-id="5cfef-192">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="5cfef-193">Una vez que haya agregado todas las conexiones, debería ver las siguientes conexiones en su entorno:</span><span class="sxs-lookup"><span data-stu-id="5cfef-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Observar conexiones":::

### <a name="edit-the-connections"></a><span data-ttu-id="5cfef-195">Edición de las conexiones</span><span class="sxs-lookup"><span data-stu-id="5cfef-195">Edit the connections</span></span>

1. <span data-ttu-id="5cfef-196">Vuelva a la página Soluciones y seleccione **Solución predeterminada.**</span><span class="sxs-lookup"><span data-stu-id="5cfef-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="5cfef-197">Seleccione **Connection Reference (preview) (Referencia de conexión [versión preliminar])** haciendo clic **en All (Todos).**</span><span class="sxs-lookup"><span data-stu-id="5cfef-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Inicio de la edición del conector":::

2. <span data-ttu-id="5cfef-199">Edite cada una de las conexiones individualmente seleccionando el icono de tres puntos.</span><span class="sxs-lookup"><span data-stu-id="5cfef-199">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="5cfef-200">Agregue las conexiones pertinentes.</span><span class="sxs-lookup"><span data-stu-id="5cfef-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Edición de conectores":::

3. <span data-ttu-id="5cfef-202">Active los flujos en la secuencia siguiente:</span><span class="sxs-lookup"><span data-stu-id="5cfef-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="5cfef-203">Centro de partners webhook Registration (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="5cfef-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="5cfef-204">Creación de una referencia de venta co-venta: Salesforce Centro de partners (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="5cfef-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="5cfef-205">Centro de partners microsoft co-sell Referral Updates to Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="5cfef-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="5cfef-206">Centro de partners a Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="5cfef-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="5cfef-207">Salesforce to Centro de partners (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="5cfef-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="5cfef-208">Salesforce Opportunity to Centro de partners (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="5cfef-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="5cfef-209">Soluciones de Salesforce microsoft para Centro de partners (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="5cfef-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="5cfef-210">Uso de api de webhook para registrarse para eventos de cambio de recursos</span><span class="sxs-lookup"><span data-stu-id="5cfef-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="5cfef-211">Las CENTRO DE PARTNERS webhook permiten registrarse para eventos de cambio de recursos.</span><span class="sxs-lookup"><span data-stu-id="5cfef-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="5cfef-212">Estos eventos de cambio se envían a la dirección URL como publicaciones HTTP.</span><span class="sxs-lookup"><span data-stu-id="5cfef-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="5cfef-213">Para registrar la dirección URL, **seleccione Centro de partners webhook Registration (Insider Preview) (Registro de webhook [insider preview])** Power Automate flujo.</span><span class="sxs-lookup"><span data-stu-id="5cfef-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="5cfef-214">Agregue conexiones para (a.) Centro de partners usuario con credenciales de administrador de referencias (b.) Centro de partners Eventos, como se resalta a continuación.</span><span class="sxs-lookup"><span data-stu-id="5cfef-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Desencadenador":::

3. <span data-ttu-id="5cfef-216">Al realizar estas actualizaciones, verá</span><span class="sxs-lookup"><span data-stu-id="5cfef-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="5cfef-218">Guarde los cambios y seleccione **Activar**.</span><span class="sxs-lookup"><span data-stu-id="5cfef-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="5cfef-219">Para habilitar Centro de partners webhooks para escuchar los cambios de eventos, realice los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="5cfef-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="5cfef-220">Seleccione **Centro de partners a Salesforce CRM (Insider Preview).**</span><span class="sxs-lookup"><span data-stu-id="5cfef-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="5cfef-221">Seleccione el **icono Editar** y seleccione Cuando se recibe una **solicitud HTTP.**</span><span class="sxs-lookup"><span data-stu-id="5cfef-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="5cfef-222">Seleccione el **icono Copiar** para copiar la dirección URL de HTTP POST proporcionada.</span><span class="sxs-lookup"><span data-stu-id="5cfef-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copiar la dirección URL":::

8. <span data-ttu-id="5cfef-224">Ahora, seleccione el flujo de Centro de partners registro de webhook (insider preview)Power Automate" y seleccione **Ejecutar**.</span><span class="sxs-lookup"><span data-stu-id="5cfef-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="5cfef-225">Asegúrese de que se abre la ventana "Flujo de ejecución" en el panel derecho y seleccione **Continuar.**</span><span class="sxs-lookup"><span data-stu-id="5cfef-225">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="5cfef-226">Escriba la siguiente información:</span><span class="sxs-lookup"><span data-stu-id="5cfef-226">Enter the following details:</span></span>

    1. <span data-ttu-id="5cfef-227">**Punto de conexión de desencadenador http:** dirección URL copiada del paso anterior</span><span class="sxs-lookup"><span data-stu-id="5cfef-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="5cfef-228">**Eventos para registrar:**"creados por referencia" y "actualizados por referencia"</span><span class="sxs-lookup"><span data-stu-id="5cfef-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="5cfef-229">**Sobrescribir los puntos de conexión de desencadenador existentes si están** presentes: Sí (esto sobrescribe los puntos de conexión existentes).</span><span class="sxs-lookup"><span data-stu-id="5cfef-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="5cfef-230">Seleccione **Ejecutar y,** a continuación, **seleccione Listo.**</span><span class="sxs-lookup"><span data-stu-id="5cfef-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="5cfef-231">El webhook ahora puede escuchar para crear y actualizar eventos.</span><span class="sxs-lookup"><span data-stu-id="5cfef-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="5cfef-232">Personalización de los pasos de sincronización</span><span class="sxs-lookup"><span data-stu-id="5cfef-232">Customize synchronization steps</span></span>

<span data-ttu-id="5cfef-233">Cuando se sincronizan las referencias de venta Centro de partners y el sistema CRM, los campos que se sincronizan en Centro de partners PC se enumeran aquí.</span><span class="sxs-lookup"><span data-stu-id="5cfef-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="5cfef-234">A menudo, los sistemas CRM están muy personalizados.</span><span class="sxs-lookup"><span data-stu-id="5cfef-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="5cfef-235">Puede personalizar los flujos de Power Automate datos.</span><span class="sxs-lookup"><span data-stu-id="5cfef-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="5cfef-236">Siga la guía de asignación de campos y, si es necesario, realice los cambios adecuados en los pasos de Power Automate flujos.</span><span class="sxs-lookup"><span data-stu-id="5cfef-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="5cfef-237">Se proporcionan asignaciones de Centros de partners de Microsoft a CRM, pero en función de su entorno crm, puede optar por personalizar aún más los campos.</span><span class="sxs-lookup"><span data-stu-id="5cfef-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="5cfef-238">Varios pasos de cada uno de los Power Automate se pueden personalizar en función de sus necesidades.</span><span class="sxs-lookup"><span data-stu-id="5cfef-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="5cfef-239">A continuación se muestran ejemplos de personalizaciones disponibles:</span><span class="sxs-lookup"><span data-stu-id="5cfef-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="5cfef-240">Para personalizar los campos de los eventos de creación o actualización en el Centro de partners sincronización de referencias de CRM:</span><span class="sxs-lookup"><span data-stu-id="5cfef-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="5cfef-241">Seleccione Centro de partners a Salesforce CRM (Insider Preview).</span><span class="sxs-lookup"><span data-stu-id="5cfef-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="5cfef-242">Seleccione **Editar** para editar o personalizar el flujo Power Automate datos.</span><span class="sxs-lookup"><span data-stu-id="5cfef-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="5cfef-243">Seleccione **(Ámbito) Sincronizar el cliente potencial o la oportunidad.**</span><span class="sxs-lookup"><span data-stu-id="5cfef-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="5cfef-244">Para personalizar las asignaciones de campos de CRM para crear eventos, seleccione Si es una nueva **oportunidad compartida y, a continuación,**.</span><span class="sxs-lookup"><span data-stu-id="5cfef-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="5cfef-245">Seleccione el subes paso si **es así y,** a continuación, expanda **Crear una nueva oportunidad en CRM.**</span><span class="sxs-lookup"><span data-stu-id="5cfef-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="5cfef-246">Puede editar las asignaciones de esta sección mediante la Guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="5cfef-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="5cfef-247">Para personalizar las asignaciones de campos de CRM para eventos de actualización, seleccione el paso "(Ámbito) Sincronizar el cliente potencial u oportunidad".</span><span class="sxs-lookup"><span data-stu-id="5cfef-247">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="5cfef-248">Seleccione **Si se trata de una actualización de una oportunidad, a continuación,**.</span><span class="sxs-lookup"><span data-stu-id="5cfef-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="5cfef-249">Seleccione el subes paso en caso afirmativo **y,** a continuación, expanda If difference between the opportunity objects in Centro de partners and CRM (Si la diferencia entre los objetos de oportunidad **de Centro de partners y CRM), a continuación, .**</span><span class="sxs-lookup"><span data-stu-id="5cfef-249">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="5cfef-250">Seleccione **If yes (Si es así)** seguido de **Update existing opportunity (Actualizar oportunidad existente).**</span><span class="sxs-lookup"><span data-stu-id="5cfef-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="5cfef-251">Para personalizar los campos para la sincronización de referencias de CRM a PC para eventos de actualización:</span><span class="sxs-lookup"><span data-stu-id="5cfef-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="5cfef-252">Seleccione **Editar**  para editar o personalizar el flujo Power Automate datos.</span><span class="sxs-lookup"><span data-stu-id="5cfef-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="5cfef-253">Seleccione **(Ámbito) Sincronizar la oportunidad.**</span><span class="sxs-lookup"><span data-stu-id="5cfef-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="5cfef-254">Para personalizar las asignaciones de campos de CRM (basadas en la guía de asignaciones de campos) para eventos de actualización, seleccione Si hay diferencias entre los objetos de cliente potencial **en Centro de partners y CRM y, a continuación,**.</span><span class="sxs-lookup"><span data-stu-id="5cfef-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="5cfef-255">Seleccione el subescalón en **caso afirmativo y,** a continuación, expanda el paso **Actualizar una referencia con datos de oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="5cfef-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="5cfef-256">Puede editar las asignaciones de esta sección en función de la Guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="5cfef-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="5cfef-257">¿Para personalizar los campos de sincronización de referencia de CRM a PC para crear eventos?</span><span class="sxs-lookup"><span data-stu-id="5cfef-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="5cfef-258">Seleccione **Editar**  para editar o personalizar el flujo Power Automate datos.</span><span class="sxs-lookup"><span data-stu-id="5cfef-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="5cfef-259">Seleccione **(Ámbito) Sincronizar referencias.**</span><span class="sxs-lookup"><span data-stu-id="5cfef-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="5cfef-260">Para personalizar las asignaciones de campos de CRM (basadas en la guía de asignaciones de campos) para crear eventos, seleccione **Crear referencia de Microsoft.**</span><span class="sxs-lookup"><span data-stu-id="5cfef-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="5cfef-261">Puede editar las asignaciones de esta sección en función de la Guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="5cfef-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="5cfef-262">Sincronización de referencias de venta bidireccional de un extremo a otro</span><span class="sxs-lookup"><span data-stu-id="5cfef-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="5cfef-263">Una vez que haya instalado, configurado y personalizado la solución Power Automate, puede probar la sincronización de referencias de venta co-venta entre Salesforce CRM y Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="5cfef-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="5cfef-264">Requisitos previos</span><span class="sxs-lookup"><span data-stu-id="5cfef-264">Pre-requisites</span></span>

<span data-ttu-id="5cfef-265">Para sincronizar las referencias entre Centro de partners y Salesforce CRM, la solución Power Automate debe delimitar claramente los campos de referencia específicos de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5cfef-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="5cfef-266">Esta identificación proporciona a los equipos vendedores la capacidad de decidir qué referencias quieren compartir con Microsoft para la venta en colaboración.</span><span class="sxs-lookup"><span data-stu-id="5cfef-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="5cfef-267">Un conjunto de campos personalizados está disponible como parte de la Centro de partners de referencias para la entidad de oportunidad de **la** solución Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="5cfef-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="5cfef-268">Un usuario administrador de CRM deberá crear una sección de CRM independiente con los **campos personalizados oportunidad.**</span><span class="sxs-lookup"><span data-stu-id="5cfef-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="5cfef-269">Los siguientes campos personalizados deben formar parte de la sección CRM:</span><span class="sxs-lookup"><span data-stu-id="5cfef-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="5cfef-270">**Sincronización con Centro de partners:** si se debe sincronizar la oportunidad con Microsoft Centro de partners</span><span class="sxs-lookup"><span data-stu-id="5cfef-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="5cfef-271">**Identificador de referencia:** campo de identificador de solo lectura para microsoft Centro de partners referencia</span><span class="sxs-lookup"><span data-stu-id="5cfef-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="5cfef-272">**Vínculo de referencia:** vínculo de solo lectura a la referencia en Microsoft Centro de partners</span><span class="sxs-lookup"><span data-stu-id="5cfef-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="5cfef-273">**Ayuda de Microsoft:** Ayuda necesaria de Microsoft para la referencia</span><span class="sxs-lookup"><span data-stu-id="5cfef-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="5cfef-274">**Productos:** lista de productos asociados a esta oportunidad</span><span class="sxs-lookup"><span data-stu-id="5cfef-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="5cfef-275">**Auditoría:** un registro de auditoría de solo lectura para sincronizar con Centro de partners referencias</span><span class="sxs-lookup"><span data-stu-id="5cfef-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="5cfef-276">Escenarios:</span><span class="sxs-lookup"><span data-stu-id="5cfef-276">SCENARIOS:</span></span>

1. <span data-ttu-id="5cfef-277">Sincronización de referencias cuando se crea o actualiza la referencia en CRM y se sincroniza en Centro de partners:</span><span class="sxs-lookup"><span data-stu-id="5cfef-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="5cfef-278">Inicie sesión en el entorno de Salesforce CRM con el usuario que tenga visibilidad en la **sección Oportunidad** de CRM.</span><span class="sxs-lookup"><span data-stu-id="5cfef-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="5cfef-279">Asegúrese de que la siguiente sección está presente al crear una "nueva oportunidad" en el entorno de Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="5cfef-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Entorno de Salesforce":::

   3. <span data-ttu-id="5cfef-281">Para sincronizar esta oportunidad con Microsoft Centro de partners, asegúrese de establecer los siguientes campos en la vista de tarjeta:</span><span class="sxs-lookup"><span data-stu-id="5cfef-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="5cfef-282">"Sincronizar con Centro de partners": Sí</span><span class="sxs-lookup"><span data-stu-id="5cfef-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="5cfef-283">"¿Cómo puede ayudar Microsoft?": seleccione una de las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="5cfef-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="5cfef-284">Productos: los IDs de solución del producto</span><span class="sxs-lookup"><span data-stu-id="5cfef-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="5cfef-285">Una vez que haya establecido la opción  **Sincronizar** con Centro de partners **en** Sí, espere 10 minutos, inicie sesión en Centro de partners cuenta.</span><span class="sxs-lookup"><span data-stu-id="5cfef-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="5cfef-286">Las referencias se sincronizarán con Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="5cfef-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="5cfef-287">Cuando la opción "Sincronizar con Centro de partners" está establecida en "Sí", si actualiza la oportunidad en Salesforce CRM, los cambios se sincronizarán con la cuenta Centro de partners cliente.</span><span class="sxs-lookup"><span data-stu-id="5cfef-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="5cfef-288">Las oportunidades que se sincronizan correctamente con Centro de partners se identificarán con ✔icono en Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="5cfef-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="5cfef-289">Sincronización de referencias cuando se crea o actualiza la referencia en Microsoft Centro de partners y sincroniza en el entorno de Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="5cfef-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="5cfef-290">Inicie sesión en Centro de partners [panel](https://partner.microsoft.com/dashboard/home).</span><span class="sxs-lookup"><span data-stu-id="5cfef-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="5cfef-291">Seleccione **Referencias en** el menú de la izquierda.</span><span class="sxs-lookup"><span data-stu-id="5cfef-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="5cfef-292">Cree una nueva referencia de venta Centro de partners haga clic en la opción "New deal" (Nueva oferta).</span><span class="sxs-lookup"><span data-stu-id="5cfef-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="5cfef-293">Inicie sesión en su entorno de Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="5cfef-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="5cfef-294">Vaya a **Open Opportunities (Oportunidades abiertas).**</span><span class="sxs-lookup"><span data-stu-id="5cfef-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="5cfef-295">La referencia creada en Microsoft Centro de partners ahora está sincronizada en Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="5cfef-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Pantalla de oportunidades de Salesforce":::

    6. <span data-ttu-id="5cfef-297">Al seleccionar una referencia sincronizada, se rellenan los detalles de la vista de tarjeta.</span><span class="sxs-lookup"><span data-stu-id="5cfef-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5cfef-298">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="5cfef-298">Next steps</span></span>

- [<span data-ttu-id="5cfef-299">Administrar los clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="5cfef-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="5cfef-300">Administrar las oportunidades de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="5cfef-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="5cfef-301">Webhooks del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="5cfef-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
