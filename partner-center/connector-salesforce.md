---
title: El conector de venta conjunta para el centro de Partners de Salesforce CRM
ms.topic: how-to
ms.date: 09/29/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizar las referencias en el centro de Partners con el CRM de Salesforce. A continuación, los vendedores pueden colaborar con Microsoft desde los sistemas CRM.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: b73f0b24538daa18b93fa206fce5eda1ab9bc9b9
ms.sourcegitcommit: 7e32544cf91f932cbeb053c9de506ba9ee773fe2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/20/2020
ms.locfileid: "94947858"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="02fc7-104">Conector de venta conjunta para Salesforce CRM: información general</span><span class="sxs-lookup"><span data-stu-id="02fc7-104">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="02fc7-105">Roles adecuados</span><span class="sxs-lookup"><span data-stu-id="02fc7-105">Appropriate roles</span></span>

- <span data-ttu-id="02fc7-106">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="02fc7-106">Referrals admin</span></span>
- <span data-ttu-id="02fc7-107">Administrador del sistema o Personalizador del sistema en CRM</span><span class="sxs-lookup"><span data-stu-id="02fc7-107">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="02fc7-108">El conector de la venta conjunta del centro de Partners permite que los vendedores covendan con Microsoft desde los sistemas CRM.</span><span class="sxs-lookup"><span data-stu-id="02fc7-108">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="02fc7-109">No tendrán que estar capacitados para utilizar el centro de partners para administrar las ofertas de venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="02fc7-109">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="02fc7-110">Mediante el uso de conectores de venta conjunta, puede crear una nueva referencia de venta conjunta para participar en un vendedor de Microsoft, recibir referencias del vendedor de Microsoft, aceptar o rechazar las referencias, modificar los datos del negocio, como el valor del negocio y la fecha de cierre.</span><span class="sxs-lookup"><span data-stu-id="02fc7-110">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="02fc7-111">También puede recibir cualquier actualización de los vendedores de Microsoft en estos acuerdos de venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="02fc7-111">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="02fc7-112">Puede hacer que todas las referencias funcionen mientras trabaja en el CRM de su elección, en lugar de hacerlo en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="02fc7-112">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="02fc7-113">La solución se basa en la solución Microsoft Power Automate y usa las API del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="02fc7-113">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="02fc7-114">Antes de instalar: requisitos previos</span><span class="sxs-lookup"><span data-stu-id="02fc7-114">Before you install - pre-requisites</span></span>

|<span data-ttu-id="02fc7-115">**Temas**</span><span class="sxs-lookup"><span data-stu-id="02fc7-115">**Topics**</span></span>   |<span data-ttu-id="02fc7-116">**Detalles**</span><span class="sxs-lookup"><span data-stu-id="02fc7-116">**Details**</span></span>   |<span data-ttu-id="02fc7-117">**Vínculos**</span><span class="sxs-lookup"><span data-stu-id="02fc7-117">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="02fc7-118">IDENTIFICADOR de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="02fc7-118">Microsoft Partner Network ID</span></span> |<span data-ttu-id="02fc7-119">Necesita un ID. de MPN válido</span><span class="sxs-lookup"><span data-stu-id="02fc7-119">You need a valid MPN ID</span></span>|<span data-ttu-id="02fc7-120">Para unirse a [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="02fc7-120">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="02fc7-121">Listo para la venta conjunta</span><span class="sxs-lookup"><span data-stu-id="02fc7-121">Co-sell ready</span></span>|<span data-ttu-id="02fc7-122">La solución de IP/servicios debe estar lista para su venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="02fc7-122">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="02fc7-123">Venda con Microsoft</span><span class="sxs-lookup"><span data-stu-id="02fc7-123">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="02fc7-124">Cuenta de Centro de partners</span><span class="sxs-lookup"><span data-stu-id="02fc7-124">Partner Center account</span></span>|<span data-ttu-id="02fc7-125">El identificador de MPN asociado al inquilino del centro de Partners debe ser el mismo que el identificador de MPN asociado a la solución de venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="02fc7-125">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="02fc7-126">Compruebe que puede ver las referencias de venta conjunta en el portal del centro de Partners antes de implementar los conectores.</span><span class="sxs-lookup"><span data-stu-id="02fc7-126">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="02fc7-127">Administración de la cuenta</span><span class="sxs-lookup"><span data-stu-id="02fc7-127">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="02fc7-128">Roles de usuario del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="02fc7-128">Partner Center user roles</span></span>|<span data-ttu-id="02fc7-129">El empleado que va a instalar y usar los conectores debe ser un administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="02fc7-129">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="02fc7-130">Asignar roles y permisos de usuarios</span><span class="sxs-lookup"><span data-stu-id="02fc7-130">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="02fc7-131">CRM de Salesforce</span><span class="sxs-lookup"><span data-stu-id="02fc7-131">Salesforce CRM</span></span>|<span data-ttu-id="02fc7-132">El rol de usuario CRM es administrador del sistema o Personalizador del sistema</span><span class="sxs-lookup"><span data-stu-id="02fc7-132">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="02fc7-133">Asignación de roles en el CRM de Salesforce</span><span class="sxs-lookup"><span data-stu-id="02fc7-133">Assign roles in Salesforce CRM</span></span>](https://help.salesforce.com/articleView?id=assigning_users_to_roles.htm&type=5)|
|<span data-ttu-id="02fc7-134">Cuenta de flujo de automatización de energía</span><span class="sxs-lookup"><span data-stu-id="02fc7-134">Power Automate Flow Account</span></span>|<span data-ttu-id="02fc7-135">Una cuenta activa de [Power Automatic](https://flow.microsoft.com) para el administrador del sistema CRM o el personalizador del sistema.</span><span class="sxs-lookup"><span data-stu-id="02fc7-135">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="02fc7-136">Dicho usuario debe iniciar sesión en [Power automatizate](https://flow.microsoft.com) al menos una vez antes de la instalación.</span><span class="sxs-lookup"><span data-stu-id="02fc7-136">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="installation-of-salesforce-package-for-microsoft-custom-fields"></a><span data-ttu-id="02fc7-137">Instalación del paquete de Salesforce para los campos personalizados de Microsoft</span><span class="sxs-lookup"><span data-stu-id="02fc7-137">Installation of Salesforce Package for Microsoft Custom Fields</span></span> 

<span data-ttu-id="02fc7-138">Para sincronizar las referencias entre el centro de Partners y el CRM de Salesforce, la solución Power Automate debe identificar claramente los campos de referencia específicos de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="02fc7-138">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly identify Microsoft specific referral fields.</span></span> <span data-ttu-id="02fc7-139">Esta demarcación proporciona a los equipos de los vendedores asociados la capacidad de decidir qué referencias desean compartir con Microsoft para la venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="02fc7-139">This demarcation provides partner seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

1. <span data-ttu-id="02fc7-140">En Salesforce, Active **notas** y agréguelo a la lista oportunidades relacionadas.</span><span class="sxs-lookup"><span data-stu-id="02fc7-140">In Salesforce, activate **Notes** and add it to the opportunities related list.</span></span> 
[<span data-ttu-id="02fc7-141">Referencia</span><span class="sxs-lookup"><span data-stu-id="02fc7-141">Reference</span></span>](https://help.salesforce.com/articleView?err=1&id=notes_admin_setup.htm&type=5)

2. <span data-ttu-id="02fc7-142">Active los **equipos de oportunidades** siguiendo estos pasos:</span><span class="sxs-lookup"><span data-stu-id="02fc7-142">Activate **Opportunity teams** by following the steps:</span></span> 
    - <span data-ttu-id="02fc7-143">En el programa de instalación, use el cuadro **búsqueda rápida** para buscar la configuración del equipo de oportunidades.</span><span class="sxs-lookup"><span data-stu-id="02fc7-143">In Setup, use the **Quick Find** box to locate Opportunity Team Settings.</span></span>
    - <span data-ttu-id="02fc7-144">Defina la configuración según sea necesario.</span><span class="sxs-lookup"><span data-stu-id="02fc7-144">Define the settings as needed.</span></span>
[<span data-ttu-id="02fc7-145">Referencia</span><span class="sxs-lookup"><span data-stu-id="02fc7-145">Reference</span></span>](https://help.salesforce.com/articleView?id=teamselling_enabling.htm&type=5]) 

3. <span data-ttu-id="02fc7-146">En Salesforce, instale los campos y objetos personalizados con el instalador de paquetes a continuación.</span><span class="sxs-lookup"><span data-stu-id="02fc7-146">In Salesforce, install custom fields and objects using package installer below.</span></span>
  
<span data-ttu-id="02fc7-147">Vaya [aquí](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) para instalar el paquete en cualquier compañía:</span><span class="sxs-lookup"><span data-stu-id="02fc7-147">Go [here](https://login.salesforce.com/packaging/installPackage.apexp?p0=04t2w000006Vs9a) to install the package into any company:</span></span>


<span data-ttu-id="02fc7-148">Nota: Si va a instalar en un espacio aislado, debe reemplazar la parte inicial de la dirección URL por http://test.salesforce.com</span><span class="sxs-lookup"><span data-stu-id="02fc7-148">Note: If you are installing into a sandbox you must replace the initial portion of the URL with http://test.salesforce.com</span></span>

4. <span data-ttu-id="02fc7-149">En Salesforce, agregue soluciones de Microsoft a la lista de **oportunidades** relacionadas.</span><span class="sxs-lookup"><span data-stu-id="02fc7-149">In Salesforce, add Microsoft Solutions to the **Opportunity** related list.</span></span> <span data-ttu-id="02fc7-150">Una vez agregado, haga clic en el icono de **llave inglesa** y actualice las propiedades.</span><span class="sxs-lookup"><span data-stu-id="02fc7-150">Once added, click on the **wrench** icon and update properties</span></span>

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="02fc7-151">Procedimiento recomendado: prueba antes de la marcha</span><span class="sxs-lookup"><span data-stu-id="02fc7-151">Best Practice: Test before you go live</span></span>

<span data-ttu-id="02fc7-152">Antes de instalar, configurar y personalizar la solución Power Automate en el entorno de producción, asegúrese de probar la solución en una instancia de CRM provisional.</span><span class="sxs-lookup"><span data-stu-id="02fc7-152">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="02fc7-153">Instale la solución Microsoft Power Automate en un entorno de ensayo o una instancia de CRM.</span><span class="sxs-lookup"><span data-stu-id="02fc7-153">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="02fc7-154">Realice una copia de la solución y ejecute la configuración y la automatización de las personalizaciones de flujo en el entorno de ensayo.</span><span class="sxs-lookup"><span data-stu-id="02fc7-154">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="02fc7-155">Pruebe la solución en una instancia de ensayo o CRM.</span><span class="sxs-lookup"><span data-stu-id="02fc7-155">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="02fc7-156">Si se realiza correctamente, importe como una solución administrada a la instancia de producción.</span><span class="sxs-lookup"><span data-stu-id="02fc7-156">On success, import as a managed solution to the production instance.</span></span>

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="02fc7-157">Instalación de la sincronización de referencias del centro de partners para Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="02fc7-157">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="02fc7-158">Vaya a [Power Automatic](https://flow.microsoft.com) y seleccione **entornos** en la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="02fc7-158">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="02fc7-159">Se mostrarán las instancias de CRM disponibles.</span><span class="sxs-lookup"><span data-stu-id="02fc7-159">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="02fc7-160">Seleccione la instancia de CRM correspondiente en la lista desplegable de la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="02fc7-160">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="02fc7-161">Seleccione **soluciones** en la barra de navegación izquierda.</span><span class="sxs-lookup"><span data-stu-id="02fc7-161">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="02fc7-162">Haga clic en el vínculo **abrir AppSource** en el menú superior.</span><span class="sxs-lookup"><span data-stu-id="02fc7-162">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abrir AppSource":::

5. <span data-ttu-id="02fc7-164">Busque **conectores de referencias del centro de partners para Salesforce** en la pantalla emergente.</span><span class="sxs-lookup"><span data-stu-id="02fc7-164">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="02fc7-166">Haga clic en el botón **obtener ahora** y **continúe**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-166">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="02fc7-167">Se abrirá la página en la que puede seleccionar el entorno de Salesforce CRM para instalar la aplicación.</span><span class="sxs-lookup"><span data-stu-id="02fc7-167">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="02fc7-168">Acepte los términos y condiciones.</span><span class="sxs-lookup"><span data-stu-id="02fc7-168">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRMS disponibles":::

8. <span data-ttu-id="02fc7-170">A continuación, se le dirigirá a la página **administrar soluciones** .</span><span class="sxs-lookup"><span data-stu-id="02fc7-170">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="02fc7-171">Vaya a "referencias del centro de Partners" con los botones de flecha de la parte inferior de la página.</span><span class="sxs-lookup"><span data-stu-id="02fc7-171">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="02fc7-172">La **instalación programada** debe aparecer junto a la solución de referencias del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="02fc7-172">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="02fc7-173">La instalación tardará 10-15 minutos.</span><span class="sxs-lookup"><span data-stu-id="02fc7-173">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="02fc7-174">Una vez completada la instalación, vuelva a [Power Automatic](https://flow.microsoft.com) y seleccione **soluciones** en el área de navegación izquierda.</span><span class="sxs-lookup"><span data-stu-id="02fc7-174">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="02fc7-175">Observe que la **sincronización de referencias del centro de partners para Salesforce** está disponible en la lista de soluciones.</span><span class="sxs-lookup"><span data-stu-id="02fc7-175">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="02fc7-176">Seleccione la **sincronización de referencias del centro de partners para Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-176">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="02fc7-177">Están disponibles los siguientes flujos y entidades:</span><span class="sxs-lookup"><span data-stu-id="02fc7-177">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/salesforce10.png" alt-text="Flujos de Salesforce":::



## <a name="configure-the-solution"></a><span data-ttu-id="02fc7-179">Configuración de la solución</span><span class="sxs-lookup"><span data-stu-id="02fc7-179">Configure the solution</span></span>

1. <span data-ttu-id="02fc7-180">Una vez que haya instalado la solución en la instancia de CRM, vuelva a [Power Automatic](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="02fc7-180">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="02fc7-181">En la lista desplegable de **entornos** de la esquina superior derecha, seleccione la instancia de CRM en la que instaló la solución Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="02fc7-181">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>
3. <span data-ttu-id="02fc7-182">Tendrá que crear conexiones que asocien las tres cuentas de usuario:</span><span class="sxs-lookup"><span data-stu-id="02fc7-182">You will need to create connections that associate the three user accounts:</span></span>
    - <span data-ttu-id="02fc7-183">Usuario del centro de Partners con credenciales de administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="02fc7-183">Partner Center user with referrals admin credentials</span></span>
    - <span data-ttu-id="02fc7-184">Eventos del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="02fc7-184">Partner Center Events</span></span>
    - <span data-ttu-id="02fc7-185">Administrador de CRM con la potencia que automatiza los flujos en la solución.</span><span class="sxs-lookup"><span data-stu-id="02fc7-185">CRM admin with the Power Automate flows in the solution.</span></span>
4. <span data-ttu-id="02fc7-186">Seleccione **conexiones** en la barra de navegación izquierda y seleccione la solución "referencias del centro de Partners" en la lista.</span><span class="sxs-lookup"><span data-stu-id="02fc7-186">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

5. <span data-ttu-id="02fc7-187">Cree una conexión haciendo clic en **crear una conexión**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-187">Create a connection by clicking **Create a connection**.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce12.png" alt-text="Crear conexión":::

- <span data-ttu-id="02fc7-189">Busque referencias del centro de Partners (versión preliminar) en la barra de búsqueda de la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="02fc7-189">Search for Partner Center Referrals (preview) in the search bar on the top right corner.</span></span>

- <span data-ttu-id="02fc7-190">Cree una conexión para el usuario del centro de Partners con el rol de credenciales de administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="02fc7-190">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

-  <span data-ttu-id="02fc7-191">A continuación, cree una conexión de eventos del centro de partners para el usuario del centro de Partners con las credenciales de administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="02fc7-191">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

- <span data-ttu-id="02fc7-192">Cree una conexión para Salesforce para el usuario administrador de CRM.</span><span class="sxs-lookup"><span data-stu-id="02fc7-192">Create a connection for Salesforce for the CRM administrator user.</span></span>

-  <span data-ttu-id="02fc7-193">Una vez que haya agregado todas las conexiones, debería ver las siguientes conexiones en su entorno:</span><span class="sxs-lookup"><span data-stu-id="02fc7-193">Once you have all the Connections added, you should see the following Connections in your environment:</span></span>

 :::image type="content" source="images/cosellconnectors/salesforce13.png" alt-text="Observar conexiones":::

### <a name="edit-the-connections"></a><span data-ttu-id="02fc7-195">Editar las conexiones</span><span class="sxs-lookup"><span data-stu-id="02fc7-195">Edit the connections</span></span>

1. <span data-ttu-id="02fc7-196">Vuelva a la página soluciones y seleccione **solución predeterminada**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-196">Return to the Solutions page and select **Default Solution**.</span></span>  <span data-ttu-id="02fc7-197">Haga clic en **todo** para seleccionar **referencia de conexión (vista previa)** .</span><span class="sxs-lookup"><span data-stu-id="02fc7-197">Select **Connection Reference (preview)** by clicking **All**.</span></span>
 
:::image type="content" source="images/cosellconnectors/salesforce14.png" alt-text="Inicio de la edición del conector":::

2. <span data-ttu-id="02fc7-199">Edite cada una de las conexiones de una en una; para ello, seleccione el icono de tres puntos.</span><span class="sxs-lookup"><span data-stu-id="02fc7-199">Edit each of the Connections one by one by selecting the three dots icon.</span></span> <span data-ttu-id="02fc7-200">Agregue las conexiones correspondientes.</span><span class="sxs-lookup"><span data-stu-id="02fc7-200">Add the relevant connections.</span></span>

:::image type="content" source="images/cosellconnectors/salesforce15.png" alt-text="Editar conectores":::

3. <span data-ttu-id="02fc7-202">Active los flujos en la secuencia siguiente:</span><span class="sxs-lookup"><span data-stu-id="02fc7-202">Turn on the flows in the following sequence:</span></span>

- <span data-ttu-id="02fc7-203">Registro del webhook del centro de Partners (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="02fc7-203">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="02fc7-204">Creación de una referencia de venta conjunta: Salesforce al centro de Partners (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="02fc7-204">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="02fc7-205">Centro de Partners: actualizaciones de referencia de venta conjunta de Microsoft en Salesforce (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="02fc7-205">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="02fc7-206">Centro de partners a Salesforce (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="02fc7-206">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="02fc7-207">Salesforce a Partner Center (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="02fc7-207">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="02fc7-208">Oportunidad de Salesforce para el centro de Partners (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="02fc7-208">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="02fc7-209">Soluciones de Salesforce de Microsoft para el centro de Partners (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="02fc7-209">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="02fc7-210">Uso de las API de webhook para registrar eventos de cambio de recursos</span><span class="sxs-lookup"><span data-stu-id="02fc7-210">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="02fc7-211">Las API del webhook del centro de Partners le permiten registrarse para los eventos de cambio de recursos.</span><span class="sxs-lookup"><span data-stu-id="02fc7-211">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="02fc7-212">Estos eventos de cambio se envían a la dirección URL como publicaciones HTTP.</span><span class="sxs-lookup"><span data-stu-id="02fc7-212">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="02fc7-213">Para registrar la dirección URL, seleccione **registro de webhook del centro de Partners (versión preliminar de Insider)** flujo de automatización.</span><span class="sxs-lookup"><span data-stu-id="02fc7-213">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="02fc7-214">Agregar conexiones para (a) el usuario del centro de Partners con credenciales de administrador de referencias (b.) eventos del centro de partners como se resaltan a continuación</span><span class="sxs-lookup"><span data-stu-id="02fc7-214">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Desencadenador":::

3. <span data-ttu-id="02fc7-216">Cuando realice estas actualizaciones, verá</span><span class="sxs-lookup"><span data-stu-id="02fc7-216">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="02fc7-218">Guarde los cambios y seleccione **Activar**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-218">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="02fc7-219">Para permitir que los webhooks del centro de Partners escuchen los cambios de eventos, realice los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="02fc7-219">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="02fc7-220">Seleccione **centro de partners para Salesforce CRM (versión preliminar de Insider)**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-220">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="02fc7-221">Seleccione el icono de **edición** y seleccione **cuando se reciba una solicitud HTTP**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-221">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="02fc7-222">Seleccione el icono de **copiar** para copiar la dirección URL http post proporcionada.</span><span class="sxs-lookup"><span data-stu-id="02fc7-222">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copiar la dirección URL":::

8. <span data-ttu-id="02fc7-224">Ahora, seleccione "registro de webhook del centro de Partners (versión preliminar de Insider)" flujo automático de energía y seleccione **Ejecutar**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-224">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="02fc7-225">Asegúrese de que se abre la ventana "flujo de ejecución" en el panel derecho y haga clic en **continuar**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-225">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="02fc7-226">Escriba la siguiente información:</span><span class="sxs-lookup"><span data-stu-id="02fc7-226">Enter the following details:</span></span>

    1. <span data-ttu-id="02fc7-227">**Punto de conexión de desencadenador http**: dirección URL copiada del paso anterior</span><span class="sxs-lookup"><span data-stu-id="02fc7-227">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="02fc7-228">**Eventos para registrar**: "referencia creada" y "referencia-actualizada"</span><span class="sxs-lookup"><span data-stu-id="02fc7-228">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="02fc7-229">**Sobrescribir puntos de conexión de desencadenador existentes si están presentes**: sí (esto Sobrescribe todos los extremos existentes).</span><span class="sxs-lookup"><span data-stu-id="02fc7-229">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="02fc7-230">Seleccione **Ejecutar** y, a continuación, haga clic en **listo.**</span><span class="sxs-lookup"><span data-stu-id="02fc7-230">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="02fc7-231">Ahora, el webhook puede escuchar la creación y actualización de eventos.</span><span class="sxs-lookup"><span data-stu-id="02fc7-231">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="02fc7-232">Personalizar pasos de sincronización</span><span class="sxs-lookup"><span data-stu-id="02fc7-232">Customize synchronization steps</span></span>

<span data-ttu-id="02fc7-233">Cuando se sincronizan las referencias de venta conjunta entre el centro de Partners y el sistema CRM, los campos que se sincronizan en el equipo del centro de Partners se enumeran aquí.</span><span class="sxs-lookup"><span data-stu-id="02fc7-233">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="02fc7-234">A menudo, los sistemas CRM son muy personalizados.</span><span class="sxs-lookup"><span data-stu-id="02fc7-234">Often CRM systems are highly customized.</span></span> <span data-ttu-id="02fc7-235">Puede personalizar los flujos de automatización.</span><span class="sxs-lookup"><span data-stu-id="02fc7-235">You can customize the Power Automate flows.</span></span> <span data-ttu-id="02fc7-236">Siga la guía de asignación de campos y, si es necesario, realice los cambios adecuados en los pasos de la potencia que automatiza los flujos.</span><span class="sxs-lookup"><span data-stu-id="02fc7-236">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="02fc7-237">Se proporcionan las asignaciones de Microsoft Partner Center a CRM, pero en función de su entorno de CRM, puede optar por personalizar aún más los campos.</span><span class="sxs-lookup"><span data-stu-id="02fc7-237">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="02fc7-238">Se pueden personalizar varios pasos de cada uno de los flujos de potencia automatizados en función de sus necesidades.</span><span class="sxs-lookup"><span data-stu-id="02fc7-238">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="02fc7-239">Estos son algunos ejemplos de las personalizaciones disponibles:</span><span class="sxs-lookup"><span data-stu-id="02fc7-239">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="02fc7-240">Para personalizar los campos de los eventos de creación o actualización en el centro de partners para la sincronización de referencias de CRM:</span><span class="sxs-lookup"><span data-stu-id="02fc7-240">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="02fc7-241">Seleccione centro de partners para Salesforce CRM (versión preliminar de Insider).</span><span class="sxs-lookup"><span data-stu-id="02fc7-241">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="02fc7-242">Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="02fc7-242">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="02fc7-243">Seleccione **(ámbito) sincronizar el cliente potencial o la oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-243">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="02fc7-244">Para personalizar las asignaciones de campos de CRM para crear eventos, seleccione **si es nueva oportunidad compartida y, a continuación**, haga clic en.</span><span class="sxs-lookup"><span data-stu-id="02fc7-244">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="02fc7-245">Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda **la sección creación de una nueva oportunidad en CRM**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-245">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="02fc7-246">Puede editar las asignaciones en esta sección mediante la guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="02fc7-246">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="02fc7-247">Para personalizar las asignaciones de campos de CRM para los eventos de actualización, haga clic en el paso "(ámbito) sincronizar el cliente potencial o la oportunidad".</span><span class="sxs-lookup"><span data-stu-id="02fc7-247">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="02fc7-248">Seleccione **si se trata de una actualización de una oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-248">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="02fc7-249">Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda **si la diferencia entre los objetos de oportunidad del centro de Partners y CRM**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-249">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="02fc7-250">Seleccione **si sí** seguido de **Actualizar oportunidad existente** .</span><span class="sxs-lookup"><span data-stu-id="02fc7-250">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="02fc7-251">Para personalizar los campos de la sincronización de referencia de CRM a equipo para eventos de actualización:</span><span class="sxs-lookup"><span data-stu-id="02fc7-251">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="02fc7-252">Seleccione **Editar**  para editar o personalizar el flujo de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="02fc7-252">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="02fc7-253">Seleccione **(ámbito) sincronizar la oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-253">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="02fc7-254">Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para eventos de actualización, seleccione **si hay diferencias entre los objetos de cliente potencial del centro de Partners y CRM y, a continuación, haga clic en**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-254">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="02fc7-255">Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda el paso **actualizar una referencia con los datos de oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-255">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="02fc7-256">Puede editar las asignaciones en esta sección basándose en la guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="02fc7-256">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="02fc7-257">Para personalizar los campos de la sincronización de referencia de CRM a equipo para crear eventos</span><span class="sxs-lookup"><span data-stu-id="02fc7-257">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="02fc7-258">Seleccione **Editar**  para editar o personalizar el flujo de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="02fc7-258">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="02fc7-259">Seleccione **(ámbito) sincronizar referencias.**</span><span class="sxs-lookup"><span data-stu-id="02fc7-259">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="02fc7-260">Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para crear eventos, seleccione **crear referencia de Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-260">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="02fc7-261">Puede editar las asignaciones en esta sección basándose en la guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="02fc7-261">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>


## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="02fc7-262">Sincronización de referencia de venta conjunta bidireccional de un extremo a otro</span><span class="sxs-lookup"><span data-stu-id="02fc7-262">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="02fc7-263">Una vez que haya instalado, configurado y personalizado la solución Power Automate, puede probar la sincronización de referencias de venta conjunta entre el centro de Partners y el CRM de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="02fc7-263">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="02fc7-264">Requisitos previos</span><span class="sxs-lookup"><span data-stu-id="02fc7-264">Pre-requisites</span></span>

<span data-ttu-id="02fc7-265">Para sincronizar las referencias entre el centro de Partners y el CRM de Salesforce, la solución Power Automate debe delimitar claramente los campos de referencia específicos de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="02fc7-265">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="02fc7-266">Esta identificación proporciona a los equipos de los vendedores la capacidad de decidir qué referencias desean compartir con Microsoft para la venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="02fc7-266">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="02fc7-267">Un conjunto de campos personalizados está disponible como parte de la sincronización de referencias del centro de partners para la entidad de **oportunidad** de la solución CRM de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="02fc7-267">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="02fc7-268">Un usuario administrador de CRM tendrá que crear una sección de CRM independiente con los campos personalizados de la **oportunidad** .</span><span class="sxs-lookup"><span data-stu-id="02fc7-268">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="02fc7-269">Los siguientes campos personalizados deben formar parte de la sección CRM:</span><span class="sxs-lookup"><span data-stu-id="02fc7-269">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="02fc7-270">**Sincronizar con el centro de Partners**: si se va a sincronizar la oportunidad con el centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="02fc7-270">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="02fc7-271">**Identificador de referencia**: un campo de identificador de solo lectura para la referencia del centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="02fc7-271">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="02fc7-272">**Vínculo de referencia**: un vínculo de solo lectura a la referencia en el centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="02fc7-272">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="02fc7-273">**Ayuda de Microsoft**: ayuda de Microsoft para la referencia</span><span class="sxs-lookup"><span data-stu-id="02fc7-273">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="02fc7-274">**Productos**: lista de productos asociados a esta oportunidad</span><span class="sxs-lookup"><span data-stu-id="02fc7-274">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="02fc7-275">**Audit**: una pista de auditoría de solo lectura para la sincronización con las referencias del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="02fc7-275">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="02fc7-276">SITUACIÓN</span><span class="sxs-lookup"><span data-stu-id="02fc7-276">SCENARIOS:</span></span>

1. <span data-ttu-id="02fc7-277">Sincronización de referencia cuando se crea o actualiza una referencia en CRM y se sincroniza en el centro de Partners:</span><span class="sxs-lookup"><span data-stu-id="02fc7-277">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="02fc7-278">Inicie sesión en el entorno de Salesforce CRM con un usuario que tenga visibilidad en la sección de **oportunidades** de CRM.</span><span class="sxs-lookup"><span data-stu-id="02fc7-278">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="02fc7-279">Asegúrese de que la siguiente sección está presente al crear una "nueva oportunidad" en el entorno de CRM de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="02fc7-279">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Entorno de Salesforce":::

   3. <span data-ttu-id="02fc7-281">Para sincronizar esta oportunidad con el centro de Partners de Microsoft, asegúrese de establecer los siguientes campos en la vista tarjeta:</span><span class="sxs-lookup"><span data-stu-id="02fc7-281">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="02fc7-282">"Sincronizar con el centro de Partners": sí</span><span class="sxs-lookup"><span data-stu-id="02fc7-282">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="02fc7-283">"¿Cómo puede ayuda de Microsoft?": Seleccione una de las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="02fc7-283">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="02fc7-284">Productos: identificadores de la solución del producto</span><span class="sxs-lookup"><span data-stu-id="02fc7-284">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="02fc7-285">Una vez que haya establecido la opción de sincronización de oportunidades  **con el centro de Partners** en **sí**, espere 10 minutos, inicie sesión en su cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="02fc7-285">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="02fc7-286">Las referencias se sincronizarán con el CRM de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="02fc7-286">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="02fc7-287">Cuando la opción "sincronizar con el centro de Partners" está establecida en "sí", si actualiza la oportunidad en el CRM de Salesforce, los cambios se sincronizarán con la cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="02fc7-287">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="02fc7-288">Las oportunidades que se sincronizan correctamente con el centro de Partners se identificarán con ✔ icono en la CRM de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="02fc7-288">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="02fc7-289">Sincronización de referencia cuando se crea o actualiza una referencia en el centro de Partners de Microsoft y se sincroniza en el entorno de Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="02fc7-289">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="02fc7-290">Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard/home)del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="02fc7-290">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="02fc7-291">Seleccione **referencias** en el menú de la izquierda.</span><span class="sxs-lookup"><span data-stu-id="02fc7-291">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="02fc7-292">Cree una nueva referencia de venta conjunta desde el centro de partners; para ello, haga clic en la opción "nuevo trato".</span><span class="sxs-lookup"><span data-stu-id="02fc7-292">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="02fc7-293">Inicie sesión en el entorno de Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="02fc7-293">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="02fc7-294">Vaya a **abrir oportunidades**.</span><span class="sxs-lookup"><span data-stu-id="02fc7-294">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="02fc7-295">La referencia creada en el centro de Partners de Microsoft ya está sincronizada en el CRM de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="02fc7-295">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Pantalla de oportunidad de Salesforce":::

    6. <span data-ttu-id="02fc7-297">Al seleccionar una referencia sincronizada, se rellenan los detalles de la vista de tarjeta.</span><span class="sxs-lookup"><span data-stu-id="02fc7-297">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="02fc7-298">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="02fc7-298">Next steps</span></span>

- [<span data-ttu-id="02fc7-299">Administrar los clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="02fc7-299">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="02fc7-300">Administrar las oportunidades de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="02fc7-300">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="02fc7-301">Webhooks del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="02fc7-301">Partner Center webhooks</span></span>](/partner-center/develop/partner-center-webhooks)
