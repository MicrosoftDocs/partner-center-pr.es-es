---
title: Migración de suscripciones de Kaizala Pro a Microsoft365
description: Obtenga información sobre cómo migrar las suscripciones de Kaizala Pro a las versiones de Microsoft365 o Office 365. Lea este artículo para obtener más información sobre la transición de los clientes.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175172"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a><span data-ttu-id="59173-104">Migración de suscripciones independientes de Kaizala Pro a versiones de Microsoft365 o Office 365</span><span class="sxs-lookup"><span data-stu-id="59173-104">Migrate Kaizala Pro Standalone subscriptions to Microsoft365 or Office 365 versions</span></span>

<span data-ttu-id="59173-105">A partir del 1 de julio de 2020, Microsoft está terminando las ventas del servicio independiente Kaizala Pro.</span><span class="sxs-lookup"><span data-stu-id="59173-105">Effective July 1, 2020, Microsoft is ending sales of the Kaizala Pro standalone service.</span></span> <span data-ttu-id="59173-106">Los clientes ya no podrán comprar nuevas suscripciones de Kaizala Pro después de esta fecha, y las suscripciones de Kaizala Pro existentes no se renovarán automáticamente cuando expiren.</span><span class="sxs-lookup"><span data-stu-id="59173-106">Customers will no longer be able to purchase new Kaizala Pro subscriptions after this date, and existing Kaizala Pro subscriptions will not renew automatically when they expire.</span></span>

<span data-ttu-id="59173-107">Para garantizar la continuidad de los clientes, debe realizar la transición de los clientes con suscripciones independientes de Kaizala pro de expiración a una opción de SKU compatible, que se enumera a continuación.</span><span class="sxs-lookup"><span data-stu-id="59173-107">To ensure continuity for customers, you should transition customers with expiring Kaizala Pro standalone subscriptions to a supported SKU option, listed below.</span></span> <span data-ttu-id="59173-108">Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes.</span><span class="sxs-lookup"><span data-stu-id="59173-108">We recommend moving customers to new subscriptions before the subscription's yearly end date to avoid any service outages for customers.</span></span>

<span data-ttu-id="59173-109">Si usa la API (de la cresta o del centro de Partners), puede detectar las suscripciones que han expirado evaluando la fecha de finalización de la suscripción junto con la propiedad renovación automática establecida en false: `auto renew = False` .</span><span class="sxs-lookup"><span data-stu-id="59173-109">If you use the API (either CREST or Partner Center), you can discover expiring subscriptions by evaluating the end date of the subscription along with the auto renew property set to false: `auto renew = False`.</span></span>

<span data-ttu-id="59173-110">Las suscripciones del plan E4 se establecerán `auto renew=False` en el 1 de julio de 2020.</span><span class="sxs-lookup"><span data-stu-id="59173-110">The E4 subscriptions will be set to `auto renew=False` on July 1, 2020.</span></span> <span data-ttu-id="59173-111">Puede trasladar a los clientes a un nuevo plan en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="59173-111">You can move customers to a new plan at any time.</span></span>

## <a name="kaizala-pro-standalone-replacement-plans"></a><span data-ttu-id="59173-112">Planes de reemplazo independientes de Kaizala Pro</span><span class="sxs-lookup"><span data-stu-id="59173-112">Kaizala Pro Standalone replacement plans</span></span>

<span data-ttu-id="59173-113">Con los nuevos planes, sus clientes pueden beneficiarse de las características y funcionalidades más recientes en Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="59173-113">With the new plans, your customers can take advantage of newer features and functionality in Microsoft 365.</span></span> <span data-ttu-id="59173-114">Los detalles de precios se encuentran en la lista de precios y en la matriz de lista de ofertas del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="59173-114">Pricing details are found on the price list and offer list matrix in Partner Center.</span></span>

- <span data-ttu-id="59173-115">[**Microsoft 365 para empresas**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), incluidos:</span><span class="sxs-lookup"><span data-stu-id="59173-115">[**Microsoft 365 for Business**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), including:</span></span>  
   - <span data-ttu-id="59173-116">Microsoft 365 Empresa Básico</span><span class="sxs-lookup"><span data-stu-id="59173-116">Microsoft 365 Business Basic</span></span>
   - <span data-ttu-id="59173-117">Microsoft 365 Empresa Estándar</span><span class="sxs-lookup"><span data-stu-id="59173-117">Microsoft 365 Business Standard</span></span>
   - <span data-ttu-id="59173-118">Microsoft 365 Empresa Premium</span><span class="sxs-lookup"><span data-stu-id="59173-118">Microsoft 365 Business Premium</span></span>
    
- <span data-ttu-id="59173-119">[**Microsoft 365 para Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), incluidos:</span><span class="sxs-lookup"><span data-stu-id="59173-119">[**Microsoft 365 for Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), including:</span></span>
   - <span data-ttu-id="59173-120">Microsoft 365 F3 (antes Microsoft 365 F1) y Office 365 F3</span><span class="sxs-lookup"><span data-stu-id="59173-120">Microsoft 365 F3 (formerly Microsoft 365 F1) and Office 365 F3</span></span>
    
- <span data-ttu-id="59173-121">[**Microsoft 365 para Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), incluido:</span><span class="sxs-lookup"><span data-stu-id="59173-121">[**Microsoft 365 for Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), including:</span></span> 
   - <span data-ttu-id="59173-122">Office 365 E1</span><span class="sxs-lookup"><span data-stu-id="59173-122">Office 365 E1</span></span>
   - <span data-ttu-id="59173-123">Microsoft 365 E3 y Office 365 E3</span><span class="sxs-lookup"><span data-stu-id="59173-123">Microsoft 365 E3 and Office 365 E3</span></span>
   - <span data-ttu-id="59173-124">Microsoft 365 E5 y Office 365 E5</span><span class="sxs-lookup"><span data-stu-id="59173-124">Microsoft 365 E5 and Office 365 E5</span></span>

- <span data-ttu-id="59173-125">[**Microsoft 365 para educación**](https://www.microsoft.com/education/buy-license/microsoft365), incluidos:</span><span class="sxs-lookup"><span data-stu-id="59173-125">[**Microsoft 365 for Education**](https://www.microsoft.com/education/buy-license/microsoft365), including:</span></span> 
    - <span data-ttu-id="59173-126">Microsoft 365 A1 y Office 365 A1</span><span class="sxs-lookup"><span data-stu-id="59173-126">Microsoft 365 A1 and Office 365 A1</span></span>
    - <span data-ttu-id="59173-127">Microsoft 365 A3 y Office 365 A3</span><span class="sxs-lookup"><span data-stu-id="59173-127">Microsoft 365 A3 and Office 365 A3</span></span>
    - <span data-ttu-id="59173-128">Microsoft 365 A5 y Office 365 A5</span><span class="sxs-lookup"><span data-stu-id="59173-128">Microsoft 365 A5 and Office 365 A5</span></span>

## <a name="transition-customers-to-new-product-plans"></a><span data-ttu-id="59173-129">Clientes de transición hacia los nuevos planes de productos</span><span class="sxs-lookup"><span data-stu-id="59173-129">Transition customers to new product plans</span></span>

<span data-ttu-id="59173-130">Microsoft ofrece continuamente nuevos productos y servicios a nuestros asociados.</span><span class="sxs-lookup"><span data-stu-id="59173-130">Microsoft continuously offers new products and services to our partners.</span></span> <span data-ttu-id="59173-131">En estos casos, es posible que tenga que actualizar los clientes a nuevos servicios o migrar sus suscripciones de SKU que se apagarán finalmente.</span><span class="sxs-lookup"><span data-stu-id="59173-131">In these cases, you may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down.</span></span> <span data-ttu-id="59173-132">La migración de los clientes de SKU retiradas a otras más recientes requiere los siguientes pasos:</span><span class="sxs-lookup"><span data-stu-id="59173-132">Migrating customers from retired SKUs to newer ones requires the following steps:</span></span>

<span data-ttu-id="59173-133">A.</span><span class="sxs-lookup"><span data-stu-id="59173-133">A.</span></span> <span data-ttu-id="59173-134">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="59173-134">Purchase the new subscription</span></span>

<span data-ttu-id="59173-135">B.</span><span class="sxs-lookup"><span data-stu-id="59173-135">B.</span></span> <span data-ttu-id="59173-136">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="59173-136">Reassign current user licenses</span></span>

<span data-ttu-id="59173-137">C.</span><span class="sxs-lookup"><span data-stu-id="59173-137">C.</span></span> <span data-ttu-id="59173-138">Cancelar suscripción anterior</span><span class="sxs-lookup"><span data-stu-id="59173-138">Cancel old subscription</span></span>


## <a name="migrate-your-customers-to-new-plans"></a><span data-ttu-id="59173-139">Migre sus clientes a nuevos planes</span><span class="sxs-lookup"><span data-stu-id="59173-139">Migrate your customers to new plans</span></span>

### <a name="a-purchase-the-new-subscription"></a><span data-ttu-id="59173-140">A.</span><span class="sxs-lookup"><span data-stu-id="59173-140">A.</span></span> <span data-ttu-id="59173-141">Comprar la nueva suscripción</span><span class="sxs-lookup"><span data-stu-id="59173-141">Purchase the new subscription</span></span>

1. <span data-ttu-id="59173-142">Para comprar la nueva suscripción, en el menú del **centro de Partners** , seleccione **clientes**, seleccione el cliente que desea migrar y, a continuación, seleccione **Agregar suscripciones**.</span><span class="sxs-lookup"><span data-stu-id="59173-142">To purchase the new subscription, from the **Partner Center** menu, select **Customers**, select the customer you want to move, and then select **Add subscriptions**.</span></span>

2. <span data-ttu-id="59173-143">Seleccione la suscripción que desea comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, seleccione **submit (enviar**).</span><span class="sxs-lookup"><span data-stu-id="59173-143">Select the subscription you want to purchase from the catalog (in this case, one of the options above), enter the number of licenses, and then select **Submit**.</span></span>

<span data-ttu-id="59173-144">El cliente debería tener ahora suscripciones antiguas y nuevas, la antigua suscripción independiente de Kaizala Pro y la nueva suscripción de destino, por ejemplo, la opción 1-Office 365 Enterprise F1.</span><span class="sxs-lookup"><span data-stu-id="59173-144">Your customer should now have both old and new subscriptions, the old Kaizala Pro Standalone subscription and the new 'target' subscription, for example, Option 1 - Office 365 Enterprise F1.</span></span>

### <a name="b-reassign-current-user-licenses"></a><span data-ttu-id="59173-145">B.</span><span class="sxs-lookup"><span data-stu-id="59173-145">B.</span></span> <span data-ttu-id="59173-146">Reasignar licencias de usuario actuales</span><span class="sxs-lookup"><span data-stu-id="59173-146">Reassign current user licenses</span></span>

1. <span data-ttu-id="59173-147">Para reasignar las licencias de los usuarios del cliente, en el menú del **centro de Partners** , seleccione **clientes**, seleccione el cliente que va a mover y, a continuación, seleccione **usuarios y licencias**.</span><span class="sxs-lookup"><span data-stu-id="59173-147">To reassign the customer's users' licenses, from the **Partner Center** menu, select **Customers**, select the customer you are moving, and then select **Users and licenses**.</span></span> <span data-ttu-id="59173-148">Se abre la página usuarios y licencias del cliente.</span><span class="sxs-lookup"><span data-stu-id="59173-148">The customer's Users and Licenses page opens.</span></span>

2. <span data-ttu-id="59173-149">Para reasignar la licencia de usuario, seleccione el usuario que desea reasignar y, a continuación, seleccione **administrar licencias**.</span><span class="sxs-lookup"><span data-stu-id="59173-149">To reassign user license, select the user to reassign and then select **Manage licenses**.</span></span>

3. <span data-ttu-id="59173-150">En la página **administrar licencias** , desactive la casilla de Kaizala Pro independiente License y seleccione un nuevo plan de servicio para la suscripción a la que se desplaza el cliente.</span><span class="sxs-lookup"><span data-stu-id="59173-150">On the **Manage licenses** page, clear the Kaizala Pro Standalone license check box, and select a new service plan for the subscription the customer is moving to.</span></span>

4.  <span data-ttu-id="59173-151">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="59173-151">Select **Submit**.</span></span> <span data-ttu-id="59173-152">Una página de confirmación enumera las nuevas asignaciones de licencias.</span><span class="sxs-lookup"><span data-stu-id="59173-152">A confirmation page lists the new license assignments.</span></span> <span data-ttu-id="59173-153">Continúe con el mismo proceso para otros usuarios que necesiten asignaciones de licencia.</span><span class="sxs-lookup"><span data-stu-id="59173-153">Continue this same process for other users who need license assignments.</span></span>

### <a name="c-cancel-old-subscription"></a><span data-ttu-id="59173-154">C.</span><span class="sxs-lookup"><span data-stu-id="59173-154">C.</span></span> <span data-ttu-id="59173-155">Cancelar suscripción anterior</span><span class="sxs-lookup"><span data-stu-id="59173-155">Cancel old subscription</span></span>

<span data-ttu-id="59173-156">Después de mover la licencia de usuario al nuevo servicio, puede cancelar con seguridad la suscripción retirada en el nivel de cliente.</span><span class="sxs-lookup"><span data-stu-id="59173-156">After moving the user license to the new service, you can safely cancel the retired subscription at the customer level.</span></span>

1.  <span data-ttu-id="59173-157">En el menú del **centro de Partners** , seleccione **clientes**.</span><span class="sxs-lookup"><span data-stu-id="59173-157">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="59173-158">Seleccione el cliente cuya suscripción va a cancelar.</span><span class="sxs-lookup"><span data-stu-id="59173-158">Select the customer whose subscription you are canceling.</span></span>

2.  <span data-ttu-id="59173-159">En la página de detalles de la suscripción, establezca la suscripción en **Suspended**.</span><span class="sxs-lookup"><span data-stu-id="59173-159">In the subscription detail page, set the subscription to **Suspended**.</span></span>

3.  <span data-ttu-id="59173-160">Seleccione **Submit** (Enviar).</span><span class="sxs-lookup"><span data-stu-id="59173-160">Select **Submit**.</span></span>

<span data-ttu-id="59173-161">Se ha suspendido la suscripción antigua y la nueva suscripción está activa.</span><span class="sxs-lookup"><span data-stu-id="59173-161">The old subscription is suspended, and the new subscription is active.</span></span> <span data-ttu-id="59173-162">La suscripción suspendida se desaprovisionará automáticamente después de 120 días.</span><span class="sxs-lookup"><span data-stu-id="59173-162">The suspended subscription will be de-provisioned automatically after 120 days.</span></span> <span data-ttu-id="59173-163">El cliente no incurre en costos adicionales para la suscripción antigua.</span><span class="sxs-lookup"><span data-stu-id="59173-163">The customer incurs no additional costs for the old subscription.</span></span>
