---
title: Establecer un presupuesto de gasto de Azure para los clientes
ms.topic: how-to
ms.date: 06/03/2020
description: Obtenga información acerca de cómo establecer o quitar los presupuestos de gastos mensuales de Azure para los clientes y también ver los datos de gasto de Azure y establecer notificaciones relacionadas con el presupuesto.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e311af31bbce65ed38c20df12243d325c7a63d04
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/01/2020
ms.locfileid: "96438984"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a><span data-ttu-id="f888b-103">Establecer, comprobar o quitar los presupuestos de gastos mensuales de Azure para los clientes del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="f888b-103">Set, check, or remove monthly Azure spending budgets for customers in Partner Center</span></span>

<span data-ttu-id="f888b-104">Se aplica a:</span><span class="sxs-lookup"><span data-stu-id="f888b-104">Applies to:</span></span>

- <span data-ttu-id="f888b-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="f888b-105">Partner Center</span></span>
- <span data-ttu-id="f888b-106">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="f888b-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="f888b-107">Puede [establecer un presupuesto de gasto de Azure mensual para sus clientes en el](#set-azure-spending-budget) centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="f888b-107">You can [set a monthly Azure spending budget for your customers](#set-azure-spending-budget) in Partner Center.</span></span> <span data-ttu-id="f888b-108">Esto ayuda a los clientes a administrar sus gastos de Azure.</span><span class="sxs-lookup"><span data-stu-id="f888b-108">This helps your customers manage their Azure spending.</span></span> <span data-ttu-id="f888b-109">Esta opción permite comparar el gasto de Azure de los clientes con el presupuesto durante el mes.</span><span class="sxs-lookup"><span data-stu-id="f888b-109">This option allows you to compare your customers' Azure spending to the budget during the month.</span></span> <span data-ttu-id="f888b-110">También ayuda a los clientes a presupuestar sus gastos de Azure, por lo que su factura mensual no es más alta de lo previsto.</span><span class="sxs-lookup"><span data-stu-id="f888b-110">It also helps your customers to budget their Azure spending so their monthly bill isn't higher than they anticipate.</span></span>

> [!NOTE]  
> <span data-ttu-id="f888b-111">Esta característica no está disponible en las cuentas de espacio aislado o prueba en producción (TIP).</span><span class="sxs-lookup"><span data-stu-id="f888b-111">This feature is not available in sandbox or Test in Production (TIP) accounts.</span></span>

<span data-ttu-id="f888b-112">Después de [establecer un presupuesto de gasto de Azure para los clientes](#set-azure-spending-budget), también puede revisar el uso del cliente de las siguientes maneras.</span><span class="sxs-lookup"><span data-stu-id="f888b-112">After you [set an Azure spending budget for your customer(s)](#set-azure-spending-budget), you can also review customer usage in the following ways.</span></span> <span data-ttu-id="f888b-113">Estas opciones pueden ayudarle a detectar servicios mal configurados o tendencias inusuales que podrían sugerir fraudes.</span><span class="sxs-lookup"><span data-stu-id="f888b-113">These options may help you spot misconfigured services or unusual trends that might suggest fraud.</span></span> <span data-ttu-id="f888b-114">Después, puede trabajar con los clientes para identificar la causa principal y administrar los costos.</span><span class="sxs-lookup"><span data-stu-id="f888b-114">You can then work with your customer(s) to identify the root cause and manage costs.</span></span> <span data-ttu-id="f888b-115">Si es necesario, también puede [cambiar el presupuesto del cliente](#set-azure-spending-budget) a una cantidad mayor.</span><span class="sxs-lookup"><span data-stu-id="f888b-115">If necessary, you can also [change the customer's budget](#set-azure-spending-budget) to a higher amount.</span></span>

- [<span data-ttu-id="f888b-116">Comprobar los gastos actuales de Azure</span><span class="sxs-lookup"><span data-stu-id="f888b-116">Check current Azure spending</span></span>](#check-current-azure-spending)

- [<span data-ttu-id="f888b-117">Activar las notificaciones por correo electrónico cuando el gasto del cliente está a punto de su límite de presupuesto</span><span class="sxs-lookup"><span data-stu-id="f888b-117">Turn on email notifications for when a customer's spending is nearing their budget limit</span></span>](#notifications-for-budget-limits)

- [<span data-ttu-id="f888b-118">Visualización de los costos inventariados por servicio para las suscripciones basadas en el uso</span><span class="sxs-lookup"><span data-stu-id="f888b-118">View itemized costs by service for usage-based subscriptions</span></span>](#itemized-costs-by-service)

<span data-ttu-id="f888b-119">También puede [quitar un presupuesto de gasto de Azure](#remove-azure-spending-budget) para los clientes en cualquier momento.</span><span class="sxs-lookup"><span data-stu-id="f888b-119">You can also [remove an Azure spending budget](#remove-azure-spending-budget) for customer(s) at any time.</span></span>

## <a name="azure-spending-data"></a><span data-ttu-id="f888b-120">Datos de gasto de Azure</span><span class="sxs-lookup"><span data-stu-id="f888b-120">Azure spending data</span></span>

<span data-ttu-id="f888b-121">Los datos de gasto de Azure son una *estimación* y los *importes de facturación reales pueden variar*.</span><span class="sxs-lookup"><span data-stu-id="f888b-121">The Azure spending data is an *estimate* and *actual billing amounts may vary*.</span></span> <span data-ttu-id="f888b-122">El valor de los datos *no refleja* impuestos, créditos, ajustes u otros cargos que puedan aplicarse.</span><span class="sxs-lookup"><span data-stu-id="f888b-122">The data's value *doesn't reflect* taxes, credits, adjustments, or other charges that may apply.</span></span>

<span data-ttu-id="f888b-123">Los datos de gasto se *actualizan una vez al día*.</span><span class="sxs-lookup"><span data-stu-id="f888b-123">The spending data is *refreshed once per day*.</span></span> <span data-ttu-id="f888b-124">Los clientes pueden seguir usando (y se le cobrará por) servicios y recursos de Azure, a menos que cambie la configuración de su cuenta en el Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="f888b-124">Your customers can continue to use (and be charged for) Azure services and resources, unless you change their account settings in the Azure portal.</span></span>

## <a name="set-azure-spending-budget"></a><span data-ttu-id="f888b-125">Establecer el presupuesto de gasto de Azure</span><span class="sxs-lookup"><span data-stu-id="f888b-125">Set Azure spending budget</span></span>

<span data-ttu-id="f888b-126">Puede *establecer un presupuesto de gasto de Azure mensual* para varios clientes en el centro de Partners:</span><span class="sxs-lookup"><span data-stu-id="f888b-126">You can *set a monthly Azure spending budget* for multiple customers in Partner Center:</span></span>

1. <span data-ttu-id="f888b-127">Inicie sesión en el [panel del centro de Partners](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="f888b-127">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="f888b-128">En el menú de la izquierda, en **CSP**, elija **gasto de Azure**.</span><span class="sxs-lookup"><span data-stu-id="f888b-128">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="f888b-129">En la página **gasto de Azure** , en **clientes con suscripciones de Microsoft Azure**, seleccione los clientes para los que desea establecer un presupuesto.</span><span class="sxs-lookup"><span data-stu-id="f888b-129">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) for whom you want to set a budget.</span></span>

4. <span data-ttu-id="f888b-130">Escriba un valor para **presupuesto mensual**.</span><span class="sxs-lookup"><span data-stu-id="f888b-130">Enter a value for **Monthly budget**.</span></span>

5. <span data-ttu-id="f888b-131">Elija **aplicar** para guardar los cambios.</span><span class="sxs-lookup"><span data-stu-id="f888b-131">Choose **Apply** to save your changes.</span></span>

<span data-ttu-id="f888b-132">También puede *establecer un presupuesto para un cliente individual* en su configuración de suscripción:</span><span class="sxs-lookup"><span data-stu-id="f888b-132">You can also *set a budget for an individual customer* in their subscription settings:</span></span>

1. <span data-ttu-id="f888b-133">Inicia sesión en el panel del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="f888b-133">Sign in to the Partner Center dashboard.</span></span>

2. <span data-ttu-id="f888b-134">En el menú de la izquierda, en **CSP**, elija **clientes**.</span><span class="sxs-lookup"><span data-stu-id="f888b-134">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="f888b-135">En la página **clientes** , seleccione el nombre de la **empresa** del cliente.</span><span class="sxs-lookup"><span data-stu-id="f888b-135">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="f888b-136">En la página **suscripciones** del cliente, en **suscripción basada** en el uso, elija **cambiar presupuesto**.</span><span class="sxs-lookup"><span data-stu-id="f888b-136">On the customer's **Subscriptions** page, under **Usage-based subscription**, choose **Change budget**.</span></span>

5. <span data-ttu-id="f888b-137">Escriba un valor para el presupuesto.</span><span class="sxs-lookup"><span data-stu-id="f888b-137">Enter a value for the budget.</span></span>

6. <span data-ttu-id="f888b-138">Elija **aplicar** para guardar los cambios.</span><span class="sxs-lookup"><span data-stu-id="f888b-138">Choose **Apply** to save your changes.</span></span>

## <a name="remove-azure-spending-budget"></a><span data-ttu-id="f888b-139">Quitar el presupuesto de gasto de Azure</span><span class="sxs-lookup"><span data-stu-id="f888b-139">Remove Azure spending budget</span></span>

<span data-ttu-id="f888b-140">Puede *quitar un presupuesto mensual de gastos de Azure* para los clientes del centro de Partners:</span><span class="sxs-lookup"><span data-stu-id="f888b-140">You can *remove a monthly Azure spending budget* for your customer(s) in Partner Center:</span></span>

1. <span data-ttu-id="f888b-141">Inicie sesión en el [panel del centro de Partners](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="f888b-141">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="f888b-142">En el menú de la izquierda, en **CSP**, elija **gasto de Azure**.</span><span class="sxs-lookup"><span data-stu-id="f888b-142">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="f888b-143">En la página **gasto de Azure** , en **clientes con suscripciones de Microsoft Azure**, seleccione los clientes cuyo presupuesto desea quitar.</span><span class="sxs-lookup"><span data-stu-id="f888b-143">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, select the customer(s) whose budget you want to remove.</span></span>

4. <span data-ttu-id="f888b-144">Elija **quitar presupuesto**.</span><span class="sxs-lookup"><span data-stu-id="f888b-144">Choose **Remove budget**.</span></span>

## <a name="check-current-azure-spending"></a><span data-ttu-id="f888b-145">Comprobar los gastos actuales de Azure</span><span class="sxs-lookup"><span data-stu-id="f888b-145">Check current Azure spending</span></span>

<span data-ttu-id="f888b-146">Puede *realizar un seguimiento de los gastos mensuales y del gasto actual de Azure* en cualquier momento:</span><span class="sxs-lookup"><span data-stu-id="f888b-146">You can *track your customers' current Azure spending and monthly budgets* at any time:</span></span>

1. <span data-ttu-id="f888b-147">Inicie sesión en el [panel del centro de Partners](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="f888b-147">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="f888b-148">En el menú de la izquierda, en **CSP**, elija **gasto de Azure**.</span><span class="sxs-lookup"><span data-stu-id="f888b-148">In the left-hand menu under **CSP**, choose **Azure spending**.</span></span>

3. <span data-ttu-id="f888b-149">En la página **gasto de Azure** , en **clientes con suscripciones de Microsoft Azure**, puede ver una visión general de los presupuestos mensuales de los clientes, las estimaciones de gastos actuales y el porcentaje de presupuesto usado.</span><span class="sxs-lookup"><span data-stu-id="f888b-149">On the **Azure spending** page, under **Customers with Microsoft Azure subscriptions**, you can see an overview of customers' monthly budgets, current spending estimates and percentage of budget used.</span></span>

## <a name="notifications-for-budget-limits"></a><span data-ttu-id="f888b-150">Notificaciones para los límites de presupuesto</span><span class="sxs-lookup"><span data-stu-id="f888b-150">Notifications for budget limits</span></span>

<span data-ttu-id="f888b-151">Puede *activar las notificaciones por correo electrónico* para cuando el gasto mensual del cliente esté cerca del límite de presupuesto.</span><span class="sxs-lookup"><span data-stu-id="f888b-151">You can *turn on email notifications* for when your customer's monthly spending is nearing their budget limit.</span></span> <span data-ttu-id="f888b-152">Al activar esta opción, se le notificará cuando los clientes usen un 80% o más de su presupuesto mensual.</span><span class="sxs-lookup"><span data-stu-id="f888b-152">When you turn on this option, you will be notified when customers use 80% or more of their monthly budget.</span></span> <span data-ttu-id="f888b-153">Esta opción le ayuda a estar atento a la factura de Azure.</span><span class="sxs-lookup"><span data-stu-id="f888b-153">This option helps you can keep an eye on your Azure bill.</span></span> <span data-ttu-id="f888b-154">Para configurar notificaciones por correo electrónico:</span><span class="sxs-lookup"><span data-stu-id="f888b-154">To configure email notifications:</span></span>

1. <span data-ttu-id="f888b-155">Inicie sesión en el Centro de datos.</span><span class="sxs-lookup"><span data-stu-id="f888b-155">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="f888b-156">Vaya a **Configuración**.</span><span class="sxs-lookup"><span data-stu-id="f888b-156">Go to **Settings**.</span></span>

3. <span data-ttu-id="f888b-157">Seleccione **mis preferencias**.</span><span class="sxs-lookup"><span data-stu-id="f888b-157">Select **My preferences**.</span></span>

4. <span data-ttu-id="f888b-158">Si no lo ha hecho, configure una dirección de correo electrónico preferida.</span><span class="sxs-lookup"><span data-stu-id="f888b-158">Configure a preferred email address if you haven't.</span></span>

5. <span data-ttu-id="f888b-159">Configure el idioma preferido para la notificación.</span><span class="sxs-lookup"><span data-stu-id="f888b-159">Configure the preferred language for the notification.</span></span>

6. <span data-ttu-id="f888b-160">Seleccione la pestaña **CSP** en la sección **preferencias de notificación** .</span><span class="sxs-lookup"><span data-stu-id="f888b-160">Select **CSP** tab under **Notification preferences** section.</span></span>

7. <span data-ttu-id="f888b-161">Compruebe la opción de correo electrónico para la notificación de **gasto de Azure** y **guárdela**.</span><span class="sxs-lookup"><span data-stu-id="f888b-161">Check the Email option for **Azure Spending** notification, and **Save**.</span></span>


## <a name="itemized-costs-by-service"></a><span data-ttu-id="f888b-162">Costos inventariados por servicio</span><span class="sxs-lookup"><span data-stu-id="f888b-162">Itemized costs by service</span></span>

<span data-ttu-id="f888b-163">Puede *ver los costos calculados (y el uso estimado) por servicio para las suscripciones basadas en el uso*:</span><span class="sxs-lookup"><span data-stu-id="f888b-163">You can *view itemized costs (and estimated usage) by service for usage-based subscriptions*:</span></span>

1. <span data-ttu-id="f888b-164">Inicie sesión en el Centro de datos.</span><span class="sxs-lookup"><span data-stu-id="f888b-164">Sign in to Partner Center.</span></span>

2. <span data-ttu-id="f888b-165">En el menú de la izquierda, en **CSP**, elija **clientes**.</span><span class="sxs-lookup"><span data-stu-id="f888b-165">In the left-hand menu under **CSP**, choose **Customers**.</span></span>

3. <span data-ttu-id="f888b-166">En la página **clientes** , seleccione el nombre de la **empresa** del cliente.</span><span class="sxs-lookup"><span data-stu-id="f888b-166">On the **Customers** page, select the customer's **Company name**.</span></span>

4. <span data-ttu-id="f888b-167">En la página **suscripciones** del cliente, en **suscripciones basadas** en el uso, seleccione el nombre de la **suscripción**.</span><span class="sxs-lookup"><span data-stu-id="f888b-167">On the customer's **Subscriptions** page, under **Usage-based subscriptions**, select the name of the **Subscription**.</span></span>

5. <span data-ttu-id="f888b-168">En la página de la suscripción, puede revisar los **costos** calculados por servicio y el **uso estimado** para el mes en curso.</span><span class="sxs-lookup"><span data-stu-id="f888b-168">On the subscription's page, you can review the **Itemized costs** by service, and the **Estimated usage** for the current month.</span></span>
