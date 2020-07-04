---
title: Precios y ofertas
ms.topic: article
ms.date: 06/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Consulte las listas de precios actuales para servicios basados en licencias como Office 365, Microsoft Dynamics CRM y Enterprise Mobility Suite, y servicios basados en uso como Azure.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 066b69cc0a70ded518c6bbaa9f35879e4b992a89
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949339"
---
# <a name="pricing-and-offers-for-office-365-dynamics-crm-enterprise-mobility-suite-azure-and-more"></a>Precios y ofertas para Office 365, Dynamics CRM, Enterprise Mobility Suite, Azure, etc.

**Se aplica a**

- Centro de partners

**Roles adecuados**

- Administrador global
- Administrador de usuarios
- Agente de administrador
- Administrador de partners de MPN
- Agente de ventas
- Administrador de facturación

Para ver los programas y ofertas más recientes del proveedor de soluciones en la nube, desde el portal de Partners, vaya a **vender > precios y ofertas**. Encontrará listas de precios independientes para los diferentes tipos de productos que están disponibles. Las siguientes listas de precios están disponibles en la página **precios y ofertas** :

- Los **servicios basados en licencias** incluyen información de precios para Office 365, Enterprise Mobility y Security E3, así como y Dynamics 365. La sección de precios basada en licencia incluye los precios actuales y de vista previa, así como la matriz de la lista de ofertas. Las listas de precios incluyen precio de venta y precios de venta (ERP) estimados para ofertas en todas las monedas admitidas. La matriz de la lista de ofertas incluye la disponibilidad del mercado y otra información importante acerca de las ofertas. Estos archivos se actualizan el primer día de cada mes.
- Los **servicios basados en el uso** incluyen información de precios para Microsoft Azure y Visual Studio. También puedes usar la [Calculadora de precios de servicios de Azure en el CSP](https://azure.microsoft.com/pricing/calculator/). La descarga basada en el uso incluye las listas de precios de CSP para todas las divisas admitidas, así como los archivos de precios de servicios compartidos en ERP. Estos archivos se actualizan el primer día de cada mes.
- **Microsoft Azure instancias reservadas** incluye información de precios para todas las monedas admitidas para las instancias reservadas de Azure. La descarga de precios también incluye los precios de los servicios compartidos en ERP. Estos archivos se actualizan el primer día de cada mes.
- Las **suscripciones de software** incluyen los precios de las suscripciones de software basadas en términos para todas las monedas admitidas. El archivo de precios incluye todas las divisas admitidas con el precio de venta y MSRP. Estos archivos se actualizan el primer día de cada mes.
- Los **precios del plan de Azure** incluyen información sobre los precios de los servicios de consumo del plan de Azure, así como los precios de reserva del plan de Azure. Los precios son precios directos o ERP y se pueden recuperar en cualquier mercado compatible determinado. Los datos de estos archivos se actualizan todos los días.
- Las **tasas de cambio** en el extranjero se utilizan para calcular la facturación que se cobra entre USD y la moneda local de los asociados. Las tarifas se actualizan el primero de cada mes y tienen el valor true para el mes dado, las tarifas están disponibles. Estos archivos se actualizan el primer día de cada mes.
- **Marketplace** incluye los precios de las soluciones de ISV del Marketplace comercial de Microsoft. Los precios se recuperan por mercado. Los datos de estos archivos se actualizan todos los días.

> [!Note] 
> Solo los asociados de CSP con la capacidad de Transact pueden ver y descargar listas de precios. Los revendedores indirectos deben [ponerse en contacto con su proveedor de CSP]( https://partner.microsoft.com/en-us/cloud-solution-provider/find-a-provider) para solicitar detalles sobre los precios

## <a name="price-list-preview-and-change-frequency"></a>Vista previa de la lista de precios y frecuencia de cambio 

Los servicios basados en licencias incluyen una vista previa de la lista de precios, siempre con 30 días antes de que se realicen cambios. Para ver la vista previa de la lista de precios, vaya a **vender > precios y ofertas**. No hay ninguna vista previa de precios para los servicios basados en el uso, ya que estos servicios son dinámicos. En la tabla siguiente se explica cómo leer la tabla de lista de precios.

|**Item**        |**Definición**      |
|:-----------   |:-----------   |
|ADD   |Un nuevo elemento a la lista de precios|
|PREC   |Cambia el precio de venta de mes a mes. Pueden producirse otros cambios no relacionados con el precio de la lista, los asociados deben comparar las listas de precios entre meses para determinar los cambios en otras propiedades.|
|DEL   |Un elemento quitado de la lista de precios|
|UNC   |Precio de lista sin cambios en la lista de precios del mes anterior  |
|Válido desde fecha   |La primera fecha en que se puede ordenar una oferta    |
|Válido hasta la fecha   |La última fecha en que se puede ordenar una oferta   |
|Nombre para mostrar de la oferta   |El nombre del cliente para la oferta   |
|Identificador de oferta   |Identificador interno de la oferta.   |
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
|Education|Customer|No, Microsoft llevará a cabo la calificación del cliente |Solo basado en licencia|
|Sin ánimo de lucro|Customer|No, el cliente se califica fuera del centro de Partners|Solo basado en licencia|
|Government Community Cloud (GCC)|Socio comercial y cliente|Una vez habilitado GCC, el asociado puede crear clientes GCC| Solo basado en licencia|
|Azure Government|Asociado|Una vez calificado, el asociado funciona en un inquilino de CSP específico para Azure Government|Recursos de Azure|

Los márgenes asociados, la diferencia entre el precio de venta y los precios de venta estimados, pueden variar de segmento a segmento. Normalmente, la educación y los no beneficios suelen tener márgenes inferiores o no para los asociados de CSP. Consulte la lista de precios basada en licencias para ver los valores exactos. 

## <a name="add-on-offer-types"></a>Tipos de oferta de complementos

Los servicios basados en licencias se pueden adquirir como ofertas o complementos base. Solo las ofertas base son reconocibles y compra a través del catálogo del centro de Partners. Los complementos deben aplicarse después de comprar las ofertas base. La columna **tipo de licencia secundario** de lista de precios basada en licencias incluye información sobre cada oferta y su tipo. Las ofertas base tienen valores **no específicos** en la columna de tipo de licencia secundario de lista de precios y se pueden adquirir en el catálogo. Los valores del tipo de licencia secundario del **complemento** no se pueden comprar en el catálogo. Para comprar estos complementos:

1. Consulte la matriz de la lista de ofertas para ver la lista de identificadores de oferta que deben adquirirse para poder comprar un complemento.
2. Compra de la oferta base desde el catálogo
3. Vaya a su cliente en la lista de clientes. Haga clic en la suscripción de la oferta base que acaba de comprar. En la página Administrar suscripción verá los complementos disponibles que se pueden aplicar a la oferta base.

> [!Note] 
> Algunas ofertas base tienen valores de **tipo de unidad** de **licencias de complementos**. Para una oferta de base, esto simplemente significa que no se asignan licencias de usuario después de la compra. Si la oferta se puede comprar en el catálogo, es una **oferta base** , independientemente del tipo de unidad en la interfaz de usuario.

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

## <a name="multi-year-term-offers"></a>Ofertas de varios años

### <a name="36-month-offers"></a>Ofertas de 36 meses

Hay aproximadamente 50 ofertas de Dynamics que tienen términos de tres años. Se identifican mediante **(36 Mo)** en el título de las ofertas. Estas ofertas son muy similares a las ofertas anuales. La única diferencia se encuentra en torno a su término. Estas ofertas tienen un período de tres años, lo que significa que las suscripciones se renovarán automáticamente después de tres años en lugar de una. A continuación se muestra un resumen de cómo funcionan estas ofertas:

- Los términos son de 36 meses, las suscripciones se renovarán automáticamente después de tres años
- Los asociados pueden cancelar o cambiar el número de licencias a lo largo del período de la suscripción
- La renovación anual será al precio del tiempo de compra durante el período de tres años.
- La frecuencia de facturación sigue siendo anual o mensual

### <a name="72-month-offers"></a>Ofertas de 72 meses

Microsoft 365 oferta de base a1 tiene un plazo de seis años.  Los complementos de Office 365 a1 están disponibles después de adquirir esta oferta de base. 

|**Nombre de la oferta**   |**Identificador de oferta**   |**Type**|
|-------------------|-----------------------|----------------------------|
|Microsoft 365 A1|778a4dce-0014-4d53-8647-314ef2b091d2|Oferta base|
|Office 365 a1 para profesores (para dispositivos)|0757d14e-7c57-456f-8dab-47d164f2ff1f|Complemento|
|Office 365 a1 para estudiantes (para dispositivos)|bae285a9-d56b-4384-b02f-38adc61a6f12|Complemento|

A continuación se muestra un resumen de cómo funcionan estas ofertas:

- El término es de 72 meses o 6 años
- La suscripción no se renueva y expira después de 6 años
- La frecuencia de facturación de la oferta se muestra como anual, pero el socio comercial se factura por la primera factura después de adquirir la suscripción.
- Las suscripciones de las ofertas de a1 72 meses se bloquean después de la compra y no se pueden cancelar y no se pueden agregar recuentos de licencias a la suscripción después de la compra inicial.
- Los asociados que necesiten cancelar deben crear una incidencia de soporte técnico con el motivo de la cancelación y el identificador de suscripción que necesitan ayuda con.

## <a name="estimated-retail-price-erp"></a>Precio comercial Estimado (ERP)

La mayoría de las listas de precios incluyen un precio de venta, el precio al que se factura el socio comercial y el precio de venta estimado. El precio de venta al por menor Estimado (ERP) también se denomina precio comercial sugerido de Microsoft o MSRP. Estos dos valores, ERP y MSRP, representan el valor de mercado estimado de los productos si un cliente ha adquirido los productos directamente de Microsoft. A continuación se muestran los detalles de ERP y MSRP para cada tipo de producto o servicio. 


|**Producto o servicio**        |**Detalles de la lista de precios de ERP y MSRP**      |
|:-----------   |:-----------   |
|Producto o servicio  |Detalles de la lista de precios de ERP y MSRP  |
|Servicios basados en licencias  |Aparece como ERP en las listas de precios basadas en licencias  |
|Servicios basados en el uso de Azure  |Se puede encontrar en las listas de precios equivalentes de servicios compartidos  |
|Reservas de Azure  |Se puede encontrar en las listas de precios equivalentes de servicios compartidos  |
|Basado en el uso del plan de Azure  |Los precios son comerciales sin descuento en hojas de precios  |
|Reservas del plan de Azure  |Referencia a las listas de precios de servicios compartidos de reservas de Azure  |
|Suscripciones de software  |Aparece como MSRP en las listas de precios de las suscripciones de software  |
|Marketplace  |Aparece como MSRP en las listas de precios de Marketplace  |

Más recursos: 

- [Precios de Azure plan](azure-plan-price-list.md)
- [Información general sobre precios de Azure](https://azure.microsoft.com/pricing/)
