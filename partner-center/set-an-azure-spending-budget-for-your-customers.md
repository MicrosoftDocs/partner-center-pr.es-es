---
title: Establecer un presupuesto de gasto de Azure para los clientes
ms.topic: how-to
ms.date: 06/03/2020
description: Obtenga información acerca de cómo establecer o quitar los presupuestos de gastos mensuales de Azure para los clientes y también ver los datos de gasto de Azure y establecer notificaciones relacionadas con el presupuesto.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e311af31bbce65ed38c20df12243d325c7a63d04
ms.sourcegitcommit: 7beb7327472dc1b0c07c101d121196fb2830bbf8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/01/2020
ms.locfileid: "96438984"
---
# <a name="set-check-or-remove-monthly-azure-spending-budgets-for-customers-in-partner-center"></a>Establecer, comprobar o quitar los presupuestos de gastos mensuales de Azure para los clientes del centro de Partners

Se aplica a:

- Centro de partners
- Centro de partners para Microsoft Cloud for US Government

Puede [establecer un presupuesto de gasto de Azure mensual para sus clientes en el](#set-azure-spending-budget) centro de Partners. Esto ayuda a los clientes a administrar sus gastos de Azure. Esta opción permite comparar el gasto de Azure de los clientes con el presupuesto durante el mes. También ayuda a los clientes a presupuestar sus gastos de Azure, por lo que su factura mensual no es más alta de lo previsto.

> [!NOTE]  
> Esta característica no está disponible en las cuentas de espacio aislado o prueba en producción (TIP).

Después de [establecer un presupuesto de gasto de Azure para los clientes](#set-azure-spending-budget), también puede revisar el uso del cliente de las siguientes maneras. Estas opciones pueden ayudarle a detectar servicios mal configurados o tendencias inusuales que podrían sugerir fraudes. Después, puede trabajar con los clientes para identificar la causa principal y administrar los costos. Si es necesario, también puede [cambiar el presupuesto del cliente](#set-azure-spending-budget) a una cantidad mayor.

- [Comprobar los gastos actuales de Azure](#check-current-azure-spending)

- [Activar las notificaciones por correo electrónico cuando el gasto del cliente está a punto de su límite de presupuesto](#notifications-for-budget-limits)

- [Visualización de los costos inventariados por servicio para las suscripciones basadas en el uso](#itemized-costs-by-service)

También puede [quitar un presupuesto de gasto de Azure](#remove-azure-spending-budget) para los clientes en cualquier momento.

## <a name="azure-spending-data"></a>Datos de gasto de Azure

Los datos de gasto de Azure son una *estimación* y los *importes de facturación reales pueden variar*. El valor de los datos *no refleja* impuestos, créditos, ajustes u otros cargos que puedan aplicarse.

Los datos de gasto se *actualizan una vez al día*. Los clientes pueden seguir usando (y se le cobrará por) servicios y recursos de Azure, a menos que cambie la configuración de su cuenta en el Azure Portal.

## <a name="set-azure-spending-budget"></a>Establecer el presupuesto de gasto de Azure

Puede *establecer un presupuesto de gasto de Azure mensual* para varios clientes en el centro de Partners:

1. Inicie sesión en el [panel del centro de Partners](https://partner.microsoft.com/dashboard/).

2. En el menú de la izquierda, en **CSP**, elija **gasto de Azure**.

3. En la página **gasto de Azure** , en **clientes con suscripciones de Microsoft Azure**, seleccione los clientes para los que desea establecer un presupuesto.

4. Escriba un valor para **presupuesto mensual**.

5. Elija **aplicar** para guardar los cambios.

También puede *establecer un presupuesto para un cliente individual* en su configuración de suscripción:

1. Inicia sesión en el panel del Centro de partners.

2. En el menú de la izquierda, en **CSP**, elija **clientes**.

3. En la página **clientes** , seleccione el nombre de la **empresa** del cliente.

4. En la página **suscripciones** del cliente, en **suscripción basada** en el uso, elija **cambiar presupuesto**.

5. Escriba un valor para el presupuesto.

6. Elija **aplicar** para guardar los cambios.

## <a name="remove-azure-spending-budget"></a>Quitar el presupuesto de gasto de Azure

Puede *quitar un presupuesto mensual de gastos de Azure* para los clientes del centro de Partners:

1. Inicie sesión en el [panel del centro de Partners](https://partner.microsoft.com/dashboard/).

2. En el menú de la izquierda, en **CSP**, elija **gasto de Azure**.

3. En la página **gasto de Azure** , en **clientes con suscripciones de Microsoft Azure**, seleccione los clientes cuyo presupuesto desea quitar.

4. Elija **quitar presupuesto**.

## <a name="check-current-azure-spending"></a>Comprobar los gastos actuales de Azure

Puede *realizar un seguimiento de los gastos mensuales y del gasto actual de Azure* en cualquier momento:

1. Inicie sesión en el [panel del centro de Partners](https://partner.microsoft.com/dashboard/).

2. En el menú de la izquierda, en **CSP**, elija **gasto de Azure**.

3. En la página **gasto de Azure** , en **clientes con suscripciones de Microsoft Azure**, puede ver una visión general de los presupuestos mensuales de los clientes, las estimaciones de gastos actuales y el porcentaje de presupuesto usado.

## <a name="notifications-for-budget-limits"></a>Notificaciones para los límites de presupuesto

Puede *activar las notificaciones por correo electrónico* para cuando el gasto mensual del cliente esté cerca del límite de presupuesto. Al activar esta opción, se le notificará cuando los clientes usen un 80% o más de su presupuesto mensual. Esta opción le ayuda a estar atento a la factura de Azure. Para configurar notificaciones por correo electrónico:

1. Inicie sesión en el Centro de datos.

2. Vaya a **Configuración**.

3. Seleccione **mis preferencias**.

4. Si no lo ha hecho, configure una dirección de correo electrónico preferida.

5. Configure el idioma preferido para la notificación.

6. Seleccione la pestaña **CSP** en la sección **preferencias de notificación** .

7. Compruebe la opción de correo electrónico para la notificación de **gasto de Azure** y **guárdela**.


## <a name="itemized-costs-by-service"></a>Costos inventariados por servicio

Puede *ver los costos calculados (y el uso estimado) por servicio para las suscripciones basadas en el uso*:

1. Inicie sesión en el Centro de datos.

2. En el menú de la izquierda, en **CSP**, elija **clientes**.

3. En la página **clientes** , seleccione el nombre de la **empresa** del cliente.

4. En la página **suscripciones** del cliente, en **suscripciones basadas** en el uso, seleccione el nombre de la **suscripción**.

5. En la página de la suscripción, puede revisar los **costos** calculados por servicio y el **uso estimado** para el mes en curso.
