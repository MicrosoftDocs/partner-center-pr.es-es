---
title: Definiciones de datos de Insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: El documento proporciona la lista de varios informes y las definiciones de datos de cada informe, que se pueden descargar desde la página del informe de descarga de Insights.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d4a805957fac7c7cff373d807347b7c6d0b13d6f
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/15/2020
ms.locfileid: "97501757"
---
# <a name="export--data-definitions"></a>Exportar: definiciones de datos 

 **Roles adecuados** 

- Visor de informes 
- Visor de informes ejecutivos 

## <a name="introduction"></a>Introducción 

El concentrador de informes de descarga del panel de Insights le permite exportar los conjuntos de datos sin procesar.  

Los distintos informes, que se pueden descargar junto con la definición de datos, son los siguientes: 

**Perfil de socio comercial**: las definiciones de datos de los distintos campos del informe de perfil son: 


| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|MPNId|IDENTIFICADOR de Microsoft Partner Network|
|PartnerName|Nombre del socio comercial |
|PGA_MPNId|IDENTIFICADOR de MPN de cuenta global de asociados|
|PGA_PartnerName|Nombre de cuenta global de socio comercial|
|City|Ubicación de la ciudad del asociado |
|País|Ubicación del país de socio comercial |
|HierarchyLevel|Indica si es un identificador de MPN global o un identificador de MPN de ubicación|

**Detalles del cliente**: las definiciones de datos de los distintos campos del informe detalles del cliente son:

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|CustomerName|Nombre del cliente |
|CustomerTenantId|Identificador de inquilino de cliente |
|CustomerTpid|Identificador primario del cliente superior |
|CustomerSegment|Segmento de cliente |
|CustomerMarket|Mercado geográfico del cliente  |
|CustomerStatus|Estado del cliente (/Inactive activo) |
|Producto|El producto se vende al cliente por el MPN. Este es uno de O365, D365, Enterprise Mobility, Power BI Microsoft Azure.|
|SKU|   SKU de producto|
|Month| Mes para el que se ha comunicado el uso y los ingresos|
|MPNId| IDENTIFICADOR de Microsoft Partner Network|
|PartnerName|   Nombre del socio comercial|
|PartnerLocation|   Ubicación geográfica del asociado|
|PartnerAttributionType|    Tipo de atribución de asociado|
|SalesChannel|  Sales Channel|
|AvailableSeats|    Puestos disponibles| 
|RevenueUSD|    Ingresos en USD|

**Rendimiento del reseller**: las definiciones de datos de los distintos campos de los informes de rendimiento del reseller son:

> [!Note]
> Los datos de ingresos y ACR solo están disponibles para los usuarios que son visores de informes ejecutivos.

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|ResellerMpnid|Identificador de Microsoft Partner Network reseller| 
|ResellerName|Reseller Name (Nombre del revendedor)|
|ResellerMarket|País Reseller de Market| 
|IndirectProviderMPNId|Identificador de Microsoft Partner Network de proveedor indirecto|
|IndirectProviderName|Nombre de proveedor indirecto|
|Month|Mes para el que se ha comunicado el uso y los ingresos|
|Producto|Nombre de producto|
|SubscriptionID|Identificador de suscripción|
|AvailableSeats|Número de puestos disponibles|
|AssignedSeats|Número de puestos asignados|
|BilledRevenueUSD|Ingresos facturados (en USD)|
|CustomerName|Nombre del cliente| 
|CustomerTPid|Identificador primario del cliente superior| 
|CustomerSegment|Segmento de cliente |
|CustomerMarket|Mercado geográfico del cliente |
|ResellerStatus|Estado del distribuidor| 

**Detalles de suscripciones**: las definiciones de datos de los distintos campos del informe de detalles de la suscripción son:

>[!Note]
>Los datos de ingresos y ACR solo están disponibles para los usuarios que son visores de informes ejecutivos

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|SubscriptionId|    GUID de la suscripción|
|SubscriptionStartDate| Fecha de inicio de la suscripción|
|SubscriptionEndDate|   Fecha de finalización de la suscripción|
|SubscriptionState| Estado de la suscripción (activo o reactivado)|
|Month| Mes para el que se ha comunicado el uso y los ingresos|
|IsAutoRenew|   Indica si la suscripción se renueva automáticamente o no (s/N)|
|CustomerName|  Nombre del cliente| 
|CustomerTenantId|  GUID del cliente|
|CustomerTpid|  Identificador primario del cliente superior| 
|CustomerSegment|   Segmento de mercado del cliente| 
|CustomerMarket|    Mercado geográfico del cliente|
|Producto|   Producto vendido al cliente por el asociado| 
|SKU|   SKU del producto |
|MPNId| IDENTIFICADOR Microsoft Partner Network del socio comercial |
|PartnerName|   Nombre del socio comercial |
|PartnerLocation|   Ubicación geográfica del socio |
|PartnerAttributionType|    Tipo de atribución para la suscripción|
|SalesChannel|  Canal de las ventas (directas/CSP, etc.) |
|AvailableSeats|    Puesto disponible actualmente|
|RevenueUSD|    Ingresos en USD|
|ID. de inscripción| IDENTIFICADOR de inscripción de la suscripción|

**Uso de Azure**: las definiciones de datos de los distintos campos del informe de uso de Azure son:

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|SubscriptionId|    GUID de la suscripción|
|SubscriptionStartDate| Fecha del inicio de la suscripción.|
|SubscriptionEndDate|   Fecha de finalización de la suscripción.|
|SubscriptionState| Estado actual de la suscripción (período abierto/cerrado/activo/ingracia)|
|Month| Fecha de agregación por mes |
|ServiceName|   Nombre del servicio de Azure|
|MeterCategory| Nombre de la categoría de medidor|
|UsageUnits|    El número de unidades utilizadas durante el ciclo de facturación |
|CustomerName|  Nombre del cliente |
|CustomerTenantId|  IDENTIFICADOR de inquilino del cliente |
|CustomerTpid|  IDENTIFICADOR primario del cliente superior |
|CustomerSegment|   Segmento del cliente |
|CustomerMarket|    Mercado geográfico del cliente |
|MPNId  |IDENTIFICADOR Microsoft Partner Network del cliente |
|PartnerName|   Nombre del socio comercial |
|PartnerLocation    |Ubicación geográfica del país del socio |
|PartnerAttributionType |Tipo de atribución de asociado|
|SalesChannel|  Canal de ventas (directo/CSP indirecto/CSP directo, etc.) |
|ACR_USD|   Ingresos consumidos por Azure en USD|
|ID. de inscripción| IDENTIFICADOR de inscripción de la suscripción de Azure|

**Office 365-uso de licencias**: las definiciones de datos de los distintos campos del informe de uso de licencias de Office 365 son:

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|CustomerTenantId|  IDENTIFICADOR de inquilino del cliente| 
|CustomerTpid|  IDENTIFICADOR primario del cliente superior |
|WorkloadName|  SFB, equipos, EXO |
|Month| Mes en el que se ha comunicado el uso|
|PaidAvailableUnits|    Número de unidades disponibles de pago|
|MonthlyActiveUsers|    Número de usuarios activos al mes|
|CustomerName|  Nombre del cliente|
|CustomerMarket|    Ubicación geográfica del país del mercado del cliente |
|CustomerSegment|   Segmento de cliente |
|MPNId| IDENTIFICADOR de Microsoft Partner Network|
|PartnerName|   Nombre del socio comercial|
|PartnerLocation|   Ubicación geográfica del asociado|
|PartnerAttributionType|    Tipo de atribución de asociado|

**Enterprise Mobility: uso de licencias**: la definición de datos de los distintos campos del informe de uso de licencias de EMS es:

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|CustomerTenantId|  IDENTIFICADOR de inquilino del cliente| 
|CustomerTpid|  IDENTIFICADOR primario del cliente superior |
|WorkloadName|  Nombre de la carga de trabajo de EMS |
|Month| Mes en el que se ha comunicado el uso|
|PaidAvailableUnits|    Número de unidades disponibles de pago|
|MonthlyActiveUsers|    Número de usuarios activos al mes|
|CustomerName|  Nombre del cliente|
|CustomerMarket|Ubicación geográfica del país del mercado del cliente |
|CustomerSegment|   Segmento de cliente |
|MPNId| IDENTIFICADOR de Microsoft Partner Network|
|PartnerName|   Nombre del socio comercial|
|PartnerLocation|   Ubicación geográfica del asociado|
|PartnerAttributionType|    Tipo de atribución de asociado|

**Dynamics 365 – uso de licencias**: la definición de datos de los distintos campos del informe de uso de licencias de Dynamics 365:

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|SubscriptionId|GUID de la suscripción|
|SubscriptionStartDate| Fecha de inicio de la suscripción|
|SubscriptionEndDate|   Fecha de finalización de la suscripción|
|SubscriptionStatus|    Estado de la suscripción |
|Month| Mes en el que se ha comunicado el uso|
|RevSumDivisionName|    Nombre de la división de la suma de Rev|
|RevSumCategoryName|    Nombre de la categoría de la suma de Rev.|
|SKU|   SKU del producto |
|SKUId| IDENTIFICADOR de SKU del producto |
|FreeVsPaidSKU| Indica si se trata de una SKU gratuita o de pago |
|SalesModel|    Canal de ventas usado para vender la suscripción|
|DetailedSalesModel|    Modelo de ventas detallado para la suscripción|
|CustomerName|  Nombre del cliente |
|CustomerTenantId|  GUID de inquilino de cliente |
|CustomerTpid|  Identificador primario del cliente superior |
|CustomerSegment|   Segmento de mercado del cliente |
|CustomerMarket|    Mercado geográfico del cliente |
|MPNId| IDENTIFICADOR de Microsoft Partner Network |
|PartnerName|   Nombre del socio comercial |
|PartnerLocation|   Ubicación geográfica del país del socio |
|PartnerAttachType| Tipo de atribución para la suscripción|
|AvailableSeats|    Puesto disponible actualmente|
|AssignedSeats| Puesto asignado actual |
|ActiveSeats|   Puestos activos actuales |
|DeploymentOpportunity| Oportunidad de implementación actual|
|ActiveUsagePercent|    Porcentaje de uso activo actual|
 
**Power bi el uso de licencias**: la definición de datos de los distintos campos del informe de uso de licencias Power BI es:

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|SubscriptionId|    GUID de la suscripción|
|SubscriptionStartDate| Fecha de inicio de la suscripción|
|SubscriptionEndDate|   Fecha de finalización de la suscripción|
|SubscriptionStatus|    Estado de la suscripción (activo o In-Active o en período de gracia)|
|Month| Fecha de agregación por mes |
|SKU|   SKU del producto |
|SKUId| IDENTIFICADOR de SKU del producto |
|FreeVsPaidSKU| Diferenciación de SKU gratis o de pago |
|SalesModel|    Modelo de ventas usado para vender la suscripción|
|DetailedSalesModel|    Modelo de ventas detallado para la suscripción|
|CustomerName|  Nombre del cliente |
|CustomerTenantId|  GUID de inquilino de cliente |
|CustomerTpid|  Identificador primario del cliente superior| 
|CustomerSegment|   Segmento de mercado del cliente |
|CustomerMarket|    Mercado geográfico del cliente |
|MPNId| IDENTIFICADOR de Microsoft Partner Network |
|PartnerName|   Nombre del socio comercial |
|PartnerLocation|   Ubicación geográfica del país del socio |
|PartnerAttachType| Tipo de atribución para la suscripción|
|AvailableSeats|    Puestos disponibles actualmente|
|AssignedSeats| Puestos asignados actuales|
|ActiveSeats|   Puestos activos actuales|
|DeploymentOpportunity| Oportunidad de implementación actual|
|ActiveUsagePercent|    Porcentaje de uso activo actual|

**Uso de equipos: reuniones y llamadas**: las definiciones de datos de los distintos campos son:

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|CustomerTenantId|  IDENTIFICADOR de inquilino del cliente |
|CustomerTpid|  IDENTIFICADOR primario del cliente superior |
|Month| Mes en el que se ha comunicado el uso|
|Subcarga de trabajo|   Subcarga de trabajo para el que se ha comunicado el uso (reuniones, llamadas, sistemas telefónicos)|
|Recuento de reuniones| Número de reuniones|
|Duración de la reunión|  Duración total de la reunión en horas|

**Equipos-detalles de uso mensual**: las definiciones de datos de los distintos campos son:

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|CustomerTenantId|  IDENTIFICADOR de inquilino del cliente |
|CustomerTpid|  IDENTIFICADOR primario del cliente superior |
|Month| Mes en el que se ha comunicado el uso|
|Subcarga de trabajo|   Subcarga de trabajo para el que se ha comunicado el uso (reuniones, llamadas, sistemas telefónicos)|
|Usuarios de escritorio| Número de usuarios que usan equipos en el escritorio|
|Usuarios móviles|  Número de usuarios que usan equipos en móvil|
|Usuarios Web| Número de usuarios que usan equipos en la web|
|AllUpParticipants| Número de usuarios distintos de equipos durante el mes|

**Uso de equipos: aplicaciones 3P**: las definiciones de datos de los distintos campos son:

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|CustomerTenantId|  IDENTIFICADOR de inquilino del cliente| 
|CustomerTpid|  IDENTIFICADOR primario del cliente superior |
|Month| Mes en el que se ha comunicado el uso|
|Nombre de la aplicación 3P|   Nombre de la aplicación Teams|
|Número de usuarios|    Número de usuarios de la aplicación|


**Detalles de aprendizaje**: las definiciones de datos de los distintos campos del informe de detalles de entrenamiento son:

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|TrainingActivityId|    Identificador del entrenamiento |
|TrainingTitle| Título del entrenamiento |
|TrainingType|  Tipo de entrenamiento (certificación/examen)|
|IndividualFirstName|   Nombre del cliente| 
|IndividualLastName|    Apellido del cliente| 
|Email| IDENTIFICADOR de correo electrónico personal del cliente|
|CorpEmail| IDENTIFICADOR de correo electrónico de Office del cliente|
|TrainingCompletionDate|    Fecha de finalización del entrenamiento |
|Month| Mes para el que se envían los datos|
|IcMCP| Indica si el usuario es un profesional certificado de Microsoft|
|MCPID| IDENTIFICADOR de MCP del usuario|
|MPNId| IDENTIFICADOR de Microsoft Partner Network |
|PartnerName|   Nombre del socio comercial |
|PartnerCityLocation|   Ubicación geográfica de la ciudad del socio |
|PartnerCountryLocation|    Ubicación geográfica del país del socio |

**Microsoft Learn**: las definiciones de datos de los distintos campos del informe de Microsoft Learn son:

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|UserName|Nombre del usuario| 
|UserId|GUID de usuario |
|TrainingName|Nombre del entrenamiento |
|TrainingType|Tipo de entrenamiento (módulo/Learning ruta de acceso)|
|Productos|Producto para el que se aplica el módulo de aprendizaje|
|Roles|Roles aplicables del entrenamiento |
|CompletionDate|Fecha de finalización del entrenamiento |
|MPNId|IDENTIFICADOR de Microsoft Partner Network |
|PartnerName|Nombre del socio comercial |
|País|Ubicación geográfica del país del socio |

**Resumen y historial de aptitudes**: la definición de datos de los distintos campos del informe de Resumen y historial de la competencia es:

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|CompetencyName|Nombre de la competencia |
|CompetencyLevel|Nivel de competencia (oro/Silver)|
|CompetencyStatus|Estado actual de la competencia (activo/inactivo/en período de gracia)|
|CompetencyStartDate|Fecha de inicio de la competencia determinada| 
|CompetencyEndDate|Fecha de finalización de la competencia determinada |

**Rendimiento** de la competencia: las definiciones de datos de los distintos campos del informe de rendimiento de la competencia son:

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|CompetencyName|    Nombre de la competencia |
|CompetencyAttainmentOptionName|    Nombre de la opción de obtención de aptitudes|
|Month| Mes para el que se registran las métricas|
|MetricName|    Nombre de la métrica relevante para la competencia|
|MetricMonthlyContribution| Contribución mensual de la métrica|
|TTMAggregate|  Métrica agregada para los 12 meses finales|
|AnniversaryYearAggregate|  Métrica agregada para el año de aniversario actual|
|GoldThreshold| Requisitos de rendimiento para satisfacer la competencia Gold|
|SilverThreshold|   Requisitos de rendimiento para satisfacer la competencia Silver|

**Ascenso de nube-M365 propens**: las definiciones de datos de los distintos campos del informe de propens de la nube Ascent-M365 son:

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|Identificador de MPN|    IDENTIFICADOR de Microsoft Partner Network|
|Nombre del asociado|  Nombre del socio comercial|
|Customer ID|   Número de identificación del cliente |
|Número DUNS|   El número de Dun & Bradstreet del cliente que se está puntuando para la propens|
|Nombre de cuenta|  Nombre de la cuenta |
|Dominio|    Dominio de la cuenta|
|Tamaño de la organización|  Tamaño de la organización|
|Sector|  Sector  |
|Vertical|  El vertical del cliente que se está puntuando para la propens, tal y como lo identifica Microsoft y otros estándares del sector (D&B)|
|Área|  Área geográfica de la ubicación|
|Subsidiaria|    La filial del cliente que se está puntuando para la propens|
|Territorio de ventas|   Territorio de ventas del cliente que se está puntuando para la propens|
|City|  Ubicación de la ciudad geográfica |
|Estado| Ubicación geográfica del estado|
|Código postal|   Código postal|
|País|   Ubicación geográfica del país |
|Segment|   Segmento de mercado |
|Subsegmento|   Subsegmento de mercado |
|Resumen de tipo de SMC|  Tipo de SMC |
|Top no administrado: base de proceso|  Principales clientes no administrados: proceso|
|Base de usuario no administrada superior| Principales clientes no administrados: usuario|
|IsNonProfit|   Si no es de lucro o para Profit (sí/no)|
|Habilitar el destino remoto en Exchange Online|   Clientes que tienen una suscripción activa a Exchange Online, que se venden a M365|
|Habilitación de la adquisición remota de trabajo local (versión actual) con CLAS propens-+ 10 licencias|Cliente que tiene un cliente de Office o Win local actual (es decir, versiones posteriores a los productos de EOS). El cliente tiene 10 o más licencias. Cliente que tiene una puntuación de propens. Los asociados deben tener como destino la conversión a M365.|
|Habilitación de la adquisición remota de trabajo local (versión actual) con CLAS propens-<10 licencias|Cliente que tiene un cliente de Office o Win local actual (es decir, versiones posteriores a los productos de EOS). El cliente tiene menos de 10 licencias. Cliente que tiene una puntuación de propens. Los asociados deben tener como destino la conversión a M365.|
|Habilitación de la adquisición remota de trabajo local (versión actual) sin CLAS propens-+ 10 licencias| Cliente que tiene un cliente de Office o Win local actual (es decir, versiones posteriores a los productos de EOS). El cliente tiene 10 o más licencias. El cliente no tiene una puntuación de propens. Los asociados deben tener como destino la conversión a M365.|
|Habilitación de la adquisición remota de trabajo local (versión actual) sin CLAS propens-<10 licencias| Cliente que tiene un cliente de Office o Win local actual (es decir, versiones posteriores a los productos de EOS). El cliente tiene menos de 10 licencias. El cliente no tiene una puntuación de propens. Los asociados deben tener como destino la conversión a M365.|
|Habilitación de la adquisición remota de trabajo local (EOS) con CLAS propens-+ 10 licencias|Cliente que tiene un cliente de Office o Win local de EOS (es decir, las versiones anteriores a y que incluyen los productos de EOS). El cliente tiene 10 o más licencias. El cliente tiene una puntuación de propens. Los asociados deben tener como destino la conversión a M365.|
|Habilitación de la adquisición remota de trabajo local (EOS) con CLAS propens-<10 licencias|Cliente que tiene un cliente de Office o Win local de EOS (es decir, las versiones anteriores a y que incluyen los productos de EOS). El cliente tiene menos de 10 licencias. El cliente tiene una puntuación de propens. Los asociados deben tener como destino la conversión a M365.|
|Habilitación de la adquisición remota de trabajo local (EOS) sin CLAS propens-+ 10 licencias| Cliente que tiene un cliente de Office o Win local actual (es decir, versiones anteriores a y que incluyen productos de EOS). El cliente tiene 10 o más licencias. El cliente no tiene una puntuación de propens. Los asociados deben tener como destino la conversión a M365.|
|Habilitación de la adquisición remota de trabajo local (EOS) sin CLAS propens-<10 licencias| Cliente que tiene un cliente de Office o Win local actual (es decir, versiones anteriores a y que incluyen productos de EOS). El cliente tiene menos de 10 licencias. El cliente no tiene una puntuación de propens. Los asociados deben tener como destino la conversión a M365.|
|Habilitar trabajo remoto: alto de propens para M365 (ACT Now/Evaluate)| Cliente potencial con alta propens para M365.|
|Habilitar trabajo remoto: competir (zoom) con M365| Clientes con zoom y M365, destinados a la conversión a equipos|
|Habilitar trabajo remoto: competir (zoom) sin M365|  Clientes con zoom, destinados a la conversión a equipos|
|Reduzca el costo y administre-M365 E3 dirigido a M365 E5| Cliente existente con M365 E3, destino para M365 E5|
|Reduzca el costo y administre los clientes de M365 BB y BS dirigidos a M365 BP.|    Los clientes de M365 BB y BS existentes, tienen como destino M365 BP|
|Transformar la productividad de la organización: propens de superficie|    El cliente muestra la propens de la superficie.|
|M365Cluster|Identifica la propens del cliente para comprar M365.  Los clústeres actúan ahora y la evaluación debe ser de destino, ya que producirán un mayor rendimiento.  Cultivar y educar a los clientes solo deben tener como destino si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes.|
|M365Fit|   Puntos de datos internos y externos que definen firmographics. La puntuación de ajuste usa un modelo similar a nuestro mejor SMB para comparar a los clientes y ver si son posibles para los productos de Microsoft Cloud. La puntuación de ajuste se actualiza trimestralmente.|
|M365Intent|    Las señales relacionadas con los medios sociales y el comportamiento en línea de un cliente definen el intento. La puntuación de intención se superpone a la parte superior del ajuste para definir los clústeres. La puntuación de intención se actualiza mensualmente.|
|SurfaceCluster|    Esto identifica la propens del cliente para la superficie de compra mediante la consolidación de las recomendaciones de ajuste y intención en un clúster.  Los clústeres actúan ahora y la evaluación debe ser de destino, ya que producirán un mayor rendimiento.  Cultivar y educar a los clientes solo deben tener como destino si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes.|
|SurfaceFit|    Puntos de datos internos y externos que definen firmographics. La puntuación de ajuste usa un modelo similar a nuestro mejor SMB para comparar a los clientes y ver si son posibles para los productos de Microsoft Cloud. La puntuación de ajuste se actualiza trimestralmente.|
|SurfaceIntent| Las señales relacionadas con los medios sociales y el comportamiento en línea de un cliente definen el intento. La puntuación de intención se superpone a la parte superior del ajuste para definir los clústeres. La puntuación de intención se actualiza mensualmente.|
|O365Cluster|   Esto identifica la propens del cliente para comprar O365.  Los clústeres actúan ahora y la evaluación debe ser de destino, ya que producirán un mayor rendimiento.  Cultivar y educar a los clientes solo deben tener como destino si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes.|
|O365Fit|   Puntos de datos internos y externos que definen firmographics. La puntuación de ajuste usa un modelo similar a nuestro mejor SMB para comparar a los clientes y ver si son posibles para los productos de Microsoft Cloud. La puntuación de ajuste se actualiza trimestralmente.|
|O365Intent|    Las señales relacionadas con los medios sociales y el comportamiento en línea de un cliente definen el intento. La puntuación de intención se superpone a la parte superior del ajuste para definir los clústeres. La puntuación de intención se actualiza mensualmente.|
|M365UpsellCustomer|    Esto identifica si el cliente muestra la propens de venta incremental para M365|
|Tiene Google|    Esta marca identifica si un cliente muestra señales competitivas para los productos de Google de propiedad.|
|Tiene AWS|   Esta marca identifica si un cliente muestra señales competitivas para productos AWS de propiedad.|
|Tiene EA|    Esto identifica si una renovación es un contrato Enterprise (EA) o una suscripción de EA|
|Tiene abierto|  Esto identifica si una renovación es un acuerdo de valor abierto o abierto.|

**Ascenso de nube-D365 propens**: las definiciones de datos de los distintos campos del informe de propens de la nube Ascent-D365 son:

| **Nombre de la columna** | **Descripción de datos** |
|---------|:---------|
|Identificador de MPN|    IDENTIFICADOR de Microsoft Partner Network|
|Nombre del asociado|  Nombre del socio comercial|
|Customer ID|   Número de identificación del cliente |
|Número DUNS|   El número de Dun & Bradstreet del cliente que se está puntuando para la propens|
|Nombre de cuenta|  Nombre de la cuenta |
|Dominio|    Dominio de la cuenta|
|Tamaño de la organización|  Tamaño de la organización|
|Sector|  Sector  |
|Vertical|  El vertical del cliente que se está puntuando para la propens, tal y como lo identifica Microsoft y otros estándares del sector (D&B)
|Área|  Área geográfica de la ubicación|
|Subsidiaria|    La filial del cliente que se está puntuando para la propens|
|Territorio de ventas|   Territorio de ventas|
|City|  Ubicación de la ciudad geográfica |
|Estado| Ubicación geográfica del estado|
|Código postal|   Código postal|
|País|   Ubicación geográfica del país |
|Segment|   Segmento de mercado |
|Subsegmento|   Subsegmento de mercado |
|Resumen de tipo de SMC|  La categorización de un cliente: las principales bases de usuarios no administradas son los clientes con más de 300 empleados, la base de proceso superior no administrada son clientes con un valor de US $10k en Azure de 3 años, una empresa mediana son clientes con 25 empleados o más, y las pequeñas empresas son clientes con menos de 25 empleados.|
|Top no administrado: base de proceso   |Principales clientes no administrados: proceso|
|Base de usuario no administrada superior| Principales clientes no administrados: usuarios|
|IsNonProfit|   Si no es de lucro o para Profit (sí/no)|
|Activar ventas digitales-M365 tamaño de la sede >= 25 puestos (modelo de propens de SalesPro)|   Cliente sin D365. Tamaño del puesto: 25 +. Los asociados deben tener como destino la venta cruzada de D365 SalesPro|
|Activar la venta digital: D365 SalesPro propens (ACT Now/Evaluate) |Clientes de alta propens sin D365.  Los asociados deben tener como destino D365 SalesPro.|
|Administración de riesgos financieros & fraude: base de la instalación local de Dynamics-Navision (modelo de propens de BC)|Cliente existente con el servicio local de Navision.  El asociado debe tener como destino for D365 BC|
|Administración del riesgo financiero & fraude: base de la instalación local de Dynamics-AX (modelo de propens de F&O)    |Cliente existente con AX local.  El asociado debe tener como destino D365 F&O|
|Administración de riesgos financieros & fraude: base de la instalación local de Dynamics-Great Plains (modelo de propens de BC)|  Cliente existente con Great Plains local.  El asociado debe tener como destino for D365 BC|
|Administración de riesgos financieros & fraude: base de la instalación local de Dynamics-Solomon (modelo de propens de BC)|Cliente existente con la infraestructura local Solomon.  El asociado debe tener como destino for D365 BC|
|Administración de riesgos financieros & fraude-base de instalación local de Dynamics-otros (modelo de propens de BC) |Cliente existente con otras soluciones locales no enumeradas anteriormente.  El asociado debe tener como destino for D365 BC|
|Creación de procesos empresariales ágiles: base de instalación local de Dynamics-AX/GP/SL/NAV/otros (modelo de propens de D365)|   Creación de procesos empresariales ágiles: base de instalación local de Dynamics-AX/GP/SL/NAV/otros (modelo de propens de D365)|
|Creación de procesos empresariales ágiles: Dynamics compite base-Mendix/OutSystems/Salesforce (modelo de propens de D365)| Creación de procesos empresariales ágiles: Dynamics compite base-Mendix/OutSystems/Salesforce (modelo de propens de D365)|
|Cree procesos empresariales ágiles: D365 F&O base de instalación |Clientes de D365 F&O existentes.  Asociado para dirigirse a Power apps.|
|Crear procesos empresariales ágiles: base de instalación de BC de D365| Clientes de BC de D365 existentes. Asociado para dirigirse a Power apps.|
|Crear procesos empresariales ágiles: base de instalación de D365 CE| Clientes existentes de D365 CE. Asociado para dirigirse a Power apps.|
|Cree una cadena de suministro resistente: gane y active la primera carga de trabajo de D365 como cadena de suministro de D365 con clientes de SAP que no son de Oracle o SAP|  Clientes de destino para la cadena de suministro de D365.|
|Compilar una cadena de suministro resistente: D365 de la cadena de suministro y/o venta directa/comercio a los clientes existentes de D365 CE |Los clientes existentes de D365 CE se dirigen a la cadena de suministro D365 entre ventas cruzadas|
|Cree una cadena de suministro resistente-cross-sell D365 sup. Chain AND/OR Retail/Commerce to D365 CE AND (Oracle OR SAP)| Clientes existentes de D365 CE con Oracle o SAP para tener como destino la cadena de suministro de D365|
|D365BCCluster| Esto identifica la propens del cliente para comprar D365 Business central.  Los clientes que muestren la propens para BC estarán en las categorías medianas y pequeñas.  Los clústeres actúan ahora y la evaluación debe ser de destino, ya que producirán un mayor rendimiento.  Cultivar y educar a los clientes solo deben tener como destino si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes.|
|D365BCFit| Puntos de datos internos y externos que definen firmographics. La puntuación de ajuste usa un modelo similar a nuestro mejor SMB para comparar a los clientes y ver si son posibles para los productos de Microsoft Cloud. La puntuación de ajuste se actualiza trimestralmente.|
|D365BCIntent|  Las señales relacionadas con los medios sociales y el comportamiento en línea de un cliente definen el intento. La puntuación de intención se superpone a la parte superior del ajuste para definir los clústeres. La puntuación de intención se actualiza mensualmente.|
|D365FOCluster| Esto identifica la propens del cliente para comprar D365 Finance and Operations.  Los clientes que muestren la propens de F&O estarán en las categorías principales no administradas. Los clústeres actúan ahora y la evaluación debe ser de destino, ya que producirán un mayor rendimiento.  Cultivar y educar a los clientes solo deben tener como destino si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes.|
|D365FOFit| Puntos de datos internos y externos que definen firmographics. La puntuación de ajuste usa un modelo similar a nuestro mejor SMB para comparar a los clientes y ver si son posibles para los productos de Microsoft Cloud. La puntuación de ajuste se actualiza trimestralmente.|
|D365FOIntent|  Las señales relacionadas con los medios sociales y el comportamiento en línea de un cliente definen el intento. La puntuación de intención se superpone a la parte superior del ajuste para definir los clústeres. La puntuación de intención se actualiza mensualmente.|
|D365CECluster| Esto identifica la propens del cliente para adquirir D365 Customer Engagement.  Los clientes que muestren la propens para CE estarán en las categorías mediana y pequeña.  Los clústeres actúan ahora y la evaluación debe ser de destino, ya que producirán un mayor rendimiento.  Cultivar y educar a los clientes solo deben tener como destino si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes.|
|D365CEFit| Ajustar para D365 CE|
|D365CEIntent|  Intención de D365 CE|
|DynamicsOnPremAXorCRM_HasOpenRenewal|  Esto identifica si un cliente tiene una renovación abierta para Dynamics local AX o CRM.|
|M365UpsellCustomer|    Esto identifica si el cliente muestra la propens de venta incremental para M365|
|Tiene Google|    Esta marca identifica si un cliente muestra señales competitivas para los productos de Google de propiedad.|
|Tiene AWS|   Esta marca identifica si un cliente muestra señales competitivas para productos AWS de propiedad.|
|Tiene EA |Esto identifica si una renovación es un contrato Enterprise (EA) o una suscripción de EA|
|Tiene abierto|  Esto identifica si una renovación es un acuerdo de valor abierto o abierto.|

**Propens de Ascent-Azure** en la nube: las definiciones de datos de los distintos campos del informe de propens de la nube Ascent-Azure son:

|**Nombre de la columna** |**Descripción de datos** |
|---------|:---------|
|Identificador de MPN|    IDENTIFICADOR de Microsoft Partner Network|
|Nombre del asociado|  Nombre del socio comercial|
|Customer ID|   Número de identificación del cliente |
|Número DUNS|   El número de Dun & Bradstreet del cliente que se está puntuando para la propens|
|Nombre de cuenta|  Nombre de la cuenta |
|Dominio|    Dominio de la cuenta|
|Tamaño de la organización|  Tamaño de la organización|
|Sector|  Sector  |
|Vertical|  El vertical del cliente que se está puntuando para la propens, tal y como lo identifica Microsoft y otros estándares del sector (D&B)|
|Área|  Área geográfica de la ubicación|
|Subsidiaria|    La filial del cliente que se está puntuando para la propens|
|Territorio de ventas|   Territorio de ventas|
|City|  Ubicación de la ciudad geográfica |
|Estado| Ubicación geográfica del estado|
|Código postal|   Código postal|
|País|   Ubicación geográfica del país |
|Segment|   Segmento de mercado |
|Subsegmento|   Subsegmento de mercado |
|Resumen de tipo de SMC|  Tipo de SMC |
|Top no administrado: base de proceso|  Principales clientes no administrados: proceso|
|Base de usuario no administrada superior| Principales clientes no administrados: usuarios|
|IsNonProfit|   Si no es de lucro o para Profit (sí/no)|
|Migrate-EOS Win Server-EOS Windows Server IB with CLAS propens-5 + licenses|   Cliente que tiene el servidor de Win local de EOS (es decir, las versiones anteriores a y que incluyen los productos de EOS). El cliente tiene 5 o más licencias. Cliente que tiene una puntuación de propens.  Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrate-EOS Win Server-EOS Windows Server IB with CLAS propens-<5 licencias|   Cliente que tiene EOS (fin de servicio) servidor Win local (es decir, versiones anteriores e incluyendo productos de EOS). El cliente tiene menos de 5 licencias. Cliente que tiene una puntuación de propens.  Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrate-EOS Win Server-EOS Windows Server IB sin propens de CLAS-5 licencias |Cliente que tiene el servidor de Win local de EOS (es decir, las versiones anteriores a y que incluyen los productos de EOS). El cliente tiene más de 5 licencias. El cliente no tiene una puntuación de propens. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrar-EOS Win Server-EOS Windows Server IB sin CLAS propens-<5 licencias|    Cliente que tiene el servidor de Win local de EOS (es decir, las versiones anteriores a y que incluyen los productos de EOS). Tiene menos de 5 licencias. El cliente no tiene una puntuación de propens. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrate-EOS SQL-EOS SQL Server IB with CLAS propens-5 + licenses|  Cliente que tiene un SQL Server de EOS local (es decir, las versiones anteriores a y que incluyen los productos de EOS). El cliente tiene más de 5 licencias. El cliente tiene una puntuación de propens.  Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrate-EOS SQL-EOS SQL Server IB con CLAS propens-<5 licencias|  Cliente que tiene un SQL Server de EOS local (es decir, las versiones anteriores a y que incluyen los productos de EOS). Tiene menos de 5 licencias. Cliente que tiene una puntuación de propens. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrate-EOS SQL-EOS SQL Server IB sin propens de CLAS-5 licencias|   Cliente que tiene un SQL Server de EOS local (es decir, las versiones anteriores a y que incluyen los productos de EOS). El cliente tiene 5 o más licencias. El cliente no tiene una puntuación de propens. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrate-EOS SQL-EOS SQL Server IB sin propens CLAS-<5 licencias|   Cliente que tiene un SQL Server de EOS local (es decir, las versiones anteriores a y que incluyen los productos de EOS). El cliente tiene menos de 5 licencias. El cliente no tiene una puntuación de propens. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrar: migrar el servidor Win local: Windows Server IB actual con CLAS propens-5 + licencias|   Cliente que tiene el servidor de Win local actual (es decir, versiones posteriores a los productos de EOS). El cliente tiene más de 5 licencias. El cliente tiene una puntuación de propens. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrar: migrar el servidor Win local: Windows Server IB actual con CLAS propens-<5 licencias|   Cliente que tiene el servidor de Win local actual (es decir, versiones posteriores a los productos de EOS). El cliente tiene menos de 5 licencias. El cliente tiene una puntuación de propens de Azure. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrar: migrar el servidor de Win local: Windows Server IB actual sin propens de CLAS-5 licencias|    Cliente que tiene el servidor de Win local actual (es decir, versiones posteriores a los productos de EOS). El cliente tiene más de 5 licencias. El cliente no tiene una puntuación de propens. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrar: migrar el servidor Win local: Windows Server IB actual sin CLAS propens-<5 licencias |Cliente que tiene el servidor de Win local actual (es decir, versiones posteriores a los productos de EOS). El cliente tiene menos de 5 licencias. El cliente no tiene una puntuación de propens. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrar: migrar a Azure SQL o a máquinas virtuales de SQL: actual SQL Server IB con CLAS propens-5 + licencias|  Cliente que tiene el SQL Server local actual (es decir, las versiones posteriores a los productos de EOS). El cliente tiene más de 5 licencias. El cliente tiene una puntuación de propens. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrar-migrar a Azure SQL o máquinas virtuales de SQL: actual SQL Server IB con propens-<5 licencias de CLAS|  Cliente que tiene el SQL Server local actual (es decir, las versiones posteriores a los productos de EOS). El cliente tiene menos de 5 licencias. El cliente tiene una puntuación de propens. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrar-migrar a Azure SQL o a máquinas virtuales de SQL: actual SQL Server IB sin propens CLAS-5 licencias|   Cliente que tiene el SQL Server local actual (es decir, las versiones posteriores a los productos de EOS). El cliente tiene más de 5 licencias. El cliente no tiene una puntuación de propens. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrar-migrar a Azure SQL o máquinas virtuales de SQL: actual SQL Server IB sin propens CLAS-<5 licencias|   Cliente que tiene el SQL Server local actual (es decir, las versiones posteriores a los productos de EOS). El cliente tiene menos de 5 licencias. El cliente no tiene una puntuación de propens. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrar-OSS-migrar a OSS DB| Cliente existente con cualquiera de los siguientes productos de la competencia: PostgreSQL, MySQL, MariaDB. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migración-OSS-Linux en Azure |Cliente existente con el producto: Linux. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migración de SAP-SAP en Azure|  Cliente existente con el producto: SAP. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrate-WVD-RDS IB |Identifica a los clientes con Windows Servicios de Escritorio remoto activos. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migración-WVD-trabajo moderno de venta cruzada a Azure/WVD|   Identifica a los clientes con M365 y no tiene Azure. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrar: VMware IB|   Cliente existente con el producto: VMware. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Migrar: Citrix IB|   Cliente existente con el producto: Citrix Systems. Los asociados deben dirigirse a estos clientes para la migración a Azure.|
|Innovate-Analytics-Power BI IB w/alta propens de Azure|   Los clientes con y la suscripción de Power BI activa incluyen: Power BI-independiente Pro, Power BI: conjuntos de Azure, conjuntos de Power BI-Office, conjuntos de Power BI-M365|
|Enable-DevOps con GitHub-VisualStudio/MSDN IB|    Clientes identificados con Visual Studio|
|Versión estándar de Win Server|   Esto muestra la versión de compras estándar de Windows Server por parte del cliente|
|Licencia de Win Server Standard|   Esto muestra el tipo de licencia de compras de Windows Server Standard por parte del cliente|
|Versión del centro de datos de Win Server|    Muestra la versión de compras del centro de datos de Windows por parte del cliente|
|Licencia del centro de datos de Win Server| Esto muestra el tipo de licencia de compras del centro de datos de Windows por parte del cliente|
|AzureFit|  Puntos de datos internos y externos que definen firmographics. La puntuación de ajuste usa un modelo similar a nuestro mejor SMB para comparar a los clientes y ver si son posibles para los productos de Microsoft Cloud. La puntuación de ajuste se actualiza trimestralmente.|
|AzureIntent|   Las señales relacionadas con los medios sociales y el comportamiento en línea de un cliente definen el intento. La puntuación de intención se superpone a la parte superior del ajuste para definir los clústeres. La puntuación de intención se actualiza mensualmente.|
|AzureCluster|  Esto identifica la propens del cliente para adquirir Azure mediante la consolidación de las recomendaciones de ajuste y intención en un clúster.  Los clústeres actúan ahora y la evaluación debe ser de destino, ya que producirán un mayor rendimiento.  Cultivar y educar a los clientes solo deben tener como destino si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes.|
|WindowsServerDataCenter_HasOpenRenewal|    Esto identifica si un cliente tiene una renovación abierta para un centro de datos de Windows Server|
|WindowsServerStandard_HasOpenRenewal|  Esto identifica si un cliente tiene una renovación abierta para Windows Server Standard|
|AzureUpsellCustomer|   Esto identifica si el cliente muestra una propens de venta incremental para Azure|
|Tiene Google|    Esta marca identifica si un cliente muestra señales competitivas para los productos de Google de propiedad.|
|Tiene AWS|   Esta marca identifica si un cliente muestra señales competitivas para productos AWS de propiedad.|
|Tiene EA |Esto identifica si una renovación es un contrato Enterprise (EA) o una suscripción de EA|
|Tiene abierto|  Esto identifica si una renovación es un acuerdo de valor abierto o abierto.|

Supens de las **renovaciones de Ascent-Agreement** en la nube: las definiciones de datos de los distintos campos del informe de propens de renovación del acuerdo de ascenso de la nube son las siguientes:

|**Nombre de la columna** |**Descripción de datos** |
|---------|:---------|
|Identificador de MPN|    IDENTIFICADOR de Microsoft Partner Network|
|Nombre del asociado|  Nombre del socio comercial|
|Customer ID|   Número de identificación del cliente |
|Número DUNS|   El número de Dun & Bradstreet del cliente que se está puntuando para la propens|
|Nombre de cuenta|  Nombre de la cuenta |
|Dominio|    Dominio de la cuenta|
|Tamaño de la organización|  Tamaño de la organización|
|Sector|  Sector  |
|Vertical|  El vertical del cliente que se está puntuando para la propens, tal y como lo identifica Microsoft y otros estándares del sector (D&B)|
|Área|  Área geográfica de la ubicación|
|Subsidiaria|    La filial del cliente que se está puntuando para la propens|
|Territorio de ventas|   Territorio de ventas|
|City|  Ubicación de la ciudad geográfica |
|Estado| Ubicación geográfica del estado|
|Código postal|   Código postal|
|País|   Ubicación geográfica del país |
|Segment|   Segmento de mercado |
|Subsegmento|   Subsegmento de mercado |
|Resumen de tipo de SMC|  Tipo de SMC |
|Top no administrado: base de proceso|  Principales clientes no administrados: proceso|
|Base de usuario no administrada superior| Principales clientes no administrados: usuarios|
|IsNonProfit|Si no es de lucro o para Profit (sí/no)|
|Tiene Google|Esta marca identifica si un cliente muestra señales competitivas para productos AWS de propiedad.|
|Tiene AWS|Esta marca identifica si un cliente muestra señales competitivas para productos AWS de propiedad.|
|Clúster de Azure|Esto identifica la propens del cliente para comprar Azure.  Los clústeres actúan ahora y la evaluación debe ser de destino, ya que producirán un mayor rendimiento.  Cultivar y educar a los clientes solo deben tener como destino si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes.|
|Clúster de D365 F&O|  Esto identifica la propens del cliente para comprar D365 Finance and Operations.  Los clientes que muestren la propens de F&O estarán en las categorías principales no administradas.  Los clústeres actúan ahora y la evaluación debe ser de destino, ya que producirán un mayor rendimiento.  Cultivar y educar a los clientes solo deben tener como destino si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes.|
|Clúster de D365 CE|   Esto identifica la propens del cliente para adquirir D365 Customer Engagement.  Los clientes que muestren la propens para CE estarán en las categorías mediana y pequeña.  Los clústeres actúan ahora y la evaluación debe ser de destino, ya que producirán un mayor rendimiento.  Cultivar y educar a los clientes solo deben tener como destino si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes.|
|Clúster de BC de D365|   Esto identifica la propens del cliente para comprar D365 Business central.  Los clientes que muestren la propens para BC estarán en las categorías medianas y pequeñas.  Los clústeres actúan ahora y la evaluación debe ser de destino, ya que producirán un mayor rendimiento.  Cultivar y educar a los clientes solo deben tener como destino si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes.|
|Clúster de M365|  Esto identifica la propens del cliente para comprar M365.  Los clústeres actúan ahora y la evaluación debe ser de destino, ya que producirán un mayor rendimiento.  Cultivar y educar a los clientes solo deben tener como destino si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes.|
|Programa de licencias|   Esto identifica el tipo de programa de licencias para la renovación.|
|Identificador del acuerdo|  Identificador del acuerdo|
|Fecha de finalización del contrato|    Fecha de finalización del contrato |
|Tipo de caducidad|   Tipo de expiración|
|Ingresos que van a expirar|  Ingresos asociados a las suscripciones que han expirado|
|Tiene EA|    Esto identifica si una renovación es un contrato Enterprise (EA) o una suscripción de EA|
|Tiene abierto|  Esto identifica si una renovación es un acuerdo de valor abierto o abierto.|
|Cliente de ventas de Azure| Esto identifica si el cliente muestra una propens de venta incremental para Azure|
|Cliente de ventas de M365|  Esto identifica si el cliente muestra la propens de venta incremental para M365|
|RevSumDivisionName|    Esto identifica el producto que está activo para la renovación.|

## <a name="next-steps"></a>Pasos siguientes

Para obtener informes, consulte [Descargar informes](pci-download-reports.md).
