---
title: Cambiar el socio de facturación directo a revendedor indirecto
ms.topic: how-to
ms.date: 06/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo un asociado del programa CSP puede usar el centro de partners para realizar la transición de un asociado de factura directa al revendedor indirecto.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e3cd791f5f9f781980d73c79f0ec18627585372a
ms.sourcegitcommit: b4771fd0781d95551e65baa481a572291c729d7d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/28/2020
ms.locfileid: "92795872"
---
# <a name="transition-from-cloud-solution-provider-csp-direct-bill-partner-to-csp-indirect-reseller"></a><span data-ttu-id="f261c-103">Transición de asociado de factura directa del Proveedor de soluciones en la nube (CSP) a revendedor indirecto de CSP</span><span class="sxs-lookup"><span data-stu-id="f261c-103">Transition from Cloud Solution Provider (CSP) direct bill partner to CSP indirect reseller</span></span>

<span data-ttu-id="f261c-104">**Se aplica a:**</span><span class="sxs-lookup"><span data-stu-id="f261c-104">**Applies to:**</span></span>
- <span data-ttu-id="f261c-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="f261c-105">Partner Center</span></span>

<span data-ttu-id="f261c-106">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="f261c-106">**Appropriate roles**</span></span>

- <span data-ttu-id="f261c-107">Todos los partners de factura directa del CSP</span><span class="sxs-lookup"><span data-stu-id="f261c-107">All CSP direct bill partners</span></span>

>[!Note]
><span data-ttu-id="f261c-108">Este artículo está destinado a los asociados directos de facturación que han decidido realizar la transición a los revendedores indirectos.</span><span class="sxs-lookup"><span data-stu-id="f261c-108">This article is intended for direct bill partners who have decided to transition to indirect resellers.</span></span> <span data-ttu-id="f261c-109">Sin embargo, aunque no haya tomado una decisión explícita todavía para inscribirse como revendedor indirecto, Microsoft informará a los asociados de factura directos que no cumplan los [requisitos](direct-partner-new-requirements.md) nuevos para el programa de socio de facturación directo de CSP cuando se [restrinjan sus capacidades de factura directa](restricted-direct-bill-capabilities.md).</span><span class="sxs-lookup"><span data-stu-id="f261c-109">However, even if you have not made an explicit decision yet to enroll as an indirect reseller, direct bill partners who do not meet the new [requirements](direct-partner-new-requirements.md) for the CSP direct bill partner program will be informed by Microsoft when their [direct bill capabilities will be restricted](restricted-direct-bill-capabilities.md).</span></span>
<br><span data-ttu-id="f261c-110">A partir del 2021 de enero, se agregará un nuevo requisito de ingresos.</span><span class="sxs-lookup"><span data-stu-id="f261c-110">As of January 2021, a new revenue requirement will be added.</span></span> <span data-ttu-id="f261c-111">Los asociados inscritos como asociados directos de factura deberán haber transaccionado al menos USD $300 000 en el programa del proveedor de soluciones en la nube en un nivel de cuenta global de socio durante los 12 meses anteriores.</span><span class="sxs-lookup"><span data-stu-id="f261c-111">Partners enrolled as a direct bill partner will need to have transacted at least USD$300K in Cloud Solution Provider program revenue at a Partner Global Account level over the previous 12 months.</span></span>

<span data-ttu-id="f261c-112">Podrá inscribirse en el programa de revendedor indirecto con el inquilino de factura directo existente.</span><span class="sxs-lookup"><span data-stu-id="f261c-112">You will be able to enroll in the indirect reseller program using your existing direct bill tenant.</span></span>

## <a name="get-started"></a><span data-ttu-id="f261c-113">Introducción</span><span class="sxs-lookup"><span data-stu-id="f261c-113">Get started</span></span>

1. <span data-ttu-id="f261c-114">Asegúrese de que el perfil de socio comercial en el centro de Partners y el ID. de MPN están actualizados.</span><span class="sxs-lookup"><span data-stu-id="f261c-114">Make sure your partner profile in Partner Center and MPN ID are current.</span></span>

2. <span data-ttu-id="f261c-115">Inicie sesión en el centro de partners como administrador global del inquilino de facturación directo que va a pasar al revendedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-115">Sign in to Partner Center as the global admin for the direct bill tenant you are transitioning to indirect reseller.</span></span>

   :::image type="content" source="images/direct/direct1.png" alt-text="Información general":::

3. <span data-ttu-id="f261c-117">Revise los detalles de su asociado en el formulario de inscripción.</span><span class="sxs-lookup"><span data-stu-id="f261c-117">Review your partner details on the enrollment form.</span></span>

   :::image type="content" source="images/direct/direct2a.png" alt-text="Inscribirse ahora":::

4. <span data-ttu-id="f261c-119">Selecciona Inscribirse ahora.</span><span class="sxs-lookup"><span data-stu-id="f261c-119">Select Enroll now.</span></span> <span data-ttu-id="f261c-120">Su empresa de revendedores indirectos usará el mismo inquilino de AAD que usa para su negocio directo.</span><span class="sxs-lookup"><span data-stu-id="f261c-120">Your indirect reseller business will use the same AAD tenant you use for your direct business.</span></span>

    > [!NOTE]
    > <span data-ttu-id="f261c-121">En principio, esta nueva funcionalidad de transición estará disponible para los partners con fechas de aniversario entre septiembre y diciembre.</span><span class="sxs-lookup"><span data-stu-id="f261c-121">Initially, this new transition capability will be available for partners with September to December anniversary dates.</span></span> <span data-ttu-id="f261c-122">Si no tiene una fecha de aniversario entre septiembre y diciembre, no verá la funcionalidad en este momento.</span><span class="sxs-lookup"><span data-stu-id="f261c-122">If you don"t have an anniversary date between September and December, you won't see the capability at this time.</span></span> <span data-ttu-id="f261c-123">Los partners con fechas aniversario posteriores a diciembre de 2018 recibirán notificación una vez que la función esté habilitada para estos partners.</span><span class="sxs-lookup"><span data-stu-id="f261c-123">Partners with anniversary dates after December 2018 will be notified later once the feature is enabled for the partners.</span></span>

5. <span data-ttu-id="f261c-124">Cuando se apruebe la inscripción, vuelva a iniciar sesión en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="f261c-124">When your enrollment is approved, sign in to Partner Center again.</span></span>

    > [!NOTE]
    > <span data-ttu-id="f261c-125">Aunque la aprobación es normalmente inmediata, puede tardar hasta cinco días laborables.</span><span class="sxs-lookup"><span data-stu-id="f261c-125">While approval is usually immediate, it can take up to five business days.</span></span> <span data-ttu-id="f261c-126">Una vez aprobada, recibirá una notificación a la dirección de correo electrónico que especificó en contacto principal en el formulario de inscripción.</span><span class="sxs-lookup"><span data-stu-id="f261c-126">Once approved, you will receive a notification to the email address you have specified under primary contact in the enrollment form.</span></span> <span data-ttu-id="f261c-127">También puede comprobar el estado de inscripción en **configuración**  >  **asociado configuración**  >  **Perfil de socio** > información del programa.</span><span class="sxs-lookup"><span data-stu-id="f261c-127">You can also check your enrollment status under **Settings** > **Partner Settings** > **Partner Profile** > Program info.</span></span>

6. <span data-ttu-id="f261c-128">En la página de **información general** , verá el contrato de revendedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-128">On your **Overview** page, you will see the indirect reseller agreement.</span></span> <span data-ttu-id="f261c-129">Selecciona **Aceptar y continuar** .</span><span class="sxs-lookup"><span data-stu-id="f261c-129">Select **Accept and continue** .</span></span> <span data-ttu-id="f261c-130">Esta acción habilita las capacidades de revendedor indirectos.</span><span class="sxs-lookup"><span data-stu-id="f261c-130">This action enables the indirect reseller capabilities.</span></span>

<span data-ttu-id="f261c-131">Cuando haya aceptado el contrato de revendedor indirecto, tenga en cuenta que el **Perfil de socio** comercial lo identifica como una factura directa y un revendedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-131">When you have accepted the indirect reseller agreement, notice that your Partner profile identifies you as **both** a direct bill and indirect reseller.</span></span>

:::image type="content" source="images/direct/direct3.png" alt-text="Acuerdo de revendedor indirecto":::

> [!IMPORTANT]
> <span data-ttu-id="f261c-133">Una vez que se inscribe como revendedor indirecto mediante la nueva funcionalidad, no hay ninguna opción para revertir a un inquilino de solo facturación directo.</span><span class="sxs-lookup"><span data-stu-id="f261c-133">Once you enroll as an indirect reseller using the new capability, there is no option to roll back to a direct bill- only tenant.</span></span> <span data-ttu-id="f261c-134">Asegúrate de evaluar completamente evaluar las necesidades de tu empresa antes de inscribirte como revendedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-134">Please make sure that you fully evaluate your business needs before enrolling as an indirect reseller.</span></span>

## <a name="while-you-transition-from-direct-to-indirect-reseller"></a><span data-ttu-id="f261c-135">Mientras realiza la transición de directo a revendedor indirecto</span><span class="sxs-lookup"><span data-stu-id="f261c-135">While you transition from direct to indirect reseller</span></span>

<span data-ttu-id="f261c-136">Durante esta fase, seguirá administrando las necesidades de suscripción de sus clientes directos, incluido el proceso de facturación.</span><span class="sxs-lookup"><span data-stu-id="f261c-136">During this phase, you will continue to manage your direct customers' subscription needs including the billing process.</span></span> <span data-ttu-id="f261c-137">También puede empezar a aceptar clientes de su proveedor indirecto y a trabajar como un revendedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-137">You can also begin accepting customers from your Indirect provider and operating as an indirect reseller.</span></span>

:::image type="content" source="images/direct/direct4.png" alt-text="Es una factura directa y un revendedor indirecto":::

## <a name="find-an-indirect-provider"></a><span data-ttu-id="f261c-139">Encontrar un proveedor indirecto</span><span class="sxs-lookup"><span data-stu-id="f261c-139">Find an indirect provider</span></span>

<span data-ttu-id="f261c-140">Después de la inscripción, aparecerá un vínculo a los proveedores indirectos en el panel de navegación izquierdo.</span><span class="sxs-lookup"><span data-stu-id="f261c-140">After enrolling, a link to Indirect providers will appear in your left nav.</span></span> <span data-ttu-id="f261c-141">Como revendedor indirecto, establecerá una relación con un proveedor indirecto que, a continuación, podrá administrar la facturación, comprar productos para sus clientes y ofrecer soporte técnico a la infraestructura.</span><span class="sxs-lookup"><span data-stu-id="f261c-141">As an indirect reseller you will establish a relationship with an indirect provider who then can handle your billing, purchase products for your customers, and support infrastructure.</span></span>

<span data-ttu-id="f261c-142">Los diferentes proveedores indirectos ofrecen diferentes servicios y soporte técnico, por lo que deberías evaluar a los proveedores en tu zona para determinar cuál de ellos se ajusta mejor a tus necesidades.</span><span class="sxs-lookup"><span data-stu-id="f261c-142">Different indirect providers offer different support and services, so you should evaluate the providers in your area to determine which ones best meet your needs.</span></span> <span data-ttu-id="f261c-143">Por lo general, la mayoría de los proveedores ofrece lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="f261c-143">Generally, most providers will:</span></span>

- <span data-ttu-id="f261c-144">Proporcionarte formación y asistencia técnicas</span><span class="sxs-lookup"><span data-stu-id="f261c-144">Provide you with technical training and assistance</span></span>
- <span data-ttu-id="f261c-145">Ayuda para comercializar tus productos y servicios</span><span class="sxs-lookup"><span data-stu-id="f261c-145">Help you market your products and services</span></span>
- <span data-ttu-id="f261c-146">Administrar la financiación y los términos de crédito</span><span class="sxs-lookup"><span data-stu-id="f261c-146">Manage your financing and credit terms</span></span>

<span data-ttu-id="f261c-147">Busque en la lista de [proveedores de Microsoft indirectos](https://partnercenter.microsoft.com/partner/find-a-provider)oficiales.</span><span class="sxs-lookup"><span data-stu-id="f261c-147">Search the list of official [Microsoft indirect providers](https://partnercenter.microsoft.com/partner/find-a-provider).</span></span>

<span data-ttu-id="f261c-148">Más información, leer  [asociado con proveedores indirectos](indirect-reseller-tasks-in-partner-center.md)</span><span class="sxs-lookup"><span data-stu-id="f261c-148">Learn more, read  [Partner with indirect providers](indirect-reseller-tasks-in-partner-center.md)</span></span>

## <a name="accept-a-partnership-invitation-from-your-indirect-provider"></a><span data-ttu-id="f261c-149">Aceptación de una invitación de Asociación de su proveedor indirecto</span><span class="sxs-lookup"><span data-stu-id="f261c-149">Accept a partnership invitation from your indirect provider</span></span>

<span data-ttu-id="f261c-150">Cuando encuentre un proveedor indirecto con el que asociar, establezca una asociación con el proveedor indirecto en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="f261c-150">When you find an indirect provider to partner with, establish a partnership with the indirect provider in Partner Center.</span></span>

<span data-ttu-id="f261c-151">El proveedor indirecto que seleccione le enviará por correo electrónico un vínculo de invitación de asociación que le llevará a su invitación en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="f261c-151">The indirect provider you select will send you in email a partnership invitation link that will take you to their invitation in Partner Center.</span></span> <span data-ttu-id="f261c-152">Asegúrese de que el administrador global inicia sesión en el centro de Partners y sigue el vínculo de invitación.</span><span class="sxs-lookup"><span data-stu-id="f261c-152">Be sure your global admin signs in to Partner Center and follows the invitation link.</span></span> <span data-ttu-id="f261c-153">Al aceptar la invitación, el nombre del proveedor aparecerá en la lista de proveedores indirectos.</span><span class="sxs-lookup"><span data-stu-id="f261c-153">When you accept the invitation, the provider's name will appear in your indirect provider list.</span></span>

## <a name="acquire-new-customers-as-indirect-reseller"></a><span data-ttu-id="f261c-154">Adquiera nuevos clientes como revendedores indirectos</span><span class="sxs-lookup"><span data-stu-id="f261c-154">Acquire new customers as indirect reseller</span></span>

<span data-ttu-id="f261c-155">Tanto usted como su proveedor indirecto deben tener relaciones de reseller con los clientes.</span><span class="sxs-lookup"><span data-stu-id="f261c-155">Both you and your indirect provider need to have reseller relationships with customers.</span></span> <span data-ttu-id="f261c-156">Estas relaciones del reseller le permiten administrar las suscripciones y servicios de un cliente en su nombre.</span><span class="sxs-lookup"><span data-stu-id="f261c-156">These reseller relationships enable you to manage a customer's subscriptions and services on their behalf.</span></span> <span data-ttu-id="f261c-157">Para adquirir un nuevo cliente que tenga un inquilino de Azure AD existente, puede invitar al cliente a establecer una relación de revendedor con usted y su proveedor al mismo tiempo.</span><span class="sxs-lookup"><span data-stu-id="f261c-157">To acquire a new customer who has an existing Azure AD tenant, you can invite the customer to establish a reseller relationship with both you and your provider at the same time.</span></span>

<span data-ttu-id="f261c-158">Para crear una invitación de revendedor indirecto:</span><span class="sxs-lookup"><span data-stu-id="f261c-158">To create an indirect reseller invitation:</span></span>

1. <span data-ttu-id="f261c-159">Seleccione **proveedores indirectos** en el panel de navegación izquierdo del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="f261c-159">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="f261c-160">Selecciona **Invitar a nuevos clientes** para invitar a un cliente a establecer una relación de revendedor contigo y con el proveedor indirecto a la vez.</span><span class="sxs-lookup"><span data-stu-id="f261c-160">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="f261c-161">El proveedor debe tener una relación de revendedor con el cliente, para que puedan enviar pedidos en nombre del cliente cuando el cliente desee comprar nuevas suscripciones o agregar nuevas licencias a las suscripciones existentes.</span><span class="sxs-lookup"><span data-stu-id="f261c-161">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

3. <span data-ttu-id="f261c-162">En la página siguiente, revise el borrador del mensaje de correo electrónico.</span><span class="sxs-lookup"><span data-stu-id="f261c-162">On the next page, review the draft email message.</span></span> <span data-ttu-id="f261c-163">Puede abrir el borrador de mensajes en el correo electrónico, o puede copiar el mensaje en el portapapeles y pegarlo en un correo electrónico.</span><span class="sxs-lookup"><span data-stu-id="f261c-163">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="f261c-164">Edite el texto del correo electrónico para indicar lo que necesita, pero asegúrese de incluir el vínculo, ya que está personalizado para conectar el cliente directamente a su cuenta y a la cuenta del proveedor.</span><span class="sxs-lookup"><span data-stu-id="f261c-164">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="f261c-165">A continuación, seleccione **Done** (Listo).</span><span class="sxs-lookup"><span data-stu-id="f261c-165">Then select **Done** .</span></span>

5. <span data-ttu-id="f261c-166">Una vez que el cliente te autorice a ti y tu proveedor como revendedores de registro, tendrás permisos de administrador para administrar sus suscripciones, licencias y usuarios en su nombre y tu proveedor indirecto podrá enviar pedidos en su nombre.</span><span class="sxs-lookup"><span data-stu-id="f261c-166">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>
6. <span data-ttu-id="f261c-167">Para administrar la cuenta, los servicios, los usuarios y las licencias del cliente, expande el registro del cliente seleccionando la flecha abajo situada junto a su nombre.</span><span class="sxs-lookup"><span data-stu-id="f261c-167">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

<span data-ttu-id="f261c-168">A diferencia de los asociados directos de facturación, los revendedores indirectos no pueden crear Azure AD inquilinos para sus nuevos clientes en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="f261c-168">Unlike direct bill partners, indirect resellers can't create Azure AD tenants for their new customers in Partner Center.</span></span> <span data-ttu-id="f261c-169">El proveedor creará el inquilino y lo especificará como revendedor indirecto para este cliente.</span><span class="sxs-lookup"><span data-stu-id="f261c-169">Your provider will create the tenant and will specify you as the indirect reseller for this customer.</span></span> <span data-ttu-id="f261c-170">Esto garantiza que el cliente aparecerá en la lista de clientes del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="f261c-170">This ensures that the customer will appear in your customer list in Partner Center.</span></span>

>[!Note]
><span data-ttu-id="f261c-171">No podrá usar la capacidad de factura directa para crear compras para los clientes que adquiera como revendedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-171">You will not be able to use your direct bill capability to create purchases for customers you acquire as an indirect reseller.</span></span>

## <a name="managing-your-direct-bill-customers-and-your-indirect-reseller-customers"></a><span data-ttu-id="f261c-172">Administración de los clientes directos de facturación y sus clientes de revendedores indirectos</span><span class="sxs-lookup"><span data-stu-id="f261c-172">Managing your direct bill customers and your indirect reseller customers</span></span>

<span data-ttu-id="f261c-173">Usted administra los clientes directos de facturación y sus clientes de revendedores indirectos de forma diferente.</span><span class="sxs-lookup"><span data-stu-id="f261c-173">You manage your direct bill customers and your indirect reseller customers differently.</span></span>

### <a name="direct-bill-customers-things-you-wont-do-as-an-indirect-reseller"></a><span data-ttu-id="f261c-174">Clientes directos de facturación (cosas que no se realizarán como revendedores indirectos)</span><span class="sxs-lookup"><span data-stu-id="f261c-174">Direct bill customers (things you won't do as an indirect reseller)</span></span>

- <span data-ttu-id="f261c-175">Crear pedidos para productos</span><span class="sxs-lookup"><span data-stu-id="f261c-175">Create orders for products</span></span>
- <span data-ttu-id="f261c-176">Administración de reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="f261c-176">Manage Azure reservations</span></span>
- <span data-ttu-id="f261c-177">Administrar el historial de pedidos</span><span class="sxs-lookup"><span data-stu-id="f261c-177">Manage their order history</span></span>
- <span data-ttu-id="f261c-178">Comprar software</span><span class="sxs-lookup"><span data-stu-id="f261c-178">Purchase software</span></span>
- <span data-ttu-id="f261c-179">Facturar directamente a los clientes</span><span class="sxs-lookup"><span data-stu-id="f261c-179">Bill customers directly</span></span>

### <a name="indirect-reseller-customers"></a><span data-ttu-id="f261c-180">Clientes de revendedores indirectos</span><span class="sxs-lookup"><span data-stu-id="f261c-180">Indirect reseller customers</span></span>

- <span data-ttu-id="f261c-181">El proveedor indirecto ordena los productos de sus clientes</span><span class="sxs-lookup"><span data-stu-id="f261c-181">Your indirect provider orders products for your customers</span></span>
- <span data-ttu-id="f261c-182">Administrar las licencias y los usuarios de los clientes</span><span class="sxs-lookup"><span data-stu-id="f261c-182">Manage customers' licenses and users</span></span>
- <span data-ttu-id="f261c-183">Controlar las renovaciones de suscripción</span><span class="sxs-lookup"><span data-stu-id="f261c-183">Handle subscription renewals</span></span>

### <a name="to-identify-customers-that-you-acquired-as-a-direct-bill-partner"></a><span data-ttu-id="f261c-184">Para identificar a los clientes adquiridos como asociados directos de factura</span><span class="sxs-lookup"><span data-stu-id="f261c-184">To identify customers that you acquired as a direct bill partner</span></span>

1. <span data-ttu-id="f261c-185">Seleccionar **clientes**</span><span class="sxs-lookup"><span data-stu-id="f261c-185">Select **Customers**</span></span>

2. <span data-ttu-id="f261c-186">Seleccionar un cliente para ver sus detalles</span><span class="sxs-lookup"><span data-stu-id="f261c-186">Select a customer to view their details</span></span>

3. <span data-ttu-id="f261c-187">Si este cliente es el que ha adquirido como asociado directo de factura, verá opciones para **Agregar** o **Ver productos** y verá sus suscripciones.</span><span class="sxs-lookup"><span data-stu-id="f261c-187">If this customer is one you acquired as a direct bill partner, you will see options to **add** or **view products** and you will see their subscriptions.</span></span>

4. <span data-ttu-id="f261c-188">Si el cliente tiene una relación de revendedor indirecta con usted, esas opciones no estarán disponibles.</span><span class="sxs-lookup"><span data-stu-id="f261c-188">If the customer has an indirect reseller relationship with you, those options will not be available.</span></span>

## <a name="move-your-direct-bill-customers-to-your-indirect-provider"></a><span data-ttu-id="f261c-189">Traslade a los clientes directos de facturación a su proveedor indirecto</span><span class="sxs-lookup"><span data-stu-id="f261c-189">Move your direct bill customers to your indirect provider</span></span>

<span data-ttu-id="f261c-190">El proveedor indirecto no puede enviar pedidos ni transferencias de suscripciones existentes para los clientes de factura directos existentes hasta que tengan una relación de revendedor con ellos.</span><span class="sxs-lookup"><span data-stu-id="f261c-190">Your indirect provider cannot submit orders or existing subscription transfers for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="f261c-191">Para establecer la relación de revendedor entre el proveedor indirecto y el cliente de factura directo existente, puede usar uno de los métodos siguientes:</span><span class="sxs-lookup"><span data-stu-id="f261c-191">To establish the reseller relationship between your indirect provider and your existing direct bill customer, you can use one of the following methods:</span></span>

- [<span data-ttu-id="f261c-192">Extensión reseller Relationship</span><span class="sxs-lookup"><span data-stu-id="f261c-192">Reseller relationship extension</span></span>](#reseller-relationship-extension)

- [<span data-ttu-id="f261c-193">Enviar una invitación de revendedor indirecto al cliente</span><span class="sxs-lookup"><span data-stu-id="f261c-193">Send an indirect reseller invitation to the customer</span></span>](#send-an-indirect-reseller-invitation-to-the-customer)

<span data-ttu-id="f261c-194">Puede encontrar información general detallada sobre el proceso paso a paso en el [documento de transición Direct to Indirect](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span><span class="sxs-lookup"><span data-stu-id="f261c-194">You can find a detailed overview of the step-by-step process in the [Direct to indirect transition document](https://partner.microsoft.com/resources/collection/Direct-Bill-transition-to-Indirect-reseller#/)</span></span>

### <a name="reseller-relationship-extension"></a><span data-ttu-id="f261c-195">Extensión reseller Relationship</span><span class="sxs-lookup"><span data-stu-id="f261c-195">Reseller relationship extension</span></span>

<span data-ttu-id="f261c-196">Puede usar la característica de extensión de relación reseller para establecer la relación de revendedor entre los clientes de facturación directos existentes y el proveedor indirecto mediante el panel del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="f261c-196">You can use the reseller relationship extension feature to establish reseller relationship between your existing direct bill customers and your indirect provider using Partner Center Dashboard.</span></span> <span data-ttu-id="f261c-197">Antes de usar la característica, tenga en cuenta lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="f261c-197">Before using the feature, note the following:</span></span>

- <span data-ttu-id="f261c-198">Esta característica solo está disponible para los asociados directos de facturación que están cambiando para convertirse en un revendedor indirecto que ha completado la [inscripción de revendedores indirectos](#get-started).</span><span class="sxs-lookup"><span data-stu-id="f261c-198">This feature is only available to direct bill partners who are transitioning to become an indirect reseller have completed the [indirect reseller enrollment](#get-started).</span></span>

- <span data-ttu-id="f261c-199">Esta característica solo se puede aplicar a los clientes de facturación directa existentes.</span><span class="sxs-lookup"><span data-stu-id="f261c-199">You can only apply this feature to existing direct bill customers.</span></span> <span data-ttu-id="f261c-200">No es aplicable a [los clientes de revendedores indirectos](#acquire-new-customers-as-indirect-reseller).</span><span class="sxs-lookup"><span data-stu-id="f261c-200">It is not applicable to [indirect reseller customers](#acquire-new-customers-as-indirect-reseller).</span></span>

- <span data-ttu-id="f261c-201">Solo puede seleccionar un proveedor indirecto para el que haya [aceptado una invitación de socio comercial de su proveedor indirecto](#accept-a-partnership-invitation-from-your-indirect-provider).</span><span class="sxs-lookup"><span data-stu-id="f261c-201">You can only select an indirect provider for which you have [accepted a partner invitation from your indirect provider](#accept-a-partnership-invitation-from-your-indirect-provider).</span></span>

- <span data-ttu-id="f261c-202">Una copia de la información de facturación que tenga para este cliente estará disponible para el proveedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-202">A copy of the bill-to info you have for this customer will be made available to the indirect provider.</span></span> <span data-ttu-id="f261c-203">Puede acceder a la información de facturación accediendo a la página de la cuenta de este cliente en el panel del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="f261c-203">You can access the bill-to info by accessing the Account page for this customer in Partner Center Dashboard.</span></span>

    > [!NOTE]
    > <span data-ttu-id="f261c-204">Mediante el uso de la característica de extensión reseller Relationship, da su consentimiento para compartir la información de facturación que tiene para este cliente con el proveedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-204">By using the reseller relationship extension feature, you consent to sharing the bill-to info you have for this customer with the indirect provider.</span></span>

- <span data-ttu-id="f261c-205">No se proporcionará a su proveedor indirecto [privilegios de administración delegada](customers-revoke-admin-privileges.md) en el inquilino del cliente.</span><span class="sxs-lookup"><span data-stu-id="f261c-205">Your indirect provider will not be provided with [delegated administration privileges](customers-revoke-admin-privileges.md) to the customer tenant.</span></span> <span data-ttu-id="f261c-206">Si el proveedor indirecto requiere privilegios de administración delegados, debe enviar una invitación de revendedor indirecto al cliente en su lugar.</span><span class="sxs-lookup"><span data-stu-id="f261c-206">If your indirect provider requires delegated administration privileges, you must send an indirect reseller invitation to the customer instead.</span></span>

- <span data-ttu-id="f261c-207">Una vez establecida la relación de revendedor, el proveedor indirecto aparecerá como un asociado de CSP al cliente en la página relaciones de socios comerciales del [centro de administración de M365](https://admin.microsoft.com/AdminPortal/Home#/partners) y [Microsoft Store para empresas](/microsoft-store/work-with-partner-microsoft-store-business).</span><span class="sxs-lookup"><span data-stu-id="f261c-207">Once the reseller relationship is established, the indirect provider will appear as a CSP partner to the customer under the Partner Relationships page in [M365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/partners) and [Microsoft Store for Business](/microsoft-store/work-with-partner-microsoft-store-business).</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="f261c-208">Para evitar confusiones y malentendidos, tiene la obligación contractual del acuerdo de socio comercial de informar y obtener el consentimiento del cliente de factura directa antes de usar la característica de extensión de relación para establecer la relación de revendedor entre un cliente de facturación directo existente y un proveedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-208">To avoid confusion and misunderstanding, you are contractually obliged by your partner agreement to inform and obtain consent from the direct bill customer before you use the relationship extension feature to establish reseller relationship between an existing direct bill customer and an indirect provider.</span></span>

<span data-ttu-id="f261c-209">Para usar esta característica en un inquilino de cliente existente:</span><span class="sxs-lookup"><span data-stu-id="f261c-209">To use this feature on an existing customer tenant:</span></span>

1. <span data-ttu-id="f261c-210">Inicie sesión en el centro de partners como **agente de administración** .</span><span class="sxs-lookup"><span data-stu-id="f261c-210">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="f261c-211">En la **Página clientes** , seleccione un cliente existente y haga clic en el icono **vínculos rápidos** para expandir la vista Resumen del cliente.</span><span class="sxs-lookup"><span data-stu-id="f261c-211">In the **Customers page** , select an existing customer and click on its **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="f261c-212">En **proveedores indirectos** , haga clic en **transferir cliente en un proveedor indirecto** .</span><span class="sxs-lookup"><span data-stu-id="f261c-212">Under **Indirect provider(s)** , click **Transfer customer on an indirect provider** .</span></span>

    :::image type="content" source="images/direct/direct5-1.png" alt-text="Transferir clientes a un proveedor indirecto":::

4. <span data-ttu-id="f261c-214">En el cuadro de diálogo emergente, seleccione el **proveedor indirecto** que le gustaría tener la relación de revendedor con el cliente.</span><span class="sxs-lookup"><span data-stu-id="f261c-214">In the pop-up dialog, select the **Indirect Provider** you would like to have reseller relationship with the customer.</span></span>

5. <span data-ttu-id="f261c-215">Haga clic en **Guardar y continuar** .</span><span class="sxs-lookup"><span data-stu-id="f261c-215">Click **Save and continue** .</span></span>

6. <span data-ttu-id="f261c-216">Compruebe que el proveedor indirecto seleccionado aparece en **proveedores indirectos** .</span><span class="sxs-lookup"><span data-stu-id="f261c-216">Verify the selected indirect provider shows up under **Indirect provider(s)** .</span></span>

    :::image type="content" source="images/direct/direct5-2.png" alt-text="Proveedor indirecto enumerado":::

### <a name="send-an-indirect-reseller-invitation-to-the-customer"></a><span data-ttu-id="f261c-218">Enviar una invitación de revendedor indirecto al cliente</span><span class="sxs-lookup"><span data-stu-id="f261c-218">Send an indirect reseller invitation to the customer</span></span>

<span data-ttu-id="f261c-219">El proveedor indirecto no podrá enviar pedidos para los clientes de factura directos existentes hasta que tengan una relación de revendedor.</span><span class="sxs-lookup"><span data-stu-id="f261c-219">Your indirect provider cannot submit orders for your existing direct bill customers until they have a reseller relationship with them.</span></span> <span data-ttu-id="f261c-220">Para establecer la relación de revendedor entre los clientes existentes y su proveedor indirecto, invite al cliente mediante una invitación de revendedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-220">To establish the reseller relationship between your existing customers and your indirect provider, invite the customer using an indirect reseller invitation.</span></span>

1. <span data-ttu-id="f261c-221">Seleccione **proveedores indirectos** en el panel de navegación izquierdo del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="f261c-221">Select **Indirect providers** from your Partner Center left nav.</span></span>

2. <span data-ttu-id="f261c-222">Selecciona **Invitar a nuevos clientes** para invitar a un cliente a establecer una relación de revendedor contigo y con el proveedor indirecto a la vez.</span><span class="sxs-lookup"><span data-stu-id="f261c-222">Select **Invite new customers** to invite a customer to establish a reseller relationship with both you and the indirect provider at the same time.</span></span> <span data-ttu-id="f261c-223">El proveedor debe tener una relación de revendedor con el cliente, para que puedan enviar pedidos en nombre del cliente cuando el cliente desee comprar nuevas suscripciones o agregar nuevas licencias a las suscripciones existentes.</span><span class="sxs-lookup"><span data-stu-id="f261c-223">The provider needs to have a reseller relationship with your customer, so they can submit orders on your customer's behalf when the customer wants to buy new subscriptions or add new licenses to existing subscriptions.</span></span>

    :::image type="content" source="images/direct/direct6.png" alt-text="Invitar a nuevos clientes":::

3. <span data-ttu-id="f261c-225">En la página siguiente, revise el borrador del mensaje de correo electrónico.</span><span class="sxs-lookup"><span data-stu-id="f261c-225">On the next page, review the draft email message.</span></span> <span data-ttu-id="f261c-226">Puede abrir el borrador de mensajes en el correo electrónico, o puede copiar el mensaje en el portapapeles y pegarlo en un correo electrónico.</span><span class="sxs-lookup"><span data-stu-id="f261c-226">You can open the draft message in email, or you can copy the message to your clipboard and paste it into an email.</span></span>

4. <span data-ttu-id="f261c-227">Edite el texto del correo electrónico para indicar lo que necesita, pero asegúrese de incluir el vínculo, ya que está personalizado para conectar el cliente directamente a su cuenta y a la cuenta del proveedor.</span><span class="sxs-lookup"><span data-stu-id="f261c-227">Edit the text in the email to say what you need but be sure to include the link as it is personalized to connect the customer directly to both your account and your provider's account.</span></span> <span data-ttu-id="f261c-228">A continuación, seleccione **Done** (Listo).</span><span class="sxs-lookup"><span data-stu-id="f261c-228">Then select **Done** .</span></span>

5. <span data-ttu-id="f261c-229">Una vez que el cliente te autorice a ti y tu proveedor como revendedores de registro, tendrás permisos de administrador para administrar sus suscripciones, licencias y usuarios en su nombre y tu proveedor indirecto podrá enviar pedidos en su nombre.</span><span class="sxs-lookup"><span data-stu-id="f261c-229">After the customer authorizes you and your provider to be their resellers of record, you'll have administrator permissions to manage their subscriptions, licenses, and users on their behalf, and your indirect provider will be able to submit orders on their behalf.</span></span>

6. <span data-ttu-id="f261c-230">Para administrar la cuenta, los servicios, los usuarios y las licencias del cliente, expande el registro del cliente seleccionando la flecha abajo situada junto a su nombre.</span><span class="sxs-lookup"><span data-stu-id="f261c-230">To manage the customer's account, services, users, and licenses, expand the customer's record by selecting the down arrow near their name.</span></span>

### <a name="microsoft-customer-agreement-acceptance"></a><span data-ttu-id="f261c-231">Aceptación del acuerdo de cliente de Microsoft</span><span class="sxs-lookup"><span data-stu-id="f261c-231">Microsoft Customer Agreement acceptance</span></span>

<span data-ttu-id="f261c-232">Microsoft Cloud acuerdo es válido hasta el 31 de enero de 2020.</span><span class="sxs-lookup"><span data-stu-id="f261c-232">Microsoft Cloud Agreement is valid until January 31, 2020.</span></span> <span data-ttu-id="f261c-233">Después de esa fecha, todos los clientes, existentes y nuevos, deben firmar el nuevo [contrato de cliente de Microsoft](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="f261c-233">After that date, all customers, existing and new, must sign the new [Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span> <span data-ttu-id="f261c-234">En el caso de los clientes de transición, si:</span><span class="sxs-lookup"><span data-stu-id="f261c-234">For transitioning customers, if:</span></span>

- <span data-ttu-id="f261c-235">**El cliente aún no ha aceptado el contrato de cliente de Microsoft**</span><span class="sxs-lookup"><span data-stu-id="f261c-235">**Customer has not accepted Microsoft Customer Agreement yet**</span></span>

   <span data-ttu-id="f261c-236">Trabaje con un proveedor indirecto para que [el cliente acepte el contrato de atención al cliente de Microsoft](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="f261c-236">Please work with Indirect Provider to have customer [accept the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

- <span data-ttu-id="f261c-237">**El cliente ha aceptado el contrato de atención al cliente de Microsoft con usted a través del centro de administración de Microsoft 365**</span><span class="sxs-lookup"><span data-stu-id="f261c-237">**Customer has accepted Microsoft Customer Agreement with you through the Microsoft 365 Admin Center**</span></span>

   <span data-ttu-id="f261c-238">La aceptación se conservará una vez que se haya establecido la relación de revendedor con el proveedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-238">The acceptance will be retained once the reseller relationship is established with the Indirect Provider.</span></span> <span data-ttu-id="f261c-239">No es necesario hacer nada.</span><span class="sxs-lookup"><span data-stu-id="f261c-239">There is nothing you need to do.</span></span>

- <span data-ttu-id="f261c-240">**El cliente ha aceptado el contrato de cliente de Microsoft con la atestación de asociados**</span><span class="sxs-lookup"><span data-stu-id="f261c-240">**Customer has accepted Microsoft Customer Agreement with you through partner attestation**</span></span>

   <span data-ttu-id="f261c-241">No se conservará la aceptación.</span><span class="sxs-lookup"><span data-stu-id="f261c-241">The acceptance will not be retained.</span></span> <span data-ttu-id="f261c-242">Trabaje con un proveedor indirecto para [actualizar la aceptación del cliente en el centro de Partners](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span><span class="sxs-lookup"><span data-stu-id="f261c-242">Please work with Indirect Provider to [update the customer's acceptance in Partner Center](confirm-customer-agreement.md#confirm-customer-acceptance-for-existing-customers).</span></span>

## <a name="transfer-existing-direct-bill-subscriptions-to-indirect-provider"></a><span data-ttu-id="f261c-243">Transferir las suscripciones de factura directa existentes al proveedor indirecto</span><span class="sxs-lookup"><span data-stu-id="f261c-243">Transfer existing direct bill subscriptions to indirect provider</span></span>

<span data-ttu-id="f261c-244">En el modelo indirecto de CSP, los revendedores indirectos no tienen relaciones de facturación con Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f261c-244">Under CSP indirect model, indirect resellers do not have billing relationships with Microsoft.</span></span> <span data-ttu-id="f261c-245">En su lugar, los revendedores indirectos obtienen las suscripciones de sus clientes a través de sus proveedores indirectos.</span><span class="sxs-lookup"><span data-stu-id="f261c-245">Instead, indirect resellers obtain subscriptions for their customers through their indirect providers.</span></span> <span data-ttu-id="f261c-246">Mientras realiza la transición de Direct Bill Partner a revendedor indirecto, debe transferir las suscripciones existentes que tiene como el socio de facturación directo a su proveedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-246">While transitioning from direct bill partner to indirect reseller, you need to transfer the existing subscriptions you have as the direct bill partner to your indirect provider.</span></span> <span data-ttu-id="f261c-247">Para ello, puede usar la característica de transferencia de suscripción de autoservicio en el panel del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="f261c-247">You can use the self-served subscription transfer feature in Partner Center Dashboard to do so.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="f261c-248">Requisitos previos</span><span class="sxs-lookup"><span data-stu-id="f261c-248">Pre-requisites</span></span>

- <span data-ttu-id="f261c-249">Esta característica solo está disponible para los asociados de transición que hayan completado la inscripción de revendedores indirectos mediante sus inquilinos de asociados directos de factura.</span><span class="sxs-lookup"><span data-stu-id="f261c-249">This feature is only available to transitioning partners who have completed the indirect reseller enrollment using their existing direct bill partner tenants</span></span>

- <span data-ttu-id="f261c-250">Antes de transferir las suscripciones asociadas a un cliente determinado, el asociado de transición debe trasladar el cliente a un proveedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-250">Before transferring subscriptions associated with a given customer, the transitioning partner must move the customer to an indirect provider.</span></span>

- <span data-ttu-id="f261c-251">El cliente debe haber [aceptado el contrato de cliente de Microsoft a través del proveedor indirecto](#microsoft-customer-agreement-acceptance).</span><span class="sxs-lookup"><span data-stu-id="f261c-251">Customer must have [accepted Microsoft Customer Agreement through the Indirect Provider](#microsoft-customer-agreement-acceptance).</span></span>

### <a name="how-to-transition-to-indirect-reseller-status"></a><span data-ttu-id="f261c-252">Transición al estado de un revendedor indirecto</span><span class="sxs-lookup"><span data-stu-id="f261c-252">How to transition to indirect reseller status</span></span>

<span data-ttu-id="f261c-253">La característica es un proceso de 4 pasos, donde:</span><span class="sxs-lookup"><span data-stu-id="f261c-253">The feature is a 4-step process, where:</span></span>

- <span data-ttu-id="f261c-254">El asociado de transición crea una solicitud de transferencia de suscripción.</span><span class="sxs-lookup"><span data-stu-id="f261c-254">The transitioning partner creates a subscription transfer request.</span></span> <span data-ttu-id="f261c-255">La solicitud contiene una o más suscripciones existentes asociadas al mismo cliente y se dirige a un proveedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-255">The request contains one or more existing subscriptions associated with the same customer and is addressed to an indirect provider.</span></span>

- <span data-ttu-id="f261c-256">El proveedor indirecto revisa y acepta (o rechaza) la solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="f261c-256">The indirect provider reviews and accepts (or reject) the transfer request.</span></span>

- <span data-ttu-id="f261c-257">El proveedor indirecto comprueba que se ha completado la solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="f261c-257">The indirect provider verifies that the transfer request is complete.</span></span>

- <span data-ttu-id="f261c-258">El asociado de transición comprueba que se ha completado la solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="f261c-258">The transitioning partner verifies that the transfer request is complete.</span></span>

### <a name="transitioning-partner"></a><span data-ttu-id="f261c-259">Asociado de transición</span><span class="sxs-lookup"><span data-stu-id="f261c-259">Transitioning partner</span></span>

> [!NOTE]
> <span data-ttu-id="f261c-260">También puede usar el [SDK/API del centro de Partners](/partner-center/develop/manage-customers) para transferir las suscripciones existentes a su proveedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-260">You can also use [Partner Center API/SDK](/partner-center/develop/manage-customers) to transfer the existing subscriptions to your indirect provider.</span></span>
>
> - [<span data-ttu-id="f261c-261">Obtener la idoneidad de la transferencia de suscripciones de un cliente</span><span class="sxs-lookup"><span data-stu-id="f261c-261">Get a customer's subscriptions transfer eligibility</span></span>](/partner-center/develop/get-customer-s-subscriptions-transfer-eligibility)
> - [<span data-ttu-id="f261c-262">Crear una transferencia de un cliente</span><span class="sxs-lookup"><span data-stu-id="f261c-262">Create a customer's transfer</span></span>](/partner-center/develop/create-a-transfer)
> - [<span data-ttu-id="f261c-263">Retirar la transferencia de un cliente</span><span class="sxs-lookup"><span data-stu-id="f261c-263">Withdraw a customer's transfer</span></span>](/partner-center/develop/withdraw-a-transfer)
> - [<span data-ttu-id="f261c-264">Aceptar una transferencia de un cliente</span><span class="sxs-lookup"><span data-stu-id="f261c-264">Accept a customer's transfer</span></span>](/partner-center/develop/accept-a-transfer)
> - [<span data-ttu-id="f261c-265">Rechazar la transferencia de un cliente</span><span class="sxs-lookup"><span data-stu-id="f261c-265">Reject a Customer's transfer</span></span>](/partner-center/develop/reject-a-transfer)
> - [<span data-ttu-id="f261c-266">Obtener las transferencias de un cliente</span><span class="sxs-lookup"><span data-stu-id="f261c-266">Get a customer's transfers</span></span>](/partner-center/develop/get-all-of-a-customer-s-transfers)
> - [<span data-ttu-id="f261c-267">Obtener detalles de la transferencia por identificador</span><span class="sxs-lookup"><span data-stu-id="f261c-267">Get transfer details by id</span></span>](/partner-center/develop/get-transfer-by-id)

### <a name="transitioning-partner---create-transfer-request"></a><span data-ttu-id="f261c-268">Transición de asociado: crear solicitud de transferencia</span><span class="sxs-lookup"><span data-stu-id="f261c-268">Transitioning partner - create transfer request</span></span>

<span data-ttu-id="f261c-269">Para crear una solicitud de transferencia como el asociado de transición:</span><span class="sxs-lookup"><span data-stu-id="f261c-269">To create a transfer request as the transitioning partner:</span></span>

1. <span data-ttu-id="f261c-270">Inicie sesión en el centro de partners como **agente de administración** .</span><span class="sxs-lookup"><span data-stu-id="f261c-270">Log in to Partner Center as an **Admin Agent** .</span></span>

2. <span data-ttu-id="f261c-271">En la página **clientes** , seleccione el cliente deseado y haga clic en el icono vínculos rápidos para expandir la vista de resumen del cliente.</span><span class="sxs-lookup"><span data-stu-id="f261c-271">In the **Customers** page, select the intended customer and click on the Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="f261c-272">En **proveedores indirectos** , confirme que aparece el proveedor indirecto previsto.</span><span class="sxs-lookup"><span data-stu-id="f261c-272">Under **Indirect provider(s)** , confirm that the intended indirect provider is listed.</span></span>

4. <span data-ttu-id="f261c-273">Haga clic en **Ver suscripciones** .</span><span class="sxs-lookup"><span data-stu-id="f261c-273">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="f261c-274">En la página **suscripciones** , busque **transferencia de suscripción** .</span><span class="sxs-lookup"><span data-stu-id="f261c-274">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

6. <span data-ttu-id="f261c-275">En **transferencia de suscripción** , haga clic en **solicitar transferencia de suscripción** .</span><span class="sxs-lookup"><span data-stu-id="f261c-275">Under **Subscription Transfer** , click **Request subscription transfer** .</span></span>

    :::image type="content" source="images/direct/direct8.png" alt-text="Solicitud de transferencia de suscripción":::

7. <span data-ttu-id="f261c-277">En el cuadro de diálogo transferir solicitud, seleccione una o varias suscripciones que se van a transferir.</span><span class="sxs-lookup"><span data-stu-id="f261c-277">In the transfer request dialog, select one or more subscriptions to be transferred.</span></span>

    :::image type="content" source="images/direct/direct9.png" alt-text="Crear solicitud de transferencia":::

8. <span data-ttu-id="f261c-279">Haga clic en **Crear** .</span><span class="sxs-lookup"><span data-stu-id="f261c-279">Click **Create** .</span></span>

9. <span data-ttu-id="f261c-280">Aparecerá una solicitud de transferencia de suscripción activa en **transferencia de suscripción** .</span><span class="sxs-lookup"><span data-stu-id="f261c-280">An active subscription transfer request will appear under **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct10.png" alt-text="Lista de solicitudes de transferencia":::

10. <span data-ttu-id="f261c-282">Informe a su proveedor indirecto de que ha creado una solicitud de transferencia de suscripción.</span><span class="sxs-lookup"><span data-stu-id="f261c-282">Inform your indirect provider that you have created a subscription transfer request to them.</span></span>

### <a name="indirect-provider---accept-transfer-request"></a><span data-ttu-id="f261c-283">Proveedor indirecto: aceptación de la solicitud de transferencia</span><span class="sxs-lookup"><span data-stu-id="f261c-283">Indirect provider - accept transfer request</span></span>

<span data-ttu-id="f261c-284">Para revisar y aceptar una solicitud de transferencia como proveedor indirecto:</span><span class="sxs-lookup"><span data-stu-id="f261c-284">To review and accept a transfer request as the indirect provider:</span></span>

1. <span data-ttu-id="f261c-285">Inicie sesión en el centro de partners como agente de **Administración** o **agente de ventas** .</span><span class="sxs-lookup"><span data-stu-id="f261c-285">Log in to Partner Center as an **Admin** Agent or **Sales Agent** .</span></span>

2. <span data-ttu-id="f261c-286">En la página **clientes** , seleccione el cliente deseado y haga clic en el icono vínculos rápidos para expandir la vista Resumen del cliente.</span><span class="sxs-lookup"><span data-stu-id="f261c-286">In the **Customers** page, select the intended customer and click on its Quick links icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="f261c-287">En **revendedores indirectos** , confirme que aparece el socio de transición.</span><span class="sxs-lookup"><span data-stu-id="f261c-287">Under **Indirect reseller(s)** , confirm the transitioning partner is listed.</span></span>

4. <span data-ttu-id="f261c-288">Haga clic en **Ver suscripciones** .</span><span class="sxs-lookup"><span data-stu-id="f261c-288">Click **View Subscriptions** .</span></span>

5. <span data-ttu-id="f261c-289">En la página **suscripciones** , busque **transferencia de suscripción** .</span><span class="sxs-lookup"><span data-stu-id="f261c-289">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

    :::image type="content" source="images/direct/direct11.png" alt-text="Ver solicitud de transferencia":::

6. <span data-ttu-id="f261c-291">En **transferencia de suscripción** , haga clic en la solicitud de transferencia para revisarla.</span><span class="sxs-lookup"><span data-stu-id="f261c-291">Under **Subscription Transfer** , click on the transfer request to review.</span></span>

7. <span data-ttu-id="f261c-292">Haga clic en **Aceptar** (o en **rechazar** ) según corresponda.</span><span class="sxs-lookup"><span data-stu-id="f261c-292">Click **Accept** (or **Reject** ) as appropriate.</span></span>

    :::image type="content" source="images/direct/direct12.png" alt-text="Aceptar solicitud de transferencia":::

8. <span data-ttu-id="f261c-294">Espere a que se complete la solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="f261c-294">Wait for the transfer request to complete.</span></span>

### <a name="indirect-provider---verify-transfer-request-is-complete"></a><span data-ttu-id="f261c-295">Proveedor indirecto: comprobar que la solicitud de transferencia se ha completado</span><span class="sxs-lookup"><span data-stu-id="f261c-295">Indirect provider - verify transfer request is complete</span></span>

1. <span data-ttu-id="f261c-296">Una vez finalizada correctamente la solicitud de transferencia, compruebe que puede ver que las suscripciones aparecen en **suscripciones** .</span><span class="sxs-lookup"><span data-stu-id="f261c-296">After the transfer request is completed successfully, verify that you can see the subscriptions appear under **Subscriptions** .</span></span>

2. <span data-ttu-id="f261c-297">Informe al asociado de transición.</span><span class="sxs-lookup"><span data-stu-id="f261c-297">Inform the transitioning partner.</span></span>

### <a name="transitioning-partner---verify-transfer-request-is-complete"></a><span data-ttu-id="f261c-298">Asociado de transición: comprobar que la solicitud de transferencia se ha completado</span><span class="sxs-lookup"><span data-stu-id="f261c-298">Transitioning partner - verify transfer request is complete</span></span>

<span data-ttu-id="f261c-299">El asociado de transición debe hacer lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="f261c-299">The transitioning partner should do the following:</span></span>

1. <span data-ttu-id="f261c-300">Inicie sesión en el centro de partners como **agente de administración** o **agente de ventas** .</span><span class="sxs-lookup"><span data-stu-id="f261c-300">Sign into Partner Center as an **Admin Agent** or **Sales Agent** .</span></span>

2. <span data-ttu-id="f261c-301">En la página **clientes** , seleccione el cliente deseado y haga clic en el icono **vínculos rápidos** para expandir la vista de resumen del cliente.</span><span class="sxs-lookup"><span data-stu-id="f261c-301">In the **Customers** page, select the intended customer and click on the **Quick links** icon to expand the summary view of the customer.</span></span>

3. <span data-ttu-id="f261c-302">Haga clic en **Ver suscripciones** .</span><span class="sxs-lookup"><span data-stu-id="f261c-302">Click **View Subscriptions** .</span></span>

4. <span data-ttu-id="f261c-303">En la página **suscripciones** , busque **transferencia de suscripción** .</span><span class="sxs-lookup"><span data-stu-id="f261c-303">In the **Subscriptions** page, look for **Subscription Transfer** .</span></span>

5. <span data-ttu-id="f261c-304">Compruebe que la solicitud de transferencia está marcada como **completa** .</span><span class="sxs-lookup"><span data-stu-id="f261c-304">Verify that the transfer request is marked as **Complete** .</span></span>

6. <span data-ttu-id="f261c-305">Compruebe que las suscripciones ya no aparecen como activas en la página **suscripciones** :</span><span class="sxs-lookup"><span data-stu-id="f261c-305">Verify that the subscription(s) no longer appear as active in the **Subscriptions** page:</span></span>

   1. <span data-ttu-id="f261c-306">Si se trata de una suscripción de Azure (MS-AZR-0145P), ya no aparecerá en la lista.</span><span class="sxs-lookup"><span data-stu-id="f261c-306">If this is an Azure subscription (MS-AZR-0145P), it will no longer be listed.</span></span>

   2. <span data-ttu-id="f261c-307">Si se trata de una suscripción basada en licencia (Office 365, Dynamics, Intune), se mostrará con el estado **suspendido** .</span><span class="sxs-lookup"><span data-stu-id="f261c-307">If this is a license-based subscription (Office 365, Dynamics, Intune), it will be listed with state as **Suspended** .</span></span>

   :::image type="content" source="images/direct/direct13.png" alt-text="Suscripción suspendida":::

### <a name="considerations"></a><span data-ttu-id="f261c-309">Consideraciones</span><span class="sxs-lookup"><span data-stu-id="f261c-309">Considerations</span></span>

- <span data-ttu-id="f261c-310">**El identificador de suscripción será diferente después de la transferencia.**</span><span class="sxs-lookup"><span data-stu-id="f261c-310">**Subscription ID will be different after transfer.**</span></span> <span data-ttu-id="f261c-311">Si es una suscripción de Azure (MS-AZR-0145P), también tendrá un identificador de suscripción de Azure, que se conserva del propietario anterior y aparecerá en el portal de administración de Azure.</span><span class="sxs-lookup"><span data-stu-id="f261c-311">If it is an Azure subscription (MS-AZR-0145P), additionally, it will have an Azure Subscription ID, which is retained from the previous owner, and will appear in the Azure management portal.</span></span>

- <span data-ttu-id="f261c-312">**No se puede hacer referencia a la misma suscripción mediante varias solicitudes de transferencia.**</span><span class="sxs-lookup"><span data-stu-id="f261c-312">**The same subscription cannot be referenced by multiple transfer requests.**</span></span> <span data-ttu-id="f261c-313">Después de haber creado una solicitud de transferencia, que incluye una suscripción existente, no se pueden crear solicitudes de transferencia adicionales, incluida la misma suscripción, hasta que se cancele la primera solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="f261c-313">After you have created a transfer request, which includes an existing subscription, you cannot create additional transfer requests including the same subscription, until the first transfer request is canceled.</span></span>

- <span data-ttu-id="f261c-314">**Los complementos para las suscripciones basadas en licencias deben transferirse junto con su suscripción base.**</span><span class="sxs-lookup"><span data-stu-id="f261c-314">**Add-ons for license-based subscriptions must be transferred along with their base subscription.**</span></span> <span data-ttu-id="f261c-315">Al crear una solicitud de transferencia, si elige una suscripción existente con uno o varios complementos, los complementos se incluirán automáticamente en la solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="f261c-315">When creating a transfer request, if you pick an existing subscription with one or more add-ons, the add-ons will automatically be included in the transfer request.</span></span>

- <span data-ttu-id="f261c-316">**Los cambios en el número de licencias de una suscripción no se reflejarán en la solicitud de transferencia existente.**</span><span class="sxs-lookup"><span data-stu-id="f261c-316">**License count changes to a subscription will not be reflected in existing transfer request.**</span></span> <span data-ttu-id="f261c-317">Después de crear una solicitud de transferencia que incluye una suscripción existente, debe evitar actualizar la cantidad de licencias de la suscripción (o los complementos asociados).</span><span class="sxs-lookup"><span data-stu-id="f261c-317">After you have created a transfer request which includes an existing subscription, you should avoid updating the license quantity of the subscription (or associated addons).</span></span> <span data-ttu-id="f261c-318">Si lo hace, la nueva cantidad no se reflejará en la solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="f261c-318">If you do so, the new quantity will not be reflected in the transfer request.</span></span> <span data-ttu-id="f261c-319">Después de que el proveedor indirecto acepte la solicitud de transferencia, la suscripción resultante tendrá la cantidad anterior.</span><span class="sxs-lookup"><span data-stu-id="f261c-319">After the indirect provider accepts the transfer request, the resultant subscription will have the old quantity.</span></span> <span data-ttu-id="f261c-320">Si desea que la nueva cantidad se transfiera al proveedor indirecto, debe cancelar la solicitud de transferencia existente y volver a crear una nueva.</span><span class="sxs-lookup"><span data-stu-id="f261c-320">If you wish for the new quantity to be transferred to the indirect provider, you must cancel the existing transfer request and recreate a new one.</span></span>

- <span data-ttu-id="f261c-321">**No todas las compras se pueden transferir mediante la transferencia de suscripción de autoservicio.**</span><span class="sxs-lookup"><span data-stu-id="f261c-321">**Not all purchases can be transferred using self-served subscription transfer.**</span></span> <span data-ttu-id="f261c-322">Actualmente, solo se pueden transferir suscripciones de O365 y suscripciones de Azure PAYG (MS-AZR-0145P) con esta característica.</span><span class="sxs-lookup"><span data-stu-id="f261c-322">Currently, you can only transfer O365 subscriptions and Azure PAYG subscriptions (MS-AZR-0145P) using this feature.</span></span> <span data-ttu-id="f261c-323">No se admiten otras compras, como los planes de Azure, las instancias reservadas de Azure, las suscripciones basadas en términos y las suscripciones de SaaS de Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="f261c-323">Other purchases including Azure Plans, Azure Reserved Instances, Term-based Subscriptions and SaaS subscriptions for Azure Marketplace are not supported.</span></span> <span data-ttu-id="f261c-324">Verá un motivo por el que no se puede transferir una suscripción en la página enviar solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="f261c-324">You will see a reason why a subscription cannot be transferred in the submit transfer request page.</span></span> <span data-ttu-id="f261c-325">Para transferir estas suscripciones, tendrá que [cancelar la suscripción existente](create-a-new-subscription.md#suspend-or-cancel-a-subscription) y comprar una nueva oferta para el cliente a través de un proveedor indirecto.</span><span class="sxs-lookup"><span data-stu-id="f261c-325">To transfer these subscriptions, you will need to [cancel the existing subscription](create-a-new-subscription.md#suspend-or-cancel-a-subscription) and purchase new offer for customer through Indirect Provider.</span></span>

- <span data-ttu-id="f261c-326">**No se puede probar con un entorno de espacio aislado.**</span><span class="sxs-lookup"><span data-stu-id="f261c-326">**Cannot be tested using sandbox environment.**</span></span>

## <a name="enroll-for-indirect-reseller-incentives"></a><span data-ttu-id="f261c-327">Inscribirse para los incentivos de reseller indirectos</span><span class="sxs-lookup"><span data-stu-id="f261c-327">Enroll for indirect reseller incentives</span></span>

<span data-ttu-id="f261c-328">Una vez que se haya inscrito correctamente como revendedor indirecto en el inquilino de asociado directo de factura existente, recibirá una invitación para inscribirse en el incentivo de revendedores indirectos en un plazo de 30 días.</span><span class="sxs-lookup"><span data-stu-id="f261c-328">After you have successfully enrolled as an indirect reseller on your existing direct bill partner tenant, you will receive an invitation to enroll for indirect reseller incentive within 30 days.</span></span> <span data-ttu-id="f261c-329">La invitación se basa en la cuenta de asociado de MPN que está asociada actualmente con el inquilino del asociado de CSP.</span><span class="sxs-lookup"><span data-stu-id="f261c-329">The invitation is based on the partner MPN account that is currently associated with your CSP partner tenant.</span></span> <span data-ttu-id="f261c-330">La invitación se enviará a la dirección de correo electrónico asociada a la cuenta de socio de MPN.</span><span class="sxs-lookup"><span data-stu-id="f261c-330">The invitation will be sent to the email address associated with the partner MPN account.</span></span>

<span data-ttu-id="f261c-331">También puede inscribirse para programas de incentivos directos de facturación con el mismo inquilino de asociados.</span><span class="sxs-lookup"><span data-stu-id="f261c-331">You are also eligible to enroll for direct bill incentive programs with that same partner tenant.</span></span> <span data-ttu-id="f261c-332">Debe administrar los programas por separado.</span><span class="sxs-lookup"><span data-stu-id="f261c-332">You must manage the programs separately.</span></span>

## <a name="next-steps"></a><span data-ttu-id="f261c-333">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="f261c-333">Next steps</span></span>

- [<span data-ttu-id="f261c-334">Información adicional sobre cómo convertirse en revendedor indirecto</span><span class="sxs-lookup"><span data-stu-id="f261c-334">Additional information on becoming an indirect reseller</span></span>](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)
- [<span data-ttu-id="f261c-335">Nuevos requisitos de asociados directos del CSP</span><span class="sxs-lookup"><span data-stu-id="f261c-335">CSP direct partner new requirements</span></span>](direct-partner-new-requirements.md)
- [<span data-ttu-id="f261c-336">Funcionalidades de facturación directa restringidas</span><span class="sxs-lookup"><span data-stu-id="f261c-336">Restricted direct bill capabilities</span></span>](restricted-direct-bill-capabilities.md)