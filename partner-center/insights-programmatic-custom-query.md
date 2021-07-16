---
title: Especificación de consulta personalizada
description: Aprenda a crear consultas personalizadas para extraer datos de tablas de análisis.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 57f2109044e604dca21b0109b5be56f40170628e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376071"
---
# <a name="custom-query-specification"></a>Especificación de consulta personalizada

Los asociados pueden usar esta especificación de consulta para formular fácilmente consultas personalizadas para extraer datos de las tablas de análisis. Las consultas se pueden usar para seleccionar solo las columnas deseadas y las métricas que coincidan con un determinado criterio. En el centro de la especificación del lenguaje se encuentra la definición del conjunto de datos sobre el que se puede escribir una consulta personalizada.

## <a name="datasets"></a>Conjuntos de datos

Del mismo modo que algunas consultas se ejecutan en una base de datos que tiene tablas y columnas, una consulta personalizada funciona en conjuntos de datos que tienen columnas y métricas. La lista completa de los conjuntos de datos disponibles para formular una consulta puede obtenerse mediante la API de conjuntos de datos.

Este es un ejemplo de un conjunto de datos que se muestra como JSON:

```json
{ 
      "datasetName": "OfficeUsage", 
      "selectableColumns": [ 
        "CustomerTenantId", 
        "CustomerTpid", 
        "WorkloadName", 
        "Month", 
        "PaidAvailableUnits", 
        "MonthlyActiveUsers", 
        "CustomerName", 
        "CustomerMarket", 
        "CustomerSegment",  
        "MPNId", 
        "PartnerName", 
        "PartnerLocation", 
        "PartnerAttributionType", 
        "IsDuplicateRowForPGA" 
      ], 
      "availableMetrics": [ 
        "CustomerCount", 
        "CustomerTenantCount", 
        "TotalPaidAvailableUnits", 
        "TotalMonthlyActiveUsers" 
      ], 
      "availableDateRanges": [ 
        "LAST_MONTH", 
        "LAST_3_MONTHS", 
        "LAST_6_MONTHS", 
        "LAST_1_YEAR", 
        "LIFETIME" 
      ], 
      "minimumRecurrenceInterval": 24 
    },
```

## <a name="parts-of-a-dataset"></a>Elementos de un conjunto de datos

- Un nombre de conjunto de datos es como el nombre de una tabla de base de datos. Por ejemplo, OfficeUsage. Un conjunto de datos tiene una lista de columnas que se pueden seleccionar, como CustomerTenantId.
- Un conjunto de datos también tiene métricas, que son como funciones de agregación en una base de datos. Por ejemplo, TotalMonthlyActiveUsers.
- Hay intervalos de tiempo fijos durante los que se pueden exportar los datos.

## <a name="formulating-a-query-on-a-dataset"></a>Formulación de una consulta en un conjunto de datos

Estas son algunas consultas de ejemplo que muestran cómo extraer varios tipos de datos.

|Consultar|    Descripción    |
|----|    ----    |
|**SELECT** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **TIMESPAN** LAST_MONTH|    Esta consulta obtiene cada CusotmerTenantID y sus PaidAvailableUnits correspondientes en el último mes.    |
|**SELECT** CustomerTenantId, PaidAvailableUnits **FROM** <br>OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10|    Esta consulta obtiene los 10 inquilinos de clientes principales en orden decreciente del número de unidades disponibles de pago.     |
|**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS |    Esta consulta obtiene los PaidAvailableUnits y MonthlyActiveUsers de todos los clientes que tienen MonthlyActiveUsers superiores a 100 000.     |
|**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM** <br>OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002') |    Esta consulta obtiene CustomerTenantId y los usuarios activos mensuales para cada mes por los dos valores customerTpId: "2a31c234-1f4e-4c60-909e-176d234f93161" y "80780748-3f9a-11eb-b378-0242ac130002".     |
|        |        |

## <a name="query-specification"></a>Especificación de consulta

En esta sección se describe la definición y la estructura de la consulta.

## <a name="grammar-reference"></a>Referencia de gramática

En esta tabla se describen los símbolos que se usan en las consultas.

|    Consultar    |    Descripción    |
|    ----    |    ----    |
|    `?`    |    Opcionales    |
|    `*`    |    Cero o más    |
|    `+`    |    Uno o más    |
|    `\|`    |    O / Una de las listas    |
|        |        |

## <a name="query-definition"></a>Definición de la consulta

La instrucción query tiene las siguientes cláusulas: SelectClause, FromClause, WhereClause, OrderClause, LimitClause y TimeSpan.

- **SeleccioneClausar:**`SELECT ColumOrMetricName (, ColumOrMetricName)*`
    - **ColumOrMetricName**: columnas y métricas definidas en el conjunto de datos
- **FromClause**: `FROM DatasetName`
    - **DatasetName**: nombre del conjunto de datos definido en el conjunto de datos
- **WhereClause**: `WHERE FilterCondition (AND FilterCondition)`
    - **FilterCondition**: valor del operador ColumOrMetricName
        - **Operador**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`
        - **Valor**: Number | StringLiteral | MultiNumberList | MultiStringList
            - **Número:**`-? [0-9]+ (. [0-9] [0-9]*)?`
            - **StringLiteral**:  `' [a-zA-Z0-9_]*'`
            - **MultiNumberList**: `(Number (,Number)*)`
            - **MultiStringList**: `(StringLiteral (,StringLiteral)*)`
- **OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`
    - **OrderCondition**: `ColumOrMetricName (ASC | DESC)*`
- **LimitClause**: `LIMIT [0-9]+`
- **TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`

## <a name="query-structure"></a>Estructura de la consulta

Una consulta de informe se compone de varios elementos:
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

A continuación, se describe cada uno de los elementos.

### `SELECT`

Este elemento de la consulta especifica las columnas que se exportarán. Las columnas que se pueden seleccionar son los campos *enumerados en selectableColumns* y *availableMetrics* secciones de un conjunto de datos.

Opcionalmente, `DISTINCT` la palabra clave se puede especificar después de `SELECT` . Si `DISTINCT` se especifica , las filas exportadas finales siempre contendrán valores distintos de las columnas seleccionadas. Las métricas se calcularán para cada combinación distinta de las columnas seleccionadas, por lo que la palabra clave no es necesaria cuando se incluye una columna de métrica `DISTINCT` en la lista seleccionar columna.

**Ejemplo**:

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

Este elemento de la consulta indica el conjunto de datos desde el que se deben exportar los datos. El nombre del conjunto de datos que se proporciona aquí debe ser un nombre de conjunto de datos válido devuelto por la API de los conjuntos de datos.

**Ejemplo**:

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

Este elemento de la consulta se usa para especificar las condiciones de filtro en el conjunto de datos. Solo las filas que coincidan con todas las condiciones enumeradas en esta cláusula estarán presentes en el archivo final exportado. La condición de filtro puede estar en cualquiera de las columnas enumeradas *en selectableColumns* y *availableMetrics*. Los valores especificados en la condición de filtro pueden ser una lista de números o una lista de cadenas solo cuando el operador es `IN` o `NOT IN`. Siempre se pueden proporcionar los valores como una cadena literal y se convertirán en los tipos nativos de columnas. Es necesario separar varias condiciones de filtro con una operación AND.

**Ejemplo**:

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

En este elemento de la consulta se especifican los criterios de ordenación de las filas exportadas. Las columnas en las que se puede definir la ordenación deben ser de *selectableColumns* y *availableMetrics* del conjunto de datos. Si no se especifica ninguna dirección de ordenación, el valor predeterminado será DESC en la columna. La ordenación se puede definir en varias columnas separando los criterios con una coma.

**Ejemplo**:

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

Este elemento de la consulta especifica el número de filas que se exportarán. El número que especifique debe ser un entero positivo distinto de cero.

### `TIMESPAN`

Este elemento de la consulta especifica el período de tiempo durante el que se deben exportar los datos. Los valores posibles deben ser del *campo availableDateRanges* de la definición del conjunto de datos.

### <a name="case-sensitivity-in-query-specification"></a>Distinción de mayúsculas y minúsculas en la especificación de consultas

La especificación no distingue entre mayúsculas y minúsculas. Las palabras clave predefinidas, los nombres de columna y los valores se pueden especificar usando mayúsculas o minúsculas.

## <a name="next-steps"></a>Pasos siguientes

- [Lista de consultas del sistema](insights-programmatic-system-queries.md)
- [Lista de consultas de ejemplo](insights-programmatic-sample-queries.md)