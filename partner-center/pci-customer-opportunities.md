---
title: 'Partner Center Insights: informes de propens de CloudAscent'
description: Obtenga información sobre los informes de propens de CloudAscent en el centro de Partners. Incluye información sobre la propens de un cliente para comprar productos de Microsoft.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 09/18/2020
ms.openlocfilehash: fd017884c29df3874a06e8c4213c6fe5f05a8995
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/19/2020
ms.locfileid: "92175285"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>CloudAscent informes de propens disponibles en el panel del centro de Partners

**Roles adecuados**
- Visor de informes ejecutivos
- Visor de informes

El panel del centro de Partners proporciona datos de propens que se pueden descargar del programa CloudAscent. Los datos muestran la propens de los clientes para comprar productos de Microsoft.  En este artículo se describe el desglose de estos datos, cómo utilizar la puntuación y lo que significa.

## <a name="summary-definitions"></a>Definiciones de Resumen

- **Clientes de SMC**: este es el número total de clientes en las descargas de propens.  Los clientes se identifican por socio de registro.
- **Acuerdos de expiración**: dentro del año fiscal actual, se proporciona el número de contratos que van a expirar.
- Ingresos que van a **expirar**: los ingresos asociados a los contratos que han expirado.
- **Abrir ingresos por expiración**: los ingresos asociados a los acuerdos de expiración abiertos.

:::image type="content" source="images/pci/cust-oppor-1.png" alt-text="Captura de pantalla del panel de Resumen oportunidades de clientes.":::

## <a name="cloudascent-smb-segmentation"></a>Segmentación de SMB de CloudAscent

El segmento de pequeñas a medianas empresas (SMB) se divide aún más en tres subsegmentos distintos.

1. **Top no Managed** incluye los mayores clientes de SMB con la mayor oportunidad de Microsoft. Los clientes no administrados principales típicos comparten características similares a las cuentas administradas, con un gran número de empleados, grandes presupuestos y gastos de ti y grandes cantidades de ingresos potenciales para Microsoft.

   Definimos las dos maneras principales no administradas:

   - **Principales basados en usuarios no administrados**: incluye cuentas con 300 o más empleados. User-Based cuentas son objetivos excelentes para la compra por primera vez o la expansión de productos de suscripción basados en usuario como M365, D365 o Surface.
   - **Basado en el proceso superior no administrado** : incluye cuentas con un potencial de Azure mayor que $10k. Las cuentas basadas en procesos incluyen Azure existente. cuentas con un potencial de año futuro significativo y cuentas que aún no han adquirido Azure pero que tienen un potencial para Azure mayor que $10k.

2. La **empresa mediana** incluye a los clientes existentes y a las cuentas de cliente con 25 a 300 empleados.

3. La **pequeña empresa** incluye todas las empresas restantes con menos de 25 empleados.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Captura de pantalla del panel de Resumen oportunidades de clientes.":::

Los principales subsegmentos de empresa sin **administrar** y **medianas** representan a los clientes de valor de tiempo de vida (LTV) de Microsoft y de los asociados de Microsoft. Por lo tanto, son las principales áreas de enfoque para impulsar el crecimiento en este segmento. En estos dos subsegmentos, estamos mejor posicionados para adquirir el socket con M365, rentabilizar aún más con las aplicaciones de línea de negocio (LOB) de D365/Azure y darse de alta LTV para Microsoft.

Hoy tenemos dos áreas clave de la oportunidad: 1. nuestro cliente agrega crecimiento; dos. Aunque hacemos bien adquirir Sockets en la nube que conducen a M365, tenemos una gran oportunidad en D365 y Azure.

La siguiente captura de pantalla representa los tres subsegmentos SMB y las rutas optimizadas al mercado. CloudAscent priorizar la generación de perfiles, la puntuación y el modelado de todas las cuentas principales no administradas y medianas.

:::image type="content" source="images/pci/cust-oppor-3.png" alt-text="Captura de pantalla del panel de Resumen oportunidades de clientes.":::

## <a name="cloudascent-machine-learning"></a>Machine Learning CloudAscent

SMB usa tecnología de aprendizaje automático para impulsar predicciones de clientes de ventas y marketing dentro de los principales segmentos de negocio no administrados y medianos. ¿Cómo se recopilan y se convierten en recomendaciones de propens?

- **Recopilación de datos**: los rastreadores web examinan y recopilan miles de millones de señales de clientes haciendo ping en los dominios de la empresa y en supervisión: entradas de blog, comunicados de prensa, transmisiones sociales y foros técnicos.  Además de las señales recopiladas, la información de firmographics se recopila de orígenes internos y externos, como D&B, la suscripción interna de Microsoft y los datos transaccionales.

- **Machine learning**: las señales se introducen en el modelo de aprendizaje automático que genera un conjunto de datos estructurado de predicciones de ventas y marketing para cada cliente por producto y clúster en la nube.  Cada cliente se Puntua con un modelo de aspecto similar al de los principales SMB de Microsoft que determina el ajuste del cliente y los algoritmos de aprendizaje automático que integran el comportamiento en línea del cliente definen como intención. La puntuación se combina en clústeres que muestran la propens de un cliente para comprar Microsoft Cloud productos.

- **Optimización**: el sistema de machine learning optimiza los modelos mediante el consumo de los datos de la transacción mensualmente y los datos de la suscripción trimestralmente.  Mediante el uso de los datos de ganancia y pérdida, el Machine Learning ajusta los algoritmos y valida que los modelos funcionan según lo previsto mediante la comparación de las recomendaciones de clúster con las oportunidades en las que se ha actuado en el servidor principal.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Captura de pantalla del panel de Resumen oportunidades de clientes.":::

## <a name="cloudascent-propensity"></a>Propens CloudAscent

¿Cómo se crean las recomendaciones de propens?

Mediante el uso de señales recopiladas a través de rastreadores web y datos proporcionados desde diversos orígenes, consolidamos los datos de firmographics y las señales de medios sociales del cliente.  La puntuación usa estas señales y datos en los modelos de comparación para los modelos de ajuste y puntuación para el intento.

1. Ajuste de cuenta de cliente

   - Puntos de datos internos y externos que definen firmographics.

   - La puntuación de ajuste usa un modelo similar a nuestro mejor SMB para comparar a los clientes y ver si son posibles para los productos de Microsoft Cloud.

   - La puntuación de ajuste se actualiza trimestralmente

2. Intención de la cuenta de cliente

   - Las señales relacionadas con los medios sociales y el comportamiento en línea de un cliente definen el intento.

   - La puntuación de intención se superpone a la parte superior del ajuste para definir los clústeres.

   - La puntuación de intención se actualiza mensualmente.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Captura de pantalla del panel de Resumen oportunidades de clientes.":::

3. Agrupación en clústeres

   Las señales de ajuste y intención se consolidan en una puntuación de agrupación en clústeres. CloudAscent tiene cuatro clústeres:

      - Act Now: clientes preparados para ventas
      - Evaluar-clientes preparados para marketing
      - Cultivar: impulsar campañas de reconocimiento
      - Formación: formación y supervisión de la intención

   La agrupación en clústeres permite a los usuarios dirigirse a clientes específicos para iniciativas de ventas y marketing en función de factores de segmento, por ejemplo: producto, Geo, sector y vertical.

   La pestaña **modelo de propens** en los libros de CloudAscent comparte la propens y los ingresos de espacio en blanco estimados. Para definir la agrupación en clústeres de ajuste y intención, se repasan los pasos siguientes:

      1. Mediante el uso de modelos de aprendizaje automático, primero calculamos la puntuación de ajuste del cliente y la puntuación de intención en una escala de 100.  Las puntuaciones exactas variarán en función de los modelos de ML.  Puntuación de ejemplo a continuación:

         |**Clasificación**|**Puntuación**|
         |---------|:---------|
         |Alto|75-100|
         |Media|55-74|
         |Baja|30 - 54|
         |Muy bajo|0 - 29|

      2. Mediante el uso de la regla anterior, clasificamos las empresas como altas, medias, bajas y muy bajas en las señales de ajuste y intención de los clientes.

      3. Trazamos las señales de ajuste y intención de los clientes en una matriz 2D con cada intersección que representa la propens.     Por ejemplo, alto ajuste + intención alta = a1, que representa la mayor propens.

      4. Por último, estos segmentos se agrupan para crear clústeres.  Por ejemplo, a1, a2, a3, A4 forman el clúster de ACT Now.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Captura de pantalla del panel de Resumen oportunidades de clientes.":::

   Para estos clientes, recomendamos que el destino sea ahora y evalúe a los clientes.

## <a name="cloudascent-products--models"></a>Modelos de & de productos de CloudAscent

En el gráfico siguiente se proporciona una vista de cada modelo de propens en CloudAscent:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Captura de pantalla del panel de Resumen oportunidades de clientes.":::

Los modelos de espacio en blanco se componen de predicciones para los clientes de Microsoft existentes en los que no tienen un producto y/o son clientes de nuevas perspectivas netas.

Los modelos de venta incremental usan datos de transacciones para predecir la posibilidad de aumentar la capacidad de venta en SKU de Azure y M365.

EOS comparte los clientes de fin de servicio para Win 7, Office 2010, SQL Server y Windows Server. Los datos de EOS se extraen de MS Sales y se superpondrán con el modelado de propens CloudAscent cuando estén disponibles. Los datos de EOS residen en el trabajo moderno y se reproducen las ventas de Azure.
