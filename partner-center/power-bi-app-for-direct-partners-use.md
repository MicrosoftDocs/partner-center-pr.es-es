---
title: Uso de Centro de partners Analytics para Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo ver los datos empresariales mediante Aplicación de análisis del Centro de partners para Power BI (para asociados directos en el programa Proveedor de soluciones en la nube (CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 95eb018a3284d2de98c0ce6a9cd0ce6299d5571a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/24/2021
ms.locfileid: "112564988"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Vea los datos empresariales con la aplicación Centro de partners Analytics para Microsoft Power BI



**Roles adecuados:** Administrador global | Administrador de usuarios | Agente de ventas | Agente de administración

## <a name="view-your-business-data"></a>Visualización de los datos empresariales

Obtenga una representación visual de los datos empresariales con la aplicación Centro de partners Analytics para Microsoft Power BI, incluidos:

- Crecimiento de la base de clientes, suscripciones y licencias

- El uso que se hace de productos de Office 365, Microsoft Dynamics y Microsoft Azure

- Las unidades de consumo diarias de cada recurso limitado en cada suscripción de Azure durante los últimos 60 días

- Costo estimado (basado en la tarjeta de tarifa más reciente)

- Capacidad de exportar conjuntos de datos y crear informes personalizados, incluidos por cliente.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Acerca de la versión preliminar de Centro de partners Analytics

- Esta aplicación es solo para asociados directos del programa Proveedor de soluciones en la nube (CSP). Otros asociados de CSP (revendedores indirectos, por ejemplo) no podrán iniciar sesión.

- Los costos estimados son datos de facturación o factura antes de impuestos y no son legalmente obligatorios. Los costos estimados están diseñados para usarse solo para la información de datos.

- La información del cliente se basa en las suscripciones. Los clientes para los que haya creado cuentas recientemente, pero que aún no tengan suscripciones, no se incluyen en los recuentos.

- El costo estimado se basa en la tarjeta de tarifa más reciente, que se basa en los precios de CSP.

- Los días son días naturales.

### <a name="business-insights-report"></a>Información de la empresa informe

- **Inquilinos de** clientes: número de inquilinos Azure Active Directory (Azure AD) de clientes que han adquirido suscripciones

- **Nuevo (últimos 30 días):** nuevos clientes que compran al menos una suscripción en los últimos 30 días

- **Renovación (últimos 30 días):** clientes sin suscripciones "activas", "en gracia" o "deshabilitadas".

- **Nuevo (últimas 24 horas):** nuevos clientes que compran al menos una suscripción en las últimas 24 horas

- Costo mensual estimado durante los últimos **12** meses: tendencia mensual del importe estimado en dólares de factura previa a impuestos agregado mensualmente durante el período de los últimos 12 meses

- Costo estimado por producto en los últimos **12** meses: los productos vendidos se ordenan según el importe estimado de la factura antes de impuestos agregado durante el período de los últimos 12 meses. Este estado indica los productos principales que más ingresos tienen.

- **Clientes de los últimos 12** meses: tendencia mensual de nuevos clientes y clientes de renovación agregados mensualmente durante el período de los últimos 12 meses

- Costo estimado por cliente durante los últimos **12** meses: los clientes se ordenan por el importe estimado de la factura antes de impuestos agregado durante el período de los últimos 12 meses. Este estado indica que los principales clientes traen la mayoría de los ingresos.

- **Recuento de clientes por producto:** productos vendidos ordenados por clientes asociados. Este estado indica los principales productos vendidos a la mayoría de los clientes.

### <a name="subscription-insights-report"></a>Informe de Subscription Insights

- **Estado de la suscripción:**

- Activo: suscripciones que pertenecen al estado "activo" o "en gracia".

  - Suspendido: suscripciones que pertenecen al estado "deshabilitado"

  - Desaprovisionado: suscripciones que pertenecen al estado "desaprovisionado" o "expirado"

- **Estado de expiración:**

  - Expirado: suscripciones que ya han expirado (donde la fecha de finalización de la suscripción es anterior)

  - Expiración después de 30 días: suscripciones que expirarán después de 30 días (donde la fecha de finalización de la suscripción es posterior a los 30 días siguientes)

  - Expiración en 30 días: suscripciones que expirarán en los próximos 30 días (donde la fecha de finalización de la suscripción está entre hoy y los próximos 30 días)

- **Total de suscripciones:** suscripciones en estado "activo", "en gracia" o "deshabilitado"

- **Nuevo (últimos 30 días):** nuevas suscripciones adquiridas por los clientes en los últimos 30 días

- **Nuevo (últimas 24 horas):** nuevas suscripciones adquiridas por los clientes en las últimas 24 horas

- **Expiración en 30 días:** suscripciones que expirarán en los próximos 30 días

- **Renovación (últimos 30 días):** suscripciones que se han desaprovisionado o suspendido (deshabilitado) en los últimos 30 días

- **Distribución por tipos de suscripción:**% de distribución del total de suscripciones por tipo de suscripción basada en licencia y por uso

- **Número de suscripciones activas por producto:** productos vendidos ordenados por recuento de suscripciones activas

- **Suscripciones de los últimos 12** meses: tendencia mensual de nuevas suscripciones y suscripciones de renovación agregadas mensualmente durante el período de los últimos 12 meses

- **Detalles de la suscripción del** cliente: vista detallada de los clientes, suscripciones y ofertas

### <a name="license-insights-report"></a>Informe de License Insights:

- **Total de licencias:** número total de licencias agregadas en todas las suscripciones basadas en licencias

- **Nuevo (últimos 30 días):** adición de licencias en los últimos 30 días

- **Renovación (últimos 30 días):** reducción de licencias en los últimos 30 días

- **Nuevo (últimas 24 horas):** adición de licencias en las últimas 24 horas

- **Licencias de los últimos 90** días: tendencia mensual de adiciones y reducciones de licencias agregadas mensualmente durante el período de los últimos 90 días

- **Número de licencias activas por producto:** productos vendidos ordenados por recuento de licencias activas

- **Número de licencias activas por cliente:** clientes ordenados por recuento de licencias activas

- Detalles del evento de licencia de cliente durante los últimos **90** días: vista detallada de los clientes, suscripciones y eventos de suscripción, incluida la fecha del evento, el nombre del evento, la cantidad y el cambio en la cantidad.

### <a name="licenses-usage-report"></a>Informe de uso de licencias:

- **Licencias asignadas por producto: productos vendidos ordenados** por recuento de asignaciones de licencias

- **Licencias en uso por producto: productos vendidos ordenados** por recuento de uso de licencias

- **Distribución por cliente de licencias asignadas:**% de distribución del total de clientes divididos en cubos del intervalo del 20 % por % de asignación de licencias

- **Distribución por cliente de licencias en uso:**% de distribución del total de clientes divididos en cubos del intervalo del 20 % por porcentaje de uso de licencias

- **Licencias asignadas por el cliente:** vista detallada de las licencias vendidas y las licencias asignadas por clientes y productos

- **Licencias en uso por parte del cliente:** vista detallada de las licencias vendidas y las licencias en uso por clientes y productos

### <a name="azure-insights-report"></a>Informe de Azure Insights:

- Clientes basados en el uso en los últimos **12** meses: tendencia mes a mes de nuevos clientes basados en el uso y clientes basados en el uso renovación agregados mensualmente durante el período de los últimos 12 meses

- Suscripciones basadas en el uso en los últimos **12** meses: tendencia mensual de nuevas suscripciones basadas en el uso y suscripciones basadas en el uso renovación agregadas mensualmente durante el período de los últimos 12 meses

- Costo estimado del uso por el cliente durante los últimos **60** días: los clientes basados en el uso se ordenan por el importe estimado de la factura antes de impuestos agregado durante el período de los últimos 60 días. Este estado indica que los principales clientes basados en el uso traen la mayoría de los ingresos.

- Costo estimado de uso por categoría en los últimos **60** días: categorías de medidores de suscripciones basadas en el uso ordenadas por importe estimado en dólares de factura antes de impuestos agregado durante el período de los últimos 60 días.

- Costo estimado de uso por suscripción durante los últimos **60** días: suscripciones basadas en el uso por importe estimado de dólares de factura previa a impuestos agregado durante el período de los últimos 60 días.

- **Costo de uso estimado por el cliente por presupuesto** de gasto: los clientes ordenados por porcentaje de su presupuesto de gasto de uso actual supera el umbral (100 %).

### <a name="azure-resource-usage-report"></a>Informe de uso de recursos de Azure:

- **Uso de recursos de Azure** por día durante el período seleccionado: unidades de consumo diarias para cada recurso de uso de cada suscripción basada en el uso durante el período seleccionado en los últimos 60 días.

- **Costo** de uso estimado de los recursos de Azure para el período seleccionado: costo estimado basado en la tarjeta de tarifa más reciente para cada recurso de uso de cada suscripción basada en el uso durante el período seleccionado en los últimos 60 días. 

## <a name="next-steps"></a>Pasos siguientes

- [Centro de partners Analytics for Power BI app overview](power-bi-app-for-direct-partners.md)

- [Instalación y versión preliminar de la Aplicación de análisis del Centro de partners para Microsoft Power BI](power-bi-app-for-direct-partners-install.md)
