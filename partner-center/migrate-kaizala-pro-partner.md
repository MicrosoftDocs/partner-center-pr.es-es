---
title: Migración de suscripciones de Kaizala Pro a Microsoft 365
description: Obtenga información sobre cómo migrar suscripciones de Kaizala Pro Microsoft 365 u versiones de Office 365. Lea este artículo para obtener más detalles sobre la transición de los clientes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 96d18c8f728c56b705d378ac56dcf46e777157f0
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172411"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a><span data-ttu-id="9bd8f-104">Migración de suscripciones independientes de Kaizala Pro Microsoft 365 u versiones de Office 365</span><span class="sxs-lookup"><span data-stu-id="9bd8f-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft 365 or Office 365 versions</span></span>

<span data-ttu-id="9bd8f-105">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="9bd8f-105">**Appropriate roles**</span></span>

- <span data-ttu-id="9bd8f-106">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="9bd8f-106">Sales agent</span></span>

<span data-ttu-id="9bd8f-107">A partir del 1 de julio de 2020, Microsoft está finalizando las ventas del servicio independiente Kaizala Pro.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-107">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="9bd8f-108">Los clientes ya no podrán comprar nuevas suscripciones de Kaizala Pro después de esta fecha y las suscripciones de Kaizala Pro existentes no se renovarán automáticamente cuando expiren.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-108">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="9bd8f-109">Para garantizar la continuidad de los clientes, debe realizar la transición de los clientes con suscripciones independientes de Kaizala Pro expiradas a una opción de SKU compatible, que se muestra a continuación.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-109">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="9bd8f-110">Se recomienda mover clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones del servicio para los clientes.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-110">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="9bd8f-111">Si usa la API (YA SEAN O CENTRO DE PARTNERS), puede detectar suscripciones que expiran evaluando la fecha de finalización de la suscripción junto con la propiedad de renovación automática establecida en false: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="9bd8f-111">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="9bd8f-112">Las suscripciones E4 se establecerán en `auto renew=False` el 1 de julio de 2020.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-112">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="9bd8f-113">Puede trasladar clientes a un nuevo plan en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-113">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="9bd8f-114">Planes de reemplazo independientes de Kaizala Pro</span><span class="sxs-lookup"><span data-stu-id="9bd8f-114">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="9bd8f-115">Con los nuevos planes, los clientes pueden aprovechar las características y funcionalidades más recientes de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-115">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="9bd8f-116">Los detalles de precios se encuentran en la lista de precios y la matriz de la lista de ofertas en Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-116">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="9bd8f-117">[**Microsoft 365 para empresas,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)incluidos:</span><span class="sxs-lookup"><span data-stu-id="9bd8f-117">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="9bd8f-118">Microsoft 365 Empresa Básico</span><span class="sxs-lookup"><span data-stu-id="9bd8f-118">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="9bd8f-119">Microsoft 365 Empresa Estándar</span><span class="sxs-lookup"><span data-stu-id="9bd8f-119">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="9bd8f-120">Microsoft 365 Empresa Premium</span><span class="sxs-lookup"><span data-stu-id="9bd8f-120">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="9bd8f-121">[**Microsoft 365 para Frontline,**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)incluidos:</span><span class="sxs-lookup"><span data-stu-id="9bd8f-121">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="9bd8f-122">Microsoft 365 F3 (antes Microsoft 365 F1) y Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="9bd8f-122">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="9bd8f-123">[**Microsoft 365 para Enterprise,**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)incluidos:</span><span class="sxs-lookup"><span data-stu-id="9bd8f-123">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="9bd8f-124">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="9bd8f-124">Office 365 E1</span></span>
   - <span data-ttu-id="9bd8f-125">Microsoft 365 E3 y Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="9bd8f-125">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="9bd8f-126">Microsoft 365 E5 y Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="9bd8f-126">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="9bd8f-127">[**Microsoft 365 for Education,**](https://www.microsoft.com/education/buy-license/microsoft365)incluidos:</span><span class="sxs-lookup"><span data-stu-id="9bd8f-127">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="9bd8f-128">Microsoft 365 A1 y Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="9bd8f-128">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="9bd8f-129">Microsoft 365 A3 y Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="9bd8f-129">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="9bd8f-130">Microsoft 365 A5 y Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="9bd8f-130">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="9bd8f-131">Clientes de transición hacia los nuevos planes de productos</span><span class="sxs-lookup"><span data-stu-id="9bd8f-131">Transition customers to new product plans</span></span>

<span data-ttu-id="9bd8f-132">Microsoft ofrece continuamente nuevos productos y servicios a nuestros asociados.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-132">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="9bd8f-133">En estos casos, es posible que tenga que actualizar los clientes a nuevos servicios o migrar sus suscripciones desde SKU que finalmente se apagarán.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-133">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="9bd8f-134">La migración de clientes de SKU retiradas a otras más recientes requiere los pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="9bd8f-134">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="9bd8f-135">A.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-135">A.</span></span> <span data-ttu-id="9bd8f-136">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="9bd8f-136">Purchase the new subscription</span></span>

<span data-ttu-id="9bd8f-137">B.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-137">B.</span></span> <span data-ttu-id="9bd8f-138">Reasignación de licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="9bd8f-138">Reassign current user licenses</span></span>

<span data-ttu-id="9bd8f-139">C.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-139">C.</span></span> <span data-ttu-id="9bd8f-140">Cancelación de una suscripción antigua</span><span class="sxs-lookup"><span data-stu-id="9bd8f-140">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="9bd8f-141">Migración de clientes a nuevos planes</span><span class="sxs-lookup"><span data-stu-id="9bd8f-141">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="9bd8f-142">A.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-142">A.</span></span> <span data-ttu-id="9bd8f-143">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="9bd8f-143">Purchase the new subscription</span></span>

1. <span data-ttu-id="9bd8f-144">Para comprar la nueva suscripción, en el menú **Centro de partners,** seleccione **Clientes,** seleccione el cliente que desea mover y, a continuación, **seleccione Agregar suscripciones.**</span><span class="sxs-lookup"><span data-stu-id="9bd8f-144">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="9bd8f-145">Seleccione la suscripción que desea comprar del catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, **seleccione Enviar**.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-145">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="9bd8f-146">El cliente debe tener ahora suscripciones antiguas y nuevas, la suscripción independiente de Kaizala Pro antigua y la nueva suscripción de "destino", por ejemplo, Opción 1- Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-146">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="9bd8f-147">B.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-147">B.</span></span> <span data-ttu-id="9bd8f-148">Reasignación de licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="9bd8f-148">Reassign current user licenses</span></span>

1. <span data-ttu-id="9bd8f-149">Para reasignar las licencias de los usuarios del cliente, en el menú **Centro de partners,** seleccione **Clientes,** seleccione el cliente que va a mover y, a continuación, seleccione Usuarios **y licencias.**</span><span class="sxs-lookup"><span data-stu-id="9bd8f-149">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="9bd8f-150">Se abre la página Usuarios y licencias del cliente.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-150">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="9bd8f-151">Para reasignar la licencia de usuario, seleccione el usuario que desea reasignar y, a continuación, **seleccione Administrar licencias.**</span><span class="sxs-lookup"><span data-stu-id="9bd8f-151">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="9bd8f-152">En la **página Administrar licencias,** desactive la casilla Licencia independiente de Kaizala Pro y seleccione un nuevo plan de servicio para la suscripción a la que se traslada el cliente.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-152">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="9bd8f-153">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="9bd8f-153">Select **Submit**.</span></span> <span data-ttu-id="9bd8f-154">Una página de confirmación enumera las nuevas asignaciones de licencias.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-154">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="9bd8f-155">Continúe este mismo proceso para otros usuarios que necesiten asignaciones de licencias.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-155">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="9bd8f-156">C.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-156">C.</span></span> <span data-ttu-id="9bd8f-157">Cancelación de una suscripción antigua</span><span class="sxs-lookup"><span data-stu-id="9bd8f-157">Cancel old subscription</span></span>

<span data-ttu-id="9bd8f-158">Después de mover la licencia de usuario al nuevo servicio, puede cancelar de forma segura la suscripción retirada en el nivel de cliente.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-158">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="9bd8f-159">En el **menú Centro de partners,** seleccione **Clientes.**</span><span class="sxs-lookup"><span data-stu-id="9bd8f-159">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="9bd8f-160">Seleccione el cliente cuya suscripción va a cancelar.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-160">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="9bd8f-161">En la página de detalles de la suscripción, establezca la suscripción en **Suspendido.**</span><span class="sxs-lookup"><span data-stu-id="9bd8f-161">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="9bd8f-162">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="9bd8f-162">Select **Submit**.</span></span>

<span data-ttu-id="9bd8f-163">Se ha suspendido la suscripción antigua y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-163">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="9bd8f-164">La suscripción suspendida se desaprovisiona automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-164">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="9bd8f-165">El cliente no incurre en costos adicionales para la suscripción antigua.</span><span class="sxs-lookup"><span data-stu-id="9bd8f-165">The customer incurs no additional costs for the old subscription.</span></span>
