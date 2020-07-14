---
title: Usar el análisis del centro de partners para Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo ver los datos empresariales con la aplicación de análisis del centro de partners para Power BI (para asociados directos en CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 248527fdbc536c552f7b2d00f208838b4ef19085
ms.sourcegitcommit: 0a6b1e6d845391539f54213efff00af4d23f028c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/14/2020
ms.locfileid: "86302291"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Vea los datos empresariales con la aplicación de análisis del centro de partners para Microsoft Power BI

**Se aplica a**

- Centro de partners

**Roles adecuados**

- Administrador global
- Administrador de usuarios
- Agente de ventas
- Agente de administrador

## <a name="view-your-business-data"></a>Visualización de los datos empresariales

Obtenga una representación visual de los datos empresariales con la aplicación del centro de partners para Power BI, entre las que se incluyen:

- Crecimiento de la base de clientes, las suscripciones y las licencias

- El uso que se hace de productos de Office 365, Microsoft Dynamics y Microsoft Azure

- Las unidades de consumo diarias de cada recurso limitado en cada suscripción de Azure durante los últimos 60 días

- Costo estimado (basado en la última carta de tarifa)

- Capacidad de exportar conjuntos de valores y crear informes personalizados, incluidos por cliente.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Acerca de la versión preliminar de la aplicación de análisis de Partner Center

- Esta aplicación es para asociados directos solo en el programa proveedor de soluciones en la nube. Otros asociados de CSP (por ejemplo, los revendedores indirectos) no podrán iniciar sesión.

- Los costos estimados son los datos de facturación y facturación previas a los impuestos y no son legalmente vinculantes. Los costos estimados están pensados para usarse solo para información de datos.

- La información del cliente se basa en las suscripciones. Los clientes que hayan creado recientemente cuentas para, pero que aún no tienen suscripciones, no se incluyen en los recuentos.

- El costo estimado se basa en la tarjeta de tarifas más reciente, que se basa en los precios de CSP.

- Los días son días del calendario.

### <a name="business-insights-report"></a>Informe de Business Insights

- **Inquilinos de cliente**: el número de distintos inquilinos de Azure ad de clientes que han adquirido suscripciones.

- **Nuevo (últimos 30 días)**: nuevos clientes que compran al menos una suscripción en los últimos 30 días

- **Renovación (últimos 30 días)**: clientes sin ninguna suscripción "activa", "en período de gracia" o "deshabilitado"

- **Nuevo (últimas 24 horas)**: nuevos clientes que compran al menos una suscripción en las últimas 24 horas

- **Costo mensual estimado en los últimos 12 meses**: tendencia de mes a mes del importe de dólar estimado de la factura anterior a los impuestos que se suma mensualmente durante el período de los últimos 12 meses

- **Costo estimado por producto en los últimos 12 meses**: productos vendidos ordenados por importe en dólares estimado de la factura de impuestos previos agregada en el período de los últimos 12 meses. Este estado indica los principales productos que aportan más ingresos.

- **Clientes de más de 12 meses**: tendencia de mes a mes de nuevos clientes y renovación de clientes agregados mensualmente durante el período de los últimos 12 meses

- **Costo estimado por cliente durante los últimos 12 meses**: clientes ordenados por importe de dólar estimado de factura previa de impuestos en el período de los últimos 12 meses. Este estado indica que los clientes principales aportan más ingresos.

- **Recuento de clientes por producto**: productos vendidos ordenados por clientes asociados. Este estado indica los principales productos que se venden a la mayoría de los clientes.

### <a name="subscription-insights-report"></a>Informe de información de suscripción

- **Estado**de la suscripción:

- Active: suscripciones que pertenecen a un estado "activo" o "en período de gracia"

  - Suspendido: suscripciones que pertenecen al estado "deshabilitado"

  - Desaprovisionado: suscripciones que pertenecen al estado "desaprovisionado" o "expirado"

- **Estado de expiración**:

  - Expired: suscripciones que ya han expirado (donde la fecha de finalización de la suscripción está en el pasado)

  - Expiración después de 30 días: suscripciones que expirarán después de 30 días (donde la fecha de finalización de la suscripción es posterior a los 30 días)

  - Expiración en 30 días: suscripciones que expirarán en los próximos 30 días (donde la fecha de finalización de la suscripción está entre hoy y los próximos 30 días)

- **Total de suscripciones**: suscripciones en estado "activo", "en período de gracia" o "deshabilitado"

- **Nuevo (últimos 30 días)**: nuevas suscripciones compradas por los clientes en los últimos 30 días

- **Nuevo (últimas 24 horas)**: nuevas suscripciones adquiridas por los clientes en las últimas 24 horas

- **Expiración en 30 días**: suscripciones que expirarán en los próximos 30 días

- **Renovación (últimos 30 días)**: las suscripciones que se han desaprovisionado o suspendido (deshabilitado) en los últimos 30 días

- **Distribución por tipos de suscripción**:% distribución de suscripciones totales por licencia y tipo de suscripción basado en el uso

- **Número de suscripciones activas por producto**: productos vendidos ordenados por recuento de suscripciones activas

- **Suscripciones en los últimos 12 meses**: tendencia de mes a mes de nuevas suscripciones y suscripciones de renovación agregadas mensualmente durante el período de los últimos 12 meses

- **Detalles**de la suscripción del cliente: vista detallada de los clientes, las suscripciones y las ofertas

### <a name="license-insights-report"></a>Informe de información de licencias:

- **Total de licencias**: número total de licencias agregadas en todas las suscripciones basadas en licencias

- **Nuevo (últimos 30 días)**: adición de licencias en los últimos 30 días

- **Renovación (últimos 30 días)**: reducción de la licencia en los últimos 30 días

- **Nuevo (últimas 24 horas)**: adición de licencias en las últimas 24 horas

- **Licencias en los últimos 90 días**: tendencia de mes a mes de adiciones y reducciones de licencias agregadas mensualmente durante el período de los últimos 90 días

- **Recuento de licencias activas por producto**: productos vendidos ordenados por recuento de licencias activas

- **Recuento de licencias activas por cliente**: clientes ordenados por recuento de licencias activas

- **Detalles de evento de licencia de cliente en los últimos 90 días**: vista detallada de los clientes, las suscripciones y los eventos de suscripción, incluida la fecha del evento, el nombre del evento, la cantidad y el cambio en la cantidad.

### <a name="licenses-usage-report"></a>Informe de uso de licencias:

- **Licencias asignadas por producto**: productos vendidos ordenados por número de asignación de licencias

- **Licencias en uso por producto**: productos vendidos ordenados por recuento de uso de licencias

- **Distribución de clientes con licencias asignadas**:% distribución de los clientes totales rotos en cubos del 20% según la asignación de licencias%

- **Distribución del cliente de licencias en uso**:% distribución de los clientes totales rotos en cubos del 20% por uso de licencias%

- **Licencias asignadas por el cliente**: vista detallada de licencias vendidas y licencias asignadas por clientes y productos

- **Licencias en uso por el cliente**: vista detallada de licencias vendidas y licencias en uso por clientes y productos

### <a name="azure-insights-report"></a>Informe de Azure Insights:

- **Clientes basados en el uso durante los últimos 12 meses**: tendencia de mes a mes de nuevos clientes basados en el uso y de clientes basados en el uso renovados que se han agregado mensualmente durante el período de los últimos 12 meses

- **Suscripciones basadas en el uso en los últimos 12 meses**: tendencia de mes a mes de nuevas suscripciones basadas en el uso y suscripciones basadas en el uso renovadas que se agregan mensualmente durante el período de los últimos 12 meses

- **Costo estimado de uso por cliente durante los últimos 60 días**: clientes basados en el uso ordenados por importe de dólar estimado de factura previa de impuestos en el período de los últimos 60 días. Este estado indica que los clientes principales basados en el uso aportan la mayor parte de los ingresos

- **Costo estimado de uso por Categoría en los últimos 60 días**: categorías de medida de las suscripciones basadas en el uso ordenadas por importe de dólar estimado de la factura de impuestos previos agregada en el período de los últimos 60 días.

- **Costo estimado de uso por suscripción en los últimos 60 días**: las suscripciones basadas en el uso por importe en dólares estimado de la factura de impuestos previos sumadas en el período de los últimos 60 días.

- **Costo de uso estimado del cliente por presupuesto de gasto**: clientes ordenados por porcentaje de su presupuesto de gasto de uso actual que supera el umbral (100%).

### <a name="azure-resource-usage-report"></a>Informe de uso de recursos de Azure:

- **Uso de recursos de Azure por día para el período seleccionado**: unidades de consumo diarias para cada recurso medido en cada suscripción basada en el uso para el período seleccionado en los últimos 60 días.

- **Costo de uso estimado de los recursos de Azure para el período seleccionado**: costo estimado basado en la última tarjeta de frecuencia para cada recurso medido en cada suscripción basada en el uso para el período seleccionado en los últimos 60 días. 

## <a name="next-steps"></a>Pasos siguientes

- [Información general de la aplicación de análisis del centro de partners para Power BI](power-bi-app-for-direct-partners.md)

- [Instalación y versión preliminar de la Aplicación de análisis del Centro de partners para Microsoft Power BI](power-bi-app-for-direct-partners-install.md)
