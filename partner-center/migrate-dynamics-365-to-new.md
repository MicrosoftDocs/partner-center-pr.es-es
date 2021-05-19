---
title: Migración de Dynamics 365 Business Edition
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo migrar ofertas de Dynamics 365 Business Edition a versiones más recientes antes de que expiren.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8232ab165ea68ebefdfbb30f3ac52c907e1b7278
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151532"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migración de ofertas de Dynamics 365 Business Edition a versiones más recientes

**Roles adecuados:** administrador global | Administrador de administración de | Agente de administración | Agente de ventas

A partir del 1 de enero de 2019, los clientes con suscripciones de Dynamics 365 Business Edition ya no pueden renovarse en estas ofertas heredadas. Las suscripciones existentes no se renovarán automáticamente cuando expiren. En la página de detalles de la suscripción, el estado de la suscripción cambiará a "Expira el [fecha]" de "Renovación automática el [fecha]".

Para garantizar la continuidad de los clientes, debe realizar la transición de los que tienen suscripciones que expiran a una opción compatible, que se muestra a continuación. Se recomienda mover clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones del servicio para los clientes.

Si usa la API (YA SEATE o Centro de partners), puede encontrar suscripciones que expiran evaluando la fecha de finalización de la suscripción junto con la propiedad renovación automática = False. Las suscripciones en cuestión se establecerán en auto renew=False el 1 de enero de 2019. Puede trasladar clientes a un nuevo plan en cualquier momento. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Dynamics 365 Business Edition que se va a retirar

- Dynamics 365 for Finance and Operations, Business Edition
- Dynamics 365 for Team Members, edición Business

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central: nuevas ofertas de Dynamics 365 Business Edition

Con las nuevas ofertas de Dynamics Business Central, los clientes pueden conectar sus finanzas, ventas, servicio y operaciones para optimizar los procesos empresariales, mejorar las interacciones de los clientes y tomar mejores decisiones. Dynamics 365 Business Central está basado en la nube y solo está disponible a través Proveedor de soluciones en la nube asociados del programa csp (CSP).
Los clientes de Dynamics 365 Business Edition pueden recibir precios de transición con descuento para las nuevas ofertas de Business Central hasta el 30 de junio de 2020.

## <a name="transition-customers-to-new-product-plans"></a>Clientes de transición hacia los nuevos planes de productos

 El traslado de clientes de SKU retiradas a otras más recientes requiere los pasos siguientes en este orden:

- Comprar la nueva suscripción
- Reasignación de licencias de usuario actuales
- Cancelación de una suscripción antigua

## <a name="purchase-the-new-plan-for-your-customer"></a>Compra del nuevo plan para el cliente

1. Seleccione **Clientes** en el panel de navegación izquierdo y, a continuación, seleccione el cliente que desea trasladar a la nueva suscripción.
2. Seleccione **Agregar suscripción.**
3. Seleccione la suscripción que desea comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, **seleccione Enviar**. 

El cliente tendrá ahora la suscripción anterior y la nueva. El siguiente paso consiste en reasignar licencias a los usuarios del cliente.

1. Seleccione **Clientes** en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.
2. Seleccione **Usuarios y licencias.**
3. Para reasignar una licencia a un usuario, selecciónelo y, a continuación, **seleccione Administrar licencias.** 
4. En  la página Administrar licencias, desactive la casilla Dynamics 365 for Sales/ Customer Engagement Plan from Basic (Qualified Offer) license (Plan de Dynamics 365 for Sales/Customer Engagement plan from Basic [Oferta calificada]) y seleccione un nuevo plan de servicio para la suscripción a la que se traslada el cliente. 
5. Seleccione **Submit** (Enviar). Lo hará para cada usuario que necesite la nueva licencia. 

Una vez que haya movido las licencias a la nueva suscripción, puede cancelar la suscripción anterior. 

1. Seleccione **Clientes** en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.
2. En la página de detalles de la suscripción, establezca la suscripción antigua en **Suspendido** y seleccione **Enviar**.

La suscripción anterior ahora está suspendida y la nueva suscripción está activa. La suscripción suspendida se desaprovisionará automáticamente después de 120 días. El cliente no incurrirá en costos adicionales por la suscripción anterior.
