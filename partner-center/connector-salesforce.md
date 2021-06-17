---
title: El conector de venta co-sell para Salesforce CRM Centro de partners
ms.topic: how-to
ms.date: 01/06/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronice las referencias en Centro de partners con su CRM de Salesforce. A continuación, los vendedores pueden vender en colaboración con Microsoft desde sus sistemas CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 74894671966ac0409f6366f33c91ddadfae1ba4c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276984"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="49954-104">Conector de venta conjunta para Salesforce CRM: información general</span><span class="sxs-lookup"><span data-stu-id="49954-104">Co-sell connector for Salesforce CRM - overview</span></span>

<span data-ttu-id="49954-105">**Roles adecuados:** Administrador de referencias | Administrador del sistema o personalizador del sistema en CRM</span><span class="sxs-lookup"><span data-stu-id="49954-105">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

<span data-ttu-id="49954-106">Centro de partners conector de venta en colaboración permite a los vendedores realizar una venta en colaboración con Microsoft desde dentro de sus sistemas CRM.</span><span class="sxs-lookup"><span data-stu-id="49954-106">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="49954-107">No tendrán que entrenarse para usar Centro de partners administrar ofertas de venta co-venta.</span><span class="sxs-lookup"><span data-stu-id="49954-107">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="49954-108">Con los conectores de venta coventa, puede crear una nueva referencia de venta coventa para atraer a un vendedor de Microsoft, recibir referencias del vendedor de Microsoft, aceptar o rechazar referencias, modificar datos de oferta, como el valor de la oferta y la fecha de cierre.</span><span class="sxs-lookup"><span data-stu-id="49954-108">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="49954-109">También puede recibir cualquier actualización de los vendedores de Microsoft sobre estas ofertas de venta coventa.</span><span class="sxs-lookup"><span data-stu-id="49954-109">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="49954-110">Puede hacer que todas las referencias funcionen mientras trabaja en el CRM de su elección en lugar de en Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="49954-110">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="49954-111">La solución se basa en Microsoft Power Automate Solution y usa Centro de partners API.</span><span class="sxs-lookup"><span data-stu-id="49954-111">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="49954-112">Antes de instalar: requisitos previos</span><span class="sxs-lookup"><span data-stu-id="49954-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="49954-113">**Temas**</span><span class="sxs-lookup"><span data-stu-id="49954-113">**Topics**</span></span>   |<span data-ttu-id="49954-114">**Detalles**</span><span class="sxs-lookup"><span data-stu-id="49954-114">**Details**</span></span>   |<span data-ttu-id="49954-115">**Vínculos**</span><span class="sxs-lookup"><span data-stu-id="49954-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="49954-116">Microsoft Partner Network id.</span><span class="sxs-lookup"><span data-stu-id="49954-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="49954-117">Necesita un identificador de MPN válido.</span><span class="sxs-lookup"><span data-stu-id="49954-117">You need a valid MPN ID</span></span>|<span data-ttu-id="49954-118">Para unirse [a MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="49954-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="49954-119">Listo para la venta conjunta</span><span class="sxs-lookup"><span data-stu-id="49954-119">Co-sell ready</span></span>|<span data-ttu-id="49954-120">La solución IP/Services debe estar lista para la venta en colaboración.</span><span class="sxs-lookup"><span data-stu-id="49954-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="49954-121">Venta con Microsoft</span><span class="sxs-lookup"><span data-stu-id="49954-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="49954-122">Cuenta de Centro de partners</span><span class="sxs-lookup"><span data-stu-id="49954-122">Partner Center account</span></span>|<span data-ttu-id="49954-123">El identificador de MPN asociado al inquilino Centro de partners debe ser el mismo que el identificador de MPN asociado a la solución de venta simultánea.</span><span class="sxs-lookup"><span data-stu-id="49954-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="49954-124">Compruebe que puede ver las referencias de venta Centro de partners portal antes de implementar los conectores.</span><span class="sxs-lookup"><span data-stu-id="49954-124">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="49954-125">Administración de la cuenta</span><span class="sxs-lookup"><span data-stu-id="49954-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="49954-126">Roles de usuario del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="49954-126">Partner Center user roles</span></span>|<span data-ttu-id="49954-127">El empleado que instalará y usará los conectores debe ser un administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="49954-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="49954-128">Asignar roles y permisos de usuarios</span><span class="sxs-lookup"><span data-stu-id="49954-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="49954-129">Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="49954-129">Salesforce CRM</span></span>|<span data-ttu-id="49954-130">El rol de usuario de CRM es Administrador del sistema o Personalizador del sistema.</span><span class="sxs-lookup"><span data-stu-id="49954-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="49954-131">Asignación de roles en Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="49954-131">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="49954-132">Power Automate Flow Account</span><span class="sxs-lookup"><span data-stu-id="49954-132">Power Automate Flow Account</span></span>|<span data-ttu-id="49954-133">Una cuenta [Power Automate](https://flow.microsoft.com) activa para el administrador del sistema CRM o el personalizador del sistema.</span><span class="sxs-lookup"><span data-stu-id="49954-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="49954-134">Ese usuario debe iniciar sesión en [Power Automate](https://flow.microsoft.com) al menos una vez antes de la instalación.</span><span class="sxs-lookup"><span data-stu-id="49954-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="49954-135">Instalación del paquete de Salesforce para campos personalizados de Microsoft</span><span class="sxs-lookup"><span data-stu-id="49954-135">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="49954-136">Para sincronizar las referencias entre Centro de partners y Salesforce CRM, la solución Power Automate debe identificar claramente los campos de referencia específicos de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="49954-136">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft-specific referral fields.</span></span> <span data-ttu-id="49954-137">Esta demarcación proporciona a los equipos de vendedores asociados la capacidad de decidir qué referencias quieren compartir con Microsoft para la venta en colaboración.</span><span class="sxs-lookup"><span data-stu-id="49954-137">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="49954-138">En Salesforce, active **Notes (Notas)** y agrégrélo a la lista de oportunidades relacionadas.</span><span class="sxs-lookup"><span data-stu-id="49954-138">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="49954-139">Referencia</span><span class="sxs-lookup"><span data-stu-id="49954-139">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="49954-140">Active **los equipos de oportunidad** siguiendo estos pasos:</span><span class="sxs-lookup"><span data-stu-id="49954-140">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="49954-141">En Configuración, use el cuadro **Búsqueda rápida para** buscar Configuración del equipo de oportunidades.</span><span class="sxs-lookup"><span data-stu-id="49954-141">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="49954-142">Defina la configuración según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="49954-142">Define the settings as needed.</span></span>
[<span data-ttu-id="49954-143">Referencia</span><span class="sxs-lookup"><span data-stu-id="49954-143">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="49954-144">En Salesforce, instale campos y objetos personalizados mediante el [instalador de paquetes](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span><span class="sxs-lookup"><span data-stu-id="49954-144">In Salesforce, install custom fields and objects using the [package installer](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006WIwV).</span></span> <span data-ttu-id="49954-145">Úsese esto para instalar el paquete en cualquier empresa.</span><span class="sxs-lookup"><span data-stu-id="49954-145">Use this to install the package into any company.</span></span>

>[!NOTE]
><span data-ttu-id="49954-146">Si va a instalar en un espacio aislado, debe reemplazar la parte inicial de la dirección URL por http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="49954-146">If you are installing into a sandbox, you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="49954-147">En Salesforce, agregue Soluciones de Microsoft a la **lista relacionada** con oportunidades.</span><span class="sxs-lookup"><span data-stu-id="49954-147">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="49954-148">Una vez agregado, seleccione el icono **de llave inglesa** y actualice las propiedades.</span><span class="sxs-lookup"><span data-stu-id="49954-148">Once added, select the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="49954-149">Procedimiento recomendado: Prueba antes de empezar a realizar la ejecución</span><span class="sxs-lookup"><span data-stu-id="49954-149">Best Practice: Test before you go live</span></span>

<span data-ttu-id="49954-150">Antes de instalar, configurar y personalizar la solución Power Automate en el entorno de producción, asegúrese de probar la solución en una instancia de CRM de almacenamiento provisional.</span><span class="sxs-lookup"><span data-stu-id="49954-150">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="49954-151">Instale microsoft Power Automate solución en un entorno de ensayo o una instancia de CRM.</span><span class="sxs-lookup"><span data-stu-id="49954-151">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="49954-152">Realice una copia de la solución y ejecute la configuración y Power Automate de flujo en el entorno de ensayo.</span><span class="sxs-lookup"><span data-stu-id="49954-152">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="49954-153">Pruebe la solución en una instancia de almacenamiento provisional o CRM.</span><span class="sxs-lookup"><span data-stu-id="49954-153">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="49954-154">Si se ejecuta correctamente, importe como una solución administrada a la instancia de producción.</span><span class="sxs-lookup"><span data-stu-id="49954-154">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="49954-155">Instalación de Centro de partners de referencias para Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="49954-155">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="49954-156">Vaya a [Power Automate](https://flow.microsoft.com) seleccione **Entornos** en la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="49954-156">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="49954-157">Esto le mostrará las instancias de CRM disponibles.</span><span class="sxs-lookup"><span data-stu-id="49954-157">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="49954-158">Seleccione la instancia de CRM adecuada en la lista desplegable de la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="49954-158">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="49954-159">Seleccione **Soluciones en** la barra de navegación izquierda.</span><span class="sxs-lookup"><span data-stu-id="49954-159">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="49954-160">Seleccione el **vínculo Abrir AppSource** en el menú superior.</span><span class="sxs-lookup"><span data-stu-id="49954-160">Select the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abra AppSource.":::

5. <span data-ttu-id="49954-162">Busque **conectores Centro de partners referencias** para Salesforce en la pantalla emergente.</span><span class="sxs-lookup"><span data-stu-id="49954-162">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce.":::

6. <span data-ttu-id="49954-164">Seleccione el **botón Obtenerla ahora** y, a continuación, **Continuar.**</span><span class="sxs-lookup"><span data-stu-id="49954-164">Select the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="49954-165">Se abrirá la página donde puede seleccionar el entorno de Salesforce CRM para instalar la aplicación.</span><span class="sxs-lookup"><span data-stu-id="49954-165">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="49954-166">Acepte los términos y condiciones.</span><span class="sxs-lookup"><span data-stu-id="49954-166">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRMS disponibles.":::

8. <span data-ttu-id="49954-168">A continuación, se le dirigirá a la **página Administrar sus** soluciones.</span><span class="sxs-lookup"><span data-stu-id="49954-168">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="49954-169">Vaya a "Centro de partners referencias" mediante los botones de flecha de la parte inferior de la página.</span><span class="sxs-lookup"><span data-stu-id="49954-169">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="49954-170">**La instalación programada debe** aparecer junto a Centro de partners de referencias.</span><span class="sxs-lookup"><span data-stu-id="49954-170">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="49954-171">La instalación llevará entre 10 y 15 minutos.</span><span class="sxs-lookup"><span data-stu-id="49954-171">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="49954-172">Una vez completada la instalación, vuelva a [Power Automate](https://flow.microsoft.com) seleccione **Soluciones en** el área de navegación izquierda.</span><span class="sxs-lookup"><span data-stu-id="49954-172">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="49954-173">Observe que **Centro de partners sincronización de referencias para Salesforce** está disponible en la lista Soluciones.</span><span class="sxs-lookup"><span data-stu-id="49954-173">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="49954-174">Seleccione **Centro de partners de referencias para Salesforce.**</span><span class="sxs-lookup"><span data-stu-id="49954-174">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="49954-175">Las siguientes Power Automate y entidades están disponibles:</span><span class="sxs-lookup"><span data-stu-id="49954-175">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Flujos de Salesforce.":::



## <a name="configure-the-solution"></a><span data-ttu-id="49954-177">Configuración de la solución</span><span class="sxs-lookup"><span data-stu-id="49954-177">Configure the solution</span></span>

1. <span data-ttu-id="49954-178">Una vez que haya instalado la solución en la instancia de CRM, vuelva a [Power Automate](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="49954-178">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="49954-179">En la **lista desplegable Entornos** de la esquina superior derecha, seleccione la instancia de CRM donde instaló la Power Automate solución.</span><span class="sxs-lookup"><span data-stu-id="49954-179">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="49954-180">Deberá crear conexiones que asocie las tres cuentas de usuario:</span><span class="sxs-lookup"><span data-stu-id="49954-180">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="49954-181">Centro de partners usuario con credenciales de administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="49954-181">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="49954-182">Eventos del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="49954-182">Partner Center Events</span></span>
    - <span data-ttu-id="49954-183">El administrador de CRM con Power Automate flujos de la solución.</span><span class="sxs-lookup"><span data-stu-id="49954-183">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="49954-184">Seleccione **Conexiones** en la barra de navegación izquierda y seleccione la solución "Centro de partners Referencias" de la lista.</span><span class="sxs-lookup"><span data-stu-id="49954-184">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="49954-185">Cree una conexión haciendo clic en **Crear una conexión.**</span><span class="sxs-lookup"><span data-stu-id="49954-185">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Cree una conexión.":::

- <span data-ttu-id="49954-187">Busque Centro de partners referencias (versión preliminar) en la barra de búsqueda de la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="49954-187">Search for Partner Center Referrals (preview) in the search bar on the top-right corner.</span></span>

- <span data-ttu-id="49954-188">Cree una conexión para el usuario Centro de partners con el rol de credenciales del administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="49954-188">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="49954-189">A continuación, cree una Centro de partners events para el Centro de partners con las credenciales del administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="49954-189">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="49954-190">Cree una conexión para Salesforce para el usuario administrador de CRM.</span><span class="sxs-lookup"><span data-stu-id="49954-190">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="49954-191">Una vez que haya agregado todas las conexiones, debería ver las siguientes conexiones en su entorno:</span><span class="sxs-lookup"><span data-stu-id="49954-191">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Observe las conexiones.":::

### <a name="edit-the-connections"></a><span data-ttu-id="49954-193">Edición de las conexiones</span><span class="sxs-lookup"><span data-stu-id="49954-193">Edit the connections</span></span>

1. <span data-ttu-id="49954-194">Vuelva a la página Soluciones y seleccione **Solución predeterminada.**</span><span class="sxs-lookup"><span data-stu-id="49954-194">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="49954-195">Seleccione **Connection Reference (preview) (Referencia de conexión [versión preliminar])** haciendo clic **en All (Todos).**</span><span class="sxs-lookup"><span data-stu-id="49954-195">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Comience la edición del conector.":::

2. <span data-ttu-id="49954-197">Edite cada una de las conexiones individualmente seleccionando el icono de tres puntos.</span><span class="sxs-lookup"><span data-stu-id="49954-197">Edit each of the Connections individually by selecting the three dots icon.</span></span> <span data-ttu-id="49954-198">Agregue las conexiones pertinentes.</span><span class="sxs-lookup"><span data-stu-id="49954-198">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Edite los conectores.":::

3. <span data-ttu-id="49954-200">Active los flujos en la secuencia siguiente:</span><span class="sxs-lookup"><span data-stu-id="49954-200">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="49954-201">Centro de partners registro de webhook (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="49954-201">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="49954-202">Creación de una referencia de venta co-venta: Salesforce Centro de partners (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="49954-202">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="49954-203">Centro de partners de referencias de venta co-venta de Microsoft a Salesforce (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="49954-203">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="49954-204">Centro de partners a Salesforce (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="49954-204">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="49954-205">Salesforce to Centro de partners (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="49954-205">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="49954-206">Salesforce Opportunity to Centro de partners (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="49954-206">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="49954-207">Soluciones de Salesforce Microsoft para Centro de partners (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="49954-207">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="49954-208">Uso de api de webhook para registrarse para eventos de cambio de recursos</span><span class="sxs-lookup"><span data-stu-id="49954-208">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="49954-209">Las CENTRO DE PARTNERS webhook permiten registrarse para eventos de cambio de recursos.</span><span class="sxs-lookup"><span data-stu-id="49954-209">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="49954-210">Estos eventos de cambio se envían a la dirección URL como publicaciones HTTP.</span><span class="sxs-lookup"><span data-stu-id="49954-210">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="49954-211">Para registrar la dirección URL, **seleccione Centro de partners registro de webhook (versión preliminar de Insider)** Power Automate flujo.</span><span class="sxs-lookup"><span data-stu-id="49954-211">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="49954-212">Agregue conexiones para (a.) Centro de partners usuario con credenciales de administrador de referencias (b.) Centro de partners Eventos, como se resalta a continuación.</span><span class="sxs-lookup"><span data-stu-id="49954-212">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="detonante.":::

3. <span data-ttu-id="49954-214">Al realizar estas actualizaciones, verá</span><span class="sxs-lookup"><span data-stu-id="49954-214">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks.":::

4. <span data-ttu-id="49954-216">Guarde los cambios y seleccione **Activar**.</span><span class="sxs-lookup"><span data-stu-id="49954-216">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="49954-217">Para habilitar Centro de partners webhooks para escuchar los cambios de eventos, realice los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="49954-217">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="49954-218">Seleccione **Centro de partners a Salesforce CRM (Insider Preview).**</span><span class="sxs-lookup"><span data-stu-id="49954-218">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="49954-219">Seleccione el **icono Editar** y seleccione Cuando se recibe una **solicitud HTTP.**</span><span class="sxs-lookup"><span data-stu-id="49954-219">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="49954-220">Seleccione el **icono Copiar** para copiar la dirección URL de HTTP POST proporcionada.</span><span class="sxs-lookup"><span data-stu-id="49954-220">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copie la dirección URL.":::

8. <span data-ttu-id="49954-222">Ahora, seleccione el flujo "Centro de partners registro de webhook (insider preview)Power Automate" y seleccione **Ejecutar**.</span><span class="sxs-lookup"><span data-stu-id="49954-222">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="49954-223">Asegúrese de que se abre la ventana "Flujo de ejecución" en el panel derecho y seleccione **Continuar.**</span><span class="sxs-lookup"><span data-stu-id="49954-223">Ensure that the "Run Flow" window opens on the right-hand pane and select **Continue**.</span></span>

10. <span data-ttu-id="49954-224">Escriba la siguiente información:</span><span class="sxs-lookup"><span data-stu-id="49954-224">Enter the following details:</span></span>

    1. <span data-ttu-id="49954-225">**Punto de conexión de desencadenador HTTP:** dirección URL copiada del paso anterior</span><span class="sxs-lookup"><span data-stu-id="49954-225">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="49954-226">**Eventos para registrar:**"creación de referencias" y "referencia actualizada"</span><span class="sxs-lookup"><span data-stu-id="49954-226">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="49954-227">**Sobrescribir los puntos de conexión de desencadenador existentes si están** presentes: Sí (esto sobrescribe los puntos de conexión existentes).</span><span class="sxs-lookup"><span data-stu-id="49954-227">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="49954-228">Seleccione **Ejecutar y,** a continuación, **seleccione Listo.**</span><span class="sxs-lookup"><span data-stu-id="49954-228">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="49954-229">El webhook ahora puede escuchar para crear y actualizar eventos.</span><span class="sxs-lookup"><span data-stu-id="49954-229">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="49954-230">Personalización de los pasos de sincronización</span><span class="sxs-lookup"><span data-stu-id="49954-230">Customize synchronization steps</span></span>

<span data-ttu-id="49954-231">Cuando se sincronizan las referencias de venta Centro de partners y el sistema CRM, los campos que se sincronizan en Centro de partners PC se enumeran aquí.</span><span class="sxs-lookup"><span data-stu-id="49954-231">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="49954-232">A menudo, los sistemas CRM están muy personalizados.</span><span class="sxs-lookup"><span data-stu-id="49954-232">Often CRM systems are highly customized.</span></span> <span data-ttu-id="49954-233">Puede personalizar los flujos de Power Automate datos.</span><span class="sxs-lookup"><span data-stu-id="49954-233">You can customize the Power Automate flows.</span></span> <span data-ttu-id="49954-234">Siga la guía de asignación de campos y, si es necesario, realice los cambios adecuados en los pasos de los flujos Power Automate campo.</span><span class="sxs-lookup"><span data-stu-id="49954-234">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="49954-235">Se proporcionan asignaciones de Centros de partners de Microsoft a CRM, pero en función de su entorno crm, puede optar por personalizar aún más los campos.</span><span class="sxs-lookup"><span data-stu-id="49954-235">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="49954-236">Se pueden personalizar varios pasos de cada uno de los Power Automate en función de sus necesidades.</span><span class="sxs-lookup"><span data-stu-id="49954-236">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="49954-237">A continuación se muestran ejemplos de personalizaciones disponibles:</span><span class="sxs-lookup"><span data-stu-id="49954-237">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="49954-238">Para personalizar los campos de los eventos de creación o actualización en el Centro de partners sincronización de referencias de CRM:</span><span class="sxs-lookup"><span data-stu-id="49954-238">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="49954-239">Seleccione Centro de partners a Salesforce CRM (versión preliminar de Insider).</span><span class="sxs-lookup"><span data-stu-id="49954-239">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="49954-240">Seleccione **Editar** para editar o personalizar el flujo Power Automate datos.</span><span class="sxs-lookup"><span data-stu-id="49954-240">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="49954-241">Seleccione **(Ámbito) Sincronizar el cliente potencial o la oportunidad.**</span><span class="sxs-lookup"><span data-stu-id="49954-241">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="49954-242">Para personalizar las asignaciones de campos de CRM para crear eventos, seleccione Si es una nueva **oportunidad compartida y, a continuación,**.</span><span class="sxs-lookup"><span data-stu-id="49954-242">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="49954-243">Seleccione el subes paso si **es así y,** a continuación, expanda **Crear una nueva oportunidad en CRM.**</span><span class="sxs-lookup"><span data-stu-id="49954-243">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="49954-244">Puede editar las asignaciones de esta sección mediante la Guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="49954-244">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="49954-245">Para personalizar las asignaciones de campos de CRM para eventos de actualización, seleccione el paso "(Ámbito) Sincronizar el cliente potencial u oportunidad".</span><span class="sxs-lookup"><span data-stu-id="49954-245">To customize CRM field mappings for update events, select the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="49954-246">Seleccione **Si se trata de una actualización de una oportunidad, a continuación,**.</span><span class="sxs-lookup"><span data-stu-id="49954-246">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="49954-247">Seleccione el subes paso en caso afirmativo **y,** a continuación, expanda If difference between the opportunity objects in Centro de partners and CRM (Si la diferencia entre los objetos de oportunidad **de Centro de partners y CRM), a continuación, .**</span><span class="sxs-lookup"><span data-stu-id="49954-247">Select the sub-step **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="49954-248">Seleccione **If yes (Si es así)** seguido de **Update existing opportunity (Actualizar oportunidad existente).**</span><span class="sxs-lookup"><span data-stu-id="49954-248">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="49954-249">Para personalizar los campos para la sincronización de referencias de CRM a PC para eventos de actualización:</span><span class="sxs-lookup"><span data-stu-id="49954-249">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="49954-250">Seleccione **Editar**  para editar o personalizar el flujo Power Automate datos.</span><span class="sxs-lookup"><span data-stu-id="49954-250">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="49954-251">Seleccione **(Ámbito) Sincronizar la oportunidad.**</span><span class="sxs-lookup"><span data-stu-id="49954-251">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="49954-252">Para personalizar las asignaciones de campos de CRM (basadas en la guía de asignaciones de campos) para eventos de actualización, seleccione Si hay diferencias entre los objetos de cliente potencial en **Centro de partners y CRM y,** a continuación, .</span><span class="sxs-lookup"><span data-stu-id="49954-252">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="49954-253">Seleccione el subescalón en **caso afirmativo y,** a continuación, expanda el paso **Actualizar una referencia con datos de oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="49954-253">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="49954-254">Puede editar las asignaciones de esta sección en función de la Guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="49954-254">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="49954-255">¿Para personalizar los campos de sincronización de referencia de CRM a PC para crear eventos?</span><span class="sxs-lookup"><span data-stu-id="49954-255">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="49954-256">Seleccione **Editar**  para editar o personalizar el flujo Power Automate datos.</span><span class="sxs-lookup"><span data-stu-id="49954-256">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="49954-257">Seleccione **(Ámbito) Sincronizar referencias.**</span><span class="sxs-lookup"><span data-stu-id="49954-257">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="49954-258">Para personalizar las asignaciones de campos de CRM (basadas en la guía de asignaciones de campos) para crear eventos, seleccione **Crear referencia de Microsoft.**</span><span class="sxs-lookup"><span data-stu-id="49954-258">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="49954-259">Puede editar las asignaciones de esta sección en función de la Guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="49954-259">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="49954-260">Sincronización de referencias de venta bidireccional de un extremo a otro</span><span class="sxs-lookup"><span data-stu-id="49954-260">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="49954-261">Una vez que haya instalado, configurado y personalizado la solución Power Automate, puede probar la sincronización de referencias de venta co-venta entre Salesforce CRM y Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="49954-261">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="49954-262">Requisitos previos</span><span class="sxs-lookup"><span data-stu-id="49954-262">Pre-requisites</span></span>

<span data-ttu-id="49954-263">Para sincronizar las referencias entre Centro de partners y Salesforce CRM, la solución Power Automate debe delimitar claramente los campos de referencia específicos de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="49954-263">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="49954-264">Esta identificación proporciona a los equipos vendedores la capacidad de decidir qué referencias quieren compartir con Microsoft para la venta en colaboración.</span><span class="sxs-lookup"><span data-stu-id="49954-264">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="49954-265">Un conjunto de campos personalizados está disponible como parte de la Centro de partners sincronización de referencias para la oportunidad de la **solución** Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="49954-265">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="49954-266">Un usuario administrador de CRM deberá crear una sección de CRM independiente con los **campos personalizados Oportunidad.**</span><span class="sxs-lookup"><span data-stu-id="49954-266">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="49954-267">Los siguientes campos personalizados deben formar parte de la sección CRM:</span><span class="sxs-lookup"><span data-stu-id="49954-267">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="49954-268">**Sincronización con Centro de partners:** si se debe sincronizar la oportunidad con Microsoft Centro de partners</span><span class="sxs-lookup"><span data-stu-id="49954-268">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="49954-269">**Identificador de referencia:** campo de identificador de solo lectura para microsoft Centro de partners referencia</span><span class="sxs-lookup"><span data-stu-id="49954-269">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="49954-270">**Vínculo de referencia:** vínculo de solo lectura a la referencia en Microsoft Centro de partners</span><span class="sxs-lookup"><span data-stu-id="49954-270">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="49954-271">**¿Cómo puede ayudar Microsoft?**: Ayuda necesaria de Microsoft para la referencia</span><span class="sxs-lookup"><span data-stu-id="49954-271">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="49954-272">**Productos:** lista de productos asociados a esta oportunidad</span><span class="sxs-lookup"><span data-stu-id="49954-272">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="49954-273">**Auditoría:** un registro de auditoría de solo lectura para sincronizar con Centro de partners referencias</span><span class="sxs-lookup"><span data-stu-id="49954-273">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="49954-274">Escenarios:</span><span class="sxs-lookup"><span data-stu-id="49954-274">SCENARIOS:</span></span>

1. <span data-ttu-id="49954-275">Sincronización de referencias cuando se crea o actualiza la referencia en CRM y se sincroniza en Centro de partners:</span><span class="sxs-lookup"><span data-stu-id="49954-275">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="49954-276">Inicie sesión en el entorno de Salesforce CRM con el usuario que tenga visibilidad en la **sección Oportunidad** de CRM.</span><span class="sxs-lookup"><span data-stu-id="49954-276">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="49954-277">Asegúrese de que la siguiente sección está presente al crear una "nueva oportunidad" en el entorno de Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="49954-277">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Entorno de Salesforce.":::

   3. <span data-ttu-id="49954-279">Para sincronizar esta oportunidad con Microsoft Centro de partners, asegúrese de establecer los siguientes campos en la vista de tarjeta:</span><span class="sxs-lookup"><span data-stu-id="49954-279">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="49954-280">"Sincronizar con Centro de partners": Sí</span><span class="sxs-lookup"><span data-stu-id="49954-280">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="49954-281">"¿Cómo puede ayudar Microsoft?": seleccione una de las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="49954-281">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="49954-282">Productos: los IDs de solución del producto</span><span class="sxs-lookup"><span data-stu-id="49954-282">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="49954-283">Una vez que haya establecido la opción  **Sincronizar** con Centro de partners **en** Sí, espere 10 minutos, inicie sesión en Centro de partners cuenta.</span><span class="sxs-lookup"><span data-stu-id="49954-283">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="49954-284">Las referencias se sincronizarán con Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="49954-284">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="49954-285">Cuando la opción "Sincronizar con Centro de partners" está establecida en "Sí", si actualiza la oportunidad en Salesforce CRM, los cambios se sincronizarán con la cuenta Centro de partners cliente.</span><span class="sxs-lookup"><span data-stu-id="49954-285">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="49954-286">Las oportunidades que se sincronizan correctamente con Centro de partners se identificarán con ✔icono en Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="49954-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="49954-287">Sincronización de referencias cuando se crea o actualiza la referencia en Microsoft Centro de partners y sincroniza en el entorno de Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="49954-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="49954-288">Inicie sesión en Centro de partners [panel](https://partner.microsoft.com/dashboard/home).</span><span class="sxs-lookup"><span data-stu-id="49954-288">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="49954-289">Seleccione **Referencias en** el menú de la izquierda.</span><span class="sxs-lookup"><span data-stu-id="49954-289">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="49954-290">Cree una nueva referencia de venta Centro de partners haga clic en la opción "New deal" (Nueva oferta).</span><span class="sxs-lookup"><span data-stu-id="49954-290">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="49954-291">Inicie sesión en su entorno de Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="49954-291">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="49954-292">Vaya a **Open Opportunities (Oportunidades abiertas).**</span><span class="sxs-lookup"><span data-stu-id="49954-292">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="49954-293">La referencia creada en Microsoft Centro de partners ahora está sincronizada en Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="49954-293">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Pantalla de oportunidades de Salesforce.":::

    6. <span data-ttu-id="49954-295">Al seleccionar una referencia sincronizada, se rellenan los detalles de la vista de tarjeta.</span><span class="sxs-lookup"><span data-stu-id="49954-295">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="49954-296">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="49954-296">Next steps</span></span>

- [<span data-ttu-id="49954-297">Administrar los clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="49954-297">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="49954-298">Administrar las oportunidades de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="49954-298">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="49954-299">Webhooks del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="49954-299">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
