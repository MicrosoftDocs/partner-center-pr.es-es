---
title: Crear y administrar perfiles de pago y impuestos en el centro de Partners
ms.topic: article
ms.date: 06/29/2020
description: Antes de que pueda pagar por su trabajo de incentivos, debe crear los perfiles de pago y fiscal.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: b7f99ff64b6cdabe8b59607e5820daf0909050f1
ms.sourcegitcommit: bea864212edc90c5f851566505deef6623f79723
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/01/2020
ms.locfileid: "85719456"
---
# <a name="payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="5145e-103">Perfiles fiscales y de pago en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="5145e-103">Payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="5145e-104">Se aplica a:</span><span class="sxs-lookup"><span data-stu-id="5145e-104">Applies to:</span></span>

- <span data-ttu-id="5145e-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="5145e-105">Partner Center</span></span>

<span data-ttu-id="5145e-106">Antes de que pueda recibir el pago de sus programas de incentivos para una ubicación de MPN determinada, debe completar la inscripción; para ello, asocie un perfil de fiscal y de pago válido al programa y la ubicación MPN.</span><span class="sxs-lookup"><span data-stu-id="5145e-106">Before you can receive payment for your incentive programs for a particular MPN location, you must complete your enrollment by associating a valid payout and tax profile with the program and MPN location.</span></span> <span data-ttu-id="5145e-107">Microsoft usará este perfil de pago e impuestos para emitir los pagos.</span><span class="sxs-lookup"><span data-stu-id="5145e-107">Microsoft will use this payout and tax profile to issue payments.</span></span> <span data-ttu-id="5145e-108">Es posible que se le permita usar la transferencia electrónica bancaria o una nota de crédito para el pago, en función de las reglas del programa de incentivos.</span><span class="sxs-lookup"><span data-stu-id="5145e-108">You may be allowed to use electronic bank transfer or a credit note for payment, depending on the rules of the incentive program.</span></span> 

<span data-ttu-id="5145e-109">Roles adecuados:</span><span class="sxs-lookup"><span data-stu-id="5145e-109">Appropriate roles:</span></span>

- <span data-ttu-id="5145e-110">Administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="5145e-110">Incentives admin</span></span>
- <span data-ttu-id="5145e-111">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="5145e-111">Billing admin</span></span>
- <span data-ttu-id="5145e-112">Administrador global</span><span class="sxs-lookup"><span data-stu-id="5145e-112">Global admin</span></span>

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a><span data-ttu-id="5145e-113">Crear y administrar perfiles de pago y impuestos en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="5145e-113">Create and manage payout and tax profiles in Partner Center</span></span>

<span data-ttu-id="5145e-114">Las secciones siguientes le guiarán a través del proceso de creación y administración de perfiles de pago y impuestos en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="5145e-114">The sections below will walk you through the process of creating and managing payment and tax profiles in Partner Center.</span></span>

>[!IMPORTANT]
><span data-ttu-id="5145e-115">Debe ser administrador de incentivos para crear o administrar perfiles de pago en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="5145e-115">You must be an Incentive admin to create or manage payment profiles in Partner Center.</span></span> <span data-ttu-id="5145e-116">Los roles de incentivos deben asignarse a cada ubicación de MPN en cada programa de incentivos.</span><span class="sxs-lookup"><span data-stu-id="5145e-116">Incentive roles must be assigned to each MPN location under each incentive program.</span></span> <span data-ttu-id="5145e-117">Para obtener más información acerca de cómo agregar administradores de incentivos en el centro de Partners, consulte [adición de usuarios de incentivos o administradores en el centro de Partners](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center).</span><span class="sxs-lookup"><span data-stu-id="5145e-117">For more information on how to add Incentive admins in Partner Center, see [How to add incentive users or admins in Partner Center](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center).</span></span>

## <a name="access-the-payout-and-tax-section-in-partner-center"></a><span data-ttu-id="5145e-118">Acceder a la sección de impuestos y pago en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="5145e-118">Access the payout and tax section in Partner Center</span></span>

1. <span data-ttu-id="5145e-119">Inicie sesión en el centro de partners mediante su cuenta de AAD (cuenta de la compañía) o la dirección de correo electrónico adecuada si se asignó alguna.</span><span class="sxs-lookup"><span data-stu-id="5145e-119">Log into Partner Center using your AAD account (company account), or the appropriate email address if one was assigned.</span></span> 

   - <span data-ttu-id="5145e-120">Se pueden registrar varios dominios en una cuenta de AAD.</span><span class="sxs-lookup"><span data-stu-id="5145e-120">Multiple domains can be registered within one AAD account.</span></span> <span data-ttu-id="5145e-121">Póngase en contacto con el administrador global para determinar qué dominios están asociados.</span><span class="sxs-lookup"><span data-stu-id="5145e-121">Contact your Global admin to determine which domains are associated.</span></span>
   - <span data-ttu-id="5145e-122">Si solo puede iniciar sesión con el **@onmicrosoft.com** dominio, póngase en contacto con el administrador de la cuenta para agregar dominios adicionales a la cuenta de AAD.</span><span class="sxs-lookup"><span data-stu-id="5145e-122">If you are only able to login with **@onmicrosoft.com** domain, contact your Account admin to add additional domains to the AAD account.</span></span>
   - <span data-ttu-id="5145e-123">Si se le pide que seleccione una cuenta **profesional o educativa** o una cuenta **personal**, seleccione **cuenta profesional o educativa**.</span><span class="sxs-lookup"><span data-stu-id="5145e-123">If prompted to select **Work or school account** or **Personal Account**, select **Work or school account**.</span></span>

2. <span data-ttu-id="5145e-124">Seleccione el icono de engranaje para abrir el menú de **configuración** y, a continuación, seleccione **configuración de socio comercial**.</span><span class="sxs-lookup"><span data-stu-id="5145e-124">Select the gear icon to open the **Settings** menu, and then select **Partner settings**.</span></span>

3. <span data-ttu-id="5145e-125">En el menú configuración de la **cuenta** , seleccione **pago e impuestos**.</span><span class="sxs-lookup"><span data-stu-id="5145e-125">In the **Account settings** menu, select **Payout and tax**.</span></span> 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a><span data-ttu-id="5145e-126">Asignación de perfiles de pago y impuestos a programas individuales</span><span class="sxs-lookup"><span data-stu-id="5145e-126">Assign payout and tax profiles to individual programs</span></span>

1. <span data-ttu-id="5145e-127">En el centro de Partners, seleccione el icono de engranaje para abrir el menú de **configuración** .</span><span class="sxs-lookup"><span data-stu-id="5145e-127">In Partner Center, select the gear icon to open the **Settings** menu.</span></span> 

2. <span data-ttu-id="5145e-128">Seleccione **configuración de socio comercial**, expanda la **sección pago y impuestos**y, a continuación, seleccione **asignación de perfil fiscal y de pago**.</span><span class="sxs-lookup"><span data-stu-id="5145e-128">Select **Partner settings**, expand the **Payout and tax section**, and then select **Payout and tax profile assignment**.</span></span> 
   
   <span data-ttu-id="5145e-129">Se mostrará una lista de los programas.</span><span class="sxs-lookup"><span data-stu-id="5145e-129">A list of your programs will be displayed.</span></span> <span data-ttu-id="5145e-130">Seleccione la flecha situada junto a un programa para ver los detalles del perfil.</span><span class="sxs-lookup"><span data-stu-id="5145e-130">Select the arrow next to a program to see profile details.</span></span> 

3. <span data-ttu-id="5145e-131">En el menú desplegable **Perfil de impuestos** , seleccione el perfil de impuestos que desee o seleccione la opción para crear un nuevo perfil.</span><span class="sxs-lookup"><span data-stu-id="5145e-131">In the **Tax Profile** dropdown menu, select the tax profile you want, or select the option to create a new profile.</span></span> <span data-ttu-id="5145e-132">Al seleccionar la opción para crear un nuevo perfil, se le redirigirá adecuadamente.</span><span class="sxs-lookup"><span data-stu-id="5145e-132">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="5145e-133">Seleccione continuar en la ventana emergente.</span><span class="sxs-lookup"><span data-stu-id="5145e-133">Select Continue in the pop-up window.</span></span> <span data-ttu-id="5145e-134">A continuación se proporciona el proceso para crear un nuevo perfil de impuestos.</span><span class="sxs-lookup"><span data-stu-id="5145e-134">The process for creating a new tax profile has been provided below.</span></span>

4. <span data-ttu-id="5145e-135">Seleccione el **método de pago**.</span><span class="sxs-lookup"><span data-stu-id="5145e-135">Select **Payment method**.</span></span>

   - <span data-ttu-id="5145e-136">Si seleccionó **transferencia bancaria electrónica** como método de pago, en la lista desplegable Perfil de pago, seleccione el perfil de pago que desee o seleccione la opción para crear un nuevo perfil.</span><span class="sxs-lookup"><span data-stu-id="5145e-136">If you have selected **Electronic bank transfer** as payment method then in the payment profile dropdown select the payment profile you want or select the option to create a new profile.</span></span> <span data-ttu-id="5145e-137">Al seleccionar la opción para crear un nuevo perfil, se le redirigirá adecuadamente.</span><span class="sxs-lookup"><span data-stu-id="5145e-137">When you select the option to create a new profile, you’ll be redirected appropriately.</span></span>  <span data-ttu-id="5145e-138">Seleccione continuar en la ventana emergente.</span><span class="sxs-lookup"><span data-stu-id="5145e-138">Select Continue in the pop-up window.</span></span> <span data-ttu-id="5145e-139">A continuación se proporciona el proceso para crear un nuevo perfil de pago.</span><span class="sxs-lookup"><span data-stu-id="5145e-139">The process for creating a new payment profile has been provided below.</span></span>

   - <span data-ttu-id="5145e-140">Si ha seleccionado **Nota de crédito** como método de pago, complete la comprobación para confirmar que el número de SAP al que se hace referencia pertenece a su organización.</span><span class="sxs-lookup"><span data-stu-id="5145e-140">If you have selected **Credit Note** as the payment method then complete the verification to confirm that the referenced SAP number belongs to your organization.</span></span>

    >[!NOTE]
    ><span data-ttu-id="5145e-141">Si hay varias entidades comerciales de Microsoft en la lista, debe seleccionar un perfil de pago para cada entidad.</span><span class="sxs-lookup"><span data-stu-id="5145e-141">If there are multiple Microsoft business entities listed, you must select a payment profile for each entity.</span></span>

    >[!NOTE]
    ><span data-ttu-id="5145e-142">La disponibilidad del método de pago depende de las reglas del programa de incentivos.</span><span class="sxs-lookup"><span data-stu-id="5145e-142">The payment method availability is dependent on the rules of the incentive program.</span></span>
    
5. <span data-ttu-id="5145e-143">Seleccione la **moneda**.</span><span class="sxs-lookup"><span data-stu-id="5145e-143">Select the **Currency**.</span></span>

6. <span data-ttu-id="5145e-144">Cuando haya completado todos los campos de pago, seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="5145e-144">When you’ve completed all of the payment fields, select **Submit**.</span></span>

## <a name="create-your-bank-profile"></a><span data-ttu-id="5145e-145">Crear el perfil de Banco</span><span class="sxs-lookup"><span data-stu-id="5145e-145">Create your bank profile</span></span>

<span data-ttu-id="5145e-146">Los perfiles de banco se crean en el nivel de organización, lo que permite asignar el mismo perfil de banco en varios programas de ID. de MPN y programas de incentivos dentro de una organización.</span><span class="sxs-lookup"><span data-stu-id="5145e-146">Bank profiles are created at an organization level, which allows for the same bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="5145e-147">Puede haber excepciones al aplicar el perfil de banca a distintos países, ya que se pueden aplicar diferentes reglas de banca y impuestos.</span><span class="sxs-lookup"><span data-stu-id="5145e-147">There may be exceptions when applying the banking profile to different countries, as different banking and tax rules may apply.</span></span>

>[!NOTE]
><span data-ttu-id="5145e-148">En las páginas siguientes, los campos con un asterisco son obligatorios.</span><span class="sxs-lookup"><span data-stu-id="5145e-148">On the following pages, fields with an asterisk are required.</span></span> <span data-ttu-id="5145e-149">Si no sabe qué es un campo, seleccione el icono de información.</span><span class="sxs-lookup"><span data-stu-id="5145e-149">If you don’t know what a field is, select the information icon.</span></span> 

1. <span data-ttu-id="5145e-150">En la página **detalles** , complete los siguientes campos: **nombre del perfil:** escriba un nombre único para identificar este perfil de pago.</span><span class="sxs-lookup"><span data-stu-id="5145e-150">On the **Details** page, complete the following fields: **Profile name:** Enter a unique name to identify this payment profile.</span></span>
    <span data-ttu-id="5145e-151">**Ubicación de la cuenta bancaria:** País en el que se encuentra el Banco de su empresa.</span><span class="sxs-lookup"><span data-stu-id="5145e-151">**Bank account location:** The country in which your company’s bank is located.</span></span>
    <span data-ttu-id="5145e-152">**Método de pago:** El método de pago preferido es para el centro de Partners es transferencia bancaria electrónica.</span><span class="sxs-lookup"><span data-stu-id="5145e-152">**Payment method:** The preferred payment method is for Partner Center is electronic bank transfer.</span></span>

2. <span data-ttu-id="5145e-153">Seleccione **Next** (Siguiente).</span><span class="sxs-lookup"><span data-stu-id="5145e-153">Select **Next**.</span></span>

3. <span data-ttu-id="5145e-154">En la página **cuenta bancaria** , escriba su información.</span><span class="sxs-lookup"><span data-stu-id="5145e-154">On the **Bank account** page, enter your information.</span></span> <span data-ttu-id="5145e-155">Los campos que se muestran en esta página variarán en función del país.</span><span class="sxs-lookup"><span data-stu-id="5145e-155">Fields shown on this page will vary by country.</span></span> 

4. <span data-ttu-id="5145e-156">Seleccione **Next** (Siguiente).</span><span class="sxs-lookup"><span data-stu-id="5145e-156">Select **Next**.</span></span>

5. <span data-ttu-id="5145e-157">En la página **beneficiario** , escriba la información adecuada.</span><span class="sxs-lookup"><span data-stu-id="5145e-157">On the **Beneficiary** page, enter the appropriate information.</span></span> <span data-ttu-id="5145e-158">El beneficiario es la persona de su empresa en la que el Banco se pondrá en contacto si necesita discutir su cuenta.</span><span class="sxs-lookup"><span data-stu-id="5145e-158">The beneficiary is the person in your company that the bank would contact if they need to discuss your account.</span></span>

6. <span data-ttu-id="5145e-159">Una vez completados los campos, seleccione **Finalizar**y, a continuación, seleccione **confirmar** para crear el perfil de banco.</span><span class="sxs-lookup"><span data-stu-id="5145e-159">When the fields are completed, select **Finish**, and then select **Confirm** to create your bank profile.</span></span>

<span data-ttu-id="5145e-160">Se le redirigirá a la página de **perfiles de pago y impuestos** .</span><span class="sxs-lookup"><span data-stu-id="5145e-160">You’ll be redirected to the **Payout and tax profiles** page.</span></span> <span data-ttu-id="5145e-161">El estado del nuevo perfil reflejará la **validación de Microsoft pendiente** hasta que se haya completado la validación.</span><span class="sxs-lookup"><span data-stu-id="5145e-161">The status of your new profile will reflect **Pending Microsoft validation** until the validation has been completed.</span></span> <span data-ttu-id="5145e-162">Esto puede tardar hasta 48 horas.</span><span class="sxs-lookup"><span data-stu-id="5145e-162">This may take up to 48 hours.</span></span> <span data-ttu-id="5145e-163">Una vez completada la validación, el estado del perfil reflejará **aprobado** o **acción requerida**.</span><span class="sxs-lookup"><span data-stu-id="5145e-163">Once validation has been completed, your profile status will reflect either **Approved** or **Action required**.</span></span> <span data-ttu-id="5145e-164">Si se **requiere una acción**, repita los pasos anteriores y proporcione la información necesaria.</span><span class="sxs-lookup"><span data-stu-id="5145e-164">If **Action Required**, repeat the steps above providing the necessary information.</span></span> 

## <a name="create-your-tax-profile"></a><span data-ttu-id="5145e-165">Crear el perfil de impuestos</span><span class="sxs-lookup"><span data-stu-id="5145e-165">Create your tax profile</span></span>

<span data-ttu-id="5145e-166">Utilice el procedimiento siguiente para proporcionar a Microsoft la información fiscal necesaria para su organización.</span><span class="sxs-lookup"><span data-stu-id="5145e-166">Use the following procedure to provide Microsoft with the tax information required for your organization.</span></span> <span data-ttu-id="5145e-167">Las páginas de esta sección son dinámicas y variarán según el país o la región.</span><span class="sxs-lookup"><span data-stu-id="5145e-167">The pages in this section are dynamic and will vary according your country or region.</span></span> <span data-ttu-id="5145e-168">Si necesita ayuda para identificar la información fiscal correcta, póngase en contacto con los orígenes de gobierno correspondientes de su país.</span><span class="sxs-lookup"><span data-stu-id="5145e-168">If you need help identifying the correct tax information, contact the appropriate government sources in your country.</span></span>

<span data-ttu-id="5145e-169">En el caso de las empresas asociadas de la América, si necesita información sobre la finalización de los formularios W8 o W9, las siguientes direcciones le llevan al sitio de IRS:</span><span class="sxs-lookup"><span data-stu-id="5145e-169">For partner companies in the Americas, if you require information on completing the W8 or W9 forms, the following addresses take you to the IRS site:</span></span>

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> <span data-ttu-id="5145e-170">Especifique solo los detalles de su empresa.</span><span class="sxs-lookup"><span data-stu-id="5145e-170">Enter only details for your company.</span></span> <span data-ttu-id="5145e-171">No escriba nunca detalles personales.</span><span class="sxs-lookup"><span data-stu-id="5145e-171">Never enter personal details.</span></span>

1. <span data-ttu-id="5145e-172">En la página **Perfil de negocio** , complete los campos obligatorios y, a continuación, seleccione **siguiente**.</span><span class="sxs-lookup"><span data-stu-id="5145e-172">On the **Business Profile** page, complete the required fields and then select **Next**.</span></span> 

2. <span data-ttu-id="5145e-173">En la página **instalación** , seleccione la opción que se aplica a su compañía.</span><span class="sxs-lookup"><span data-stu-id="5145e-173">On the **Setup** page, select the option that applies to your company.</span></span>

   - <span data-ttu-id="5145e-174">Seleccione la opción de la izquierda si su empresa se incorpora solo en el Estados Unidos, o si este perfil es para un individuo.</span><span class="sxs-lookup"><span data-stu-id="5145e-174">Select the option on the left if your company is incorporated in the United States only, or if this profile is for an individual.</span></span> 
   - <span data-ttu-id="5145e-175">Seleccione la opción de la derecha si su empresa se incorpora fuera del Estados Unidos y, a continuación, seleccione su país o región en la lista.</span><span class="sxs-lookup"><span data-stu-id="5145e-175">Select the option on the right if your company is incorporated outside of the United States, and then select your country/region from the list.</span></span>

3. <span data-ttu-id="5145e-176">Seleccione **Next** (Siguiente).</span><span class="sxs-lookup"><span data-stu-id="5145e-176">Select **Next**.</span></span> 

4. <span data-ttu-id="5145e-177">En la página **Estado de impuestos** , escriba la información necesaria y, a continuación, seleccione **siguiente**.</span><span class="sxs-lookup"><span data-stu-id="5145e-177">On the **Tax status** page, enter the required information, and then select **Next**.</span></span> <span data-ttu-id="5145e-178">Los campos de esta página variarán en función del país.</span><span class="sxs-lookup"><span data-stu-id="5145e-178">Fields on this page will vary by country.</span></span> <span data-ttu-id="5145e-179">los detalles.</span><span class="sxs-lookup"><span data-stu-id="5145e-179">your details.</span></span> 

5. <span data-ttu-id="5145e-180">En la página de **documentación adicional** , los campos obligatorios y seleccione **siguiente**.</span><span class="sxs-lookup"><span data-stu-id="5145e-180">On the **Additional documentation** page, the required fields and select **Next**.</span></span> 

6. <span data-ttu-id="5145e-181">Seleccione **examinar** para cargar los documentos requeridos por su país o región.</span><span class="sxs-lookup"><span data-stu-id="5145e-181">Select **Browse** to upload any documents required by your country or region.</span></span> <span data-ttu-id="5145e-182">Cuando se muestre el nombre del documento, seleccione **cargar**.</span><span class="sxs-lookup"><span data-stu-id="5145e-182">When the document name is shown, select **Upload**.</span></span> 

7. <span data-ttu-id="5145e-183">Si necesita quitar el documento, seleccione **quitar**.</span><span class="sxs-lookup"><span data-stu-id="5145e-183">If you need to remove the document, select **Remove**.</span></span>

8. <span data-ttu-id="5145e-184">Para guardar y continuar, seleccione **Finalizar**.</span><span class="sxs-lookup"><span data-stu-id="5145e-184">To save and continue, select **Finish**.</span></span>

9. <span data-ttu-id="5145e-185">Seleccione **confirmar** en el mensaje emergente.</span><span class="sxs-lookup"><span data-stu-id="5145e-185">Select **Confirm** on the pop-up message.</span></span> <span data-ttu-id="5145e-186">Volverá a la página de configuración de **pagos y impuestos** .</span><span class="sxs-lookup"><span data-stu-id="5145e-186">You’ll be taken back to the **Payout and tax setup** page.</span></span>

## <a name="payout-and-tax-profile-faqs"></a><span data-ttu-id="5145e-187">Preguntas más frecuentes sobre el pago y el perfil fiscal</span><span class="sxs-lookup"><span data-stu-id="5145e-187">Payout and tax profile FAQs</span></span>

### <a name="why-do-i-need-to-provide-my-payout-andor-tax-details"></a><span data-ttu-id="5145e-188">¿Por qué es necesario proporcionar los detalles de pago o de impuestos?</span><span class="sxs-lookup"><span data-stu-id="5145e-188">Why do I need to provide my payout and/or tax details?</span></span>

<span data-ttu-id="5145e-189">Con el fin de recibir pagos de los programas de incentivos de Microsoft, debe completar la inscripción proporcionando detalles de pago e impuestos válidos.</span><span class="sxs-lookup"><span data-stu-id="5145e-189">In order to receive payouts for Microsoft incentive programs, you need to complete enrollment by providing valid payout and tax details.</span></span> <span data-ttu-id="5145e-190">Una inscripción se considera completa solo cuando Microsoft valida el pago y el perfil fiscal que proporcione.</span><span class="sxs-lookup"><span data-stu-id="5145e-190">An enrollment is considered complete only when the payout and tax profile you provide is validated by Microsoft.</span></span>

### <a name="how-do-i-know-that-i-need-to-provideupdate-my-payout-andor-tax-details"></a><span data-ttu-id="5145e-191">Cómo sabe que necesito proporcionar o actualizar los datos de pago o de impuestos?</span><span class="sxs-lookup"><span data-stu-id="5145e-191">How do I know that I need to provide/update my payout and/or tax details?</span></span>

<span data-ttu-id="5145e-192">Todos los asociados que se inscriben en un nuevo programa de incentivos deben proporcionar detalles de pago e impuestos válidos para completar la inscripción.</span><span class="sxs-lookup"><span data-stu-id="5145e-192">All partners enrolling in a new incentive program must provide valid payout and tax details to complete the enrollment.</span></span>

<span data-ttu-id="5145e-193">Es posible que también tenga que proporcionar información actualizada si cambian las reglas para el programa de incentivos, o si los aspectos del perfil expiran o se vuelven obsoletos.</span><span class="sxs-lookup"><span data-stu-id="5145e-193">You may also need to provide updated information if the rules for your incentive program change, or if aspects of the profile expire or become outdated.</span></span> <span data-ttu-id="5145e-194">Si esto ocurre, la página de información general mostrará el estado **acción requerida-actualizar banco o Perfil de impuesto**.</span><span class="sxs-lookup"><span data-stu-id="5145e-194">If this happens, your Overview page will show a status of **Action required – Update bank and/or tax profile**.</span></span>

### <a name="how-do-i-provide-update-my-payout-and-or-tax-details"></a><span data-ttu-id="5145e-195">Cómo proporciono o actualizo mis datos de pago o fiscales?</span><span class="sxs-lookup"><span data-stu-id="5145e-195">How do I provide/ update my payout and/ or tax details?</span></span>

<span data-ttu-id="5145e-196">Para obtener información detallada sobre cómo actualizar los detalles de pago y de impuestos en el centro de Partners, consulte [creación y administración de perfiles bancarios y de impuestos en el centro de Partners](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center) .</span><span class="sxs-lookup"><span data-stu-id="5145e-196">For detailed information on how to on how to update payment and tax details in Partner Center, see [How to create and manage bank and tax profiles in Partner Center](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center)</span></span>

### <a name="why-dont-i-see-my-enrollments-when-i-go-to-assign-my-payout-and-tax-profile"></a><span data-ttu-id="5145e-197">¿Por qué no veo mis inscripciones cuando me quiero asignar mi perfil de pago y fiscal?</span><span class="sxs-lookup"><span data-stu-id="5145e-197">Why don't I see my enrollments when I go to assign my payout and tax profile?</span></span>

<span data-ttu-id="5145e-198">Solo los administradores de incentivos de la ubicación de MPN pueden crear o administrar perfiles fiscales y de pago.</span><span class="sxs-lookup"><span data-stu-id="5145e-198">Only incentive admins for your MPN location can create or manage payout and tax profiles.</span></span> <span data-ttu-id="5145e-199">Podría ser que no tuviera los permisos adecuados o que haya iniciado sesión con una cuenta que no tenga estos permisos.</span><span class="sxs-lookup"><span data-stu-id="5145e-199">It could be that you don’t have the proper permissions, or that you’re logged in with an account that does not have these permissions.</span></span> <span data-ttu-id="5145e-200">Póngase en contacto con el administrador de la organización para administrar los permisos bancarios y fiscales.</span><span class="sxs-lookup"><span data-stu-id="5145e-200">Contact your organization administrator to manage permissions for bank and tax.</span></span>

### <a name="where-can-i-see-the-payout-and-tax-profiles-for-my-organization-that-i-can-use"></a><span data-ttu-id="5145e-201">¿Dónde puedo ver los perfiles fiscales y de pago de mi organización que puedo usar?</span><span class="sxs-lookup"><span data-stu-id="5145e-201">Where can I see the payout and tax profiles for my organization that I can use?</span></span>

<span data-ttu-id="5145e-202">Use el procedimiento siguiente para ver los perfiles de pago y impuestos:</span><span class="sxs-lookup"><span data-stu-id="5145e-202">Use the following procedure to see payout and tax profiles:</span></span>

1. <span data-ttu-id="5145e-203">Inicie sesión en Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="5145e-203">Log into Partner Center.</span></span>

2. <span data-ttu-id="5145e-204">Seleccione el icono de engranaje para abrir el menú **Configuración**.</span><span class="sxs-lookup"><span data-stu-id="5145e-204">Select the gear icon to open the **Settings** menu.</span></span>

3. <span data-ttu-id="5145e-205">Seleccione **configuración de socio comercial**.</span><span class="sxs-lookup"><span data-stu-id="5145e-205">Select **Partner settings**.</span></span>

4. <span data-ttu-id="5145e-206">En **Configuración de cuenta**, seleccione **Pago e impuestos** y, a continuación, seleccione **Perfiles fiscales y de pago**.</span><span class="sxs-lookup"><span data-stu-id="5145e-206">Under **Account settings**, select **Payout and tax**, and then select **Payout and tax profile**.</span></span> <span data-ttu-id="5145e-207">Verá todos los perfiles fiscales y de pago existentes junto con el estado y la capacidad de edición.</span><span class="sxs-lookup"><span data-stu-id="5145e-207">You’ll see all existing payment and tax profiles along with status and ability to edit.</span></span>

### <a name="my-organization-is-participating-in-multiple-incentive-programs-do-i-need-to-provide-my-payment-and-tax-profile-multiple-times"></a><span data-ttu-id="5145e-208">Mi organización participa en varios programas de incentivos.</span><span class="sxs-lookup"><span data-stu-id="5145e-208">My organization is participating in multiple incentive programs.</span></span> <span data-ttu-id="5145e-209">¿Es necesario proporcionar el perfil de pago y de impuestos varias veces?</span><span class="sxs-lookup"><span data-stu-id="5145e-209">Do I need to provide my payment and tax profile multiple times?</span></span>

<span data-ttu-id="5145e-210">Con los perfiles de pago, depende de usted.</span><span class="sxs-lookup"><span data-stu-id="5145e-210">With payment profiles, it’s usually up to you.</span></span> <span data-ttu-id="5145e-211">Los perfiles de pago se crean en el nivel de la organización, lo que permite asignar el mismo perfil bancario en varios programas de identificador de MPN y programas de incentivos dentro de una organización.</span><span class="sxs-lookup"><span data-stu-id="5145e-211">Payment profiles are created at an organization level, which allows for the same bank profile to be assigned across multiple MPN ID’s and incentive programs within an organization.</span></span> <span data-ttu-id="5145e-212">En la mayoría de los casos, puede volver a usar un perfil existente o crear uno nuevo.</span><span class="sxs-lookup"><span data-stu-id="5145e-212">In most cases, you can either reuse an existing profile or create a new one.</span></span>

<span data-ttu-id="5145e-213">No obstante, puede haber excepciones al aplicar el perfil bancario a distintos países o regiones, ya que se pueden aplicar reglas bancarias o fiscales.</span><span class="sxs-lookup"><span data-stu-id="5145e-213">There may be exceptions, however, when applying your bank profile to different countries or regions, as local bank or tax rules may apply.</span></span>

<span data-ttu-id="5145e-214">Los perfiles fiscales creados para una ubicación de MPN se reutilizan y se rellenan automáticamente cuando la misma ubicación de MPN participa en otro programa de incentivos.</span><span class="sxs-lookup"><span data-stu-id="5145e-214">Tax profiles created for an MPN location get reused and automatically populated when the same MPN location participates in other incentive program.</span></span> <span data-ttu-id="5145e-215">Pero puede haber excepciones.</span><span class="sxs-lookup"><span data-stu-id="5145e-215">But there can be exceptions.</span></span> <span data-ttu-id="5145e-216">Por ejemplo, las reglas de pago de un nuevo programa de incentivos pueden requerir detalles adicionales para el perfil fiscal.</span><span class="sxs-lookup"><span data-stu-id="5145e-216">For example, the payout rules of a new incentive program may require additional details for the tax profile.</span></span>  

### <a name="i-am-only-able-to-log-in-with-my-onmicrosoftcom-domain-what-should-i-do"></a><span data-ttu-id="5145e-217">Solo puedo iniciar sesión con mi @onmicrosoft.com dominio.</span><span class="sxs-lookup"><span data-stu-id="5145e-217">I am only able to log in with my @onmicrosoft.com domain.</span></span> <span data-ttu-id="5145e-218">  ¿Qué debo hacer?</span><span class="sxs-lookup"><span data-stu-id="5145e-218">What should I do?</span></span>

<span data-ttu-id="5145e-219">Póngase en contacto con el administrador de la cuenta para agregar dominios adicionales a la cuenta de AAD.</span><span class="sxs-lookup"><span data-stu-id="5145e-219">Contact your Account administrator to add additional domains to the AAD account.</span></span>
