---
title: El conector de venta conjunta para el centro de Partners de Salesforce CRM
ms.topic: how-to
ms.date: 05/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizar las referencias en el centro de Partners con el CRM de Salesforce
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 4f636da49504c69c1e0e44c176fb76a4d7f8a78e
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527838"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a><span data-ttu-id="1b8cc-103">Conector de venta conjunta para Salesforce CRM: información general</span><span class="sxs-lookup"><span data-stu-id="1b8cc-103">Co-sell connector for Salesforce CRM - overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="1b8cc-104">Roles adecuados</span><span class="sxs-lookup"><span data-stu-id="1b8cc-104">Appropriate roles</span></span>

- <span data-ttu-id="1b8cc-105">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="1b8cc-105">Referrals admin</span></span>
- <span data-ttu-id="1b8cc-106">Administrador del sistema o Personalizador del sistema en CRM</span><span class="sxs-lookup"><span data-stu-id="1b8cc-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="1b8cc-107">El conector de la venta conjunta del centro de Partners permite que los vendedores covendan con Microsoft desde los sistemas CRM.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="1b8cc-108">No tendrán que estar capacitados para utilizar el centro de partners para administrar las ofertas de venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="1b8cc-109">Mediante el uso de conectores de venta conjunta, puede crear una nueva referencia de venta conjunta para participar en un vendedor de Microsoft, recibir referencias del vendedor de Microsoft, aceptar o rechazar las referencias, modificar los datos del negocio, como el valor del negocio y la fecha de cierre.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-109">Using the Co-sell connectors, you can create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span>  <span data-ttu-id="1b8cc-110">También puede recibir cualquier actualización de los vendedores de Microsoft en estos acuerdos de venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="1b8cc-111">Puede hacer que todas las referencias funcionen mientras trabaja en el CRM de su elección, en lugar de hacerlo en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-111">You can do all of your referrals work while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="1b8cc-112">La solución se basa en la solución Microsoft Power Automate y usa las API del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="1b8cc-113">Antes de instalar: requisitos previos</span><span class="sxs-lookup"><span data-stu-id="1b8cc-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="1b8cc-114">**Temas**</span><span class="sxs-lookup"><span data-stu-id="1b8cc-114">**Topics**</span></span>   |<span data-ttu-id="1b8cc-115">**Detalles**</span><span class="sxs-lookup"><span data-stu-id="1b8cc-115">**Details**</span></span>   |<span data-ttu-id="1b8cc-116">**Vínculos**</span><span class="sxs-lookup"><span data-stu-id="1b8cc-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="1b8cc-117">IDENTIFICADOR de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="1b8cc-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="1b8cc-118">Necesita un ID. de MPN válido</span><span class="sxs-lookup"><span data-stu-id="1b8cc-118">You need a valid MPN ID</span></span>|<span data-ttu-id="1b8cc-119">Para unirse a [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="1b8cc-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="1b8cc-120">Venta conjunta lista</span><span class="sxs-lookup"><span data-stu-id="1b8cc-120">Co-sell ready</span></span>|<span data-ttu-id="1b8cc-121">La solución de IP/servicios debe estar lista para su venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="1b8cc-122">Venda con Microsoft</span><span class="sxs-lookup"><span data-stu-id="1b8cc-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="1b8cc-123">Cuenta de Centro de partners</span><span class="sxs-lookup"><span data-stu-id="1b8cc-123">Partner Center account</span></span>|<span data-ttu-id="1b8cc-124">El identificador de MPN asociado al inquilino del centro de Partners debe ser el mismo que el identificador de MPN asociado a la solución de venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="1b8cc-125">Compruebe que puede ver las referencias de venta conjunta en el portal del centro de Partners antes de implementar los conectores.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="1b8cc-126">Administración de la cuenta</span><span class="sxs-lookup"><span data-stu-id="1b8cc-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="1b8cc-127">Roles de usuario del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="1b8cc-127">Partner Center user roles</span></span>|<span data-ttu-id="1b8cc-128">El empleado que va a instalar y usar los conectores debe ser un administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="1b8cc-129">Asignar roles y permisos de usuarios</span><span class="sxs-lookup"><span data-stu-id="1b8cc-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="1b8cc-130">CRM de Salesforce</span><span class="sxs-lookup"><span data-stu-id="1b8cc-130">Salesforce CRM</span></span>|<span data-ttu-id="1b8cc-131">El rol de usuario CRM es administrador del sistema o Personalizador del sistema</span><span class="sxs-lookup"><span data-stu-id="1b8cc-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="1b8cc-132">Asignación de roles en el CRM de Salesforce</span><span class="sxs-lookup"><span data-stu-id="1b8cc-132">Assign roles in Salesforce CRM</span></span>](https://docs.microsoft.com/SalesforceCRM/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="1b8cc-133">Cuenta de flujo de automatización de energía</span><span class="sxs-lookup"><span data-stu-id="1b8cc-133">Power Automate Flow Account</span></span>|<span data-ttu-id="1b8cc-134">Una cuenta activa de [Power Automatic](https://flow.microsoft.com) para el administrador del sistema CRM o el personalizador del sistema.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="1b8cc-135">Dicho usuario debe iniciar sesión en [Power automatizate](https://flow.microsoft.com) al menos una vez antes de la instalación.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a><span data-ttu-id="1b8cc-136">Instalación de la sincronización de referencias del centro de partners para Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="1b8cc-136">Install Partner Center Referrals Synchronization for Salesforce CRM</span></span>

1. <span data-ttu-id="1b8cc-137">Vaya a [Power Automatic](https://flow.microsoft.com) y seleccione **entornos** en la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="1b8cc-138">Se mostrarán las instancias de CRM disponibles.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-138">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="1b8cc-139">Seleccione la instancia de CRM correspondiente en la lista desplegable de la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="1b8cc-140">Seleccione **soluciones** en la barra de navegación izquierda.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="1b8cc-141">Haga clic en el vínculo **abrir AppSource** en el menú superior.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-141">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abrir AppSource":::

5. <span data-ttu-id="1b8cc-143">Busque **conectores de referencias del centro de partners para Salesforce** en la pantalla emergente.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-143">Search for **Partner Center Referrals Connectors for Salesforce** in the pop-up screen.</span></span>  

   :::image type="content" source="images/salesforce/salesforce1.png" alt-text="Salesforce":::

6. <span data-ttu-id="1b8cc-145">Haga clic en el botón **obtener ahora** y **continúe**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-145">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="1b8cc-146">Se abrirá la página en la que puede seleccionar el entorno de Salesforce CRM para instalar la aplicación.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-146">This opens the page where you can select the Salesforce CRM  environment to install application.</span></span>  <span data-ttu-id="1b8cc-147">Acepte los términos y condiciones.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-147">Agree to terms and conditions.</span></span>

   :::image type="content" source="images/salesforce/available-crm.png" alt-text="CRMS disponibles":::

8. <span data-ttu-id="1b8cc-149">A continuación, se le dirigirá a la página **administrar soluciones** .</span><span class="sxs-lookup"><span data-stu-id="1b8cc-149">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="1b8cc-150">Vaya a "referencias del centro de Partners" con los botones de flecha de la parte inferior de la página.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-150">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="1b8cc-151">La **instalación programada** debe aparecer junto a la solución de referencias del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-151">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="1b8cc-152">La instalación tardará 10-15 minutos.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-152">Installation will take 10-15 minutes.</span></span>

9. <span data-ttu-id="1b8cc-153">Una vez completada la instalación, vuelva a [Power Automatic](https://flow.microsoft.com) y seleccione **soluciones** en el área de navegación izquierda.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-153">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="1b8cc-154">Observe que la **sincronización de referencias del centro de partners para Salesforce** está disponible en la lista de soluciones.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-154">Notice that **Partner Center Referrals Synchronization for Salesforce** is available in the Solutions list.</span></span>

10. <span data-ttu-id="1b8cc-155">Seleccione la **sincronización de referencias del centro de partners para Salesforce**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-155">Select **Partner Center Referrals Synchronization for Salesforce**.</span></span> <span data-ttu-id="1b8cc-156">Están disponibles los siguientes flujos y entidades:</span><span class="sxs-lookup"><span data-stu-id="1b8cc-156">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/salesforce/salesforce-flows.png" alt-text="Flujos de Salesforce":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="1b8cc-158">Procedimiento recomendado: prueba antes de la marcha</span><span class="sxs-lookup"><span data-stu-id="1b8cc-158">Best Practice: Test before you go live</span></span>

<span data-ttu-id="1b8cc-159">Antes de instalar, configurar y personalizar la solución Power Automate en el entorno de producción, asegúrese de probar la solución en una instancia de CRM provisional.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-159">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="1b8cc-160">Instale la solución Microsoft Power Automate en un entorno de ensayo o una instancia de CRM.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-160">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>

- <span data-ttu-id="1b8cc-161">Realice una copia de la solución y ejecute la configuración y la automatización de las personalizaciones de flujo en el entorno de ensayo.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-161">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>

- <span data-ttu-id="1b8cc-162">Pruebe la solución en una instancia de ensayo o CRM.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-162">Test the solution on a staging/CRM instance.</span></span>

- <span data-ttu-id="1b8cc-163">En caso de éxito, importe como solución administrada a la instancia de producción.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-163">On success, import as managed solution to the production instance.</span></span>

## <a name="configure-the-solution"></a><span data-ttu-id="1b8cc-164">Configuración de la solución</span><span class="sxs-lookup"><span data-stu-id="1b8cc-164">Configure the solution</span></span>

1. <span data-ttu-id="1b8cc-165">Una vez que haya instalado la solución en la instancia de CRM, vuelva a [Power Automatic](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="1b8cc-165">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="1b8cc-166">En la lista desplegable de **entornos** de la esquina superior derecha, seleccione la instancia de CRM en la que instaló la solución Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-166">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="1b8cc-167">Tendrá que crear conexiones que asocien las tres cuentas de usuario:</span><span class="sxs-lookup"><span data-stu-id="1b8cc-167">You will need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="1b8cc-168">Usuario del centro de Partners con credenciales de administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="1b8cc-168">Partner Center user with referrals admin credentials</span></span>
   - <span data-ttu-id="1b8cc-169">Eventos del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="1b8cc-169">Partner Center Events</span></span>
   - <span data-ttu-id="1b8cc-170">Administrador de CRM con la potencia que automatiza los flujos en la solución.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-170">CRM admin with the Power Automate flows in the solution.</span></span>

   1. <span data-ttu-id="1b8cc-171">Seleccione **conexiones** en la barra de navegación izquierda y seleccione la solución "referencias del centro de Partners" en la lista.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-171">Select **Connections** from the left navigation bar and select the "Partner Center Referrals" solution from the list.</span></span>

   2. <span data-ttu-id="1b8cc-172">Cree una conexión haciendo clic en **crear una conexión**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-172">Create a connection by clicking **Create a connection**.</span></span>

       :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Crear conexión":::

   3. <span data-ttu-id="1b8cc-174">Busque **referencias del centro de Partners (versión preliminar)** en la barra de búsqueda de la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>

   4. <span data-ttu-id="1b8cc-175">Cree una conexión para el usuario del centro de Partners con el rol de credenciales de administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-175">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

   5. <span data-ttu-id="1b8cc-176">A continuación, cree una conexión de eventos del centro de partners para el usuario del centro de Partners con las credenciales de administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-176">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

   6. <span data-ttu-id="1b8cc-177">Cree una conexión para Common Data Service (entorno actual) para el usuario administrador de CRM.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-177">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="1b8cc-178">Para asociar los flujos de alimentación automatizada con las conexiones, edite cada uno de los flujos de Power Automatic para conectarse a Common Data Service y a las referencias del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-178">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="1b8cc-179">Guarde los cambios.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-179">Save the changes.</span></span>

5. <span data-ttu-id="1b8cc-180">**Encienda** los flujos automatizar energía.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-180">**Turn on** the the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="1b8cc-181">Uso de las API de webhook para registrar eventos de cambio de recursos</span><span class="sxs-lookup"><span data-stu-id="1b8cc-181">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="1b8cc-182">Las API del webhook del centro de Partners le permiten registrarse para los eventos de cambio de recursos.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-182">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="1b8cc-183">Estos eventos de cambio se envían a la dirección URL como publicaciones HTTP.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-183">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="1b8cc-184">Para registrar la dirección URL, seleccione **registro de webhook del centro de Partners (versión preliminar de Insider)** flujo de automatización.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-184">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="1b8cc-185">Agregar conexiones para () Usuario del centro de Partners con credenciales de administrador de referencias (b.) Eventos del centro de Partners, tal y como se resalta</span><span class="sxs-lookup"><span data-stu-id="1b8cc-185">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Desencadenador":::

3. <span data-ttu-id="1b8cc-187">Cuando realice estas actualizaciones, verá</span><span class="sxs-lookup"><span data-stu-id="1b8cc-187">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="1b8cc-189">Guarde los cambios y seleccione **Activar**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-189">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="1b8cc-190">Para permitir que los webhooks del centro de Partners escuchen los cambios de eventos, realice los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="1b8cc-190">To enable Partner Center webhooks to listen to event changes, perform the following steps:</span></span>

5. <span data-ttu-id="1b8cc-191">Seleccione **centro de partners para Salesforce CRM (versión preliminar de Insider)**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-191">Select **Partner Center to Salesforce CRM (Insider Preview)**.</span></span>

6. <span data-ttu-id="1b8cc-192">Seleccione el icono de **edición** y seleccione **cuando se reciba una solicitud HTTP**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-192">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="1b8cc-193">Seleccione el icono de **copiar** para copiar la dirección URL http post proporcionada.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-193">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/salesforce/copy-url.png" alt-text="Copiar la dirección URL":::

8. <span data-ttu-id="1b8cc-195">Ahora, seleccione "registro de webhook del centro de Partners (versión preliminar de Insider)" flujo automático de energía y seleccione **Ejecutar**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-195">Now select the "Partner Center Webhook Registration (Insider Preview)" Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="1b8cc-196">Asegúrese de que se abre la ventana "flujo de ejecución" en el panel derecho y haga clic en **continuar**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-196">Ensure that the "Run Flow" window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="1b8cc-197">Escriba la siguiente información:</span><span class="sxs-lookup"><span data-stu-id="1b8cc-197">Enter the following details:</span></span>

    1. <span data-ttu-id="1b8cc-198">**Punto de conexión de desencadenador http**: dirección URL copiada del paso anterior</span><span class="sxs-lookup"><span data-stu-id="1b8cc-198">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="1b8cc-199">**Eventos para registrar**: "referencia creada" y "referencia-actualizada"</span><span class="sxs-lookup"><span data-stu-id="1b8cc-199">**Events to Register**: "referral-created" and "referral-updated"</span></span>

    3. <span data-ttu-id="1b8cc-200">**Sobrescribir puntos de conexión de desencadenador existentes si están presentes**: sí (esto Sobrescribe todos los extremos existentes).</span><span class="sxs-lookup"><span data-stu-id="1b8cc-200">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="1b8cc-201">Seleccione **Ejecutar** y, a continuación, haga clic en **listo.**</span><span class="sxs-lookup"><span data-stu-id="1b8cc-201">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="1b8cc-202">Ahora, el webhook puede escuchar la creación y actualización de eventos.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-202">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="1b8cc-203">Personalizar pasos de sincronización</span><span class="sxs-lookup"><span data-stu-id="1b8cc-203">Customize synchronization steps</span></span>

<span data-ttu-id="1b8cc-204">Cuando se sincronizan las referencias de venta conjunta entre el centro de Partners y el sistema CRM, los campos que se sincronizan en el equipo del centro de Partners se enumeran aquí.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-204">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="1b8cc-205">A menudo, los sistemas CRM son muy personalizados.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-205">Often CRM systems are highly customized.</span></span> <span data-ttu-id="1b8cc-206">Puede personalizar los flujos de automatización.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-206">You can customize the Power Automate flows.</span></span> <span data-ttu-id="1b8cc-207">Siga la guía de asignación de campos y, si es necesario, realice los cambios adecuados en los pasos de la potencia que automatiza los flujos.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-207">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="1b8cc-208">Se proporcionan las asignaciones de Microsoft Partner Center a CRM, pero en función de su entorno de CRM, puede optar por personalizar aún más los campos.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-208">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="1b8cc-209">Se pueden personalizar varios pasos de cada uno de los flujos de potencia automatizados en función de sus necesidades.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-209">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="1b8cc-210">Estos son algunos ejemplos de las personalizaciones disponibles:</span><span class="sxs-lookup"><span data-stu-id="1b8cc-210">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="1b8cc-211">Para personalizar los campos de los eventos de creación o actualización en el centro de partners para la sincronización de referencias de CRM:</span><span class="sxs-lookup"><span data-stu-id="1b8cc-211">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span>

   1. <span data-ttu-id="1b8cc-212">Seleccione centro de partners para Salesforce CRM (versión preliminar de Insider).</span><span class="sxs-lookup"><span data-stu-id="1b8cc-212">Select Partner Center to Salesforce CRM (Insider Preview).</span></span>

   2. <span data-ttu-id="1b8cc-213">Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-213">Select **Edit** to edit/customize the Power Automate flow.</span></span>

   3. <span data-ttu-id="1b8cc-214">Seleccione **(ámbito) sincronizar el cliente potencial o la oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-214">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="1b8cc-215">Para personalizar las asignaciones de campos de CRM para crear eventos, seleccione **si es nueva oportunidad compartida y, a continuación**, haga clic en.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-215">To customize CRM field mappings for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="1b8cc-216">Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda **la sección creación de una nueva oportunidad en CRM**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-216">Select the sub-step **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="1b8cc-217">Puede editar las asignaciones en esta sección mediante la guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-217">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

   1. <span data-ttu-id="1b8cc-218">Para personalizar las asignaciones de campos de CRM para los eventos de actualización, haga clic en el paso "(ámbito) sincronizar el cliente potencial o la oportunidad".</span><span class="sxs-lookup"><span data-stu-id="1b8cc-218">To customize CRM field mappings for update events, click on the step "(Scope) Synchronize the lead or opportunity".</span></span>

   2. <span data-ttu-id="1b8cc-219">Seleccione **si se trata de una actualización de una oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-219">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="1b8cc-220">Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda **si la diferencia entre los objetos de oportunidad del centro de Partners y CRM**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-220">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

   3. <span data-ttu-id="1b8cc-221">Seleccione **si sí** seguido de **Actualizar oportunidad existente** .</span><span class="sxs-lookup"><span data-stu-id="1b8cc-221">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="1b8cc-222">Para personalizar los campos de la sincronización de referencia de CRM a equipo para eventos de actualización:</span><span class="sxs-lookup"><span data-stu-id="1b8cc-222">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

   1. <span data-ttu-id="1b8cc-223">Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-223">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="1b8cc-224">Seleccione **(ámbito) sincronizar la oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-224">Select **(Scope) Synchronize the opportunity**.</span></span>

   3. <span data-ttu-id="1b8cc-225">Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para eventos de actualización, seleccione **si hay diferencias entre los objetos de cliente potencial del centro de Partners y CRM y, a continuación, haga clic en**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-225">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span>

   4. <span data-ttu-id="1b8cc-226">Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda el paso **actualizar una referencia con los datos de oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-226">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="1b8cc-227">Puede editar las asignaciones en esta sección basándose en la guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-227">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="1b8cc-228">Para personalizar los campos de la sincronización de referencia de CRM a equipo para crear eventos</span><span class="sxs-lookup"><span data-stu-id="1b8cc-228">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   1. <span data-ttu-id="1b8cc-229">Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-229">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   2. <span data-ttu-id="1b8cc-230">Seleccione **(ámbito) sincronizar referencias.**</span><span class="sxs-lookup"><span data-stu-id="1b8cc-230">Select **(Scope) Synchronizing Referrals.**</span></span>

   3. <span data-ttu-id="1b8cc-231">Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para crear eventos, seleccione **crear referencia de Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-231">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

<span data-ttu-id="1b8cc-232">Puede editar las asignaciones en esta sección basándose en la guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-232">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="create-separate-section-in-salesforce-crm-opportunity-layout"></a><span data-ttu-id="1b8cc-233">Crear una sección independiente en el diseño de oportunidades de Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="1b8cc-233">Create Separate Section in Salesforce CRM Opportunity Layout</span></span>

<span data-ttu-id="1b8cc-234">Para sincronizar las referencias entre el centro de Partners y el CRM de Salesforce, la solución Power Automate debe delimitar claramente los campos de referencia específicos de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-234">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="1b8cc-235">Esto proporciona a los equipos de los vendedores la capacidad de decidir qué referencias desean compartir con Microsoft para la venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-235">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="1b8cc-236">Un conjunto de campos personalizados está disponible como parte de la sincronización de referencias del centro de partners para la entidad de **oportunidad** de CRM de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-236">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM **Opportunity** entity.</span></span> <span data-ttu-id="1b8cc-237">Un usuario administrador de CRM tendrá que crear una sección de CRM independiente con los campos personalizados de la **oportunidad** .</span><span class="sxs-lookup"><span data-stu-id="1b8cc-237">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>
<span data-ttu-id="1b8cc-238">El usuario administrador de Salesforce CRM deberá crear una sección de CRM independiente.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-238">Salesforce CRM administrator user will need to create a separate CRM section.</span></span>

<span data-ttu-id="1b8cc-239">Los siguientes campos personalizados deben formar parte de la sección CRM:</span><span class="sxs-lookup"><span data-stu-id="1b8cc-239">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="1b8cc-240">**Sincronizar con el centro de Partners**: si se va a sincronizar la oportunidad con el centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="1b8cc-240">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="1b8cc-241">**Identificador de referencia**: un campo de identificador de solo lectura para la referencia del centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="1b8cc-241">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="1b8cc-242">**Vínculo de referencia**: un vínculo de solo lectura a la referencia en el centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="1b8cc-242">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="1b8cc-243">**¿Cómo puede ayudarle Microsoft?**</span><span class="sxs-lookup"><span data-stu-id="1b8cc-243">**How can Microsoft help?**</span></span> <span data-ttu-id="1b8cc-244">Ayuda necesaria de Microsoft para la referencia</span><span class="sxs-lookup"><span data-stu-id="1b8cc-244">Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="1b8cc-245">**Productos**: lista de productos asociados a esta oportunidad</span><span class="sxs-lookup"><span data-stu-id="1b8cc-245">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="1b8cc-246">**Audit**: una pista de auditoría de solo lectura para la sincronización con la referencia del centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="1b8cc-246">**Audit**: A read only audit trail for syncing with Microsoft Partner Center referral</span></span>

### <a name="set-up-fields-and-relationships"></a><span data-ttu-id="1b8cc-247">Configurar campos y relaciones</span><span class="sxs-lookup"><span data-stu-id="1b8cc-247">Set up fields and relationships</span></span>

1. <span data-ttu-id="1b8cc-248">Inicie sesión en su cuenta de Salesforce y vaya a la **oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-248">Sign into your Salesforce account and go to **Opportunity**.</span></span>

2. <span data-ttu-id="1b8cc-249">Haga clic en las opciones de **configuración** y **Editar objeto** para agregar los campos necesarios.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-249">Click on the **Setup** and **Edit Object** options to add the necessary fields.</span></span>

3. <span data-ttu-id="1b8cc-250">Seleccionar **campos & relaciones** en el panel de navegación izquierdo</span><span class="sxs-lookup"><span data-stu-id="1b8cc-250">Select **Fields & Relationships** from the left navigation</span></span>

   :::image type="content" source="images/salesforce/fields1.png" alt-text="Campos":::

4. <span data-ttu-id="1b8cc-252">Agregue los campos siguientes en los **campos &** tabla de relaciones:</span><span class="sxs-lookup"><span data-stu-id="1b8cc-252">Add the following fields in the **Fields & Relationship** table:</span></span>

   |<span data-ttu-id="1b8cc-253">**Etiqueta de campo**</span><span class="sxs-lookup"><span data-stu-id="1b8cc-253">**Field label**</span></span>   |<span data-ttu-id="1b8cc-254">**Nombre del campo**</span><span class="sxs-lookup"><span data-stu-id="1b8cc-254">**Field name**</span></span>|<span data-ttu-id="1b8cc-255">**Tipo de datos**</span><span class="sxs-lookup"><span data-stu-id="1b8cc-255">**Data type**</span></span>|<span data-ttu-id="1b8cc-256">**Indizó**</span><span class="sxs-lookup"><span data-stu-id="1b8cc-256">**Indexed**</span></span>|
   |---------------------|:-------------------|:--------------|:----------------|
   |<span data-ttu-id="1b8cc-257">Auditoría</span><span class="sxs-lookup"><span data-stu-id="1b8cc-257">Audit</span></span>| <span data-ttu-id="1b8cc-258">Audit__c</span><span class="sxs-lookup"><span data-stu-id="1b8cc-258">Audit__c</span></span>|<span data-ttu-id="1b8cc-259">Área de texto largo (100.000) (línea visible 4)</span><span class="sxs-lookup"><span data-stu-id="1b8cc-259">Long Text Area(100000)(visible line 4)</span></span>||
   |<span data-ttu-id="1b8cc-260">¿Cómo puede ayudarle Microsoft?</span><span class="sxs-lookup"><span data-stu-id="1b8cc-260">How can Microsoft help?</span></span>|<span data-ttu-id="1b8cc-261">How_can_Microsoft_help_c</span><span class="sxs-lookup"><span data-stu-id="1b8cc-261">How_can_Microsoft_help_c</span></span>|<span data-ttu-id="1b8cc-262">Lista desplegable</span><span class="sxs-lookup"><span data-stu-id="1b8cc-262">Picklist\*</span></span>|
   |<span data-ttu-id="1b8cc-263">Productos</span><span class="sxs-lookup"><span data-stu-id="1b8cc-263">Products</span></span>|<span data-ttu-id="1b8cc-264">Products_c</span><span class="sxs-lookup"><span data-stu-id="1b8cc-264">Products_c</span></span>|<span data-ttu-id="1b8cc-265">texto (255)</span><span class="sxs-lookup"><span data-stu-id="1b8cc-265">text (255)</span></span>||
   |<span data-ttu-id="1b8cc-266">Referral</span><span class="sxs-lookup"><span data-stu-id="1b8cc-266">Referral</span></span> | <span data-ttu-id="1b8cc-267">Referral_Identfier_c</span><span class="sxs-lookup"><span data-stu-id="1b8cc-267">Referral_Identfier_c</span></span>|<span data-ttu-id="1b8cc-268">Texto (100) (ID. externo)</span><span class="sxs-lookup"><span data-stu-id="1b8cc-268">Text(100)(External ID)</span></span>|<span data-ttu-id="1b8cc-269">sí</span><span class="sxs-lookup"><span data-stu-id="1b8cc-269">yes</span></span>|
   |<span data-ttu-id="1b8cc-270">Vínculo de referencia</span><span class="sxs-lookup"><span data-stu-id="1b8cc-270">Referral Link</span></span>| <span data-ttu-id="1b8cc-271">Referral_Link_c_</span><span class="sxs-lookup"><span data-stu-id="1b8cc-271">Referral_Link_c_</span></span>|<span data-ttu-id="1b8cc-272">URL (255)</span><span class="sxs-lookup"><span data-stu-id="1b8cc-272">URL(255)</span></span>||
   |<span data-ttu-id="1b8cc-273">Sincronizar con el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="1b8cc-273">Sync with Partner Center</span></span>|<span data-ttu-id="1b8cc-274">sync_with_partner_center_c</span><span class="sxs-lookup"><span data-stu-id="1b8cc-274">sync_with_partner_center_c</span></span>|<span data-ttu-id="1b8cc-275">CheckBox (valor predeterminado desactivado)</span><span class="sxs-lookup"><span data-stu-id="1b8cc-275">Checkbox (default unchecked)</span></span>||

   <span data-ttu-id="1b8cc-276">\* Valores de lista desplegable:</span><span class="sxs-lookup"><span data-stu-id="1b8cc-276">\*Picklist values:</span></span>

   - <span data-ttu-id="1b8cc-277">Propuesta de valor específico de carga de trabajo</span><span class="sxs-lookup"><span data-stu-id="1b8cc-277">Workload specific value proposition</span></span>
   - <span data-ttu-id="1b8cc-278">Arquitectura técnica del cliente</span><span class="sxs-lookup"><span data-stu-id="1b8cc-278">Customer technical architecture</span></span>
   - <span data-ttu-id="1b8cc-279">Prueba de concepto o demostración</span><span class="sxs-lookup"><span data-stu-id="1b8cc-279">Proof of concept or demo</span></span>
   - <span data-ttu-id="1b8cc-280">Comillas o licencias</span><span class="sxs-lookup"><span data-stu-id="1b8cc-280">Quotes or licensing</span></span>
   - <span data-ttu-id="1b8cc-281">Éxito del cliente de ventas</span><span class="sxs-lookup"><span data-stu-id="1b8cc-281">Post sales customer success</span></span>
   - <span data-ttu-id="1b8cc-282">General u otro</span><span class="sxs-lookup"><span data-stu-id="1b8cc-282">General or other</span></span>

5. <span data-ttu-id="1b8cc-283">Los campos se crearían en **campos & relaciones**</span><span class="sxs-lookup"><span data-stu-id="1b8cc-283">The fields would get created under **Fields & Relationships**</span></span>

   :::image type="content" source="images/salesforce/fields2.png" alt-text="Campos creados":::

6. <span data-ttu-id="1b8cc-285">En el diseño de la oportunidad, cree una sección independiente con los campos indicados anteriormente.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-285">In the Opportunity layout, create a separate section with the fields as listed above.</span></span>

   - <span data-ttu-id="1b8cc-286">Esta sección debe estar disponible para los vendedores en el diseño de la oportunidad.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-286">This section should be available for the sellers in the Opportunity layout</span></span>

   :::image type="content" source="images/salesforce/pc-fields-layout.png" alt-text="Diseño de campos del centro de Partners":::

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="1b8cc-288">Sincronización de referencia de venta conjunta bidireccional de un extremo a otro</span><span class="sxs-lookup"><span data-stu-id="1b8cc-288">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="1b8cc-289">Una vez que haya instalado, configurado y personalizado la solución Power Automate, puede probar la sincronización de referencias de venta conjunta entre el centro de Partners y el CRM de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-289">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Salesforce CRM and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="1b8cc-290">Requisitos previos</span><span class="sxs-lookup"><span data-stu-id="1b8cc-290">Pre-requisites</span></span>

<span data-ttu-id="1b8cc-291">Para sincronizar las referencias entre el centro de Partners y el CRM de Salesforce, la solución Power Automate debe delimitar claramente los campos de referencia específicos de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-291">To synchronize the referrals across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="1b8cc-292">Esta identificación proporciona a los equipos de los vendedores la capacidad de decidir qué referencias desean compartir con Microsoft para la venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-292">This identification provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="1b8cc-293">Un conjunto de campos personalizados está disponible como parte de la sincronización de referencias del centro de partners para la entidad de **oportunidad** de la solución CRM de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-293">A set of custom fields is available as part of Partner Center Referrals Synchronization for Salesforce CRM solution **Opportunity** entity.</span></span> <span data-ttu-id="1b8cc-294">Un usuario administrador de CRM tendrá que crear una sección de CRM independiente con los campos personalizados de la **oportunidad** .</span><span class="sxs-lookup"><span data-stu-id="1b8cc-294">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="1b8cc-295">Los siguientes campos personalizados deben formar parte de la sección CRM:</span><span class="sxs-lookup"><span data-stu-id="1b8cc-295">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="1b8cc-296">**Sincronizar con el centro de Partners**: si se va a sincronizar la oportunidad con el centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="1b8cc-296">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="1b8cc-297">**Identificador de referencia**: un campo de identificador de solo lectura para la referencia del centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="1b8cc-297">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="1b8cc-298">**Vínculo de referencia**: un vínculo de solo lectura a la referencia en el centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="1b8cc-298">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="1b8cc-299">**Ayuda de Microsoft**: ayuda de Microsoft para la referencia</span><span class="sxs-lookup"><span data-stu-id="1b8cc-299">**How can Microsoft help**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="1b8cc-300">**Productos**: lista de productos asociados a esta oportunidad</span><span class="sxs-lookup"><span data-stu-id="1b8cc-300">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="1b8cc-301">**Audit**: una pista de auditoría de solo lectura para la sincronización con las referencias del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="1b8cc-301">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="1b8cc-302">SITUACIÓN</span><span class="sxs-lookup"><span data-stu-id="1b8cc-302">SCENARIOS:</span></span>

1. <span data-ttu-id="1b8cc-303">Sincronización de referencia cuando se crea o actualiza una referencia en CRM y se sincroniza en el centro de Partners:</span><span class="sxs-lookup"><span data-stu-id="1b8cc-303">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="1b8cc-304">Inicie sesión en el entorno de Salesforce CRM con un usuario que tenga visibilidad en la sección de **oportunidades** de CRM.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-304">Sign into your Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="1b8cc-305">Asegúrese de que la siguiente sección está presente al crear una "nueva oportunidad" en el entorno de CRM de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-305">Ensure that the following section is present when you create a "New Opportunity" in Salesforce CRM environment</span></span>

      :::image type="content" source="images/salesforce/salesforce-scenario-1.png" alt-text="Entorno de Salesforce":::

   3. <span data-ttu-id="1b8cc-307">Para sincronizar esta oportunidad con el centro de Partners de Microsoft, asegúrese de establecer los siguientes campos en la vista tarjeta:</span><span class="sxs-lookup"><span data-stu-id="1b8cc-307">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

       - <span data-ttu-id="1b8cc-308">"Sincronizar con el centro de Partners": sí</span><span class="sxs-lookup"><span data-stu-id="1b8cc-308">"Sync with Partner Center": Yes</span></span>
       - <span data-ttu-id="1b8cc-309">"¿Cómo puede ayuda de Microsoft?": Seleccione una de las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="1b8cc-309">"How can Microsoft help?": Select from the following options:</span></span>
       - <span data-ttu-id="1b8cc-310">Productos: identificadores de la solución del producto</span><span class="sxs-lookup"><span data-stu-id="1b8cc-310">Products: Solution IDs of the product</span></span>

   4. <span data-ttu-id="1b8cc-311">Una vez que haya establecido la opción de sincronización de oportunidades **con el centro de Partners** en **sí**, espere 10 minutos, inicie sesión en su cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-311">Once you have set the opportunity  **Sync with Partner Center** option to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="1b8cc-312">Las referencias se sincronizarán con el CRM de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-312">Your referrals will be synchronized with Salesforce CRM.</span></span>

   5. <span data-ttu-id="1b8cc-313">Cuando la opción "sincronizar con el centro de Partners" está establecida en "sí", si actualiza la oportunidad en el CRM de Salesforce, los cambios se sincronizarán con la cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-313">When the "Sync with Partner Center" option is set to "Yes", if you update the opportunity in Salesforce CRM, the changes will synchronize with your Partner Center account.</span></span>

   6. <span data-ttu-id="1b8cc-314">Las oportunidades que se sincronizan correctamente con el centro de Partners se identificarán con ✔ icono en la CRM de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-314">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Salesforce CRM.</span></span>

2. <span data-ttu-id="1b8cc-315">Sincronización de referencia cuando se crea o actualiza una referencia en el centro de Partners de Microsoft y se sincroniza en el entorno de Salesforce CRM:</span><span class="sxs-lookup"><span data-stu-id="1b8cc-315">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Salesforce CRM environment:</span></span>

    1. <span data-ttu-id="1b8cc-316">Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard/home)del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-316">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    2. <span data-ttu-id="1b8cc-317">Seleccione **referencias** en el menú de la izquierda.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-317">Select **Referrals** from the left-hand menu.</span></span>

    3. <span data-ttu-id="1b8cc-318">Cree una nueva referencia de venta conjunta desde el centro de partners; para ello, haga clic en la opción "nuevo trato".</span><span class="sxs-lookup"><span data-stu-id="1b8cc-318">Create a new Co-sell referral from Partner Center by clicking "New deal" option.</span></span>

    4. <span data-ttu-id="1b8cc-319">Inicie sesión en el entorno de Salesforce CRM.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-319">Sign into your Salesforce CRM environment.</span></span>

    5. <span data-ttu-id="1b8cc-320">Vaya a **abrir oportunidades**.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-320">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="1b8cc-321">La referencia creada en el centro de Partners de Microsoft ya está sincronizada en el CRM de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-321">The referral created in Microsoft Partner Center is now synchronized in Salesforce CRM.</span></span>

       :::image type="content" source="images/salesforce/salesforce-casino-e.png" alt-text="Pantalla de oportunidad de Salesforce":::

    6. <span data-ttu-id="1b8cc-323">Al seleccionar una referencia sincronizada, se rellenan los detalles de la vista de tarjeta.</span><span class="sxs-lookup"><span data-stu-id="1b8cc-323">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1b8cc-324">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="1b8cc-324">Next steps</span></span>

- [<span data-ttu-id="1b8cc-325">¿Más información sobre la plataforma Microsoft Power Automate?</span><span class="sxs-lookup"><span data-stu-id="1b8cc-325">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/-automate/)

- [<span data-ttu-id="1b8cc-326">Administrar los clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="1b8cc-326">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="1b8cc-327">Administrar las oportunidades de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="1b8cc-327">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="1b8cc-328">Webhooks del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="1b8cc-328">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)