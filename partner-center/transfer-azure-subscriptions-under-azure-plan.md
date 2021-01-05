---
title: Transferencia de una suscripción de Azure a un plan de Azure a otro asociado de CSP
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo cambiar el asociado del programa proveedor de soluciones en la nube asociado a las suscripciones de Azure de un cliente en un plan de Azure.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: e792e4af2999924ba8be77ec0517ce56c1db7a27
ms.sourcegitcommit: ed5c873d19f0464cc986fe6e852383cd4280daf6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/05/2021
ms.locfileid: "97893213"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a><span data-ttu-id="cfc4a-103">Transfiera las suscripciones del plan de Azure de un cliente a un asociado diferente</span><span class="sxs-lookup"><span data-stu-id="cfc4a-103">Transfer a customer's Azure plan subscriptions to a different partner</span></span>

<span data-ttu-id="cfc4a-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="cfc4a-104">**Appropriate roles**</span></span>

- <span data-ttu-id="cfc4a-105">Partners del programa Proveedor de soluciones en la nube (CSP)</span><span class="sxs-lookup"><span data-stu-id="cfc4a-105">Partners in the Cloud Solution Provider (CSP) program</span></span>

<span data-ttu-id="cfc4a-106">En este artículo se describe cómo un cliente puede cambiar sus suscripciones de Azure en un plan de Azure de un proveedor de soluciones en la nube (CSP) a otro.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-106">This article describes how a customer can switch their Azure subscriptions under an Azure plan from one Cloud Solution Provider (CSP) to another.</span></span>

<span data-ttu-id="cfc4a-107">Para cambiar las suscripciones de Azure de un cliente de un asociado diferente, siga estos pasos.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-107">To switch a customer's Azure subscriptions from a different partner, follow these steps.</span></span> <span data-ttu-id="cfc4a-108">Tanto el socio como el cliente tienen que completar los pasos.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-108">Both the partner and the customer have steps to complete.</span></span>

>[!Note]  
><span data-ttu-id="cfc4a-109">Solo los asociados con una relación de facturación directa con Microsoft pueden acceder a las herramientas de transición.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-109">Only partners with a direct billing relationship with Microsoft can access the transition tooling.</span></span> <span data-ttu-id="cfc4a-110">Los revendedores indirectos deben trabajar con sus proveedores indirectos para aprovechar esta herramienta de transición.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-110">Indirect Resellers must work with their Indirect Providers to leverage this transition tool.</span></span>

<span data-ttu-id="cfc4a-111">El cliente debe estar en conversación con ambos asociados (actuales y futuros) antes de que se aproveche esta herramienta.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-111">The customer must be in conversation with both partners (current and future) prior to this tool being leveraged.</span></span> <span data-ttu-id="cfc4a-112">Es necesario tener una conversación sin conexión para evitar la confusión y la renovación.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-112">An offline conversation needs to be had to avoid confusion and churn.</span></span> <span data-ttu-id="cfc4a-113">Además, los asociados y los clientes deben comprender estas consideraciones y requisitos previos antes de iniciar una transición:</span><span class="sxs-lookup"><span data-stu-id="cfc4a-113">In addition, partners and customers should understand these considerations and prerequisites prior to initiating a transition:</span></span>

<span data-ttu-id="cfc4a-114">**Consideraciones clave:**</span><span class="sxs-lookup"><span data-stu-id="cfc4a-114">**Key considerations:**</span></span>

- <span data-ttu-id="cfc4a-115">Azure Reservations no se moverá con la suscripción a un socio comercial futuro</span><span class="sxs-lookup"><span data-stu-id="cfc4a-115">Azure Reservations will not move with the subscription to future partner</span></span>
- <span data-ttu-id="cfc4a-116">Los precios de CSP para los servicios de Azure en el socio actual no se transfieren</span><span class="sxs-lookup"><span data-stu-id="cfc4a-116">CSP pricing for Azure services under current partner will not transition</span></span>  
- <span data-ttu-id="cfc4a-117">Las responsabilidades de soporte técnico del cliente se trasladarán al asociado futuro</span><span class="sxs-lookup"><span data-stu-id="cfc4a-117">Support responsibilities for customer will move to future partner</span></span>
- <span data-ttu-id="cfc4a-118">La facturación y la facturación se trasladarán al asociado futuro en el momento de la transferencia</span><span class="sxs-lookup"><span data-stu-id="cfc4a-118">Billing and invoicing will move to future partner at time of transfer</span></span>
- <span data-ttu-id="cfc4a-119">El Access Control de Role-Based de Azure (RBAC) no se ve afectado por la transferencia</span><span class="sxs-lookup"><span data-stu-id="cfc4a-119">Azure Role-Based Access Control (RBAC) is not affected by the transfer</span></span>
- <span data-ttu-id="cfc4a-120">El administrador en nombre de (AOBO) no se concederá de forma predeterminada al socio comercial futuro</span><span class="sxs-lookup"><span data-stu-id="cfc4a-120">Admin on Behalf Of (AOBO) will not be granted by default to the future partner</span></span>
- <span data-ttu-id="cfc4a-121">Los productos de Marketplace de terceros se transferirán siempre que los productos superen la comprobación de elegibilidad del Marketplace.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-121">Third-party marketplace products will transfer as long as the products pass the Marketplace eligibility check.</span></span>
    - <span data-ttu-id="cfc4a-122">No hay descuentos especiales ni restricciones regionales</span><span class="sxs-lookup"><span data-stu-id="cfc4a-122">There are no special discounts or regional restrictions</span></span>
    - <span data-ttu-id="cfc4a-123">Los productos no están basados en la suscripción</span><span class="sxs-lookup"><span data-stu-id="cfc4a-123">The products are non-subscription based</span></span>
    - <span data-ttu-id="cfc4a-124">El asociado futuro debe trabajar con el publicador para asegurarse de que se encuentran en la lista de permitidos para la implementación del producto.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-124">The future partner should work with the publisher to make sure they are on the allow-list for deployment of the product</span></span>
    - <span data-ttu-id="cfc4a-125">Si no se cumplen todas estas condiciones para transferir los productos de Marketplace, se deben cancelar las suscripciones de Azure y, después, volver a comprar los productos de Marketplace con el nuevo socio comercial.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-125">If not all of these conditions are met in order to transfer the Marketplace products should be canceled, the Azure subscriptions transferred, and then repurchase of Marketplace products with the new partner</span></span>

<span data-ttu-id="cfc4a-126">**Requisitos previos:**</span><span class="sxs-lookup"><span data-stu-id="cfc4a-126">**Prerequisites:**</span></span>

- <span data-ttu-id="cfc4a-127">El cliente contrata al asociado de CSP actual en su intención de transición</span><span class="sxs-lookup"><span data-stu-id="cfc4a-127">Customer engages current CSP partner on their intent to transition</span></span>
- <span data-ttu-id="cfc4a-128">El asociado de CSP futuro funciona con el cliente para garantizar que se puedan satisfacer las necesidades del cliente</span><span class="sxs-lookup"><span data-stu-id="cfc4a-128">Future CSP partner works with customer to ensure customer needs can be met</span></span>
- <span data-ttu-id="cfc4a-129">El asociado de CSP futuro establece una relación con el cliente y compra un plan de Azure antes de comenzar la transición</span><span class="sxs-lookup"><span data-stu-id="cfc4a-129">Future CSP partner establishes a relationship with customer and purchases an Azure plan before the transition begins</span></span>  
- <span data-ttu-id="cfc4a-130">El cliente debe firmar el acuerdo de cliente de Microsoft con el asociado de CSP futuro</span><span class="sxs-lookup"><span data-stu-id="cfc4a-130">Customer must sign Microsoft Customer Agreement with future CSP partner</span></span>
- <span data-ttu-id="cfc4a-131">El asociado de CSP futuro debe haber firmado el acuerdo de asociado de Microsoft para usar esta herramienta</span><span class="sxs-lookup"><span data-stu-id="cfc4a-131">Future CSP partner must have signed the Microsoft Partner Agreement to use this tool</span></span>

## <a name="customer-tasks-to-be-completed"></a><span data-ttu-id="cfc4a-132">Tareas del cliente que se van a completar</span><span class="sxs-lookup"><span data-stu-id="cfc4a-132">Customer tasks to be completed</span></span>

<span data-ttu-id="cfc4a-133">Para transferir una suscripción de Azure en un plan de Azure, el cliente debe iniciar el proceso poniéndose en contacto con su asociado actual.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-133">To transfer an Azure subscription under an Azure plan, the customer must start the process by contacting their current partner.</span></span> <span data-ttu-id="cfc4a-134">Deben recopilar el dominio y el nombre de la empresa de su socio actual para que su asociado futuro pueda completar el formulario de solicitud de transferencia en su nombre.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-134">They should collect their current partner's company name and domain so their future partner can complete the transfer request form on their behalf.</span></span>

<span data-ttu-id="cfc4a-135">El cliente también debe identificar las suscripciones que desean transferir desde su socio actual.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-135">The customer must also identify the subscriptions they wish to transfer from their current partner.</span></span> <span data-ttu-id="cfc4a-136">No se pueden cambiar los asociados de las suscripciones a Office 365, Enterprise Mobility Suite o Microsoft Dynamics CRM.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-136">You can't change partners for Office 365, Enterprise Mobility Suite, or Microsoft Dynamics CRM subscriptions.</span></span>

>[!Note]  
><span data-ttu-id="cfc4a-137">Es responsabilidad del asociado futuro completar el formulario de solicitud de transferencia que inicia el proceso de transferencia.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-137">It is the future partner's responsibility to complete the transfer request form that initiates the transfer process.</span></span> <span data-ttu-id="cfc4a-138">Microsoft no puede intervenir en nombre del cliente o del socio actual.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-138">Microsoft cannot intervene on behalf of the customer or the current partner.</span></span> <span data-ttu-id="cfc4a-139">El cliente debe planear trabajar en estrecha colaboración con sus asociados futuros y actuales para que la transición se lleve a cabo sin problemas.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-139">The customer should plan to work closely with their future and current partner to make the transition go smoothly.</span></span>

## <a name="future-partner-tasks-to-be-completed"></a><span data-ttu-id="cfc4a-140">Futuras tareas de asociados que se van a completar</span><span class="sxs-lookup"><span data-stu-id="cfc4a-140">Future partner tasks to be completed</span></span>

<span data-ttu-id="cfc4a-141">El socio comercial de la suscripción debe completar un formulario de solicitud de transferencia desde el centro de partners para solicitar una transferencia de suscripción:</span><span class="sxs-lookup"><span data-stu-id="cfc4a-141">The future partner of the subscription needs to complete a transfer request form from Partner Center to request a subscription transfer:</span></span>

1.  <span data-ttu-id="cfc4a-142">En el menú del centro de Partners, seleccione **clientes** y, a continuación, seleccione el cliente en nombre del que desea completar un formulario de solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-142">From the Partner Center menu, select **Customers**, then select the customer you wish to complete a transfer request form on behalf of.</span></span>
2.  <span data-ttu-id="cfc4a-143">En el menú del cliente, seleccione **suscripciones**.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-143">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="cfc4a-144">Seleccione la sección **solicitud de transferencia** .</span><span class="sxs-lookup"><span data-stu-id="cfc4a-144">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="cfc4a-145">En la **sección solicitud de transferencia**, seleccione **Agregar nueva solicitud**.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-145">From the **Transfer request section**, select **Add new request**.</span></span>

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sección transferencias":::

5.  <span data-ttu-id="cfc4a-147">Complete el formulario **nueva solicitud de transferencia** .</span><span class="sxs-lookup"><span data-stu-id="cfc4a-147">Complete the **New transfer request** form.</span></span>

6.  <span data-ttu-id="cfc4a-148">Seleccione **Enviar solicitud de transferencia** de  >  **envío**.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-148">Select **Send transfer request** > **Send**.</span></span>

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Formulario completar solicitud de transferencia":::

7.  <span data-ttu-id="cfc4a-150">Revisar confirmación de solicitud de transferencia</span><span class="sxs-lookup"><span data-stu-id="cfc4a-150">Review Transfer request confirmation</span></span>

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Revisión de la transferencia pendiente":::

    >[!Note]
    ><span data-ttu-id="cfc4a-152">El asociado futuro puede cancelar la solicitud de transferencia seleccionando **Cancelar solicitud** en la esquina superior derecha solo cuando el estado de la solicitud de transferencia es "pendiente".</span><span class="sxs-lookup"><span data-stu-id="cfc4a-152">The future partner can cancel the transfer request by selecting **cancel request** in the upper right-hand corner only when the transfer request status is “pending”.</span></span> <span data-ttu-id="cfc4a-153">Una vez que el estado de la solicitud de transferencia es "en curso" o "completo", no se podrán realizar las cancelaciones.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-153">Once the transfer request status is “in progress” or “complete”, cancellations will not be possible.</span></span>

## <a name="current-partner-tasks-to-be-completed"></a><span data-ttu-id="cfc4a-154">Tareas de asociados actuales para completar</span><span class="sxs-lookup"><span data-stu-id="cfc4a-154">Current partner tasks to be completed</span></span>

<span data-ttu-id="cfc4a-155">El agente de administración del asociado actual del cliente recibirá un correo electrónico que solicitará a su cliente una transferencia de sus suscripciones:</span><span class="sxs-lookup"><span data-stu-id="cfc4a-155">The current partner's Admin Agent of the customer will receive an email that their customer is requesting a transfer of their subscriptions:</span></span>

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Revisar":::

<span data-ttu-id="cfc4a-157">Revise y acepte el formulario de solicitud de transferencia del centro de partners para completar la transferencia de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-157">Review and accept the transfer request form from Partner Center to complete the subscription transfer.</span></span>

>[!Note]  
><span data-ttu-id="cfc4a-158">Si el asociado actual no realiza ninguna acción en un plazo de 30 días, la solicitud expirará y el asociado futuro tendrá un para crear una nueva solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-158">If no action is taken by the current partner within 30 days the request will expire and the future partner will have a to create a new transfer request.</span></span>

1.  <span data-ttu-id="cfc4a-159">Seleccione **revisar solicitud de transferencia** desde el correo electrónico o</span><span class="sxs-lookup"><span data-stu-id="cfc4a-159">Select **Review transfer Request** from the email OR</span></span>
1.  <span data-ttu-id="cfc4a-160">En el menú del centro de Partners, seleccione **clientes** y, a continuación, seleccione el cliente al que se ha enviado una solicitud de transferencia en nombre de.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-160">From the Partner Center menu, select **Customers**, then select the customer that a transfer request has been submitted on behalf of.</span></span>
2.  <span data-ttu-id="cfc4a-161">En el menú del cliente, seleccione **suscripciones**.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-161">From the Customer menu, select **Subscriptions**.</span></span>
3.  <span data-ttu-id="cfc4a-162">Seleccione la sección **solicitud de transferencia** .</span><span class="sxs-lookup"><span data-stu-id="cfc4a-162">Select the **Transfer request** section.</span></span>
4.  <span data-ttu-id="cfc4a-163">Expanda transferir información seleccionando el **identificador de solicitud de transferencia** elegido en **solicitudes recibidas** .</span><span class="sxs-lookup"><span data-stu-id="cfc4a-163">Expand transfer information by selecting the chosen **Transfer request ID** under **Received requests**</span></span>

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Solicitud de transferencia de revisiones de origen":::

5.  <span data-ttu-id="cfc4a-165">Revise la solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-165">Review transfer request.</span></span> <span data-ttu-id="cfc4a-166">Seleccione las suscripciones de Azure solicitadas que se van a transferir.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-166">Select the requested Azure subscriptions to transfer.</span></span>

>[!Note]  
> <span data-ttu-id="cfc4a-167">Antes de continuar, tenga en cuenta que ya no tendrá acceso a las suscripciones seleccionadas.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-167">Before proceeding please note: You will no longer have access to the selected subscriptions.</span></span>
> <span data-ttu-id="cfc4a-168">No se le facturará para su uso adicional.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-168">You will not be invoiced for further usage.</span></span>
> <span data-ttu-id="cfc4a-169">Las reservas de Azure no se transfieren con las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-169">Azure reservations do not transfer with the subscriptions.</span></span>

6.  <span data-ttu-id="cfc4a-170">A continuación, seleccione **Aceptar y transferir** para completar el proceso de transferencia.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-170">Then select **Accept and transfer** to complete the transfer process.</span></span>

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Seleccione las suscripciones que se van a transferir en sus planes de Azure":::

7.  <span data-ttu-id="cfc4a-172">Permite ver la confirmación de aceptación de transferencia.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-172">View transfer acceptance confirmation.</span></span>

   <span data-ttu-id="cfc4a-173">En este momento, el socio comercial, el cliente y el socio actual recibirán una notificación de la solicitud de transferencia aceptada por correo electrónico.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-173">At this point, the future partner, the customer, and current partner will be notified of the accepted transfer request via email.</span></span>

   <span data-ttu-id="cfc4a-174">Después de, se ha aceptado la transición el estado de la transferencia podría permanecer pendiente hasta 15 minutos mientras se actualiza el sistema.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-174">After, the transition has been accepted the transfer status might remain Pending for up to 15 minutes while the system is updated.</span></span> <span data-ttu-id="cfc4a-175">Si tarda más, el sistema seguirá intentando tres días.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-175">If it takes longer, the system will keep trying for three days.</span></span> <span data-ttu-id="cfc4a-176">Si el estado de la transferencia sigue siendo pendiente, el asociado debe enviar una solicitud de servicio.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-176">If the transfer status still remains Pending, the partner should submit a service request.</span></span>

   <span data-ttu-id="cfc4a-177">Una vez completada la transferencia, las suscripciones incluidas en la solicitud aparecerán en el plan de Azure del asociado futuro y ya no aparecerán en la lista.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-177">Once the transfer is complete, the subscriptions included within the request will appear in the Azure plan of the future partner, and no longer be listed with you.</span></span>

>[!Note]  
><span data-ttu-id="cfc4a-178">Para los proveedores indirectos: informe a su revendedor indirecto de que se ha aceptado la solicitud de transferencia.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-178">For Indirect Providers: Please inform your Indirect Reseller that the transfer request has been accepted.</span></span>

### <a name="managing-your-transferred-customer-subscriptions"></a><span data-ttu-id="cfc4a-179">Administración de las suscripciones de clientes transferidas</span><span class="sxs-lookup"><span data-stu-id="cfc4a-179">Managing your transferred customer subscriptions</span></span>
- <span data-ttu-id="cfc4a-180">El acceso a los usuarios, grupos o entidades de servicio existentes que se asignaron mediante el control de acceso basado en rol de Azure (RBAC) no se ve afectado durante la transición.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-180">Access to existing users, groups, or service principals that were assigned using Azure role-based access control (RBAC) isn't affected during the transition.</span></span> <span data-ttu-id="cfc4a-181">El control de acceso basado en roles [(RBAC de Azure)](/azure/role-based-access-control/overview) de Azure ayuda a su cliente a administrar quién tiene acceso a los recursos de Azure, lo que puede hacer con esos recursos y a qué áreas tienen acceso.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-181">Azure role-based access control [(Azure RBAC)](/azure/role-based-access-control/overview) helps your customer manage who has access to Azure resources, what they can do with those resources, and what areas they have access to.</span></span> <span data-ttu-id="cfc4a-182">Como el nuevo asociado, no se le concede ningún acceso RBAC a los recursos de su cliente después de la transferencia de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-182">As the new partner you aren't given any RBAC access to your customer’s resources after the subscription transfer.</span></span> <span data-ttu-id="cfc4a-183">El socio anterior del cliente conserva su acceso RBAC.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-183">Your customer’s previous partner retains their RBAC access.</span></span> <span data-ttu-id="cfc4a-184">Trabaje con su cliente para conocer quién tiene conocimiento de sus suscripciones y cómo realizar los cambios deseados.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-184">Work with your customer to understand who has insight into their subscriptions and how to make any wanted changes.</span></span>

- <span data-ttu-id="cfc4a-185">Por lo tanto, es importante que el cliente Quite el acceso RBAC de Azure para su asociado anterior y agregue acceso para el nuevo socio.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-185">Consequently, it’s important that your customer removes Azure RBAC access for their previous partner and add access for the new partner.</span></span> <span data-ttu-id="cfc4a-186">Para más información sobre el cliente que otorga nuevo acceso, consulte [¿Qué es el control de acceso basado en roles de Azure (RBAC de Azure)?](/azure/role-based-access-control/overview)</span><span class="sxs-lookup"><span data-stu-id="cfc4a-186">For more information about your customer giving new access, see [What is Azure role-based access control (Azure RBAC)?](/azure/role-based-access-control/overview)</span></span> <span data-ttu-id="cfc4a-187">Para obtener más información sobre el cliente que quita el acceso RBAC del asociado anterior, consulte [quitar una asignación de roles](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span><span class="sxs-lookup"><span data-stu-id="cfc4a-187">For more information about your customer removing your previous partner’s RBAC access, see [Remove a role assignment](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment).</span></span>

- <span data-ttu-id="cfc4a-188">Además, no obtiene automáticamente acceso [de administrador en nombre de (Aobo)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) a las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-188">Additionally, you don’t automatically get [Admin on Behalf Of (AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) access to your subscriptions.</span></span> <span data-ttu-id="cfc4a-189">AOBO es necesario para que los asociados administren las suscripciones de Azure de su cliente en su nombre.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-189">AOBO is necessary for partner’s to manage their customer’s Azure subscriptions on their behalf.</span></span> <span data-ttu-id="cfc4a-190">Para obtener más información sobre los privilegios de Azure, consulte [obtención de permisos para administrar el servicio o la suscripción de un cliente.](./customers-revoke-admin-privileges.md)</span><span class="sxs-lookup"><span data-stu-id="cfc4a-190">For more information about Azure privileges, see [Obtain permissions to manage a customer’s service or subscription.](./customers-revoke-admin-privileges.md)</span></span>

## <a name="next-steps"></a><span data-ttu-id="cfc4a-191">Pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="cfc4a-191">Next steps:</span></span>

- [<span data-ttu-id="cfc4a-192">(RBAC de Azure)</span><span class="sxs-lookup"><span data-stu-id="cfc4a-192">(Azure RBAC)</span></span>](/azure/role-based-access-control/overview)
- [<span data-ttu-id="cfc4a-193">Obtener permisos para administrar el servicio o la suscripción de un cliente.</span><span class="sxs-lookup"><span data-stu-id="cfc4a-193">Obtain permissions to manage a customer’s service or subscription.</span></span>](./customers-revoke-admin-privileges.md)
