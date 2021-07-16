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
# <a name="programmatic-access-paradigm"></a><span data-ttu-id="47fb8-104">Paradigma del acceso mediante programación</span><span class="sxs-lookup"><span data-stu-id="47fb8-104">Programmatic access paradigm</span></span>

<span data-ttu-id="47fb8-105">En este diagrama se muestra el patrón de llamada API que se usa para crear una nueva plantilla de informe, programar el informe personalizado y recuperar los datos de error.</span><span class="sxs-lookup"><span data-stu-id="47fb8-105">This diagram shows the API call pattern used to create a new report template, schedule the custom report and retrieve failure data.</span></span>

:::image type="content" source="images/insights/prog-acc-paradigm.png" alt-text="Flujo de alto nivel":::
<span data-ttu-id="47fb8-107">***Figura 1: Flujo de alto nivel del patrón de llamada API***</span><span class="sxs-lookup"><span data-stu-id="47fb8-107">***Figure 1: High level flow of the API call pattern***</span></span>

<span data-ttu-id="47fb8-108">En esta lista se proporcionan más detalles sobre la figura 1.</span><span class="sxs-lookup"><span data-stu-id="47fb8-108">This list provides more details about Figure 1.</span></span>

1. <span data-ttu-id="47fb8-109">La aplicación cliente puede definir el esquema o plantilla del informe personalizado llamando a la [API de creación de consultas de informes](#create-report-query-api).</span><span class="sxs-lookup"><span data-stu-id="47fb8-109">The Client Application can define the custom report schema/template by calling the [Create Report Query API](#create-report-query-api).</span></span> <span data-ttu-id="47fb8-110">Como alternativa, puede elegir una plantilla de informe (QueryId) de los ejemplos de biblioteca de plantillas de informe que se enumeran [aquí.](insights-programmatic-system-queries.md)</span><span class="sxs-lookup"><span data-stu-id="47fb8-110">Alternately, you can pick a report template (QueryId) from the report template library samples listed [here.](insights-programmatic-system-queries.md)</span></span>
2. <span data-ttu-id="47fb8-111">Si se ejecuta correctamente, Create Report Query API devuelve queryId.</span><span class="sxs-lookup"><span data-stu-id="47fb8-111">On success, the Create Report Query API returns the QueryId.</span></span>
3. <span data-ttu-id="47fb8-112">A continuación, la aplicación cliente debe llamar a [Create Report API](#create-report-api) mediante QueryId junto con la fecha de inicio del informe, el intervalo de repetición, la periodicidad y un URI de devolución de llamada opcional.</span><span class="sxs-lookup"><span data-stu-id="47fb8-112">The client application then needs to call the [Create Report API](#create-report-api) using the QueryId along with the report start date, Repeat Interval, Recurrence, and an optional Callback URI.</span></span>
4. <span data-ttu-id="47fb8-113">Si se ejecuta correctamente, [Create Report API](#create-report-api) devuelve reportId.</span><span class="sxs-lookup"><span data-stu-id="47fb8-113">On Success, the [Create Report API](#create-report-api) returns the ReportId.</span></span>
5. <span data-ttu-id="47fb8-114">La aplicación cliente recibe una notificación en la dirección URL de devolución de llamada en cuanto los datos del informe están listos para su descarga.</span><span class="sxs-lookup"><span data-stu-id="47fb8-114">The client application gets notified at the callback URL as soon as the report data is ready for download.</span></span>
6. <span data-ttu-id="47fb8-115">A continuación, la aplicación cliente usa [get report executions API](#get-report-execution-api) para consultar el estado del informe con el identificador de informe y el intervalo de fechas.</span><span class="sxs-lookup"><span data-stu-id="47fb8-115">The client application then uses the [Get Report Executions API](#get-report-execution-api) to query the status of the report with the Report ID and date range.</span></span>
7. <span data-ttu-id="47fb8-116">Si se ejecuta correctamente, se devuelve el vínculo de descarga del informe y la aplicación puede iniciar la descarga de los datos.</span><span class="sxs-lookup"><span data-stu-id="47fb8-116">On success, the report download link is returned and the application can initiate download of the data.</span></span>

## <a name="report-query-language-specification"></a><span data-ttu-id="47fb8-117">Especificación del lenguaje de consulta de informes</span><span class="sxs-lookup"><span data-stu-id="47fb8-117">Report query language specification</span></span>

<span data-ttu-id="47fb8-118">Aunque proporcionamos [consultas del sistema](insights-programmatic-system-queries.md) que puede usar para crear informes, también puede crear sus propias consultas en función de sus necesidades empresariales.</span><span class="sxs-lookup"><span data-stu-id="47fb8-118">While we do provide [system queries](insights-programmatic-system-queries.md) you can use to create reports, you can also create your own queries based on your business needs.</span></span> <span data-ttu-id="47fb8-119">Para más información sobre las consultas personalizadas, consulte [Especificación de consultas personalizadas.](insights-programmatic-custom-query.md)</span><span class="sxs-lookup"><span data-stu-id="47fb8-119">To learn more about custom queries, see [Custom Query Specification](insights-programmatic-custom-query.md).</span></span>

## <a name="create-report-query-api"></a><span data-ttu-id="47fb8-120">API de creación de consultas de informes</span><span class="sxs-lookup"><span data-stu-id="47fb8-120">Create report query API</span></span>

<span data-ttu-id="47fb8-121">La API ayuda a crear consultas personalizadas que definen el conjunto de datos desde el que se deben exportar las columnas y las métricas.</span><span class="sxs-lookup"><span data-stu-id="47fb8-121">The API helps to create custom queries that define the dataset from which columns and metrics need to be exported.</span></span> <span data-ttu-id="47fb8-122">La API proporciona la flexibilidad para crear una nueva plantilla de informes en función de sus necesidades empresariales.</span><span class="sxs-lookup"><span data-stu-id="47fb8-122">The API provides the flexibility to create a new reporting template based on your business needs.</span></span>  

<span data-ttu-id="47fb8-123">También puede usar las [consultas del sistema](insights-programmatic-system-queries.md) que proporcionamos.</span><span class="sxs-lookup"><span data-stu-id="47fb8-123">You can also use the [system queries](insights-programmatic-system-queries.md) we provide.</span></span> <span data-ttu-id="47fb8-124">Cuando no se necesitan plantillas de informe personalizadas, puede llamar a [Create Report API](#create-report-api) directamente mediante los QueryId de las consultas del sistema que se proporcionan.</span><span class="sxs-lookup"><span data-stu-id="47fb8-124">When custom report templates are not needed, you can call [Create Report API](#create-report-api) directly using the QueryIds of the system queries that are provided.</span></span>  

<span data-ttu-id="47fb8-125">En el ejemplo siguiente se muestra cómo crear una consulta personalizada para obtener los 10 clientes principales por ingresos del mes pasado.</span><span class="sxs-lookup"><span data-stu-id="47fb8-125">The following example shows how to create a custom query to get top 10 customers by revenue for last month.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="47fb8-126">Sintaxis de la solicitud</span><span class="sxs-lookup"><span data-stu-id="47fb8-126">Request syntax</span></span>

|    <span data-ttu-id="47fb8-127">Método</span><span class="sxs-lookup"><span data-stu-id="47fb8-127">Method</span></span>     |    <span data-ttu-id="47fb8-128">URI de solicitud</span><span class="sxs-lookup"><span data-stu-id="47fb8-128">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="47fb8-129">POST</span><span class="sxs-lookup"><span data-stu-id="47fb8-129">POST</span></span>     |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries`|
|||

### <a name="request-header"></a><span data-ttu-id="47fb8-130">Encabezado de solicitud</span><span class="sxs-lookup"><span data-stu-id="47fb8-130">Request header</span></span>

|    <span data-ttu-id="47fb8-131">Encabezado</span><span class="sxs-lookup"><span data-stu-id="47fb8-131">Header</span></span>     |    <span data-ttu-id="47fb8-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="47fb8-132">Type</span></span>     |    <span data-ttu-id="47fb8-133">Descripción</span><span class="sxs-lookup"><span data-stu-id="47fb8-133">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="47fb8-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="47fb8-134">Authorization</span></span>     |    <span data-ttu-id="47fb8-135">string</span><span class="sxs-lookup"><span data-stu-id="47fb8-135">string</span></span> |<span data-ttu-id="47fb8-136">Necesario.</span><span class="sxs-lookup"><span data-stu-id="47fb8-136">Required.</span></span> <span data-ttu-id="47fb8-137">El token de acceso de Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="47fb8-137">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="47fb8-138">El formato es  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="47fb8-138">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="47fb8-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47fb8-139">Content-Type</span></span>     |<span data-ttu-id="47fb8-140">string</span><span class="sxs-lookup"><span data-stu-id="47fb8-140">string</span></span> |`Application/JSON` |
||||

### <a name="path-parameter"></a><span data-ttu-id="47fb8-141">Parámetro Path</span><span class="sxs-lookup"><span data-stu-id="47fb8-141">Path parameter</span></span>

<span data-ttu-id="47fb8-142">Ninguno</span><span class="sxs-lookup"><span data-stu-id="47fb8-142">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="47fb8-143">Parámetro de consulta</span><span class="sxs-lookup"><span data-stu-id="47fb8-143">Query parameter</span></span>

<span data-ttu-id="47fb8-144">Ninguno</span><span class="sxs-lookup"><span data-stu-id="47fb8-144">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="47fb8-145">Carga de solicitud de ejemplo</span><span class="sxs-lookup"><span data-stu-id="47fb8-145">Sample request payload</span></span>

```json
{ 
  "Name": "CustomersRevenueQuery", 
  "Description": "Query to get top 10 customers by revenue for last month", 
  "Query": "SELECT CustomerName, Product, BilledRevenueUSD FROM CustomersAndTenants ORDER BY BilledRevenueUSD LIMIT 10 TIMESPAN LAST_MONTH" 
}
```

### <a name="glossary"></a><span data-ttu-id="47fb8-146">Glosario</span><span class="sxs-lookup"><span data-stu-id="47fb8-146">Glossary</span></span>

<span data-ttu-id="47fb8-147">En esta tabla se proporcionan las definiciones clave de los elementos de la carga de solicitud.</span><span class="sxs-lookup"><span data-stu-id="47fb8-147">This table provides the key definitions of elements in the request payload.</span></span>

|<span data-ttu-id="47fb8-148">Parámetro</span><span class="sxs-lookup"><span data-stu-id="47fb8-148">Parameter</span></span>|    <span data-ttu-id="47fb8-149">Obligatorio</span><span class="sxs-lookup"><span data-stu-id="47fb8-149">Required</span></span>     |    <span data-ttu-id="47fb8-150">Descripción</span><span class="sxs-lookup"><span data-stu-id="47fb8-150">Description</span></span>     |    <span data-ttu-id="47fb8-151">Valores permitidos</span><span class="sxs-lookup"><span data-stu-id="47fb8-151">Allowed Values</span></span>     |
|-----|    -----    |    -----    |    -----    |
|<span data-ttu-id="47fb8-152">Nombre</span><span class="sxs-lookup"><span data-stu-id="47fb8-152">Name</span></span> |    <span data-ttu-id="47fb8-153">Sí</span><span class="sxs-lookup"><span data-stu-id="47fb8-153">Yes</span></span>     |    <span data-ttu-id="47fb8-154">Nombre descriptivo de la consulta</span><span class="sxs-lookup"><span data-stu-id="47fb8-154">Friendly name of the query</span></span>     |    <span data-ttu-id="47fb8-155">string</span><span class="sxs-lookup"><span data-stu-id="47fb8-155">string</span></span>     |
|    <span data-ttu-id="47fb8-156">Descripción</span><span class="sxs-lookup"><span data-stu-id="47fb8-156">Description</span></span>     |    <span data-ttu-id="47fb8-157">No</span><span class="sxs-lookup"><span data-stu-id="47fb8-157">No</span></span>     |    <span data-ttu-id="47fb8-158">Descripción de lo que devuelve la consulta</span><span class="sxs-lookup"><span data-stu-id="47fb8-158">Description of what the query returns</span></span>     |    <span data-ttu-id="47fb8-159">string</span><span class="sxs-lookup"><span data-stu-id="47fb8-159">string</span></span>     |
|    <span data-ttu-id="47fb8-160">Consultar</span><span class="sxs-lookup"><span data-stu-id="47fb8-160">Query</span></span>     |    <span data-ttu-id="47fb8-161">Sí</span><span class="sxs-lookup"><span data-stu-id="47fb8-161">Yes</span></span>     |    <span data-ttu-id="47fb8-162">Cadena de consulta del informe.</span><span class="sxs-lookup"><span data-stu-id="47fb8-162">Report query string</span></span>     |    <span data-ttu-id="47fb8-163">Tipo de datos: cadena</span><span class="sxs-lookup"><span data-stu-id="47fb8-163">Data type: string</span></span> <br> <span data-ttu-id="47fb8-164">[Consulta personalizada](insights-programmatic-custom-query.md) basada en la necesidad empresarial</span><span class="sxs-lookup"><span data-stu-id="47fb8-164">[Custom query](insights-programmatic-custom-query.md) based on business need</span></span> |
|        |        |        |        |

> [!Note]
> <span data-ttu-id="47fb8-165">Para obtener ejemplos de consultas personalizadas, [consulte Ejemplos de consultas de ejemplo.](insights-programmatic-sample-queries.md)</span><span class="sxs-lookup"><span data-stu-id="47fb8-165">For custom query samples, see [Examples of sample queries.](insights-programmatic-sample-queries.md)</span></span>

### <a name="sample-response"></a><span data-ttu-id="47fb8-166">Respuesta de muestra</span><span class="sxs-lookup"><span data-stu-id="47fb8-166">Sample response</span></span>

<span data-ttu-id="47fb8-167">La carga de respuesta tiene la estructura siguiente:</span><span class="sxs-lookup"><span data-stu-id="47fb8-167">The response payload is structured as follows:</span></span>

<span data-ttu-id="47fb8-168">Códigos de respuesta: 200, 400, 401, 403, 500</span><span class="sxs-lookup"><span data-stu-id="47fb8-168">Response Codes: 200, 400, 401, 403, 500</span></span>

<span data-ttu-id="47fb8-169">Ejemplo de carga de respuesta:</span><span class="sxs-lookup"><span data-stu-id="47fb8-169">Response payload example:</span></span>

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

### <a name="glossary"></a><span data-ttu-id="47fb8-170">Glosario</span><span class="sxs-lookup"><span data-stu-id="47fb8-170">Glossary</span></span>

<span data-ttu-id="47fb8-171">En esta tabla se proporcionan las definiciones clave de los elementos de la carga de solicitud.</span><span class="sxs-lookup"><span data-stu-id="47fb8-171">This table provides the key definitions of elements in the request payload.</span></span>

|    <span data-ttu-id="47fb8-172">Parámetro</span><span class="sxs-lookup"><span data-stu-id="47fb8-172">Parameter</span></span>     |    <span data-ttu-id="47fb8-173">Descripción</span><span class="sxs-lookup"><span data-stu-id="47fb8-173">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="47fb8-174">QueryId</span><span class="sxs-lookup"><span data-stu-id="47fb8-174">QueryId</span></span>     |    <span data-ttu-id="47fb8-175">Identificador único universal (UUID) de la consulta que creó</span><span class="sxs-lookup"><span data-stu-id="47fb8-175">Universally unique identifier (UUID) of the query you created</span></span>     |
|    <span data-ttu-id="47fb8-176">Nombre</span><span class="sxs-lookup"><span data-stu-id="47fb8-176">Name</span></span>     |    <span data-ttu-id="47fb8-177">Nombre descriptivo dado a la consulta en la carga de la solicitud</span><span class="sxs-lookup"><span data-stu-id="47fb8-177">Friendly name given to the query in the request payload</span></span>     |
|    <span data-ttu-id="47fb8-178">Descripción</span><span class="sxs-lookup"><span data-stu-id="47fb8-178">Description</span></span>     |    <span data-ttu-id="47fb8-179">Descripción proporcionada durante la creación de la consulta.</span><span class="sxs-lookup"><span data-stu-id="47fb8-179">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="47fb8-180">Consultar</span><span class="sxs-lookup"><span data-stu-id="47fb8-180">Query</span></span>     |    <span data-ttu-id="47fb8-181">Consulta de informe pasada como entrada durante la creación de la consulta</span><span class="sxs-lookup"><span data-stu-id="47fb8-181">Report query passed as input during query creation</span></span>     |
|    <span data-ttu-id="47fb8-182">Tipo</span><span class="sxs-lookup"><span data-stu-id="47fb8-182">Type</span></span>     |    <span data-ttu-id="47fb8-183">Establézcala en `userDefined`</span><span class="sxs-lookup"><span data-stu-id="47fb8-183">Set to `userDefined`</span></span>     |
|    <span data-ttu-id="47fb8-184">Usuario</span><span class="sxs-lookup"><span data-stu-id="47fb8-184">User</span></span>     |    <span data-ttu-id="47fb8-185">Identificador de usuario usado para crear la consulta</span><span class="sxs-lookup"><span data-stu-id="47fb8-185">User ID used to create of the query</span></span>     |
|    <span data-ttu-id="47fb8-186">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="47fb8-186">CreatedTime</span></span>     |    <span data-ttu-id="47fb8-187">Hora UTC en que se creó la consulta en el formato aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="47fb8-187">UTC Time the query was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="47fb8-188">TotalCount</span><span class="sxs-lookup"><span data-stu-id="47fb8-188">TotalCount</span></span>     |    <span data-ttu-id="47fb8-189">Número de conjuntos de datos en la matriz de valores.</span><span class="sxs-lookup"><span data-stu-id="47fb8-189">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="47fb8-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="47fb8-190">StatusCode</span></span>     |    <span data-ttu-id="47fb8-191">Código de resultado</span><span class="sxs-lookup"><span data-stu-id="47fb8-191">Result Code</span></span> <br> <span data-ttu-id="47fb8-192">Los valores posibles son 200, 400, 401, 403 y 500.</span><span class="sxs-lookup"><span data-stu-id="47fb8-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|    <span data-ttu-id="47fb8-193">message</span><span class="sxs-lookup"><span data-stu-id="47fb8-193">message</span></span>     |    <span data-ttu-id="47fb8-194">Mensaje de estado de la ejecución de la API.</span><span class="sxs-lookup"><span data-stu-id="47fb8-194">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="create-report-api"></a><span data-ttu-id="47fb8-195">API de creación de informes</span><span class="sxs-lookup"><span data-stu-id="47fb8-195">Create report API</span></span>

<span data-ttu-id="47fb8-196">Al crear correctamente una plantilla de informe personalizada [](#create-report-query-api) y recibir el QueryID como parte de la respuesta Crear consulta de informe, se puede llamar a esta API para programar una consulta que se ejecutará a intervalos regulares.</span><span class="sxs-lookup"><span data-stu-id="47fb8-196">On creating a custom report template successfully and receiving the QueryID as part of [Create Report Query](#create-report-query-api) response, this API can be called to schedule a query to be executed at regular intervals.</span></span> <span data-ttu-id="47fb8-197">Puede establecer una frecuencia y una programación para la entrega del informe.</span><span class="sxs-lookup"><span data-stu-id="47fb8-197">You can set a frequency and schedule for the report to be delivered.</span></span>
<span data-ttu-id="47fb8-198">En el caso de las consultas del sistema que proporcionamos, también se puede llamar a la API de creación de informes con [QueryId](insights-programmatic-system-queries.md).</span><span class="sxs-lookup"><span data-stu-id="47fb8-198">For system queries we provide, the Create Report API can also be called with [QueryId](insights-programmatic-system-queries.md).</span></span>

### <a name="callback-url"></a><span data-ttu-id="47fb8-199">Dirección URL de devolución de llamadas</span><span class="sxs-lookup"><span data-stu-id="47fb8-199">Callback URL</span></span>

<span data-ttu-id="47fb8-200">La API de creación de informes acepta una dirección URL de devolución de llamada.</span><span class="sxs-lookup"><span data-stu-id="47fb8-200">The create report API accepts a callback URL.</span></span> <span data-ttu-id="47fb8-201">Se llamará a esta dirección URL una vez que la generación del informe sea correcta.</span><span class="sxs-lookup"><span data-stu-id="47fb8-201">This URL will be called once the report generation is successful.</span></span> <span data-ttu-id="47fb8-202">La dirección URL de devolución de llamada debe ser accesible públicamente.</span><span class="sxs-lookup"><span data-stu-id="47fb8-202">The callback URL should be publicly reachable.</span></span> <span data-ttu-id="47fb8-203">Además de la dirección URL, también se puede dar un método de devolución de llamada.</span><span class="sxs-lookup"><span data-stu-id="47fb8-203">In addition to the URL a callback method can also be given.</span></span> <span data-ttu-id="47fb8-204">El método de devolución de llamada solo puede ser "GET" o "POST".</span><span class="sxs-lookup"><span data-stu-id="47fb8-204">The callback method can only be "GET" or "POST".</span></span> <span data-ttu-id="47fb8-205">El método predeterminado si no se pasa ningún valor será "POST".</span><span class="sxs-lookup"><span data-stu-id="47fb8-205">The default method if no value is passed will be "POST".</span></span> <span data-ttu-id="47fb8-206">El reportId que ha completado la generación siempre se pasará de vuelta durante la devolución de llamada.</span><span class="sxs-lookup"><span data-stu-id="47fb8-206">The reportId that has completed generation will always be passed back during the callback.</span></span>

<span data-ttu-id="47fb8-207">Devolución de llamada POST: si la dirección URL pasada era , la dirección URL de devolución a la que se `https://www.contosso.com/callback` llamó será `https://www.contosso.com/callback/<reportID>`</span><span class="sxs-lookup"><span data-stu-id="47fb8-207">POST callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback/<reportID>`</span></span> 

<span data-ttu-id="47fb8-208">Devolución de llamada GET: si la dirección URL pasada era , la dirección URL de devolución a la `https://www.contosso.com/callback` que se llamó será `https://www.contosso.com/callback?reportId=<reportID>`</span><span class="sxs-lookup"><span data-stu-id="47fb8-208">GET callback: If the URL passed was `https://www.contosso.com/callback`, then the called back URL will be `https://www.contosso.com/callback?reportId=<reportID>`</span></span> 

### <a name="executenow-reports"></a><span data-ttu-id="47fb8-209">Informes de ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="47fb8-209">ExecuteNow reports</span></span>

<span data-ttu-id="47fb8-210">Hay un aprovisionamiento para generar un informe sin programación.</span><span class="sxs-lookup"><span data-stu-id="47fb8-210">There is a provision to generate a report without scheduling.</span></span> <span data-ttu-id="47fb8-211">La carga de la API de creación de informes puede aceptar un parámetro , que pondrá en cola el informe para que se genere en cuanto se llame `ExecuteNow` a la API.</span><span class="sxs-lookup"><span data-stu-id="47fb8-211">The report create API payload can accept a parameter `ExecuteNow`, which will enqueue the report to be generated as soon as the API is called.</span></span> <span data-ttu-id="47fb8-212">Cuando `ExecuteNow` se establece en true, se omiten los campos: , , ya que estos informes no están `StartTime` `RecurrenceCount` `RecurrenceInterval` programados.</span><span class="sxs-lookup"><span data-stu-id="47fb8-212">When `ExecuteNow` is set to true, the fields: `StartTime`, `RecurrenceCount`, `RecurrenceInterval` are ignored as these reports are not scheduled.</span></span>

<span data-ttu-id="47fb8-213">Se pueden pasar dos campos adicionales cuando `ExecuteNow` es true, `QueryStartTime` y `QueryEndTime` .</span><span class="sxs-lookup"><span data-stu-id="47fb8-213">Two additional fields can be passed when `ExecuteNow` is true, `QueryStartTime` and `QueryEndTime`.</span></span> <span data-ttu-id="47fb8-214">Estos dos campos invalidarán el `TIMESPAN` campo de la consulta.</span><span class="sxs-lookup"><span data-stu-id="47fb8-214">These two fields will override the `TIMESPAN` field in the query.</span></span> <span data-ttu-id="47fb8-215">Estos campos no son aplicables a los informes programados, ya que los datos se generarán continuamente durante un período de tiempo fijo que no cambia.</span><span class="sxs-lookup"><span data-stu-id="47fb8-215">These fields are not applicable for scheduled reports as data will get continuously generated for a fixed time period that does not change.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="47fb8-216">Sintaxis de la solicitud</span><span class="sxs-lookup"><span data-stu-id="47fb8-216">Request syntax</span></span>

|    <span data-ttu-id="47fb8-217">Método</span><span class="sxs-lookup"><span data-stu-id="47fb8-217">Method</span></span>     |    <span data-ttu-id="47fb8-218">URI de solicitud</span><span class="sxs-lookup"><span data-stu-id="47fb8-218">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="47fb8-219">POST</span><span class="sxs-lookup"><span data-stu-id="47fb8-219">POST</span></span>     |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport` |

### <a name="request-header"></a><span data-ttu-id="47fb8-220">Encabezado de solicitud</span><span class="sxs-lookup"><span data-stu-id="47fb8-220">Request header</span></span>

|    <span data-ttu-id="47fb8-221">Encabezado</span><span class="sxs-lookup"><span data-stu-id="47fb8-221">Header</span></span>     |    <span data-ttu-id="47fb8-222">Tipo</span><span class="sxs-lookup"><span data-stu-id="47fb8-222">Type</span></span>     |    <span data-ttu-id="47fb8-223">Descripción</span><span class="sxs-lookup"><span data-stu-id="47fb8-223">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="47fb8-224">Authorization</span><span class="sxs-lookup"><span data-stu-id="47fb8-224">Authorization</span></span>     |    <span data-ttu-id="47fb8-225">string</span><span class="sxs-lookup"><span data-stu-id="47fb8-225">string</span></span> |<span data-ttu-id="47fb8-226">Necesario.</span><span class="sxs-lookup"><span data-stu-id="47fb8-226">Required.</span></span> <span data-ttu-id="47fb8-227">El token de acceso de Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="47fb8-227">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="47fb8-228">El formato es  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="47fb8-228">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="47fb8-229">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47fb8-229">Content-Type</span></span>     |<span data-ttu-id="47fb8-230">string</span><span class="sxs-lookup"><span data-stu-id="47fb8-230">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="47fb8-231">Parámetro de ruta de acceso</span><span class="sxs-lookup"><span data-stu-id="47fb8-231">Path Parameter</span></span>

<span data-ttu-id="47fb8-232">Ninguno</span><span class="sxs-lookup"><span data-stu-id="47fb8-232">None</span></span>

### <a name="query-parameter"></a><span data-ttu-id="47fb8-233">Parámetro de consulta</span><span class="sxs-lookup"><span data-stu-id="47fb8-233">Query Parameter</span></span>

<span data-ttu-id="47fb8-234">Ninguno</span><span class="sxs-lookup"><span data-stu-id="47fb8-234">None</span></span>

### <a name="sample-request-payload"></a><span data-ttu-id="47fb8-235">Carga de solicitud de ejemplo</span><span class="sxs-lookup"><span data-stu-id="47fb8-235">Sample request payload</span></span>

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

### <a name="glossary"></a><span data-ttu-id="47fb8-236">Glosario</span><span class="sxs-lookup"><span data-stu-id="47fb8-236">Glossary</span></span>

<span data-ttu-id="47fb8-237">Las definiciones clave de los elementos de la carga de solicitud se articulan a continuación:</span><span class="sxs-lookup"><span data-stu-id="47fb8-237">Key definitions of elements in the request payload are articulated below:</span></span>

|    <span data-ttu-id="47fb8-238">Parámetro</span><span class="sxs-lookup"><span data-stu-id="47fb8-238">Parameter</span></span>     |    <span data-ttu-id="47fb8-239">Obligatorio</span><span class="sxs-lookup"><span data-stu-id="47fb8-239">Required</span></span>     |    <span data-ttu-id="47fb8-240">Descripción</span><span class="sxs-lookup"><span data-stu-id="47fb8-240">Description</span></span>     |    <span data-ttu-id="47fb8-241">Valores permitidos</span><span class="sxs-lookup"><span data-stu-id="47fb8-241">Allowed Values</span></span>     |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="47fb8-242">ReportName</span><span class="sxs-lookup"><span data-stu-id="47fb8-242">ReportName</span></span>     |    <span data-ttu-id="47fb8-243">Sí</span><span class="sxs-lookup"><span data-stu-id="47fb8-243">Yes</span></span>     |    <span data-ttu-id="47fb8-244">Nombre que se va a asignar al informe</span><span class="sxs-lookup"><span data-stu-id="47fb8-244">Name to be assigned to the report</span></span>     |    <span data-ttu-id="47fb8-245">string</span><span class="sxs-lookup"><span data-stu-id="47fb8-245">string</span></span>     |
|    <span data-ttu-id="47fb8-246">Descripción</span><span class="sxs-lookup"><span data-stu-id="47fb8-246">Description</span></span>     |    <span data-ttu-id="47fb8-247">No</span><span class="sxs-lookup"><span data-stu-id="47fb8-247">No</span></span>     |    <span data-ttu-id="47fb8-248">Descripción del informe creado</span><span class="sxs-lookup"><span data-stu-id="47fb8-248">Description of the created report</span></span>     |    <span data-ttu-id="47fb8-249">string</span><span class="sxs-lookup"><span data-stu-id="47fb8-249">string</span></span>     |
|    <span data-ttu-id="47fb8-250">QueryId</span><span class="sxs-lookup"><span data-stu-id="47fb8-250">QueryId</span></span>     |    <span data-ttu-id="47fb8-251">Sí</span><span class="sxs-lookup"><span data-stu-id="47fb8-251">Yes</span></span>     |    <span data-ttu-id="47fb8-252">Id. de consulta del informe.</span><span class="sxs-lookup"><span data-stu-id="47fb8-252">Report query ID</span></span>     |    <span data-ttu-id="47fb8-253">string</span><span class="sxs-lookup"><span data-stu-id="47fb8-253">string</span></span>     |
|    <span data-ttu-id="47fb8-254">StartTime</span><span class="sxs-lookup"><span data-stu-id="47fb8-254">StartTime</span></span>     |    <span data-ttu-id="47fb8-255">Sí</span><span class="sxs-lookup"><span data-stu-id="47fb8-255">Yes</span></span>     |    <span data-ttu-id="47fb8-256">Marca de tiempo UTC en la que comenzará la generación del informe.</span><span class="sxs-lookup"><span data-stu-id="47fb8-256">UTC Timestamp at which the report generation will begin.</span></span> <br> <span data-ttu-id="47fb8-257">El formato debe ser aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="47fb8-257">The format should be: yyyy-MM-ddTHH:mm:ssZ</span></span>       |    <span data-ttu-id="47fb8-258">string</span><span class="sxs-lookup"><span data-stu-id="47fb8-258">string</span></span>     |
|    <span data-ttu-id="47fb8-259">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="47fb8-259">ExecuteNow</span></span>     |    <span data-ttu-id="47fb8-260">No</span><span class="sxs-lookup"><span data-stu-id="47fb8-260">No</span></span>     |    <span data-ttu-id="47fb8-261">Este parámetro debe usarse para crear un informe que se ejecutará una sola vez.</span><span class="sxs-lookup"><span data-stu-id="47fb8-261">This parameter should be used to create a report that will be executed only once.</span></span> <span data-ttu-id="47fb8-262">`StartTime`, `RecurrenceInterval` y `RecurrenceCount` se omiten si se establece en true.</span><span class="sxs-lookup"><span data-stu-id="47fb8-262">`StartTime`, `RecurrenceInterval` and `RecurrenceCount` are ignored if this is set to true.</span></span> <span data-ttu-id="47fb8-263">El informe se ejecuta inmediatamente de forma asincrónica</span><span class="sxs-lookup"><span data-stu-id="47fb8-263">The report is executed immediately in an asynchronous fashion</span></span>     |    <span data-ttu-id="47fb8-264">true/false</span><span class="sxs-lookup"><span data-stu-id="47fb8-264">true/false</span></span>     |
|    <span data-ttu-id="47fb8-265">QueryStartTime</span><span class="sxs-lookup"><span data-stu-id="47fb8-265">QueryStartTime</span></span>     |    <span data-ttu-id="47fb8-266">No</span><span class="sxs-lookup"><span data-stu-id="47fb8-266">No</span></span>     |    <span data-ttu-id="47fb8-267">Opcionalmente, especifica la hora de inicio de la consulta que extrae los datos.</span><span class="sxs-lookup"><span data-stu-id="47fb8-267">Optionally specifies the start time for the query extracting the data.</span></span> <span data-ttu-id="47fb8-268">Este parámetro solo es aplicable para un informe de ejecución de una vez que `ExecuteNow` se ha establecido en true.</span><span class="sxs-lookup"><span data-stu-id="47fb8-268">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="47fb8-269">Al establecer este parámetro se invalida `TIMESPAN` el especificado en la consulta.</span><span class="sxs-lookup"><span data-stu-id="47fb8-269">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="47fb8-270">El formato debe ser aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="47fb8-270">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="47fb8-271">Marca de tiempo como string</span><span class="sxs-lookup"><span data-stu-id="47fb8-271">Timestamp as string</span></span>     |
|    <span data-ttu-id="47fb8-272">QueryEndTime</span><span class="sxs-lookup"><span data-stu-id="47fb8-272">QueryEndTime</span></span>     |    <span data-ttu-id="47fb8-273">No</span><span class="sxs-lookup"><span data-stu-id="47fb8-273">No</span></span>     |    <span data-ttu-id="47fb8-274">Opcionalmente, especifica la hora de fin de la consulta que extrae los datos.</span><span class="sxs-lookup"><span data-stu-id="47fb8-274">Optionally specifies the end time for the query extracting the data.</span></span> <span data-ttu-id="47fb8-275">Este parámetro solo es aplicable para un informe de ejecución de una vez que `ExecuteNow` se ha establecido en true.</span><span class="sxs-lookup"><span data-stu-id="47fb8-275">This parameter is applicable only for one time execution report that have `ExecuteNow` set to true.</span></span> <span data-ttu-id="47fb8-276">Al establecer este parámetro se invalida `TIMESPAN` el especificado en la consulta.</span><span class="sxs-lookup"><span data-stu-id="47fb8-276">Setting this parameter overrides `TIMESPAN` given in the query.</span></span> <span data-ttu-id="47fb8-277">El formato debe ser aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="47fb8-277">The format should be yyyy-MM-ddTHH:mm:ssZ</span></span>     |    <span data-ttu-id="47fb8-278">Marca de tiempo como string</span><span class="sxs-lookup"><span data-stu-id="47fb8-278">Timestamp as string</span></span>     |
|    <span data-ttu-id="47fb8-279">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="47fb8-279">RecurrenceInterval</span></span>     |    <span data-ttu-id="47fb8-280">Sí</span><span class="sxs-lookup"><span data-stu-id="47fb8-280">Yes</span></span>     |    <span data-ttu-id="47fb8-281">Frecuencia en horas en que se debe generar el informe.</span><span class="sxs-lookup"><span data-stu-id="47fb8-281">Frequency in hours at which the report should be generated.</span></span> <br> <span data-ttu-id="47fb8-282">El valor mínimo es 4 y el valor máximo es 2160.</span><span class="sxs-lookup"><span data-stu-id="47fb8-282">Minimum value is 4 and Maximum value is 2160.</span></span>      |    <span data-ttu-id="47fb8-283">integer</span><span class="sxs-lookup"><span data-stu-id="47fb8-283">integer</span></span>     |
|    <span data-ttu-id="47fb8-284">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="47fb8-284">RecurrenceCount</span></span>     |    <span data-ttu-id="47fb8-285">No</span><span class="sxs-lookup"><span data-stu-id="47fb8-285">No</span></span>     |    <span data-ttu-id="47fb8-286">Número de informes que se van a generar.</span><span class="sxs-lookup"><span data-stu-id="47fb8-286">Number of reports to be generated.</span></span>     |    <span data-ttu-id="47fb8-287">integer</span><span class="sxs-lookup"><span data-stu-id="47fb8-287">integer</span></span>     |
|    <span data-ttu-id="47fb8-288">Formato</span><span class="sxs-lookup"><span data-stu-id="47fb8-288">Format</span></span>     |    <span data-ttu-id="47fb8-289">No</span><span class="sxs-lookup"><span data-stu-id="47fb8-289">No</span></span>     |    <span data-ttu-id="47fb8-290">Formato del archivo exportado.</span><span class="sxs-lookup"><span data-stu-id="47fb8-290">File format of the exported file.</span></span> <br> <span data-ttu-id="47fb8-291">El valor predeterminado es CSV.</span><span class="sxs-lookup"><span data-stu-id="47fb8-291">Default is CSV.</span></span>    |    <span data-ttu-id="47fb8-292">"CSV"/"TSV"</span><span class="sxs-lookup"><span data-stu-id="47fb8-292">"CSV"/"TSV"</span></span>     |
|    <span data-ttu-id="47fb8-293">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="47fb8-293">CallbackUrl</span></span>     |    <span data-ttu-id="47fb8-294">No</span><span class="sxs-lookup"><span data-stu-id="47fb8-294">No</span></span>     |    <span data-ttu-id="47fb8-295">Dirección URL accesible públicamente que se puede configurar opcionalmente como destino de devolución de llamada</span><span class="sxs-lookup"><span data-stu-id="47fb8-295">Publicly reachable URL that can be optionally configured as callback destination</span></span>     |    <span data-ttu-id="47fb8-296">Cadena (dirección URL http)</span><span class="sxs-lookup"><span data-stu-id="47fb8-296">String (http URL)</span></span>     |
|    <span data-ttu-id="47fb8-297">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="47fb8-297">CallbackMethod</span></span>     |    <span data-ttu-id="47fb8-298">No</span><span class="sxs-lookup"><span data-stu-id="47fb8-298">No</span></span>     |    <span data-ttu-id="47fb8-299">Método que se va a usar para la devolución de llamada</span><span class="sxs-lookup"><span data-stu-id="47fb8-299">The method to be used for callback</span></span>     |    <span data-ttu-id="47fb8-300">GET/POST</span><span class="sxs-lookup"><span data-stu-id="47fb8-300">GET/POST</span></span>     |
|        |        |        |        |

### <a name="sample-response"></a><span data-ttu-id="47fb8-301">Respuesta de muestra</span><span class="sxs-lookup"><span data-stu-id="47fb8-301">Sample response</span></span>

<span data-ttu-id="47fb8-302">La carga de respuesta tiene la estructura siguiente:</span><span class="sxs-lookup"><span data-stu-id="47fb8-302">The response payload is structured as follows:</span></span>

<span data-ttu-id="47fb8-303">Códigos de respuesta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="47fb8-303">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="47fb8-304">Ejemplo de carga de respuesta:</span><span class="sxs-lookup"><span data-stu-id="47fb8-304">Response payload example:</span></span>

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

### <a name="glossary"></a><span data-ttu-id="47fb8-305">Glosario</span><span class="sxs-lookup"><span data-stu-id="47fb8-305">Glossary</span></span>

<span data-ttu-id="47fb8-306">Las definiciones clave de los elementos de la respuesta se articulan a continuación:</span><span class="sxs-lookup"><span data-stu-id="47fb8-306">Key definitions of elements in the response are articulated below:</span></span>

|    <span data-ttu-id="47fb8-307">Parámetro</span><span class="sxs-lookup"><span data-stu-id="47fb8-307">Parameter</span></span>     |    <span data-ttu-id="47fb8-308">Descripción</span><span class="sxs-lookup"><span data-stu-id="47fb8-308">Description</span></span>     |
|    ----    |    ----    |
|    <span data-ttu-id="47fb8-309">ReportId</span><span class="sxs-lookup"><span data-stu-id="47fb8-309">ReportId</span></span>     |    <span data-ttu-id="47fb8-310">Identificador único universal (UUID) del informe que creó.</span><span class="sxs-lookup"><span data-stu-id="47fb8-310">Universally unique identifier (UUID) of the report you created</span></span>     |
|    <span data-ttu-id="47fb8-311">ReportName</span><span class="sxs-lookup"><span data-stu-id="47fb8-311">ReportName</span></span>     |    <span data-ttu-id="47fb8-312">Nombre dado al informe en la carga útil de solicitud</span><span class="sxs-lookup"><span data-stu-id="47fb8-312">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="47fb8-313">Descripción</span><span class="sxs-lookup"><span data-stu-id="47fb8-313">Description</span></span>     |    <span data-ttu-id="47fb8-314">Descripción proporcionada durante la creación del informe.</span><span class="sxs-lookup"><span data-stu-id="47fb8-314">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="47fb8-315">QueryId</span><span class="sxs-lookup"><span data-stu-id="47fb8-315">QueryId</span></span>     |    <span data-ttu-id="47fb8-316">Id. de consulta pasado en el momento en que creó el informe.</span><span class="sxs-lookup"><span data-stu-id="47fb8-316">Query ID passed at the time you created the report</span></span>     |
|    <span data-ttu-id="47fb8-317">Consultar</span><span class="sxs-lookup"><span data-stu-id="47fb8-317">Query</span></span>     |    <span data-ttu-id="47fb8-318">Texto de la consulta que se ejecutará para este informe.</span><span class="sxs-lookup"><span data-stu-id="47fb8-318">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="47fb8-319">Usuario</span><span class="sxs-lookup"><span data-stu-id="47fb8-319">User</span></span>     |    <span data-ttu-id="47fb8-320">Identificador de usuario usado para crear el informe</span><span class="sxs-lookup"><span data-stu-id="47fb8-320">User ID used to create the report</span></span>     |
|    <span data-ttu-id="47fb8-321">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="47fb8-321">CreatedTime</span></span>     |    <span data-ttu-id="47fb8-322">Hora UTC en que se creó el informe en el formato aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="47fb8-322">UTC Time the report was created in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="47fb8-323">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="47fb8-323">ModifiedTime</span></span>     |    <span data-ttu-id="47fb8-324">Hora UTC en que se modificó el informe en el formato aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="47fb8-324">UTC Time the report was last modified in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="47fb8-325">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="47fb8-325">ExecuteNow</span></span>     |    <span data-ttu-id="47fb8-326">`ExecuteNow` marca establecida en el momento en que se creó el informe</span><span class="sxs-lookup"><span data-stu-id="47fb8-326">`ExecuteNow` flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="47fb8-327">StartTime</span><span class="sxs-lookup"><span data-stu-id="47fb8-327">StartTime</span></span>     |    <span data-ttu-id="47fb8-328">Hora UTC en que se iniciará la ejecución del informe en el formato aaaa-MM-ddTHH:mm:ssZ</span><span class="sxs-lookup"><span data-stu-id="47fb8-328">UTC Time the report execution will begin in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="47fb8-329">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="47fb8-329">ReportStatus</span></span>     |    <span data-ttu-id="47fb8-330">Estado de la ejecución del informe.</span><span class="sxs-lookup"><span data-stu-id="47fb8-330">Status of the report execution.</span></span> <span data-ttu-id="47fb8-331">Los valores posibles `Paused` son `Active` , y `Inactive`</span><span class="sxs-lookup"><span data-stu-id="47fb8-331">The possible values are `Paused`, `Active`, and `Inactive`</span></span>     |
|    <span data-ttu-id="47fb8-332">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="47fb8-332">RecurrenceInterval</span></span>     |    <span data-ttu-id="47fb8-333">Intervalo de periodicidad proporcionado durante la creación del informe.</span><span class="sxs-lookup"><span data-stu-id="47fb8-333">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="47fb8-334">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="47fb8-334">RecurrenceCount</span></span>     |    <span data-ttu-id="47fb8-335">Recuento de periodicidad proporcionado durante la creación del informe.</span><span class="sxs-lookup"><span data-stu-id="47fb8-335">Recurrence count provided during report creation.</span></span>      |
|    <span data-ttu-id="47fb8-336">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="47fb8-336">CallbackUrl</span></span>     |    <span data-ttu-id="47fb8-337">Dirección URL de devolución de llamada proporcionada en la solicitud.</span><span class="sxs-lookup"><span data-stu-id="47fb8-337">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="47fb8-338">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="47fb8-338">CallbackMethod</span></span>     |    <span data-ttu-id="47fb8-339">Método de devolución de llamada proporcionado en la solicitud</span><span class="sxs-lookup"><span data-stu-id="47fb8-339">Callback method provided in the request</span></span>     |
|    <span data-ttu-id="47fb8-340">Formato</span><span class="sxs-lookup"><span data-stu-id="47fb8-340">Format</span></span>     |    <span data-ttu-id="47fb8-341">Formato de los archivos de informe.</span><span class="sxs-lookup"><span data-stu-id="47fb8-341">Format of the report files.</span></span> <span data-ttu-id="47fb8-342">Los valores posibles son `CSV` o `TSV` .</span><span class="sxs-lookup"><span data-stu-id="47fb8-342">The possible values are `CSV` or `TSV`.</span></span>     |
|    <span data-ttu-id="47fb8-343">TotalCount</span><span class="sxs-lookup"><span data-stu-id="47fb8-343">TotalCount</span></span>     |    <span data-ttu-id="47fb8-344">Número de registros de la matriz Value</span><span class="sxs-lookup"><span data-stu-id="47fb8-344">Number of records in the Value array</span></span>     |
|    <span data-ttu-id="47fb8-345">StatusCode</span><span class="sxs-lookup"><span data-stu-id="47fb8-345">StatusCode</span></span>     |    <span data-ttu-id="47fb8-346">Código de resultado</span><span class="sxs-lookup"><span data-stu-id="47fb8-346">Result Code</span></span>     |
|    <span data-ttu-id="47fb8-347">message</span><span class="sxs-lookup"><span data-stu-id="47fb8-347">message</span></span>     |    <span data-ttu-id="47fb8-348">Los valores posibles son 200, 400, 401, 403, 500.</span><span class="sxs-lookup"><span data-stu-id="47fb8-348">The possible values are 200, 400, 401, 403, 500.</span></span> <span data-ttu-id="47fb8-349">Mensaje de estado de la ejecución de la API.</span><span class="sxs-lookup"><span data-stu-id="47fb8-349">Status message from the execution of the API</span></span>     |
|        |        |

## <a name="get-report-execution-api"></a><span data-ttu-id="47fb8-350">Obtener la API de ejecución de informes</span><span class="sxs-lookup"><span data-stu-id="47fb8-350">Get report execution API</span></span>

<span data-ttu-id="47fb8-351">Puede usar este método para consultar el estado de una ejecución de informe mediante el ReportId recibido de [Create Report API.](#create-report-api)</span><span class="sxs-lookup"><span data-stu-id="47fb8-351">You can use this method to query the status of a report execution using the ReportId received from [Create Report API](#create-report-api).</span></span> <span data-ttu-id="47fb8-352">El método devuelve el vínculo de descarga del informe si el informe está listo para su descarga.</span><span class="sxs-lookup"><span data-stu-id="47fb8-352">The method returns the report download link if the report is ready for download.</span></span> <span data-ttu-id="47fb8-353">De lo contrario, el método devolverá el estado.</span><span class="sxs-lookup"><span data-stu-id="47fb8-353">Otherwise, the method returns the status.</span></span> <span data-ttu-id="47fb8-354">También puede usar esta API para obtener todas las ejecuciones que se han producido para un informe determinado.</span><span class="sxs-lookup"><span data-stu-id="47fb8-354">You can also use this API to get all the executions that have happened for a given report.</span></span>  

>[!IMPORTANT]
><span data-ttu-id="47fb8-355">Esta API tiene parámetros de consulta predeterminados establecidos para `executionStatus=Completed` y `getLatestExecution=true` .</span><span class="sxs-lookup"><span data-stu-id="47fb8-355">This API has default query parameters set for `executionStatus=Completed` and `getLatestExecution=true`.</span></span> <span data-ttu-id="47fb8-356">Por lo tanto, si se llama a la API antes de la primera ejecución correcta del informe devolverá 404.</span><span class="sxs-lookup"><span data-stu-id="47fb8-356">Hence, calling the API before the first successful execution of the report will return 404.</span></span> <span data-ttu-id="47fb8-357">Las ejecuciones pendientes se pueden obtener estableciendo `executionStatus=Pending`.</span><span class="sxs-lookup"><span data-stu-id="47fb8-357">Pending executions can be obtained by setting `executionStatus=Pending`.</span></span>

### <a name="request-syntax"></a><span data-ttu-id="47fb8-358">Sintaxis de la solicitud</span><span class="sxs-lookup"><span data-stu-id="47fb8-358">Request syntax</span></span>

|    <span data-ttu-id="47fb8-359">Método</span><span class="sxs-lookup"><span data-stu-id="47fb8-359">Method</span></span>     |    <span data-ttu-id="47fb8-360">URI de solicitud</span><span class="sxs-lookup"><span data-stu-id="47fb8-360">Request URI</span></span>     |
|----- | -----|
|    <span data-ttu-id="47fb8-361">GET</span><span class="sxs-lookup"><span data-stu-id="47fb8-361">GET</span></span>    |`https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/execution/{reportId}?executionId={executionId}&executionStatus={executionStatus}&getLatestExecution={getLatestExecution}`  |

### <a name="request-header"></a><span data-ttu-id="47fb8-362">Encabezado de solicitud</span><span class="sxs-lookup"><span data-stu-id="47fb8-362">Request header</span></span>

|    <span data-ttu-id="47fb8-363">Encabezado</span><span class="sxs-lookup"><span data-stu-id="47fb8-363">Header</span></span>     |    <span data-ttu-id="47fb8-364">Tipo</span><span class="sxs-lookup"><span data-stu-id="47fb8-364">Type</span></span>     |    <span data-ttu-id="47fb8-365">Descripción</span><span class="sxs-lookup"><span data-stu-id="47fb8-365">Description</span></span>     |
|-------|-----|------|
|    <span data-ttu-id="47fb8-366">Authorization</span><span class="sxs-lookup"><span data-stu-id="47fb8-366">Authorization</span></span>     |    <span data-ttu-id="47fb8-367">string</span><span class="sxs-lookup"><span data-stu-id="47fb8-367">string</span></span> |<span data-ttu-id="47fb8-368">Necesario.</span><span class="sxs-lookup"><span data-stu-id="47fb8-368">Required.</span></span> <span data-ttu-id="47fb8-369">El token de acceso de Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="47fb8-369">The Azure Active Directory (Azure AD) access token.</span></span> <span data-ttu-id="47fb8-370">El formato es  `Bearer <token>` .</span><span class="sxs-lookup"><span data-stu-id="47fb8-370">The format is `Bearer <token>`.</span></span>|
|    <span data-ttu-id="47fb8-371">Content-Type</span><span class="sxs-lookup"><span data-stu-id="47fb8-371">Content-Type</span></span>     |<span data-ttu-id="47fb8-372">string</span><span class="sxs-lookup"><span data-stu-id="47fb8-372">string</span></span> |`Application/JSON` |

### <a name="path-parameter"></a><span data-ttu-id="47fb8-373">Parámetro Path</span><span class="sxs-lookup"><span data-stu-id="47fb8-373">Path parameter</span></span>

|    <span data-ttu-id="47fb8-374">Nombre de parámetro</span><span class="sxs-lookup"><span data-stu-id="47fb8-374">Parameter Name</span></span>    |    <span data-ttu-id="47fb8-375">Obligatorio</span><span class="sxs-lookup"><span data-stu-id="47fb8-375">Required</span></span>    |    <span data-ttu-id="47fb8-376">Tipo</span><span class="sxs-lookup"><span data-stu-id="47fb8-376">Type</span></span>    |    <span data-ttu-id="47fb8-377">Descripción</span><span class="sxs-lookup"><span data-stu-id="47fb8-377">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="47fb8-378">reportId</span><span class="sxs-lookup"><span data-stu-id="47fb8-378">reportId</span></span>    |    <span data-ttu-id="47fb8-379">Sí</span><span class="sxs-lookup"><span data-stu-id="47fb8-379">Yes</span></span>    |    <span data-ttu-id="47fb8-380">string</span><span class="sxs-lookup"><span data-stu-id="47fb8-380">string</span></span>    |    <span data-ttu-id="47fb8-381">Filtre para obtener los detalles de ejecución de solo los informes con el valor de reportId especificado en este argumento.</span><span class="sxs-lookup"><span data-stu-id="47fb8-381">Filter to get execution details of only reports with the reportId given in this argument.</span></span> <span data-ttu-id="47fb8-382">Se pueden especificar varios reportIds si se separan con un punto y coma ";".</span><span class="sxs-lookup"><span data-stu-id="47fb8-382">Multiple reportIds can be specified by separating them with a semicolon ";".</span></span>    |
|        |        |        |        |

### <a name="query-parameter"></a><span data-ttu-id="47fb8-383">Parámetro de consulta</span><span class="sxs-lookup"><span data-stu-id="47fb8-383">Query parameter</span></span>

|    <span data-ttu-id="47fb8-384">Nombre de parámetro</span><span class="sxs-lookup"><span data-stu-id="47fb8-384">Parameter Name</span></span>    |    <span data-ttu-id="47fb8-385">Obligatorio</span><span class="sxs-lookup"><span data-stu-id="47fb8-385">Required</span></span>    |    <span data-ttu-id="47fb8-386">Tipo</span><span class="sxs-lookup"><span data-stu-id="47fb8-386">Type</span></span>    |    <span data-ttu-id="47fb8-387">Descripción</span><span class="sxs-lookup"><span data-stu-id="47fb8-387">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="47fb8-388">executionId</span><span class="sxs-lookup"><span data-stu-id="47fb8-388">executionId</span></span>    |    <span data-ttu-id="47fb8-389">No</span><span class="sxs-lookup"><span data-stu-id="47fb8-389">No</span></span>    |    <span data-ttu-id="47fb8-390">string</span><span class="sxs-lookup"><span data-stu-id="47fb8-390">string</span></span>    |    <span data-ttu-id="47fb8-391">Filtre para obtener detalles de solo los informes con el executionId especificado en este argumento.</span><span class="sxs-lookup"><span data-stu-id="47fb8-391">Filter to get details of only reports with the executionId given in this argument.</span></span> <span data-ttu-id="47fb8-392">Se pueden especificar varios executionIds si se separan con un punto y coma ";".</span><span class="sxs-lookup"><span data-stu-id="47fb8-392">Multiple executionIds can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="47fb8-393">executionStatus</span><span class="sxs-lookup"><span data-stu-id="47fb8-393">executionStatus</span></span>    |    <span data-ttu-id="47fb8-394">No</span><span class="sxs-lookup"><span data-stu-id="47fb8-394">No</span></span>    |    <span data-ttu-id="47fb8-395">Cadena/enumeración</span><span class="sxs-lookup"><span data-stu-id="47fb8-395">String/enum</span></span>    |    <span data-ttu-id="47fb8-396">Filtre para obtener detalles de solo los informes con executionStatus especificado en este argumento.</span><span class="sxs-lookup"><span data-stu-id="47fb8-396">Filter to get details of only reports with the executionStatus given in this argument.</span></span> <br> <span data-ttu-id="47fb8-397">Los valores válidos `Pending` son: `Running` , y `Paused` `Completed` .</span><span class="sxs-lookup"><span data-stu-id="47fb8-397">Valid values are: `Pending`, `Running`, `Paused` and `Completed`.</span></span> <br> <span data-ttu-id="47fb8-398">El valor predeterminado es `Completed`.</span><span class="sxs-lookup"><span data-stu-id="47fb8-398">The default value is `Completed`.</span></span> <br> <span data-ttu-id="47fb8-399">Se pueden especificar varios estados si se separan con un punto y coma ";".</span><span class="sxs-lookup"><span data-stu-id="47fb8-399">Multiple statuses can be specified by separating them with a semicolon ";".</span></span>    |
|    <span data-ttu-id="47fb8-400">getLatestExecution</span><span class="sxs-lookup"><span data-stu-id="47fb8-400">getLatestExecution</span></span>    |    <span data-ttu-id="47fb8-401">No</span><span class="sxs-lookup"><span data-stu-id="47fb8-401">No</span></span>    |    <span data-ttu-id="47fb8-402">boolean</span><span class="sxs-lookup"><span data-stu-id="47fb8-402">boolean</span></span>    |    <span data-ttu-id="47fb8-403">La API devolverá los detalles de la ejecución más reciente.</span><span class="sxs-lookup"><span data-stu-id="47fb8-403">The API will return details of the latest execution.</span></span> <span data-ttu-id="47fb8-404">De forma predeterminada, este parámetro se establece en true.</span><span class="sxs-lookup"><span data-stu-id="47fb8-404">By default, this parameter is set to true.</span></span><br> <span data-ttu-id="47fb8-405">Si decide pasar el valor de este parámetro como false, la API devolverá las instancias de ejecución de los últimos 90 días.</span><span class="sxs-lookup"><span data-stu-id="47fb8-405">If you choose to pass the value of this parameter as false, then the API will return the last 90 days execution instances.</span></span>    |
|        |        |        |        |

### <a name="sample-request-payload"></a><span data-ttu-id="47fb8-406">Carga de solicitud de ejemplo</span><span class="sxs-lookup"><span data-stu-id="47fb8-406">Sample Request Payload</span></span>

<span data-ttu-id="47fb8-407">Ninguno</span><span class="sxs-lookup"><span data-stu-id="47fb8-407">None</span></span>

### <a name="sample-response"></a><span data-ttu-id="47fb8-408">Respuesta de ejemplo</span><span class="sxs-lookup"><span data-stu-id="47fb8-408">Sample Response</span></span>

<span data-ttu-id="47fb8-409">La carga de respuesta tiene la estructura siguiente:</span><span class="sxs-lookup"><span data-stu-id="47fb8-409">The response payload is structured as follows:</span></span>

<span data-ttu-id="47fb8-410">Códigos de respuesta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="47fb8-410">Response Codes: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="47fb8-411">Ejemplo de carga de respuesta:</span><span class="sxs-lookup"><span data-stu-id="47fb8-411">Response payload example:</span></span>

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

<span data-ttu-id="47fb8-412">Una vez completada la ejecución del informe, se muestra el estado de ejecución `Completed`.</span><span class="sxs-lookup"><span data-stu-id="47fb8-412">Once report execution is complete, the execution status `Completed` is shown.</span></span> <span data-ttu-id="47fb8-413">Puede descargar el informe seleccionando la dirección URL en `reportAccessSecureLink`.</span><span class="sxs-lookup"><span data-stu-id="47fb8-413">You can download the report by selecting the URL in the `reportAccessSecureLink`.</span></span>

### <a name="glossary"></a><span data-ttu-id="47fb8-414">Glosario</span><span class="sxs-lookup"><span data-stu-id="47fb8-414">Glossary</span></span>

<span data-ttu-id="47fb8-415">Definiciones clave de los elementos de la respuesta.</span><span class="sxs-lookup"><span data-stu-id="47fb8-415">Key definitions of elements in the response.</span></span>

|    <span data-ttu-id="47fb8-416">Parámetro</span><span class="sxs-lookup"><span data-stu-id="47fb8-416">Parameter</span></span>    |    <span data-ttu-id="47fb8-417">Descripción</span><span class="sxs-lookup"><span data-stu-id="47fb8-417">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="47fb8-418">ExecutionId</span><span class="sxs-lookup"><span data-stu-id="47fb8-418">ExecutionId</span></span>    |    <span data-ttu-id="47fb8-419">Identificador único universal (UUID) de la instancia de ejecución.</span><span class="sxs-lookup"><span data-stu-id="47fb8-419">Universally unique identifier (UUID) of the execution instance</span></span>    |
|    <span data-ttu-id="47fb8-420">ReportId</span><span class="sxs-lookup"><span data-stu-id="47fb8-420">ReportId</span></span>    |    <span data-ttu-id="47fb8-421">Id. de informe asociado a la instancia de ejecución.</span><span class="sxs-lookup"><span data-stu-id="47fb8-421">Report ID associated with the execution instance</span></span>    |
|    <span data-ttu-id="47fb8-422">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="47fb8-422">RecurrenceInterval</span></span>    |    <span data-ttu-id="47fb8-423">Intervalo de periodicidad proporcionado durante la creación del informe.</span><span class="sxs-lookup"><span data-stu-id="47fb8-423">Recurrence interval provided during report creation</span></span>    |
|    <span data-ttu-id="47fb8-424">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="47fb8-424">RecurrenceCount</span></span>    |    <span data-ttu-id="47fb8-425">Recuento de periodicidad proporcionado durante la creación del informe.</span><span class="sxs-lookup"><span data-stu-id="47fb8-425">Recurrence count provided during report creation</span></span>    |
|    <span data-ttu-id="47fb8-426">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="47fb8-426">CallbackUrl</span></span>    |    <span data-ttu-id="47fb8-427">Dirección URL de devolución de llamada asociada a la instancia de ejecución.</span><span class="sxs-lookup"><span data-stu-id="47fb8-427">Callback URL associated with the execution instance</span></span>    |
|    <span data-ttu-id="47fb8-428">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="47fb8-428">CallbackMethod</span></span>    |    <span data-ttu-id="47fb8-429">Método de devolución de llamada asociado a la instancia de ejecución</span><span class="sxs-lookup"><span data-stu-id="47fb8-429">Callback method associated with the execution instance</span></span>    |
|    <span data-ttu-id="47fb8-430">Formato</span><span class="sxs-lookup"><span data-stu-id="47fb8-430">Format</span></span>    |    <span data-ttu-id="47fb8-431">Formato del archivo generado al final de la ejecución.</span><span class="sxs-lookup"><span data-stu-id="47fb8-431">Format of the generated file at the end of execution</span></span>    |
|    <span data-ttu-id="47fb8-432">ExecutionStatus</span><span class="sxs-lookup"><span data-stu-id="47fb8-432">ExecutionStatus</span></span>    |    <span data-ttu-id="47fb8-433">Estado de la instancia de ejecución del informe.</span><span class="sxs-lookup"><span data-stu-id="47fb8-433">Status of the report execution instance.</span></span> <br> <span data-ttu-id="47fb8-434">Los valores válidos son `Pending`, `Running`, `Paused` y `Completed`.</span><span class="sxs-lookup"><span data-stu-id="47fb8-434">Valid values are: `Pending`, `Running`, `Paused`, and `Completed`</span></span>    |
|    <span data-ttu-id="47fb8-435">ReportAccessSecureLink</span><span class="sxs-lookup"><span data-stu-id="47fb8-435">ReportAccessSecureLink</span></span>    |<span data-ttu-id="47fb8-436">Vínculo a través del cual se puede acceder al informe de forma segura.</span><span class="sxs-lookup"><span data-stu-id="47fb8-436">Link through which the report can be accessed securely</span></span>        |
|    <span data-ttu-id="47fb8-437">ReportExpiryTime</span><span class="sxs-lookup"><span data-stu-id="47fb8-437">ReportExpiryTime</span></span>    |    <span data-ttu-id="47fb8-438">Hora UTC después de la cual el vínculo de informe expirará en el formato aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="47fb8-438">UTC Time after which the report link will expire in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="47fb8-439">ReportGeneratedTime</span><span class="sxs-lookup"><span data-stu-id="47fb8-439">ReportGeneratedTime</span></span>    |    <span data-ttu-id="47fb8-440">Hora UTC a la que se generó el informe en el formato aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="47fb8-440">UTC Time at which the report was generated in this format: yyyy-MM-ddTHH:mm:ssZ</span></span>    |
|    <span data-ttu-id="47fb8-441">TotalCount</span><span class="sxs-lookup"><span data-stu-id="47fb8-441">TotalCount</span></span>    |    <span data-ttu-id="47fb8-442">Número de conjuntos de datos en la matriz de valores.</span><span class="sxs-lookup"><span data-stu-id="47fb8-442">Number of datasets in the Value array</span></span>    |
|    <span data-ttu-id="47fb8-443">StatusCode</span><span class="sxs-lookup"><span data-stu-id="47fb8-443">StatusCode</span></span>    |    <span data-ttu-id="47fb8-444">Código de resultado</span><span class="sxs-lookup"><span data-stu-id="47fb8-444">Result Code</span></span> <br> <span data-ttu-id="47fb8-445">Los valores posibles son 200, 400, 401, 403, 404 y 500.</span><span class="sxs-lookup"><span data-stu-id="47fb8-445">The possible values are 200, 400, 401, 403, 404 and 500</span></span>    |
|    <span data-ttu-id="47fb8-446">message</span><span class="sxs-lookup"><span data-stu-id="47fb8-446">message</span></span>    |    <span data-ttu-id="47fb8-447">Mensaje de estado de la ejecución de la API.</span><span class="sxs-lookup"><span data-stu-id="47fb8-447">Status message from the execution of the API</span></span>    |
|        |        |

## <a name="next-steps"></a><span data-ttu-id="47fb8-448">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="47fb8-448">Next steps</span></span>

- <span data-ttu-id="47fb8-449">Pruebe las API a través de la dirección [URL de la API de swagger.](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span><span class="sxs-lookup"><span data-stu-id="47fb8-449">Try out the APIs through the [swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html)</span></span>
- [<span data-ttu-id="47fb8-450">Realice su primera llamada API</span><span class="sxs-lookup"><span data-stu-id="47fb8-450">Make your first API call</span></span>](insights-programmatic-first-api-call.md)