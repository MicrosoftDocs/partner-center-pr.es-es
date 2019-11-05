---
title: Personalización de la experiencia rápida de un dispositivo con perfiles de Windows AutoPilot | Centro de Partners
description: Preconfigurar la configuración rápida de un dispositivo con perfiles de AutoPilot.
ms.topic: article
ms.date: 03/18/2019
author: maggiepuccievans
ms.author: evansma
keywords: AutoPilot, Windows AutoPilot, Microsoft AutoPilot, implementación sin interacción rápida, Oobe, pantallas de inicio de sesión, no actualizadas
ms.localizationpriority: medium
ms.openlocfilehash: 7861efa8c0fd7e03488ba3f222fcb3a476c06cc2
ms.sourcegitcommit: 76c34fd8dc544cea93496079df68759a1da9098c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/04/2019
ms.locfileid: "73544050"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="66d07-104">Personalización de la experiencia rápida de un dispositivo con perfiles de Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="66d07-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

<span data-ttu-id="66d07-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="66d07-105">**Applies to**</span></span>

- <span data-ttu-id="66d07-106">CSP directo: factura, proveedores indirectos y distribuidores indirectos</span><span class="sxs-lookup"><span data-stu-id="66d07-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="66d07-107">Si administra los dispositivos del cliente, es posible que tenga que personalizar la experiencia rápida (OOBE) para los usuarios del cliente.</span><span class="sxs-lookup"><span data-stu-id="66d07-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="66d07-108">Puede preconfigurar nuevos dispositivos con perfiles de Windows AutoPilot antes de entregar los dispositivos a los clientes y aplicar nuevos perfiles a los dispositivos que los clientes ya han comprado.</span><span class="sxs-lookup"><span data-stu-id="66d07-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="66d07-109">Tenga en cuenta que los OEM han empezado a incluir una etiqueta de envío en el exterior del cuadro dispositivo AutoPilot que muestra el identificador de la clave de producto del dispositivo **(pkid)** .</span><span class="sxs-lookup"><span data-stu-id="66d07-109">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device’s **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="66d07-110">Este código de barras bidimensional y legible proporciona a los asociados de nivel inferior una manera de registrar dispositivos para el piloto automático sin tener que volver a realizar la conversión unboxing de los dispositivos y cosechar el ID. de dispositivo mediante medios alternativos.</span><span class="sxs-lookup"><span data-stu-id="66d07-110">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="66d07-111">En este artículo se explica cómo crear y aplicar perfiles de AutoPilot a dispositivos del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="66d07-111">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="66d07-112">Si no está familiarizado con AutoPilot, revise la información de estos artículos:</span><span class="sxs-lookup"><span data-stu-id="66d07-112">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="66d07-113">Información general de Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="66d07-113">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="66d07-114">Guía de referencia de implementación de AutoPilot</span><span class="sxs-lookup"><span data-stu-id="66d07-114">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="66d07-115">Introducción</span><span class="sxs-lookup"><span data-stu-id="66d07-115">Overview</span></span>

<span data-ttu-id="66d07-116">Con la característica de Windows AutoPilot del centro de Partners, puede crear perfiles personalizados para aplicarlos a los dispositivos del cliente.</span><span class="sxs-lookup"><span data-stu-id="66d07-116">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="66d07-117">La siguiente configuración de perfil estaba disponible en el momento en que se publicó este artículo:</span><span class="sxs-lookup"><span data-stu-id="66d07-117">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="66d07-118">Omitir la configuración de privacidad.</span><span class="sxs-lookup"><span data-stu-id="66d07-118">Skip privacy settings.</span></span> <span data-ttu-id="66d07-119">Esta configuración de Perfil de AutoPilot opcional permite a las organizaciones no preguntar sobre la configuración de privacidad durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="66d07-119">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="66d07-120">Deshabilite la creación de cuentas de administrador local en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66d07-120">Disable local admin account creation on the device.</span></span> <span data-ttu-id="66d07-121">Las organizaciones pueden decidir si el usuario que configura el dispositivo debe tener acceso de administrador una vez completado el proceso.</span><span class="sxs-lookup"><span data-stu-id="66d07-121">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="66d07-122">Configure automáticamente el dispositivo para el trabajo o la escuela.</span><span class="sxs-lookup"><span data-stu-id="66d07-122">Automatically set up device for work or school.</span></span> <span data-ttu-id="66d07-123">Todos los dispositivos registrados con AutoPilot se considerarán automáticamente dispositivos de trabajo o escuela, por lo que no se le pedirá esta pregunta durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="66d07-123">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="66d07-124">Omitir las páginas de configuración de registro de Cortana, OneDrive y OEM.</span><span class="sxs-lookup"><span data-stu-id="66d07-124">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="66d07-125">Todos los dispositivos registrados con AutoPilot omitirán automáticamente estas páginas durante el proceso de la experiencia rápida (OOBE).</span><span class="sxs-lookup"><span data-stu-id="66d07-125">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="66d07-126">Omitir contrato de licencia para el usuario final (CLUF).</span><span class="sxs-lookup"><span data-stu-id="66d07-126">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="66d07-127">A partir de la versión 1709 de Windows 10, las organizaciones pueden decidir omitir la página del CLUF presentada durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="66d07-127">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="66d07-128">Consulte [descartado de CLUF de Windows AutoPilot](#windows-autopilot-eula-dismissal) para obtener información importante que se debe tener en cuenta al omitir la página del CLUF durante la instalación de Windows.</span><span class="sxs-lookup"><span data-stu-id="66d07-128">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="66d07-129">Se aplican las siguientes limitaciones y permisos de administración de perfiles y dispositivos:</span><span class="sxs-lookup"><span data-stu-id="66d07-129">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="66d07-130">Los asociados de CSP pueden seguir administrando los perfiles de AutoPilot para los clientes existentes con quienes tienen relaciones de reseller, incluso si los clientes han quitado los privilegios de administración delegada del socio.</span><span class="sxs-lookup"><span data-stu-id="66d07-130">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="66d07-131">Puede administrar los dispositivos existentes para los clientes que ha agregado.</span><span class="sxs-lookup"><span data-stu-id="66d07-131">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="66d07-132">No puede administrar los dispositivos que el cliente ha cargado en Microsoft Store para empresas o en el portal de Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="66d07-132">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="66d07-133">Crear y administrar perfiles de AutoPilot en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="66d07-133">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="66d07-134">En el centro de Partners, puede crear perfiles de implementación de Windows AutoPilot y aplicarlos a los dispositivos.</span><span class="sxs-lookup"><span data-stu-id="66d07-134">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="66d07-135">Solo los agentes de administración pueden crear y aplicar perfiles.</span><span class="sxs-lookup"><span data-stu-id="66d07-135">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="66d07-136">Crear un nuevo perfil AutoPilot</span><span class="sxs-lookup"><span data-stu-id="66d07-136">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="66d07-137">Seleccione **clientes** en el menú del centro de Partners y, a continuación, seleccione el cliente para el que va a crear el perfil de AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="66d07-137">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="66d07-138">En la página de detalles del cliente, seleccione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="66d07-138">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="66d07-139">En **perfiles de Windows AutoPilot** , seleccione **Agregar nuevo perfil**.</span><span class="sxs-lookup"><span data-stu-id="66d07-139">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="66d07-140">Escriba el nombre y la descripción del perfil y, a continuación, establezca la configuración de OOBE.</span><span class="sxs-lookup"><span data-stu-id="66d07-140">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="66d07-141">Elija entre:</span><span class="sxs-lookup"><span data-stu-id="66d07-141">Choose from:</span></span>  

   - <span data-ttu-id="66d07-142">Omitir la configuración de privacidad en el programa de instalación</span><span class="sxs-lookup"><span data-stu-id="66d07-142">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="66d07-143">Deshabilitar la cuenta de administrador local en el programa de instalación</span><span class="sxs-lookup"><span data-stu-id="66d07-143">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="66d07-144">Omitir automáticamente las páginas durante la instalación</span><span class="sxs-lookup"><span data-stu-id="66d07-144">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="66d07-145">(Incluye *la configuración seleccionada automáticamente para el trabajo o la escuela* y *omitir las páginas de configuración de registro de Cortana, OneDrive y OEM*)</span><span class="sxs-lookup"><span data-stu-id="66d07-145">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="66d07-146">Omitir contrato de licencia para el usuario final (CLUF)</span><span class="sxs-lookup"><span data-stu-id="66d07-146">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="66d07-147">Consulte [descartado de CLUF de Windows AutoPilot](#windows-autopilot-eula-dismissal) para obtener información importante que se debe tener en cuenta al omitir la página del CLUF durante la instalación de Windows.</span><span class="sxs-lookup"><span data-stu-id="66d07-147">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="66d07-148">Selecciona **Enviar** cuando hayas acabado.</span><span class="sxs-lookup"><span data-stu-id="66d07-148">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="66d07-149">Aplicar un perfil de AutoPilot a los dispositivos del cliente</span><span class="sxs-lookup"><span data-stu-id="66d07-149">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="66d07-150">En las instrucciones siguientes se supone que ya ha agregado los dispositivos del cliente al centro de Partners y que puede acceder a su lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="66d07-150">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="66d07-151">Si aún no ha agregado los dispositivos del cliente, siga las instrucciones de [Agregar dispositivos a la cuenta de un cliente](#add-devices-to-a-customers-account) y, a continuación, siga los pasos que se indican a continuación.</span><span class="sxs-lookup"><span data-stu-id="66d07-151">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="66d07-152">Después de crear un perfil de AutoPilot para un cliente, puede aplicarlo a los dispositivos del cliente.</span><span class="sxs-lookup"><span data-stu-id="66d07-152">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="66d07-153">Seleccione **clientes** en el menú del centro de Partners y, a continuación, seleccione el cliente para el que ha creado el perfil AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="66d07-153">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="66d07-154">En la página de detalles del cliente, seleccione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="66d07-154">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="66d07-155">En **aplicar perfiles a dispositivos** , seleccione los dispositivos o grupos de dispositivos a los que quiere agregar perfiles y, a continuación, seleccione **aplicar perfil**.</span><span class="sxs-lookup"><span data-stu-id="66d07-155">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="66d07-156">El perfil que acaba de aplicar aparece en la columna **perfil** .</span><span class="sxs-lookup"><span data-stu-id="66d07-156">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="66d07-157">Siga los pasos que se indican a continuación para comprobar que el perfil se aplicará correctamente al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66d07-157">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="66d07-158">a.</span><span class="sxs-lookup"><span data-stu-id="66d07-158">a.</span></span>  <span data-ttu-id="66d07-159">Conectar un dispositivo a la red y activarlo.</span><span class="sxs-lookup"><span data-stu-id="66d07-159">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="66d07-160">b.</span><span class="sxs-lookup"><span data-stu-id="66d07-160">b.</span></span>  <span data-ttu-id="66d07-161">Comprueba que aparezcan las pantallas OOBE apropiadas (si es el caso).</span><span class="sxs-lookup"><span data-stu-id="66d07-161">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="66d07-162">c.</span><span class="sxs-lookup"><span data-stu-id="66d07-162">c.</span></span>  <span data-ttu-id="66d07-163">Cuando se detenga el proceso de OOBE, restablezca el dispositivo a su configuración predeterminada de fábrica para prepararlo para un nuevo usuario.</span><span class="sxs-lookup"><span data-stu-id="66d07-163">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="66d07-164">Quitar un perfil de AutoPilot del dispositivo de un cliente</span><span class="sxs-lookup"><span data-stu-id="66d07-164">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="66d07-165">Seleccione **clientes** en el menú del centro de Partners y, a continuación, seleccione el cliente para el que ha creado el perfil AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="66d07-165">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="66d07-166">En la página de detalles del cliente, seleccione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="66d07-166">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="66d07-167">En **aplicar perfiles a dispositivos** , seleccione los dispositivos de los que desea quitar el perfil y, a continuación, seleccione **quitar perfil**.</span><span class="sxs-lookup"><span data-stu-id="66d07-167">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="66d07-168">La eliminación de un perfil de un dispositivo no elimina el perfil de la lista.</span><span class="sxs-lookup"><span data-stu-id="66d07-168">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="66d07-169">Si desea eliminar un perfil, siga las instrucciones de [actualización o eliminación de un perfil de AutoPilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="66d07-169">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="66d07-170">Actualización o eliminación de un perfil de AutoPilot</span><span class="sxs-lookup"><span data-stu-id="66d07-170">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="66d07-171">Si un cliente desea cambiar la experiencia rápida después de haber enviado los dispositivos a ellos, puede cambiar el perfil en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="66d07-171">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="66d07-172">Cuando el dispositivo del cliente se conecta a Internet, se descargará la versión más reciente del perfil durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="66d07-172">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="66d07-173">Además, cada vez que un cliente restaura un dispositivo a su configuración predeterminada de fábrica, el dispositivo descargará la versión más reciente del perfil durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="66d07-173">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="66d07-174">Seleccione **clientes** en el menú del centro de Partners y, a continuación, seleccione el cliente que desea cambiar un perfil de AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="66d07-174">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="66d07-175">En la página de detalles del cliente, seleccione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="66d07-175">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="66d07-176">En **perfiles de Windows AutoPilot** , seleccione el perfil que necesita actualizar.</span><span class="sxs-lookup"><span data-stu-id="66d07-176">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="66d07-177">Realice los cambios necesarios y, a continuación, seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="66d07-177">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="66d07-178">Para eliminar este perfil, seleccione **eliminar perfil** en la esquina superior derecha de la página.</span><span class="sxs-lookup"><span data-stu-id="66d07-178">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="66d07-179">Agregar dispositivos a la cuenta de un cliente</span><span class="sxs-lookup"><span data-stu-id="66d07-179">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="66d07-180">Los agentes de ventas y los agentes de administración pueden agregar dispositivos a la cuenta de un cliente.</span><span class="sxs-lookup"><span data-stu-id="66d07-180">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="66d07-181">Para poder aplicar perfiles de AutoPilot personalizados a los dispositivos del cliente, debe tener acceso a la lista de dispositivos del cliente.</span><span class="sxs-lookup"><span data-stu-id="66d07-181">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="66d07-182">Si tiene previsto usar el nombre del OEM, el número de serie y la combinación de modelos, tenga en cuenta estas limitaciones:</span><span class="sxs-lookup"><span data-stu-id="66d07-182">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="66d07-183">Esta tupla solo funciona para dispositivos más recientes (por ejemplo, hash 4k) y no se admite para los hashes 128B (RS2 y dispositivos anteriores).</span><span class="sxs-lookup"><span data-stu-id="66d07-183">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="66d07-184">El registro de la tupla distingue entre mayúsculas y minúsculas, por lo que los datos del archivo deben coincidir ***exactamente*** con los nombres del modelo y del fabricante, tal como lo proporciona el proveedor de OEM (proveedor de hardware).</span><span class="sxs-lookup"><span data-stu-id="66d07-184">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="66d07-185">Siga las instrucciones que se indican a continuación para agregar dispositivos a la cuenta de un cliente en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="66d07-185">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="66d07-186">Seleccione **customers (clientes** ) en el menú del centro de Partners y seleccione el cliente cuyos dispositivos desea administrar.</span><span class="sxs-lookup"><span data-stu-id="66d07-186">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="66d07-187">En la página de detalles del cliente, seleccione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="66d07-187">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="66d07-188">En **aplicar perfiles a dispositivos** , seleccione **Agregar dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="66d07-188">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="66d07-189">Escriba un nombre para la lista de dispositivos y, a continuación, seleccione **examinar** para cargar la lista de clientes (en formato de archivo. csv) en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="66d07-189">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="66d07-190">Debe haber recibido este archivo. csv con la compra del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="66d07-190">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="66d07-191">Si no recibió un archivo. csv, puede crear uno usted mismo siguiendo los pasos descritos en [Agregar dispositivos a Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="66d07-191">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="66d07-192">Cargue el archivo. csv y, a continuación, seleccione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="66d07-192">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="66d07-193">Si recibe un mensaje de error al intentar cargar el archivo. csv, compruebe el formato del archivo.</span><span class="sxs-lookup"><span data-stu-id="66d07-193">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="66d07-194">Solo puede utilizar el hash de hardware, el nombre de OEM, el número de serie y el modelo (en ese orden de columna), o el identificador de producto de Windows.</span><span class="sxs-lookup"><span data-stu-id="66d07-194">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="66d07-195">También puede usar el archivo. csv de ejemplo que se proporciona en el vínculo junto a **Agregar dispositivos** para crear una lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="66d07-195">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="66d07-196">El archivo. csv debería tener un aspecto similar al siguiente:</span><span class="sxs-lookup"><span data-stu-id="66d07-196">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="66d07-197">**Número de serie del dispositivo, ID. de producto de Windows, hash de hardware, nombre de fabricante, modelo de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="66d07-197">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="66d07-198">**{serialNumber},,, Microsoft Corporation, Surface Laptop**</span><span class="sxs-lookup"><span data-stu-id="66d07-198">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

<span data-ttu-id="66d07-199">Tenga en cuenta que "nombre del fabricante" y "modelo de dispositivo" distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="66d07-199">Note that "Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="66d07-200">Si no sabe qué valor poner para el modelo de nombre de fabricante y dispositivo, puede ejecutarlo en el dispositivo para recopilar los valores correctos:</span><span class="sxs-lookup"><span data-stu-id="66d07-200">If you don’t know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="66d07-201">Descartado de CLUF de Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="66d07-201">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="66d07-202">INFORMACIÓN IMPORTANTE</span><span class="sxs-lookup"><span data-stu-id="66d07-202">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="66d07-203">Windows AutoPilot le permite configurar instalaciones personalizadas de Windows en los dispositivos que administra para sus clientes.</span><span class="sxs-lookup"><span data-stu-id="66d07-203">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="66d07-204">Si el cliente tiene autorización para hacerlo, puede suprimir u ocultar determinadas pantallas de configuración que se suelen presentar a los usuarios al configurar Windows, incluida la pantalla de aceptación del CLUF (contrato de licencia para el usuario final).</span><span class="sxs-lookup"><span data-stu-id="66d07-204">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="66d07-205">Al usar esta función, acepta que la supresión y ocultación de las pantallas que están diseñadas para proporcionar a los usuarios aviso o aceptación de términos significa que ha obtenido el consentimiento y la autorización suficientes del cliente para ocultar términos y que usted, en nombre de su cliente (ya sea una organización o un usuario individual como caso), dar su consentimiento a cualquier aviso y aceptar los términos aplicables a su cliente.</span><span class="sxs-lookup"><span data-stu-id="66d07-205">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="66d07-206">Esto incluye que estás de acuerdo con los términos y condiciones de la licencia o el anuncio que se presenta al usuario si no la suprimiste u ocultaste con esta herramienta.</span><span class="sxs-lookup"><span data-stu-id="66d07-206">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="66d07-207">Tu cliente no puede usar el software de Windows en esos dispositivos si ha adquirido de manera válida una licencia para el software desde Microsoft o sus distribuidores con licencia.</span><span class="sxs-lookup"><span data-stu-id="66d07-207">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>
