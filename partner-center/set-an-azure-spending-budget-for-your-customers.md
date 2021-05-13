---
title: Establecer, comprobar o quitar los presupuestos de gastos mensuales de Azure para los clientes del Centro de partners
ms.topic: how-to
ms.date: 03/17/2021
description: Aprenda a establecer o quitar presupuestos de gasto mensuales de Azure para los clientes, así como a ver los datos de gasto de Azure y a establecer notificaciones relacionadas con el presupuesto.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 14e901f51841e58b28a3cbbb1b7a19ce89d7c324
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855359"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Establecer, comprobar o quitar los presupuestos de gastos mensuales de Azure para los clientes de Centro de partners

**Roles adecuados:** Agente de administración

Puede establecer [un presupuesto de gasto mensual de Azure para los clientes](#set-azure-spending-budget) en Centro de partners. Esto ayuda a los clientes a administrar sus gastos de Azure. Esta opción le permite comparar los gastos de Azure de los clientes con el presupuesto durante el mes. También ayuda a los clientes a presupuestar sus gastos de Azure para que su factura mensual no sea mayor de lo previsto.

> [!NOTE]  
> Esta característica no está disponible en cuentas de espacio aislado o prueba en producción (TIP).

Después de [establecer un presupuesto de gastos de Azure](#set-azure-spending-budget)para los clientes, también puede revisar el uso de los clientes de las maneras siguientes. Estas opciones pueden ayudarle a detectar servicios mal configurados o tendencias inusuales que podrían sugerir fraudes. A continuación, puede trabajar con los clientes para identificar la causa principal y administrar los costos. Si es necesario, también puede [cambiar el presupuesto del](#set-azure-spending-budget) cliente a una cantidad mayor.

- [Comprobación de los gastos actuales de Azure](#check-current-azure-spending)

- [Activar las notificaciones por correo electrónico cuando el gasto de un cliente se acerca a su límite de presupuesto](#notifications-for-budget-limits)

- [Visualización de los costos por servicio por servicio para suscripciones basadas en el uso](#itemized-costs-by-service)

También puede quitar [un presupuesto de gastos de Azure](#remove-azure-spending-budget) para los clientes en cualquier momento.

## <a name="azure-spending-data"></a>Datos de gasto de Azure

Los datos de gasto de Azure son *una estimación* y *los importes de facturación reales pueden variar.* El valor de los datos *no refleja los* impuestos, créditos, ajustes u otros cargos que se puedan aplicar.

Los datos de gasto *se actualizan una vez al día.* Los clientes pueden seguir usando (y se les cobrará por) los servicios y recursos de Azure, a menos que cambie la configuración de su cuenta en el Azure Portal.

## <a name="set-azure-spending-budget"></a>Establecer el presupuesto de gastos de Azure

Puede establecer *un presupuesto mensual de gastos de Azure* para varios clientes en Centro de partners:

1. Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).

2. En el menú izquierdo de **CSP,** elija **Gastos de Azure.**

3. En la **página de gastos** de Azure, en Clientes con **Microsoft Azure suscripciones,** seleccione los clientes para los que desea establecer un presupuesto.

4. Escriba un valor para **Presupuesto mensual.**

5. Elija **Aplicar** para guardar los cambios.

También puede establecer *un presupuesto para un cliente individual en* su configuración de suscripción:

1. Inicie sesión en el panel del Centro de partners.

2. En el menú izquierdo de **CSP,** elija **Clientes.**

3. En la **página** Clientes, seleccione el nombre de la compañía **del cliente.**

4. En la página Suscripciones **del** cliente, en Suscripción basada en **uso,** elija **Cambiar presupuesto.**

5. Escriba un valor para el presupuesto.

6. Elija **Aplicar** para guardar los cambios.

## <a name="remove-azure-spending-budget"></a>Eliminación del presupuesto de gastos de Azure

Puede quitar *un presupuesto mensual de gastos de Azure* para los clientes en Centro de partners:

1. Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).

2. En el menú izquierdo de **CSP,** elija **Gastos de Azure.**

3. En la **página Gastos** de Azure, en Clientes **con Microsoft Azure suscripciones,** seleccione los clientes cuyo presupuesto desea quitar.

4. Elija **Quitar presupuesto.**

## <a name="check-current-azure-spending"></a>Comprobación de los gastos actuales de Azure

Puede realizar *un seguimiento de los gastos actuales* de Azure de los clientes y los presupuestos mensuales en cualquier momento:

1. Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).

2. En el menú izquierdo de **CSP,** elija **Gastos de Azure.**

3. En la página de gastos de **Azure,** en Clientes con suscripciones Microsoft Azure **,** puede ver información general sobre los presupuestos mensuales de los clientes, las estimaciones de gasto actuales y el porcentaje de presupuesto usado.

## <a name="notifications-for-budget-limits"></a>Notificaciones de límites de presupuesto

Puede activar *las notificaciones por correo electrónico* cuando el gasto mensual del cliente esté cerca de su límite de presupuesto. Al activar esta opción, se le notificará cuando los clientes usen el 80 % o más de su presupuesto mensual. Esta opción le ayuda a mantenerse al tanto de la factura de Azure. Para configurar notificaciones por correo electrónico:

1. Inicie sesión en el Centro de datos.

2. Vaya a **Configuración**.

3. Seleccione **Mis preferencias.**

4. Configure una dirección de correo electrónico preferida si no lo ha hecho.

5. Configure el idioma preferido para la notificación.

6. Seleccione la **pestaña CSP** en la **sección Preferencias de** notificación.

7. Active la opción Correo electrónico para **la notificación de gasto** de Azure y **Guarde**.


## <a name="itemized-costs-by-service"></a>Costos por servicio por elemento

Puede ver *los costos por elemento (y el uso estimado) por servicio para las suscripciones basadas en el uso:*

1. Inicie sesión en el Centro de datos.

2. En el menú izquierdo de **CSP,** elija **Clientes.**

3. En la **página Clientes,** seleccione el nombre de la **compañía del cliente.**

4. En la página Suscripciones **del** cliente, en Suscripciones basadas en **uso,** seleccione el nombre de la **suscripción**.

5. En la página de la suscripción, puede revisar los costos por servicio y el Uso estimado **del** mes actual. 


## <a name="next-steps"></a>Pasos siguientes

- [Nueva experiencia comercial en CSP: facturación de Azure](azure-plan-billing.md)
