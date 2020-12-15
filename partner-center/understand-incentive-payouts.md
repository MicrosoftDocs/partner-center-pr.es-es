---
title: Ver los detalles del programa y el incentivo
ms.topic: article
ms.date: 11/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Use estas páginas para ver y administrar el estado del programa incentivos
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4bf1c7a2abceffc812666456ddae252fca70d8f1
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492728"
---
# <a name="view-your-incentives-program-details"></a>Ver los detalles del programa incentivos

**Se aplica a**

- Centro de partners

**Roles adecuados**

- Administrador de incentivos
- Usuario de incentivos
- Visor de solo lectura de incentivos
- Administrador global
- Administrador de partners de MPN

En este artículo se explica cómo acceder a la página de **información general de mis incentivos** , en la que se muestra el estado general de los programas de incentivos, así como el estado de cada programa en cada ubicación. También proporciona los distintos Estados de inscripción. 

>[!NOTE]
>Para obtener más información acerca de las características de incentivos y incentivos del centro de Partners, consulte [inversiones e incentivos para asociados](https://partner.microsoft.com/membership/partner-incentives) (inicio de sesión obligatorio).

## <a name="access-the-incentives-overview-page"></a>Acceder a la página de información general sobre incentivos

1. Inicie sesión en el [panel del centro de Partners](https://partner.microsoft.com/dashboard).
1. Seleccione **incentivos** e **información general** en el menú.
1. Vea el resumen de ingresos y pagos en la parte superior de la página y más detalles en la tabla siguiente. También puede ordenar, agrupar y expandir la tabla adjunta:

   - Para ordenar por columna, seleccione el nombre de la columna.
   - Para agrupar por programa, seleccione la pestaña **por programa** situada encima de la tabla.
   - Para agrupar por ubicación, seleccione la pestaña **por ubicación** situada encima de la tabla.
   - Para ver más detalles acerca de las inscripciones dentro de un grupo específico, seleccione el símbolo de cheurón al final de una fila determinada. Este cheurón expande la vista.
1. Si se requiere una acción adicional para inscribirse en un programa, esta información aparecerá en la columna **Estado**. En este caso, seleccione el símbolo del botón de contenido adicional para obtener información sobre los pasos que debe realizar.

## <a name="enrollment-status"></a>Estado de inscripción

En la tabla siguiente se explican los distintos Estados de inscripción que se muestran en la columna **Estado** .

| **Estado**         | **Aparece cuando** |
|:------------------------------------|:------------------|
| Acción requerida  | El asociado ha aceptado una invitación para inscribirse en un programa de incentivos, pero puede que tenga que actualizar la información bancaria o fiscal. Consulte la columna **Actions Required (acciones necesarias** ) para ver los pasos siguientes o vínculos para actualizar la información bancaria o fiscal en el centro de Partners. |
| Descontinuado  | El programa de estímulo específico ya no se ofrece en el sistema de incentivos. |
| Inscrito  | Se ha validado toda la información fiscal y bancaria. No es necesario realizar ninguna otra acción de inscripción en el socio. |
| Inscribiendo  | El usuario no es un administrador de incentivos y la inscripción está en la **acción necesaria** o **validando** los Estados de inscripción.|
| Inactivo/no válido | Es posible que el programa de incentivos no esté abierto a la inscripción en este momento o que el asociado no cumpla los requisitos actuales para la inscripción o la reinscripción. <br><br> Si el estado es no **válido**, el asociado no cumple los requisitos de elegibilidad actuales para el programa. al seleccionar el vínculo **vea los requisitos de idoneidad** bajo el estado de inscripción se mostrarán los requisitos de idoneidad y cuáles de estos requisitos se han cumplido. <br><br> También puede ver un estado **inactivo** de las inscripciones de la organización virtual (Vorg) o de la cuenta global de socio (PGA) que ya no están activas en el programa de incentivos.  |
| Invitado  | Se ha enviado una nueva invitación de inscripción del programa de incentivos al socio, pero el socio todavía no ha iniciado el proceso de inscripción. La columna **acciones requeridas** adyacentes muestra los pasos siguientes y los vínculos relacionados.  |
| Validando la inscripción  | El asociado ya ha completado o actualizado la información bancaria y fiscal para una inscripción nueva o existente y está esperando a que Microsoft valide esta información. Durante el proceso de validación, la validación de la **inscripción** puede aparecer hasta 48 horas.  |

## <a name="see-your-payment-information"></a>Ver la información de pago

Seleccione el icono de pago en la esquina superior derecha de la pantalla para obtener acceso a los distintos resúmenes:

- Historial de transacciones
- Pagos
- Exportar datos

:::image type="content" source="images/payouts/payout-overview.png" alt-text="Muestra el icono de pago en la esquina superior derecha del portal del centro de Partners.":::

Esta información incluye los ingresos y pagos totales de incentivos desde que se inscribió en los programas de incentivos. También en esta página se incluyen las ganancias y los pagos por ubicación o programa, así como las acciones que haya que realizar para inscribirse en un programa en una ubicación específica. 

También puede usar la [API de pago de socios comerciales](https://apidocs.microsoft.com/services/partnerpayouts) para conectarse y obtener datos de pagos y transacciones de pago directamente. Consulte las [instrucciones de pago](payout-statement.md) para obtener más información.

## <a name="next-steps"></a>Pasos siguientes
- [Balances de pagos](payout-statement.md)
