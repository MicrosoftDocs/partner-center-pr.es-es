---
title: Administración de las ubicaciones en tu cuenta de partner
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Aprenda a agregar una nueva ubicación y cómo se usa el identificador de MPN de ubicación en programas de incentivos, empresas de CSP, suscripciones y otras transacciones.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702899"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="4a350-103">Administración de las ubicaciones de la cuenta de MPN y adición (eliminación) de una ubicación</span><span class="sxs-lookup"><span data-stu-id="4a350-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="4a350-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="4a350-104">**Appropriate roles**</span></span>

- <span data-ttu-id="4a350-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="4a350-105">Global admin</span></span>
- <span data-ttu-id="4a350-106">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="4a350-106">Account admin</span></span>

<span data-ttu-id="4a350-107">Los identificadores de MPN de ubicación identifican cada ubicación específica de la empresa.</span><span class="sxs-lookup"><span data-stu-id="4a350-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="4a350-108">Use el identificador de MPN de ubicación para inscribirse en programas de incentivos, para realizar transacciones de empresas del programa Proveedor de soluciones en la nube (CSP) y para otras transacciones comerciales.</span><span class="sxs-lookup"><span data-stu-id="4a350-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="4a350-109">El identificador de MPN global se usa para actividades no transaccionales, como las solicitudes de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="4a350-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-scenario-is-typical"></a><span data-ttu-id="4a350-110">El escenario siguiente es típico:</span><span class="sxs-lookup"><span data-stu-id="4a350-110">The following scenario is typical:</span></span>

<span data-ttu-id="4a350-111">Contoso tiene su cuenta global de partner (PGA) en el Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="4a350-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="4a350-112">La PGA es su empresa legal registrada, cuyo identificador de MPN global se usa para administrar todos los negocios no transaccionales.</span><span class="sxs-lookup"><span data-stu-id="4a350-112">The PGA is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="4a350-113">Contoso también tiene cuentas de ubicación de partner (PLA) equivalentes a subsidiarias o divisiones en otras ubicaciones del Reino Unido, Francia y EE. UU.</span><span class="sxs-lookup"><span data-stu-id="4a350-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="4a350-114">En la estructura de cuentas de MPN, estas PLA se representan como identificadores de MPN de ubicación únicos.</span><span class="sxs-lookup"><span data-stu-id="4a350-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="4a350-115">Las PLA se usan para negocios transaccionales, como los programas de CSP o de incentivos.</span><span class="sxs-lookup"><span data-stu-id="4a350-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="4a350-116">Los pagos están vinculados a ubicaciones específicas.</span><span class="sxs-lookup"><span data-stu-id="4a350-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="4a350-117">Hay una relación 1-1 entre un inquilino de CSP y un identificador de ubicación de MPN.</span><span class="sxs-lookup"><span data-stu-id="4a350-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Estructura de ubicaciones de MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="4a350-119">Requisitos previos para agregar una nueva cuenta para una empresa de CSP</span><span class="sxs-lookup"><span data-stu-id="4a350-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="4a350-120">Para agregar una nueva cuenta de empresa de CSP, empiece por asegurarse de cumplir los requisitos previos.</span><span class="sxs-lookup"><span data-stu-id="4a350-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="4a350-121">Debe tener un identificador de MPN de ubicación en el país en el que quiere hacer negocios de CSP.</span><span class="sxs-lookup"><span data-stu-id="4a350-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="4a350-122">Para crear una nueva ubicación de MPN, lea "Agregar una ubicación de MPN" a continuación.</span><span class="sxs-lookup"><span data-stu-id="4a350-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="4a350-123">Para crear una nueva inscripción de CSP Indirect Reseller, lea [Trabajar con proveedores indirectos](indirect-reseller-tasks-in-partner-center.md#get-started).</span><span class="sxs-lookup"><span data-stu-id="4a350-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="4a350-124">Recuerde iniciar sesión con las **nuevas** credenciales de la cuenta de CSP **nueva**.</span><span class="sxs-lookup"><span data-stu-id="4a350-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="4a350-125">No use las credenciales existentes, ya que el Centro de partners reconocerá que ya tiene una cuenta.</span><span class="sxs-lookup"><span data-stu-id="4a350-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="4a350-126">Acepte el contrato Microsoft Partner Agreement y active la cuenta.</span><span class="sxs-lookup"><span data-stu-id="4a350-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="4a350-127">Si desea inscribirse como partner de facturación directa, consulte [Requisitos para partners de facturación directa](direct-partner-new-requirements.md).</span><span class="sxs-lookup"><span data-stu-id="4a350-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-and-update-your-mpn-locations"></a><span data-ttu-id="4a350-128">Visualización y actualización de las ubicaciones de MPN</span><span class="sxs-lookup"><span data-stu-id="4a350-128">View and update your MPN locations</span></span>

1. <span data-ttu-id="4a350-129">Inicie sesión en el [panel](https://partner.microsoft.com/dashboard/home) del Centro de partners con las credenciales de la cuenta de MPN.</span><span class="sxs-lookup"><span data-stu-id="4a350-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="4a350-130">(Las credenciales de MPN pueden ser diferentes de las credenciales del programa CSP).</span><span class="sxs-lookup"><span data-stu-id="4a350-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="4a350-131">Desde el icono de **Configuración**, seleccione **Configuración de la cuenta**, **Perfil de la organización** y **Legal**.</span><span class="sxs-lookup"><span data-stu-id="4a350-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="4a350-132">En la pestaña **Asociado**, compruebe que no hay ningún mensaje de error de banner que le pida que corrija las ubicaciones migradas desde PMC.</span><span class="sxs-lookup"><span data-stu-id="4a350-132">On the **Partner** tab, verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span>  <span data-ttu-id="4a350-133">Si las ubicaciones no se configuraron correctamente en PMC y todavía no se han pasado al equipo, debe actualizarlas.</span><span class="sxs-lookup"><span data-stu-id="4a350-133">If your locations were not set up correctly in PMC, and have not transitioned yet to PC, you need to update those locations.</span></span>

:::image type="content" source="images/locations/location-two.png" alt-text="Captura de pantalla que muestra cómo actualizar la ubicación.":::
 
4.  <span data-ttu-id="4a350-135">En la pantalla **Revisar ubicaciones de PMC**, seleccione **Actualizar**.</span><span class="sxs-lookup"><span data-stu-id="4a350-135">On the **Review PMC locations** screen, select **Update**.</span></span>
<span data-ttu-id="4a350-136">Actualice los campos siguientes:</span><span class="sxs-lookup"><span data-stu-id="4a350-136">Update the following fields:</span></span>

- <span data-ttu-id="4a350-137">**Campo de nombre**: asegúrese de que el nombre de la ubicación de la compañía sea correcto.</span><span class="sxs-lookup"><span data-stu-id="4a350-137">**Name field**: Make sure that the name of the company location is correct.</span></span> <span data-ttu-id="4a350-138">Si se muestra un error duplicado, intente cambiar de Contoso a Contoso, Inc., por ejemplo.</span><span class="sxs-lookup"><span data-stu-id="4a350-138">If a duplicate error is displayed, try changing from, for example, Contoso to Contoso, Inc.</span></span>

- <span data-ttu-id="4a350-139">**Campo de entidad jurídica**: asegúrese de que ha elegido la entidad jurídica a la que está asociada la ubicación.</span><span class="sxs-lookup"><span data-stu-id="4a350-139">**Legal Entity field**: Make sure that you have chosen the legal entity the location is tied to</span></span>

- <span data-ttu-id="4a350-140">**Campos de línea de dirección 1 y 2**: asegúrese de que la dirección es correcta.</span><span class="sxs-lookup"><span data-stu-id="4a350-140">**Address line 1 & 2 fields**: Make sure that the address is correct</span></span>

- <span data-ttu-id="4a350-141">**Campos de ciudad y estado o provincia**: asegúrese de que la combinación entre la ciudad y el estado o provincia sea correcta.</span><span class="sxs-lookup"><span data-stu-id="4a350-141">**City & State/Province fields**: Make sure the combination between the city and the state/province is correct.</span></span> <span data-ttu-id="4a350-142">Hay países en los que se aplicará el menú desplegable para elegir el estado o provincia y, en otros, el campo tendrá que insertarse manualmente.</span><span class="sxs-lookup"><span data-stu-id="4a350-142">There are countries where the dropdown menu for choosing the State/Province will apply, and in other countries that field will need to manually be inserted.</span></span>

- <span data-ttu-id="4a350-143">**Campo de código postal**: asegúrese de que el campo Código postal coincida con el país, la región, la ciudad o la dirección indicados.</span><span class="sxs-lookup"><span data-stu-id="4a350-143">**ZIP/ Postal code field**: Make sure the Zip Code field is matching your indicated Country, Region, City, or Address.</span></span>

- <span data-ttu-id="4a350-144">**Campos de información de contacto principal**: asegúrese de que se rellenan los campos de nombre y apellidos y que la dirección de correo electrónico indicada es un correo electrónico del trabajo y no uno personal (por ejemplo, @outlook.com, @live.com, etc.).</span><span class="sxs-lookup"><span data-stu-id="4a350-144">**Primary contact information fields**: Make sure the first and last name fields are filled and that the e-mail address indicated is a work e-mail address and not a personal one (for example, @outlook.com, @live.com, etc.)</span></span>

- <span data-ttu-id="4a350-145">**Campo de número de teléfono**: asegúrese de que el número de teléfono no incluya caracteres especiales, espacios ni código de país.</span><span class="sxs-lookup"><span data-stu-id="4a350-145">**Phone number field**: Make sure that the Phone number does NOT include special characters, spaces, or country code.</span></span> <span data-ttu-id="4a350-146">El valor especificado en el campo de número de teléfono siempre contendrá un máximo de 10 caracteres.</span><span class="sxs-lookup"><span data-stu-id="4a350-146">The value entered in the Phone Number field will always contain a maximum of 10 characters.</span></span>

5. <span data-ttu-id="4a350-147">Si no hay ningún mensaje de error, desde **Configuración**, seleccione **Configuración de la cuenta**, **Perfil de la organización** e **Identificadores**.</span><span class="sxs-lookup"><span data-stu-id="4a350-147">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

6. <span data-ttu-id="4a350-148">Busque el id. de MPN con el tipo "Ubicación" que coincida con el país de esta cuenta de CSP y úselo para completar la asociación.</span><span class="sxs-lookup"><span data-stu-id="4a350-148">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to complete the association.</span></span>

7. <span data-ttu-id="4a350-149">Si no encuentra el id. de MPN de la ubicación que coincide con la cuenta de CSP que quiere usar, puede agregar una nueva ubicación que creará un nuevo id. de MPN.</span><span class="sxs-lookup"><span data-stu-id="4a350-149">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location, which will create a new MPN ID.</span></span> <span data-ttu-id="4a350-150">Consulte **Agregar una ubicación de MPN** a continuación.</span><span class="sxs-lookup"><span data-stu-id="4a350-150">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="4a350-151">Agregar una ubicación de MPN</span><span class="sxs-lookup"><span data-stu-id="4a350-151">Add an MPN location</span></span>

1. <span data-ttu-id="4a350-152">Iniciar sesión con la cuenta de MPN en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="4a350-152">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="4a350-153">(Las credenciales de MPN pueden ser diferentes de las credenciales del programa CSP).</span><span class="sxs-lookup"><span data-stu-id="4a350-153">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="4a350-154">La cuenta de MPN debe tener privilegios de administrador global o de cuenta.</span><span class="sxs-lookup"><span data-stu-id="4a350-154">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="4a350-155">Desde el **icono de Configuración**, seleccione **Configuración de la cuenta** y, a continuación, elija **Perfil de la organización**.</span><span class="sxs-lookup"><span data-stu-id="4a350-155">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="4a350-156">Seleccione **Legal** y, a continuación, en la pestaña **Partner**, seleccione **Ubicaciones de la empresa** y haga clic en **Agregar una ubicación**.</span><span class="sxs-lookup"><span data-stu-id="4a350-156">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="4a350-157">Proporcione los detalles necesarios, como el nombre, la dirección y el contacto de la empresa correspondientes a la ubicación que desea agregar a la empresa.</span><span class="sxs-lookup"><span data-stu-id="4a350-157">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="4a350-158">Haga clic en **Agregar ubicación**.</span><span class="sxs-lookup"><span data-stu-id="4a350-158">Click **Add location**.</span></span> <span data-ttu-id="4a350-159">Se creará un nuevo ID de MPN para la nueva ubicación, que puede utilizar para las transacciones y los incentivos del programa CSP.</span><span class="sxs-lookup"><span data-stu-id="4a350-159">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Agregar un nuevo perfil legal de la empresa":::

> [!NOTE]
> <span data-ttu-id="4a350-161">Una vez agregada una ubicación en el Centro de partners, no se puede quitar.</span><span class="sxs-lookup"><span data-stu-id="4a350-161">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="4a350-162">Verá **MPN** en el menú izquierdo del Centro de partners si ha usado el identificador de MPN correcto para iniciar sesión.</span><span class="sxs-lookup"><span data-stu-id="4a350-162">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="add-the-registration-number-id"></a><span data-ttu-id="4a350-163">Adición del identificador numérico de registro</span><span class="sxs-lookup"><span data-stu-id="4a350-163">Add the registration number ID</span></span>

<span data-ttu-id="4a350-164">Si es proveedor indirecto, partner de facturación directa o revendedor indirecto y hace negocios con clientes nuevos o existentes en los siguientes países, tiene que proporcionar los números de identificación del registro para su empresa.</span><span class="sxs-lookup"><span data-stu-id="4a350-164">If you are an Indirect provider, Direct bill partner, or Indirect reseller and you are doing business with new or existing customers in the following countries, you need to provide registration ID numbers for your business.</span></span> <span data-ttu-id="4a350-165">Si el país en el que hace negocios no aparece a continuación, la identificación del registro es opcional.</span><span class="sxs-lookup"><span data-stu-id="4a350-165">If the country you are doing business in is not listed below, the registration ID is optional.</span></span>

- <span data-ttu-id="4a350-166">Armenia</span><span class="sxs-lookup"><span data-stu-id="4a350-166">Armenia</span></span> 
- <span data-ttu-id="4a350-167">Azerbaiyán</span><span class="sxs-lookup"><span data-stu-id="4a350-167">Azerbaijan</span></span> 
- <span data-ttu-id="4a350-168">Belarús</span><span class="sxs-lookup"><span data-stu-id="4a350-168">Belarus</span></span> 
- <span data-ttu-id="4a350-169">Brasil</span><span class="sxs-lookup"><span data-stu-id="4a350-169">Brazil</span></span> 
- <span data-ttu-id="4a350-170">Hungría</span><span class="sxs-lookup"><span data-stu-id="4a350-170">Hungary</span></span> 
- <span data-ttu-id="4a350-171">India</span><span class="sxs-lookup"><span data-stu-id="4a350-171">India</span></span> 
- <span data-ttu-id="4a350-172">Iraq</span><span class="sxs-lookup"><span data-stu-id="4a350-172">Iraq</span></span> 
- <span data-ttu-id="4a350-173">Kazajistán</span><span class="sxs-lookup"><span data-stu-id="4a350-173">Kazakhstan</span></span> 
- <span data-ttu-id="4a350-174">Kirguistán</span><span class="sxs-lookup"><span data-stu-id="4a350-174">Kyrgyzstan</span></span> 
- <span data-ttu-id="4a350-175">Moldova</span><span class="sxs-lookup"><span data-stu-id="4a350-175">Moldova</span></span> 
- <span data-ttu-id="4a350-176">Myanmar</span><span class="sxs-lookup"><span data-stu-id="4a350-176">Myanmar</span></span> 
- <span data-ttu-id="4a350-177">Polonia</span><span class="sxs-lookup"><span data-stu-id="4a350-177">Poland</span></span> 
- <span data-ttu-id="4a350-178">Rusia</span><span class="sxs-lookup"><span data-stu-id="4a350-178">Russia</span></span> 
- <span data-ttu-id="4a350-179">Arabia Saudí</span><span class="sxs-lookup"><span data-stu-id="4a350-179">Saudi Arabia</span></span> 
- <span data-ttu-id="4a350-180">Sudáfrica</span><span class="sxs-lookup"><span data-stu-id="4a350-180">South Africa</span></span> 
- <span data-ttu-id="4a350-181">Sudán del Sur</span><span class="sxs-lookup"><span data-stu-id="4a350-181">South Sudan</span></span>  
- <span data-ttu-id="4a350-182">Tayikistán</span><span class="sxs-lookup"><span data-stu-id="4a350-182">Tajikistan</span></span> 
- <span data-ttu-id="4a350-183">Tailandia</span><span class="sxs-lookup"><span data-stu-id="4a350-183">Thailand</span></span>
- <span data-ttu-id="4a350-184">Turquía</span><span class="sxs-lookup"><span data-stu-id="4a350-184">Turkey</span></span> 
- <span data-ttu-id="4a350-185">Ucrania</span><span class="sxs-lookup"><span data-stu-id="4a350-185">Ukraine</span></span> 
- <span data-ttu-id="4a350-186">Emiratos Árabes Unidos</span><span class="sxs-lookup"><span data-stu-id="4a350-186">United Arab Emirates</span></span> 
- <span data-ttu-id="4a350-187">Uzbekistán</span><span class="sxs-lookup"><span data-stu-id="4a350-187">Uzbekistan</span></span> 
- <span data-ttu-id="4a350-188">Venezuela</span><span class="sxs-lookup"><span data-stu-id="4a350-188">Venezuela</span></span>
- <span data-ttu-id="4a350-189">Vietnam</span><span class="sxs-lookup"><span data-stu-id="4a350-189">Vietnam</span></span> 


<span data-ttu-id="4a350-190">Para obtener más información, lea [Información del id. de registro.](reg-number-id.md)</span><span class="sxs-lookup"><span data-stu-id="4a350-190">For more information, read [Registration ID number information](reg-number-id.md)</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="4a350-191">Eliminación de una ubicación</span><span class="sxs-lookup"><span data-stu-id="4a350-191">Delete a location</span></span>

<span data-ttu-id="4a350-192">Para eliminar una ubicación de la cuenta, deberá ponerse en contacto con el [servicio de soporte técnico para asociados](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="4a350-192">To delete a location from your account, you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="4a350-193">Asegúrese de que comprende el impacto que tiene esta acción.</span><span class="sxs-lookup"><span data-stu-id="4a350-193">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="4a350-194">Las ubicaciones eliminadas no se pueden recuperar y todo lo relacionado con ese id. de MPN específico ya no se reconocerá ni estará activo para la empresa.</span><span class="sxs-lookup"><span data-stu-id="4a350-194">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="4a350-195">Cambiar el país de la cuenta global del asociado</span><span class="sxs-lookup"><span data-stu-id="4a350-195">Change country of Partner global account</span></span> 

1. <span data-ttu-id="4a350-196">Iniciar sesión con la cuenta de MPN en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="4a350-196">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="4a350-197">(Las credenciales de MPN pueden ser diferentes de las credenciales del programa CSP).</span><span class="sxs-lookup"><span data-stu-id="4a350-197">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="4a350-198">La cuenta de MPN debe tener privilegios de administrador global o de cuenta.</span><span class="sxs-lookup"><span data-stu-id="4a350-198">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="4a350-199">En la pestaña **Partner**, diríjase a **Ubicaciones de la empresa** y compruebe la lista de ubicaciones para asegurarse de que se muestra la ubicación que quiere como entidad jurídica.</span><span class="sxs-lookup"><span data-stu-id="4a350-199">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="4a350-200">Para agregar una ubicación, haga clic en **Agregar una ubicación** y, en el control flotante, proporcione los detalles necesarios, como el nombre, la dirección y el contacto principal de la empresa correspondientes a la ubicación que desea agregar a la empresa.</span><span class="sxs-lookup"><span data-stu-id="4a350-200">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="4a350-201">Seleccione **Cambiar el país** junto al menú desplegable **País o región** y siga los pasos que se indican.</span><span class="sxs-lookup"><span data-stu-id="4a350-201">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Control flotante de datos del perfil legal de la empresa":::

5. <span data-ttu-id="4a350-203">Haga clic en **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="4a350-203">Click **Save**.</span></span>

6. <span data-ttu-id="4a350-204">El país de la cuenta global de MPN se cambiará por el país del nuevo perfil legal.</span><span class="sxs-lookup"><span data-stu-id="4a350-204">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="4a350-205">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="4a350-205">Next steps</span></span>

- <span data-ttu-id="4a350-206">Obtenga más información acerca del [proceso de verificación](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="4a350-206">Learn about the [verification process](verification-responses.md).</span></span>
