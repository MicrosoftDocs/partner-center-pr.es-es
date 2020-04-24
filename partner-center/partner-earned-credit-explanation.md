---
title: Crédito obtenido del partner por los servicios administrados (versión preliminar) | Centro de partners
ms.topic: article
ms.date: 10/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtén información acerca de cómo se calculan y pagan los créditos obtenidos del partner de Microsoft para los servicios administrados y cómo asegurarte de que cumples los requisitos.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: 776fea7eea91e15f872021356562af05e89f1fcf
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2020
ms.locfileid: "75005004"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Cómo se calcula y paga el crédito que obtiene el partner

**Roles adecuados**
-   Administrador global
-   Administrador de usuarios
-   Agente de administrador
-   Administrador de facturación
-   Agente de ventas

El crédito obtenido del partner para los servicios administrados (PEC) reconoce y recompensa a aquellos partners que poseen el control operativo de TI las 24 horas del día los 7 días de la semana, y la administración de ciertas partes o de todo el entorno de Azure de sus clientes. De manera predeterminada, en CSP, a los partners se les otorgan los derechos de acceso necesarios a la suscripción del cliente, lo que les permite realizar una administración operativa las 24 horas y los 7 días de la semana, además de controlar los recursos de la suscripción. En la siguiente sección se describen formas adicionales mediante las cuales el cliente puede proporcionar acceso al partner con el que realizará la transacción. El importe de la factura mensual es al cantidad neta del crédito obtenido del partner. Los partners pueden ver los detalles del PEC en su archivo de conciliación mensual. Para conocer formas adicionales en las que el cliente puede proporcionar acceso al partner con el que realizará la transacción, consulta [Administración de suscripciones y recursos del plan de Azure](azure-plan-manage.md).

Lee también [Restablecer los privilegios de administrador para las suscripciones de Azure CSP](revoke-reinstate-csp.md)

## <a name="important-eligibility-and-calculation-information"></a>Información importante sobre la idoneidad y el cálculo

- El partner debe tener un acuerdo de MPN activo y un rol de RBAC válido para recibir el crédito obtenido para los activos de Azure que administra. 

- En el caso de proveedores indirectos y sus revendedores indirectos, el proveedor indirecto será apto para PEC si el proveedor indirecto, el revendedor indirecto o ambos tienen el control operativo y la administración de los recursos de Azure del cliente en CSP las 24 horas y los 7 días de la semana.

- El valor de PEC está asociado al consumo facturado (de pago) de los servicios de Azure del cliente en CSP y que administra el partner. Asimismo, este valor de PEC está disponible solo para partners en CSP y que factura Microsoft (proveedor indirecto y partners de facturación directa). 

- Servicios válidos: El crédito obtenido del partner se aplica a los servicios enumerados en los [precios de consumo del plan de Azure](https://partner.microsoft.com/commerce/sales) que los partners pueden exportar desde la página de **precios del plan de Azure**. Ten en cuenta que hay excepciones que incluyen, sin limitación, productos de terceros identificados como **Tercero** en la columna **Etiquetas** de la lista de precios de consumo del plan de Azure y las reservas del plan de Azure, y productos de la lista de precios del Marketplace.

- El PEC se calcula a diario y se puede ver en el archivo de uso diario y en el archivo de conciliación de facturas mensuales. Un partner (proveedor indirecto o revendedor indirecto) debe tener acceso durante todo el día (24x7) para asegurarse de obtener el valor del PEC.  

- El valor del PEC se obtiene en el nivel de recursos de Azure. Si el partner tiene acceso válido a la suscripción o al nivel del grupo de recursos, cada recurso que desempeñe hasta la entidad superior obtendrá el PEC.  

- Los detalles del PEC también estarán disponibles en [Azure Cost Management](https://go.microsoft.com/fwlink/?linkid=2106482)

## <a name="azure-cost-management"></a>Azure Cost Management

 Azure Cost Management (ACM) con Análisis de costos te permite, como partner, ver los costos que han recibido el beneficio del PEC.  

1. En Azure Portal, inicia sesión en el inquilino del partner y selecciona **Cost Management + facturación**.
2.  Selecciona **Cost Management**.
3.  Selecciona **Análisis de costos**.

La vista Análisis de costos mostrará los costos de la cuenta de facturación para todos los servicios adquiridos y consumidos con los precios que paga a Microsoft.

4.  Selecciona **PartnerEarnedCreditApplied** en el menú desplegable de un gráfico dinámico para ver los costos que tienen el PEC aplicado. Si la propiedad propiedad **PartnerEarnedCreditApplied** es True, el costo asociado tiene la ventaja del crédito obtenido del partner. 

Si la propiedad PartnerEarnedCreditApplied es False, el costo asociado no cumple los requisitos necesarios para el crédito o el servicio adquirido no es apto para el crédito obtenido por el partner.

Nota: Normalmente, el uso de los servicios tarda de 8 a 24 horas en aparecer en **Cost Management** y los créditos de PEC aparecerán en 48 horas desde el momento del acceso en Azure Cost Management.

5. También puedes agrupar y filtrar por la propiedad **PartnerEarnedCreditApplied** con las características de filtro **Agrupar por y Agregar** características de filtro para desglosar los costos que tienen el PEC aplicado y los que no lo tienen.

 **Para más información**

- [Créditos obtenidos del partner: introducción](partner-earned-credit.md)

- En la lista de precios puedes encontrar ejemplos detallados de los cálculos de créditos obtenidos del partner, a los que puedes acceder a través del panel del Centro de partners (es necesario iniciar sesión).

- [Cambiar al plan de Azure: introducción](azure-plan-get-started.md)

- [Administrar suscripciones y recursos en el plan de Azure](azure-plan-manage.md)

- [Restablecer los privilegios de administrador para las suscripciones de Azure CSP](revoke-reinstate-csp.md)

