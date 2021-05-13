---
title: Transferencia de una suscripción de Azure en un plan de Azure a otro asociado de CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprenda a cambiar el asociado de Proveedor de soluciones en la nube asociado a las suscripciones de Azure de un cliente en un plan de Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: dcacc6da51fe40c7eb05997f5409ef5fadbcf693
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856056"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="1f847-103">Transferencia de las suscripciones del plan de Azure de un cliente a otro partner</span><span class="sxs-lookup"><span data-stu-id="1f847-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="1f847-104">**Roles adecuados:** administrador de | Agente de ventas | Agente de facturación</span><span class="sxs-lookup"><span data-stu-id="1f847-104">**Appropriate roles**: Account admin | Sales agent | Billing agent</span></span>

<span data-ttu-id="1f847-105">En este artículo se describe cómo un cliente puede cambiar sus suscripciones de Azure en un plan de Azure de un Proveedor de soluciones en la nube (CSP) a otro.</span><span class="sxs-lookup"><span data-stu-id="1f847-105">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="1f847-106">Para cambiar las suscripciones de Azure de un cliente de otro asociado, siga estos pasos.</span><span class="sxs-lookup"><span data-stu-id="1f847-106">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="1f847-107">Tanto el asociado como el cliente tienen pasos que completar.</span><span class="sxs-lookup"><span data-stu-id="1f847-107">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="1f847-108">Solo los asociados con una relación de facturación directa con Microsoft pueden acceder a las herramientas de transición.</span><span class="sxs-lookup"><span data-stu-id="1f847-108">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="1f847-109">Los revendedores indirectos deben trabajar con sus proveedores indirectos para aprovechar esta herramienta de transición.</span><span class="sxs-lookup"><span data-stu-id="1f847-109">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="1f847-110">El cliente debe estar en conversación con ambos asociados (actual y futuro) antes de aprovechar esta herramienta.</span><span class="sxs-lookup"><span data-stu-id="1f847-110">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="1f847-111">Es necesario tener una conversación sin conexión para evitar confusiones y abandonos.</span><span class="sxs-lookup"><span data-stu-id="1f847-111">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="1f847-112">Además, los partners y clientes deben comprender estas consideraciones y requisitos previos antes de iniciar una transición:</span><span class="sxs-lookup"><span data-stu-id="1f847-112">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="1f847-113">**Consideraciones clave:**</span><span class="sxs-lookup"><span data-stu-id="1f847-113">**Key considerations:**</span></span>

- <span data-ttu-id="1f847-114">Azure Reservations no se moverá con la suscripción al asociado futuro</span><span class="sxs-lookup"><span data-stu-id="1f847-114">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="1f847-115">Los precios de CSP para los servicios de Azure en el asociado actual no realizarán la transición</span><span class="sxs-lookup"><span data-stu-id="1f847-115">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="1f847-116">Las responsabilidades de soporte técnico del cliente se trasladarán al asociado futuro</span><span class="sxs-lookup"><span data-stu-id="1f847-116">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="1f847-117">La facturación y la facturación se moverán al asociado futuro en el momento de la transferencia</span><span class="sxs-lookup"><span data-stu-id="1f847-117">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="1f847-118">Azure Role-Based Access Control (RBAC) no se ve afectado por la transferencia</span><span class="sxs-lookup"><span data-stu-id="1f847-118">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="1f847-119">El administrador en nombre de (AOBO) no se concederá de forma predeterminada al asociado futuro</span><span class="sxs-lookup"><span data-stu-id="1f847-119">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="1f847-120">Los productos de Marketplace de terceros se transferirán siempre y cuando los productos pasen la comprobación de idoneidad de Marketplace.</span><span class="sxs-lookup"><span data-stu-id="1f847-120">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="1f847-121">No hay descuentos especiales ni restricciones regionales</span><span class="sxs-lookup"><span data-stu-id="1f847-121">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="1f847-122">Los productos no están basados en suscripciones</span><span class="sxs-lookup"><span data-stu-id="1f847-122">The products are non-subscription based</span></span>
    - <span data-ttu-id="1f847-123">El asociado futuro debe trabajar con el publicador para asegurarse de que están en la lista de permitidos para la implementación del producto.</span><span class="sxs-lookup"><span data-stu-id="1f847-123">The future partner should work with the publisher to make sure they are on the allow list for deployment of the product</span></span>
    - <span data-ttu-id="1f847-124">Si no se cumplen todas estas condiciones para transferir los productos de Marketplace, se deben cancelar las suscripciones de Azure y, a continuación, volver a comprar productos de Marketplace con el nuevo asociado.</span><span class="sxs-lookup"><span data-stu-id="1f847-124">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="1f847-125">**Requisitos previos:**</span><span class="sxs-lookup"><span data-stu-id="1f847-125">**Prerequisites:**</span></span>

- <span data-ttu-id="1f847-126">El cliente interactúa con el asociado de CSP actual en su intención de realizar la transición.</span><span class="sxs-lookup"><span data-stu-id="1f847-126">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="1f847-127">El futuro asociado de CSP trabaja con el cliente para asegurarse de que se pueden satisfacer las necesidades del cliente.</span><span class="sxs-lookup"><span data-stu-id="1f847-127">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="1f847-128">El futuro asociado de CSP establece una relación con el cliente y adquiere un plan de Azure antes de que comience la transición.</span><span class="sxs-lookup"><span data-stu-id="1f847-128">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="1f847-129">El cliente debe firmar Contrato de cliente de Microsoft asociado de CSP futuro</span><span class="sxs-lookup"><span data-stu-id="1f847-129">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="1f847-130">El futuro asociado de CSP debe haber firmado el Contrato de asociado de Microsoft para usar esta herramienta.</span><span class="sxs-lookup"><span data-stu-id="1f847-130">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="1f847-131">Tareas del cliente que se deben completar</span><span class="sxs-lookup"><span data-stu-id="1f847-131">Customer tasks to be completed</span></span>

<span data-ttu-id="1f847-132">Para transferir una suscripción de Azure en un plan de Azure, el cliente debe iniciar el proceso ponerse en contacto con su asociado actual.</span><span class="sxs-lookup"><span data-stu-id="1f847-132">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="1f847-133">Deben recopilar el nombre de la compañía y el dominio de su asociado actual para que su asociado futuro pueda completar el formulario de solicitud de transferencia en su nombre.</span><span class="sxs-lookup"><span data-stu-id="1f847-133">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="1f847-134">El cliente también debe identificar las suscripciones que desea transferir desde su asociado actual.</span><span class="sxs-lookup"><span data-stu-id="1f847-134">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="1f847-135">No se pueden cambiar los asociados para las suscripciones de Office 365, Enterprise Mobility Suite o Microsoft Dynamics CRM.</span><span class="sxs-lookup"><span data-stu-id="1f847-135">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="1f847-136">Es responsabilidad del asociado futuro completar el formulario de solicitud de transferencia que inicia el proceso de transferencia.</span><span class="sxs-lookup"><span data-stu-id="1f847-136">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="1f847-137">Microsoft no puede intervención en nombre del cliente o del asociado actual.</span><span class="sxs-lookup"><span data-stu-id="1f847-137">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="1f847-138">El cliente debe planear trabajar estrechamente con su asociado futuro y actual para que la transición se realice sin problemas.</span><span class="sxs-lookup"><span data-stu-id="1f847-138">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="1f847-139">Tareas futuras de asociados que se completarán</span><span class="sxs-lookup"><span data-stu-id="1f847-139">Future partner tasks to be completed</span></span>

<span data-ttu-id="1f847-140">El asociado futuro de la suscripción debe completar un formulario de solicitud de transferencia Centro de partners solicitar una transferencia de suscripción:</span><span class="sxs-lookup"><span data-stu-id="1f847-140">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="1f847-141">En el Centro de partners, seleccione **Clientes** y, a continuación, seleccione el cliente del que desea completar un formulario de solicitud de transferencia en nombre de .</span><span class="sxs-lookup"><span data-stu-id="1f847-141">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="1f847-142">En el menú Cliente, seleccione **Suscripciones.**</span><span class="sxs-lookup"><span data-stu-id="1f847-142">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="1f847-143">Seleccione la **sección Solicitud de** transferencia.</span><span class="sxs-lookup"><span data-stu-id="1f847-143">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="1f847-144">En la **sección Solicitud de transferencia,** seleccione **Agregar nueva solicitud.**</span><span class="sxs-lookup"><span data-stu-id="1f847-144">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sección Transferencias":::

5.  <span data-ttu-id="1f847-146">Complete el **formulario Nueva solicitud de** transferencia.</span><span class="sxs-lookup"><span data-stu-id="1f847-146">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="1f847-147">Seleccione **Send transfer request** Send (Enviar solicitud de  >  **transferencia).**</span><span class="sxs-lookup"><span data-stu-id="1f847-147">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formulario de solicitud de transferencia completo":::

7.  <span data-ttu-id="1f847-149">Revisión de la confirmación de la solicitud de transferencia</span><span class="sxs-lookup"><span data-stu-id="1f847-149">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Revisión de la transferencia pendiente":::

    >[!Note]
    ><span data-ttu-id="1f847-151">El asociado futuro puede cancelar la solicitud de transferencia seleccionando **Cancelar** solicitud en la esquina superior derecha solo cuando el estado de la solicitud de transferencia sea "pendiente".</span><span class="sxs-lookup"><span data-stu-id="1f847-151">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="1f847-152">Una vez que el estado de la solicitud de transferencia está "en curso" o "completo", las cancelaciones no serán posibles.</span><span class="sxs-lookup"><span data-stu-id="1f847-152">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="1f847-153">Tareas actuales de asociados que se deben completar</span><span class="sxs-lookup"><span data-stu-id="1f847-153">Current partner tasks to be completed</span></span>

<span data-ttu-id="1f847-154">El agente de administración del cliente del asociado actual recibirá un correo electrónico en el que el cliente solicita una transferencia de sus suscripciones:</span><span class="sxs-lookup"><span data-stu-id="1f847-154">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Revisar":::

<span data-ttu-id="1f847-156">Revise y acepte el formulario de solicitud de transferencia Centro de partners para completar la transferencia de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="1f847-156">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="1f847-157">Si el asociado actual no hace ninguna acción en un plazo de 30 días, la solicitud expirará y el asociado futuro tendrá una para crear una nueva solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="1f847-157">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="1f847-158">Seleccione **Revisar solicitud de transferencia** desde el correo electrónico O</span><span class="sxs-lookup"><span data-stu-id="1f847-158">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="1f847-159">En el Centro de partners, seleccione **Clientes** y, a continuación, seleccione el cliente del que se ha enviado una solicitud de transferencia en nombre de .</span><span class="sxs-lookup"><span data-stu-id="1f847-159">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="1f847-160">En el menú Cliente, seleccione **Suscripciones.**</span><span class="sxs-lookup"><span data-stu-id="1f847-160">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="1f847-161">Seleccione la **sección Solicitud de** transferencia.</span><span class="sxs-lookup"><span data-stu-id="1f847-161">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="1f847-162">Expanda la información de transferencia seleccionando el identificador de **solicitud de transferencia elegido** en Solicitudes **recibidas.**</span><span class="sxs-lookup"><span data-stu-id="1f847-162">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Solicitud de transferencia de revisiones de origen":::

5.  <span data-ttu-id="1f847-164">Revise la solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="1f847-164">Review transfer request.</span></span> <span data-ttu-id="1f847-165">Seleccione las suscripciones de Azure solicitadas para transferir.</span><span class="sxs-lookup"><span data-stu-id="1f847-165">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="1f847-166">Antes de continuar, tenga en cuenta que ya no tendrá acceso a las suscripciones seleccionadas.</span><span class="sxs-lookup"><span data-stu-id="1f847-166">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="1f847-167">No se le facturará por uso adicional.</span><span class="sxs-lookup"><span data-stu-id="1f847-167">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="1f847-168">Las reservas de Azure no se transfieren con las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="1f847-168">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="1f847-169">A **continuación, seleccione Aceptar y transferir** para completar el proceso de transferencia.</span><span class="sxs-lookup"><span data-stu-id="1f847-169">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Selección de las suscripciones que se transferirán en los planes de Azure":::

7.  <span data-ttu-id="1f847-171">Ver confirmación de aceptación de transferencia.</span><span class="sxs-lookup"><span data-stu-id="1f847-171">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="1f847-172">En este momento, el asociado futuro, el cliente y el asociado actual recibirán una notificación de la solicitud de transferencia aceptada por correo electrónico.</span><span class="sxs-lookup"><span data-stu-id="1f847-172">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="1f847-173">Después de que se haya aceptado la transición, el estado de transferencia podría permanecer pendiente durante un máximo de 15 minutos mientras se actualiza el sistema.</span><span class="sxs-lookup"><span data-stu-id="1f847-173">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="1f847-174">Si tarda más, el sistema seguirá intentando durante tres días.</span><span class="sxs-lookup"><span data-stu-id="1f847-174">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="1f847-175">Si el estado de transferencia sigue siendo Pendiente, el asociado debe enviar una solicitud de servicio.</span><span class="sxs-lookup"><span data-stu-id="1f847-175">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="1f847-176">Una vez completada la transferencia, las suscripciones incluidas en la solicitud aparecerán en el plan de Azure del asociado futuro y ya no se mostrarán con usted.</span><span class="sxs-lookup"><span data-stu-id="1f847-176">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="1f847-177">Para proveedores indirectos: informe a su revendedor indirecto de que se ha aceptado la solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="1f847-177">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="1f847-178">Administración de las suscripciones de cliente transferidas</span><span class="sxs-lookup"><span data-stu-id="1f847-178">Managing your transferred customer subscriptions</span></span>

- <span data-ttu-id="1f847-179">El acceso a los usuarios, grupos o entidades de servicio existentes que se asignaron mediante el control de acceso basado en rol de Azure (RBAC) no se ve afectado durante la transición.</span><span class="sxs-lookup"><span data-stu-id="1f847-179">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="1f847-180">El control de acceso basado en rol [de Azure (RBAC](/azure/role-based-access-control/overview) de Azure) ayuda al cliente a administrar quién tiene acceso a los recursos de Azure, qué puede hacer con esos recursos y a qué áreas tiene acceso.</span><span class="sxs-lookup"><span data-stu-id="1f847-180">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="1f847-181">Como nuevo asociado, no se le proporciona acceso RBAC a los recursos del cliente después de la transferencia de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="1f847-181">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="1f847-182">El asociado anterior del cliente conserva su acceso RBAC.</span><span class="sxs-lookup"><span data-stu-id="1f847-182">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="1f847-183">Trabaje con el cliente para comprender quién tiene información sobre sus suscripciones y cómo realizar los cambios deseados.</span><span class="sxs-lookup"><span data-stu-id="1f847-183">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="1f847-184">Por lo tanto, es importante que el cliente quite el acceso RBAC de Azure para su asociado anterior y agregue acceso al nuevo asociado.</span><span class="sxs-lookup"><span data-stu-id="1f847-184">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="1f847-185">Para más información sobre el cliente que proporciona nuevo acceso, consulte ¿Qué es el control de acceso basado en [rol de Azure (RBAC de Azure)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="1f847-185">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="1f847-186">Para obtener más información sobre cómo el cliente quita el acceso RBAC del asociado anterior, consulte [Eliminación de una asignación de roles.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)</span><span class="sxs-lookup"><span data-stu-id="1f847-186">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="1f847-187">Además, no obtiene automáticamente acceso de administrador en nombre [de (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) a las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="1f847-187">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="1f847-188">AOBO es necesario para que los asociados administren las suscripciones de Azure de sus clientes en su nombre.</span><span class="sxs-lookup"><span data-stu-id="1f847-188">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="1f847-189">Para más información sobre los privilegios de Azure, consulte [Obtención de permisos para administrar el servicio o](./customers-revoke-admin-privileges.md) la suscripción de un cliente.</span><span class="sxs-lookup"><span data-stu-id="1f847-189">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="1f847-190">Pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="1f847-190">Next steps:</span></span>

- [<span data-ttu-id="1f847-191">(RBAC de Azure)</span><span class="sxs-lookup"><span data-stu-id="1f847-191">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="1f847-192">Obtenga permisos para administrar el servicio o la suscripción de un cliente.</span><span class="sxs-lookup"><span data-stu-id="1f847-192">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
