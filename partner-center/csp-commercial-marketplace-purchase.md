---
title: Compra de ofertas de Marketplace comercial
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo los asociados del programa CSP pueden usar Centro de partners Marketplace para realizar compras de ofertas de SaaS de proveedores de software independientes (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3f5cf4895fa4d66c65215989d808a1dd18ef9064
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147860"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Comprar productos de Marketplace comercial para sus clientes en Centro de partners


**Roles adecuados:** administrador global | Agente de administración

Como asociado en el programa Proveedor de soluciones en la nube (CSP), puede usar el marketplace comercial para comprar suscripciones para sus clientes a determinados productos de software como servicio (SaaS) ofrecidos por fabricantes de software independientes (ISV).

Al ofrecer suscripciones SaaS de ISV a los clientes, puede ayudar a diferenciar su negocio. También puede proporcionar a los clientes acceso a los paquetes de software que abordan sus necesidades empresariales específicas. Las licencias y suscripciones de estos productos SaaS de Marketplace se administran desde publicadores de ISV igual que se administran las licencias y las suscripciones de los productos de Microsoft.

Puede comprar suscripciones **saaS basadas** en licencias o **suscripciones basadas en** el uso. Para más información sobre la diferencia entre la facturación basada en licencias y la basada en el uso, consulte [Conceptos básicos de facturación.](billing-basics.md)

## <a name="purchase-license-based-and-metered-saas-subscriptions-in-partner-center"></a>Compra de suscripciones SaaS basadas en licencias y de uso Centro de partners

Puede comprar suscripciones para productos SaaS de uso medidor o basado en licencias que ofrecen los anunciantes de ISV mediante el mismo proceso que usa para comprar suscripciones para productos de Microsoft.

Para comprar una suscripción de SaaS basada en licencias o de uso Centro de partners, consulte [Creación, suspensión o cancelación de suscripciones de cliente.](create-a-new-subscription.md#create-a-new-subscription)

También puedes usar las [API del Centro de partners](/partner-center/develop/) para crear suscripciones de Marketplace comercial para los clientes. (Para más información sobre el uso de Centro de partners API, consulte Creación de una suscripción [para productos de Marketplace comercial).](/partner-center/develop/create-subscription-azure-marketplace-products)

>[!IMPORTANT]
> Como asociado del programa CSP,  puede comprar suscripciones **SaaS** basadas en licencias o de uso medidor a publicadores de ISV dentro de Centro de partners. Esto significa que puede comprar **cualquier** oferta **de** SaaS basada en licencia o [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) con uso que el publicador de ISV haya puesto a su disposición, incluidas las ofertas exclusivas a las que tenga acceso. Para comprar o administrar otras ofertas de Marketplace comercial de isv (por ejemplo, ofertas basadas en el uso que implican aplicaciones de Azure, contenedores o máquinas [virtuales),](https://portal.azure.com/)debe ir a la Azure Portal .

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Comprar suscripciones basadas en el uso en el Azure Portal

A diferencia de las suscripciones saaS basadas en licencias de publicadores de ISV de terceros, las suscripciones basadas en el uso requieren primero que un cliente tenga una suscripción de Azure. La facturación de marketplace comercial, los recursos basados en el uso se enmarcan en la suscripción de Azure del cliente. Una vez que el cliente tiene una suscripción de Azure, un asociado del programa CSP puede seguir estos pasos para adquirir una suscripción de Marketplace comercial para ellos:

1. Inicie sesión en Centro de partners [panel y,](https://partner.microsoft.com/dashboard)a continuación, **seleccione Clientes** en el menú de la izquierda.

2. Seleccione el cliente específico y, a continuación, **seleccione Suscripciones.**  

3. En Suscripciones **basadas en uso,** seleccione **Todos los recursos.** Esto le lleva al Portal de administración de Azure.

4. En el Portal de administración de Azure, **seleccione Crear un recurso** en el menú de la izquierda.

5. Seleccione **Ver todo** en la parte superior de la Azure Marketplace lista.

6. Para restringir la lista, use filtros en la parte superior de la lista de Marketplace. Por ejemplo, puede seleccionar **Microsoft**  o **Partner** en la lista desplegable Publicador para ver solo las ofertas de Microsoft o las de un publicador de ISV.

7. Elija una oferta específica y, a continuación, **seleccione Crear**.

## <a name="next-steps"></a>Pasos siguientes

- [Administración de ofertas de Marketplace comercial](csp-commercial-marketplace-purchase.md)