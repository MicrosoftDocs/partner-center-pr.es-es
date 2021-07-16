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
# <a name="custom-query-specification"></a><span data-ttu-id="787b8-103">Especificación de consulta personalizada</span><span class="sxs-lookup"><span data-stu-id="787b8-103">Custom query specification</span></span>

<span data-ttu-id="787b8-104">Los asociados pueden usar esta especificación de consulta para formular fácilmente consultas personalizadas para extraer datos de las tablas de análisis.</span><span class="sxs-lookup"><span data-stu-id="787b8-104">Partners can use this query specification to easily formulate custom queries for extracting data from analytics tables.</span></span> <span data-ttu-id="787b8-105">Las consultas se pueden usar para seleccionar solo las columnas deseadas y las métricas que coincidan con un determinado criterio.</span><span class="sxs-lookup"><span data-stu-id="787b8-105">The queries can be used to select only the desired columns and metrics that match a certain criterion.</span></span> <span data-ttu-id="787b8-106">En el centro de la especificación del lenguaje se encuentra la definición del conjunto de datos sobre el que se puede escribir una consulta personalizada.</span><span class="sxs-lookup"><span data-stu-id="787b8-106">At the heart of the language specification is the dataset definition on which a custom query can be written.</span></span>

## <a name="datasets"></a><span data-ttu-id="787b8-107">Conjuntos de datos</span><span class="sxs-lookup"><span data-stu-id="787b8-107">Datasets</span></span>

<span data-ttu-id="787b8-108">Del mismo modo que algunas consultas se ejecutan en una base de datos que tiene tablas y columnas, una consulta personalizada funciona en conjuntos de datos que tienen columnas y métricas.</span><span class="sxs-lookup"><span data-stu-id="787b8-108">In the same way that some queries are run against a database that has tables and columns, a custom query works on Datasets that have columns and metrics.</span></span> <span data-ttu-id="787b8-109">La lista completa de los conjuntos de datos disponibles para formular una consulta puede obtenerse mediante la API de conjuntos de datos.</span><span class="sxs-lookup"><span data-stu-id="787b8-109">The full list of available datasets for formulating a query can be obtained by using the datasets API.</span></span>

<span data-ttu-id="787b8-110">Este es un ejemplo de un conjunto de datos que se muestra como JSON:</span><span class="sxs-lookup"><span data-stu-id="787b8-110">This is an example of a dataset shown as a JSON:</span></span>

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

## <a name="parts-of-a-dataset"></a><span data-ttu-id="787b8-111">Elementos de un conjunto de datos</span><span class="sxs-lookup"><span data-stu-id="787b8-111">Parts of a dataset</span></span>

- <span data-ttu-id="787b8-112">Un nombre de conjunto de datos es como el nombre de una tabla de base de datos.</span><span class="sxs-lookup"><span data-stu-id="787b8-112">A dataset name is like a database table name.</span></span> <span data-ttu-id="787b8-113">Por ejemplo, OfficeUsage.</span><span class="sxs-lookup"><span data-stu-id="787b8-113">For example, OfficeUsage.</span></span> <span data-ttu-id="787b8-114">Un conjunto de datos tiene una lista de columnas que se pueden seleccionar, como CustomerTenantId.</span><span class="sxs-lookup"><span data-stu-id="787b8-114">A dataset has a list of columns that can be selected, such as CustomerTenantId.</span></span>
- <span data-ttu-id="787b8-115">Un conjunto de datos también tiene métricas, que son como funciones de agregación en una base de datos.</span><span class="sxs-lookup"><span data-stu-id="787b8-115">A dataset also has metrics, which are like aggregation functions in a database.</span></span> <span data-ttu-id="787b8-116">Por ejemplo, TotalMonthlyActiveUsers.</span><span class="sxs-lookup"><span data-stu-id="787b8-116">For example, TotalMonthlyActiveUsers.</span></span>
- <span data-ttu-id="787b8-117">Hay intervalos de tiempo fijos durante los que se pueden exportar los datos.</span><span class="sxs-lookup"><span data-stu-id="787b8-117">There are fixed time spans over which data can be exported.</span></span>

## <a name="formulating-a-query-on-a-dataset"></a><span data-ttu-id="787b8-118">Formulación de una consulta en un conjunto de datos</span><span class="sxs-lookup"><span data-stu-id="787b8-118">Formulating a query on a dataset</span></span>

<span data-ttu-id="787b8-119">Estas son algunas consultas de ejemplo que muestran cómo extraer varios tipos de datos.</span><span class="sxs-lookup"><span data-stu-id="787b8-119">These are some sample queries that show how to extract various types of data.</span></span>

|<span data-ttu-id="787b8-120">Consultar</span><span class="sxs-lookup"><span data-stu-id="787b8-120">Query</span></span>|    <span data-ttu-id="787b8-121">Descripción</span><span class="sxs-lookup"><span data-stu-id="787b8-121">Description</span></span>    |
|----|    ----    |
|<span data-ttu-id="787b8-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="787b8-122">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="787b8-123">OfficeUsage **TIMESPAN** LAST_MONTH</span><span class="sxs-lookup"><span data-stu-id="787b8-123">OfficeUsage **TIMESPAN** LAST_MONTH</span></span>|    <span data-ttu-id="787b8-124">Esta consulta obtiene cada CusotmerTenantID y sus PaidAvailableUnits correspondientes en el último mes.</span><span class="sxs-lookup"><span data-stu-id="787b8-124">This query will get every CusotmerTenantID and its corresponding PaidAvailableUnits in the last 1 month.</span></span>    |
|<span data-ttu-id="787b8-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span><span class="sxs-lookup"><span data-stu-id="787b8-125">**SELECT** CustomerTenantId, PaidAvailableUnits **FROM**</span></span> <br><span data-ttu-id="787b8-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span><span class="sxs-lookup"><span data-stu-id="787b8-126">OfficeUsage **ORDER** BY PaidAvailableUnits **LIMIT** 10</span></span>|    <span data-ttu-id="787b8-127">Esta consulta obtiene los 10 inquilinos de clientes principales en orden decreciente del número de unidades disponibles de pago.</span><span class="sxs-lookup"><span data-stu-id="787b8-127">This query will get the top 10 customer tenants in decreasing order of the number of paid available units.</span></span>     |
|<span data-ttu-id="787b8-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span><span class="sxs-lookup"><span data-stu-id="787b8-128">**SELECT** CustomerTenantId, PaidAvailableUnits, MonthlyActiveUsers **FROM** OfficeUsage **WHERE** MonthlyActiveUsers > 100000 **ORDER BY** MonthlyActiveUsers **TIMESPAN** LAST_6_MONTHS</span></span> |    <span data-ttu-id="787b8-129">Esta consulta obtiene los PaidAvailableUnits y MonthlyActiveUsers de todos los clientes que tienen MonthlyActiveUsers superiores a 100 000.</span><span class="sxs-lookup"><span data-stu-id="787b8-129">This query will get the PaidAvailableUnits and MonthlyActiveUsers of all the Customers who have MonthlyActiveUsers greater than 100,000.</span></span>     |
|<span data-ttu-id="787b8-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span><span class="sxs-lookup"><span data-stu-id="787b8-130">**SELECT** CustomerTenantId, Month, MonthlyActiveUsers **FROM**</span></span> <br><span data-ttu-id="787b8-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span><span class="sxs-lookup"><span data-stu-id="787b8-131">OfficeUsage **WHERE** CustomerTpId IN ('2a31c234-1f4e-4c60-909e-76d234f93161', '80780748-3f9a-11eb-b378-0242ac130002')</span></span> |    <span data-ttu-id="787b8-132">Esta consulta obtiene CustomerTenantId y los usuarios activos mensuales para cada mes por los dos valores customerTpId: "2a31c234-1f4e-4c60-909e-176d234f93161" y "80780748-3f9a-11eb-b378-0242ac130002".</span><span class="sxs-lookup"><span data-stu-id="787b8-132">This query will get the CustomerTenantId and the monthly active users for every month by the two CustomerTpId values: '2a31c234-1f4e-4c60-909e-76d234f93161' and '80780748-3f9a-11eb-b378-0242ac130002'.</span></span>     |
|        |        |

## <a name="query-specification"></a><span data-ttu-id="787b8-133">Especificación de consulta</span><span class="sxs-lookup"><span data-stu-id="787b8-133">Query specification</span></span>

<span data-ttu-id="787b8-134">En esta sección se describe la definición y la estructura de la consulta.</span><span class="sxs-lookup"><span data-stu-id="787b8-134">This section describes the query definition and structure.</span></span>

## <a name="grammar-reference"></a><span data-ttu-id="787b8-135">Referencia de gramática</span><span class="sxs-lookup"><span data-stu-id="787b8-135">Grammar reference</span></span>

<span data-ttu-id="787b8-136">En esta tabla se describen los símbolos que se usan en las consultas.</span><span class="sxs-lookup"><span data-stu-id="787b8-136">This table describes the symbols used in queries.</span></span>

|    <span data-ttu-id="787b8-137">Consultar</span><span class="sxs-lookup"><span data-stu-id="787b8-137">Query</span></span>    |    <span data-ttu-id="787b8-138">Descripción</span><span class="sxs-lookup"><span data-stu-id="787b8-138">Description</span></span>    |
|    ----    |    ----    |
|    `?`    |    <span data-ttu-id="787b8-139">Opcionales</span><span class="sxs-lookup"><span data-stu-id="787b8-139">Optional</span></span>    |
|    `*`    |    <span data-ttu-id="787b8-140">Cero o más</span><span class="sxs-lookup"><span data-stu-id="787b8-140">Zero or more</span></span>    |
|    `+`    |    <span data-ttu-id="787b8-141">Uno o más</span><span class="sxs-lookup"><span data-stu-id="787b8-141">One or more</span></span>    |
|    `\|`    |    <span data-ttu-id="787b8-142">O / Una de las listas</span><span class="sxs-lookup"><span data-stu-id="787b8-142">Or / One of the lists</span></span>    |
|        |        |

## <a name="query-definition"></a><span data-ttu-id="787b8-143">Definición de la consulta</span><span class="sxs-lookup"><span data-stu-id="787b8-143">Query definition</span></span>

<span data-ttu-id="787b8-144">La instrucción query tiene las siguientes cláusulas: SelectClause, FromClause, WhereClause, OrderClause, LimitClause y TimeSpan.</span><span class="sxs-lookup"><span data-stu-id="787b8-144">The query statement has the following clauses: SelectClause, FromClause, WhereClause, OrderClause, LimitClause, and TimeSpan.</span></span>

- <span data-ttu-id="787b8-145">**SeleccioneClausar:**`SELECT ColumOrMetricName (, ColumOrMetricName)*`</span><span class="sxs-lookup"><span data-stu-id="787b8-145">**SelectClause**: `SELECT ColumOrMetricName (, ColumOrMetricName)*`</span></span>
    - <span data-ttu-id="787b8-146">**ColumOrMetricName**: columnas y métricas definidas en el conjunto de datos</span><span class="sxs-lookup"><span data-stu-id="787b8-146">**ColumOrMetricName**: Columns and Metrics defined within the Dataset</span></span>
- <span data-ttu-id="787b8-147">**FromClause**: `FROM DatasetName`</span><span class="sxs-lookup"><span data-stu-id="787b8-147">**FromClause**: `FROM DatasetName`</span></span>
    - <span data-ttu-id="787b8-148">**DatasetName**: nombre del conjunto de datos definido en el conjunto de datos</span><span class="sxs-lookup"><span data-stu-id="787b8-148">**DatasetName**: Dataset name defined within the Dataset</span></span>
- <span data-ttu-id="787b8-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span><span class="sxs-lookup"><span data-stu-id="787b8-149">**WhereClause**: `WHERE FilterCondition (AND FilterCondition)`</span></span>
    - <span data-ttu-id="787b8-150">**FilterCondition**: valor del operador ColumOrMetricName</span><span class="sxs-lookup"><span data-stu-id="787b8-150">**FilterCondition**: ColumOrMetricName Operator Value</span></span>
        - <span data-ttu-id="787b8-151">**Operador**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span><span class="sxs-lookup"><span data-stu-id="787b8-151">**Operator**:  `=` | `>` | `<` | `>=` | `<=` | `!=` | `LIKE` | `NOT LIKE` | `IN` | `NOT IN`</span></span>
        - <span data-ttu-id="787b8-152">**Valor**: Number | StringLiteral | MultiNumberList | MultiStringList</span><span class="sxs-lookup"><span data-stu-id="787b8-152">**Value**: Number | StringLiteral | MultiNumberList | MultiStringList</span></span>
            - <span data-ttu-id="787b8-153">**Número:**`-? [0-9]+ (. [0-9] [0-9]*)?`</span><span class="sxs-lookup"><span data-stu-id="787b8-153">**Number**: `-? [0-9]+ (. [0-9] [0-9]*)?`</span></span>
            - <span data-ttu-id="787b8-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span><span class="sxs-lookup"><span data-stu-id="787b8-154">**StringLiteral**:  `' [a-zA-Z0-9_]*'`</span></span>
            - <span data-ttu-id="787b8-155">**MultiNumberList**: `(Number (,Number)*)`</span><span class="sxs-lookup"><span data-stu-id="787b8-155">**MultiNumberList**: `(Number (,Number)*)`</span></span>
            - <span data-ttu-id="787b8-156">**MultiStringList**: `(StringLiteral (,StringLiteral)*)`</span><span class="sxs-lookup"><span data-stu-id="787b8-156">**MultiStringList**: `(StringLiteral (,StringLiteral)*)`</span></span>
- <span data-ttu-id="787b8-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span><span class="sxs-lookup"><span data-stu-id="787b8-157">**OrderClause**: `ORDER BY OrderCondition (,OrderCondition)`</span></span>
    - <span data-ttu-id="787b8-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span><span class="sxs-lookup"><span data-stu-id="787b8-158">**OrderCondition**: `ColumOrMetricName (ASC | DESC)*`</span></span>
- <span data-ttu-id="787b8-159">**LimitClause**: `LIMIT [0-9]+`</span><span class="sxs-lookup"><span data-stu-id="787b8-159">**LimitClause**: `LIMIT [0-9]+`</span></span>
- <span data-ttu-id="787b8-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span><span class="sxs-lookup"><span data-stu-id="787b8-160">**TimeSpan**: `TIMESPAN ( TODAY | YESTERDAY | LAST_7_DAYS | LAST_14_DAYS |LAST_30_DAYS | LAST_90_DAYS | LAST_180_DAYS | LAST_365_DAYS |LAST_MONTH | LAST_3_MONTHS | LAST_6_MONTHS | LAST_1_YEAR | LIFETIME)`</span></span>

## <a name="query-structure"></a><span data-ttu-id="787b8-161">Estructura de la consulta</span><span class="sxs-lookup"><span data-stu-id="787b8-161">Query Structure</span></span>

<span data-ttu-id="787b8-162">Una consulta de informe se compone de varios elementos:</span><span class="sxs-lookup"><span data-stu-id="787b8-162">A Report query is made up of multiple parts:</span></span>
- `SELECT`
- `FROM`
- `WHERE`
- `ORDER BY`
- `LIMIT`
- `TIMESPAN`

<span data-ttu-id="787b8-163">A continuación, se describe cada uno de los elementos.</span><span class="sxs-lookup"><span data-stu-id="787b8-163">Each part is described below.</span></span>

### `SELECT`

<span data-ttu-id="787b8-164">Este elemento de la consulta especifica las columnas que se exportarán.</span><span class="sxs-lookup"><span data-stu-id="787b8-164">This part of the query specifies the columns that will get exported.</span></span> <span data-ttu-id="787b8-165">Las columnas que se pueden seleccionar son los campos *enumerados en selectableColumns* y *availableMetrics* secciones de un conjunto de datos.</span><span class="sxs-lookup"><span data-stu-id="787b8-165">The columns that can be selected are the fields listed in *selectableColumns* and *availableMetrics* sections of a dataset.</span></span>

<span data-ttu-id="787b8-166">Opcionalmente, `DISTINCT` la palabra clave se puede especificar después de `SELECT` .</span><span class="sxs-lookup"><span data-stu-id="787b8-166">Optionally, `DISTINCT` keyword can be specified after `SELECT`.</span></span> <span data-ttu-id="787b8-167">Si `DISTINCT` se especifica , las filas exportadas finales siempre contendrán valores distintos de las columnas seleccionadas.</span><span class="sxs-lookup"><span data-stu-id="787b8-167">If `DISTINCT` is specified, then the final exported rows will always contain distinct values of the selected columns.</span></span> <span data-ttu-id="787b8-168">Las métricas se calcularán para cada combinación distinta de las columnas seleccionadas, por lo que la palabra clave no es necesaria cuando se incluye una columna de métrica `DISTINCT` en la lista seleccionar columna.</span><span class="sxs-lookup"><span data-stu-id="787b8-168">Metrics will be calculated for every distinct combination of the selected columns, hence `DISTINCT` keyword is not required when a metric column is included in the select column list.</span></span>

<span data-ttu-id="787b8-169">**Ejemplo**:</span><span class="sxs-lookup"><span data-stu-id="787b8-169">**Example:**</span></span>

```sql
SELECT CustomerTenantId, PaidAvailableUnits; 
SELECT DISTINCT CustomerTenantId
```

### `FROM`

<span data-ttu-id="787b8-170">Este elemento de la consulta indica el conjunto de datos desde el que se deben exportar los datos.</span><span class="sxs-lookup"><span data-stu-id="787b8-170">This part of the query indicates the dataset from which data needs to be exported.</span></span> <span data-ttu-id="787b8-171">El nombre del conjunto de datos que se proporciona aquí debe ser un nombre de conjunto de datos válido devuelto por la API de los conjuntos de datos.</span><span class="sxs-lookup"><span data-stu-id="787b8-171">The dataset name given here needs to be a valid dataset name returned by the datasets API.</span></span>

<span data-ttu-id="787b8-172">**Ejemplo**:</span><span class="sxs-lookup"><span data-stu-id="787b8-172">**Example:**</span></span>

- `FROM  OfficeUsage`
- `FROM  AzureUsage`

### `WHERE`

<span data-ttu-id="787b8-173">Este elemento de la consulta se usa para especificar las condiciones de filtro en el conjunto de datos.</span><span class="sxs-lookup"><span data-stu-id="787b8-173">This part of the query is used to specify filter conditions on the dataset.</span></span> <span data-ttu-id="787b8-174">Solo las filas que coincidan con todas las condiciones enumeradas en esta cláusula estarán presentes en el archivo final exportado.</span><span class="sxs-lookup"><span data-stu-id="787b8-174">Only rows matching all the conditions listed in this clause will be present in the final exported file.</span></span> <span data-ttu-id="787b8-175">La condición de filtro puede estar en cualquiera de las columnas enumeradas *en selectableColumns* y *availableMetrics*.</span><span class="sxs-lookup"><span data-stu-id="787b8-175">The filter condition can be on any of the columns listed in *selectableColumns* and *availableMetrics*.</span></span> <span data-ttu-id="787b8-176">Los valores especificados en la condición de filtro pueden ser una lista de números o una lista de cadenas solo cuando el operador es `IN` o `NOT IN`.</span><span class="sxs-lookup"><span data-stu-id="787b8-176">The values specified in the filter condition can be a list of numbers or a list of strings only when the operator is `IN` or `NOT IN`.</span></span> <span data-ttu-id="787b8-177">Siempre se pueden proporcionar los valores como una cadena literal y se convertirán en los tipos nativos de columnas.</span><span class="sxs-lookup"><span data-stu-id="787b8-177">The values can always be given as a literal string and they will be converted to the native types of columns.</span></span> <span data-ttu-id="787b8-178">Es necesario separar varias condiciones de filtro con una operación AND.</span><span class="sxs-lookup"><span data-stu-id="787b8-178">Multiple filter conditions need to be separated with an AND operation.</span></span>

<span data-ttu-id="787b8-179">**Ejemplo**:</span><span class="sxs-lookup"><span data-stu-id="787b8-179">**Example:**</span></span>

- `CustomerTenantId= '868368da-957d-4959-8992-3c12dc7e6260'`
- `CustomerName LIKE '%Contoso%'`
- `CustomerId NOT IN (1000, 1001, 1002)`
- `OrderQuantity=100`
- `CustomerTenantId='7b487ac0-ce12-b732-dcd6-91a1e4e74a50' AND CustomerTpId=' 0f8b7fa0-eb83-a183-1225-ca153ef807aa'`

### `ORDER BY`

<span data-ttu-id="787b8-180">En este elemento de la consulta se especifican los criterios de ordenación de las filas exportadas.</span><span class="sxs-lookup"><span data-stu-id="787b8-180">This part of the query specifies the ordering criteria for the exported rows.</span></span> <span data-ttu-id="787b8-181">Las columnas en las que se puede definir la ordenación deben ser de *selectableColumns* y *availableMetrics* del conjunto de datos.</span><span class="sxs-lookup"><span data-stu-id="787b8-181">The columns on which ordering can be defined need to be from the *selectableColumns* and *availableMetrics* of the dataset.</span></span> <span data-ttu-id="787b8-182">Si no se especifica ninguna dirección de ordenación, el valor predeterminado será DESC en la columna.</span><span class="sxs-lookup"><span data-stu-id="787b8-182">If there is no ordering direction specified, it will be defaulted to DESC on the column.</span></span> <span data-ttu-id="787b8-183">La ordenación se puede definir en varias columnas separando los criterios con una coma.</span><span class="sxs-lookup"><span data-stu-id="787b8-183">Ordering can be defined on multiple columns by separating the criteria with a comma.</span></span>

<span data-ttu-id="787b8-184">**Ejemplo**:</span><span class="sxs-lookup"><span data-stu-id="787b8-184">**Example:**</span></span>

- `ORDER BY  MonthlyActiveUsers ASC,  Month DESC`
- `ORDER BY CustomerName ASC,  Month`

### `LIMIT`

<span data-ttu-id="787b8-185">Este elemento de la consulta especifica el número de filas que se exportarán.</span><span class="sxs-lookup"><span data-stu-id="787b8-185">This part of the query specifies the number of rows that will be exported.</span></span> <span data-ttu-id="787b8-186">El número que especifique debe ser un entero positivo distinto de cero.</span><span class="sxs-lookup"><span data-stu-id="787b8-186">The number you specify needs to be a positive nonzero integer.</span></span>

### `TIMESPAN`

<span data-ttu-id="787b8-187">Este elemento de la consulta especifica el período de tiempo durante el que se deben exportar los datos.</span><span class="sxs-lookup"><span data-stu-id="787b8-187">This part of the query specifies the time duration for which the data needs to be exported.</span></span> <span data-ttu-id="787b8-188">Los valores posibles deben ser del *campo availableDateRanges* de la definición del conjunto de datos.</span><span class="sxs-lookup"><span data-stu-id="787b8-188">The possible values should be from the *availableDateRanges* field in the dataset definition.</span></span>

### <a name="case-sensitivity-in-query-specification"></a><span data-ttu-id="787b8-189">Distinción de mayúsculas y minúsculas en la especificación de consultas</span><span class="sxs-lookup"><span data-stu-id="787b8-189">Case sensitivity in query specification</span></span>

<span data-ttu-id="787b8-190">La especificación no distingue entre mayúsculas y minúsculas.</span><span class="sxs-lookup"><span data-stu-id="787b8-190">The specification is completely case insensitive.</span></span> <span data-ttu-id="787b8-191">Las palabras clave predefinidas, los nombres de columna y los valores se pueden especificar usando mayúsculas o minúsculas.</span><span class="sxs-lookup"><span data-stu-id="787b8-191">Predefined keywords, column names and values can be specified using upper or lower case.</span></span>

## <a name="next-steps"></a><span data-ttu-id="787b8-192">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="787b8-192">Next steps</span></span>

- [<span data-ttu-id="787b8-193">Lista de consultas del sistema</span><span class="sxs-lookup"><span data-stu-id="787b8-193">List of system queries</span></span>](insights-programmatic-system-queries.md)
- [<span data-ttu-id="787b8-194">Lista de consultas de ejemplo</span><span class="sxs-lookup"><span data-stu-id="787b8-194">List of sample queries</span></span>](insights-programmatic-sample-queries.md)