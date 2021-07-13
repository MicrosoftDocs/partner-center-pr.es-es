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
ms.openlocfilehash: 9deebf3d9aab2d4dc7953da67a7eb17078b3d30c
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277018"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="41f64-103">Procedimiento de confirmación de que el cliente ha aceptado el Contrato de cliente de Microsoft para el programa CSP</span><span class="sxs-lookup"><span data-stu-id="41f64-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="41f64-104">**Roles adecuados**: Agente de administración | Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="41f64-104">**Appropriate roles**: Admin agent | Sales agent</span></span>


<span data-ttu-id="41f64-105">Los clientes tienen dos opciones para aceptar el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="41f64-105">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="41f64-106">**Opción 1**: atestación del partner de la aceptación del cliente; el partner puede confirmar la aceptación del cliente mediante el SDK o la API del Centro de partners o a través del panel del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="41f64-106">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="41f64-107">**Opción 2**: aceptación directa del cliente; el asociado puede invitar al cliente a través de una dirección URL para que revise y acepte el contrato en el Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="41f64-107">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="41f64-108">Acceso a la plantilla del Contrato de cliente de Microsoft</span><span class="sxs-lookup"><span data-stu-id="41f64-108">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="41f64-109">Puedes descargar manualmente la versión más reciente de la plantilla del Contrato de cliente de Microsoft desde [aquí](https://aka.ms/customeragreement).</span><span class="sxs-lookup"><span data-stu-id="41f64-109">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="41f64-110">El Contrato de cliente de Microsoft es específico para cada país o región.</span><span class="sxs-lookup"><span data-stu-id="41f64-110">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="41f64-111">Al solicitar la plantilla del Contrato de cliente de Microsoft, asegúrate de seleccionar el país o región correcto en función de la ubicación del cliente.</span><span class="sxs-lookup"><span data-stu-id="41f64-111">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="41f64-112">Opción 1: Confirmación de la aceptación por parte del cliente en el Centro de partners</span><span class="sxs-lookup"><span data-stu-id="41f64-112">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="41f64-113">Los partners de facturación directa pueden confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft en el Centro de partners para clientes nuevos y clientes existentes.</span><span class="sxs-lookup"><span data-stu-id="41f64-113">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="41f64-114">Los revendedores indirectos no pueden dar fe en nombre de sus clientes y deben colaborar con su proveedor indirecto para completar la atestación.</span><span class="sxs-lookup"><span data-stu-id="41f64-114">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="41f64-115">Confirmar la aceptación de los clientes nuevos</span><span class="sxs-lookup"><span data-stu-id="41f64-115">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="41f64-116">Si creas un nuevo inquilino de cliente en el Centro de partners, sigue los pasos que se describen a continuación para confirmar la aceptación del cliente del Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="41f64-116">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="41f64-117">Para poder seguir estos pasos, debes ser agente de administración o de ventas.</span><span class="sxs-lookup"><span data-stu-id="41f64-117">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="41f64-118">Selecciona **Clientes** y, a continuación, **Nuevo cliente**.</span><span class="sxs-lookup"><span data-stu-id="41f64-118">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="41f64-119">En **Información de cuenta**, especifica los datos de la empresa y su contacto principal.</span><span class="sxs-lookup"><span data-stu-id="41f64-119">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="41f64-120">En **Contrato de Microsoft**, selecciona el cuadro para dar fe de que el cliente ha aceptado el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="41f64-120">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="41f64-121">En **Fecha de aceptación del contrato**, introduce la fecha adecuada.</span><span class="sxs-lookup"><span data-stu-id="41f64-121">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="41f64-122">No puedes elegir para esto una fecha futura.</span><span class="sxs-lookup"><span data-stu-id="41f64-122">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="41f64-123">Comprueba que la información de contacto del usuario principal que se muestra sea correcta.</span><span class="sxs-lookup"><span data-stu-id="41f64-123">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="41f64-124">Si no es correcta, selecciona **Actualizar** y escribe la información exacta de la persona que aceptó el contrato.</span><span class="sxs-lookup"><span data-stu-id="41f64-124">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="41f64-125">Selecciona **Siguiente** para continuar con la creación del inquilino del cliente.</span><span class="sxs-lookup"><span data-stu-id="41f64-125">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Cliente nuevo.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="41f64-127">Confirmar la aceptación de los clientes existentes</span><span class="sxs-lookup"><span data-stu-id="41f64-127">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="41f64-128">Debes ser agente de administración o de ventas para poder hacer esto:</span><span class="sxs-lookup"><span data-stu-id="41f64-128">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="41f64-129">Selecciona **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="41f64-129">Select **Customers**.</span></span> <span data-ttu-id="41f64-130">Busca y selecciona el cliente.</span><span class="sxs-lookup"><span data-stu-id="41f64-130">Find and select the customer.</span></span>

2. <span data-ttu-id="41f64-131">Selecciona **Información de cuenta**.</span><span class="sxs-lookup"><span data-stu-id="41f64-131">Select **Account info**.</span></span>

3. <span data-ttu-id="41f64-132">En **Contrato de cliente de Microsoft**, selecciona **Actualizar**.</span><span class="sxs-lookup"><span data-stu-id="41f64-132">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="41f64-133">Escribe el **Nombre**, los **Apellidos**, la **Dirección de correo electrónico** y el **Número de teléfono** (opcional) de la persona que aceptó el contrato.</span><span class="sxs-lookup"><span data-stu-id="41f64-133">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="41f64-134">En **Fecha de aceptación del contrato**, introduce la fecha adecuada.</span><span class="sxs-lookup"><span data-stu-id="41f64-134">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="41f64-135">No puedes elegir para esto una fecha futura.</span><span class="sxs-lookup"><span data-stu-id="41f64-135">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="41f64-136">Selecciona **Guardar** y continúa.</span><span class="sxs-lookup"><span data-stu-id="41f64-136">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Cliente existente.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="41f64-138">Recuperar la confirmación de la aceptación del cliente</span><span class="sxs-lookup"><span data-stu-id="41f64-138">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="41f64-139">Siga los pasos que se describen a continuación para recuperar la confirmación de que un cliente existente ha aceptado el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="41f64-139">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="41f64-140">Debes ser agente de administración o agente de ventas para poder hacer esto.</span><span class="sxs-lookup"><span data-stu-id="41f64-140">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="41f64-141">Selecciona **Clientes** y, a continuación, busca y selecciona el cliente que quieras ver.</span><span class="sxs-lookup"><span data-stu-id="41f64-141">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="41f64-142">Selecciona **Información de cuenta**.</span><span class="sxs-lookup"><span data-stu-id="41f64-142">Select **Account info**.</span></span>

3. <span data-ttu-id="41f64-143">En **Contrato de cliente de Microsoft**, consulta si el cliente ha proporcionado la confirmación.</span><span class="sxs-lookup"><span data-stu-id="41f64-143">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="41f64-144">Confirmación de la aceptación por parte del cliente mediante el SDK o la API del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="41f64-144">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="41f64-145">Puedes usar el SDK o la API del Centro de partners para confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="41f64-145">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="41f64-146">Para obtener más información sobre la API o el SDK, consulta:</span><span class="sxs-lookup"><span data-stu-id="41f64-146">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="41f64-147">Obtener los metadatos del acuerdo del Contrato de cliente de Microsoft</span><span class="sxs-lookup"><span data-stu-id="41f64-147">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="41f64-148">Confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft</span><span class="sxs-lookup"><span data-stu-id="41f64-148">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="41f64-149">Obtener la confirmación de la aceptación por parte del cliente del Contrato de cliente de Microsoft</span><span class="sxs-lookup"><span data-stu-id="41f64-149">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="41f64-150">Obtener un vínculo de descarga para la plantilla del Contrato de cliente de Microsoft</span><span class="sxs-lookup"><span data-stu-id="41f64-150">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="41f64-151">Opción 2: Aceptación del cliente en el Centro de administración de Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="41f64-151">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="41f64-152">Los partners pueden invitar a clientes nuevos y existentes, a través de una dirección URL, para que revisen y acepten el contrato en el Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="41f64-152">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="41f64-153">En las siguientes secciones se muestra cómo puedes:</span><span class="sxs-lookup"><span data-stu-id="41f64-153">The next few sections show you how to:</span></span>

- <span data-ttu-id="41f64-154">Crear un cliente nuevo e invitarlo para que revise y acepte el contrato.</span><span class="sxs-lookup"><span data-stu-id="41f64-154">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="41f64-155">Invitar a un cliente nuevo para que revise y acepte la relación y el contrato de revendedor.</span><span class="sxs-lookup"><span data-stu-id="41f64-155">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="41f64-156">Invitar a un cliente existente para que revise y acepte el contrato.</span><span class="sxs-lookup"><span data-stu-id="41f64-156">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="41f64-157">Puedes usar el [SDK o la API del Centro de partners](/partner-center/develop/get-direct-sign-status-of-customer-agreement) para obtener el estado de la aceptación directa por parte de un cliente del Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="41f64-157">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="41f64-158">Crear un cliente nuevo e invitarlo para que revise y acepte el contrato</span><span class="sxs-lookup"><span data-stu-id="41f64-158">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="41f64-159">Sigue los pasos que se indican a continuación para crear un cliente nuevo en el Centro de partners e invitarlo para que revise y acepte el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="41f64-159">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="41f64-160">En la pestaña **Clientes** del Centro de partners, selecciona **Agregar cliente**.</span><span class="sxs-lookup"><span data-stu-id="41f64-160">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="41f64-161">En **Información de la cuenta**, escribe la información sobre el nuevo cliente en todos los campos obligatorios, incluido el nombre de la empresa del cliente y el contacto principal.</span><span class="sxs-lookup"><span data-stu-id="41f64-161">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="41f64-162">En **Contrato de cliente**, seleccione **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center** (Se pedirá al cliente que acepte el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365).</span><span class="sxs-lookup"><span data-stu-id="41f64-162">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="41f64-163">Completa los demás campos obligatorios en la página.</span><span class="sxs-lookup"><span data-stu-id="41f64-163">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="41f64-164">Selecciona **Siguiente: revisión** y sigue los pasos para crear el inquilino del cliente.</span><span class="sxs-lookup"><span data-stu-id="41f64-164">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="41f64-165">Los clientes nuevos no pueden hacer compras hasta que acepten el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="41f64-165">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Crear un cliente nuevo.":::

5. <span data-ttu-id="41f64-167">Cuando llegues a la pantalla **Confirmación** del nuevo flujo de trabajo del cliente, guarda las credenciales del cliente.</span><span class="sxs-lookup"><span data-stu-id="41f64-167">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="41f64-168">Deberás proporcionar estas credenciales al cliente más adelante.</span><span class="sxs-lookup"><span data-stu-id="41f64-168">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="41f64-169">Fuera del Centro de partners, crea y envía un correo electrónico en el que invites al cliente a aceptar el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="41f64-169">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="41f64-170">Asegúrate de incluir los elementos siguientes en el correo electrónico:</span><span class="sxs-lookup"><span data-stu-id="41f64-170">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="41f64-171">Un vínculo a esta[ dirección URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (inicio de sesión obligatorio)</span><span class="sxs-lookup"><span data-stu-id="41f64-171">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="41f64-172">Las credenciales del cliente que guardó en el paso 5.</span><span class="sxs-lookup"><span data-stu-id="41f64-172">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="41f64-173">A continuación, el cliente recibirá la invitación por correo electrónico del partner y seleccionará la [dirección URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="41f64-173">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="41f64-174">El cliente deberá iniciar sesión en el Centro de administración de Microsoft 365 con las credenciales del cliente que recibió.</span><span class="sxs-lookup"><span data-stu-id="41f64-174">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="41f64-175">El cliente marcará la casilla para aceptar el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="41f64-175">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="41f64-176">Invitación de un cliente nuevo para que revise y acepte la relación de revendedor y el Contrato de cliente de Microsoft</span><span class="sxs-lookup"><span data-stu-id="41f64-176">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="41f64-177">Usa los pasos siguientes para invitar a un nuevo cliente para que revise y acepte la relación de revendedor y el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="41f64-177">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="41f64-178">En la pestaña **Clientes** en el Centro de partners, selecciona el vínculo **Solicitar una relación de revendedor**.</span><span class="sxs-lookup"><span data-stu-id="41f64-178">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="41f64-179">Se generará una plantilla de correo electrónico automático, que incluirá texto y una dirección URL parametrizada que dirigirá al cliente al Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="41f64-179">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="41f64-180">Puedes personalizar la plantilla de correo electrónico generada automáticamente y, a continuación, seleccionar **Copiar al portapapeles** o **Abrir en correo**.</span><span class="sxs-lookup"><span data-stu-id="41f64-180">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="41f64-181">Usa esta plantilla de correo electrónico para invitar al cliente a aceptar la solicitud de **relación de revendedor** y el **Contrato de cliente de Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="41f64-181">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="41f64-182">(Nota: En la invitación por correo electrónico, asegúrate de que el partner también incluye la dirección URL que se proporcionó automáticamente, así como las credenciales del cliente que se crearon recientemente).</span><span class="sxs-lookup"><span data-stu-id="41f64-182">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="Crear una relación.":::

5. <span data-ttu-id="41f64-184">El cliente recibirá una invitación por correo electrónico y hará clic en la dirección URL parametrizada.</span><span class="sxs-lookup"><span data-stu-id="41f64-184">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="41f64-185">El cliente usará las credenciales proporcionadas en el correo electrónico para iniciar sesión en el Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="41f64-185">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="41f64-186">El cliente marcará la casilla para aceptar la **relación de revendedor** y el **Contrato de cliente de Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="41f64-186">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="41f64-187">En la misma dirección URL, el cliente podrá ver una lista consolidada de los diferentes partners con los que trabaja.</span><span class="sxs-lookup"><span data-stu-id="41f64-187">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="41f64-188">Podrá seleccionar un partner para ver los detalles.</span><span class="sxs-lookup"><span data-stu-id="41f64-188">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Aceptar el contrato.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="41f64-190">Invitación de un cliente existente para que revise y acepte el contrato</span><span class="sxs-lookup"><span data-stu-id="41f64-190">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="41f64-191">Usa los pasos siguientes para invitar a un cliente existente para que revise y acepte el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="41f64-191">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="41f64-192">Crea el correo electrónico del cliente con la dirección URL incrustada para invitar a tu cliente para que acepte el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="41f64-192">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="41f64-193">El cliente recibe la invitación por correo electrónico y hace clic en la [dirección URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="41f64-193">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="41f64-194">El cliente escribe sus credenciales en el Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="41f64-194">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="41f64-195">El cliente marcará la casilla para aceptar el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="41f64-195">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="41f64-196">En la misma dirección URL, el cliente podrá ver la lista consolidada de los diferentes partners con los que trabaja.</span><span class="sxs-lookup"><span data-stu-id="41f64-196">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="41f64-197">Podrá seleccionar un partner para ver los detalles.</span><span class="sxs-lookup"><span data-stu-id="41f64-197">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Cliente.":::

>[!NOTE]
><span data-ttu-id="41f64-199">En determinados escenarios, es posible que los clientes no puedan aceptar directamente el Contrato de cliente de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="41f64-199">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="41f64-200">Para obtener más información sobre estas situaciones, consulte Dos escenarios en los que es necesario dar fe en nombre del cliente, a continuación.</span><span class="sxs-lookup"><span data-stu-id="41f64-200">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="41f64-201">Dos escenarios en los que es necesario dar fe en nombre de tu cliente</span><span class="sxs-lookup"><span data-stu-id="41f64-201">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="41f64-202">Hay dos escenarios en los que es posible que los clientes no puedan aceptar directamente el Contrato de cliente de Microsoft en el Centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="41f64-202">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="41f64-203">**Escenario 1**: un cliente existente que ha comprado cualquier de los productos siguientes a través de una relación de partner existente: ofertas, software o suscripciones de software, instancias reservadas o plan de Azure.</span><span class="sxs-lookup"><span data-stu-id="41f64-203">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="41f64-204">Dicho cliente ahora intenta realizar una nueva compra (esta no incluye la renovación automática).</span><span class="sxs-lookup"><span data-stu-id="41f64-204">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="41f64-205">Cuando el cliente haga clic en la dirección URL, recibirá el mensaje "Póngase en contacto con su partner para confirmar que acepta el Contrato de cliente de Microsoft".</span><span class="sxs-lookup"><span data-stu-id="41f64-205">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="41f64-206">**Para resolverlo**: debes dar fe en nombre del cliente.</span><span class="sxs-lookup"><span data-stu-id="41f64-206">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Captura de pantalla de la página del centro de administración de Microsoft 365 que le pide que se una a su partner para confirmar la aceptación del Contrato de cliente de Microsoft.":::

<span data-ttu-id="41f64-208">**Escenario 2**: un cliente existente que ha adquirido cualquiera de las siguientes ofertas, software y suscripciones de software, instancias reservadas y plan de Azure.</span><span class="sxs-lookup"><span data-stu-id="41f64-208">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="41f64-209">Dicho cliente ahora intenta realizar una nueva compra con un nuevo partner.</span><span class="sxs-lookup"><span data-stu-id="41f64-209">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="41f64-210">Cuando el cliente haga clic en la dirección URL del Centro de administración de Microsoft 365 para aceptar la nueva relación del partner y el contrato, recibirá el mensaje "Póngase en contacto con su partner para confirmar que acepta el Contrato de cliente de Microsoft".</span><span class="sxs-lookup"><span data-stu-id="41f64-210">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="41f64-211">**Para resolverlo**: debes dar fe en nombre del cliente.</span><span class="sxs-lookup"><span data-stu-id="41f64-211">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="41f64-212">Confirmación de que un cliente ha aceptado el contrato</span><span class="sxs-lookup"><span data-stu-id="41f64-212">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="41f64-213">Si intenta crear un nuevo pedido para un cliente existente al que no has confirmado con anterioridad, recibirá un aviso para completar la confirmación.</span><span class="sxs-lookup"><span data-stu-id="41f64-213">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="41f64-214">Usa el siguiente procedimiento para hacerlo.</span><span class="sxs-lookup"><span data-stu-id="41f64-214">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="41f64-215">Escribe el **Nombre**, los **Apellidos**, la **Dirección de correo electrónico** y el **Número de teléfono** (opcional) del usuario que aceptó el contrato.</span><span class="sxs-lookup"><span data-stu-id="41f64-215">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="41f64-216">En **Fecha de aceptación del contrato**, introduce la fecha adecuada.</span><span class="sxs-lookup"><span data-stu-id="41f64-216">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="41f64-217">No puedes elegir para esto una fecha futura.</span><span class="sxs-lookup"><span data-stu-id="41f64-217">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="41f64-218">Selecciona **Guardar y continuar**.</span><span class="sxs-lookup"><span data-stu-id="41f64-218">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="41f64-219">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="41f64-219">Next steps</span></span>

- [<span data-ttu-id="41f64-220">Comprobar o actualizar la información del perfil de empresa</span><span class="sxs-lookup"><span data-stu-id="41f64-220">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="41f64-221">Contratos de cliente de Microsoft (por región, idioma)</span><span class="sxs-lookup"><span data-stu-id="41f64-221">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
