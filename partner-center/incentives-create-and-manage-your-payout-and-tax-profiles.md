---
title: Perfiles fiscales y de pago en el Centro de partners
ms.topic: how-to
ms.date: 09/11/2020
description: Cree y administre su perfil fiscal y de pago para que pueda pagar su trabajo de incentivos.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: de143ecfae1b803e0743a28db5cda5ae9a3d5f2d
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999319"
---
# <a name="create-and-manage-incentives-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="ee937-103">Crear y administrar perfiles de pago y fiscal de incentivos en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="ee937-103">Create and manage incentives payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="ee937-104">**Se aplica a:**</span><span class="sxs-lookup"><span data-stu-id="ee937-104">**Applies to:**</span></span>

- <span data-ttu-id="ee937-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ee937-105">Partner Center</span></span>

<span data-ttu-id="ee937-106">**Roles adecuados:**</span><span class="sxs-lookup"><span data-stu-id="ee937-106">**Appropriate roles:**</span></span>

- <span data-ttu-id="ee937-107">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="ee937-107">Incentives admin</span></span>
- <span data-ttu-id="ee937-108">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="ee937-108">Billing admin</span></span>
- <span data-ttu-id="ee937-109">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ee937-109">Global admin</span></span>

<span data-ttu-id="ee937-110">Antes de que pueda recibir el pago de sus programas de incentivos para una ubicación de MPN determinada, debe completar la inscripción; para ello, asocie un perfil de fiscal y de pago válido al programa y la ubicación MPN.</span><span class="sxs-lookup"><span data-stu-id="ee937-110">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="ee937-111">Microsoft usará este perfil fiscal y de pago para emitir los pagos.</span><span class="sxs-lookup"><span data-stu-id="ee937-111">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="ee937-112">Es posible que se le permita usar la transferencia electrónica bancaria o una nota de crédito para el pago, en función de las reglas del programa de incentivos.</span><span class="sxs-lookup"><span data-stu-id="ee937-112">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

## <a name="roles-currencies-and-other-microsoft-programs"></a><span data-ttu-id="ee937-113">Roles, monedas y otros programas de Microsoft</span><span class="sxs-lookup"><span data-stu-id="ee937-113">Roles, currencies, and other Microsoft programs</span></span>

<span data-ttu-id="ee937-114">Es importante comprender la información siguiente antes de empezar a trabajar con el pago y el perfil fiscal.</span><span class="sxs-lookup"><span data-stu-id="ee937-114">It's important to understand the information below before you get started with your payout and tax profile.</span></span>

### <a name="roles-and-permissions"></a><span data-ttu-id="ee937-115">Roles y permisos</span><span class="sxs-lookup"><span data-stu-id="ee937-115">Roles and permissions</span></span>

<span data-ttu-id="ee937-116">Debe ser un administrador de incentivos para introducir información bancaria y fiscal para los pagos de incentivos.</span><span class="sxs-lookup"><span data-stu-id="ee937-116">You must be an Incentives Admin to enter bank and tax information for incentive payments.</span></span> <span data-ttu-id="ee937-117">Si es un administrador de la cuenta o MPN, puede asignarse a usted mismo o a un colega para que sea el administrador de incentivos.</span><span class="sxs-lookup"><span data-stu-id="ee937-117">If you're an MPN/Account Admin, you can assign yourself and/or a colleague to be the Incentives Admin.</span></span>

<span data-ttu-id="ee937-118">Si necesita solicitar permisos de administrador de incentivos, póngase en contacto con el administrador de MPN o el administrador global. Puede averiguar qué usuarios de su empresa tienen estos roles; para ello, inicie sesión en el [panel del centro de Partners](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="ee937-118">If you need to request Incentives Admin permissions, contact your MPN Admin or Global Admin. You can find out who in your company has these roles by signing into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span> <span data-ttu-id="ee937-119">En el icono de **configuración** de la parte superior derecha, seleccione **Administración de usuarios** y, a continuación, filtre en administrador global.</span><span class="sxs-lookup"><span data-stu-id="ee937-119">From the **Settings** icon at the top right, select **User Management** and then filter on Global Admin.</span></span>

<span data-ttu-id="ee937-120">Incentivos: los usuarios pueden ver los ingresos y los informes de beneficios y de pago, pero no pueden editar los detalles de los bancos y los impuestos.</span><span class="sxs-lookup"><span data-stu-id="ee937-120">Incentives Users can view Incentive earnings and payment details and reports, but can’t edit bank and tax details.</span></span>

### <a name="choose-your-disbursement-currency"></a><span data-ttu-id="ee937-121">Elegir la moneda de desembolso</span><span class="sxs-lookup"><span data-stu-id="ee937-121">Choose your disbursement currency</span></span>

<span data-ttu-id="ee937-122">De forma predeterminada, los pagos de incentivos se realizan en la moneda local de cada entidad respectiva.</span><span class="sxs-lookup"><span data-stu-id="ee937-122">By default, incentives payments are made in the local currency of each respective entity.</span></span> <span data-ttu-id="ee937-123">Puede especificar una moneda diferente durante la configuración del perfil.</span><span class="sxs-lookup"><span data-stu-id="ee937-123">You can specify a different currency during profile setup.</span></span> <span data-ttu-id="ee937-124">Los pagos se calcularán usando una tasa de cambio de acuerdo con la configuración mensual de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="ee937-124">Payments will be calculated using an exchange rate as set monthly by Microsoft.</span></span> <span data-ttu-id="ee937-125">Será responsable de cualquier cambio en el valor debido a la moneda seleccionada.</span><span class="sxs-lookup"><span data-stu-id="ee937-125">You’ll be responsible for any changes in value due to the currency selected.</span></span>

### <a name="bank-and-tax-information-and-other-programs"></a><span data-ttu-id="ee937-126">Información bancaria y fiscal y otros programas</span><span class="sxs-lookup"><span data-stu-id="ee937-126">Bank and tax information and other programs</span></span>

<span data-ttu-id="ee937-127">Proporcione la información que se describe a continuación aunque Microsoft ya use los datos bancarios para los pagos.</span><span class="sxs-lookup"><span data-stu-id="ee937-127">Provide the information described below even if Microsoft already uses your bank data for payments.</span></span> <span data-ttu-id="ee937-128">Esto ayuda a garantizar la privacidad y la seguridad de los datos de su empresa, ya que copiar el perfil en la nueva herramienta podría exponer información confidencial.</span><span class="sxs-lookup"><span data-stu-id="ee937-128">This helps ensure the privacy and security of your company’s data, since copying your profile to the new tool could expose sensitive information.</span></span> <span data-ttu-id="ee937-129">Seguir este proceso también es una buena oportunidad para asegurarse de que los datos estén completos y sean precisos.</span><span class="sxs-lookup"><span data-stu-id="ee937-129">Going through this process is also a good opportunity to ensure the data is complete and accurate.</span></span>

### <a name="using-different-profiles-for-different-microsoft-programs"></a><span data-ttu-id="ee937-130">Usar perfiles diferentes para distintos programas de Microsoft</span><span class="sxs-lookup"><span data-stu-id="ee937-130">Using different profiles for different Microsoft programs</span></span>

<span data-ttu-id="ee937-131">Dentro del minorista, los pagos por cada uno de los cinco programas de incentivos comerciales pueden dirigirse a la misma cuenta bancaria.</span><span class="sxs-lookup"><span data-stu-id="ee937-131">Within retail, payments for each of the five retail incentive programs can go to the same bank account.</span></span> <span data-ttu-id="ee937-132">Como alternativa, puede elegir que los pagos de Xbox minorista se dirijan a una cuenta bancaria mientras que la oficina de venta directa se paga a una cuenta bancaria diferente.</span><span class="sxs-lookup"><span data-stu-id="ee937-132">Alternatively, you can choose to have Retail Xbox payments go into one bank account while Retail Office is paid to a different bank account.</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="ee937-133">Crear y administrar perfiles de pago y impuestos en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="ee937-133">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="ee937-134">Las secciones siguientes le guiarán a través del proceso de creación y administración de perfiles de pago y impuestos en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="ee937-134">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="ee937-135">Debe ser administrador de incentivos para crear o administrar perfiles de pago en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="ee937-135">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="ee937-136">Los roles de incentivos deben asignarse a cada ubicación de MPN en cada programa de incentivos.</span><span class="sxs-lookup"><span data-stu-id="ee937-136">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="ee937-137">Para obtener más información acerca de cómo agregar administradores de incentivos en el centro de Partners, consulte [crear cuentas de usuario](create-user-accounts-and-set-permissions.md).</span><span class="sxs-lookup"><span data-stu-id="ee937-137">For more information on how to add Incentive admins in Partner Center, see [Create user accounts](create-user-accounts-and-set-permissions.md).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="ee937-138">Acceder a la sección de impuestos y pago en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="ee937-138">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="ee937-139">Inicie sesión en el [panel del centro de Partners](https://partner.microsoft.com/dashboard/) con la cuenta de Azure Active Directory (Azure ad) (cuenta de la compañía) o la dirección de correo electrónico adecuada si se asignó alguna.</span><span class="sxs-lookup"><span data-stu-id="ee937-139">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/) using your Azure Active Directory (Azure AD) account (company account), or the appropriate email address if one was assigned.</span></span>

   - <span data-ttu-id="ee937-140">Se pueden registrar varios dominios en una cuenta de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ee937-140">Multiple domains can be registered within one Azure AD account.</span></span> <span data-ttu-id="ee937-141">Póngase en contacto con el administrador global para determinar qué dominios están asociados.</span><span class="sxs-lookup"><span data-stu-id="ee937-141">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="ee937-142">Si solo puede iniciar sesión con el @onmicrosoft.com dominio, póngase en contacto con el administrador de la cuenta para agregar dominios adicionales a la cuenta de Azure ad.</span><span class="sxs-lookup"><span data-stu-id="ee937-142">If you're only able to log in with the @onmicrosoft.com domain, contact your Account admin to add additional domains to the Azure AD account.</span></span>
   - <span data-ttu-id="ee937-143">Si se le pide que seleccione una cuenta **profesional o educativa** o una cuenta **personal**, seleccione **cuenta profesional o educativa**.</span><span class="sxs-lookup"><span data-stu-id="ee937-143">If you're prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="ee937-144">Seleccione el icono de engranaje para abrir el menú de **configuración** y, a continuación, seleccione **configuración de socio comercial**.</span><span class="sxs-lookup"><span data-stu-id="ee937-144">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="ee937-145">En el menú configuración de la **cuenta** , seleccione **pago e impuestos**.</span><span class="sxs-lookup"><span data-stu-id="ee937-145">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="ee937-146">Asignación de perfiles de pago y impuestos a programas individuales</span><span class="sxs-lookup"><span data-stu-id="ee937-146">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="ee937-147">Inicie sesión en el [panel del centro de Partners](https://partner.microsoft.com/dashboard/)y seleccione el icono de engranaje para abrir el menú de **configuración** .</span><span class="sxs-lookup"><span data-stu-id="ee937-147">Sign into the [Partner Center dashboard](https://partner.microsoft.com/dashboard/), and then select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="ee937-148">Seleccione **configuración de socio comercial**, expanda la **sección pago y impuestos**y, a continuación, seleccione **asignación de perfil fiscal y de pago**.</span><span class="sxs-lookup"><span data-stu-id="ee937-148">Select **Partner settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="ee937-149">Se mostrará una lista de los programas.</span><span class="sxs-lookup"><span data-stu-id="ee937-149">A list of your programs will be displayed.</span></span> <span data-ttu-id="ee937-150">Seleccione la flecha situada junto a un programa para ver los detalles del perfil.</span><span class="sxs-lookup"><span data-stu-id="ee937-150">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="ee937-151">En el menú desplegable **Perfil de impuestos** , seleccione el perfil de impuestos que desee o seleccione la opción para crear un nuevo perfil.</span><span class="sxs-lookup"><span data-stu-id="ee937-151">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="ee937-152">Al seleccionar la opción para crear un nuevo perfil, se le redirigirá adecuadamente.</span><span class="sxs-lookup"><span data-stu-id="ee937-152">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="ee937-153">Seleccione continuar en la ventana emergente.</span><span class="sxs-lookup"><span data-stu-id="ee937-153">Select Continue in the pop-up window.</span></span> <span data-ttu-id="ee937-154">A continuación se proporciona el proceso para crear un nuevo perfil de impuestos.</span><span class="sxs-lookup"><span data-stu-id="ee937-154">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="ee937-155">Seleccione el **método de pago**.</span><span class="sxs-lookup"><span data-stu-id="ee937-155">Select **Payment method**.</span></span>

   - <span data-ttu-id="ee937-156">Si ha seleccionado **transferencia bancaria electrónica** como método de pago, seleccione el perfil de pago que desee o seleccione la opción para crear un nuevo perfil.</span><span class="sxs-lookup"><span data-stu-id="ee937-156">If you have selected **Electronic bank transfer** as your payment method, select the payment profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="ee937-157">Al seleccionar la opción para crear un nuevo perfil, se le redirigirá adecuadamente.</span><span class="sxs-lookup"><span data-stu-id="ee937-157">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span> <span data-ttu-id="ee937-158">Seleccione continuar en la ventana emergente.</span><span class="sxs-lookup"><span data-stu-id="ee937-158">Select Continue in the pop-up window.</span></span> <span data-ttu-id="ee937-159">A continuación se proporciona el proceso para crear un nuevo perfil de pago.</span><span class="sxs-lookup"><span data-stu-id="ee937-159">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="ee937-160">Si ha seleccionado **Nota de crédito** como método de pago, complete la comprobación.</span><span class="sxs-lookup"><span data-stu-id="ee937-160">If you have selected **Credit Note** as your payment method, then complete the verification.</span></span> <span data-ttu-id="ee937-161">Esto confirma que el número de SAP al que se hace referencia pertenece a su organización.</span><span class="sxs-lookup"><span data-stu-id="ee937-161">This confirms that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="ee937-162">Si hay varias entidades comerciales de Microsoft en la lista, debe seleccionar un perfil de pago para cada entidad.</span><span class="sxs-lookup"><span data-stu-id="ee937-162">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="ee937-163">La disponibilidad del método de pago depende de las reglas del programa de incentivos.</span><span class="sxs-lookup"><span data-stu-id="ee937-163">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="ee937-164">Seleccione la **moneda**.</span><span class="sxs-lookup"><span data-stu-id="ee937-164">Select the **Currency**.</span></span>

6. <span data-ttu-id="ee937-165">Cuando haya completado todos los campos de pago, seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="ee937-165">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="ee937-166">Crear el perfil de Banco</span><span class="sxs-lookup"><span data-stu-id="ee937-166">Create your bank profile</span></span>

<span data-ttu-id="ee937-167">Los perfiles de banco se crean en el nivel de organización.</span><span class="sxs-lookup"><span data-stu-id="ee937-167">Bank profiles are created at an organization level.</span></span> <span data-ttu-id="ee937-168">Esto permite asignar un perfil de banco a través de varios programas de ID. de MPN y de incentivos dentro de una organización.</span><span class="sxs-lookup"><span data-stu-id="ee937-168">This allows one bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="ee937-169">Puede haber excepciones al aplicar el perfil de banca a distintos países, ya que se pueden aplicar diferentes reglas de banca y impuestos.</span><span class="sxs-lookup"><span data-stu-id="ee937-169">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="ee937-170">En las páginas siguientes, los campos con un asterisco son obligatorios.</span><span class="sxs-lookup"><span data-stu-id="ee937-170">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="ee937-171">Si no sabe qué es un campo, seleccione el icono de información.</span><span class="sxs-lookup"><span data-stu-id="ee937-171">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="ee937-172">En la página **detalles** , complete los siguientes campos: **nombre del perfil:** escriba un nombre único para identificar este perfil de pago.</span><span class="sxs-lookup"><span data-stu-id="ee937-172">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="ee937-173">**Ubicación de la cuenta bancaria:** País en el que se encuentra el Banco de su empresa.</span><span class="sxs-lookup"><span data-stu-id="ee937-173">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="ee937-174">**Método de pago:** El método de pago preferido para el centro de Partners es transferencia bancaria electrónica.</span><span class="sxs-lookup"><span data-stu-id="ee937-174">**Payment method:** The preferred payment method for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="ee937-175">Seleccione **Next** (Siguiente).</span><span class="sxs-lookup"><span data-stu-id="ee937-175">Select **Next**.</span></span>

3. <span data-ttu-id="ee937-176">En la página **cuenta bancaria** , escriba su información.</span><span class="sxs-lookup"><span data-stu-id="ee937-176">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="ee937-177">Los campos que se muestran en esta página variarán en función del país.</span><span class="sxs-lookup"><span data-stu-id="ee937-177">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="ee937-178">Seleccione **Next** (Siguiente).</span><span class="sxs-lookup"><span data-stu-id="ee937-178">Select **Next**.</span></span>

5. <span data-ttu-id="ee937-179">En la página **beneficiario** , escriba la información adecuada.</span><span class="sxs-lookup"><span data-stu-id="ee937-179">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="ee937-180">El beneficiario es la persona de su empresa en la que el Banco se pondrá en contacto si necesita discutir su cuenta.</span><span class="sxs-lookup"><span data-stu-id="ee937-180">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="ee937-181">Una vez completados los campos, seleccione **Finalizar**y, a continuación, seleccione **confirmar** para crear el perfil de banco.</span><span class="sxs-lookup"><span data-stu-id="ee937-181">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="ee937-182">Se le redirigirá a la página de **perfiles de pago y impuestos** .</span><span class="sxs-lookup"><span data-stu-id="ee937-182">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="ee937-183">El estado del nuevo perfil reflejará la **validación de Microsoft pendiente** hasta que se haya completado la validación.</span><span class="sxs-lookup"><span data-stu-id="ee937-183">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="ee937-184">Este proceso puede tardar hasta 48 horas.</span><span class="sxs-lookup"><span data-stu-id="ee937-184">This process may take up to 48 hours.</span></span> <span data-ttu-id="ee937-185">Una vez completada la validación, el estado del perfil reflejará **aprobado** o **acción requerida**.</span><span class="sxs-lookup"><span data-stu-id="ee937-185">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="ee937-186">Si se **requiere una acción**, repita los pasos anteriores y proporcione la información necesaria.</span><span class="sxs-lookup"><span data-stu-id="ee937-186">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="ee937-187">Crear el perfil de impuestos</span><span class="sxs-lookup"><span data-stu-id="ee937-187">Create your tax profile</span></span>

<span data-ttu-id="ee937-188">Utilice el procedimiento siguiente para proporcionar a Microsoft la información fiscal necesaria para su organización.</span><span class="sxs-lookup"><span data-stu-id="ee937-188">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="ee937-189">Las páginas de esta sección son dinámicas y variarán en función de su país o región.</span><span class="sxs-lookup"><span data-stu-id="ee937-189">The pages in this section are dynamic and will vary according to your country or region.</span></span> <span data-ttu-id="ee937-190">Si necesita ayuda para identificar la información fiscal correcta, póngase en contacto con los orígenes de gobierno correspondientes de su país.</span><span class="sxs-lookup"><span data-stu-id="ee937-190">If you need help with identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="ee937-191">En el caso de las empresas asociadas de la América, si necesita información sobre la finalización de los formularios W8 o W9, las siguientes direcciones le llevan al sitio de IRS:</span><span class="sxs-lookup"><span data-stu-id="ee937-191">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="ee937-192">Especifique solo los detalles de su empresa.</span><span class="sxs-lookup"><span data-stu-id="ee937-192">Enter only details for your company.</span></span> <span data-ttu-id="ee937-193">No escriba nunca detalles personales.</span><span class="sxs-lookup"><span data-stu-id="ee937-193">Never enter personal details.</span></span>

1. <span data-ttu-id="ee937-194">En la página **Perfil de negocio** , complete los campos obligatorios y, a continuación, seleccione **siguiente**.</span><span class="sxs-lookup"><span data-stu-id="ee937-194">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="ee937-195">En la página **instalación** , seleccione la opción que se aplica a su compañía.</span><span class="sxs-lookup"><span data-stu-id="ee937-195">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="ee937-196">Seleccione la opción de la izquierda si su empresa se incorpora solo en el Estados Unidos, o si este perfil es para un individuo.</span><span class="sxs-lookup"><span data-stu-id="ee937-196">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span>
   - <span data-ttu-id="ee937-197">Seleccione la opción de la derecha si su empresa se incorpora fuera del Estados Unidos y, a continuación, seleccione su país o región en la lista.</span><span class="sxs-lookup"><span data-stu-id="ee937-197">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="ee937-198">Seleccione **Next** (Siguiente).</span><span class="sxs-lookup"><span data-stu-id="ee937-198">Select **Next**.</span></span> 

4. <span data-ttu-id="ee937-199">En la página **Estado de impuestos** , escriba la información necesaria y, a continuación, seleccione **siguiente**.</span><span class="sxs-lookup"><span data-stu-id="ee937-199">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="ee937-200">Los campos de esta página variarán en función del país.</span><span class="sxs-lookup"><span data-stu-id="ee937-200">Fields on this page will vary by country.</span></span> <span data-ttu-id="ee937-201">los detalles.</span><span class="sxs-lookup"><span data-stu-id="ee937-201">your details.</span></span> 

5. <span data-ttu-id="ee937-202">En la página de **documentación adicional** , los campos obligatorios y seleccione **siguiente**.</span><span class="sxs-lookup"><span data-stu-id="ee937-202">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="ee937-203">Seleccione **examinar** para cargar los documentos requeridos por su país o región.</span><span class="sxs-lookup"><span data-stu-id="ee937-203">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="ee937-204">Cuando se muestre el nombre del documento, seleccione **cargar**.</span><span class="sxs-lookup"><span data-stu-id="ee937-204">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="ee937-205">Si necesita quitar el documento, seleccione **quitar**.</span><span class="sxs-lookup"><span data-stu-id="ee937-205">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="ee937-206">Para guardar y continuar, seleccione **Finalizar**.</span><span class="sxs-lookup"><span data-stu-id="ee937-206">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="ee937-207">Seleccione **confirmar** en el mensaje emergente.</span><span class="sxs-lookup"><span data-stu-id="ee937-207">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="ee937-208">Volverá a la página de configuración de **pagos y impuestos** .</span><span class="sxs-lookup"><span data-stu-id="ee937-208">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ee937-209">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="ee937-209">Next steps</span></span>

- [<span data-ttu-id="ee937-210">Preguntas frecuentes sobre el pago de incentivos y el perfil fiscal</span><span class="sxs-lookup"><span data-stu-id="ee937-210">Incentives payout and tax profile FAQs</span></span>](incentives-payout-tax-profile-faqs.md)
