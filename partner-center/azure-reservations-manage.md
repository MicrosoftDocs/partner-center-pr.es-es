---
title: Administración de reservas de Azure para clientes
description: Obtenga información sobre cómo administrar reservas de Azure para un cliente, incluido cómo cancelar una reserva, intercambiar una reserva o solicitar un reembolso.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 1184b199d6235dd1d16fe981000bae44b797f76a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149492"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Administración, cancelación, intercambio o reembolso Microsoft Azure reservas para clientes

**Roles adecuados:** agente de administración | Administrador global | Agente del departamento de soporte técnico | Agente de ventas | Administrador de administración de usuarios

En este artículo se explica cómo administrar las reservas de Azure para un cliente, incluido cómo cancelar una reserva, intercambiar una reserva o solicitar un reembolso.

> [!NOTE]
> Este artículo solo se aplica a los asociados del programa Proveedor de soluciones en la nube (CSP). Los clientes que usan otros tipos de suscripciones (por ejemplo, suscripciones de pago por uso, individuales, Contrato de cliente de Microsoft o Contrato Enterprise) deben leer en su lugar esta documentación de [reservas de Azure](/azure/cost-management-billing/reservations).

Para administrar las reservas de Azure de sus clientes después de la compra, seleccionará el cliente y la reserva que desea administrar en Centro de partners y, a continuación, hará cambios en la reserva en la Azure Portal.

1. Para empezar, seleccione **Clientes en** el menú Centro de partners y, a continuación, seleccione el cliente cuyas reservas desea administrar. 

2. En el menú de la página de detalles del cliente, seleccione **Reservas de Azure** y, a continuación, seleccione la reserva específica que desea administrar.  

3. En **Acciones,** seleccione **Administrar** para ir al registro de reserva del cliente en el Azure Portal. En la página de detalles de la reserva, siga estos pasos para completar las tareas.  

    | **Select**   | **To**    |
    |:-----------------------------|:-----------------|
    | **Información general**   | Vea los detalles de la reserva de un cliente, incluida la fecha de expiración, el ámbito y los datos de uso. **NOTA** Seleccione **Reembolso** para crear una solicitud de soporte técnico para un reembolso prorrateada. Seleccione **Exchange** para crear una solicitud de soporte técnico para intercambiar la parte no utilizada del período de reserva.  
    | **Control de acceso (IAM)**   | Administrar el acceso a la información de reserva del cliente.|
    | **Configuración**   | Cambie el ámbito de la reserva o la suscripción de Azure a la que está asociada la reserva.    |
    | **Propiedades**   | Vea las propiedades de la reserva y copie en el Portapapeles el identificador de reserva y el identificador del pedido de reserva. **NOTA** El soporte técnico puede solicitarle el identificador de reserva y el identificador del pedido de reserva cuando solicite soporte técnico en nombre de un cliente.    |
    | **Nueva solicitud de soporte técnico**    | Solicite ayuda a Soporte técnico de Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Cancelación o intercambio de una reserva

Si en algún momento las necesidades empresariales de un cliente cambian, es posible que quiera cancelar una reserva y obtener un reembolso o intercambiar el importe del reembolso prorrateado de una reserva que se usará para el precio de una nueva reserva.

En ambos escenarios, Microsoft le devuelve el importe para que pueda administrar las transacciones financieras resultantes con sus clientes. Microsoft no se pondrá en contacto directamente con los clientes sobre facturación, cancelaciones o reembolsos.

### <a name="how-cancellations-work"></a>Cómo funcionan las cancelaciones

Los clientes pueden solicitar cancelar una reserva en cualquier momento (el importe del reembolso está límite en 50 000 USD al año). La cancelación de una reserva permite al cliente devolver el importe de los meses restantes de una reserva de Azure por una tarifa de terminación anticipada. El saldo prorrateado restante, menos el precio de terminación anticipada, se devuelve a su cuenta para que pueda devolver la cuenta del cliente. 

Consulte a continuación los detalles de cancelación y las tarifas.


|**Fecha de cancelación**<br> (días)   |**Uso**    |**Crédito**  |**Finalización anticipada**<br> individual    |**Límite de reembolso** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 o menos                         | No          | 100 %       | No                              | 50 000 USD   |
|5 o menos                         | Sí         | Prorrateada  | No                              | 50 000 USD   |
|Más de 5                        | No          | Prorrateada  | 12 %                             | 50 000 USD   |
|Más de 5                        | Sí         | Prorrateada  | 12 %                             | 50 000 USD   |

### <a name="how-exchanges-work"></a>Cómo funcionan los intercambios 

Si un cliente quiere comprar una reserva diferente de la que le compró originalmente, puede solicitar un intercambio. El intercambio de una reserva puede ser una alternativa atractiva a cancelar una reserva, ya que permite al cliente usar el importe prorrateado del reembolso hasta el precio de la nueva reserva. 

El importe prorrateado del reembolso se ha devuelto a su cuenta para que pueda ofrecer al cliente un intercambio.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Solicitud de reembolso o cambio en nombre de un cliente

Para presentar una solicitud de soporte técnico para un reembolso o cambio en nombre de los clientes, seleccionará el cliente y la reserva en Centro de partners y, a continuación, creará la solicitud de soporte técnico en la Azure Portal. 

>[!NOTE]
>Soporte técnico de Microsoft agentes pueden pedirle que proporcione el identificador de reserva y el identificador del pedido de reserva. Puede encontrar esta información en la página Propiedades de la **reserva** en el Azure Portal.

1. Para empezar, seleccione **Clientes en** el menú Centro de partners y, a continuación, seleccione el cliente que quiere un reembolso. 

2. En la página de detalles del cliente, seleccione **Reservas de Azure** y, a continuación, seleccione la reserva específica que el cliente quiere que se devuelva.  

3. En **Acciones,** seleccione **Reembolso** para ir al registro de reserva del cliente en Azure Portal iniciar una solicitud de soporte técnico.  

4. En la **página Nueva solicitud de soporte** técnico, siga estos pasos para solicitar un reembolso. Seleccione **Siguiente** después de cada paso. 

   |**Step**                    |**Selecciones**    |
   |:---------------------------|:-----------------|
   |**1 Conceptos básicos**                |Tipo de problema: Facturación.  |
   |**2 Problema**               |Tipo de problema: Administración de reservas. Categoría: Intercambios y reembolsos. |
   |**3 Información de contacto**   |Seleccione sus preferencias y escriba la información necesaria. 

5. Seleccione **Crear** cuando haya terminado.

## <a name="azure-reservations-resources"></a>Recursos de reservas de Azure

|**Para información acerca de**   |**Lee esto**    |
|:-----------------------------|:-----------------|
|Introducción a las reservas de Azure en CSP  | [Vender Microsoft Azure instancias reservadas](azure-reservations.md) |
|Compra de reservas de Azure para sus clientes en Centro de partners   | [Compra de reservas de Azure](azure-reservations-buying.md) |
|Determinar el tamaño correcto de la máquina virtual y comprobar el uso de la máquina virtual del cliente   | [Tamaño de máquina virtual para el uso máximo de reservas de Azure](azure-usage.md)   |
|Compra de reservas de Azure mediante Centro de partners API | [Comprar Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) en la documentación Centro de partners desarrolladores   |
|Conceder a los clientes permiso para comprar sus propias reservas de Azure de una suscripción que haya adquirido para ellos. | [Conceder a los clientes permiso para comprar sus propias reservas de Azure](give-customers-permission.md)   |