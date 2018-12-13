---
title: Migrar Dynamics 365 empresas Edition ofrece a las versiones más recientes | El centro de partners
ms.topic: article
ms.date: 12/12/2018
description: Ya no se pueden renovar suscripciones de Dynamics 365 edición Business.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: labrenne
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Dynamics 365 offers, renew offers, new Dynamics 365 SKUs
ms.openlocfilehash: 11f0d9262856d28adb4d67871503d86f2d4945ac
ms.sourcegitcommit: 23adf424dd43ed0281473f97d535d73c59c92b01
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/13/2018
ms.locfileid: "8968292"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrar Dynamics 365 empresas Edition ofrece a las versiones más recientes 

**Se aplica a**

- Centro de partners

Estas ofertas heredadas; ya no pueden renovar eficaz del 1 de enero de 2019, los clientes con suscripciones de Dynamics 365 Business Edition las suscripciones existentes no se renovarán automáticamente cuando expiren. En la página de detalles de la suscripción, el estado cambiará a "Expira el [fecha]" desde "Se renovará automáticamente en [fecha]".

Para garantizar la continuidad para los clientes, debes pasarlas personas con suscripciones vayan a caducar a una opción compatible, como aparece a continuación. Recomendamos pasar a los clientes a las nuevas suscripciones, antes de la fecha de finalización anual de la suscripción, para evitar interrupciones del servicio a los clientes.

Si usas la API (CREST o centro de partners), puedes encontrar renovar suscripciones vayan a caducar evaluando la fecha de finalización de la suscripción junto con la automática = False propiedad. Las suscripciones en cuestión se establecerá automáticamente renovar = False el 1 de enero de 2019. Puedes mover a los clientes a un plan nuevo en cualquier momento. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Las ediciones de empresas de Dynamics 365 se retira

- Dynamics 365 para Finance and Operations, edición Business
- Dynamics 365 for Team Members, edición Business

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics empresas Central: las nuevas ofertas de edición Business de Dynamics 365

Con las nuevas ofertas de Dynamics empresas Central, los clientes pueden conectar sus finanzas, ventas, servicio y operaciones para optimizar los procesos de negocio, mejorar las interacciones del cliente y tomar mejor las decisiones. Dynamics 365 empresas Central está en la nube y está disponible a través de los partners del programa de proveedor de soluciones en la nube (CSP) solo.
Los clientes de edición de empresas pueden optar a recibir la transición con descuento de precios para el nuevo Central de empresas de Dynamics 365 ofrece hasta el 30 de junio de 2020.

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