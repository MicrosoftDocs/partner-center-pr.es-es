---
title: Migración de suscripciones de Skype Empresarial
description: Obtenga información sobre cómo y cuándo migrar determinados clientes con suscripciones del Plan 1 de Skype Empresarial Online a nuevas versiones de Office 365.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: a8de5b824a24b07607b5365848ec1027ca0d08e8
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551544"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migración de suscripciones del Plan 1 de Skype Empresarial Online a las versiones más modernas de Office 365

**Roles adecuados:** Agente de ventas

El plan 1 de Skype Empresarial Online se retirará, a partir del 1 de agosto de 2018. Después de esa fecha, los clientes ya no pueden adquirir nuevas suscripciones del Plan 1 de Skype Empresarial, y las suscripciones existentes no se renovarán automáticamente cuando expiren y no proporcionarán una opción de renovación. En la página de detalles de la suscripción, el estado de la suscripción del Plan 1 de Skype Empresarial Online ha cambiado a "Expira en [fecha]" de "Renovación automática en [fecha]".  

Para garantizar la continuidad de los clientes, debe realizar la transición de los clientes con suscripciones del plan 1 de Skype Empresarial Online que expiran a una opción de SKU compatible, que se muestra a continuación. Se recomienda mover clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones del servicio para los clientes. 

>[!NOTE]
>Se han retirado las SKU comerciales y gubernamentales del Plan 1 de Skype Empresarial Online.

Si usa la API (REST de comercio (EXPIRE) o Centro de partners), busque las suscripciones que expiran mediante la evaluación de la fecha de finalización de la suscripción junto con la propiedad renovación automática = False. Las suscripciones del Plan 1 de Skype Empresarial Online se establecerán en renovación automática=False el 1 de septiembre de 2018. Puede trasladar clientes a un nuevo plan en cualquier momento. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Planes de reemplazo del Plan 1 de Skype Empresarial Online

Con los nuevos planes, los clientes pueden aprovechar las características y funcionalidades más recientes de Office 365. Los detalles de precios se encuentran en la lista de precios y la matriz de la lista de ofertas Centro de partners. 

- Opción 1: Office 365 Enterprise F1
- Opción 2: Microsoft 365 Enterprise F1
- Opción 3: Otros planes de Office 365

|**Característica**    |**Opción 1**   |**Opción 2**   |**Opción 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Obtener todas las características incluidas en el plan 1 de Skype Empresarial Online|Sí   |Sí   |Sí   |
|Mensajería instantánea y presencia |Sí   |Sí   |Sí   |
|Audio y vídeo punto a punto a través de IP|Sí   |Sí   |Sí   
|Unión a reuniones como usuario autenticado| Sí   |Sí   |Sí   |

## <a name="transition-customers-to-new-product-plans"></a>Clientes de transición hacia los nuevos planes de productos

Microsoft ofrece continuamente nuevos productos y servicios a nuestros asociados. En estos casos, es posible que tenga que actualizar los clientes a nuevos servicios o migrar sus suscripciones desde SKU que finalmente se apagarán. La migración de clientes de SKU retiradas a otras más recientes requiere los pasos siguientes:

- Comprar la nueva suscripción
- Reasignación de licencias de usuario actuales
- Cancelación de una suscripción antigua

### <a name="migrate-your-customers-to-new-plans"></a>Migración de clientes a nuevos planes

1. Para comprar la nueva suscripción, en el menú **Centro de partners,** seleccione **Clientes,** seleccione el cliente que desea mover y, a continuación, **seleccione Agregar suscripciones.**

2. Seleccione la suscripción que desea comprar del catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, **seleccione Enviar**. 

Ahora, el cliente debe tener suscripciones antiguas y nuevas, la antigua suscripción del plan 1 de Skype Empresarial Online y la nueva suscripción de "destino", por ejemplo, Opción 1: Office 365 Enterprise F1.

3. Para reasignar las licencias de los usuarios del cliente, en el menú **Centro de partners,** seleccione **Clientes,** seleccione el cliente que va a mover y, a continuación, seleccione Usuarios **y licencias.** Se abre la página Usuarios y licencias del cliente.

4. Para reasignar la licencia de usuario, seleccione el usuario que desea reasignar y, a continuación, **seleccione Administrar licencias.**

5. En la página Administrar **licencias,** desactive la casilla de licencia Plan 1 de Skype Empresarial Online y seleccione un nuevo plan de servicio para la suscripción a la que se traslada el cliente.

6. Seleccione **Submit** (Enviar). Una página de confirmación enumera las nuevas asignaciones de licencias. Continúe este mismo proceso para otros usuarios que necesiten asignaciones de licencias.

Después de mover la licencia de usuario al nuevo servicio, puede cancelar de forma segura la suscripción retirada en el nivel de cliente.

7. En el **menú Centro de partners,** seleccione **Clientes.** Seleccione el cliente cuya suscripción va a cancelar.

8. En la página de detalles de la suscripción, establezca la suscripción en **Suspendido.**

9. Seleccione **Enviar.**

Se ha suspendido la suscripción antigua y la nueva suscripción está activa. La suscripción suspendida se desaprovisiona automáticamente después de 120 días. El cliente no incurre en costos adicionales para la suscripción antigua.

## <a name="next-steps"></a>Pasos siguientes

- [Asesores: Creación y envío de una invitación de prueba para que los clientes prueben Office 365](advisors-create-a-trial-invitation.md)
- [Asesores: Creación de la base de clientes con invitaciones de prueba y ofertas de compra de Office 365](advisors-build-your-business.md)
- [Asesores: Creación de una oferta de compra](advisor-create-a-purchase-offer.md)
