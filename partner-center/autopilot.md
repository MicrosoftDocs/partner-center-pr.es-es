---
title: Personalización de la experiencia de configuración de un dispositivo
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Antes de entregar el nuevo dispositivo de un cliente, puede usar perfiles de Windows Autopilot para personalizar o configurar previamente la experiencia de configuración (OOBE) del dispositivo.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 5294495403be729adecb5a7814ade4f9d454a0f6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149832"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="e97fe-103">Usar perfiles de Windows Autopilot en dispositivos nuevos para personalizar la experiencia rápida de un cliente</span><span class="sxs-lookup"><span data-stu-id="e97fe-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="e97fe-104">**Roles adecuados:** agente de administración | Administrador global | Agente de ventas | Administrador de administración de usuarios</span><span class="sxs-lookup"><span data-stu-id="e97fe-104">**Appropriate roles**: Admin agent | Global admin | Sales agent | User management admin</span></span>

<span data-ttu-id="e97fe-105">Si administra dispositivos de cliente, es posible que tenga que personalizar la experiencia personalizada (OOBE) para los usuarios del cliente.</span><span class="sxs-lookup"><span data-stu-id="e97fe-105">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="e97fe-106">Puede configurar previamente nuevos dispositivos con Windows Autopilot antes de entregar los dispositivos a los clientes y aplicar nuevos perfiles a los dispositivos que los clientes ya han adquirido.</span><span class="sxs-lookup"><span data-stu-id="e97fe-106">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="e97fe-107">Tenga en cuenta que los OEM han empezado a incluir una etiqueta de envío en el exterior de la caja del dispositivo Autopilot que muestra el identificador de clave de producto **(PKID) del dispositivo.**</span><span class="sxs-lookup"><span data-stu-id="e97fe-107">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="e97fe-108">Este código de barras 1 dimensional y legible proporciona a los asociados de nivel inferior una manera de registrar dispositivos para Autopilot sin tener que desboxear los dispositivos y recolección del identificador de dispositivo por medios alternativos.</span><span class="sxs-lookup"><span data-stu-id="e97fe-108">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="e97fe-109">En este artículo se explica cómo crear y aplicar perfiles de Autopilot a dispositivos de Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="e97fe-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="e97fe-110">Si aún no está familiarizado con Autopilot, revise la información de estos artículos:</span><span class="sxs-lookup"><span data-stu-id="e97fe-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="e97fe-111">Información general de Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="e97fe-111">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="e97fe-112">Guía de referencia de implementación de Autopilot</span><span class="sxs-lookup"><span data-stu-id="e97fe-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="e97fe-113">Información general</span><span class="sxs-lookup"><span data-stu-id="e97fe-113">Overview</span></span>

<span data-ttu-id="e97fe-114">Con la Windows Autopilot en Centro de partners, puede crear perfiles personalizados para aplicarlos a los dispositivos del cliente.</span><span class="sxs-lookup"><span data-stu-id="e97fe-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="e97fe-115">La siguiente configuración de perfil estaba disponible en el momento en que se publicó este artículo:</span><span class="sxs-lookup"><span data-stu-id="e97fe-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="e97fe-116">Omitir la configuración de privacidad.</span><span class="sxs-lookup"><span data-stu-id="e97fe-116">Skip privacy settings.</span></span> <span data-ttu-id="e97fe-117">Esta configuración de perfil opcional de Autopilot permite a las organizaciones no preguntar sobre la configuración de privacidad durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="e97fe-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="e97fe-118">Deshabilite la creación de cuentas de administrador local en el dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e97fe-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="e97fe-119">Las organizaciones pueden decidir si el usuario que configura el dispositivo debe tener acceso de administrador una vez completado el proceso.</span><span class="sxs-lookup"><span data-stu-id="e97fe-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="e97fe-120">Configure automáticamente el dispositivo para el trabajo o la escuela.</span><span class="sxs-lookup"><span data-stu-id="e97fe-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="e97fe-121">Todos los dispositivos registrados con Autopilot se considerarán automáticamente dispositivos de trabajo o educativos, por lo que esta pregunta no se hará durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="e97fe-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="e97fe-122">Omita las páginas de configuración de registro de Cortana, OneDrive y OEM.</span><span class="sxs-lookup"><span data-stu-id="e97fe-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="e97fe-123">Todos los dispositivos registrados con Autopilot omitirán automáticamente estas páginas durante el proceso de configuración automática (OOBE).</span><span class="sxs-lookup"><span data-stu-id="e97fe-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="e97fe-124">Omitir el Contrato de licencia del usuario final (CLUF).</span><span class="sxs-lookup"><span data-stu-id="e97fe-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="e97fe-125">A partir Windows 10 versión 1709, las organizaciones pueden decidir omitir la página del CLUF presentada durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="e97fe-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="e97fe-126">Consulte [Windows Autopilot licencia del CLUF](#windows-autopilot-eula-dismissal) a continuación para obtener información importante a tener en cuenta sobre la omisión de la página clufór durante la instalación de Windows.</span><span class="sxs-lookup"><span data-stu-id="e97fe-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="e97fe-127">Se aplican las siguientes limitaciones y permisos de administración de perfiles y dispositivos:</span><span class="sxs-lookup"><span data-stu-id="e97fe-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="e97fe-128">Los asociados de CSP pueden seguir administrando los perfiles de Autopilot para los clientes existentes con quienes tienen relaciones de revendedor, incluso si los clientes han quitado los privilegios de administración delegada del asociado.</span><span class="sxs-lookup"><span data-stu-id="e97fe-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="e97fe-129">Puede administrar los dispositivos existentes para los clientes que ha agregado.</span><span class="sxs-lookup"><span data-stu-id="e97fe-129">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="e97fe-130">No puede administrar los dispositivos que el cliente ha cargado en Microsoft Store para empresas o en el portal de Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="e97fe-130">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="e97fe-131">Creación y administración de perfiles de Autopilot en Centro de partners</span><span class="sxs-lookup"><span data-stu-id="e97fe-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="e97fe-132">En Centro de partners, puede crear perfiles de Windows Autopilot y aplicarlos a los dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e97fe-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="e97fe-133">Solo los agentes de administración pueden crear y aplicar perfiles.</span><span class="sxs-lookup"><span data-stu-id="e97fe-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="e97fe-134">Creación de un nuevo perfil de Autopilot</span><span class="sxs-lookup"><span data-stu-id="e97fe-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="e97fe-135">Seleccione **Clientes** en el Centro de partners y, a continuación, seleccione el cliente para el que va a crear el perfil de Autopilot.</span><span class="sxs-lookup"><span data-stu-id="e97fe-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="e97fe-136">En la página de detalles del cliente, seleccione **Dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="e97fe-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="e97fe-137">En **Windows Autopilot perfiles,** seleccione **Agregar nuevo perfil.**</span><span class="sxs-lookup"><span data-stu-id="e97fe-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="e97fe-138">Escriba el nombre y la descripción del perfil y, a continuación, configure los valores de OOBE.</span><span class="sxs-lookup"><span data-stu-id="e97fe-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="e97fe-139">Elija de entre las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="e97fe-139">Choose from:</span></span>  

   - <span data-ttu-id="e97fe-140">Omitir la configuración de privacidad en la configuración</span><span class="sxs-lookup"><span data-stu-id="e97fe-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="e97fe-141">Deshabilitación de la cuenta de administrador local en la instalación</span><span class="sxs-lookup"><span data-stu-id="e97fe-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="e97fe-142">Omitir páginas automáticamente en la configuración</span><span class="sxs-lookup"><span data-stu-id="e97fe-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="e97fe-143">(Incluye *Seleccionar automáticamente la configuración para el trabajo* o la escuela y omitir las páginas de configuración de registro de *Cortana, OneDrive y OEM)*</span><span class="sxs-lookup"><span data-stu-id="e97fe-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="e97fe-144">Omitir el contrato de licencia del usuario final (CLUF)</span><span class="sxs-lookup"><span data-stu-id="e97fe-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="e97fe-145">Consulte [Windows Autopilot licencia del CLUF](#windows-autopilot-eula-dismissal) a continuación para obtener información importante a tener en cuenta sobre la omisión de la página clufór durante la instalación de Windows.</span><span class="sxs-lookup"><span data-stu-id="e97fe-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="e97fe-146">Seleccione **Enviar** cuando haya terminado.</span><span class="sxs-lookup"><span data-stu-id="e97fe-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="e97fe-147">Aplicación de un perfil de Autopilot a dispositivos de cliente</span><span class="sxs-lookup"><span data-stu-id="e97fe-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="e97fe-148">En las instrucciones siguientes se supone que ya ha agregado los dispositivos del cliente a Centro de partners y que puede acceder a su lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e97fe-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="e97fe-149">Si aún no ha agregado los dispositivos del cliente, siga las instrucciones de Adición de dispositivos a la cuenta de un cliente y, [a](#add-devices-to-a-customers-account) continuación, siga los pasos que se indican a continuación.</span><span class="sxs-lookup"><span data-stu-id="e97fe-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="e97fe-150">Después de crear un perfil de Autopilot para un cliente, puede aplicarlo a los dispositivos del cliente.</span><span class="sxs-lookup"><span data-stu-id="e97fe-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="e97fe-151">Seleccione **Clientes** en el menú Centro de partners y, a continuación, seleccione el cliente para el que creó el perfil de Autopilot.</span><span class="sxs-lookup"><span data-stu-id="e97fe-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="e97fe-152">En la página de detalles del cliente, seleccione **Dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="e97fe-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="e97fe-153">En **Aplicar perfiles a dispositivos,** seleccione los dispositivos o grupos de dispositivos a los que desea agregar perfiles y, a continuación, **seleccione Aplicar perfil.**</span><span class="sxs-lookup"><span data-stu-id="e97fe-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="e97fe-154">El perfil que acaba de aplicar aparece en la **columna** Perfil.</span><span class="sxs-lookup"><span data-stu-id="e97fe-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="e97fe-155">Siga estos pasos para comprobar que el perfil se aplicará correctamente al dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e97fe-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="e97fe-156">a.</span><span class="sxs-lookup"><span data-stu-id="e97fe-156">a.</span></span>  <span data-ttu-id="e97fe-157">Conecte un dispositivo a la red y encándalo.</span><span class="sxs-lookup"><span data-stu-id="e97fe-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="e97fe-158">b.</span><span class="sxs-lookup"><span data-stu-id="e97fe-158">b.</span></span>  <span data-ttu-id="e97fe-159">Compruebe que aparecen las pantallas de OOBE adecuadas (si las hay).</span><span class="sxs-lookup"><span data-stu-id="e97fe-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="e97fe-160">c.</span><span class="sxs-lookup"><span data-stu-id="e97fe-160">c.</span></span>  <span data-ttu-id="e97fe-161">Cuando se detenga el proceso de OOBE, restablezca el dispositivo a su configuración predeterminada de fábrica para prepararlo para un nuevo usuario.</span><span class="sxs-lookup"><span data-stu-id="e97fe-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="e97fe-162">Eliminación de un perfil de Autopilot del dispositivo de un cliente</span><span class="sxs-lookup"><span data-stu-id="e97fe-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="e97fe-163">Seleccione **Clientes** en el menú Centro de partners y, a continuación, seleccione el cliente para el que creó el perfil de Autopilot.</span><span class="sxs-lookup"><span data-stu-id="e97fe-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="e97fe-164">En la página de detalles del cliente, seleccione **Dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="e97fe-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="e97fe-165">En **Aplicar perfiles a dispositivos,** seleccione los dispositivos de los que desea quitar el perfil y, a continuación, **seleccione Quitar perfil.**</span><span class="sxs-lookup"><span data-stu-id="e97fe-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="e97fe-166">La eliminación de un perfil de un dispositivo no elimina el perfil de la lista.</span><span class="sxs-lookup"><span data-stu-id="e97fe-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="e97fe-167">Si desea eliminar un perfil, siga las instrucciones de [Actualización o eliminación de un perfil de Autopilot.](#update-or-delete-an-autopilot-profile)</span><span class="sxs-lookup"><span data-stu-id="e97fe-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="e97fe-168">Actualización o eliminación de un perfil de Autopilot</span><span class="sxs-lookup"><span data-stu-id="e97fe-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="e97fe-169">Si un cliente desea cambiar la experiencia lista para usar después de haberle enviado los dispositivos, puede cambiar el perfil en Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="e97fe-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="e97fe-170">Cuando el dispositivo del cliente se conecte a Internet, descargará la versión más reciente del perfil durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="e97fe-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="e97fe-171">Además, cada vez que un cliente restaura un dispositivo a su configuración predeterminada de fábrica, el dispositivo descargará de nuevo la versión más reciente del perfil durante el proceso de OOBE.</span><span class="sxs-lookup"><span data-stu-id="e97fe-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="e97fe-172">Seleccione **Clientes** en el Centro de partners y, a continuación, seleccione el cliente que quiere que cambie un perfil de Autopilot.</span><span class="sxs-lookup"><span data-stu-id="e97fe-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="e97fe-173">En la página de detalles del cliente, seleccione **Dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="e97fe-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="e97fe-174">En **Windows Autopilot perfiles,** seleccione el perfil que necesita actualizar.</span><span class="sxs-lookup"><span data-stu-id="e97fe-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="e97fe-175">Realice los cambios necesarios y, a continuación, **seleccione Enviar**.</span><span class="sxs-lookup"><span data-stu-id="e97fe-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="e97fe-176">Para eliminar este perfil, seleccione **Eliminar perfil** en la esquina superior derecha de la página.</span><span class="sxs-lookup"><span data-stu-id="e97fe-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="e97fe-177">Agregar dispositivos a la cuenta de un cliente</span><span class="sxs-lookup"><span data-stu-id="e97fe-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="e97fe-178">Los agentes de ventas y los agentes de administración pueden agregar dispositivos a la cuenta de un cliente.</span><span class="sxs-lookup"><span data-stu-id="e97fe-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="e97fe-179">Para poder aplicar perfiles personalizados de Autopilot a los dispositivos del cliente, debe poder acceder a la lista de dispositivos del cliente.</span><span class="sxs-lookup"><span data-stu-id="e97fe-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="e97fe-180">Si tiene previsto usar el nombre de OEM, el número de serie y la combinación de modelos, tenga en cuenta estas limitaciones:</span><span class="sxs-lookup"><span data-stu-id="e97fe-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="e97fe-181">Esta tupla solo funciona para dispositivos más recientes (hashes de 4k, por ejemplo) y no se admite para hashes 128b (RS2 y dispositivos anteriores).</span><span class="sxs-lookup"><span data-stu-id="e97fe-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="e97fe-182">El registro de tupla distingue mayúsculas de minúsculas, por  lo que los datos del archivo deben coincidir exactamente con los nombres de modelo y fabricante proporcionados por el proveedor oem (proveedor de hardware).</span><span class="sxs-lookup"><span data-stu-id="e97fe-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="e97fe-183">Siga las instrucciones siguientes para agregar dispositivos a la cuenta de un cliente en Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="e97fe-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="e97fe-184">Seleccione **Clientes** en el Centro de partners y, a continuación, seleccione el cliente cuyos dispositivos desea administrar.</span><span class="sxs-lookup"><span data-stu-id="e97fe-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="e97fe-185">En la página de detalles del cliente, seleccione **Dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="e97fe-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="e97fe-186">En **Aplicar perfiles a dispositivos,** **seleccione Agregar dispositivos.**</span><span class="sxs-lookup"><span data-stu-id="e97fe-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="e97fe-187">Escriba un nombre para la  lista de dispositivos y, a continuación, seleccione Examinar para cargar la lista del cliente (en formato de archivo .csv) para Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="e97fe-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="e97fe-188">Debería haber recibido este archivo .csv con la compra del dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e97fe-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="e97fe-189">Si no recibió un archivo .csv, puede crear uno usted mismo siguiendo los pasos descritos en Incorporación de dispositivos a [Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="e97fe-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="e97fe-190">Cargue el archivo .csv y seleccione **Guardar.**</span><span class="sxs-lookup"><span data-stu-id="e97fe-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="e97fe-191">Si recibe un mensaje de error al intentar cargar el archivo .csv, compruebe el formato del archivo.</span><span class="sxs-lookup"><span data-stu-id="e97fe-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="e97fe-192">Solo puede utilizar el hash de hardware, el nombre de OEM, el número de serie y el modelo (en ese orden de columna), o el identificador de producto de Windows.</span><span class="sxs-lookup"><span data-stu-id="e97fe-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="e97fe-193">También puede usar el archivo .csv de ejemplo proporcionado en el vínculo junto a **Agregar dispositivos** para crear una lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e97fe-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="e97fe-194">El archivo .csv debe tener un aspecto parecido al siguiente:</span><span class="sxs-lookup"><span data-stu-id="e97fe-194">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="e97fe-195">**Número de serie del dispositivo, id. de producto de Windows, hash de hardware, nombre del fabricante, modelo de dispositivo**</span><span class="sxs-lookup"><span data-stu-id="e97fe-195">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="e97fe-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span><span class="sxs-lookup"><span data-stu-id="e97fe-196">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="e97fe-197">"Nombre de fabricante" y "Modelo de dispositivo" distinguen mayúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="e97fe-197">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="e97fe-198">Si no sabe qué valor se debe colocar para el nombre del fabricante y el modelo de dispositivo, puede ejecutarlo en el dispositivo para recopilar los valores correctos:</span><span class="sxs-lookup"><span data-stu-id="e97fe-198">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="e97fe-199">Windows Autopilot del CLUF</span><span class="sxs-lookup"><span data-stu-id="e97fe-199">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="e97fe-200">INFORMACIÓN IMPORTANTE</span><span class="sxs-lookup"><span data-stu-id="e97fe-200">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="e97fe-201">Windows Autopilot permite configurar instalaciones personalizadas de Windows en dispositivos que administra para los clientes.</span><span class="sxs-lookup"><span data-stu-id="e97fe-201">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="e97fe-202">Si el cliente lo autoriza, puede suprimir u ocultar determinadas pantallas de configuración que normalmente se presentan a los usuarios al configurar Windows, incluida la pantalla de aceptación del CLUF (Contrato de licencia del usuario final).</span><span class="sxs-lookup"><span data-stu-id="e97fe-202">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="e97fe-203">Al usar esta función, acepta que suprimir u ocultar las pantallas diseñadas para proporcionar a los usuarios el aviso o la aceptación de los términos significa que ha obtenido el consentimiento y la autorización suficientes del cliente para ocultar los términos, y que usted, en nombre del cliente (ya sea una organización o un usuario individual según sea el caso), da su consentimiento a los avisos y acepta los términos aplicables a su cliente.</span><span class="sxs-lookup"><span data-stu-id="e97fe-203">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="e97fe-204">Esto incluye el acuerdo con los términos y condiciones de la licencia o el aviso que se presentaría al usuario si no lo suprimió u ocultó mediante esta herramienta.</span><span class="sxs-lookup"><span data-stu-id="e97fe-204">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="e97fe-205">El cliente no puede usar el software de Windows en esos dispositivos si el cliente no ha adquirido válidamente una licencia para el software de Microsoft o sus distribuidores con licencia.</span><span class="sxs-lookup"><span data-stu-id="e97fe-205">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>