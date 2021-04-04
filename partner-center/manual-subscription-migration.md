---
title: Migración de suscripciones de Dynamics 365 válidas
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo migrar desde suscripciones básicas de Dynamics 365 a una nueva suscripción antes de que expiren las suscripciones existentes.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 363c97b8c2b62e8d6b62cbe3b2807fb3c0ef3e38
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132747"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrar Dynamics 365 y Customer Engagement Plan de las versiones básicas (ofertas aptas) a las versiones más recientes

**Roles adecuados**

- Administrador global
- Administrador del control de usuarios
- Agente de administrador
- Agente de ventas

A partir del 1 de enero de 2019, los clientes con Dynamics 365 para el plan de participación de ventas y clientes de las suscripciones básicas (ofertas calificadas) ya no podrán renovar estas ofertas heredadas. las suscripciones existentes no se renovarán automáticamente cuando expiren. En la página de detalles de la suscripción, el estado de la suscripción cambiará a "expira el [fecha]" de "se renueva automáticamente en [fecha]". 

Para garantizar la continuidad de los clientes, debe realizar la transición de las suscripciones que van a expirar a una opción admitida, que se enumera a continuación. Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes.

Si usa la API (de la cresta o del centro de Partners), puede encontrar suscripciones que van a expirar mediante la evaluación de la fecha de finalización de la suscripción junto con la propiedad auto Renew = false. Las suscripciones en cuestión se establecerán en renovación automática = false el 1 de enero de 2019. Puede trasladar a los clientes a un nuevo plan en cualquier momento. 

### <a name="the-dynamics-365-offers-being-retired"></a>Se están retirando las ofertas de Dynamics 365

- Dynamics 365 for sales Enterprise Edition CRMOL Basic (oferta calificada)
- Dynamics 365 for sales Enterprise Edition CRMOL Basic (oferta calificada) para profesores
- Dynamics 365 for sales Enterprise Edition CRMOL Basic (oferta calificada) para estudiantes
- Dynamics 365 for sales Enterprise Edition (precios de la administración pública) CRMOL Basic (oferta calificada)
- Dynamics 365 for sales Enterprise Edition de SA for CRM Basic (oferta calificada)
- Dynamics 365 for sales Enterprise Edition de SA for CRM Basic (oferta calificada) para profesores
- Dynamics 365 for sales Enterprise Edition de SA for CRM Basic (oferta calificada) para estudiantes
- Dynamics 365 for sales Enterprise Edition (precios de la administración pública) de SA for CRM Basic (oferta calificada)
- Dynamics 365 for sales Enterprise Edition Add-On para CRM Basic (oferta calificada)
- Dynamics 365 for sales Enterprise Edition Add-On para CRM Basic (oferta calificada) para profesores
- Dynamics 365 for sales Enterprise Edition Add-On para CRM Basic (oferta calificada) para estudiantes
- Dynamics 365 for sales Enterprise Edition (precios para la administración pública) Add-On para CRM básico (oferta calificada)
- Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (oferta calificada)
- Dynamics 365 Customer Engagement plan Enterprise Edition (precios para la administración pública) CRMOL Basic (oferta calificada)
- Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (oferta calificada) para estudiantes
- Dynamics 365 Customer Engagement plan Enterprise Edition CRMOL Basic (oferta calificada) para profesores
- Dynamics 365 Customer Engagement plan Enterprise Edition de SA for CRM Basic (oferta calificada)
- Dynamics 365 Customer Engagement plan Enterprise Edition (precios de la administración pública) de SA for CRM Basic (oferta calificada)
- Dynamics 365 Customer Engagement plan Enterprise Edition de SA for CRM Basic (oferta calificada) para estudiantes
- Dynamics 365 Customer Engagement plan Enterprise Edition de SA for CRM Basic (oferta calificada) para profesores
- Dynamics 365 Customer Engagement plan Enterprise Edition Add-On para CRM Basic (oferta calificada)
- Dynamics 365 Customer Engagement plan Enterprise Edition (precios para la administración pública) Add-On para CRM básico (oferta calificada)
- Dynamics 365 Customer Engagement plan Enterprise Edition Add-On para CRM Basic (oferta calificada) para estudiantes
- Dynamics 365 Customer Engagement plan Enterprise Edition Add-On para CRM Basic (oferta calificada) para profesores



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for sales/Customer Engagement plan from Basic (ofertas calificadas) planes de reemplazo

**Ofertas retiradas**   

- Dynamics 365 para ventas de CRM Basic o CRMOL Basic (oferta calificada)
- Plan de Dynamics 365 Customer Engagement de CRM Basic o CRMOL Basic (oferta calificada)

**Opciones de reemplazo**
- Dynamics 365 for sales Professional (nuevo)
- Dynamics 365 for sales Professional (nuevo)
- Dynamics 365 for Customer Service
- Plan de Dynamics 365 Customer Engagement o
- Miembros del equipo de Dynamics 365



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
 

 



