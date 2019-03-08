---
title: Administrar reservas de Microsoft Azure en nombre de los clientes | Centro de partners
ms.topic: article
ms.date: 10/29/2018
Description: Para administrar las reservas de Azure después de la compra de sus clientes, deberá seleccione la que desea administrar en el centro de partners de reserva y el cliente y, a continuación, realizar cambios en la reserva en el portal de Azure.
author: LauraBrenner
ms.author: v-petand
keywords: Azure, las reservas de direcciones, administrar, facturación, adquirir, Cancelar, exchange, tasa de finalización anticipada
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: de1846b6259764b40059ece1d311e5f63587a525
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584508"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>Administrar reservas de Microsoft Azure en nombre de los clientes

**Se aplica a**

-  Centro de partners
-  Microsoft Azure Portal
-  Partners de CSP

Para administrar las reservas de Azure después de la compra de sus clientes, deberá seleccione la que desea administrar en el centro de partners de reserva y el cliente y, a continuación, realizar cambios en la reserva en el portal de Azure. 

1. Para empezar, seleccione **clientes** en el menú de centro de partners y, a continuación, seleccione el cliente cuyas reservas de direcciones que desea administrar. 

2. En el menú de la página de detalles del cliente, selecciona **Reservas de Azure** y, a continuación, selecciona la reserva específica que quieras administrar.  

3. En **Acciones**, selecciona **Administrar** para ir al registro de reserva del cliente en Azure Portal. En la página de detalles de la reserva, sigue los pasos siguientes para completar tareas.  

    | **Select**   | **Para**    |
    |:-----------------------------|:-----------------|
    | **Información general**   | Ver detalles de la reserva de un cliente, incluidos la fecha de expiración, el ámbito y los datos de uso. **NOTA** Selecciona **Reembolso** para crear una solicitud de soporte para un reembolso prorrateado. Selecciona **Exchange** para crear una solicitud de soporte para intercambiar la parte no usada del término de reserva.  
    | **Control de acceso (IAM)**   | Administrar el acceso a la información de la reserva del cliente.|
    | **Configuración**   | Cambiar el ámbito de la reserva o la suscripción de Azure a la que está asociada la reserva.    |
    | **Propiedades**   | Ver propiedades de la reserva y copiar en el Portapapeles el id. de la reserva y el id. del pedido de reserva. **NOTA** El departamento de soporte puede solicitarle el id. de reserva y el id. del pedido de reserva al solicitar soporte en nombre de un cliente.    |
    | **Nueva solicitud de soporte técnico**    | Solicitar ayuda del soporte técnico de Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Cancelar o cambiar una reserva 

Si en cualquier momento las de un cliente necesidades empresariales evolucionan, es posible que desean cancelar una reserva y obtener un reembolso o cantidad de la reserva un reembolso prorrateado se puede usar en el precio de una nueva reserva de exchange.

En ambos escenarios, Microsoft reembolsos la cantidad para usted, lo que, a continuación, puede administrar las transacciones financieras resultantes con sus clientes. Microsoft no ponerse en contacto con los clientes directamente sobre la facturación, cancelaciones y reembolsos.   
 

**Cómo funcionan las cancelaciones**

Los clientes pueden solicitar para cancelar una reserva en cualquier momento (cantidad de reembolso tope 50.000 dólares al año). Cancelar una reserva permite al cliente devolver la cantidad de los meses restantes de una reserva de Azure para una cuota de finalización anticipada. El balance prorrateado restante, menos la tasa de finalización anticipada, se devuelve a su cuenta para que se puede reembolsar la cuenta del cliente. 

Consulte a continuación para las cuotas y los detalles de la cancelación.


|**Fecha de cancelación**<br> (días)   |**Usage**    |**Credit**  |**Finalización prematura**<br> individual    |**Límite de reembolso** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 o menos                         | No          | 100 %       | No                              | 50.000 USD   |
|5 o menos                         | Sí         | Proporcional  | No                              | 50.000 USD   |
|Más de 5                        | No          | Proporcional  | 12%                             | 50.000 USD   |
|Más de 5                        | Sí         | Proporcional  | 12%                             | 50.000 USD   |


**Cómo funcionan los intercambios** 

Si un cliente desea comprar una reserva diferente a la que compraron originalmente parte del usuario, pueden solicitar un intercambio. Intercambiar una reserva puede ser una alternativa atractiva para cancelar una reserva, ya que permite al cliente utilizar la cantidad de reembolso prorrateado hacia el precio de la reserva de nuevas. 

Por lo que puede ofrecer al cliente un intercambio, se abona el importe de reembolso prorrateado a su cuenta.


## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Solicitar un reembolso o cambio en nombre de un cliente 

Para realizar una solicitud de soporte técnico para obtener un reembolso o exchange en nombre de sus clientes, deberá seleccionar el cliente y la reserva en el centro de partners y, a continuación, cree la solicitud de soporte técnico en el portal de Azure. 

>[!NOTE]
>Soporte técnico de Microsoft puede pedirte proporcionar el id. de reserva y el id. del pedido de reserva. Puedes encontrar esta información en la página **Propiedades** de la reserva del Azure Portal. 

1. Para empezar, seleccione **clientes** en el menú de centro de partners y a continuación, seleccione el cliente que desea un reembolso. 

2. En la página de detalles del cliente, selecciona **Azure Reservations** y, a continuación, la reserva específica que el cliente quiera que se le reembolse.  

3. En **Acciones**, selecciona **Reembolso** para ir al registro de reserva del cliente en Azure Portal e iniciar una solicitud de soporte.  

4. En la página **Nueva solicitud de soporte técnico**, sigue los pasos que vienen a continuación para solicitar un reembolso. Selecciona **Siguiente** después de cada paso. 

    |**Paso**                    |**Selecciones**    |
    |:---------------------------|:-----------------|
    |**Conceptos básicos 1**                |Tipo de problema: Facturación.  |
    |**Problema 2**               |Tipo de problema: Administración de reserva. Categoría: Los intercambios y los reembolsos. |
    |**Información de contacto 3**   |Selecciona tus preferencias y escribe la información necesaria. 

5.  Selecciona **Crear** cuando termines.

## <a name="azure-reservations-resources"></a>Recursos de Azure Reservations
|**Para obtener información acerca de**   |**Lea este**    |
|:-----------------------------|:-----------------|
|Reservas de Azure en la introducción del CSP  | [Vende instancias reservadas de Microsoft Azure](azure-reservations.md) |
|Compra de reservas de Azure para sus clientes en el centro de partners   |[Comprar reservas de Azure](azure-reservations-buying.md) |
|Determinar el tamaño correcto de VM y comprobar el uso de VM del cliente   |[Ajuste de tamaño de máquina virtual para el uso de reserva máximo de Azure](azure-usage.md)   |
|Compra de reservas de Azure usando la API del Centro de partners | [Purchase Azure Reserved VM Instances (Comprar Azure Reserved VM Instances)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) en la documentación de desarrolladores del Centro de partners

