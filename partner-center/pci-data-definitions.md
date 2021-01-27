---
title: Definiciones de datos de Insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: En el documento se muestran varios informes y sus definiciones de datos, que puede descargar en la página del informe de descarga de Insights.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 427ca3b60ec527a6a371a232538647448d03b084
ms.sourcegitcommit: 6632d7452be36010bfc8c6823efe5a5197377989
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/27/2021
ms.locfileid: "98861400"
---
# <a name="export--data-definitions"></a>Exportar: definiciones de datos 

 **Roles adecuados** 

- Visor de informes 
- Visor de informes ejecutivos 

## <a name="introduction"></a>Introducción 

Mediante el uso del centro de descarga de informes en el panel de Insights, puede exportar los conjuntos de información sin procesar. 

Los distintos informes, que puede descargar junto con sus definiciones de datos, se enumeran en las tablas siguientes: 

### <a name="partner-profile-report"></a>**Informe de Perfil de socio comercial**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| MPNId | Identificador de Microsoft Partner Network (MPN) | 
| PartnerName | Nombre del socio comercial | 
| PGA_MPNId | Identificador de la cuenta global de socio MPN | 
| PGA_PartnerName | Nombre de cuenta global de socio comercial | 
| City (Ciudad) | Ubicación de la ciudad del socio comercial | 
| Country (País) | Ubicación del país del socio comercial | 
| HierarchyLevel | Indica si es un identificador de MPN global o un identificador de MPN de ubicación | 

### <a name="customer-details-report"></a>**Informe de detalles del cliente**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CustomerName | Nombre del cliente | 
| CustomerTenantId | Identificador del inquilino del cliente | 
| CustomerTpid | Identificador del cliente primario superior | 
| CustomerSegment | Segmento de cliente | 
| CustomerMarket | Mercado geográfico del cliente | 
| CustomerStatus | Estado del cliente (activo o inactivo) | 
| Producto | El producto se vende al cliente mediante MPN: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI o Microsoft Azure | 
| SKU | SKU de producto | 
| Month (Mes) | Mes para el que se ha comunicado el uso y los ingresos | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nombre del socio comercial | 
| PartnerLocation | Ubicación geográfica del socio | 
| PartnerAttributionType | Tipo de atribución del asociado | 
| SalesChannel | Canal de ventas | 
| AvailableSeats | Puestos disponibles | 
| RevenueUSD | Ingresos en dólares estadounidenses | 

### <a name="reseller-performance-report"></a>**Informe de rendimiento del reseller**

> [!Note]
> Los datos de ingresos y ACR solo están disponibles para los usuarios que son ejecutivos de informes.

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| ResellerMPNid | Identificador de Microsoft Partner Network reseller | 
| ResellerName | Nombre del revendedor. | 
| ResellerMarket | País Reseller de Market | 
| IndirectProviderMPNId | Identificador del proveedor indirecto Microsoft Partner Network | 
| IndirectProviderName | Nombre de proveedor indirecto | 
| Month (Mes) | Mes para el que se ha comunicado el uso y los ingresos | 
| Producto | Nombre de producto | 
| SubscriptionID | Identificador de la suscripción | 
| AvailableSeats | Número de puestos disponibles | 
| AssignedSeats | Número de puestos asignados | 
| BilledRevenueUSD | Ingresos facturados en dólares estadounidenses | 
| CustomerName | Nombre del cliente | 
| CustomerTPid | Identificador del cliente primario superior | 
| CustomerSegment | Segmento de cliente | 
| CustomerMarket | Mercado geográfico del cliente | 
| ResellerStatus | Estado del distribuidor | 

### <a name="subscription-details-report"></a>**Informe de detalles de la suscripción**

>[!Note]
>Los datos de ingresos y ACR solo están disponibles para los usuarios que son ejecutivos de informes.

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| SubscriptionId | GUID de la suscripción | 
| SubscriptionStartDate | Fecha de inicio de la suscripción | 
| SubscriptionEndDate | Fecha de finalización de la suscripción | 
| SubscriptionState | Estado de la suscripción (activo o reactivado) | 
| Month (Mes) | Mes para el que se ha comunicado el uso y los ingresos | 
| IsAutoRenew | Indica si la suscripción se renueva (sí o no) | 
| CustomerName | Nombre del cliente | 
| CustomerTenantId | GUID del cliente | 
| CustomerTpid | Identificador primario del cliente superior | 
| CustomerSegment | Segmento de mercado del cliente | 
| CustomerMarket | Mercado geográfico del cliente | 
| Producto | Producto vendido al cliente por el asociado | 
| SKU | SKU del producto | 
| MPNId | IDENTIFICADOR Microsoft Partner Network del socio comercial | 
| PartnerName | Nombre del socio comercial | 
| PartnerLocation | Ubicación geográfica del socio | 
| PartnerAttributionType | Tipo de atribución para la suscripción | 
| SalesChannel | Canal de ventas directas, CSP (proveedor de soluciones en la nube), etc. | 
| AvailableSeats | Puesto disponible actualmente | 
| RevenueUSD | Ingresos en dólares estadounidenses | 
| ID. de inscripción | IDENTIFICADOR de inscripción de la suscripción | 

### <a name="azure-usage-report"></a>**Informe de uso de Azure**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| SubscriptionId | GUID de la suscripción | 
| SubscriptionStartDate | Fecha del inicio de la suscripción. | 
| SubscriptionEndDate | La fecha de finalización de la suscripción | 
| SubscriptionState | Estado actual de la suscripción (abierto, cerrado, activo o en período de gracia) | 
| Month (Mes) | Fecha de agregación por mes | 
| ServiceName | Nombre del servicio de Azure | 
| MeterCategory | Nombre de la categoría de medidor | 
| UsageUnits | El número de unidades que se usan durante el ciclo de facturación | 
| CustomerName | Nombre del cliente | 
| CustomerTenantId | IDENTIFICADOR de inquilino del cliente | 
| CustomerTpid | IDENTIFICADOR primario del cliente superior | 
| CustomerSegment | Segmento del cliente | 
| CustomerMarket | Mercado geográfico del cliente | 
| MPNId | IDENTIFICADOR Microsoft Partner Network del cliente | 
| PartnerName | Nombre del socio comercial | 
| PartnerLocation | Ubicación geográfica del país del socio | 
| PartnerAttributionType | Tipo de atribución del asociado | 
| SalesChannel | Canal de las ventas (directo/CSP, indirecto/CSP, directo, etc.) | 
| ACR_USD | Ingresos consumidos por Azure (ACR) en dólares estadounidenses | 
| ID. de inscripción | IDENTIFICADOR de inscripción de la suscripción de Azure | 

### <a name="office-365-license-usage-report"></a>**Informe de uso de licencias de Office 365**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CustomerTenantId | IDENTIFICADOR de inquilino del cliente | 
| CustomerTpid | IDENTIFICADOR primario del cliente superior | 
| WorkloadName | Skype empresarial, equipos y Exchange Online | 
| Month (Mes) | Mes en el que se ha comunicado el uso | 
| PaidAvailableUnits | Número de unidades disponibles de pago | 
| MonthlyActiveUsers | Número de usuarios activos al mes | 
| CustomerName | Nombre del cliente | 
| CustomerMarket | Ubicación geográfica del país del mercado del cliente | 
| CustomerSegment | Segmento de cliente | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nombre del socio comercial | 
| PartnerLocation | Ubicación geográfica del socio | 
| PartnerAttributionType | Tipo de atribución del asociado | 

### <a name="enterprise-mobility-license-usage-report"></a>**Informe de uso de licencias de Enterprise Mobility**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CustomerTenantId | IDENTIFICADOR de inquilino del cliente | 
| CustomerTpid | IDENTIFICADOR primario del cliente superior | 
| WorkloadName | Nombre de la carga de trabajo de Enterprise Mobility + Security (EMS) | 
| Month (Mes) | Mes en el que se ha comunicado el uso | 
| PaidAvailableUnits | Número de unidades disponibles de pago | 
| MonthlyActiveUsers | Número de usuarios activos al mes | 
| CustomerName | Nombre del cliente | 
| CustomerMarket | Ubicación geográfica del país del mercado del cliente | 
| CustomerSegment | Segmento de cliente | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nombre del socio comercial | 
| PartnerLocation | Ubicación geográfica del socio | 
| PartnerAttributionType | Tipo de atribución del asociado | 

### <a name="dynamics-365-license-usage-report"></a>**Informe de uso de licencias de Dynamics 365**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| SubscriptionId | GUID de la suscripción | 
| SubscriptionStartDate | Fecha de inicio de la suscripción | 
| SubscriptionEndDate | Fecha de finalización de la suscripción | 
| SubscriptionStatus | Estado de la suscripción | 
| Month (Mes) | Mes en el que se ha comunicado el uso | 
| RevSumDivisionName | Nombre de la división de la suma de Rev | 
| RevSumCategoryName | Nombre de la categoría de la suma de Rev. | 
| SKU | SKU del producto | 
| SKUId | IDENTIFICADOR de SKU del producto | 
| FreeVsPaidSKU | Indica si se trata de una SKU gratuita o de pago | 
| SalesModel | Canal de ventas que se usa para vender la suscripción | 
| DetailedSalesModel | Modelo de ventas detallado para la suscripción | 
| CustomerName | Nombre del cliente | 
| CustomerTenantId | GUID del inquilino del cliente | 
| CustomerTpid | Identificador primario del cliente superior | 
| CustomerSegment | Segmento de mercado del cliente | 
| CustomerMarket | Mercado geográfico del cliente | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nombre del socio comercial | 
| PartnerLocation | Ubicación geográfica del país del socio | 
| PartnerAttachType | Tipo de atribución para la suscripción | 
| AvailableSeats | Puesto disponible actualmente | 
| AssignedSeats | Puesto asignado actual | 
| ActiveSeats | Puestos activos actuales | 
| DeploymentOpportunity | Oportunidad de implementación actual | 
| ActiveUsagePercent | Porcentaje de uso activo actual | 

### <a name="power-bi-license-usage-report"></a>**Power BI informe de uso de licencias**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| SubscriptionId | GUID de la suscripción | 
| SubscriptionStartDate | Fecha de inicio de la suscripción | 
| SubscriptionEndDate | Fecha de finalización de la suscripción | 
| SubscriptionStatus | Estado de la suscripción (activo, inactivo o en período de gracia) | 
| Month (Mes) | Fecha de agregación por mes | 
| SKU | SKU del producto | 
| SKUId | IDENTIFICADOR de SKU del producto | 
| FreeVsPaidSKU | Diferenciación de SKU gratis o de pago | 
| SalesModel | Modelo de ventas que se usa para vender la suscripción | 
| DetailedSalesModel | Modelo de ventas detallado para la suscripción | 
| CustomerName | Nombre del cliente | 
| CustomerTenantId | GUID del inquilino del cliente | 
| CustomerTpid | Identificador del cliente primario superior | 
| CustomerSegment | Segmento de mercado del cliente | 
| CustomerMarket | Mercado geográfico del cliente | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nombre del socio comercial | 
| PartnerLocation | Ubicación geográfica del país del socio | 
| PartnerAttachType | Tipo de atribución para la suscripción | 
| AvailableSeats | Puestos disponibles actualmente | 
| AssignedSeats | Puestos asignados actuales | 
| ActiveSeats | Puestos activos actuales | 
| DeploymentOpportunity | Oportunidad de implementación actual | 
| ActiveUsagePercent | Porcentaje de uso activo actual | 

### <a name="teams-meetings-and-calls-report"></a>**Informe de reuniones y llamadas de equipos**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CustomerTenantId | IDENTIFICADOR de inquilino del cliente | 
| CustomerTpid | Identificador del cliente primario superior | 
| Month (Mes) | Mes en el que se ha comunicado el uso | 
| Subcarga de trabajo | Subcarga de trabajo para el que se ha comunicado el uso (reuniones, llamadas o sistemas telefónicos) | 
| Recuento de reuniones | Número de reuniones | 
| Duración de la reunión | Duración total de la reunión en horas | 

### <a name="teams-monthly-usage-report"></a>**Informe de uso mensual de equipos**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CustomerTenantId | IDENTIFICADOR de inquilino del cliente | 
| CustomerTpid | Identificador del cliente primario superior | 
| Month (Mes) | Mes en el que se ha comunicado el uso | 
| Subcarga de trabajo | Subcarga de trabajo para el que se ha comunicado el uso (reuniones, llamadas o sistemas telefónicos) | 
| Usuarios de escritorio | Número de usuarios que usan equipos en el escritorio | 
| Usuarios móviles | Número de usuarios que usan equipos en móvil | 
| Usuarios Web | Número de usuarios que usan equipos en la web | 
| AllUpParticipants | Número de usuarios únicos de equipos durante el mes | 

### <a name="teams-usage-3p-apps-report"></a>**Informe de aplicaciones 3P de uso de equipos**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CustomerTenantId | IDENTIFICADOR de inquilino del cliente | 
| CustomerTpid | IDENTIFICADOR primario del cliente superior | 
| Month (Mes) | Mes en el que se ha comunicado el uso | 
| Nombre de la aplicación 3P | Nombre de la aplicación Teams | 
| Número de usuarios | Número de usuarios de la aplicación | 


### <a name="training-details-report"></a>**Informe de detalles de aprendizaje**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| TrainingActivityId | Identificador del entrenamiento | 
| TrainingTitle | Título del entrenamiento | 
| TrainingType | Tipo de entrenamiento (certificación o examen) | 
| IndividualFirstName | Nombre del cliente | 
| IndividualLastName | Apellido del cliente | 
| Correo electrónico | IDENTIFICADOR de correo electrónico personal del cliente | 
| CorpEmail | IDENTIFICADOR de correo electrónico de Office del cliente | 
| TrainingCompletionDate | Fecha de finalización del entrenamiento | 
| Month (Mes) | Mes para el que se envían los datos | 
| IcMCP | Indica si el usuario es Microsoft Certified Professional (MCP) | 
| MCPID | IDENTIFICADOR de MCP del usuario | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nombre del socio comercial | 
| PartnerCityLocation | Ubicación geográfica de la ciudad del socio | 
| PartnerCountryLocation | Ubicación geográfica del país del socio | 

### <a name="microsoft-learn-report"></a>**Microsoft Learn informe**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| UserName | Nombre del usuario | 
| UserId | GUID del usuario | 
| TrainingName | Nombre del entrenamiento | 
| TrainingType | Tipo de entrenamiento (módulo o ruta de aprendizaje) | 
| Productos | Producto para el que se aplica el módulo de aprendizaje | 
| Roles | Roles aplicables del entrenamiento | 
| CompletionDate | Fecha de finalización del entrenamiento | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nombre del socio comercial | 
| Country (País) | Ubicación geográfica del país del socio | 

### <a name="competency-summary-and-history-report"></a>**Informe de Resumen y historial de competencias**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CompetencyName | Nombre de la competencia | 
| CompetencyLevel | Nivel de competencia (Gold o Silver) | 
| CompetencyStatus | Estado actual de la competencia (activo, inactivo o en período de gracia) | 
| CompetencyStartDate | Fecha de inicio de la competencia | 
| CompetencyEndDate | Fecha de finalización de la competencia | 

### <a name="competency-performance-report"></a>**Informe de rendimiento de la competencia**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CompetencyName | Nombre de la competencia | 
| CompetencyAttainmentOptionName | Nombre de la opción de obtención de aptitudes | 
| Month (Mes) | Mes para el que se registran las métricas | 
| MetricName | Nombre de la métrica que es relevante para la competencia | 
| MetricMonthlyContribution | Contribución mensual de la métrica | 
| TTMAggregate | Métrica agregada para los 12 meses finales | 
| AnniversaryYearAggregate | Métrica agregada para el año de aniversario actual | 
| GoldThreshold | Requisitos de rendimiento para satisfacer la competencia Gold | 
| SilverThreshold | Requisitos de rendimiento para satisfacer la competencia Silver | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Microsoft 365 informe de propens de la nube**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| Identificador de MPN | IDENTIFICADOR de Microsoft Partner Network | 
| Nombre del asociado | Nombre del socio comercial | 
| Customer ID | Número de identificación del cliente | 
| Número DUNS | El número de Dun & Bradstreet (D&B) del cliente que se está puntuando para la propens | 
| Nombre de cuenta | Nombre de la cuenta | 
| Domain | Dominio de la cuenta | 
| Tamaño de la organización | Tamaño de la organización | 
| Sector | Sector al que pertenece la organización | 
| Vertical | El vertical del cliente que se está puntuando para la propens, tal y como lo identifica Microsoft, D&B y otros estándares del sector. | 
| Área | Área geográfica de la ubicación | 
| Subsidiaria | La subsidiaria del cliente que se está puntuando para la propens | 
| Territorio de ventas | Territorio de ventas del cliente que se está puntuando para la propens | 
| City (Ciudad) | Ubicación geográfica de la ciudad de la organización | 
| State | Ubicación geográfica del estado de la organización | 
| Código postal | Código postal de la organización | 
| Country (País) | Ubicación geográfica del país de la organización | 
| Segment | Segmento de mercado | 
| Subsegmento | Subsegmento de mercado | 
| Resumen de tipo de SMC | Tipo de SMC | 
| Top no administrado: base de proceso | Principales clientes no administrados: proceso | 
| Base de usuario no administrada superior | Principales clientes no administrados: usuario | 
| IsNonProfit | Indica si la organización no es de lucro (sí o no) | 
| Habilitar el destino remoto en Exchange Online | Clientes que tienen una suscripción activa a Exchange Online, que se venden en Microsoft 365 | 
| Habilitar la adquisición remota de trabajo local (versión actual) con la propens de ascenso de la nube-+ 10 licencias | Cliente que tiene un cliente de Office o Windows local actual. Es decir, la versión del cliente es posterior a una versión de final de ciclo de vida (EOL). El cliente tiene 10 o más licencias. Cliente que tiene una puntuación de propens. El asociado debe tener como destino la conversión a Microsoft 365. | 
| Habilitar la adquisición remota de trabajo local (versión actual) con propens de ascenso de la nube-<10 licencias | Cliente que tiene un cliente de Office o Windows local actual (es decir, una versión posterior a la EOL). El cliente tiene menos de 10 licencias. Cliente que tiene una puntuación de propens. El asociado debe tener como destino la conversión a Microsoft 365. | 
| Habilitar la adquisición remota de trabajo local (versión actual) sin propens de ascenso de nube-+ 10 licencias | Cliente que tiene un cliente de Office o Windows local actual (es decir, una versión posterior a la EOL). El cliente tiene 10 o más licencias. El cliente no tiene una puntuación de propens. El asociado debe tener como destino la conversión a Microsoft 365. | 
| Habilitar la adquisición remota de trabajo local (versión actual) sin propens de ascenso de nube-<10 licencias | Cliente que tiene un cliente de Office o Windows local actual (es decir, una versión posterior a la EOL). El cliente tiene menos de 10 licencias. El cliente no tiene una puntuación de propens. El asociado debe tener como destino la conversión a Microsoft 365. | 
| Habilitar la adquisición remota de trabajo local (versión EOL) con la propens de ascenso de la nube-+ 10 licencias | Cliente que tiene un cliente de Office o Windows local EOL (es decir, una versión EOL o anterior). El cliente tiene 10 o más licencias. El cliente tiene una puntuación de propens. El asociado debe tener como destino la conversión a Microsoft 365. | 
| Habilitación de la adquisición remota de trabajo local (versión EOL) con propens de ascenso de nube-<10 licencias | Cliente que tiene un cliente de Office o Windows local EOL (es decir, una versión EOL o anterior). El cliente tiene menos de 10 licencias. El cliente tiene una puntuación de propens. El asociado debe tener como destino la conversión a Microsoft 365. | 
| Habilitación de la adquisición remota de trabajo local (versión EOL) sin propens de ascenso de nube-+ 10 licencias | Cliente que tiene un cliente de Office o Windows local actual (es decir, una versión EOL o anterior). El cliente tiene 10 o más licencias. El cliente no tiene una puntuación de propens. El asociado debe tener como destino la conversión a Microsoft 365. | 
| Habilitar la adquisición remota de trabajo local (versión EOL) sin propens de ascenso de nube-<10 licencias | Cliente que tiene un cliente de Office o Windows local actual (es decir, una versión EOL o anterior). El cliente tiene menos de 10 licencias. El cliente no tiene una puntuación de propens. El asociado debe tener como destino la conversión a Microsoft 365. | 
| Habilitación del trabajo remoto: alto de propens para Microsoft 365 (NowithEvaluate de Act) | Cliente potencial con alta propens para Microsoft 365 | 
| Habilitar trabajo remoto: compite (zoom) con Microsoft 365 | Cliente con zoom y Microsoft 365, destino para la conversión a equipos | 
| Habilitar trabajo remoto: competir (zoom) sin Microsoft 365 | Cliente con zoom, destino para la conversión a equipos | 
| Reduzca el costo y administre Microsoft 365 E3 orientado a Microsoft 365 E5 | Cliente existente con Microsoft 365 E3, dirigido a Microsoft 365 E5 | 
| Reduzca los costos y administre los clientes de Microsoft 365 Empresa Basic y Business Standard y el estándar de la empresa destinados a Microsoft 365 Empresa Premium | Clientes existentes Microsoft 365 Empresa Basic y Business Standard, dirigido a Microsoft 365 Empresa Premium | 
| Transformar la productividad de la organización: propens de superficie | El cliente muestra una propens para Surface | 
| M365Cluster | Identifica la propens de un cliente para adquirir Microsoft 365. Destino Act Now y evalúe los clústeres porque producirán un mayor rendimiento. Dirigirse a los clientes solo si todavía existe capacidad después de ACT Now y a evaluar los clientes de destino. | 
| M365Fit | Puntos de datos internos y externos que definen firmographics. La puntuación de ajuste usa un modelo de Lookalike a nuestras mejores empresas pequeñas o medianas (SMB) para comparar clientes y ver si son posibles para los productos en la nube de Microsoft. La puntuación de ajuste se actualiza trimestralmente. | 
| M365Intent | Las señales relacionadas con los medios sociales y el comportamiento en línea de un cliente definen el intento. La puntuación de intención se superpone al ajuste para definir los clústeres. La puntuación de intención se actualiza mensualmente. | 
| SurfaceCluster | Identifica la propens de un cliente para la superficie de compra mediante la consolidación de las recomendaciones de ajuste y intención en un clúster. Destino Act Now y evalúe los clústeres porque producirán un mayor rendimiento. Dirigirse a los clientes solo si todavía existe capacidad después de ACT Now y a evaluar los clientes de destino. | 
| SurfaceFit | Puntos de datos internos y externos que definen firmographics. La puntuación de ajuste usa un modelo de Lookalike a nuestras mejores SMB para comparar a los clientes y ver si son posibles para los productos en la nube de Microsoft. La puntuación de ajuste se actualiza trimestralmente. | 
| SurfaceIntent | Las señales relacionadas con los medios sociales y el comportamiento en línea de un cliente definen el intento. La puntuación de intención se superpone al ajuste para definir los clústeres. La puntuación de intención se actualiza mensualmente. | 
| O365Cluster | Identifica la propens del cliente para comprar Office 365. Destino Act Now y evalúe los clústeres porque producirán un mayor rendimiento. Dirigirse a los clientes solo si todavía existe capacidad después de ACT Now y a evaluar los clientes de destino. | 
| O365Fit | Puntos de datos internos y externos que definen firmographics. La puntuación de ajuste usa un modelo de Lookalike a nuestras mejores SMB para comparar a los clientes y ver si son posibles para los productos en la nube de Microsoft. La puntuación de ajuste se actualiza trimestralmente. | 
| O365Intent | Las señales relacionadas con los medios sociales y el comportamiento en línea de un cliente definen el intento. La puntuación de intención se superpone al ajuste para definir los clústeres. La puntuación de intención se actualiza mensualmente. | 
| M365UpsellCustomer | Identifica si el cliente muestra la propens de venta incremental para Microsoft 365 | 
| Tiene Google | Identifica si el cliente muestra señales competitivas para los productos de Google de propiedad. | 
| Tiene AWS | Identifica si el cliente muestra señales competitivas para productos de Amazon Web Services propietarios (AWS). | 
| Tiene EA | Identifica si una renovación es un contrato Enterprise (EA) o una suscripción de EA | 
| Tiene abierto | Identifica si una renovación es un acuerdo de valor abierto o abierto. | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Ascenso de la nube: informe de propens de Dynamics 365**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| Identificador de MPN | IDENTIFICADOR de Microsoft Partner Network | 
| Nombre del asociado | Nombre del socio comercial | 
| Customer ID | Número de identificación del cliente | 
| Número DUNS | El número de Dun & Bradstreet del cliente que se está puntuando para la propens | 
| Nombre de cuenta | Nombre de la cuenta | 
| Domain | Dominio de la cuenta | 
| Tamaño de la organización | Tamaño de la organización | 
| Sector | Sector al que pertenece la organización | 
| Vertical | El vertical del cliente que se está puntuando para la propens, tal y como lo identifica Microsoft, D&B y otros estándares del sector.
| Área | Área geográfica de la ubicación | 
| Subsidiaria | La subsidiaria del cliente que se está puntuando para la propens | 
| Territorio de ventas | Territorio de ventas del cliente que se está puntuando para la propens | 
| City (Ciudad) | Ubicación de la ciudad geográfica | 
| State | Ubicación geográfica del estado | 
| Código postal | Código postal de la organización | 
| Country (País) | Ubicación geográfica del país | 
| Segment | Segmento de mercado | 
| Subsegmento | Subsegmento de mercado | 
| Resumen de tipo de SMC | La categorización de un cliente: las principales bases de usuarios no administradas son clientes con más de 300 empleados, las principales bases de proceso no administradas son clientes con USD10, 000 en Azure con un potencial de tres años, las empresas medianas son clientes con 25 empleados o más, y las pequeñas empresas son clientes con menos de 25 empleados. | 
| Top no administrado: base de proceso | Principales clientes no administrados: proceso | 
| Base de usuario no administrada superior | Principales clientes no administrados: usuarios | 
| IsNonProfit | Indica si la organización no es de lucro (sí o no) | 
| Activar las ventas digitales: tamaño de Microsoft 365 puesto >= 25 puestos (modelo de propens de SalesPro) | Cliente sin Dynamics 365. Tamaño del puesto: 25 +. El asociado debe ser el destino de la venta cruzada de Dynamics 365 SalesPro. | 
| Activar la venta digital: SalesPro propens-Dynamics 365 (ACT Now or Evaluate) | Clientes de alta propens sin Dynamics 365. El asociado debe tener como destino Dynamics 365 SalesPro. | 
| Administración de riesgos financieros & fraude: base de instalación local de Dynamics-Navision (modelo de propens de Business central) | Cliente existente con Navision local. El asociado debe tener como destino Dynamics 365 Business central. | 
| Administración de riesgos financieros & fraude: base de instalación local de Dynamics AX (modelo de propens de Dynamics 365 Finance + operaciones) | Cliente existente con AX local. El asociado debe ser el destino de las operaciones financieras y de Dynamics 365. | 
| Administración de riesgos financieros & fraude: base de instalación local de Dynamics-Great Plains (modelo de propens de Business central) | Cliente existente con Great Plains local. El asociado debe tener como destino Dynamics 365 Business central. | 
| Administración de riesgos financieros & fraude: base de instalación local de Dynamics-Solomon (modelo de propens de Business central) | Cliente existente con Solomon local. El asociado debe tener como destino Dynamics 365 Business central. | 
| Administración de riesgos financieros & fraude-base de instalación local de Dynamics-otros (modelo de propens de Business central) | Cliente existente con otras soluciones locales no enumeradas anteriormente. El asociado debe tener como destino Dynamics 365 Business central. | 
| Creación de procesos empresariales ágiles: base de instalación local de Dynamics-AX/GP/SL/NAV/otros (modelo de propens de Dynamics 365) | Creación de procesos empresariales ágiles: base de instalación local de Dynamics-AX/GP/SL/NAV/otros (modelo de propens de Dynamics 365) | 
| Crear procesos empresariales ágiles: Dynamics compite base-Mendix/OutSystems/Salesforce (modelo de propens de Dynamics 365) | Crear procesos empresariales ágiles: Dynamics compite base-Mendix/OutSystems/Salesforce (modelo de propens de Dynamics 365) | 
| Crear procesos empresariales ágiles: Dynamics 365 Finance + Operations (base de instalación) | Clientes existentes de Dynamics 365 Finance + Operations. Asociado para dirigirse a Power apps. | 
| Creación de procesos empresariales ágiles: base de la instalación de Dynamics 365 Business central | Clientes existentes de Dynamics 365 Business central. Asociado para dirigirse a Power apps. | 
| Creación de procesos empresariales ágiles: base de instalación de Dynamics 365 Customer Engagement | Clientes existentes de Dynamics 365 Customer Engagement. Asociado para dirigirse a Power apps. | 
| Cree una cadena de suministro resistente: Windows y active la primera carga de trabajo de Dynamics 365 como administración de la cadena de suministro de Dynamics 365 con clientes que no sean de Oracle o SAP ERP (planeamiento de recursos empresariales) | Clientes de destino para la administración de la cadena de suministro de Dynamics 365 | 
| Creación de una cadena de suministro resistente: ventas cruzadas de administración de cadenas de suministro de Dynamics 365 y/o comercio minorista o comercial a clientes de Dynamics 365 Customer Engagement existentes | Clientes existentes de Dynamics 365 Customer Engagement para dirigirse a la administración de la cadena de suministro de Dynamics 365 de ventas cruzadas. | 
| Cree una cadena de suministro resistente: ventas cruzadas de Dynamics 365 administración de cadenas de suministro y/o comercio minorista o comercial a Dynamics 365 Customer Engagement y Oracle o SAP | Clientes existentes de Dynamics 365 Customer Engagement con Oracle o SAP como destino para la administración de la cadena de suministro de Dynamics 365 | 
| D365BCCluster | Identifica la propens del cliente para comprar Dynamics 365 Business central. Los clientes que muestren una propens for Business central estarán en las categorías medianas y pequeñas. Destino Act Now y evalúe los clústeres, ya que producirán un mayor rendimiento. Dirigirse a los clientes y educar solo si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes. | 
| D365BCFit | Puntos de datos internos y externos que definen firmographics. Ajustar puntuación usa un modelo de Lookalike a nuestro mejor SMB para comparar a los clientes y ver si son posibles para los productos en la nube de Microsoft. La puntuación de ajuste se actualiza trimestralmente. | 
| D365BCIntent | Las señales relacionadas con los medios sociales y el comportamiento en línea de un cliente definen el intento. La puntuación de intención se superpone al ajuste para definir los clústeres. La puntuación de intención se actualiza mensualmente. | 
| D365FOCluster | Identifica la propens del cliente para comprar Dynamics 365 Finance and Operations. Los clientes que muestren una propens for Finance + Operations estarán en las categorías principales no administradas. Destino Act Now y evalúe los clústeres, ya que producirán un mayor rendimiento. Dirigirse a los clientes y educar solo si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes. | 
| D365FOFit | Puntos de datos internos y externos que definen firmographics. Ajustar puntuación usa un modelo de Lookalike a nuestro mejor SMB para comparar a los clientes y ver si son posibles para los productos en la nube de Microsoft. La puntuación de ajuste se actualiza trimestralmente. | 
| D365FOIntent | Las señales relacionadas con los medios sociales y el comportamiento en línea de un cliente definen el intento. La puntuación de intención se superpone al ajuste para definir los clústeres. La puntuación de intención se actualiza mensualmente. | 
| D365CECluster | Identifica la propens del cliente para comprar Dynamics 365 Customer Engagement. Los clientes que muestren una propens para el compromiso de los clientes estarán en las categorías mediana y pequeña. Destino Act Now y evalúe los clústeres, ya que producirán un mayor rendimiento. Dirigirse a los clientes y educar solo si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes. | 
| D365CEFit | Indica el ajuste de Dynamics 365 Customer Engagement | 
| D365CEIntent | Indica la intención de Dynamics 365 Customer Engagement | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Identifica si el cliente tiene una renovación abierta para Dynamics on-premises AX o CRM | 
| M365UpsellCustomer | Identifica si el cliente muestra la propens de venta incremental para Microsoft 365 | 
| Tiene Google | Identifica si el cliente muestra señales competitivas para los productos de Google de propiedad. | 
| Tiene AWS | Identifica si el cliente muestra señales competitivas para productos AWS de propiedad. | 
| Tiene EA | Identifica si una renovación es una suscripción de EA o EA | 
| Tiene abierto | Identifica si una renovación es un acuerdo de valor abierto o abierto. | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Ascenso de nube: informe de propens de Azure**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| Identificador de MPN | IDENTIFICADOR de Microsoft Partner Network | 
| Nombre del asociado | Nombre del socio comercial | 
| Customer ID | Número de identificación del cliente | 
| Número DUNS | El número de Dun & Bradstreet del cliente que se está puntuando para la propens | 
| Nombre de cuenta | Nombre de la cuenta | 
| Domain | Dominio de la cuenta | 
| Tamaño de la organización | Tamaño de la organización | 
| Sector | Sector | 
| Vertical | El vertical del cliente que se está puntuando para la propens, tal y como lo identifica Microsoft, D&B y otros estándares del sector. | 
| Área | Área geográfica de la ubicación | 
| Subsidiaria | La subsidiaria del cliente que se está puntuando para la propens | 
| Territorio de ventas | Territorio de ventas del cliente que se está puntuando para la propens | 
| City (Ciudad) | Ubicación de la ciudad geográfica | 
| State | Ubicación geográfica del estado | 
| Código postal | Código postal de la organización | 
| Country (País) | Ubicación geográfica del país | 
| Segment | Segmento de mercado | 
| Subsegmento | Subsegmento de mercado | 
| Resumen de tipo de SMC | Tipo de SMC | 
| Top no administrado: base de proceso | Principales clientes no administrados: proceso | 
| Base de usuario no administrada superior | Principales clientes no administrados: usuarios | 
| IsNonProfit | Indica si la organización no es de lucro (sí o no) | 
| Migrar-EOL de Windows Server: EOL de Windows Server IB con propens de ascenso de la nube (más de 5 licencias) | Cliente que tiene un servidor de Windows local EOL (es decir, una versión EOL o anterior). El cliente tiene 5 o más licencias. Cliente que tiene una puntuación de propens. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar-EOL de Windows Server: EOL de Windows Server IB con propens de ascenso de la nube-<5 licencias | Cliente que tiene un servidor de Windows local EOL (es decir, una versión EOL o anterior). El cliente tiene menos de 5 licencias. Cliente que tiene una puntuación de propens. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar-EOL de Windows Server: EOL de Windows Server IB sin propens de ascenso de la nube-5 + licencias | Cliente que tiene un servidor de Windows local EOL (es decir, una versión EOL o anterior). El cliente tiene más de 5 licencias. El cliente no tiene una puntuación de propens. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar-EOL de Windows Server: EOL de Windows Server IB sin propens de ascenso de nube-<5 licencias | Cliente que tiene un servidor de Windows local EOL (es decir, una versión EOL o anterior). Tiene menos de 5 licencias. El cliente no tiene una puntuación de propens. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar-EOL SQL-EOL SQL Server IB con propens de ascenso de nube-5 licencias | Cliente que tiene un SQL Server de EOL local (es decir, una versión EOL o anterior). El cliente tiene más de 5 licencias. El cliente tiene una puntuación de propens. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar-EOL SQL-EOL SQL Server IB con propens de ascenso de nube-<5 licencias | Cliente que tiene un SQL Server de EOL local (es decir, una versión EOL o anterior). Tiene menos de 5 licencias. Cliente que tiene una puntuación de propens. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar-EOL SQL-EOL SQL Server IB sin propens de ascenso de nube-5 licencias | Cliente que tiene un SQL Server de EOL local (es decir, una versión EOL o anterior). El cliente tiene 5 o más licencias. El cliente no tiene una puntuación de propens. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar-EOL SQL-EOL SQL Server IB sin propens de ascenso de nube-<5 licencias | Cliente que tiene un SQL Server de EOL local (es decir, una versión EOL o anterior). El cliente tiene menos de 5 licencias. El cliente no tiene una puntuación de propens. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar: migrar Windows Server local: Windows Server IB actual con propensión de ascenso de la nube-5 + licencias | Cliente que tiene un servidor de Windows local actual (es decir, una versión posterior a la EOL). El cliente tiene más de 5 licencias. El cliente tiene una puntuación de propens. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar: migrar Windows Server local: Windows Server IB actual con propens de la nube-<5 licencias | Cliente que tiene un servidor de Windows local actual (es decir, una versión posterior a la EOL). El cliente tiene menos de 5 licencias. El cliente tiene una puntuación de propens de Azure. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar: migrar Windows Server local: Windows Server IB actual sin propens de ascenso de nube-5 + licencias | Cliente que tiene un servidor de Windows local actual (es decir, una versión posterior a la EOL). El cliente tiene más de 5 licencias. El cliente no tiene una puntuación de propens. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar: migrar Windows Server local: Windows Server IB actual sin propens de ascenso de nube-<5 licencias | Cliente que tiene un servidor de Windows local actual (es decir, una versión posterior a la EOL). El cliente tiene menos de 5 licencias. El cliente no tiene una puntuación de propens. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar-migrar a Azure SQL o máquinas virtuales SQL (VM): actual SQL Server IB con propens de ascenso de nube-5 + licencias | Cliente que tiene una SQL Server local actual (es decir, una versión posterior a la EOL). El cliente tiene más de 5 licencias. El cliente tiene una puntuación de propens. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar: migrar a Azure SQL o a máquinas virtuales de SQL: actual SQL Server IB con propens-<5 de Cloud Ascent | Cliente que tiene una SQL Server local actual (es decir, una versión posterior a la EOL). El cliente tiene menos de 5 licencias. El cliente tiene una puntuación de propens. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar-migrar a Azure SQL o a máquinas virtuales de SQL: actual SQL Server IB sin propens de ascenso de nube-5 + licencias | Cliente que tiene una SQL Server local actual (es decir, una versión posterior a la EOL). El cliente tiene más de 5 licencias. El cliente no tiene una puntuación de propens. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar-migrar a Azure SQL o a máquinas virtuales de SQL: actual SQL Server IB sin propens de ascenso de nube-<5 licencias | Cliente que tiene una SQL Server local actual (es decir, una versión posterior a la EOL). El cliente tiene menos de 5 licencias. El cliente no tiene una puntuación de propens. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar-OSS-migrar a la base de Shakespeare de código abierto (OSS) | Cliente existente con cualquiera de los siguientes productos de la competencia: PostgreSQL, MySQL, MariaDB. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración-OSS-Linux en Azure | Cliente existente con Linux. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración de SAP-SAP en Azure | Cliente existente con SAP. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar: escritorio virtual de Windows-Servicios de Escritorio remoto IB | Identifica a los clientes con Windows Servicios de Escritorio remoto activos. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración: escritorio virtual de Windows-trabajo moderno de venta cruzada para Azure/WVD | Identifica a los clientes con Microsoft 365 y no tiene Azure. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar: VMware IB | Cliente existente con el producto: VMware. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar: Citrix IB | Cliente existente con el producto: Citrix Systems. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Innovate-Analytics-Power BI IB con alta propens de Azure | Los clientes con y la suscripción de Power BI activa incluyen: Power BI-independiente Pro, Power BI: conjuntos de Azure, conjuntos de Power BI-Office, Power BI Suites-Microsoft 365 | 
| Enable-DevOps con GitHub-Visual Studio/MSDN IB | Identifica a los clientes con versiones activas de Visual Studio | 
| Versión de Windows Server Standard | Muestra la versión de compras estándar de Windows Server por parte del cliente | 
| Licencia de Windows Server Standard | Muestra el tipo de licencia de compras de Windows Server Standard realizadas por el cliente | 
| Versión del centro de datos de Windows Server | Muestra la versión de compras del centro de datos de Windows por parte del cliente | 
| Licencia del centro de datos de Windows Server | Muestra el tipo de licencia de compras del centro de datos de Windows por parte del cliente | 
| AzureFit | Puntos de datos internos y externos que definen firmographics. Ajustar puntuación usa un modelo de Lookalike a nuestro mejor SMB para comparar a los clientes y ver si son posibles para los productos en la nube de Microsoft. La puntuación de ajuste se actualiza trimestralmente. | 
| AzureIntent | Las señales relacionadas con los medios sociales y el comportamiento en línea de un cliente definen el intento. La puntuación de intención se superpone al ajuste para definir los clústeres. La puntuación de intención se actualiza mensualmente. | 
| AzureCluster | Identifica la propens del cliente para adquirir Azure mediante la consolidación de las recomendaciones de ajuste y intención en un clúster. Destino Act Now y evalúe los clústeres, ya que producirán un mayor rendimiento. Dirigirse a los clientes y educar solo si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes. | 
| WindowsServerDataCenter_HasOpenRenewal | Identifica si el cliente tiene una renovación abierta para Windows Server Datacenter | 
| WindowsServerStandard_HasOpenRenewal | Identifica si el cliente tiene una renovación abierta para Windows Server Standard | 
| AzureUpsellCustomer | Identifica si el cliente muestra una propens de venta incremental para Azure | 
| Tiene Google | Identifica si el cliente muestra señales competitivas para los productos de Google de propiedad. | 
| Tiene AWS | Identifica si el cliente muestra señales competitivas para productos AWS de propiedad. | 
| Tiene EA | Identifica si una renovación es una suscripción de EA o EA | 
| Tiene abierto | Identifica si una renovación es un acuerdo de valor abierto o abierto. | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Informe de propens de renovación de acuerdo-ascenso de nube**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| Identificador de MPN | IDENTIFICADOR de Microsoft Partner Network | 
| Nombre del asociado | Nombre del socio comercial | 
| Customer ID | Número de identificación del cliente | 
| Número DUNS | El número de Dun & Bradstreet del cliente que se está puntuando para la propens | 
| Nombre de cuenta | Nombre de la cuenta | 
| Domain | Dominio de la cuenta | 
| Tamaño de la organización | Tamaño de la organización | 
| Sector | Sector | 
| Vertical | El vertical del cliente que se está puntuando para la propens, tal y como lo identifica Microsoft, D&B y otros estándares del sector. | 
| Área | Área geográfica de la ubicación | 
| Subsidiaria | La subsidiaria del cliente que se está puntuando para la propens | 
| Territorio de ventas | Territorio de ventas del cliente que se está puntuando para la propens | 
| City (Ciudad) | Ubicación de la ciudad geográfica | 
| State | Ubicación geográfica del estado | 
| Código postal | Código postal de la organización | 
| Country (País) | Ubicación geográfica del país | 
| Segment | Segmento de mercado | 
| Subsegmento | Subsegmento de mercado | 
| Resumen de tipo de SMC | Tipo de SMC | 
| Top no administrado: base de proceso | Principales clientes no administrados: proceso | 
| Base de usuario no administrada superior | Principales clientes no administrados: usuarios | 
| IsNonProfit | Indica si la organización no es de lucro (sí o no) | 
| Tiene Google | Identifica si el cliente muestra señales competitivas para productos AWS de propiedad. | 
| Tiene AWS | Identifica si el cliente muestra señales competitivas para productos AWS de propiedad. | 
| Clúster de Azure | Identifica la propens del cliente para comprar Azure. Destino Act Now y evalúe los clústeres, ya que producirán un mayor rendimiento. Dirigirse a los clientes y educar solo si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes. | 
| D365 el clúster de operaciones y finanzas | Identifica la propens del cliente para comprar Dynamics 365 Finance and Operations. Los clientes que muestren una propens for Finance + Operations estarán en las categorías principales no administradas. Destino Act Now y evalúe los clústeres, ya que producirán un mayor rendimiento. Dirigirse a los clientes y educar solo si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes. | 
| Clúster de D365 CE | Identifica la propens del cliente para comprar Dynamics 365 Customer Engagement. Los clientes que muestren una propens para el compromiso de los clientes estarán en las categorías mediana y pequeña. Destino Act Now y evalúe los clústeres, ya que producirán un mayor rendimiento. Dirigirse a los clientes y educar solo si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes. | 
| Clúster de BC de D365 | Identifica la propens del cliente para comprar Dynamics 365 Business central. Los clientes que muestren una propens for Business central estarán en las categorías medianas y pequeñas. Destino Act Now y evalúe los clústeres, ya que producirán un mayor rendimiento. Dirigirse a los clientes y educar solo si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes. | 
| Clúster de Microsoft 365 | Identifica la propens del cliente para comprar Microsoft 365. Destino Act Now y evalúe los clústeres, ya que producirán un mayor rendimiento. Dirigirse a los clientes y educar solo si todavía existe capacidad después de dirigirse a Act Now y evaluar a los clientes. | 
| Programa de licencias | Identifica el tipo de programa de licencias para la renovación. | 
| Identificador del acuerdo | Identificador del acuerdo | 
| Fecha de finalización del contrato | Fecha de finalización del acuerdo | 
| Tipo de caducidad | Tipo de expiración | 
| Ingresos que van a expirar | Ingresos asociados a las suscripciones que han expirado | 
| Tiene EA | Identifica si una renovación es una suscripción de EA o EA | 
| Tiene abierto | Identifica si una renovación es un acuerdo de valor abierto o abierto. | 
| Cliente de ventas de Azure | Identifica si el cliente muestra una propens de venta incremental para Azure | 
| Microsoft 365 cliente de ventas | Identifica si el cliente muestra la propens de venta incremental para Microsoft 365 | 
| RevSumDivisionName | Identifica el producto que se va a renovar. | 

## <a name="next-steps"></a>Pasos siguientes

Para obtener más información, vea [Descargar informes](pci-download-reports.md).
