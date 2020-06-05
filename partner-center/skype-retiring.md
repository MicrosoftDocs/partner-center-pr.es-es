---
title: Migrar algunas suscripciones de Skype empresarial
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Obtenga información sobre cómo y cuándo migrar determinados clientes con suscripciones de Skype empresarial online plan 1 que expiren a las nuevas versiones de Office 365.
author: LauraBrenner
ms.author: labrenne
keywords: Planes de Skype empresarial, retirar Skype, Office 365
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8e3a16450d9ac15785315a1b4b077e1872e1303a
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/04/2020
ms.locfileid: "84425964"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migración de suscripciones del Plan 1 de Skype Empresarial Online a las versiones más modernas de Office 365

**Se aplica a**

- Centro de partners

Se retirará el plan 1 de Skype empresarial online, a partir del 1 de agosto de 2018. Después de esa fecha, los clientes ya no podrán comprar nuevas suscripciones al plan 1 de Skype empresarial y las suscripciones existentes no se renovarán automáticamente cuando expiren y no proporcionarán una opción de renovación. En la página de detalles de la suscripción, el estado de la suscripción al plan 1 de Skype empresarial online ha cambiado a "expira el [fecha]" de "renoticias automática en [fecha]".  

Para garantizar la continuidad de los clientes, debe realizar la transición de los clientes con suscripciones de Skype empresarial online plan 1 que expiren a una opción de SKU compatible, que se enumeran a continuación. Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes. 

>[!NOTE]
>Se han retirado las SKU Commercial y Government de Skype empresarial online.

Si usa la API (de la cresta o del centro de Partners), busque suscripciones que expiren evaluando la fecha de finalización de la suscripción junto con la propiedad auto Renew = false. Las suscripciones de Skype empresarial online plan 1 se establecerán en renovación automática = false el 1 de septiembre de 2018. Puede trasladar a los clientes a un nuevo plan en cualquier momento. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Planes de reemplazo de Skype empresarial online plan 1

Con los nuevos planes, sus clientes pueden beneficiarse de las características y funcionalidades más recientes de Office 365. Los detalles de precios se encuentran en la lista de precios y en la matriz de lista de ofertas del centro de Partners. 

- Opción 1: Office 365 Enterprise F1
- Opción 2: Microsoft 365 Enterprise F1
- Opción 3: otros planes de Office 365

|**Característica**    |**Opción 1**   |**Opción 2**   |**Opción 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Obtener todas las características incluidas en Skype empresarial online plan 1|Sí   |Sí   |Sí   |
|Mensajería instantánea y presencia |Sí   |Sí   |Sí   |
|Audio y vídeo punto a punto en IP|Sí   |Sí   |Sí   
|Unirse a reuniones como usuario autenticado| Sí   |Sí   |Sí   |

## <a name="transition-customers-to-new-product-plans"></a>Clientes de transición hacia los nuevos planes de productos

Microsoft ofrece continuamente nuevos productos y servicios a nuestros asociados. En estos casos, es posible que tenga que actualizar los clientes a nuevos servicios o migrar sus suscripciones de SKU que se apagarán finalmente. La migración de los clientes de SKU retiradas a otras más recientes requiere los siguientes pasos:

- Comprar la nueva suscripción
- Reasignar licencias de usuario actuales
- Cancelar suscripción anterior

### <a name="migrate-your-customers-to-new-plans"></a>Migre sus clientes a nuevos planes

1. Para comprar la nueva suscripción, en el **menú del centro de Partners**, seleccione **clientes**, seleccione el cliente que desea migrar y, a continuación, seleccione **Agregar suscripciones**.

2. Seleccione la suscripción que desea comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, seleccione **submit (enviar**). 

El cliente debería tener ahora suscripciones antiguas y nuevas, la suscripción del plan 1 de Skype empresarial online anterior y la nueva suscripción de destino, por ejemplo, la opción 1: Office 365 Enterprise F1.

3. Para reasignar las licencias de los usuarios del cliente, en el menú del **centro de Partners** , seleccione **clientes**, seleccione el cliente que va a mover y, a continuación, seleccione **usuarios y licencias**. Se abre la página usuarios y licencias del cliente.

4. Para reasignar la licencia de usuario, seleccione el usuario que desea reasignar y, a continuación, seleccione **administrar licencias.**

5. En la página **administrar licencias** , desactive la casilla de licencia del plan 1 de Skype empresarial online y seleccione un nuevo plan de servicio para la suscripción a la que el cliente se está moviendo.

6. Seleccione **Submit** (Enviar). Una página de confirmación enumera las nuevas asignaciones de licencias. Continúe con el mismo proceso para otros usuarios que necesiten asignaciones de licencia.

Después de mover la licencia de usuario al nuevo servicio, puede cancelar con seguridad la suscripción retirada en el nivel de cliente.

7. En el menú del **centro de Partners** , seleccione **clientes**. Seleccione el cliente cuya suscripción va a cancelar.

8. En la página de detalles de la suscripción, establezca la suscripción en **Suspended**.

9. Seleccione **submit (enviar).**

Se ha suspendido la suscripción antigua y la nueva suscripción está activa. La suscripción suspendida se desaprovisionará automáticamente después de 120 días. El cliente no incurre en costos adicionales para la suscripción antigua.

