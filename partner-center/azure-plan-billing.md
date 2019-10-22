---
title: 'Plan de Azure: facturación | Centro de partners'
ms.topic: article
ms.date: 10/04/2019
description: Aquí se describe la factura y la estructura del archivo de conciliación.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: 28e670635ca7fcff60041fcb5c93b3ddd5e4069d
ms.sourcegitcommit: cd90a59ff0ea81197b603abcb7bf462c4fb1edbe
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/09/2019
ms.locfileid: "72171300"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nueva experiencia comercial en CSP: facturación de Azure 

La facturación del plan Azure es una experiencia de facturación simplificada que usa una fecha de facturación única alineada y un período de facturación basado en los meses del calendario. Para obtener información sobre la plataforma de facturación, consulta la [guía de operaciones de comercio moderno del Centro de partners](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx).

## <a name="summary-of-billing-essentials"></a>Resumen de los elementos esenciales de la facturación

- **Fecha de facturación**: La factura y el archivo de conciliación estarán disponibles en el panel o API del Centro de partners antes del día 8 (medianoche, UTC).

- **Período de facturación**: El período de facturación de la factura coincidirá con el mes natural; por ejemplo, 10/1-10/31, 11/1-11/30.

- **Períodos del servicio de cargos**: Los cargos coincidirán con el mes natural. Por ejemplo, si el partner facturado agrega servicios de Azure a través de un plan de Azure el 15/10 y el cliente comienza a consumir los servicios de Azure el mismo 15/10, el partner facturado recibirá la factura o la conciliación el 8/11 referente al consumo del cliente durante el período de servicio del 15/10 al 31/10. La factura del próximo mes que se generará el 8/12 y contendrá todos los cargos del período de servicio del 01/11 al 11/31.

- **Plazo de pago de la factura**: Neto, 60 días.

- **Moneda de la factura** : Los partners seguirán siendo facturados en la moneda asignada del país del cliente. Por ejemplo, si el partner facturado está en Irlanda y tiene clientes en el Reino Unido, Noruega y Alemania, entonces el partner facturado recibirá una factura o conciliación en GBP, NOK y EUR.

- **Incentivos de partners**: Pagado a 45 días desde el final del mes de la factura.

##  <a name="access-your-invoices-and-recon-files"></a>Acceder a las facturas y archivos de conciliación

El administrador global o el administrador de facturación de tu empresa recibirá un correo electrónico cuando una factura esté lista para ver. 

**Para acceder a la factura y al archivo de reconocimiento:**

1. Inicia sesión en el Centro de partners.

2. En el menú del Centro de partners, selecciona **Billing** (Facturación).

3. Selecciona la pestaña **Calendar-based** (Basado en calendario) y la moneda que quieras.

![facturación](images/azure/billing1.png)

4. Selecciona **Invoice and Recon file** (Factura y archivo de conciliación).  

Para ver las facturas históricas y los archivos de conciliación, amplía la fila del historial de facturación a continuación.

## <a name="read-the-invoice"></a>Leer la factura

1. La factura estará disponible el día 8 de cada mes a más tardar.

2. Los partners tienen 60 días para remitir el pago.

3. El período de facturación cubrirá un mes dado del calendario; por ejemplo del 1/10 al 31/10.

4. Los cargos son netos en cuanto a los ajustes (el importe es el valor neto del "crédito obtenido del partner por los servicios administrados").

5. Revisa el archivo de conciliación de facturas y el archivo de uso con clasificación diaria para obtener los detalles adicionales de facturación.

![factura](images/azure/invoice1.png)

## <a name="read-the-recon-file"></a>Leer el archivo de conciliación

1. Cada medidor de suscripciones de Azure puede tener hasta dos líneas de facturación en el archivo de conciliación.

2. Si el medidor puede tener en cuenta cualquier tipo de descuento o crédito (como los descuentos de nivel 1 o el crédito obtenido del partner por los servicios administrados) durante todo el mes natural, el archivo de conciliación solo contendrá una línea de facturación. La columna **PriceAdjusmentDescription**  hará referencia al descuento o al crédito acumulado; el precio por unidad vigente será el precio comercial menos el crédito obtenido del partner o cualquier otro descuento.

3. Si el medidor no es apto para el crédito obtenido del partner por los servicios administrados durante todo el mes natural, el archivo de conciliación solo contendrá una línea de facturación y el precio por unidad vigente será el precio de venta al por menor (que es el precio por unidad).

4. Si el medidor calificado para el **crédito obtenido del partner por los servicios administrados** durante una parte del mes, el archivo de conciliación contendrá dos líneas de facturación. Una línea representará los días que el medidor haya calificado y la segunda línea representará los días que el medidor no calificó. 

## <a name="read-the-daily-usage-file"></a>Leer el archivo de uso diario

- Los medidores de suscripción en un plan de Azure se clasifican y se acumulan diariamente. 

- **El crédito obtenido del partner por los servicios administrados**  se determina y se aplica diariamente.

- Cada medidor de suscripciones tendrá una fila por cada día del mes en el que se haya consumido.

- Consulta el ejemplo que aparece a continuación:

  - El medidor es apto para el **crédito obtenido del partner por los servicios administrados** del 01/07 al 03/07 (ten en cuenta que el precio unitario efectivo es el precio del minorista menos el crédito obtenido del partner).

   - El medidor no es apto para el **crédito obtenido del partner por los servicios administrados** del 04/07 al 07/07 (ten en cuenta que el precio unitario efectivo es el precio del minorista).

    - El medidor es apto para el **crédito obtenido del partner por los servicios administrados** del 08/07 al 31/07 (ten en cuenta que el precio unitario efectivo es el precio del minorista).

![recon2](images/azure/billing2.png) 

## <a name="invoice-in-customer-currency"></a>Factura en la moneda del cliente 

Los servicios de Azure a través de un plan de Azure tendrán un precio de USD y se facturarán en la moneda asignada en el país del cliente. Si la moneda de facturación no es USD, el tipo de cambio usado se mostrará en la última página de la factura. Los tipos de cambio se determinan mensualmente y se aplican a la factura siguiente. Para obtener una lista completa de las monedas de los países, consulta la [matriz de moneda del cliente y la disponibilidad de los países en cuanto a las nuevas ofertas comerciales](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3Qn1V). 

Microsoft usará [Thomson Reuters](https://developers.thomsonreuters.com/content/wm-company) para determinar el tipo de cambio que se usará para convertir la moneda de los precios a la moneda de la factura. El tipo de cambio se actualizará y estará disponible el día anterior al primer día del mes para el que se aplica.

**Ejemplo**:  los cargos de uso para el período de servicio del 1 de agosto al 31 de agosto se facturarán mediante el tipo de cambio publicado el 1 de agosto. Estos cargos aparecerán en la factura de septiembre y el tipo de cambio se anotará en la última página de la misma. 

Los usuarios inquilinos del partner continuarán viendo información relacionada con roles específicos referentes a todos los clientes y todos los pedidos, independientemente de la moneda de facturación. Además, el usuario podrá ver todas las facturas en todas las monedas.  
 
## <a name="azure-reservations"></a>Reservas de Azure 

Si compras [reservas de Azure](https://docs.microsoft.com/partner-center/azure-reservations) a través de un plan de Azure, inicialmente, solo será posible elegir la facturación única en Centro de partners. La facturación mensual está disponible en Azure Portal. La facturación mensual estará disponible en el Centro de partners posteriormente. 

## <a name="azure-cost-management"></a>Azure Cost Management 

Las herramientas de Azure Cost Management ayudarán a las organizaciones a visualizar, administrar y optimizar los costos en Microsoft Azure. Esta característica estará disponible en Azure Portal. Los partners tendrán una solución siempre activa y de baja latencia con las siguientes características disponibles: 

- Análisis más detallado y alertas presupuestarias 
- API y conectores de Power BI 
- Vista de varios clientes 
- Gratis para administrar los costos de Azure 
- Expansión de roles y usuarios 

Consulta la [administración de costos de Azure](https://azure.microsoft.com/services/cost-management) para obtener más información sobre esta característica, que estuvo disponible en los Contratos Enterprise en febrero de 2019. Esta opción solo está disponible con los servicios de Azure que se compraron como parte de esta nueva experiencia comercial de Azure en CSP. 
 
## <a name="azure-spending"></a>Gastos de Azure 

La herramienta de gastos de Azure estará disponible en el Centro de partners en la nueva experiencia comercial de CSP. Cuando se aplique, esta funcionalidad permitirá a los partners ver lo siguiente:  

- El presupuesto total de un cliente 
- El total de gastos estimados en un plan de Azure existente 
- El porcentaje de uso de los clientes en cada período de facturación 

Dado que el modelo de facturación para los servicios de Azure a través de un plan de Azure es el consumo de pago posterior, para evitar recibir una factura más grande de lo previsto, los partners pueden aplicar un presupuesto mensual y realizar un seguimiento del porcentaje de uso. Se puede aplicar un presupuesto a un cliente o a varios clientes al mismo tiempo. 

![Gastos de Azure](images/azure/azurespend.png)

**Para obtener más información**

-  La forma en que se calcula el crédito obtenido del partner (PEC) se encuentra en la lista de precios disponible en el panel del Centro de partners. 
   
-  [Compra del plan de Azure](purchase-azure-plan.md)

-  [Lista de precios para la nueva experiencia comercial en CSP](azure-plan-price-list.md)
