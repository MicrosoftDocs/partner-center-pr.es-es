---
title: Solución de problemas de conectores de referencias de venta conjunta
ms.topic: how-to
ms.date: 09/21/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga respuestas a preguntas habituales sobre el uso de conectores de venta conjunta. Lea estas preguntas más frecuentes sobre cómo solucionar problemas de conectores de venta conjunta.
author: sroy
ms.author: sroy
ms.localizationpriority: medium
ms.openlocfilehash: 988a696a8a0a0abb4d37e3915c76f905ec5b35b0
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/14/2020
ms.locfileid: "92031268"
---
# <a name="troubleshoot-co-sell-referrals-connectors"></a><span data-ttu-id="a7b59-104">Solución de problemas de conectores de referencias de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="a7b59-104">Troubleshoot co-sell referrals connectors</span></span>

<span data-ttu-id="a7b59-105">**Se aplica a:**</span><span class="sxs-lookup"><span data-stu-id="a7b59-105">**Applies to:**</span></span>

- <span data-ttu-id="a7b59-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="a7b59-106">Partner Center</span></span>
- <span data-ttu-id="a7b59-107">Dynamics 365 CRM</span><span class="sxs-lookup"><span data-stu-id="a7b59-107">Dynamics 365 CRM</span></span>
- <span data-ttu-id="a7b59-108">CRM de Salesforce</span><span class="sxs-lookup"><span data-stu-id="a7b59-108">Salesforce CRM</span></span>

<span data-ttu-id="a7b59-109">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="a7b59-109">**Appropriate roles**</span></span>

- <span data-ttu-id="a7b59-110">Administrador de referencias</span><span class="sxs-lookup"><span data-stu-id="a7b59-110">Referrals admin</span></span>
- <span data-ttu-id="a7b59-111">Administrador del sistema o Personalizador del sistema en CRM</span><span class="sxs-lookup"><span data-stu-id="a7b59-111">System admin or system customizer on the CRM</span></span>

 ## <a name="questions-and-answers-about-pre-requisites"></a><span data-ttu-id="a7b59-112">Preguntas y respuestas sobre los requisitos previos</span><span class="sxs-lookup"><span data-stu-id="a7b59-112">Questions and answers about pre-requisites</span></span>

1. <span data-ttu-id="a7b59-113">¿Puede usar una solución de conectores de referencias de venta conjunta de prueba para su entorno?</span><span class="sxs-lookup"><span data-stu-id="a7b59-113">Can you use a trial co-sell referrals connectors solution for your environment?</span></span>

<span data-ttu-id="a7b59-114">Si está en el entorno de prueba o ensayo, puede optar por la solución de prueba.</span><span class="sxs-lookup"><span data-stu-id="a7b59-114">If you are on the test/staging environment, you can opt for trial solution.</span></span> <span data-ttu-id="a7b59-115">La versión de pago de los conectores está disponible en AppSource en US $15/month.</span><span class="sxs-lookup"><span data-stu-id="a7b59-115">The paid version of the Connectors is available in AppSource at US$ 15/month.</span></span> <span data-ttu-id="a7b59-116">Con la conexión de pago, obtendrá 10 000 llamadas API al día.</span><span class="sxs-lookup"><span data-stu-id="a7b59-116">With the paid connection, you will be getting 10K API calls per day.</span></span> <span data-ttu-id="a7b59-117">Los conectores son contenedores que se encuentran en la parte superior de las API de referencia del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="a7b59-117">The Connectors are wrappers on top of Partner Center referral APIs.</span></span> <span data-ttu-id="a7b59-118">Cada vez que se ejecutan las soluciones de conector para un evento de **creación** o **actualización** sobre las oportunidades en el centro de Partners o en el lado de CRM, se realiza una llamada API.</span><span class="sxs-lookup"><span data-stu-id="a7b59-118">Whenever the connector solutions run for a **Create** or **Update** event on the opportunities on either Partner Center or the CRM side, an API call is made.</span></span>

2. <span data-ttu-id="a7b59-119">¿Qué rol necesita para crear secciones en el entorno de CRM?</span><span class="sxs-lookup"><span data-stu-id="a7b59-119">What role do you need to create sections in CRM environment?</span></span>

<span data-ttu-id="a7b59-120">Los usuarios que son administradores del sistema o personalizadores del sistema pueden aplicar cambios para todos.</span><span class="sxs-lookup"><span data-stu-id="a7b59-120">Users who are system admins or system customizers can apply changes for everyone.</span></span> <span data-ttu-id="a7b59-121">Sin embargo, todos los usuarios de la aplicación pueden personalizar el sistema e incluso compartir algunas de sus personalizaciones con otras personas.</span><span class="sxs-lookup"><span data-stu-id="a7b59-121">All app users, however,  can personalize the system and even share some of their customizations with others.</span></span> 

3. <span data-ttu-id="a7b59-122">¿Los vendedores de asociados necesitan roles especiales para trabajar en el centro de Partners?</span><span class="sxs-lookup"><span data-stu-id="a7b59-122">Do partner sellers need special roles to work on Partner Center?</span></span>
 
<span data-ttu-id="a7b59-123">A los vendedores asociados se les debe asignar el rol de administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="a7b59-123">Partner sellers must be assigned the “Referrals admin” role.</span></span> <span data-ttu-id="a7b59-124">Para obtener más información, consulte la siguiente [información general sobre los permisos] (Create-User-accounts-and-set-permissions).</span><span class="sxs-lookup"><span data-stu-id="a7b59-124">For more information, refer to the following [Permissions overview)(create-user-accounts-and-set-permissions).</span></span>

4. <span data-ttu-id="a7b59-125">¿Qué campos deben configurarse en primer lugar en el entorno de CRM?</span><span class="sxs-lookup"><span data-stu-id="a7b59-125">What fields need to be set up first in your CRM environment?</span></span> 

<span data-ttu-id="a7b59-126">• Asegúrese de que la moneda sea adecuada para su ubicación y que se encuentra en el entorno de CRM con precisión.</span><span class="sxs-lookup"><span data-stu-id="a7b59-126">• Make sure your currency is appropriate to your location and is in your CRM environment accurately.</span></span> <span data-ttu-id="a7b59-127">• El equipo de ventas debe aparecer en el entorno de CRM como usuarios de CRM.</span><span class="sxs-lookup"><span data-stu-id="a7b59-127">• Your sales team should be listed in your CRM environment as CRM users.</span></span>

5. <span data-ttu-id="a7b59-128">¿Cuáles son los requisitos previos necesarios para automatizar la creación de entornos?</span><span class="sxs-lookup"><span data-stu-id="a7b59-128">What pre-requisites are required for Power Automate environment creation?</span></span>

<span data-ttu-id="a7b59-129">Para usar el entorno de automatización de energía, necesita:</span><span class="sxs-lookup"><span data-stu-id="a7b59-129">To use the Power Automate environment, you need:</span></span>

- <span data-ttu-id="a7b59-130">Se necesita una licencia de Power Automatic.</span><span class="sxs-lookup"><span data-stu-id="a7b59-130">A Power Automate license is required.</span></span>
- <span data-ttu-id="a7b59-131">Se requiere un mínimo de 1 GB de almacenamiento.</span><span class="sxs-lookup"><span data-stu-id="a7b59-131">A minimum of 1-GB storage is required.</span></span>

6.  <span data-ttu-id="a7b59-132">¿Necesita una suscripción a Dynamics 365 para usar la solución de conectores de Salesforce?</span><span class="sxs-lookup"><span data-stu-id="a7b59-132">Do you need a Dynamics 365 subscription to use Salesforce Connectors solution?</span></span>

<span data-ttu-id="a7b59-133">La solución de conector de Salesforce es de tipo "flujo de Dynamics" que admite la sincronización con otros sistemas CRM.</span><span class="sxs-lookup"><span data-stu-id="a7b59-133">The Salesforce Connector solution is of type “Dynamics Flow” that supports synchronizing with other CRM systems.</span></span> <span data-ttu-id="a7b59-134">La solución no requiere que tenga una instancia de Dynamics 365 o una suscripción.</span><span class="sxs-lookup"><span data-stu-id="a7b59-134">The solution doesn’t require you to have a Dynamics 365 instance or a subscription.</span></span> <span data-ttu-id="a7b59-135">Al instalar la solución Salesforce, puede aparecer una lista desplegable con el entorno de CDS existente en la empresa.</span><span class="sxs-lookup"><span data-stu-id="a7b59-135">While installing the Salesforce solution, a drop-down with existing CDS environment in your company may appear.</span></span> <span data-ttu-id="a7b59-136">Debe seleccionar ese entorno.</span><span class="sxs-lookup"><span data-stu-id="a7b59-136">You need to select that environment.</span></span> <span data-ttu-id="a7b59-137">Además, si obtiene el error "no encontramos una organización de Dynamics 365 conectada al usuario que inició sesión", deberá crear un nuevo entorno para el conector.</span><span class="sxs-lookup"><span data-stu-id="a7b59-137">In addition, if you get the error "We couldn't find a Dynamics 365 organization connected to signed-in user", then you will need to create new environment for connector.</span></span>

## <a name="questions-and-answers-about-configuration"></a><span data-ttu-id="a7b59-138">Preguntas y respuestas acerca de la configuración</span><span class="sxs-lookup"><span data-stu-id="a7b59-138">Questions and answers about configuration</span></span>

1. <span data-ttu-id="a7b59-139">¿Qué debe hacer si se plantea el siguiente error al activar los flujos en Power automatization Platform?</span><span class="sxs-lookup"><span data-stu-id="a7b59-139">What should you do if you face the following error while activating flows in Power Automate Platform?</span></span>

<span data-ttu-id="a7b59-140">Error: no se pudo realizar la solicitud a Azure Resource Manager: "{" error ": {" Code ":" WorkflowTriggerNotFound "," message ":" no se encontró el desencadenador "e14d00f1-1fdf-4b1b-AAAC-54a5064093d3" del flujo de trabajo "manual". "}}".</span><span class="sxs-lookup"><span data-stu-id="a7b59-140">Error: Request to Azure Resource Manager failed with error: '{"error":{"code":"WorkflowTriggerNotFound","message":"The workflow 'e14d00f1-1fdf-4b1b-aaac-54a5064093d3' trigger 'manual' could not be found."}}'.</span></span> 

<span data-ttu-id="a7b59-141">Siga estos pasos de solución de problemas:</span><span class="sxs-lookup"><span data-stu-id="a7b59-141">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="a7b59-142">Elimine la conexión de CDS y, a continuación, vuelva a crear las conexiones de CDS.</span><span class="sxs-lookup"><span data-stu-id="a7b59-142">Delete the CDS connection and then recreate the CDS connections.</span></span>
- <span data-ttu-id="a7b59-143">Activar y desactivar el flujo secundario</span><span class="sxs-lookup"><span data-stu-id="a7b59-143">Turn the child flow off and on</span></span> 
- <span data-ttu-id="a7b59-144">Elimine la solución y, a continuación, vuelva a instalar la solución.</span><span class="sxs-lookup"><span data-stu-id="a7b59-144">Delete solution and then reinstall the solution.</span></span> 

2.  <span data-ttu-id="a7b59-145">¿Qué debe hacer si se plantea el error "iniciar sesión" al agregar un conector del centro de partners a la plataforma de automatización de energía?</span><span class="sxs-lookup"><span data-stu-id="a7b59-145">What should you do if you face the "Sign in" error while adding a Partner Center connector in Power Automate Platform?</span></span>

:::image type="content" source="images/cosellconnectors/failure.png" alt-text="Mensaje de error que requiere inicio de sesión":::

<span data-ttu-id="a7b59-147">Siga este paso de solución de problemas:</span><span class="sxs-lookup"><span data-stu-id="a7b59-147">Follow this troubleshooting step:</span></span>

- <span data-ttu-id="a7b59-148">Use las credenciales del centro de partners para iniciar sesión en el entorno de Flow (flow.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="a7b59-148">Use your Partner Center credentials to sign into the flow environment once (flow.microsoft.com).</span></span>


3. <span data-ttu-id="a7b59-149">¿Qué debe hacer si recibe el siguiente error al activar el flujo del centro de partners a CRM en la plataforma de automatización de energía?</span><span class="sxs-lookup"><span data-stu-id="a7b59-149">What should you do if you receive the following error while activating the Partner Center to CRM flow in Power Automate Platform?</span></span>
 
:::image type="content" source="images/cosellconnectors/powererror.png" alt-text="Mensaje de error que requiere inicio de sesión":::

<span data-ttu-id="a7b59-151">Siga estos pasos de solución de problemas:</span><span class="sxs-lookup"><span data-stu-id="a7b59-151">Follow these troubleshooting steps:</span></span>

- <span data-ttu-id="a7b59-152">Active los dos flujos secundarios siguientes antes de activar el flujo de CRM al centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="a7b59-152">Activate the following two child flows first before you activate the Partner Center to CRM flow.</span></span>
      - <span data-ttu-id="a7b59-153">Centro de partners a CRM: Ayudante (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="a7b59-153">Partner Center to CRM - Helper (Insider Preview)</span></span>
      - <span data-ttu-id="a7b59-154">Centro de Partners: actualizaciones de referencia de venta conjunta de Microsoft a CRM (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="a7b59-154">Partner Center Microsoft Co-sell Referral Updates to CRM (Insider Preview)</span></span>

4. <span data-ttu-id="a7b59-155">¿Qué debe hacer si no puede agregar conexiones al flujo al intentar editar el flujo?</span><span class="sxs-lookup"><span data-stu-id="a7b59-155">What should you do when you aren't able to add connections to the flow when you try to edit the flow?</span></span>

<span data-ttu-id="a7b59-156">Puede agregar conexiones al flujo mientras el flujo se está ejecutando y agregar cada flujo por separado.</span><span class="sxs-lookup"><span data-stu-id="a7b59-156">You add connections to the flow while the flow is running, and you add to each flow separately.</span></span>  <span data-ttu-id="a7b59-157">Si el cuadro de diálogo para agregar conexiones no se abre automáticamente mientras se edita el flujo, puede editar cada uno de los pasos y subpasos de los flujos individualmente.</span><span class="sxs-lookup"><span data-stu-id="a7b59-157">If the dialog to add connections doesn't open up automatically while editing the flow, then you can edit each of the steps and sub steps of the flows individually.</span></span>

- <span data-ttu-id="a7b59-158">Seleccione cada flujo y edítelo de forma individual.</span><span class="sxs-lookup"><span data-stu-id="a7b59-158">Select each flow and edit them individually.</span></span>
- <span data-ttu-id="a7b59-159">Expanda todos los pasos del flujo</span><span class="sxs-lookup"><span data-stu-id="a7b59-159">Expand all the steps in the flow</span></span> 

:::image type="content" source="images/cosellconnectors/flowsteps.png" alt-text="Mensaje de error que requiere inicio de sesión":::

- <span data-ttu-id="a7b59-161">Seleccione los pasos en los que verá un icono de advertencia pidiéndole asociar conexiones y agregue conexiones.</span><span class="sxs-lookup"><span data-stu-id="a7b59-161">Select the steps where you see a warning icon asking to associate connections, and add connections.</span></span> 

:::image type="content" source="images/cosellconnectors/editflow.png" alt-text="Mensaje de error que requiere inicio de sesión":::


5. <span data-ttu-id="a7b59-163">¿Qué debe hacer si los flujos de la solución de conectores de las referencias de venta conjunta no se activan?</span><span class="sxs-lookup"><span data-stu-id="a7b59-163">What should you do if the flows of the Co-sell Referrals Connectors solution don’t turn on?</span></span>

<span data-ttu-id="a7b59-164">A.</span><span class="sxs-lookup"><span data-stu-id="a7b59-164">A.</span></span> <span data-ttu-id="a7b59-165">En Power Automate, tendrá que editar los flujos en el siguiente orden y actualizarlos para que usen las conexiones correctas:</span><span class="sxs-lookup"><span data-stu-id="a7b59-165">In Power Automate, you'll need to edit flows in the following order and update them to use the correct connections:</span></span>

- <span data-ttu-id="a7b59-166">Registro del webhook del centro de Partners (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="a7b59-166">Partner Center Webhook Registration (Insider Preview)</span></span>
- <span data-ttu-id="a7b59-167">Creación de una referencia de venta conjunta: Salesforce al centro de Partners (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="a7b59-167">Create Co-sell Referral - Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="a7b59-168">Centro de Partners: actualizaciones de referencia de venta conjunta de Microsoft en Salesforce (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="a7b59-168">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="a7b59-169">Centro de partners a Salesforce (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="a7b59-169">Partner Center to Salesforce (Insider Preview)</span></span>
- <span data-ttu-id="a7b59-170">Salesforce a Partner Center (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="a7b59-170">Salesforce to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="a7b59-171">Oportunidad de Salesforce para el centro de Partners (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="a7b59-171">Salesforce Opportunity to Partner Center (Insider Preview)</span></span>
- <span data-ttu-id="a7b59-172">Soluciones de Salesforce de Microsoft para el centro de Partners (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="a7b59-172">Salesforce Microsoft Solutions to Partner Center (Insider Preview)</span></span>

 <span data-ttu-id="a7b59-173">B.</span><span class="sxs-lookup"><span data-stu-id="a7b59-173">B.</span></span> <span data-ttu-id="a7b59-174">Para cada flujo, seleccione la opción **ejecutar solo usuarios** .</span><span class="sxs-lookup"><span data-stu-id="a7b59-174">For each of flow, select **Run only users** option.</span></span> <span data-ttu-id="a7b59-175">Seleccione **Usar conexión** en lugar de **proporcionados por el usuario de solo ejecución**.</span><span class="sxs-lookup"><span data-stu-id="a7b59-175">Select **Use connection** instead of **Provided by run-only user**.</span></span>  

:::image type="content" source="images/cosellconnectors/runonly.png" alt-text="Mensaje de error que requiere inicio de sesión":::


<span data-ttu-id="a7b59-177">C.</span><span class="sxs-lookup"><span data-stu-id="a7b59-177">C.</span></span> <span data-ttu-id="a7b59-178">Active estos flujos que se indican a continuación:</span><span class="sxs-lookup"><span data-stu-id="a7b59-178">Activate these below mentioned flows:</span></span>

 - <span data-ttu-id="a7b59-179">Centro de Partners: actualizaciones de referencia de venta conjunta de Microsoft en Salesforce (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="a7b59-179">Partner Center Microsoft Co-sell Referral Updates to Salesforce (Insider Preview)</span></span>

- <span data-ttu-id="a7b59-180">Salesforce a Partner Center (versión preliminar de Insider)</span><span class="sxs-lookup"><span data-stu-id="a7b59-180">Salesforce to Partner Center (Insider Preview)</span></span>

    
<span data-ttu-id="a7b59-181">D.</span><span class="sxs-lookup"><span data-stu-id="a7b59-181">D.</span></span> <span data-ttu-id="a7b59-182">Active todos los flujos restantes.</span><span class="sxs-lookup"><span data-stu-id="a7b59-182">Activate all the remaining flows.</span></span>

<span data-ttu-id="a7b59-183">E.</span><span class="sxs-lookup"><span data-stu-id="a7b59-183">E.</span></span> <span data-ttu-id="a7b59-184">En el registro del webhook del centro de Partners de Flow, seleccione **Ejecutar**.</span><span class="sxs-lookup"><span data-stu-id="a7b59-184">At flow Partner Center Webhook Registration, select **Run**.</span></span> <span data-ttu-id="a7b59-185">Proporcione la **dirección URL http** de la primera acción del **centro de Partners al flujo de Salesforce** .</span><span class="sxs-lookup"><span data-stu-id="a7b59-185">Provide the **http url** from the first action in **Partner Center to Salesforce** flow.</span></span> <span data-ttu-id="a7b59-186">Seleccione las cuatro opciones en **eventos para registrarse** y seleccione **sí** para sobrescribir.</span><span class="sxs-lookup"><span data-stu-id="a7b59-186">Select all four options under **Events to register** and select **yes** for Overwrite.</span></span>

## <a name="questions-and-answers-about-runmaintenance"></a><span data-ttu-id="a7b59-187">Preguntas y respuestas sobre la ejecución/mantenimiento</span><span class="sxs-lookup"><span data-stu-id="a7b59-187">Questions and answers about Run/Maintenance</span></span>

1. <span data-ttu-id="a7b59-188">¿Cómo se solucionan los problemas en caso de que se produzcan errores durante la ejecución del flujo de energía automatizada?</span><span class="sxs-lookup"><span data-stu-id="a7b59-188">How do you troubleshoot in case of failures during Power Automate flow execution?</span></span>

<span data-ttu-id="a7b59-189">Para asegurarse de que los flujos de energía automatizada se ejecutan como se espera y para solucionar errores durante la ejecución, consulte [solucionar errores de flujo](/power-automate/fix-flow-failures).</span><span class="sxs-lookup"><span data-stu-id="a7b59-189">To ensure that your Power Automate flows run as you expect and to troubleshoot failures during execution, refer to [Fix flow failures](/power-automate/fix-flow-failures).</span></span>

2. <span data-ttu-id="a7b59-190">¿Qué debe hacer si ve referencias que no están sincronizadas correctamente en el centro de Partners o en el entorno de CRM?</span><span class="sxs-lookup"><span data-stu-id="a7b59-190">What should you do if you see referrals that aren't synchronized properly in Partner Center or CRM environment?</span></span>
 
<span data-ttu-id="a7b59-191">Para determinar el estado de la sincronización de referencias, seleccione **Auditoría**.</span><span class="sxs-lookup"><span data-stu-id="a7b59-191">To determine the status of referral synchronization, select **Audit**.</span></span> 

:::image type="content" source="images/cosellconnectors/synch.png" alt-text="Mensaje de error que requiere inicio de sesión":::

<span data-ttu-id="a7b59-193">Asegúrese de que se cumplen las condiciones siguientes:</span><span class="sxs-lookup"><span data-stu-id="a7b59-193">Ensure that the following conditions are met:</span></span>

- <span data-ttu-id="a7b59-194">El identificador de la solución se proporciona como parte de la oportunidad.</span><span class="sxs-lookup"><span data-stu-id="a7b59-194">Solution id is provided as part of the opportunity.</span></span>

- <span data-ttu-id="a7b59-195">Se requiere código de país de dos letras.</span><span class="sxs-lookup"><span data-stu-id="a7b59-195">Two letter country code is required.</span></span>

- <span data-ttu-id="a7b59-196">Cuando se selecciona ayuda de Microsoft para la oportunidad, se requiere la información de contacto del cliente.</span><span class="sxs-lookup"><span data-stu-id="a7b59-196">When help from Microsoft is selected for the opportunity, customer contact information is required.</span></span>

3. <span data-ttu-id="a7b59-197">Cómo asegurarse de que una referencia se va a sincronizar de forma bidireccional</span><span class="sxs-lookup"><span data-stu-id="a7b59-197">How to ensure that a referral will synchronize bi-directionally?</span></span>

<span data-ttu-id="a7b59-198">Siga estos pasos:</span><span class="sxs-lookup"><span data-stu-id="a7b59-198">Do the following steps:</span></span>

- <span data-ttu-id="a7b59-199">Los vendedores asociados deben asegurarse de que tienen habilitada la opción **sincronizar con el centro de Partners** en la sección CRM.</span><span class="sxs-lookup"><span data-stu-id="a7b59-199">Partner sellers need to ensure that they have enabled **Sync with Partner Center** option in the CRM section.</span></span>

:::image type="content" source="images/cosellconnectors/enablesynch.png" alt-text="Mensaje de error que requiere inicio de sesión":::

- <span data-ttu-id="a7b59-201">Los vendedores deben proporcionar los ingresos y la fecha de cierre al calificar a un cliente potencial.</span><span class="sxs-lookup"><span data-stu-id="a7b59-201">Sellers need to provide revenue and closing date when qualifying a lead.</span></span>

- <span data-ttu-id="a7b59-202">Si se proporciona el identificador de CRM en la fase de **creación** o **actualización** de la oportunidad de venta conjunta, pero no se encuentra una oportunidad de cliente con ese identificador en CRM, se omitirá actualizar o crear.</span><span class="sxs-lookup"><span data-stu-id="a7b59-202">If CRM ID is provided in the **create** or **update** stage of co-sell opportunity, but a lead opportunity with that ID is not found in CRM, then update or create will be ignored.</span></span>

- <span data-ttu-id="a7b59-203">Asegúrese de que el campo de moneda de referencia está configurado en el entorno de Salesforce.</span><span class="sxs-lookup"><span data-stu-id="a7b59-203">Ensure that referral currency field is configured on Salesforce environment.</span></span> 

4. <span data-ttu-id="a7b59-204">¿Qué debe hacer si el conector se desconecta y se pierde la sincronización de una referencia.</span><span class="sxs-lookup"><span data-stu-id="a7b59-204">What should you do if the connector gets disconnected and you miss a referral synchronization.</span></span> 

<span data-ttu-id="a7b59-205">A continuación se muestran algunas de las opciones que puede probar:</span><span class="sxs-lookup"><span data-stu-id="a7b59-205">Following are few of the options that you can try out:</span></span>

- <span data-ttu-id="a7b59-206">Compruebe si el nombre de usuario o la contraseña han expirado para el usuario del centro de Partners con roles de administrador de referencias.</span><span class="sxs-lookup"><span data-stu-id="a7b59-206">Check whether username or password has expired for the Partner Center user with referral admin roles.</span></span>

- <span data-ttu-id="a7b59-207">Puede ir a la oportunidad no sincronizada, realizar una actualización menor y observar si la referencia se ha sincronizado.</span><span class="sxs-lookup"><span data-stu-id="a7b59-207">You can go to the un-synchronized opportunity, make a minor update, and observe whether the referral has synchronized.</span></span>

- <span data-ttu-id="a7b59-208">Si los flujos se han ejecutado y han dado error, seleccione el flujo y vuelva a enviar la ejecución que ha producido un error.</span><span class="sxs-lookup"><span data-stu-id="a7b59-208">If the flows have run and failed, then select the flow and re-submit the run which has failed.</span></span>

5. <span data-ttu-id="a7b59-209">¿Qué debe hacer cuando se produce un error de acceso denegado?</span><span class="sxs-lookup"><span data-stu-id="a7b59-209">What should you do when you get access denied errors?</span></span>

<span data-ttu-id="a7b59-210">Asegúrese de que existen los roles adecuados</span><span class="sxs-lookup"><span data-stu-id="a7b59-210">Make sure the appropriate roles exist</span></span>

- <span data-ttu-id="a7b59-211">Rol de administrador de referencias para el vendedor del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="a7b59-211">Referral Administrator role for Partner Center seller</span></span> 
 
- <span data-ttu-id="a7b59-212">Rol de administrador del sistema o del Personalizador del sistema en la instancia de CRM</span><span class="sxs-lookup"><span data-stu-id="a7b59-212">System Administrator or System Customizer role on your CRM instance</span></span>

- <span data-ttu-id="a7b59-213">Asegúrese de que el usuario de la cuenta de flujo de Power Automate inicia sesión https://flow.microsoft.com al menos una vez de antemano.</span><span class="sxs-lookup"><span data-stu-id="a7b59-213">Ensure that the Power Automate flow account user logs into https://flow.microsoft.com at least once beforehand</span></span>

6. <span data-ttu-id="a7b59-214">Si ve que falta el código de país de la **cuenta de cliente** al crear una oportunidad de venta conjunta, ¿qué debe hacer?</span><span class="sxs-lookup"><span data-stu-id="a7b59-214">If you see that **Customer account country code** is missing while creating a Co-sell opportunity, what should you do?</span></span>

<span data-ttu-id="a7b59-215">Tendrá que agregar el código de país de dos letras ISO a la cuenta de cliente en CRM.</span><span class="sxs-lookup"><span data-stu-id="a7b59-215">You will need to add the ISO two-letter country code to the Customer account in CRM.</span></span>

7. <span data-ttu-id="a7b59-216">¿Qué debe hacer si ve el error el identificador de la **solución es necesario** al crear una oportunidad de venta conjunta?</span><span class="sxs-lookup"><span data-stu-id="a7b59-216">What should you do if you see the error that **Solution ID is required** while creating a Co-sell opportunity?</span></span>

<span data-ttu-id="a7b59-217">Con el fin de crear una referencia de venta conjunta, necesita una solución lista para participar de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a7b59-217">In order to create a co-sell referral, you need a Microsoft co-sell ready solution.</span></span> 

8. <span data-ttu-id="a7b59-218">¿Qué debe hacer cuando vea oportunidades de venta conjunta creadas en el centro de partners que no se sincronizan con CRM aunque no se produzcan errores de flujo:</span><span class="sxs-lookup"><span data-stu-id="a7b59-218">What should you do when you see Co-sell opportunities created in Partner Center that aren't synchronized to CRM even though there are no flow errors:</span></span>

<span data-ttu-id="a7b59-219">Haga lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="a7b59-219">Do the following:</span></span>

- <span data-ttu-id="a7b59-220">Una vez que haya creado un nuevo trato de venta conjunta en el centro de Partners, compruebe si se invoca el flujo del centro de partners a Dynamics 365 (es posible que se invoque varias veces).</span><span class="sxs-lookup"><span data-stu-id="a7b59-220">After you have created a new co-sell deal in Partner Center, check if Partner Center to Dynamics 365 flow gets invoked (it might get invoked multiple times).</span></span>

- <span data-ttu-id="a7b59-221">Si se invoca el flujo, compruebe todos los flujos invocados e identifique la ejecución de flujo que actualizaría el CRM.</span><span class="sxs-lookup"><span data-stu-id="a7b59-221">If the flow gets invoked, check all invoked flows, and identify the flow run which would update the CRM.</span></span> <span data-ttu-id="a7b59-222">Puede seguir las acciones y comprobar si se ha actualizado el CRM o si se ha producido un problema.</span><span class="sxs-lookup"><span data-stu-id="a7b59-222">You can follow the actions and verify if it did update the CRM or encountered a problem.</span></span>

- <span data-ttu-id="a7b59-223">Consulte *nuevo trato*\* en el centro de partners para ver si se rellena con el identificador de CRM.</span><span class="sxs-lookup"><span data-stu-id="a7b59-223">Check *New deal*\* in Partner Center to see if it gets populated with CRM ID.</span></span>

- <span data-ttu-id="a7b59-224">Asegúrese de que el trato no se cierra accidentalmente como "ganada" o "perdida" en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="a7b59-224">Make sure that the deal is not accidentally closed as “Won” or “Lost” in Partner Center.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a7b59-225">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="a7b59-225">Next steps</span></span>

- [<span data-ttu-id="a7b59-226">Administrar los clientes potenciales</span><span class="sxs-lookup"><span data-stu-id="a7b59-226">Manage leads</span></span>](manage-leads.md)
 
- [<span data-ttu-id="a7b59-227">Administrar las oportunidades de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="a7b59-227">Manage co-sell opportunities</span></span>](manage-co-sell-opportunities.md)