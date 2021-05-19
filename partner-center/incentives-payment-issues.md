---
title: Solución de problemas de pagos y ganancias
ms.topic: article
ms.date: 02/05/2021
description: Obtenga información sobre cómo resolver problemas como pérdidas o ganancias incorrectas, problemas de elegibilidad y cómo conciliar las ganancias de los incentivos.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: 7b67564fbf469ac23ad514d96c3ec7b27bb3a5e6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151957"
---
# <a name="troubleshooting-missing-payments-incorrect-earnings-and-other-issues"></a>Solución de problemas de pagos que faltan, ganancias incorrectas y otros problemas

**Roles adecuados:** Administrador de incentivos

Este artículo le ayudará a resolver las ganancias o problemas de pago del programa de incentivos. Entre los asuntos tratados se incluyen los plazos de pago, la comprobación de la idoneidad de las ganancias y la importancia de configurar correctamente los perfiles fiscales y de pago.

## <a name="who-can-create-or-update-payout-and-tax-profiles-for-my-organization"></a>¿Quién puede crear o actualizar perfiles fiscales y de pago para mi organización?

Los usuarios que tienen el rol de administrador de incentivos en Centro de partners para el programa de incentivos pertinente y la ubicación de MPN pueden actualizar y ver los perfiles fiscales y de pago de la organización.

## <a name="how-long-does-it-take-for-microsoft-to-approve-my-pending-payout-andor-tax-profiles"></a>¿Cuánto tiempo tarda Microsoft en aprobar mis perfiles fiscales o de pago pendientes?

La validación puede tardar hasta 48 horas. Durante este tiempo, el estado del perfil en la página de información general se mostrará como Validating enrollment (Validando inscripción). Una vez completado el proceso, el  estado se mostrará como Inscrito si se realiza correctamente o Acción necesaria: actualizar los detalles de pago o **impuestos** si es necesario.

## <a name="how-do-i-know-if-i-have-completed-my-payout-and-tax-profile-correctly"></a>Cómo saber si he completado mi perfil fiscal y de pago correctamente?

El estado de la inscripción se muestra en la página de información general. Cuando haya terminado de crear los perfiles, su estado será **Validación de la inscripción.** Una vez validada la información, el estado cambia **a Inscrito.** Este estado indica que el perfil fiscal y de pago y la inscripción se han completado correctamente.

## <a name="why-do-i-need-to-update-my-tax-profile-to-use-it-with-a-new-incentive-program"></a>¿Por qué es necesario actualizar mi perfil fiscal para usarlo con un nuevo programa de incentivos?

Pagamos los incentivos de distintas ubicaciones en función del tipo de incentivo. Estas distintas ubicaciones pueden requerir información fiscal adicional, en función de las reglas del programa de incentivos, para procesarse correctamente.

## <a name="how-can-i-delete-a-payment-andor-tax-profile"></a>¿Cómo puedo eliminar un perfil de pago o fiscal?

Microsoft no admite actualmente la posibilidad de eliminar los perfiles fiscales y de pago existentes.

## <a name="my-payment-is-missing-or-incorrect"></a>Falta mi pago o es incorrecto.

Si faltan pagos o son incorrectos, suele deberse a uno de los siguientes motivos:

- **Es posible que no sea apto.**  Las ganancias solo estarán disponibles si se cumplen los requisitos de idoneidad operativa, es decir, estar inscrito en el período de ganancias del programa correspondiente.
- **Es posible que no haya cumplido los requisitos.**  Compruebe si ha cumplido las reglas de ingresos aptos y de elegibilidad para el incentivo que está buscando.

  **Para comprobar su idoneidad**

  1. Inicie sesión en [Incentivos para partners.](https://partner.microsoft.com/membership/partner-incentives)

  2. Desplácese hacia abajo hasta los documentos del programa.
  
  3. Seleccione el vínculo de documento que desee y, a continuación, revise las secciones. 

**Reglas de ingresos aptos** y elegibilidad **de los asociados.**

- **El perfil de pago puede estar incompleto.** La fecha de inicio de sus ingresos de incentivos será el primer día del mes en el que haya completado todos los requisitos de idoneidad, incluida la incorporación con los detalles fiscales y de pago. Los beneficios no estarán disponibles durante los meses anteriores a la finalización fiscal y de pago. Por ejemplo, si completa todos los requisitos durante el mes de abril de 2020, la fecha de inicio de las ganancias será el 1 de abril de 2020.
- **Es posible que tenga una acción pendiente.**  Podría deberse a que los incentivos no se están procesando porque existe una acción pendiente.

  **Para ver las acciones pendientes**

  1. Inicie sesión en [Incentivos para partners.](https://partner.microsoft.com/membership/partner-incentives)
  2. Abra la **página Historial de transacciones.** Revise los campos de esta página para ver las acciones pendientes que se deben completar, como El perfil de impuestos **pendiente,** Perfil de pago pendiente o Envío de **facturas fiscales pendientes.**

Si estas acciones no ayudan y los pagos siguen faltando o son incorrectos, póngase en contacto con el servicio [de soporte técnico.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="how-can-i-reconcile-my-adjustments"></a>¿Cómo puedo conciliar mis ajustes?

Puede buscar y conciliar los ajustes descargando los detalles de ganancias y transacciones.

1. Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).
2. En la barra de navegación superior, seleccione el icono money y, a continuación, seleccione **Historial de transacciones.**
3. Aplique los filtros adecuados. (Consulte la **nota** importante a continuación).
4. Una vez filtrados los datos, seleccione **Iniciar descarga y,** a continuación, **exportar datos.** Los datos se abrirán en un archivo CSV.
5. En el archivo CSV, vaya a Columna P, **Tipo de ganancia**.
6. Filtre esta columna por **Adjustment-Desajuste**. Puede ver el mes de cada ajuste en la columna S.

>[!IMPORTANT]
>Los ajustes aplicados a períodos de ganancias anteriores no serán visibles en las ganancias del mes en el que se aplicó el ajuste. Los ajustes siempre reflejarán en el informe de ganancias del mes al que se aplicó el ajuste.
>
>Por ejemplo, un ajuste de las ganancias de enero de 2019 que se procesó en septiembre de 2019 no reflejará el importe de las ganancias de septiembre de 2019. Sin embargo, cuando se reciba el pago de septiembre de 2019, incluirá el ajuste de enero de 2019 que se aplicó en septiembre. En este escenario, tendría que descargar los detalles de la transacción de enero de 2019 para ver el ajuste que se aplicó.
>
>Tenga esto en cuenta al establecer los filtros de fecha. Como se mencionó anteriormente, los ajustes de períodos anteriores solo estarán visibles en el mes al que se aplicó el ajuste. Compruebe que el intervalo de fechas seleccionado corresponde al mes del ajuste que está intentando localizar. Es posible que tenga que seleccionar **Borrar todo** para quitar los filtros y, a continuación, aplicar otros nuevos.

## <a name="why-are-my-co-op-claim-payments-made-in-two-different-currencies"></a>¿Por qué mis pagos de notificaciones de cooperación se realizan en dos monedas diferentes?

Cuando se obtienen fondos de cooperación de diferentes entidades de Microsoft, los pagos se realizan en la moneda local de cada entidad respectiva.  

## <a name="why-was-i-paid-in-a-currency-other-than-my-co-op-claim-currency"></a>¿Por qué se pagó en una moneda distinta de la moneda de la notificación de cooperación?

Cada programa de incentivos tiene un perfil de banco que se creó durante la instalación. La moneda especificada en ese perfil es la moneda en la que se le pagará.

## <a name="i-dont-see-earnings-for-a-certain-period"></a>No veo ganancias durante un período determinado.

Cuando no ve las ganancias durante un período en el que se esperan, normalmente se debe a uno de los siguientes problemas:

- **Es posible que no sea apto.**  Las ganancias solo estarán disponibles si se cumplen los requisitos de idoneidad operativa, es decir, estar inscrito en el período de ganancias del programa correspondiente.

- **El perfil de pago puede estar incompleto.**  La fecha de inicio de sus ingresos de incentivos será el primer día del mes en el que haya completado todos los requisitos de idoneidad, incluida la incorporación con los detalles fiscales y de pago. Los beneficios no estarán disponibles durante los meses anteriores a la finalización fiscal y de pago. Por ejemplo, si completa todos los requisitos durante el mes de abril de 2020, la fecha de inicio de las ganancias será el 1 de abril de 2020.

Si ha completado los requisitos de idoneidad, incluida la incorporación con detalles fiscales y de pago a tiempo, y aún faltan ganancias, póngase en contacto con el soporte [técnico.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="my-earnings-are-missing-or-incorrect"></a>Mis ganancias faltan o son incorrectas

Los beneficios que faltan o son incorrectos pueden deberse a uno de los siguientes problemas:

- **Es posible que no se hayan cumplido los requisitos.**  Compruebe si ha cumplido las reglas de [elegibilidad](#my-payment-is-missing-or-incorrect) y de ingresos aptas para el incentivo que está buscando.

- **Puede haber una discrepancia.**  Si cumple los requisitos [](incentives-confirm-your-earnings-eligibility.md) [de](incentives-determined-your-program-eligibility.md) idoneidad del programa y de elegibilidad de las ganancias y las ganancias siguen apareciendo incorrectas, la siguiente información puede ayudarle a recuperar los datos.

Las ganancias se muestran tanto en la página **Historial de transacciones** como en **la página Pagos.** Para acceder a ambas páginas, seleccione el icono **pago** en la barra de navegación Centro de partners.

:::image type="content" source="images/incentives/paymenticon.png" alt-text="Información de la transacción":::

Es posible que los importes de ganancias mensuales de la vista Historial de transacciones no se alineen con el importe de pago recibido durante un mes específico. Esto se debe a los recálculos y ajustes de los períodos de ganancias anteriores que se aplican a pagos futuros.

Por ejemplo, un ajuste de las ganancias de enero de 2019 que se procesó en septiembre de 2019 no se reflejará en el importe de las ganancias de septiembre de 2019. sin embargo, cuando se reciba el pago de septiembre de 2019, incluirá el ajuste de enero de 2019 que se aplicó en septiembre.

En este escenario, tendría que descargar los detalles de la transacción para obtener una vista completa de todas las ganancias incluidas en el pago.  Además, puede ir a la vista Pagos para descargar las transacciones de cada pago.

### <a name="transaction-history"></a>Historial de transacciones

Esta vista muestra las tendencias de ganancias y pagos por mes, las ganancias por estado y los detalles de la transacción, junto con el estado de pago de cada transacción. Los datos solo son visibles para los programas y los id. de MPN para los que es un usuario o administrador de incentivos.

### <a name="payments"></a>Pagos

Esta vista le permite ver los pagos de todos los programas y los ID de MPN. Los datos solo son visibles para los programas y los id. de MPN para los que es un usuario o administrador de incentivos. Desde esta vista, puede descargar la remesa o ver los detalles de la transacción mediante pago.

| Para hacer esto | Vaya aquí |
| ------ | :----------- | 
| Ver la información de pago por línea, incluidas las ganancias y los importes de pago en la moneda local  | Consulte el **campo Lista de** pagos.   |
| Descarga de una letra de remesa   |  Seleccione **Pago remesa.**  |
| Visualización de los detalles del nivel de transacción para un pago específico |  Seleccionar **vista**  |
| Exportación de detalles de transacción a Excel  |  Seleccione **Iniciar descarga** y, a continuación, seleccione Exportar **datos.** Todos los filtros seleccionados se aplicarán a los datos exportados. Una vez que el estado haya cambiado a Completado, seleccione **Descargar** y siga las indicaciones para exportar el informe detallado de transacciones. Actualice la página si el estado no se actualiza en un plazo de cinco minutos.  |

### <a name="missing-or-incorrect-earnings-and-payments"></a>Ganancias y pagos incorrectos o ausentes

Si no puede encontrar los detalles de un pago o transacción, compruebe si ha aplicado los filtros correctos. Dado que algunos nombres de programa han cambiado (por ejemplo, el asociado directo de CSP 1T ahora CSP Direct Bill Partner), es posible que tenga que usar varias selecciones.

Si todavía no encuentra sus ganancias o cree que las ganancias mostradas son incorrectas, póngase en contacto con el soporte [técnico.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="how-do-i-reconcile-my-earnings"></a>Cómo conciliar mis ganancias?

Si hay alguna discrepancia en sus ganancias, realice los pasos siguientes:

1. **Compruebe que reúne los requisitos para las ganancias.**  Las ganancias solo estarán disponibles si cumple la elegibilidad [del programa](incentives-determined-your-program-eligibility.md) y la idoneidad de [las ganancias.](incentives-confirm-your-earnings-eligibility.md)

2. **Compruebe que el perfil de pago está completo.**  La fecha de inicio de sus ingresos de incentivos será el primer día del mes en el que haya completado todos los requisitos de idoneidad, incluida la incorporación con los detalles fiscales y de pago. Los beneficios no estarán disponibles durante los meses anteriores a la finalización fiscal y de pago. Por ejemplo, si completa todos los requisitos durante el mes de abril de 2020, la fecha de inicio de las ganancias será el 1 de abril de 2020. 

3. **Compruebe que reúne los requisitos.**  Compruebe si ha cumplido las reglas de ingresos [aptos](#my-payment-is-missing-or-incorrect) y de elegibilidad para el programa de incentivos.

Si estas acciones no ayudan y las ganancias todavía no se concilian, póngase en contacto con el soporte [técnico.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="where-can-i-find-my-rates"></a>¿Dónde puedo encontrar mis tarifas?

1. Inicie sesión en [Incentivos para partners.](https://partner.microsoft.com/membership/partner-incentives)

2. Desplácese hacia abajo para acceder a los documentos del programa.

3. Seleccione el vínculo del documento para el programa correspondiente.

4. En el documento, consulte la sección Estructura **del programa y Tarifas**.

## <a name="next-steps"></a>Pasos siguientes

- [Administración de reclamaciones de cooperación](incentives-managing-co-op-claims.md)