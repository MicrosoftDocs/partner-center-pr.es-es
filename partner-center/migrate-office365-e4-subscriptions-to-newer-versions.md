---
title: Migración de suscripciones de Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4 Edition se retirará a partir del 7 de abril de 2017. Obtenga información sobre cómo migrar las suscripciones de clientes a las versiones más recientes de Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132628"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrar suscripciones de Office 365 E4 a las versiones más recientes de Office 365

**Roles adecuados**

- Administrador global
- Administrador del control de usuarios
- Agente de administrador
- Agente de ventas

El plan Office 365 Enterprise E4 se ha retirado, en vigor el 7 de abril de 2017. Ya no se pueden comprar nuevas suscripciones a Office 365 E4 después de esta fecha, y las suscripciones de E4 existentes no se renovarán automáticamente cuando expiren.

Cuando finalicen las suscripciones a E4, se cancelarán. Para garantizar la continuidad de los clientes, debe realizar la transición de los clientes con suscripciones de E4 que expiren a una opción de SKU admitida, que se enumeran a continuación. Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes. 

> [!NOTE]  
> Se han retirado las SKU de Office 365 Enterprise E4 Commercial y Government.
 
En la página de detalles de la suscripción, el estado de la suscripción de E4 ha cambiado a "expira el [fecha]" de "renueve automáticamente en [fecha]". 

Si usa la API (de la cresta o del centro de Partners), puede detectar las suscripciones que van a expirar mediante la evaluación de la fecha de finalización de la suscripción junto con la propiedad auto Renew = false. 

Las suscripciones del plan E4 se establecerán en renovación automática = false en el 7 de abril de 2017. Puede trasladar a los clientes a un nuevo plan en cualquier momento. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Planes de reemplazo de Office 365 Enterprise E4 Edition

Puede optar por mantener la misma funcionalidad con E4 o hacer que los clientes aprovechen las características y funcionalidades más recientes de Office 365 y Skype empresarial online. Los detalles de precios se encuentran en la lista de precios y en la matriz de lista de ofertas del centro de Partners. Secure Product Enterprise E3 o Secure productiva Enterprise E5 se pueden sustituir en las siguientes opciones para Office 365 Enterprise E3 u Office 365 Enterprise E5, respectivamente.

- Opción 1: Office 365 Enterprise E5

- Opción 2: Office 365 Enterprise E3 + PBX en la nube de Skype empresarial

- Opción 3: Office 365 Enterprise E3 + CAL de Skype empresarial Plus (paridad de precio y funcionalidad con E4)

- Opción 4: Office 365 Enterprise E3


| Característica | Opción 1 | Opción 2 | Opción 3 | Opción 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Obtener todas las características incluidas en Office 365 Enterprise E4? | Sí | Sí | Sí | No |
| Números de teléfono administrados en Office 365 | Sí | Sí | No | No |
| Números de teléfono administrados tanto en el entorno local como en Office 365 (implementación híbrida) | Sí | Sí | No | No |
| ¿Desea agregar un plan de llamada de voz RTC? | Sí | Sí | No | No |
| ¿Conferencias RTC? | Sí | No | No | No |
| Herramientas avanzadas para la colaboración, el análisis y la seguridad | Sí | No | No | No |
| Informes interactivos, paneles y visualizaciones de datos | Sí | No | No | No | 
| ¿Más control sobre la seguridad y el cumplimiento de los datos con la privacidad, la transparencia y los controles de usuario mejorados? | Sí | No | No | No | 

## <a name="transition-customers-to-new-product-plans"></a>Clientes de transición hacia los nuevos planes de productos

Microsoft ofrece continuamente nuevos productos y servicios a nuestros asociados. En estos casos, es posible que tenga que actualizar los clientes a nuevos servicios o migrar sus suscripciones de SKU que se apagarán finalmente. La migración de los clientes de SKU retiradas a otras más recientes requiere los siguientes pasos:

-   Comprar la nueva suscripción
-   Reasignar licencias de usuario actuales
-   Cancelar la suscripción antigua

Siga estos pasos para migrar la suscripción Office 365 Enterprise E4 de un cliente a una de las opciones de la tabla anterior.

### <a name="step-1---purchase-the-new-subscription"></a>Paso 1: compra de la nueva suscripción

1. En el menú del **centro de Partners** , seleccione **clientes**, seleccione el cliente que desea migrar y, a continuación, seleccione **Agregar suscripciones**.

2. Seleccione la suscripción que desea comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, seleccione **submit (enviar**).

   El cliente debería tener ahora suscripciones antiguas y nuevas, la antigua suscripción de Office 365 Enterprise E4 y la nueva suscripción de destino, por ejemplo, la opción 1-Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Paso 2: reasignación de las licencias de los usuarios del cliente

1. En el menú del **centro de Partners** , seleccione **clientes**, seleccione el cliente que desea migrar y, a continuación, seleccione **usuarios y licencias**. Se abre la página usuarios y licencias del cliente.

2. Para reasignar licencias de usuario, seleccione el usuario que desea reasignar y, a continuación, seleccione **administrar licencias**.

3. En la página **administrar licencias** , desactive la casilla **Office 365 Enterprise E4** License y seleccione un nuevo plan de servicio para la suscripción a la que está pasando el cliente.

4. Seleccione **Submit** (Enviar). Una página de confirmación enumera las nuevas asignaciones de licencias.

5. Sigue los mismos pasos con otros usuarios del cliente que necesiten la reasignación de licencias.

Después de mover las licencias de usuario al nuevo servicio, puede cancelar con seguridad la suscripción retirada en el nivel superior del cliente.

### <a name="step-3---cancel-the-old-subscription"></a>Paso 3: cancelar la suscripción anterior

1. En el menú del **centro de Partners** , seleccione **clientes**. Seleccione el cliente que desea trasladar y seleccione la suscripción que desea cancelar.

2. En la página Detalles de la suscripción, establezca el estado de la suscripción en **Suspended**.

3. Seleccione **Submit** (Enviar).

La suscripción anterior se suspende y la nueva suscripción está activa. La suscripción suspendida se desaprovisionará automáticamente después de 120 días. El cliente no incurre en costos adicionales para la suscripción antigua.



 



