---
title: Establecer, comprobar o quitar los presupuestos de gastos mensuales de Azure para los clientes del Centro de partners
ms.topic: how-to
ms.date: 03/17/2021
description: Obtenga información acerca de cómo establecer o quitar los presupuestos de gastos mensuales de Azure para los clientes y también ver los datos de gasto de Azure y establecer notificaciones relacionadas con el presupuesto.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eaf54898d7a130ca38e5a2aaeba279fb722c9e66
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712756"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="9021f-103">Establecer, comprobar o quitar los presupuestos de gastos mensuales de Azure para los clientes del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="9021f-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="9021f-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="9021f-104">**Appropriate roles**</span></span>

- <span data-ttu-id="9021f-105">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="9021f-105">Admin agent</span></span>

<span data-ttu-id="9021f-106">Puede [establecer un presupuesto de gasto de Azure mensual para sus clientes en el](#set-azure-spending-budget) centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="9021f-106">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="9021f-107">Esto ayuda a los clientes a administrar sus gastos de Azure.</span><span class="sxs-lookup"><span data-stu-id="9021f-107">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="9021f-108">Esta opción permite comparar el gasto de Azure de los clientes con el presupuesto durante el mes.</span><span class="sxs-lookup"><span data-stu-id="9021f-108">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="9021f-109">También ayuda a los clientes a presupuestar sus gastos de Azure, por lo que su factura mensual no es más alta de lo previsto.</span><span class="sxs-lookup"><span data-stu-id="9021f-109">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="9021f-110">Esta característica no está disponible en las cuentas de espacio aislado o prueba en producción (TIP).</span><span class="sxs-lookup"><span data-stu-id="9021f-110">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="9021f-111">Después de [establecer un presupuesto de gasto de Azure para los clientes](#set-azure-spending-budget), también puede revisar el uso del cliente de las siguientes maneras.</span><span class="sxs-lookup"><span data-stu-id="9021f-111">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="9021f-112">Estas opciones pueden ayudarle a detectar servicios mal configurados o tendencias inusuales que podrían sugerir fraudes.</span><span class="sxs-lookup"><span data-stu-id="9021f-112">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="9021f-113">Después, puede trabajar con los clientes para identificar la causa principal y administrar los costos.</span><span class="sxs-lookup"><span data-stu-id="9021f-113">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="9021f-114">Si es necesario, también puede [cambiar el presupuesto del cliente](#set-azure-spending-budget) a una cantidad mayor.</span><span class="sxs-lookup"><span data-stu-id="9021f-114">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="9021f-115">Comprobar los gastos actuales de Azure</span><span class="sxs-lookup"><span data-stu-id="9021f-115">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="9021f-116">Activar las notificaciones por correo electrónico cuando el gasto del cliente está a punto de su límite de presupuesto</span><span class="sxs-lookup"><span data-stu-id="9021f-116">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="9021f-117">Visualización de los costos inventariados por servicio para las suscripciones basadas en el uso</span><span class="sxs-lookup"><span data-stu-id="9021f-117">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="9021f-118">También puede [quitar un presupuesto de gasto de Azure](#remove-azure-spending-budget) para los clientes en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="9021f-118">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="9021f-119">Datos de gasto de Azure</span><span class="sxs-lookup"><span data-stu-id="9021f-119">Azure spending data</span></span>

<span data-ttu-id="9021f-120">Los datos de gasto de Azure son una *estimación* y los *importes de facturación reales pueden variar*.</span><span class="sxs-lookup"><span data-stu-id="9021f-120">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="9021f-121">El valor de los datos *no refleja* impuestos, créditos, ajustes u otros cargos que puedan aplicarse.</span><span class="sxs-lookup"><span data-stu-id="9021f-121">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="9021f-122">Los datos de gasto se *actualizan una vez al día*.</span><span class="sxs-lookup"><span data-stu-id="9021f-122">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="9021f-123">Los clientes pueden seguir usando (y se le cobrará por) servicios y recursos de Azure, a menos que cambie la configuración de su cuenta en el Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="9021f-123">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="9021f-124">Establecer el presupuesto de gasto de Azure</span><span class="sxs-lookup"><span data-stu-id="9021f-124">Set Azure spending budget</span></span>

<span data-ttu-id="9021f-125">Puede *establecer un presupuesto de gasto de Azure mensual* para varios clientes en el centro de Partners:</span><span class="sxs-lookup"><span data-stu-id="9021f-125">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="9021f-126">Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="9021f-126">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="9021f-127">En el menú de la izquierda, en **CSP**, elija **gasto de Azure**.</span><span class="sxs-lookup"><span data-stu-id="9021f-127">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="9021f-128">En la página **gasto de Azure** , en **clientes con suscripciones de Microsoft Azure**, seleccione los clientes para los que desea establecer un presupuesto.</span><span class="sxs-lookup"><span data-stu-id="9021f-128">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="9021f-129">Escriba un valor para **presupuesto mensual**.</span><span class="sxs-lookup"><span data-stu-id="9021f-129">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="9021f-130">Elija **aplicar** para guardar los cambios.</span><span class="sxs-lookup"><span data-stu-id="9021f-130">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="9021f-131">También puede *establecer un presupuesto para un cliente individual* en su configuración de suscripción:</span><span class="sxs-lookup"><span data-stu-id="9021f-131">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="9021f-132">Inicie sesión en el panel del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="9021f-132">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="9021f-133">En el menú de la izquierda, en **CSP**, elija **clientes**.</span><span class="sxs-lookup"><span data-stu-id="9021f-133">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="9021f-134">En la página **clientes** , seleccione el nombre de la **empresa** del cliente.</span><span class="sxs-lookup"><span data-stu-id="9021f-134">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="9021f-135">En la página **suscripciones** del cliente, en **suscripción basada** en el uso, elija **cambiar presupuesto**.</span><span class="sxs-lookup"><span data-stu-id="9021f-135">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="9021f-136">Escriba un valor para el presupuesto.</span><span class="sxs-lookup"><span data-stu-id="9021f-136">Enter a value for the budget.</span></span>

6. <span data-ttu-id="9021f-137">Elija **aplicar** para guardar los cambios.</span><span class="sxs-lookup"><span data-stu-id="9021f-137">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="9021f-138">Quitar el presupuesto de gasto de Azure</span><span class="sxs-lookup"><span data-stu-id="9021f-138">Remove Azure spending budget</span></span>

<span data-ttu-id="9021f-139">Puede *quitar un presupuesto mensual de gastos de Azure* para los clientes del centro de Partners:</span><span class="sxs-lookup"><span data-stu-id="9021f-139">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="9021f-140">Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="9021f-140">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="9021f-141">En el menú de la izquierda, en **CSP**, elija **gasto de Azure**.</span><span class="sxs-lookup"><span data-stu-id="9021f-141">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="9021f-142">En la página **gasto de Azure** , en **clientes con suscripciones de Microsoft Azure**, seleccione los clientes cuyo presupuesto desea quitar.</span><span class="sxs-lookup"><span data-stu-id="9021f-142">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="9021f-143">Elija **quitar presupuesto**.</span><span class="sxs-lookup"><span data-stu-id="9021f-143">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="9021f-144">Comprobar los gastos actuales de Azure</span><span class="sxs-lookup"><span data-stu-id="9021f-144">Check current Azure spending</span></span>

<span data-ttu-id="9021f-145">Puede *realizar un seguimiento de los gastos mensuales y del gasto actual de Azure* en cualquier momento:</span><span class="sxs-lookup"><span data-stu-id="9021f-145">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="9021f-146">Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="9021f-146">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="9021f-147">En el menú de la izquierda, en **CSP**, elija **gasto de Azure**.</span><span class="sxs-lookup"><span data-stu-id="9021f-147">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="9021f-148">En la página **gasto de Azure** , en **clientes con suscripciones de Microsoft Azure**, puede ver una visión general de los presupuestos mensuales de los clientes, las estimaciones de gastos actuales y el porcentaje de presupuesto usado.</span><span class="sxs-lookup"><span data-stu-id="9021f-148">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="9021f-149">Notificaciones para los límites de presupuesto</span><span class="sxs-lookup"><span data-stu-id="9021f-149">Notifications for budget limits</span></span>

<span data-ttu-id="9021f-150">Puede *activar las notificaciones por correo electrónico* para cuando el gasto mensual del cliente esté cerca del límite de presupuesto.</span><span class="sxs-lookup"><span data-stu-id="9021f-150">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="9021f-151">Al activar esta opción, se le notificará cuando los clientes usen un 80% o más de su presupuesto mensual.</span><span class="sxs-lookup"><span data-stu-id="9021f-151">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="9021f-152">Esta opción le ayuda a estar atento a la factura de Azure.</span><span class="sxs-lookup"><span data-stu-id="9021f-152">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="9021f-153">Para configurar notificaciones por correo electrónico:</span><span class="sxs-lookup"><span data-stu-id="9021f-153">To configure email notifications:</span></span>

1. <span data-ttu-id="9021f-154">Inicie sesión en el Centro de datos.</span><span class="sxs-lookup"><span data-stu-id="9021f-154">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="9021f-155">Vaya a **Configuración**.</span><span class="sxs-lookup"><span data-stu-id="9021f-155">Go to **Settings**.</span></span>

3. <span data-ttu-id="9021f-156">Seleccione **mis preferencias**.</span><span class="sxs-lookup"><span data-stu-id="9021f-156">Select **My preferences**.</span></span>

4. <span data-ttu-id="9021f-157">Si no lo ha hecho, configure una dirección de correo electrónico preferida.</span><span class="sxs-lookup"><span data-stu-id="9021f-157">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="9021f-158">Configure el idioma preferido para la notificación.</span><span class="sxs-lookup"><span data-stu-id="9021f-158">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="9021f-159">Seleccione la pestaña **CSP** en la sección **preferencias de notificación** .</span><span class="sxs-lookup"><span data-stu-id="9021f-159">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="9021f-160">Compruebe la opción de correo electrónico para la notificación de **gasto de Azure** y **guárdela**.</span><span class="sxs-lookup"><span data-stu-id="9021f-160">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="9021f-161">Costos inventariados por servicio</span><span class="sxs-lookup"><span data-stu-id="9021f-161">Itemized costs by service</span></span>

<span data-ttu-id="9021f-162">Puede *ver los costos calculados (y el uso estimado) por servicio para las suscripciones basadas en el uso*:</span><span class="sxs-lookup"><span data-stu-id="9021f-162">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="9021f-163">Inicie sesión en el Centro de datos.</span><span class="sxs-lookup"><span data-stu-id="9021f-163">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="9021f-164">En el menú de la izquierda, en **CSP**, elija **clientes**.</span><span class="sxs-lookup"><span data-stu-id="9021f-164">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="9021f-165">En la página **clientes** , seleccione el nombre de la **empresa** del cliente.</span><span class="sxs-lookup"><span data-stu-id="9021f-165">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="9021f-166">En la página **suscripciones** del cliente, en **suscripciones basadas** en el uso, seleccione el nombre de la **suscripción**.</span><span class="sxs-lookup"><span data-stu-id="9021f-166">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="9021f-167">En la página de la suscripción, puede revisar los **costos** calculados por servicio y el **uso estimado** para el mes en curso.</span><span class="sxs-lookup"><span data-stu-id="9021f-167">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="9021f-168">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="9021f-168">Next steps</span></span>

- [<span data-ttu-id="9021f-169">Nueva experiencia comercial en CSP: facturación de Azure</span><span class="sxs-lookup"><span data-stu-id="9021f-169">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
