---
title: Precios y ofertas
ms.topic: article
ms.date: 01/07/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Consulte las listas de precios actuales para servicios basados en licencias como Office 365, Microsoft Dynamics CRM y Enterprise Mobility Suite, y servicios basados en uso como Azure.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1cf69258b507258e1186514c54fa11ebf8a57d36
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854526"
---
# <a name="pricing-and-offers-for-office-365-dynamics-crm-enterprise-mobility-suite-azure-and-more"></a>Precios y ofertas para Office 365, Dynamics CRM, Enterprise Mobility Suite, Azure, etc.


**Roles adecuados:** Administrador global | Administrador de administración de | Agente de administración | Administrador de asociados de MPN | Agente de ventas | Administrador de facturación

Para ver las ofertas y programas de Proveedor de soluciones en la nube más recientes, en el panel del Portal de partners, vaya a **Vender > Precios y ofertas**. Encontrará listas de precios independientes para los distintos tipos de productos que están disponibles. Las siguientes listas de precios están disponibles en la página **Precios y ofertas**:

- **Los servicios basados en** licencias incluyen información de precios para Office 365, Enterprise Mobility y Security E3, así como y Dynamics 365. La sección precios basados en licencias incluye los precios actuales y en versión preliminar, así como la matriz de la lista de ofertas. Las listas de precios incluyen el precio de la lista y los precios de venta al por menor estimados (ERP) para las ofertas en todas las monedas admitidas. La matriz de lista de ofertas incluye disponibilidad del mercado y otra información importante sobre las ofertas. Estos archivos se actualizan el primer día de cada mes.
- **Los servicios basados en el** uso incluyen información de precios Microsoft Azure y Visual Studio. También puedes usar la [Calculadora de precios de servicios de Azure en el CSP](https://azure.microsoft.com/pricing/calculator/). La descarga basada en el uso incluye las listas de precios de CSP para todas las monedas admitidas, así como los archivos de precios de servicios compartidos en ERP. Estos archivos se actualizan el primer día de cada mes.
- **Microsoft Azure reserved instances incluye** información de precios para todas las monedas admitidas para Azure Reserved Instances. La descarga de precios también incluye los precios de Servicios compartidos en ERP. Estos archivos se actualizan el primer día de cada mes.
- **Las suscripciones de software** incluyen los precios de las suscripciones de software basadas en términos para todas las monedas admitidas. El archivo de precios incluye todas las monedas admitidas con list price y MSRP. Estos archivos se actualizan el primer día de cada mes.
- **Los precios del plan de Azure** incluyen información de precios para los servicios de consumo del plan de Azure, así como los precios de las reservas del plan de Azure. Los precios son precios directos o ERP y se pueden recuperar para cualquier mercado admitido determinado. Los datos de estos archivos se actualizan todos los días.
- **Las tasas de cambio** se usan para calcular la facturación cobrada entre USD y la moneda local de los asociados. Las tarifas se actualizan el primero de cada mes y se mantienen en true para el mes dado. Las tarifas están disponibles. Estos archivos se actualizan el primer día de cada mes.
- **Marketplace** incluye los precios de las soluciones de ISV del marketplace comercial de Microsoft. Los precios se recuperan por mercado. Los datos de estos archivos se actualizan todos los días.

> [!Note] 
> Solo los asociados de CSP con la capacidad de realizar transacciones pueden ver y descargar listas de precios. Los revendedores indirectos deben [ponerse en contacto con su proveedor de CSP]( https://partner.microsoft.com/cloud-solution-provider/find-a-provider) para solicitar detalles sobre los precios.

## <a name="price-list-preview-and-change-frequency"></a>Vista previa de la lista de precios y frecuencia de cambio 

Los servicios basados en licencias incluyen una vista previa de la lista de precios, que se proporciona con 30 días de antelación a los cambios. Para ver la versión preliminar de la lista de precios, vaya **a Sell > Pricing and offers (Precios y ofertas).** No hay ninguna versión preliminar de precios para los servicios basados en el uso, ya que estos servicios son dinámicos. En la tabla siguiente se explica cómo leer la tabla de lista de precios.

|**Elemento**        |**Definición**      |
|:-----------   |:-----------   |
|ADD   |Nuevo elemento en la lista de precios|
|Chg   |Cambios en el precio de la lista de mes a mes. Pueden producirse otros cambios no relacionados con el precio de la lista; los asociados deben comparar las listas de precios entre meses para determinar los cambios en otras propiedades.|
|DEL   |Un elemento quitado de la lista de precios|
|UNC   |Lista de precios sin cambios con respecto a la lista de precios del mes anterior  |
|Válido desde la fecha   |La primera fecha en que se puede pedir una oferta    |
|Válido hasta la fecha   |La última fecha en que se puede pedir una oferta   |
|Nombre para mostrar de la oferta   |Nombre orientado al cliente de la oferta   |
|Id. de oferta   |Identificador interno de la oferta   |
|Tipo de contrato de licencia   |Los tipos de contrato de licencia pueden ser corporativos, gubernamentales o académicos. El tipo de contrato determina a qué tipos de cliente se puede vender la oferta.|
|Unidad de compra   |La duración de la oferta que se compra. Las unidades de compra suelen ser de un mes.   |
|Tipo de licencia secundaria   |Los tipos de licencia secundarios serán no específicos, complementos o pruebas. El complemento indica que hay productos de requisitos previos que el cliente debe comprar antes de adquirir el complemento.|
|Tipo de cliente final   |Se relaciona con el tipo de contrato de licencia: licencia corporativa: revendedor en la nube corporativo, licencia gubernamental, administración pública de revendedores en la nube o licencia académica: profesores de revendedores en la nube o estudiantes de revendedores en la nube   |
|Precio de la lista   |El precio que pagará el asociado   |
|Precio de ERP   |El precio de venta al por menor estimado o recomendado para el cliente   |

## <a name="price-changes"></a>Cambios en los precios

Los cambios en los precios son una ocurrencia común. Los asociados pueden prever los cambios en los precios de las ofertas basadas en licencias mediante la vista previa de la lista de precios. En el panel Centro de partners, abra la página Precios y ofertas para ver la vista previa de la lista de precios.

Sin embargo, los precios basados en el uso de Azure no tienen ninguna versión preliminar. Los asociados pueden mantenerse al día con los cambios en los precios de consumo de Azure mediante la API RateCard, que devuelve los precios de los medidores de ese día.

|**Tipo de producto**   |**Ejemplos de productos**  |**Versión preliminar disponible** |**Cambiar detalles**|
|-----------------------|:-----------------------|:-------------------|------------------|
|Basado en licencias|Office, Dynamics, Intune, Windows Enterprise|30 días|Enumeración de los cambios de precios marcados como CHNG en las listas de precios de versión preliminar|
|Basado en uso|Recursos de Azure|No disponible|Registro de cambios disponible en la pestaña Historial de cambios de la lista de precios **del mes** anterior|
|Software||No disponible|Comparación manual de listas de precios de mes a mes|
|Reservations|Máquinas virtuales, de pago previo|No disponible|Comparación manual de listas de precios de mes a mes|

Los precios basados en el uso pueden cambiar a lo largo de un mes. Para obtener los precios diarios "actuales" de estos recursos de Azure, los asociados deben llamar a la API RateCard. 

> [!Note] 
> Los cambios en el precio de la suscripción solo se aplican durante una renovación. El cargo mensual de un partner se determina según el precio de compra o el precio en el momento de crear una suscripción. Si un precio aumenta o disminuye después de adquirir el período anual, no se cobra al asociado el precio cambiado hasta la renovación, normalmente en el período de 12 meses.

## <a name="pricing-and-special-segments"></a>Precios y segmentos especiales

CSP ofrece algunos servicios a segmentos de mercado especiales, como la nube de la comunidad educativa, sin ánimo de lucro y gubernamental. No todos los servicios están disponibles en todos los canales. Ningún segmento tiene como valor predeterminado lo que llamamos segmento "comercial". Todos los precios basados en licencias están disponibles en la lista de precios basados en licencias de la página Precios y ofertas. Azure Government precios están disponibles en la lista de precios basados en uso cuando se ha iniciado sesión en el Azure Government CSP habilitado. Las suscripciones de software y el software perpetuo aún no admiten estos segmentos especiales.

|**Segmento**   |**que necesita calificar**   |**El partner califica al cliente**|**Tipos de productos habilitados**|
|-------------------|-----------------------|----------------------------|-----------------------------|
|Education|Customer|No, Microsoft realizará la calificación del cliente. |Solo basado en licencias|
|Sin ánimo de lucro|Customer|No, el cliente cumple los requisitos fuera de Centro de partners|Solo basado en licencias|
|Government Community Cloud (GCC)|Asociado y cliente|Una vez habilitado GCC, el asociado puede crear clientes de GCC.| Solo basado en licencias|
|Azure Government|Asociado|Una vez calificado, el asociado opera en un inquilino de CSP específico de Azure Government|Recursos de Azure|

Los márgenes de los asociados, la diferencia entre el precio de la lista y los precios de venta al por menor estimados, pueden variar de un segmento a otro. Normalmente, la educación y las organizaciones sin ánimo de lucro tienden a tener márgenes inferiores o ninguno para los asociados de CSP. Consulte la lista de precios basados en licencias para obtener los valores exactos. 

## <a name="add-on-offer-types"></a>Tipos de ofertas de complementos

Los servicios basados en licencias se pueden adquirir como ofertas base o complementos. Solo las ofertas base son reconocibles y comprables a través del catálogo Centro de partners base. Debe aplicar complementos después de comprar las ofertas base. La columna Tipo de licencia **secundaria** de la lista de precios basada en licencias incluye información sobre cada oferta y su tipo. Las ofertas base **tienen valores no específicos** en la columna de tipo de licencia secundaria de la lista de precios y se pueden adquirir en el catálogo. Los valores de tipo de **licencia secundaria del complemento** no se pueden adquirir en el catálogo. Para comprar estos complementos:

1. Consulte la matriz de lista de ofertas para ver la lista de los identidades de oferta que deben adquirirse antes de poder comprar un complemento.
2. Compra de la oferta base del catálogo
3. Vaya a su cliente desde la lista de clientes. Haga clic en la suscripción de la oferta base que acaba de comprar. En la página Administrar suscripción, verá complementos disponibles que se pueden aplicar a la oferta base.

> [!Note] 
> Algunas ofertas base tienen **valores de tipo** unidad de licencias de **complemento.** Para una oferta base, esto simplemente significa que no se asignan licencias de usuario después de la compra. Si la oferta se puede comprar en el catálogo, es una **oferta base** independientemente del tipo de unidad en la interfaz de usuario.

## <a name="pricing-between-azure-and-non-azure"></a>Precios entre Azure y no Azure

Los precios difieren en los distintos tipos de ofertas. Los precios basados en licencias suelen ser la cantidad por licencia de un mes determinado. Los precios basados en el uso se determinan mediante el uso de un recurso determinado, con un identificador de medidor asociado. No se cobra a los asociados por adquirir la suscripción de Azure. Sin embargo, a los asociados se les cobra por los recursos consumidos por las distintas implementaciones de la suscripción de Azure. Los precios de la lista de precios basados en el uso se organizan en torno a diferentes identificadores de medidor de recursos en Azure.

Las reservas de Azure son compras basadas en términos para el tipo de recurso determinado: Virtual Machines. La compra de una reserva de Azure permite a un asociado pagar por adelantado (términos de uno o tres años) y reservar una máquina virtual determinada. Las reservas ahorran dinero al asociado y garantizan que su máquina virtual siempre esté disponible durante el período. Un asociado puede alinear la reserva que desea con los identificadores de medidor de recursos basados en el uso. Los identificadores de medidor son coherentes en todo el recurso, ya sea que el asociado compre una máquina virtual o simplemente implemente la máquina virtual como un recurso basado en el uso.

## <a name="offers-matrix"></a>Matriz de ofertas

En la página Precios y ofertas, consulte la Matriz de ofertas de revendedores en la nube para obtener información sobre las diferentes SKU y paquetes de productos disponibles para vender. La matriz de ofertas incluye qué ofertas están disponibles por configuración regional. Si un elemento aparece en la lista de precios, pero no en la matriz de ofertas, significa que los productos no se pueden ordenar todavía. En cuanto están disponibles para su pedido, se actualiza la matriz de ofertas.

Para los asociados de CSP que usan Centro de partners Software Development Kits (SDK). Microsoft también publica una lista de los servicios de Azure en CSP en la página Precios y ofertas.

### <a name="offers-matrix-and-price-list-questions"></a>Preguntas sobre la matriz de ofertas y la lista de precios

Si tiene alguna pregunta sobre la lista de precios u matriz de ofertas, envíe una solicitud de servicio a través del Centro de partners.

## <a name="offer-limits"></a>Límites de la oferta

Algunas ofertas basadas en licencias tienen ciertas reglas y limitaciones que prohíben varias compras para el mismo cliente. Estas reglas se aplican a la mayoría de las pruebas y a muchas de las ofertas de pequeñas empresas. **Las ofertas de pequeñas** empresas se definen mediante aquellas que tienen un número máximo de licencias inferior a 300.

Estas restricciones de compra se definen como parte de la configuración de la oferta y se pueden encontrar buscando en la matriz de la lista de ofertas. Dos columnas de datos funcionan juntas para definir el cumplimiento: 1. Ámbito de límite de la oferta y 2. Límite de la oferta. Las restricciones se aplican durante una compra. El catálogo del Centro de partners no permitirá que un partner compre más ofertas de las que permiten las reglas. Cualquier intento de infringir las restricciones producirá un error.

El ámbito del límite de la oferta se registra como una columna en la matriz de la lista de ofertas y puede tener valores de None, Lifetime o Concurrent. 

- Las ofertas **con None** se pueden comprar sin restricciones.
- **Las ofertas** de duración solo se pueden comprar una vez.
- **Las** ofertas simultáneas se pueden comprar tantas veces como lo permita el valor **límite** de la oferta para esa oferta. La mayoría de las pruebas tienen un ámbito de límite de oferta de duración con un límite de oferta de "1". La mayoría de las ofertas empresariales pequeñas tienen un ámbito de límite de oferta simultáneo con un límite de oferta de "2".

> [!IMPORTANT]
> Los límites de simultaneidad se aplican incluso si se cancela una oferta. Una oferta debe cancelarse completamente y desaprovisionarse para liberar un espacio adicional que permita otra compra.

### <a name="taxes-and-pricing"></a>Impuestos y precios

Todos los precios de las listas de precios de CSP del Centro de partners están incluidos en los impuestos. Para obtener más información en el documento Centro de partners [impuestos y exenciones fiscales](tax-and-tax-exemptions.md).

## <a name="multi-year-term-offers"></a>Ofertas a largo plazo de varios años

### <a name="36-month-offers"></a>Ofertas de 36 meses

Hay aproximadamente 50 ofertas de Dynamics que tienen términos de tres años. Estos se identifican mediante **(36 mes)** en el título de las ofertas. Estas ofertas son similares a las ofertas anuales. La única diferencia está en torno a su término. Estas ofertas tienen un período de tres años para que las suscripciones se renueve automáticamente después de tres años en lugar de uno. A continuación se muestra un resumen de cómo funcionan estas ofertas:

- Los términos son de 36 meses y las suscripciones se renovarán automáticamente después de tres años.
- Los asociados pueden cancelar o cambiar el número de licencias a lo largo del período de la suscripción.
- La renovación anual estará al precio del tiempo de compra para el período de tres años.
- La frecuencia de facturación sigue siendo anual o mensual

### <a name="72-month-offers"></a>Ofertas de 72 meses

Microsoft 365 oferta base A1 tiene un período de seis años.  Los complementos de Office 365 A1 están disponibles después de adquirir esta oferta base. 

|**Nombre de la oferta**   |**Identificador de oferta**   |**Tipo**|
|-------------------|-----------------------|----------------------------|
|Microsoft 365 A1|778a4dce-0014-4d53-8647-314ef2b091d2|Oferta base|
|Office 365 A1 para profesores (para dispositivo)|0757d14e-7c57-456f-8dab-47d164f2ff1f|Complemento|
|Office 365 A1 para estudiantes (para dispositivo)|bae285a9-d56b-4384-b02f-38adc61a6f12|Complemento|

A continuación se muestra un resumen de cómo funcionan estas ofertas:

- El plazo es de 72 meses o seis años.
- La suscripción no se renueva y expira después de seis años
- La frecuencia de facturación de la oferta se muestra como anual, pero el asociado se factura por adelantado en su primera factura después de adquirir la suscripción.
- Las suscripciones de las ofertas A1 de 72 meses están bloqueadas después de la compra y no se pueden cancelar y los recuentos de licencias no se pueden agregar a la suscripción después de la compra inicial.
- Esta suscripción no se puede cancelar y no se puede reembolsar.

## <a name="estimated-retail-price-erp"></a>Precio de venta al por menor estimado (ERP)

La mayoría de las listas de precios incluyen un precio de lista, el precio que se factura al asociado y el precio de venta al por menor estimado. El precio de venta al por menor estimado (ERP) también se denomina precio de venta al por menor sugerido por Microsoft o MSRP. Estos dos valores, ERP y MSRP, representan el valor de mercado estimado de los productos si un cliente comprara los productos directamente a Microsoft. A continuación se muestran los detalles de ERP/MSRP para cada tipo de producto o servicio. 


|**Producto o servicio**        |**Detalles de la lista de precios de ERP y MSRP**      |
|:-----------   |:-----------   |
|Producto o servicio  |Detalles de la lista de precios de ERP y MSRP  |
|Servicios basados en licencias  |Aparece como ERP en las listas de precios basadas en licencias  |
|Servicios basados en el uso de Azure  |Se puede encontrar en las listas de precios equivalentes de servicios compartidos.  |
|Reservas de Azure  |Se puede encontrar en las listas de precios equivalentes de servicios compartidos.  |
|Basado en el uso del plan de Azure  |Los precios son minoristas sin descuento en las hojas de precios  |
|Reservas de planes de Azure  |Referencia de las listas de precios de servicios compartidos de reservas de Azure  |
|Suscripciones de software  |Aparece como MSRP en las listas de precios de suscripciones de software  |
|Marketplace  |Aparece como MSRP en las listas de precios de Marketplace  |

Más recursos: 

- [Precios del plan de Azure](azure-plan-price-list.md)
- [Introducción a los precios de Azure](https://azure.microsoft.com/pricing/)
