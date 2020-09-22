---
title: 'Información general: CSP Marketplace'
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprenda a vender suscripciones de clientes a ofertas de software como servicio (SaaS) de fabricantes de software independientes (ISV) en Marketplace.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 66fc51901e6c6e72698eaf4a669627b228ee63ba
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000409"
---
# <a name="overview-of-the-commercial-marketplace-in-partner-center"></a>Información general sobre Marketplace comercial del Centro de partners

**Se aplica a**

- Centro de partners
- Partners del programa CSP

Ser un asociado en el programa proveedor de soluciones en la nube (CSP) le permite agrupar y vender productos de Microsoft junto con soluciones publicadas por proveedores de software independientes (ISV) de terceros. Poder agrupar soluciones de esta manera le permite atender mejor a los clientes finales y aumentar su negocio de servicios de CSP.

Como asociado en el programa CSP, puede usar el centro de partners para comprar muchas soluciones de ISV del Marketplace comercial de Microsoft. Esto le proporciona varias ventajas clave a usted y a sus clientes:

- Acceso a un catálogo de soluciones de software optimizadas para entornos y tecnologías de Microsoft.
- Ciclo de adquisición simplificado y reducido.
- Una única integración con las API del centro de Partners. (Esta integración permite el acceso a un catálogo de soluciones de ISV, reduce el costo de las operaciones y la ingeniería, y simplifica la administración de varias suscripciones de proveedor y la facturación a través de un solo proveedor).
- Implementación y aprovisionamiento simplificados en el inquilino de Azure del cliente (para soluciones basadas en máquinas virtuales).
- Reduce los posibles desafíos con la compra directa o la contratación de ISV, la configuración y la integración de soluciones de Microsoft, y la necesidad de administrar o consolidar las facturas periódicas de varios proveedores.

## <a name="overview-of-csp-offers-in-the-commercial-marketplace"></a>Información general sobre las ofertas de CSP en Marketplace comercial

Si es un asociado en el programa CSP, hay muchas actividades comerciales de Marketplace que puede querer realizar en lo que respecta a las ofertas de ISV. Vea la tabla siguiente para obtener más información acerca de cada actividad.

|**Si desea**  |**Lectura**   |
|:------------------------------------|:------------------|
|Obtenga información acerca de cómo ver o Buscar ofertas disponibles, precios, detalles del producto o información de contacto del editor | [Detección de ofertas](csp-commercial-marketplace-discover.md) | 
|Obtenga información sobre cómo comprar e implementar una oferta   | [Ofertas de compra](csp-commercial-marketplace-purchase.md)   | 
|Obtenga información sobre cómo cancelar o renovar una suscripción o agregar o quitar licencias.  | [Administración de ofertas](csp-commercial-marketplace-manage.md) |
|Más información sobre cómo funciona la facturación para las compras comerciales de Marketplace | [Descripción de la facturación](csp-commercial-marketplace-billing.md) |
|Más información sobre quién es responsable de qué tipos de soporte técnico para compras de ISV | [Descripción del soporte técnico](csp-commercial-marketplace-support.md) |
|Obtenga información acerca de los contratos y las responsabilidades de los asociados de CSP e ISV en el Marketplace comercial | [Comprender la contratación](csp-commercial-marketplace-contracting.md) |

> [!NOTE]
> En esta información general se describe cómo los asociados del programa CSP pueden usar determinadas características de Marketplace comercial en el centro de Partners. A diferencia de los asociados en el programa CSP, los publicadores ISV tienen un rol de Marketplace diferente. También tienen disponibles diferentes características de Marketplace comercial en el centro de Partners. Para obtener más información sobre el rol de los editores de ISV, consulte la [Introducción a Azure Commercial Marketplace](/azure/marketplace/partner-center-portal/commercial-marketplace-overview).

## <a name="where-to-complete-commercial-marketplace-activities"></a>Dónde completar las actividades comerciales de Marketplace

Como asociado en el programa CSP, puede completar muchas actividades comerciales de Marketplace para las ofertas de SaaS de ISV directamente desde el [Panel](https://partner.microsoft.com/dashboard) del centro de Partners o mediante las [API del centro de Partners](/partner-center/develop/). Sin embargo, para realizar otras actividades de Marketplace, puede que tenga que ir a:

- [Portal de administración de Microsoft Azure](https://portal.azure.com/)

    O bien

- Un sistema o sitio web de un publicador de ISV de terceros

Gran parte del lugar en el que vaya a completar actividades comienza con el tipo de oferta que elija. En la actualidad, los asociados del programa CSP pueden Transact dos tipos de ofertas con publicadores de ISV de terceros:

1. Ofertas SaaS basadas en licencias  
2. Ofertas basadas en el uso (incluidas las ofertas basadas en máquinas virtuales, contenedores o aplicaciones de Azure)

Vaya a los [conceptos básicos de facturación](billing-basics.md) para obtener más información sobre cómo la facturación difiere entre las ofertas basadas en licencias y las ofertas basadas en el uso.  

Para saber dónde completar una actividad específica de Marketplace para las ofertas de ISV basadas en licencias o en el uso, consulte las tablas siguientes.

|**Para las ofertas de SaaS basadas en licencias de ISV**  |**Uso**  |
|:------------------------------------|:------------------|
|Para detectar o Buscar ofertas disponibles  | API del centro de Partners o del centro de Partners  |
|Para comprar una oferta  | API del centro de Partners o del centro de Partners  |
|Para implementar una oferta comprada (configuración de la cuenta, administración de software o implementación en el inquilino de AAD del cliente)  | Sistema o sitio web del anunciante de ISV  |
|Para cancelar o renovar las suscripciones de la oferta o agregar o quitar licencias | API del centro de Partners o del centro de Partners  |
|Para crear usuarios o administrar permisos  | Sistema o sitio web del anunciante de ISV  |

|**Para las ofertas basadas en el uso de ISV**  |**Uso**  |
|:------------------------------------|:------------------|
|Para detectar o Buscar ofertas disponibles  | Panel del centro de Partners, API del centro de Partners o Azure Portal  |
|Para comprar una oferta  | Azure portal  |
|Para implementar una oferta comprada (configuración de la cuenta, administración de software o implementación en el inquilino de AAD del cliente)  | Azure portal  |
|Para cancelar o renovar las suscripciones de la oferta o agregar o quitar licencias | Azure portal  |
|Para crear usuarios o administrar permisos  | Azure Portal  |

## <a name="next-steps"></a>Pasos siguientes

- [Descubra o vea ofertas comerciales de Marketplace](csp-commercial-marketplace-discover.md)
- [Comprar ofertas comerciales de Marketplace](csp-commercial-marketplace-purchase.md)