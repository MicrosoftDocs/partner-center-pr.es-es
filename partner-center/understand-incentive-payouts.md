---
title: Visualización de los detalles de incentivos y programas
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Use estas páginas para ver y administrar Programa Incentivos estado.
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 33ec3befdc4b2bab2f31d25d210679594debbbf1
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277256"
---
# <a name="view-your-incentives-program-details"></a>Visualización de los detalles del programa de incentivos

**Roles adecuados:** administrador de incentivos | Incentivos para usuarios | Administrador global | Administrador de asociados de MPN

En este artículo se explica la página de información general Mis **incentivos,** que muestra el estado general de los programas de incentivos, así como el estado de cada programa en cada ubicación. También proporciona los distintos estados de inscripción.

>[!NOTE]
>Para obtener más información sobre los incentivos y las características de incentivos Centro de partners, consulte Inversiones e [incentivos para](https://partner.microsoft.com/membership/partner-incentives) partners (se requiere inicio de sesión).

## <a name="access-the-incentives-overview-page"></a>Acceso a la página de información general de incentivos

1. Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard).
1. Seleccione **Incentivos** y, a **continuación, Información** general en el menú.
1. Vea el resumen de ingresos y pagos en la parte superior de la página y más detalles en la tabla siguiente. También puede ordenar, agrupar y expandir la tabla que lo acompaña:

   - Para ordenar por columna, seleccione el nombre de la columna.
   - Para agrupar por programa, seleccione la **pestaña Por programa** encima de la tabla.
   - Para agrupar por ubicación, seleccione la **pestaña Por ubicación** encima de la tabla.
   - Para ver más detalles sobre las inscripciones dentro de un grupo específico, seleccione el símbolo de contenido adicional al final de una fila determinada. Este botón de contenido adicional expande la vista.
1. Si se requiere una acción adicional para inscribirse en un programa, esta información aparecerá en la columna **Estado**. En este caso, seleccione el símbolo del botón de contenido adicional para obtener información sobre los pasos que debe realizar.

## <a name="enrollment-status"></a>Estado de inscripción

En la tabla siguiente se explican los distintos estados de inscripción que se muestran en la **columna** Estado.

| **Estado**         | **Aparece cuando** |
|:------------------------------------|:------------------|
| Acción requerida  | El asociado ha aceptado una invitación para inscribirse en un programa de incentivos, pero puede que tenga que actualizar la información bancaria o fiscal. Consulte la **columna Actions required (Acciones** necesarias) para ver los pasos siguientes o vínculos para actualizar la información bancaria o fiscal en Centro de partners. |
| Descontinuado  | El programa de incentivos específico ya no se ofrece en el sistema de incentivos. |
| Inscrito  | Se ha validado toda la información fiscal y bancaria. El asociado no requiere ninguna otra acción de inscripción. |
| Inscribiendo  | El usuario no es un administrador de incentivos y la inscripción está en los estados **Acción requerida** o Validación **de la** inscripción.|
| Inactivo o no apto | Es posible que el programa de incentivos no esté abierto a la inscripción en este momento o que el asociado no cumpla los requisitos actuales para la inscripción o la reinscripción. <br><br> Si el estado es **No apto,** el asociado no cumple los requisitos de idoneidad actuales para el programa; Si selecciona el vínculo **Ver requisitos de** elegibilidad debajo del estado de inscripción, se mostrarán los requisitos de idoneidad y cuál de estos requisitos se ha cumplido. <br><br> También puede ver un estado inactivo para las **inscripciones** de organización virtual (POMG) o cuenta global de asociados (PGA) que ya no están activas en el programa de incentivos.  |
| Invitado  | Se ha enviado una nueva invitación de inscripción del programa de incentivos al asociado, pero el asociado aún no ha iniciado el proceso de inscripción. La columna **Acciones** necesarias adyacente muestra los pasos siguientes y los vínculos relacionados.  |
| Validación de la inscripción  | El asociado ya ha completado o actualizado la información bancaria y fiscal de una inscripción nueva o existente y está esperando a que Microsoft valide esta información. Durante el proceso de validación, **la validación de la** inscripción puede aparecer durante un máximo de 48 horas.  |

## <a name="see-your-payment-information"></a>Ver la información de pago

Seleccione el icono de pago en la esquina superior derecha de la pantalla para acceder a estos resúmenes diferentes:

- Historial de transacciones
- Pagos
- Exportar datos

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Se muestra el icono Pago en la esquina superior derecha del portal del Centro de partners.":::

Esta información incluye los ingresos y pagos totales de incentivos desde que se inscribió en los programas de incentivos. También en esta página se incluyen las ganancias y los pagos por ubicación o programa, así como las acciones que haya que realizar para inscribirse en un programa en una ubicación específica. 

También puede usar partner [Payout API](https://apidocs.microsoft.com/services/partnerpayouts) para conectarse y obtener datos de transacción y pago directamente. Consulte [Payout statements (Extractos de pago)](payout-statement.md) para obtener más información.

## <a name="next-steps"></a>Pasos siguientes

- [Extractos de pagos](payout-statement.md)
