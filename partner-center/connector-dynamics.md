---
title: El conector de venta conjunta para el centro de Partners de Dynamics 365 CRM
ms.topic: article
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizar las referencias en el centro de Partners con el CRM de Dynamics 365
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 3b5170edaaadca3c4045e7ebed174b5d52b06bdd
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991653"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="5afdc-103">Conector de venta conjunta para Dynamics 365 CRM: información general</span><span class="sxs-lookup"><span data-stu-id="5afdc-103">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="5afdc-104">Roles adecuados</span><span class="sxs-lookup"><span data-stu-id="5afdc-104">Appropriate roles</span></span>

- <span data-ttu-id="5afdc-105">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="5afdc-105">Referrals admin</span></span>
- <span data-ttu-id="5afdc-106">Administrador del sistema o Personalizador del sistema en CRM</span><span class="sxs-lookup"><span data-stu-id="5afdc-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="5afdc-107">El conector de la venta conjunta del centro de Partners permite que los vendedores covendan con Microsoft desde los sistemas CRM.</span><span class="sxs-lookup"><span data-stu-id="5afdc-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="5afdc-108">No tendrán que estar capacitados para utilizar el centro de partners para administrar las ofertas de venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="5afdc-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="5afdc-109">Use los conectores de venta conjunta para crear una nueva referencia de venta conjunta con el fin de invitar a un vendedor de Microsoft, recibir referencias del vendedor de Microsoft, aceptar o rechazar referencias, modificar el trato de los datos, como el valor del trato y la fecha de cierre.</span><span class="sxs-lookup"><span data-stu-id="5afdc-109">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="5afdc-110">También puede recibir cualquier actualización de los vendedores de Microsoft en estos acuerdos de venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="5afdc-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="5afdc-111">Puede realizar todas las referencias en el CRM de su elección, en lugar de hacerlo en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="5afdc-111">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="5afdc-112">La solución se basa en la solución Microsoft Power Automate y usa las API del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="5afdc-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="5afdc-113">Antes de instalar: requisitos previos</span><span class="sxs-lookup"><span data-stu-id="5afdc-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="5afdc-114">**Temas**</span><span class="sxs-lookup"><span data-stu-id="5afdc-114">**Topics**</span></span>   |<span data-ttu-id="5afdc-115">**Detalles**</span><span class="sxs-lookup"><span data-stu-id="5afdc-115">**Details**</span></span>   |<span data-ttu-id="5afdc-116">**Vínculos**</span><span class="sxs-lookup"><span data-stu-id="5afdc-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="5afdc-117">IDENTIFICADOR de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="5afdc-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="5afdc-118">Necesita un ID. de MPN válido</span><span class="sxs-lookup"><span data-stu-id="5afdc-118">You need a valid MPN ID</span></span>|<span data-ttu-id="5afdc-119">Para unirse a [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="5afdc-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="5afdc-120">Lista de coventas</span><span class="sxs-lookup"><span data-stu-id="5afdc-120">Cosell ready</span></span>|<span data-ttu-id="5afdc-121">La solución de IP/servicios debe estar lista para su venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="5afdc-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="5afdc-122">Venda con Microsoft</span><span class="sxs-lookup"><span data-stu-id="5afdc-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="5afdc-123">Cuenta del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="5afdc-123">Partner Center account</span></span>|<span data-ttu-id="5afdc-124">El identificador de MPN asociado al inquilino del centro de Partners debe ser el mismo que el identificador de MPN asociado a la solución de venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="5afdc-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="5afdc-125">Compruebe que puede ver las referencias de venta conjunta en el portal del centro de Partners antes de implementar los conectores.</span><span class="sxs-lookup"><span data-stu-id="5afdc-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="5afdc-126">Administración de la cuenta</span><span class="sxs-lookup"><span data-stu-id="5afdc-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="5afdc-127">Roles de usuario del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="5afdc-127">Partner Center user roles</span></span>|<span data-ttu-id="5afdc-128">El empleado que va a instalar y usar los conectores debe ser un administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="5afdc-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="5afdc-129">Asignar roles y permisos de usuarios</span><span class="sxs-lookup"><span data-stu-id="5afdc-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="5afdc-130">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="5afdc-130">Dynamics 365 CRM</span></span>|<span data-ttu-id="5afdc-131">El rol de usuario CRM es administrador del sistema o Personalizador del sistema</span><span class="sxs-lookup"><span data-stu-id="5afdc-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="5afdc-132">Asignación de roles en Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="5afdc-132">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="5afdc-133">Cuenta de flujo de automatización de energía</span><span class="sxs-lookup"><span data-stu-id="5afdc-133">Power Automate Flow Account</span></span>|<span data-ttu-id="5afdc-134">Una cuenta activa de [Power Automatic](https://flow.microsoft.com) para el administrador del sistema CRM o el personalizador del sistema.</span><span class="sxs-lookup"><span data-stu-id="5afdc-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="5afdc-135">Dicho usuario debe iniciar sesión en [Power automatizate](https://flow.microsoft.com) al menos una vez antes de la instalación.</span><span class="sxs-lookup"><span data-stu-id="5afdc-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="5afdc-136">Instalación de la sincronización de referencias del centro de partners para Dynamics 365 (solución de automatización de energía)</span><span class="sxs-lookup"><span data-stu-id="5afdc-136">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span>

1. <span data-ttu-id="5afdc-137">Vaya a [Power Automatic](https://flow.microsoft.com) y seleccione **entornos** en la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="5afdc-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="5afdc-138">Este paso le mostrará las instancias de CRM disponibles.</span><span class="sxs-lookup"><span data-stu-id="5afdc-138">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="5afdc-139">Seleccione la instancia de CRM correspondiente en la lista desplegable de la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="5afdc-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span>

3. <span data-ttu-id="5afdc-140">Seleccione **soluciones** en la barra de navegación izquierda.</span><span class="sxs-lookup"><span data-stu-id="5afdc-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="5afdc-141">Haga clic en el vínculo **abrir AppSource** en el menú superior.</span><span class="sxs-lookup"><span data-stu-id="5afdc-141">Click on the **Open AppSource** link on the top menu.</span></span>

   :::image type="content" source="images/cosellconnectors/openappsource.png" alt-text="Abrir AppSource":::

5. <span data-ttu-id="5afdc-143">Busque **conectores de referencias del centro de partners para Dynamics365** en la pantalla emergente.</span><span class="sxs-lookup"><span data-stu-id="5afdc-143">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="5afdc-144">Haga clic en el botón **obtener ahora** y **continúe**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-144">Click the **Get it now** button and then **Continue**.</span></span>

7. <span data-ttu-id="5afdc-145">Se abrirá la página en la que puede seleccionar el entorno de CRM (Dynamics 365) para instalar la aplicación.</span><span class="sxs-lookup"><span data-stu-id="5afdc-145">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="5afdc-146">Acepte los términos y condiciones.</span><span class="sxs-lookup"><span data-stu-id="5afdc-146">Agree to terms and conditions.</span></span>

8. <span data-ttu-id="5afdc-147">A continuación, se le dirigirá a la página **administrar soluciones** .</span><span class="sxs-lookup"><span data-stu-id="5afdc-147">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="5afdc-148">Vaya a "referencias del centro de Partners" con los botones de flecha de la parte inferior de la página.</span><span class="sxs-lookup"><span data-stu-id="5afdc-148">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="5afdc-149">La **instalación programada** debe aparecer junto a la solución de referencias del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="5afdc-149">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="5afdc-150">La instalación tardará 10-15 minutos.</span><span class="sxs-lookup"><span data-stu-id="5afdc-150">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="5afdc-151">Una vez completada la instalación, vuelva a [Power Automatic](https://flow.microsoft.com) y seleccione **soluciones** en el área de navegación izquierda.</span><span class="sxs-lookup"><span data-stu-id="5afdc-151">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="5afdc-152">Observe que la **sincronización de las referencias del centro de partners para Dynamics 365** está disponible en la lista de soluciones.</span><span class="sxs-lookup"><span data-stu-id="5afdc-152">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="5afdc-153">Seleccione la **sincronización de referencias del centro de partners para Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-153">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="5afdc-154">Están disponibles los siguientes flujos y entidades:</span><span class="sxs-lookup"><span data-stu-id="5afdc-154">The following Power Automate flows and entities are available:</span></span>

    :::image type="content" source="images/cosellconnectors/dynamics-available-crms.png" alt-text="CRMS disponibles":::

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="5afdc-156">Procedimiento recomendado: prueba antes de la marcha</span><span class="sxs-lookup"><span data-stu-id="5afdc-156">Best practice: test before you go live</span></span>

<span data-ttu-id="5afdc-157">Antes de instalar, configurar y personalizar la solución Power Automate en el entorno de producción, asegúrese de probar la solución en una instancia de CRM provisional.</span><span class="sxs-lookup"><span data-stu-id="5afdc-157">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="5afdc-158">Instale la solución Microsoft Power Automate en un entorno de ensayo o una instancia de CRM.</span><span class="sxs-lookup"><span data-stu-id="5afdc-158">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="5afdc-159">Realice una copia de la solución y ejecute la configuración y la automatización de las personalizaciones de flujo en el entorno de ensayo.</span><span class="sxs-lookup"><span data-stu-id="5afdc-159">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="5afdc-160">Pruebe la solución en una instancia de ensayo o CRM.</span><span class="sxs-lookup"><span data-stu-id="5afdc-160">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="5afdc-161">En caso de éxito, importe como solución administrada a la instancia de producción.</span><span class="sxs-lookup"><span data-stu-id="5afdc-161">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="5afdc-162">Configuración de la solución</span><span class="sxs-lookup"><span data-stu-id="5afdc-162">Configure the solution</span></span>

1. <span data-ttu-id="5afdc-163">Una vez que haya instalado la solución en la instancia de CRM, vuelva a [Power Automatic](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="5afdc-163">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="5afdc-164">En la lista desplegable de **entornos** de la esquina superior derecha, seleccione la instancia de CRM en la que instaló la solución Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="5afdc-164">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="5afdc-165">Deberá crear conexiones que asocien las tres cuentas de usuario:</span><span class="sxs-lookup"><span data-stu-id="5afdc-165">You'll need to create connections that associate the three user accounts:</span></span>

   - <span data-ttu-id="5afdc-166">Usuario del centro de Partners con credenciales de administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="5afdc-166">Partner Center user with referrals admin credentials</span></span>

   - <span data-ttu-id="5afdc-167">Eventos del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="5afdc-167">Partner Center Events</span></span>

   - <span data-ttu-id="5afdc-168">Administrador de CRM con la potencia que automatiza los flujos en la solución.</span><span class="sxs-lookup"><span data-stu-id="5afdc-168">CRM admin with the Power Automate flows in the solution.</span></span>

      1. <span data-ttu-id="5afdc-169">Seleccione **conexiones** en la barra de navegación izquierda y seleccione la solución "referencias del centro de Partners" en la lista.</span><span class="sxs-lookup"><span data-stu-id="5afdc-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

      2. <span data-ttu-id="5afdc-170">Cree una conexión haciendo clic en **crear una conexión**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-170">Create a connection by clicking **Create a connection**.</span></span>

         :::image type="content" source="images/cosellconnectors/createconnection.png" alt-text="Crear conexión":::

      3. <span data-ttu-id="5afdc-172">Busque **referencias del centro de Partners (versión preliminar)** en la barra de búsqueda en la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="5afdc-172">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

      4. <span data-ttu-id="5afdc-173">Cree una conexión para el usuario del centro de Partners con el rol de credenciales de administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="5afdc-173">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

      5. <span data-ttu-id="5afdc-174">A continuación, cree una conexión de eventos del centro de partners para el usuario del centro de Partners con las credenciales de administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="5afdc-174">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

      6. <span data-ttu-id="5afdc-175">Cree una conexión para Common Data Service (entorno actual) para el usuario administrador de CRM.</span><span class="sxs-lookup"><span data-stu-id="5afdc-175">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="5afdc-176">Para asociar los flujos de alimentación automatizada con las conexiones, edite cada uno de los flujos de Power Automatic para conectarse a Common Data Service y a las referencias del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="5afdc-176">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="5afdc-177">Guarde los cambios.</span><span class="sxs-lookup"><span data-stu-id="5afdc-177">Save the changes.</span></span>

5. <span data-ttu-id="5afdc-178">**Encienda** los flujos automáticos de energía.</span><span class="sxs-lookup"><span data-stu-id="5afdc-178">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="5afdc-179">Uso de las API de webhook para registrar eventos de cambio de recursos</span><span class="sxs-lookup"><span data-stu-id="5afdc-179">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="5afdc-180">Las API del webhook del centro de Partners le permiten registrarse para los eventos de cambio de recursos.</span><span class="sxs-lookup"><span data-stu-id="5afdc-180">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="5afdc-181">Estos eventos de cambio se envían a la dirección URL como publicaciones HTTP.</span><span class="sxs-lookup"><span data-stu-id="5afdc-181">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="5afdc-182">Para registrar la dirección URL, seleccione **registro de webhook del centro de Partners (versión preliminar de Insider)** flujo de automatización.</span><span class="sxs-lookup"><span data-stu-id="5afdc-182">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="5afdc-183">Agregar conexiones para () Usuario del centro de Partners con credenciales de administrador de referencias (b.) Eventos del centro de Partners, tal y como se resalta</span><span class="sxs-lookup"><span data-stu-id="5afdc-183">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

   :::image type="content" source="images/cosellconnectors/triggerflow.png" alt-text="Desencadenador":::

3. <span data-ttu-id="5afdc-185">Cuando realice estas actualizaciones, verá</span><span class="sxs-lookup"><span data-stu-id="5afdc-185">When you make these updates, you'll see</span></span>

   :::image type="content" source="images/cosellconnectors/webhook1.png" alt-text="Webhooks":::

4. <span data-ttu-id="5afdc-187">Guarde los cambios y seleccione **Activar**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-187">Save your changes and select **Turn on**.</span></span>

   <span data-ttu-id="5afdc-188">Para permitir que los webhooks del centro de Partners escuchen los cambios de eventos, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="5afdc-188">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="5afdc-189">Seleccione **centro de partners para Dynamics 365 (versión preliminar de Insider)**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-189">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="5afdc-190">Seleccione el icono de **edición** y seleccione **cuando se reciba una solicitud HTTP**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-190">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="5afdc-191">Seleccione el icono de **copiar** para copiar la dirección URL http post proporcionada.</span><span class="sxs-lookup"><span data-stu-id="5afdc-191">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

   :::image type="content" source="images/cosellconnectors/copyurl.png" alt-text="Copiar la dirección URL":::

8. <span data-ttu-id="5afdc-193">Ahora, seleccione "registro de webhook del centro de Partners (versión preliminar de Insider)" flujo automático de energía y seleccione **Ejecutar**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-193">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="5afdc-194">Asegúrese de que se abre la ventana "flujo de ejecución" en el panel derecho y haga clic en **continuar**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-194">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="5afdc-195">Escriba la siguiente información:</span><span class="sxs-lookup"><span data-stu-id="5afdc-195">Enter the following details:</span></span>

    1. <span data-ttu-id="5afdc-196">**Punto de conexión de desencadenador http**: dirección URL copiada del paso anterior</span><span class="sxs-lookup"><span data-stu-id="5afdc-196">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    2. <span data-ttu-id="5afdc-197">**Eventos para registrar**: "referencia creada" y "referencia-actualizada"</span><span class="sxs-lookup"><span data-stu-id="5afdc-197">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    3. <span data-ttu-id="5afdc-198">**Sobrescribir puntos de conexión de desencadenador existentes si están presentes**: sí (esto Sobrescribe todos los extremos existentes).</span><span class="sxs-lookup"><span data-stu-id="5afdc-198">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

11. <span data-ttu-id="5afdc-199">Seleccione **Ejecutar** y, a continuación, haga clic en **listo.**</span><span class="sxs-lookup"><span data-stu-id="5afdc-199">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="5afdc-200">Ahora, el webhook puede escuchar la creación y actualización de eventos.</span><span class="sxs-lookup"><span data-stu-id="5afdc-200">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="5afdc-201">Personalizar pasos de sincronización</span><span class="sxs-lookup"><span data-stu-id="5afdc-201">Customize synchronization steps</span></span>

<span data-ttu-id="5afdc-202">Cuando se sincronizan las referencias de venta conjunta entre el centro de Partners y el sistema CRM, los campos que se sincronizan en el equipo del centro de Partners se enumeran aquí.</span><span class="sxs-lookup"><span data-stu-id="5afdc-202">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="5afdc-203">A menudo, los sistemas CRM son muy personalizados.</span><span class="sxs-lookup"><span data-stu-id="5afdc-203">Often CRM systems are highly customized.</span></span> <span data-ttu-id="5afdc-204">Puede personalizar los flujos de automatización.</span><span class="sxs-lookup"><span data-stu-id="5afdc-204">You can customize the Power Automate flows.</span></span> <span data-ttu-id="5afdc-205">Siga la guía de asignación de campos y, si es necesario, realice los cambios adecuados en los pasos de la potencia que automatiza los flujos.</span><span class="sxs-lookup"><span data-stu-id="5afdc-205">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="5afdc-206">Se proporcionan las asignaciones de Microsoft Partner Center a CRM, pero en función de su entorno de CRM, puede optar por personalizar aún más los campos.</span><span class="sxs-lookup"><span data-stu-id="5afdc-206">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="5afdc-207">Se pueden personalizar varios pasos de cada uno de los flujos de potencia automatizados en función de sus necesidades.</span><span class="sxs-lookup"><span data-stu-id="5afdc-207">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="5afdc-208">Estos son algunos ejemplos de las personalizaciones disponibles:</span><span class="sxs-lookup"><span data-stu-id="5afdc-208">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="5afdc-209">Para personalizar los campos de los eventos de creación o actualización en el centro de partners para la sincronización de referencias de CRM:</span><span class="sxs-lookup"><span data-stu-id="5afdc-209">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="5afdc-210">a.</span><span class="sxs-lookup"><span data-stu-id="5afdc-210">a.</span></span> <span data-ttu-id="5afdc-211">Seleccione centro de partners para Dynamics 365 (versión preliminar de Insider) o centro de partners a Salesforce (versión preliminar de Insider).</span><span class="sxs-lookup"><span data-stu-id="5afdc-211">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="5afdc-212">b.</span><span class="sxs-lookup"><span data-stu-id="5afdc-212">b.</span></span> <span data-ttu-id="5afdc-213">Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="5afdc-213">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="5afdc-214">c.</span><span class="sxs-lookup"><span data-stu-id="5afdc-214">c.</span></span> <span data-ttu-id="5afdc-215">Seleccione **(ámbito) sincronizar el cliente potencial o la oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-215">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="5afdc-216">Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para crear eventos, seleccione si se trata de una **nueva oportunidad compartida y, a continuación**, haga clic en.</span><span class="sxs-lookup"><span data-stu-id="5afdc-216">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="5afdc-217">Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda **crear una nueva oportunidad en CRM**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-217">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="5afdc-218">Puede editar las asignaciones en esta sección mediante la guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="5afdc-218">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="5afdc-219">d.</span><span class="sxs-lookup"><span data-stu-id="5afdc-219">d.</span></span> <span data-ttu-id="5afdc-220">Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para los eventos de actualización, haga clic en el paso "(ámbito) sincronizar el cliente potencial o la oportunidad".</span><span class="sxs-lookup"><span data-stu-id="5afdc-220">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="5afdc-221">e.</span><span class="sxs-lookup"><span data-stu-id="5afdc-221">e.</span></span> <span data-ttu-id="5afdc-222">Seleccione **si se trata de una actualización de una oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-222">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="5afdc-223">Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda **si la diferencia entre los objetos de oportunidad del centro de Partners y CRM**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-223">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="5afdc-224">f.</span><span class="sxs-lookup"><span data-stu-id="5afdc-224">f.</span></span> <span data-ttu-id="5afdc-225">Seleccione **si sí** seguido de **Actualizar oportunidad existente** .</span><span class="sxs-lookup"><span data-stu-id="5afdc-225">Select **If yes** followed with **Update existing opportunity**</span></span>

3. <span data-ttu-id="5afdc-226">Para personalizar los campos de la sincronización de referencia de CRM a equipo para eventos de actualización:</span><span class="sxs-lookup"><span data-stu-id="5afdc-226">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="5afdc-227">a.</span><span class="sxs-lookup"><span data-stu-id="5afdc-227">a.</span></span> <span data-ttu-id="5afdc-228">Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="5afdc-228">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="5afdc-229">b.</span><span class="sxs-lookup"><span data-stu-id="5afdc-229">b.</span></span> <span data-ttu-id="5afdc-230">Seleccione **(ámbito) sincronizar la oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-230">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="5afdc-231">c.</span><span class="sxs-lookup"><span data-stu-id="5afdc-231">c.</span></span> <span data-ttu-id="5afdc-232">Para personalizar las asignaciones de campos de CRM para los eventos de actualización, seleccione **si hay diferencias entre los objetos de cliente potencial del centro de Partners y CRM y, a continuación, haga clic en**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-232">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="5afdc-233">d.</span><span class="sxs-lookup"><span data-stu-id="5afdc-233">d.</span></span> <span data-ttu-id="5afdc-234">Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda el paso **actualizar una referencia con los datos de oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-234">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

   <span data-ttu-id="5afdc-235">Puede editar las asignaciones en esta sección basándose en la guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="5afdc-235">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="5afdc-236">Para personalizar los campos de la sincronización de referencia de CRM a equipo para crear eventos</span><span class="sxs-lookup"><span data-stu-id="5afdc-236">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="5afdc-237">a.</span><span class="sxs-lookup"><span data-stu-id="5afdc-237">a.</span></span> <span data-ttu-id="5afdc-238">Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="5afdc-238">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="5afdc-239">b.</span><span class="sxs-lookup"><span data-stu-id="5afdc-239">b.</span></span> <span data-ttu-id="5afdc-240">Seleccione **(ámbito) sincronizar referencias.**</span><span class="sxs-lookup"><span data-stu-id="5afdc-240">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="5afdc-241">c.</span><span class="sxs-lookup"><span data-stu-id="5afdc-241">c.</span></span> <span data-ttu-id="5afdc-242">Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para crear eventos, seleccione **crear referencia de Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-242">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span>

   <span data-ttu-id="5afdc-243">Puede editar las asignaciones en esta sección basándose en la guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="5afdc-243">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="5afdc-244">Sincronización de referencia de venta conjunta bidireccional de un extremo a otro</span><span class="sxs-lookup"><span data-stu-id="5afdc-244">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="5afdc-245">Una vez que haya instalado, configurado y personalizado la solución Power Automate, puede probar la sincronización de referencias de venta conjunta entre Dynamics 365 y el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="5afdc-245">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="5afdc-246">Requisitos previos</span><span class="sxs-lookup"><span data-stu-id="5afdc-246">Pre-requisites</span></span>

<span data-ttu-id="5afdc-247">Para sincronizar las referencias entre el centro de Partners y Dynamics 365 CRM, la solución Power Automate marca claramente los campos de referencia específicos de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5afdc-247">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="5afdc-248">Esta identificación proporciona a los equipos de vendedores la capacidad de decidir qué referencias desean compartir con Microsoft para la venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="5afdc-248">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="5afdc-249">Un conjunto de campos personalizados está disponible como parte de la entidad de **oportunidad** .</span><span class="sxs-lookup"><span data-stu-id="5afdc-249">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="5afdc-250">Un usuario administrador de CRM tendrá que crear una sección de CRM independiente con los campos personalizados de la **oportunidad** .</span><span class="sxs-lookup"><span data-stu-id="5afdc-250">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="5afdc-251">Los siguientes campos personalizados deben formar parte de la sección CRM:</span><span class="sxs-lookup"><span data-stu-id="5afdc-251">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="5afdc-252">**Sincronizar con el centro de Partners**: si se va a sincronizar la oportunidad con el centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="5afdc-252">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="5afdc-253">**Identificador de referencia**: un campo de identificador de solo lectura para la referencia del centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="5afdc-253">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="5afdc-254">**Vínculo de referencia**: un vínculo de solo lectura a la referencia en el centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="5afdc-254">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="5afdc-255">**¿Cómo puede ayudarle Microsoft?**: ayuda necesaria de Microsoft para la referencia</span><span class="sxs-lookup"><span data-stu-id="5afdc-255">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="5afdc-256">**Productos**: lista de productos asociados a esta oportunidad</span><span class="sxs-lookup"><span data-stu-id="5afdc-256">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="5afdc-257">**Audit**: una pista de auditoría de solo lectura para la sincronización con las referencias del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="5afdc-257">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="5afdc-258">SITUACIÓN</span><span class="sxs-lookup"><span data-stu-id="5afdc-258">SCENARIOS:</span></span>

1. <span data-ttu-id="5afdc-259">Sincronización de referencia cuando se crea o actualiza una referencia en CRM y se sincroniza en el centro de Partners:</span><span class="sxs-lookup"><span data-stu-id="5afdc-259">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

   1. <span data-ttu-id="5afdc-260">Inicie sesión en el entorno de CRM de Dynamics 365 con un usuario que tenga visibilidad en la sección de **oportunidades** de CRM.</span><span class="sxs-lookup"><span data-stu-id="5afdc-260">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

   2. <span data-ttu-id="5afdc-261">Asegúrese de que la siguiente sección está presente al crear una "nueva oportunidad" en el entorno de Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="5afdc-261">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

      :::image type="content" source="images/cosellconnectors/opportunity.png" alt-text="Oportunidad":::

   3. <span data-ttu-id="5afdc-263">Para sincronizar esta oportunidad con el centro de Partners de Microsoft, asegúrese de establecer los siguientes campos en la vista tarjeta:</span><span class="sxs-lookup"><span data-stu-id="5afdc-263">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

      - <span data-ttu-id="5afdc-264">**Sincronizar con el centro de Partners**: sí</span><span class="sxs-lookup"><span data-stu-id="5afdc-264">**Sync with Partner Center**: Yes</span></span>

      - <span data-ttu-id="5afdc-265">**¿Cómo puede ayudarle Microsoft?**: Seleccione una de las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="5afdc-265">**How can Microsoft help?**: Select from the following:</span></span>

         :::image type="content" source="images/cosellconnectors/help.png" alt-text="Selecciones de la ayuda":::

      - <span data-ttu-id="5afdc-267">**Productos**: identificadores de la solución del producto</span><span class="sxs-lookup"><span data-stu-id="5afdc-267">**Products**: Solution IDs of the product</span></span>

   4. <span data-ttu-id="5afdc-268">Una vez creada la oportunidad en Dynamics 365 con la opción **sincronizar con el centro de Partners** establecida en **sí**, espere 10 minutos y, a continuación, inicie sesión en su cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="5afdc-268">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="5afdc-269">Las referencias se sincronizarán con Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="5afdc-269">Your referrals will be synchronized with Dynamics 365.</span></span>

   5. <span data-ttu-id="5afdc-270">Del mismo modo, para una oportunidad que tuviera la opción "sincronizar con el centro de Partners" establecida en "sí", si actualizas la oportunidad en Dynamics 365 CRM, los cambios se sincronizarán en la cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="5afdc-270">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

   6. <span data-ttu-id="5afdc-271">Las oportunidades que se sincronizan correctamente con el centro de Partners se identificarán con ✔ icono en Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="5afdc-271">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="5afdc-272">Sincronización de referencia cuando se crea o actualiza una referencia en el centro de Partners de Microsoft y se sincroniza en el entorno de Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="5afdc-272">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

   1. <span data-ttu-id="5afdc-273">Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard/home)del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="5afdc-273">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

   2. <span data-ttu-id="5afdc-274">Seleccione **referencias** en el menú de la izquierda.</span><span class="sxs-lookup"><span data-stu-id="5afdc-274">Select **Referrals** from the left-hand menu.</span></span>

   3. <span data-ttu-id="5afdc-275">Cree una nueva referencia de venta conjunta desde el centro de partners; para ello, haga clic en la opción "nuevo trato".</span><span class="sxs-lookup"><span data-stu-id="5afdc-275">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

   4. <span data-ttu-id="5afdc-276">Inicie sesión en el entorno de CRM de Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="5afdc-276">Sign into your Dynamics 365 CRM environment.</span></span>

   5. <span data-ttu-id="5afdc-277">Vaya a **abrir oportunidades**.</span><span class="sxs-lookup"><span data-stu-id="5afdc-277">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="5afdc-278">La referencia creada en el centro de Partners de Microsoft ya está sincronizada en Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="5afdc-278">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

   6. <span data-ttu-id="5afdc-279">Al seleccionar una referencia sincronizada, se rellenan los detalles de la vista de tarjeta.</span><span class="sxs-lookup"><span data-stu-id="5afdc-279">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="5afdc-280">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="5afdc-280">Next steps</span></span>

- [<span data-ttu-id="5afdc-281">Administrar los clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="5afdc-281">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="5afdc-282">Administrar las oportunidades de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="5afdc-282">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="5afdc-283">¿Más información sobre la plataforma Microsoft Power Automate?</span><span class="sxs-lookup"><span data-stu-id="5afdc-283">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="5afdc-284">Webhooks del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="5afdc-284">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)