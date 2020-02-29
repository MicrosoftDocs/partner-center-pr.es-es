---
title: Precios y ofertas | Centro de partners
ms.topic: article
ms.date: 02/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: La lista de ofertas incluye las distintas familias de productos que se pueden adquirir a través del centro de Partners y su información de precios.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e33b89e76a57e1e6f5457e208a61bc04ad841271
ms.sourcegitcommit: 2634057663a0ea27393212f898018538dada796e
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 02/28/2020
ms.locfileid: "78161519"
---
# <a name="pricing-and-offers"></a>Precios y ofertas

**Se aplica a**

-  Centro de asociados

**Roles adecuados**
-   Administrador global
-   Administrador de usuarios
-   Agente de administrador
-   Administrador de partners de MPN
-   Agente de ventas
-   Administrador de facturación

Para ver los programas y ofertas más recientes del proveedor de soluciones en la nube, vaya a **vender > precios y ofertas**. Encontrará listas de precios independientes para los servicios basados en licencias, como Office 365, Microsoft Dynamics CRM y Enterprise Mobility Suite, y para los servicios basados en uso que incluyen Azure. 

La lista de ofertas incluye las distintas familias de productos que se pueden adquirir a través del centro de Partners. Estos actualmente incluyen Office 365, Enterprise Mobility Suite, Microsoft Dynamics CRM y Microsoft Azure. Esta lista se seguirá expandiendo a medida que los nuevos productos estén disponibles.

Dentro de cada una de estas familias de productos, hay diferentes SKU y paquetes de productos disponibles para su venta en función de su negocio. Siempre puede tener acceso a los detalles más recientes sobre estos productos mediante la matriz de ofertas de revendedores en la nube, que está disponible en la página precios y ofertas.

## <a name="price-list-preview-and-change-frequency"></a>Vista previa de la lista de precios y frecuencia de cambio 

Los servicios basados en licencias incluyen una vista previa de la lista de precios, siempre con 30 días antes de que se realicen cambios. Para ver la vista previa de la lista de precios, vaya a **vender > precios y ofertas**. No hay ninguna vista previa de precios para los servicios basados en uso ya que estos servicios son dinámicos. En la tabla siguiente se explica cómo leer la tabla de lista de precios.

|**Item**        |**Definición**      |
|:-----------   |:-----------   |
|SUMA   |Un nuevo elemento a la lista de precios|
|CHG   |Cambia el precio de venta de mes a mes. Pueden producirse otros cambios no relacionados con el precio de la lista, los asociados deben comparar las listas de precios entre meses para determinar los cambios en otras propiedades.|
|SUPR   |Un elemento quitado de la lista de precios|
|UNC   |Precio de lista sin cambios en la lista de precios del mes anterior  |
|Valid from date   |La primera fecha en la que se puede pedir una oferta    |
|Valid to date   |La última fecha en la que se puede pedir una oferta   |
|Offer display name   |El nombre de la oferta que se mostrará a los clientes   |
|Identificador de oferta   |El identificador interno de la oferta   |
|License agreement type   |Los tipos de contrato de licencia pueden ser corporativos, gubernamentales o académicos y determinar a qué tipos de clientes se puede vender la oferta.|
|Purchase unit   |La duración de la oferta que se compra. Las unidades de compra suelen ser de un mes.   |
|Secondary license type   |Los tipos de licencias secundarias serán no específicos, complemento o evaluación. Complemento indica que hay productos necesarios que el cliente debe comprar antes de comprar el complemento.|
|End customer type   |Vuelve a estar relacionado con el tipo de contrato de licencia: licencia corporativa: Reseller de la nube de la empresa, licencia de gobierno, administrador de revendedores de la nube o licencia académica-profesor del distribuidor de la nube o estudiante del Reseller de la nube   |
|List price   |El precio que el partner pagará   |
|ERP price   |El precio estimado o recomendado de venta para el cliente   |

## <a name="price-changes"></a>Cambios de precio

Los cambios de precio son una repetición común. Los asociados pueden anticiparse a los cambios de precios de las ofertas basadas en licencias. para ello, examine la vista previa de la lista de precios en la página precios y ofertas en el panel del centro de Partners. Los precios basados en el uso de Azure no tienen vista previa. Los asociados pueden mantenerse al día con los cambios de precios de consumo de Azure mediante la API de RateCard, que devuelve los precios de las métricas de ese día.

|**Tipo de producto**   |**Ejemplos de productos**  |**Vista previa disponible** |**Cambiar detalles**|
|-----------------------|:-----------------------|:-------------------|------------------|
|Basado en licencia|Office, Dynamics, Intune, Windows Enterprise|30 días|Lista de cambios de precios marcados como CHNG en las listas de precios de vista previa|
|Basado en el uso|Recursos de Azure|No disponible|Registro de cambios disponible en la pestaña **historial de cambios** de la lista de precios del mes anterior|
|Software||No disponible|Comparar listas de precios manualmente de un mes a otro|
|Reservas|Máquinas virtuales, prepago|No disponible|Comparar listas de precios manualmente de un mes a otro|

Los precios basados en el uso pueden cambiar a lo largo de un mes. Para obtener los precios diarios actuales de estos recursos de Azure, los asociados deben llamar a la API de RateCard. 

>[!Note] 
>Los cambios de precio de suscripción solo se aplican durante una renovación. Los cargos mensuales de un asociado se determinan con el precio de compra o el precio en el momento de la creación de una suscripción. Si un precio aumenta o disminuye después de adquirir el plazo anual, el asociado no se cobrará el precio modificado hasta la renovación, normalmente en el plazo de 12 meses.

## <a name="pricing-and-special-segments"></a>Precios y segmentos especiales

CSP ofrece algunos servicios a segmentos de mercado especiales, por ejemplo, educación, sin ánimo de lucro y en la nube de la comunidad gubernamental. No todos los servicios están disponibles en todos los canales. Ningún segmento tiene como valor predeterminado lo que llamamos segmento "comercial". Todos los precios basados en licencias están disponibles en la lista de precios basada en licencias en la página precios y ofertas. Azure Government precios está disponible en la lista de precios basada en el uso cuando se inicia sesión en el inquilino de CSP habilitado para Azure Government.

|**Sector**   |**Quién debe calificar**   |**El asociado califica al cliente**|**Tipos de productos habilitados**|
|-------------------|-----------------------|----------------------------|-----------------------------|
|Educación|Cliente|No, Microsoft llevará a cabo la calificación del cliente |Solo basado en licencia|
|Sin ánimo de lucro|Cliente|No, el cliente se califica fuera del centro de Partners|Solo basado en licencia|
|Government Community Cloud (GCC)|Socio comercial y cliente|Una vez habilitado GCC, el asociado puede crear clientes GCC| Solo basado en licencia|
|Azure gov|Asociado|Una vez calificada, el asociado funciona en un inquilino de CSP específico de Azure gov|Recursos de Azure|

Los márgenes asociados, la diferencia entre el precio de venta y los precios de venta estimados, pueden variar de segmento a segmento. Normalmente, la educación y los no beneficios suelen tener márgenes inferiores o no para los asociados de CSP. Consulte la lista de precios basada en licencias para ver los valores exactos.  
## <a name="pricing-between-azure-and-non-azure"></a>Precios entre Azure y no Azure

Los precios difieren en diferentes tipos de ofertas. Los precios basados en licencias suelen ser la cantidad por puesto (licencia) de un mes determinado. Los precios basados en el uso se determinan mediante el uso de un recurso determinado, con un identificador de medidor asociado. Los asociados no se cobran por adquirir la suscripción de Azure, pero se cobra por los recursos consumidos por diferentes implementaciones en la suscripción. Los precios de la lista de precios basada en el uso están organizados en torno a distintos identificadores de medidor de recursos en Azure.

Las reservas de Azure son compras basadas en términos para el tipo de recurso en particular Virtual Machines. La compra de una reserva de Azure permite que un asociado pague previamente (términos de una o tres años) y Reserve una máquina virtual determinada, lo que ahorra dinero al socio y garantiza que su máquina virtual siempre está disponible mientras dure el plazo. Un asociado puede alinear la reserva que desee con los identificadores de medidor de recursos basados en el uso. Los identificadores de medidor son coherentes en todo el recurso, tanto si el asociado compra una máquina virtual como si simplemente implementa la máquina virtual como un recurso basado en el uso. 


## <a name="offers-matrix"></a>Matriz de ofertas

Obtén información sobre los diferentes paquetes de productos y SKU que están disponibles para vender en la Matriz de ofertas para revendedores de soluciones en la nube en la página Precios y ofertas. La matriz de ofertas incluye las ofertas que están disponibles por configuración regional. Si un elemento está en la lista de precios pero todavía no aparece en la matriz de la oferta, significa que aún no se pueden ordenar los productos. En cuanto estén disponibles para pedirse, la matriz de ofertas se actualiza.

Para los partners CSP que usan los Kits de desarrollo de software (SDK) del Centro de partners. Microsoft también publica una lista de los servicios de Azure en CSP en la página Precios y ofertas.

### <a name="offers-matrix-and-price-list-questions"></a>Ofrece preguntas sobre matrices y listas de precios

Si tiene preguntas sobre la lista de precios o la matriz de ofertas, envíe una solicitud de servicio a través del centro de Partners.

### <a name="taxes-and-pricing"></a>Impuestos y precios

Todos los precios de las listas de precios de CSP del centro de Partners son impuestos incluidos. Para obtener más información en el centro de Partners, documentar los [impuestos y las exenciones fiscales](https://docs.microsoft.com/partner-center/tax-and-tax-exemptions).
