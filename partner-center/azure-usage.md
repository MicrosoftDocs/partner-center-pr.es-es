---
title: Cambio de tamaño de máquina virtual de Azure para usar la máxima reserva
ms.topic: how-to
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Obtenga información acerca de cómo cambiar el tamaño de una máquina virtual (VM) a las necesidades informáticas de sus clientes al comprar Microsoft Azure reservas para ellas.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: bc9fc14598e7c96f9cc1b55eba7c59af68ad84a9
ms.sourcegitcommit: b79504dbfc335aca995f370e15a654829acdaaff
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/06/2020
ms.locfileid: "87900108"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="66da3-103">Cambio de tamaño de VM de Microsoft Azure para el uso de reserva máximo</span><span class="sxs-lookup"><span data-stu-id="66da3-103">Microsoft Azure VM sizing for maximum reservation usage</span></span>

<span data-ttu-id="66da3-104">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="66da3-104">**Applies to**</span></span>

- <span data-ttu-id="66da3-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="66da3-105">Partner Center</span></span>
- <span data-ttu-id="66da3-106">Azure portal</span><span class="sxs-lookup"><span data-stu-id="66da3-106">Azure portal</span></span>
- <span data-ttu-id="66da3-107">Partners del programa CSP</span><span class="sxs-lookup"><span data-stu-id="66da3-107">Partners in the CSP program</span></span>
 
> [!NOTE]
> <span data-ttu-id="66da3-108">Este artículo se aplica únicamente a los asociados del programa proveedor de soluciones en la nube (CSP).</span><span class="sxs-lookup"><span data-stu-id="66da3-108">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="66da3-109">Los clientes que usen otros tipos de suscripciones (como, por ejemplo, pago por uso, individuo, contrato de cliente de Microsoft o suscripciones Contrato Enterprise), en su lugar, deberán leer [esta documentación](https://docs.microsoft.com/azure/cost-management-billing/reservations)de las reservas de Azure.</span><span class="sxs-lookup"><span data-stu-id="66da3-109">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="66da3-110">Determinar el tamaño de la máquina virtual para la reserva de Azure de un cliente</span><span class="sxs-lookup"><span data-stu-id="66da3-110">Determine the VM size for a customer's Azure reservation</span></span>

<span data-ttu-id="66da3-111">Al comprar Microsoft Azure reservas en nombre de sus clientes, deberá elegir un tamaño de máquina virtual (VM) para satisfacer las necesidades informáticas del cliente.</span><span class="sxs-lookup"><span data-stu-id="66da3-111">When buying Microsoft Azure reservations on behalf of your customers, you'll need to choose a virtual machine (VM) sized to meet the customer's computing needs.</span></span> <span data-ttu-id="66da3-112">Puede encontrar esta información mediante uno de estos métodos:</span><span class="sxs-lookup"><span data-stu-id="66da3-112">You can find this information using one of these methods:</span></span>

- <span data-ttu-id="66da3-113">API de uso de Azure</span><span class="sxs-lookup"><span data-stu-id="66da3-113">Azure utilization API</span></span>
- <span data-ttu-id="66da3-114">El Portal de Azure</span><span class="sxs-lookup"><span data-stu-id="66da3-114">The Azure portal</span></span>
- <span data-ttu-id="66da3-115">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="66da3-115">Azure PowerShell</span></span>
- <span data-ttu-id="66da3-116">La API de Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="66da3-116">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="66da3-117">A continuación se proporcionan instrucciones para usar cada uno de estos métodos.</span><span class="sxs-lookup"><span data-stu-id="66da3-117">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="66da3-118">Después de comprar una reserva, el descuento de la reserva se aplica automáticamente a las máquinas virtuales que coinciden con los atributos y la cantidad de la reserva.</span><span class="sxs-lookup"><span data-stu-id="66da3-118">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="66da3-119">No es necesario asignar la reserva a una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="66da3-119">You don't need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="66da3-120">Los descuentos de reserva no se aplican a las máquinas virtuales de promoción o clásicas.</span><span class="sxs-lookup"><span data-stu-id="66da3-120">Reservation discounts don't apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="66da3-121">Para identificar correctamente el tipo y el tamaño de la máquina virtual que se va a comprar en nombre de su cliente, debe usar uno de los métodos descritos a continuación, ya que el tipo de serie de la máquina virtual no se muestra correctamente en los archivos de conciliación del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="66da3-121">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a><span data-ttu-id="66da3-122">Obtención de información de tamaño de la máquina virtual mediante la API de uso de Azure</span><span class="sxs-lookup"><span data-stu-id="66da3-122">Get VM sizing information using the Azure utilization API</span></span>

1. <span data-ttu-id="66da3-123">Use el valor para el atributo ServiceType de additionalInfo en la respuesta de la API para identificar el tamaño de la máquina virtual que se va a comprar.</span><span class="sxs-lookup"><span data-stu-id="66da3-123">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span>

2. <span data-ttu-id="66da3-124">Para obtener más información, consulte [obtención de los registros de uso de un cliente para Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) en la [API del centro de Partners](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="66da3-124">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a><span data-ttu-id="66da3-125">Obtención de información de tamaño de la máquina virtual mediante el Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="66da3-125">Get VM sizing information using the Microsoft Azure portal</span></span>

1. <span data-ttu-id="66da3-126">En el centro de Partners, vaya a la página de **clientes** .</span><span class="sxs-lookup"><span data-stu-id="66da3-126">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="66da3-127">Busque el cliente que desea comprar reservas de máquinas virtuales de Azure y, después, seleccione la flecha abajo para expandir la información del cliente.</span><span class="sxs-lookup"><span data-stu-id="66da3-127">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="66da3-128">Seleccione **portal de administración de Microsoft Azure** para abrir el registro del cliente en el Azure portal.</span><span class="sxs-lookup"><span data-stu-id="66da3-128">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>

3. <span data-ttu-id="66da3-129">Seleccione **máquinas virtuales** en el menú del portal y, a continuación, seleccione la máquina virtual para la que desea comprar una reserva.</span><span class="sxs-lookup"><span data-stu-id="66da3-129">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span>

4. <span data-ttu-id="66da3-130">En la página de detalles de la máquina virtual, busque la información de tamaño y región, como se muestra a continuación, y use esta información para comprar la reserva en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="66da3-130">On the VM's detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

   :::image type="content" source="images/usage1.png" alt-text="Información de tamaño y región en la página de detalles":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a><span data-ttu-id="66da3-132">Obtención de información de tamaño de máquina virtual mediante Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="66da3-132">Get VM sizing information using Microsoft Azure PowerShell</span></span>

<span data-ttu-id="66da3-133">Use la información de la imagen siguiente para obtener la ubicación y el tamaño de la máquina virtual para la que desea comprar una reserva.</span><span class="sxs-lookup"><span data-stu-id="66da3-133">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

:::image type="content" source="images/usage2.png" alt-text="Ubicación y tamaño de la máquina virtual":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a><span data-ttu-id="66da3-135">Obtención de información de tamaño de la máquina virtual mediante la API de Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="66da3-135">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>

1. <span data-ttu-id="66da3-136">Con las API de ARMClient o ARM, llame al cliente de ARM para la máquina virtual para la que desea comprar una reserva.</span><span class="sxs-lookup"><span data-stu-id="66da3-136">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2. <span data-ttu-id="66da3-137">/subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? API-version = 2017-12-01</span><span class="sxs-lookup"><span data-stu-id="66da3-137">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3. <span data-ttu-id="66da3-138">La llamada devuelve los valores de **vmSize** y **Location**, como se muestra a continuación.</span><span class="sxs-lookup"><span data-stu-id="66da3-138">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    :::image type="content" source="images/usage3.png" alt-text="valor vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="valor de ubicación":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="66da3-141">Comprobación del uso de VM de Azure y el descuento de reserva</span><span class="sxs-lookup"><span data-stu-id="66da3-141">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="66da3-142">Después de comprar una instancia reservada de máquina virtual de Azure en nombre de un cliente, el descuento por pagar por el espacio de máquina virtual de antemano se aplica automáticamente a las máquinas virtuales que coinciden con los atributos y la cantidad de la reserva del cliente.</span><span class="sxs-lookup"><span data-stu-id="66da3-142">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer's reservation.</span></span>

<span data-ttu-id="66da3-143">Puede comprobar el uso de la reserva del cliente y ver a qué máquinas virtuales se aplican los descuentos de reserva mediante uno de los métodos siguientes:</span><span class="sxs-lookup"><span data-stu-id="66da3-143">You can verify the customer's reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>

- <span data-ttu-id="66da3-144">El Portal de Azure</span><span class="sxs-lookup"><span data-stu-id="66da3-144">The Azure portal</span></span>
- <span data-ttu-id="66da3-145">API de uso de Azure</span><span class="sxs-lookup"><span data-stu-id="66da3-145">Azure utilization API</span></span>

<span data-ttu-id="66da3-146">A continuación se proporcionan instrucciones para usar cada uno de estos métodos.</span><span class="sxs-lookup"><span data-stu-id="66da3-146">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="66da3-147">Solo la API de uso de Azure muestra la máquina virtual a la que se aplica el descuento.</span><span class="sxs-lookup"><span data-stu-id="66da3-147">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="66da3-148">Compruebe el uso de la reserva del cliente en el Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="66da3-148">Verify the customer's reservation usage in the Microsoft Azure portal</span></span>

1. <span data-ttu-id="66da3-149">En el centro de Partners, vaya a la página de **clientes** .</span><span class="sxs-lookup"><span data-stu-id="66da3-149">In Partner Center, go to your **Customers** page.</span></span>

2. <span data-ttu-id="66da3-150">Busque el cliente cuyo descuento de reserva y el uso desea comprobar y, a continuación, seleccione la flecha abajo para expandir la información del cliente.</span><span class="sxs-lookup"><span data-stu-id="66da3-150">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer's information.</span></span> <span data-ttu-id="66da3-151">Seleccione **portal de administración de Microsoft Azure** para abrir el registro del cliente en el Azure portal.</span><span class="sxs-lookup"><span data-stu-id="66da3-151">Select **Microsoft Azure Management Portal** to open the customer's record in the Azure portal.</span></span>
3. <span data-ttu-id="66da3-152">Seleccione **reservas** en el menú del portal y, a continuación, seleccione la reserva para la que desea comprobar el uso.</span><span class="sxs-lookup"><span data-stu-id="66da3-152">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span>
4. <span data-ttu-id="66da3-153">En la página **información general** , compruebe el gráfico de uso de la reserva, que muestra la cantidad de reserva que se aplicó a las máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="66da3-153">On the **Overview** page check the reservation's utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span>

    >[!NOTE]
    ><span data-ttu-id="66da3-154">Los datos de uso se pueden retrasar hasta 8 horas.</span><span class="sxs-lookup"><span data-stu-id="66da3-154">Utilization data may be delayed by up to 8 hours.</span></span>

    <span data-ttu-id="66da3-155">a.</span><span class="sxs-lookup"><span data-stu-id="66da3-155">a.</span></span> <span data-ttu-id="66da3-156">Si el uso de la reserva es del 100%, el cliente obtiene todos los ahorros posibles que puede proporcionar la compra de reserva.</span><span class="sxs-lookup"><span data-stu-id="66da3-156">If the reservation's utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span>
    <span data-ttu-id="66da3-157">b.</span><span class="sxs-lookup"><span data-stu-id="66da3-157">b.</span></span> <span data-ttu-id="66da3-158">Si el uso de la reserva es 0%, el descuento no se aplica a ninguna máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="66da3-158">If the reservation's usage is 0%, the discount is not being applied to any virtual machine.</span></span>
    <span data-ttu-id="66da3-159">c.</span><span class="sxs-lookup"><span data-stu-id="66da3-159">c.</span></span> <span data-ttu-id="66da3-160">Si el uso de la reserva está entre 1% y 99%, hay ventajas no utilizadas.</span><span class="sxs-lookup"><span data-stu-id="66da3-160">If the reservation's usage is between 1% and 99%, there are unused benefits.</span></span>

5. <span data-ttu-id="66da3-161">Para evitar esta situación, determine el tamaño correcto de la máquina virtual para satisfacer las necesidades informáticas de los clientes antes de hacer la compra.</span><span class="sxs-lookup"><span data-stu-id="66da3-161">To avoid this situation, determine the correct size VM to support the customer's computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="66da3-162">Comprobación del uso de la reserva del cliente con la API de uso de Azure</span><span class="sxs-lookup"><span data-stu-id="66da3-162">Verify the customer's reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="66da3-163">Solo la API de uso de Azure muestra la máquina virtual a la que se aplica el descuento.</span><span class="sxs-lookup"><span data-stu-id="66da3-163">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="66da3-164">Puede obtener datos de uso de reserva con la API de uso de Azure para comprobar que el cliente está obteniendo el descuento de reserva y ver a qué máquinas virtuales (máquinas virtuales) se aplica el descuento.</span><span class="sxs-lookup"><span data-stu-id="66da3-164">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="66da3-165">Compare el ejemplo a con el ejemplo B para ver cómo comprobar el uso de la reserva de un cliente.</span><span class="sxs-lookup"><span data-stu-id="66da3-165">Compare Example A to Example B to see how to verify a customer's reservation usage.</span></span>

:::image type="content" source="images/usage5.png" alt-text="Ejemplos de uso de reserva":::

- <span data-ttu-id="66da3-167">ReservationId identifica la reserva de Azure que se usó para aplicar el descuento a la máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="66da3-167">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
- <span data-ttu-id="66da3-168">consumptionMeter es el MeterId de la máquina virtual que tiene aplicado el descuento de reserva.</span><span class="sxs-lookup"><span data-stu-id="66da3-168">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
- <span data-ttu-id="66da3-169">El ReservationMeter muestra el costo $0 desde que se aplicó el descuento de reserva.</span><span class="sxs-lookup"><span data-stu-id="66da3-169">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span>

<span data-ttu-id="66da3-170">Para obtener más información, consulte [obtención de los registros de uso de un cliente para Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) en la [API del centro de Partners](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="66da3-170">For more information, see [Get a customer's utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="66da3-171">Los costos de software, como Microsoft Windows Server, no se incluyen actualmente en el precio de una reserva de máquinas virtuales y aparecerán como elementos de línea independientes en el registro de pedidos y en la factura.</span><span class="sxs-lookup"><span data-stu-id="66da3-171">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="66da3-172">Sin embargo, si un cliente tiene la ventaja de uso híbrido de Azure, no se aplicarán los costos de software.</span><span class="sxs-lookup"><span data-stu-id="66da3-172">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="66da3-173">Para obtener más información, consulte [los costos de software de Windows no incluidos con las instancias reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="66da3-173">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="66da3-174">Recursos de reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="66da3-174">Azure reservations resources</span></span>

|<span data-ttu-id="66da3-175">**Para información acerca de**</span><span class="sxs-lookup"><span data-stu-id="66da3-175">**For information about**</span></span>   |<span data-ttu-id="66da3-176">**Lee esto**</span><span class="sxs-lookup"><span data-stu-id="66da3-176">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="66da3-177">Información general sobre las reservas de Azure en CSP</span><span class="sxs-lookup"><span data-stu-id="66da3-177">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="66da3-178">Vender Microsoft Azure instancias reservadas de máquina virtual</span><span class="sxs-lookup"><span data-stu-id="66da3-178">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="66da3-179">Compra de reservas de Azure para sus clientes en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="66da3-179">Purchasing Azure reservations for your customers in Partner Center</span></span>   | [<span data-ttu-id="66da3-180">Comprar reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="66da3-180">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="66da3-181">Administración de las reservas de Azure en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="66da3-181">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="66da3-182">Administración de las reservas de Azure en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="66da3-182">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="66da3-183">Compra de reservas de Azure en el Azure Portal</span><span class="sxs-lookup"><span data-stu-id="66da3-183">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="66da3-184">[Pagar por adelantado máquinas virtuales con Azure Reserved VM instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) en la ayuda de Azure</span><span class="sxs-lookup"><span data-stu-id="66da3-184">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="66da3-185">Administración de las reservas de Azure en el Azure Portal</span><span class="sxs-lookup"><span data-stu-id="66da3-185">Managing Azure reservations in the Azure portal</span></span>   | <span data-ttu-id="66da3-186">[Administración de instancias reservadas de máquina virtual](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) en la ayuda de Azure</span><span class="sxs-lookup"><span data-stu-id="66da3-186">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="66da3-187">Compra de reservas de Azure mediante la API del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="66da3-187">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="66da3-188">[Comprar Azure Reserved VM instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) en la documentación para desarrolladores del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="66da3-188">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="66da3-189">Otorgar permiso a los clientes para comprar sus propias reservas de Azure a partir de una suscripción que haya adquirido.</span><span class="sxs-lookup"><span data-stu-id="66da3-189">Giving customers permission to buy their own Azure reservations from a subscription you purchased for them.</span></span> | [<span data-ttu-id="66da3-190">Conceder permiso a los clientes para que compren sus propias reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="66da3-190">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
