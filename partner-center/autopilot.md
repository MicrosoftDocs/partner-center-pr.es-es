---
title: Personalizar la experiencia de out-of-box de un dispositivo con perfiles de Windows Autopilot | Centro de partners
description: Preconfigurar la experiencia de out-of-box de un dispositivo con perfiles de Autopilot.
ms.topic: article
ms.date: 03/18/19
author: maggiepuccievans
ms.author: evansma
keywords: AutoPilot, autopilot de windows, autopilot de microsoft, una implementación sin retoques, oobe, pantallas de inicio de sesión, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: e940a7ccf79f6b43d3712a2f3ae2f9b150e1473e
ms.sourcegitcommit: f5dbd07185059aa5faddf1c5daa556f634ce97ee
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2019
ms.locfileid: "58162225"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="cf0c3-104">Personalizar la experiencia de out-of-box de un dispositivo con perfiles de Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="cf0c3-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

<span data-ttu-id="cf0c3-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="cf0c3-105">**Applies to**</span></span>

- <span data-ttu-id="cf0c3-106">Asociados de CSP directo factura, los proveedores indirectos y revendedores indirectos</span><span class="sxs-lookup"><span data-stu-id="cf0c3-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="cf0c3-107">Si administra dispositivos de cliente, deberá personalizar la experiencia de out-of-box (OOBE) para los usuarios del cliente.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="cf0c3-108">Puede configurar previamente los nuevos dispositivos con perfiles de Windows Autopilot antes de entregar los dispositivos a los clientes y aplicar nuevos perfiles para dispositivos clientes ya han adquirido.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="cf0c3-109">En este artículo se explica cómo crear y aplicar los perfiles de Autopilot en dispositivos de centro de partners.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="cf0c3-110">Si no ya está familiarizado con el piloto automático, revise la información en estos artículos:</span><span class="sxs-lookup"><span data-stu-id="cf0c3-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="cf0c3-111">Información general de Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="cf0c3-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="cf0c3-112">Guía de referencia de implementación de AutoPilot</span><span class="sxs-lookup"><span data-stu-id="cf0c3-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="cf0c3-113">Información general</span><span class="sxs-lookup"><span data-stu-id="cf0c3-113">Overview</span></span>

<span data-ttu-id="cf0c3-114">Con la característica de Windows Autopilot en Centro de partners, puede crear perfiles personalizados para aplicar a los dispositivos cliente.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="cf0c3-115">La siguiente configuración del perfil estaba disponible en el momento en que se publicó este artículo:</span><span class="sxs-lookup"><span data-stu-id="cf0c3-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="cf0c3-116">Omitir la configuración de privacidad.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-116">Skip privacy settings.</span></span> <span data-ttu-id="cf0c3-117">Esta configuración de perfil de Autopilot opcional permite a las organizaciones no preguntar sobre la configuración de privacidad durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="cf0c3-118">Deshabilitar la creación de la cuenta de administrador local en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="cf0c3-119">Las organizaciones pueden decidir si el usuario configura el dispositivo debe tener acceso de administrador, una vez completado el proceso.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="cf0c3-120">Configurar automáticamente dispositivos de empresa o centro educativo.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="cf0c3-121">Todos los dispositivos registrados con Autopilot automáticamente se considerará trabajo o educativas de los dispositivos, por lo que esta pregunta no se les pedirá durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="cf0c3-122">Omitir las páginas de instalación del registro de OEM, OneDrive y Cortana.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="cf0c3-123">Todos los dispositivos registrados con Autopilot omitirá automáticamente estas páginas durante el proceso de configuración de-rápida (OOBE).</span><span class="sxs-lookup"><span data-stu-id="cf0c3-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="cf0c3-124">Omitir el contrato de licencia de usuario final (CLUF).</span><span class="sxs-lookup"><span data-stu-id="cf0c3-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="cf0c3-125">A partir de Windows 10 versión 1709, las organizaciones pueden decidir omitir la página del CLUF presentada durante el proceso OOBE.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="cf0c3-126">Consulte [despido de términos de licencia de Windows Autopilot](#windows-autopilot-eula-dismissal) a continuación para que obtener información importante a tener en cuenta acerca de la omisión de la página del CLUF Windows durante la instalación.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="cf0c3-127">Se aplican los siguientes permisos de administración de perfil y el dispositivo y limitaciones:</span><span class="sxs-lookup"><span data-stu-id="cf0c3-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="cf0c3-128">Los asociados de CSP pueden seguir administrar perfiles de Autopilot para los clientes existentes con los que tienen relaciones de distribuidor, incluso si los clientes han quitado privilegios de administración delegada del asociado.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="cf0c3-129">Puede administrar los dispositivos existentes para los clientes que se han agregado.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-129">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="cf0c3-130">No puede administrar dispositivos de que su cliente ha cargado en Microsoft Store para empresas o el Portal de Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="cf0c3-131">Crear y administrar perfiles de Autopilot en Centro de partners</span><span class="sxs-lookup"><span data-stu-id="cf0c3-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="cf0c3-132">En el centro de partners, puede crear perfiles de Windows Autopilot deployment y aplicarlas a los dispositivos.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="cf0c3-133">Solo los agentes de administración pueden crear y aplicar los perfiles.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="cf0c3-134">Crear un nuevo perfil de Autopilot</span><span class="sxs-lookup"><span data-stu-id="cf0c3-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="cf0c3-135">Seleccione **clientes** desde el menú de centro de partners y, a continuación, seleccione el cliente que está creando el perfil de Autopilot para.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="cf0c3-136">En la página de detalles del cliente, seleccione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="cf0c3-137">En **perfiles de Windows Autopilot** seleccione **Agregar nuevo perfil**.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="cf0c3-138">Escriba el nombre y una descripción del perfil y, a continuación, configure las opciones de bienvenida de Windows.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="cf0c3-139">Elegir entre:</span><span class="sxs-lookup"><span data-stu-id="cf0c3-139">Choose from:</span></span>  

   - <span data-ttu-id="cf0c3-140">Omitir la configuración de privacidad en el programa de instalación</span><span class="sxs-lookup"><span data-stu-id="cf0c3-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="cf0c3-141">Deshabilitar la cuenta de administrador local en el programa de instalación</span><span class="sxs-lookup"><span data-stu-id="cf0c3-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="cf0c3-142">Omitir automáticamente las páginas durante la instalación</span><span class="sxs-lookup"><span data-stu-id="cf0c3-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="cf0c3-143">(Incluye *seleccionar automáticamente la configuración para el trabajo o escuela* y *páginas de configuración de registro de OEM, OneDrive y Skip Cortana*)</span><span class="sxs-lookup"><span data-stu-id="cf0c3-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="cf0c3-144">Omitir el contrato de licencia de usuario final (CLUF)</span><span class="sxs-lookup"><span data-stu-id="cf0c3-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="cf0c3-145">Consulte [despido de términos de licencia de Windows Autopilot](#windows-autopilot-eula-dismissal) a continuación para que obtener información importante a tener en cuenta acerca de la omisión de la página del CLUF Windows durante la instalación.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="cf0c3-146">Selecciona **Enviar** cuando hayas acabado.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="cf0c3-147">Un perfil de Autopilot se aplican a dispositivos de cliente</span><span class="sxs-lookup"><span data-stu-id="cf0c3-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="cf0c3-148">Las instrucciones siguientes se suponen que ya ha agregado los dispositivos del cliente al centro de partners y que puede tener acceso a su lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="cf0c3-149">Si aún no ha agregado los dispositivos del cliente, siga las instrucciones de [agregar dispositivos a una cuenta de cliente](#add-devices-to-a-customers-account) y, a continuación, siga los pasos siguientes.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="cf0c3-150">Después de crear un perfil de Autopilot para un cliente, puede aplicarla a los dispositivos del cliente.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="cf0c3-151">Seleccione **clientes** desde el menú de centro de partners y, a continuación, seleccione el cliente que creó para el perfil de Autopilot.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="cf0c3-152">En la página de detalles del cliente, seleccione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="cf0c3-153">En **perfiles se aplican a dispositivos** seleccione los dispositivos o grupos de dispositivos que desea agregar a los perfiles y, a continuación, seleccione **aplicar perfil**.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="cf0c3-154">El perfil que acaba de aplicar aparece en el **perfil** columna.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="cf0c3-155">Siga los pasos siguientes para comprobar que el perfil se aplicará correctamente al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="cf0c3-156">a.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-156">a.</span></span>  <span data-ttu-id="cf0c3-157">Conectar un dispositivo a la red y enciéndalo.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="cf0c3-158">b.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-158">b.</span></span>  <span data-ttu-id="cf0c3-159">Comprueba que aparezcan las pantallas OOBE apropiadas (si es el caso).</span><span class="sxs-lookup"><span data-stu-id="cf0c3-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="cf0c3-160">c.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-160">c.</span></span>  <span data-ttu-id="cf0c3-161">Cuando se detiene el proceso OOBE, restablecer el dispositivo a la configuración predeterminada de fábrica para prepararlo para un usuario nuevo.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="cf0c3-162">Quitar un perfil de Autopilot de dispositivo del cliente</span><span class="sxs-lookup"><span data-stu-id="cf0c3-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="cf0c3-163">Seleccione **clientes** desde el menú de centro de partners y, a continuación, seleccione el cliente que creó para el perfil de Autopilot.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="cf0c3-164">En la página de detalles del cliente, seleccione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="cf0c3-165">En **perfiles se aplican a dispositivos** seleccione los dispositivos que desea quitar el perfil de y, a continuación, seleccione **quitar perfil**.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="cf0c3-166">Quitar un perfil de un dispositivo no elimina el perfil de la lista.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="cf0c3-167">Si desea eliminar un perfil, siga las instrucciones de [Update o delete de un perfil de Autopilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="cf0c3-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="cf0c3-168">Actualizar o eliminar un perfil de Autopilot</span><span class="sxs-lookup"><span data-stu-id="cf0c3-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="cf0c3-169">Si un cliente quiere cambiar la configuración rápida después de haber enviado los dispositivos que les, puede cambiar el perfil en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="cf0c3-170">Cuando el dispositivo del cliente se conecta a internet, descargará la última versión de perfil durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="cf0c3-171">Además, siempre que un cliente restaura un dispositivo a la configuración predeterminada de fábrica, el dispositivo nuevo descargará la última versión de perfil durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="cf0c3-172">Seleccione **clientes** en el menú de centro de partners y a continuación, seleccione el cliente que desea cambiar un perfil de Autopilot.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="cf0c3-173">En la página de detalles del cliente, seleccione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="cf0c3-174">En **perfiles de Windows Autopilot** seleccione el perfil que se debe actualizar.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="cf0c3-175">Realice los cambios necesarios y, a continuación, seleccione **enviar**.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="cf0c3-176">Para eliminar este perfil, seleccione **eliminar perfil** desde la esquina superior derecha de la página.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="cf0c3-177">Agregar dispositivos a una cuenta de cliente</span><span class="sxs-lookup"><span data-stu-id="cf0c3-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="cf0c3-178">Los agentes de ventas y los agentes de administración pueden agregar dispositivos a una cuenta de cliente.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="cf0c3-179">Antes de aplicar los perfiles de Autopilot personalizados a los dispositivos de cliente, debe poder tener acceso a la lista de dispositivos del cliente.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="cf0c3-180">Si tiene previsto usar el nombre, número de serie y combinación de modelos de OEM, tenga en cuenta estas limitaciones:</span><span class="sxs-lookup"><span data-stu-id="cf0c3-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="cf0c3-181">Esta tupla solo funciona para los dispositivos más recientes (4 k hashes, por ejemplo) y no es compatible con hashes de 128b (RS2 y dispositivos anteriores).</span><span class="sxs-lookup"><span data-stu-id="cf0c3-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="cf0c3-182">El registro de la tupla distingue mayúsculas de minúsculas, por lo que los datos en el archivo deben coincidir con los nombres de modelo y fabricante ***exactamente*** proporcionados por el proveedor OEM (proveedor de hardware).</span><span class="sxs-lookup"><span data-stu-id="cf0c3-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="cf0c3-183">Siga las instrucciones siguientes para agregar dispositivos a una cuenta de cliente en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="cf0c3-184">Seleccione **clientes** en el menú de centro de partners y, a continuación, seleccione el cliente cuyos dispositivos desea administrar.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="cf0c3-185">En la página de detalles del cliente, seleccione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="cf0c3-186">En **perfiles se aplican a dispositivos** seleccione **agregar dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="cf0c3-187">Escriba un nombre para la lista de dispositivos y, a continuación, seleccione **examinar** para cargar la lista del cliente (en formato de archivo .csv) al centro de partners.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="cf0c3-188">Debe haber recibido este archivo .csv con la compra de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="cf0c3-189">Si no ha recibido un archivo .csv, puede crear uno usted mismo, siga los pasos descritos en [agregar dispositivos a Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="cf0c3-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="cf0c3-190">Cargue el archivo .csv y, a continuación, seleccione **guardar**.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="cf0c3-191">Si recibe un mensaje de error al intentar cargar el archivo .csv, compruebe el formato del archivo.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="cf0c3-192">Puede usar solo, el hash del hardware o el nombre del OEM, número de serie y modelo (en ese orden de columna) o el identificador de producto de Windows.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="cf0c3-193">También puede usar el archivo .csv de ejemplo proporcionado en el vínculo junto a **agregar dispositivos** para crear una lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="cf0c3-194">Despido de términos de licencia de Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="cf0c3-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="cf0c3-195">INFORMACIÓN IMPORTANTE</span><span class="sxs-lookup"><span data-stu-id="cf0c3-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="cf0c3-196">Windows Autopilot le permite configurar instalaciones personalizadas de Windows en dispositivos administrados para sus clientes.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="cf0c3-197">Si dispone de autorización para hacerlo por el cliente, puede suprimir u ocultar determinadas pantallas de instalación que normalmente se presentan a los usuarios al configurar Windows, incluida la pantalla de aceptación de términos de licencia (contrato de licencia de usuario final).</span><span class="sxs-lookup"><span data-stu-id="cf0c3-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="cf0c3-198">Mediante el uso de esta función, acepta al suprimir u ocultación de ninguna de las pantallas que está diseñada para proporcionar a los usuarios con notificación o aceptación de significa términos que haya obtenido suficiente consentimiento y autorización de su cliente para ocultar los términos y que usted, en nombre de el cliente (si una organización o un usuario individual en su caso puede ser), da su consentimiento para los avisos y aceptar cualquiera los términos que son aplicables a su cliente.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="cf0c3-199">Esto incluye que estás de acuerdo con los términos y condiciones de la licencia o el anuncio que se presenta al usuario si no la suprimiste u ocultaste con esta herramienta.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="cf0c3-200">Tu cliente no puede usar el software de Windows en esos dispositivos si ha adquirido de manera válida una licencia para el software desde Microsoft o sus distribuidores con licencia.</span><span class="sxs-lookup"><span data-stu-id="cf0c3-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>