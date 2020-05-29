---
title: El conector de venta conjunta para el centro de Partners de Dynamics 365 CRM
ms.topic: article
ms.date: 05/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sincronizar las referencias en el centro de Partners con el CRM de Dynamics 365
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: 87b1d27fa2f42eeba3b0f8308648536c0686911e
ms.sourcegitcommit: c13723216761e60d2b37596efc71f5fdecb30be1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/28/2020
ms.locfileid: "84145139"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="23652-103">Conector de venta conjunta para Dynamics 365 CRM: información general</span><span class="sxs-lookup"><span data-stu-id="23652-103">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="23652-104">Roles adecuados</span><span class="sxs-lookup"><span data-stu-id="23652-104">Appropriate roles</span></span>

- <span data-ttu-id="23652-105">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="23652-105">Referrals admin</span></span>
- <span data-ttu-id="23652-106">Administrador del sistema o Personalizador del sistema en CRM</span><span class="sxs-lookup"><span data-stu-id="23652-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="23652-107">El conector de la venta conjunta del centro de Partners permite que los vendedores covendan con Microsoft desde los sistemas CRM.</span><span class="sxs-lookup"><span data-stu-id="23652-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="23652-108">No tendrán que estar capacitados para utilizar el centro de partners para administrar las ofertas de venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="23652-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="23652-109">Use los conectores de venta conjunta para crear una nueva referencia de venta conjunta con el fin de invitar a un vendedor de Microsoft, recibir referencias del vendedor de Microsoft, aceptar o rechazar referencias, modificar el trato de los datos, como el valor del trato y la fecha de cierre.</span><span class="sxs-lookup"><span data-stu-id="23652-109">Use the Co-sell connectors, to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, and closing date.</span></span> <span data-ttu-id="23652-110">También puede recibir cualquier actualización de los vendedores de Microsoft en estos acuerdos de venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="23652-110">You can also receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="23652-111">Puede realizar todas las referencias en el CRM de su elección, en lugar de hacerlo en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="23652-111">You can do all of your referrals work within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="23652-112">La solución se basa en la solución Microsoft Power Automate y usa las API del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="23652-112">The solution is based on Microsoft Power Automate Solution and uses Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="23652-113">Antes de instalar: requisitos previos</span><span class="sxs-lookup"><span data-stu-id="23652-113">Before you install - pre-requisites</span></span>

|<span data-ttu-id="23652-114">**Temas**</span><span class="sxs-lookup"><span data-stu-id="23652-114">**Topics**</span></span>   |<span data-ttu-id="23652-115">**Detalles**</span><span class="sxs-lookup"><span data-stu-id="23652-115">**Details**</span></span>   |<span data-ttu-id="23652-116">**Vínculos**</span><span class="sxs-lookup"><span data-stu-id="23652-116">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="23652-117">IDENTIFICADOR de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="23652-117">Microsoft Partner Network ID</span></span> |<span data-ttu-id="23652-118">Necesita un ID. de MPN válido</span><span class="sxs-lookup"><span data-stu-id="23652-118">You need a valid MPN ID</span></span>|<span data-ttu-id="23652-119">Para unirse a [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="23652-119">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="23652-120">Lista de coventas</span><span class="sxs-lookup"><span data-stu-id="23652-120">Cosell ready</span></span>|<span data-ttu-id="23652-121">La solución de IP/servicios debe estar lista para su venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="23652-121">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="23652-122">Venda con Microsoft</span><span class="sxs-lookup"><span data-stu-id="23652-122">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="23652-123">Cuenta del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="23652-123">Partner Center account</span></span>|<span data-ttu-id="23652-124">El identificador de MPN asociado al inquilino del centro de Partners debe ser el mismo que el identificador de MPN asociado a la solución de venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="23652-124">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="23652-125">Compruebe que puede ver las referencias de venta conjunta en el portal del centro de Partners antes de implementar los conectores.</span><span class="sxs-lookup"><span data-stu-id="23652-125">Verify that you can see your co-sell referrals in Partner Center portal before deploying the connectors.</span></span>|[<span data-ttu-id="23652-126">Administración de la cuenta</span><span class="sxs-lookup"><span data-stu-id="23652-126">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="23652-127">Roles de usuario del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="23652-127">Partner Center user roles</span></span>|<span data-ttu-id="23652-128">El empleado que va a instalar y usar los conectores debe ser un administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="23652-128">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="23652-129">Asignar roles y permisos de usuarios</span><span class="sxs-lookup"><span data-stu-id="23652-129">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="23652-130">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="23652-130">Dynamics 365 CRM</span></span>|<span data-ttu-id="23652-131">El rol de usuario CRM es administrador del sistema o Personalizador del sistema</span><span class="sxs-lookup"><span data-stu-id="23652-131">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="23652-132">Asignación de roles en Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="23652-132">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="23652-133">Cuenta de flujo de automatización de energía</span><span class="sxs-lookup"><span data-stu-id="23652-133">Power Automate Flow Account</span></span>|<span data-ttu-id="23652-134">Una cuenta activa de [Power Automatic](https://flow.microsoft.com) para el administrador del sistema CRM o el personalizador del sistema.</span><span class="sxs-lookup"><span data-stu-id="23652-134">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="23652-135">Dicho usuario debe iniciar sesión en [Power automatizate](https://flow.microsoft.com) al menos una vez antes de la instalación.</span><span class="sxs-lookup"><span data-stu-id="23652-135">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="23652-136">Instalación de la sincronización de referencias del centro de partners para Dynamics 365 (solución de automatización de energía)</span><span class="sxs-lookup"><span data-stu-id="23652-136">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span> 

1. <span data-ttu-id="23652-137">Vaya a [Power Automatic](https://flow.microsoft.com) y seleccione **entornos** en la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="23652-137">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="23652-138">Este paso le mostrará las instancias de CRM disponibles.</span><span class="sxs-lookup"><span data-stu-id="23652-138">This step will show you the available CRM instances.</span></span>

2. <span data-ttu-id="23652-139">Seleccione la instancia de CRM correspondiente en la lista desplegable de la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="23652-139">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="23652-140">Seleccione **soluciones** en la barra de navegación izquierda.</span><span class="sxs-lookup"><span data-stu-id="23652-140">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="23652-141">Haga clic en el vínculo **abrir AppSource** en el menú superior.</span><span class="sxs-lookup"><span data-stu-id="23652-141">Click on the **Open AppSource** link on the top menu.</span></span>

![Abrir AppSource](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="23652-143">Busque **conectores de referencias del centro de partners para Dynamics365** en la pantalla emergente.</span><span class="sxs-lookup"><span data-stu-id="23652-143">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="23652-144">Haga clic en el botón **obtener ahora** y **continúe**.</span><span class="sxs-lookup"><span data-stu-id="23652-144">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="23652-145">Se abrirá la página en la que puede seleccionar el entorno de CRM (Dynamics 365) para instalar la aplicación.</span><span class="sxs-lookup"><span data-stu-id="23652-145">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="23652-146">Acepte los términos y condiciones.</span><span class="sxs-lookup"><span data-stu-id="23652-146">Agree to terms and conditions.</span></span> 

8. <span data-ttu-id="23652-147">A continuación, se le dirigirá a la página **administrar soluciones** .</span><span class="sxs-lookup"><span data-stu-id="23652-147">You're then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="23652-148">Vaya a "referencias del centro de Partners" con los botones de flecha de la parte inferior de la página.</span><span class="sxs-lookup"><span data-stu-id="23652-148">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="23652-149">La **instalación programada** debe aparecer junto a la solución de referencias del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="23652-149">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="23652-150">La instalación tardará 10-15 minutos.</span><span class="sxs-lookup"><span data-stu-id="23652-150">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="23652-151">Una vez completada la instalación, vuelva a [Power Automatic](https://flow.microsoft.com) y seleccione **soluciones** en el área de navegación izquierda.</span><span class="sxs-lookup"><span data-stu-id="23652-151">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="23652-152">Observe que la **sincronización de las referencias del centro de partners para Dynamics 365** está disponible en la lista de soluciones.</span><span class="sxs-lookup"><span data-stu-id="23652-152">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="23652-153">Seleccione la **sincronización de referencias del centro de partners para Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="23652-153">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="23652-154">Están disponibles los siguientes flujos y entidades:</span><span class="sxs-lookup"><span data-stu-id="23652-154">The following Power Automate flows and entities are available:</span></span>

![CRMS disponibles](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="23652-156">Procedimiento recomendado: prueba antes de la marcha</span><span class="sxs-lookup"><span data-stu-id="23652-156">Best practice: test before you go live</span></span>

<span data-ttu-id="23652-157">Antes de instalar, configurar y personalizar la solución Power Automate en el entorno de producción, asegúrese de probar la solución en una instancia de CRM provisional.</span><span class="sxs-lookup"><span data-stu-id="23652-157">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="23652-158">Instale la solución Microsoft Power Automate en un entorno de ensayo o una instancia de CRM.</span><span class="sxs-lookup"><span data-stu-id="23652-158">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="23652-159">Realice una copia de la solución y ejecute la configuración y la automatización de las personalizaciones de flujo en el entorno de ensayo.</span><span class="sxs-lookup"><span data-stu-id="23652-159">Make a copy of the solution and run your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="23652-160">Pruebe la solución en una instancia de ensayo o CRM.</span><span class="sxs-lookup"><span data-stu-id="23652-160">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="23652-161">En caso de éxito, importe como solución administrada a la instancia de producción.</span><span class="sxs-lookup"><span data-stu-id="23652-161">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="23652-162">Configuración de la solución</span><span class="sxs-lookup"><span data-stu-id="23652-162">Configure the solution</span></span>

1. <span data-ttu-id="23652-163">Una vez que haya instalado la solución en la instancia de CRM, vuelva a [Power Automatic](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="23652-163">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="23652-164">En la lista desplegable de **entornos** de la esquina superior derecha, seleccione la instancia de CRM en la que instaló la solución Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="23652-164">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="23652-165">Deberá crear conexiones que asocien las tres cuentas de usuario:</span><span class="sxs-lookup"><span data-stu-id="23652-165">You'll need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="23652-166">Usuario del centro de Partners con credenciales de administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="23652-166">Partner Center user with referrals admin credentials</span></span> 

- <span data-ttu-id="23652-167">Eventos del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="23652-167">Partner Center Events</span></span>

- <span data-ttu-id="23652-168">Administrador de CRM con la potencia que automatiza los flujos en la solución.</span><span class="sxs-lookup"><span data-stu-id="23652-168">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="23652-169">a.</span><span class="sxs-lookup"><span data-stu-id="23652-169">a.</span></span> <span data-ttu-id="23652-170">Seleccione **conexiones** en la barra de navegación izquierda y seleccione la solución "referencias del centro de Partners" en la lista.</span><span class="sxs-lookup"><span data-stu-id="23652-170">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>

    <span data-ttu-id="23652-171">b.</span><span class="sxs-lookup"><span data-stu-id="23652-171">b.</span></span> <span data-ttu-id="23652-172">Cree una conexión haciendo clic en **crear una conexión**.</span><span class="sxs-lookup"><span data-stu-id="23652-172">Create a connection by clicking **Create a connection**.</span></span>

    ![Crear conexión](images/cosellconnectors/createconnection.png)

    <span data-ttu-id="23652-174">c.</span><span class="sxs-lookup"><span data-stu-id="23652-174">c.</span></span> <span data-ttu-id="23652-175">Busque **referencias del centro de Partners (versión preliminar)** en la barra de búsqueda en la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="23652-175">Search for **Partner Center Referrals (preview)** in the search bar on the top-right corner.</span></span>

    <span data-ttu-id="23652-176">d.</span><span class="sxs-lookup"><span data-stu-id="23652-176">d.</span></span> <span data-ttu-id="23652-177">Cree una conexión para el usuario del centro de Partners con el rol de credenciales de administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="23652-177">Create a connection for your Partner Center user with the credentials role of Referrals admin.</span></span>

    <span data-ttu-id="23652-178">e.</span><span class="sxs-lookup"><span data-stu-id="23652-178">e.</span></span> <span data-ttu-id="23652-179">A continuación, cree una conexión de eventos del centro de partners para el usuario del centro de Partners con las credenciales de administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="23652-179">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin.</span></span>

    <span data-ttu-id="23652-180">f.</span><span class="sxs-lookup"><span data-stu-id="23652-180">f.</span></span> <span data-ttu-id="23652-181">Cree una conexión para Common Data Service (entorno actual) para el usuario administrador de CRM.</span><span class="sxs-lookup"><span data-stu-id="23652-181">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="23652-182">Para asociar los flujos de alimentación automatizada con las conexiones, edite cada uno de los flujos de Power Automatic para conectarse a Common Data Service y a las referencias del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="23652-182">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="23652-183">Guarde los cambios.</span><span class="sxs-lookup"><span data-stu-id="23652-183">Save the changes.</span></span>

5. <span data-ttu-id="23652-184">**Encienda** los flujos automáticos de energía.</span><span class="sxs-lookup"><span data-stu-id="23652-184">**Turn on** the Power Automate flows.</span></span>

## <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="23652-185">Uso de las API de webhook para registrar eventos de cambio de recursos</span><span class="sxs-lookup"><span data-stu-id="23652-185">Use Webhook APIs to register for resource change events</span></span>

<span data-ttu-id="23652-186">Las API del webhook del centro de Partners le permiten registrarse para los eventos de cambio de recursos.</span><span class="sxs-lookup"><span data-stu-id="23652-186">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="23652-187">Estos eventos de cambio se envían a la dirección URL como publicaciones HTTP.</span><span class="sxs-lookup"><span data-stu-id="23652-187">These change events are sent to your url as HTTP posts.</span></span>

1. <span data-ttu-id="23652-188">Para registrar la dirección URL, seleccione **registro de webhook del centro de Partners (versión preliminar de Insider)** flujo de automatización.</span><span class="sxs-lookup"><span data-stu-id="23652-188">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="23652-189">Agregar conexiones para () Usuario del centro de Partners con credenciales de administrador de referencias (b.) Eventos del centro de Partners, tal y como se resalta</span><span class="sxs-lookup"><span data-stu-id="23652-189">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![Desencadenador](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="23652-191">Cuando realice estas actualizaciones, verá</span><span class="sxs-lookup"><span data-stu-id="23652-191">When you make these updates, you'll see</span></span>

![webhooks](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="23652-193">Guarde los cambios y seleccione **Activar**.</span><span class="sxs-lookup"><span data-stu-id="23652-193">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="23652-194">Para permitir que los webhooks del centro de Partners escuchen los cambios de eventos, siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="23652-194">To enable Partner Center webhooks to listen to event changes, do the following steps:</span></span>

5. <span data-ttu-id="23652-195">Seleccione **centro de partners para Dynamics 365 (versión preliminar de Insider)**.</span><span class="sxs-lookup"><span data-stu-id="23652-195">Select **Partner Center to Dynamics 365 (Insider Preview)**.</span></span>

6. <span data-ttu-id="23652-196">Seleccione el icono de **edición** y seleccione **cuando se reciba una solicitud HTTP**.</span><span class="sxs-lookup"><span data-stu-id="23652-196">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="23652-197">Seleccione el icono de **copiar** para copiar la dirección URL http post proporcionada.</span><span class="sxs-lookup"><span data-stu-id="23652-197">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![Copiar la dirección URL](images/cosellconnectors/copyurl.png)

8. <span data-ttu-id="23652-199">Ahora, seleccione "registro de webhook del centro de Partners (versión preliminar de Insider)" flujo automático de energía y seleccione **Ejecutar**.</span><span class="sxs-lookup"><span data-stu-id="23652-199">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="23652-200">Asegúrese de que se abre la ventana "flujo de ejecución" en el panel derecho y haga clic en **continuar**.</span><span class="sxs-lookup"><span data-stu-id="23652-200">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="23652-201">Escriba la siguiente información:</span><span class="sxs-lookup"><span data-stu-id="23652-201">Enter the following details:</span></span> 

    <span data-ttu-id="23652-202">a.</span><span class="sxs-lookup"><span data-stu-id="23652-202">a.</span></span> <span data-ttu-id="23652-203">**Punto de conexión de desencadenador http**: dirección URL copiada del paso anterior</span><span class="sxs-lookup"><span data-stu-id="23652-203">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="23652-204">b.</span><span class="sxs-lookup"><span data-stu-id="23652-204">b.</span></span> <span data-ttu-id="23652-205">**Eventos para registrar**: "referencia creada" y "referencia-actualizada"</span><span class="sxs-lookup"><span data-stu-id="23652-205">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="23652-206">c.</span><span class="sxs-lookup"><span data-stu-id="23652-206">c.</span></span> <span data-ttu-id="23652-207">**Sobrescribir puntos de conexión de desencadenador existentes si están presentes**: sí (esto Sobrescribe todos los extremos existentes).</span><span class="sxs-lookup"><span data-stu-id="23652-207">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span> 

11. <span data-ttu-id="23652-208">Seleccione **Ejecutar** y, a continuación, haga clic en **listo.**</span><span class="sxs-lookup"><span data-stu-id="23652-208">Select **Run** and then select **Done.**</span></span>

<span data-ttu-id="23652-209">Ahora, el webhook puede escuchar la creación y actualización de eventos.</span><span class="sxs-lookup"><span data-stu-id="23652-209">The webhook can now listen to create and update events.</span></span>

## <a name="customize-synchronization-steps"></a><span data-ttu-id="23652-210">Personalizar pasos de sincronización</span><span class="sxs-lookup"><span data-stu-id="23652-210">Customize synchronization steps</span></span>

<span data-ttu-id="23652-211">Cuando se sincronizan las referencias de venta conjunta entre el centro de Partners y el sistema CRM, los campos que se sincronizan en el equipo del centro de Partners se enumeran aquí.</span><span class="sxs-lookup"><span data-stu-id="23652-211">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="23652-212">A menudo, los sistemas CRM son muy personalizados.</span><span class="sxs-lookup"><span data-stu-id="23652-212">Often CRM systems are highly customized.</span></span> <span data-ttu-id="23652-213">Puede personalizar los flujos de automatización.</span><span class="sxs-lookup"><span data-stu-id="23652-213">You can customize the Power Automate flows.</span></span> <span data-ttu-id="23652-214">Siga la guía de asignación de campos y, si es necesario, realice los cambios adecuados en los pasos de la potencia que automatiza los flujos.</span><span class="sxs-lookup"><span data-stu-id="23652-214">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="23652-215">Se proporcionan las asignaciones de Microsoft Partner Center a CRM, pero en función de su entorno de CRM, puede optar por personalizar aún más los campos.</span><span class="sxs-lookup"><span data-stu-id="23652-215">Microsoft Partner Centers to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="23652-216">Se pueden personalizar varios pasos de cada uno de los flujos de potencia automatizados en función de sus necesidades.</span><span class="sxs-lookup"><span data-stu-id="23652-216">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="23652-217">Estos son algunos ejemplos de las personalizaciones disponibles:</span><span class="sxs-lookup"><span data-stu-id="23652-217">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="23652-218">Para personalizar los campos de los eventos de creación o actualización en el centro de partners para la sincronización de referencias de CRM:</span><span class="sxs-lookup"><span data-stu-id="23652-218">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="23652-219">a.</span><span class="sxs-lookup"><span data-stu-id="23652-219">a.</span></span> <span data-ttu-id="23652-220">Seleccione centro de partners para Dynamics 365 (versión preliminar de Insider) o centro de partners a Salesforce (versión preliminar de Insider).</span><span class="sxs-lookup"><span data-stu-id="23652-220">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="23652-221">b.</span><span class="sxs-lookup"><span data-stu-id="23652-221">b.</span></span> <span data-ttu-id="23652-222">Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="23652-222">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="23652-223">c.</span><span class="sxs-lookup"><span data-stu-id="23652-223">c.</span></span> <span data-ttu-id="23652-224">Seleccione **(ámbito) sincronizar el cliente potencial o la oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="23652-224">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="23652-225">Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para crear eventos, seleccione si se trata de una **nueva oportunidad compartida y, a continuación**, haga clic en.</span><span class="sxs-lookup"><span data-stu-id="23652-225">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="23652-226">Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda **crear una nueva oportunidad en CRM**.</span><span class="sxs-lookup"><span data-stu-id="23652-226">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="23652-227">Puede editar las asignaciones en esta sección mediante la guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="23652-227">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="23652-228">d.</span><span class="sxs-lookup"><span data-stu-id="23652-228">d.</span></span> <span data-ttu-id="23652-229">Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para los eventos de actualización, haga clic en el paso "(ámbito) sincronizar el cliente potencial o la oportunidad".</span><span class="sxs-lookup"><span data-stu-id="23652-229">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="23652-230">e.</span><span class="sxs-lookup"><span data-stu-id="23652-230">e.</span></span> <span data-ttu-id="23652-231">Seleccione **si se trata de una actualización de una oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="23652-231">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="23652-232">Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda **si la diferencia entre los objetos de oportunidad del centro de Partners y CRM**.</span><span class="sxs-lookup"><span data-stu-id="23652-232">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="23652-233">f.</span><span class="sxs-lookup"><span data-stu-id="23652-233">f.</span></span> <span data-ttu-id="23652-234">Seleccione **si sí** seguido de **Actualizar oportunidad existente** .</span><span class="sxs-lookup"><span data-stu-id="23652-234">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="23652-235">Para personalizar los campos de la sincronización de referencia de CRM a equipo para eventos de actualización:</span><span class="sxs-lookup"><span data-stu-id="23652-235">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="23652-236">a.</span><span class="sxs-lookup"><span data-stu-id="23652-236">a.</span></span> <span data-ttu-id="23652-237">Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="23652-237">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="23652-238">b.</span><span class="sxs-lookup"><span data-stu-id="23652-238">b.</span></span> <span data-ttu-id="23652-239">Seleccione **(ámbito) sincronizar la oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="23652-239">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="23652-240">c.</span><span class="sxs-lookup"><span data-stu-id="23652-240">c.</span></span> <span data-ttu-id="23652-241">Para personalizar las asignaciones de campos de CRM para los eventos de actualización, seleccione **si hay diferencias entre los objetos de cliente potencial del centro de Partners y CRM y, a continuación, haga clic en**.</span><span class="sxs-lookup"><span data-stu-id="23652-241">To customize CRM field mappings for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="23652-242">d.</span><span class="sxs-lookup"><span data-stu-id="23652-242">d.</span></span> <span data-ttu-id="23652-243">Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda el paso **actualizar una referencia con los datos de oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="23652-243">Select the sub-step **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="23652-244">Puede editar las asignaciones en esta sección basándose en la guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="23652-244">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="23652-245">Para personalizar los campos de la sincronización de referencia de CRM a equipo para crear eventos</span><span class="sxs-lookup"><span data-stu-id="23652-245">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="23652-246">a.</span><span class="sxs-lookup"><span data-stu-id="23652-246">a.</span></span> <span data-ttu-id="23652-247">Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="23652-247">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="23652-248">b.</span><span class="sxs-lookup"><span data-stu-id="23652-248">b.</span></span> <span data-ttu-id="23652-249">Seleccione **(ámbito) sincronizar referencias.**</span><span class="sxs-lookup"><span data-stu-id="23652-249">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="23652-250">c.</span><span class="sxs-lookup"><span data-stu-id="23652-250">c.</span></span> <span data-ttu-id="23652-251">Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para crear eventos, seleccione **crear referencia de Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="23652-251">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="23652-252">Puede editar las asignaciones en esta sección basándose en la guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="23652-252">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="23652-253">Sincronización de referencia de venta conjunta bidireccional de un extremo a otro</span><span class="sxs-lookup"><span data-stu-id="23652-253">End-to-end bi-directional co-sell referral synchronization</span></span>

<span data-ttu-id="23652-254">Una vez que haya instalado, configurado y personalizado la solución Power Automate, puede probar la sincronización de referencias de venta conjunta entre Dynamics 365 y el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="23652-254">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="23652-255">Requisitos previos</span><span class="sxs-lookup"><span data-stu-id="23652-255">Pre-requisites</span></span>

<span data-ttu-id="23652-256">Para sincronizar las referencias entre el centro de Partners y Dynamics 365 CRM, la solución Power Automate marca claramente los campos de referencia específicos de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="23652-256">To synchronize the referrals across Partner Center and Dynamics 365 CRM, the Power Automate solution clearly demarcates Microsoft-specific referral fields.</span></span> <span data-ttu-id="23652-257">Esta identificación proporciona a los equipos de vendedores la capacidad de decidir qué referencias desean compartir con Microsoft para la venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="23652-257">This identification gives your seller teams  the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="23652-258">Un conjunto de campos personalizados está disponible como parte de la entidad de **oportunidad** .</span><span class="sxs-lookup"><span data-stu-id="23652-258">A set of custom fields is available as part of the **Opportunity** entity.</span></span> <span data-ttu-id="23652-259">Un usuario administrador de CRM tendrá que crear una sección de CRM independiente con los campos personalizados de la **oportunidad** .</span><span class="sxs-lookup"><span data-stu-id="23652-259">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="23652-260">Los siguientes campos personalizados deben formar parte de la sección CRM:</span><span class="sxs-lookup"><span data-stu-id="23652-260">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="23652-261">**Sincronizar con el centro de Partners**: si se va a sincronizar la oportunidad con el centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="23652-261">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="23652-262">**Identificador de referencia**: un campo de identificador de solo lectura para la referencia del centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="23652-262">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="23652-263">**Vínculo de referencia**: un vínculo de solo lectura a la referencia en el centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="23652-263">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="23652-264">**¿Cómo puede ayudarle Microsoft?**: ayuda necesaria de Microsoft para la referencia</span><span class="sxs-lookup"><span data-stu-id="23652-264">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="23652-265">**Productos**: lista de productos asociados a esta oportunidad</span><span class="sxs-lookup"><span data-stu-id="23652-265">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="23652-266">**Audit**: una pista de auditoría de solo lectura para la sincronización con las referencias del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="23652-266">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>


### <a name="scenarios"></a><span data-ttu-id="23652-267">SITUACIÓN</span><span class="sxs-lookup"><span data-stu-id="23652-267">SCENARIOS:</span></span>

1. <span data-ttu-id="23652-268">Sincronización de referencia cuando se crea o actualiza una referencia en CRM y se sincroniza en el centro de Partners:</span><span class="sxs-lookup"><span data-stu-id="23652-268">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="23652-269">a.</span><span class="sxs-lookup"><span data-stu-id="23652-269">a.</span></span> <span data-ttu-id="23652-270">Inicie sesión en el entorno de CRM de Dynamics 365 con un usuario que tenga visibilidad en la sección de **oportunidades** de CRM.</span><span class="sxs-lookup"><span data-stu-id="23652-270">Sign into your Dynamics 365 CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="23652-271">b.</span><span class="sxs-lookup"><span data-stu-id="23652-271">b.</span></span> <span data-ttu-id="23652-272">Asegúrese de que la siguiente sección está presente al crear una "nueva oportunidad" en el entorno de Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="23652-272">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   ![Oportunidad](images/cosellconnectors/opportunity.png)

    <span data-ttu-id="23652-274">c.</span><span class="sxs-lookup"><span data-stu-id="23652-274">c.</span></span> <span data-ttu-id="23652-275">Para sincronizar esta oportunidad con el centro de Partners de Microsoft, asegúrese de establecer los siguientes campos en la vista tarjeta:</span><span class="sxs-lookup"><span data-stu-id="23652-275">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="23652-276">**Sincronizar con el centro de Partners**: sí</span><span class="sxs-lookup"><span data-stu-id="23652-276">**Sync with Partner Center**: Yes</span></span>

    - <span data-ttu-id="23652-277">**¿Cómo puede ayudarle Microsoft?**: Seleccione una de las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="23652-277">**How can Microsoft help?**: Select from the following:</span></span>

    ![Selecciones de la ayuda](images/cosellconnectors/help.png)

    - <span data-ttu-id="23652-279">**Productos**: identificadores de la solución del producto</span><span class="sxs-lookup"><span data-stu-id="23652-279">**Products**: Solution IDs of the product</span></span>

    <span data-ttu-id="23652-280">d.</span><span class="sxs-lookup"><span data-stu-id="23652-280">d.</span></span> <span data-ttu-id="23652-281">Una vez creada la oportunidad en Dynamics 365 con la opción **sincronizar con el centro de Partners** establecida en **sí**, espere 10 minutos y, a continuación, inicie sesión en su cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="23652-281">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, and then sign into your Partner Center account.</span></span> <span data-ttu-id="23652-282">Las referencias se sincronizarán con Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="23652-282">Your referrals will be synchronized with Dynamics 365.</span></span>

    <span data-ttu-id="23652-283">e.</span><span class="sxs-lookup"><span data-stu-id="23652-283">e.</span></span> <span data-ttu-id="23652-284">Del mismo modo, para una oportunidad que tuviera la opción "sincronizar con el centro de Partners" establecida en "sí", si actualizas la oportunidad en Dynamics 365 CRM, los cambios se sincronizarán en la cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="23652-284">Likewise, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    <span data-ttu-id="23652-285">f.</span><span class="sxs-lookup"><span data-stu-id="23652-285">f.</span></span> <span data-ttu-id="23652-286">Las oportunidades que se sincronizan correctamente con el centro de Partners se identificarán con ✔ icono en Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="23652-286">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="23652-287">Sincronización de referencia cuando se crea o actualiza una referencia en el centro de Partners de Microsoft y se sincroniza en el entorno de Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="23652-287">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span>

    <span data-ttu-id="23652-288">a.</span><span class="sxs-lookup"><span data-stu-id="23652-288">a.</span></span> <span data-ttu-id="23652-289">Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard/home)del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="23652-289">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="23652-290">b.</span><span class="sxs-lookup"><span data-stu-id="23652-290">b.</span></span> <span data-ttu-id="23652-291">Seleccione **referencias** en el menú de la izquierda.</span><span class="sxs-lookup"><span data-stu-id="23652-291">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="23652-292">c.</span><span class="sxs-lookup"><span data-stu-id="23652-292">c.</span></span> <span data-ttu-id="23652-293">Cree una nueva referencia de venta conjunta desde el centro de partners; para ello, haga clic en la opción "nuevo trato".</span><span class="sxs-lookup"><span data-stu-id="23652-293">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="23652-294">d.</span><span class="sxs-lookup"><span data-stu-id="23652-294">d.</span></span> <span data-ttu-id="23652-295">Inicie sesión en el entorno de CRM de Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="23652-295">Sign into your Dynamics 365 CRM environment.</span></span> 

    <span data-ttu-id="23652-296">e.</span><span class="sxs-lookup"><span data-stu-id="23652-296">e.</span></span> <span data-ttu-id="23652-297">Vaya a **abrir oportunidades**.</span><span class="sxs-lookup"><span data-stu-id="23652-297">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="23652-298">La referencia creada en el centro de Partners de Microsoft ya está sincronizada en Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="23652-298">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

    <span data-ttu-id="23652-299">f.</span><span class="sxs-lookup"><span data-stu-id="23652-299">f.</span></span> <span data-ttu-id="23652-300">Al seleccionar una referencia sincronizada, se rellenan los detalles de la vista de tarjeta.</span><span class="sxs-lookup"><span data-stu-id="23652-300">When you select a synchronized referral, the card view details are populated.</span></span>

## <a name="next-steps"></a><span data-ttu-id="23652-301">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="23652-301">Next steps</span></span>

- [<span data-ttu-id="23652-302">Administrar los clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="23652-302">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="23652-303">Administrar las oportunidades de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="23652-303">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

- [<span data-ttu-id="23652-304">¿Más información sobre la plataforma Microsoft Power Automate?</span><span class="sxs-lookup"><span data-stu-id="23652-304">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="23652-305">Webhooks del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="23652-305">Partner Center webhooks</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhooks)