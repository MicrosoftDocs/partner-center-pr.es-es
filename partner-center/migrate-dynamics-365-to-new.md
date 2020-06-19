---
title: Migración de Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo migrar ofertas de Dynamics 365 Business Edition calificadas a versiones más recientes antes de que expiren.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
Keywords: Ofertas de Dynamics 365, renovar ofertas, nuevas SKU de Dynamics 365
ms.openlocfilehash: 9675f607d183c5d427371de4f09f088fd267c573
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/18/2020
ms.locfileid: "84992082"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migración de ofertas de Dynamics 365 Business Edition a versiones más recientes

**Se aplica a**

- Centro de partners

**Roles adecuados**
- Administrador global
- Administrador de usuarios
- Agente de administrador
- Agente de ventas

A partir del 1 de enero de 2019, los clientes con suscripciones de Dynamics 365 Business Edition ya no podrán renovar en estas ofertas heredadas. las suscripciones existentes no se renovarán automáticamente cuando expiren. En la página de detalles de la suscripción, el estado de la suscripción cambiará a "expira el [fecha]" de "se renueva automáticamente en [fecha]".

Para garantizar la continuidad de los clientes, debe realizar la transición de las suscripciones que van a expirar a una opción admitida, que se enumera a continuación. Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes.

Si usa la API (de la cresta o del centro de Partners), puede encontrar suscripciones que van a expirar mediante la evaluación de la fecha de finalización de la suscripción junto con la propiedad auto Renew = false. Las suscripciones en cuestión se establecerán en renovación automática = false el 1 de enero de 2019. Puede trasladar a los clientes a un nuevo plan en cualquier momento. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Las ediciones Business de Dynamics 365 que se están retirando

- Dynamics 365 for Finance and Operations, Business Edition
- Dynamics 365 for Team Members, edición Business

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business central: las ofertas nuevas de Dynamics 365 Business Edition

Con las nuevas ofertas de Dynamics Business central, sus clientes pueden conectar sus finanzas, ventas, servicios y operaciones para simplificar los procesos empresariales, mejorar las interacciones de los clientes y tomar mejores decisiones. Dynamics 365 Business central se basa en la nube y está disponible a través de los asociados de programas del proveedor de soluciones en la nube (CSP).
Los clientes de Dynamics 365 Business Edition pueden recibir precios de transición con descuento para las nuevas ofertas de Business central hasta el 30 de junio de 2020.

## <a name="transition-customers-to-new-product-plans"></a>Clientes de transición hacia los nuevos planes de productos

 El traslado de los clientes de las SKU retiradas a otras más recientes requiere los pasos siguientes en este orden:

- Comprar la nueva suscripción
- Reasignar licencias de usuario actuales
- Cancelar suscripción anterior

## <a name="purchase-the-new-plan-for-your-customer"></a>Compre el nuevo plan para su cliente

1. Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que desea desplazar a la nueva suscripción.
2. Seleccione **Agregar suscripción**.
3. Seleccione la suscripción que desea comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, seleccione **submit (enviar**). 

El cliente tendrá ahora la suscripción antigua y la nueva. El siguiente paso consiste en volver a asignar las licencias a los usuarios del cliente.

1. Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.
2. Seleccione **usuarios y licencias**.
3. Para reasignar una licencia a un usuario, seleccione el usuario y, a continuación, seleccione **administrar licencias**. 
4. En la página **administrar licencias** , desactive la casilla Dynamics 365 for sales/Customer Engagement plan from Basic (oferta calificada) y seleccione un nuevo plan de servicio para la suscripción a la que está pasando el cliente. 
5. Seleccione **Submit** (Enviar). Lo hará para cada usuario que necesite la nueva licencia. 

Una vez que haya migrado las licencias a la nueva suscripción, puede cancelar la suscripción anterior. 

1. Seleccione **customers (clientes** ) en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.
2. En la página de detalles de la suscripción, establezca la suscripción antigua en **Suspended** y seleccione **submit (enviar**).

La suscripción anterior se ha suspendido y la nueva suscripción está activa. La suscripción suspendida se desaprovisionará automáticamente después de 120 días. El cliente no incurrirá en costos adicionales por la suscripción anterior.
