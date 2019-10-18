---
title: Administrar reservas de Microsoft Azure en nombre de los clientes | Centro de partners
ms.topic: article
ms.date: 03/15/2019
Description: Para administrar las reservas de Azure de sus clientes después de la compra, seleccione el cliente y la reserva que desea administrar en el centro de Partners y, a continuación, realice cambios en la reserva en el Azure Portal.
author: LauraBrenner
ms.author: labrenne
keywords: Azure, reservas, administración, facturación, compra, cancelación, intercambio, cuota de finalización anticipada
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: b7e9726acbba54daf8404fdf4a3d2b4961c5123a
ms.sourcegitcommit: 4b8cad9f24229767dd44fa9418fe57e10d74f390
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/01/2019
ms.locfileid: "71704158"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>Administrar reservas de Microsoft Azure en nombre de los clientes       

**Se aplica a**

-  Centro de partners
-  Microsoft Azure Portal 
-  Partners de CSP

Para administrar las reservas de Azure de sus clientes después de la compra, seleccione el cliente y la reserva que desea administrar en el centro de Partners y, a continuación, realice cambios en la reserva en el Azure Portal. 

1. Para empezar, seleccione **customers (clientes** ) en el menú del centro de Partners y seleccione el cliente cuyas reservas desea administrar. 

2. En el menú de la página de detalles del cliente, selecciona **Reservas de Azure** y, a continuación, selecciona la reserva específica que quieras administrar.  

3. En **Acciones**, selecciona **Administrar** para ir al registro de reserva del cliente en Azure Portal. En la página de detalles de la reserva, sigue los pasos siguientes para completar tareas.  

    | **No**   | **Para**    |
    |:-----------------------------|:-----------------|
    | **Introducción**   | Ver detalles de la reserva de un cliente, incluidos la fecha de expiración, el ámbito y los datos de uso. **NOTA** Selecciona **Reembolso** para crear una solicitud de soporte para un reembolso prorrateado. Selecciona **Exchange** para crear una solicitud de soporte para intercambiar la parte no usada del término de reserva.  
    | **Access Control (IAM)**   | Administrar el acceso a la información de la reserva del cliente.|
    | **Configuración**   | Cambiar el ámbito de la reserva o la suscripción de Azure a la que está asociada la reserva.    |
    | **Propiedades**   | Ver propiedades de la reserva y copiar en el Portapapeles el id. de la reserva y el id. del pedido de reserva. **NOTA** El departamento de soporte puede solicitarle el id. de reserva y el id. del pedido de reserva al solicitar soporte en nombre de un cliente.    |
    | **Nueva solicitud de soporte técnico**    | Solicitar ayuda del soporte técnico de Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Cancelar o cambiar una reserva 

Si en algún momento cambian las necesidades empresariales de un cliente, es posible que deseen cancelar una reserva y obtener un reembolso o intercambiar el importe de reembolso prorrateado de una reserva para usarlo en el precio de una nueva reserva.

En ambos escenarios, Microsoft reembolsa el importe para que pueda administrar las transacciones financieras resultantes con sus clientes. Microsoft no se pone en contacto directamente con los clientes sobre la facturación, las cancelaciones o los reembolsos.   
 

**Cómo funcionan las cancelaciones**

Los clientes pueden solicitar la cancelación de una reserva en cualquier momento (importe de reembolso limitado en $50.000 al año). La cancelación de una reserva permite al cliente devolver la cantidad de los meses restantes de una reserva de Azure para una cuota de finalización temprana. El saldo prorrateado restante, menos la cuota de finalización temprana, se reembolsa a su cuenta para que pueda reembolsar la cuenta del cliente. 

Consulte a continuación los detalles y las tarifas de cancelación.


|**Fecha de cancelación**<br> durante   |**Uso**    |**Pondrá**  |**Finalización temprana**<br> individual    |**Límite de reembolso** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 o menos                         | No          | 100 %       | No                              | $50.000 USD   |
|5 o menos                         | Sí         | Prorrateado  | No                              | $50.000 USD   |
|Más de 5                        | No          | Prorrateado  | 305                             | $50.000 USD   |
|Más de 5                        | Sí         | Prorrateado  | 305                             | $50.000 USD   |


**Cómo funcionan los intercambios** 

Si un cliente desea comprar una reserva diferente de la que compró originalmente, puede solicitar un intercambio. El intercambio de una reserva puede ser una alternativa atractiva a la cancelación de una reserva, ya que permite al cliente usar el importe de reembolso prorrateado en relación con el precio de la nueva reserva. 

El importe del reembolso prorrateado se abona en la cuenta para que pueda ofrecer al cliente un intercambio.


## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Solicitar un reembolso o cambio en nombre de un cliente 

Para enviar una solicitud de soporte técnico para un reembolso o Exchange en nombre de sus clientes, seleccione el cliente y la reserva en el centro de Partners y, a continuación, cree la solicitud de soporte técnico en el Azure Portal. 

>[!NOTE]
>Soporte técnico de Microsoft puede pedirte proporcionar el id. de reserva y el id. del pedido de reserva. Puedes encontrar esta información en la página **Propiedades** de la reserva del Azure Portal. 

1. Para empezar, seleccione **customers (clientes** ) en el menú del centro de Partners y seleccione el cliente que desea un reembolso. 

2. En la página de detalles del cliente, selecciona **Azure Reservations** y, a continuación, la reserva específica que el cliente quiera que se le reembolse.  

3. En **Acciones**, selecciona **Reembolso** para ir al registro de reserva del cliente en Azure Portal e iniciar una solicitud de soporte.  

4. En la página **Nueva solicitud de soporte técnico**, sigue los pasos que vienen a continuación para solicitar un reembolso. Selecciona **Siguiente** después de cada paso. 

    |**Pasar**                    |**Selecciones**    |
    |:---------------------------|:-----------------|
    |**1 conceptos básicos**                |Tipo de problema: facturación  |
    |**2 problema**               |Tipo de problema: administración de reservas. Categoría: intercambios y reembolsos. |
    |**3 información de contacto**   |Selecciona tus preferencias y escribe la información necesaria. 

5.  Selecciona **Crear** cuando termines.

## <a name="azure-reservations-resources"></a>Recursos de Azure Reservations
|**Para obtener información sobre**   |**Lea este**    |
|:-----------------------------|:-----------------|
|Reservas de Azure en la introducción del CSP  | [Vender Microsoft Azure instancias reservadas](azure-reservations.md) |
|Compra de reservas de Azure para sus clientes en el centro de Partners   |[Comprar reservas de Azure](azure-reservations-buying.md) |
|Determinar el tamaño correcto de VM y comprobar el uso de VM del cliente   |[Tamaño de máquina virtual para el uso máximo de reserva de Azure](azure-usage.md)   |
|Compra de reservas de Azure usando la API del Centro de partners | [Purchase Azure Reserved VM Instances (Comprar Azure Reserved VM Instances)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) en la documentación de desarrolladores del Centro de partners

