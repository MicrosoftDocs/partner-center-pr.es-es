---
title: Migrar de Dynamics 365 y Customer Engagement planear de Basic (ofertas completas) para las versiones más recientes | Centro de partners
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 para Sales / ya no se puede renovar el Plan de Engagement de cliente desde suscripciones Basic (ofrece completo).
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Las ofertas de Dynamics 365, renovar las ofertas, nuevas SKU de Dynamics 365
ms.openlocfilehash: e5128abe71cfab4e2cdabb0cafcd5fd7df56b116
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134405"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrar Dynamics 365 y el plan Customer Engagement desde las versiones básicas (ofertas calificados) a versiones más recientes

**Se aplica a**

-  Centro de partners

Efectivo el 1 de enero de 2019, los clientes con Dynamics 365 para Sales / Customer Engagement Plan desde suscripciones Basic (ofrece completo) ya no se puede renovar estas ofertas heredadas; las suscripciones existentes no se renovarán automáticamente cuando expiran. En la página de detalles de la suscripción, el estado de la suscripción cambiará a "Expira el [fecha]" de "Renueva automáticamente el [fecha]". 


Para garantizar la continuidad de los clientes, debe realizar la transición aquellos con las suscripciones que van a expirar a una opción admitida, que se enumeran a continuación. Te recomendamos mover los clientes a las nuevas suscripciones antes de la fecha de finalización para evitar interrupciones en el servicio a los clientes.

Si usa la API (CREST o centro de partners), puede encontrar la renovación de suscripciones caducadas mediante la evaluación de la fecha de finalización de la suscripción, junto con el auto = False property. Las suscripciones en cuestión se establecerá en auto renovar = False, 1 de enero de 2019. Puedes mover a los clientes a un plan nuevo en cualquier momento. 

### <a name="the-dynamics-365-offers-being-retired"></a>El Dynamics 365 ofrece retirará

- Dynamics 365 para ventas Enterprise Edition CRMOL Basic (oferta completa)
- Dynamics 365 para ventas Enterprise Edition CRMOL básico (oferta completa) para profesores
- Dynamics 365 para ventas Enterprise Edition CRMOL básico (oferta completa) para estudiantes
- Dynamics 365 para ventas Enterprise Edition (precios para administración pública) CRMOL Basic (oferta completa)
- Dynamics 365 para ventas Enterprise Edition de SA para CRM Basic (oferta completa)
- Dynamics 365 para ventas Enterprise Edition de SA para CRM Basic (oferta completa) para profesores
- Dynamics 365 para ventas Enterprise Edition de SA para CRM Basic (oferta completa) para estudiantes
- Dynamics 365 para ventas de Enterprise Edition (precios para administración pública) de SA para CRM Basic (oferta completa)
- Dynamics 365 para el complemento de edición Enterprise de ventas para CRM Basic (oferta completa)
- Dynamics 365 para el complemento de edición Enterprise de ventas para CRM Basic (oferta completa) para profesores
- Dynamics 365 para el complemento de edición Enterprise de ventas para CRM Basic (oferta completa) para estudiantes
- Dynamics 365 para el complemento de ventas de Enterprise Edition (precios para administración pública) para CRM Basic (oferta completa)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL básico (oferta completa)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (precios para administración pública) CRMOL básico (oferta completa)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL básico (oferta completa) para estudiantes
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL básico (oferta completa) para profesores
- Dynamics 365 Customer Engagement Plan Enterprise Edition de SA para CRM Basic (oferta completa)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (precios para administración pública) de SA para CRM Basic (oferta completa)
- Dynamics 365 Customer Engagement Plan Enterprise Edition de SA para CRM Basic (oferta completa) para estudiantes
- Dynamics 365 Customer Engagement Plan Enterprise Edition de SA para CRM Basic (oferta completa) para profesores
- Complemento Dynamics 365 Customer Engagement Plan Enterprise Edition para CRM Basic (oferta completa)
- Complemento Dynamics 365 Customer Engagement Plan Enterprise Edition (precios para administración pública) para CRM Basic (oferta completa)
- Dynamics 365 Customer Engagement Plan Enterprise Edition complemento para CRM Basic (oferta completa) para estudiantes
- Dynamics 365 Customer Engagement Plan Enterprise Edition complemento CRM Basic (oferta completa) para profesores



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 para Sales / planes de Customer Engagement planear de reemplazo de Basic (ofrece completo)

**Ofertas retiradas**   

- Dynamics 365 para ventas de CRM Basic o CRMOL Basic (oferta completa)
- Dynamics 365 Customer Engagement Plan de CRM Basic o CRMOL Basic (oferta completa)

**Opciones de reemplazo**
- Dynamics 365 para profesionales de ventas (nuevo)
- Dynamics 365 para profesionales de ventas (nuevo)
- Dynamics 365 para el servicio al cliente
- Plan de Dynamics 365 Customer Engagement o
- Miembros del equipo de Dynamics 365



## <a name="transition-customers-to-new-product-plans"></a>Clientes de transición hacia los nuevos planes de productos

Mover a los clientes de SKU retiradas a los más recientes requiere los pasos siguientes en este orden:

- Comprar la nueva suscripción
- Reasignar licencias de usuario actuales
- Cancelar suscripción antigua

## <a name="purchase-the-new-plan-for-your-customer"></a>El nuevo plan de compra para su cliente

1. Seleccione **clientes** desde el panel de navegación izquierdo y, a continuación, seleccione el cliente que desea mover a la nueva suscripción.
2. Seleccione **Agregar suscripción**.
3. Selecciona la suscripción que quieras adquirir del catálogo (en este caso, una de las opciones que se indican más arriba), escribe el número de licencias y, a continuación, **Enviar**. 

El cliente tendrá ahora la suscripción antigua y una nueva. El siguiente paso es volver a asignar licencias a los usuarios del cliente.

1. Seleccione **clientes** desde el panel de navegación izquierdo y, a continuación, seleccione el cliente que está moviendo.
2. Selecciona **Usuarios y licencias**.
3. Para reasignar una licencia a un usuario, seleccione el usuario y, a continuación, seleccione **administrar licencias**. 
4. En el **administrar licencias** página, desactive el Dynamics 365 para Sales / Plan de compromiso del cliente de Basic (oferta completo) casilla de verificación de licencia y seleccione un nuevo plan de servicio para la suscripción que el cliente se mueve a. 
5. Selecciona **Enviar**. Hará esto para cada usuario que necesita la nueva licencia. 

Una vez que haya movido las licencias a través a la nueva suscripción puede cancelar la suscripción antigua. 

1. Seleccione **clientes** desde el panel de navegación izquierdo y, a continuación, seleccione el cliente que está moviendo.
2. En la página de detalles de suscripción, establezca la suscripción antigua **Suspended** y seleccione **enviar**.

Ahora se suspende la suscripción antigua y la nueva suscripción está activa. Se cancelará el aprovisionamiento de la suscripción suspendida automáticamente después de 120 días. Su cliente no incurrirá en ningún costo adicional para la suscripción antigua.
 

 



