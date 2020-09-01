---
title: Panel de información general de Partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vea una instantánea de cómo realiza las ventas e implementación, el crecimiento de los clientes y el crecimiento de los ingresos con licencias, suscripciones y consumo de Azure.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 91075e8aab1759904a1549dd38bee6fb886c1c65
ms.sourcegitcommit: 5f31146f50e01dc4c1922e0a5bc369f0a3cd8162
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/01/2020
ms.locfileid: "89220493"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>Información general sobre los informes del panel disponibles en la información del centro de Partners
 
El panel Información general de Insights proporciona una vista de instantánea de los indicadores clave de rendimiento, como clientes, suscripciones, ingresos de consumo de Azure, licencias, etc. Puede visualizar los siguientes gráficos en el informe de información general.

- Resumen  
- Distribución geográfica de sus clientes, suscripciones y licencias  
- Tendencia de crecimiento de los clientes 
- Tendencia de crecimiento de suscripciones 
- Tendencia de crecimiento de ingresos consumido de Azure 
- Tendencia de crecimiento de licencias 

## <a name="summary"></a>Resumen

El resumen incluye información sobre los clientes, ingresos consumidos de Azure (ACR), suscripciones vendidas, suscripciones activas y licencias implementadas. 

:::image type="content" source="images/pci/summary.png" alt-text="Resumen de licencias":::

Consulte a continuación para obtener más información acerca de cada sección del Resumen.

### <a name="customers"></a>Clientes

El área **clientes** incluye:

- El recuento actual de todos los clientes con al menos una suscripción activa asociada a su empresa a través de diferentes tipos de atribución y en todos los productos en la nube.
- El porcentaje de crecimiento de los clientes durante el intervalo de fechas seleccionado.
- El micro gráfico presenta la tendencia de mes a mes del recuento de clientes en el intervalo de fechas seleccionado.

### <a name="azure-consumed-revenue-acr"></a>Ingresos consumidos por Azure (ACR)

El área **ingresos consumidos de Azure (ACR)** del resumen incluye:

- El total de ingresos consumidos de Azure (en EE. UU. $) le atribuye el intervalo de fechas seleccionado.
- Porcentaje de crecimiento o disminución del ACR con atributos (en US $) durante el intervalo de fechas seleccionado.
- El micro gráfico presenta una tendencia mensual del ACR que nos atribuye al usuario sobre el intervalo de fechas seleccionado. 

> [!NOTE]
> Los datos de ingresos consumidos de Azure (ACR) están disponibles para los usuarios a los que se ha asignado el rol ejecutivo de visor de informes. 
 
### <a name="subscriptions-sold"></a>Suscripciones vendidas

El área **suscripciones vendidas** en el resumen incluye:

- El número total actual de suscripciones de productos en la nube (activas e inactivas) que le vendió o administra.  
- El crecimiento porcentual o el rechazo en las suscripciones durante el intervalo de fechas seleccionado.
- El micro gráfico presenta la tendencia de mes a mes de las suscripciones totales sobre el intervalo de fechas seleccionado.

### <a name="active-subscriptions"></a>Suscripciones activas

El área **suscripciones activas** del resumen incluye:

- El recuento actual de suscripciones de productos en la nube con uso activo medido en función de la telemetría del producto. Esto excluye todas las suscripciones de prueba en el caso de las suscripciones de Azure.  
- El porcentaje de crecimiento de las suscripciones activas en el intervalo de fechas seleccionado.
- El micro gráfico presenta la tendencia de mes a mes de las suscripciones activas en el intervalo de fechas seleccionado.
 
### <a name="licenses-deployed"></a>Licencias implementadas

El área de **licencias implementadas** en el resumen incluye:
 
- El recuento de todas las licencias de productos en la nube implementadas en las suscripciones de clientes durante el período de tiempo seleccionado. 
- El crecimiento porcentual o el rechazo en estas licencias durante el intervalo de fechas seleccionado. 
- El micro gráfico muestra la tendencia de mes a mes de estas licencias asignadas en el intervalo de fechas seleccionado.

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>Distribución geográfica de sus clientes, suscripciones y licencias

Esta vista es una distribución geográfica del total de clientes, suscripciones y licencias por país del cliente. Haga clic en las distintas pestañas para ver cada una de estas perspectivas en el mapa. Puede buscar y seleccionar un país en la cuadrícula para ampliar la ubicación en el mapa. Vuelva a la vista original presionando el botón Inicio en el mapa. Al hacer clic en cada pestaña (por ejemplo, clientes, suscripciones), se muestra el valor de la métrica para cada país, así como el% del total del país.  

:::image type="content" source="images/pci/geosummary.png" alt-text="Resumen geográfico":::

## <a name="customers-growth-trend"></a>Tendencia de crecimiento de los clientes

Tendencia mensual de recuentos totales de clientes para el intervalo de fechas seleccionado. El eje X representa los meses del intervalo de fechas seleccionado y el eje Y representa el recuento total de clientes para ese mes. 

:::image type="content" source="images/pci/customergrowth.png" alt-text="tendencia de crecimiento de los clientes":::

## <a name="subscriptions-growth-trend"></a>Tendencia de crecimiento de suscripciones

Esto indica la tendencia del recuento de suscripciones de clientes para el intervalo de fechas seleccionado. El eje X representa los meses del intervalo de fechas seleccionado y el eje Y representa el recuento de suscripciones del producto seleccionado. Desplácese por el control deslizante situado en la parte superior del gráfico para acercar el gráfico hasta un período de tiempo específico. 

:::image type="content" source="images/pci/subscriptiongrowth.png" alt-text="Tendencia de crecimiento de suscripciones":::

## <a name="azure-consumed-revenue-growth-trend"></a>Tendencia de crecimiento de ingresos consumido de Azure

Tendencia mensual de los ingresos consumidos por Azure $ con el atributo en el intervalo de fechas seleccionado. El eje X representa los meses del intervalo de fechas seleccionado y el eje Y representa el total de ingresos consumidos de Azure $ atribuidos a usted durante el mes.

> [!NOTE]
> Los ingresos consumidos por Azure (ACR) solo estarán visibles para los usuarios a los que se haya asignado el rol Executive Report Viewer. 

:::image type="content" source="images/pci/azureconsumed.png" alt-text="Consumo de Azure":::

## <a name="licenses-growth-trend"></a>Tendencia de crecimiento de licencias
 
Tendencia de las licencias asignadas por todos los clientes durante el intervalo de fechas seleccionado. El eje X representa los meses del intervalo de fechas seleccionado y el eje Y representa el recuento de licencias del producto que ha seleccionado. Desplácese por el control deslizante situado en la parte superior del gráfico para acercar el gráfico hasta un período de tiempo específico.  

:::image type="content" source="images/pci/licensesgrowth.png" alt-text="licencias":::

## <a name="next-steps"></a>Pasos siguientes

Para obtener más informes, consulte [información del centro de Partners](partner-center-insights.md).
