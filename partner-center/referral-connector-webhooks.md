---
title: Uso de webhooks para obtener eventos de cambio de recursos
ms.topic: article
ms.date: 05/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Uso de las API de webhook para averiguar cuándo se producen cambios en los recursos de las referencias
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: referencias, API de webhook, eventos de cambio de recursos
ms.localizationpriority: medium
ms.openlocfilehash: a141776f1b591ebe41bb740051802b4b55cf36f0
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/22/2020
ms.locfileid: "83796211"
---
# <a name="use-webhook-apis-to-register-for-resource-change-events"></a><span data-ttu-id="292ea-104">Uso de las API de webhook para registrar eventos de cambio de recursos</span><span class="sxs-lookup"><span data-stu-id="292ea-104">Use Webhook APIs to register for resource change events</span></span>

### <a name="appropriate-roles"></a><span data-ttu-id="292ea-105">Roles adecuados</span><span class="sxs-lookup"><span data-stu-id="292ea-105">Appropriate roles</span></span>

- <span data-ttu-id="292ea-106">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="292ea-106">Referrals admin</span></span>
- <span data-ttu-id="292ea-107">Administrador del sistema o Personalizador del sistema para Dynamics 365 CRM o CRM de Salesforce</span><span class="sxs-lookup"><span data-stu-id="292ea-107">System admin or System customizer for Dynamics 365 CRM or Salesforce CRM</span></span>


<span data-ttu-id="292ea-108">Las API del webhook del centro de Partners le permiten registrarse para los eventos de cambio de recursos.</span><span class="sxs-lookup"><span data-stu-id="292ea-108">The Partner Center Webhook APIs allow you to register for resource change events.</span></span> <span data-ttu-id="292ea-109">Estos eventos de cambio se envían a la dirección URL como publicaciones HTTP.</span><span class="sxs-lookup"><span data-stu-id="292ea-109">These change events are sent to your url as HTTP posts.</span></span>

>[!NOTE]
><span data-ttu-id="292ea-110">En este tema se explican las API de webhook para Dynamics 365 CRM y el CRM de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="292ea-110">This topic explains Webhook APIs for both Dynamics 365 CRM and Salesforce CRM.</span></span>

1. <span data-ttu-id="292ea-111">Para registrar la dirección URL, seleccione **registro de webhook del centro de Partners (versión preliminar de Insider)** flujo de automatización.</span><span class="sxs-lookup"><span data-stu-id="292ea-111">To register your url, select **Partner Center Webhook Registration (Insider Preview)** Power Automate flow.</span></span>

2. <span data-ttu-id="292ea-112">Agregar conexiones para () Usuario del centro de Partners con credenciales de administrador de referencias (b.) Eventos del centro de Partners, tal y como se resalta</span><span class="sxs-lookup"><span data-stu-id="292ea-112">Add connections for (a.) Partner Center user with referrals admin credentials (b.) Partner Center Events as highlighted below</span></span>

![Desencadenador](images/cosellconnectors/triggerflow.png)

3. <span data-ttu-id="292ea-114">Cuando realice estas actualizaciones, verá</span><span class="sxs-lookup"><span data-stu-id="292ea-114">When you make these updates, you will see</span></span>

![webhooks](images/cosellconnectors/webhook1.png)

4. <span data-ttu-id="292ea-116">Guarde los cambios y seleccione **Activar**.</span><span class="sxs-lookup"><span data-stu-id="292ea-116">Save your changes and select **Turn on**.</span></span> 

<span data-ttu-id="292ea-117">Para permitir que los webhooks del centro de Partners escuchen los cambios de eventos en los objetos de coexistencia o de referencia independiente IP en el centro de Partners y en los sistemas CRM, realice los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="292ea-117">To enable Partner Center webhooks to listen to event changes in the IP Co-sell/independent referral objects in Partner Center and CRM systems perform the following steps:</span></span>

5. <span data-ttu-id="292ea-118">Seleccione **centro de partners para Dynamics 365 (versión preliminar de Insider)** o **centro de partners a Salesforce (versión preliminar de Insider)**.</span><span class="sxs-lookup"><span data-stu-id="292ea-118">Select **Partner Center to Dynamics 365 (Insider Preview)** or **Partner Center to Salesforce (Insider Preview)**.</span></span>

6. <span data-ttu-id="292ea-119">Seleccione el icono de **edición** y seleccione **cuando se reciba una solicitud HTTP**.</span><span class="sxs-lookup"><span data-stu-id="292ea-119">Select the **Edit** icon and select **When a HTTP request is received**.</span></span>

7. <span data-ttu-id="292ea-120">Seleccione el icono de **copiar** para copiar la dirección URL http post proporcionada.</span><span class="sxs-lookup"><span data-stu-id="292ea-120">Select the **Copy** icon to copy the provided HTTP POST URL.</span></span>

![Copiar la dirección URL](images/cosellconnectors/copyurl.png)

8. <span data-ttu-id="292ea-122">Ahora, seleccione "registro de webhook del centro de Partners (versión preliminar de Insider)" flujo automático de energía y seleccione **Ejecutar**.</span><span class="sxs-lookup"><span data-stu-id="292ea-122">Now select the “Partner Center Webhook Registration (Insider Preview)” Power Automate flow and select **Run**.</span></span>

9. <span data-ttu-id="292ea-123">Asegúrese de que se abre la ventana "flujo de ejecución" en el panel derecho y haga clic en **continuar**.</span><span class="sxs-lookup"><span data-stu-id="292ea-123">Ensure that the “Run Flow” window opens on the right-hand pane and click **Continue**.</span></span>

10. <span data-ttu-id="292ea-124">Escriba la siguiente información:</span><span class="sxs-lookup"><span data-stu-id="292ea-124">Enter the following details:</span></span> 

    <span data-ttu-id="292ea-125">a.</span><span class="sxs-lookup"><span data-stu-id="292ea-125">a.</span></span> <span data-ttu-id="292ea-126">**Punto de conexión de desencadenador http**: dirección URL copiada del paso anterior</span><span class="sxs-lookup"><span data-stu-id="292ea-126">**Http Trigger Endpoint**: URL copied from earlier step</span></span>

    <span data-ttu-id="292ea-127">b.</span><span class="sxs-lookup"><span data-stu-id="292ea-127">b.</span></span> <span data-ttu-id="292ea-128">**Eventos para registrar**: "referencia creada" y "referencia-actualizada"</span><span class="sxs-lookup"><span data-stu-id="292ea-128">**Events to Register**: “referral-created” and “referral-updated”</span></span>

    <span data-ttu-id="292ea-129">c.</span><span class="sxs-lookup"><span data-stu-id="292ea-129">c.</span></span> <span data-ttu-id="292ea-130">**Sobrescribir puntos de conexión de desencadenador existentes si están presentes**: sí (esto Sobrescribe todos los extremos existentes).</span><span class="sxs-lookup"><span data-stu-id="292ea-130">**Overwrite existing trigger endpoints if present**: Yes (This overwrites any existing endpoints.)</span></span>

<span data-ttu-id="292ea-131">El webhook ahora puede escuchar cambios (crear y actualizar eventos).</span><span class="sxs-lookup"><span data-stu-id="292ea-131">The webhook can now listen to changes (create and update events).</span></span> 

11. <span data-ttu-id="292ea-132">Seleccione **Ejecutar** y, a continuación, haga clic en **listo.**</span><span class="sxs-lookup"><span data-stu-id="292ea-132">Select **Run** and then select **Done.**</span></span>

 ## <a name="customize-synchronization-steps"></a><span data-ttu-id="292ea-133">Personalizar pasos de sincronización</span><span class="sxs-lookup"><span data-stu-id="292ea-133">Customize synchronization steps</span></span>

<span data-ttu-id="292ea-134">Cuando se sincronizan las referencias de venta conjunta entre el centro de Partners y el sistema CRM, los campos que se sincronizan en el equipo del centro de Partners se enumeran aquí.</span><span class="sxs-lookup"><span data-stu-id="292ea-134">When Co-sell referrals are synced between Partner Center and your CRM system, the fields that are synced on Partner Center PC are listed here.</span></span>

<span data-ttu-id="292ea-135">A menudo, los sistemas CRM son muy personalizados.</span><span class="sxs-lookup"><span data-stu-id="292ea-135">Often CRM systems are highly customized.</span></span> <span data-ttu-id="292ea-136">Puede personalizar los flujos de automatización.</span><span class="sxs-lookup"><span data-stu-id="292ea-136">You can customize the Power Automate flows.</span></span> <span data-ttu-id="292ea-137">Siga la guía de asignación de campos y, si es necesario, realice los cambios adecuados en los pasos de la potencia que automatiza los flujos.</span><span class="sxs-lookup"><span data-stu-id="292ea-137">Follow the field mapping guide, and if necessary, make appropriate changes in the steps of the Power Automate flows.</span></span>  <span data-ttu-id="292ea-138">Se proporcionan asignaciones del centro de Partners de Microsoft a CRM, pero en función de su entorno de CRM, puede optar por personalizar aún más los campos.</span><span class="sxs-lookup"><span data-stu-id="292ea-138">Microsoft Partner Center to CRM mappings are provided, but based on your CRM environment, you can choose to further customize the fields.</span></span>

<span data-ttu-id="292ea-139">Se pueden personalizar varios pasos de cada uno de los flujos de potencia automatizados en función de sus necesidades.</span><span class="sxs-lookup"><span data-stu-id="292ea-139">Multiple steps of each of the Power Automate flows can be customized based on your needs.</span></span> <span data-ttu-id="292ea-140">Estos son algunos ejemplos de las personalizaciones disponibles:</span><span class="sxs-lookup"><span data-stu-id="292ea-140">The following are examples of available customizations:</span></span>

1. <span data-ttu-id="292ea-141">Para personalizar los campos de los eventos de creación o actualización en el centro de partners para la sincronización de referencias de CRM:</span><span class="sxs-lookup"><span data-stu-id="292ea-141">To customize the fields for the create or update events in the Partner Center to CRM referral synchronization:</span></span> 

    <span data-ttu-id="292ea-142">a.</span><span class="sxs-lookup"><span data-stu-id="292ea-142">a.</span></span> <span data-ttu-id="292ea-143">Seleccione centro de partners para Dynamics 365 (versión preliminar de Insider) o centro de partners a Salesforce (versión preliminar de Insider).</span><span class="sxs-lookup"><span data-stu-id="292ea-143">Select Partner Center to Dynamics 365 (Insider Preview) or Partner Center to Salesforce (Insider Preview).</span></span>

    <span data-ttu-id="292ea-144">b.</span><span class="sxs-lookup"><span data-stu-id="292ea-144">b.</span></span> <span data-ttu-id="292ea-145">Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="292ea-145">Select **Edit** to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="292ea-146">c.</span><span class="sxs-lookup"><span data-stu-id="292ea-146">c.</span></span> <span data-ttu-id="292ea-147">Seleccione **(ámbito) sincronizar el cliente potencial o la oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="292ea-147">Select **(Scope) Synchronize the lead or opportunity**.</span></span>

2. <span data-ttu-id="292ea-148">Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para crear eventos, seleccione si se trata de una **nueva oportunidad compartida y, a continuación**, haga clic en.</span><span class="sxs-lookup"><span data-stu-id="292ea-148">To customize CRM field mappings (based on field mappings guide) for create events, select **If it’s new Shared opportunity, then**.</span></span> <span data-ttu-id="292ea-149">Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda **crear una nueva oportunidad en CRM**.</span><span class="sxs-lookup"><span data-stu-id="292ea-149">Select the substep **if yes** and then expand **Creating a new opportunity in the CRM**.</span></span> <span data-ttu-id="292ea-150">Puede editar las asignaciones en esta sección mediante la guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="292ea-150">You can edit the mappings in this section using the Field Mapping Guide.</span></span>

    <span data-ttu-id="292ea-151">d.</span><span class="sxs-lookup"><span data-stu-id="292ea-151">d.</span></span> <span data-ttu-id="292ea-152">Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para los eventos de actualización, haga clic en el paso "(ámbito) sincronizar el cliente potencial o la oportunidad".</span><span class="sxs-lookup"><span data-stu-id="292ea-152">For customizing CRM field mappings (based on field mappings guide) for update events, click on the step “(Scope) Synchronize the lead or opportunity”.</span></span>

    <span data-ttu-id="292ea-153">e.</span><span class="sxs-lookup"><span data-stu-id="292ea-153">e.</span></span> <span data-ttu-id="292ea-154">Seleccione **si se trata de una actualización de una oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="292ea-154">Select **If it’s an update to an opportunity, then**.</span></span> <span data-ttu-id="292ea-155">Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda **si la diferencia entre los objetos de oportunidad del centro de Partners y CRM**.</span><span class="sxs-lookup"><span data-stu-id="292ea-155">Select the substep **if yes** and then expand **If difference between the opportunity objects in Partner Center and CRM, then**.</span></span>  

    <span data-ttu-id="292ea-156">f.</span><span class="sxs-lookup"><span data-stu-id="292ea-156">f.</span></span> <span data-ttu-id="292ea-157">Seleccione **si sí** seguido de **Actualizar oportunidad existente** .</span><span class="sxs-lookup"><span data-stu-id="292ea-157">Select **If yes** followed with **Update existing opportunity**</span></span>
       
3. <span data-ttu-id="292ea-158">Para personalizar los campos de la sincronización de referencia de CRM a equipo para eventos de actualización:</span><span class="sxs-lookup"><span data-stu-id="292ea-158">To customize the fields for CRM to PC referral synchronization for update events:</span></span>

    <span data-ttu-id="292ea-159">a.</span><span class="sxs-lookup"><span data-stu-id="292ea-159">a.</span></span> <span data-ttu-id="292ea-160">Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="292ea-160">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

    <span data-ttu-id="292ea-161">b.</span><span class="sxs-lookup"><span data-stu-id="292ea-161">b.</span></span> <span data-ttu-id="292ea-162">Seleccione **(ámbito) sincronizar la oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="292ea-162">Select **(Scope) Synchronize the opportunity**.</span></span>

    <span data-ttu-id="292ea-163">c.</span><span class="sxs-lookup"><span data-stu-id="292ea-163">c.</span></span> <span data-ttu-id="292ea-164">Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para eventos de actualización, seleccione **si hay diferencias entre los objetos de cliente potencial del centro de Partners y CRM y, a continuación, haga clic en**.</span><span class="sxs-lookup"><span data-stu-id="292ea-164">For customizing CRM field mappings (based on field mappings guide) for update events, select **If there is difference between the lead objects in Partner Center and CRM, then**.</span></span> 

    <span data-ttu-id="292ea-165">d.</span><span class="sxs-lookup"><span data-stu-id="292ea-165">d.</span></span> <span data-ttu-id="292ea-166">Seleccione el subpaso en **caso afirmativo** y, a continuación, expanda el paso **actualizar una referencia con los datos de oportunidad**.</span><span class="sxs-lookup"><span data-stu-id="292ea-166">Select the substep **if yes** and then expand the step **Update a referral with opportunity data**.</span></span>

<span data-ttu-id="292ea-167">Puede editar las asignaciones en esta sección basándose en la guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="292ea-167">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

4. <span data-ttu-id="292ea-168">Para personalizar los campos de la sincronización de referencia de CRM a equipo para crear eventos</span><span class="sxs-lookup"><span data-stu-id="292ea-168">To customize the fields for CRM to PC referral synchronization for create events?</span></span>

   <span data-ttu-id="292ea-169">a.</span><span class="sxs-lookup"><span data-stu-id="292ea-169">a.</span></span> <span data-ttu-id="292ea-170">Seleccione **Editar** para editar o personalizar el flujo de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="292ea-170">Select **Edit**  to edit/customize the Power Automate flow.</span></span>

   <span data-ttu-id="292ea-171">b.</span><span class="sxs-lookup"><span data-stu-id="292ea-171">b.</span></span> <span data-ttu-id="292ea-172">Seleccione **(ámbito) sincronizar referencias.**</span><span class="sxs-lookup"><span data-stu-id="292ea-172">Select **(Scope) Synchronizing Referrals.**</span></span>

   <span data-ttu-id="292ea-173">c.</span><span class="sxs-lookup"><span data-stu-id="292ea-173">c.</span></span> <span data-ttu-id="292ea-174">Para personalizar las asignaciones de campos de CRM (según la guía de asignaciones de campos) para crear eventos, seleccione **crear referencia de Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="292ea-174">For customizing CRM field mappings (based on field mappings guide) for create events, select **Create Microsoft Referral**.</span></span> 

<span data-ttu-id="292ea-175">Puede editar las asignaciones en esta sección basándose en la guía de asignación de campos.</span><span class="sxs-lookup"><span data-stu-id="292ea-175">You can edit the mappings in this section based on the Field Mapping Guide.</span></span>

## <a name="end-to-end-bi-directional-co-sell-referral-synchronization"></a><span data-ttu-id="292ea-176">Sincronización de referencia de venta conjunta bidireccional de un extremo a otro</span><span class="sxs-lookup"><span data-stu-id="292ea-176">End-to-End Bi-directional Co-sell Referral Synchronization</span></span>

<span data-ttu-id="292ea-177">Una vez que haya instalado, configurado y personalizado la solución Power Automate, puede probar la sincronización de referencias de venta conjunta entre Dynamics 365 o Salesforce y Partner Center.</span><span class="sxs-lookup"><span data-stu-id="292ea-177">Once you have installed, configured, and customized the Power Automate solution, you can test for Co-sell referrals synchronization between Dynamics 365 or Salesforce and Partner Center.</span></span>

### <a name="pre-requisites"></a><span data-ttu-id="292ea-178">Requisitos previos</span><span class="sxs-lookup"><span data-stu-id="292ea-178">Pre-requisites</span></span>

<span data-ttu-id="292ea-179">Para sincronizar las referencias entre el centro de Partners y Dynamics 365 CRM o entre el centro de Partners y el CRM de Salesforce, la solución Power Automate debe delimitar claramente los campos de referencia específicos de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="292ea-179">To synchronize the referrals across Partner Center and Dynamics 365 CRM or across Partner Center and Salesforce CRM, the Power Automate solution needs to clearly demarcate Microsoft-specific referral fields.</span></span> <span data-ttu-id="292ea-180">Esto proporciona a los equipos de los vendedores la capacidad de decidir qué referencias desean compartir con Microsoft para la venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="292ea-180">This provides your seller teams with the ability to decide which referrals they want to share with Microsoft for co-selling.</span></span>

<span data-ttu-id="292ea-181">Un conjunto de campos personalizados está disponible como parte de la sincronización de referencias del centro de partners para la entidad de la **oportunidad** de la solución Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="292ea-181">A set of custom fields is available as part of Partner Center Referrals Synchronization for Dynamics 365 solution **Opportunity** entity.</span></span> <span data-ttu-id="292ea-182">Un usuario administrador de CRM tendrá que crear una sección de CRM independiente con los campos personalizados de la **oportunidad** .</span><span class="sxs-lookup"><span data-stu-id="292ea-182">A CRM admin user will need to create a separate CRM section with the **Opportunity** custom fields.</span></span>

<span data-ttu-id="292ea-183">Los siguientes campos personalizados deben formar parte de la sección CRM:</span><span class="sxs-lookup"><span data-stu-id="292ea-183">The following custom fields should be part of the CRM section:</span></span>

- <span data-ttu-id="292ea-184">**Sincronizar con el centro de Partners**: si se va a sincronizar la oportunidad con el centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="292ea-184">**Sync with Partner Center**: Whether to sync the opportunity with Microsoft Partner Center</span></span>

- <span data-ttu-id="292ea-185">**Identificador de referencia**: un campo de identificador de solo lectura para la referencia del centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="292ea-185">**Referral Identifier**: A read-only identifier field for Microsoft Partner Center referral</span></span>

- <span data-ttu-id="292ea-186">**Vínculo de referencia**: un vínculo de solo lectura a la referencia en el centro de Partners de Microsoft</span><span class="sxs-lookup"><span data-stu-id="292ea-186">**Referral Link**: A read-only link to the referral in Microsoft Partner Center</span></span>

- <span data-ttu-id="292ea-187">**¿Cómo puede ayudarle Microsoft?**: ayuda necesaria de Microsoft para la referencia</span><span class="sxs-lookup"><span data-stu-id="292ea-187">**How can Microsoft help?**: Help required from Microsoft for the referral</span></span>

- <span data-ttu-id="292ea-188">**Productos**: lista de productos asociados a esta oportunidad</span><span class="sxs-lookup"><span data-stu-id="292ea-188">**Products**: List of products associated with this opportunity</span></span>

- <span data-ttu-id="292ea-189">**Audit**: una pista de auditoría de solo lectura para la sincronización con las referencias del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="292ea-189">**Audit**: A read-only audit trail for syncing with Partner Center referrals</span></span>

### <a name="scenarios"></a><span data-ttu-id="292ea-190">SITUACIÓN</span><span class="sxs-lookup"><span data-stu-id="292ea-190">SCENARIOS:</span></span>

1. <span data-ttu-id="292ea-191">Sincronización de referencia cuando se crea o actualiza una referencia en CRM y se sincroniza en el centro de Partners:</span><span class="sxs-lookup"><span data-stu-id="292ea-191">Referral synchronization when referral is created or updated in CRM and synced in Partner Center:</span></span>

    <span data-ttu-id="292ea-192">a.</span><span class="sxs-lookup"><span data-stu-id="292ea-192">a.</span></span> <span data-ttu-id="292ea-193">Inicie sesión en el entorno de CRM de Dynamics 365 o en el entorno de Salesforce CRM con un usuario que tenga visibilidad en la sección de **oportunidades** de CRM.</span><span class="sxs-lookup"><span data-stu-id="292ea-193">Sign into your Dynamics 365 CRM environment or Salesforce CRM environment with user who has visibility in the **Opportunity** section of the CRM.</span></span>

    <span data-ttu-id="292ea-194">b.</span><span class="sxs-lookup"><span data-stu-id="292ea-194">b.</span></span> <span data-ttu-id="292ea-195">Asegúrese de que la siguiente sección está presente al crear una "nueva oportunidad" en el entorno de Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="292ea-195">Ensure that the following section is present when you create a “New Opportunity” in Dynamics 365 environment</span></span>

   ![Oportunidad](images/cosellconnectors/opportunity.png)

    <span data-ttu-id="292ea-197">c.</span><span class="sxs-lookup"><span data-stu-id="292ea-197">c.</span></span> <span data-ttu-id="292ea-198">Para sincronizar esta oportunidad con el centro de Partners de Microsoft, asegúrese de establecer los siguientes campos en la vista tarjeta:</span><span class="sxs-lookup"><span data-stu-id="292ea-198">To synchronize this opportunity with Microsoft Partner Center, ensure that you set the following fields in the card view:</span></span>

    - <span data-ttu-id="292ea-199">"Sincronizar con el centro de Partners": sí</span><span class="sxs-lookup"><span data-stu-id="292ea-199">“Sync with Partner Center”: Yes</span></span>

    - <span data-ttu-id="292ea-200">"¿Cómo puede ayuda de Microsoft?": Seleccione una de las siguientes opciones:</span><span class="sxs-lookup"><span data-stu-id="292ea-200">"How can Microsoft help?”: Select from the following:</span></span>

    ![Selecciones de la ayuda](images/cosellconnectors/help.png)

    - <span data-ttu-id="292ea-202">Productos: identificadores de la solución del producto</span><span class="sxs-lookup"><span data-stu-id="292ea-202">Products: Solution IDs of the product</span></span>

    <span data-ttu-id="292ea-203">d.</span><span class="sxs-lookup"><span data-stu-id="292ea-203">d.</span></span> <span data-ttu-id="292ea-204">Una vez creada la oportunidad en Dynamics 365 con la opción **sincronizar con el centro de Partners** establecida en **sí**, espere 10 minutos, inicie sesión en su cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="292ea-204">Once the opportunity is created in Dynamics 365 with **Sync with Partner Center** option set to **Yes**, wait 10 minutes, sign into your Partner Center account.</span></span> <span data-ttu-id="292ea-205">Las referencias se sincronizarán con Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="292ea-205">Your referrals will be synchronized with Dynamics 365.</span></span>

    <span data-ttu-id="292ea-206">e.</span><span class="sxs-lookup"><span data-stu-id="292ea-206">e.</span></span> <span data-ttu-id="292ea-207">Por lo tanto, para una oportunidad que tuviera la opción "sincronizar con el centro de Partners" establecida en "sí", si actualizas la oportunidad en Dynamics 365 CRM, los cambios se sincronizarán en la cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="292ea-207">Consequently, for an opportunity that had “Sync with Partner Center” option set to “Yes”, if you update the opportunity in Dynamics 365 CRM, the changes will be synchronized in your Partner Center account.</span></span>

    <span data-ttu-id="292ea-208">f.</span><span class="sxs-lookup"><span data-stu-id="292ea-208">f.</span></span> <span data-ttu-id="292ea-209">Las oportunidades que se sincronizan correctamente con el centro de Partners se identificarán con ✔ icono en Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="292ea-209">Opportunities that are synchronized successfully with Partner Center will be identified with ✔icon in Dynamics 365.</span></span>

2. <span data-ttu-id="292ea-210">Sincronización de referencia cuando se crea o actualiza una referencia en el centro de Partners de Microsoft y se sincroniza en el entorno de Dynamics 365:</span><span class="sxs-lookup"><span data-stu-id="292ea-210">Referral Synchronization when referral is created or updated in Microsoft Partner Center and synchronized in Dynamics 365 environment:</span></span> 

    <span data-ttu-id="292ea-211">a.</span><span class="sxs-lookup"><span data-stu-id="292ea-211">a.</span></span> <span data-ttu-id="292ea-212">Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard/home)del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="292ea-212">Sign into your Partner Center [dashboard](https://partner.microsoft.com/dashboard/home).</span></span>

    <span data-ttu-id="292ea-213">b.</span><span class="sxs-lookup"><span data-stu-id="292ea-213">b.</span></span> <span data-ttu-id="292ea-214">Seleccione **referencias** en el menú de la izquierda.</span><span class="sxs-lookup"><span data-stu-id="292ea-214">Select **Referrals** from the left-hand menu.</span></span>

    <span data-ttu-id="292ea-215">c.</span><span class="sxs-lookup"><span data-stu-id="292ea-215">c.</span></span> <span data-ttu-id="292ea-216">Cree una nueva referencia de venta conjunta desde el centro de partners; para ello, haga clic en la opción "nuevo trato".</span><span class="sxs-lookup"><span data-stu-id="292ea-216">Create a new Co-sell referral from Partner Center by clicking “New deal” option.</span></span>

    <span data-ttu-id="292ea-217">d.</span><span class="sxs-lookup"><span data-stu-id="292ea-217">d.</span></span> <span data-ttu-id="292ea-218">Inicie sesión en el entorno de CRM de Dynamics 365.</span><span class="sxs-lookup"><span data-stu-id="292ea-218">Sign into your Dynamics 365 CRM environment.</span></span> 

    <span data-ttu-id="292ea-219">e.</span><span class="sxs-lookup"><span data-stu-id="292ea-219">e.</span></span> <span data-ttu-id="292ea-220">Vaya a **abrir oportunidades**.</span><span class="sxs-lookup"><span data-stu-id="292ea-220">Navigate to **Open Opportunities**.</span></span> <span data-ttu-id="292ea-221">La referencia creada en el centro de Partners de Microsoft ya está sincronizada en Dynamics 365 CRM.</span><span class="sxs-lookup"><span data-stu-id="292ea-221">The referral created in Microsoft Partner Center is now synchronized in Dynamics 365 CRM.</span></span>

    <span data-ttu-id="292ea-222">f.</span><span class="sxs-lookup"><span data-stu-id="292ea-222">f.</span></span> <span data-ttu-id="292ea-223">Al seleccionar una referencia sincronizada, se rellenan los detalles de la vista de tarjeta.</span><span class="sxs-lookup"><span data-stu-id="292ea-223">When you select a synchronized referral, the card view details are populated.</span></span>

 ### <a name="next-steps"></a><span data-ttu-id="292ea-224">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="292ea-224">Next steps</span></span>

- [<span data-ttu-id="292ea-225">¿Más información sobre la plataforma Microsoft Power Automate?</span><span class="sxs-lookup"><span data-stu-id="292ea-225">More about Microsoft Power Automate platform?</span></span>](https://docs.microsoft.com/power-automate/)

- [<span data-ttu-id="292ea-226">Eventos del webhook del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="292ea-226">Partner Center webhook events</span></span>](https://docs.microsoft.com/partner-center/develop/partner-center-webhook-events)

- [<span data-ttu-id="292ea-227">Administrar los clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="292ea-227">Manage leads</span></span>](manage-leads.md)

- [<span data-ttu-id="292ea-228">Administrar las oportunidades de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="292ea-228">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
