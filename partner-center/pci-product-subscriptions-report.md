---
title: Informe de suscripciones de Partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vea lo que está haciendo bien y dónde puede mejorar en relación con las suscripciones en la nube que vende o administra para sus clientes.
author: shthota77
ms.author: shthota
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0f1f2498f9c91f467b4b2b1980a14995782a5137
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436674"
---
# <a name="product-subscriptions-report-available-from-the-partner-center-insights-dashboard"></a>Informe de suscripciones de productos disponible en el panel de Partner Center Insights

**Roles adecuados**
- Administrador global
- Agente de administrador
- Visor de informes
- Visor de informes ejecutivos

El informe de suscripciones de producto presenta análisis sobre las suscripciones en la nube que ha vendido o que administra para sus clientes. Se trata de un informe específico del producto que incluye el rendimiento de las suscripciones asociadas a productos en la nube como Office 365, Azure, Dynamics, etc.

Puede ver las secciones siguientes del informe de suscripciones de productos.

- Resumen
- Propagación geográfica de suscripciones
- Tendencia de adición/renovación de suscripciones
- Distribución de suscripciones por ubicaciones de asociados, canales de ventas, SKU, tipo de Asociación de socios, segmento
- Tendencia por Estados de suscripción
- Tendencia de productos

 > [!NOTE]
 > Este informe está disponible en el panel de información. Para ver este informe, debe tener asignado un rol específico en el centro de Partners, como administrador global, administrador de la cuenta, visor de informes o visor de informes ejecutivos. Para obtener más información, consulte el administrador global de su empresa. Los tipos específicos de datos de este informe también pueden estar disponibles para los usuarios con privilegios ejecutivos del visor de informes.

**Resumen**

En la sección Resumen se presenta una vista de instantánea de los indicadores clave de rendimiento (KPI) relacionados con las suscripciones vendidas o administradas por el usuario para sus clientes.  

- Suscripciones: recuento actual de las suscripciones de productos en la nube vendidas o administradas por el usuario.
Porcentaje de crecimiento o disminución de suscripciones durante el intervalo de fechas seleccionado.

El micro gráfico presenta una tendencia mensual de suscripciones en el recuento durante el intervalo de fechas seleccionado.

- Suscripciones activas: recuento actual de suscripciones de productos en la nube con uso activo medido en función de la telemetría del producto. Esto excluye todas las suscripciones de prueba en el caso de las suscripciones de Azure.
Porcentaje de crecimiento o disminución de suscripciones activas durante el período de tiempo seleccionado.

El micro gráfico presenta una tendencia de mes a mes de suscripciones activas durante el intervalo de fechas seleccionado.

- Suscripciones agregadas: el número total de suscripciones de clientes que ha agregado (vendido o administrado) durante el intervalo de fechas seleccionado. Las nuevas suscripciones con estado **activo** o **renovado** se cuentan como suscripciones agregadas.
Porcentaje de crecimiento o rechazo de suscripciones agregadas en el último mes completo en comparación con el primer mes completo.

El micro gráfico presenta una tendencia mensual de las suscripciones agregadas durante el intervalo de fechas seleccionado.

- Suscripciones renovadas: se han renovado las suscripciones de clientes totales durante el intervalo de fechas seleccionado. Las suscripciones con estado **desaprovisionado** o **suspendidas** en ese mes se cuentan como una suscripción renovada.  
Porcentaje de suscripciones rotadas durante el intervalo de fechas seleccionado.

El micro gráfico presenta una tendencia mensual de las suscripciones rotadas en el intervalo de fechas seleccionado.

- Suscripciones por productos: desglose del número de suscripciones actual por productos en la nube.

:::image type="content" source="images/pci/pci-sub-report-summary-1.png" alt-text="Resumen del informe de suscripciones":::

**Propagación geográfica de suscripciones**

La vista **suscripciones por geografía** muestra la distribución geográfica de las suscripciones totales por mercados de clientes. El importe total de la suscripción incluye tanto las suscripciones vendidas como las suscripciones activas.

La tabla **número de países o** regiones presenta el total de países o regiones en los que tiene suscripciones y la cantidad por país de suscripciones totales y activas.

Puede buscar y seleccionar un país en la cuadrícula para ampliar la ubicación en el mapa. Presione la opción **Inicio** en el mapa para revertir a la vista original. Mantenga el puntero sobre el mapa para ver todas las suscripciones y suscripciones activas por país. Ambos campos de la cuadrícula se pueden ordenar.

:::image type="content" source="images/pci/pci-sub-report-sub-by-geography-2.png" alt-text="suscripciones por geografía":::

**Agregaciones de suscripción/paginación**

Esta vista presenta una tendencia de suscripciones. Estas se dividen en distintas categorías (nuevas, existentes y renovadas) para el intervalo de fechas seleccionado. El eje X representa los meses del intervalo de fechas seleccionado. El eje Y representa el recuento de suscripciones. Las suscripciones rotadas se representan en la escala negativa del eje Y. 

El gráfico de columnas apiladas presenta un desglose de las suscripciones nuevas, existentes y renovadas del mes. Puede volver a generar el gráfico de columnas, desglosado con elementos de pila concretos. Para ello, seleccione los elementos específicos en la leyenda. También puede utilizar el control deslizante de la parte superior del gráfico para acercar un período específico.

:::image type="content" source="images/pci/pci-sub-report-sub-adds-churns-3.png" alt-text="agregación de suscripciones y paginación":::

**Distribución de suscripciones**

Esta vista presenta un desglose de las suscripciones actuales por las ubicaciones de MPN, los segmentos de cliente, el canal de ventas o el modelo de precios de Azure y el tipo de atribución (por ejemplo, DPOR, DAP, etc.). Haga clic en las pestañas correspondientes para ver el desglose por estas categorías. Para generar el gráfico circular con un desglose de categorías de elementos específicas, seleccione esas categorías de elementos en la leyenda.

:::image type="content" source="images/pci/pci-sub-report-distribution-4.png" alt-text="distribución de suscripciones":::

**Distribución de estado de suscripción**

Esta vista muestra la distribución de las suscripciones de clientes actuales por Estado o estado de la suscripción. Esto incluye los siguientes Estados de suscripción: **activo**, **deshabilitado**, **desaprovisionado**, **abierto**, **gracia**, **cerrado**y **otros**.

:::image type="content" source="images/pci/pci-sub-report-sub-states-5.png" alt-text="distribución de estado de suscripción":::

**Tendencia de productos**

Esta vista muestra un gráfico de barras y dos gráficos circulares. El gráfico de barras presenta una tendencia mensual de las suscripciones desglosadas por productos comerciales, como Azure, Office, Dynamics, etc.

Los dos gráficos circulares muestran un desglose de las suscripciones de los clientes actuales. El primer gráfico circular divide las suscripciones por productos. El segundo gráfico circular divide las suscripciones por SKU o planes. Al seleccionar un producto en el gráfico circular desglose **por productos** , el gráfico circular adyacente mostrará un desglose de las suscripciones de este producto por SKU.

:::image type="content" source="images/pci/pci-sub-report-prods-trend-6.png" alt-text="tendencia de productos":::

> [!NOTE]
 > Es posible que el número de suscripciones dividido por SKU no siempre coincida con el número total de suscripciones para ese producto. Esto puede ocurrir si un cliente ha adquirido varias SKU en la misma suscripción de producto.

## <a name="next-steps"></a>Pasos siguientes

- Para obtener más informes, consulte [información del centro de Partners](partner-center-insights.md).
