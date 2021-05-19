---
title: Migración de suscripciones de Kaizala Pro a Microsoft 365
description: Obtenga información sobre cómo migrar suscripciones de Kaizala Pro Microsoft 365 u versiones de Office 365. Lea este artículo para obtener más detalles sobre la transición de los clientes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146432"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Migración de suscripciones independientes de Kaizala Pro Microsoft 365 u versiones de Office 365

**Roles adecuados:** Agente de ventas

A partir del 1 de julio de 2020, Microsoft está finalizando las ventas del servicio independiente Kaizala Pro. Los clientes ya no podrán comprar nuevas suscripciones de Kaizala Pro después de esta fecha y las suscripciones de Kaizala Pro existentes no se renovarán automáticamente cuando expiren.

Para garantizar la continuidad de los clientes, debe realizar la transición de los clientes con suscripciones independientes de Kaizala Pro expiradas a una opción de SKU compatible, que se muestra a continuación. Se recomienda mover clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones del servicio para los clientes.

Si usa la API (YA SEAN O CENTRO DE PARTNERS), puede detectar suscripciones que expiran evaluando la fecha de finalización de la suscripción junto con la propiedad de renovación automática establecida en false: `auto renew = False` .

Las suscripciones E4 se establecerán en `auto renew=False` el 1 de julio de 2020. Puede trasladar clientes a un nuevo plan en cualquier momento.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Planes de reemplazo independientes de Kaizala Pro

Con los nuevos planes, los clientes pueden aprovechar las características y funcionalidades más recientes de Microsoft 365. Los detalles de precios se encuentran en la lista de precios y la matriz de la lista de ofertas en Centro de partners.

- [**Microsoft 365 para empresas,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)incluidos:  
   - Microsoft 365 Empresa Básico
   - Microsoft 365 Empresa Estándar
   - Microsoft 365 Empresa Premium
    
- [**Microsoft 365 para Frontline,**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)incluidos:
   - Microsoft 365 F3 (antes Microsoft 365 F1) y Office 365 F3
    
- [**Microsoft 365 para Enterprise,**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)incluidos: 
   - Office 365 E1
   - Microsoft 365 E3 y Office 365 E3
   - Microsoft 365 E5 y Office 365 E5

- [**Microsoft 365 for Education,**](https://www.microsoft.com/education/buy-license/microsoft365)incluidos: 
    - Microsoft 365 A1 y Office 365 A1
    - Microsoft 365 A3 y Office 365 A3
    - Microsoft 365 A5 y Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Clientes de transición hacia los nuevos planes de productos

Microsoft ofrece continuamente nuevos productos y servicios a nuestros asociados. En estos casos, es posible que tenga que actualizar los clientes a nuevos servicios o migrar sus suscripciones desde SKU que finalmente se apagarán. La migración de clientes de SKU retiradas a otras más recientes requiere los pasos siguientes:

A. Comprar la nueva suscripción

B. Reasignación de licencias de usuario actuales

C. Cancelación de una suscripción antigua


## <a name="migrate-your-customers-to-new-plans"></a>Migración de clientes a nuevos planes

### <a name="a-purchase-the-new-subscription"></a>A. Comprar la nueva suscripción

1. Para comprar la nueva suscripción, en el menú **Centro de partners,** seleccione **Clientes,** seleccione el cliente que desea mover y, a continuación, **seleccione Agregar suscripciones.**

2. Seleccione la suscripción que desea comprar del catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, **seleccione Enviar**.

El cliente debe tener ahora suscripciones antiguas y nuevas, la suscripción independiente de Kaizala Pro antigua y la nueva suscripción de "destino", por ejemplo, Opción 1- Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Reasignación de licencias de usuario actuales

1. Para reasignar las licencias de los usuarios del cliente, en el menú **Centro de partners,** seleccione **Clientes,** seleccione el cliente que va a mover y, a continuación, seleccione Usuarios **y licencias.** Se abre la página Usuarios y licencias del cliente.

2. Para reasignar la licencia de usuario, seleccione el usuario que desea reasignar y, a continuación, **seleccione Administrar licencias.**

3. En la **página Administrar licencias,** desactive la casilla Licencia independiente de Kaizala Pro y seleccione un nuevo plan de servicio para la suscripción a la que se traslada el cliente.

4.  Seleccione **Submit** (Enviar). Una página de confirmación enumera las nuevas asignaciones de licencias. Continúe este mismo proceso para otros usuarios que necesiten asignaciones de licencias.

### <a name="c-cancel-old-subscription"></a>C. Cancelación de una suscripción antigua

Después de mover la licencia de usuario al nuevo servicio, puede cancelar de forma segura la suscripción retirada en el nivel de cliente.

1.  En el **menú Centro de partners,** seleccione **Clientes.** Seleccione el cliente cuya suscripción va a cancelar.

2.  En la página de detalles de la suscripción, establezca la suscripción en **Suspendido.**

3.  Seleccione **Submit** (Enviar).

Se ha suspendido la suscripción antigua y la nueva suscripción está activa. La suscripción suspendida se desaprovisiona automáticamente después de 120 días. El cliente no incurre en costos adicionales para la suscripción antigua.
