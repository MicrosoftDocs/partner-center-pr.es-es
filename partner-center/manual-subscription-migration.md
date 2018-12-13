---
title: Migrar de Dynamics 365 y el Plan de participación de clientes de Basic (ofertas completos) a versiones más recientes | El centro de partners
ms.topic: article
ms.date: 12/12/2018
description: Dynamics 365 for Sales o ya no se puede renovar el Plan de participación de cliente de suscripciones de Basic (ofrece completo).
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: b4b25dd80a684c9060b28461a9e6f594651ae224
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968275"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrar de Dynamics 365 y el Plan de participación de clientes de Basic (ofertas completos) a versiones más recientes

**Se aplica a**

-  Centro de partners

Efectiva el 1 de enero de 2019, los clientes con Dynamics 365 for Sales o Plan de participación de cliente de suscripciones de Basic (ofrece completo) ya no se pueden renovar estas ofertas heredadas; las suscripciones existentes no se renovarán automáticamente cuando expiren. En la página de detalles de la suscripción, el estado cambiará a "Expira el [fecha]" desde "Se renovará automáticamente en [fecha]". 


Para garantizar la continuidad para los clientes, debes pasarlas personas con suscripciones vayan a caducar a una opción compatible, como aparece a continuación. Recomendamos pasar a los clientes a las nuevas suscripciones, antes de la fecha de finalización anual de la suscripción, para evitar interrupciones del servicio a los clientes.

Si usas la API (CREST o centro de partners), puedes encontrar renovar suscripciones vayan a caducar evaluando la fecha de finalización de la suscripción junto con la automática = False propiedad. Las suscripciones en cuestión se establecerá automáticamente renovar = False el 1 de enero de 2019. Puedes mover a los clientes a un plan nuevo en cualquier momento. 

### <a name="the-dynamics-365-offers-being-retired"></a>El de Dynamics 365 ofrece que se retiran

- Dynamics 365 ventas Enterprise Edition CRMOL Basic (calificado oferta)
- Dynamics 365 ventas Enterprise Edition CRMOL Basic (calificado oferta) para profesores
- Dynamics 365 ventas Enterprise Edition CRMOL Basic (calificado oferta) para estudiantes
- Dynamics 365 ventas Enterprise Edition (Government precios) CRMOL Basic (calificado oferta)
- Dynamics 365 para la edición Enterprise de venta de Microsoft software Assurance CRM Basic (calificado oferta)
- Dynamics 365 para la edición Enterprise de venta de Microsoft software Assurance CRM Basic (calificado oferta) para profesores
- Dynamics 365 para la edición Enterprise de venta de Microsoft software Assurance CRM Basic (calificado oferta) para estudiantes
- Dynamics 365 para Enterprise ventas (Government precios) de Microsoft software Assurance CRM Basic (calificado oferta)
- Dynamics 365 para el complemento de ventas de Enterprise Edition CRM Basic (calificado oferta)
- Dynamics 365 para el complemento de ventas de Enterprise Edition CRM Basic (calificado oferta) para profesores
- Dynamics 365 para el complemento de ventas de Enterprise Edition CRM Basic (calificado oferta) para estudiantes
- Dynamics 365 para el complemento de ventas de Enterprise Edition (Government precios) CRM Basic (calificado oferta)
- Dynamics 365 cliente Engagement Plan Enterprise Edition CRMOL Basic (calificado oferta)
- Dynamics 365 cliente Engagement Plan Enterprise Edition (Government precios) CRMOL Basic (calificado oferta)
- Dynamics 365 cliente Engagement Plan Enterprise Edition CRMOL Basic (calificado oferta) para estudiantes
- Dynamics 365 cliente Engagement Plan Enterprise Edition CRMOL Basic (calificado oferta) para profesores
- Dynamics 365 cliente Engagement Plan Enterprise Edition desde Microsoft software Assurance CRM Basic (calificado oferta)
- Dynamics 365 cliente Engagement Plan Enterprise Edition (Government precios) de Microsoft software Assurance CRM Basic (calificado oferta)
- Dynamics 365 cliente Engagement Plan Enterprise Edition desde Microsoft software Assurance CRM Basic (calificado oferta) para estudiantes
- Dynamics 365 cliente Engagement Plan Enterprise Edition desde Microsoft software Assurance CRM Basic (calificado oferta) para profesores
- Dynamics 365 cliente Engagement Plan Enterprise Edition complemento CRM Basic (calificado oferta)
- Dynamics 365 cliente Engagement Plan Enterprise Edition (Government precios) complemento CRM Basic (calificado oferta)
- Dynamics 365 cliente Engagement Plan Enterprise Edition complemento CRM Basic (calificado oferta) para estudiantes
- Dynamics 365 cliente Engagement Plan Enterprise Edition complemento CRM Basic (calificado oferta) para profesores



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales o los planes de participación de cliente previsto de reemplazo de Basic (ofrece completo)

**Retirada ofertas**   

- Dynamics 365 para las ventas de CRM Basic o CRMOL Basic (calificado oferta)
- Dynamics 365 Customer Engagement Plan de CRM Basic o CRMOL Basic (calificado oferta)

**Opciones de reemplazo**
- Dynamics 365 para profesionales de ventas (nuevo)
- Dynamics 365 para profesionales de ventas (nuevo)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer Engagement Plan o
- Miembros del equipo de Dynamics 365



## <a name="transition-customers-to-new-product-plans"></a>Pasar a los clientes a nuevos planes de producto

Mover los clientes desde SKU retiradas a unas más recientes que requiere los pasos siguientes en este orden:

- Comprar la nueva suscripción
- Reasignar licencias de usuario actuales
- Cancelar suscripción antigua

## <a name="purchase-the-new-plan-for-your-customer"></a>El nuevo plan de compra para el cliente

1. Selecciona **los clientes** desde el menú de navegación izquierdo y, a continuación, selecciona al cliente que quieras mover a la nueva suscripción.
2. Selecciona **Agregar suscripción**.
3. Selecciona la suscripción que quieras adquirir del catálogo (en este caso, una de las opciones que se indican más arriba), escribe el número de licencias y, a continuación, **Enviar**. 

El cliente ahora tendrá la suscripción antigua y uno nuevo. El siguiente paso es reasignar licencias a los usuarios del cliente.

1. Selecciona **los clientes** desde el menú de navegación izquierdo y, a continuación, selecciona al cliente que se mueve.
2. Selecciona **Usuarios y licencias**.
3. Para reasignar una licencia a un usuario, selecciona el usuario y, a continuación, selecciona **Administrar licencias**. 
4. En la página **Administrar licencias** , borrar el Dynamics 365 for Sales / Customer Engagement Plan de Basic (ofrecer calificado) casilla de verificación de licencia y selecciona un nuevo plan de servicio de la suscripción que se cambia el cliente. 
5. Selecciona **Enviar**. Para hacer esto para cada usuario que necesita la nueva licencia. 

Una vez que traslades las licencias a la nueva suscripción puede cancelar la suscripción antigua. 

1. Selecciona **los clientes** desde el menú de navegación izquierdo y, a continuación, selecciona al cliente que se mueve.
2. En la página de detalles de suscripción, Establece la suscripción antigua a **suspendida** y seleccione **Enviar**.

Ahora se suspende la suscripción antigua y la nueva suscripción está activa. Se cancelará el aprovisionamiento de la suscripción suspendida automáticamente después de 120 días. El cliente no conllevará ningún coste adicional para la suscripción antigua.
 

 



