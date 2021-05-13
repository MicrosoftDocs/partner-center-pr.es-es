---
title: panel de información general de Centro de partners Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vea una instantánea de cómo está haciendo con las ventas y la implementación, el crecimiento de los clientes y el crecimiento de los ingresos con licencias, suscripciones y consumo de Azure.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e274b0a637c7fd4944a395ba7e38154e36d2a9e3
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855206"
---
# <a name="overview-dashboard-reports-available-in-partner-center-insights"></a>Revisar los informes del panel disponibles en la Información acerca del Centro de partners
 
**Roles adecuados:** Administrador global | Agente de administración | Visor de informes | Visor de informes ejecutivos

El panel Información general proporciona una vista de instantánea de los indicadores clave de rendimiento, como clientes, suscripciones, ingresos de consumo de Azure y licencias. Puede visualizar los gráficos siguientes en el informe De información general.

- Resumen  
- Propagación geográfica de sus clientes, suscripciones y licencias  
- Tendencia de crecimiento de los clientes 
- Tendencia de crecimiento de suscripciones 
- Tendencia de crecimiento de los ingresos consumidos por Azure 
- Tendencia de crecimiento de licencias 

## <a name="summary"></a>Resumen

El resumen incluye información sobre los clientes, Ingresos por consumo de Azure (ACR), las suscripciones vendidas, las suscripciones activas y las licencias implementadas. 

:::image type="content" source="images/pci/summary.png" alt-text="Resumen de licencias":::

A continuación se proporciona más información sobre cada sección del resumen.

### <a name="customers"></a>Clientes

El **área Clientes** incluye:

- El recuento actual de todos los clientes con al menos una suscripción activa asociada a su empresa a través de diferentes tipos de atribución y en todos los productos en la nube.
- Porcentaje de crecimiento de los clientes durante el intervalo de fechas seleccionado.
- El micro gráfico presenta la tendencia mensual del recuento de clientes dentro del intervalo de fechas seleccionado.

### <a name="azure-consumed-revenue-acr"></a>Ingresos por consumo de Azure (ACR)

El **área Ingresos por consumo de Azure (ACR)** del resumen incluye:

- El total Ingresos por consumo de Azure (en US $) que se le atribuyó en el intervalo de fechas seleccionado.
- Porcentaje de crecimiento o disminución de ACR con atributos (en US $) durante el intervalo de fechas seleccionado.
- El micro chart presenta una tendencia mensual de ACR US$ que se le atribuyó en el intervalo de fechas seleccionado. 

> [!NOTE]
> Ingresos por consumo de Azure (ACR) están disponibles para los usuarios a los que se ha asignado el rol visor de informes ejecutivos 
 
### <a name="subscriptions-sold"></a>Suscripciones vendidas

El **área Suscripciones vendidas** del resumen incluye:

- Recuento total actual de suscripciones de productos en la nube (activas e inactivas) vendidas o administradas por usted.  
- Porcentaje de crecimiento o disminución de suscripciones durante el intervalo de fechas seleccionado.
- El micro gráfico presenta la tendencia de mes a mes del total de suscripciones durante el intervalo de fechas seleccionado.

### <a name="active-subscriptions"></a>Suscripciones activas

El **área Suscripciones activas** del resumen incluye:

- Recuento actual de suscripciones de productos en la nube con uso activo medido en función de la telemetría del producto. Esto excluye todas las suscripciones de prueba en el caso de las suscripciones de Azure.  
- Porcentaje de crecimiento de suscripciones activas en el intervalo de fechas seleccionado.
- El micro gráfico presenta la tendencia de mes a mes de las suscripciones activas en el intervalo de fechas seleccionado.
 
### <a name="licenses-deployed"></a>Licencias implementadas

El **área Licencias implementadas** en el resumen incluye:
 
- Recuento de todas las licencias de productos en la nube implementadas en las suscripciones de los clientes durante el período de tiempo seleccionado. 
- Porcentaje de crecimiento o disminución de estas licencias durante el intervalo de fechas seleccionado. 
- El micro gráfico muestra la tendencia de mes a mes de estas licencias asignadas en el intervalo de fechas seleccionado.

## <a name="geographical-spread-of-your-customers-subscriptions-and-licenses"></a>Propagación geográfica de sus clientes, suscripciones y licencias

Esta vista es una distribución geográfica del total de clientes, suscripciones y licencias por país del cliente. Seleccione las distintas pestañas para ver cada una de estas conclusiones en el mapa. Puede buscar y seleccionar un país en la cuadrícula para ampliar la ubicación en el mapa. Vuelva a la vista original presionando el botón Inicio del mapa. Al hacer clic en cada pestaña (por ejemplo, Clientes, Suscripciones) se muestra el valor de la métrica de cada país y el porcentaje del total del país.  

:::image type="content" source="images/pci/geosummary.png" alt-text="Resumen geográfico":::

## <a name="customers-growth-trend"></a>Tendencia de crecimiento de los clientes

Tendencia mensual del número total de clientes para el intervalo de fechas seleccionado. El eje X representa los meses del intervalo de fechas seleccionado y el eje Y representa el recuento total de clientes para ese mes. 

:::image type="content" source="images/pci/customergrowth.png" alt-text="tendencia de crecimiento de los clientes":::

## <a name="subscriptions-growth-trend"></a>Tendencia de crecimiento de suscripciones

Esto indica la tendencia del recuento de suscripciones de cliente para el intervalo de fechas seleccionado. El eje X representa los meses del intervalo de fechas seleccionado y el eje Y representa el recuento de suscripciones del producto seleccionado. Desplácese por el control deslizante de la parte superior del gráfico para acercar el gráfico a un período de tiempo específico. 

:::image type="content" source="images/pci/subscriptiongrowth.png" alt-text="Tendencia de crecimiento de la suscripción":::

## <a name="azure-consumed-revenue-growth-trend"></a>Ingresos por consumo de Azure tendencia de crecimiento

Tendencia mensual de los ingresos consumidos por Azure en US$ que se le atribuyó en el intervalo de fechas seleccionado. El eje X representa los meses del intervalo de fechas seleccionado y el eje Y representa los ingresos totales consumidos por Azure en US$ que se le atribuyen durante el mes.

> [!NOTE]
> Ingresos por consumo de Azure (ACR) solo será visible para los usuarios a los que se haya asignado el rol visor de informes ejecutivos. 

:::image type="content" source="images/pci/azureconsumed.png" alt-text="Consumo de Azure":::

## <a name="licenses-growth-trend"></a>Tendencia de crecimiento de licencias
 
Tendencia de licencias asignadas por todos los clientes durante el intervalo de fechas seleccionado. El eje X representa los meses del intervalo de fechas seleccionado y el eje Y representa el recuento de licencias del producto que ha seleccionado. Desplácese por el control deslizante de la parte superior del gráfico para acercar el gráfico a un período de tiempo específico.  

:::image type="content" source="images/pci/licensesgrowth.png" alt-text="licencias":::

## <a name="next-steps"></a>Pasos siguientes

Para obtener más informes, [vea Centro de partners Insights](partner-center-insights.md).
