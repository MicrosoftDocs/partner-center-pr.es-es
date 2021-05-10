---
title: Definiciones de datos de Insights
ms.topic: article
ms.date: 12/14/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: En el documento se enumeran varios informes y sus definiciones de datos, que puede descargar desde la página del informe de descarga de Insights.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21be5b22c453174fcb66e9409d6e26dad8e25c6b
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686354"
---
# <a name="export--data-definitions"></a>Exportar: definiciones de datos 

**Roles adecuados** 

- Visor de informes
- Visor de informes ejecutivos

## <a name="introduction"></a>Introducción 

Mediante el centro descargar informes en el panel de Insights, puede exportar los conjuntos de datos sin procesar. 

Los distintos informes, que puede descargar junto con sus definiciones de datos, se enumeran en las tablas siguientes: 

### <a name="partner-profile-report"></a>**Informe de perfil de asociado**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| MPNId | Identificador de Microsoft Partner Network (MPN) | 
| PartnerName | Nombre del asociado | 
| PGA_MPNId | Identificador del MPN de la cuenta global del asociado | 
| PGA_PartnerName | Nombre de cuenta global del asociado | 
| City | Ubicación de ciudad del asociado | 
| País | Ubicación del país del asociado | 
| HierarchyLevel | Indica si es un identificador de MPN global o un identificador de MPN de ubicación. | 

### <a name="customer-details-report"></a>**Informe de detalles del cliente**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CustomerName | Nombre del cliente | 
| CustomerTenantId | Identificador del inquilino del cliente | 
| CustomerTpid | Identificador del elemento primario principal del cliente | 
| CustomerSegment | Segmento de cliente | 
| CustomerMarket | Mercado geográfico del cliente | 
| CustomerStatus | Estado del cliente (activo o inactivo) | 
| Producto | Producto vendido al cliente por MPN: O365, DYNAMICS 365, Enterprise Mobility + Security, Power BI o Microsoft Azure | 
| SKU | SKU de producto | 
| Mes | Mes para el que se notifican el uso y los ingresos | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nombre del asociado | 
| PartnerLocation | Ubicación geográfica del asociado | 
| PartnerAttributionType | Tipo de atribución del asociado | 
| SalesChannel | Canal de ventas | 
| AvailableSeats | Puestos disponibles | 
| IngresosUSD | Ingresos en dólares estadounidenses | 

### <a name="reseller-performance-report"></a>**Informe de rendimiento del revendedor**

> [!Note]
> Los datos de ingresos y ACR solo están disponibles para los usuarios que son visores de informes ejecutivos.

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| ResellerMPNid | Identificador de Microsoft Partner Network distribuidor | 
| ResellerName | Nombre del revendedor. | 
| ResellerMarket | País de distribuidor del mercado | 
| IndirectProviderMPNId | Identificador del proveedor indirecto Microsoft Partner Network | 
| IndirectProviderName | Nombre del proveedor indirecto | 
| Mes | Mes para el que se notifica el uso y los ingresos | 
| Producto | Nombre de producto | 
| SubscriptionID | Identificador de la suscripción | 
| AvailableSeats | Número de puestos disponibles | 
| AssignedSeats | Número de puestos asignados | 
| BilledRevenueUSD | Ingresos facturados en dólares estadounidenses | 
| CustomerName | Nombre del cliente | 
| CustomerTPid | Identificador del elemento primario principal del cliente | 
| CustomerSegment | Segmento de cliente | 
| CustomerMarket | Mercado geográfico del cliente | 
| ResellerStatus | Estado del revendedor | 

### <a name="subscription-details-report"></a>**Informe de detalles de la suscripción**

>[!Note]
>Los ingresos y los datos de ACR solo están disponibles para los usuarios que son visores de informes ejecutivos.

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| SubscriptionId | GUID de la suscripción | 
| SubscriptionStartDate | Fecha de inicio de la suscripción | 
| SubscriptionEndDate | Fecha de finalización de la suscripción | 
| SubscriptionState | Estado de la suscripción (activo o renovación) | 
| Mes | Mes para el que se notifican el uso y los ingresos | 
| IsAutoRenew | Indica si la suscripción es automáticanuevo (Sí o No) | 
| CustomerName | Nombre del cliente | 
| CustomerTenantId | GUID del cliente | 
| CustomerTpid | Identificador primario principal del cliente | 
| CustomerSegment | Segmento de mercado del cliente | 
| CustomerMarket | Mercado geográfico del cliente | 
| Producto | Producto vendido al cliente por el asociado | 
| SKU | SKU del producto | 
| MPNId | Microsoft Partner Network identificador del asociado | 
| PartnerName | Nombre del asociado | 
| PartnerLocation | Ubicación geográfica del asociado | 
| PartnerAttributionType | Tipo de atribución para la suscripción | 
| SalesChannel | Canal de ventas: Directo, CSP (Proveedor de soluciones en la nube), y así sucesivamente | 
| AvailableSeats | Puesto disponible actual | 
| RevenueUSD | Ingresos en dólares estadounidenses | 
| Identificador de inscripción | Identificador de inscripción de la suscripción | 

### <a name="azure-usage-report"></a>**Informe de uso de Azure**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| SubscriptionId | GUID de la suscripción | 
| SubscriptionStartDate | Fecha de inicio de la suscripción | 
| SubscriptionEndDate | Fecha del final de la suscripción | 
| SubscriptionState | Estado actual de la suscripción (Abierto, Cerrado, Activo o En período de gracia) | 
| Mes | Fecha agregada por mes | 
| ServiceName | Nombre del servicio de Azure | 
| MeterCategory | Nombre de la categoría de medidor | 
| UsageUnits | Número de unidades que se usan durante el ciclo de facturación | 
| CustomerName | Nombre del cliente | 
| CustomerTenantId | Identificador de inquilino del cliente | 
| CustomerTpid | Identificador primario principal del cliente | 
| CustomerSegment | Segmento del cliente | 
| CustomerMarket | Mercado geográfico del cliente | 
| MPNId | Microsoft Partner Network identificador del cliente | 
| PartnerName | Nombre del asociado | 
| PartnerLocation | Ubicación geográfica del país del asociado | 
| PartnerAttributionType | Tipo de atribución del asociado | 
| SalesChannel | Canal de las ventas (Directo/CSP, Indirecto/CSP, Directo, y así sucesivamente) | 
| ACR_USD | Ingresos consumidos por Azure (ACR) en dólares estadounidenses | 
| Identificador de inscripción | Identificador de inscripción de la suscripción de Azure | 

### <a name="office-365-license-usage-report"></a>**Informe de uso de licencias de Office 365**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CustomerTenantId | Identificador de inquilino del cliente | 
| CustomerTpid | Identificador primario principal del cliente | 
| WorkloadName | Skype Empresarial, Teams, Exchange Online | 
| Mes | Mes para el que se notifica el uso | 
| PaidAvailableUnits | Número de unidades disponibles de pago | 
| MonthlyActiveUsers | Número de usuarios activos mensuales | 
| CustomerName | Nombre del cliente | 
| CustomerMarket | Ubicación geográfica del país del mercado del cliente | 
| CustomerSegment | Segmento de cliente | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nombre del asociado | 
| PartnerLocation | Ubicación geográfica del asociado | 
| PartnerAttributionType | Tipo de atribución del asociado | 

### <a name="enterprise-mobility-license-usage-report"></a>**Informe de uso de licencias de Enterprise Mobility**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CustomerTenantId | Identificador de inquilino del cliente | 
| CustomerTpid | Identificador primario principal del cliente | 
| WorkloadName | Nombre de la carga de Enterprise Mobility + Security de trabajo (EMS) | 
| Mes | Mes para el que se notifica el uso | 
| PaidAvailableUnits | Número de unidades disponibles de pago | 
| MonthlyActiveUsers | Número de usuarios activos mensuales | 
| CustomerName | Nombre del cliente | 
| CustomerMarket | Ubicación geográfica del país del mercado del cliente | 
| CustomerSegment | Segmento de cliente | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nombre del asociado | 
| PartnerLocation | Ubicación geográfica del asociado | 
| PartnerAttributionType | Tipo de atribución del asociado | 

### <a name="dynamics-365-license-usage-report"></a>**Informe de uso de licencias de Dynamics 365**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| SubscriptionId | GUID de la suscripción | 
| SubscriptionStartDate | Fecha de inicio de la suscripción | 
| SubscriptionEndDate | Fecha de finalización de la suscripción | 
| SubscriptionStatus | Estado de la suscripción | 
| Mes | Mes para el que se notifica el uso | 
| RevSumDivisionName | Nombre de la división rev sum | 
| RevSumCategoryName | Nombre de la categoría rev sum | 
| SKU | SKU del producto | 
| SKUId | Id. de SKU del producto | 
| FreeVsPaidSKU | Indica si se trata de una SKU gratuita o de pago. | 
| SalesModel | Canal de ventas que se usa para vender la suscripción | 
| DetailedSalesModel | Modelo de ventas detallado para la suscripción | 
| CustomerName | Nombre del cliente | 
| CustomerTenantId | GUID del inquilino del cliente | 
| CustomerTpid | Identificador primario principal del cliente | 
| CustomerSegment | Segmento de mercado del cliente | 
| CustomerMarket | Mercado geográfico del cliente | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nombre del asociado | 
| PartnerLocation | Ubicación geográfica del país del asociado | 
| PartnerAttachType | Tipo de atribución para la suscripción | 
| AvailableSeats | Puesto disponible actual | 
| AssignedSeats | Puesto asignado actual | 
| ActiveSeats | Puestos activos actuales | 
| DeploymentOpportunity | Oportunidad de implementación actual | 
| ActiveUsagePercent | Porcentaje de uso activo actual | 

### <a name="power-bi-license-usage-report"></a>**Power BI de uso de licencias**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| SubscriptionId | GUID de la suscripción | 
| SubscriptionStartDate | Fecha de inicio de la suscripción | 
| SubscriptionEndDate | Fecha de finalización de la suscripción | 
| SubscriptionStatus | Estado de la suscripción (activo, inactivo o en período de gracia) | 
| Mes | Fecha agregada por mes | 
| SKU | SKU del producto | 
| SKUId | Id. de SKU del producto | 
| FreeVsPaidSKU | Diferenciador de SKU gratis o de pago | 
| SalesModel | Modelo de ventas que se usa para vender la suscripción | 
| DetailedSalesModel | Modelo de ventas detallado para la suscripción | 
| CustomerName | Nombre del cliente | 
| CustomerTenantId | GUID del inquilino del cliente | 
| CustomerTpid | Identificador del elemento primario principal del cliente | 
| CustomerSegment | Segmento de mercado del cliente | 
| CustomerMarket | Mercado geográfico del cliente | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nombre del asociado | 
| PartnerLocation | Ubicación geográfica del país del asociado | 
| PartnerAttachType | Tipo de atribución para la suscripción | 
| AvailableSeats | Puestos disponibles actualmente | 
| AssignedSeats | Puestos asignados actualmente | 
| ActiveSeats | Puestos activos actuales | 
| DeploymentOpportunity | Oportunidad de implementación actual | 
| ActiveUsagePercent | Porcentaje de uso activo actual | 

### <a name="teams-meetings-and-calls-report"></a>**Informe de reuniones y llamadas de Teams**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CustomerTenantId | Identificador de inquilino del cliente | 
| CustomerTpid | Identificador del elemento primario principal del cliente | 
| Mes | Mes para el que se notifica el uso | 
| Subworkload | Subcarga para la que se notifica el uso (reuniones, llamadas o sistemas telefónicos) | 
| Recuento de reuniones | Número de reuniones | 
| Duración de la reunión | Duración total de la reunión en horas | 

### <a name="teams-monthly-usage-report"></a>**Informe de uso mensual de Teams**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CustomerTenantId | Identificador de inquilino del cliente | 
| CustomerTpid | Identificador del elemento primario principal del cliente | 
| Mes | Mes para el que se notifica el uso | 
| Subworkload | Subcarga para la que se notifica el uso (reuniones, llamadas o sistemas telefónicos) | 
| Usuarios de escritorio | Número de usuarios que usan Teams en el escritorio | 
| Usuarios móviles | Número de usuarios que usan Teams en dispositivos móviles | 
| Usuarios web | Número de usuarios que usan Teams en la web | 
| AllUpParticipants | Número de usuarios únicos de Teams para el mes | 

### <a name="teams-usage-3p-apps-report"></a>**Informe de aplicaciones 3P de uso de Teams**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CustomerTenantId | Identificador de inquilino del cliente | 
| CustomerTpid | Identificador primario principal del cliente | 
| Mes | Mes para el que se notifica el uso | 
| Nombre de la aplicación 3P | Nombre de la aplicación Teams | 
| Número de usuarios | Número de usuarios de la aplicación | 


### <a name="training-details-report"></a>**Informe de detalles de entrenamiento**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| TrainingActivityId | Identificador del entrenamiento | 
| TrainingTitle | Título del entrenamiento | 
| TrainingType | Tipo de entrenamiento (certificación o examen) | 
| IndividualFirstName | Nombre del cliente | 
| IndividualLastName | Apellidos del cliente | 
| Correo electrónico | Identificador de correo electrónico personal del cliente | 
| CorpEmail | Identificador de correo electrónico de office del cliente | 
| TrainingCompletionDate | Fecha de finalización del entrenamiento | 
| Mes | Mes para el que se notifican los datos | 
| IcMCP | Indica si el usuario es un profesional certificado de Microsoft (MCP) | 
| MCPID | Id. de MCP del usuario | 
| MPNId | Identificador de Microsoft Partner Network | 
| PartnerName | Nombre del asociado | 
| PartnerCityLocation | Ubicación geográfica de la ciudad del asociado | 
| PartnerCountryLocation | Ubicación geográfica del país del asociado | 

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
| PartnerName | Nombre del asociado | 
| País | Ubicación geográfica del país del asociado | 

### <a name="competency-summary-and-history-report"></a>**Resumen de competencias e informe de historial**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CompetencyName | Nombre de la competencia | 
| CompetencyLevel | Nivel de la competencia (Gold o Silver) | 
| CompetencyStatus | Estado actual de la competencia (Activo, Inactivo o En período de gracia) | 
| CompetencyStartDate | Fecha de inicio de la competencia | 
| CompetencyEndDate | Fecha de finalización de la competencia | 

### <a name="competency-performance-report"></a>**Informe de rendimiento de competencias**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| CompetencyName | Nombre de la competencia | 
| CompetencyAttainmentOptionName | Nombre de la opción de alcance de la competencia | 
| Mes | Mes para el que se notifican las métricas | 
| MetricName | Nombre de la métrica que es relevante para la competencia | 
| MetricMonthlyContribution | Contribución mensual de la métrica | 
| TTMAggregate | Métrica agregada para los 12 meses finales | 
| AnniversaryYearAggregate | Métrica agregada para el año de aniversario actual | 
| GoldThreshold | Requisito de rendimiento para cumplir la competencia Gold | 
| SilverThreshold | Requisito de rendimiento para cumplir la competencia Silver | 

### <a name="cloud-ascent---microsoft-365-propensity-report"></a>**Cloud Ascent: informe Microsoft 365 propensity**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| Identificador de MPN | Microsoft Partner Network id. | 
| Nombre del asociado | Nombre del asociado | 
| Customer ID | Número de identificador del cliente | 
| Número DUNS | Número de & Dun (D&B) del cliente al que se está puntundo la propensidad | 
| Nombre de cuenta | Nombre de la cuenta | 
| Domain | Dominio de la cuenta | 
| Tamaño de la organización | Tamaño de la organización | 
| Sector | Sector al que pertenece la organización | 
| Vertical | Vertical del cliente que se está puntundo por la propensidad, tal como lo identifican Microsoft, D&B y otros estándares del sector. | 
| Área | Área geográfica de la ubicación | 
| Subsidiaria | Subsidiaria del cliente al que se le está puntundo la propiedad | 
| Territorio de ventas | El territorio de ventas del cliente al que se le está puntundo la propiedad | 
| City | Ubicación geográfica de la ciudad de la organización | 
| Estado | Ubicación del estado geográfico de la organización | 
| Código postal | Código postal de la organización | 
| País | Ubicación geográfica del país de la organización | 
| Segment | Segmento de mercado | 
| Sub Segment | Subsegment del mercado | 
| Resumen de tipos de SMC | Tipo de SMC | 
| Principal no administrado: base de proceso | Principales clientes no administrados: proceso | 
| Principales no administrados: base de usuarios | Principales clientes no administrados: usuario | 
| IsNonProfit | Indica si la organización es sin ánimo de lucro (Sí o No) | 
| Habilitación del trabajo remoto: exchange online de destino | Los clientes que tienen una suscripción activa a Exchange Online, pueden obtener una Microsoft 365 | 
| Habilitación del trabajo remoto: adquisición local (versión actual) con propensidad de Ascent en la nube: +10 licencias | Cliente que tiene un cliente de Office o Windows local actual. Es decir, la versión del cliente es posterior a una versión de fin de ciclo de vida (EOL). El cliente tiene 10 o más licencias. Cliente que tiene una puntuación de propiedad. El asociado debe tener como destino la conversión Microsoft 365. | 
| Habilitación del trabajo remoto: adquisición local (versión actual) con propensidad de Ascent en la nube: <10 licencias | Cliente que tiene un cliente de Office o Windows local actual (es decir, una versión posterior a EOL). El cliente tiene menos de 10 licencias. Cliente que tiene una puntuación de propiedad. El asociado debe tener como destino la conversión a Microsoft 365. | 
| Habilitación del trabajo remoto: adquisición local (versión actual) sin propensidad de Ascent en la nube: +10 licencias | Cliente que tiene un cliente de Office o Windows local actual (es decir, una versión posterior a EOL). El cliente tiene 10 o más licencias. El cliente no tiene una puntuación de propiedad. El asociado debe tener como destino la conversión a Microsoft 365. | 
| Habilitación del trabajo remoto: adquisición local (versión actual) sin propensidad de Cloud Ascent <10 licencias | Cliente que tiene un cliente de Office o Windows local actual (es decir, una versión posterior a EOL). El cliente tiene menos de 10 licencias. El cliente no tiene una puntuación de propiedad. El asociado debe tener como destino la conversión a Microsoft 365. | 
| Habilitación del trabajo remoto: adquisición local (versión EOL) con propensidad de Ascent en la nube: +10 licencias | Cliente que tiene un cliente de Office o Windows local de EOL (es decir, una versión de EOL o anterior). El cliente tiene 10 o más licencias. El cliente tiene una puntuación de propiedad. El asociado debe tener como destino la conversión a Microsoft 365. | 
| Habilitación del trabajo remoto: adquisición local (versión EOL) con propensidad de Ascent en la nube: <10 licencias | Cliente que tiene un cliente de Office o Windows local de EOL (es decir, una versión de EOL o anterior). El cliente tiene menos de 10 licencias. El cliente tiene una puntuación de propiedad. El asociado debe tener como destino la conversión Microsoft 365. | 
| Habilitación del trabajo remoto: adquisición local (versión EOL) sin propensidad de Ascent en la nube: +10 licencias | Cliente que tiene un cliente de Office o Windows local actual (es decir, una versión de EOL o anterior). El cliente tiene 10 o más licencias. El cliente no tiene una puntuación de propiedad. El asociado debe tener como destino la conversión Microsoft 365. | 
| Habilitación del trabajo remoto: adquisición local (versión EOL) sin propensidad de Ascent en la nube: <10 licencias | Cliente que tiene un cliente de Office o Windows local actual (es decir, una versión de EOL o anterior). El cliente tiene menos de 10 licencias. El cliente no tiene una puntuación de propiedad. El asociado debe tener como destino la conversión Microsoft 365. | 
| Habilitación del trabajo remoto: perspectiva de alta propensidad para Microsoft 365 (Act NowithEvaluate) | Cliente potencial con alta propensidad para Microsoft 365 | 
| Habilitación del trabajo remoto: compite (Zoom) con Microsoft 365 | Cliente con Zoom y Microsoft 365, destino para la conversión a Teams | 
| Habilitación del trabajo remoto: compite (Zoom) sin Microsoft 365 | Cliente con Zoom, destino para la conversión a Teams | 
| Reducción de costos y administración: Microsoft 365 E3 destinado a Microsoft 365 E5 | Cliente existente con Microsoft 365 E3, destino de Microsoft 365 E5 | 
| Reducir costos y administrar: Microsoft 365 clientes de Business Basic y Business Standard destinados a Microsoft 365 Business Premium | Clientes Microsoft 365 Business Basic y Business Standard, destino de Microsoft 365 Business Premium | 
| Transformación de la productividad organizativa: propensidad de surface | El cliente muestra una propensidad para Surface | 
| M365Cluster | Identifica la propensión de un cliente a comprar Microsoft 365. Actuar ahora y evaluar clústeres de destino porque producirán un mayor rendimiento. Fomentar y formar a los clientes de destino solo si todavía hay capacidad después de que los clientes actúen ahora y evalúen a los clientes. | 
| M365Fit | Puntos de datos internos y externos que definen firmográficas. La puntuación de ajuste usa un modelo similar al de nuestras mejores pequeñas o medianas empresas (SMB) para comparar a los clientes y ver si son una posible opción para los productos en la nube de Microsoft. La puntuación de ajuste se actualiza trimestralmente. | 
| M365Intent | Las señales relacionadas con las redes sociales y el comportamiento en línea de un cliente definen la intención. La puntuación de intención se sobrepase en Ajustar para definir los clústeres. La puntuación de intención se actualiza mensualmente. | 
| SurfaceCluster | Identifica la propensión de un cliente a comprar Surface mediante la consolidación de las recomendaciones Ajustar e Intención en un clúster. Actuar ahora y evaluar clústeres de destino porque producirán un mayor rendimiento. Fomente y eduque a los clientes solo si todavía hay capacidad después de que los clientes actuar ahora y evaluar estén dirigidos. | 
| SurfaceFit | Puntos de datos internos y externos que definen firmographics. La puntuación de ajuste usa un modelo similar a nuestros mejores SMB para comparar a los clientes y ver si son una posible opción para los productos en la nube de Microsoft. La puntuación de ajuste se actualiza trimestralmente. | 
| SurfaceIntent | Las señales relacionadas con las redes sociales y el comportamiento en línea de un cliente definen la intención. La puntuación de intención se sobrelada en Ajustar para definir los clústeres. La puntuación de intención se actualiza mensualmente. | 
| O365Cluster | Identifica la propensión del cliente a comprar Office 365. Actuar ahora y evaluar clústeres de destino porque producirán un mayor rendimiento. Fomente a los clientes solo si aún hay capacidad después de que actúe ahora y evalúe a los clientes. | 
| O365Fit | Puntos de datos internos y externos que definen firmographics. La puntuación de ajuste usa un modelo similar a nuestros mejores SMB para comparar a los clientes y ver si son una posible opción para los productos en la nube de Microsoft. La puntuación de ajuste se actualiza trimestralmente. | 
| O365Intent | Las señales relacionadas con las redes sociales y el comportamiento en línea de un cliente definen la intención. La puntuación de intención se sobrepase en Ajustar para definir los clústeres. La puntuación de intención se actualiza mensualmente. | 
| M365UpsellCustomer | Identifica si el cliente muestra la propensidad de las ventas para Microsoft 365 | 
| Tiene Google | Identifica si el cliente muestra señales competitivas para poseer productos de Google. | 
| Tiene AWS | Identifica si el cliente muestra señales competitivas para poseer Amazon Web Services (AWS) | 
| Tiene EA | Identifica si una renovación es un contrato Enterprise (EA) o una suscripción de EA. | 
| Tiene abierto | Identifica si una renovación es un contrato open o open value | 

### <a name="cloud-ascent---dynamics-365-propensity-report"></a>**Cloud Ascent: informe de propensidad de Dynamics 365**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| Identificador de MPN | Microsoft Partner Network id. | 
| Nombre del asociado | Nombre del asociado | 
| Customer ID | Número de identificador de cliente | 
| Número DUNS | El número & Desanualado del cliente al que se le está puntundo la propensidad | 
| Nombre de cuenta | Nombre de la cuenta | 
| Domain | Dominio de la cuenta | 
| Tamaño de la organización | Tamaño de la organización | 
| Sector | Sector al que pertenece la organización | 
| Vertical | Vertical del cliente que se está puntundo por propensidad, como se identifica en Microsoft, D&B y otros estándares del sector.
| Área | Área geográfica de la ubicación | 
| Subsidiaria | Subsidiaria del cliente al que se le está puntundo por propensidad | 
| Territorio de ventas | El territorio de ventas del cliente al que se está puntundo la propiedad | 
| City | Ubicación geográfica de la ciudad | 
| Estado | Ubicación del estado geográfico | 
| Código postal | Código postal de la organización | 
| País | Ubicación geográfica del país | 
| Segment | Segmento de mercado | 
| Sub Segment | Subsegment del mercado | 
| Resumen de tipos de SMC | Categorización de un cliente: las principales bases de usuarios no administrados son clientes con más de 300 empleados, las bases de proceso no administradas principales son clientes con un potencial de tres años de USD 10 000 en Azure, las medianas son clientes con 25 empleados o más, y las pequeñas empresas son clientes con menos de 25 empleados. | 
| Principal no administrado: base de proceso | Principales clientes no administrados: proceso | 
| Principales no administrados: base de usuarios | Principales clientes no administrados: usuarios | 
| IsNonProfit | Indica si la organización es sin ánimo de lucro (Sí o No) | 
| Activación de la venta digital Microsoft 365 tamaño de puesto >= 25 puestos (modelo de propensidad de SalesPro) | Cliente sin Dynamics 365. Tamaño del puesto: 25+. El partner debe tener como destino la venta cruzada de Dynamics 365 SalesPro. | 
| Activación de la venta digital: propensidad de Dynamics 365 SalesPro (actuar ahora o evaluar) | Clientes de alta propensidad sin Dynamics 365. El partner debe tener como destino Dynamics 365 SalesPro. | 
| Administración de riesgos financieros & fraude: base de instalación local de Dynamics: Navision (modelo de propensidad de Business Central) | Cliente existente con Navision local. El asociado debe tener como destino Dynamics 365 Business Central. | 
| Administración de riesgos financieros & fraudes: base de instalación local de Dynamics: Dynamics AX (modelo de propensidad de Dynamics 365 Finance + Operations) | Cliente existente con AX local. El asociado debe tener como destino Dynamics 365 Finance + Operations. | 
| Administración de riesgos financieros & fraude: base de instalación local de Dynamics: Great Plains (modelo de propensidad de Business Central) | Cliente existente con Great Plains local. El asociado debe tener como destino Dynamics 365 Business Central. | 
| Administración de riesgos financieros & fraudes: base de instalación local de Dynamics - Loba (modelo de propensidad de Business Central) | Cliente existente con Premises Premises. El partner debe tener como destino Dynamics 365 Business Central. | 
| Administración de riesgos financieros & fraudes- Base de instalación local de Dynamics - Otros (modelo de propensidad de Business Central) | Cliente existente con otras soluciones locales que no se han enumerado anteriormente. El partner debe tener como destino Dynamics 365 Business Central. | 
| Creación de procesos empresariales ágiles: base de instalación local de Dynamics: AX/GP/SL/NAV/Otros (modelo de propensidad de Dynamics 365) | Creación de procesos empresariales ágiles: base de instalación local de Dynamics: AX/GP/SL/NAV/Other (modelo de propensidad de Dynamics 365) | 
| Creación de procesos empresariales ágiles: Dynamics compite en base: Mendix/OutSystems/Salesforce (modelo de propensidad de Dynamics 365) | Creación de procesos empresariales ágiles: Dynamics Compet Base - Mendix/OutSystems/Salesforce (modelo de propensidad de Dynamics 365) | 
| Creación de procesos empresariales ágiles: base de instalación de Dynamics 365 Finance + Operations | Clientes existentes de Dynamics 365 Finance + Operations. Partner to target Power Apps. | 
| Creación de procesos empresariales ágiles: base de instalación de Dynamics 365 Business Central | Clientes existentes de Dynamics 365 Business Central. Partner to target Power Apps. | 
| Creación de procesos empresariales ágiles: base de instalación de Dynamics 365 Customer Engagement | Clientes existentes de Dynamics 365 Customer Engagement. Partner to target Power Apps. | 
| Creación de una cadena de suministro resistente: Windows y activación de la primera carga de trabajo de Dynamics 365 como Dynamics 365 Supply Chain Management con clientes que no son de Oracle o SAP ERP (planeamiento de recursos empresariales) | Clientes de destino para la administración de la cadena de suministro de Dynamics 365 | 
| Creación de una cadena de suministro resistente: administración de la cadena de suministro de Dynamics 365 cruzada o comercio minorista a clientes existentes de Dynamics 365 Customer Engagement | Clientes existentes de Dynamics 365 Customer Engagement para dirigirse a la administración de la cadena de suministro de Dynamics 365 de venta cruzada. | 
| Creación de una cadena de suministro resistente: administración de la cadena de suministro de Dynamics 365 de venta cruzada o venta minorista o comercial a Dynamics 365 Customer Engagement y Oracle o SAP | Clientes existentes de Dynamics 365 Customer Engagement con Oracle o SAP para dirigirse a Dynamics 365 Supply Chain Management | 
| D365BCCluster | Identifica la propensión del cliente a comprar Dynamics 365 Business Central. Los clientes que muestren una propiedad para Business Central estarán en las categorías Mediano y Pequeño. Actuar ahora y evaluar clústeres de destino, ya que producirán un mayor rendimiento. Fomentar y formar a los clientes de destino solo si todavía hay capacidad después de dirigirSe a actuar ahora y evaluar a los clientes. | 
| D365BCFit | Puntos de datos internos y externos que definen firmográficas. La puntuación de ajuste usa un modelo similar a nuestro mejor SMB para comparar a los clientes y ver si son una posible opción para los productos en la nube de Microsoft. La puntuación de ajuste se actualiza trimestralmente. | 
| D365BCIntent | Las señales relacionadas con las redes sociales y el comportamiento en línea de un cliente definen la intención. La puntuación de intención se sobrepase en Ajustar para definir los clústeres. La puntuación de intención se actualiza mensualmente. | 
| D365FOCluster | Identifica la propensión del cliente a comprar Dynamics 365 Finance and Operations. Los clientes que muestren una propiedad para Finance + Operations estarán en las principales categorías no administradas. Actuar ahora y evaluar clústeres de destino, ya que producirán un mayor rendimiento. Fomentar y formar a los clientes de destino solo si todavía hay capacidad después de dirigirse a los clientes de Act Now y Evaluate. | 
| D365FOFit | Puntos de datos internos y externos que definen firmographics. La puntuación de ajuste usa un modelo similar a nuestro mejor SMB para comparar a los clientes y ver si son una posible opción para los productos en la nube de Microsoft. La puntuación de ajuste se actualiza trimestralmente. | 
| D365FOIntent | Las señales relacionadas con las redes sociales y el comportamiento en línea de un cliente definen la intención. La puntuación de intención se sobrelada en Ajustar para definir los clústeres. La puntuación de intención se actualiza mensualmente. | 
| D365CECluster | Identifica la propensión del cliente a comprar Dynamics 365 Customer Engagement. Los clientes que muestren una propensura para Customer Engagement estarán en las categorías Mediano y Pequeño. Actuar ahora y evaluar clústeres de destino, ya que producirán un mayor rendimiento. Fomentar y formar a los clientes de destino solo si todavía hay capacidad después de dirigirse a los clientes de Act Now y Evaluate. | 
| D365CEFit | Indica que se ajusta a Dynamics 365 Customer Engagement | 
| D365CEIntent | Indica la intención de Dynamics 365 Customer Engagement | 
| DynamicsOnPremAXorCRM_HasOpenRenewal | Identifica si el cliente tiene una renovación abierta para Dynamics on-premises AX o CRM. | 
| M365UpsellCustomer | Identifica si el cliente muestra la propensidad de las ventas para Microsoft 365 | 
| Tiene Google | Identifica si el cliente muestra señales competitivas para poseer productos de Google. | 
| Tiene AWS | Identifica si el cliente muestra señales competitivas para poseer productos de AWS. | 
| Tiene EA | Identifica si una renovación es un CONTRATO o una suscripción de EA. | 
| Tiene abierto | Identifica si una renovación es un contrato open o open value | 

### <a name="cloud-ascent---azure-propensity-report"></a>**Cloud Ascent: informe de propensidad de Azure**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| Identificador de MPN | Microsoft Partner Network id. | 
| Nombre del asociado | Nombre del asociado | 
| Customer ID | Número de identificador de cliente | 
| Número DUNS | El número & Desanualado del cliente al que se le está puntundo la propensidad | 
| Nombre de cuenta | Nombre de la cuenta | 
| Domain | Dominio de la cuenta | 
| Tamaño de la organización | Tamaño de la organización | 
| Sector | Sector | 
| Vertical | Vertical del cliente que se está puntundo por propensidad, como se identifica en Microsoft, D&B y otros estándares del sector. | 
| Área | Área geográfica de la ubicación | 
| Subsidiaria | Subsidiaria del cliente al que se le está puntundo por propensidad | 
| Territorio de ventas | El territorio de ventas del cliente al que se está puntundo la propiedad | 
| City | Ubicación geográfica de la ciudad | 
| Estado | Ubicación del estado geográfico | 
| Código postal | Código postal de la organización | 
| País | Ubicación geográfica del país | 
| Segment | Segmento de mercado | 
| Sub Segment | Subsegment del mercado | 
| Resumen del tipo SMC | Tipo de SMC | 
| Principal no administrado: base de proceso | Principales clientes no administrados: proceso | 
| Principales no administrados: base de usuarios | Principales clientes no administrados: usuarios | 
| IsNonProfit | Indica si la organización es sin ánimo de lucro (Sí o No) | 
| Migrar - EOL Windows Server - EOL Windows Server IB con propensidad de ascención en la nube - más de 5 licencias | Cliente que tiene un servidor de Windows Server local EOL (es decir, una versión de EOL o anterior). El cliente tiene 5 o más licencias. Cliente que tiene una puntuación de propiedad. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migrar - EOL Windows Server - EOL Windows Server IB with Cloud Ascent propensity ( EOL Windows Server - EOL Windows Server IB with Cloud Ascent propensity - <5 licencias | Cliente que tiene un servidor de Windows Server local EOL (es decir, una versión de EOL o anterior). El cliente tiene menos de 5 licencias. Cliente que tiene una puntuación de propiedad. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración - EOL Windows Server - EOL Windows Server IB sin propensidad de ascención en la nube : más de 5 licencias | Cliente que tiene un servidor de Windows Server local EOL (es decir, una versión de EOL o anterior). El cliente tiene más de 5 licencias. El cliente no tiene una puntuación de propiedad. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración - EOL Windows Server - EOL Windows Server IB sin propensidad de ascención en la nube: <5 licencias | Cliente que tiene un servidor de Windows Server local EOL (es decir, una versión de EOL o anterior). Tiene menos de 5 licencias. El cliente no tiene una puntuación de propiedad. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración - EOL SQL - EOL SQL Server IB con propensidad de ascención en la nube : más de 5 licencias | Cliente que tiene una versión local de EOL SQL Server (es decir, una versión de EOL o anterior). El cliente tiene más de 5 licencias. El cliente tiene una puntuación de propiedad. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración - EOL SQL - EOL SQL Server IB con propensidad de ascención de nube - <5 licencias | Cliente que tiene una versión local de EOL SQL Server (es decir, una versión de EOL o anterior). Tiene menos de 5 licencias. Cliente que tiene una puntuación de propiedad. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración - EOL SQL - EOL SQL Server IB sin propensidad de ascención de nube - más de 5 licencias | Cliente que tiene una versión local de EOL SQL Server (es decir, una versión de EOL o anterior). El cliente tiene 5 o más licencias. El cliente no tiene una puntuación de propiedad. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración - EOL SQL - EOL SQL Server IB sin propensidad de ascención de nube- <5 licencias | Cliente que tiene una versión local de EOL SQL Server (es decir, una versión de EOL o anterior). El cliente tiene menos de 5 licencias. El cliente no tiene una puntuación de propiedad. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración: migración de Windows Server local: windows server IB actual con propensidad de ascención en la nube: más de 5 licencias | Cliente que tiene una instancia de Windows Server local actual (es decir, una versión posterior a EOL). El cliente tiene más de 5 licencias. El cliente tiene una puntuación de propiedad. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración: migración de Windows Server local: windows server ib actual con propensidad de ascención en la nube <5 licencias | Cliente que tiene una instancia de Windows Server local actual (es decir, una versión posterior a EOL). El cliente tiene menos de 5 licencias. El cliente tiene una puntuación de propiedad para Azure. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración: migración de Windows Server local: windows server IB actual sin propensidad de ascención en la nube: más de 5 licencias | Cliente que tiene una instancia de Windows Server local actual (es decir, una versión posterior a EOL). El cliente tiene más de 5 licencias. El cliente no tiene una puntuación de propiedad. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración: migración de Windows Server local: Windows Server IB actual sin propensidad de ascención en la nube: <5 licencias | Cliente que tiene una instancia de Windows Server local actual (es decir, una versión posterior a EOL). El cliente tiene menos de 5 licencias. El cliente no tiene una puntuación de propiedad. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración: migración a Azure SQL o máquinas virtuales (VM) SQL( actuales SQL Server IB con propensidad de ascención a la nube : más de 5 licencias | Cliente que tiene una versión local SQL Server (es decir, una versión posterior a EOL). El cliente tiene más de 5 licencias. El cliente tiene una puntuación de propiedad. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración: migración a máquinas Azure SQL sql o a máquinas virtuales sql: SQL Server IB con propensidad de ascención en la nube: <5 licencias | Cliente que tiene una versión local SQL Server (es decir, una versión posterior a EOL). El cliente tiene menos de 5 licencias. El cliente tiene una puntuación de propiedad. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración: migración a máquinas virtuales Azure SQL o SQL: versión SQL Server IB sin propensidad de ascención en la nube: más de 5 licencias | Cliente que tiene una versión local SQL Server (es decir, una versión posterior a EOL). El cliente tiene más de 5 licencias. El cliente no tiene una puntuación de propiedad. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración: migración a máquinas virtuales Azure SQL o SQL( versión SQL Server IB sin propensidad de ascención en la nube: <5 licencias | Cliente que tiene una versión local SQL Server (es decir, una versión posterior a EOL). El cliente tiene menos de 5 licencias. El cliente no tiene una puntuación de propiedad. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración : sistema operativo: migración a la base de datos de Código abierto de Shakespeare (OSS) | Los clientes existentes con cualquiera de los siguientes productos compiten: PostgreSQL, MySQL, MariaDB. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración de OSS en Linux en Azure | Cliente existente con Linux. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración: SAP: SAP en Azure | Cliente existente con SAP. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración - Windows Virtual Desktop - Servicios de Escritorio remoto IB | Identifica los clientes con windows activo Servicios de Escritorio remoto. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración de Windows Virtual Desktop de trabajo moderno de venta cruzada a Azure/WVD | Identifica los clientes con Microsoft 365 y no tiene Azure. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración: VMware IB | Cliente existente con el producto: VMware. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Migración: Citrix IB | Cliente existente con el producto: Citrix Systems. El asociado debe dirigirse a este cliente para la migración a Azure. | 
| Innovación: Analytics: Power BI IB con alta propensidad de Azure | Clientes con y suscripción Power BI Active Power BI, incluidos: Power BI - Standalone Pro, Power BI - Azure Suites, Power BI - Office Suites, Power BI Suites - Microsoft 365 | 
| Habilitar - DevOps con GitHub - Visual Studio/MSDN IB | Identifica clientes con versiones de Visual Studio activas | 
| Versión estándar de Windows Server | Muestra la versión de las compras de Windows Server Standard realizadas por el cliente | 
| Licencia de Windows Server Standard | Muestra el tipo de licencia de las compras de Windows Server Standard realizadas por el cliente | 
| Versión de Windows Server Data Center | Muestra la versión de las compras de Windows Data Center realizadas por el cliente | 
| Licencia de Windows Server Data Center | Muestra el tipo de licencia de las compras de Windows Data Center realizadas por el cliente | 
| AzureFit | Puntos de datos internos y externos que definen firmographics. La puntuación de ajuste usa un modelo similar a nuestro mejor SMB para comparar a los clientes y ver si son una posible opción para los productos en la nube de Microsoft. La puntuación de ajuste se actualiza trimestralmente. | 
| AzureIntent | Las señales relacionadas con las redes sociales y el comportamiento en línea de un cliente definen la intención. La puntuación de intención se sobrelada en Ajustar para definir los clústeres. La puntuación de intención se actualiza mensualmente. | 
| AzureCluster | Identifica la propensión del cliente a comprar Azure mediante la consolidación de las recomendaciones de ajuste e intención en un clúster. Actuar ahora y evaluar clústeres de destino, ya que producirán un mayor rendimiento. Fomentar y formar a los clientes de destino solo si todavía hay capacidad después de dirigirSe a actuar ahora y evaluar a los clientes. | 
| WindowsServerDataCenter_HasOpenRenewal | Identifica si el cliente tiene una renovación abierta para Windows Server Datacenter | 
| WindowsServerStandard_HasOpenRenewal | Identifica si el cliente tiene una renovación abierta para Windows Server Standard. | 
| AzureUpsellCustomer | Identifica si el cliente muestra la propensidad de las ventas emergentes para Azure. | 
| Tiene Google | Identifica si el cliente muestra señales competitivas para poseer productos de Google. | 
| Tiene AWS | Identifica si el cliente muestra señales competitivas para poseer productos de AWS. | 
| Tiene EA | Identifica si una renovación es un CONTRATO o una suscripción de EA. | 
| Tiene abierto | Identifica si una renovación es un contrato open o open value | 

### <a name="cloud-ascent---agreement-renewal-propensity-report"></a>**Cloud Ascent: informe de propensidad de renovación de contratos**

| Nombre de la columna | Descripción de los datos | 
| :--------- | :--------- | 
| Identificador de MPN | Microsoft Partner Network id. | 
| Nombre del asociado | Nombre del asociado | 
| Customer ID | Número de identificador de cliente | 
| Número DUNS | El número & Brad street del cliente al que se está puntundo por propensidad | 
| Nombre de cuenta | Nombre de la cuenta | 
| Domain | Dominio de la cuenta | 
| Tamaño de la organización | Tamaño de la organización | 
| Sector | Sector | 
| Vertical | Vertical del cliente que se está puntundo por propensidad, como se identifica en Microsoft, D&B y otros estándares del sector. | 
| Área | Área geográfica de la ubicación | 
| Subsidiaria | Subsidiaria del cliente al que se le está puntundo por propensidad | 
| Territorio de ventas | El territorio de ventas del cliente al que se está puntundo la propiedad | 
| City | Ubicación geográfica de la ciudad | 
| Estado | Ubicación del estado geográfico | 
| Código postal | Código postal de la organización | 
| País | Ubicación geográfica del país | 
| Segment | Segmento de mercado | 
| Sub Segment | Subsegment del mercado | 
| Resumen de tipos de SMC | Tipo de SMC | 
| Principal no administrado: base de proceso | Principales clientes no administrados: proceso | 
| Principales no administrados: base de usuarios | Principales clientes no administrados: usuarios | 
| IsNonProfit | Indica si la organización es sin ánimo de lucro (Sí o No) | 
| Tiene Google | Identifica si el cliente muestra señales competitivas para poseer productos de AWS. | 
| Tiene AWS | Identifica si el cliente muestra señales competitivas para poseer productos de AWS. | 
| Clúster de Azure | Identifica la propensión del cliente a comprar Azure. Actuar ahora y evaluar clústeres de destino, ya que producirán un mayor rendimiento. Fomentar y formar a los clientes de destino solo si todavía hay capacidad después de dirigirSe a actuar ahora y evaluar a los clientes. | 
| D365 Finance + Operations Cluster | Identifica la propensión del cliente a comprar Dynamics 365 Finance and Operations. Los clientes que muestren una propiedad para Finance + Operations estarán en las principales categorías no administradas. Actuar ahora y evaluar clústeres de destino, ya que producirán un mayor rendimiento. Fomentar y formar a los clientes de destino solo si todavía hay capacidad después de dirigirse a los clientes de Act Now y Evaluate. | 
| Clúster de D365 CE | Identifica la propensión del cliente a comprar Dynamics 365 Customer Engagement. Los clientes que muestren una propensura para Customer Engagement estarán en las categorías Mediano y Pequeño. Actuar ahora y evaluar clústeres de destino, ya que producirán un mayor rendimiento. Fomentar y formar a los clientes de destino solo si todavía hay capacidad después de dirigirse a los clientes de Act Now y Evaluate. | 
| Clúster de D365 BC | Identifica la propensión del cliente a comprar Dynamics 365 Business Central. Los clientes que muestren una tendencia para Business Central estarán en las categorías Mediano y Pequeño. Actuar ahora y evaluar clústeres de destino, ya que producirán un mayor rendimiento. Fomentar y formar a los clientes de destino solo si todavía hay capacidad después de dirigirse a los clientes de Act Now y Evaluate. | 
| Microsoft 365 Cluster | Identifica la propensión del cliente a comprar Microsoft 365. Actuar ahora y evaluar clústeres de destino, ya que producirán un mayor rendimiento. Fomentar y formar a los clientes de destino solo si todavía hay capacidad después de dirigirse a los clientes de Act Now y Evaluate. | 
| Programa de licencias | Identifica el tipo de programa de licencia para la renovación. | 
| Identificador del acuerdo | Identificador del contrato | 
| Fecha de finalización del contrato | Fecha de finalización del contrato | 
| Tipo de caducidad | Tipo de expiración | 
| Ingresos que expiran | Ingresos asociados a suscripciones que expiran | 
| Tiene EA | Identifica si una renovación es un CONTRATO o una suscripción de EA. | 
| Tiene abierto | Identifica si una renovación es un contrato open o open value | 
| Cliente de Azure Upsell | Identifica si el cliente muestra la propensidad de las ventas emergentes para Azure. | 
| Microsoft 365 cliente de Upsell | Identifica si el cliente muestra la propensidad de las ventas para Microsoft 365 | 
| RevSumDivisionName | Identifica el producto que está en proceso de renovación. | 

## <a name="next-steps"></a>Pasos siguientes

Para obtener más información, vea [Descargar informes.](pci-download-reports.md)
