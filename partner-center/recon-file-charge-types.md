---
title: Tipos de cargos de archivo de conciliación
ms.topic: article
ms.date: 06/05/2020
description: Descubra los tipos de cargos (como, basado en licencias, basados en el uso, y una sola vez), créditos y descuentos en los archivos de conciliación del centro de Partners.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1ec4f4a483ecfd106f7ec41b85372e136524a046
ms.sourcegitcommit: 1796d3d0ec2e06a3792852377ff81127b4d22fe0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/17/2020
ms.locfileid: "84909113"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Comprender los distintos tipos de cargos en los archivos de conciliación del centro de Partners

**Se aplica a**

- Centro de partners
- Centro de partners para Microsoft Cloud for US Government

**Roles adecuados**

- Agente de administrador
- Administrador de facturación
- Administrador global

En este tema se describen las asignaciones entre una sección de factura y los tipos de cargos asociados que podrían estar en el archivo de conciliación. La factura proporciona un resumen de los cargos. El archivo de conciliación proporciona un desglose detallado de las transacciones de elementos de línea, incluidos los tipos de cargos. Para obtener más información acerca de los archivos de conciliación, consulte [uso de archivos de conciliación](use-the-reconciliation-files.md).

Tanto [los archivos de conciliación basados en el uso](usage-based-recon-files.md) como [los archivos de conciliación basados en licencias](license-based-recon-files.md) solo muestran las transacciones y los cargos relacionados con el uso (unidades consumidas y cargos relacionados).

> [!NOTE]
> No se muestran en el archivo de conciliación los créditos, descuentos o reembolsos de un solo descuento que aparecen en la factura como **ajustes** .

## <a name="map-charge-types-to-invoice-charges"></a>Asignación de tipos de cargos a cargos de factura

Para hacer referencias cruzadas de los importes de los cargos entre su factura y el archivo de conciliación, use las opciones de filtro de Microsoft Excel. Filtre por tipos de carga en el archivo de conciliación para asignar los cargos de la factura a un conjunto de desgloses de gastos en el archivo de conciliación.

## <a name="license-based-charges"></a>Cargos basados en licencias

Para asignar estos cargos basados en licencias a la factura, sume la columna **amount** del archivo basado en licencia.

| Descripción de cargos (columna ChargeType en el archivo de conciliación) | Explicación de cargos |
| ------------------------------------------------------------- | ------------------ |
| Tarifa de activación | La cantidad que se cobra al cliente cuando usa la suscripción después de la compra. |
| Cuota de cancelación | Los cargos prorrateados se reembolsan al cliente cuando se cambian los puestos asociados. |
| Cancelar prorrateo de instancia | Los cargos prorrateados se cancelan cuando el cliente con una suscripción mensual tiene una suscripción suspendida y los puestos asociados cambian en el mismo mes. |
| Tarifa de ciclo | Cargos periódicos de una suscripción. |
| Prorrateo de instancia de ciclo | Cargos prorrateados evaluados por el cliente cuando se cambian los puestos asociados. |
| Tarifas de prorrateo al cancelar | Reembolso prorrateado de la parte no utilizada del servicio tras la cancelación. |
| Tarifas de prorrateo cuando se convierten de la oferta actual | Cargos prorrateados después de la conversión de la suscripción mensual actual a una suscripción anual. |
| Cuotas de protarifas cuando se convierten a una nueva oferta | Cargos prorrateados después de convertir una suscripción mensual a una nueva suscripción anual. |
| Tarifas prorrateadas al comprar | El tipo de cargo de una suscripción cuando se usa la facturación anual. |
| Precio de compra | El tipo de cargo de una suscripción cuando se usa la facturación mensual. |
| Cuota de prorrateo al renovar | Tarifas prorrateadas tras la renovación de la suscripción. |
| Precio de renovación | Cargo por renovar una suscripción |
| Tarifas de protarifas al activar | Tarifas prorrateadas de la activación hasta el final del período de facturación. |

## <a name="one-time-charges"></a>Cargos por única vez

Para asignar estos cargos de un solo tiempo a la factura, sume la columna **amount** del archivo basado en licencia.

| Descripción de cargos (columna ChargeType en el archivo de conciliación) | Explicación de cargos |
| ------------------------------------------------------------- | ------------------ |
| Nuevo | Se usa cuando se crea una nueva compra. |
| addQuantity | Se usa tanto en el reembolso de la compra original como en la nueva cantidad después de un aumento. |
| removeQuantity | Se usa tanto en el reembolso de la compra original como en la nueva cantidad tras una disminución. |
| Cancelar | Se usa cuando se cancela una suscripción. |
| Convert | Se usa cuando se actualiza una licencia pero el número de puestos permanece inalterado. |

## <a name="usage-charges"></a>Cargos de uso

Para asignar estos cargos de uso a la factura, sume la columna **PretaxCharges** del archivo basado en el uso.

| Descripción de cargos (columna ChargeType en el archivo de conciliación) | Explicación de cargos |
| ------------------------------------------------------------- | ------------------ |
| Evaluar la cuota de uso al cancelar | Precio de uso de acceso a la cancelación por el uso no pagado durante el período de facturación actual. |
| Evaluar la cuota de uso del ciclo actual | Precio de uso de acceso para el período de facturación actual. |

### <a name="credits"></a>Créditos

Para asignar estos créditos a su factura:

- Sume el **TotalForCustomer** del archivo basado en licencia.
- Sume la columna **PostTaxTotal** del archivo basado en el uso.

| Descripción de cargos (columna ChargeType en el archivo de conciliación) | Explicación de cargos |
| ------------------------------------------------------------- | ------------------ |
| Desplazar un elemento de línea | Reembolso completo o parcial a un elemento de línea, incluidos los impuestos. |

### <a name="usage-based-discounts"></a>Descuentos basados en el uso

Para asignar estos descuentos basados en el uso a la factura, sume la columna **PretaxCharges** del archivo basado en el uso.

| Descripción de cargos (columna ChargeType en el archivo de conciliación) | Explicación de cargos |
| ------------------------------------------------------------- | ------------------ |
| Descuento de activación | Descuento que se aplica cuando se activa la suscripción. |
| Descuento por ciclo | Descuento aplicado a los cargos periódicos. |
| Renovar descuento | Descuento que se aplica cuando se renueva la suscripción. |
| Cancelar descuento | Cargos que se aplica cuando se cancelan los descuentos. |

### <a name="license-based-discounts"></a>Descuentos basados en licencias

Para asignar descuentos basados en licencias a la factura, sume la columna **TotalOtherDiscount** del archivo basado en licencia.

*Los descuentos basados en licencias se pueden aplicar a varios tipos de cargos.*
