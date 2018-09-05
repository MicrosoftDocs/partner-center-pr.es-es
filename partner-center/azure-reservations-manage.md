---
title: Administrar reservas de Microsoft Azure en nombre de los clientes | Centro de partners
Description: Purchasing and managing Azure reservations on behalf of your customers.
author: v-petand
keywords: Azure, reservas, administrar, facturación, comprar
ms.localizationpriority: medium
ms.openlocfilehash: 5025c32da86944f65c548a7e3ef6e61f7275522e
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/31/2018
ms.locfileid: "2877405"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>Administrar reservas de Microsoft Azure en nombre de los clientes

**Se aplica a**

-  Panel de partners
-  Portal de Microsoft Azure
-  Partners de CSP

Para administrar Azure reservations posterior tus clientes a la compra, tendrás seleccionar el cliente y la reserva que quieres administrar en el panel de partners y, a continuación, realizar cambios en la reserva en el portal de Azure. 

1. Para empezar, selecciona **Clientes** en el menú del panel y, a continuación, el cliente cuyas reservas quieres administrar. 

2. En el menú de la página de detalles del cliente, selecciona **las reservas de Azure** y, a continuación, selecciona la reserva específica que quieras administrar.  

3. En **Acciones**, selecciona **Administrar** para ir al registro de reserva del cliente en Azure Portal. En la página de detalles de la reserva, sigue los pasos siguientes para completar tareas.  

| **Selecciona**   | **Para**    |
|:-----------------------------|:-----------------|
| **Introducción**   | Ver detalles de la reserva de un cliente, incluidos la fecha de expiración, el ámbito y los datos de uso. **NOTA** Selecciona **Reembolso** para crear una solicitud de soporte para un reembolso prorrateado. Selecciona **Exchange** para crear una solicitud de soporte para intercambiar la parte no usada del término de reserva.  
| **Access Control (IAM)**   | Administrar el acceso a la información de la reserva del cliente.|
| **Configuración**   | Cambiar el ámbito de la reserva o la suscripción de Azure a la que está asociada la reserva.    |
| **Propiedades**   | Ver propiedades de la reserva y copiar en el Portapapeles el id. de la reserva y el id. del pedido de reserva. **NOTA** El departamento de soporte puede solicitarle el id. de reserva y el id. del pedido de reserva al solicitar soporte en nombre de un cliente.    |
| **Nueva solicitud de soporte técnico**    | Solicitar ayuda del soporte técnico de Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Cancelar o cambiar una reserva 
Cuando cambien las necesidades empresariales de tus clientes, es posible que quieran cancelar una reserva o cambiar el importe del reembolso prorrateado de una reserva para usarlo para el precio de una nueva reserva. 

**Cómo funcionan las cancelaciones**

Los clientes pueden cancelar una reserva en cualquier momento (hasta 50000$ al año). La cancelación permite al cliente devolver los meses restantes de una reserva de Azure a Microsoft por un cargo por anulación anticipada. El balance prorrateado restante, menos la cuota, se reembolsarán a la comprobar original del cliente. 

**Cómo funcionan los intercambios** 

Un intercambio permite a un cliente recibir un reembolso prorrateado en función de la duración de tiempo restante de la reserva y aplicar el importe del reembolso a una nueva reserva.   

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Solicitar un reembolso o cambio en nombre de un cliente 

Para enviar una solicitud de soporte para un reembolso o cambio en nombre de los clientes, selecciona el cliente y la reserva en el Panel de partners y, a continuación, crea la solicitud de soporte en el Azure Portal. 

>[!NOTE]
>Soporte técnico de Microsoft puede pedirte proporcionar el id. de reserva y el id. del pedido de reserva. Puedes encontrar esta información en la página **Propiedades** de la reserva del Azure Portal. 

1. Para empezar, selecciona **Clientes** en el menú del panel y, a continuación, el cliente que quiere un reembolso. 

2. En la página de detalles del cliente, selecciona **Azure Reservations** y, a continuación, la reserva específica que el cliente quiera que se le reembolse.  

3. En **las acciones**, selecciona **reembolsar** para ir al registro de reserva del cliente en el Azure portal e iniciar una solicitud de soporte técnico.  

4. En la página **Nueva solicitud de soporte técnico**, sigue los pasos siguientes para solicitar un reembolso. Selecciona **Siguiente** después de cada paso. 

|**Paso**   |**Selecciones**    |
|:-----------------------------|:-----------------|
|**1 Conceptos básicos**   |Tipo de problema: facturación  |
|**2 Problema**   |Tipo de problema: administración de reservas. Categoría: intercambios y reembolsos. |
|**3 Información de contacto**   |Selecciona tus preferencias y escribe la información necesaria. Selecciona **Crear** cuando termines.   |

## <a name="azure-reservations-resources"></a>Recursos de Azure Reservations
|**Para obtener información acerca de**   |**Lee esto**    |
|:-----------------------------|:-----------------|
|Reservas de Azure en introducción de CSP  | [Vender instancias reservadas de Azure de Microsoft](azure-reservations.md) |
|Comprar reservas de Azure para los clientes de tu Panel de partners   |[Comprar reservas de Azure](azure-reservations-buying.md) |
|Determinación del tamaño correcto de la máquina virtual y comprobar el uso de la máquina virtual del cliente   |[Cambio de tamaño de la VM para el uso máximo de reserva de Azure](azure-usage.md)   |
|Comprar Azure Reservations con la API del Centro de partners | [Purchase Azure Reserved VM Instances (Comprar Azure Reserved VM Instances)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) en la documentación de desarrolladores del Centro de partners

