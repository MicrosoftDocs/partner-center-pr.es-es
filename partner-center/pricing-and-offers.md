---
title: Precios y ofertas | Centro de partners
ms.topic: article
ms.date: 09/26/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: La lista de ofertas incluye las distintas familias de productos que se pueden adquirir a través del centro de Partners y su información de precios.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: ca270413291ba0d09ca03d9b8b270a65f77a46b1
ms.sourcegitcommit: 2ba40700aeb94c38ba850973dd7ff3330c577937
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/03/2020
ms.locfileid: "75631829"
---
# <a name="pricing-and-offers"></a>Precios y ofertas

**Se aplica a**

-  Centro de partners

**Roles adecuados**
-   Administrador global
-   Administrador de usuarios
-   Agente de administración
-   Administrador de partners de MPN
-   Agente de ventas
-   Administrador de facturación

Para ver las últimas listas de precios y ofertas del programa Proveedor de soluciones en la nube, ve a **Vender > Precios y ofertas**. Encontrarás listas de precios independientes para los servicios basados en licencias, tales como Office 365, Microsoft Dynamics CRM y Enterprise Mobility Suite y para los servicios basados en uso, como por ejemplo, Azure. 

La lista de ofertas incluye las distintas familias de productos que se pueden adquirir a través del centro de Partners. Actualmente se incluyen los siguientes productos: Office 365, Enterprise Mobility Suite, Microsoft Dynamics CRM y Microsoft Azure. Esta lista aumentará.

Dentro de cada una de estas gamas de productos hay diferentes SKU y paquetes de productos que están a tu disposición para que los vendas en tu negocio. Siempre puedes acceder a la información más reciente de cada uno de estos productos con la Matriz de ofertas para distribuidores de servicios en la nube que está disponible en la página Precios y ofertas.

## <a name="pricelist-preview-and-change-frequency"></a>Vista previa de lista de precios y frecuencia de cambios 

Los servicios basados en licencias incluye una vista previa de lista de precios, que se proporciona con 30 días de antelación de que se produzcan cambios. Para ver la vista previa de la lista de precios, ve a **Vender > Precios y ofertas**. No hay ninguna vista previa de precios para los servicios basados en uso ya que estos servicios son dinámicos. En la siguiente tabla se explica cómo leer la tabla de lista de precios.

|**Item**        |**Definición**      |
|:-----------   |:-----------   |
|AGREGAR   |Un artículo nuevo a la lista de precios|
|CHG   |Cambia el precio de venta de mes a mes. Pueden producirse otros cambios que no estén relacionados con el precio de la lista, los asociados deben comparar otras propiedades de mes a mes para determinar otros cambios.|
|DEL   |Un artículo que se ha quitado de la lista de precios|
|UNC   |Precio de lista sin cambios en el pricelist del mes anterior  |
|Valid from date   |La primera fecha en la que se puede pedir una oferta    |
|Valid to date   |La última fecha en la que se puede pedir una oferta   |
|Offer display name   |El nombre de la oferta que se mostrará a los clientes   |
|Offer ID   |El identificador interno de la oferta   |
|License agreement type   |Se trata de cualquier contrato corporativo, gubernamental o académico y determina los tipos de clientes a los que se puede vender la oferta.|
|Purchase unit   |La duración de la oferta que se compra. Suele ser un mes.   |
|Secondary license type   |Puede ser de evaluación, complemento o no específica. Complemento indica que hay productos necesarios que el cliente debe comprar antes de comprar el complemento.|
|End customer type   |Guarda relación con el tipo de contrato de licencia: licencia corporativa (licencia gubernamental, corporativa de revendedor de soluciones en la nube), licencia académica o gubernamental de revendedor de soluciones en la nube (estudiante o personal docente revendedores de soluciones en la nube)   |
|List price   |El precio que el partner pagará   |
|ERP price   |El precio estimado o recomendado de venta para el cliente   |

## <a name="price-changes"></a>Cambios en los precios

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

CSP ofrece algunos servicios a segmentos de mercado especiales, por ejemplo, educación, sin ánimo de lucro y en la nube de la comunidad gubernamental. No todos los servicios están disponibles en todos los canales. Ningún segmento tiene como valor predeterminado lo que llamamos segmento "comercial". Todos los precios basados en licencias están disponibles en la lista de precios basada en licencias en la página precios y ofertas. Los precios de Azure gov están disponibles en la lista de precios basada en el uso cuando se inicia sesión en el inquilino de CSP habilitado para Azure gov.

|**Segmento**   |**Quién debe calificar**   |**El asociado califica al cliente**|**Tipos de productos habilitados**|
|-------------------|-----------------------|----------------------------|-----------------------------|
|Education|Cliente|No, Microsoft llevará a cabo la calificación del cliente |Solo basado en licencia|
|Sin ánimo de lucro|Cliente|No, el cliente se califica fuera del centro de Partners|Solo basado en licencia|
|Government Community Cloud (GCC)|Socio comercial y cliente|Una vez habilitado GCC, el asociado puede crear clientes GCC| Solo basado en licencia|
|Azure gov|Partner|Una vez calificada, el asociado funciona en un inquilino de CSP específico de Azure gov|Recursos de Azure|

Los márgenes asociados, la diferencia entre el precio de venta y los precios de venta estimados, pueden variar de segmento a segmento. Normalmente, la educación y los no beneficios suelen tener márgenes inferiores o no para los asociados de CSP. Consulte la lista de precios basada en licencias para ver los valores exactos.  
## <a name="pricing-between-azure-and-non-azure"></a>Precios entre Azure y no Azure

Los precios difieren en diferentes tipos de ofertas. Los precios basados en licencias suelen ser la cantidad por puesto (licencia) de un mes determinado. Los precios basados en el uso se determinan mediante el uso de un recurso determinado, con un identificador de medidor asociado. Los asociados no se cobran por adquirir la suscripción de Azure, pero se cobra por los recursos consumidos por diferentes implementaciones en la suscripción. Los precios de la lista de precios basada en el uso están organizados en torno a distintos identificadores de medidor de recursos en Azure.

Las reservas de Azure son compras basadas en términos para el tipo de recurso en particular Virtual Machines. La compra de una reserva de Azure permite que un asociado pague previamente (términos de uno o tres años) y Reserve una máquina virtual determinada. Esto ahorra dinero al socio comercial y garantiza que su máquina virtual siempre está disponible mientras dure el período. Un asociado puede alinear la reserva que desee con los identificadores de medidor de recursos basados en el uso. Los identificadores de medidor son coherentes en todo el recurso, tanto si el asociado compra una máquina virtual como si simplemente implementa la máquina virtual como un recurso basado en el uso. 


## <a name="offers-matrix"></a>Matriz de ofertas

Obtén información sobre los diferentes paquetes de productos y SKU que están disponibles para vender en la Matriz de ofertas para revendedores de soluciones en la nube en la página Precios y ofertas. La matriz de ofertas incluye las ofertas que están disponibles por configuración regional. Si un artículo se encuentra en la lista de precios pero aún no aparece en la matriz de ofertas, esto significa que aún no se pueden solicitar los productos. En cuanto estén disponibles para pedirse, la matriz de ofertas se actualiza.

Para los asociados de CSP que usan los kits de desarrollo de software (SDK) del centro de Partners. Microsoft también publica una lista de los servicios de Azure en CSP en la página Precios y ofertas.

### <a name="offers-matrix-and-pricelist-questions"></a>Preguntas sobre la lista de precios y la matriz de ofertas

Si tiene alguna pregunta sobre la matriz de pricelist o de la oferta, envíe una solicitud de servicio a través del centro de Partners.
