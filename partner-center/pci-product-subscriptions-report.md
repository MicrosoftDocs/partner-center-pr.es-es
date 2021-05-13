---
title: Centro de partners de suscripciones de Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vea lo que está haciendo bien y dónde puede mejorar con respecto a las suscripciones en la nube que vende o administra para sus clientes.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 89806b08485bc4bd286c2e14a19924ca0e281b6d
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854475"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Informe de suscripciones de productos disponible en el panel Centro de partners Insights

**Roles adecuados:** administrador global | Agente de administración | Visor de informes | Visor de informes ejecutivos

El informe Suscripciones de productos presenta análisis sobre las suscripciones en la nube que ha vendido o que administra para sus clientes. Se trata de un informe específico del producto que incluye el rendimiento de las suscripciones asociadas a productos en la nube como Office 365, Azure, Dynamics y otros.

Puede ver las secciones siguientes en el informe Suscripciones de productos.

- Resumen
- Propagación geográfica de suscripciones
- Tendencia de adición y renovación de suscripciones
- Distribución de suscripciones por ubicaciones de asociados, canal de ventas, SKU, tipo de asociación de asociados, segmento
- Tendencia por estados de suscripción
- Tendencia de los productos

 > [!NOTE]
 > Este informe está disponible en el panel de Insights. Para ver este informe, debe tener asignado un rol específico en Centro de partners, como Administrador global, Administrador de cuentas, Visor de informes o Visor de informes ejecutivos. Para obtener más información, vea El administrador global de su empresa. Los tipos específicos de datos de este informe también pueden estar disponibles solo para los usuarios con privilegios del Visor de informes ejecutivos.

## <a name="summary"></a>Resumen

En la sección de resumen se presenta una vista de instantánea de los indicadores clave de rendimiento (KPI) relacionados con las suscripciones vendidas o administradas por usted para sus clientes.  

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="Resumen del informe de suscripciones":::

Para obtener más información sobre cada sección del resumen, consulte a continuación:

- Suscripciones:
  - Recuento actual de las suscripciones de productos en la nube vendidas o administradas por usted.
  - Porcentaje de crecimiento o disminución de suscripciones durante el intervalo de fechas seleccionado.
  - El gráfico Micro presenta una tendencia mensual del recuento de suscripciones durante el intervalo de fechas seleccionado.

- Suscripciones activas:
  - Recuento actual de suscripciones de productos en la nube con uso activo medido en función de la telemetría del producto. Esto excluye todas las suscripciones de prueba en el caso de las suscripciones de Azure.
  - Porcentaje de crecimiento o disminución de suscripciones activas durante el período de tiempo seleccionado.
  - El gráfico Micro presenta una tendencia mensual de suscripciones activas durante el intervalo de fechas seleccionado.

- Suscripciones agregadas:
  - Total de suscripciones de cliente agregadas (vendidas o administradas) por el usuario durante el intervalo de fechas seleccionado. Las nuevas suscripciones **con estado Activo** o **Renovado** se cuentan como Suscripciones agregadas.
  - Porcentaje de crecimiento o disminución de suscripciones agregadas en el último mes completo en comparación con el primer mes completo.
  - El gráfico Micro presenta una tendencia mensual de las suscripciones agregadas durante el intervalo de fechas seleccionado.

- Suscripciones activas:
  - Total de suscripciones de cliente que se han renovación durante el intervalo de fechas seleccionado. Las suscripciones con **el estado Desaprovisionado** **o Suspendido** en ese mes se cuentan como una suscripción de renovación.  
  - Porcentaje de suscripciones que se han renovación durante el intervalo de fechas seleccionado.
  - El gráfico Micro presenta una tendencia mensual de suscripciones que se han renovación en el intervalo de fechas seleccionado.

- Suscripciones por productos: desglose del recuento actual de suscripciones por productos en la nube.

## <a name="geographical-spread-of-subscriptions"></a>Propagación geográfica de suscripciones

La **vista Suscripciones por geografía muestra** la distribución geográfica del total de suscripciones por mercados de clientes. El importe total de la suscripción incluye tanto las suscripciones vendidas como las suscripciones activas.

La **tabla Number of countries/region** (Número de países o regiones) presenta el total de países o regiones en los que tiene suscripciones y la cantidad por país de suscripciones totales y activas.

Puede buscar y seleccionar un país en la cuadrícula para ampliar la ubicación en el mapa. Presione la **opción** Inicio del mapa para volver a la vista original. Mantenga el puntero sobre el mapa para ver todas las suscripciones y suscripciones activas por país. Ambos campos de la cuadrícula se pueden ordenar.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="suscripciones por geografía":::

## <a name="subscription-addschurns"></a>Agregaciones o abandonos de suscripciones

Esta vista presenta una tendencia de suscripciones. Se desglosan en distintas categorías (Nuevo, Existente, Renovación) para el intervalo de fechas seleccionado. El eje X representa los meses del intervalo de fechas seleccionado. El eje Y representa el recuento de suscripciones. Las suscripciones de renovación se representan en la escala negativa del eje Y. 

El gráfico de columnas apiladas presenta un desglose de las suscripciones nuevas, existentes y renovación del mes. Puede volver a generar el gráfico de columnas, desglosado con elementos de pila específicos. Para ello, seleccione esos elementos específicos en la leyenda. También puede usar el control deslizante situado en la parte superior del gráfico para acercar un punto específico.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="agregaciones y abandonos de suscripciones":::

## <a name="subscription-distribution"></a>Distribución de suscripciones

Esta vista presenta un desglose de las suscripciones actuales según las ubicaciones de MPN, los segmentos de cliente, el canal de ventas o el modelo de precios de Azure y el tipo de atribución (por ejemplo, DPOR, DAP y otros). Seleccione las pestañas correspondientes para ver el desglose por estas categorías. Para compilar el gráfico circular con un desglose de categorías de elementos específicas, seleccione esas categorías de elementos en la leyenda.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="distribución de suscripciones":::

## <a name="subscription-state-distribution"></a>Distribución del estado de suscripción

Esta vista muestra la distribución de las suscripciones de cliente actuales por estado o estado de suscripción. Esto incluye los siguientes estados de suscripción: **Active**, **Disabled**, **Deprovisioned**, **Open**, **InGracePeriod**, **Closed** y **otros**.

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="distribución de estado de suscripción":::

## <a name="products-trend"></a>Tendencia de productos

Esta vista muestra un gráfico de barras y dos gráficos circulares. El gráfico de barras presenta una tendencia mensual de suscripciones desglosadas por productos comerciales, como Azure, Office, Dynamics, etc.

Los dos gráficos circulares muestran un desglose de las suscripciones de cliente actuales. El primer gráfico circular desglosa las suscripciones por productos. El segundo gráfico circular desglosa las suscripciones por SKU o planes. Al seleccionar un producto  en el desglose por gráfico circular Productos, el gráfico circular adyacente mostrará un desglose de las suscripciones de ese producto por SKU.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="tendencia de productos":::

> [!NOTE]
 > Es posible que el recuento de suscripciones desglosado por SKU no coincida siempre con el recuento total de suscripciones de ese producto. Esto puede ocurrir si un cliente ha adquirido varias SKU en la misma suscripción de producto.

## <a name="next-steps"></a>Pasos siguientes

- Para obtener más informes, [vea Centro de partners Insights](partner-center-insights.md).

>[!NOTE] 
> Puede descargar los datos sin procesar que encenderán este informe desde la sección Descargar informes del panel de Insights. [Más información](pci-download-reports.md) 
