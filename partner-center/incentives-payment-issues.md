---
title: Solución de problemas de pagos y ganancias
ms.topic: article
ms.date: 02/05/2021
description: Obtenga información acerca de cómo solucionar problemas, como pérdidas de beneficios o incorrectas, problemas de elegibilidad y cómo conciliar las ganancias de los incentivos.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.openlocfilehash: c6ff8915384f8c7ab98fa058f2e45e3d0b4f7214
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/02/2021
ms.locfileid: "106179520"
---
# <a name="troubleshooting-missing-payments-incorrect-earnings-and-other-issues"></a>Solución de problemas de pagos que faltan, ingresos incorrectos y otros problemas

**Roles adecuados**

- Administrador de incentivos

Este artículo le ayudará a resolver cualquier problema de beneficios o de pago en el programa de incentivos. Entre los temas descritos se incluyen el control del tiempo de los pagos, la comprobación de la idoneidad de sus ganancias y la importancia de configurar los perfiles fiscales y de pago correctamente.

## <a name="who-can-create-or-update-payout-and-tax-profiles-for-my-organization"></a>¿Quién puede crear o actualizar perfiles de pago y impuestos para mi organización?

Los usuarios que tengan el rol de administrador de incentivos en el centro de partners para el programa de estímulo pertinente y la ubicación MPN pueden actualizar y ver los perfiles de pago y impuestos de la organización.

## <a name="how-long-does-it-take-for-microsoft-to-approve-my-pending-payout-andor-tax-profiles"></a>¿Cuánto tiempo tarda Microsoft en aprobar mis perfiles fiscales o de pago pendientes?

La validación puede tardar hasta 48 horas. Durante este tiempo, el estado del perfil en la página de información general se mostrará como Validating enrollment (Validando inscripción). Una vez completado el proceso, el estado se mostrará como **inscrito** si se realiza correctamente, o **acción requerida, actualizar el pago** o los detalles de impuestos, si es necesario.

## <a name="how-do-i-know-if-i-have-completed-my-payout-and-tax-profile-correctly"></a>Cómo saber si he completado mi perfil fiscal y de pago correctamente?

El estado de la inscripción se muestra en la página de información general. Cuando haya terminado de crear los perfiles, su estado será **validando la inscripción**. Una vez que se haya validado la información, el estado cambia a **inscrito**. Este estado indica que el pago y el perfil fiscal y su inscripción se han completado correctamente.

## <a name="why-do-i-need-to-update-my-tax-profile-to-use-it-with-a-new-incentive-program"></a>¿Por qué es necesario actualizar mi perfil fiscal para usarlo con un nuevo programa de incentivos?

Pagamos los incentivos de distintas ubicaciones en función del tipo de incentivo. Estas distintas ubicaciones pueden requerir información fiscal adicional, en función de las reglas del programa de incentivos, para procesarse correctamente.

## <a name="how-can-i-delete-a-payment-andor-tax-profile"></a>¿Cómo puedo eliminar un perfil de pago o fiscal?

Microsoft no admite actualmente la posibilidad de eliminar los perfiles fiscales y de pago existentes.

## <a name="my-payment-is-missing-or-incorrect"></a>Falta el pago o es incorrecto

Si faltan pagos o son incorrectos, suele deberse a uno de los siguientes motivos:

- **Es posible que no sea válido.**  Las ganancias solo estarán disponibles si se cumplen los requisitos de idoneidad operativa, es decir, estar inscrito en el período de ganancias del programa correspondiente.
- **Es posible que no se hayan cumplido los requisitos.**  Compruebe si ha cumplido las reglas de elegibilidad y de ingresos aptas para el incentivo que está buscando.

  **Para comprobar su elegibilidad**

  1. Inicie sesión en los [incentivos para asociados](https://partner.microsoft.com/membership/partner-incentives).

  2. Desplácese hacia abajo hasta los documentos del programa.
  
  3. Seleccione el vínculo de documento que desee y, a continuación, revise las secciones 

**Idoneidad para asociados** y **reglas de ingresos válidas**.

- **El perfil de pago puede estar incompleto.** La fecha de inicio de sus ingresos de incentivos será el primer día del mes en el que haya completado todos los requisitos de idoneidad, incluida la incorporación con los detalles fiscales y de pago. Los beneficios no estarán disponibles durante los meses anteriores a la finalización fiscal y de pago. Por ejemplo, si completa todos los requisitos durante el mes de abril de 2020, la fecha de inicio de las ganancias será el 1 de abril de 2020.
- Es **posible que tenga una acción pendiente**.  Podría deberse a que los incentivos no se están procesando porque existe una acción pendiente.

  **Para ver las acciones pendientes**

  1. Inicie sesión en los [incentivos para asociados](https://partner.microsoft.com/membership/partner-incentives).
  2. Abra la página **historial de transacciones** . Revise los campos de esta página para ver las acciones pendientes que se deben completar, como el **Perfil de impuestos pendiente**, el **Perfil de pago pendiente** o el **envío de facturas de impuestos pendientes**.

Si estas acciones no son de ayuda y los pagos todavía faltan o son incorrectos, póngase en contacto [con el soporte técnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="how-can-i-reconcile-my-adjustments"></a>¿Cómo puedo conciliar mis ajustes?

Puede buscar y reconciliar los ajustes descargando los detalles de la transacción y la ganancia.

1. Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).
2. En la barra de navegación superior, seleccione el icono de moneda y, a continuación, seleccione **historial de transacciones**.
3. Aplique los filtros adecuados. (Consulte la nota **importante** que aparece a continuación).
4. Una vez que haya filtrado los datos, seleccione **iniciar descarga** y, a continuación, seleccione **exportar datos**. Los datos se abrirán en un archivo CSV.
5. En el archivo CSV, vaya a la columna P, **tipo de obtención**.
6. Filtre esta columna para **ajustar el descuento**. Puede ver el mes de cada ajuste en las columnas.

>[!IMPORTANT]
>Los ajustes aplicados a períodos de ganancias anteriores no serán visibles en las ganancias del mes en que se aplicó el ajuste. Los ajustes siempre se reflejarán en el informe de ganancias del mes en el que se aplicó el ajuste.
>
>Por ejemplo, un ajuste para las ganancias de enero de 2019 que se procesó en septiembre de 2019 no se reflejará en la cantidad de ganancias del 2019 de septiembre. Sin embargo, cuando se recibe el pago del 2019 de septiembre, incluirá el ajuste del 2019 de enero que se aplicó en septiembre. En este escenario, deberá descargar los detalles de la transacción del 2019 de enero para ver el ajuste que se aplicó.
>
>Tenga esto en cuenta al establecer los filtros de fecha. Como se mencionó anteriormente, los ajustes de los períodos anteriores solo estarán visibles en el mes en que se aplicó el ajuste. Compruebe que el intervalo de fechas seleccionado se corresponde con el mes del ajuste que está intentando localizar. Es posible que deba seleccionar **Borrar todo** para quitar los filtros y, a continuación, aplicar otros nuevos.

## <a name="why-are-my-co-op-claim-payments-made-in-two-different-currencies"></a>¿Por qué mis pagos de notificaciones de cooperación se realizan en dos monedas diferentes?

Cuando se obtienen fondos de cooperación de diferentes entidades de Microsoft, los pagos se realizan en la moneda local de cada entidad respectiva.  

## <a name="why-was-i-paid-in-a-currency-other-than-my-co-op-claim-currency"></a>¿Por qué se pagó en una moneda distinta de la moneda de la notificación de cooperación?

Cada programa de incentivos tiene un perfil de banco que se creó durante la instalación. La moneda especificada en ese perfil es la moneda en la que se le pagará.

## <a name="i-dont-see-earnings-for-a-certain-period"></a>No veo ganancias durante un período determinado

Cuando no ve ganancias durante un período en el que se espera, normalmente se debe a uno de los siguientes problemas:

- **Es posible que no sea válido.**  Las ganancias solo estarán disponibles si se cumplen los requisitos de idoneidad operativa, es decir, estar inscrito en el período de ganancias del programa correspondiente.

- **El perfil de pago puede estar incompleto.**  La fecha de inicio de sus ingresos de incentivos será el primer día del mes en el que haya completado todos los requisitos de idoneidad, incluida la incorporación con los detalles fiscales y de pago. Los beneficios no estarán disponibles durante los meses anteriores a la finalización fiscal y de pago. Por ejemplo, si completa todos los requisitos durante el mes de abril de 2020, la fecha de inicio de las ganancias será el 1 de abril de 2020.

Si ha completado los requisitos de idoneidad, incluida la incorporación con los detalles de pago y de impuestos en el tiempo, y todavía faltan beneficios, póngase en contacto [con el soporte técnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="my-earnings-are-missing-or-incorrect"></a>Mis ganancias faltan o son incorrectas

Los beneficios que faltan o son incorrectos pueden deberse a uno de los siguientes problemas:

- **Es posible que no se hayan cumplido los requisitos.**  Compruebe si ha cumplido las reglas de [elegibilidad](#my-payment-is-missing-or-incorrect) y de ingresos aptas para el incentivo que está buscando.

- **Puede haber una discrepancia.**  Si cumple los requisitos de [idoneidad de programas](incentives-determined-your-program-eligibility.md) y de elegibilidad de los [ingresos](incentives-confirm-your-earnings-eligibility.md) y las ganancias siguen apareciendo incorrectas, la siguiente información puede ayudarle a recuperar los datos.

Las ganancias se muestran en la página **historial de transacciones** y en la página **pagos** . Puede tener acceso a ambas páginas seleccionando el icono de **pago** en la barra de navegación del centro de Partners.

:::image type="content" source="images/incentives/paymenticon.png" alt-text="Información de la transacción":::

Es posible que los importes de la ganancia mensual en la vista del historial de transacciones no se alineen con el importe de pago recibido durante un mes determinado. Esto se debe a los recálculos y ajustes de períodos de obtención anteriores que se aplican a los pagos futuros.

Por ejemplo, un ajuste para las ganancias de enero de 2019 que se procesó en septiembre de 2019 no se reflejará en la cantidad de ganancias del 2019 de septiembre; sin embargo, cuando se recibe el pago del 2019 de septiembre, incluirá el ajuste del 2019 de enero que se aplicó en septiembre.

En este escenario, tendría que descargar los detalles de la transacción para obtener una vista completa de todos los ingresos incluidos en el pago.  Además, puede navegar a la vista de pagos para descargar transacciones para cada pago.

### <a name="transaction-history"></a>Historial de transacciones

Esta vista muestra las tendencias de obtención y pago por mes, ganancias por estado y detalles de transacción junto con el estado de pago de cada transacción. Los datos solo son visibles para los programas y los ID. de MPN para los que es usuario o administrador de incentivos.

### <a name="payments"></a>Pagos

Esta vista le permite ver los pagos de todos los programas y los ID. de MPN. Los datos solo son visibles para los programas y los ID. de MPN para los que es usuario o administrador de incentivos. Desde esta vista, puede descargar la información de la transacción o ver los detalles del pago.

| Para hacer esto | Vaya aquí |
| ------ | :----------- | 
| Ver la información de pago por línea, incluidos los importes de la ganancia y el pago en la moneda local  | Ver el campo **lista de pagos**   |
| Descarga de una carta de envío   |  Seleccionar **remesa de pago**  |
| Ver detalles de nivel de transacción para un pago específico |  Seleccionar **vista**  |
| Exportar los detalles de la transacción a Excel  |  Seleccione **iniciar descarga** y, a continuación, seleccione **exportar datos**. Todos los filtros seleccionados se aplicarán a los datos exportados. Una vez que el estado cambie a completado, seleccione **Descargar** y siga las indicaciones para exportar el informe transacciones detalladas. Actualice la página si el estado no se actualiza en un plazo de cinco minutos.  |

### <a name="missing-or-incorrect-earnings-and-payments"></a>Ganancias y pagos incorrectos o ausentes

Si no puede encontrar un pago o datos de transacción, compruebe si ha aplicado los filtros correctos. Puesto que algunos nombres de programa han cambiado (por ejemplo, CSP 1T Direct Partner es ahora CSP Direct Bill Partner), puede que tenga que usar selecciones múltiples.

Si sigue sin poder encontrar sus ganancias o cree que los beneficios mostrados son incorrectos, póngase en contacto [con el soporte técnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="how-do-i-reconcile-my-earnings"></a>¿Cómo conciliar mis ganancias?

Si hay alguna discrepancia en sus ganancias, realice los pasos siguientes:

1. **Compruebe que reúne los requisitos para las ganancias.**  Las ganancias solo estarán disponibles si se cumplen los requisitos de los [programas](incentives-determined-your-program-eligibility.md) y los [beneficios](incentives-confirm-your-earnings-eligibility.md).

2. **Compruebe que el perfil de pago está completo.**  La fecha de inicio de sus ingresos de incentivos será el primer día del mes en el que haya completado todos los requisitos de idoneidad, incluida la incorporación con los detalles fiscales y de pago. Los beneficios no estarán disponibles durante los meses anteriores a la finalización fiscal y de pago. Por ejemplo, si completa todos los requisitos durante el mes de abril de 2020, la fecha de inicio de las ganancias será el 1 de abril de 2020. 

3. **Compruebe que reúne los requisitos.**  Compruebe si se ha cumplido la [elegibilidad](#my-payment-is-missing-or-incorrect) y las reglas de ingresos aptas para su programa de incentivos.

Si estas acciones no sirven de ayuda y las ganancias todavía no se han conciliado, póngase en contacto [con el soporte técnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="where-can-i-find-my-rates"></a>¿Dónde puedo encontrar mis tarifas?

1. Inicie sesión en los [incentivos para asociados](https://partner.microsoft.com/membership/partner-incentives).

2. Desplácese hacia abajo para obtener acceso a los documentos del programa.

3. Seleccione el vínculo del documento para el programa correspondiente.

4. En el documento, consulte la sección **estructura y tasas del programa**.

## <a name="next-steps"></a>Pasos siguientes

- [Administración de reclamaciones de cooperación](incentives-managing-co-op-claims.md)