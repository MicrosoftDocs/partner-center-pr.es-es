---
title: Cambio de tamaño de máquina virtual de Azure para usar la máxima reserva
description: Obtenga información acerca de cómo cambiar el tamaño de una máquina virtual (VM) a las necesidades informáticas de sus clientes al comprar Microsoft Azure reservas para ellas.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: ba24376bad1d04fcbc9f02d442f0cba7e6354bd3
ms.sourcegitcommit: c40f826bb1143555bf3a1c2c806c34024f0f6019
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/02/2020
ms.locfileid: "89367099"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Cambio de tamaño de VM de Microsoft Azure para el uso de reserva máximo

**Se aplica a**

- Centro de partners
- Azure portal
- Partners del programa CSP
 
> [!NOTE]
> Este artículo se aplica únicamente a los asociados del programa proveedor de soluciones en la nube (CSP). Los clientes que usen otros tipos de suscripciones (como, por ejemplo, pago por uso, individuo, contrato de cliente de Microsoft o suscripciones Contrato Enterprise), en su lugar, deberán leer [esta documentación](https://docs.microsoft.com/azure/cost-management-billing/reservations)de las reservas de Azure.

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Determinar el tamaño de la máquina virtual para la reserva de Azure de un cliente

Al comprar Microsoft Azure reservas en nombre de sus clientes, deberá elegir un tamaño de máquina virtual (VM) para satisfacer las necesidades informáticas del cliente. Puede encontrar esta información mediante uno de estos métodos:

- API de uso de Azure
- El Portal de Azure
- Azure PowerShell
- La API de Azure Resource Manager (ARM)

A continuación se proporcionan instrucciones para usar cada uno de estos métodos. Después de comprar una reserva, el descuento de la reserva se aplica automáticamente a las máquinas virtuales que coinciden con los atributos y la cantidad de la reserva. No es necesario asignar la reserva a una máquina virtual.

>[!NOTE]
>Los descuentos de reserva no se aplican a las máquinas virtuales de promoción o clásicas.

>[!IMPORTANT]
>Para identificar correctamente el tipo y el tamaño de la máquina virtual que se va a comprar en nombre de su cliente, debe usar uno de los métodos descritos a continuación, ya que el tipo de serie de la máquina virtual no se muestra correctamente en los archivos de conciliación del centro de Partners.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Obtención de información de tamaño de la máquina virtual mediante la API de uso de Azure

1. Use el valor para el atributo ServiceType de additionalInfo en la respuesta de la API para identificar el tamaño de la máquina virtual que se va a comprar.

2. Para obtener más información, consulte [obtención de los registros de uso de un cliente para Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) en la [API del centro de Partners](https://docs.microsoft.com/partner-center/develop/).

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Obtención de información de tamaño de la máquina virtual mediante el Microsoft Azure Portal

1. En el centro de Partners, vaya a la página de **clientes** .

2. Busque el cliente que desea comprar reservas de máquinas virtuales de Azure y, después, seleccione la flecha abajo para expandir la información del cliente. Seleccione **portal de administración de Microsoft Azure** para abrir el registro del cliente en el Azure portal.

3. Seleccione **máquinas virtuales** en el menú del portal y, a continuación, seleccione la máquina virtual para la que desea comprar una reserva.

4. En la página de detalles de la máquina virtual, busque la información de tamaño y región, como se muestra a continuación, y use esta información para comprar la reserva en el centro de Partners.  

   :::image type="content" source="images/usage1.png" alt-text="Información de tamaño y región en la página de detalles":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Obtención de información de tamaño de máquina virtual mediante Microsoft Azure PowerShell

Use la información de la imagen siguiente para obtener la ubicación y el tamaño de la máquina virtual para la que desea comprar una reserva. 

:::image type="content" source="images/usage2.png" alt-text="Ubicación y tamaño de la máquina virtual":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Obtención de información de tamaño de la máquina virtual mediante la API de Azure Resource Manager (ARM)

1. Con las API de ARMClient o ARM, llame al cliente de ARM para la máquina virtual para la que desea comprar una reserva.

2. /subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? API-version = 2017-12-01

3. La llamada devuelve los valores de **vmSize** y **Location**, como se muestra a continuación.

    :::image type="content" source="images/usage3.png" alt-text="valor vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="valor de ubicación":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Comprobación del uso de VM de Azure y el descuento de reserva

Después de comprar una instancia reservada de máquina virtual de Azure en nombre de un cliente, el descuento por pagar por el espacio de máquina virtual de antemano se aplica automáticamente a las máquinas virtuales que coinciden con los atributos y la cantidad de la reserva del cliente.

Puede comprobar el uso de la reserva del cliente y ver a qué máquinas virtuales se aplican los descuentos de reserva mediante uno de los métodos siguientes:

- El Portal de Azure
- API de uso de Azure

A continuación se proporcionan instrucciones para usar cada uno de estos métodos.

>[!NOTE]
>Solo la API de uso de Azure muestra la máquina virtual a la que se aplica el descuento.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Compruebe el uso de la reserva del cliente en el Microsoft Azure Portal

1. En el centro de Partners, vaya a la página de **clientes** .

2. Busque el cliente cuyo descuento de reserva y el uso desea comprobar y, a continuación, seleccione la flecha abajo para expandir la información del cliente. Seleccione **portal de administración de Microsoft Azure** para abrir el registro del cliente en el Azure portal.
3. Seleccione **reservas** en el menú del portal y, a continuación, seleccione la reserva para la que desea comprobar el uso.
4. En la página **información general** , compruebe el gráfico de uso de la reserva, que muestra la cantidad de reserva que se aplicó a las máquinas virtuales.

    >[!NOTE]
    >Los datos de uso se pueden retrasar hasta 8 horas.

    a. Si el uso de la reserva es del 100%, el cliente obtiene todos los ahorros posibles que puede proporcionar la compra de reserva.
    b. Si el uso de la reserva es 0%, el descuento no se aplica a ninguna máquina virtual.
    c. Si el uso de la reserva está entre 1% y 99%, hay ventajas no utilizadas.

5. Para evitar esta situación, determine el tamaño correcto de la máquina virtual para satisfacer las necesidades informáticas de los clientes antes de hacer la compra.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Comprobación del uso de la reserva del cliente con la API de uso de Azure

>[!NOTE]
>Solo la API de uso de Azure muestra la máquina virtual a la que se aplica el descuento.  

Puede obtener datos de uso de reserva con la API de uso de Azure para comprobar que el cliente está obteniendo el descuento de reserva y ver a qué máquinas virtuales (máquinas virtuales) se aplica el descuento. Compare el ejemplo a con el ejemplo B para ver cómo comprobar el uso de la reserva de un cliente.

:::image type="content" source="images/usage5.png" alt-text="Ejemplos de uso de reserva":::

- ReservationId identifica la reserva de Azure que se usó para aplicar el descuento a la máquina virtual.
- consumptionMeter es el MeterId de la máquina virtual que tiene aplicado el descuento de reserva.
- El ReservationMeter muestra el costo $0 desde que se aplicó el descuento de reserva.

Para obtener más información, consulte [obtención de los registros de uso de un cliente para Azure](https://docs.microsoft.com/partner-center/develop/get-a-customer-s-utilization-record-for-azure) en la [API del centro de Partners](https://docs.microsoft.com/partner-center/develop/).

>[!IMPORTANT]
>Los costos de software, como Microsoft Windows Server, no se incluyen actualmente en el precio de una reserva de máquinas virtuales y aparecerán como elementos de línea independientes en el registro de pedidos y en la factura. Sin embargo, si un cliente tiene la ventaja de uso híbrido de Azure, no se aplicarán los costos de software. Para obtener más información, consulte [los costos de software de Windows no incluidos con las instancias reservadas](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs).  

## <a name="azure-reservations-resources"></a>Recursos de reservas de Azure

|**Para información acerca de**   |**Lee esto**    |
|:-----------------------------|:-----------------|
|Información general sobre las reservas de Azure en CSP  | [Vender Microsoft Azure instancias reservadas de máquina virtual](azure-reservations.md)
|Compra de reservas de Azure para sus clientes en el centro de Partners   | [Comprar reservas de Azure](azure-reservations-buying.md)
|Administración de las reservas de Azure en el centro de Partners | [Administración de las reservas de Azure en el centro de Partners](azure-reservations-manage.md)
|Compra de reservas de Azure en el Azure Portal | [Pagar por adelantado máquinas virtuales con Azure Reserved VM instances](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) en la ayuda de Azure |
|Administración de las reservas de Azure en el Azure Portal   | [Administración de instancias reservadas de máquina virtual](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) en la ayuda de Azure  |
|Compra de reservas de Azure mediante la API del centro de Partners | [Comprar Azure Reserved VM instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) en la documentación para desarrolladores del centro de Partners   |
|Otorgar permiso a los clientes para comprar sus propias reservas de Azure a partir de una suscripción que haya adquirido. | [Conceder permiso a los clientes para que compren sus propias reservas de Azure](give-customers-permission.md)   |
