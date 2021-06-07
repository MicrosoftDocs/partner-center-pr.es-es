---
title: Ofertas privadas en Azure Marketplace
description: Obtenga información sobre las ofertas privadas en Azure Marketplace.
ms.service: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 06/03/2021
ms.openlocfilehash: 55d0716b183e9e8905e631447e547396d6f55404
ms.sourcegitcommit: 9cb6bc9df20540f812b7932f88e520976c1aa85a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/06/2021
ms.locfileid: "111534181"
---
# <a name="private-plans-in-azure-marketplace"></a>Planes privados en Azure Marketplace

Los planes privados son la forma en que los publicadores proporcionan planes personalizados a clientes específicos. Los planes privados solo están disponibles para las ofertas de pago que se pueden adquirir e instalar directamente desde el Azure Portal. Los publicadores no pueden crear planes privados para servicios de consultoría, ningún servicio que tenga **Contacto** conmigo como llamada a la acción ni ningún servicio gratuito, independientemente de si se puede instalar desde el portal o no.

## <a name="find-private-plans-in-the-azure-portal"></a>Busque planes privados en el Azure Portal

Cuando un asociado publica un plan privado, solo es visible para los usuarios aptos en la **sección Marketplace** de la Azure Portal. Estos usuarios se definen mediante el identificador de suscripción o el identificador de inquilino, según el tipo de oferta. Si es apto para planes privados, hay dos maneras de encontrarlos en el portal.

> [!NOTE]
> Los planes privados se pueden buscar pero no se pueden filtrar (por categoría) en el Azure Portal.

En la Azure Portal, seleccione **+ Crear un recurso** o busque "Marketplace" para ir a la página **marketplace.** Si es apto para planes privados, verá el banner You **have private plans available (Tiene** planes privados disponibles) en la parte superior de la página. Seleccione **Ver ofertas privadas y planes para** ir a la página de planes privados.

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="Banner que se muestra cuando hay planes privados disponibles.":::

## <a name="review-private-plans"></a>Revisión de planes privados

Un plan privado forma parte de varios planes de una oferta. Cada oferta puede tener varios planes, tanto públicos como privados, pero los planes privados se muestran en una lista independiente de los planes públicos.

Puede ver los planes privados disponibles en la **pestaña Planes,** marcados con un distintivo **privado** distintivo:

:::image type="content" source="media/private-offers/private-badge.png" alt-text="Página de planes marcada como Privada.":::

Si tiene más de una suscripción, verá todos los planes privados disponibles para todas las suscripciones. Al seleccionar **Crear**, se le enruta a la página de creación de recursos para empezar a configurar el recurso.

Si selecciona **Crear** y tiene varias suscripciones, pero no todas se agregan al plan privado, es posible que la suscripción predeterminada no sea la suscripción apta para este plan privado. En este caso, seleccione la suscripción correcta.

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="Vínculo que muestra que hay más planes privados disponibles.":::

## <a name="next-steps"></a>Pasos siguientes

- [¿Qué es Azure Marketplace?](azure-marketplace-overview.md)
