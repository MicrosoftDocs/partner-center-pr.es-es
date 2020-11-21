---
title: Ofertas privadas en Azure Marketplace
description: Obtenga información sobre las ofertas privadas en Azure Marketplace.
ms.prod: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 055151f0420d642d591554a829dc21b69df84ebd
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007389"
---
# <a name="private-offers-in-azure-marketplace"></a>Ofertas privadas en Azure Marketplace

Las ofertas privadas son el modo en que los publicadores proporcionan planes personalizados a clientes específicos. Esta opción solo se admite actualmente en la experiencia de Azure Marketplace en el Azure Portal. Las ofertas privadas solo están disponibles para las ofertas de pago que se pueden adquirir e instalar directamente desde el Azure Portal. El publicador no puede crear ofertas privadas para servicios de consultoría, ningún servicio que se haya puesto **en contacto** como una llamada a una acción o cualquier servicio gratuito, independientemente de si se puede instalar desde el portal o no.

## <a name="find-private-offers-in-the-azure-portal"></a>Busque ofertas privadas en el Azure Portal

Cuando un asociado publica una oferta privada, solo es visible para los usuarios válidos en la sección **Marketplace** de la Azure portal. Estos usuarios se definen mediante el identificador de suscripción o el identificador de inquilino, según el tipo de oferta. Si es válido para las ofertas privadas, hay dos maneras de encontrarlas en el portal.

> [!NOTE]
> Actualmente, las ofertas privadas no se pueden buscar ni filtrar (por categoría) en el Azure Portal.

En el Azure Portal, seleccione **+ crear un recurso** o busque "Marketplace" para ir a la página de **Marketplace** . Si es válido para las ofertas privadas, verá el banner **tiene ofertas privadas disponibles** en la parte superior de la página. Seleccione **Ver ofertas privadas** para ir a la página de ofertas privadas.

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="El banner que aparece cuando tiene ofertas privadas disponibles.":::

Como alternativa, si ve el banner de ofertas privadas, también puede desplazarse a la parte inferior de la página de la galería de productos y verá un subconjunto de las ofertas privadas. Seleccione el vínculo para **Ver más información** para ir a la página de ofertas privadas.

:::image type="content" source="media/private-offers/see-more-link.png" alt-text="Muestra las ofertas privadas en la parte inferior de la pantalla, junto con el vínculo ver más.":::

## <a name="review-private-plans"></a>Revisar planes privados

Una oferta privada es realmente un plan privado dentro de una oferta. Cada oferta puede tener varios planes, tanto públicos como privados, pero los planes privados se muestran en una lista independiente de los planes públicos.

Puede ver los planes privados disponibles en la pestaña **planes** , marcados con un distintivo **privado** distintivo:

:::image type="content" source="media/private-offers/private-badge.png" alt-text="Página de planes marcada como privada.":::

Si tiene más de una suscripción, verá todas las ofertas privadas disponibles para todas las suscripciones. Al seleccionar **crear**, se le dirigirá a la página de creación de recursos para comenzar a configurar el recurso.

Si selecciona **crear** y tiene varias suscripciones, pero no todas ellas se agregan al plan privado, es posible que la suscripción predeterminada no sea la suscripción válida para esta oferta privada. En este caso, seleccione la suscripción correcta.

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="El vínculo que muestra hay más ofertas privadas disponibles.":::

## <a name="next-steps"></a>Pasos siguientes

- [¿Qué es Azure Marketplace?](azure-marketplace-overview.md)
