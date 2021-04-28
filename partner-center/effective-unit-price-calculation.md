---
title: Cálculo del precio unitario vigente
ms.topic: how-to
ms.date: 04/02/2021
description: Obtenga información sobre el precio unitario efectivo y cómo se calcula. En este artículo también se incluye un cálculo de ejemplo.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1473b3c0b90cca1152b4dab0b8efec86dbc3d22d
ms.sourcegitcommit: f8fd51e1acdbfafdde86d6490bade66c63033ebd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/28/2021
ms.locfileid: "108172224"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Cálculo de precios unitarios efectivos para el consumo del plan de Azure

**Roles adecuados**

- Administrador de facturación

## <a name="the-effective-unit-price"></a>El precio unitario efectivo

El precio unitario efectivo se calcula en el nivel de medidor (en lugar del nivel de recurso) y se ajusta diariamente según el uso del medidor.

Calculamos el precio unitario efectivo mediante los tres factores siguientes:

- Consumo, que se supervisa diariamente a lo largo del ciclo de facturación
- Costo facturable del medidor
- Niveles (si procede)

Dado que supervisamos el consumo diariamente a lo largo del ciclo de facturación, el precio unitario efectivo fluctúa. El precio final de un ciclo de facturación determinado estará disponible después de detener el cálculo de consumo y cerrar el período de facturación. Verá la mayoría de los cambios en el consumo después de la cuarta o quinta posición decimal.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Averiguar si el medidor usa precios por niveles

Si no sabe si el medidor usa precios por niveles, use el procedimiento siguiente para averiguarlo. 

1. Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).
2. Seleccione **Vender,** seleccione **Precios y ofertas** y, a continuación, seleccione Precios del plan de **Azure.**
3. Busque el medidor por identificador y, a continuación, descargue los datos de precios. 

## <a name="sample-calculation"></a>Cálculo de ejemplo

En la tabla siguiente se proporciona un ejemplo de cómo se calcula el precio unitario efectivo durante el período de apertura.

En la tabla , se aplican los valores siguientes: 

- **UP** = Precio unitario del recurso/hora = 0,868

- **BCU** = Unidad de consumo facturable para el medidor

- **BC** = Costo facturable para el medidor = BCU * UP * 0,85. Esto refleja un ajuste para el descuento del 15 % de PEC. A continuación, usamos el límite inferior de la función para limitar el valor a dos dígitos después del separador decimal, con el fin de cobrar la cantidad mínima. 

- **Precio unitario efectivo** = BCU/BC

>[!NOTE]

>Nota: El medidor de este ejemplo no tiene niveles en precios u otros descuentos: los factores de precio unitario efectivo en los porcentajes de descuento y otros ajustes.


| Date | BCU (unidad de consumo facturable) | BC (costo facturable) | Precio unitario efectivo |
| ------ | ----------- | ----------- | ----------- |  
| 3 de agosto | 29 | 21.39 | 0.737586206896552 |
| 10 de agosto | 210.950039 | 155.63 | 0.737757626107858 |
| 25 de agosto | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>Pasos siguientes

- [Facturación e impuestos](billing.md)
