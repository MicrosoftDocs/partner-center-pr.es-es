---
title: Administración de reservas de Azure para clientes
ms.topic: how-to
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Obtenga información sobre cómo administrar las reservas de Azure para un cliente, incluido cómo cancelar una reserva, intercambiar una reserva o solicitar un reembolso.
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 126d8bcae5ca7feb3eefe414bd14e476b4047d11
ms.sourcegitcommit: b79504dbfc335aca995f370e15a654829acdaaff
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/06/2020
ms.locfileid: "87900072"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Administración, cancelación, intercambio o reembolso de Microsoft Azure reservas para clientes

**Se aplica a**

- Centro de partners
- Microsoft Azure Portal 
- Asociados en CSP

**Roles adecuados**

- Agente de administrador
- Administrador global
- Agente del departamento de soporte técnico
- Agente de ventas
- Administrador del control de usuarios

> [!NOTE]
> Este artículo se aplica únicamente a los asociados del programa proveedor de soluciones en la nube (CSP). Los clientes que usen otros tipos de suscripciones (como, por ejemplo, pago por uso, individuo, contrato de cliente de Microsoft o suscripciones Contrato Enterprise), en su lugar, deberán leer [esta documentación](https://docs.microsoft.com/azure/cost-management-billing/reservations)de las reservas de Azure.

Para administrar las reservas de Azure de sus clientes después de la compra, seleccione el cliente y la reserva que desea administrar en el centro de Partners y, a continuación, realice cambios en la reserva en el Azure Portal.

1. Para empezar, seleccione **customers (clientes** ) en el menú del centro de Partners y seleccione el cliente cuyas reservas desea administrar. 

2. En el menú de la página de detalles del cliente, seleccione **reservas de Azure** y, después, seleccione la reserva específica que desea administrar.  

3. En **acciones**, seleccione **administrar** para ir al registro de reserva del cliente en el Azure portal. En la página de detalles de la reserva, siga los pasos que se indican a continuación para completar las tareas.  

    | **Select**   | **To**    |
    |:-----------------------------|:-----------------|
    | **Información general**   | Ver detalles de la reserva de un cliente, incluida la fecha de expiración, el ámbito y los datos de uso. **Nota:** Seleccione **reembolso** para crear una solicitud de soporte técnico para un reembolso prorrateado. Seleccione **Exchange** para crear una solicitud de soporte técnico para intercambiar la parte no utilizada del término de reserva.  
    | **Access Control (IAM)**   | Administrar el acceso a la información de reserva del cliente.|
    | **Configuración**   | Cambiar el ámbito de la reserva o la suscripción de Azure a la que está asociada la reserva.    |
    | **Propiedades**   | Vea las propiedades de la reserva y copie en el Portapapeles el ID. de reserva y el ID. de pedido de reserva. **Nota:** El soporte técnico puede pedirle el identificador de reserva y el identificador de pedido de reserva cuando solicite soporte técnico en nombre de un cliente.    |
    | **Nueva solicitud de soporte técnico**    | Solicitar ayuda de Soporte técnico de Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Cancelar o intercambiar una reserva

Si en algún momento cambian las necesidades empresariales de un cliente, es posible que deseen cancelar una reserva y obtener un reembolso o intercambiar el importe de reembolso prorrateado de una reserva para usarlo en el precio de una nueva reserva.

En ambos escenarios, Microsoft reembolsa el importe para que pueda administrar las transacciones financieras resultantes con sus clientes. Microsoft no se pone en contacto directamente con los clientes sobre la facturación, las cancelaciones o los reembolsos.

### <a name="how-cancellations-work"></a>Cómo funcionan las cancelaciones

Los clientes pueden solicitar la cancelación de una reserva en cualquier momento (importe de reembolso limitado en $50.000 al año). La cancelación de una reserva permite al cliente devolver la cantidad de los meses restantes de una reserva de Azure para una cuota de finalización temprana. El saldo prorrateado restante, menos la cuota de finalización temprana, se reembolsa a su cuenta para que pueda reembolsar la cuenta del cliente. 

Consulte a continuación los detalles y las tarifas de cancelación.


|**Fecha de cancelación**<br> durante   |**Uso**    |**Crédito**  |**Finalización temprana**<br> individual    |**Límite de reembolso** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 o menos                         | No          | 100%       | No                              | $50.000 USD   |
|5 o menos                         | Sí         | Prorrateado  | No                              | $50.000 USD   |
|Más de 5                        | No          | Prorrateado  | 12 %                             | $50.000 USD   |
|Más de 5                        | Sí         | Prorrateado  | 12 %                             | $50.000 USD   |

### <a name="how-exchanges-work"></a>Cómo funcionan los intercambios 

Si un cliente desea comprar una reserva diferente de la que compró originalmente, puede solicitar un intercambio. El intercambio de una reserva puede ser una alternativa atractiva a la cancelación de una reserva, ya que permite al cliente usar el importe de reembolso prorrateado en relación con el precio de la nueva reserva. 

El importe del reembolso prorrateado se abona en la cuenta para que pueda ofrecer al cliente un intercambio.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Solicitar un reembolso o intercambiar en nombre de un cliente

Para enviar una solicitud de soporte técnico para un reembolso o Exchange en nombre de sus clientes, seleccione el cliente y la reserva en el centro de Partners y, a continuación, cree la solicitud de soporte técnico en el Azure Portal. 

>[!NOTE]
>Soporte técnico de Microsoft agentes pueden pedirle que proporcione el identificador de reserva y el ID. de pedido de reserva. Puede encontrar esta información en la página de **propiedades** de la reserva en el Azure portal.

1. Para empezar, seleccione **customers (clientes** ) en el menú del centro de Partners y seleccione el cliente que desea un reembolso. 

2. En la página de detalles del cliente, seleccione **reservas de Azure** y, después, seleccione la reserva específica que el cliente desea reembolsar.  

3. En **acciones**, seleccione **reembolso** para ir al registro de reserva del cliente en el Azure portal e iniciar una solicitud de soporte técnico.  

4. En la página **nueva solicitud de soporte técnico** , siga los pasos que se indican a continuación para solicitar un reembolso. Seleccione **siguiente** después de cada paso. 

   |**Step**                    |**Selecciones**    |
   |:---------------------------|:-----------------|
   |**1 conceptos básicos**                |Tipo de problema: facturación.  |
   |**2 problema**               |Tipo de problema: administración de reserva. Categoría: intercambios y reembolsos. |
   |**3 información de contacto**   |Seleccione sus preferencias y escriba la información necesaria. 

5. Seleccione **Crear** cuando haya terminado.

## <a name="azure-reservations-resources"></a>Recursos de reservas de Azure

|**Para información acerca de**   |**Lee esto**    |
|:-----------------------------|:-----------------|
|Información general sobre las reservas de Azure en CSP  | [Vender Microsoft Azure instancias reservadas](azure-reservations.md) |
|Compra de reservas de Azure para sus clientes en el centro de Partners   | [Comprar reservas de Azure](azure-reservations-buying.md) |
|Determinar el tamaño correcto de la máquina virtual y comprobar el uso de la máquina virtual del cliente   | [Tamaño de máquina virtual para el uso máximo de reserva de Azure](azure-usage.md)   |
|Compra de reservas de Azure mediante la API del centro de Partners | [Comprar Azure Reserved VM instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) en la documentación para desarrolladores del centro de Partners   |
|Otorgar permiso a los clientes para comprar sus propias reservas de Azure a partir de una suscripción que haya adquirido. | [Conceder permiso a los clientes para que compren sus propias reservas de Azure](give-customers-permission.md)   |

