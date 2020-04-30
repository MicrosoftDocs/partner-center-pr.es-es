---
title: Precios y ofertas
ms.topic: article
ms.date: 02/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: La lista de ofertas incluye las distintas familias de productos que se pueden adquirir a través del centro de Partners y su información de precios.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 19e935122d1223c87714ca8c3a3f4fd212f2cf3c
ms.sourcegitcommit: 4731d6647db34cf214f781f9e002074210fcfc29
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/21/2020
ms.locfileid: "81664284"
---
# <a name="pricing-and-offers"></a>Precios y ofertas

**Se aplica a**

- Centro de partners

**Roles adecuados**

- Administrador global
- Administrador de usuarios
- Agente de administrador
- Administrador de partners de MPN
- Agente de ventas
- Administrador de facturación

Para ver los programas y ofertas más recientes del proveedor de soluciones en la nube, desde el portal de Partners, vaya a **vender > precios y ofertas**. Encontrará listas de precios independientes para los servicios basados en licencias, como Office 365, Microsoft Dynamics CRM y Enterprise Mobility Suite, y para los servicios basados en uso que incluyen Azure.

La lista de ofertas incluye las distintas familias de productos que se pueden adquirir a través del centro de Partners. Estos actualmente incluyen Office 365, Enterprise Mobility Suite, Microsoft Dynamics CRM y Microsoft Azure. Esta lista se seguirá expandiendo a medida que los nuevos productos estén disponibles.

Dentro de cada una de estas familias de productos, hay diferentes SKU y paquetes de productos disponibles para su venta en función de su negocio. Siempre puede tener acceso a los detalles más recientes sobre estos productos mediante la matriz de ofertas de revendedores en la nube, que está disponible en la página precios y ofertas.

## <a name="price-list-preview-and-change-frequency"></a>Vista previa de la lista de precios y frecuencia de cambio 

Los servicios basados en licencias incluyen una vista previa de la lista de precios, siempre con 30 días antes de que se realicen cambios. Para ver la vista previa de la lista de precios, vaya a **vender > precios y ofertas**. No hay ninguna vista previa de precios para los servicios basados en el uso, ya que estos servicios son dinámicos. En la tabla siguiente se explica cómo leer la tabla de lista de precios.

|**Elemento**        |**Definición**      |
|:-----------   |:-----------   |
|ADD   |Un nuevo elemento a la lista de precios|
|PREC   |Cambia el precio de venta de mes a mes. Pueden producirse otros cambios no relacionados con el precio de la lista, los asociados deben comparar las listas de precios entre meses para determinar los cambios en otras propiedades.|
|DEL   |Un elemento quitado de la lista de precios|
|UNC   |Precio de lista sin cambios en la lista de precios del mes anterior  |
|Válido desde fecha   |La primera fecha en que se puede ordenar una oferta    |
|Válido hasta la fecha   |La última fecha en que se puede ordenar una oferta   |
|Nombre para mostrar de la oferta   |El nombre del cliente para la oferta   |
|Id. de oferta   |Identificador interno de la oferta.   |
|Tipo de contrato de licencia   |Los tipos de contrato de licencia pueden ser corporativos, gubernamentales o académicos. El tipo de contrato determina a qué tipos de clientes se puede vender la oferta.|
|Unidad de compra   |La duración de compra de la oferta. Las unidades de compra suelen ser de un mes.   |
|Tipo de licencia secundario   |Los tipos de licencias secundarias serán no específicos, complemento o evaluación. El complemento indica que hay productos necesarios que el cliente debe adquirir antes de adquirir el complemento.|
|Tipo de cliente final   |Vuelve a estar relacionado con el tipo de contrato de licencia: licencia corporativa: Reseller de la nube de la empresa, licencia de gobierno, administrador de revendedores de la nube o licencia académica-profesor del distribuidor de la nube o estudiante del Reseller de la nube   |
|Precio de lista   |El precio que pagará el asociado   |
|Precio de ERP   |El precio de venta al cliente estimado o recomendado   |

## <a name="price-changes"></a>Cambios en los precios

Los cambios de precio son una repetición común. Los asociados pueden anticiparse a los cambios de precios de las ofertas basadas en licencias mirando la vista previa de la lista de precios. En el panel del centro de Partners, abra la página precios y ofertas para ver la vista previa de la lista de precios.

Sin embargo, los precios basados en el uso de Azure no tienen vista previa. Los asociados pueden mantenerse al día con los cambios de precios de consumo de Azure mediante la API de RateCard, que devuelve los precios de las métricas de ese día.

|**Tipo de producto**   |**Ejemplos de productos**  |**Vista previa disponible** |**Cambiar detalles**|
|-----------------------|:-----------------------|:-------------------|------------------|
|Basado en licencia|Office, Dynamics, Intune, Windows Enterprise|30 días|Lista de cambios de precios marcados como CHNG en las listas de precios de vista previa|
|Basado en el uso|Recursos de Azure|No disponible|Registro de cambios disponible en la pestaña **historial de cambios** de la lista de precios del mes anterior|
|Software||No disponible|Comparar listas de precios manualmente de un mes a otro|
|Reservations|Máquinas virtuales, prepago|No disponible|Comparar listas de precios manualmente de un mes a otro|

Los precios basados en el uso pueden cambiar a lo largo de un mes. Para obtener los precios diarios actuales de estos recursos de Azure, los asociados deben llamar a la API de RateCard. 

> [!Note] 
> Los cambios de precio de suscripción solo se aplican durante una renovación. Los cargos mensuales de un asociado se determinan con el precio de compra o el precio en el momento de la creación de una suscripción. Si un precio aumenta o disminuye después de adquirir el plazo anual, el asociado no se cobrará el precio modificado hasta la renovación, normalmente en el plazo de 12 meses.

## <a name="pricing-and-special-segments"></a>Precios y segmentos especiales

CSP ofrece algunos servicios a segmentos de mercado especiales, por ejemplo, educación, sin ánimo de lucro y en la nube de la comunidad gubernamental. No todos los servicios están disponibles en todos los canales. Ningún segmento tiene como valor predeterminado lo que llamamos segmento "comercial". Todos los precios basados en licencias están disponibles en la lista de precios basada en licencias en la página precios y ofertas. Azure Government precios está disponible en la lista de precios basada en el uso cuando se inicia sesión en el inquilino de CSP habilitado para Azure Government.

|**Segmento**   |**Quién debe calificar**   |**El asociado califica al cliente**|**Tipos de productos habilitados**|
|-------------------|-----------------------|----------------------------|-----------------------------|
|Educación|Customer|No, Microsoft llevará a cabo la calificación del cliente |Solo basado en licencia|
|Sin ánimo de lucro|Customer|No, el cliente se califica fuera del centro de Partners|Solo basado en licencia|
|Government Community Cloud (GCC)|Socio comercial y cliente|Una vez habilitado GCC, el asociado puede crear clientes GCC| Solo basado en licencia|
|Azure Government|Asociado|Una vez calificado, el asociado funciona en un inquilino de CSP específico para Azure Government|Recursos de Azure|

Los márgenes asociados, la diferencia entre el precio de venta y los precios de venta estimados, pueden variar de segmento a segmento. Normalmente, la educación y los no beneficios suelen tener márgenes inferiores o no para los asociados de CSP. Consulte la lista de precios basada en licencias para ver los valores exactos.  
## <a name="pricing-between-azure-and-non-azure"></a>Precios entre Azure y no Azure

Los precios difieren en diferentes tipos de ofertas. Los precios basados en licencias suelen ser la cantidad por puesto (licencia) de un mes determinado. Los precios basados en el uso se determinan mediante el uso de un recurso determinado, con un identificador de medidor asociado. Los asociados no se cobran por adquirir la suscripción de Azure. Sin embargo, se cobra a los asociados los recursos consumidos por diferentes implementaciones en la suscripción de Azure. Los precios de la lista de precios basada en el uso están organizados en torno a distintos identificadores de medidor de recursos en Azure.

Las reservas de Azure son compras basadas en términos para el tipo de recurso en particular Virtual Machines. La compra de una reserva de Azure permite que un asociado pague previamente (términos de uno o tres años) y Reserve una máquina virtual determinada. Las reservas guardan el dinero del socio comercial y garantizan que la máquina virtual esté siempre disponible mientras dure el período. Un asociado puede alinear la reserva que desee con los identificadores de medidor de recursos basados en el uso. Los identificadores de medidor son coherentes en todo el recurso, tanto si el asociado compra una máquina virtual como si simplemente implementa la máquina virtual como un recurso basado en el uso.

## <a name="offers-matrix"></a>Matriz de ofertas

En la página precios y ofertas, vea la matriz de la oferta del Reseller de la nube para obtener información acerca de las diferentes SKU y paquetes de productos disponibles para su venta. La matriz de ofertas incluye qué ofertas están disponibles por configuración regional. Si un elemento aparece en la lista de precios pero no en la matriz de la oferta, significa que aún no se pueden ordenar los productos. En cuanto estén disponibles para el pedido, se actualizará la matriz de ofertas.

Para los asociados de CSP que usan los kits de desarrollo de software (SDK) del centro de Partners. Microsoft también publica una lista de los servicios de Azure en CSP en la página de precios y ofertas.

### <a name="offers-matrix-and-price-list-questions"></a>Ofrece preguntas sobre matrices y listas de precios

Si tiene preguntas sobre la lista de precios o la matriz de ofertas, envíe una solicitud de servicio a través del centro de Partners.

## <a name="offer-limits"></a>Límites de la oferta

Algunas ofertas basadas en licencias tienen ciertas reglas y limitaciones que prohíben varias compras para el mismo cliente. Estas reglas se aplican a la mayoría de las ofertas de evaluación y a muchas de las pequeñas empresas. Las **ofertas de pequeñas empresas** están definidas por las ofertas que tienen un recuento máximo de licencias inferior a 300.

Estas restricciones de compra se definen como parte de la configuración de la oferta y se pueden encontrar mirando en la matriz de la lista de ofertas. Dos columnas de datos trabajan juntas para definir la aplicación: 1. Ámbito de límite de la oferta y 2. Límite de la oferta. Las restricciones se aplican durante una compra. El catálogo del centro de Partners impedirá que un socio adquiera más ofertas de las que permiten las reglas. Cualquier intento de infringir las restricciones producirá un error.

El ámbito del límite de la oferta se registra como una columna en la matriz de la lista de ofertas y puede tener valores de ninguno, duración o simultáneo. 

- Las ofertas con **ninguno** se pueden adquirir sin restricciones.
- Las ofertas de **duración** solo se pueden adquirir una vez.
- Las ofertas **simultáneas** se pueden comprar tantas veces como permita el valor de límite de la **oferta** para esa oferta. La mayoría de las pruebas tienen un ámbito de límite de ofertas de duración con un límite de oferta de "1". La mayoría de las ofertas de pequeñas empresas tienen un ámbito de límite de oferta simultáneo con un límite de oferta de "2".

> [!IMPORTANT]
> Los límites de simultaneidad se aplican incluso si se cancela una oferta. Una oferta debe cancelarse completamente y, a continuación, desaprovisionarse para liberar un espacio adicional que permita otra compra.

### <a name="taxes-and-pricing"></a>Impuestos y precios

Todos los precios de las listas de precios de CSP del centro de Partners son impuestos incluidos. Para obtener más información en el centro de Partners, documentar los [impuestos y las exenciones fiscales](tax-and-tax-exemptions.md).
