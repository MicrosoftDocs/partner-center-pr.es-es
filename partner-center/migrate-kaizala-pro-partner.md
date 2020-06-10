---
title: Migración de suscripciones de Kaizala Pro a Microsoft365
description: Obtenga información sobre cómo migrar las suscripciones de Kaizala Pro a las versiones de Microsoft365 o Office 365.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 842f4c0f88eec370821fa05c40cfadeee7fee12a
ms.sourcegitcommit: 8b7ef46a88aa5eb52ceefadfc5b0a06c3702d123
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/09/2020
ms.locfileid: "84611241"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a><span data-ttu-id="ea4ec-103">Migración de suscripciones independientes de Kaizala Pro a versiones de Microsoft365 o Office 365</span><span class="sxs-lookup"><span data-stu-id="ea4ec-103">Migrate Kaizala Pro Standalone subscriptions to Microsoft365 or Office 365 versions</span></span>

<span data-ttu-id="ea4ec-104">A partir del 1 de julio de 2020, Microsoft está terminando las ventas del servicio independiente Kaizala Pro.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-104">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="ea4ec-105">Los clientes ya no podrán comprar nuevas suscripciones de Kaizala Pro después de esta fecha, y las suscripciones de Kaizala Pro existentes no se renovarán automáticamente cuando expiren.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-105">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="ea4ec-106">Para garantizar la continuidad de los clientes, debe realizar la transición de los clientes con suscripciones independientes de Kaizala pro de expiración a una opción de SKU compatible, que se enumera a continuación.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-106">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="ea4ec-107">Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-107">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="ea4ec-108">Si usa la API (de la cresta o del centro de Partners), puede detectar las suscripciones que han expirado evaluando la fecha de finalización de la suscripción junto con la propiedad renovación automática establecida en false: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="ea4ec-108">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="ea4ec-109">Las suscripciones del plan E4 se establecerán `auto renew=False` en el 1 de julio de 2020.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-109">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="ea4ec-110">Puede trasladar a los clientes a un nuevo plan en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-110">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="ea4ec-111">Planes de reemplazo independientes de Kaizala Pro</span><span class="sxs-lookup"><span data-stu-id="ea4ec-111">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="ea4ec-112">Con los nuevos planes, sus clientes pueden beneficiarse de las características y funcionalidades más recientes en Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-112">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="ea4ec-113">Los detalles de precios se encuentran en la lista de precios y en la matriz de lista de ofertas del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-113">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="ea4ec-114">[**Microsoft 365 para empresas**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), incluidos:</span><span class="sxs-lookup"><span data-stu-id="ea4ec-114">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="ea4ec-115">Microsoft 365 Empresa Basic</span><span class="sxs-lookup"><span data-stu-id="ea4ec-115">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="ea4ec-116">Estándar Microsoft 365 Empresa</span><span class="sxs-lookup"><span data-stu-id="ea4ec-116">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="ea4ec-117">Microsoft 365 Empresa Premium</span><span class="sxs-lookup"><span data-stu-id="ea4ec-117">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="ea4ec-118">[**Microsoft 365 para Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), incluidos:</span><span class="sxs-lookup"><span data-stu-id="ea4ec-118">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="ea4ec-119">Microsoft 365 F3 (antes Microsoft 365 F1) y Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="ea4ec-119">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="ea4ec-120">[**Microsoft 365 para Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), incluido:</span><span class="sxs-lookup"><span data-stu-id="ea4ec-120">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="ea4ec-121">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="ea4ec-121">Office 365 E1</span></span>
   - <span data-ttu-id="ea4ec-122">Microsoft 365 E3 y Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="ea4ec-122">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="ea4ec-123">Microsoft 365 E5 y Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="ea4ec-123">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="ea4ec-124">[**Microsoft 365 para educación**](https://www.microsoft.com/education/buy-license/microsoft365), incluidos:</span><span class="sxs-lookup"><span data-stu-id="ea4ec-124">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="ea4ec-125">Microsoft 365 a1 y Office 365 a1</span><span class="sxs-lookup"><span data-stu-id="ea4ec-125">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="ea4ec-126">Microsoft 365 a3 y Office 365 a3</span><span class="sxs-lookup"><span data-stu-id="ea4ec-126">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="ea4ec-127">Microsoft 365 A5 y Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="ea4ec-127">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="ea4ec-128">Clientes de transición hacia los nuevos planes de productos</span><span class="sxs-lookup"><span data-stu-id="ea4ec-128">Transition customers to new product plans</span></span>

<span data-ttu-id="ea4ec-129">Microsoft ofrece continuamente nuevos productos y servicios a nuestros asociados.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-129">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="ea4ec-130">En estos casos, es posible que tenga que actualizar los clientes a nuevos servicios o migrar sus suscripciones de SKU que se apagarán finalmente.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-130">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="ea4ec-131">La migración de los clientes de SKU retiradas a otras más recientes requiere los siguientes pasos:</span><span class="sxs-lookup"><span data-stu-id="ea4ec-131">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="ea4ec-132">A.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-132">A.</span></span> <span data-ttu-id="ea4ec-133">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="ea4ec-133">Purchase the new subscription</span></span>

<span data-ttu-id="ea4ec-134">B.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-134">B.</span></span> <span data-ttu-id="ea4ec-135">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="ea4ec-135">Reassign current user licenses</span></span>

<span data-ttu-id="ea4ec-136">C.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-136">C.</span></span> <span data-ttu-id="ea4ec-137">Cancelar suscripción anterior</span><span class="sxs-lookup"><span data-stu-id="ea4ec-137">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="ea4ec-138">Migre sus clientes a nuevos planes</span><span class="sxs-lookup"><span data-stu-id="ea4ec-138">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="ea4ec-139">A.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-139">A.</span></span> <span data-ttu-id="ea4ec-140">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="ea4ec-140">Purchase the new subscription</span></span>

1. <span data-ttu-id="ea4ec-141">Para comprar la nueva suscripción, en el menú del **centro de Partners** , seleccione **clientes**, seleccione el cliente que desea migrar y, a continuación, seleccione **Agregar suscripciones**.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-141">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="ea4ec-142">Seleccione la suscripción que desea comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="ea4ec-142">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="ea4ec-143">El cliente debería tener ahora suscripciones antiguas y nuevas, la antigua suscripción independiente de Kaizala Pro y la nueva suscripción de destino, por ejemplo, la opción 1-Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-143">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="ea4ec-144">B.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-144">B.</span></span> <span data-ttu-id="ea4ec-145">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="ea4ec-145">Reassign current user licenses</span></span>

1. <span data-ttu-id="ea4ec-146">Para reasignar las licencias de los usuarios del cliente, en el menú del **centro de Partners** , seleccione **clientes**, seleccione el cliente que va a mover y, a continuación, seleccione **usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-146">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="ea4ec-147">Se abre la página usuarios y licencias del cliente.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-147">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="ea4ec-148">Para reasignar la licencia de usuario, seleccione el usuario que desea reasignar y, a continuación, seleccione **administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-148">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="ea4ec-149">En la página **administrar licencias** , desactive la casilla de Kaizala Pro independiente License y seleccione un nuevo plan de servicio para la suscripción a la que se desplaza el cliente.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-149">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="ea4ec-150">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="ea4ec-150">Select **Submit**.</span></span> <span data-ttu-id="ea4ec-151">Una página de confirmación enumera las nuevas asignaciones de licencias.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-151">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="ea4ec-152">Continúe con el mismo proceso para otros usuarios que necesiten asignaciones de licencia.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-152">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="ea4ec-153">C.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-153">C.</span></span> <span data-ttu-id="ea4ec-154">Cancelar suscripción anterior</span><span class="sxs-lookup"><span data-stu-id="ea4ec-154">Cancel old subscription</span></span>

<span data-ttu-id="ea4ec-155">Después de mover la licencia de usuario al nuevo servicio, puede cancelar con seguridad la suscripción retirada en el nivel de cliente.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-155">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="ea4ec-156">En el menú del **centro de Partners** , seleccione **clientes**.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-156">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="ea4ec-157">Seleccione el cliente cuya suscripción va a cancelar.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-157">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="ea4ec-158">En la página de detalles de la suscripción, establezca la suscripción en **Suspended**.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-158">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="ea4ec-159">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="ea4ec-159">Select **Submit**.</span></span>

<span data-ttu-id="ea4ec-160">Se ha suspendido la suscripción antigua y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-160">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="ea4ec-161">La suscripción suspendida se desaprovisionará automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-161">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="ea4ec-162">El cliente no incurre en costos adicionales para la suscripción antigua.</span><span class="sxs-lookup"><span data-stu-id="ea4ec-162">The customer incurs no additional costs for the old subscription.</span></span>
