---
title: Cambio de tamaño de VM de Microsoft Azure para uso máximo de reserva | El centro de partners
ms.topic: article
ms.date: 10/29/2018
Description: When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.
author: v-petand
ms.author: v-petand
keywords: azure, reservas, vm, administrar, uso, cambio de tamaño
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 344eb01f363c7a79ca27082e3eeb1531889f134b
ms.sourcegitcommit: 15d8b6de2b8a4c7d01852f5ed3603338d4281b00
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/17/2019
ms.locfileid: "9014822"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="0128a-103">Cambio de tamaño de la VM de Microsoft Azure para el uso máximo de reserva</span><span class="sxs-lookup"><span data-stu-id="0128a-103">Microsoft Azure VM sizing for maximum reservation usage</span></span> 

**<span data-ttu-id="0128a-104">Se aplica a</span><span class="sxs-lookup"><span data-stu-id="0128a-104">Applies to</span></span>**

-  <span data-ttu-id="0128a-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="0128a-105">Partner Center</span></span>
-  <span data-ttu-id="0128a-106">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="0128a-106">Azure portal</span></span>
-  <span data-ttu-id="0128a-107">Partners de CSP</span><span class="sxs-lookup"><span data-stu-id="0128a-107">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="0128a-108">Determinar el tamaño de la máquina virtual para la reserva de Azure de un cliente</span><span class="sxs-lookup"><span data-stu-id="0128a-108">Determine the VM size for a customer’s Azure reservation</span></span> 

<span data-ttu-id="0128a-109">Al comprar reservas de Microsoft Azure en nombre de tus clientes, deberás elegir una máquina virtual (VM) con el tamaño adecuado para satisfacer las necesidades informáticas del cliente.</span><span class="sxs-lookup"><span data-stu-id="0128a-109">When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.</span></span> <span data-ttu-id="0128a-110">Encontrarás esta información usando uno de estos métodos:</span><span class="sxs-lookup"><span data-stu-id="0128a-110">You can find this information using one of these methods:</span></span>

-   <span data-ttu-id="0128a-111">API Azure Utilization</span><span class="sxs-lookup"><span data-stu-id="0128a-111">Azure utilization API</span></span>
-   <span data-ttu-id="0128a-112">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="0128a-112">The Azure portal</span></span>
-   <span data-ttu-id="0128a-113">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="0128a-113">Azure PowerShell</span></span>
-   <span data-ttu-id="0128a-114">La API de Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="0128a-114">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="0128a-115">A continuación, encontrarás instrucciones para cada uno de estos métodos.</span><span class="sxs-lookup"><span data-stu-id="0128a-115">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="0128a-116">Después de comprar una reserva, el descuento de reserva se aplicará automáticamente a las máquinas virtuales que coincidan con los atributos y la cantidad de la reserva.</span><span class="sxs-lookup"><span data-stu-id="0128a-116">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="0128a-117">No es necesario asignar la reserva a una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="0128a-117">You don’t need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="0128a-118">Los descuentos de reserva no se aplican a máquinas virtuales clásicas o promocionales.</span><span class="sxs-lookup"><span data-stu-id="0128a-118">Reservation discounts don’t apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="0128a-119">Para identificar correctamente el tipo y el tamaño de la máquina virtual que se debe comprar en nombre del cliente, debes usar uno de los métodos que se describen a continuación ya que el tipo de serie de la máquina virtual no se muestra correctamente en los archivos de conciliación del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="0128a-119">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>


**<span data-ttu-id="0128a-120">Obtener información de cambio de tamaño de máquina virtual con la API Azure Utilization</span><span class="sxs-lookup"><span data-stu-id="0128a-120">Get VM sizing information using the Azure utilization API</span></span>**

1.  <span data-ttu-id="0128a-121">Usa el valor del atributo ServiceType de additionalInfo en la respuesta de la API para identificar el tamaño de la máquina virtual que se comprará.</span><span class="sxs-lookup"><span data-stu-id="0128a-121">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span> 

2.  <span data-ttu-id="0128a-122">Para obtener más información, consulta [Obtener los registros de uso de un cliente para Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) en la [API del Centro de partners](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="0128a-122">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span> 

**<span data-ttu-id="0128a-123">Obtener información de cambio de tamaño de máquina virtual con el portal de Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="0128a-123">Get VM sizing information using the Microsoft Azure portal</span></span>**

1.  <span data-ttu-id="0128a-124">En el centro de partners, ve a la página de **los clientes** .</span><span class="sxs-lookup"><span data-stu-id="0128a-124">In Partner Center, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="0128a-125">Encuentra al cliente que quiera comprar reservas de VM de Azure y, a continuación, selecciona la flecha abajo para expandir la información del cliente.</span><span class="sxs-lookup"><span data-stu-id="0128a-125">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="0128a-126">Selecciona **Portal de administración de Microsoft Azure** para abrir el registro del cliente en el Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="0128a-126">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="0128a-127">Selecciona **Máquinas virtuales** en el menú del portal y, a continuación, la máquina virtual para la que quieras comprar una reserva.</span><span class="sxs-lookup"><span data-stu-id="0128a-127">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span> 

4.  <span data-ttu-id="0128a-128">En la página de detalles de la VM, encuentra la información de tamaño y región, como se muestra a continuación, y usa esta información para comprar la reserva en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="0128a-128">On the VM’s detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![Información de tamaño y región en la página de detalles](images/usage1.png)

**<span data-ttu-id="0128a-130">Obtener información de cambio de tamaño de VM con el Microsoft Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="0128a-130">Get VM sizing information using Microsoft Azure PowerShell</span></span>**

<span data-ttu-id="0128a-131">Usa la información de la imagen siguiente para obtener la ubicación y el tamaño de la VM para la que quieres comprar una reserva.</span><span class="sxs-lookup"><span data-stu-id="0128a-131">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![Tamaño y la ubicación de la máquina virtual](images/usage2.png)

**<span data-ttu-id="0128a-133">Obtener información de cambio de tamaño de VM con la API de Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="0128a-133">Get VM sizing information using the Azure Resource Manager (ARM) API</span></span>**

1.  <span data-ttu-id="0128a-134">Con ARMClient o las API de ARM, llama al cliente de ARM para la VM para la que quieres comprar una reserva.</span><span class="sxs-lookup"><span data-stu-id="0128a-134">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2.  <span data-ttu-id="0128a-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="0128a-135">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3.  <span data-ttu-id="0128a-136">La llamada devuelve los valores de **vmSize** y **ubicación**, como se muestra a continuación.</span><span class="sxs-lookup"><span data-stu-id="0128a-136">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    <span data-ttu-id="0128a-137">![valor de vmSize](images/usage3.png)
    ![valor de ubicación](images/usage4.png)</span><span class="sxs-lookup"><span data-stu-id="0128a-137">![vmSize value](images/usage3.png)
![location value](images/usage4.png)</span></span>
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="0128a-138">Comprobar descuento de reserva y uso de la VM de Azure</span><span class="sxs-lookup"><span data-stu-id="0128a-138">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="0128a-139">Después de adquirir una instancia de VM reservada de Azure en nombre de un cliente, el descuento de pagar por adelantado el espacio de la VM se aplica automáticamente a las máquinas virtuales que coinciden con los atributos y la cantidad de la reserva del cliente.</span><span class="sxs-lookup"><span data-stu-id="0128a-139">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer’s reservation.</span></span> 

<span data-ttu-id="0128a-140">Puedes comprobar el uso de la reserva del cliente y ver a qué máquinas virtuales se aplican los descuentos de reserva mediante uno de los siguientes métodos:</span><span class="sxs-lookup"><span data-stu-id="0128a-140">You can verify the customer’s reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>   

-   <span data-ttu-id="0128a-141">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="0128a-141">The Azure portal</span></span>
-   <span data-ttu-id="0128a-142">API Azure Utilization</span><span class="sxs-lookup"><span data-stu-id="0128a-142">Azure utilization API</span></span>

<span data-ttu-id="0128a-143">A continuación, encontrarás instrucciones para cada uno de estos métodos.</span><span class="sxs-lookup"><span data-stu-id="0128a-143">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="0128a-144">Solo la API Azure Utilization muestra a qué máquina virtual se está aplicando el descuento.</span><span class="sxs-lookup"><span data-stu-id="0128a-144">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="0128a-145">Comprobar el uso de reserva del cliente en el portal de Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="0128a-145">Verify the customer’s reservation usage in the Microsoft Azure portal</span></span>

1.  <span data-ttu-id="0128a-146">En el centro de partners, ve a la página de **los clientes** .</span><span class="sxs-lookup"><span data-stu-id="0128a-146">In Partner Center, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="0128a-147">Encuentra al cliente del que quieres comprar el uso y el descuento de la reserva y, a continuación, selecciona la flecha abajo para expandir la información del cliente.</span><span class="sxs-lookup"><span data-stu-id="0128a-147">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="0128a-148">Selecciona **Portal de administración de Microsoft Azure** para abrir el registro del cliente en el portal de Azure.</span><span class="sxs-lookup"><span data-stu-id="0128a-148">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="0128a-149">Selecciona **Reservas** en el menú del portal y, a continuación, la reserva para la que quieras comprobar el uso.</span><span class="sxs-lookup"><span data-stu-id="0128a-149">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span> 

4.  <span data-ttu-id="0128a-150">En la página **Introducción**, comprueba el gráfico de uso de la reserva, que muestra la cantidad de la reserva aplicada a máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="0128a-150">On the **Overview** page check the reservation’s utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span> 

    >[!NOTE]
    ><span data-ttu-id="0128a-151">Los datos de uso se pueden retrasar hasta un máximo de 8 horas.</span><span class="sxs-lookup"><span data-stu-id="0128a-151">Utilization data may be delayed by up to 8 hours.</span></span>
    
    <span data-ttu-id="0128a-152">a.</span><span class="sxs-lookup"><span data-stu-id="0128a-152">a.</span></span>  <span data-ttu-id="0128a-153">Si el uso de la reserva es 100%, el cliente obtiene el posible ahorro que la compra de la reserva pueda proporcionar.</span><span class="sxs-lookup"><span data-stu-id="0128a-153">If the reservation’s utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span> 
    
    <span data-ttu-id="0128a-154">b.</span><span class="sxs-lookup"><span data-stu-id="0128a-154">b.</span></span>  <span data-ttu-id="0128a-155">Si el uso de la reserva es del 0%, el descuento no se está aplicando a ninguna máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="0128a-155">If the reservation’s usage is 0%, the discount is not being applied to any virtual machine.</span></span> 
    
    <span data-ttu-id="0128a-156">c.</span><span class="sxs-lookup"><span data-stu-id="0128a-156">c.</span></span>  <span data-ttu-id="0128a-157">Si el uso de la reserva es de entre el 1 y el 99%, hay ventajas que no se emplean.</span><span class="sxs-lookup"><span data-stu-id="0128a-157">If the reservation’s usage is between 1% and 99%, there are unused benefits.</span></span> 

5.  <span data-ttu-id="0128a-158">Para evitar esta situación, determina la VM de tamaño correcto para admitir las necesidades informáticas del cliente antes de realizar la compra.</span><span class="sxs-lookup"><span data-stu-id="0128a-158">To avoid this situation, determine the correct size VM to support the customer’s computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="0128a-159">Comprobar el uso de reserva del cliente con la API Azure Utilization</span><span class="sxs-lookup"><span data-stu-id="0128a-159">Verify the customer’s reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="0128a-160">Solo la Azure utilization API muestra a qué máquina virtual se está aplicando el descuento.</span><span class="sxs-lookup"><span data-stu-id="0128a-160">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="0128a-161">Puedes obtener datos de uso de reserva con la API Azure Utilization para comprobar que el cliente está obteniendo el descuento de la reserva y para ver a qué VM (máquinas virtuales) se aplica el descuento.</span><span class="sxs-lookup"><span data-stu-id="0128a-161">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="0128a-162">Compara el ejemplo A con el ejemplo B para ver cómo comprobar el uso de reserva de un cliente.</span><span class="sxs-lookup"><span data-stu-id="0128a-162">Compare Example A to Example B to see how to verify a customer’s reservation usage.</span></span> 

![Ejemplos de uso de reserva](images/usage5.png)

-   <span data-ttu-id="0128a-164">El reservationId identifica la reserva de Azure que se usó para aplicar el descuento a la VM.</span><span class="sxs-lookup"><span data-stu-id="0128a-164">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
-   <span data-ttu-id="0128a-165">consumptionMeter es el MeterId para la VM que tiene el descuento de reserva aplicado.</span><span class="sxs-lookup"><span data-stu-id="0128a-165">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
-   <span data-ttu-id="0128a-166">El ReservationMeter muestra un costo de 0$ desde que se aplicó el descuento de reserva.</span><span class="sxs-lookup"><span data-stu-id="0128a-166">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span> 

<span data-ttu-id="0128a-167">Para obtener más información, consulta [Obtener los registros de uso de un cliente para Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) en la [API del Centro de partners](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="0128a-167">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="0128a-168">Los costes de software, como Microsoft Windows Server, no se incluyen actualmente en el precio de una reserva de VM y aparecerán como elementos de línea independientes en el registro de pedido y en tu factura.</span><span class="sxs-lookup"><span data-stu-id="0128a-168">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="0128a-169">Sin embargo, si el cliente dispone de la Ventaja de uso híbrido de Microsoft Azure, no se aplicarán los costos de software.</span><span class="sxs-lookup"><span data-stu-id="0128a-169">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="0128a-170">Para obtener más información, consulta [Costos de software de Windows no incluidos con las instancias reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="0128a-170">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="0128a-171">Recursos de Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="0128a-171">Azure reservations resources</span></span>
|**<span data-ttu-id="0128a-172">Para obtener información acerca de</span><span class="sxs-lookup"><span data-stu-id="0128a-172">For information about</span></span>**   |**<span data-ttu-id="0128a-173">Lee esto</span><span class="sxs-lookup"><span data-stu-id="0128a-173">Read this</span></span>**    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="0128a-174">Reservas de Azure en introducción de CSP</span><span class="sxs-lookup"><span data-stu-id="0128a-174">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="0128a-175">Vender Microsoft Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="0128a-175">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="0128a-176">Comprar reservas de Azure para tus clientes en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="0128a-176">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="0128a-177">Comprar reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="0128a-177">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="0128a-178">Administración de Azure reservations en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="0128a-178">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="0128a-179">Administración de Azure reservations en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="0128a-179">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="0128a-180">Comprar Azure Reservations en el Azure Portal</span><span class="sxs-lookup"><span data-stu-id="0128a-180">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="0128a-181">[Pagar por adelantado máquinas virtuales con instancias reservadas de máquina virtual](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) en la Ayuda de Azure</span><span class="sxs-lookup"><span data-stu-id="0128a-181">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="0128a-182">Administración de Azure Reservations en el Azure Portal</span><span class="sxs-lookup"><span data-stu-id="0128a-182">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="0128a-183">[Administración de instancias reservadas de máquina virtual](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) en la Ayuda de Azure</span><span class="sxs-lookup"><span data-stu-id="0128a-183">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="0128a-184">Comprar Azure Reservations con la API del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="0128a-184">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="0128a-185">[Purchase Azure Reserved VM Instances (Comprar Azure Reserved VM Instances)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) en la documentación de desarrolladores del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="0128a-185">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>



