---
title: 'Obtener la API de informe: Ideas datos'
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para obtener todos los identificadores de informe disponibles en Centro de partners insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376122"
---
# <a name="get-report-api"></a><span data-ttu-id="41ce5-103">Obtención de API de informe</span><span class="sxs-lookup"><span data-stu-id="41ce5-103">Get report API</span></span>

<span data-ttu-id="41ce5-104">Esta API obtiene todos los informes que se han programado.</span><span class="sxs-lookup"><span data-stu-id="41ce5-104">This API gets all the reports that have been scheduled.</span></span>

<span data-ttu-id="41ce5-105">**Sintaxis de la solicitud**</span><span class="sxs-lookup"><span data-stu-id="41ce5-105">**Request syntax**</span></span>

|    <span data-ttu-id="41ce5-106">Método</span><span class="sxs-lookup"><span data-stu-id="41ce5-106">Method</span></span>    |    <span data-ttu-id="41ce5-107">URI de solicitud</span><span class="sxs-lookup"><span data-stu-id="41ce5-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="41ce5-108">GET</span><span class="sxs-lookup"><span data-stu-id="41ce5-108">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

<span data-ttu-id="41ce5-109">**Encabezado de solicitud**</span><span class="sxs-lookup"><span data-stu-id="41ce5-109">**Request header**</span></span>

|    <span data-ttu-id="41ce5-110">Encabezado</span><span class="sxs-lookup"><span data-stu-id="41ce5-110">Header</span></span>    |    <span data-ttu-id="41ce5-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="41ce5-111">Type</span></span>    |    <span data-ttu-id="41ce5-112">Descripción</span><span class="sxs-lookup"><span data-stu-id="41ce5-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="41ce5-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="41ce5-113">Authorization</span></span>    |    <span data-ttu-id="41ce5-114">string</span><span class="sxs-lookup"><span data-stu-id="41ce5-114">string</span></span>    |    <span data-ttu-id="41ce5-115">Necesario.</span><span class="sxs-lookup"><span data-stu-id="41ce5-115">Required.</span></span> <span data-ttu-id="41ce5-116">Token Azure Active Directory de acceso de Azure Active Directory (AAD) en el formulario`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="41ce5-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="41ce5-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="41ce5-117">Content-Type</span></span>    |    <span data-ttu-id="41ce5-118">string</span><span class="sxs-lookup"><span data-stu-id="41ce5-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="41ce5-119">**Parámetro de ruta de acceso**</span><span class="sxs-lookup"><span data-stu-id="41ce5-119">**Path parameter**</span></span>

<span data-ttu-id="41ce5-120">Ninguno</span><span class="sxs-lookup"><span data-stu-id="41ce5-120">None</span></span>

<span data-ttu-id="41ce5-121">**Parámetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="41ce5-121">**Query parameter**</span></span>

|    <span data-ttu-id="41ce5-122">Nombre de parámetro</span><span class="sxs-lookup"><span data-stu-id="41ce5-122">Parameter Name</span></span>    |    <span data-ttu-id="41ce5-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="41ce5-123">Type</span></span>    |    <span data-ttu-id="41ce5-124">Obligatorio</span><span class="sxs-lookup"><span data-stu-id="41ce5-124">Required</span></span>    |    <span data-ttu-id="41ce5-125">Descripción</span><span class="sxs-lookup"><span data-stu-id="41ce5-125">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="41ce5-126">reportId</span><span class="sxs-lookup"><span data-stu-id="41ce5-126">reportId</span></span>     |    <span data-ttu-id="41ce5-127">string</span><span class="sxs-lookup"><span data-stu-id="41ce5-127">string</span></span>    |    <span data-ttu-id="41ce5-128">No</span><span class="sxs-lookup"><span data-stu-id="41ce5-128">No</span></span>    |    <span data-ttu-id="41ce5-129">Filtre para obtener detalles de solo los informes con el valor de reportId especificado en este argumento.</span><span class="sxs-lookup"><span data-stu-id="41ce5-129">Filter to get details of only reports with the reportId given in this argument</span></span>     |
|    <span data-ttu-id="41ce5-130">reportName</span><span class="sxs-lookup"><span data-stu-id="41ce5-130">reportName</span></span>     |    <span data-ttu-id="41ce5-131">string</span><span class="sxs-lookup"><span data-stu-id="41ce5-131">string</span></span>    |    <span data-ttu-id="41ce5-132">No</span><span class="sxs-lookup"><span data-stu-id="41ce5-132">No</span></span>    |    <span data-ttu-id="41ce5-133">Filtre para obtener detalles de solo los informes con el valor reportName especificado en este argumento.</span><span class="sxs-lookup"><span data-stu-id="41ce5-133">Filter to get details of only reports with the reportName given in this argument</span></span>     |
|    <span data-ttu-id="41ce5-134">queryId</span><span class="sxs-lookup"><span data-stu-id="41ce5-134">queryId</span></span>     |    <span data-ttu-id="41ce5-135">string</span><span class="sxs-lookup"><span data-stu-id="41ce5-135">string</span></span>    |    <span data-ttu-id="41ce5-136">No</span><span class="sxs-lookup"><span data-stu-id="41ce5-136">No</span></span>    |    <span data-ttu-id="41ce5-137">Filtre para obtener detalles de solo los informes con el valor de queryId especificado en este argumento.</span><span class="sxs-lookup"><span data-stu-id="41ce5-137">Filter to get details of only reports with the queryId given in this argument</span></span>     |
|        |        |        |        |


<span data-ttu-id="41ce5-138">**Carga de solicitud**</span><span class="sxs-lookup"><span data-stu-id="41ce5-138">**Request payload**</span></span>

<span data-ttu-id="41ce5-139">Ninguno</span><span class="sxs-lookup"><span data-stu-id="41ce5-139">None</span></span>

<span data-ttu-id="41ce5-140">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="41ce5-140">**Glossary**</span></span>

<span data-ttu-id="41ce5-141">Ninguno</span><span class="sxs-lookup"><span data-stu-id="41ce5-141">None</span></span>

<span data-ttu-id="41ce5-142">**Respuesta**</span><span class="sxs-lookup"><span data-stu-id="41ce5-142">**Response**</span></span>

<span data-ttu-id="41ce5-143">La carga de respuesta tiene la estructura siguiente:</span><span class="sxs-lookup"><span data-stu-id="41ce5-143">The response payload is structured as follows:</span></span>

<span data-ttu-id="41ce5-144">Código de respuesta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="41ce5-144">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="41ce5-145">Ejemplo de carga de respuesta:</span><span class="sxs-lookup"><span data-stu-id="41ce5-145">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "ReportId": "string", 
      "ReportName": "string", 
      "Description": "string", 
      "QueryId": "string", 
      "Query": "string", 
      "User": "string", 
      "CreatedTime": "string", 
      "ModifiedTime": "string", 
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

<span data-ttu-id="41ce5-146">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="41ce5-146">**Glossary**</span></span>

<span data-ttu-id="41ce5-147">En esta tabla se definen los elementos clave de la respuesta:</span><span class="sxs-lookup"><span data-stu-id="41ce5-147">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="41ce5-148">Parámetro</span><span class="sxs-lookup"><span data-stu-id="41ce5-148">Parameter</span></span>    |    <span data-ttu-id="41ce5-149">Descripción</span><span class="sxs-lookup"><span data-stu-id="41ce5-149">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="41ce5-150">ReportId</span><span class="sxs-lookup"><span data-stu-id="41ce5-150">ReportId</span></span>     |    <span data-ttu-id="41ce5-151">UUID único del informe que se creó.</span><span class="sxs-lookup"><span data-stu-id="41ce5-151">Unique UUID of the report that was created</span></span>     |
|    <span data-ttu-id="41ce5-152">ReportName</span><span class="sxs-lookup"><span data-stu-id="41ce5-152">ReportName</span></span>     |    <span data-ttu-id="41ce5-153">Nombre dado al informe en la carga útil de solicitud</span><span class="sxs-lookup"><span data-stu-id="41ce5-153">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="41ce5-154">Descripción</span><span class="sxs-lookup"><span data-stu-id="41ce5-154">Description</span></span>     |    <span data-ttu-id="41ce5-155">Descripción dada cuando se creó el informe.</span><span class="sxs-lookup"><span data-stu-id="41ce5-155">Description given when the report was created</span></span>     |
|    <span data-ttu-id="41ce5-156">QueryId</span><span class="sxs-lookup"><span data-stu-id="41ce5-156">QueryId</span></span>     |    <span data-ttu-id="41ce5-157">Id. de consulta pasado en el momento en que se creó el informe.</span><span class="sxs-lookup"><span data-stu-id="41ce5-157">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="41ce5-158">Consultar</span><span class="sxs-lookup"><span data-stu-id="41ce5-158">Query</span></span>     |    <span data-ttu-id="41ce5-159">Texto de la consulta que se ejecutará para este informe.</span><span class="sxs-lookup"><span data-stu-id="41ce5-159">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="41ce5-160">Usuario</span><span class="sxs-lookup"><span data-stu-id="41ce5-160">User</span></span>     |    <span data-ttu-id="41ce5-161">Identificador de usuario usado para crear el informe</span><span class="sxs-lookup"><span data-stu-id="41ce5-161">User ID used to create the report</span></span>     |
|    <span data-ttu-id="41ce5-162">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="41ce5-162">CreatedTime</span></span>     |    <span data-ttu-id="41ce5-163">Hora de creación del informe.</span><span class="sxs-lookup"><span data-stu-id="41ce5-163">Time the report was created.</span></span> <span data-ttu-id="41ce5-164">El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="41ce5-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="41ce5-165">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="41ce5-165">ModifiedTime</span></span>     |    <span data-ttu-id="41ce5-166">Hora en que se modificó el informe por última vez.</span><span class="sxs-lookup"><span data-stu-id="41ce5-166">Time the report was last modified.</span></span> <span data-ttu-id="41ce5-167">El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="41ce5-167">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="41ce5-168">executeNow</span><span class="sxs-lookup"><span data-stu-id="41ce5-168">executeNow</span></span>     |    <span data-ttu-id="41ce5-169">Marca ExecuteNow establecida en el momento en que se creó el informe</span><span class="sxs-lookup"><span data-stu-id="41ce5-169">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="41ce5-170">StartTime</span><span class="sxs-lookup"><span data-stu-id="41ce5-170">StartTime</span></span>     |    <span data-ttu-id="41ce5-171">Se iniciará la ejecución de la hora.</span><span class="sxs-lookup"><span data-stu-id="41ce5-171">Time execution will begin.</span></span> <span data-ttu-id="41ce5-172">El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="41ce5-172">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="41ce5-173">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="41ce5-173">ReportStatus</span></span>     |    <span data-ttu-id="41ce5-174">Estado de la ejecución del informe.</span><span class="sxs-lookup"><span data-stu-id="41ce5-174">Status of the report execution.</span></span> <span data-ttu-id="41ce5-175">Los valores posibles son en pausa, activo e inactivo.</span><span class="sxs-lookup"><span data-stu-id="41ce5-175">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="41ce5-176">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="41ce5-176">RecurrenceInterval</span></span>     |    <span data-ttu-id="41ce5-177">Intervalo de periodicidad proporcionado durante la creación del informe.</span><span class="sxs-lookup"><span data-stu-id="41ce5-177">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="41ce5-178">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="41ce5-178">RecurrenceCount</span></span>     |    <span data-ttu-id="41ce5-179">Recuento de periodicidad proporcionado durante la creación del informe.</span><span class="sxs-lookup"><span data-stu-id="41ce5-179">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="41ce5-180">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="41ce5-180">CallbackUrl</span></span>     |    <span data-ttu-id="41ce5-181">Dirección URL de devolución de llamada proporcionada en la solicitud.</span><span class="sxs-lookup"><span data-stu-id="41ce5-181">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="41ce5-182">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="41ce5-182">CallbackMethod</span></span>    |    <span data-ttu-id="41ce5-183">Método de devolución de llamada proporcionado en la solicitud</span><span class="sxs-lookup"><span data-stu-id="41ce5-183">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="41ce5-184">Formato</span><span class="sxs-lookup"><span data-stu-id="41ce5-184">Format</span></span>     |    <span data-ttu-id="41ce5-185">Formato de los archivos de informe.</span><span class="sxs-lookup"><span data-stu-id="41ce5-185">Format of the report files</span></span>     |
|    <span data-ttu-id="41ce5-186">TotalCount</span><span class="sxs-lookup"><span data-stu-id="41ce5-186">TotalCount</span></span>     |    <span data-ttu-id="41ce5-187">Número de conjuntos de datos en la matriz de valores.</span><span class="sxs-lookup"><span data-stu-id="41ce5-187">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="41ce5-188">Message</span><span class="sxs-lookup"><span data-stu-id="41ce5-188">Message</span></span>     |    <span data-ttu-id="41ce5-189">Mensaje de estado de la ejecución de la API.</span><span class="sxs-lookup"><span data-stu-id="41ce5-189">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="41ce5-190">StatusCode</span><span class="sxs-lookup"><span data-stu-id="41ce5-190">StatusCode</span></span>     |    <span data-ttu-id="41ce5-191">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="41ce5-191">Result Code.</span></span> <span data-ttu-id="41ce5-192">Los valores posibles son 200, 400, 401, 403 y 500.</span><span class="sxs-lookup"><span data-stu-id="41ce5-192">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |