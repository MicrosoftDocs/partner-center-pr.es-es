---
title: 'Detectar ofertas: marketplace comercial'
ms.topic: how-to
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo los asociados de CSP pueden usar Centro de partners para ver o buscar ofertas de SaaS o precios en Marketplace de proveedores de software independientes (ISV).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ab30f8391df58155c8511dc628b1fefd94c8d768
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147979"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>Descubra ofertas y precios en Centro de partners marketplace comercial

**Roles adecuados:** Administrador global | Agente de administración

Cuando los proveedores de software independientes (ISV) deciden publicar una oferta en el marketplace comercial, también pueden decidir si quieren que la oferta esté disponible en el programa CSP. Si deciden vender la oferta a través del programa CSP, los asociados de CSP deben ver la oferta en Centro de partners Marketplace.

Si una oferta de ISV no aparece como se espera en Centro de partners, puede deberse a lo siguiente:

- El ISV decidió no vender la oferta a través del programa CSP. Por ejemplo, es posible que algunos productos de ISV estén disponibles en otras áreas del marketplace comercial (como [en Microsoft AppSource](https://appsource.microsoft.com/) y [Azure Marketplace),](https://azuremarketplace.microsoft.com/)pero es posible que no aparezcan para los asociados del programa CSP en Centro de partners Marketplace.

- El ISV decidió hacer que la oferta fuera exclusiva solo para un número selecto de asociados de CSP. Para obtener más información sobre las ofertas exclusivas, vea más adelante en este tema de ayuda.

- Es posible que el tipo de oferta no sea transaccionable Centro de partners o Azure Portal (por ejemplo, contenedores o algunas ofertas basadas en el uso).

- Es posible que el país de facturación de los clientes asociados no sea compatible con esta oferta de ISV.

## <a name="view-marketplace-offers-in-partner-center"></a>Visualización de ofertas de Marketplace en Centro de partners

Para ver las ofertas de Marketplace comercial disponibles en el programa CSP:

1. Inicie sesión Centro de partners [panel y,](https://partner.microsoft.com/dashboard)a continuación, **seleccione CSP** en el menú de navegación izquierdo.

2. Seleccione **Vender,** seguido de **Marketplace.** De forma predeterminada, verá productos de todos los tipos y categorías.

3. Seleccione un filtro por tipo o categoría. También puede usar La **búsqueda para** buscar palabras clave específicas, nombres de ofertas o nombres de publicadores de ISV.

4. Seleccione una oferta de producto específica de la lista. Esto le llevará a una pestaña Información general del producto donde puede obtener más información sobre la oferta. La información de esta pestaña podría incluir: 

    - Una descripción del producto u oferta

    - Más información sobre el publicador de ISV

    - Vínculos a documentación o materiales de marketing cargados por el publicador de ISV

    - Otros posibles contactos de ISV para el soporte al cliente, ingeniería o un contacto para el programa CSP

5. Para obtener más información sobre los planes disponibles, las SKU o los precios de una oferta, seleccione la **pestaña Planes y** precios. Esta pestaña le mostrará:

    - Los mercados en los que está disponible esta oferta

    - Una lista de SKU o planes disponibles para la oferta

    - Precios de cada SKU o plan disponible

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Visualización de ofertas de Marketplace mediante Centro de partners API

Los asociados del programa CSP también pueden usar las API para devolver una lista de ofertas aptas. Las ofertas aptas serán solo aquellas ofertas de ISV de SaaS disponibles para que el asociado las pueda vender a través Centro de partners Marketplace. Para los asociados que usan API para identificar ofertas en el catálogo, consulte la guía para obtener una lista [de ofertas para un mercado.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Vea los precios más recientes de las ofertas de Marketplace en Centro de partners

Siga estos pasos para obtener los detalles de precios más recientes asociados a una oferta:

1. Inicie sesión en Centro de partners [panel y,](https://partner.microsoft.com/dashboard)a continuación, **seleccione CSP** en el menú de navegación izquierdo.

2. Seleccione **Vender,** seguido de **Precios y ofertas.**

3. Desplácese hacia abajo hasta la **sección Marketplace,** seleccione una ubicación y descargue **precios de Marketplace.** Esto genera una hoja de cálculo con los datos de precios más recientes de SaaS, las ofertas basadas en licencias y las ofertas de uso medidor disponibles en los publicadores de ISV. Algunos precios de aplicaciones de Azure también pueden aparecer aquí. Esta información se actualiza diariamente, por lo que puede comprobar los precios actuales con la frecuencia que elija.

4. Si un producto ISV incluye un período de evaluación gratuita, la hoja de cálculo mostrará dos filas para ese producto:

    - Una fila muestra el precio de evaluación gratuita de cero. Esto significa que hay disponible un período de evaluación gratuita.

    - La otra fila muestra el precio y los términos que se aplicarán una vez que se supere el período de evaluación gratuita.

Como asociado del programa CSP, puede ser apto para otros incentivos asociados a determinadas ofertas de marketplace comercial. Para más información sobre otros incentivos, consulte la guía [de incentivos de CSP](https://aka.ms/partnerincentives) (requiere inicio de sesión de CSP).

## <a name="learn-about-marketplace-exclusive-offers"></a>Más información sobre las ofertas exclusivas de Marketplace

Los ISV tienen la opción de hacer que sus ofertas estén disponibles solo para asociados específicos del programa CSP. Esto se conoce como oferta exclusiva. Todos los asociados del programa CSP todavía pueden ver todas las ofertas de ISV Centro de partners marketplace comercial, incluidas las ofertas marcadas como Exclusivas.

Si una oferta **no** está marcada como Exclusiva, todos los asociados pueden comprar esa oferta (suponiendo que el país de facturación del cliente seleccionado coincida con la disponibilidad de país de la oferta del ISV).

Sin embargo, para cualquier oferta marcada como Exclusiva, solo los asociados seleccionados por el ISV podrán comprar esa oferta.

> [!NOTE]
> Si ve una oferta marcada como Exclusiva que le gustaría vender a sus clientes, puede ponerse en contacto directamente con el ISV y solicitar permiso para vender la oferta exclusiva. Al ver los detalles de una oferta exclusiva, es posible que vea un vínculo Ponerse en contacto con **ISV** que puede seleccionar.

Para obtener más información sobre la experiencia de ISV en el marketplace comercial, lea [Proveedores de soluciones en la nube](/azure/marketplace/cloud-solution-providers).

Para obtener más información sobre la experiencia de CSP en Marketplace, lea [Introducción al marketplace comercial.](csp-commercial-marketplace-overview.md)

## <a name="next-steps"></a>Pasos siguientes

- [Compra de ofertas de Marketplace comercial](csp-commercial-marketplace-purchase.md)