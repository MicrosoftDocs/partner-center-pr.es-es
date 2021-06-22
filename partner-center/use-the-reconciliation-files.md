---
title: Uso de los archivos de conciliación
ms.topic: article
ms.date: 03/26/2021
description: Obtenga información sobre los archivos de conciliación Centro de partners y cómo interpretar las vistas detalladas de elementos de línea de los cargos de un ciclo de facturación determinado.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431569"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Obtenga información sobre cómo leer los elementos de línea en los archivos Centro de partners conciliación

**Roles adecuados:** Administrador de facturación | Administrador global

Puede descargar los archivos de conciliación Centro de partners obtener una vista detallada de cada cargo en un ciclo de facturación. Los detalles del elemento de línea incluyen cargos por las suscripciones de cada cliente y eventos detallados (por ejemplo, una adición a medio plazo de licencias a una suscripción).

Para obtener información sobre cómo leer la **factura,** vea [Leer la factura.](read-your-bill.md)

## <a name="understand-reconciliation-file-fields"></a>Información sobre los campos del archivo de conciliación

- [Campos de archivos de conciliación basados en licencias](license-based-recon-files.md)
- [Campos de archivos de conciliación basados en el uso](usage-based-recon-files.md)
- [Campos de archivos de conciliación de uso con clasificación diaria](daily-rated-usage-recon-files.md)
- [Campos de archivo de conciliación de CSP de compra única](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Información sobre los tipos de cargos en los archivos de conciliación

Para comprender los tipos de cargos en los archivos de conciliación (la **columna ChargeType),** vea [Tipos de cargos de archivo de conciliación](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Corrección de problemas de formato

En ocasiones, un archivo de conciliación puede contener problemas de formato. Por ejemplo, este problema puede producirse si no se usa la configuración regional en-US.

Siga estos pasos para corregir cualquier problema de formato en los archivos de conciliación:

1. Abra el archivo de conciliación (.csv formato) en Microsoft Excel.
2. Seleccione la primera columna del archivo.
3. Abra el **Asistente para convertir texto en columnas**. En la cinta de opciones, **seleccione Datos** y, a continuación, seleccione Texto **a columnas.**
4. En el asistente, seleccione **Tipo de archivo delimitado**. Después, seleccione **Siguiente**.
5. En el **campo Delimitadores,** seleccione **Coma**. (Si **tab** ya está seleccionado, puede dejar esta opción seleccionada). A continuación, **seleccione Siguiente.**
6. En el **campo Formato de datos de** columna, seleccione **Date:MDY**. Después, seleccione **Siguiente**.
7. En el campo **Formato de datos de** columna, seleccione Texto **para** todas las columnas de cantidad. A continuación, seleccione **Finish** (Finalizar).

## <a name="download-reconciliation-files-programmatically"></a>Descarga de archivos de conciliación mediante programación

Los archivos de conciliación pueden ser muy grandes y a veces son difíciles de descargar. Para descargar archivos de conciliación mediante programación, vea [Obtener elementos de línea de factura.](/partner-center/develop/get-invoiceline-items)

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Si el archivo supera el límite de filas en Excel

Si puede descargar un archivo de conciliación pero no abrirlo en Microsoft Excel, probablemente significa que el archivo contiene más filas de las que excel permitirá. Si esto sucede, puede usar cualquiera de los procedimientos siguientes para abrir el archivo.

### <a name="open-a-recon-file-in-power-bi"></a>Abra un archivo de conciliación en Power BI

1. Descargue el archivo de conciliación como lo haría normalmente.
2. Descargue, instale y abra una instancia de Microsoft Power BI.
3. En la Power BI **Inicio,** seleccione **Obtener datos.**
4. En la lista de **orígenes de datos comunes,** seleccione **Texto/CSV.**
5. Cuando se le solicite, abra el archivo de conciliación.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Abrir un archivo de conciliación en una tabla dinámica de Excel

1. Descargue el archivo de conciliación como lo haría normalmente.
2. Abra un nuevo archivo en Microsoft Excel.
3. En la **pestaña Datos,** seleccione **Obtener datos,** **Desde archivo** y, a continuación, **texto/CSV.**
4. Cuando se le solicite, abra el archivo de conciliación. Aparecerán los datos.
5. En el **menú desplegable** Cargar, seleccione **Cargar en** y, a continuación, **seleccione Aceptar.**
6. En el **cuadro de diálogo Importar** datos, seleccione Informe de tabla **dinámica** para abrir el archivo.

## <a name="negative-amount-displayed"></a>Cantidad negativa mostrada

Es posible que vea una cantidad negativa en el archivo de conciliación. Este problema se produce normalmente por uno de los siguientes motivos:

- Ha cancelado o reducido recientemente el número de licencias.
- Ha recibido crédito para un contrato de licencia de servicio (SLA) o para el consumo de Azure.

Para obtener más información acerca de esta transacción, revise su atributo de tipo de carga en el archivo de conciliación.

## <a name="map-taxes-or-vat"></a>Asignación de impuestos o IVA

Para asignar impuestos o impuestos al valor agregado (IVA) a la factura:

- Sumar la **columna** Impuestos del archivo basado en licencia.
- Sumar **la columna TaxAmount** del archivo basado en uso.

## <a name="itemize-reconciliation-files-by-partner"></a>Elementos de los archivos de conciliación por asociado

Los asociados **del modelo indirecto** pueden usar estos campos adicionales en los archivos de conciliación basados en licencias y basados en el uso para especificar los archivos por revendedor.

| Identificador de MPN | Descripción |
| ------ | ----------- |
| Identificador de MPN | Identificador Microsoft Partner Network (MPN) del asociado de Proveedor de soluciones en la nube (CSP) (directo o indirecto). |
| [Id. de MPN del revendedor](#reseller-mpn-id) | Identificador [de MPN del revendedor del registro de la suscripción.](#reseller-mpn-id) Este campo corresponde al identificador de revendedor que aparece para la suscripción específica en Centro de partners. Solo aparece en los archivos de conciliación de partners en el modelo indirecto. |

### <a name="reseller-mpn-id"></a>Id. de MPN del revendedor

Si un asociado de CSP vende la suscripción directamente al cliente, su identificador **de MPN** aparece dos veces, como el identificador de **MPN** y el identificador **de MPN del revendedor.**

Si un asociado de CSP tiene un revendedor sin identificador **de MPN,** este valor se establece en el identificador **de MPN del** asociado en su lugar.

Si el asociado de CSP quita un **id. de MPN de revendedor,** este valor se establecerá en *-1.*

Para ver o actualizar el identificador **de MPN del revendedor:**

1. Inicie sesión en el Centro de datos.
2. En el menú del Centro de partners, selecciona **Clientes**.
3. Elija el cliente de la lista.
4. En el menú del cliente, seleccione **Suscripciones.**
5. Elija la suscripción de la lista.
6. Selecciona **Actualizar** para cambiar el valor de **Revendedor (id. de MPN)**.

## <a name="next-steps"></a>Pasos siguientes

- [Cómo leer el archivo de conciliación & facturación](read-your-bill.md) 