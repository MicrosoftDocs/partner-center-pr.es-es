---
title: Ajuste de tamaño de máquina virtual de Microsoft Azure para el uso de reserva máximo | Centro de partners
ms.topic: article
ms.date: 10/29/2018
Description: Al comprar reservas de Microsoft Azure en nombre de tus clientes, deberás elegir una máquina virtual (VM) con el tamaño adecuado para satisfacer las necesidades informáticas del cliente.
author: LauraBrenner
ms.author: v-petand
keywords: azure, reservas, vm, administrar, uso, cambio de tamaño
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: cbe24b3da0b9cadf1ed9e8d9f06b5b575bf16d22
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586968"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a><span data-ttu-id="850dd-104">Cambio de tamaño de la VM de Microsoft Azure para el uso máximo de reserva</span><span class="sxs-lookup"><span data-stu-id="850dd-104">Microsoft Azure VM sizing for maximum reservation usage</span></span> 

<span data-ttu-id="850dd-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="850dd-105">**Applies to**</span></span>

-  <span data-ttu-id="850dd-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="850dd-106">Partner Center</span></span>
-  <span data-ttu-id="850dd-107">Portal de Azure</span><span class="sxs-lookup"><span data-stu-id="850dd-107">Azure portal</span></span>
-  <span data-ttu-id="850dd-108">Partners de CSP</span><span class="sxs-lookup"><span data-stu-id="850dd-108">Partners in CSP</span></span>

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a><span data-ttu-id="850dd-109">Determinar el tamaño de la máquina virtual para la reserva de Azure de un cliente</span><span class="sxs-lookup"><span data-stu-id="850dd-109">Determine the VM size for a customer’s Azure reservation</span></span> 

<span data-ttu-id="850dd-110">Al comprar reservas de Microsoft Azure en nombre de tus clientes, deberás elegir una máquina virtual (VM) con el tamaño adecuado para satisfacer las necesidades informáticas del cliente.</span><span class="sxs-lookup"><span data-stu-id="850dd-110">When buying Microsoft Azure reservations on behalf of your customers, you’ll need to choose a virtual machine (VM) sized to meet the customer’s computing needs.</span></span> <span data-ttu-id="850dd-111">Encontrarás esta información usando uno de estos métodos:</span><span class="sxs-lookup"><span data-stu-id="850dd-111">You can find this information using one of these methods:</span></span>

-   <span data-ttu-id="850dd-112">API Azure Utilization</span><span class="sxs-lookup"><span data-stu-id="850dd-112">Azure utilization API</span></span>
-   <span data-ttu-id="850dd-113">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="850dd-113">The Azure portal</span></span>
-   <span data-ttu-id="850dd-114">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="850dd-114">Azure PowerShell</span></span>
-   <span data-ttu-id="850dd-115">La API de Azure Resource Manager (ARM)</span><span class="sxs-lookup"><span data-stu-id="850dd-115">The Azure Resource Manager (ARM) API</span></span>

<span data-ttu-id="850dd-116">A continuación, encontrarás instrucciones para cada uno de estos métodos.</span><span class="sxs-lookup"><span data-stu-id="850dd-116">Instructions for using each of these methods are below.</span></span> <span data-ttu-id="850dd-117">Después de comprar una reserva, el descuento de reserva se aplicará automáticamente a las máquinas virtuales que coincidan con los atributos y la cantidad de la reserva.</span><span class="sxs-lookup"><span data-stu-id="850dd-117">After you buy a reservation, the reservation discount is applied automatically to virtual machines matching the attributes and quantity of the reservation.</span></span> <span data-ttu-id="850dd-118">No es necesario asignar la reserva a una máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="850dd-118">You don’t need to assign the reservation to a VM.</span></span>

>[!NOTE]
><span data-ttu-id="850dd-119">Los descuentos de reserva no se aplican a máquinas virtuales clásicas o promocionales.</span><span class="sxs-lookup"><span data-stu-id="850dd-119">Reservation discounts don’t apply to classic or promotional VMs.</span></span>

>[!IMPORTANT]
><span data-ttu-id="850dd-120">Para identificar correctamente el tipo y el tamaño de la máquina virtual que se debe comprar en nombre del cliente, debes usar uno de los métodos que se describen a continuación ya que el tipo de serie de la máquina virtual no se muestra correctamente en los archivos de conciliación del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="850dd-120">To correctly identify the type and size of VM to buy on behalf of your customer, you must use one of the methods described below as the VM series type is not correctly displayed in Partner Center reconciliation files.</span></span>


<span data-ttu-id="850dd-121">**Obtenga información mediante el uso de API de Azure de tamaño de máquina virtual**</span><span class="sxs-lookup"><span data-stu-id="850dd-121">**Get VM sizing information using the Azure utilization API**</span></span>

1.  <span data-ttu-id="850dd-122">Usa el valor del atributo ServiceType de additionalInfo en la respuesta de la API para identificar el tamaño de la máquina virtual que se comprará.</span><span class="sxs-lookup"><span data-stu-id="850dd-122">Use the value for ServiceType attribute from additionalInfo in the API response to identify the VM size to buy.</span></span> 

2.  <span data-ttu-id="850dd-123">Para obtener más información, consulta [Obtener los registros de uso de un cliente para Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) en la [API del Centro de partners](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="850dd-123">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span> 

<span data-ttu-id="850dd-124">**Obtenga información mediante el portal de Microsoft Azure de tamaño de máquina virtual**</span><span class="sxs-lookup"><span data-stu-id="850dd-124">**Get VM sizing information using the Microsoft Azure portal**</span></span>

1.  <span data-ttu-id="850dd-125">En el centro de partners, vaya a su **clientes** página.</span><span class="sxs-lookup"><span data-stu-id="850dd-125">In Partner Center, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="850dd-126">Encuentra al cliente que quiera comprar reservas de VM de Azure y, a continuación, selecciona la flecha abajo para expandir la información del cliente.</span><span class="sxs-lookup"><span data-stu-id="850dd-126">Find the customer who wants to buy Azure VM reservations and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="850dd-127">Selecciona **Portal de administración de Microsoft Azure** para abrir el registro del cliente en el portal de Azure.</span><span class="sxs-lookup"><span data-stu-id="850dd-127">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="850dd-128">Selecciona **Máquinas virtuales** en el menú del portal y, a continuación, la máquina virtual para la que quieras comprar una reserva.</span><span class="sxs-lookup"><span data-stu-id="850dd-128">Select **Virtual machines** from the portal menu and then select the VM for which you want to buy a reservation.</span></span> 

4.  <span data-ttu-id="850dd-129">En la página de detalles de la VM, encuentra la información de tamaño y región, como se muestra a continuación, y usa esta información para comprar la reserva en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="850dd-129">On the VM’s detail page, find the size and region information, as illustrated below, and use this information to purchase the reservation in Partner Center.</span></span>  

    ![Información de tamaño y la región en la página de detalles](images/usage1.png)

<span data-ttu-id="850dd-131">**Obtenga información con Microsoft Azure PowerShell de tamaño de máquina virtual**</span><span class="sxs-lookup"><span data-stu-id="850dd-131">**Get VM sizing information using Microsoft Azure PowerShell**</span></span>

<span data-ttu-id="850dd-132">Usa la información de la imagen siguiente para obtener la ubicación y el tamaño de la VM para la que quieres comprar una reserva.</span><span class="sxs-lookup"><span data-stu-id="850dd-132">Use the information in the image below to get the location and size of the VM for which you want to buy a reservation.</span></span> 

![Tamaño y la ubicación de la máquina virtual](images/usage2.png)

<span data-ttu-id="850dd-134">**Obtenga información mediante la API de Azure Resource Manager (ARM) de tamaño de máquina virtual**</span><span class="sxs-lookup"><span data-stu-id="850dd-134">**Get VM sizing information using the Azure Resource Manager (ARM) API**</span></span>

1.  <span data-ttu-id="850dd-135">Con ARMClient o las API de ARM, llama al cliente de ARM para la VM para la que quieres comprar una reserva.</span><span class="sxs-lookup"><span data-stu-id="850dd-135">Using the ARMClient or the ARM APIs, call the ARM client for the VM for which you want to buy a reservation.</span></span>

2.  <span data-ttu-id="850dd-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span><span class="sxs-lookup"><span data-stu-id="850dd-136">/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01</span></span>

3.  <span data-ttu-id="850dd-137">La llamada devuelve los valores de **vmSize** y **ubicación**, como se muestra a continuación.</span><span class="sxs-lookup"><span data-stu-id="850dd-137">The call returns the values for **vmSize** and **location**, as illustrated below.</span></span>

    <span data-ttu-id="850dd-138">![valor de vmSize](images/usage3.png)
    ![valor de ubicación](images/usage4.png)</span><span class="sxs-lookup"><span data-stu-id="850dd-138">![vmSize value](images/usage3.png)
![location value](images/usage4.png)</span></span>
 

## <a name="verify-azure-vm-usage-and-reservation-discount"></a><span data-ttu-id="850dd-139">Comprobar descuento de reserva y uso de la VM de Azure</span><span class="sxs-lookup"><span data-stu-id="850dd-139">Verify Azure VM usage and reservation discount</span></span>

<span data-ttu-id="850dd-140">Después de adquirir una instancia de VM reservada de Azure en nombre de un cliente, el descuento de pagar por adelantado el espacio de la VM se aplica automáticamente a las máquinas virtuales que coinciden con los atributos y la cantidad de la reserva del cliente.</span><span class="sxs-lookup"><span data-stu-id="850dd-140">After you purchase an Azure Reserved VM Instance on behalf of a customer, the discount for paying for VM space in advance is automatically applied to the virtual machines that match the attributes and quantity of the customer’s reservation.</span></span> 

<span data-ttu-id="850dd-141">Puedes comprobar el uso de la reserva del cliente y ver a qué máquinas virtuales se aplican los descuentos de reserva mediante uno de los siguientes métodos:</span><span class="sxs-lookup"><span data-stu-id="850dd-141">You can verify the customer’s reservation usage and see which virtual machines the reservation discounts are applied to by using one of the following methods:</span></span>   

-   <span data-ttu-id="850dd-142">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="850dd-142">The Azure portal</span></span>
-   <span data-ttu-id="850dd-143">API Azure Utilization</span><span class="sxs-lookup"><span data-stu-id="850dd-143">Azure utilization API</span></span>

<span data-ttu-id="850dd-144">A continuación, encontrarás instrucciones para cada uno de estos métodos.</span><span class="sxs-lookup"><span data-stu-id="850dd-144">Instructions for using each of these methods are below.</span></span>

>[!NOTE]
><span data-ttu-id="850dd-145">Solo la API Azure Utilization muestra a qué máquina virtual se está aplicando el descuento.</span><span class="sxs-lookup"><span data-stu-id="850dd-145">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a><span data-ttu-id="850dd-146">Comprobar el uso de reserva del cliente en el portal de Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="850dd-146">Verify the customer’s reservation usage in the Microsoft Azure portal</span></span>

1.  <span data-ttu-id="850dd-147">En el centro de partners, vaya a su **clientes** página.</span><span class="sxs-lookup"><span data-stu-id="850dd-147">In Partner Center, go to your **Customers** page.</span></span>

2.  <span data-ttu-id="850dd-148">Encuentra al cliente del que quieres comprar el uso y el descuento de la reserva y, a continuación, selecciona la flecha abajo para expandir la información del cliente.</span><span class="sxs-lookup"><span data-stu-id="850dd-148">Find the customer whose reservation discount and usage you want to verify and then select the down arrow to expand the customer’s information.</span></span> <span data-ttu-id="850dd-149">Selecciona **Portal de administración de Microsoft Azure** para abrir el registro del cliente en el portal de Azure.</span><span class="sxs-lookup"><span data-stu-id="850dd-149">Select **Microsoft Azure Management Portal** to open the customer’s record in the Azure portal.</span></span> 

3.  <span data-ttu-id="850dd-150">Selecciona **Reservas** en el menú del portal y, a continuación, la reserva para la que quieras comprobar el uso.</span><span class="sxs-lookup"><span data-stu-id="850dd-150">Select **Reservations** from the portal menu and then select the reservation you want to check usage for.</span></span> 

4.  <span data-ttu-id="850dd-151">En la página **Introducción**, comprueba el gráfico de uso de la reserva, que muestra la cantidad de la reserva aplicada a máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="850dd-151">On the **Overview** page check the reservation’s utilization graph, which shows how much of the reservation was applied to virtual machines.</span></span> 

    >[!NOTE]
    ><span data-ttu-id="850dd-152">Los datos de uso se pueden retrasar hasta un máximo de 8 horas.</span><span class="sxs-lookup"><span data-stu-id="850dd-152">Utilization data may be delayed by up to 8 hours.</span></span>
    
    <span data-ttu-id="850dd-153">a.</span><span class="sxs-lookup"><span data-stu-id="850dd-153">a.</span></span>  <span data-ttu-id="850dd-154">Si el uso de la reserva es 100 %, el cliente obtiene el posible ahorro que la compra de la reserva pueda proporcionar.</span><span class="sxs-lookup"><span data-stu-id="850dd-154">If the reservation’s utilization is 100%, your customer is getting all the possible savings that the reservation purchase can provide.</span></span> 
    
    <span data-ttu-id="850dd-155">b.</span><span class="sxs-lookup"><span data-stu-id="850dd-155">b.</span></span>  <span data-ttu-id="850dd-156">Si el uso de la reserva es del 0 %, el descuento no se está aplicando a ninguna máquina virtual.</span><span class="sxs-lookup"><span data-stu-id="850dd-156">If the reservation’s usage is 0%, the discount is not being applied to any virtual machine.</span></span> 
    
    <span data-ttu-id="850dd-157">c.</span><span class="sxs-lookup"><span data-stu-id="850dd-157">c.</span></span>  <span data-ttu-id="850dd-158">Si el uso de la reserva es de entre el 1 y el 99 %, hay ventajas que no se emplean.</span><span class="sxs-lookup"><span data-stu-id="850dd-158">If the reservation’s usage is between 1% and 99%, there are unused benefits.</span></span> 

5.  <span data-ttu-id="850dd-159">Para evitar esta situación, determina la VM de tamaño correcto para admitir las necesidades informáticas del cliente antes de realizar la compra.</span><span class="sxs-lookup"><span data-stu-id="850dd-159">To avoid this situation, determine the correct size VM to support the customer’s computing needs before making the purchase.</span></span>

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a><span data-ttu-id="850dd-160">Comprobar el uso de reserva del cliente con la API Azure Utilization</span><span class="sxs-lookup"><span data-stu-id="850dd-160">Verify the customer’s reservation usage with the Azure utilization API</span></span>

>[!NOTE]
><span data-ttu-id="850dd-161">Solo la API Azure Utilization muestra a qué máquina virtual se está aplicando el descuento.</span><span class="sxs-lookup"><span data-stu-id="850dd-161">Only the Azure utilization API shows which virtual machine the discount is being applied to.</span></span>  

<span data-ttu-id="850dd-162">Puedes obtener datos de uso de reserva con la API Azure Utilization para comprobar que el cliente está obteniendo el descuento de la reserva y para ver a qué VM (máquinas virtuales) se aplica el descuento.</span><span class="sxs-lookup"><span data-stu-id="850dd-162">You can get reservation usage data with the Azure utilization API to verify that the customer is getting the reservation discount and to see which VMs (virtual machines) the discount is applied to.</span></span> <span data-ttu-id="850dd-163">Compara el ejemplo A con el ejemplo B para ver cómo comprobar el uso de reserva de un cliente.</span><span class="sxs-lookup"><span data-stu-id="850dd-163">Compare Example A to Example B to see how to verify a customer’s reservation usage.</span></span> 

![Ejemplos de uso de reserva](images/usage5.png)

-   <span data-ttu-id="850dd-165">El reservationId identifica la reserva de Azure que se usó para aplicar el descuento a la VM.</span><span class="sxs-lookup"><span data-stu-id="850dd-165">The reservationId identifies the Azure reservation that was used to apply the discount to the VM.</span></span>
-   <span data-ttu-id="850dd-166">consumptionMeter es el MeterId para la VM que tiene el descuento de reserva aplicado.</span><span class="sxs-lookup"><span data-stu-id="850dd-166">consumptionMeter is the MeterId for the VM that has the reservation discount applied to it.</span></span>
-   <span data-ttu-id="850dd-167">El ReservationMeter muestra un costo de 0 $ desde que se aplicó el descuento de reserva.</span><span class="sxs-lookup"><span data-stu-id="850dd-167">The ReservationMeter shows $0 cost since the reservation discount was applied.</span></span> 

<span data-ttu-id="850dd-168">Para obtener más información, consulta [Obtener los registros de uso de un cliente para Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) en la [API del Centro de partners](https://docs.microsoft.com/partner-center/develop/).</span><span class="sxs-lookup"><span data-stu-id="850dd-168">For more information, see [Get a customer’s utilization records for Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in the [Partner Center API](https://docs.microsoft.com/partner-center/develop/).</span></span>

>[!IMPORTANT]
><span data-ttu-id="850dd-169">Los costes de software, como Microsoft Windows Server, no se incluyen actualmente en el precio de una reserva de VM y aparecerán como elementos de línea independientes en el registro de pedido y en tu factura.</span><span class="sxs-lookup"><span data-stu-id="850dd-169">Software costs, such as Microsoft Windows Server, are not currently included in the price of a VM reservation and will appear as separate line items in the order record and on your invoice.</span></span> <span data-ttu-id="850dd-170">Sin embargo, si el cliente dispone de la Ventaja de uso híbrido de Microsoft Azure, no se aplicarán los costos de software.</span><span class="sxs-lookup"><span data-stu-id="850dd-170">However, if a customer has the Azure Hybrid Use Benefit, the software costs will not be applied.</span></span> <span data-ttu-id="850dd-171">Para obtener más información, consulta [Costos de software de Windows no incluidos con las instancias reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span><span class="sxs-lookup"><span data-stu-id="850dd-171">For more information, see [Windows software costs not included with Reserved Instances](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).</span></span>  

## <a name="azure-reservations-resources"></a><span data-ttu-id="850dd-172">Recursos de Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="850dd-172">Azure reservations resources</span></span>
|<span data-ttu-id="850dd-173">**Para obtener información acerca de**</span><span class="sxs-lookup"><span data-stu-id="850dd-173">**For information about**</span></span>   |<span data-ttu-id="850dd-174">**Lea este**</span><span class="sxs-lookup"><span data-stu-id="850dd-174">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
|<span data-ttu-id="850dd-175">Reservas de Azure en la introducción del CSP</span><span class="sxs-lookup"><span data-stu-id="850dd-175">Azure reservations in CSP overview</span></span>  | [<span data-ttu-id="850dd-176">Vende instancias reservadas de VM de Azure de Microsoft</span><span class="sxs-lookup"><span data-stu-id="850dd-176">Sell Microsoft Azure Reserved VM Instances</span></span>](azure-reservations.md)
|<span data-ttu-id="850dd-177">Compra de reservas de Azure para sus clientes en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="850dd-177">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="850dd-178">Comprar reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="850dd-178">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="850dd-179">Administración de las reservas de Azure en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="850dd-179">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="850dd-180">Administración de las reservas de Azure en el centro de partners</span><span class="sxs-lookup"><span data-stu-id="850dd-180">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="850dd-181">Compra de reservas de Azure en Azure Portal</span><span class="sxs-lookup"><span data-stu-id="850dd-181">Purchasing Azure reservations in the Azure portal</span></span> | <span data-ttu-id="850dd-182">[Pagar por adelantado máquinas virtuales con instancias reservadas de máquina virtual](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) en la Ayuda de Azure</span><span class="sxs-lookup"><span data-stu-id="850dd-182">[Prepay for virtual machines with Azure Reserved VM Instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) in the Azure Help</span></span> |
|<span data-ttu-id="850dd-183">Administración de Azure Reservations en el Azure Portal</span><span class="sxs-lookup"><span data-stu-id="850dd-183">Managing Azure reservations in the Azure portal</span></span>   |<span data-ttu-id="850dd-184">[Administración de instancias reservadas de máquina virtual](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) en la Ayuda de Azure</span><span class="sxs-lookup"><span data-stu-id="850dd-184">[Manage reserved VM instances](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) in the Azure Help</span></span>  |
|<span data-ttu-id="850dd-185">Compra de reservas de Azure usando la API del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="850dd-185">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="850dd-186">[Purchase Azure Reserved VM Instances (Comprar Azure Reserved VM Instances)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) en la documentación de desarrolladores del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="850dd-186">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>



