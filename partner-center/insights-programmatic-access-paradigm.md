---
title: Paradigma de acceso mediante programación para Ideas datos
description: Descripción del flujo de alto nivel del patrón de llamada de API para el análisis mediante programación. También se tratan las API para acceder a los informes de análisis de Conclusiones de asociados.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: dcdd54fcc744fdb1683259203188c309a3949eff
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375889"
---
# <a name="programmatic-access-paradigm"></a>Paradigma del acceso mediante programación

En este diagrama se muestra el patrón de llamada API que se usa para crear una nueva plantilla de informe, programar el informe personalizado y recuperar los datos de error.

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Flujo de alto nivel":::
***Figura 1: Flujo de alto nivel del patrón de llamada API***

En esta lista se proporcionan más detalles sobre la figura 1.

1. La aplicación cliente puede definir el esquema o plantilla del informe personalizado llamando a la [API de creación de consultas de informes](#create-report-query-api). Como alternativa, puede elegir una plantilla de informe (QueryId) de los ejemplos de biblioteca de plantillas de informe que se enumeran [aquí.](insights-programmatic-system-queries.md)
2. Si se ejecuta correctamente, Create Report Query API devuelve queryId.
3. A continuación, la aplicación cliente debe llamar a [Create Report API](#create-report-api) mediante QueryId junto con la fecha de inicio del informe, el intervalo de repetición, la periodicidad y un URI de devolución de llamada opcional.
4. Si se ejecuta correctamente, [Create Report API](#create-report-api) devuelve reportId.
5. La aplicación cliente recibe una notificación en la dirección URL de devolución de llamada en cuanto los datos del informe están listos para su descarga.
6. A continuación, la aplicación cliente usa [get report executions API](#get-report-execution-api) para consultar el estado del informe con el identificador de informe y el intervalo de fechas.
7. Si se ejecuta correctamente, se devuelve el vínculo de descarga del informe y la aplicación puede iniciar la descarga de los datos.

## <a name="report-query-language-specification"></a>Especificación del lenguaje de consulta de informes

Aunque proporcionamos [consultas del sistema](insights-programmatic-system-queries.md) que puede usar para crear informes, también puede crear sus propias consultas en función de sus necesidades empresariales. Para más información sobre las consultas personalizadas, consulte [Especificación de consultas personalizadas.](insights-programmatic-custom-query.md)

## <a name="create-report-query-api"></a>API de creación de consultas de informes

La API ayuda a crear consultas personalizadas que definen el conjunto de datos desde el que se deben exportar las columnas y las métricas. La API proporciona la flexibilidad para crear una nueva plantilla de informes en función de sus necesidades empresariales.  

También puede usar las [consultas del sistema](insights-programmatic-system-queries.md) que proporcionamos. Cuando no se necesitan plantillas de informe personalizadas, puede llamar a [Create Report API](#create-report-api) directamente mediante los QueryId de las consultas del sistema que se proporcionan.  

En el ejemplo siguiente se muestra cómo crear una consulta personalizada para obtener los 10 clientes principales por ingresos del mes pasado.

### <a name="request-syntax"></a>Sintaxis de la solicitud

|    Método     |    URI de solicitud     |
|----- | -----|
|    POST     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a>Encabezado de solicitud

|    Encabezado     |    Tipo     |    Descripción     |
|-------|-----|------|
|    Authorization     |    string |Necesario. El token de acceso de Azure Active Directory (Azure AD). El formato es  `Bearer <token>` .|
|    Content-Type     |string |`Application/JSON` |
||||

### <a name="path-parameter"></a>Parámetro Path

Ninguno

### <a name="query-parameter"></a>Parámetro de consulta

Ninguno

### <a name="sample-request-payload"></a>Carga de solicitud de ejemplo

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a>Glosario

En esta tabla se proporcionan las definiciones clave de los elementos de la carga de solicitud.

|Parámetro|    Obligatorio     |    Descripción     |    Valores permitidos     |
|-----|    -----    |    -----    |    -----    |
|Nombre |    Sí     |    Nombre descriptivo de la consulta     |    string     |
|    Descripción     |    No     |    Descripción de lo que devuelve la consulta     |    string     |
|    Consultar     |    Sí     |    Cadena de consulta del informe.     |    Tipo de datos: cadena <br> [Consulta personalizada](insights-programmatic-custom-query.md) basada en la necesidad empresarial |
|        |        |        |        |

> [!Note]
> Para obtener ejemplos de consultas personalizadas, [consulte Ejemplos de consultas de ejemplo.](insights-programmatic-sample-queries.md)

### <a name="sample-response"></a>Respuesta de muestra

La carga de respuesta tiene la estructura siguiente:

Códigos de respuesta: 200, 400, 401, 403, 500

Ejemplo de carga de respuesta:

```json
{ 
  "value": [ 
    { 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
      "name": "CustomersRevenueQuery",
      "description": "Query to get top 10 customers by revenue for last month",
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH",
      "type": "userDefined",
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T12:52:39Z" 
    }
  ], 
  "nextLink": null,
  "totalCount": 1,
  "message": "Query created successfully",
  "statusCode": 200,
  "dataRedacted": false
} 
```

### <a name="glossary"></a>Glosario

En esta tabla se proporcionan las definiciones clave de los elementos de la carga de solicitud.

|    Parámetro     |    Descripción     |
|    ----    |    ----    |
|    QueryId     |    Identificador único universal (UUID) de la consulta que creó     |
|    Nombre     |    Nombre descriptivo dado a la consulta en la carga de la solicitud     |
|    Descripción     |    Descripción proporcionada durante la creación de la consulta.     |
|    Consultar     |    Consulta de informe pasada como entrada durante la creación de la consulta     |
|    Tipo     |    Establézcala en `userDefined`     |
|    Usuario     |    Identificador de usuario usado para crear la consulta     |
|    CreatedTime     |    Hora UTC en que se creó la consulta en el formato aaaa-MM-ddTHH:mm:ssZ     |
|    TotalCount     |    Número de conjuntos de datos en la matriz de valores.     |
|    StatusCode     |    Código de resultado <br> Los valores posibles son 200, 400, 401, 403 y 500.     |
|    message     |    Mensaje de estado de la ejecución de la API.     |
|        |        |

## <a name="create-report-api"></a>API de creación de informes

Al crear correctamente una plantilla de informe personalizada [](#create-report-query-api) y recibir el QueryID como parte de la respuesta Crear consulta de informe, se puede llamar a esta API para programar una consulta que se ejecutará a intervalos regulares. Puede establecer una frecuencia y una programación para la entrega del informe.
En el caso de las consultas del sistema que proporcionamos, también se puede llamar a la API de creación de informes con [QueryId](insights-programmatic-system-queries.md).

### <a name="callback-url"></a>Dirección URL de devolución de llamadas

La API de creación de informes acepta una dirección URL de devolución de llamada. Se llamará a esta dirección URL una vez que la generación del informe sea correcta. La dirección URL de devolución de llamada debe ser accesible públicamente. Además de la dirección URL, también se puede dar un método de devolución de llamada. El método de devolución de llamada solo puede ser "GET" o "POST". El método predeterminado si no se pasa ningún valor será "POST". El reportId que ha completado la generación siempre se pasará de vuelta durante la devolución de llamada.

Devolución de llamada POST: si la dirección URL pasada era , la dirección URL de devolución a la que se `https://www.contosso.com/callback` llamó será `https://www.contosso.com/callback/<reportID>` 

Devolución de llamada GET: si la dirección URL pasada era , la dirección URL de devolución a la `https://www.contosso.com/callback` que se llamó será `https://www.contosso.com/callback?reportId=<reportID>` 

### <a name="executenow-reports"></a>Informes de ExecuteNow

Hay un aprovisionamiento para generar un informe sin programación. La carga de la API de creación de informes puede aceptar un parámetro , que pondrá en cola el informe para que se genere en cuanto se llame `ExecuteNow` a la API. Cuando `ExecuteNow` se establece en true, se omiten los campos: , , ya que estos informes no están `StartTime` `RecurrenceCount` `RecurrenceInterval` programados.

Se pueden pasar dos campos adicionales cuando `ExecuteNow` es true, `QueryStartTime` y `QueryEndTime` . Estos dos campos invalidarán el `TIMESPAN` campo de la consulta. Estos campos no son aplicables a los informes programados, ya que los datos se generarán continuamente durante un período de tiempo fijo que no cambia.

### <a name="request-syntax"></a>Sintaxis de la solicitud

|    Método     |    URI de solicitud     |
|----- | -----|
|    POST     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a>Encabezado de solicitud

|    Encabezado     |    Tipo     |    Descripción     |
|-------|-----|------|
|    Authorization     |    string |Necesario. El token de acceso de Azure Active Directory (Azure AD). El formato es  `Bearer <token>` .|
|    Content-Type     |string |`Application/JSON` |

### <a name="path-parameter"></a>Parámetro de ruta de acceso

Ninguno

### <a name="query-parameter"></a>Parámetro de consulta

Ninguno

### <a name="sample-request-payload"></a>Carga de solicitud de ejemplo

```json
{
  "ReportName": "Top10_CustomersReport",
  "Description": "Top 10 customers by revenue for last month",
  "QueryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033",
  "StartTime": "2021-03-31T18:41:00Z",
  "ExecuteNow": false,
  "QueryStartTime": null,
  "QueryEndTime": null,
  "RecurrenceInterval": 24,
  "RecurrenceCount": 100,
  "Format": "CSV",
  "CallbackUrl": "https://<SampleCallbackUrl>",
  "CallbackMethod": "GET"
}
```

### <a name="glossary"></a>Glosario

Las definiciones clave de los elementos de la carga de solicitud se articulan a continuación:

|    Parámetro     |    Obligatorio     |    Descripción     |    Valores permitidos     |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Sí     |    Nombre que se va a asignar al informe     |    string     |
|    Descripción     |    No     |    Descripción del informe creado     |    string     |
|    QueryId     |    Sí     |    Id. de consulta del informe.     |    string     |
|    StartTime     |    Sí     |    Marca de tiempo UTC en la que comenzará la generación del informe. <br> El formato debe ser aaaa-MM-ddTHH:mm:ssZ.       |    string     |
|    ExecuteNow     |    No     |    Este parámetro debe usarse para crear un informe que se ejecutará una sola vez. `StartTime`, `RecurrenceInterval` y `RecurrenceCount` se omiten si se establece en true. El informe se ejecuta inmediatamente de forma asincrónica     |    true/false     |
|    QueryStartTime     |    No     |    Opcionalmente, especifica la hora de inicio de la consulta que extrae los datos. Este parámetro solo es aplicable para un informe de ejecución de una vez que `ExecuteNow` se ha establecido en true. Al establecer este parámetro se invalida `TIMESPAN` el especificado en la consulta. El formato debe ser aaaa-MM-ddTHH:mm:ssZ.     |    Marca de tiempo como string     |
|    QueryEndTime     |    No     |    Opcionalmente, especifica la hora de fin de la consulta que extrae los datos. Este parámetro solo es aplicable para un informe de ejecución de una vez que `ExecuteNow` se ha establecido en true. Al establecer este parámetro se invalida `TIMESPAN` el especificado en la consulta. El formato debe ser aaaa-MM-ddTHH:mm:ssZ.     |    Marca de tiempo como string     |
|    RecurrenceInterval     |    Sí     |    Frecuencia en horas en que se debe generar el informe. <br> El valor mínimo es 4 y el valor máximo es 2160.      |    integer     |
|    RecurrenceCount     |    No     |    Número de informes que se van a generar.     |    integer     |
|    Formato     |    No     |    Formato del archivo exportado. <br> El valor predeterminado es CSV.    |    "CSV"/"TSV"     |
|    CallbackUrl     |    No     |    Dirección URL accesible públicamente que se puede configurar opcionalmente como destino de devolución de llamada     |    Cadena (dirección URL http)     |
|    CallbackMethod     |    No     |    Método que se va a usar para la devolución de llamada     |    GET/POST     |
|        |        |        |        |

### <a name="sample-response"></a>Respuesta de muestra

La carga de respuesta tiene la estructura siguiente:

Códigos de respuesta: 200, 400, 401, 403, 404, 500

Ejemplo de carga de respuesta:

```json
{ 
  "value": [
    { 
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf", 
      "reportName": "Top10_CustomersReport", 
      "description": "Top 10 customers by revenue for last month", 
      "queryId": "ec8366a4-d96e-4194-8c37-d5dbc0639033", 
      "query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH", 
      "user": "GAUser@PITEST2.ccsctp.net", 
      "createdTime": "2021-03-30T13:11:58Z", 
      "modifiedTime": null, 
      "executeNow": false, 
      "startTime": "2021-03-31T18:41:00Z", 
      "reportStatus": "Active", 
      "recurrenceInterval": 24, 
      "recurrenceCount": 100, 
      "callbackUrl": "https://<SampleCallbackUrl>", 
      "callbackMethod": "GET", 
      "format": "csv"
    } 
  ], 
  "nextLink": null, 
  "totalCount": 1, 
  "message": "Report created successfully", 
  "statusCode": 200, 
  "dataRedacted": false 
}
```

### <a name="glossary"></a>Glosario

Las definiciones clave de los elementos de la respuesta se articulan a continuación:

|    Parámetro     |    Descripción     |
|    ----    |    ----    |
|    ReportId     |    Identificador único universal (UUID) del informe que creó.     |
|    ReportName     |    Nombre dado al informe en la carga útil de solicitud     |
|    Descripción     |    Descripción proporcionada durante la creación del informe.     |
|    QueryId     |    Id. de consulta pasado en el momento en que creó el informe.     |
|    Consultar     |    Texto de la consulta que se ejecutará para este informe.     |
|    Usuario     |    Identificador de usuario usado para crear el informe     |
|    CreatedTime     |    Hora UTC en que se creó el informe en el formato aaaa-MM-ddTHH:mm:ssZ.     |
|    ModifiedTime     |    Hora UTC en que se modificó el informe en el formato aaaa-MM-ddTHH:mm:ssZ.     |
|    ExecuteNow     |    `ExecuteNow` marca establecida en el momento en que se creó el informe     |
|    StartTime     |    Hora UTC en que se iniciará la ejecución del informe en el formato aaaa-MM-ddTHH:mm:ssZ     |
|    ReportStatus     |    Estado de la ejecución del informe. Los valores posibles `Paused` son `Active` , y `Inactive`     |
|    RecurrenceInterval     |    Intervalo de periodicidad proporcionado durante la creación del informe.     |
|    RecurrenceCount     |    Recuento de periodicidad proporcionado durante la creación del informe.      |
|    CallbackUrl     |    Dirección URL de devolución de llamada proporcionada en la solicitud.     |
|    CallbackMethod     |    Método de devolución de llamada proporcionado en la solicitud     |
|    Formato     |    Formato de los archivos de informe. Los valores posibles son `CSV` o `TSV` .     |
|    TotalCount     |    Número de registros de la matriz Value     |
|    StatusCode     |    Código de resultado     |
|    message     |    Los valores posibles son 200, 400, 401, 403, 500. Mensaje de estado de la ejecución de la API.     |
|        |        |

## <a name="get-report-execution-api"></a>Obtener la API de ejecución de informes

Puede usar este método para consultar el estado de una ejecución de informe mediante el ReportId recibido de [Create Report API.](#create-report-api) El método devuelve el vínculo de descarga del informe si el informe está listo para su descarga. De lo contrario, el método devolverá el estado. También puede usar esta API para obtener todas las ejecuciones que se han producido para un informe determinado.  

>[!IMPORTANT]
>Esta API tiene parámetros de consulta predeterminados establecidos para `executionStatus=Completed` y `getLatestExecution=true` . Por lo tanto, si se llama a la API antes de la primera ejecución correcta del informe devolverá 404. Las ejecuciones pendientes se pueden obtener estableciendo `executionStatus=Pending`.

### <a name="request-syntax"></a>Sintaxis de la solicitud

|    Método     |    URI de solicitud     |
|----- | -----|
|    GET    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a>Encabezado de solicitud

|    Encabezado     |    Tipo     |    Descripción     |
|-------|-----|------|
|    Authorization     |    string |Necesario. El token de acceso de Azure Active Directory (Azure AD). El formato es  `Bearer <token>` .|
|    Content-Type     |string |`Application/JSON` |

### <a name="path-parameter"></a>Parámetro Path

|    Nombre de parámetro    |    Obligatorio    |    Tipo    |    Descripción    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId    |    Sí    |    string    |    Filtre para obtener los detalles de ejecución de solo los informes con el valor de reportId especificado en este argumento. Se pueden especificar varios reportIds si se separan con un punto y coma ";".    |
|        |        |        |        |

### <a name="query-parameter"></a>Parámetro de consulta

|    Nombre de parámetro    |    Obligatorio    |    Tipo    |    Descripción    |
|    ----    |    ----    |    ----    |    ----    |
|    executionId    |    No    |    string    |    Filtre para obtener detalles de solo los informes con el executionId especificado en este argumento. Se pueden especificar varios executionIds si se separan con un punto y coma ";".    |
|    executionStatus    |    No    |    Cadena/enumeración    |    Filtre para obtener detalles de solo los informes con executionStatus especificado en este argumento. <br> Los valores válidos `Pending` son: `Running` , y `Paused` `Completed` . <br> El valor predeterminado es `Completed`. <br> Se pueden especificar varios estados si se separan con un punto y coma ";".    |
|    getLatestExecution    |    No    |    boolean    |    La API devolverá los detalles de la ejecución más reciente. De forma predeterminada, este parámetro se establece en true.<br> Si decide pasar el valor de este parámetro como false, la API devolverá las instancias de ejecución de los últimos 90 días.    |
|        |        |        |        |

### <a name="sample-request-payload"></a>Carga de solicitud de ejemplo

Ninguno

### <a name="sample-response"></a>Respuesta de ejemplo

La carga de respuesta tiene la estructura siguiente:

Códigos de respuesta: 200, 400, 401, 403, 404, 500

Ejemplo de carga de respuesta:

```json
{
  "value": [
    {
      "executionId": "906931dc-4f2f-4195-bbb2-d7295c7550d3",
      "reportId": "d9548477-16d4-492a-bf9c-0cf91a9f69bf",
      "recurrenceInterval": 24,
      "recurrenceCount": 100,
      "callbackUrl": null,
      "callbackMethod": null,
      "format": "csv",
      "executionStatus": "Completed",
      "reportLocation": null,
      "reportAccessSecureLink": "https://<path to report for download>",
      "reportExpiryTime": null,
      "reportGeneratedTime": "2021-03-31T18:41:00Z"
    }
  ],
  "nextLink": null,
  "totalCount": 1,
  "message": null,
  "statusCode": 200,
  "dataRedacted": false
}
```

Una vez completada la ejecución del informe, se muestra el estado de ejecución `Completed`. Puede descargar el informe seleccionando la dirección URL en `reportAccessSecureLink`.

### <a name="glossary"></a>Glosario

Definiciones clave de los elementos de la respuesta.

|    Parámetro    |    Descripción    |
|    ----    |    ----    |
|    ExecutionId    |    Identificador único universal (UUID) de la instancia de ejecución.    |
|    ReportId    |    Id. de informe asociado a la instancia de ejecución.    |
|    RecurrenceInterval    |    Intervalo de periodicidad proporcionado durante la creación del informe.    |
|    RecurrenceCount    |    Recuento de periodicidad proporcionado durante la creación del informe.    |
|    CallbackUrl    |    Dirección URL de devolución de llamada asociada a la instancia de ejecución.    |
|    CallbackMethod    |    Método de devolución de llamada asociado a la instancia de ejecución    |
|    Formato    |    Formato del archivo generado al final de la ejecución.    |
|    ExecutionStatus    |    Estado de la instancia de ejecución del informe. <br> Los valores válidos son `Pending`, `Running`, `Paused` y `Completed`.    |
|    ReportAccessSecureLink    |Vínculo a través del cual se puede acceder al informe de forma segura.        |
|    ReportExpiryTime    |    Hora UTC después de la cual el vínculo de informe expirará en el formato aaaa-MM-ddTHH:mm:ssZ.    |
|    ReportGeneratedTime    |    Hora UTC a la que se generó el informe en el formato aaaa-MM-ddTHH:mm:ssZ.    |
|    TotalCount    |    Número de conjuntos de datos en la matriz de valores.    |
|    StatusCode    |    Código de resultado <br> Los valores posibles son 200, 400, 401, 403, 404 y 500.    |
|    message    |    Mensaje de estado de la ejecución de la API.    |
|        |        |

## <a name="next-steps"></a>Pasos siguientes

- Pruebe las API a través de la dirección [URL de la API de swagger.](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)
- [Realice su primera llamada API](insights-programmatic-first-api-call.md)