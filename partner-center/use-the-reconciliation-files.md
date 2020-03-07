---
title: Usar los archivos de conciliación | Centro de Partners
ms.topic: article
ms.date: 11/21/2019
description: Use los archivos de conciliación para comprender las vistas detalladas de elementos de línea de los cargos del centro de Partners.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.assetid: FA6A6FCB-2597-44E7-93F8-8D1DD35D52EA
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 6bb65718159019c9ae47aa384524d9d52043d39b
ms.sourcegitcommit: eb4fc25524cc68c10906ccd3392914e805213ee5
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2020
ms.locfileid: "78340223"
---
# <a name="use-your-reconciliation-files"></a>Usar los archivos de conciliación

Dirigido a:

- Centro de asociados
- Centro de partners para Microsoft Cloud for US Government

Puede descargar los archivos de conciliación del centro de partners para obtener una vista detallada de los elementos de línea de cada cargo en un ciclo de facturación. Los detalles de los elementos de línea incluyen los cargos de las suscripciones de cada cliente y eventos detallados (por ejemplo, una adición de puestos a mediados de puestos a una suscripción).

Roles adecuados:

- Administrador de facturación
- Administrador global

Para obtener información sobre cómo leer la **factura**, consulte [leer su](read-your-bill.md)factura.

## <a name="understand-reconciliation-file-fields"></a>Descripción de los campos de archivo de conciliación

- [Campos de archivos de conciliación basados en licencias](license-based-recon-files.md)
- [Campos de archivos de conciliación basados en el uso](usage-based-recon-files.md)
- [Campos de archivo de conciliación único y periódico](one-time-recurring-recon-files.md)
- [Campos de archivo de conciliación de uso con clasificación diaria](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Descripción de los tipos de carga en los archivos de conciliación

Para comprender los tipos de cargos de los archivos de conciliación (la columna **ChargeType** ), vea [reconciliar tipos de cargos de archivo](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Corregir problemas de formato

En ocasiones, un archivo de conciliación puede contener problemas de formato. Por ejemplo, este problema podría producirse si no se utiliza la configuración regional en-US.

Siga estos pasos para corregir los problemas de formato en los archivos de conciliación:

1. Abra el archivo de conciliación (en formato. csv) en Microsoft Excel.
2. Seleccione la primera columna del archivo.
3. Abra el **Asistente para convertir texto en columnas**. En la cinta de opciones, seleccione **datos**y, a continuación, seleccione **texto en columnas**.
4. En el asistente, seleccione **tipo de archivo delimitado**. A continuación, seleccione **siguiente**.
5. En el campo **delimitadores** , seleccione **coma**. (Si la **pestaña** ya está seleccionada, puede dejar esta opción seleccionada). A continuación, seleccione **siguiente**.
6. En el campo **formato de datos de columna** , seleccione **Fecha: MDA**. A continuación, seleccione **siguiente**.
7. En el campo **formato de datos de columna** , seleccione **texto** para todas las columnas de importe. A continuación, seleccione **Finalizar**.

## <a name="download-reconciliation-files-programmatically"></a>Descargar archivos de conciliación mediante programación

Los archivos de conciliación pueden ser muy grandes y a veces son difíciles de descargar. Para descargar los archivos de conciliación mediante programación, vea [obtener artículos de línea de factura](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).

## <a name="map-taxes-or-vat"></a>Impuestos de mapa o IVA

Para asignar impuestos o impuestos sobre el valor añadido (IVA) a la factura:

- Sume la columna **Tax** del archivo basado en licencia.
- Sume la columna **TaxAmount** del archivo basado en el uso.

## <a name="itemize-reconciliation-files-by-partner"></a>Elemento de conciliación de elementos por asociado

Los asociados en el **modelo indirecto** pueden utilizar estos campos adicionales en los archivos de conciliación basados en la licencia y en el uso para que los revendan los archivos.

| Id. de MPN | Descripción |
| ------ | ----------- |
| Id. de MPN | Identificador Microsoft Partner Network (MPN) del asociado del proveedor de soluciones en la nube (CSP) (directo o indirecto). |
| [ID. de revendedor MPN](#reseller-mpn-id) | [Identificador de MPN del distribuidor de registro de la suscripción](#reseller-mpn-id). Este campo corresponde al ID. de distribuidor que se muestra para la suscripción específica del centro de Partners. Solo aparece en los archivos de conciliación de partners en el modelo indirecto. |

### <a name="reseller-mpn-id"></a>Id. de MPN del revendedor

Si un asociado de CSP vendió la suscripción directamente al cliente, su **identificador de MPN** aparece dos veces, como el **identificador de MPN** y el ID. de **MPN del reseller**.

Si un asociado de CSP tiene un revendedor sin **identificador de MPN**, este valor se establece en el **identificador de MPN** del asociado en su lugar.

Si el asociado de CSP quita un ID. de **revendedor de MPN**, este valor se establecerá en *-1*.

Para ver o actualizar el **ID. de revendedor MPN**:

1. Inicia sesión en el Centro de partners.
2. En el menú del Centro de partners, selecciona **Clientes**.
3. Elige el cliente de la lista.
4. En el menú del cliente, seleccione **suscripciones**.
5. Elija la suscripción de la lista.
6. Selecciona **Actualizar** para cambiar el valor de **Revendedor (id. de MPN)** .
