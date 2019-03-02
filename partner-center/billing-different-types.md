---
title: Descripción de los tipos de facturación en el centro de partners | El centro de partners
ms.topic: article
ms.date: 03/01/2019
Description: Obtener información sobre los distintos tipos de facturación, períodos de facturación y las fechas de facturación
author: labrenne
ms.author: labrenne
keywords: facturación, pagos, pedidos, archivos de conciliación, archivo de conciliación
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 777a98f8780eb036b4bac99eca9a5621d61da66b
ms.sourcegitcommit: 8bfd1358a0ef86e46bee2a1097d86de3c9e969e8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/02/2019
ms.locfileid: "9122315"
---
# <a name="understanding-the-types-of-billing-in-partner-center"></a>Descripción de los tipos de facturación en el centro de partners

**Se aplica a:**

-  Centro de partners
-  Partners en el programa CSP

Dependiendo de los tipos de productos que has comprado para los clientes, podría tener diferentes períodos de facturación y enviará una factura en días diferentes del mismo mes. En este artículo se explica lo que está cambiando a partir del 1 de marzo de 2019, y cómo afectará a los cambios.

## <a name="billing-for-recurring-charges"></a>Facturación para cargos periódicos

No está cambiando la experiencia de facturación para cargos periódicos de suscripciones basadas en licencia y basadas en uso. Continuaremos facturará el día del mes que se seleccione como la fecha de facturación y el período de facturación seguirá siendo el mes antes de esa fecha. Si has seleccionado el día 15 del mes de la fecha de facturación, se facturará para toda la actividad desde el 15 de un mes para el 14 del próximo mes del calendario. Facturas y archivos de conciliación están disponibles para el público 2 a 4 días después de la fecha de facturación.

Como antes, se te facturará de estos productos en la moneda del país o región en que encuentran, independientemente de la ubicación del cliente vender el producto.

## <a name="billing-for-one-time-and-select-recurring-charges"></a>Facturación para cargos periódicos de una sola vez y seleccionados

A partir del 1 de marzo de 2019, presentamos una nueva experiencia de facturación para cargos periódicos y única para productos de Microsoft y de terceros ISV.

Para estos productos, el período de facturación comienza en el primer día del mes del calendario y termina el último día del mes del calendario. Haremos que la factura disponible 8 días del mes siguiente. 

En otras palabras, todas las transacciones que realices entre el 1 de mayo y el 31 de mayo de 2019 aparecerán en tu factura de 8 de junio. Las transacciones que realices entre el 1 de junio y el 30 de junio de 2019 aparecerán en tu factura de 8 de julio. Te podría obtener una factura para las compras periódicas y única en la misma factura. 

También puedes comprobar tu saldo de cuenta o factura siempre que quieras (por ejemplo, entre el 1 de mayo y 7 de junio) y ver la actividad más reciente de la cuenta sin tener que esperar la factura. Ten en cuenta que cuando se registra la factura en el 8, incluirá impuestos y otros cargos aplicables y los créditos, por lo que la cantidad final puede diferir de lo que aparece durante el período de facturación. 

Tendrá acceso a las facturas de la misma forma que debes hacer ahora, en el centro de partners o por la API. Aparecerá antes de medianoche UTC de 8 días del mes. 

|**Experiencia de facturación**|**Tipos de producto**|**Fecha de facturación**|**Billing period**|**Divisa de facturación**|**¿Actividad actual disponible?**|
|:----------------|:--------------|:--------------|:--------------|:--------------|:--------------|
|Cargos periódicos de suscripciones basadas en licencia y basadas en uso |Todos los productos del [catálogo de servicios en línea](https://partner.microsoft.com/commerce/preferredoffers/list). Algunos ejemplos son Office 365, Microsoft 365, Azure Active Directory, Azure (pago por uso), Dynamics 365, PowerBI Pro |La fecha seleccionada al crear la cuenta del centro de partners |El mes antes de la fecha de facturación. |La moneda del país o región encuentran en. Por ejemplo, si tu empresa se encuentra en el Reino Unido, se te facturará en libras esterlinas (GBP). Si tu empresa se encuentra en la India, te enviaremos bill en India rupias (INR).  |No |
|Cargos periódicos y único para productos de Microsoft y de terceros ISV |Todos los SaaS suscripciones, reservas de Azure y productos de software (permanente y suscripción) que ofrece Microsoft e ISV de terceros. Ver los productos disponibles en el [mercado](https://partner.microsoft.com/commerce/sales?type=Any&category=Any). Algunos ejemplos son software SUSE Linux (suscripción de software), Windows Server 2019 Essentials (software permanente), Azure ISV SaaS suscripción del producto. |8 días de cada mes |Desde el primer día en el último día de cada mes del calendario |La moneda del país o región del cliente se encuentra en. Esto significa que recibirás diferentes facturas y archivos de conciliación en la moneda del país o región cada cliente vendido a en el período de facturación. |Sí |
