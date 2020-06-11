---
title: Personalización de la experiencia rápida de un dispositivo
ms.topic: article
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Antes de entregar el nuevo dispositivo del cliente, puede usar los perfiles de Windows AutoPilot para personalizar o configurar previamente la configuración rápida (OOBE) del dispositivo.
author: LauraBrenner
ms.author: labrenne
keywords: AutoPilot, Windows AutoPilot, Microsoft AutoPilot, implementación sin interacción rápida, Oobe, pantallas de inicio de sesión, no actualizadas
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: a3067b674b7784df34fba3de9cfaa5b44349b8c4
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679192"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="72772-104">Usar perfiles de Windows AutoPilot en dispositivos nuevos para personalizar la experiencia rápida de un cliente</span><span class="sxs-lookup"><span data-stu-id="72772-104">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="72772-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="72772-105">**Applies to**</span></span>

- <span data-ttu-id="72772-106">CSP directo: factura, proveedores indirectos y distribuidores indirectos</span><span class="sxs-lookup"><span data-stu-id="72772-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="72772-107">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="72772-107">**Appropriate roles**</span></span>

- <span data-ttu-id="72772-108">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="72772-108">Admin agent</span></span>
- <span data-ttu-id="72772-109">Administrador global</span><span class="sxs-lookup"><span data-stu-id="72772-109">Global admin</span></span>
- <span data-ttu-id="72772-110">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="72772-110">Sales agent</span></span>
- <span data-ttu-id="72772-111">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="72772-111">User management admin</span></span>

<span data-ttu-id="72772-112">Si administra los dispositivos del cliente, es posible que tenga que personalizar la experiencia rápida (OOBE) para los usuarios del cliente.</span><span class="sxs-lookup"><span data-stu-id="72772-112">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="72772-113">Puede preconfigurar nuevos dispositivos con perfiles de Windows AutoPilot antes de entregar los dispositivos a los clientes y aplicar nuevos perfiles a los dispositivos que los clientes ya han comprado.</span><span class="sxs-lookup"><span data-stu-id="72772-113">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="72772-114">Tenga en cuenta que los OEM han empezado a incluir una etiqueta de envío en el exterior del cuadro dispositivo AutoPilot que muestra el identificador de la clave de producto del dispositivo **(pkid)**.</span><span class="sxs-lookup"><span data-stu-id="72772-114">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="72772-115">Este código de barras bidimensional y legible proporciona a los asociados de nivel inferior una manera de registrar dispositivos para el piloto automático sin tener que volver a realizar la conversión unboxing de los dispositivos y cosechar el ID. de dispositivo mediante medios alternativos.</span><span class="sxs-lookup"><span data-stu-id="72772-115">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="72772-116">En este artículo se explica cómo crear y aplicar perfiles de AutoPilot a dispositivos del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="72772-116">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="72772-117">Si no está familiarizado con AutoPilot, revise la información de estos artículos:</span><span class="sxs-lookup"><span data-stu-id="72772-117">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="72772-118">Información general de Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="72772-118">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="72772-119">Guía de referencia de implementación de AutoPilot</span><span class="sxs-lookup"><span data-stu-id="72772-119">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="72772-120">Información general</span><span class="sxs-lookup"><span data-stu-id="72772-120">Overview</span></span>

<span data-ttu-id="72772-121">Con la característica de Windows AutoPilot del centro de Partners, puede crear perfiles personalizados para aplicarlos a los dispositivos del cliente.</span><span class="sxs-lookup"><span data-stu-id="72772-121">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="72772-122">La siguiente configuración de perfil estaba disponible en el momento en que se publicó este artículo:</span><span class="sxs-lookup"><span data-stu-id="72772-122">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="72772-123">Omitir la configuración de privacidad.</span><span class="sxs-lookup"><span data-stu-id="72772-123">Skip privacy settings.</span></span> <span data-ttu-id="72772-124">Esta configuración de Perfil de AutoPilot opcional permite a las organizaciones no preguntar sobre la configuración de privacidad durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="72772-124">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="72772-125">Deshabilite la creación de cuentas de administrador local en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="72772-125">Disable local admin account creation on the device.</span></span> <span data-ttu-id="72772-126">Las organizaciones pueden decidir si el usuario que configura el dispositivo debe tener acceso de administrador una vez completado el proceso.</span><span class="sxs-lookup"><span data-stu-id="72772-126">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="72772-127">Configure automáticamente el dispositivo para el trabajo o la escuela.</span><span class="sxs-lookup"><span data-stu-id="72772-127">Automatically set up device for work or school.</span></span> <span data-ttu-id="72772-128">Todos los dispositivos registrados con AutoPilot se considerarán automáticamente dispositivos de trabajo o escuela, por lo que no se le pedirá esta pregunta durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="72772-128">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="72772-129">Omitir las páginas de configuración de registro de Cortana, OneDrive y OEM.</span><span class="sxs-lookup"><span data-stu-id="72772-129">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="72772-130">Todos los dispositivos registrados con AutoPilot omitirán automáticamente estas páginas durante el proceso de la experiencia rápida (OOBE).</span><span class="sxs-lookup"><span data-stu-id="72772-130">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="72772-131">Omitir contrato de licencia para el usuario final (CLUF).</span><span class="sxs-lookup"><span data-stu-id="72772-131">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="72772-132">A partir de la versión 1709 de Windows 10, las organizaciones pueden decidir omitir la página del CLUF presentada durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="72772-132">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="72772-133">Consulte [descartado de CLUF de Windows AutoPilot](#windows-autopilot-eula-dismissal) para obtener información importante que se debe tener en cuenta al omitir la página del CLUF durante la instalación de Windows.</span><span class="sxs-lookup"><span data-stu-id="72772-133">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="72772-134">Se aplican las siguientes limitaciones y permisos de administración de perfiles y dispositivos:</span><span class="sxs-lookup"><span data-stu-id="72772-134">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="72772-135">Los asociados de CSP pueden seguir administrando los perfiles de AutoPilot para los clientes existentes con quienes tienen relaciones de reseller, incluso si los clientes han quitado los privilegios de administración delegada del socio.</span><span class="sxs-lookup"><span data-stu-id="72772-135">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="72772-136">Puede administrar los dispositivos existentes para los clientes que ha agregado.</span><span class="sxs-lookup"><span data-stu-id="72772-136">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="72772-137">No puede administrar los dispositivos que el cliente ha cargado en Microsoft Store para empresas o en el portal de Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="72772-137">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="72772-138">Crear y administrar perfiles de AutoPilot en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="72772-138">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="72772-139">En el centro de Partners, puede crear perfiles de implementación de Windows AutoPilot y aplicarlos a los dispositivos.</span><span class="sxs-lookup"><span data-stu-id="72772-139">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="72772-140">Solo los agentes de administración pueden crear y aplicar perfiles.</span><span class="sxs-lookup"><span data-stu-id="72772-140">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="72772-141">Crear un nuevo perfil AutoPilot</span><span class="sxs-lookup"><span data-stu-id="72772-141">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="72772-142">Seleccione **clientes** en el menú del centro de Partners y, a continuación, seleccione el cliente para el que va a crear el perfil de AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="72772-142">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="72772-143">En la página de detalles del cliente, seleccione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="72772-143">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="72772-144">En **perfiles de Windows AutoPilot** , seleccione **Agregar nuevo perfil**.</span><span class="sxs-lookup"><span data-stu-id="72772-144">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="72772-145">Escriba el nombre y la descripción del perfil y, a continuación, establezca la configuración de OOBE.</span><span class="sxs-lookup"><span data-stu-id="72772-145">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="72772-146">Elija de entre las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="72772-146">Choose from:</span></span>  

   - <span data-ttu-id="72772-147">Omitir la configuración de privacidad en el programa de instalación</span><span class="sxs-lookup"><span data-stu-id="72772-147">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="72772-148">Deshabilitar la cuenta de administrador local en el programa de instalación</span><span class="sxs-lookup"><span data-stu-id="72772-148">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="72772-149">Omitir páginas automáticamente en el programa de instalación</span><span class="sxs-lookup"><span data-stu-id="72772-149">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="72772-150">(Incluye *la configuración seleccionada automáticamente para el trabajo o la escuela* y *omitir las páginas de configuración de registro de Cortana, OneDrive y OEM*)</span><span class="sxs-lookup"><span data-stu-id="72772-150">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="72772-151">Omitir contrato de licencia para el usuario final (CLUF)</span><span class="sxs-lookup"><span data-stu-id="72772-151">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="72772-152">Consulte [descartado de CLUF de Windows AutoPilot](#windows-autopilot-eula-dismissal) para obtener información importante que se debe tener en cuenta al omitir la página del CLUF durante la instalación de Windows.</span><span class="sxs-lookup"><span data-stu-id="72772-152">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="72772-153">Seleccione **Enviar** cuando termine.</span><span class="sxs-lookup"><span data-stu-id="72772-153">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="72772-154">Aplicar un perfil de AutoPilot a los dispositivos del cliente</span><span class="sxs-lookup"><span data-stu-id="72772-154">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="72772-155">En las instrucciones siguientes se supone que ya ha agregado los dispositivos del cliente al centro de Partners y que puede acceder a su lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="72772-155">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="72772-156">Si aún no ha agregado los dispositivos del cliente, siga las instrucciones de [Agregar dispositivos a la cuenta de un cliente](#add-devices-to-a-customers-account) y, a continuación, siga los pasos que se indican a continuación.</span><span class="sxs-lookup"><span data-stu-id="72772-156">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="72772-157">Después de crear un perfil de AutoPilot para un cliente, puede aplicarlo a los dispositivos del cliente.</span><span class="sxs-lookup"><span data-stu-id="72772-157">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="72772-158">Seleccione **clientes** en el menú del centro de Partners y, a continuación, seleccione el cliente para el que ha creado el perfil AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="72772-158">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="72772-159">En la página de detalles del cliente, seleccione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="72772-159">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="72772-160">En **aplicar perfiles a dispositivos** , seleccione los dispositivos o grupos de dispositivos a los que quiere agregar perfiles y, a continuación, seleccione **aplicar perfil**.</span><span class="sxs-lookup"><span data-stu-id="72772-160">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="72772-161">El perfil que acaba de aplicar aparece en la columna **perfil** .</span><span class="sxs-lookup"><span data-stu-id="72772-161">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="72772-162">Siga los pasos que se indican a continuación para comprobar que el perfil se aplicará correctamente al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="72772-162">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="72772-163">a.</span><span class="sxs-lookup"><span data-stu-id="72772-163">a.</span></span>  <span data-ttu-id="72772-164">Conectar un dispositivo a la red y activarlo.</span><span class="sxs-lookup"><span data-stu-id="72772-164">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="72772-165">b.</span><span class="sxs-lookup"><span data-stu-id="72772-165">b.</span></span>  <span data-ttu-id="72772-166">Compruebe que aparecen las pantallas OOBE adecuadas (si existen).</span><span class="sxs-lookup"><span data-stu-id="72772-166">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="72772-167">c.</span><span class="sxs-lookup"><span data-stu-id="72772-167">c.</span></span>  <span data-ttu-id="72772-168">Cuando se detenga el proceso de OOBE, restablezca el dispositivo a su configuración predeterminada de fábrica para prepararlo para un nuevo usuario.</span><span class="sxs-lookup"><span data-stu-id="72772-168">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="72772-169">Quitar un perfil de AutoPilot del dispositivo de un cliente</span><span class="sxs-lookup"><span data-stu-id="72772-169">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="72772-170">Seleccione **clientes** en el menú del centro de Partners y, a continuación, seleccione el cliente para el que ha creado el perfil AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="72772-170">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="72772-171">En la página de detalles del cliente, seleccione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="72772-171">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="72772-172">En **aplicar perfiles a dispositivos** , seleccione los dispositivos de los que desea quitar el perfil y, a continuación, seleccione **quitar perfil**.</span><span class="sxs-lookup"><span data-stu-id="72772-172">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="72772-173">La eliminación de un perfil de un dispositivo no elimina el perfil de la lista.</span><span class="sxs-lookup"><span data-stu-id="72772-173">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="72772-174">Si desea eliminar un perfil, siga las instrucciones de [actualización o eliminación de un perfil de AutoPilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="72772-174">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="72772-175">Actualización o eliminación de un perfil de AutoPilot</span><span class="sxs-lookup"><span data-stu-id="72772-175">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="72772-176">Si un cliente desea cambiar la experiencia rápida después de haber enviado los dispositivos a ellos, puede cambiar el perfil en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="72772-176">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="72772-177">Cuando el dispositivo del cliente se conecta a Internet, se descargará la versión más reciente del perfil durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="72772-177">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="72772-178">Además, cada vez que un cliente restaura un dispositivo a su configuración predeterminada de fábrica, el dispositivo descargará la versión más reciente del perfil durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="72772-178">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="72772-179">Seleccione **clientes** en el menú del centro de Partners y, a continuación, seleccione el cliente que desea cambiar un perfil de AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="72772-179">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="72772-180">En la página de detalles del cliente, seleccione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="72772-180">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="72772-181">En **perfiles de Windows AutoPilot** , seleccione el perfil que necesita actualizar.</span><span class="sxs-lookup"><span data-stu-id="72772-181">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="72772-182">Realice los cambios necesarios y, a continuación, seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="72772-182">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="72772-183">Para eliminar este perfil, seleccione **eliminar perfil** en la esquina superior derecha de la página.</span><span class="sxs-lookup"><span data-stu-id="72772-183">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="72772-184">Agregar dispositivos a la cuenta de un cliente</span><span class="sxs-lookup"><span data-stu-id="72772-184">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="72772-185">Los agentes de ventas y los agentes de administración pueden agregar dispositivos a la cuenta de un cliente.</span><span class="sxs-lookup"><span data-stu-id="72772-185">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="72772-186">Para poder aplicar perfiles de AutoPilot personalizados a los dispositivos del cliente, debe tener acceso a la lista de dispositivos del cliente.</span><span class="sxs-lookup"><span data-stu-id="72772-186">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="72772-187">Si tiene previsto usar el nombre del OEM, el número de serie y la combinación de modelos, tenga en cuenta estas limitaciones:</span><span class="sxs-lookup"><span data-stu-id="72772-187">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="72772-188">Esta tupla solo funciona para dispositivos más recientes (por ejemplo, hash 4k) y no se admite para los hashes 128B (RS2 y dispositivos anteriores).</span><span class="sxs-lookup"><span data-stu-id="72772-188">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="72772-189">El registro de la tupla distingue entre mayúsculas y minúsculas, por lo que los datos del archivo deben coincidir ***exactamente*** con los nombres del modelo y del fabricante, tal como lo proporciona el proveedor de OEM (proveedor de hardware).</span><span class="sxs-lookup"><span data-stu-id="72772-189">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="72772-190">Siga las instrucciones que se indican a continuación para agregar dispositivos a la cuenta de un cliente en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="72772-190">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="72772-191">Seleccione **customers (clientes** ) en el menú del centro de Partners y seleccione el cliente cuyos dispositivos desea administrar.</span><span class="sxs-lookup"><span data-stu-id="72772-191">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="72772-192">En la página de detalles del cliente, seleccione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="72772-192">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="72772-193">En **aplicar perfiles a dispositivos** , seleccione **Agregar dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="72772-193">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="72772-194">Escriba un nombre para la lista de dispositivos y, a continuación, seleccione **examinar** para cargar la lista de clientes (en formato de archivo. csv) en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="72772-194">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="72772-195">Debe haber recibido este archivo. csv con la compra del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="72772-195">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="72772-196">Si no recibió un archivo. csv, puede crear uno usted mismo siguiendo los pasos descritos en [Agregar dispositivos a Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="72772-196">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="72772-197">Cargue el archivo. csv y, a continuación, seleccione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="72772-197">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="72772-198">Si recibe un mensaje de error al intentar cargar el archivo. csv, compruebe el formato del archivo.</span><span class="sxs-lookup"><span data-stu-id="72772-198">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="72772-199">Solo puede utilizar el hash de hardware, el nombre de OEM, el número de serie y el modelo (en ese orden de columna), o el identificador de producto de Windows.</span><span class="sxs-lookup"><span data-stu-id="72772-199">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="72772-200">También puede usar el archivo. csv de ejemplo que se proporciona en el vínculo junto a **Agregar dispositivos** para crear una lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="72772-200">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="72772-201">El archivo. csv debería tener un aspecto similar al siguiente:</span><span class="sxs-lookup"><span data-stu-id="72772-201">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="72772-202">**Número de serie del dispositivo, ID. de producto de Windows, hash de hardware, nombre de fabricante, modelo de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="72772-202">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="72772-203">**{serialNumber},,, Microsoft Corporation, Surface Laptop**</span><span class="sxs-lookup"><span data-stu-id="72772-203">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="72772-204">"Nombre del fabricante" y "modelo de dispositivo" distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="72772-204">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="72772-205">Si no sabe qué valor poner para el modelo de nombre de fabricante y dispositivo, puede ejecutarlo en el dispositivo para recopilar los valores correctos:</span><span class="sxs-lookup"><span data-stu-id="72772-205">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="72772-206">Descartado de CLUF de Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="72772-206">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="72772-207">INFORMACIÓN IMPORTANTE</span><span class="sxs-lookup"><span data-stu-id="72772-207">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="72772-208">Windows AutoPilot le permite configurar instalaciones personalizadas de Windows en los dispositivos que administra para sus clientes.</span><span class="sxs-lookup"><span data-stu-id="72772-208">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="72772-209">Si el cliente tiene autorización para hacerlo, puede suprimir u ocultar determinadas pantallas de configuración que se suelen presentar a los usuarios al configurar Windows, incluida la pantalla de aceptación del CLUF (contrato de licencia para el usuario final).</span><span class="sxs-lookup"><span data-stu-id="72772-209">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="72772-210">Mediante esta función, está de acuerdo en que suprimir u ocultar las pantallas que están diseñadas para proporcionar a los usuarios aviso o aceptación de términos significa que ha obtenido el consentimiento y la autorización suficientes del cliente para ocultar los términos, y que usted, en nombre de su cliente (ya sea una organización o un usuario individual como caso), da su consentimiento a los avisos y acepta los términos aplicables a su cliente.</span><span class="sxs-lookup"><span data-stu-id="72772-210">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="72772-211">Esto incluye el acuerdo con los términos y condiciones de la licencia o el aviso que se presentará al usuario si no lo suprime u oculta mediante esta herramienta.</span><span class="sxs-lookup"><span data-stu-id="72772-211">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="72772-212">Es posible que el cliente no use el software de Windows en dichos dispositivos si el cliente no ha adquirido una licencia para el software de Microsoft o sus distribuidores con licencia.</span><span class="sxs-lookup"><span data-stu-id="72772-212">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>
