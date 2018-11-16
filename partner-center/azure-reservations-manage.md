---
title: Administrar reservas de Microsoft Azure en nombre de los clientes | Centro de partners
ms.topic: article
ms.date: 10/29/2018
Description: Managing Azure reservations on behalf of your customers.
author: v-petand
ms.author: v-petand
keywords: Azure, reservas, administrar, facturación, comprar, Cancelar, exchange, tarifa de finalización anticipada
ms.localizationpriority: medium
ms.openlocfilehash: fde21951dacab70a9f9b03d853647aabcc40d9af
ms.sourcegitcommit: 7a68540d64d17c4d9139da4f94d679f9d91b67c4
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/15/2018
ms.locfileid: "7011415"
---
# <a name="manage-microsoft-azure-reservations-on-behalf-of-your-customers"></a>Administrar reservas de Microsoft Azure en nombre de los clientes

**Se aplica a**

-  Centro de partners
-  Portal de Microsoft Azure
-  Partners de CSP

Para administrar Azure reservations posterior tus clientes a la compra, tendrás que selecciona el cliente y la reserva que quieres administrar en el centro de partners y, a continuación, realizar cambios en la reserva en el portal de Azure. 

1. Para empezar, selecciona **los clientes** en el menú del centro de partners y, a continuación, selecciona al cliente cuyas reservas quieres administrar. 

2. En el menú de la página de detalles del cliente, selecciona **reservas de Azure** y, a continuación, selecciona la reserva específica que quieras administrar.  

3. En **Acciones**, selecciona **Administrar** para ir al registro de reserva del cliente en Azure Portal. En la página de detalles de la reserva, sigue los pasos siguientes para completar tareas.  

    | **Selecciona**   | **Para**    |
    |:-----------------------------|:-----------------|
    | **Introducción**   | Ver detalles de la reserva de un cliente, incluidos la fecha de expiración, el ámbito y los datos de uso. **NOTA** Selecciona **Reembolso** para crear una solicitud de soporte para un reembolso prorrateado. Selecciona **Exchange** para crear una solicitud de soporte para intercambiar la parte no usada del término de reserva.  
    | **Access Control (IAM)**   | Administrar el acceso a la información de la reserva del cliente.|
    | **Configuración**   | Cambiar el ámbito de la reserva o la suscripción de Azure a la que está asociada la reserva.    |
    | **Propiedades**   | Ver propiedades de la reserva y copiar en el Portapapeles el id. de la reserva y el id. del pedido de reserva. **NOTA** El departamento de soporte puede solicitarle el id. de reserva y el id. del pedido de reserva al solicitar soporte en nombre de un cliente.    |
    | **Nueva solicitud de soporte técnico**    | Solicitar ayuda del soporte técnico de Microsoft.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Cancelar o cambiar una reserva 

Si en cualquier momento cambien las necesidades empresariales de un cliente, es posible que quieren cancelar una reserva y obtener un reembolso o cambiar el importe del reembolso prorrateado de una reserva para usarlo para el precio de una nueva reserva.

En ambos de estos escenarios, Microsoft reembolsos la cantidad que, para que, a continuación, puede administrar las transacciones financieras resultantes con los clientes. Microsoft no ponerse en contacto con los clientes directamente sobre facturación, las cancelaciones o reembolsos.   
 

**Cómo funcionan las cancelaciones**

Los clientes pueden solicitar cancelar una reserva en cualquier momento (importe del reembolso limitado a 50 000 $ al año). Cancelar una reserva permite al cliente devolver la cantidad de los demás meses de una reserva de Azure para una cuota de finalización anticipada. El balance prorrateado restante, menos la cuota de finalización anticipado, se devuelve a tu cuenta para que pueda reembolsar la cuenta del cliente. 

Consulta a continuación para las cuotas y los detalles de la cancelación.


|**Fecha de cancelación**<br> (en días)   |**Usage**    |**Crédito**  |**Finalización anticipada**<br> de empresa    |**Límite de reembolso** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 o menos                         | No          | 100%       | No                              | 50000 USD   |
|5 o menos                         | Sí         | Prorrateado  | No                              | 50000 USD   |
|Más de 5                        | No          | Prorrateado  | 12%                             | 50000 USD   |
|Más de 5                        | Sí         | Prorrateado  | 12%                             | 50000 USD   |


**Cómo funcionan los intercambios** 

Si un cliente quiere comprar una reserva diferente a la que has comprados originalmente del usuario, puede solicitar un intercambio. Intercambiar una reserva puede ser una alternativa atractiva para cancelar una reserva, ya que permite al cliente usar el importe del reembolso prorrateado hacia el precio de la reserva nuevo. 

El importe del reembolso prorrateado se abonará a tu cuenta para que el cliente puede ofrecer un intercambio.


## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Solicitar un reembolso o cambio en nombre de un cliente 

Para presentar una solicitud de soporte técnico para un reembolso o cambio en nombre de los clientes, tendrás seleccionar el cliente y la reserva en el centro de partners y, a continuación, crear la solicitud de soporte técnico en el portal de Azure. 

>[!NOTE]
>Soporte técnico de Microsoft puede pedirte proporcionar el id. de reserva y el id. del pedido de reserva. Puedes encontrar esta información en la página **Propiedades** de la reserva del Azure Portal. 

1. Para empezar, selecciona **los clientes** en el menú del centro de partners y, a continuación, selecciona al cliente que quiere un reembolso. 

2. En la página de detalles del cliente, selecciona **Azure Reservations** y, a continuación, la reserva específica que el cliente quiera que se le reembolse.  

3. En **las acciones**, selecciona **reembolsar** para ir al registro de reserva del cliente en Azure portal e iniciar una solicitud de soporte técnico.  

4. En la página **Nueva solicitud de soporte técnico**, sigue los pasos siguientes para solicitar un reembolso. Selecciona **Siguiente** después de cada paso. 

    |**Paso**                    |**Selecciones**    |
    |:---------------------------|:-----------------|
    |**1 Conceptos básicos**                |Tipo de problema: facturación  |
    |**2 Problema**               |Tipo de problema: administración de reservas. Categoría: intercambios y reembolsos. |
    |**3 Información de contacto**   |Selecciona tus preferencias y escribe la información necesaria. 

5.  Selecciona **Crear** cuando termines.

## <a name="azure-reservations-resources"></a>Recursos de Azure Reservations
|**Para obtener información acerca de**   |**Lee esto**    |
|:-----------------------------|:-----------------|
|Reservas de Azure en introducción de CSP  | [Vender instancias reservadas de Azure de Microsoft](azure-reservations.md) |
|Comprar reservas de Azure para tus clientes en el centro de partners   |[Comprar reservas de Azure](azure-reservations-buying.md) |
|Determinación del tamaño correcto de la máquina virtual y comprobar el uso de la máquina virtual del cliente   |[Cambio de tamaño de la VM para el uso máximo de reserva de Azure](azure-usage.md)   |
|Comprar Azure Reservations con la API del Centro de partners | [Purchase Azure Reserved VM Instances (Comprar Azure Reserved VM Instances)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) en la documentación de desarrolladores del Centro de partners

