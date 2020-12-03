---
title: Cálculo del precio unitario vigente
ms.topic: how-to
ms.date: 11/10/2020
description: Obtenga información sobre el precio unitario efectivo y cómo se calcula. En este artículo también se incluye un cálculo de ejemplo.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6ca6e9bf6a49e695314a3e33e36d2d1d5d4d2a25
ms.sourcegitcommit: 147813ba322653c989df5afe0b3bf0c252523a92
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/03/2020
ms.locfileid: "96556334"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Cálculo de precio por unidad efectivo para el consumo de planes de Azure

## <a name="the-effective-unit-price"></a>El precio unitario efectivo

El precio unitario efectivo se calcula en el nivel de medidor (en lugar del nivel de recurso) y se ajusta diariamente según el uso del medidor.

Calculamos el precio unitario efectivo mediante los tres factores siguientes:

- Consumo, que se supervisa diariamente a lo largo del ciclo de facturación
- Costo facturable del medidor
- Organización en niveles (si es aplicable)

Dado que supervisamos el consumo diariamente a lo largo del ciclo de facturación, el precio de la unidad efectiva fluctuará. El precio final de un ciclo de facturación determinado estará disponible después de detener el cálculo de consumo y cerrar el período de facturación. Verá la mayoría de los cambios de consumo después de la cuarta o quinta posición decimal.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Averigüe si su medidor usa precios por niveles

Si no sabe si el medidor usa precios por niveles, use el procedimiento siguiente para averiguarlo. 

1. Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).
2. Seleccione **vender**, seleccione **precios y ofertas** y, luego, seleccione **precios del plan de Azure**.
3. Busque el medidor según el identificador y, a continuación, descargue los datos de precios. 

## <a name="sample-calculation"></a>Cálculo de ejemplo

En la tabla siguiente se ofrece un ejemplo de cómo se calcula el precio unitario efectivo durante el período abierto.

En la tabla se aplican los siguientes valores: 

- **Up** = precio unitario del recurso/hora = 0,868

- **BCU** = unidad de consumo facturable para el medidor

- **BC** = costo facturable para el medidor = BCU * UP * 0,85. Esto refleja un ajuste para el 15% de descuento de PEC. A continuación, usamos el límite inferior de la función para limitar el valor a dos dígitos después del separador decimal, con el fin de cobrar la cantidad mínima. 

- **Precio por unidad vigente** = BCU/BC

>[!NOTE]
>Nota: el medidor de este ejemplo no tiene niveles en los precios.

| Date | BCU (unidad de consumo facturable) | BC (costo facturable) | Precio unitario efectivo |
| ------ | ----------- | ----------- | ----------- |  
| 3-ago | 29 | 21,39 | 0.737586206896552 |
| 10-ago | 210,950039 | 155,63 | 0.737757626107858 |
| 25-ago | 555,950039 | 410,17 | 0.737782122900436 |

## <a name="next-steps"></a>Pasos siguientes

- [Facturación e impuestos](billing.md)
