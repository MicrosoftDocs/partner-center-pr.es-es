---
title: Tipos de cargo de archivo de conciliación
ms.topic: article
ms.date: 06/05/2020
description: Descubra los tipos de cargos (por ejemplo, basados en licencias, basados en el uso y una sola vez), créditos y descuentos en Centro de partners conciliación.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 10438ba30c6eb5ba5b1daef1ad16521f1f8e77c6
ms.sourcegitcommit: 70b8ebbe0d431c7a13529f9eabd1b24f40108a46
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/14/2021
ms.locfileid: "113989781"
---
# <a name="understand-the-different-charge-types-in-partner-center-reconciliation-files"></a>Comprender los diferentes tipos de cargos en los archivos Centro de partners conciliación

**Se aplica a**: Centro de partners | Centro de partners para Microsoft Cloud for US Government

**Roles adecuados**: Agente de administración | Administrador de facturación | Administrador global

En este artículo se describen las asignaciones entre una sección de factura y los tipos de cargos asociados que podrían estar en el archivo de conciliación. La factura proporciona un resumen de los cargos. El archivo de conciliación proporciona un desglose detallado de las transacciones de elementos de línea, incluidos los tipos de cargos. Para obtener más información sobre los archivos de conciliación, [vea cómo usar archivos de conciliación](use-the-reconciliation-files.md).

Tanto los archivos de [](license-based-recon-files.md) [conciliación](usage-based-recon-files.md) basados en el uso como los archivos de conciliación basados en licencias solo muestran transacciones y cargos relacionados con el uso (unidades consumidas y cargos relacionados).

> [!NOTE]
> Los créditos, descuentos o reembolsos únicos  que aparecen en la factura como Ajustes no se muestran en el archivo de conciliación.

## <a name="map-charge-types-to-invoice-charges"></a>Asignación de tipos de cargos a cargos de factura

Para hacer referencia cruzada a los importes de cargos entre la factura y el archivo de conciliación, use las opciones de filtro de Microsoft Excel. Filtre por tipos de cargos en el archivo de conciliación para asignar los cargos de factura a un conjunto de desgloses de cargos en el archivo de conciliación.

## <a name="license-based-charges"></a>Cargos basados en licencias

Para asignar estos cargos basados en licencia a la factura, sume la columna **Importe** del archivo basado en licencia.

| Descripción del cargo (columna ChargeType en el archivo de conciliación) | Explicación de cargos |
| ------------------------------------------------------------- | ------------------ |
| Tarifa de activación | Importe que se cobra al cliente cuando usa la suscripción después de la compra. |
| Cuota de cancelación | Los cargos prorrateados se devuelven al cliente cuando se cambian las licencias asociadas. |
| Cancelación de la prorrateo de la instancia | Los cargos prorrateados se cancelan cuando el cliente con una suscripción mensual ha suspendido la suscripción y las licencias asociadas han cambiado en el mismo mes. |
| Tarifa de ciclo | Cargos periódicos de una suscripción. |
| Prorrateo de instancia de ciclo | Cargos prorrateados evaluados por el cliente cuando se cambian las licencias asociadas. |
| Tarifas prorrateas cuando se cancela | Reembolso prorrateado para la parte no utilizada del servicio tras la cancelación. |
| Prorratear las tarifas cuando se convierten fuera de la oferta actual | Cargos prorrateados después de convertir la suscripción mensual actual en una suscripción anual. |
| Tarifas prorrateas al convertir en una nueva oferta | Cargos prorrateados después de convertir una suscripción mensual en una nueva suscripción anual. |
| Tarifas prorrateadas al comprar | Tipo de cargo de una suscripción cuando se usa la facturación mensual o anual. |
| Prorate fee when renew (Prorate fee when renew) | Tarifas prorrateadas tras la renovación de la suscripción. |
| Renovación de la cuota | Cargo por renovar una suscripción |
| Tarifas prorrateas al activarse | Tarifas prorrateadas desde la activación hasta el final del período de facturación. |

## <a name="one-time-charges"></a>Cargos únicos

Para asignar estos cargos únicos a la factura, sume la columna **Importe** del archivo basado en licencia.

| Descripción del cargo (columna ChargeType en el archivo de conciliación) | Explicación de cargos |
| ------------------------------------------------------------- | ------------------ |
| nuevo | Se usa cuando se crea una nueva compra. |
| renew | Se usa cuando se renueva una suscripción después del final del período. |
| addQuantity | Se usa tanto en el reembolso de la compra original como en la nueva cantidad después de un aumento. |
| removeQuantity | Se usa tanto en el reembolso de la compra original como en la nueva cantidad después de una disminución. |
| cancelImmediate | Se usa cuando se cancela una suscripción. |
| Convertir | Se usa cuando se actualiza una licencia. |
| customerCredit | Se usa cuando se dan créditos (por ejemplo, Azure, SLA, etc.) en una transacción. |

## <a name="usage-charges"></a>Cargos de uso

Para asignar estos cargos de uso a la factura, sume la columna **PretaxCharges** del archivo basado en uso.

| Descripción del cargo (columna ChargeType en el archivo de conciliación) | Explicación de cargos |
| ------------------------------------------------------------- | ------------------ |
| Evaluación de la cuota de uso cuando se cancela | Precio de uso de acceso a la cancelación por el uso no pagado durante el período de facturación actual. |
| Evaluación de la cuota de uso para el ciclo actual | Precio de uso de acceso para el período de facturación actual. |

### <a name="credits"></a>Créditos

Para asignar estos créditos a la factura:

- Sumar **totalForCustomer** del archivo basado en licencia.
- Sume **la columna PostTaxTotal** del archivo basado en uso.

| Descripción del cargo (columna ChargeType en el archivo de conciliación) | Explicación de cargos |
| ------------------------------------------------------------- | ------------------ |
| Desplazamiento de un elemento de línea | Reembolso completo o parcial a un elemento de línea, incluidos los impuestos. |

### <a name="usage-based-discounts"></a>Descuentos basados en el uso

Para asignar estos descuentos basados en el uso a la factura, sume la columna **PretaxCharges** del archivo basado en uso.

| Descripción del cargo (columna ChargeType en el archivo de conciliación) | Explicación de cargos |
| ------------------------------------------------------------- | ------------------ |
| Descuento por activación | Descuento aplicado cuando se activa la suscripción. |
| Descuento por ciclo | Descuento aplicado a los cargos periódicos. |
| Renovación del descuento | Descuento aplicado cuando se renueva la suscripción. |
| Cancelación del descuento | Cargos que se aplica cuando se cancelan los descuentos. |

### <a name="license-based-discounts"></a>Descuentos basados en licencias

Para asignar descuentos basados en licencias a la factura, sume la **columna TotalOtherDiscount** del archivo basado en licencia.

*Los descuentos basados en licencias se pueden aplicar a varios tipos de cargos.*
