---
title: Lista de consultas del sistema para el acceso mediante programación a Partner Insights
description: Obtenga más información sobre las consultas del sistema que puede usar para acceder a los datos de análisis de Partner Insights.
ms.topic: reference
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 4b0bd5411d02463b015cf812cde78e34ef853814
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375830"
---
# <a name="list-of-system-queries-for-partner-insights-programmatic-access"></a><span data-ttu-id="f5d82-103">Lista de consultas del sistema para el acceso mediante programación a Partner Insights</span><span class="sxs-lookup"><span data-stu-id="f5d82-103">List of system queries for partner insights programmatic access</span></span>

<span data-ttu-id="f5d82-104">Las siguientes consultas del sistema se pueden usar en [Create Report API](insights-programmatic-access-paradigm.md#create-report-api) directamente con queryId.</span><span class="sxs-lookup"><span data-stu-id="f5d82-104">The following system queries can be used in the [Create Report API](insights-programmatic-access-paradigm.md#create-report-api) directly with a QueryId.</span></span> <span data-ttu-id="f5d82-105">Las consultas del sistema son como los informes de exportación Centro de partners durante un período de cálculo de seis meses (6 M).</span><span class="sxs-lookup"><span data-stu-id="f5d82-105">The system queries are like the export reports in Partner Center for a six-month (6M) computation period.</span></span>

<span data-ttu-id="f5d82-106">Para obtener más información sobre los nombres de columna, los atributos y la descripción, consulte las [definiciones de datos.](insights-data-definitions.md)</span><span class="sxs-lookup"><span data-stu-id="f5d82-106">For more details on the column names, attributes, and description, please refer to the [Data Definitions](insights-data-definitions.md)</span></span>

<span data-ttu-id="f5d82-107">En las secciones siguientes se proporcionan consultas para varios informes.</span><span class="sxs-lookup"><span data-stu-id="f5d82-107">The following sections provide report queries for various reports.</span></span>

## <a name="customers"></a><span data-ttu-id="f5d82-108">Clientes</span><span class="sxs-lookup"><span data-stu-id="f5d82-108">Customers</span></span>

<span data-ttu-id="f5d82-109">Informe de clientes de los últimos seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-109">The Customers report for the last six months</span></span>

<span data-ttu-id="f5d82-110">Id. de consulta: `6664daf3-c161-423a-92a1-0ea6db2c0384`</span><span class="sxs-lookup"><span data-stu-id="f5d82-110">Query ID: `6664daf3-c161-423a-92a1-0ea6db2c0384`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-111">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-111">Report query</span></span>
```sql
SELECT PGAMpnId,MpnId,PartnerName,CustomerName,CustomerTpid,DUNSNumber,CustomerSegment,TopSegment,
CustomerMarket,CustomerStatus,CustomerTenantId,CustomerTenantName,CustomerTenantCountry,TenantDomainName,
Product,RawProductName,ProductPartNumber,SKU,Month,PartnerLocation,PartnerAttributionType,SalesChannel,
IsDuplicateRowForPGA,AvailableSeats,BilledRevenueUSD,AzureConsumedRevenueUSD 
FROM CustomersAndTenants TIMESPAN LAST_6_MONTHS
```

## <a name="seats-subscriptions-and-revenue"></a><span data-ttu-id="f5d82-112">Suscripciones e ingresos de puestos</span><span class="sxs-lookup"><span data-stu-id="f5d82-112">Seats Subscriptions and Revenue</span></span>

<span data-ttu-id="f5d82-113">Informe de puestos, suscripciones e ingresos de los últimos seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-113">Seats, subscriptions, and revenue report for the last six months</span></span>

<span data-ttu-id="f5d82-114">Id. de consulta: `c9fc1c79-4408-49ff-97f9-e1aa3f155804`</span><span class="sxs-lookup"><span data-stu-id="f5d82-114">Query ID: `c9fc1c79-4408-49ff-97f9-e1aa3f155804`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-115">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-115">Report query</span></span>

```sql
SELECT PGAMpnId,MpnId,SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionState,month,
IsAutoRenew,CustomerName,CustomerTenantId,CustomerTpid,DUNSNumber,CustomerSegment,TopSegment,CustomerMarket,
ProductFamily,ReportingProductName,Product,RawProductName,ProductPartNumber,SKU,RevSumDivisionName,PartnerName,
SolutionArea,PartnerLocation,PartnerAttributionType,SalesChannel,PricingLevel,EnrollmentNumber,
IsDuplicateRowForPGA,SubscriptionStartMonth,TotalSoldSeats,TotalAssignedSeats,BilledRevenueUSD,
AzureConsumedRevenueUSD FROM SeatsSubscriptionsAndRevenue TIMESPAN LAST_6_MONTHS
```

## <a name="partner-profile"></a><span data-ttu-id="f5d82-116">Perfil de partner</span><span class="sxs-lookup"><span data-stu-id="f5d82-116">Partner Profile</span></span>

<span data-ttu-id="f5d82-117">Generación de perfiles de datos</span><span class="sxs-lookup"><span data-stu-id="f5d82-117">Profile data</span></span>

<span data-ttu-id="f5d82-118">Id. de consulta: `e65f3a4f-fb99-4319-97ff-59e57566a871`</span><span class="sxs-lookup"><span data-stu-id="f5d82-118">Query ID: `e65f3a4f-fb99-4319-97ff-59e57566a871`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-119">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-119">Report query</span></span>

```sql
SELECT MPNId,PartnerName,PGA_MPNId,PGA_PartnerName,City,Country,HierarchyLevel 
FROM Profile
```

## <a name="azure-usage"></a><span data-ttu-id="f5d82-120">Uso de Azure</span><span class="sxs-lookup"><span data-stu-id="f5d82-120">Azure Usage</span></span>

<span data-ttu-id="f5d82-121">Informe de AzureUsage de los últimos seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-121">AzureUsage report for the last six months</span></span>

<span data-ttu-id="f5d82-122">Id. de consulta: `d1a4d75e-5ca8-4847-845f-ee0a9be6f07b`</span><span class="sxs-lookup"><span data-stu-id="f5d82-122">Query ID: `d1a4d75e-5ca8-4847-845f-ee0a9be6f07b`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-123">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-123">Report query</span></span>

```sql
SELECT PGAMpnId,SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,FirstUseDate,SubscriptionState,Month,
ServiceName,MeterCategory,UsageUnits,UsageQuantity,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MpnId,PartnerName,PartnerLocation,PartnerAttributionType,SalesChannel,EnrollmentNumber,
IsACRDuplicateAtPGALevel,ResellerID,ResellerName,MonthlySubscriptionLevelACR,TotalACR 
FROM AzureUsage TIMESPAN LAST_6_MONTHS
```

## <a name="office-usage"></a><span data-ttu-id="f5d82-124">Office Uso</span><span class="sxs-lookup"><span data-stu-id="f5d82-124">Office Usage</span></span>

<span data-ttu-id="f5d82-125">Informe de OfficeUsage de los últimos seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-125">OfficeUsage report for the last six months</span></span>

<span data-ttu-id="f5d82-126">Id. de consulta: `d8349f7b-a7d1-467e-b26d-434d4a50f26a`</span><span class="sxs-lookup"><span data-stu-id="f5d82-126">Query ID: `d8349f7b-a7d1-467e-b26d-434d4a50f26a`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-127">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-127">Report query</span></span>

```sql
SELECT CustomerTenantId,CustomerTpid,WorkloadName,Month,PaidAvailableUnits,MonthlyActiveUsers,CustomerName,
CustomerMarket,CustomerSegment,MPNId,PartnerName,PartnerLocation,PartnerAttributionType,IsDuplicateRowForPGA
FROM OfficeUsage TIMESPAN LAST_6_MONTHS
```

## <a name="dynamics-usage"></a><span data-ttu-id="f5d82-128">Uso de Dynamics</span><span class="sxs-lookup"><span data-stu-id="f5d82-128">Dynamics Usage</span></span>

<span data-ttu-id="f5d82-129">Informe de DynamicsUsage durante seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-129">DynamicsUsage report for six months</span></span>

<span data-ttu-id="f5d82-130">Id. de consulta: `6209a8fd-93af-442e-8b3f-3df0f77e8463`</span><span class="sxs-lookup"><span data-stu-id="f5d82-130">Query ID: `6209a8fd-93af-442e-8b3f-3df0f77e8463`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-131">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-131">Report query</span></span>

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,RevSumDivisionName,
RevSumCategoryName,SKU,SKUId,FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,
CustomerTpid,CustomerSegment,CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,AvailableSeats,
AssignedSeats,ActiveSeats,DeploymentOpportunity,ActiveUsagePercent 
FROM DynamicsUsage TIMESPAN LAST_6_MONTHS
```

## <a name="power-bi-usage"></a><span data-ttu-id="f5d82-132">Uso de Power BI</span><span class="sxs-lookup"><span data-stu-id="f5d82-132">Power BI usage</span></span>

<span data-ttu-id="f5d82-133">Informe de PowerBIUsage durante seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-133">PowerBIUsage report for six months</span></span>

<span data-ttu-id="f5d82-134">Id. de consulta: `40ebfe2f-7183-4427-a911-5c9b45b6df15`</span><span class="sxs-lookup"><span data-stu-id="f5d82-134">Query ID: `40ebfe2f-7183-4427-a911-5c9b45b6df15`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-135">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-135">Report query</span></span>

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,SKU,SKUId,
FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,PartnerHierarchy,AvailableSeats,
AssignedSeats,ActiveSeats,DeploymentOpportunity,ActiveUsagePercent 
FROM PowerBIUsage TIMESPAN LAST_6_MONTHS
```

## <a name="ems-usage"></a><span data-ttu-id="f5d82-136">Uso de EMS</span><span class="sxs-lookup"><span data-stu-id="f5d82-136">EMS Usage</span></span>

<span data-ttu-id="f5d82-137">Informe de EMSUsage durante seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-137">EMSUsage report for six months</span></span>

<span data-ttu-id="f5d82-138">Id. de consulta: `d7f20ea4-8751-4d6b-b1d7-821c316acd6a`</span><span class="sxs-lookup"><span data-stu-id="f5d82-138">Query ID: `d7f20ea4-8751-4d6b-b1d7-821c316acd6a`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-139">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-139">Report query</span></span>

```sql
SELECT SubscriptionId,SubscriptionStartDate,SubscriptionEndDate,SubscriptionStatus,Month,SKU,SKUId,
FreeVsPaidSKU,SalesModel,DetailedSalesModel,CustomerName,CustomerTenantId,CustomerTpid,CustomerSegment,
CustomerMarket,MPNId,PartnerName,PartnerLocation,PartnerAttachType,PartnerHierarchy,PaidAvailableUnits,
MonthlyActiveUsers,AADPPaidAvailableUnits,IntunePaidAvailableUnits,AzipPaidAvailableUnits,
AADPMonthlyActiveUsers,IntuneMonthlyActiveUsers,AzipMonthlyActiveUsers FROM EMSUsage TIMESPAN LAST_6_MONTHS
```

## <a name="competency-performance-requirement-report"></a><span data-ttu-id="f5d82-140">Informe de requisitos de rendimiento de competencia</span><span class="sxs-lookup"><span data-stu-id="f5d82-140">Competency Performance requirement report</span></span>

<span data-ttu-id="f5d82-141">Informe competencyPeformanceRequirement durante seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-141">CompetencyPeformanceRequirement report for six months</span></span>

<span data-ttu-id="f5d82-142">Id. de consulta: `3a0e1adc-f5c1-42ac-9422-8e944bf81ae5`</span><span class="sxs-lookup"><span data-stu-id="f5d82-142">Query ID: `3a0e1adc-f5c1-42ac-9422-8e944bf81ae5`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-143">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-143">Report query</span></span>

```sql
SELECT CompetencyName,CompetencyAttainmentOptionName,Month,MetricName,MetricMonthlyContribution,TTMAggregate,
AnniversaryYearAggregate,GoldThreshold,SilverThreshold 
FROM CompetencyPeformanceRequirement 
TIMESPAN LAST_6_MONTHS
```

## <a name="cloud-products-reseller-performance"></a><span data-ttu-id="f5d82-144">Rendimiento del revendedor de productos en la nube</span><span class="sxs-lookup"><span data-stu-id="f5d82-144">Cloud products reseller performance</span></span>

### <a name="report-description"></a><span data-ttu-id="f5d82-145">Descripción del informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-145">Report description</span></span>

<span data-ttu-id="f5d82-146">Informe CloudProductsResellerPerformance durante seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-146">CloudProductsResellerPerformance report for six months</span></span>

<span data-ttu-id="f5d82-147">Id. de consulta: `c09c2eda-861b-4664-8ee8-48a14745a26a`</span><span class="sxs-lookup"><span data-stu-id="f5d82-147">Query ID: `c09c2eda-861b-4664-8ee8-48a14745a26a`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-148">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-148">Report query</span></span>

```sql
SELECT ResellerMpnid,ResellerName,ResellerMarket,IndirectProviderMPNId,IndirectProviderName,Month,Product,
SubscriptionID,AvailableSeats,AssignedSeats,BilledRevenueUSD,CustomerName,CustomerTPid,CustomerSegment,
CustomerMarket,ResellerStatus 
FROM CloudProductsResellerPerformance TIMESPAN LAST_6_MONTHS
```

## <a name="clas-agreement-renewal-propensity"></a><span data-ttu-id="f5d82-149">Propensidad de renovación del contrato DE CLAS</span><span class="sxs-lookup"><span data-stu-id="f5d82-149">CLAS Agreement Renewal propensity</span></span>

<span data-ttu-id="f5d82-150">Informe CLASAgreementRenewalsPropensity durante seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-150">CLASAgreementRenewalsPropensity report for six months</span></span>

<span data-ttu-id="f5d82-151">Id. de consulta: `c4fc87ac-4cca-44cd-bf4d-835ac513f9ee`</span><span class="sxs-lookup"><span data-stu-id="f5d82-151">Query ID: `c4fc87ac-4cca-44cd-bf4d-835ac513f9ee`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-152">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-152">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,HasGoogle,HasAWS,AzureCluster,D365FOCluster,D365CECluster,D365BCCluster,
M365Cluster,LicenseProgram,AgreementID,AgreementEndDate,ExpirationType,ExpiringRevenue,HasEA,HasOpen,
AzureUpsellCustomer,M365UpsellCustomer,RevSumDivisionName 
FROM CLASAgreementRenewalsPropensity
```

## <a name="clas-azure-propensity"></a><span data-ttu-id="f5d82-153">Propensidad de Azure de CLAS</span><span class="sxs-lookup"><span data-stu-id="f5d82-153">CLAS Azure propensity</span></span>

<span data-ttu-id="f5d82-154">Informe de CLASAzurePropensity durante seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-154">CLASAzurePropensity report for six months</span></span>

<span data-ttu-id="f5d82-155">Id. de consulta: `9a18bd70-8f90-4bd2-8266-5f6e453e3ee7`</span><span class="sxs-lookup"><span data-stu-id="f5d82-155">Query ID: `9a18bd70-8f90-4bd2-8266-5f6e453e3ee7`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-156">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-156">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,MigrateEOSWinServerWithCLASPropensityAbove5Licenses,
MigrateEOSWinServerWithCLASPropensityBelow5Licenses,
MigrateEOSWinServerWithoutCLASPropensityAbove5Licenses,
MigrateEOSWinServerWithoutCLASPropensityBelow5Licenses,MigrateEOSSQLWithCLASPropensityAbove5Licenses,
MigrateEOSSQLWithCLASPropensityBelow5Licenses,MigrateEOSSQLWithoutCLASPropensityAbove5Licenses,
MigrateEOSSQLWithoutCLASPropensityBelow5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithCLASPropensityAbove5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithCLASPropensityBelow5Licenses,
MigrateOnPremWinServerCurrentWindowsServerWithoutCLASPropensityAbove5Licenses,
MigrateOnPremWinServerCurrentWindowsServerIBWithoutCLASPropensityBelow5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithCLASPropensityAbove5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithCLASPropensityBelow5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithoutCLASPropensityAbove5Licenses,
MigrateToAzureSQLOrSQLVMsCurrentSQLServerWithoutCLASPropensityBelow5Licenses,MigrateOSSMigrateToOSSDB,
MigrateOSSLinuxOnAzure,MigrateSAPOnAzure,MigrateWVDRDSIB,MigrateWVDCrossSellModernWorkToAzureWVD,
MigrateVMWareIB,MigrateCitrixIB,InnovateAnalyticsPowerBIIBWithHighAzurepropensity,
EnableDevOpsWithGitHubVisualStudioMSDNIB,WinServerStandardVersion,WinServerStandardLicense,
WinServerDataCenterVersion,WinServerDataCenterLicense,AzureFit,AzureIntent,AzureCluster,
WindowsServerDataCenter_HasOpenRenewal,WindowsServerStandard_HasOpenRenewal,AzureUpsellCustomer,HasGoogle,
HasAWS,HasEA,HasOpen 
FROM CLASAzurePropensity
```

## <a name="clas-d365-propensity"></a><span data-ttu-id="f5d82-157">Propiedad de CLAS D365</span><span class="sxs-lookup"><span data-stu-id="f5d82-157">CLAS D365 propensity</span></span>

<span data-ttu-id="f5d82-158">Informe CLASD365Propensity durante seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-158">CLASD365Propensity report for six months</span></span>

<span data-ttu-id="f5d82-159">Id. de consulta: `258fdcac-6e9c-4072-af27-b1b3d97be16c`</span><span class="sxs-lookup"><span data-stu-id="f5d82-159">Query ID: `258fdcac-6e9c-4072-af27-b1b3d97be16c`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-160">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-160">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,ActivateDigitalSellingM365SeatSizeAbove25SeatsSalesProPropensityModel,
ActivateDigitalSellingD365SalesProPropensityActNowOrEvaluate,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseNavisionBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseAXFAndOPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseGreatPlainsBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseSolomonBCPropensityModel,
ManagingFinancialRiskAndFraudDynamicsOnPremInstallBaseOthersBCPropensityModel,
ManagingFinancialRiskAndFraudNewCustomerAcquisitionFAndOPropensityModel,
ManagingFinancialRiskAndFraudNewCustomerAcquisitionBCPropensityModel,
BuildAgileBusinessProcessesDynamicsOnPremInstallBaseAXGPSLNAVOtherD365PropensityModel,
BuildAgileBusinessProcessesDynamicsCompeteBaseMendixOutsystemsSalesforceD365PropensityModel,
BuildAgileBusinessProcessesD365FAndOInstallBase,BuildAgileBusinessProcessesD365BCInstallBase,
BuildAgileBusinessProcessesD365CEInstallBase,
BuildaResilientSupplyChainWinandActivateFirstD365WorkloadasD365SupplyChainwithNonOracleSAPERPCustomers,
BuildaResilientSupplyChainCrossSellD365SupplyChainANDORRetailCommercetoExistingD365CECustomers,
BuildaResilientSupplyChainCrossSellD365SupChainANDORRetailCommercetoD365CEANDOracleORSAP,D365BCCluster,
D365BCFit,D365BCIntent,D365FOCluster,D365FOFit,D365FOIntent,D365CECluster,D365CEFit,D365CEIntent,
DynamicsOnPremAXorCRM_HasOpenRenewal,M365UpsellCustomer,HasGoogle,HasAWS,HasEA,HasOpen 
FROM CLASD365Propensity
```

## <a name="clas-m365-propensity"></a><span data-ttu-id="f5d82-161">Propiedad de CLAS M365</span><span class="sxs-lookup"><span data-stu-id="f5d82-161">CLAS M365 propensity</span></span>

<span data-ttu-id="f5d82-162">Informe CLASM365Propensity durante seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-162">CLASM365Propensity report for six months</span></span>

<span data-ttu-id="f5d82-163">Id. de consulta: `fbe00e32-fdde-4465-b3e4-41bbd021a130`</span><span class="sxs-lookup"><span data-stu-id="f5d82-163">Query ID: `fbe00e32-fdde-4465-b3e4-41bbd021a130`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-164">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-164">Report query</span></span>

```sql
SELECT MPNID,PartnerName,CustomerID,DUNSNumber,AccountName,Domain,OrgSize,Industry,Vertical,Area,Subsidiary,
SalesTerritory,City,State,PostalCode,Country,Segment,SubSegment,SMCTypeSummary,TopUnmanagedComputeBase,
TopUnmanagedUserBase,IsNonProfit,EnableRemoteWorkTargetExchangeOnline,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithoutCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionCurrentVersionwithoutCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithCLASPropensityBelow10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithoutCLASPropensityAbove10Licenses,
EnableRemoteWorkOnPremAcquisitionEOSwithoutCLASPropensityBelow10Licenses,
EnableRemoteWorkHighPropensityProspectforM365ActNowEvaluate,EnableRemoteWorkCompeteZoomwithM365,
EnableRemoteWorkCompeteZoomwithoutM365,ReduceCostandManageM365E3targetedforM365E5,
ReduceCostandManageM365BBandBScustomerstargetedforM365BP,TransformOrganizationalProductivitySurfacePropensity,
M365Cluster,M365Fit,M365Intent,SurfaceCluster,SurfaceFit,SurfaceIntent,O365Cluster,O365Fit,O365Intent,
M365UpsellCustomer,HasGoogle,HasAWS,HasEA,HasOpen 
FROM CLASM365Propensity
```

## <a name="teams-usage-3p-apps"></a><span data-ttu-id="f5d82-165">Teams Uso de aplicaciones 3P</span><span class="sxs-lookup"><span data-stu-id="f5d82-165">Teams Usage 3P Apps</span></span>

<span data-ttu-id="f5d82-166">Informe teamsUsage3PApps durante seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-166">TeamsUsage3PApps report for six months</span></span>

<span data-ttu-id="f5d82-167">Id. de consulta: `42d287be-cc76-4109-a066-f3140ad97fe2`</span><span class="sxs-lookup"><span data-stu-id="f5d82-167">Query ID: `42d287be-cc76-4109-a066-f3140ad97fe2`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-168">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-168">Report query</span></span>

```sql
SELECT CustomerId,CustomerTenantId,CustomerName,CustomerCountry,DateKey,AppName,UserCount 
FROM TeamsUsage3PApps TIMESPAN LAST_6_MONTHS
```

## <a name="teams-usage-workload"></a><span data-ttu-id="f5d82-169">Teams de trabajo de uso</span><span class="sxs-lookup"><span data-stu-id="f5d82-169">Teams usage workload</span></span>

<span data-ttu-id="f5d82-170">Informe TeamsUsageWorkload durante seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-170">TeamsUsageWorkload report for six months</span></span>

<span data-ttu-id="f5d82-171">Id. de consulta: `817fe875-acb0-4c45-9201-b7a35a60235a`</span><span class="sxs-lookup"><span data-stu-id="f5d82-171">Query ID: `817fe875-acb0-4c45-9201-b7a35a60235a`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-172">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-172">Report query</span></span>

```sql
SELECT CustomerId,CustomerTenantId,MonthKey,SubWorkload,DesktopUsers,WebUsers,MobileUsers,AllUpPartiticipants
FROM TeamsUsageWorkload TIMESPAN LAST_6_MONTHS
```

## <a name="teams-usage-meetings-and-calls"></a><span data-ttu-id="f5d82-173">Teams y llamadas de uso</span><span class="sxs-lookup"><span data-stu-id="f5d82-173">Teams usage meetings and calls</span></span>

<span data-ttu-id="f5d82-174">Informe TeamsUsageMeetingsAndCalls durante seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-174">TeamsUsageMeetingsAndCalls report for six months</span></span>

<span data-ttu-id="f5d82-175">Id. de consulta: `b7bd73a8-47e8-4c57-b915-445708cfd7bf`</span><span class="sxs-lookup"><span data-stu-id="f5d82-175">Query ID: `b7bd73a8-47e8-4c57-b915-445708cfd7bf`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-176">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-176">Report query</span></span>

```sql
SELECT CustomerId,CustomerTenantId,DateKey,SubWorkload,MeetingCount,MeetingDuration 
FROM TeamsUsageMeetingsAndCalls TIMESPAN LAST_6_MONTHS
```

## <a name="competency-summary-history"></a><span data-ttu-id="f5d82-177">Historial de resumen de competencias</span><span class="sxs-lookup"><span data-stu-id="f5d82-177">Competency summary history</span></span>

<span data-ttu-id="f5d82-178">Informe CompetencySummaryHistory durante seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-178">CompetencySummaryHistory report for six months</span></span>

<span data-ttu-id="f5d82-179">Id. de consulta: `fddab2aa-523d-47f6-90fe-588557306db4`</span><span class="sxs-lookup"><span data-stu-id="f5d82-179">Query ID: `fddab2aa-523d-47f6-90fe-588557306db4`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-180">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-180">Report query</span></span>

```sql
SELECT CompetencyName,CompetencyLevel,CompetencyStatus,CompetencyStartDate,CompetencyEndDate 
FROM CompetencySummaryHistory TIMESPAN LAST_6_MONTHS
```

## <a name="training-completion"></a><span data-ttu-id="f5d82-181">Finalización del entrenamiento</span><span class="sxs-lookup"><span data-stu-id="f5d82-181">Training completion</span></span>

<span data-ttu-id="f5d82-182">Informe de finalizaciones de entrenamiento durante seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-182">Training Completions report for six months</span></span>

<span data-ttu-id="f5d82-183">Id. de consulta: `20f5da57-3c2a-481b-b6a0-ec34d6db14e2`</span><span class="sxs-lookup"><span data-stu-id="f5d82-183">Query ID: `20f5da57-3c2a-481b-b6a0-ec34d6db14e2`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-184">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-184">Report query</span></span>

```sql
SELECT TrainingActivityId,TrainingTitle,TrainingType,AADUserId,TrainingCompletionDate,Month,IcMCP,MCPID,MPNId,
PartnerName,PartnerCityLocation,PartnerCountryLocation 
FROM TrainingCompletions TIMESPAN LAST_6_MONTHS
```

## <a name="microsoft-learn"></a><span data-ttu-id="f5d82-185">Microsoft Learn</span><span class="sxs-lookup"><span data-stu-id="f5d82-185">Microsoft Learn</span></span>

<span data-ttu-id="f5d82-186">Microsoft Learn informe de los últimos seis meses</span><span class="sxs-lookup"><span data-stu-id="f5d82-186">Microsoft Learn report for the last six months</span></span>

<span data-ttu-id="f5d82-187">Id. de consulta: `0e06c7c3-75ab-4cd5-8178-8cf1a2de49cc`</span><span class="sxs-lookup"><span data-stu-id="f5d82-187">Query ID: `0e06c7c3-75ab-4cd5-8178-8cf1a2de49cc`</span></span>

### <a name="report-query"></a><span data-ttu-id="f5d82-188">Consulta de informe</span><span class="sxs-lookup"><span data-stu-id="f5d82-188">Report query</span></span>

```sql
SELECT UserName,UserId,TrainingName,TrainingType,Products,Roles,CompletionDate,MPNId,PartnerName,CustomerMarket 
FROM MSLearn TIMESPAN LAST_6_MONTHS
```

## <a name="next-steps"></a><span data-ttu-id="f5d82-189">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="f5d82-189">Next steps</span></span>

- [<span data-ttu-id="f5d82-190">API para acceder a los datos de análisis de Conclusiones de asociados</span><span class="sxs-lookup"><span data-stu-id="f5d82-190">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
- [<span data-ttu-id="f5d82-191">Aplicación de ejemplo para acceder a los datos de análisis de Partner Insights</span><span class="sxs-lookup"><span data-stu-id="f5d82-191">Sample application for accessing partner insights analytics data</span></span>](insights-programmatic-sample-application.md)