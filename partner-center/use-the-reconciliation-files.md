---
title: Usar los archivos de conciliación
ms.topic: article
ms.date: 03/26/2021
description: Obtenga información acerca de los archivos de conciliación en el centro de Partners y cómo interpretar las vistas detalladas del artículo de línea de los cargos de un ciclo de facturación determinado.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: aefd5258c778fd8a7b92bfe49f245bf818497fb8
ms.sourcegitcommit: dd51744a4af3797493a5ebbfc766dab86ff00477
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/29/2021
ms.locfileid: "105730097"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Obtenga información sobre cómo leer los elementos de línea de los archivos de conciliación del centro de Partners

**Roles adecuados**

- Administrador de facturación
- Administrador global

Puede descargar los archivos de conciliación del centro de partners para obtener una vista detallada de los elementos de línea de cada cargo en un ciclo de facturación. Los detalles de los elementos de línea incluyen los cargos de las suscripciones de cada cliente y eventos detallados (por ejemplo, una adición de licencias a mediados de la suscripción).

Para obtener información sobre cómo leer la **factura**, consulte [leer su](read-your-bill.md)factura.

## <a name="understand-reconciliation-file-fields"></a>Descripción de los campos de archivo de conciliación

- [Campos de archivos de conciliación basados en licencias](license-based-recon-files.md)
- [Campos de archivos de conciliación basados en el uso](usage-based-recon-files.md)
- [Campos de archivos de conciliación de uso con clasificación diaria](daily-rated-usage-recon-files.md)
- [Campos de archivo de conciliación de CSP de compra única](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Descripción de los tipos de carga en los archivos de conciliación

Para comprender los tipos de cargos de los archivos de conciliación (la columna **ChargeType** ), vea [reconciliar tipos de cargos de archivo](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Corregir problemas de formato

En ocasiones, un archivo de conciliación puede contener problemas de formato. Por ejemplo, este problema podría producirse si no se utiliza la configuración regional en-US.

Siga estos pasos para corregir los problemas de formato en los archivos de conciliación:

1. Abra el archivo de conciliación (en formato. csv) en Microsoft Excel.
2. Seleccione la primera columna del archivo.
3. Abra el **Asistente para convertir texto en columnas**. En la cinta de opciones, seleccione **datos** y, a continuación, seleccione **texto en columnas**.
4. En el asistente, seleccione **tipo de archivo delimitado**. Después, seleccione **Siguiente**.
5. En el campo **delimitadores** , seleccione **coma**. (Si la **pestaña** ya está seleccionada, puede dejar esta opción seleccionada). A continuación, seleccione **siguiente**.
6. En el campo **formato de datos de columna** , seleccione **Fecha: MDA**. Después, seleccione **Siguiente**.
7. En el campo **formato de datos de columna** , seleccione **texto** para todas las columnas de importe. A continuación, seleccione **Finish** (Finalizar).

## <a name="download-reconciliation-files-programmatically"></a>Descargar archivos de conciliación mediante programación

Los archivos de conciliación pueden ser muy grandes y a veces son difíciles de descargar. Para descargar los archivos de conciliación mediante programación, vea [obtener artículos de línea de factura](/partner-center/develop/get-invoiceline-items).

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Si el archivo supera el límite de filas de Excel

Si es capaz de descargar un archivo de conciliación pero no lo abre en Microsoft Excel, probablemente significa que el archivo contiene más filas de las que Excel permitirá. Si esto ocurre, puede usar cualquiera de los procedimientos siguientes para abrir el archivo.

### <a name="open-a-recon-file-in-power-bi"></a>Abra un archivo de conciliación en Power BI

1. Descargue el archivo de conciliación como lo haría normalmente.
2. Descargue, instale y abra una instancia de Power BI.
3. En la pestaña **Inicio** de Power BI, seleccione **obtener datos**.
4. En la lista de **orígenes de datos comunes**, seleccione **Text/CSV**.
5. Cuando se le solicite, abra el archivo de conciliación.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Apertura de un archivo de conciliación en una tabla dinámica de Excel

1. Descargue el archivo de conciliación como lo haría normalmente.
2. Abra un archivo nuevo en Microsoft Excel.
3. En la pestaña **datos** , seleccione **obtener datos**, seleccione **desde archivo** y, a continuación, seleccione **texto/CSV**.
4. Cuando se le solicite, abra el archivo de conciliación. Los datos aparecerán.
5. En el menú desplegable **cargar** , seleccione **cargar en** y, a continuación, haga clic en **Aceptar**.
6. En el cuadro de diálogo **importar datos** , seleccione **Informe de tabla dinámica** para abrir el archivo.

## <a name="negative-amount-displayed"></a>Importe negativo mostrado

Es posible que vea una cantidad negativa en el archivo de conciliación. Esto probablemente se debe a una de las siguientes causas:

- Recientemente ha cancelado o reducido el número de licencias
- Ha recibido crédito por un contrato de licencia de servicio (SLA) o por el consumo de Azure

Para obtener más información acerca de esta transacción, revise su atributo de tipo de carga en el archivo de conciliación.

## <a name="map-taxes-or-vat"></a>Impuestos de mapa o IVA

Para asignar impuestos o impuestos sobre el valor añadido (IVA) a la factura:

- Sume la columna **Tax** del archivo basado en licencia.
- Sume la columna **TaxAmount** del archivo basado en el uso.

## <a name="itemize-reconciliation-files-by-partner"></a>Elemento de conciliación de elementos por asociado

Los asociados en el **modelo indirecto** pueden utilizar estos campos adicionales en los archivos de conciliación basados en la licencia y en el uso para que los revendan los archivos.

| Identificador de MPN | Descripción |
| ------ | ----------- |
| Identificador de MPN | Identificador Microsoft Partner Network (MPN) del asociado del proveedor de soluciones en la nube (CSP) (directo o indirecto). |
| [Id. de MPN del revendedor](#reseller-mpn-id) | [Identificador de MPN del distribuidor de registro de la suscripción](#reseller-mpn-id). Este campo corresponde al ID. de distribuidor que se muestra para la suscripción específica del centro de Partners. Solo aparece en los archivos de conciliación de partners en el modelo indirecto. |

### <a name="reseller-mpn-id"></a>Id. de MPN del revendedor

Si un asociado de CSP vendió la suscripción directamente al cliente, su **identificador de MPN** aparece dos veces, como el **identificador de MPN** y el ID. de **MPN del reseller**.

Si un asociado de CSP tiene un revendedor sin **identificador de MPN**, este valor se establece en el **identificador de MPN** del asociado en su lugar.

Si el asociado de CSP quita un ID. de **revendedor de MPN**, este valor se establecerá en *-1*.

Para ver o actualizar el **ID. de revendedor MPN**:

1. Inicie sesión en el Centro de datos.
2. En el menú del Centro de partners, selecciona **Clientes**.
3. Elija el cliente de la lista.
4. En el menú del cliente, seleccione **suscripciones**.
5. Elija la suscripción de la lista.
6. Selecciona **Actualizar** para cambiar el valor de **Revendedor (id. de MPN)**.

## <a name="next-steps"></a>Pasos siguientes

- [Cómo leer el archivo de conciliación & de la factura](read-your-bill.md) 