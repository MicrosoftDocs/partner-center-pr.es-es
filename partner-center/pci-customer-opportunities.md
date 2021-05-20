---
title: 'Centro de partners Insights: informes de propensidad de CloudAscent'
description: Obtenga información sobre los informes de CloudAscent Propensity en Centro de partners. Incluye información sobre la propensión de un cliente a comprar productos de Microsoft.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 430aea81964d1b75514b6e1377bd2ba1af41b538
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110153045"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>Informes de Propensity de CloudAscent disponibles en Centro de partners panel

**Roles adecuados:** Visor de informes ejecutivos | Visor de informes

El Centro de partners proporciona datos de propiedad descargables del programa CloudAscent. Los datos muestran la probabilidad de los clientes de comprar productos de Microsoft.  En este artículo se describe el desglose de estos datos, cómo usar la puntuación y lo que significa.

## <a name="summary-definitions"></a>Definiciones de resumen

- **Clientes de SMC:** este es el número total de clientes en las descargas de propiedad.  Los clientes se identifican por asociado de registro.
- **Expirar contratos:** en el año fiscal actual, se proporciona el número de contratos que expiran.
- **Ingresos de expiración abiertos:** los ingresos asociados a los contratos de expiración abiertos.

:::image type="content" source="images/pci/cust-oppor-11.png" alt-text="Captura de pantalla del panel Resumen de oportunidades de clientes.":::

## <a name="cloudascent-smb-segmentation"></a>Segmentación de SMB cloudAscent

El segmento de pequeñas y medianas empresas (SMB) se divide en tres sub segmentos distintos.

1. **Los principales no administrados** incluyen los clientes SMB más grandes con más oportunidades para Microsoft. Los principales clientes no administrados comparten características similares a las cuentas administradas, con un gran número de empleados, grandes presupuestos de TI y gastos, y grandes cantidades de ingresos potenciales para Microsoft.

   Definimos Top Unmanaged de dos maneras:

   - **Principales basados en usuarios no** administrados: incluye cuentas con 300 o más empleados. User-Based cuentas son destinos excelentes para la compra por primera vez o la expansión de productos de suscripción basados en el usuario, como Microsoft 365, Dynamics 365 o Surface.
   - **Principal basado en proceso no administrado:** incluye cuentas con un potencial de Azure superior a 10 000 USD. Las cuentas basadas en proceso incluyen Azure existente. cuentas con un potencial significativo del año futuro y cuentas que aún no han comprado Azure, pero que tienen un potencial de Azure superior a 10 000 USD.

2. **Medium Business incluye** clientes existentes y cuentas de clientes potenciales con entre 25 y 300 empleados.

3. **Small Business** incluye empresas con entre 10 y 25 empleados.

4. **Very Small Business incluye** empresas con entre 1 y 9 empleados.

:::image type="content" source="images/pci/cust-oppor-2.png" alt-text="Cliente por tipo de SMC.":::

**Los principales**  subsegmentos de negocio medio y no administrado representan clientes de alto valor de tiempo de vida (LTV) para Microsoft y asociados de Microsoft. Por este problema, son las principales áreas de enfoque para impulsar el crecimiento en este segmento. En estos dos subsegmentos, estamos mejor posicionados para adquirir el socket con Microsoft 365, monetizar aún más con las aplicaciones de línea de negocio (LOB) de D365/Azure y lograr un alto LTV para Microsoft.

Hoy en día tenemos dos áreas clave de oportunidad: 1. nuestro cliente agrega crecimiento; 2. aunque se adquieren bien sockets en la nube a la Microsoft 365, tenemos una gran oportunidad en Dynamics 365 y Azure.

La captura de pantalla siguiente representa los cuatro subsegmentos smb. CloudAscent prioriza la generación de perfiles, la puntuación y el modelado de todas las cuentas principales de negocio no administradas y medianas.

:::image type="content" source="images/pci/cust-oppor-32.png" alt-text="Captura de pantalla de los subsegmentos de SMB.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB usa la tecnología de aprendizaje automático para impulsar las predicciones de clientes de ventas y marketing dentro de los segmentos principales de negocio no administrado y medio. ¿Cómo se recopilan y convierten las señales en recomendaciones de propiedad?

- **Recopilación** de datos: los rastreadores web analizan y recopilan miles de millones de señales de clientes haciendo ping a los dominios de la empresa y supervisando entradas de blog, notas de la publicación, transmisiones sociales y foros técnicos.  Además de las señales recopiladas, se recopila información de firmegrafía de orígenes internos y externos, como D&B, suscripción interna de Microsoft y datos transaccionales.

- **Machine Learning:** las señales se introducen en el modelo de aprendizaje automático que genera un conjunto de datos estructurado de predicciones de ventas y marketing para cada cliente por producto y clúster en la nube.  Cada cliente se puntua mediante un modelo similar al smb principal de Microsoft que determina el ajuste del cliente y los algoritmos de aprendizaje automático que integran el comportamiento en línea del cliente definen como intención. La puntuación se combina en clústeres que muestran la propensión de un cliente a comprar productos en la nube de Microsoft.

- **Optimización:** el Machine Learning optimiza los modelos consumiendo los datos de transacción mensualmente y los datos de suscripción trimestralmente.  Con los datos de win/loss, el Machine Learning ajusta los algoritmos y valida que los modelos funcionan según lo previsto mediante la comparación de las recomendaciones del clúster con las oportunidades que se han actuado en MSX.

:::image type="content" source="images/pci/cust-oppor-4.png" alt-text="Captura de pantalla del aprendizaje automático de SMB.":::

## <a name="cloudascent-propensity"></a>Propensidad de CloudAscent

¿Cómo se crean las recomendaciones de propensidad?

Mediante el uso de señales recopiladas a través de rastreadores web y datos proporcionados desde diversos orígenes, consolidamos los datos de firmographics y las señales de redes sociales del cliente.  La puntuación usa estas señales y datos en los modelos de comparación para ajustar y puntuar los modelos de intención.

1. Ajuste de la cuenta de cliente

   - Puntos de datos internos y externos que definen firmegrafías.

   - La puntuación de ajuste usa un modelo similar al de nuestro mejor SMB para comparar a los clientes y ver si son una posible opción para Los productos en la nube de Microsoft.

   - La puntuación de ajuste se actualiza trimestralmente

2. Intención de cuenta de cliente

   - Las señales relacionadas con las redes sociales y el comportamiento en línea de un cliente definen la intención.

   - La puntuación de intención se sobrepase sobre la opción adecuada para definir los clústeres.

   - La puntuación de intención se actualiza mensualmente.

   :::image type="content" source="images/pci/cust-oppor-5.png" alt-text="Modelos predictivos de SMB cloudAscent.":::

3. Agrupación en clústeres

   Las señales de ajuste e intención se consolidan en una puntuación de agrupación en clústeres. CloudAscent tiene cuatro clústeres:

      - Actuar ahora: clientes listos para ventas
      - Evaluación: clientes preparados para marketing
      - Fomentar: impulsar campañas de reconocimiento
      - Educación: educación y supervisión de intenciones

   La agrupación en clústeres permite a los usuarios dirigirse a clientes específicos para iniciativas de ventas y marketing basadas en factores de segmento, por ejemplo: producto, geo, sector y vertical.

   La **pestaña Modelo de propensidad** de los libros CloudAscent comparte la propiedad y los ingresos estimados del espacio en blanco. Para definir la agrupación en clústeres de Ajustar e Intención, se van a seguir estos pasos:

      1. Con los modelos de ML, primero calculamos la puntuación de ajuste del cliente y la puntuación de intención en una escala de 100.  Las puntuaciones exactas variarán en función de los modelos de ML.  Puntuaciones de ejemplo siguientes:

         |**Clasificación**|**Puntuación**|
         |---------|:---------|
         |Alto|75 - 100|
         |Media|55 - 74|
         |Bajo|30 - 54|
         |Muy bajo|0 - 29|

      2. Con la regla anterior, clasificamos las empresas para que sean alta, media, baja y muy baja en las señales de ajuste del cliente y de intención.

      3. Trazamos las señales de ajuste e intención del cliente en una matriz 2D con cada intersección que representa la propensidad. Por ejemplo, High Fit + High Intent = A1, que representa la mayor propensidad.

      4. Por último, estos segmentos se agrupan para formar clústeres.  Por ejemplo, A1, A2, A3, A4 forman el clúster Act Now.

         :::image type="content" source="images/pci/cust-oppor-6.png" alt-text="Modelos CloudAscent.":::

   Para estos clientes, se recomienda dirigirse a actuar ahora y evaluar a los clientes.

## <a name="cloudascent-products--models"></a>CloudAscent Products & Models

En el gráfico siguiente se proporciona una vista de cada modelo de propiedad dentro de CloudAscent:

:::image type="content" source="images/pci/cust-oppor-7.png" alt-text="Modelo de propensidad CloudAscent.":::

Los modelos de espacio en blanco se componen de predicciones para clientes de Microsoft existentes en los que no tienen un producto o son clientes potenciales nuevos.

Los modelos de venta al por mayor usan datos de transacción para predecir el potencial de ventas por uso en Azure Microsoft 365 SKU.

Estos clientes ya tendrán Azure o Microsoft 365 y el modelo de venta superior muestra que es probable que compren más de su SKU existente.

EOS comparte los clientes de fin de servicio (EOS) para Win 7, Office 2010, SQL Server y Windows Server. Los datos de EOS se extraen de MS Sales y se superpuestos con el modelado de propensidad cloudAscent cuando está disponible. Los datos de EOS se encuentra en las instancias de Modern Work y Azure Sales.
