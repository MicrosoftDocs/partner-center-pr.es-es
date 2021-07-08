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
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Cambio de tamaño de VM de Microsoft Azure para el uso de reserva máximo

**Roles adecuados:** agente de administración | Agente de ventas

En este artículo se explica cómo cambiar el tamaño de una máquina virtual (VM) a las necesidades informáticas de los clientes al comprar Microsoft Azure reservas para ellos.
 
> [!NOTE]
> Este artículo solo se aplica a los asociados del programa Proveedor de soluciones en la nube (CSP). Los clientes que usan otros tipos de suscripciones (por ejemplo, suscripciones de pago por [uso,](/azure/cost-management-billing/reservations)individuales, Contrato de cliente de Microsoft o Enterprise Agreement) deben leer en su lugar esta documentación de reservas de Azure .

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>Determinación del tamaño de máquina virtual de la reserva de Azure de un cliente

Al comprar Microsoft Azure reservas en nombre de los clientes, deberá elegir una máquina virtual (VM) de tamaño para satisfacer las necesidades informáticas del cliente. Puede encontrar esta información mediante uno de estos métodos:

- API de uso de Azure
- El Portal de Azure
- Azure PowerShell
- The Azure Resource Manager (ARM) API

A continuación se proporcionan instrucciones para usar cada uno de estos métodos. Después de comprar una reserva, el descuento por reserva se aplica automáticamente a las máquinas virtuales que coinciden con los atributos y la cantidad de la reserva. No es necesario asignar la reserva a una máquina virtual.

>[!NOTE]
>Los descuentos de reserva no se aplican a las máquinas virtuales clásicas o promocionales.

>[!IMPORTANT]
>Para identificar correctamente el tipo y el tamaño de la máquina virtual que se va a comprar en nombre del cliente, debe usar uno de los métodos que se describen a continuación, ya que el tipo de serie de máquina virtual no se muestra correctamente en Centro de partners de conciliación.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Obtener información de tamaño de máquina virtual mediante la API de uso de Azure

1. Use el valor del atributo ServiceType de additionalInfo en la respuesta de la API para identificar el tamaño de máquina virtual que se debe comprar.

2. Para obtener más información, consulte [Obtener los registros de](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) uso de un cliente para Azure en Centro de partners [API](/partner-center/develop/).

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Obtener información de tamaño de máquina virtual mediante Microsoft Azure portal

1. En Centro de partners, vaya a la **página** Clientes.

2. Busque el cliente que quiere comprar reservas de máquinas virtuales de Azure y, a continuación, seleccione la flecha abajo para expandir la información del cliente. Seleccione **Microsoft Azure Portal de administración** para abrir el registro del cliente en el Azure Portal.

3. Seleccione **Máquinas virtuales en** el menú del portal y, a continuación, seleccione la máquina virtual para la que quiere comprar una reserva.

4. En la página de detalles de la máquina virtual, busque la información de tamaño y región, como se muestra a continuación, y use esta información para comprar la reserva en Centro de partners.  

   :::image type="content" source="images/usage1.png" alt-text="Información de tamaño y región en la página de detalles.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Obtener información de tamaño de máquina virtual mediante Microsoft Azure PowerShell

Use la información de la imagen siguiente para obtener la ubicación y el tamaño de la máquina virtual para la que desea comprar una reserva. 

:::image type="content" source="images/usage2.png" alt-text="Ubicación y tamaño de la máquina virtual.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Obtener información de tamaño de máquina virtual mediante la API Azure Resource Manager (ARM)

1. Con ARMClient o las API de ARM, llame al cliente de ARM para la máquina virtual para la que desea comprar una reserva.

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. La llamada devuelve los valores de **vmSize** y **location**, como se muestra a continuación.

    :::image type="content" source="images/usage3.png" alt-text="Valor de vmSize.":::
    :::image type="content" source="images/usage4.png" alt-text="valor de ubicación.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Comprobación del uso de máquinas virtuales de Azure y el descuento por reserva

Después de comprar una instancia reservada de máquina virtual de Azure en nombre de un cliente, el descuento por pagar por el espacio de máquina virtual por adelantado se aplica automáticamente a las máquinas virtuales que coinciden con los atributos y la cantidad de la reserva del cliente.

Puede comprobar el uso de reservas del cliente y ver a qué máquinas virtuales se aplican los descuentos de reserva mediante uno de los métodos siguientes:

- El Portal de Azure
- API de uso de Azure

A continuación se proporcionan instrucciones para usar cada uno de estos métodos.

>[!NOTE]
>Solo la API de uso de Azure muestra a qué máquina virtual se aplica el descuento.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Comprobación del uso de reservas del cliente en el portal Microsoft Azure cliente

1. En Centro de partners, vaya a la **página** Clientes.

2. Busque el cliente cuyo descuento y uso de reserva desea comprobar y, a continuación, seleccione la flecha abajo para expandir la información del cliente. Seleccione **Microsoft Azure Portal de administración** para abrir el registro del cliente en el Azure Portal.
3. Seleccione **Reservas en el** menú del portal y, a continuación, seleccione la reserva para la que desea comprobar el uso.
4. En la **página Información** general, compruebe el gráfico de uso de la reserva, que muestra la cantidad de la reserva que se aplicó a las máquinas virtuales.

    >[!NOTE]
    >Los datos de uso pueden retrasarse hasta 8 horas.

    a. Si el uso de la reserva es del 100 %, el cliente está obteniendo todos los ahorros posibles que puede proporcionar la compra de reserva.
    b. Si el uso de la reserva es del 0 %, el descuento no se aplica a ninguna máquina virtual.
    c. Si el uso de la reserva está entre el 1 % y el 99 %, hay ventajas no utilizadas.

5. Para evitar esta situación, determine el tamaño correcto de la máquina virtual para satisfacer las necesidades informáticas del cliente antes de realizar la compra.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Comprobación del uso de reservas del cliente con la API de uso de Azure

>[!NOTE]
>Solo la API de uso de Azure muestra a qué máquina virtual se aplica el descuento.  

Puede obtener datos de uso de reservas con la API de uso de Azure para comprobar que el cliente obtiene el descuento de reserva y para ver a qué máquinas virtuales (máquinas virtuales) se aplica el descuento. Compare el ejemplo A con el ejemplo B para ver cómo comprobar el uso de reservas de un cliente.

:::image type="content" source="images/usage5.png" alt-text="Ejemplos de uso de reservas.":::

- ReservationId identifica la reserva de Azure que se usó para aplicar el descuento a la máquina virtual.
- consumptionMeter es el MeterId de la máquina virtual que tiene aplicado el descuento de reserva.
- ReservationMeter muestra un costo de 0 USD desde que se aplicó el descuento de reserva.

Para obtener más información, consulte [Obtener los registros de](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) uso de un cliente para Azure en Centro de partners [API](/partner-center/develop/).

>[!IMPORTANT]
>Los costos de software, como Microsoft Windows Server, no se incluyen actualmente en el precio de una reserva de máquina virtual y aparecerán como elementos de línea independientes en el registro de pedido y en la factura. Sin embargo, si un cliente tiene la Ventaja de uso híbrido de Azure, no se aplicarán los costos de software. Para obtener más información, [vea Windows costos de software no incluidos con instancias reservadas.](/azure/billing/billing-reserved-instance-windows-software-costs)  

## <a name="next-steps"></a>Pasos siguientes

|**Para información acerca de**   |**Lee esto**    |
|:-----------------------------|:-----------------|
|Introducción a las reservas de Azure en CSP  | [Vender Microsoft Azure instancias reservadas de máquina virtual](azure-reservations.md)
|Compra de reservas de Azure para los clientes en Centro de partners   | [Compra de reservas de Azure](azure-reservations-buying.md)
|Administración de reservas de Azure en Centro de partners | [Administración de reservas de Azure en Centro de partners](azure-reservations-manage.md)
|Compra de reservas de Azure en la Azure Portal | [Pago por adelantado de máquinas virtuales con Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) en la Ayuda de Azure |
|Administración de reservas de Azure en el Azure Portal   | [Administración de instancias reservadas de máquina virtual](/azure/billing/billing-manage-reserved-vm-instance) en la Ayuda de Azure  |
|Compra de reservas de Azure mediante Centro de partners API | [Comprar Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) en la documentación Centro de partners desarrolladores   |
|Conceder a los clientes permiso para comprar sus propias reservas de Azure en una suscripción que haya adquirido para ellos. | [Conceder a los clientes permiso para comprar sus propias reservas de Azure](give-customers-permission.md)   |