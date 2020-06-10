---
title: Migración de suscripciones de Kaizala Pro a Microsoft365
description: Obtenga información sobre cómo migrar las suscripciones de Kaizala Pro a las versiones de Microsoft365 o Office 365.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 842f4c0f88eec370821fa05c40cfadeee7fee12a
ms.sourcegitcommit: 8b7ef46a88aa5eb52ceefadfc5b0a06c3702d123
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/09/2020
ms.locfileid: "84611241"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a>Migración de suscripciones independientes de Kaizala Pro a versiones de Microsoft365 o Office 365

A partir del 1 de julio de 2020, Microsoft está terminando las ventas del servicio independiente Kaizala Pro. Los clientes ya no podrán comprar nuevas suscripciones de Kaizala Pro después de esta fecha, y las suscripciones de Kaizala Pro existentes no se renovarán automáticamente cuando expiren.

Para garantizar la continuidad de los clientes, debe realizar la transición de los clientes con suscripciones independientes de Kaizala pro de expiración a una opción de SKU compatible, que se enumera a continuación. Se recomienda mover a los clientes a nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones de servicio para los clientes.

Si usa la API (de la cresta o del centro de Partners), puede detectar las suscripciones que han expirado evaluando la fecha de finalización de la suscripción junto con la propiedad renovación automática establecida en false: `auto renew = False` .

Las suscripciones del plan E4 se establecerán `auto renew=False` en el 1 de julio de 2020. Puede trasladar a los clientes a un nuevo plan en cualquier momento.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Planes de reemplazo independientes de Kaizala Pro

Con los nuevos planes, sus clientes pueden beneficiarse de las características y funcionalidades más recientes en Microsoft 365. Los detalles de precios se encuentran en la lista de precios y en la matriz de lista de ofertas del centro de Partners.

- [**Microsoft 365 para empresas**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), incluidos:  
   - Microsoft 365 Empresa Basic
   - Estándar Microsoft 365 Empresa
   - Microsoft 365 Empresa Premium
    
- [**Microsoft 365 para Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), incluidos:
   - Microsoft 365 F3 (antes Microsoft 365 F1) y Office 365 F3
    
- [**Microsoft 365 para Enterprise**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), incluido: 
   - Office 365 E1
   - Microsoft 365 E3 y Office 365 E3
   - Microsoft 365 E5 y Office 365 E5

- [**Microsoft 365 para educación**](https://www.microsoft.com/education/buy-license/microsoft365), incluidos: 
    - Microsoft 365 a1 y Office 365 a1
    - Microsoft 365 a3 y Office 365 a3
    - Microsoft 365 A5 y Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Clientes de transición hacia los nuevos planes de productos

Microsoft ofrece continuamente nuevos productos y servicios a nuestros asociados. En estos casos, es posible que tenga que actualizar los clientes a nuevos servicios o migrar sus suscripciones de SKU que se apagarán finalmente. La migración de los clientes de SKU retiradas a otras más recientes requiere los siguientes pasos:

A. Comprar la nueva suscripción

B. Reasignar licencias de usuario actuales

C. Cancelar suscripción anterior


## <a name="migrate-your-customers-to-new-plans"></a>Migre sus clientes a nuevos planes

### <a name="a-purchase-the-new-subscription"></a>A. Comprar la nueva suscripción

1. Para comprar la nueva suscripción, en el menú del **centro de Partners** , seleccione **clientes**, seleccione el cliente que desea migrar y, a continuación, seleccione **Agregar suscripciones**.

2. Seleccione la suscripción que desea comprar en el catálogo (en este caso, una de las opciones anteriores), escriba el número de licencias y, a continuación, seleccione **submit (enviar**).

El cliente debería tener ahora suscripciones antiguas y nuevas, la antigua suscripción independiente de Kaizala Pro y la nueva suscripción de destino, por ejemplo, la opción 1-Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Reasignar licencias de usuario actuales

1. Para reasignar las licencias de los usuarios del cliente, en el menú del **centro de Partners** , seleccione **clientes**, seleccione el cliente que va a mover y, a continuación, seleccione **usuarios y licencias**. Se abre la página usuarios y licencias del cliente.

2. Para reasignar la licencia de usuario, seleccione el usuario que desea reasignar y, a continuación, seleccione **administrar licencias**.

3. En la página **administrar licencias** , desactive la casilla de Kaizala Pro independiente License y seleccione un nuevo plan de servicio para la suscripción a la que se desplaza el cliente.

4.  Seleccione **Submit** (Enviar). Una página de confirmación enumera las nuevas asignaciones de licencias. Continúe con el mismo proceso para otros usuarios que necesiten asignaciones de licencia.

### <a name="c-cancel-old-subscription"></a>C. Cancelar suscripción anterior

Después de mover la licencia de usuario al nuevo servicio, puede cancelar con seguridad la suscripción retirada en el nivel de cliente.

1.  En el menú del **centro de Partners** , seleccione **clientes**. Seleccione el cliente cuya suscripción va a cancelar.

2.  En la página de detalles de la suscripción, establezca la suscripción en **Suspended**.

3.  Seleccione **Submit** (Enviar).

Se ha suspendido la suscripción antigua y la nueva suscripción está activa. La suscripción suspendida se desaprovisionará automáticamente después de 120 días. El cliente no incurre en costos adicionales para la suscripción antigua.
