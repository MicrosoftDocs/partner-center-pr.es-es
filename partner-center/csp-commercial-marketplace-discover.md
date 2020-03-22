---
title: Descubra ofertas en el Marketplace comercial | Centro de Partners
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo los asociados de CSP pueden usar el centro de partners para ver o Buscar ofertas de SaaS o precios de fabricantes de software independientes (ISV).
author: MicheleHope
ms.author: v-mihope
keywords: suscripciones, Marketplace, Marketplace comercial, terceros, ISV, ofertas de SaaS, programa de proveedor de soluciones en la nube, programa CSP, asociados de CSP
ms.localizationpriority: medium
ms.openlocfilehash: 23a31646165576842b625ec4f05a8da404fae01d
ms.sourcegitcommit: 36b8242cc8c47ed36d16f86338a075080c2441e1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/21/2020
ms.locfileid: "80114947"
---
# <a name="discover-offers-and-pricing-in-the-commercial-marketplace"></a>Descubra ofertas y precios en Marketplace comercial

**Se aplica a**

- Centro de asociados
- Partners del programa CSP

**Roles adecuados**

- Administrador global
- Agente de administrador

Cuando fabricantes de software independientes (ISV) deciden publicar una oferta en el Marketplace comercial, también pueden decidir si desean que la oferta esté disponible en el programa CSP. Si optan por vender la oferta a través del programa CSP, los asociados de CSP deben ver la oferta en el área Marketplace del centro de Partners. 

Si una oferta de ISV no aparece como se espera en el centro de Partners, puede deberse a que:

- El ISV decidió no vender la oferta a través del programa CSP. Por ejemplo, es posible que algunos productos de ISV estén disponibles en otras áreas del Marketplace comercial (por ejemplo, en [Microsoft AppSource](https://appsource.microsoft.com/) y [Azure Marketplace](https://azuremarketplace.microsoft.com/)), pero que no aparezcan para los CSP del centro de Partners Marketplace.

- El ISV decidió poner la oferta en exclusiva solo a un número seleccionado de asociados de CSP. Para obtener más información sobre las ofertas exclusivas, vea más adelante en este tema de ayuda.

- Es posible que el tipo de oferta no sea transactable a través del centro de Partners o Azure Portal (por ejemplo, contenedores o algunas ofertas basadas en el uso).

- Es posible que el país de facturación de los clientes asociados no sea compatible con esta oferta de ISV.

## <a name="view-marketplace-offers-in-partner-center"></a>Ver ofertas de Marketplace en el centro de Partners

Para ver las ofertas de Marketplace comercial disponibles en el programa CSP: 

1. Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard)del centro de Partners y seleccione **CSP** en el menú de navegación izquierdo.

2. Seleccione **vender**, seguido de **Marketplace**. De forma predeterminada, verá los productos de todos los tipos y categorías.

3. Seleccione un filtro por tipo o categoría. También puede usar la **búsqueda** para buscar palabras clave específicas, nombres de ofertas o los nombres de los publicadores de ISV.

4. Seleccione una oferta de producto específica de la lista. Esto le llevará a la pestaña Información general del producto, donde puede obtener más información acerca de la oferta. La información de esta pestaña podría incluir: 

    - Una descripción del producto o de la oferta

    - Más información sobre el publicador de ISV

    - Vínculos a documentación o materiales de marketing cargados por el publicador de ISV

    - Otros posibles contactos de ISV para la asistencia al cliente, la ingeniería o un contacto para el programa CSP

5. Para ver más información sobre los planes, las SKU o los precios disponibles de una oferta, seleccione la pestaña **planes y precios** . Esta pestaña le mostrará:

    - Los mercados en los que está disponible esta oferta

    - Una lista de SKU o planes disponibles para la oferta

    - Precios de cada SKU o plan disponibles

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Ver ofertas de Marketplace a través de las API del centro de Partners

Los asociados del programa CSP también pueden usar las API para devolver una lista de ofertas válidas. Las ofertas válidas solo estarán disponibles para que el asociado pueda vender a través del Marketplace del centro de Partners. En el caso de los asociados que usan las API para identificar ofertas en el catálogo, consulte las instrucciones para [obtener una lista de ofertas para un mercado](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market).

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Vea los precios más recientes de la oferta de Marketplace en el centro de Partners

Siga estos pasos para obtener los detalles de precios más recientes asociados a una oferta:

1. Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard)del centro de Partners y seleccione **CSP** en el menú de navegación izquierdo.

2. Seleccione **vender**, seguido de **Marketplace**. Aparecerá una lista de ofertas de Marketplace.

3. Desplácese hacia abajo hasta la sección **Marketplace** (bajo **precios del plan de Azure**) y seleccione **Exportar lista de precios** en la esquina superior derecha. Esto genera una hoja de cálculo con los datos de precios más recientes para SaaS, ofertas basadas en licencias disponibles en los publicadores de ISV. Algunos precios de las aplicaciones de Azure también pueden aparecer aquí. Esta información se actualiza diariamente, por lo que se puede comprobar el precio actual con la frecuencia que se elija.

4. Si un producto ISV incluye un período de evaluación gratuita, la hoja de cálculo mostrará dos filas para ese producto:

    - Una fila muestra el precio de evaluación gratuita de cero. Esto significa que hay disponible un período de evaluación gratuita.

    - La otra fila muestra el precio y los términos que se aplicarán una vez finalizado el período de evaluación gratuita.

Como asociado del programa CSP, puede ser válido para otros incentivos asociados a determinadas ofertas de Marketplace comerciales. Para obtener más información acerca de otros incentivos, consulte la [Guía de incentivos de CSP](https://aka.ms/partnerincentives) (requiere inicio de sesión de CSP).

## <a name="learn-about-marketplace-exclusive-offers"></a>Más información sobre las ofertas exclusivas de Marketplace

Los ISV tienen la opción de hacer que sus ofertas estén disponibles solo para determinados asociados en el programa CSP. Esto se conoce como una oferta exclusiva. Todos los asociados del programa CSP todavía pueden ver todas las ofertas de ISV en el Marketplace comercial del centro de Partners, incluidas las ofertas marcadas como exclusivas.

Si una oferta **no** está marcada como exclusiva, todos los asociados pueden adquirirla (suponiendo que el país de facturación seleccionado del cliente coincida con la disponibilidad del país de la oferta del ISV).

En el caso de cualquier oferta marcada como exclusiva, sin embargo, solo los asociados seleccionados por el ISV podrán comprar esa oferta.

> [!NOTE]
> Si ve una oferta marcada como exclusiva que le gustaría vender a sus clientes, póngase en contacto directamente con el ISV y pida permiso para vender la oferta exclusiva. Al ver los detalles de una oferta exclusiva, puede ver un vínculo de **ISV de contacto** que puede seleccionar.

Para obtener más información sobre la experiencia de ISV en Marketplace comercial, lea [proveedores de soluciones](https://docs.microsoft.com/azure/marketplace/cloud-solution-providers)en la nube.

Para obtener más información sobre la experiencia de CSP en Marketplace, consulte [información general de Marketplace comercial](csp-commercial-marketplace-overview.md).

## <a name="next-steps"></a>Pasos siguientes

- [Comprar ofertas comerciales de Marketplace](csp-commercial-marketplace-purchase.md)