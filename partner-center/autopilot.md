---
title: Personalizar la experiencia out-of-box de un dispositivo con perfiles de Windows Autopilot | El centro de partners
description: Preconfigurar experiencia out-of-box de un dispositivo con perfiles Autopilot.
author: maggiepuccievans
keywords: AutoPilot, autopilot de windows, autopilot de microsoft, implementación sin interacción, oobe, pantallas de inicio de sesión, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 7df979042799954c5b43a2adef1915941db02e57
ms.sourcegitcommit: 90d656ed3a4d056a0506f7b5e2b1b8c728f58c46
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/19/2018
ms.locfileid: "8976812"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="02e97-104">Personalizar la experiencia out-of-box de un dispositivo con perfiles de Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="02e97-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

**<span data-ttu-id="02e97-105">Se aplica a</span><span class="sxs-lookup"><span data-stu-id="02e97-105">Applies to</span></span>**

- <span data-ttu-id="02e97-106">Los partners de CSP directo factura, los proveedores indirectos y distribuidores indirectos</span><span class="sxs-lookup"><span data-stu-id="02e97-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="02e97-107">Si puedes administrar dispositivos de los clientes, puede que tengas personalizar la experiencia out-of-box (OOBE) para los usuarios del cliente.</span><span class="sxs-lookup"><span data-stu-id="02e97-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="02e97-108">Puedes configurar previamente nuevos dispositivos con perfiles Autopilot de Windows antes de entregar los dispositivos a los clientes y aplicar los perfiles nuevos a los dispositivos que ya hayan comprado los clientes.</span><span class="sxs-lookup"><span data-stu-id="02e97-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="02e97-109">En este artículo se explica cómo crear y aplicar los perfiles Autopilot a los dispositivos en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="02e97-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="02e97-110">Si no ya estás familiarizado con Autopilot, revisa la información de estos artículos:</span><span class="sxs-lookup"><span data-stu-id="02e97-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="02e97-111">Introducción a WindowsAutoPilot</span><span class="sxs-lookup"><span data-stu-id="02e97-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="02e97-112">Guía de referencia de implementación de AutoPilot</span><span class="sxs-lookup"><span data-stu-id="02e97-112">Autopilot deployment reference guide</span></span>](http://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="02e97-113">Introducción</span><span class="sxs-lookup"><span data-stu-id="02e97-113">Overview</span></span>

<span data-ttu-id="02e97-114">Con la característica Windows Autopilot en el centro de partners, puedes crear perfiles personalizados para aplicar a dispositivos de los clientes.</span><span class="sxs-lookup"><span data-stu-id="02e97-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="02e97-115">La siguiente configuración de perfil estaba disponible en el momento en que se publicó este artículo:</span><span class="sxs-lookup"><span data-stu-id="02e97-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="02e97-116">Omitir la configuración de privacidad.</span><span class="sxs-lookup"><span data-stu-id="02e97-116">Skip privacy settings.</span></span> <span data-ttu-id="02e97-117">Esta opción de configuración opcional del perfil de Autopilot permite a las organizaciones preguntar sobre la configuración de privacidad durante el proceso OOBE.</span><span class="sxs-lookup"><span data-stu-id="02e97-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="02e97-118">Deshabilitar la creación de cuentas de administrador local en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="02e97-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="02e97-119">Las organizaciones pueden decidir si el usuario configura el dispositivo debe tener acceso de administrador una vez completado el proceso.</span><span class="sxs-lookup"><span data-stu-id="02e97-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="02e97-120">Configura automáticamente el dispositivo para el trabajo o escuela.</span><span class="sxs-lookup"><span data-stu-id="02e97-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="02e97-121">Todos los dispositivos registrados con Autopilot automáticamente se considerarán trabajo o colegio dispositivos, por lo que esta pregunta no se le pida durante el proceso OOBE.</span><span class="sxs-lookup"><span data-stu-id="02e97-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="02e97-122">Omitir páginas de configuración de registro de OEM, OneDrive y Cortana.</span><span class="sxs-lookup"><span data-stu-id="02e97-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="02e97-123">Todos los dispositivos registrados con Autopilot omitirán automáticamente estas páginas durante el proceso de out-of-box rápida (OOBE).</span><span class="sxs-lookup"><span data-stu-id="02e97-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="02e97-124">Omitir contrato de licencia de usuario final (CLUF).</span><span class="sxs-lookup"><span data-stu-id="02e97-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="02e97-125">A partir de Windows 10, versión 1709, las organizaciones pueden decidir omitir la página del CLUF presentada durante el proceso de configuración rápida.</span><span class="sxs-lookup"><span data-stu-id="02e97-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="02e97-126">Consulta [desestimación del CLUF de Windows Autopilot](#windows-autopilot-eula-dismissal) a continuación para obtener información importante a tener en cuenta acerca de la omisión de la página del CLUF durante la instalación de Windows.</span><span class="sxs-lookup"><span data-stu-id="02e97-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="02e97-127">Se aplican los permisos de administración de dispositivos y el perfil y limitaciones siguientes:</span><span class="sxs-lookup"><span data-stu-id="02e97-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="02e97-128">Los partners de CSP pueden seguir administrar los perfiles de Autopilot para los clientes existentes con los que tienen relaciones de revendedor, incluso si los clientes han quitado los privilegios de administración delegada del partner.</span><span class="sxs-lookup"><span data-stu-id="02e97-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="02e97-129">Puedes administrar los dispositivos existentes para los clientes que se han agregado por el usuario o por otro partner de CSP.</span><span class="sxs-lookup"><span data-stu-id="02e97-129">You can manage existing devices for your customers that have been added either by you or by another CSP partner.</span></span>

- <span data-ttu-id="02e97-130">No puedes administrar dispositivos que se haya cargado tu cliente a Microsoft Store para empresas o el Portal de Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="02e97-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="02e97-131">Crear y administrar perfiles Autopilot en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="02e97-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="02e97-132">En el centro de partners, puedes crear perfiles de implementación de Windows Autopilot y aplicarlos a los dispositivos.</span><span class="sxs-lookup"><span data-stu-id="02e97-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="02e97-133">Crear y aplicar los perfiles sólo los agentes de administración.</span><span class="sxs-lookup"><span data-stu-id="02e97-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="02e97-134">Crear un nuevo perfil de Autopilot</span><span class="sxs-lookup"><span data-stu-id="02e97-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="02e97-135">Selecciona **los clientes** desde el menú del centro de partners y, a continuación, selecciona al cliente que vas a crear el perfil de Autopilot para.</span><span class="sxs-lookup"><span data-stu-id="02e97-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="02e97-136">En la página de detalles del cliente, selecciona **los dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="02e97-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="02e97-137">En **los perfiles de Windows Autopilot** selecciona **Agregar nuevo perfil**.</span><span class="sxs-lookup"><span data-stu-id="02e97-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="02e97-138">Escribe el nombre del perfil y una descripción y, a continuación, configura las opciones de configuración rápida.</span><span class="sxs-lookup"><span data-stu-id="02e97-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="02e97-139">Elegir entre:</span><span class="sxs-lookup"><span data-stu-id="02e97-139">Choose from:</span></span>  

   - <span data-ttu-id="02e97-140">Omitir la configuración de privacidad en configuración</span><span class="sxs-lookup"><span data-stu-id="02e97-140">Skip privacy settings in setup</span></span>
   
   - <span data-ttu-id="02e97-141">Deshabilitar la cuenta de administrador local en el programa de instalación</span><span class="sxs-lookup"><span data-stu-id="02e97-141">Disable local admin account in setup</span></span>
   
   - <span data-ttu-id="02e97-142">Omitir automáticamente las páginas durante la instalación</span><span class="sxs-lookup"><span data-stu-id="02e97-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="02e97-143">(Incluye *páginas de configuración de registro de OEM, OneDrive y omitir Cortana*y *Seleccionar automáticamente la configuración de trabajo o escuela* )</span><span class="sxs-lookup"><span data-stu-id="02e97-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
   
   - <span data-ttu-id="02e97-144">Omitir contrato de licencia de usuario final (CLUF)</span><span class="sxs-lookup"><span data-stu-id="02e97-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] <span data-ttu-id="02e97-145">Consulta [desestimación del CLUF de Windows Autopilot](#windows-autopilot-eula-dismissal) a continuación para obtener información importante a tener en cuenta acerca de la omisión de la página del CLUF durante la instalación de Windows.</span><span class="sxs-lookup"><span data-stu-id="02e97-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="02e97-146">Selecciona **Enviar** cuando hayas acabado.</span><span class="sxs-lookup"><span data-stu-id="02e97-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="02e97-147">Aplicar un perfil de Autopilot a dispositivos de los clientes</span><span class="sxs-lookup"><span data-stu-id="02e97-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="02e97-148">Las siguientes instrucciones se suponen que ya has agregado dispositivos del cliente al centro de partners y que puedes acceder a su lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="02e97-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="02e97-149">Si aún no ha agregado los dispositivos del cliente, sigue las instrucciones de [Agregar dispositivos a una cuenta de cliente](#add-devices-to-a-customers-account) y, a continuación, sigue los pasos siguientes.</span><span class="sxs-lookup"><span data-stu-id="02e97-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="02e97-150">Después de crear un perfil de Autopilot para un cliente, se puede aplicar a los dispositivos del cliente.</span><span class="sxs-lookup"><span data-stu-id="02e97-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="02e97-151">Selecciona **los clientes** desde el menú del centro de partners y, a continuación, selecciona al cliente que creó el perfil de Autopilot para.</span><span class="sxs-lookup"><span data-stu-id="02e97-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="02e97-152">En la página de detalles del cliente, selecciona **los dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="02e97-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="02e97-153">En **los perfiles de aplicar a dispositivos** selecciona los dispositivos o grupos de dispositivos que quieres agregar perfiles para y, a continuación, seleccione **Aplicar perfil**.</span><span class="sxs-lookup"><span data-stu-id="02e97-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="02e97-154">El perfil que aplica solo aparece en la columna **perfil** .</span><span class="sxs-lookup"><span data-stu-id="02e97-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="02e97-155">Sigue los pasos siguientes para comprobar que el perfil se aplicará correctamente en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="02e97-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="02e97-156">a.</span><span class="sxs-lookup"><span data-stu-id="02e97-156">a.</span></span>  <span data-ttu-id="02e97-157">Conecta un dispositivo a la red y enciéndelo.</span><span class="sxs-lookup"><span data-stu-id="02e97-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="02e97-158">b.</span><span class="sxs-lookup"><span data-stu-id="02e97-158">b.</span></span>  <span data-ttu-id="02e97-159">Comprueba que aparezcan las pantallas OOBE apropiadas (si es el caso).</span><span class="sxs-lookup"><span data-stu-id="02e97-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="02e97-160">c.</span><span class="sxs-lookup"><span data-stu-id="02e97-160">c.</span></span>  <span data-ttu-id="02e97-161">Cuando se detiene el proceso OOBE, restablece el dispositivo a su configuración predeterminada de fábrica para prepararlo para un usuario nuevo.</span><span class="sxs-lookup"><span data-stu-id="02e97-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="02e97-162">Quitar un perfil de Autopilot de dispositivo de un cliente</span><span class="sxs-lookup"><span data-stu-id="02e97-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="02e97-163">Selecciona **los clientes** desde el menú del centro de partners y, a continuación, selecciona al cliente que creó el perfil de Autopilot para.</span><span class="sxs-lookup"><span data-stu-id="02e97-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="02e97-164">En la página de detalles del cliente, selecciona **los dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="02e97-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="02e97-165">En **los perfiles de aplicar a dispositivos** seleccionar los dispositivos que quieres quitar el perfil y, a continuación, selecciona **quitar perfil**.</span><span class="sxs-lookup"><span data-stu-id="02e97-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

  >[!NOTE]
  ><span data-ttu-id="02e97-166">Eliminar un perfil de un dispositivo no elimina el perfil de tu lista.</span><span class="sxs-lookup"><span data-stu-id="02e97-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="02e97-167">Si quieres eliminar un perfil, sigue las instrucciones de [actualización o eliminar un perfil de Autopilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="02e97-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="02e97-168">Actualizar o eliminar un perfil de Autopilot</span><span class="sxs-lookup"><span data-stu-id="02e97-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="02e97-169">Si un cliente quiere cambiar la experiencia out-of-box después de que hayas enviado los dispositivos a ellos, puedes cambiar el perfil del centro de partners.</span><span class="sxs-lookup"><span data-stu-id="02e97-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="02e97-170">Cuando el dispositivo del cliente se conecta a internet, que descargue la versión más reciente de perfil durante el proceso OOBE.</span><span class="sxs-lookup"><span data-stu-id="02e97-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="02e97-171">También, siempre que un cliente restaura un dispositivo con la configuración predeterminada de fábrica, el dispositivo se vuelve a descargar la versión más reciente del perfil durante el proceso OOBE.</span><span class="sxs-lookup"><span data-stu-id="02e97-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="02e97-172">Selecciona **clientes** en el menú del centro de partners y, a continuación, selecciona al cliente que quiere cambiar un perfil de Autopilot.</span><span class="sxs-lookup"><span data-stu-id="02e97-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="02e97-173">En la página de detalles del cliente, selecciona **los dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="02e97-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="02e97-174">En **los perfiles de Windows Autopilot** selecciona el perfil que tengas que actualizar.</span><span class="sxs-lookup"><span data-stu-id="02e97-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="02e97-175">Realiza los cambios necesarios y, a continuación, selecciona **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="02e97-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="02e97-176">Para eliminar el perfil, selecciona **eliminar el perfil** de la esquina superior derecha de la página.</span><span class="sxs-lookup"><span data-stu-id="02e97-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="02e97-177">Agregar dispositivos a una cuenta de cliente</span><span class="sxs-lookup"><span data-stu-id="02e97-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="02e97-178">Los agentes de ventas y los agentes de administración pueden agregar dispositivos a una cuenta de cliente.</span><span class="sxs-lookup"><span data-stu-id="02e97-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="02e97-179">Antes de que se pueden aplicar perfiles personalizados de Autopilot para dispositivos de los clientes, debe ser capaz de acceder a la lista de dispositivos del cliente.</span><span class="sxs-lookup"><span data-stu-id="02e97-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="02e97-180">Si vas a usar el nombre de OEM, número de serie y combinación de modelos, ten en cuenta estas limitaciones:</span><span class="sxs-lookup"><span data-stu-id="02e97-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="02e97-181">Funciona tuplas solo para dispositivos más recientes (4 k hash, por ejemplo) y no se admite para 128b hash (RS2 y dispositivos anteriores).</span><span class="sxs-lookup"><span data-stu-id="02e97-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="02e97-182">El registro de tupla distingue mayúsculas de minúsculas, por lo que los datos en el archivo deben coincidir con el fabricante y modelo de nombres ***exactamente*** como proporcionados por el proveedor de OEM (proveedor de hardware).</span><span class="sxs-lookup"><span data-stu-id="02e97-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="02e97-183">Sigue estas instrucciones para agregar dispositivos a una cuenta de cliente en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="02e97-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="02e97-184">Selecciona **los clientes** desde el menú del centro de partners y, a continuación, selecciona al cliente cuyos dispositivos que quieres administrar.</span><span class="sxs-lookup"><span data-stu-id="02e97-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="02e97-185">En la página de detalles del cliente, selecciona **los dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="02e97-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="02e97-186">En **los perfiles de aplicar a dispositivos** seleccionar **Agregar dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="02e97-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="02e97-187">Escribe un nombre para la lista de dispositivos y, a continuación, selecciona **Examinar** para cargar la lista del cliente (en formato de archivo .csv) en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="02e97-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="02e97-188">Debe haber recibido este archivo .csv con la compra del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="02e97-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="02e97-189">Si no recibes un archivo .csv, puedes crear una tú mismo siguiendo los pasos de [Agregar dispositivos a Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="02e97-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="02e97-190">Carga el archivo .csv y, a continuación, selecciona **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="02e97-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="02e97-191">Si recibes un mensaje de error al intentar cargar el archivo .csv, comprueba el formato del archivo.</span><span class="sxs-lookup"><span data-stu-id="02e97-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="02e97-192">Puedes usar solo, el hash de hardware o el nombre del OEM, número de serie y modelo (en ese orden de columna) o el identificador de producto de Windows.</span><span class="sxs-lookup"><span data-stu-id="02e97-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="02e97-193">También puedes usar el archivo .csv de muestra proporcionado desde el vínculo situado junto a **Agregar dispositivos** para crear una lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="02e97-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="02e97-194">Desestimación del CLUF de Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="02e97-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="02e97-195">INFORMACIÓN IMPORTANTE</span><span class="sxs-lookup"><span data-stu-id="02e97-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="02e97-196">Windows Autopilot te permite configurar instalaciones personalizadas de Windows en dispositivos que administras para tus clientes.</span><span class="sxs-lookup"><span data-stu-id="02e97-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="02e97-197">Si autorizado no lo haces, el cliente, puedes suprimir u ocultar determinadas pantallas de configuración que normalmente se muestran a los usuarios al configurar Windows, incluida la pantalla de aceptación de términos (contrato de licencia de usuario final).</span><span class="sxs-lookup"><span data-stu-id="02e97-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="02e97-198">Al usar esta función, aceptas suprimir u ocultar cualquiera de las pantallas que está diseñada para proporcionar a los usuarios aviso o aceptación de significa términos que has obtenido el consentimiento suficiente y autorización desde el cliente para ocultar los términos y que, en nombre de el cliente (si una organización o un usuario individual como el caso), autorizas notificaciones y aceptas los términos aplicables al cliente.</span><span class="sxs-lookup"><span data-stu-id="02e97-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="02e97-199">Esto incluye que estás de acuerdo con los términos y condiciones de la licencia o el anuncio que se presenta al usuario si no la suprimiste u ocultaste con esta herramienta.</span><span class="sxs-lookup"><span data-stu-id="02e97-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="02e97-200">Tu cliente no puede usar el software de Windows en esos dispositivos si ha adquirido de manera válida una licencia para el software desde Microsoft o sus distribuidores con licencia.</span><span class="sxs-lookup"><span data-stu-id="02e97-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>