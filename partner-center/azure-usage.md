---
title: Microsoft Azure el tamaño de la máquina virtual para el uso máximo de reserva | Centro de Partners
ms.topic: article
ms.date: 08/05/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Al comprar Microsoft Azure reservas en nombre de sus clientes, deberá elegir un tamaño de máquina virtual (VM) para satisfacer las necesidades informáticas del cliente.
author: LauraBrenner
ms.author: labrenne
keywords: azure, reservas, vm, administrar, uso, cambio de tamaño
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 9d0c2935bd5a2202b50ffc470fbef144ce4d20e2
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653780"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Cambio de tamaño de la VM de Microsoft Azure para el uso máximo de reserva

**Se aplica a**

- Centro de partners
- Azure Portal
- Partners de CSP

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Determinar el tamaño de la máquina virtual para la reserva de Azure de un cliente 

Al comprar Microsoft Azure reservas en nombre de sus clientes, deberá elegir un tamaño de máquina virtual (VM) para satisfacer las necesidades informáticas del cliente. Encontrarás esta información usando uno de estos métodos:

- API Azure Utilization
- Azure Portal
- Azure PowerShell
- La API de Azure Resource Manager (ARM)

A continuación, encontrarás instrucciones para cada uno de estos métodos. Después de comprar una reserva, el descuento de reserva se aplicará automáticamente a las máquinas virtuales que coincidan con los atributos y la cantidad de la reserva. No es necesario asignar la reserva a una máquina virtual.

>[!NOTE]
>Los descuentos de reserva no se aplican a las máquinas virtuales de promoción o clásicas.

>[!IMPORTANT]
>Para identificar correctamente el tipo y el tamaño de la máquina virtual que se debe comprar en nombre del cliente, debes usar uno de los métodos que se describen a continuación ya que el tipo de serie de la máquina virtual no se muestra correctamente en los archivos de conciliación del Centro de partners.

**Obtención de información de tamaño de la máquina virtual mediante la API de uso de Azure**

1. Usa el valor del atributo ServiceType de additionalInfo en la respuesta de la API para identificar el tamaño de la máquina virtual que se comprará.
2. Para obtener más información, consulte [obtención de los registros de uso de un cliente para Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) en la [API del centro de Partners](https://docs.microsoft.com/partner-center/develop/).

**Obtención de información de tamaño de la máquina virtual mediante el Microsoft Azure Portal**

1. En el centro de Partners, vaya a la página de **clientes** .
2. Busque el cliente que desea comprar reservas de máquinas virtuales de Azure y, después, seleccione la flecha abajo para expandir la información del cliente. Seleccione **portal de administración de Microsoft Azure** para abrir el registro del cliente en el Azure portal.
3. Selecciona **Máquinas virtuales** en el menú del portal y, a continuación, la máquina virtual para la que quieras comprar una reserva.
4. En la página de detalles de la máquina virtual, busque la información de tamaño y región, como se muestra a continuación, y use esta información para comprar la reserva en el centro de Partners.  

    ![Información de tamaño y región en la página de detalles](images/usage1.png)

**Obtención de información de tamaño de máquina virtual mediante Microsoft Azure PowerShell**

Usa la información de la imagen siguiente para obtener la ubicación y el tamaño de la VM para la que quieres comprar una reserva. 

![Ubicación y tamaño de la máquina virtual](images/usage2.png)

**Obtención de información de tamaño de la máquina virtual mediante la API de Azure Resource Manager (ARM)**

1. Con ARMClient o las API de ARM, llama al cliente de ARM para la VM para la que quieres comprar una reserva.

2. /subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01

3. La llamada devuelve los valores de **vmSize** y **ubicación**, como se muestra a continuación.

    ![valor de vmSize](images/usage3.png) ![valor de ubicación](images/usage4.png)

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Comprobar descuento de reserva y uso de la VM de Azure

Después de comprar una instancia reservada de máquina virtual de Azure en nombre de un cliente, el descuento por pagar por el espacio de máquina virtual de antemano se aplica automáticamente a las máquinas virtuales que coinciden con los atributos y la cantidad de la reserva del cliente.

Puede comprobar el uso de la reserva del cliente y ver a qué máquinas virtuales se aplican los descuentos de reserva mediante uno de los métodos siguientes:

- Azure Portal
- API Azure Utilization

A continuación, encontrarás instrucciones para cada uno de estos métodos.

>[!NOTE]
>Solo la API Azure Utilization muestra a qué máquina virtual se está aplicando el descuento.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Compruebe el uso de la reserva del cliente en el Microsoft Azure Portal

1. En el centro de Partners, vaya a la página de **clientes** .

2. Busque el cliente cuyo descuento de reserva y el uso desea comprobar y, a continuación, seleccione la flecha abajo para expandir la información del cliente. Seleccione **portal de administración de Microsoft Azure** para abrir el registro del cliente en el Azure portal.
3. Selecciona **Reservas** en el menú del portal y, a continuación, la reserva para la que quieras comprobar el uso.
4. En la página **información general** , compruebe el gráfico de uso de la reserva, que muestra la cantidad de reserva que se aplicó a las máquinas virtuales.

    >[!NOTE]
    >Los datos de uso se pueden retrasar hasta un máximo de 8 horas.

    a. Si el uso de la reserva es del 100%, el cliente obtiene todos los ahorros posibles que puede proporcionar la compra de reserva.
    b. Si el uso de la reserva es 0%, el descuento no se aplica a ninguna máquina virtual.
    c. Si el uso de la reserva está entre 1% y 99%, hay ventajas no utilizadas.

5. Para evitar esta situación, determine el tamaño correcto de la máquina virtual para satisfacer las necesidades informáticas de los clientes antes de hacer la compra.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Comprobación del uso de la reserva del cliente con la API de uso de Azure

>[!NOTE]
>Solo la API Azure Utilization muestra a qué máquina virtual se está aplicando el descuento.  

Puedes obtener datos de uso de reserva con la API Azure Utilization para comprobar que el cliente está obteniendo el descuento de la reserva y para ver a qué VM (máquinas virtuales) se aplica el descuento. Compare el ejemplo a con el ejemplo B para ver cómo comprobar el uso de la reserva de un cliente.

![Ejemplos de uso de reserva](images/usage5.png)

- El reservationId identifica la reserva de Azure que se usó para aplicar el descuento a la VM.
- consumptionMeter es el MeterId para la VM que tiene el descuento de reserva aplicado.
- El ReservationMeter muestra un costo de 0 $ desde que se aplicó el descuento de reserva.

Para obtener más información, consulte [obtención de los registros de uso de un cliente para Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) en la [API del centro de Partners](https://docs.microsoft.com/partner-center/develop/).

>[!IMPORTANT]
>Los costes de software, como Microsoft Windows Server, no se incluyen actualmente en el precio de una reserva de VM y aparecerán como elementos de línea independientes en el registro de pedido y en tu factura. Sin embargo, si el cliente dispone de la Ventaja de uso híbrido de Microsoft Azure, no se aplicarán los costos de software. Para obtener más información, consulta [Costos de software de Windows no incluidos con las instancias reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Recursos de Azure Reservations

|**Para obtener información sobre**   |**Lee esto**    |
|:-----------------------------|:-----------------|
|Reservas de Azure en la introducción del CSP  | [Vender Microsoft Azure instancias reservadas de máquina virtual](azure-reservations.md)
|Compra de reservas de Azure para sus clientes en el centro de Partners   |[Comprar reservas de Azure](azure-reservations-buying.md)
|Administración de las reservas de Azure en el centro de Partners | [Administración de las reservas de Azure en el centro de Partners](azure-reservations-manage.md)
|Compra de reservas de Azure en Azure Portal | [Pagar por adelantado máquinas virtuales con instancias reservadas de máquina virtual](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) en la Ayuda de Azure |
|Administración de Azure Reservations en el Azure Portal   |[Administración de instancias reservadas de máquina virtual](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) en la Ayuda de Azure  |
|Compra de reservas de Azure usando la API del Centro de partners | [Purchase Azure Reserved VM Instances (Comprar Azure Reserved VM Instances)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) en la documentación de desarrolladores del Centro de partners
