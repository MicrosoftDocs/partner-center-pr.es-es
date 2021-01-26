---
title: Administración de las ubicaciones en tu cuenta de partner
ms.topic: how-to
ms.date: 01/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Aprenda a agregar una nueva ubicación y cómo se usa el identificador de MPN de ubicación en programas de incentivos, empresas de CSP, suscripciones y otras transacciones.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38ea8a451f51d80998643e2a023420ea3efaa6ba
ms.sourcegitcommit: e99882e9b6c9b1a0f7427fb133693b1d977be76b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/26/2021
ms.locfileid: "98773435"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a><span data-ttu-id="8392d-103">Administración de las ubicaciones de la cuenta de MPN y adición de una nueva ubicación</span><span class="sxs-lookup"><span data-stu-id="8392d-103">Manage your MPN account locations and add a new location</span></span>


<span data-ttu-id="8392d-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="8392d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="8392d-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="8392d-105">Global admin</span></span>
- <span data-ttu-id="8392d-106">Administrador de cuentas</span><span class="sxs-lookup"><span data-stu-id="8392d-106">Account admin</span></span>

<span data-ttu-id="8392d-107">Los identificadores de MPN de ubicación identifican cada ubicación específica de la empresa.</span><span class="sxs-lookup"><span data-stu-id="8392d-107">The location MPN ID identifies each specific location of your company.</span></span> <span data-ttu-id="8392d-108">Use el identificador de MPN de ubicación para inscribirse en programas de incentivos, para realizar transacciones de empresas del programa Proveedor de soluciones en la nube (CSP) y para otras transacciones comerciales.</span><span class="sxs-lookup"><span data-stu-id="8392d-108">You use the location MPN ID to enroll in incentive programs, to transact Cloud Solution Provider (CSP) business, and other business transactions.</span></span> <span data-ttu-id="8392d-109">El identificador de MPN global se usa para actividades no transaccionales, como las solicitudes de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="8392d-109">The global MPN ID is used for non-transactional activities such as support requests.</span></span>

## <a name="the-following-is-a-typical-scenario"></a><span data-ttu-id="8392d-110">El siguiente ejemplo es un escenario típico:</span><span class="sxs-lookup"><span data-stu-id="8392d-110">The following is a typical scenario:</span></span>

<span data-ttu-id="8392d-111">Contoso tiene su cuenta global de partner (PGA) en el Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="8392d-111">Contoso has its Partner global account (PGA) in the UK.</span></span> <span data-ttu-id="8392d-112">Se trata de su empresa legal registrada, cuyo identificador de MPN global se usa para administrar todos los negocios no transaccionales.</span><span class="sxs-lookup"><span data-stu-id="8392d-112">This is their registered legal business, and it's global MPN ID is used for managing all non-transactional business.</span></span> <span data-ttu-id="8392d-113">Contoso también tiene cuentas de ubicación de partner (PLA) equivalentes a subsidiarias o divisiones en otras ubicaciones del Reino Unido, Francia y EE. UU.</span><span class="sxs-lookup"><span data-stu-id="8392d-113">Contoso also has Partner location accounts (PLA) equivalent to subsidiaries or divisions in another location in the UK, France, and the USA.</span></span> <span data-ttu-id="8392d-114">En la estructura de cuentas de MPN, estas PLA se representan como identificadores de MPN de ubicación únicos.</span><span class="sxs-lookup"><span data-stu-id="8392d-114">In the MPN Account structure, these PLAs are represented as unique location MPN IDs.</span></span> <span data-ttu-id="8392d-115">Las PLA se usan para negocios transaccionales, como los programas de CSP o de incentivos.</span><span class="sxs-lookup"><span data-stu-id="8392d-115">The PLAs are used for transactional business such as CSP or incentives programs.</span></span> <span data-ttu-id="8392d-116">Los pagos están vinculados a ubicaciones específicas.</span><span class="sxs-lookup"><span data-stu-id="8392d-116">Payouts are tied to specific locations.</span></span> 

>[!NOTE]
><span data-ttu-id="8392d-117">Hay una relación 1-1 entre un inquilino de CSP y un identificador de ubicación de MPN.</span><span class="sxs-lookup"><span data-stu-id="8392d-117">There is a 1-1 relationship between a CSP tenant and an MPN location ID.</span></span>

:::image type="content" source="images/locations/locations1.png" alt-text="Estructura de ubicaciones de MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-location-for-a-csp-business"></a><span data-ttu-id="8392d-119">Requisitos previos para agregar una nueva ubicación de cuenta para una empresa de CSP</span><span class="sxs-lookup"><span data-stu-id="8392d-119">Prerequisites in order to add a new account location for a CSP business</span></span>

<span data-ttu-id="8392d-120">Para agregar una nueva ubicación de empresa de CSP, hay varios requisitos previos:</span><span class="sxs-lookup"><span data-stu-id="8392d-120">To add a new CSP business location, there are several prerequisites:</span></span>

1. <span data-ttu-id="8392d-121">Debe tener un identificador de MPN de ubicación en el país en el que quiere hacer negocios.</span><span class="sxs-lookup"><span data-stu-id="8392d-121">You must have a location MPN ID in the country where you want to do business.</span></span>

1. <span data-ttu-id="8392d-122">Necesita un nuevo inquilino de Azure AD en la [región de la empresa](regional-authorization-overview.md) que aún no está inscrito en CSP.</span><span class="sxs-lookup"><span data-stu-id="8392d-122">You need a new Azure AD tenant in the [region of business](regional-authorization-overview.md) which is not already enrolled into CSP.</span></span> <span data-ttu-id="8392d-123">Créelo al inscribirse en CSP.</span><span class="sxs-lookup"><span data-stu-id="8392d-123">Create this when you enroll in CSP.</span></span>
 
3. <span data-ttu-id="8392d-124">Use el nuevo inquilino de AAD para inscribirse en el programa CSP en la región.</span><span class="sxs-lookup"><span data-stu-id="8392d-124">Use the new AAD tenant to enroll into CSP program in the region.</span></span>
<span data-ttu-id="8392d-125">Proporcione los detalles de la empresa legal, incluidos el nombre legal de la empresa, su dirección y los detalles del contacto principal.</span><span class="sxs-lookup"><span data-stu-id="8392d-125">Providing legal company details including the legal company name, address, primary contact details.</span></span> <span data-ttu-id="8392d-126">Esta cuenta se someterá a una verificación: asegúrese de agregar información válida.</span><span class="sxs-lookup"><span data-stu-id="8392d-126">This account will undergo verification, so make sure to add valid information.</span></span>

>[!NOTE] 
 ><span data-ttu-id="8392d-127">Recuerde iniciar sesión con las **nuevas** credenciales para el **nuevo** inquilino de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8392d-127">Remember to sign in with the **new** credentials for the **new** Azure AD tenant.</span></span> <span data-ttu-id="8392d-128">No use las credenciales existentes, ya que el Centro de partners reconocerá que ya tiene una cuenta.</span><span class="sxs-lookup"><span data-stu-id="8392d-128">Don't use your existing credentials as Partner Center will recognize you as already having an account.</span></span>

4. <span data-ttu-id="8392d-129">Acepte el contrato Microsoft Partner Agreement y active la cuenta.</span><span class="sxs-lookup"><span data-stu-id="8392d-129">Accept the Microsoft Partner Agreement and activate the account.</span></span>

## <a name="add-an-mpn-location"></a><span data-ttu-id="8392d-130">Agregar una ubicación de MPN</span><span class="sxs-lookup"><span data-stu-id="8392d-130">Add an MPN location</span></span>

1. <span data-ttu-id="8392d-131">Inicie sesión con la cuenta de MPN en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="8392d-131">Sign in using the MPN account in Partner Center .</span></span> <span data-ttu-id="8392d-132">La cuenta de MPN debe tener privilegios de administrador global o de cuenta.</span><span class="sxs-lookup"><span data-stu-id="8392d-132">The MPN account should have Global Admin or Account Admin privileges.</span></span> 

1. <span data-ttu-id="8392d-133">En el **icono Configuración**, seleccione **Configuración de la organización**.</span><span class="sxs-lookup"><span data-stu-id="8392d-133">From the **Setting icon**, select the **Organization settings**.</span></span>

2. <span data-ttu-id="8392d-134">Seleccione **Legal** y, a continuación, seleccione **Ubicaciones.**</span><span class="sxs-lookup"><span data-stu-id="8392d-134">Select **Legal** and then select **Locations.**</span></span>

3. <span data-ttu-id="8392d-135">Seleccione **Agregar una ubicación** e inserte los detalles de la dirección de la ubicación que quiera agregar a la empresa, así como un contacto principal para la ubicación.</span><span class="sxs-lookup"><span data-stu-id="8392d-135">Select **Add a location**, and insert the address details of the location that you want to add to your company as well as a primary contact for the location.</span></span>

> [!NOTE]
> <span data-ttu-id="8392d-136">Una vez agregada una ubicación en el Centro de partners, no se puede quitar.</span><span class="sxs-lookup"><span data-stu-id="8392d-136">Once a location is added in Partner Center, it cannot be removed.</span></span> <span data-ttu-id="8392d-137">Verá **MPN** en el menú izquierdo del Centro de partners si ha usado el identificador de MPN correcto para iniciar sesión.</span><span class="sxs-lookup"><span data-stu-id="8392d-137">You will see **MPN** in the left menu of Partner Center if you have used the correct MPN ID to sign in.</span></span>

## <a name="change-global-partner-account-location"></a><span data-ttu-id="8392d-138">Cambio de la ubicación de la cuenta de partner global</span><span class="sxs-lookup"><span data-stu-id="8392d-138">Change Global partner account location</span></span>

1. <span data-ttu-id="8392d-139">En **[Ubicaciones de la empresa](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** , compruebe la lista de ubicaciones para asegurarse de que se muestra la ubicación que quiere como entidad jurídica.</span><span class="sxs-lookup"><span data-stu-id="8392d-139">On **[Business locations](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)**, check the list of locations to ensure that the location you want as your legal entity is listed.</span></span> <span data-ttu-id="8392d-140">Si no es así, agrégala.</span><span class="sxs-lookup"><span data-stu-id="8392d-140">If it isn't, add it.</span></span>

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Captura de pantalla de la página de ubicaciones de cuentas del Centro de Partners con una lista de todas las ubicaciones actuales.":::

2. <span data-ttu-id="8392d-142">Selecciona **Legal** y luego **Update legal business profile** (Actualizar perfil de denominación legal de la empresa).</span><span class="sxs-lookup"><span data-stu-id="8392d-142">Select **Legal** and then select **Update legal business profile**</span></span>
  
3. <span data-ttu-id="8392d-143">Selecciona la región, la entidad jurídica y **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="8392d-143">Select the region and legal entity and **Submit** it.</span></span>

  
## <a name="next-steps"></a><span data-ttu-id="8392d-144">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="8392d-144">Next steps</span></span>

- <span data-ttu-id="8392d-145">Obtenga más información acerca del [proceso de verificación](verification-responses.md).</span><span class="sxs-lookup"><span data-stu-id="8392d-145">Learn about the [verification process](verification-responses.md).</span></span>
