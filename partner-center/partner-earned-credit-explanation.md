---
title: Créditos obtenidos del partner para servicios administrados
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo se calculan y pagan los créditos obtenidos del partner (PEC) de Microsoft para los servicios administrados y cómo asegurarse de que cumple los requisitos.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 3acc078b3de3c0443ee64fdaaba2d486d9c466c8
ms.sourcegitcommit: e9066768ab8e242c03f0a7e3ce460ae8cd2e3fda
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/17/2020
ms.locfileid: "97622174"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Cómo se calcula y paga el crédito que obtiene el partner

**Roles adecuados**

- Administrador global
- Administrador de usuarios
- Agente de administrador
- Administrador de facturación
- Agente de ventas

El crédito obtenido del partner para los servicios administrados (PEC) reconoce y recompensa a aquellos partners que poseen el control operativo de TI las 24 horas del día los 7 días de la semana, y la administración de ciertas partes o de todo el entorno de Azure de sus clientes. De manera predeterminada, en CSP, a los partners se les otorgan los derechos de acceso necesarios a la suscripción del cliente, lo que les permite realizar una administración operativa las 24 horas y los 7 días de la semana, además de controlar los recursos de la suscripción. En la siguiente sección se describen formas adicionales mediante las cuales el cliente puede proporcionar acceso al partner con el que realizará la transacción. El importe de la factura mensual es al cantidad neta del crédito obtenido del partner. Los partners pueden ver los detalles del PEC en su archivo de conciliación mensual. Para conocer formas adicionales en las que el cliente puede proporcionar acceso al partner con el que realizará la transacción, consulta [Administración de suscripciones y recursos del plan de Azure](azure-plan-manage.md).

Lee también [Restablecer los privilegios de administrador para las suscripciones de Azure CSP](revoke-reinstate-csp.md)

## <a name="eligibility"></a>Elegibilidad

Para recibir los créditos obtenidos por los partners (PEC), se aplican los requisitos siguientes: 

- Debe tener un contrato de MPN activo y un rol de control de acceso basado en rol (RBAC) válido para recibir el crédito obtenido para los activos de Azure que administra.

- Debe tener la administración y el control operativo ininterrumpidos de los recursos de Azure del cliente en CSP. Esto significa que debe tener privilegios de administrador en la suscripción de Azure del cliente, el grupo de recursos de Azure y el recurso de Azure. En el caso de proveedores indirectos y sus revendedores indirectos, el proveedor indirecto será apto para PEC si el proveedor indirecto, el revendedor indirecto o ambos tienen este control operativo. Para obtener más información al respecto, consulte [Restablecer los privilegios de administrador para las suscripciones del programa CSP de Azure](https://docs.microsoft.com/partner-center/revoke-reinstate-csp).

- Además de los requisitos anteriores, los PEC solo se aplican a los servicios enumerados en los precios de consumo del plan de Azure, que se pueden exportar desde la página de [precios del plan de Azure](https://partner.microsoft.com/commerce/sales).

- Los PEC **no** se pueden aplicar a los servicios siguientes:
    - Reservas del plan de Azure.
    - Productos de terceros identificados como Terceros en la columna Etiquetas del precio de consumo del plan de Azure.
    - Productos en la lista de precios de Marketplace.
    - [Máquinas virtuales de Azure Spot](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- El valor del PEC se obtiene en el nivel de recursos de Azure. Si tiene acceso válido a la suscripción o al nivel del grupo de recursos, cada recurso que se acumule hasta la entidad superior obtendrá PEC.

- Los detalles sobre los PEC también están disponibles en la página de [Azure Cost Management](https://docs.microsoft.com/azure/cost-management-billing/costs/get-started-partners).

### <a name="calculation"></a>Cálculo

El PEC se calcula a diario y se puede ver en el archivo de uso diario y en el archivo de conciliación de facturas mensuales. Un partner (proveedor indirecto o revendedor indirecto) debe tener acceso durante todo el día (24x7) para asegurarse de obtener el valor del PEC. El valor de PEC se calcula a diario a partir de los recursos de Azure administrados. El valor máximo de PEC para un período de facturación determinado (mes) es del 15 %. Los partners que conservan el acceso con privilegios persistentes a lo largo del mes (intervalo de acceso) y para todos los recursos aplicables (ámbito de acceso) obtienen un valor de PEC completo del 15 %. La reducción del ámbito y el intervalo generan una tasa de PEC inferior para el mes. El archivo de uso de valoración diaria muestra a diario si se aplica el valor de PEC para un recurso de Azure. Los partners también pueden inscribirse para recibir alertas en caso de cambio en el acceso con privilegios persistentes.

## <a name="azure-cost-management"></a>Azure Cost Management

Azure Cost Management (ACM) con Análisis de costos te permite, como partner, ver los costos que han recibido el beneficio del PEC.  

1. En [Azure Portal](https://portal.azure.com), inicie sesión en su inquilino de partner y seleccione **Administración de costos + facturación**.

2. Selecciona **Cost Management**.

3. Selecciona **Análisis de costos**.

   La vista Análisis de costos mostrará los costos de la cuenta de facturación para todos los servicios adquiridos y consumidos con los precios que paga a Microsoft.

4. Selecciona **PartnerEarnedCreditApplied** en el menú desplegable de un gráfico dinámico para ver los costos que tienen el PEC aplicado. Si la propiedad propiedad **PartnerEarnedCreditApplied** es True, el costo asociado tiene la ventaja del crédito obtenido del partner. 

   Si la propiedad PartnerEarnedCreditApplied es False, el costo asociado no cumple los requisitos necesarios para el crédito o el servicio adquirido no es apto para el crédito obtenido por el partner.

   >[!NOTE] 
   >Normalmente, el uso de los servicios tarda de 8 a 24 horas en aparecer en **Cost Management** y los créditos de PEC aparecerán en 48 horas desde el momento del acceso en Azure Cost Management.

5. También puedes agrupar y filtrar por la propiedad **PartnerEarnedCreditApplied** con las características de filtro **Agrupar por y Agregar** características de filtro para desglosar los costos que tienen el PEC aplicado y los que no lo tienen.

## <a name="next-steps"></a>Pasos siguientes

- [Créditos obtenidos del partner: introducción](partner-earned-credit.md)

- En la lista de precios puedes encontrar ejemplos detallados de los cálculos de créditos obtenidos del partner, a los que puedes acceder a través del panel del Centro de partners (es necesario iniciar sesión).

- [Cambiar al plan de Azure: introducción](azure-plan-get-started.md)

- [Administrar suscripciones y recursos en el plan de Azure](azure-plan-manage.md)

- [Revocación o restablecimiento de los privilegios de administrador para las suscripciones del programa CSP de Azure](revoke-reinstate-csp.md)
