---
title: Solución de problemas de conectores de referencias de venta conjunta
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga respuestas a preguntas comunes sobre el uso de conectores de venta co-sell. Lea estas preguntas más frecuentes sobre cómo solucionar problemas de los conectores de venta co-sell.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: bb7a227624c548a29046b80d3bd5fa363a4aee2f
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276943"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="7f62e-104">Solución de problemas de conectores de referencias de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="7f62e-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="7f62e-105">**Se aplica a**: Dynamics 365 CRM | Salesforce CRM</span><span class="sxs-lookup"><span data-stu-id="7f62e-105">**Applies to**: Dynamics 365 CRM | Salesforce CRM</span></span>

<span data-ttu-id="7f62e-106">**Roles adecuados:** Administrador de referencias | Administrador del sistema o personalizador del sistema en CRM</span><span class="sxs-lookup"><span data-stu-id="7f62e-106">**Appropriate roles**: Referrals admin | System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="7f62e-107">Preguntas y respuestas sobre los requisitos previos</span><span class="sxs-lookup"><span data-stu-id="7f62e-107">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="7f62e-108">¿Puede usar una solución de conectores de referencias de venta co-venta de prueba para su entorno?</span><span class="sxs-lookup"><span data-stu-id="7f62e-108">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="7f62e-109">Si se encuentra en el entorno de prueba o ensayo, puede optar por la solución de prueba.</span><span class="sxs-lookup"><span data-stu-id="7f62e-109">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="7f62e-110">La versión de pago de los conectores está disponible en AppSource a 15 USD/mes.</span><span class="sxs-lookup"><span data-stu-id="7f62e-110">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="7f62e-111">Con la conexión de pago, recibirá 10 000 llamadas API al día.</span><span class="sxs-lookup"><span data-stu-id="7f62e-111">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="7f62e-112">Los conectores son contenedores sobre Centro de partners API de referencia.</span><span class="sxs-lookup"><span data-stu-id="7f62e-112">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="7f62e-113">Cada vez que las soluciones de conector se ejecutan para un evento Create **o** **Update** en las oportunidades de Centro de partners o CRM, se realiza una llamada API.</span><span class="sxs-lookup"><span data-stu-id="7f62e-113">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="7f62e-114">¿Qué rol necesita para crear secciones en el entorno de CRM?</span><span class="sxs-lookup"><span data-stu-id="7f62e-114">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="7f62e-115">Los usuarios que son administradores del sistema o personalizadores del sistema pueden aplicar cambios para todos los usuarios.</span><span class="sxs-lookup"><span data-stu-id="7f62e-115">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="7f62e-116">Sin embargo, todos los usuarios de la aplicación pueden personalizar el sistema e incluso compartir algunas de sus personalizaciones con otros usuarios.</span><span class="sxs-lookup"><span data-stu-id="7f62e-116">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="7f62e-117">¿Necesitan los vendedores asociados roles especiales para trabajar en Centro de partners?</span><span class="sxs-lookup"><span data-stu-id="7f62e-117">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="7f62e-118">A los vendedores asociados se les debe asignar el rol "Administrador de referencias".</span><span class="sxs-lookup"><span data-stu-id="7f62e-118">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="7f62e-119">Para obtener más información, vea [Información general sobre permisos.](create-user-accounts-and-set-permissions.md)</span><span class="sxs-lookup"><span data-stu-id="7f62e-119">For more information, see [Permissions overview](create-user-accounts-and-set-permissions.md).</span></span>

4. <span data-ttu-id="7f62e-120">¿Qué campos se deben configurar primero en el entorno de CRM?</span><span class="sxs-lookup"><span data-stu-id="7f62e-120">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="7f62e-121">• Asegúrese de que la moneda es adecuada para su ubicación y que se encuentra en su entorno crm con precisión.</span><span class="sxs-lookup"><span data-stu-id="7f62e-121">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="7f62e-122">• El equipo de ventas debe aparecer en el entorno de CRM como usuarios de CRM.</span><span class="sxs-lookup"><span data-stu-id="7f62e-122">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="7f62e-123">¿Qué requisitos previos son necesarios para crear Power Automate entorno?</span><span class="sxs-lookup"><span data-stu-id="7f62e-123">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="7f62e-124">Para usar el Power Automate, necesita:</span><span class="sxs-lookup"><span data-stu-id="7f62e-124">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="7f62e-125">Se requiere Power Automate licencia.</span><span class="sxs-lookup"><span data-stu-id="7f62e-125">A Power Automate license is required.</span></span>
- <span data-ttu-id="7f62e-126">Se requiere un almacenamiento mínimo de 1 GB.</span><span class="sxs-lookup"><span data-stu-id="7f62e-126">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="7f62e-127">¿Necesita una suscripción de Dynamics 365 para usar la solución Salesforce Connectors?</span><span class="sxs-lookup"><span data-stu-id="7f62e-127">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="7f62e-128">La solución Salesforce Connector es de tipo "Dynamics Flow", que admite la sincronización con otros sistemas CRM.</span><span class="sxs-lookup"><span data-stu-id="7f62e-128">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="7f62e-129">La solución no requiere que tenga una instancia de Dynamics 365 o una suscripción.</span><span class="sxs-lookup"><span data-stu-id="7f62e-129">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="7f62e-130">Al instalar la solución salesforce, puede aparecer una lista desplegable con el entorno de CDS existente en su empresa.</span><span class="sxs-lookup"><span data-stu-id="7f62e-130">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="7f62e-131">Debe seleccionar ese entorno.</span><span class="sxs-lookup"><span data-stu-id="7f62e-131">You need to select that environment.</span></span> <span data-ttu-id="7f62e-132">Además, si recibe el error "No se pudo encontrar una organización de Dynamics 365 conectada al usuario que ha iniciado sesión", deberá crear un nuevo entorno para el conector.</span><span class="sxs-lookup"><span data-stu-id="7f62e-132">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="7f62e-133">Preguntas y respuestas sobre la configuración</span><span class="sxs-lookup"><span data-stu-id="7f62e-133">Questions and answers about configuration</span></span>

1. <span data-ttu-id="7f62e-134">¿Qué debe hacer si se enfrenta al siguiente error al activar flujos en Power Automate Platform?</span><span class="sxs-lookup"><span data-stu-id="7f62e-134">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="7f62e-135">Error: Error al solicitar Azure Resource Manager error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span><span class="sxs-lookup"><span data-stu-id="7f62e-135">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="7f62e-136">Siga estos pasos de solución de problemas:</span><span class="sxs-lookup"><span data-stu-id="7f62e-136">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="7f62e-137">Elimine la conexión de CDS y vuelva a crear las conexiones DE CDS.</span><span class="sxs-lookup"><span data-stu-id="7f62e-137">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="7f62e-138">Desactivar y activar el flujo secundario</span><span class="sxs-lookup"><span data-stu-id="7f62e-138">Turn the child flow off and on</span></span> 
- <span data-ttu-id="7f62e-139">Elimine la solución y vuelva a instalarla.</span><span class="sxs-lookup"><span data-stu-id="7f62e-139">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="7f62e-140">¿Qué debe hacer si se encuentra con el error "Iniciar sesión" al agregar un conector Centro de partners en Power Automate Platform?</span><span class="sxs-lookup"><span data-stu-id="7f62e-140">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Mensaje de error que requiere inicio de sesión.":::

<span data-ttu-id="7f62e-142">Siga este paso de solución de problemas:</span><span class="sxs-lookup"><span data-stu-id="7f62e-142">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="7f62e-143">Use sus Centro de partners para iniciar sesión en el entorno de flujo una vez (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="7f62e-143">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="7f62e-144">¿Qué debe hacer si recibe el siguiente error al activar el flujo de Centro de partners a CRM en Power Automate Platform?</span><span class="sxs-lookup"><span data-stu-id="7f62e-144">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Mensaje de error que requiere actualizaciones.":::

<span data-ttu-id="7f62e-146">Siga estos pasos de solución de problemas:</span><span class="sxs-lookup"><span data-stu-id="7f62e-146">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="7f62e-147">Active primero los dos flujos secundarios siguientes antes de activar Centro de partners flujo de CRM.</span><span class="sxs-lookup"><span data-stu-id="7f62e-147">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="7f62e-148">Centro de partners a CRM- Helper (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7f62e-148">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="7f62e-149">Centro de partners actualizaciones de referencias de venta co-venta de Microsoft a CRM (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="7f62e-149">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="7f62e-150">¿Qué debe hacer cuando no puede agregar conexiones al flujo al intentar editar el flujo?</span><span class="sxs-lookup"><span data-stu-id="7f62e-150">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="7f62e-151">Se agregan conexiones al flujo mientras se ejecuta el flujo y se agrega a cada flujo por separado.</span><span class="sxs-lookup"><span data-stu-id="7f62e-151">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="7f62e-152">Si el cuadro de diálogo para agregar conexiones no se abre automáticamente al editar el flujo, puede editar cada uno de los pasos y sub pasos de los flujos individualmente.</span><span class="sxs-lookup"><span data-stu-id="7f62e-152">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="7f62e-153">Seleccione cada flujo y edirlos individualmente.</span><span class="sxs-lookup"><span data-stu-id="7f62e-153">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="7f62e-154">Expandir todos los pasos del flujo</span><span class="sxs-lookup"><span data-stu-id="7f62e-154">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Pasos que necesitan conexiones.":::

- <span data-ttu-id="7f62e-156">Seleccione los pasos en los que verá un icono de advertencia que le pide que asocie conexiones y agregue conexiones.</span><span class="sxs-lookup"><span data-stu-id="7f62e-156">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Edite el flujo paso a paso.":::


5. <span data-ttu-id="7f62e-158">¿Qué debe hacer si los flujos de la solución Conectores de referencias de venta co-venta no se activa?</span><span class="sxs-lookup"><span data-stu-id="7f62e-158">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="7f62e-159">A.</span><span class="sxs-lookup"><span data-stu-id="7f62e-159">A.</span></span> <span data-ttu-id="7f62e-160">En Power Automate, deberá editar los flujos en el orden siguiente y actualizarlos para usar las conexiones correctas:</span><span class="sxs-lookup"><span data-stu-id="7f62e-160">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="7f62e-161">Centro de partners webhook registration (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7f62e-161">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="7f62e-162">Creación de una referencia de venta co-venta: Salesforce Centro de partners (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="7f62e-162">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="7f62e-163">Centro de partners actualizaciones de referencias de venta co-venta de Microsoft a Salesforce (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="7f62e-163">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="7f62e-164">Centro de partners a Salesforce (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="7f62e-164">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="7f62e-165">Salesforce to Centro de partners (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7f62e-165">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="7f62e-166">Salesforce Opportunity to Centro de partners (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7f62e-166">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="7f62e-167">Salesforce Microsoft Solutions to Centro de partners (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7f62e-167">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="7f62e-168">B.</span><span class="sxs-lookup"><span data-stu-id="7f62e-168">B.</span></span> <span data-ttu-id="7f62e-169">Para cada flujo, seleccione la **opción Ejecutar solo usuarios.**</span><span class="sxs-lookup"><span data-stu-id="7f62e-169">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="7f62e-170">Seleccione **Usar conexión en** lugar de Proporcionado por el usuario de solo **ejecución.**</span><span class="sxs-lookup"><span data-stu-id="7f62e-170">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Para activar un flujo.":::


<span data-ttu-id="7f62e-172">C.</span><span class="sxs-lookup"><span data-stu-id="7f62e-172">C.</span></span> <span data-ttu-id="7f62e-173">Active estos flujos mencionados a continuación:</span><span class="sxs-lookup"><span data-stu-id="7f62e-173">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="7f62e-174">Centro de partners actualizaciones de referencias de venta co-venta de Microsoft a Salesforce (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="7f62e-174">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="7f62e-175">Salesforce to Centro de partners (Insider Preview)</span><span class="sxs-lookup"><span data-stu-id="7f62e-175">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="7f62e-176">D.</span><span class="sxs-lookup"><span data-stu-id="7f62e-176">D.</span></span> <span data-ttu-id="7f62e-177">Active todos los flujos restantes.</span><span class="sxs-lookup"><span data-stu-id="7f62e-177">Activate all the remaining flows.</span></span>

<span data-ttu-id="7f62e-178">E.</span><span class="sxs-lookup"><span data-stu-id="7f62e-178">E.</span></span> <span data-ttu-id="7f62e-179">En flow Centro de partners registro de webhook, seleccione **Ejecutar**.</span><span class="sxs-lookup"><span data-stu-id="7f62e-179">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="7f62e-180">Proporcione la **dirección URL http** de la primera acción en Centro de partners flujo de **Salesforce.**</span><span class="sxs-lookup"><span data-stu-id="7f62e-180">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="7f62e-181">Seleccione las cuatro opciones en **Eventos para registrar y** seleccione Sí **en** Sobrescribir.</span><span class="sxs-lookup"><span data-stu-id="7f62e-181">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="7f62e-182">Preguntas y respuestas sobre ejecución/mantenimiento</span><span class="sxs-lookup"><span data-stu-id="7f62e-182">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="7f62e-183">¿Cómo se solucionan los errores durante la Power Automate de flujo?</span><span class="sxs-lookup"><span data-stu-id="7f62e-183">How do you troubleshoot failures during Power Automate flow execution?</span></span>

<span data-ttu-id="7f62e-184">Para asegurarse de que los flujos de Power Automate se ejecutan según lo previsto y para solucionar los errores durante la ejecución, consulte [Corrección de errores de flujo](/power-automate/fix-flow-failures).</span><span class="sxs-lookup"><span data-stu-id="7f62e-184">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="7f62e-185">¿Qué debe hacer si ve referencias que no están sincronizadas correctamente en Centro de partners o crm?</span><span class="sxs-lookup"><span data-stu-id="7f62e-185">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="7f62e-186">Para determinar el estado de la sincronización de referencias, seleccione **Auditar**.</span><span class="sxs-lookup"><span data-stu-id="7f62e-186">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Sincronización de referencias.":::

<span data-ttu-id="7f62e-188">Asegúrese de que se cumplen las condiciones siguientes:</span><span class="sxs-lookup"><span data-stu-id="7f62e-188">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="7f62e-189">El identificador de la solución se proporciona como parte de la oportunidad.</span><span class="sxs-lookup"><span data-stu-id="7f62e-189">Solution ID is provided as part of the opportunity.</span></span>

- <span data-ttu-id="7f62e-190">Se requiere un código de país de dos letras.</span><span class="sxs-lookup"><span data-stu-id="7f62e-190">Two letter country code is required.</span></span>

- <span data-ttu-id="7f62e-191">Cuando se selecciona ayuda de Microsoft para la oportunidad, se requiere información de contacto del cliente.</span><span class="sxs-lookup"><span data-stu-id="7f62e-191">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="7f62e-192">¿Cómo asegurarse de que una referencia se sincronizará bidireccionalmente?</span><span class="sxs-lookup"><span data-stu-id="7f62e-192">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="7f62e-193">Siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="7f62e-193">Do the following steps:</span></span>

- <span data-ttu-id="7f62e-194">Los vendedores asociados deben asegurarse de que han habilitado la opción **Sync with Centro de partners** en la sección CRM.</span><span class="sxs-lookup"><span data-stu-id="7f62e-194">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Asegúrese de que ha habilitado Synch.":::

- <span data-ttu-id="7f62e-196">Los vendedores deben proporcionar los ingresos y la fecha de cierre al calificar a un cliente potencial.</span><span class="sxs-lookup"><span data-stu-id="7f62e-196">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="7f62e-197">Si el identificador de  CRM  se proporciona en la fase de creación o actualización de la oportunidad de venta en colaboración, pero no se encuentra una oportunidad de cliente potencial con ese identificador en CRM, se omitirá la actualización o la creación.</span><span class="sxs-lookup"><span data-stu-id="7f62e-197">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="7f62e-198">Asegúrese de que el campo de moneda de referencia está configurado en el entorno de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="7f62e-198">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="7f62e-199">¿Qué debe hacer si el conector se desconecta y se pierde una sincronización de referencias?</span><span class="sxs-lookup"><span data-stu-id="7f62e-199">What should you do if the connector gets disconnected and you miss a referral synchronization.?</span></span>

<span data-ttu-id="7f62e-200">Estas son algunas de las opciones que puede probar:</span><span class="sxs-lookup"><span data-stu-id="7f62e-200">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="7f62e-201">Compruebe si el nombre de usuario o la contraseña han expirado para Centro de partners usuario con roles de administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="7f62e-201">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="7f62e-202">Puede ir a la oportunidad no sincronizada, realizar una actualización secundaria y observar si la referencia se ha sincronizado.</span><span class="sxs-lookup"><span data-stu-id="7f62e-202">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="7f62e-203">Si los flujos se han ejecutado y han dado error, seleccione el flujo y vuelva a enviar la ejecución que ha dado error.</span><span class="sxs-lookup"><span data-stu-id="7f62e-203">If the flows have run and failed, then select the flow and re-submit the run that has failed.</span></span>

5. <span data-ttu-id="7f62e-204">¿Qué debe hacer al obtener errores de acceso denegado?</span><span class="sxs-lookup"><span data-stu-id="7f62e-204">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="7f62e-205">Asegúrese de que existen los roles adecuados.</span><span class="sxs-lookup"><span data-stu-id="7f62e-205">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="7f62e-206">Rol administrador de referencias para Centro de partners vendedor</span><span class="sxs-lookup"><span data-stu-id="7f62e-206">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="7f62e-207">Rol Administrador del sistema o Personalizador del sistema en la instancia de CRM</span><span class="sxs-lookup"><span data-stu-id="7f62e-207">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="7f62e-208">Asegúrese de que el Power Automate usuario de la cuenta de flujo de trabajo inicia sesión al https://flow.microsoft.com menos una vez con antelación.</span><span class="sxs-lookup"><span data-stu-id="7f62e-208">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="7f62e-209">Si ve que falta el **código de país** de la cuenta de cliente al crear una oportunidad de venta en colaboración, ¿qué debe hacer?</span><span class="sxs-lookup"><span data-stu-id="7f62e-209">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="7f62e-210">Deberá agregar el código de país iso de dos letras a la cuenta de cliente en CRM.</span><span class="sxs-lookup"><span data-stu-id="7f62e-210">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="7f62e-211">¿Qué debe hacer si ve el error de que el identificador de **solución es necesario** al crear una oportunidad de venta en colaboración?</span><span class="sxs-lookup"><span data-stu-id="7f62e-211">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="7f62e-212">Para crear una referencia de venta en colaboración, necesita una solución preparada para la venta en colaboración de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7f62e-212">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="7f62e-213">¿Qué debe hacer cuando vea que se crean oportunidades de venta Centro de partners que no están sincronizadas con CRM aunque no haya errores de flujo?</span><span class="sxs-lookup"><span data-stu-id="7f62e-213">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors?</span></span>

<span data-ttu-id="7f62e-214">Haga lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="7f62e-214">Do the following:</span></span>

- <span data-ttu-id="7f62e-215">Después de haber creado una nueva oferta de venta Centro de partners en Centro de partners, compruebe si se invoca el flujo de Centro de partners a Dynamics 365 (es posible que se invoque varias veces).</span><span class="sxs-lookup"><span data-stu-id="7f62e-215">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="7f62e-216">Si se invoca el flujo, compruebe todos los flujos invocados e identifique la ejecución del flujo que actualizaría el CRM.</span><span class="sxs-lookup"><span data-stu-id="7f62e-216">If the flow gets invoked, check all invoked flows, and identify the flow run which that would update the CRM.</span></span> <span data-ttu-id="7f62e-217">Puede seguir las acciones y comprobar si ha actualizado crm o ha detectado un problema.</span><span class="sxs-lookup"><span data-stu-id="7f62e-217">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="7f62e-218">Active **Nueva oferta** en Centro de partners para ver si se rellena con el identificador de CRM.</span><span class="sxs-lookup"><span data-stu-id="7f62e-218">Check **New deal** in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="7f62e-219">Asegúrese de que la oferta no se cierre accidentalmente como **Ganada** o **Perdida** en Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="7f62e-219">Make sure that the deal is not accidentally closed as **Won** or **Lost** in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7f62e-220">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="7f62e-220">Next steps</span></span>

- [<span data-ttu-id="7f62e-221">Administrar los clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="7f62e-221">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="7f62e-222">Administrar las oportunidades de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="7f62e-222">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)
