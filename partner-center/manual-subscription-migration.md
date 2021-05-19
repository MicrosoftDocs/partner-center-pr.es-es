---
title: Migración de suscripciones de Dynamics 365 calificadas
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo migrar de suscripciones de Dynamics 365 básicas y calificadas a una nueva suscripción antes de que expiren las suscripciones existentes.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5ba6992eff64031aed0dafeb5a5010983396ab63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151651"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrar Dynamics 365 y Customer Engagement Plan de las versiones básicas (ofertas aptas) a las versiones más recientes

**Roles adecuados:** administrador global | Administrador de administración de | Agente de administración | Agente de ventas

A partir del 1 de enero de 2019, los clientes con Dynamics 365 for Sales/Customer Engagement Plan de suscripciones básicas (ofertas calificadas) ya no podrán renovar estas ofertas heredadas. Las suscripciones existentes no se renovarán automáticamente cuando expiren. En la página de detalles de la suscripción, el estado de la suscripción cambiará a "Expira el [fecha]" de "Renovación automática el [fecha]". 

Para garantizar la continuidad de los clientes, debe realizar la transición de los que tienen suscripciones que expiran a una opción compatible, que se muestra a continuación. Se recomienda mover clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones del servicio para los clientes.

Si usa la API (YA SEATE o Centro de partners), puede encontrar suscripciones que expiran evaluando la fecha de finalización de la suscripción junto con la propiedad renovación automática = False. Las suscripciones en cuestión se establecerán en auto renew=False el 1 de enero de 2019. Puede trasladar clientes a un nuevo plan en cualquier momento. 

### <a name="the-dynamics-365-offers-being-retired"></a>Las ofertas de Dynamics 365 que se retiran

- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (oferta calificada)
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Oferta calificada) para profesores
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (Oferta calificada) para estudiantes
- Dynamics 365 for Sales Enterprise Edition (precios gubernamentales) CRMOL Basic (oferta calificada)
- Dynamics 365 for Sales Enterprise Edition from SA for CRM Basic (Oferta calificada)
- Dynamics 365 for Sales Enterprise Edition from SA for CRM Basic (Oferta calificada) para profesores
- Dynamics 365 for Sales Enterprise Edition from SA for CRM Basic (Oferta calificada) para estudiantes
- Dynamics 365 for Sales Enterprise Edition (precios gubernamentales) de SA para CRM Basic (oferta calificada)
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (oferta calificada)
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (oferta calificada) para profesores
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (oferta calificada) para estudiantes
- Dynamics 365 for Sales Enterprise Edition (precios gubernamentales) Add-On para CRM Basic (oferta calificada)
- Plan de Dynamics 365 Customer Engagement Enterprise Edition CRMOL Basic (oferta calificada)
- Plan de Dynamics 365 Customer Engagement Enterprise Edition (precios gubernamentales) CRMOL Basic (oferta calificada)
- Plan de Dynamics 365 Customer Engagement Enterprise Edition CRMOL Basic (oferta calificada) para estudiantes
- Plan de Dynamics 365 Customer Engagement Enterprise Edition CRMOL Basic (oferta calificada) para profesores
- Plan de Dynamics 365 Customer Engagement Enterprise Edition de SA para CRM Basic (oferta calificada)
- Plan de Dynamics 365 Customer Engagement Enterprise Edition (precios gubernamentales) de SA para CRM Basic (oferta calificada)
- Plan de Dynamics 365 Customer Engagement Enterprise Edition de SA for CRM Basic (oferta calificada) para estudiantes
- Plan de Dynamics 365 Customer Engagement Enterprise Edition de SA para CRM Basic (oferta calificada) para profesores
- Plan de Dynamics 365 Customer Engagement Enterprise Edition Add-On para CRM Basic (oferta calificada)
- Plan de Dynamics 365 Customer Engagement Enterprise Edition (precios gubernamentales) Add-On para CRM Basic (oferta calificada)
- Plan de Dynamics 365 Customer Engagement Enterprise Edition Add-On para CRM Basic (oferta calificada) para estudiantes
- Plan de Dynamics 365 Customer Engagement Enterprise Edition Add-On para CRM Basic (oferta calificada) para profesores



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Plan de Dynamics 365 for Sales/Customer Engagement de planes de reemplazo básicos (ofertas calificadas)

**Ofertas retiradas**   

- Dynamics 365 for Sales de CRM Basic o CRMOL Basic (oferta calificada)
- Plan de Dynamics 365 Customer Engagement de CRM Basic o CRMOL Basic (oferta calificada)

**Opciones de reemplazo**
- Dynamics 365 for Sales Professional (NUEVO)
- Dynamics 365 for Sales Professional (NUEVO)
- Dynamics 365 for Customer Service
- Plan de Dynamics 365 Customer Engagement o
- Miembros del equipo de Dynamics 365



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
4. En  la página Administrar licencias, desactive la casilla Dynamics 365 for Sales/Customer Engagement Plan from Basic (Qualified Offer) license (Plan de Dynamics 365 for Sales/Customer Engagement plan from Basic [Oferta calificada]) y seleccione un nuevo plan de servicio para la suscripción a la que el cliente va a pasar. 
5. Seleccione **Submit** (Enviar). Lo hará para cada usuario que necesite la nueva licencia. 

Una vez que haya movido las licencias a la nueva suscripción, puede cancelar la suscripción anterior. 

1. Seleccione **Clientes** en el panel de navegación izquierdo y, a continuación, seleccione el cliente que va a mover.
2. En la página de detalles de la suscripción, establezca la suscripción antigua en **Suspendido** y seleccione **Enviar**.

La suscripción anterior ahora está suspendida y la nueva suscripción está activa. La suscripción suspendida se desaprovisionará automáticamente después de 120 días. El cliente no incurrirá en costos adicionales por la suscripción anterior.
 

 



