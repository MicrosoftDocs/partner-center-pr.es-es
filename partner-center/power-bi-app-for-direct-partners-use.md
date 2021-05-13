---
title: Uso de Centro de partners Analytics para Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo ver los datos empresariales mediante el Aplicación de análisis del Centro de partners para Power BI (para asociados directos en CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 96fe57f6e89928a69051c2e201c444882500b844
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855036"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a><span data-ttu-id="1d96c-103">Visualización de los datos empresariales con la aplicación Centro de partners Analytics para Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="1d96c-103">View your business data with the Partner Center Analytics app for Microsoft Power BI</span></span>



<span data-ttu-id="1d96c-104">**Roles adecuados:** administrador global | Administrador de administración de | Agente de ventas | Agente de administración</span><span class="sxs-lookup"><span data-stu-id="1d96c-104">**Appropriate roles**: Global admin | User management admin | Sales agent | Admin agent</span></span>

## <a name="view-your-business-data"></a><span data-ttu-id="1d96c-105">Visualización de los datos empresariales</span><span class="sxs-lookup"><span data-stu-id="1d96c-105">View your business data</span></span>

<span data-ttu-id="1d96c-106">Obtenga una representación visual de los datos empresariales con el Aplicación de análisis del Centro de partners para Power BI, incluidos:</span><span class="sxs-lookup"><span data-stu-id="1d96c-106">Get a visual representation of your business data with the Partner Center Analytics app for Power BI, including:</span></span>

- <span data-ttu-id="1d96c-107">Crecimiento de la base de clientes, suscripciones y licencias</span><span class="sxs-lookup"><span data-stu-id="1d96c-107">Growth of your customer base, subscriptions, and licenses</span></span>

- <span data-ttu-id="1d96c-108">El uso que se hace de productos de Office 365, Microsoft Dynamics y Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="1d96c-108">Usage of Office 365, Microsoft Dynamics, and Microsoft Azure products</span></span>

- <span data-ttu-id="1d96c-109">Las unidades de consumo diarias de cada recurso limitado en cada suscripción de Azure durante los últimos 60 días</span><span class="sxs-lookup"><span data-stu-id="1d96c-109">Daily consumption units for each metered resource in each Azure subscription for the last 60 days</span></span>

- <span data-ttu-id="1d96c-110">Costo estimado (basado en la tarjeta de tarifa más reciente)</span><span class="sxs-lookup"><span data-stu-id="1d96c-110">Estimated cost (based on latest rate card)</span></span>

- <span data-ttu-id="1d96c-111">Capacidad de exportar conjuntos de datos y crear informes personalizados, incluidos por cliente.</span><span class="sxs-lookup"><span data-stu-id="1d96c-111">Ability to export datasets and create custom reports, including per customer.</span></span>

### <a name="about-the-partner-center-analytics-app-preview-release"></a><span data-ttu-id="1d96c-112">Acerca de la versión preliminar de Centro de partners Analytics</span><span class="sxs-lookup"><span data-stu-id="1d96c-112">About the Partner Center Analytics app preview release</span></span>

- <span data-ttu-id="1d96c-113">Esta aplicación es solo para asociados directos Proveedor de soluciones en la nube programa.</span><span class="sxs-lookup"><span data-stu-id="1d96c-113">This app is for direct partners in the Cloud Solution Provider program only.</span></span> <span data-ttu-id="1d96c-114">Otros asociados de CSP (revendedores indirectos, por ejemplo) no podrán iniciar sesión.</span><span class="sxs-lookup"><span data-stu-id="1d96c-114">Other partners in CSP (indirect resellers, for example) will not be able to sign in.</span></span>

- <span data-ttu-id="1d96c-115">Los costos estimados son datos de facturación o factura previas a impuestos y no son legalmente obligatorios.</span><span class="sxs-lookup"><span data-stu-id="1d96c-115">Any estimated costs are pre-tax billing / invoice data, and are not legally binding.</span></span> <span data-ttu-id="1d96c-116">Los costos estimados están diseñados para usarse solo para la información de datos.</span><span class="sxs-lookup"><span data-stu-id="1d96c-116">Estimated costs are meant to be used for data insights only.</span></span>

- <span data-ttu-id="1d96c-117">La información del cliente se basa en las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="1d96c-117">Customer information is based on subscriptions.</span></span> <span data-ttu-id="1d96c-118">Los clientes para los que ha creado recientemente cuentas, pero que aún no tienen suscripciones, no se incluyen en los recuentos.</span><span class="sxs-lookup"><span data-stu-id="1d96c-118">Any customers that you've recently created accounts for, but who don't yet have subscriptions, aren't included in counts.</span></span>

- <span data-ttu-id="1d96c-119">El costo estimado se basa en la tarjeta de tarifa más reciente, que se basa en los precios de CSP.</span><span class="sxs-lookup"><span data-stu-id="1d96c-119">Estimated cost is based on latest rate card, which is based on CSP pricing.</span></span>

- <span data-ttu-id="1d96c-120">Los días son días naturales.</span><span class="sxs-lookup"><span data-stu-id="1d96c-120">Days are calendar days.</span></span>

### <a name="business-insights-report"></a><span data-ttu-id="1d96c-121">Información de la empresa informe</span><span class="sxs-lookup"><span data-stu-id="1d96c-121">Business Insights report</span></span>

- <span data-ttu-id="1d96c-122">**Inquilinos de clientes:** número de inquilinos Azure AD inquilinos de clientes que han adquirido suscripciones</span><span class="sxs-lookup"><span data-stu-id="1d96c-122">**Customer tenants**: Number of distinct Azure AD tenants of customers that have purchased subscriptions</span></span>

- <span data-ttu-id="1d96c-123">**Nuevo (últimos 30 días):** nuevos clientes que compran al menos una suscripción en los últimos 30 días</span><span class="sxs-lookup"><span data-stu-id="1d96c-123">**New (last 30 days)**: New customers purchasing at least one subscription in last 30 days</span></span>

- <span data-ttu-id="1d96c-124">**Renovación (últimos 30 días):** clientes sin suscripciones "activas", "en gracia" o "deshabilitadas".</span><span class="sxs-lookup"><span data-stu-id="1d96c-124">**Churn (last 30 days)**: Customers without any “active", “in grace" or “disabled" subscriptions</span></span>

- <span data-ttu-id="1d96c-125">**Nuevo (últimas 24 horas):** nuevos clientes que compran al menos una suscripción en las últimas 24 horas</span><span class="sxs-lookup"><span data-stu-id="1d96c-125">**New (last 24 hours)**: New customers purchasing at least one subscription in last 24 hours</span></span>

- <span data-ttu-id="1d96c-126">Costo mensual estimado durante los últimos **12** meses: tendencia mensual del importe estimado en dólares de factura previa a impuestos agregado mensualmente durante el período de los últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="1d96c-126">**Estimated monthly cost over last 12 months**: Month over month trend of estimated pre-tax invoice dollar amount aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="1d96c-127">Costo estimado por producto en los últimos **12** meses: los productos vendidos se ordenan según el importe estimado en dólares de factura previa a impuestos agregado durante el período de los últimos 12 meses.</span><span class="sxs-lookup"><span data-stu-id="1d96c-127">**Estimated cost by product over last 12 months**: Products sold sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="1d96c-128">Este estado indica los productos principales que más ingresos tienen.</span><span class="sxs-lookup"><span data-stu-id="1d96c-128">This status indicates top products bringing most revenue.</span></span>

- <span data-ttu-id="1d96c-129">**Clientes de los últimos 12** meses: tendencia mensual de nuevos clientes y clientes de renovación agregados mensualmente durante el período de los últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="1d96c-129">**Customers over last 12 months**: Month over month trend of new customers and churn customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="1d96c-130">Costo estimado por cliente durante los últimos **12** meses: los clientes se ordenan por importe estimado en dólares de factura antes de impuestos agregado durante el período de los últimos 12 meses.</span><span class="sxs-lookup"><span data-stu-id="1d96c-130">**Estimated cost by customer over last 12 months**: Customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 12 months.</span></span> <span data-ttu-id="1d96c-131">Este estado indica que los principales clientes traen la mayoría de los ingresos.</span><span class="sxs-lookup"><span data-stu-id="1d96c-131">This status indicates top customers bringing most revenue.</span></span>

- <span data-ttu-id="1d96c-132">**Recuento de clientes por producto:** productos vendidos ordenados por clientes asociados.</span><span class="sxs-lookup"><span data-stu-id="1d96c-132">**Customer count by product**: Products sold sorted by associated customers.</span></span> <span data-ttu-id="1d96c-133">Este estado indica los principales productos vendidos a la mayoría de los clientes.</span><span class="sxs-lookup"><span data-stu-id="1d96c-133">This status indicates top products sold to most customers.</span></span>

### <a name="subscription-insights-report"></a><span data-ttu-id="1d96c-134">Informe de Subscription Insights</span><span class="sxs-lookup"><span data-stu-id="1d96c-134">Subscription Insights report</span></span>

- <span data-ttu-id="1d96c-135">**Estado de la suscripción:**</span><span class="sxs-lookup"><span data-stu-id="1d96c-135">**Subscription status**:</span></span>

- <span data-ttu-id="1d96c-136">Activo: suscripciones que pertenecen al estado "activo" o "en gracia".</span><span class="sxs-lookup"><span data-stu-id="1d96c-136">Active: Subscriptions belonging to either “active" or “in grace" state</span></span>

  - <span data-ttu-id="1d96c-137">Suspendido: suscripciones que pertenecen al estado "deshabilitado"</span><span class="sxs-lookup"><span data-stu-id="1d96c-137">Suspended: Subscriptions belonging to “disabled" state</span></span>

  - <span data-ttu-id="1d96c-138">Desaprovisionado: suscripciones que pertenecen al estado "desaprovisionado" o "expirado"</span><span class="sxs-lookup"><span data-stu-id="1d96c-138">De-provisioned: Subscriptions belonging to “de-provisioned" or “expired" status</span></span>

- <span data-ttu-id="1d96c-139">**Estado de expiración:**</span><span class="sxs-lookup"><span data-stu-id="1d96c-139">**Expiry status**:</span></span>

  - <span data-ttu-id="1d96c-140">Expirado: suscripciones que ya han expirado (donde la fecha de finalización de la suscripción es anterior)</span><span class="sxs-lookup"><span data-stu-id="1d96c-140">Expired: Subscriptions that have already expired (where subscription end date is in past)</span></span>

  - <span data-ttu-id="1d96c-141">Expiración después de 30 días: suscripciones que expirarán después de 30 días (donde la fecha de finalización de la suscripción es posterior a los 30 días siguientes)</span><span class="sxs-lookup"><span data-stu-id="1d96c-141">Expiring after 30 days: Subscriptions that will expire after 30 days (where subscription end date is after next 30 days)</span></span>

  - <span data-ttu-id="1d96c-142">Expiración en 30 días: suscripciones que expirarán en los próximos 30 días (donde la fecha de finalización de la suscripción está entre hoy y los próximos 30 días)</span><span class="sxs-lookup"><span data-stu-id="1d96c-142">Expiring in 30 days: Subscriptions that will expire within next 30 days (where subscription end date is between today and next 30 days)</span></span>

- <span data-ttu-id="1d96c-143">**Total de suscripciones:** suscripciones en estado "activo", "en gracia" o "deshabilitado"</span><span class="sxs-lookup"><span data-stu-id="1d96c-143">**Total subscriptions**: Subscriptions in “active," “in grace" or “disabled" status</span></span>

- <span data-ttu-id="1d96c-144">**Nuevo (últimos 30 días):** nuevas suscripciones adquiridas por los clientes en los últimos 30 días</span><span class="sxs-lookup"><span data-stu-id="1d96c-144">**New (last 30 days)**: New subscriptions purchased by customers within last 30 days</span></span>

- <span data-ttu-id="1d96c-145">**Nuevo (últimas 24 horas):** nuevas suscripciones adquiridas por los clientes en las últimas 24 horas</span><span class="sxs-lookup"><span data-stu-id="1d96c-145">**New (last 24 hours)**: New subscriptions purchased by customers within last 24 hours</span></span>

- <span data-ttu-id="1d96c-146">**Expiración en 30 días:** suscripciones que expirarán en los próximos 30 días</span><span class="sxs-lookup"><span data-stu-id="1d96c-146">**Expiring in 30 days**: Subscriptions that will expire within next 30 days</span></span>

- <span data-ttu-id="1d96c-147">**Renovación (últimos 30 días):** suscripciones que se han desaprovisionado o suspendido (deshabilitado) en los últimos 30 días</span><span class="sxs-lookup"><span data-stu-id="1d96c-147">**Churn (last 30 days)**: Subscriptions that have been de-provisioned or Suspended (disabled) within last 30 days</span></span>

- <span data-ttu-id="1d96c-148">**Distribución por tipos de suscripción:**% de distribución del total de suscripciones por tipo de suscripción basada en licencia y por uso</span><span class="sxs-lookup"><span data-stu-id="1d96c-148">**Distribution by subscription types**: % distribution of total subscriptions by License based and usage-based subscription type</span></span>

- <span data-ttu-id="1d96c-149">**Recuento de suscripciones activas por producto:** productos vendidos ordenados por recuento de suscripciones activas</span><span class="sxs-lookup"><span data-stu-id="1d96c-149">**Active subscription count by product**: Products sold sorted by active subscriptions count</span></span>

- <span data-ttu-id="1d96c-150">**Suscripciones de los últimos 12** meses: tendencia mes a mes de nuevas suscripciones y suscripciones de renovación agregadas mensualmente durante el período de los últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="1d96c-150">**Subscriptions over last 12 months**: Month over month trend of new subscriptions and churn subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="1d96c-151">**Detalles de la suscripción del** cliente: vista detallada de los clientes, suscripciones y ofertas</span><span class="sxs-lookup"><span data-stu-id="1d96c-151">**Customer subscription details**: Detailed view of the customers, subscriptions, and offers</span></span>

### <a name="license-insights-report"></a><span data-ttu-id="1d96c-152">Informe de License Insights:</span><span class="sxs-lookup"><span data-stu-id="1d96c-152">License Insights report:</span></span>

- <span data-ttu-id="1d96c-153">**Total de licencias:** número total de licencias agregadas en todas las suscripciones basadas en licencias</span><span class="sxs-lookup"><span data-stu-id="1d96c-153">**Total licenses**: Total number of licenses aggregated across all license-based subscriptions</span></span>

- <span data-ttu-id="1d96c-154">**Nuevo (últimos 30 días):** adición de licencias en los últimos 30 días</span><span class="sxs-lookup"><span data-stu-id="1d96c-154">**New (last 30 days)**: License addition within last 30 days</span></span>

- <span data-ttu-id="1d96c-155">**Renovación (últimos 30 días):** reducción de licencias en los últimos 30 días</span><span class="sxs-lookup"><span data-stu-id="1d96c-155">**Churn (last 30 days)**: License reduction within last 30 days</span></span>

- <span data-ttu-id="1d96c-156">**Nuevo (últimas 24 horas):** adición de licencias en las últimas 24 horas</span><span class="sxs-lookup"><span data-stu-id="1d96c-156">**New (last 24 hours)**: License addition within last 24 hours</span></span>

- <span data-ttu-id="1d96c-157">**Licencias de los últimos 90** días: tendencia mes a mes de adiciones y reducciones de licencias agregadas mensualmente durante el período de los últimos 90 días</span><span class="sxs-lookup"><span data-stu-id="1d96c-157">**Licenses over last 90 days**: Month over month trend of license additions and reductions aggregated monthly over the period of last 90 days</span></span>

- <span data-ttu-id="1d96c-158">**Recuento de licencias activas por producto:** productos vendidos ordenados por recuento de licencias activas</span><span class="sxs-lookup"><span data-stu-id="1d96c-158">**Active license count by product**: Products sold sorted by active license count</span></span>

- <span data-ttu-id="1d96c-159">**Número de licencias activas por cliente:** clientes ordenados por recuento de licencias activas</span><span class="sxs-lookup"><span data-stu-id="1d96c-159">**Active license count by customer**: Customers sorted by active license count</span></span>

- <span data-ttu-id="1d96c-160">Detalles del evento de licencia del cliente durante los últimos **90** días: vista detallada de los clientes, las suscripciones y los eventos de suscripción, incluida la fecha del evento, el nombre del evento, la cantidad y el cambio en la cantidad.</span><span class="sxs-lookup"><span data-stu-id="1d96c-160">**Customer license event details over last 90 days**: Detailed view of the customers, subscriptions, and subscription events including event date, event name, quantity, and change in quantity.</span></span>

### <a name="licenses-usage-report"></a><span data-ttu-id="1d96c-161">Informe de uso de licencias:</span><span class="sxs-lookup"><span data-stu-id="1d96c-161">Licenses Usage report:</span></span>

- <span data-ttu-id="1d96c-162">**Licencias asignadas por producto: productos vendidos ordenados** por recuento de asignaciones de licencias</span><span class="sxs-lookup"><span data-stu-id="1d96c-162">**Licenses assigned by product**: Products sold sorted by license assignment count</span></span>

- <span data-ttu-id="1d96c-163">**Licencias en uso por producto: productos vendidos ordenados** por recuento de uso de licencias</span><span class="sxs-lookup"><span data-stu-id="1d96c-163">**Licenses in use by product**: Products sold sorted by license usage count</span></span>

- <span data-ttu-id="1d96c-164">**Distribución por cliente de licencias asignadas:**% de distribución del total de clientes divididos en cubos del intervalo del 20 % por % de asignación de licencias</span><span class="sxs-lookup"><span data-stu-id="1d96c-164">**Customer distribution of licenses assigned**: % distribution of total customers broken in buckets of 20% range by license assignment %</span></span>

- <span data-ttu-id="1d96c-165">**Distribución por cliente de licencias en uso:**% de distribución del total de clientes divididos en cubos del intervalo del 20 % por porcentaje de uso de licencias</span><span class="sxs-lookup"><span data-stu-id="1d96c-165">**Customer distribution of licenses in use**: % distribution of total customers broken in buckets of 20% range by license usage %</span></span>

- <span data-ttu-id="1d96c-166">**Licencias asignadas por el cliente:** vista detallada de las licencias vendidas y las licencias asignadas por clientes y productos</span><span class="sxs-lookup"><span data-stu-id="1d96c-166">**Licenses assigned by customer**: Detailed view of licenses sold and licenses assigned by customers and products</span></span>

- <span data-ttu-id="1d96c-167">**Licencias en uso por parte del cliente:** vista detallada de las licencias vendidas y las licencias en uso por clientes y productos</span><span class="sxs-lookup"><span data-stu-id="1d96c-167">**Licenses in use by customer**: Detailed view of licenses sold and licenses in use by customers and products</span></span>

### <a name="azure-insights-report"></a><span data-ttu-id="1d96c-168">Informe de Azure Insights:</span><span class="sxs-lookup"><span data-stu-id="1d96c-168">Azure Insights report:</span></span>

- <span data-ttu-id="1d96c-169">Clientes basados en el uso en los últimos **12** meses: tendencia mes a mes de nuevos clientes basados en el uso y clientes basados en el uso renovación agregados mensualmente durante el período de los últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="1d96c-169">**Usage-based customers over last 12 months**: Month over month trend of new usage-based customers and churned usage-based customers aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="1d96c-170">Suscripciones basadas en el uso en los últimos **12** meses: tendencia mensual de nuevas suscripciones basadas en el uso y suscripciones basadas en el uso renovación agregadas mensualmente durante el período de los últimos 12 meses</span><span class="sxs-lookup"><span data-stu-id="1d96c-170">**Usage-based subscriptions over last 12 months**: Month over month trend of new usage-based subscriptions and churned usage-based subscriptions aggregated monthly over the period of last 12 months</span></span>

- <span data-ttu-id="1d96c-171">Costo estimado de uso por cliente durante los últimos **60** días: los clientes basados en el uso se ordenan por el importe estimado de la factura antes de impuestos agregado durante el período de los últimos 60 días.</span><span class="sxs-lookup"><span data-stu-id="1d96c-171">**Estimated cost of usage by customer over last 60 days**: Usage-based customers sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span> <span data-ttu-id="1d96c-172">Este estado indica que los principales clientes basados en el uso traen la mayoría de los ingresos.</span><span class="sxs-lookup"><span data-stu-id="1d96c-172">This status indicates top usage-based customers bringing most revenue</span></span>

- <span data-ttu-id="1d96c-173">Costo estimado de uso por categoría en los últimos **60** días: categorías de medidores de suscripciones basadas en el uso ordenadas por importe estimado en dólares de factura antes de impuestos agregado durante el período de los últimos 60 días.</span><span class="sxs-lookup"><span data-stu-id="1d96c-173">**Estimated cost of usage by category over last 60 days**: Meter categories of usage-based subscriptions sorted by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="1d96c-174">Costo estimado de uso por suscripción durante los últimos **60** días: suscripciones basadas en el uso por importe estimado de dólares de factura previa a impuestos agregado durante el período de los últimos 60 días.</span><span class="sxs-lookup"><span data-stu-id="1d96c-174">**Estimated cost of usage by subscription over last 60 days**: Usage-based subscriptions by estimated pre-tax invoice dollar amount aggregated over the period of last 60 days.</span></span>

- <span data-ttu-id="1d96c-175">**Costo de uso estimado por el cliente por presupuesto** de gasto: los clientes ordenados por porcentaje de su presupuesto de gasto de uso actual supera el umbral (100 %).</span><span class="sxs-lookup"><span data-stu-id="1d96c-175">**Customer estimated usage cost by spending budget**: Customers sorted by percentage of their current usage spending budget exceeding threshold (100%).</span></span>

### <a name="azure-resource-usage-report"></a><span data-ttu-id="1d96c-176">Informe de uso de recursos de Azure:</span><span class="sxs-lookup"><span data-stu-id="1d96c-176">Azure Resource Usage report:</span></span>

- <span data-ttu-id="1d96c-177">**Uso de recursos de Azure** por día durante el período seleccionado: unidades de consumo diarias para cada recurso de uso de cada suscripción basada en el uso durante el período seleccionado en los últimos 60 días.</span><span class="sxs-lookup"><span data-stu-id="1d96c-177">**Usage of Azure resources by day for selected period**: Daily consumption units for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span>

- <span data-ttu-id="1d96c-178">**Costo** de uso estimado de los recursos de Azure para el período seleccionado: costo estimado basado en la tarjeta de tarifa más reciente para cada recurso de uso de cada suscripción basada en el uso durante el período seleccionado en los últimos 60 días.</span><span class="sxs-lookup"><span data-stu-id="1d96c-178">**Estimated usage cost of Azure resources for selected period**: Estimated cost based on latest rate card for each metered resource in each usage-based subscription for selected period within the last 60 days.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="1d96c-179">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="1d96c-179">Next steps</span></span>

- [<span data-ttu-id="1d96c-180">Centro de partners Analytics for Power BI introducción a la aplicación</span><span class="sxs-lookup"><span data-stu-id="1d96c-180">Partner Center Analytics for Power BI app overview</span></span>](power-bi-app-for-direct-partners.md)

- [<span data-ttu-id="1d96c-181">Instalación y versión preliminar de la Aplicación de análisis del Centro de partners para Microsoft Power BI</span><span class="sxs-lookup"><span data-stu-id="1d96c-181">Install and preview the Partner Center Analytics app for Microsoft Power BI</span></span>](power-bi-app-for-direct-partners-install.md)
