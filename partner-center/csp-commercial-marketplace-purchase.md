---
title: Comprar ofertas comerciales de Marketplace
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo los asociados de programas de CSP pueden usar el Marketplace del centro de partners para realizar compras de clientes de ofertas de SaaS de fabricantes de software independientes (ISV).
author: rbars
ms.author: rbars
keywords: suscripciones, Marketplace, Marketplace comercial, terceros, ISV, ofertas de SaaS, programa de proveedor de soluciones en la nube, compra de una oferta, compra de una suscripción
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0450acd0cfe6586e26baf55c128e64c88f680ba9
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/03/2020
ms.locfileid: "85947698"
---
# <a name="purchase-commercial-marketplace-products-for-your-customers-in-partner-center"></a>Compre productos comerciales de Marketplace para sus clientes en el centro de Partners

**Se aplica a**

- Centro de partners
- Partners del programa CSP

**Roles adecuados**

- Administrador global
- Agente de administrador

Como asociado en el programa del proveedor de soluciones en la nube (CSP), puede usar Marketplace comercial para comprar suscripciones para los clientes a determinados productos de software como servicio (SaaS) ofrecidos por fabricantes de software independientes (ISV). 

Al ofrecer suscripciones de ISV SaaS a los clientes, puede ayudar a diferenciar su negocio. También puede proporcionar a los clientes acceso a los paquetes de software que se ocupan de sus necesidades empresariales específicas. Puede administrar licencias y suscripciones para estos productos SaaS de Marketplace de editores de ISV, al igual que administra licencias y suscripciones para productos de Microsoft.

Puede adquirir suscripciones de SaaS **basadas en licencias** o suscripciones **basadas en el uso** . Para obtener más información acerca de la diferencia entre la facturación basada en licencias y la facturación basada en el uso, consulte [aspectos básicos de facturación](billing-basics.md).

## <a name="purchase-license-based-saas-subscriptions-in-partner-center"></a>Comprar suscripciones SaaS basadas en licencias en el centro de Partners

Puede adquirir suscripciones para productos SaaS basados en licencias ofrecidos por los publicadores de ISV mediante el mismo proceso que usa para adquirir suscripciones para productos de Microsoft.

Para comprar una suscripción de SaaS basada en licencias en el centro de Partners, consulte [creación, suspensión o cancelación de suscripciones de clientes](create-a-new-subscription.md#create-a-new-subscription).

También puedes usar las [API del Centro de partners](https://docs.microsoft.com/partner-center/develop/) para crear suscripciones de Marketplace comercial para los clientes. (Para obtener más información sobre el uso de las API del centro de Partners, consulte [creación de una suscripción para productos comerciales de Marketplace](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products)).

>[!IMPORTANT]
> Como asociado en el programa CSP, solo puede comprar suscripciones de SaaS **basadas en licencias** de los publicadores ISV del centro de Partners. Esto significa que puede comprar cualquier oferta **de SaaS basada en licencia** que el publicador de ISV le haya puesto a su disposición, incluidas las [ofertas exclusivas](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) a las que tenga acceso. Para comprar o administrar otras ofertas comerciales de Marketplace de fabricantes de software independientes (como las ofertas basadas en **el uso, el uso**medido o las basadas en el consumo que impliquen aplicaciones, contenedores o máquinas virtuales de Azure), debe ir al [Azure portal](https://portal.azure.com/). Para obtener más información, vea el siguiente tema.

## <a name="purchase-usage-based-subscriptions-in-the-azure-portal"></a>Compre suscripciones basadas en el uso en el Azure Portal

A diferencia de las suscripciones de SaaS basadas en licencias de los publicadores de ISV de terceros, las suscripciones basadas en el uso primero requieren que un cliente tenga una suscripción de Azure. La facturación de Marketplace comercial, los recursos basados en el uso se encuentra en la suscripción de Azure del cliente. Una vez que el cliente tiene una suscripción de Azure, un asociado en el programa CSP puede seguir estos pasos para adquirir una suscripción comercial de Marketplace para ellos:

1. Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard)del centro de Partners y seleccione **customers (clientes** ) en el menú izquierdo.

2. Seleccione el cliente específico y, a continuación, seleccione **suscripciones**.  

3. En las **suscripciones basadas**en el uso, seleccione **todos los recursos**. Esto le llevará al portal de administración de Azure.

4. En el portal de administración de Azure, seleccione **crear un recurso** en el menú de la izquierda.

5. Seleccione **ver todo** en la parte superior de la lista de Azure Marketplace.

6. Para restringir la lista, use filtros en la parte superior de la lista de Marketplace. Por ejemplo, puede seleccionar **Microsoft** o **Partner** en la lista desplegable **publicador** para ver solo las ofertas de Microsoft o las de un publicador de ISV.

7. Elija una oferta específica y, luego, seleccione **crear**.

## <a name="next-steps"></a>Pasos siguientes

- [Administrar ofertas comerciales de Marketplace](csp-commercial-marketplace-purchase.md)