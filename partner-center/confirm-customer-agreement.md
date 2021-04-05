---
title: Procedimiento de confirmación de que el cliente ha aceptado el Contrato de cliente de Microsoft para el programa CSP
description: Los asociados del Proveedor de soluciones en la nube (CSP) deben confirmar la aceptación del cliente del Contrato de cliente de Microsoft antes de solicitar servicios Microsoft para los clientes.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633785"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="34806-103">Procedimiento de confirmación de que el cliente ha aceptado el Contrato de cliente de Microsoft para el programa CSP</span><span class="sxs-lookup"><span data-stu-id="34806-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="34806-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="34806-104">**Appropriate roles**</span></span>

- <span data-ttu-id="34806-105">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="34806-105">Admin agent</span></span>
- <span data-ttu-id="34806-106">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="34806-106">Sales agent</span></span>


<span data-ttu-id="34806-107">Los clientes tienen dos opciones para aceptar el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34806-107">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="34806-108">**Opción 1**: atestación del partner de la aceptación del cliente; el partner puede confirmar la aceptación del cliente mediante el SDK o la API del Centro de partners o a través del panel del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="34806-108">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="34806-109">**Opción 2**: aceptación directa del cliente; el asociado puede invitar al cliente a través de una dirección URL para que revise y acepte el contrato en el Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="34806-109">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="34806-110">Acceso a la plantilla del Contrato de cliente de Microsoft</span><span class="sxs-lookup"><span data-stu-id="34806-110">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="34806-111">Puedes descargar manualmente la versión más reciente de la plantilla del Contrato de cliente de Microsoft desde [aquí](https://aka.ms/customeragreement).</span><span class="sxs-lookup"><span data-stu-id="34806-111">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="34806-112">El Contrato de cliente de Microsoft es específico para cada país o región.</span><span class="sxs-lookup"><span data-stu-id="34806-112">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="34806-113">Al solicitar la plantilla del Contrato de cliente de Microsoft, asegúrate de seleccionar el país o región correcto en función de la ubicación del cliente.</span><span class="sxs-lookup"><span data-stu-id="34806-113">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="34806-114">Opción 1: Confirmación de la aceptación por parte del cliente en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="34806-114">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="34806-115">Los partners de facturación directa pueden confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft en el Centro de partners para clientes nuevos y clientes existentes.</span><span class="sxs-lookup"><span data-stu-id="34806-115">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="34806-116">Los revendedores indirectos no pueden dar fe en nombre de sus clientes y deben colaborar con su proveedor indirecto para completar la atestación.</span><span class="sxs-lookup"><span data-stu-id="34806-116">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="34806-117">Confirmar la aceptación de los clientes nuevos</span><span class="sxs-lookup"><span data-stu-id="34806-117">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="34806-118">Si creas un nuevo inquilino de cliente en el Centro de partners, sigue los pasos que se describen a continuación para confirmar la aceptación del cliente del Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34806-118">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="34806-119">Para poder seguir estos pasos, debes ser agente de administración o de ventas.</span><span class="sxs-lookup"><span data-stu-id="34806-119">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="34806-120">Selecciona **Clientes** y, a continuación, **Nuevo cliente**.</span><span class="sxs-lookup"><span data-stu-id="34806-120">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="34806-121">En **Información de cuenta**, especifica los datos de la empresa y su contacto principal.</span><span class="sxs-lookup"><span data-stu-id="34806-121">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="34806-122">En **Contrato de Microsoft**, selecciona el cuadro para dar fe de que el cliente ha aceptado el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34806-122">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="34806-123">En **Fecha de aceptación del contrato**, introduce la fecha adecuada.</span><span class="sxs-lookup"><span data-stu-id="34806-123">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="34806-124">No puedes elegir para esto una fecha futura.</span><span class="sxs-lookup"><span data-stu-id="34806-124">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="34806-125">Comprueba que la información de contacto del usuario principal que se muestra sea correcta.</span><span class="sxs-lookup"><span data-stu-id="34806-125">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="34806-126">Si no es correcta, selecciona **Actualizar** y escribe la información exacta de la persona que aceptó el contrato.</span><span class="sxs-lookup"><span data-stu-id="34806-126">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="34806-127">Selecciona **Siguiente** para continuar con la creación del inquilino del cliente.</span><span class="sxs-lookup"><span data-stu-id="34806-127">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Cliente nuevo":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="34806-129">Confirmar la aceptación de los clientes existentes</span><span class="sxs-lookup"><span data-stu-id="34806-129">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="34806-130">Debes ser agente de administración o de ventas para poder hacer esto:</span><span class="sxs-lookup"><span data-stu-id="34806-130">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="34806-131">Selecciona **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="34806-131">Select **Customers**.</span></span> <span data-ttu-id="34806-132">Busca y selecciona el cliente.</span><span class="sxs-lookup"><span data-stu-id="34806-132">Find and select the customer.</span></span>

2. <span data-ttu-id="34806-133">Selecciona **Información de cuenta**.</span><span class="sxs-lookup"><span data-stu-id="34806-133">Select **Account info**.</span></span>

3. <span data-ttu-id="34806-134">En **Contrato de cliente de Microsoft**, selecciona **Actualizar**.</span><span class="sxs-lookup"><span data-stu-id="34806-134">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="34806-135">Escribe el **Nombre**, los **Apellidos**, la **Dirección de correo electrónico** y el **Número de teléfono** (opcional) de la persona que aceptó el contrato.</span><span class="sxs-lookup"><span data-stu-id="34806-135">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="34806-136">En **Fecha de aceptación del contrato**, introduce la fecha adecuada.</span><span class="sxs-lookup"><span data-stu-id="34806-136">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="34806-137">No puedes elegir para esto una fecha futura.</span><span class="sxs-lookup"><span data-stu-id="34806-137">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="34806-138">Selecciona **Guardar** y continúa.</span><span class="sxs-lookup"><span data-stu-id="34806-138">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Cliente existente":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="34806-140">Recuperar la confirmación de la aceptación del cliente</span><span class="sxs-lookup"><span data-stu-id="34806-140">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="34806-141">Siga los pasos que se describen a continuación para recuperar la confirmación de que un cliente existente ha aceptado el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34806-141">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="34806-142">Debes ser agente de administración o agente de ventas para poder hacer esto.</span><span class="sxs-lookup"><span data-stu-id="34806-142">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="34806-143">Selecciona **Clientes** y, a continuación, busca y selecciona el cliente que quieras ver.</span><span class="sxs-lookup"><span data-stu-id="34806-143">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="34806-144">Selecciona **Información de cuenta**.</span><span class="sxs-lookup"><span data-stu-id="34806-144">Select **Account info**.</span></span>

3. <span data-ttu-id="34806-145">En **Contrato de cliente de Microsoft**, consulta si el cliente ha proporcionado la confirmación.</span><span class="sxs-lookup"><span data-stu-id="34806-145">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="34806-146">Confirmación de la aceptación por parte del cliente mediante el SDK o la API del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="34806-146">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="34806-147">Puedes usar el SDK o la API del Centro de partners para confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34806-147">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="34806-148">Para obtener más información sobre la API o el SDK, consulta:</span><span class="sxs-lookup"><span data-stu-id="34806-148">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="34806-149">Obtener los metadatos del acuerdo del Contrato de cliente de Microsoft</span><span class="sxs-lookup"><span data-stu-id="34806-149">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="34806-150">Confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft</span><span class="sxs-lookup"><span data-stu-id="34806-150">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="34806-151">Obtener la confirmación de la aceptación por parte del cliente del Contrato de cliente de Microsoft</span><span class="sxs-lookup"><span data-stu-id="34806-151">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="34806-152">Obtener un vínculo de descarga para la plantilla del Contrato de cliente de Microsoft</span><span class="sxs-lookup"><span data-stu-id="34806-152">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="34806-153">Opción 2: Aceptación del cliente en el Centro de administración de Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="34806-153">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="34806-154">Los partners pueden invitar a clientes nuevos y existentes, a través de una dirección URL, para que revisen y acepten el contrato en el Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="34806-154">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="34806-155">En las siguientes secciones se muestra cómo puedes:</span><span class="sxs-lookup"><span data-stu-id="34806-155">The next few sections show you how to:</span></span>

- <span data-ttu-id="34806-156">Crear un cliente nuevo e invitarlo para que revise y acepte el contrato.</span><span class="sxs-lookup"><span data-stu-id="34806-156">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="34806-157">Invitar a un cliente nuevo para que revise y acepte la relación y el contrato de revendedor.</span><span class="sxs-lookup"><span data-stu-id="34806-157">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="34806-158">Invitar a un cliente existente para que revise y acepte el contrato.</span><span class="sxs-lookup"><span data-stu-id="34806-158">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="34806-159">Puedes usar el [SDK o la API del Centro de partners](/partner-center/develop/get-direct-sign-status-of-customer-agreement) para obtener el estado de la aceptación directa por parte de un cliente del Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34806-159">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="34806-160">Crear un cliente nuevo e invitarlo para que revise y acepte el contrato</span><span class="sxs-lookup"><span data-stu-id="34806-160">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="34806-161">Sigue los pasos que se indican a continuación para crear un cliente nuevo en el Centro de partners e invitarlo para que revise y acepte el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="34806-161">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="34806-162">En la pestaña **Clientes** del Centro de partners, selecciona **Agregar cliente**.</span><span class="sxs-lookup"><span data-stu-id="34806-162">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="34806-163">En **Información de la cuenta**, escribe la información sobre el nuevo cliente en todos los campos obligatorios, incluido el nombre de la empresa del cliente y el contacto principal.</span><span class="sxs-lookup"><span data-stu-id="34806-163">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="34806-164">En **Contrato de cliente**, seleccione **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center** (Se pedirá al cliente que acepte el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365).</span><span class="sxs-lookup"><span data-stu-id="34806-164">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="34806-165">Completa los demás campos obligatorios en la página.</span><span class="sxs-lookup"><span data-stu-id="34806-165">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="34806-166">Selecciona **Siguiente: revisión** y sigue los pasos para crear el inquilino del cliente.</span><span class="sxs-lookup"><span data-stu-id="34806-166">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="34806-167">Los clientes nuevos no pueden hacer compras hasta que acepten el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34806-167">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Crear un cliente nuevo":::

5. <span data-ttu-id="34806-169">Cuando llegues a la pantalla **Confirmación** del nuevo flujo de trabajo del cliente, guarda las credenciales del cliente.</span><span class="sxs-lookup"><span data-stu-id="34806-169">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="34806-170">Deberás proporcionar estas credenciales al cliente más adelante.</span><span class="sxs-lookup"><span data-stu-id="34806-170">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="34806-171">Fuera del Centro de partners, crea y envía un correo electrónico en el que invites al cliente a aceptar el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="34806-171">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="34806-172">Asegúrate de incluir los elementos siguientes en el correo electrónico:</span><span class="sxs-lookup"><span data-stu-id="34806-172">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="34806-173">Un vínculo a esta[ dirección URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (inicio de sesión obligatorio)</span><span class="sxs-lookup"><span data-stu-id="34806-173">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="34806-174">Las credenciales del cliente que guardó en el paso 5.</span><span class="sxs-lookup"><span data-stu-id="34806-174">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="34806-175">A continuación, el cliente recibirá la invitación por correo electrónico del partner y seleccionará la [dirección URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="34806-175">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="34806-176">El cliente deberá iniciar sesión en el Centro de administración de Microsoft 365 con las credenciales del cliente que recibió.</span><span class="sxs-lookup"><span data-stu-id="34806-176">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="34806-177">El cliente marcará la casilla para aceptar el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34806-177">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="34806-178">Invitación de un cliente nuevo para que revise y acepte la relación de revendedor y el Contrato de cliente de Microsoft</span><span class="sxs-lookup"><span data-stu-id="34806-178">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="34806-179">Usa los pasos siguientes para invitar a un nuevo cliente para que revise y acepte la relación de revendedor y el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34806-179">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="34806-180">En la pestaña **Clientes** en el Centro de partners, selecciona el vínculo **Solicitar una relación de revendedor**.</span><span class="sxs-lookup"><span data-stu-id="34806-180">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="34806-181">Se generará una plantilla de correo electrónico automático, que incluirá texto y una dirección URL parametrizada que dirigirá al cliente al Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="34806-181">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="34806-182">Puedes personalizar la plantilla de correo electrónico generada automáticamente y, a continuación, seleccionar **Copiar al portapapeles** o **Abrir en correo**.</span><span class="sxs-lookup"><span data-stu-id="34806-182">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="34806-183">Usa esta plantilla de correo electrónico para invitar al cliente a aceptar la solicitud de **relación de revendedor** y el **Contrato de cliente de Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="34806-183">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="34806-184">(Nota: En la invitación por correo electrónico, asegúrate de que el partner también incluye la dirección URL que se proporcionó automáticamente, así como las credenciales del cliente que se crearon recientemente).</span><span class="sxs-lookup"><span data-stu-id="34806-184">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Crear una relación":::

5. <span data-ttu-id="34806-186">El cliente recibirá una invitación por correo electrónico y hará clic en la dirección URL parametrizada.</span><span class="sxs-lookup"><span data-stu-id="34806-186">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="34806-187">El cliente usará las credenciales proporcionadas en el correo electrónico para iniciar sesión en el Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="34806-187">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="34806-188">El cliente marcará la casilla para aceptar la **relación de revendedor** y el **Contrato de cliente de Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="34806-188">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="34806-189">En la misma dirección URL, el cliente podrá ver una lista consolidada de los diferentes partners con los que trabaja.</span><span class="sxs-lookup"><span data-stu-id="34806-189">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="34806-190">Podrá seleccionar un partner para ver los detalles.</span><span class="sxs-lookup"><span data-stu-id="34806-190">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Aceptar el contrato":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="34806-192">Invitación de un cliente existente para que revise y acepte el contrato</span><span class="sxs-lookup"><span data-stu-id="34806-192">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="34806-193">Usa los pasos siguientes para invitar a un cliente existente para que revise y acepte el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34806-193">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="34806-194">Crea el correo electrónico del cliente con la dirección URL incrustada para invitar a tu cliente para que acepte el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34806-194">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="34806-195">El cliente recibe la invitación por correo electrónico y hace clic en la [dirección URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="34806-195">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="34806-196">El cliente escribe sus credenciales en el Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="34806-196">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="34806-197">El cliente marcará la casilla para aceptar el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34806-197">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="34806-198">En la misma dirección URL, el cliente podrá ver la lista consolidada de los diferentes partners con los que trabaja.</span><span class="sxs-lookup"><span data-stu-id="34806-198">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="34806-199">Podrá seleccionar un partner para ver los detalles.</span><span class="sxs-lookup"><span data-stu-id="34806-199">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Cliente":::

>[!NOTE]
><span data-ttu-id="34806-201">En determinados escenarios, es posible que los clientes no puedan aceptar directamente el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="34806-201">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="34806-202">Para obtener más información sobre estas situaciones, consulte Dos escenarios en los que es necesario dar fe en nombre del cliente, a continuación.</span><span class="sxs-lookup"><span data-stu-id="34806-202">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="34806-203">Dos escenarios en los que es necesario dar fe en nombre de tu cliente</span><span class="sxs-lookup"><span data-stu-id="34806-203">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="34806-204">Hay dos escenarios en los que es posible que los clientes no puedan aceptar directamente el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="34806-204">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="34806-205">**Escenario 1**: un cliente existente que ha comprado cualquier de los productos siguientes a través de una relación de partner existente: ofertas, software o suscripciones de software, instancias reservadas o plan de Azure.</span><span class="sxs-lookup"><span data-stu-id="34806-205">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="34806-206">Dicho cliente ahora intenta realizar una nueva compra (esta no incluye la renovación automática).</span><span class="sxs-lookup"><span data-stu-id="34806-206">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="34806-207">Cuando el cliente haga clic en la dirección URL, recibirá el mensaje "Póngase en contacto con su partner para confirmar que acepta el Contrato de cliente de Microsoft".</span><span class="sxs-lookup"><span data-stu-id="34806-207">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="34806-208">**Para resolverlo**: debes dar fe en nombre del cliente.</span><span class="sxs-lookup"><span data-stu-id="34806-208">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Captura de pantalla de la página del centro de administración de Microsoft 365 que le pide que se una a su partner para confirmar la aceptación del Contrato de cliente de Microsoft.":::

<span data-ttu-id="34806-210">**Escenario 2**: un cliente existente que ha adquirido cualquiera de las siguientes ofertas, software y suscripciones de software, instancias reservadas y plan de Azure.</span><span class="sxs-lookup"><span data-stu-id="34806-210">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="34806-211">Dicho cliente ahora intenta realizar una nueva compra con un nuevo partner.</span><span class="sxs-lookup"><span data-stu-id="34806-211">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="34806-212">Cuando el cliente haga clic en la dirección URL del Centro de administración de Microsoft 365 para aceptar la nueva relación del partner y el contrato, recibirá el mensaje "Póngase en contacto con su partner para confirmar que acepta el Contrato de cliente de Microsoft".</span><span class="sxs-lookup"><span data-stu-id="34806-212">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="34806-213">**Para resolverlo**: debes dar fe en nombre del cliente.</span><span class="sxs-lookup"><span data-stu-id="34806-213">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="34806-214">Confirmación de que un cliente ha aceptado el contrato</span><span class="sxs-lookup"><span data-stu-id="34806-214">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="34806-215">Si intenta crear un nuevo pedido para un cliente existente al que no has confirmado con anterioridad, recibirá un aviso para completar la confirmación.</span><span class="sxs-lookup"><span data-stu-id="34806-215">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="34806-216">Usa el siguiente procedimiento para hacerlo.</span><span class="sxs-lookup"><span data-stu-id="34806-216">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="34806-217">Escribe el **Nombre**, los **Apellidos**, la **Dirección de correo electrónico** y el **Número de teléfono** (opcional) del usuario que aceptó el contrato.</span><span class="sxs-lookup"><span data-stu-id="34806-217">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="34806-218">En **Fecha de aceptación del contrato**, introduce la fecha adecuada.</span><span class="sxs-lookup"><span data-stu-id="34806-218">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="34806-219">No puedes elegir para esto una fecha futura.</span><span class="sxs-lookup"><span data-stu-id="34806-219">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="34806-220">Selecciona **Guardar y continuar**.</span><span class="sxs-lookup"><span data-stu-id="34806-220">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="34806-221">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="34806-221">Next steps</span></span>

- [<span data-ttu-id="34806-222">Comprobar o actualizar la información del perfil de empresa</span><span class="sxs-lookup"><span data-stu-id="34806-222">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="34806-223">Contratos de cliente de Microsoft (por región, idioma)</span><span class="sxs-lookup"><span data-stu-id="34806-223">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
