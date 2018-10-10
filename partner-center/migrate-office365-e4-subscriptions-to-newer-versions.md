---
title: Migrar suscripciones de Office 365 E4 a las versiones más recientes de Office 365 | Centro de partners
description: La edición de Office 365 Enterprise E4 se retirará a partir del 7 de abril de 2017. Obtén información sobre cómo migrar las suscripciones de cliente a las versiones más recientes de Office 365.
author: MaggiePucciEvans
ms.localizationpriority: medium
ms.openlocfilehash: 75999aa004ae03d4ec871fc706d757a192105320
ms.sourcegitcommit: 123a7f53d633c27eb5f982926d856de47afb1042
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/09/2018
ms.locfileid: "4490181"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrar de suscripciones de Office 365 E4 a las versiones más recientes de Office 365

**Se aplica a:**

-  Centro de partners

El plan Office 365 Enterprise E4 se retira de forma efectiva el 7 de abril de 2017. Ya no se podrán adquirir nuevas suscripciones de Office 365 E4 después de esta fecha, y las suscripciones E4 existentes no se renovarán automáticamente cuando expiren.

Cuando finalicen suscripciones de E4, se cancelarán. Para garantizar la continuidad de los clientes, debes pasar los clientes cuyas suscripciones a E4 vayan a caducar a una opción de SKU compatible, como aparece a continuación. Te recomendamos mover los clientes a las nuevas suscripciones antes de la fecha de finalización para evitar interrupciones en el servicio a los clientes. 

> [!NOTE]  
>  Se retiran tanto Office 365 Enterprise E4 comercial y SKU del gobierno.
 
En la página de detalles de la suscripción, el estado de la suscripción a E4 ha cambiado de "Se renovará automáticamente en [fecha]" a "Expira en [fecha]". 

Si usas la API (CREST o el Centro de partners), puedes descubrir suscripciones caducadas mediante la evaluación de la fecha de finalización de la suscripción junto con la renovación automática = False propiedad. 

Las suscripciones E4 se establece como renovación automática = Falso el 7 de abril de 2017. Puedes mover a los clientes a un plan nuevo en cualquier momento. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Planes de reemplazo de la edición Office 365 Enterprise E4

Puedes elegir mantener la misma funcionalidad con E4 o puedes hacer que los clientes saquen provecho de las nuevas características y funciones de Office 365 y Skype Empresarial Online. Los detalles de precios se encuentran en la lista de precios y en la matriz de lista de ofertas en el Centro de partners. Secure Productive Enterprise E3 o Secure Productive Enterprise E5 puede sustituirse en las siguientes opciones por Office 365 Enterprise E3 o Office 365 Enterprise E5 respectivamente.

- Opción 1: Office 365 Enterprise E5

- Opción 2: E3 de Office 365 empresa + Skype Empresarial Cloud PBX

- Opción 3: Office 365 Enterprise E3 + Skype Empresarial + CAL (paridad de precio y la funcionalidad con E4)

- Opción 4: Office 365 Enterprise E3


| Función | Opción 1 | Opción 2 | Opción 3 | Opción 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| ¿Obtener todas las características incluidas en Office 365 Enterprise E4? | Sí | Sí | Sí | No |
| ¿Números de teléfono administrados en Office 365? | Sí | Sí | No | No |
| ¿Números de teléfono administrados en local y en Office 365 (implementación híbrida)? | Sí | Sí | No | No |
| ¿Opción para agregar un plan de llamadas de voz RTC? | Sí | Sí | No | No |
| ¿Conferencias RTC? | Sí | No | No | No |
| ¿Herramientas avanzadas de colaboración, análisis y seguridad? | Sí | No | No | No |
| ¿Visualizaciones interactivas de informes, paneles y datos? | Sí | No | No | No | 
| ¿Más control sobre la seguridad de los datos y la conformidad con la privacidad integradas, transparencia y controles de usuario refinados? | Sí | No | No | No | 

## <a name="transition-customers-to-new-product-plans"></a>Clientes de transición hacia los nuevos planes de productos

Microsoft ofrece de forma continua nuevos productos y servicios a nuestros partners. En estos casos, podrías tener que actualizar a los clientes con los nuevos servicios o migrar sus suscripciones de SKU que finalmente se apagarán. Migración de los clientes desde SKU retiradas a unas más recientes que requieren los siguiente pasos:

-   Comprar la nueva suscripción
-   Reasignar licencias de usuario actual
-   Cancelar la suscripción antigua

Sigue estos pasos para migrar la suscripción a Office 365 Enterprise E4 de un cliente a una de las opciones en la tabla anterior.

### <a name="step-1---purchase-the-new-subscription"></a>Paso 1 - Comprar la nueva suscripción

1. En el menú del **Centro de partners** , selecciona **los clientes**, selecciona al cliente que deseas mover y, a continuación, selecciona **Agregar suscripciones**.

2. Selecciona la suscripción que quieras adquirir del catálogo (en este caso, una de las opciones que se indican más arriba), escribe el número de licencias y, a continuación, **Enviar**.

   El cliente ahora debería tener suscripciones antiguas y nuevas, la suscripción antigua a Office 365 Enterprise E4 y el nuevo "destino" de la suscripción, por ejemplo, opción 1: Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Paso 2: Reasignar licencias de los usuarios del cliente

1. En el menú del **Centro de partners** , selecciona **los clientes**, selecciona al cliente que deseas mover y, a continuación, selecciona **los usuarios y licencias**. La página Usuarios y licencias del cliente se abrirá.

2. Para reasignar licencias de usuario, selecciona el usuario para reasignar y, a continuación, selecciona **Administrar licencias**.

3. En la página **Administrar licencias** desactiva la casilla de verificación de licencia de **Office 365 Enterprise E4**  selecciona un nuevo plan de servicio de la suscripción a la que se cambia el cliente.

4. Selecciona **Enviar**. Una página de confirmación enumera las nuevas asignaciones de licencias.

5. Sigue los mismos pasos con otros usuarios del cliente que necesiten la reasignación de licencias.

Después de mover las licencias de usuario al nuevo servicio, puedes cancelar de forma segura la suscripción retirada al nivel superior del cliente.

### <a name="step-3---cancel-the-old-subscription"></a>Paso 3 - Cancelar la suscripción antigua

1. En el menú del **Centro de partners** , selecciona **los clientes**. Selecciona al cliente que quieres mover y selecciona la suscripción que quieres cancelar.

2. En la página de detalles de suscripción, establece el estado de la suscripción a **Suspendida**.

3. Selecciona **Enviar**.

Se ha suspendido la suscripción antigua y la nueva suscripción está activa. Se cancelará el aprovisionamiento de la suscripción suspendida automáticamente después de 120 días. El cliente no incurre en costos adicionales para la suscripción antigua.



 



