---
title: Cambio de tamaño de máquina virtual de Azure para usar la máxima reserva
description: Obtenga información sobre cómo cambiar el tamaño de una máquina virtual (VM) a las necesidades informáticas de los clientes al comprar Microsoft Azure reservas para ellos.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 650618de7460f4667c60ac58cbe6716530db7f16
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510200"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="663e6-103">Cambio de tamaño de VM de Microsoft Azure para el uso de reserva máximo</span><span class="sxs-lookup"><span data-stu-id="663e6-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="663e6-104">**Roles adecuados:** agente de administración | Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="663e6-104">**Appropriate roles**: Admin agent | Sales agent</span></span>

<span data-ttu-id="663e6-105">En este artículo se explica cómo cambiar el tamaño de una máquina virtual (VM) a las necesidades informáticas de los clientes al comprar Microsoft Azure reservas para ellos.</span><span class="sxs-lookup"><span data-stu-id="663e6-105">This article explains how to size a virtual machine (VM) to your customers' computing needs when you buy Microsoft Azure reservations for them.</span></span>
 
> [!NOTE]
> <span data-ttu-id="663e6-106">Este artículo solo se aplica a los asociados del programa Proveedor de soluciones en la nube (CSP).</span><span class="sxs-lookup"><span data-stu-id="663e6-106">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="663e6-107">Los clientes que usan otros tipos de suscripciones (por ejemplo, suscripciones de pago por [uso,](/azure/cost-management-billing/reservations)individuales, Contrato de cliente de Microsoft o Enterprise Agreement) deben leer en su lugar esta documentación de reservas de Azure .</span><span class="sxs-lookup"><span data-stu-id="663e6-107">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="663e6-108">Determinación del tamaño de máquina virtual de la reserva de Azure de un cliente</span><span class="sxs-lookup"><span data-stu-id="663e6-108">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="663e6-109">Al comprar Microsoft Azure reservas en nombre de los clientes, deberá elegir una máquina virtual (VM) de tamaño para satisfacer las necesidades informáticas del cliente.</span><span class="sxs-lookup"><span data-stu-id="663e6-109">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="663e6-110">Puede encontrar esta información mediante uno de estos métodos:</span><span class="sxs-lookup"><span data-stu-id="663e6-110">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="663e6-111">API de uso de Azure</span><span class="sxs-lookup"><span data-stu-id="663e6-111">Azure utilization API</span></span>
- <span data-ttu-id="663e6-112">El Portal de Azure</span><span class="sxs-lookup"><span data-stu-id="663e6-112">The Azure portal</span></span>
- <span data-ttu-id="663e6-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="663e6-113">Azure PowerShell</span></span>
- <span data-ttu-id="663e6-114">The Azure Resource Manager (ARM) API</span><span class="sxs-lookup"><span data-stu-id="663e6-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="663e6-115">A continuación se proporcionan instrucciones para usar cada uno de estos métodos.</span><span class="sxs-lookup"><span data-stu-id="663e6-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="663e6-116">Después de comprar una reserva, el descuento por reserva se aplica automáticamente a las máquinas virtuales que coinciden con los atributos y la cantidad de la reserva.</span><span class="sxs-lookup"><span data-stu-id="663e6-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="663e6-117">No es necesario asignar la reserva a una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="663e6-117">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="663e6-118">Los descuentos de reserva no se aplican a las máquinas virtuales clásicas o promocionales.</span><span class="sxs-lookup"><span data-stu-id="663e6-118">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="663e6-119">Para identificar correctamente el tipo y el tamaño de la máquina virtual que se va a comprar en nombre del cliente, debe usar uno de los métodos que se describen a continuación, ya que el tipo de serie de máquina virtual no se muestra correctamente en Centro de partners de conciliación.</span><span class="sxs-lookup"><span data-stu-id="663e6-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="663e6-120">Obtener información de tamaño de máquina virtual mediante la API de uso de Azure</span><span class="sxs-lookup"><span data-stu-id="663e6-120">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="663e6-121">Use el valor del atributo ServiceType de additionalInfo en la respuesta de la API para identificar el tamaño de máquina virtual que se debe comprar.</span><span class="sxs-lookup"><span data-stu-id="663e6-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="663e6-122">Para obtener más información, consulte [Obtener los registros de](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) uso de un cliente para Azure en Centro de partners [API](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="663e6-122">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="663e6-123">Obtener información de tamaño de máquina virtual mediante Microsoft Azure portal</span><span class="sxs-lookup"><span data-stu-id="663e6-123">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="663e6-124">En Centro de partners, vaya a la **página** Clientes.</span><span class="sxs-lookup"><span data-stu-id="663e6-124">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="663e6-125">Busque el cliente que quiere comprar reservas de máquinas virtuales de Azure y, a continuación, seleccione la flecha abajo para expandir la información del cliente.</span><span class="sxs-lookup"><span data-stu-id="663e6-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="663e6-126">Seleccione **Microsoft Azure Portal de administración** para abrir el registro del cliente en el Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="663e6-126">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="663e6-127">Seleccione **Máquinas virtuales en** el menú del portal y, a continuación, seleccione la máquina virtual para la que quiere comprar una reserva.</span><span class="sxs-lookup"><span data-stu-id="663e6-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="663e6-128">En la página de detalles de la máquina virtual, busque la información de tamaño y región, como se muestra a continuación, y use esta información para comprar la reserva en Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="663e6-128">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Información de tamaño y región en la página de detalles.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="663e6-130">Obtener información de tamaño de máquina virtual mediante Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="663e6-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="663e6-131">Use la información de la imagen siguiente para obtener la ubicación y el tamaño de la máquina virtual para la que desea comprar una reserva.</span><span class="sxs-lookup"><span data-stu-id="663e6-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Ubicación y tamaño de la máquina virtual.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="663e6-133">Obtener información de tamaño de máquina virtual mediante la API Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="663e6-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="663e6-134">Con ARMClient o las API de ARM, llame al cliente de ARM para la máquina virtual para la que desea comprar una reserva.</span><span class="sxs-lookup"><span data-stu-id="663e6-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. <span data-ttu-id="663e6-135">La llamada devuelve los valores de **vmSize** y **location**, como se muestra a continuación.</span><span class="sxs-lookup"><span data-stu-id="663e6-135">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="Valor de vmSize.":::
    :::image type="content" source="images/usage4.png" alt-text="valor de ubicación.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="663e6-138">Comprobación del uso de máquinas virtuales de Azure y el descuento por reserva</span><span class="sxs-lookup"><span data-stu-id="663e6-138">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="663e6-139">Después de comprar una instancia reservada de máquina virtual de Azure en nombre de un cliente, el descuento por pagar por el espacio de máquina virtual por adelantado se aplica automáticamente a las máquinas virtuales que coinciden con los atributos y la cantidad de la reserva del cliente.</span><span class="sxs-lookup"><span data-stu-id="663e6-139">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="663e6-140">Puede comprobar el uso de reservas del cliente y ver a qué máquinas virtuales se aplican los descuentos de reserva mediante uno de los métodos siguientes:</span><span class="sxs-lookup"><span data-stu-id="663e6-140">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="663e6-141">El Portal de Azure</span><span class="sxs-lookup"><span data-stu-id="663e6-141">The Azure portal</span></span>
- <span data-ttu-id="663e6-142">API de uso de Azure</span><span class="sxs-lookup"><span data-stu-id="663e6-142">Azure utilization API</span></span>

<span data-ttu-id="663e6-143">A continuación se proporcionan instrucciones para usar cada uno de estos métodos.</span><span class="sxs-lookup"><span data-stu-id="663e6-143">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="663e6-144">Solo la API de uso de Azure muestra a qué máquina virtual se aplica el descuento.</span><span class="sxs-lookup"><span data-stu-id="663e6-144">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="663e6-145">Comprobación del uso de reservas del cliente en el portal Microsoft Azure cliente</span><span class="sxs-lookup"><span data-stu-id="663e6-145">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="663e6-146">En Centro de partners, vaya a la **página** Clientes.</span><span class="sxs-lookup"><span data-stu-id="663e6-146">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="663e6-147">Busque el cliente cuyo descuento y uso de reserva desea comprobar y, a continuación, seleccione la flecha abajo para expandir la información del cliente.</span><span class="sxs-lookup"><span data-stu-id="663e6-147">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="663e6-148">Seleccione **Microsoft Azure Portal de administración** para abrir el registro del cliente en el Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="663e6-148">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="663e6-149">Seleccione **Reservas en el** menú del portal y, a continuación, seleccione la reserva para la que desea comprobar el uso.</span><span class="sxs-lookup"><span data-stu-id="663e6-149">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="663e6-150">En la **página Información** general, compruebe el gráfico de uso de la reserva, que muestra la cantidad de la reserva que se aplicó a las máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="663e6-150">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="663e6-151">Los datos de uso pueden retrasarse hasta 8 horas.</span><span class="sxs-lookup"><span data-stu-id="663e6-151">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="663e6-152">a.</span><span class="sxs-lookup"><span data-stu-id="663e6-152">a.</span></span> <span data-ttu-id="663e6-153">Si el uso de la reserva es del 100 %, el cliente está obteniendo todos los ahorros posibles que puede proporcionar la compra de reserva.</span><span class="sxs-lookup"><span data-stu-id="663e6-153">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="663e6-154">b.</span><span class="sxs-lookup"><span data-stu-id="663e6-154">b.</span></span> <span data-ttu-id="663e6-155">Si el uso de la reserva es del 0 %, el descuento no se aplica a ninguna máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="663e6-155">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="663e6-156">c.</span><span class="sxs-lookup"><span data-stu-id="663e6-156">c.</span></span> <span data-ttu-id="663e6-157">Si el uso de la reserva está entre el 1 % y el 99 %, hay ventajas no utilizadas.</span><span class="sxs-lookup"><span data-stu-id="663e6-157">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="663e6-158">Para evitar esta situación, determine el tamaño correcto de la máquina virtual para satisfacer las necesidades informáticas del cliente antes de realizar la compra.</span><span class="sxs-lookup"><span data-stu-id="663e6-158">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="663e6-159">Comprobación del uso de reservas del cliente con la API de uso de Azure</span><span class="sxs-lookup"><span data-stu-id="663e6-159">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="663e6-160">Solo la API de uso de Azure muestra a qué máquina virtual se aplica el descuento.</span><span class="sxs-lookup"><span data-stu-id="663e6-160">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="663e6-161">Puede obtener datos de uso de reservas con la API de uso de Azure para comprobar que el cliente obtiene el descuento de reserva y para ver a qué máquinas virtuales (máquinas virtuales) se aplica el descuento.</span><span class="sxs-lookup"><span data-stu-id="663e6-161">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="663e6-162">Compare el ejemplo A con el ejemplo B para ver cómo comprobar el uso de reservas de un cliente.</span><span class="sxs-lookup"><span data-stu-id="663e6-162">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Ejemplos de uso de reservas.":::

- <span data-ttu-id="663e6-164">ReservationId identifica la reserva de Azure que se usó para aplicar el descuento a la máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="663e6-164">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="663e6-165">consumptionMeter es el MeterId de la máquina virtual que tiene aplicado el descuento de reserva.</span><span class="sxs-lookup"><span data-stu-id="663e6-165">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="663e6-166">ReservationMeter muestra un costo de 0 USD desde que se aplicó el descuento de reserva.</span><span class="sxs-lookup"><span data-stu-id="663e6-166">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="663e6-167">Para obtener más información, consulte [Obtener los registros de](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) uso de un cliente para Azure en Centro de partners [API](/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="663e6-167">For more information, see [Get a customer's utilization records for Azure](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="663e6-168">Los costos de software, como Microsoft Windows Server, no se incluyen actualmente en el precio de una reserva de máquina virtual y aparecerán como elementos de línea independientes en el registro de pedido y en la factura.</span><span class="sxs-lookup"><span data-stu-id="663e6-168">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="663e6-169">Sin embargo, si un cliente tiene la Ventaja de uso híbrido de Azure, no se aplicarán los costos de software.</span><span class="sxs-lookup"><span data-stu-id="663e6-169">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="663e6-170">Para obtener más información, [vea Windows costos de software no incluidos con instancias reservadas.](/azure/billing/billing-reserved-instance-windows-software-costs)</span><span class="sxs-lookup"><span data-stu-id="663e6-170">For more information, see [Windows software costs not included with Reserved Instances](/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="next-steps"></a><span data-ttu-id="663e6-171">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="663e6-171">Next steps</span></span>

|<span data-ttu-id="663e6-172">**Para información acerca de**</span><span class="sxs-lookup"><span data-stu-id="663e6-172">**For information about**</span></span>   |<span data-ttu-id="663e6-173">**Lee esto**</span><span class="sxs-lookup"><span data-stu-id="663e6-173">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="663e6-174">Introducción a las reservas de Azure en CSP</span><span class="sxs-lookup"><span data-stu-id="663e6-174">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="663e6-175">Vender Microsoft Azure instancias reservadas de máquina virtual</span><span class="sxs-lookup"><span data-stu-id="663e6-175">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="663e6-176">Compra de reservas de Azure para los clientes en Centro de partners</span><span class="sxs-lookup"><span data-stu-id="663e6-176">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="663e6-177">Compra de reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="663e6-177">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="663e6-178">Administración de reservas de Azure en Centro de partners</span><span class="sxs-lookup"><span data-stu-id="663e6-178">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="663e6-179">Administración de reservas de Azure en Centro de partners</span><span class="sxs-lookup"><span data-stu-id="663e6-179">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="663e6-180">Compra de reservas de Azure en la Azure Portal</span><span class="sxs-lookup"><span data-stu-id="663e6-180">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="663e6-181">[Pago por adelantado de máquinas virtuales con Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) en la Ayuda de Azure</span><span class="sxs-lookup"><span data-stu-id="663e6-181">[Prepay for virtual machines with Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="663e6-182">Administración de reservas de Azure en el Azure Portal</span><span class="sxs-lookup"><span data-stu-id="663e6-182">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="663e6-183">[Administración de instancias reservadas de máquina virtual](/azure/billing/billing-manage-reserved-vm-instance) en la Ayuda de Azure</span><span class="sxs-lookup"><span data-stu-id="663e6-183">[Manage reserved VM instances](/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="663e6-184">Compra de reservas de Azure mediante Centro de partners API</span><span class="sxs-lookup"><span data-stu-id="663e6-184">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="663e6-185">[Comprar Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) en la documentación Centro de partners desarrolladores</span><span class="sxs-lookup"><span data-stu-id="663e6-185">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="663e6-186">Conceder a los clientes permiso para comprar sus propias reservas de Azure en una suscripción que haya adquirido para ellos.</span><span class="sxs-lookup"><span data-stu-id="663e6-186">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="663e6-187">Conceder a los clientes permiso para comprar sus propias reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="663e6-187">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |