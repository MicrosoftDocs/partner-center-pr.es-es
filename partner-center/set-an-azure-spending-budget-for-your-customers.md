---
title: Establecer, comprobar o quitar los presupuestos de gastos mensuales de Azure para los clientes del Centro de partners
ms.topic: how-to
ms.date: 03/17/2021
description: Aprenda a establecer o quitar presupuestos de gasto mensuales de Azure para los clientes, así como a ver los datos de gasto de Azure y a establecer notificaciones relacionadas con el presupuesto.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855359"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="bd3f0-103">Establecer, comprobar o quitar los presupuestos de gastos mensuales de Azure para los clientes de Centro de partners</span><span class="sxs-lookup"><span data-stu-id="bd3f0-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="bd3f0-104">**Roles adecuados:** Agente de administración</span><span class="sxs-lookup"><span data-stu-id="bd3f0-104">**Appropriate roles**: Admin agent</span></span>

<span data-ttu-id="bd3f0-105">Puede establecer [un presupuesto de gasto mensual de Azure para los clientes](#set-azure-spending-budget) en Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-105">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="bd3f0-106">Esto ayuda a los clientes a administrar sus gastos de Azure.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-106">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="bd3f0-107">Esta opción le permite comparar los gastos de Azure de los clientes con el presupuesto durante el mes.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-107">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="bd3f0-108">También ayuda a los clientes a presupuestar sus gastos de Azure para que su factura mensual no sea mayor de lo previsto.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-108">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="bd3f0-109">Esta característica no está disponible en cuentas de espacio aislado o prueba en producción (TIP).</span><span class="sxs-lookup"><span data-stu-id="bd3f0-109">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="bd3f0-110">Después de [establecer un presupuesto de gastos de Azure](#set-azure-spending-budget)para los clientes, también puede revisar el uso de los clientes de las maneras siguientes.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-110">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="bd3f0-111">Estas opciones pueden ayudarle a detectar servicios mal configurados o tendencias inusuales que podrían sugerir fraudes.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-111">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="bd3f0-112">A continuación, puede trabajar con los clientes para identificar la causa principal y administrar los costos.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-112">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="bd3f0-113">Si es necesario, también puede [cambiar el presupuesto del](#set-azure-spending-budget) cliente a una cantidad mayor.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-113">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="bd3f0-114">Comprobación de los gastos actuales de Azure</span><span class="sxs-lookup"><span data-stu-id="bd3f0-114">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="bd3f0-115">Activar las notificaciones por correo electrónico cuando el gasto de un cliente se acerca a su límite de presupuesto</span><span class="sxs-lookup"><span data-stu-id="bd3f0-115">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="bd3f0-116">Visualización de los costos por servicio por servicio para suscripciones basadas en el uso</span><span class="sxs-lookup"><span data-stu-id="bd3f0-116">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="bd3f0-117">También puede quitar [un presupuesto de gastos de Azure](#remove-azure-spending-budget) para los clientes en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-117">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="bd3f0-118">Datos de gasto de Azure</span><span class="sxs-lookup"><span data-stu-id="bd3f0-118">Azure spending data</span></span>

<span data-ttu-id="bd3f0-119">Los datos de gasto de Azure son *una estimación* y *los importes de facturación reales pueden variar.*</span><span class="sxs-lookup"><span data-stu-id="bd3f0-119">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="bd3f0-120">El valor de los datos *no refleja los* impuestos, créditos, ajustes u otros cargos que se puedan aplicar.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-120">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="bd3f0-121">Los datos de gasto *se actualizan una vez al día.*</span><span class="sxs-lookup"><span data-stu-id="bd3f0-121">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="bd3f0-122">Los clientes pueden seguir usando (y se les cobrará por) los servicios y recursos de Azure, a menos que cambie la configuración de su cuenta en el Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-122">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="bd3f0-123">Establecer el presupuesto de gastos de Azure</span><span class="sxs-lookup"><span data-stu-id="bd3f0-123">Set Azure spending budget</span></span>

<span data-ttu-id="bd3f0-124">Puede establecer *un presupuesto mensual de gastos de Azure* para varios clientes en Centro de partners:</span><span class="sxs-lookup"><span data-stu-id="bd3f0-124">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="bd3f0-125">Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="bd3f0-125">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="bd3f0-126">En el menú izquierdo de **CSP,** elija **Gastos de Azure.**</span><span class="sxs-lookup"><span data-stu-id="bd3f0-126">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="bd3f0-127">En la **página de gastos** de Azure, en Clientes con **Microsoft Azure suscripciones,** seleccione los clientes para los que desea establecer un presupuesto.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-127">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="bd3f0-128">Escriba un valor para **Presupuesto mensual.**</span><span class="sxs-lookup"><span data-stu-id="bd3f0-128">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="bd3f0-129">Elija **Aplicar** para guardar los cambios.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-129">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="bd3f0-130">También puede establecer *un presupuesto para un cliente individual en* su configuración de suscripción:</span><span class="sxs-lookup"><span data-stu-id="bd3f0-130">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="bd3f0-131">Inicie sesión en el panel del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-131">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="bd3f0-132">En el menú izquierdo de **CSP,** elija **Clientes.**</span><span class="sxs-lookup"><span data-stu-id="bd3f0-132">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="bd3f0-133">En la **página** Clientes, seleccione el nombre de la compañía **del cliente.**</span><span class="sxs-lookup"><span data-stu-id="bd3f0-133">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="bd3f0-134">En la página Suscripciones **del** cliente, en Suscripción basada en **uso,** elija **Cambiar presupuesto.**</span><span class="sxs-lookup"><span data-stu-id="bd3f0-134">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="bd3f0-135">Escriba un valor para el presupuesto.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-135">Enter a value for the budget.</span></span>

6. <span data-ttu-id="bd3f0-136">Elija **Aplicar** para guardar los cambios.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-136">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="bd3f0-137">Eliminación del presupuesto de gastos de Azure</span><span class="sxs-lookup"><span data-stu-id="bd3f0-137">Remove Azure spending budget</span></span>

<span data-ttu-id="bd3f0-138">Puede quitar *un presupuesto mensual de gastos de Azure* para los clientes en Centro de partners:</span><span class="sxs-lookup"><span data-stu-id="bd3f0-138">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="bd3f0-139">Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="bd3f0-139">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="bd3f0-140">En el menú izquierdo de **CSP,** elija **Gastos de Azure.**</span><span class="sxs-lookup"><span data-stu-id="bd3f0-140">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="bd3f0-141">En la **página Gastos** de Azure, en Clientes **con Microsoft Azure suscripciones,** seleccione los clientes cuyo presupuesto desea quitar.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-141">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="bd3f0-142">Elija **Quitar presupuesto.**</span><span class="sxs-lookup"><span data-stu-id="bd3f0-142">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="bd3f0-143">Comprobación de los gastos actuales de Azure</span><span class="sxs-lookup"><span data-stu-id="bd3f0-143">Check current Azure spending</span></span>

<span data-ttu-id="bd3f0-144">Puede realizar *un seguimiento de los gastos actuales* de Azure de los clientes y los presupuestos mensuales en cualquier momento:</span><span class="sxs-lookup"><span data-stu-id="bd3f0-144">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="bd3f0-145">Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="bd3f0-145">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="bd3f0-146">En el menú izquierdo de **CSP,** elija **Gastos de Azure.**</span><span class="sxs-lookup"><span data-stu-id="bd3f0-146">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="bd3f0-147">En la página de gastos de **Azure,** en Clientes con suscripciones Microsoft Azure **,** puede ver información general sobre los presupuestos mensuales de los clientes, las estimaciones de gasto actuales y el porcentaje de presupuesto usado.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-147">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="bd3f0-148">Notificaciones de límites de presupuesto</span><span class="sxs-lookup"><span data-stu-id="bd3f0-148">Notifications for budget limits</span></span>

<span data-ttu-id="bd3f0-149">Puede activar *las notificaciones por correo electrónico* cuando el gasto mensual del cliente esté cerca de su límite de presupuesto.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-149">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="bd3f0-150">Al activar esta opción, se le notificará cuando los clientes usen el 80 % o más de su presupuesto mensual.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-150">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="bd3f0-151">Esta opción le ayuda a mantenerse al tanto de la factura de Azure.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-151">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="bd3f0-152">Para configurar notificaciones por correo electrónico:</span><span class="sxs-lookup"><span data-stu-id="bd3f0-152">To configure email notifications:</span></span>

1. <span data-ttu-id="bd3f0-153">Inicie sesión en el Centro de datos.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-153">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="bd3f0-154">Vaya a **Configuración**.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-154">Go to **Settings**.</span></span>

3. <span data-ttu-id="bd3f0-155">Seleccione **Mis preferencias.**</span><span class="sxs-lookup"><span data-stu-id="bd3f0-155">Select **My preferences**.</span></span>

4. <span data-ttu-id="bd3f0-156">Configure una dirección de correo electrónico preferida si no lo ha hecho.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-156">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="bd3f0-157">Configure el idioma preferido para la notificación.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-157">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="bd3f0-158">Seleccione la **pestaña CSP** en la **sección Preferencias de** notificación.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-158">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="bd3f0-159">Active la opción Correo electrónico para **la notificación de gasto** de Azure y **Guarde**.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-159">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="bd3f0-160">Costos por servicio por elemento</span><span class="sxs-lookup"><span data-stu-id="bd3f0-160">Itemized costs by service</span></span>

<span data-ttu-id="bd3f0-161">Puede ver *los costos por elemento (y el uso estimado) por servicio para las suscripciones basadas en el uso:*</span><span class="sxs-lookup"><span data-stu-id="bd3f0-161">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="bd3f0-162">Inicie sesión en el Centro de datos.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-162">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="bd3f0-163">En el menú izquierdo de **CSP,** elija **Clientes.**</span><span class="sxs-lookup"><span data-stu-id="bd3f0-163">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="bd3f0-164">En la **página Clientes,** seleccione el nombre de la **compañía del cliente.**</span><span class="sxs-lookup"><span data-stu-id="bd3f0-164">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="bd3f0-165">En la página Suscripciones **del** cliente, en Suscripciones basadas en **uso,** seleccione el nombre de la **suscripción**.</span><span class="sxs-lookup"><span data-stu-id="bd3f0-165">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="bd3f0-166">En la página de la suscripción, puede revisar los costos por servicio y el Uso estimado **del** mes actual. </span><span class="sxs-lookup"><span data-stu-id="bd3f0-166">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>


## <a name="next-steps"></a><span data-ttu-id="bd3f0-167">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="bd3f0-167">Next steps</span></span>

- [<span data-ttu-id="bd3f0-168">Nueva experiencia comercial en CSP: facturación de Azure</span><span class="sxs-lookup"><span data-stu-id="bd3f0-168">New commerce experience in CSP - Azure billing</span></span>](azure-plan-billing.md)
