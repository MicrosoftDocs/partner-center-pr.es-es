---
title: El conector de venta conjunta para el centro de Partners de Dynamics 365 CRM
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usar el conector de Dynamics 365, obtener referencias de Microsoft
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: bddd29e9136d998ef8a25616d2058d1380b36665
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825692"
---
# <a name="co-sell-connector-for-dynamics-365-crm--overview"></a><span data-ttu-id="23050-103">Conector de venta conjunta para Dynamics 365 CRM: información general</span><span class="sxs-lookup"><span data-stu-id="23050-103">Co-sell connector for Dynamics 365 CRM – Overview</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="23050-104">Roles adecuados</span><span class="sxs-lookup"><span data-stu-id="23050-104">Appropriate roles</span></span>

- <span data-ttu-id="23050-105">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="23050-105">Referrals admin</span></span>
- <span data-ttu-id="23050-106">Administrador del sistema o Personalizador del sistema en CRM</span><span class="sxs-lookup"><span data-stu-id="23050-106">System admin or system customizer on the CRM</span></span>

<span data-ttu-id="23050-107">El conector de la venta conjunta del centro de Partners permite que los vendedores covendan con Microsoft desde los sistemas CRM.</span><span class="sxs-lookup"><span data-stu-id="23050-107">Partner Center co-sell connector enables your sellers to co-sell with Microsoft from within your CRM systems.</span></span> <span data-ttu-id="23050-108">No tendrán que estar capacitados para utilizar el centro de partners para administrar las ofertas de venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="23050-108">They won’t have to be trained to use Partner Center to manage Co-sell deals.</span></span> <span data-ttu-id="23050-109">Mediante el uso de conectores de venta conjunta, podrá crear una nueva referencia de venta conjunta para invitar a un vendedor de Microsoft, recibir referencias del vendedor de Microsoft, aceptar o rechazar las referencias, modificar los datos de los acuerdos, como el valor del negocio, la fecha de cierre, etc., así como recibir las actualizaciones de los vendedores de Microsoft en relación con la venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="23050-109">Using the Co-sell connectors, you will be able to create a new Co-sell referral to engage a Microsoft seller, receive referrals from the Microsoft seller, accept/decline referrals, modify deal data such as deal value, closing date etc. as well as receive any updates from the Microsoft sellers on these Co-sell deals.</span></span> <span data-ttu-id="23050-110">Puede hacer todo esto mientras trabaja en el CRM de su elección en lugar de hacerlo en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="23050-110">You can do all of this while working within the CRM of your choice rather than in Partner Center.</span></span> 

<span data-ttu-id="23050-111">La solución se basa en la solución Microsoft Power Automate y usa las API del centro de Partners de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="23050-111">The solution is based on Microsoft Power Automate Solution and uses Microsoft Partner Center APIs.</span></span>

## <a name="before-you-install---pre-requisites"></a><span data-ttu-id="23050-112">Antes de instalar: requisitos previos</span><span class="sxs-lookup"><span data-stu-id="23050-112">Before you install - pre-requisites</span></span>

|<span data-ttu-id="23050-113">**Temas**</span><span class="sxs-lookup"><span data-stu-id="23050-113">**Topics**</span></span>   |<span data-ttu-id="23050-114">**Detalles**</span><span class="sxs-lookup"><span data-stu-id="23050-114">**Details**</span></span>   |<span data-ttu-id="23050-115">**Vínculos**</span><span class="sxs-lookup"><span data-stu-id="23050-115">**Links**</span></span>   |
|--------------|--------------------|------|
|<span data-ttu-id="23050-116">IDENTIFICADOR de Microsoft Partner Network</span><span class="sxs-lookup"><span data-stu-id="23050-116">Microsoft Partner Network ID</span></span> |<span data-ttu-id="23050-117">Necesita un ID. de MPN válido</span><span class="sxs-lookup"><span data-stu-id="23050-117">You need a valid MPN ID</span></span>|<span data-ttu-id="23050-118">Para unirse a [MPN](https://partner.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="23050-118">To join [MPN](https://partner.microsoft.com/)</span></span>|
|<span data-ttu-id="23050-119">Venta conjunta lista</span><span class="sxs-lookup"><span data-stu-id="23050-119">Co-sell ready</span></span>|<span data-ttu-id="23050-120">La solución de IP/servicios debe estar lista para su venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="23050-120">Your IP/Services solution must be co-sell ready.</span></span>|[<span data-ttu-id="23050-121">Venda con Microsoft</span><span class="sxs-lookup"><span data-stu-id="23050-121">Sell with Microsoft</span></span>](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|<span data-ttu-id="23050-122">Cuenta del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="23050-122">Partner Center account</span></span>|<span data-ttu-id="23050-123">El identificador de MPN asociado al inquilino del centro de Partners debe ser el mismo que el identificador de MPN asociado a la solución de venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="23050-123">The MPN ID associated with the Partner Center tenant must be same as the MPN ID associated with your Co-sell solution.</span></span> <span data-ttu-id="23050-124">Compruebe que puede ver las referencias de venta conjunta en el portal del centro de Partners antes de implementar los conectores.</span><span class="sxs-lookup"><span data-stu-id="23050-124">Verify that you can see your co-sell referrals in Partner Center portal prior to deploying the connectors.</span></span>|[<span data-ttu-id="23050-125">Administración de la cuenta</span><span class="sxs-lookup"><span data-stu-id="23050-125">Manage your account</span></span>](create-user-accounts-and-set-permissions.md)|
|<span data-ttu-id="23050-126">Roles de usuario del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="23050-126">Partner Center user roles</span></span>|<span data-ttu-id="23050-127">El empleado que va a instalar y usar los conectores debe ser un administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="23050-127">The employee who will install and use the connectors must be a Referrals admin</span></span>|[<span data-ttu-id="23050-128">Asignar roles y permisos de usuarios</span><span class="sxs-lookup"><span data-stu-id="23050-128">Assign users roles and permissions</span></span>](create-user-accounts-and-set-permissions.md)| |<span data-ttu-id="23050-129">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="23050-129">Dynamics 365 CRM</span></span>|<span data-ttu-id="23050-130">El rol de usuario CRM es administrador del sistema o Personalizador del sistema</span><span class="sxs-lookup"><span data-stu-id="23050-130">The CRM user role is System admin or System customizer</span></span>|[<span data-ttu-id="23050-131">Asignación de roles en Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="23050-131">Assign roles in Dynamics 365</span></span>](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|<span data-ttu-id="23050-132">Cuenta de flujo de automatización de energía</span><span class="sxs-lookup"><span data-stu-id="23050-132">Power Automate Flow Account</span></span>|<span data-ttu-id="23050-133">Una cuenta activa de [Power Automatic](https://flow.microsoft.com) para el administrador del sistema CRM o el personalizador del sistema.</span><span class="sxs-lookup"><span data-stu-id="23050-133">An active [Power Automate](https://flow.microsoft.com) account for the CRM System admin or System customizer.</span></span> <span data-ttu-id="23050-134">Dicho usuario debe iniciar sesión en [Power automatizate](https://flow.microsoft.com) al menos una vez antes de la instalación.</span><span class="sxs-lookup"><span data-stu-id="23050-134">That user should sign into [Power Automate](https://flow.microsoft.com) at least once before installation.</span></span>|

## <a name="install-partner-center-referrals-synchronization-for-dynamics-365-power-automate-solution"></a><span data-ttu-id="23050-135">Instalación de la sincronización de referencias del centro de partners para Dynamics 365 (solución de automatización de energía)</span><span class="sxs-lookup"><span data-stu-id="23050-135">Install Partner Center Referrals Synchronization for Dynamics 365 (Power Automate Solution)</span></span> 

1. <span data-ttu-id="23050-136">Vaya a [Power Automatic](https://flow.microsoft.com) y seleccione **entornos** en la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="23050-136">Go to [Power Automate](https://flow.microsoft.com) and select **Environments** on the right top corner.</span></span> <span data-ttu-id="23050-137">Se mostrarán las instancias de CRM disponibles.</span><span class="sxs-lookup"><span data-stu-id="23050-137">This will show you the available CRM instances.</span></span>

2. <span data-ttu-id="23050-138">Seleccione la instancia de CRM correspondiente en la lista desplegable de la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="23050-138">Select the appropriate CRM instance from the drop-down on the right top corner.</span></span> 

3. <span data-ttu-id="23050-139">Seleccione **soluciones** en la barra de navegación izquierda.</span><span class="sxs-lookup"><span data-stu-id="23050-139">Select **Solutions** on the left navigation bar.</span></span>

4. <span data-ttu-id="23050-140">Haga clic en el vínculo **abrir AppSource** en el menú superior.</span><span class="sxs-lookup"><span data-stu-id="23050-140">Click on the **Open AppSource** link on the top menu.</span></span>

![Abrir AppSource](images/cosellconnectors/openappsource.png)

5. <span data-ttu-id="23050-142">Busque **conectores de referencias del centro de partners para Dynamics365** en la pantalla emergente.</span><span class="sxs-lookup"><span data-stu-id="23050-142">Search for **Partner Center Referrals Connectors for Dynamics365** in the pop-up screen.</span></span>  

6. <span data-ttu-id="23050-143">Haga clic en el botón **obtener ahora** y **continúe**.</span><span class="sxs-lookup"><span data-stu-id="23050-143">Click the **Get it now** button and then **Continue**.</span></span> 

7. <span data-ttu-id="23050-144">Se abrirá la página en la que puede seleccionar el entorno de CRM (Dynamics 365) para instalar la aplicación.</span><span class="sxs-lookup"><span data-stu-id="23050-144">This opens the page where you can select the CRM (Dynamics 365) environment to install application.</span></span>  <span data-ttu-id="23050-145">Acepte los términos y condiciones.</span><span class="sxs-lookup"><span data-stu-id="23050-145">Agree to terms and conditions.</span></span> 

8. <span data-ttu-id="23050-146">A continuación, se le dirigirá a la página **administrar soluciones** .</span><span class="sxs-lookup"><span data-stu-id="23050-146">You are then directed to the **Manage your solutions** page.</span></span>  <span data-ttu-id="23050-147">Vaya a "referencias del centro de Partners" con los botones de flecha de la parte inferior de la página.</span><span class="sxs-lookup"><span data-stu-id="23050-147">Navigate to "Partner Center Referrals" by using the arrow buttons on the bottom of the page.</span></span> <span data-ttu-id="23050-148">La **instalación programada** debe aparecer junto a la solución de referencias del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="23050-148">**Installation scheduled** should appear next to Partner Center Referrals solution.</span></span> <span data-ttu-id="23050-149">La instalación tardará 10-15 minutos.</span><span class="sxs-lookup"><span data-stu-id="23050-149">Installation will take 10-15 minutes.</span></span> 

9. <span data-ttu-id="23050-150">Una vez completada la instalación, vuelva a [Power Automatic](https://flow.microsoft.com) y seleccione **soluciones** en el área de navegación izquierda.</span><span class="sxs-lookup"><span data-stu-id="23050-150">Once the installation is complete, navigate back to [Power Automate](https://flow.microsoft.com) and select **Solutions** from left navigation area.</span></span> <span data-ttu-id="23050-151">Observe que la **sincronización de las referencias del centro de partners para Dynamics 365** está disponible en la lista de soluciones.</span><span class="sxs-lookup"><span data-stu-id="23050-151">Notice that **Partner Center Referrals Synchronization for Dynamics 365** is available in the Solutions list.</span></span>

10. <span data-ttu-id="23050-152">Seleccione la **sincronización de referencias del centro de partners para Dynamics 365**.</span><span class="sxs-lookup"><span data-stu-id="23050-152">Select **Partner Center Referrals Synchronization for Dynamics 365**.</span></span> <span data-ttu-id="23050-153">Están disponibles los siguientes flujos y entidades:</span><span class="sxs-lookup"><span data-stu-id="23050-153">The following Power Automate flows and entities are available:</span></span>

![CRMS disponibles](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a><span data-ttu-id="23050-155">Procedimiento recomendado: prueba antes de la marcha</span><span class="sxs-lookup"><span data-stu-id="23050-155">Best Practice: Test before you go live</span></span>

<span data-ttu-id="23050-156">Antes de instalar, configurar y personalizar la solución Power Automate en el entorno de producción, asegúrese de probar la solución en una instancia de CRM provisional.</span><span class="sxs-lookup"><span data-stu-id="23050-156">Before you install, configure, and customize the Power Automate solution on the production environment, be sure to test the solution on a staging CRM instance.</span></span>

- <span data-ttu-id="23050-157">Instale la solución Microsoft Power Automate en un entorno de ensayo o una instancia de CRM.</span><span class="sxs-lookup"><span data-stu-id="23050-157">Install Microsoft Power Automate solution on a staging environment/CRM instance.</span></span>
- <span data-ttu-id="23050-158">Realice una copia de la solución y realice la configuración y las personalizaciones de flujo de automatización en el entorno de ensayo.</span><span class="sxs-lookup"><span data-stu-id="23050-158">Make a copy of the solution and perform your configuration and Power Automate flow customizations on the staging environment.</span></span>
- <span data-ttu-id="23050-159">Pruebe la solución en una instancia de ensayo o CRM.</span><span class="sxs-lookup"><span data-stu-id="23050-159">Test the solution on a staging/CRM instance.</span></span> 
- <span data-ttu-id="23050-160">En caso de éxito, importe como solución administrada a la instancia de producción.</span><span class="sxs-lookup"><span data-stu-id="23050-160">On success, import as managed solution to the production instance.</span></span> 

## <a name="configure-the-solution"></a><span data-ttu-id="23050-161">Configuración de la solución</span><span class="sxs-lookup"><span data-stu-id="23050-161">Configure the solution</span></span>

1. <span data-ttu-id="23050-162">Una vez que haya instalado la solución en la instancia de CRM, vuelva a [Power Automatic](https://flow.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="23050-162">Once you have installed the solution in your CRM instance, navigate back to [Power Automate](https://flow.microsoft.com/).</span></span>

2. <span data-ttu-id="23050-163">En la lista desplegable de **entornos** de la esquina superior derecha, seleccione la instancia de CRM en la que instaló la solución Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="23050-163">From the **Environments** drop-down on the right top corner, select the CRM instance where you installed the Power Automate solution.</span></span>

3. <span data-ttu-id="23050-164">Tendrá que crear conexiones que asocien las tres cuentas de usuario:</span><span class="sxs-lookup"><span data-stu-id="23050-164">You will need to create connections that associate the three user accounts:</span></span> 

- <span data-ttu-id="23050-165">Usuario del centro de Partners con credenciales de administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="23050-165">Partner Center user with referrals admin credentials</span></span> 
- <span data-ttu-id="23050-166">Eventos del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="23050-166">Partner Center Events</span></span>
- <span data-ttu-id="23050-167">Administrador de CRM con la potencia que automatiza los flujos en la solución.</span><span class="sxs-lookup"><span data-stu-id="23050-167">CRM admin with the Power Automate flows in the solution.</span></span> 

    <span data-ttu-id="23050-168">a.</span><span class="sxs-lookup"><span data-stu-id="23050-168">a.</span></span> <span data-ttu-id="23050-169">Seleccione **conexiones** en la barra de navegación izquierda y seleccione la solución "referencias del centro de Partners" en la lista.</span><span class="sxs-lookup"><span data-stu-id="23050-169">Select **Connections** from the left navigation bar and select the “Partner Center Referrals” solution from the list.</span></span>
    <span data-ttu-id="23050-170">b.</span><span class="sxs-lookup"><span data-stu-id="23050-170">b.</span></span> <span data-ttu-id="23050-171">Cree una conexión haciendo clic en **crear una conexión**.</span><span class="sxs-lookup"><span data-stu-id="23050-171">Create a connection by clicking **Create a connection**.</span></span> 

    ![Crear conexión](images/cosellconnectors/createconnection.png)
    
    <span data-ttu-id="23050-173">c.</span><span class="sxs-lookup"><span data-stu-id="23050-173">c.</span></span> <span data-ttu-id="23050-174">Busque **referencias del centro de Partners (versión preliminar)** en la barra de búsqueda de la esquina superior derecha.</span><span class="sxs-lookup"><span data-stu-id="23050-174">Search for **Partner Center Referrals (preview)** in the search bar on the top right corner.</span></span>
    <span data-ttu-id="23050-175">d.</span><span class="sxs-lookup"><span data-stu-id="23050-175">d.</span></span> <span data-ttu-id="23050-176">Cree una conexión para el usuario del centro de Partners con el rol de credenciales de administrador de referencias. e:..</span><span class="sxs-lookup"><span data-stu-id="23050-176">Create a connection for your Partner Center user with the credentials role of Referrals admin. e.</span></span> <span data-ttu-id="23050-177">A continuación, cree una conexión de eventos del centro de partners para el usuario del centro de Partners con las credenciales de administrador de referencias. formato.</span><span class="sxs-lookup"><span data-stu-id="23050-177">Next, create a Partner Center Events connection for your Partner Center user with the credentials of Referrals admin. f.</span></span> <span data-ttu-id="23050-178">Cree una conexión para Common Data Service (entorno actual) para el usuario administrador de CRM.</span><span class="sxs-lookup"><span data-stu-id="23050-178">Create a connection for Common Data Service (current environment) for the CRM administrator user.</span></span>

4. <span data-ttu-id="23050-179">Para asociar los flujos de alimentación automatizada con las conexiones, edite cada uno de los flujos de Power Automatic para conectarse a Common Data Service y a las referencias del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="23050-179">To associate the Power Automate flows with the connections, edit each of the Power Automate flows to connect to Common Data Service and Partner Center Referrals.</span></span> <span data-ttu-id="23050-180">Guarde los cambios.</span><span class="sxs-lookup"><span data-stu-id="23050-180">Save the changes.</span></span>

5. <span data-ttu-id="23050-181">**Encienda** los flujos automatizar energía.</span><span class="sxs-lookup"><span data-stu-id="23050-181">**Turn on** the the Power Automate flows.</span></span>

## <a name="next-steps"></a><span data-ttu-id="23050-182">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="23050-182">Next steps</span></span>

- [<span data-ttu-id="23050-183">Uso de webhooks para obtener eventos de cambio de recursos</span><span class="sxs-lookup"><span data-stu-id="23050-183">Use Webhooks to get resource change events</span></span>](referral-connector-webhooks.md)

- [<span data-ttu-id="23050-184">¿Más información sobre la plataforma Microsoft Power Automate?</span><span class="sxs-lookup"><span data-stu-id="23050-184">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="23050-185">Administrar los clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="23050-185">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="23050-186">Administrar las oportunidades de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="23050-186">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)

