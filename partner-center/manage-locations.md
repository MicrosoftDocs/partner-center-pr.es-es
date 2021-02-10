---
title: Administración de las ubicaciones en tu cuenta de partner
ms.topic: how-to
ms.date: 02/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Aprenda a agregar una nueva ubicación y cómo se usa el identificador de MPN de ubicación en programas de incentivos, empresas de CSP, suscripciones y otras transacciones.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 41ffaeaf0fb46659142949872295523546bb91c1
ms.sourcegitcommit: 5768f10cd122a20fe3df3062ea34e7096d99f639
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/09/2021
ms.locfileid: "100005915"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a><span data-ttu-id="892ae-103">Administración de las ubicaciones de la cuenta de MPN y adición (eliminación) de una ubicación</span><span class="sxs-lookup"><span data-stu-id="892ae-103">Manage your MPN account locations and add (delete) a location</span></span>


<span data-ttu-id="892ae-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="892ae-104">**Appropriate roles**</span></span>

- <span data-ttu-id="892ae-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="892ae-105">Global admin</span></span>
- <span data-ttu-id="892ae-106">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="892ae-106">Account admin</span></span>

<span data-ttu-id="892ae-107">Los identificadores de MPN de ubicación identifican cada ubicación específica de la empresa.</span><span class="sxs-lookup"><span data-stu-id="892ae-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="892ae-108">Use el identificador de MPN de ubicación para inscribirse en programas de incentivos, para realizar transacciones de empresas del programa Proveedor de soluciones en la nube (CSP) y para otras transacciones comerciales.</span><span class="sxs-lookup"><span data-stu-id="892ae-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="892ae-109">El identificador de MPN global se usa para actividades no transaccionales, como las solicitudes de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="892ae-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="892ae-110">El siguiente ejemplo es un escenario típico:</span><span class="sxs-lookup"><span data-stu-id="892ae-110">The following is a typical scenario:</span></span>

<span data-ttu-id="892ae-111">Contoso tiene su cuenta global de partner (PGA) en el Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="892ae-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="892ae-112">Se trata de su empresa legal registrada, cuyo identificador de MPN global se usa para administrar todos los negocios no transaccionales.</span><span class="sxs-lookup"><span data-stu-id="892ae-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="892ae-113">Contoso también tiene cuentas de ubicación de partner (PLA) equivalentes a subsidiarias o divisiones en otras ubicaciones del Reino Unido, Francia y EE. UU.</span><span class="sxs-lookup"><span data-stu-id="892ae-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="892ae-114">En la estructura de cuentas de MPN, estas PLA se representan como identificadores de MPN de ubicación únicos.</span><span class="sxs-lookup"><span data-stu-id="892ae-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="892ae-115">Las PLA se usan para negocios transaccionales, como los programas de CSP o de incentivos.</span><span class="sxs-lookup"><span data-stu-id="892ae-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="892ae-116">Los pagos están vinculados a ubicaciones específicas.</span><span class="sxs-lookup"><span data-stu-id="892ae-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="892ae-117">Hay una relación 1-1 entre un inquilino de CSP y un identificador de ubicación de MPN.</span><span class="sxs-lookup"><span data-stu-id="892ae-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Estructura de ubicaciones de MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a><span data-ttu-id="892ae-119">Requisitos previos para agregar una nueva cuenta para una empresa de CSP</span><span class="sxs-lookup"><span data-stu-id="892ae-119">Prerequisites in order to add a new account for a CSP business</span></span>

<span data-ttu-id="892ae-120">Para agregar una nueva cuenta de empresa de CSP, empiece por asegurarse de cumplir los requisitos previos.</span><span class="sxs-lookup"><span data-stu-id="892ae-120">To add a new CSP business account, start by ensuring that you have fulfilled the prerequisites.</span></span>

1. <span data-ttu-id="892ae-121">Debe tener un identificador de MPN de ubicación en el país en el que quiere hacer negocios de CSP.</span><span class="sxs-lookup"><span data-stu-id="892ae-121">You must have a location MPN ID in the country where you want to do CSP business.</span></span> <span data-ttu-id="892ae-122">Para crear una nueva ubicación de MPN, lea "Agregar una ubicación de MPN" a continuación.</span><span class="sxs-lookup"><span data-stu-id="892ae-122">To create a new MPN location, read “Add an MPN location” below.</span></span>
  
1. <span data-ttu-id="892ae-123">Para crear una nueva inscripción de CSP Indirect Reseller, lea [Trabajar con proveedores indirectos](indirect-reseller-tasks-in-partner-center.md#get-started).</span><span class="sxs-lookup"><span data-stu-id="892ae-123">To create a new CSP Indirect Reseller enrollment, read [Work with Indirect providers](indirect-reseller-tasks-in-partner-center.md#get-started)</span></span> 

>[!NOTE] 
 ><span data-ttu-id="892ae-124">Recuerde iniciar sesión con las **nuevas** credenciales de la cuenta de CSP **nueva**.</span><span class="sxs-lookup"><span data-stu-id="892ae-124">Remember to sign in with the **new** credentials for the **new** CSP account.</span></span> <span data-ttu-id="892ae-125">No use las credenciales existentes, ya que el Centro de partners reconocerá que ya tiene una cuenta.</span><span class="sxs-lookup"><span data-stu-id="892ae-125">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

2. <span data-ttu-id="892ae-126">Acepte el contrato Microsoft Partner Agreement y active la cuenta.</span><span class="sxs-lookup"><span data-stu-id="892ae-126">Accept the Microsoft Partner Agreement and activate the account.</span></span>

1. <span data-ttu-id="892ae-127">Si desea inscribirse como partner de facturación directa, consulte [Requisitos para partners de facturación directa](direct-partner-new-requirements.md).</span><span class="sxs-lookup"><span data-stu-id="892ae-127">If you want to enroll as a Direct Bill partner, read [Requirements for Direct Bill partners](direct-partner-new-requirements.md)</span></span>

## <a name="view-your-mpn-locations"></a><span data-ttu-id="892ae-128">Visualización de las ubicaciones de MPN</span><span class="sxs-lookup"><span data-stu-id="892ae-128">View your MPN locations</span></span>

1. <span data-ttu-id="892ae-129">Inicie sesión en el [panel](https://partner.microsoft.com/dashboard/home) del Centro de partners con las credenciales de la cuenta de MPN.</span><span class="sxs-lookup"><span data-stu-id="892ae-129">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) with your MPN account credentials.</span></span> <span data-ttu-id="892ae-130">(Las credenciales de MPN pueden ser diferentes de las credenciales del programa CSP).</span><span class="sxs-lookup"><span data-stu-id="892ae-130">(Your MPN credentials may be different from your CSP credentials)</span></span> 
 
1. <span data-ttu-id="892ae-131">Desde el icono de **Configuración**, seleccione **Configuración de la cuenta**, **Perfil de la organización** y **Legal**.</span><span class="sxs-lookup"><span data-stu-id="892ae-131">From the **Settings** icon, select **Account settings**, **Organization profile**, **Legal**.</span></span> 

1. <span data-ttu-id="892ae-132">En la pestaña **Partner**, compruebe que no hay ningún mensaje de error de banner que le pida que corrija las ubicaciones migradas desde PMC.</span><span class="sxs-lookup"><span data-stu-id="892ae-132">On the **Partner** tab verify that there isn't a banner error message asking you to fix migrated locations from PMC.</span></span> <span data-ttu-id="892ae-133">Si es así, siga las instrucciones y corrija dichas ubicaciones.</span><span class="sxs-lookup"><span data-stu-id="892ae-133">If there is, follow instructions and fix those locations.</span></span> 

3. <span data-ttu-id="892ae-134">Si no hay ningún mensaje de error, desde **Configuración**, seleccione **Configuración de la cuenta**, **Perfil de la organización** e **Identificadores**.</span><span class="sxs-lookup"><span data-stu-id="892ae-134">If there isn't an error message, then from  **Settings**, select  **Account Settings**, **Organization profile**, **Identifiers**.</span></span>

4. <span data-ttu-id="892ae-135">Busque el id. de MPN con el tipo "Ubicación" que coincida con el país de esta cuenta de CSP y úselo para realizar la búsqueda a continuación y completar la asociación.</span><span class="sxs-lookup"><span data-stu-id="892ae-135">Find the MPN ID with Type "Location" that matches the country of this CSP account and use it to search below and complete association.</span></span>

5. <span data-ttu-id="892ae-136">Si no encuentra el id. de MPN de la ubicación que coincide con la cuenta de CSP que quiere usar, puede agregar una nueva ubicación que creará un nuevo id. de MPN.</span><span class="sxs-lookup"><span data-stu-id="892ae-136">If you can’t find the location MPN ID that matches the CSP account you want to use, you can add a new location which will create a new MPN ID.</span></span> <span data-ttu-id="892ae-137">Consulte **Agregar una ubicación de MPN** a continuación.</span><span class="sxs-lookup"><span data-stu-id="892ae-137">See **Add an MPN location** below.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="892ae-138">Agregar una ubicación de MPN</span><span class="sxs-lookup"><span data-stu-id="892ae-138">Add an MPN location</span></span>

1. <span data-ttu-id="892ae-139">Iniciar sesión con la cuenta de MPN en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="892ae-139">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="892ae-140">(Las credenciales de MPN pueden ser diferentes de las credenciales del programa CSP).</span><span class="sxs-lookup"><span data-stu-id="892ae-140">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="892ae-141">La cuenta de MPN debe tener privilegios de administrador global o de cuenta.</span><span class="sxs-lookup"><span data-stu-id="892ae-141">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="892ae-142">Desde el **icono de Configuración**, seleccione **Configuración de la cuenta** y, a continuación, elija **Perfil de la organización**.</span><span class="sxs-lookup"><span data-stu-id="892ae-142">From the **Settings icon**, select the **Account settings** and then select **Organization profile**.</span></span>

2. <span data-ttu-id="892ae-143">Seleccione **Legal** y, a continuación, en la pestaña **Partner**, seleccione **Ubicaciones de la empresa** y haga clic en **Agregar una ubicación**.</span><span class="sxs-lookup"><span data-stu-id="892ae-143">Select **Legal** and then, on the **Partner** tab, select **Business locations,** and click on **Add a location.**</span></span>

3. <span data-ttu-id="892ae-144">Proporcione los detalles necesarios, como el nombre, la dirección y el contacto de la empresa correspondientes a la ubicación que desea agregar a la empresa.</span><span class="sxs-lookup"><span data-stu-id="892ae-144">Provide the required details including business name, address, and contact for the location that you want to add to your company.</span></span>
 
1. <span data-ttu-id="892ae-145">Haga clic en **Agregar ubicación**.</span><span class="sxs-lookup"><span data-stu-id="892ae-145">Click **Add location**.</span></span> <span data-ttu-id="892ae-146">Se creará un nuevo ID de MPN para la nueva ubicación, que puede utilizar para las transacciones y los incentivos del programa CSP.</span><span class="sxs-lookup"><span data-stu-id="892ae-146">This will create a new MPN ID for the new location which you can use for CSP transactions and incentives.</span></span>

:::image type="content" source="images/legal-biz.png" alt-text="Agregar un nuevo perfil legal de la empresa":::

> [!NOTE]
> <span data-ttu-id="892ae-148">Una vez agregada una ubicación en el Centro de partners, no se puede quitar.</span><span class="sxs-lookup"><span data-stu-id="892ae-148">Once a location is added in Partner Center, you cannot remove it.</span></span> <span data-ttu-id="892ae-149">Verá **MPN** en el menú izquierdo del Centro de partners si ha usado el identificador de MPN correcto para iniciar sesión.</span><span class="sxs-lookup"><span data-stu-id="892ae-149">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="delete-a-location"></a><span data-ttu-id="892ae-150">Eliminación de una ubicación</span><span class="sxs-lookup"><span data-stu-id="892ae-150">Delete a location</span></span>

<span data-ttu-id="892ae-151">Para eliminar una ubicación de la cuenta, deberá ponerse en contacto con el [servicio de soporte técnico para partners](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span><span class="sxs-lookup"><span data-stu-id="892ae-151">To delete a location from your account you will need to contact [Partner Support](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b).</span></span> <span data-ttu-id="892ae-152">Asegúrese de que comprende el impacto que tiene esta acción.</span><span class="sxs-lookup"><span data-stu-id="892ae-152">Make sure that you understand the impact this action has.</span></span> <span data-ttu-id="892ae-153">Las ubicaciones eliminadas no se pueden recuperar y todo lo relacionado con ese id. de MPN específico ya no se reconocerá ni estará activo para la empresa.</span><span class="sxs-lookup"><span data-stu-id="892ae-153">Deleted locations cannot be retrieved and anything tied to that specific MPN id will no longer be recognized or be active for your company.</span></span>

## <a name="change-country-of-partner-global-account"></a><span data-ttu-id="892ae-154">Cambiar el país de la cuenta global del asociado</span><span class="sxs-lookup"><span data-stu-id="892ae-154">Change country of Partner global account</span></span> 

1. <span data-ttu-id="892ae-155">Iniciar sesión con la cuenta de MPN en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="892ae-155">Sign in using the MPN account in Partner Center.</span></span> <span data-ttu-id="892ae-156">(Las credenciales de MPN pueden ser diferentes de las credenciales del programa CSP).</span><span class="sxs-lookup"><span data-stu-id="892ae-156">(Your MPN credentials may be different from your CSP credentials) .</span></span> <span data-ttu-id="892ae-157">La cuenta de MPN debe tener privilegios de administrador global o de cuenta.</span><span class="sxs-lookup"><span data-stu-id="892ae-157">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

2. <span data-ttu-id="892ae-158">En la pestaña **Partner**, diríjase a **Ubicaciones de la empresa** y compruebe la lista de ubicaciones para asegurarse de que se muestra la ubicación que quiere como entidad jurídica.</span><span class="sxs-lookup"><span data-stu-id="892ae-158">On the **Partner** tab, go to **Business locations** and check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> 
 
1. <span data-ttu-id="892ae-159">Para agregar una ubicación, haga clic en **Agregar una ubicación** y, en el control flotante, proporcione los detalles necesarios, como el nombre, la dirección y el contacto principal de la empresa correspondientes a la ubicación que desea agregar a la empresa.</span><span class="sxs-lookup"><span data-stu-id="892ae-159">To add a location, click **Add a location**, and, in the fly out, provide the required details including business name, address, and primary contact for the location that you want to add to your company.</span></span> 
 
1. <span data-ttu-id="892ae-160">Seleccione **Cambiar el país** junto al menú desplegable **País o región** y siga los pasos que se indican.</span><span class="sxs-lookup"><span data-stu-id="892ae-160">Select **Change your country** next to the **Country/region** drop-down and follow the steps.</span></span> 

:::image type="content" source="images/lbp.png" alt-text="Control flotante de datos del perfil legal de la empresa":::

5. <span data-ttu-id="892ae-162">Haga clic en **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="892ae-162">Click **Save**.</span></span>

6. <span data-ttu-id="892ae-163">El país de la cuenta global de MPN se cambiará por el país del nuevo perfil legal.</span><span class="sxs-lookup"><span data-stu-id="892ae-163">MPN global account country will be changed to the new legal country.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="892ae-164">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="892ae-164">Next steps</span></span>

- <span data-ttu-id="892ae-165">Obtenga más información acerca del [proceso de verificación](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="892ae-165">Learn about the [verification process](verification-responses.md).</span></span>
