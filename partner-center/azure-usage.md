---
title: Cambio de tamaño de VM de Azure de Microsoft para el uso máximo de reserva | Panel de partners
Description: Information on purchasing and managing Azure reservations
author: v-petand
keywords: azure, reservas, vm, administrar, uso, cambio de tamaño
ms.localizationpriority: medium
ms.openlocfilehash: bb7d022ba45462db313a9f4e16cc47e4550dbef6
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/31/2018
ms.locfileid: "2875785"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="2f74c-103">Cambio de tamaño de la VM de Microsoft Azure para el uso máximo de reserva</span><span class="sxs-lookup"><span data-stu-id="2f74c-103">Microsoft Azure VM sizing for maximum reservation usage</span></span> 

**<span data-ttu-id="2f74c-104">Se aplica a</span><span class="sxs-lookup"><span data-stu-id="2f74c-104">Applies to</span></span>**

-  <span data-ttu-id="2f74c-105">Panel de partners</span><span class="sxs-lookup"><span data-stu-id="2f74c-105">Partner dashboard</span></span>
-  <span data-ttu-id="2f74c-106">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="2f74c-106">Azure portal</span></span>
-  <span data-ttu-id="2f74c-107">Partners de CSP</span><span class="sxs-lookup"><span data-stu-id="2f74c-107">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="2f74c-108">Determinar el tamaño de la máquina virtual para la reserva de Azure de un cliente</span><span class="sxs-lookup"><span data-stu-id="2f74c-108">Determine the VM size for a customer’s Azure reservation</span></span> 

<span data-ttu-id="2f74c-109">Al comprar reservas de Microsoft Azure en nombre de tus clientes, deberás elegir una máquina virtual (VM) con el tamaño adecuado para satisfacer las necesidades informáticas del cliente.</span><span class="sxs-lookup"><span data-stu-id="2f74c-109">When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.</span></span> <span data-ttu-id="2f74c-110">Encontrarás esta información usando uno de estos métodos:</span><span class="sxs-lookup"><span data-stu-id="2f74c-110">You can find this information using one of these methods:</span></span>

-   <span data-ttu-id="2f74c-111">API Azure Utilization</span><span class="sxs-lookup"><span data-stu-id="2f74c-111">Azure utilization API</span></span>
-   <span data-ttu-id="2f74c-112">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="2f74c-112">The Azure portal</span></span>
-   <span data-ttu-id="2f74c-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="2f74c-113">Azure PowerShell</span></span>
-   <span data-ttu-id="2f74c-114">La API de Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="2f74c-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="2f74c-115">A continuación, encontrarás instrucciones para cada uno de estos métodos.</span><span class="sxs-lookup"><span data-stu-id="2f74c-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="2f74c-116">Después de comprar una reserva, el descuento de reserva se aplicará automáticamente a las máquinas virtuales que coincidan con los atributos y la cantidad de la reserva.</span><span class="sxs-lookup"><span data-stu-id="2f74c-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="2f74c-117">No es necesario asignar la reserva a una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="2f74c-117">You don’t need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="2f74c-118">Los descuentos de reserva no se aplican a máquinas virtuales clásicas o promocionales.</span><span class="sxs-lookup"><span data-stu-id="2f74c-118">Reservation discounts don’t apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="2f74c-119">Para identificar correctamente el tipo y el tamaño de la máquina virtual que se debe comprar en nombre del cliente, debes usar uno de los métodos que se describen a continuación ya que el tipo de serie de la máquina virtual no se muestra correctamente en los archivos de conciliación del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="2f74c-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>


**<span data-ttu-id="2f74c-120">Obtener información de cambio de tamaño de máquina virtual con la API Azure Utilization</span><span class="sxs-lookup"><span data-stu-id="2f74c-120">Get VM sizing information using the Azure utilization API</span></span>**

1.  <span data-ttu-id="2f74c-121">Usa el valor del atributo ServiceType de additionalInfo en la respuesta de la API para identificar el tamaño de la máquina virtual que se comprará.</span><span class="sxs-lookup"><span data-stu-id="2f74c-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span> 

2.  <span data-ttu-id="2f74c-122">Para obtener más información, consulta [obtener los registros de uso de un cliente de Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) en el [panel de partners API](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="2f74c-122">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner dashboard API](https://docs.microsoft.com/partner-center/develop/).</span></span> 

**<span data-ttu-id="2f74c-123">Obtener información de cambio de tamaño de máquina virtual con el portal de Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="2f74c-123">Get VM sizing information using the Microsoft Azure portal</span></span>**

1.  <span data-ttu-id="2f74c-124">En el panel de partners, ve a la página de **los clientes** .</span><span class="sxs-lookup"><span data-stu-id="2f74c-124">In your Partner dashboard, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="2f74c-125">Encuentra al cliente que quiera comprar reservas de VM de Azure y, a continuación, selecciona la flecha abajo para expandir la información del cliente.</span><span class="sxs-lookup"><span data-stu-id="2f74c-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="2f74c-126">Selecciona **Portal de administración de Microsoft Azure** para abrir el registro del cliente en el Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="2f74c-126">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="2f74c-127">Selecciona **Máquinas virtuales** en el menú del portal y, a continuación, la máquina virtual para la que quieras comprar una reserva.</span><span class="sxs-lookup"><span data-stu-id="2f74c-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span> 

4.  <span data-ttu-id="2f74c-128">En la página de detalles de la VM, encuentra la información de tamaño y región, como se muestra a continuación, y usa esta información para comprar la reserva en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="2f74c-128">On the VM’s detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![](images/usage1.png)

**<span data-ttu-id="2f74c-129">Obtener información de cambio de tamaño de VM con el Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="2f74c-129">Get VM sizing information using Microsoft Azure PowerShell</span></span>**

<span data-ttu-id="2f74c-130">Usa la información de la imagen siguiente para obtener la ubicación y el tamaño de la VM para la que quieres comprar una reserva.</span><span class="sxs-lookup"><span data-stu-id="2f74c-130">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![](images/usage2.png)

**<span data-ttu-id="2f74c-131">Obtener información de cambio de tamaño de VM con la API de Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="2f74c-131">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>**

1.  <span data-ttu-id="2f74c-132">Con ARMClient o las API de ARM, llama al cliente de ARM para la VM para la que quieres comprar una reserva.</span><span class="sxs-lookup"><span data-stu-id="2f74c-132">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2.  <span data-ttu-id="2f74c-133">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="2f74c-133">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3.  <span data-ttu-id="2f74c-134">La llamada devuelve los valores de **vmSize** y **ubicación**, como se muestra a continuación.</span><span class="sxs-lookup"><span data-stu-id="2f74c-134">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    ![](images/usage3.png)
    ![](images/usage4.png)
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="2f74c-135">Comprobar descuento de reserva y uso de la VM de Azure</span><span class="sxs-lookup"><span data-stu-id="2f74c-135">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="2f74c-136">Después de adquirir una instancia de VM reservada de Azure en nombre de un cliente, el descuento de pagar por adelantado el espacio de la VM se aplica automáticamente a las máquinas virtuales que coinciden con los atributos y la cantidad de la reserva del cliente.</span><span class="sxs-lookup"><span data-stu-id="2f74c-136">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer’s reservation.</span></span> 

<span data-ttu-id="2f74c-137">Puedes comprobar el uso de la reserva del cliente y ver a qué máquinas virtuales se aplican los descuentos de reserva mediante uno de los siguientes métodos:</span><span class="sxs-lookup"><span data-stu-id="2f74c-137">You can verify the customer’s reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>   

-   <span data-ttu-id="2f74c-138">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="2f74c-138">The Azure portal</span></span>
-   <span data-ttu-id="2f74c-139">API Azure Utilization</span><span class="sxs-lookup"><span data-stu-id="2f74c-139">Azure utilization API</span></span>

<span data-ttu-id="2f74c-140">A continuación, encontrarás instrucciones para cada uno de estos métodos.</span><span class="sxs-lookup"><span data-stu-id="2f74c-140">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="2f74c-141">Solo la API Azure Utilization muestra a qué máquina virtual se está aplicando el descuento.</span><span class="sxs-lookup"><span data-stu-id="2f74c-141">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="2f74c-142">Comprobar el uso de reserva del cliente en el portal de Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="2f74c-142">Verify the customer’s reservation usage in the Microsoft Azure portal</span></span>

1.  <span data-ttu-id="2f74c-143">En el panel de partners, ve a la página de **los clientes** .</span><span class="sxs-lookup"><span data-stu-id="2f74c-143">In your Partner dashboard, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="2f74c-144">Encuentra al cliente del que quieres comprar el uso y el descuento de la reserva y, a continuación, selecciona la flecha abajo para expandir la información del cliente.</span><span class="sxs-lookup"><span data-stu-id="2f74c-144">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="2f74c-145">Selecciona **Portal de administración de Microsoft Azure** para abrir el registro del cliente en el portal de Azure.</span><span class="sxs-lookup"><span data-stu-id="2f74c-145">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="2f74c-146">Selecciona **Reservas** en el menú del portal y, a continuación, la reserva para la que quieras comprobar el uso.</span><span class="sxs-lookup"><span data-stu-id="2f74c-146">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span> 

4.  <span data-ttu-id="2f74c-147">En la página **Introducción**, comprueba el gráfico de uso de la reserva, que muestra la cantidad de la reserva aplicada a máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="2f74c-147">On the **Overview** page check the reservation’s utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span> 

    >[!NOTE]
    ><span data-ttu-id="2f74c-148">Los datos de uso se pueden retrasar hasta un máximo de 8 horas.</span><span class="sxs-lookup"><span data-stu-id="2f74c-148">Utilization data may be delayed by up to 8 hours.</span></span>
    
    <span data-ttu-id="2f74c-149">a.</span><span class="sxs-lookup"><span data-stu-id="2f74c-149">a.</span></span>  <span data-ttu-id="2f74c-150">Si el uso de la reserva es 100%, el cliente obtiene el posible ahorro que la compra de la reserva pueda proporcionar.</span><span class="sxs-lookup"><span data-stu-id="2f74c-150">If the reservation’s utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span> 
    
    <span data-ttu-id="2f74c-151">b.</span><span class="sxs-lookup"><span data-stu-id="2f74c-151">b.</span></span>  <span data-ttu-id="2f74c-152">Si el uso de la reserva es del 0%, el descuento no se está aplicando a ninguna máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="2f74c-152">If the reservation’s usage is 0%, the discount is not being applied to any virtual machine.</span></span> 
    
    <span data-ttu-id="2f74c-153">c.</span><span class="sxs-lookup"><span data-stu-id="2f74c-153">c.</span></span>  <span data-ttu-id="2f74c-154">Si el uso de la reserva es de entre el 1 y el 99%, hay ventajas que no se emplean.</span><span class="sxs-lookup"><span data-stu-id="2f74c-154">If the reservation’s usage is between 1% and 99%, there are unused benefits.</span></span> 

5.  <span data-ttu-id="2f74c-155">Para evitar esta situación, determina la VM de tamaño correcto para admitir las necesidades informáticas del cliente antes de realizar la compra.</span><span class="sxs-lookup"><span data-stu-id="2f74c-155">To avoid this situation, determine the correct size VM to support the customer’s computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="2f74c-156">Comprobar el uso de reserva del cliente con la API Azure Utilization</span><span class="sxs-lookup"><span data-stu-id="2f74c-156">Verify the customer’s reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="2f74c-157">Solo la Azure utilization API muestra a qué máquina virtual se está aplicando el descuento.</span><span class="sxs-lookup"><span data-stu-id="2f74c-157">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="2f74c-158">Puedes obtener datos de uso de reserva con la API Azure Utilization para comprobar que el cliente está obteniendo el descuento de la reserva y para ver a qué VM (máquinas virtuales) se aplica el descuento.</span><span class="sxs-lookup"><span data-stu-id="2f74c-158">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="2f74c-159">Compara el ejemplo A con el ejemplo B para ver cómo comprobar el uso de reserva de un cliente.</span><span class="sxs-lookup"><span data-stu-id="2f74c-159">Compare Example A to Example B to see how to verify a customer’s reservation usage.</span></span> 

![](images\usage5.png)

-   <span data-ttu-id="2f74c-160">El reservationId identifica la reserva de Azure que se usó para aplicar el descuento a la VM.</span><span class="sxs-lookup"><span data-stu-id="2f74c-160">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
-   <span data-ttu-id="2f74c-161">consumptionMeter es el MeterId para la VM que tiene el descuento de reserva aplicado.</span><span class="sxs-lookup"><span data-stu-id="2f74c-161">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
-   <span data-ttu-id="2f74c-162">El ReservationMeter muestra un costo de 0$ desde que se aplicó el descuento de reserva.</span><span class="sxs-lookup"><span data-stu-id="2f74c-162">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span> 

<span data-ttu-id="2f74c-163">Para obtener más información, consulta [Obtener los registros de uso de un cliente para Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) en la [API del Centro de partners](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="2f74c-163">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="2f74c-164">Los costes de software, como Microsoft Windows Server, no se incluyen actualmente en el precio de una reserva de VM y aparecerán como elementos de línea independientes en el registro de pedido y en tu factura.</span><span class="sxs-lookup"><span data-stu-id="2f74c-164">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="2f74c-165">Sin embargo, si el cliente dispone de la Ventaja de uso híbrido de Microsoft Azure, no se aplicarán los costos de software.</span><span class="sxs-lookup"><span data-stu-id="2f74c-165">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="2f74c-166">Para obtener más información, consulta [Costos de software de Windows no incluidos con las instancias reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="2f74c-166">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="2f74c-167">Recursos de Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="2f74c-167">Azure reservations resources</span></span>
|**<span data-ttu-id="2f74c-168">Para obtener información acerca de</span><span class="sxs-lookup"><span data-stu-id="2f74c-168">For information about</span></span>**   |**<span data-ttu-id="2f74c-169">Lee esto</span><span class="sxs-lookup"><span data-stu-id="2f74c-169">Read this</span></span>**    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="2f74c-170">Reservas de Azure en introducción de CSP</span><span class="sxs-lookup"><span data-stu-id="2f74c-170">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="2f74c-171">Vender Microsoft Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="2f74c-171">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="2f74c-172">Comprar reservas de Azure para tus clientes en el panel de partners</span><span class="sxs-lookup"><span data-stu-id="2f74c-172">Purchasing Azure reservations for your customers in your Partner dashboard</span></span>   |[<span data-ttu-id="2f74c-173">Comprar reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="2f74c-173">Buy Azure reservations</span></span>](azure-reservations-buying.md)
| <span data-ttu-id="2f74c-174">Administración de Azure reservations en el panel de partners</span><span class="sxs-lookup"><span data-stu-id="2f74c-174">Managing Azure reservations in your Partner dashboard</span></span> | [<span data-ttu-id="2f74c-175">Administración de Azure reservations en el panel de partners</span><span class="sxs-lookup"><span data-stu-id="2f74c-175">Managing Azure reservations in your Partner dashboard</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="2f74c-176">Comprar Azure Reservations en el Azure Portal</span><span class="sxs-lookup"><span data-stu-id="2f74c-176">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="2f74c-177">[Pagar por adelantado máquinas virtuales con instancias reservadas de máquina virtual](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) en la Ayuda de Azure</span><span class="sxs-lookup"><span data-stu-id="2f74c-177">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="2f74c-178">Administración de Azure Reservations en el Azure Portal</span><span class="sxs-lookup"><span data-stu-id="2f74c-178">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="2f74c-179">[Administración de instancias reservadas de máquina virtual](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) en la Ayuda de Azure</span><span class="sxs-lookup"><span data-stu-id="2f74c-179">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="2f74c-180">Comprar Azure Reservations con la API del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="2f74c-180">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="2f74c-181">[Purchase Azure Reserved VM Instances (Comprar Azure Reserved VM Instances)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) en la documentación de desarrolladores del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="2f74c-181">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>



