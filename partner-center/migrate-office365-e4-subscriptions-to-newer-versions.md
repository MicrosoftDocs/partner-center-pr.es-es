---
title: Migración de suscripciones de Office 365 E4
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office edición 365 Enterprise E4 se retiró a partir del 7 de abril de 2017. Obtenga información sobre cómo migrar las suscripciones de los clientes a versiones más recientes de Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f738ddace805838cdf202c23cca8535c11cbdf54
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151566"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrar suscripciones de Office 365 E4 a las versiones más recientes de Office 365

**Roles adecuados:** administrador global | Administrador de administración de | Agente de administración | Agente de ventas

El plan Office 365 Enterprise E4 se ha retirado, a partir del 7 de abril de 2017. Ya no puede comprar nuevas suscripciones de Office 365 E4 después de esta fecha, y las suscripciones E4 existentes no se renovarán automáticamente cuando expiren.

Cuando finalicen las suscripciones E4, se cancelarán. Para garantizar la continuidad de los clientes, debe realizar la transición de los clientes con suscripciones E4 que expiran a una opción de SKU compatible, que se muestra a continuación. Se recomienda mover clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones del servicio para los clientes. 

> [!NOTE]  
> Se retiraron las SKU comerciales y gubernamentales de Office 365 Enterprise E4.
 
En la página de detalles de la suscripción, el estado de la suscripción E4 ha cambiado a "Expira en [fecha]" de "Renovación automática en [fecha]". 

Si usa la API (YA SEATE o Centro de partners), puede detectar suscripciones que expiran mediante la evaluación de la fecha de finalización de la suscripción junto con la propiedad renovación automática = False. 

Las suscripciones E4 se establecerán en auto renew=False el 7 de abril de 2017. Puede trasladar clientes a un nuevo plan en cualquier momento. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Planes de reemplazo de la edición Office 365 Enterprise E4

Puede optar por mantener la misma funcionalidad con E4 o hacer que los clientes aprovechen las características y funcionalidades más recientes en Office 365 y Skype Empresarial Online. Los detalles de precios se encuentran en la lista de precios y la matriz de la lista de ofertas Centro de partners. Secure Product Enterprise E3 o Secure Productive Enterprise E5 se pueden sustituir en las siguientes opciones para Office 365 Enterprise E3 u Office 365 Enterprise E5, respectivamente.

- Opción 1: Office 365 Enterprise E5

- Opción 2: Office 365 Enterprise E3 + Skype Empresarial Cloud CTRL

- Opción 3: Office 365 Enterprise E3 + Skype Empresarial Plus CAL (paridad de precio y funcionalidad con E4)

- Opción 4: Office 365 Enterprise E3


| Característica | Opción 1 | Opción 2 | Opción 3 | Opción 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| ¿Obtiene todas las características incluidas en Office 365 Enterprise E4? | Sí | Sí | Sí | No |
| ¿Números de teléfono administrados en Office 365? | Sí | Sí | No | No |
| ¿Números de teléfono administrados tanto en el entorno local como en Office 365 (implementación híbrida)? | Sí | Sí | No | No |
| ¿Opción para agregar un plan de llamadas de voz RTC? | Sí | Sí | No | No |
| PSTN Conferencing? | Sí | No | No | No |
| ¿Herramientas avanzadas para la colaboración, el análisis y la seguridad? | Sí | No | No | No |
| ¿Informes interactivos, paneles y visualizaciones de datos? | Sí | No | No | No | 
| ¿Más control sobre la seguridad de los datos y el cumplimiento de la privacidad, la transparencia y los controles de usuario refinados integrados? | Sí | No | No | No | 

## <a name="transition-customers-to-new-product-plans"></a>Clientes de transición hacia los nuevos planes de productos

Microsoft ofrece continuamente nuevos productos y servicios a nuestros asociados. En estos casos, es posible que tenga que actualizar los clientes a nuevos servicios o migrar sus suscripciones desde SKU que finalmente se apagarán. La migración de clientes de SKU retiradas a otras más recientes requiere los pasos siguientes:

-   Comprar la nueva suscripción
-   Reasignación de licencias de usuario actuales
-   Cancelar la suscripción antigua

Siga estos pasos para migrar la suscripción de Office 365 Enterprise E4 de un cliente a una de las opciones de la tabla anterior.

### <a name="step-1---purchase-the-new-subscription"></a>Paso 1: Compra de la nueva suscripción

1. En el **Centro de partners,** seleccione **Clientes,** seleccione el cliente que desea mover y, a continuación, **seleccione Agregar suscripciones.**

2. Seleccione la suscripción que quiere comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, **seleccione Enviar**.

   El cliente debe tener ahora suscripciones antiguas y nuevas, la antigua suscripción de Office 365 Enterprise E4 y la nueva suscripción de "destino", por ejemplo, Opción 1- Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Paso 2: Reasignar las licencias de los usuarios del cliente

1. En el **Centro de partners,** seleccione **Clientes,** seleccione el cliente que desea mover y, a continuación, **seleccione Usuarios y licencias.** Se abre la página Usuarios y licencias del cliente.

2. Para reasignar licencias de usuario, seleccione el usuario que desea reasignar y, a continuación, **seleccione Administrar licencias.**

3. En la página Administrar **licencias,** desactive la casilla Licencia de **Office 365 Enterprise E4** y seleccione un nuevo plan de servicio para la suscripción a la que se traslada el cliente.

4. Seleccione **Submit** (Enviar). Una página de confirmación enumera las nuevas asignaciones de licencias.

5. Sigue los mismos pasos con otros usuarios del cliente que necesiten la reasignación de licencias.

Después de mover las licencias de usuario al nuevo servicio, puede cancelar de forma segura la suscripción retirada en el nivel de cliente superior.

### <a name="step-3---cancel-the-old-subscription"></a>Paso 3: Cancelar la suscripción anterior

1. En el **menú Centro de partners,** seleccione **Clientes.** Seleccione el cliente que desea mover y seleccione la suscripción que desea cancelar.

2. En la página de detalles de la suscripción, establezca el estado de la suscripción en **Suspendido.**

3. Seleccione **Submit** (Enviar).

La suscripción anterior se suspende y la nueva suscripción está activa. La suscripción suspendida se desaprovisiona automáticamente después de 120 días. El cliente no incurre en costos adicionales para la suscripción antigua.



 



