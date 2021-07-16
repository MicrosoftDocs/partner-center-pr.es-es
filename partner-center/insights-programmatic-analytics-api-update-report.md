---
title: Actualización de la API de informe
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para actualizar los parámetros de informe en Centro de partners insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376090"
---
# <a name="update-report-api"></a><span data-ttu-id="71c03-103">Actualización de la API de informe</span><span class="sxs-lookup"><span data-stu-id="71c03-103">Update report API</span></span>

<span data-ttu-id="71c03-104">Esta API ayuda a modificar un parámetro de informe.</span><span class="sxs-lookup"><span data-stu-id="71c03-104">This API helps you modify a report parameter.</span></span>

<span data-ttu-id="71c03-105">**Sintaxis de la solicitud**</span><span class="sxs-lookup"><span data-stu-id="71c03-105">**Request syntax**</span></span>

|    <span data-ttu-id="71c03-106">Método</span><span class="sxs-lookup"><span data-stu-id="71c03-106">Method</span></span>    |    <span data-ttu-id="71c03-107">URI de la solicitud</span><span class="sxs-lookup"><span data-stu-id="71c03-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="71c03-108">PUT</span><span class="sxs-lookup"><span data-stu-id="71c03-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="71c03-109">**Encabezado de solicitud**</span><span class="sxs-lookup"><span data-stu-id="71c03-109">**Request header**</span></span>

|    <span data-ttu-id="71c03-110">Encabezado</span><span class="sxs-lookup"><span data-stu-id="71c03-110">Header</span></span>    |    <span data-ttu-id="71c03-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="71c03-111">Type</span></span>    |    <span data-ttu-id="71c03-112">Descripción</span><span class="sxs-lookup"><span data-stu-id="71c03-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="71c03-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="71c03-113">Authorization</span></span>    |    <span data-ttu-id="71c03-114">string</span><span class="sxs-lookup"><span data-stu-id="71c03-114">string</span></span>    |    <span data-ttu-id="71c03-115">Necesario.</span><span class="sxs-lookup"><span data-stu-id="71c03-115">Required.</span></span> <span data-ttu-id="71c03-116">Token Azure Active Directory de acceso de Azure Active Directory (AAD) en el formulario`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="71c03-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="71c03-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="71c03-117">Content-Type</span></span>    |    <span data-ttu-id="71c03-118">string</span><span class="sxs-lookup"><span data-stu-id="71c03-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="71c03-119">**Parámetro de ruta de acceso**</span><span class="sxs-lookup"><span data-stu-id="71c03-119">**Path parameter**</span></span>

|    <span data-ttu-id="71c03-120">Nombre de parámetro</span><span class="sxs-lookup"><span data-stu-id="71c03-120">Parameter Name</span></span>    |    <span data-ttu-id="71c03-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="71c03-121">Type</span></span>    |    <span data-ttu-id="71c03-122">Obligatorio</span><span class="sxs-lookup"><span data-stu-id="71c03-122">Required</span></span>    |    <span data-ttu-id="71c03-123">Descripción</span><span class="sxs-lookup"><span data-stu-id="71c03-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="71c03-124">reportId</span><span class="sxs-lookup"><span data-stu-id="71c03-124">reportId</span></span>     |    <span data-ttu-id="71c03-125">string</span><span class="sxs-lookup"><span data-stu-id="71c03-125">string</span></span>    |    <span data-ttu-id="71c03-126">No</span><span class="sxs-lookup"><span data-stu-id="71c03-126">No</span></span>    |    <span data-ttu-id="71c03-127">Id. del informe que se está modificando</span><span class="sxs-lookup"><span data-stu-id="71c03-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="71c03-128">**Parámetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="71c03-128">**Query parameter**</span></span>

<span data-ttu-id="71c03-129">Ninguno</span><span class="sxs-lookup"><span data-stu-id="71c03-129">None</span></span>

<span data-ttu-id="71c03-130">**Carga de solicitud**</span><span class="sxs-lookup"><span data-stu-id="71c03-130">**Request payload**</span></span>

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

<span data-ttu-id="71c03-131">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="71c03-131">**Glossary**</span></span>

<span data-ttu-id="71c03-132">En esta tabla se indican las definiciones clave de los elementos de la respuesta.</span><span class="sxs-lookup"><span data-stu-id="71c03-132">This table lists the key definitions of elements in the response.</span></span>

|    <span data-ttu-id="71c03-133">Parámetro</span><span class="sxs-lookup"><span data-stu-id="71c03-133">Parameter</span></span>    |    <span data-ttu-id="71c03-134">Obligatorio</span><span class="sxs-lookup"><span data-stu-id="71c03-134">Required</span></span>    |    <span data-ttu-id="71c03-135">Descripción</span><span class="sxs-lookup"><span data-stu-id="71c03-135">Description</span></span>    |    <span data-ttu-id="71c03-136">Valores permitidos</span><span class="sxs-lookup"><span data-stu-id="71c03-136">Allowed Values</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="71c03-137">ReportName</span><span class="sxs-lookup"><span data-stu-id="71c03-137">ReportName</span></span>     |    <span data-ttu-id="71c03-138">Sí</span><span class="sxs-lookup"><span data-stu-id="71c03-138">Yes</span></span>     |    <span data-ttu-id="71c03-139">Nombre que se va a asignar al informe</span><span class="sxs-lookup"><span data-stu-id="71c03-139">Name to be assigned to the report</span></span>     |    <span data-ttu-id="71c03-140">String</span><span class="sxs-lookup"><span data-stu-id="71c03-140">String</span></span>     |
|    <span data-ttu-id="71c03-141">Descripción</span><span class="sxs-lookup"><span data-stu-id="71c03-141">Description</span></span>     |    <span data-ttu-id="71c03-142">No</span><span class="sxs-lookup"><span data-stu-id="71c03-142">No</span></span>     |    <span data-ttu-id="71c03-143">Descripción del informe creado</span><span class="sxs-lookup"><span data-stu-id="71c03-143">Description of the created report</span></span>     |    <span data-ttu-id="71c03-144">String</span><span class="sxs-lookup"><span data-stu-id="71c03-144">String</span></span>     |
|    <span data-ttu-id="71c03-145">StartTime</span><span class="sxs-lookup"><span data-stu-id="71c03-145">StartTime</span></span>     |    <span data-ttu-id="71c03-146">Sí</span><span class="sxs-lookup"><span data-stu-id="71c03-146">Yes</span></span>    |    <span data-ttu-id="71c03-147">Marca de tiempo después de la que comenzará la generación del informe</span><span class="sxs-lookup"><span data-stu-id="71c03-147">Timestamp after which the report generation will begin</span></span>     |    <span data-ttu-id="71c03-148">String</span><span class="sxs-lookup"><span data-stu-id="71c03-148">String</span></span>     |
|    <span data-ttu-id="71c03-149">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="71c03-149">RecurrenceInterval</span></span>     |    <span data-ttu-id="71c03-150">No</span><span class="sxs-lookup"><span data-stu-id="71c03-150">No</span></span>     |    <span data-ttu-id="71c03-151">Frecuencia (en horas) con la que se debe generar el informe.</span><span class="sxs-lookup"><span data-stu-id="71c03-151">Frequency at which the report should be generated in hours.</span></span> <span data-ttu-id="71c03-152">El valor mínimo es 4.</span><span class="sxs-lookup"><span data-stu-id="71c03-152">Minimum value is 4</span></span>     |    <span data-ttu-id="71c03-153">Entero</span><span class="sxs-lookup"><span data-stu-id="71c03-153">Integer</span></span>     |
|    <span data-ttu-id="71c03-154">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="71c03-154">RecurrenceCount</span></span>     |    <span data-ttu-id="71c03-155">No</span><span class="sxs-lookup"><span data-stu-id="71c03-155">No</span></span>     |    <span data-ttu-id="71c03-156">Números de informe que se generarán.</span><span class="sxs-lookup"><span data-stu-id="71c03-156">Numbers of report to be generated.</span></span> <span data-ttu-id="71c03-157">El valor predeterminado es indefinido.</span><span class="sxs-lookup"><span data-stu-id="71c03-157">Default is indefinite.</span></span>     |    <span data-ttu-id="71c03-158">Entero</span><span class="sxs-lookup"><span data-stu-id="71c03-158">Integer</span></span>     |
|    <span data-ttu-id="71c03-159">Formato</span><span class="sxs-lookup"><span data-stu-id="71c03-159">Format</span></span>     |    <span data-ttu-id="71c03-160">No</span><span class="sxs-lookup"><span data-stu-id="71c03-160">No</span></span>    |    <span data-ttu-id="71c03-161">Formato del archivo exportado.</span><span class="sxs-lookup"><span data-stu-id="71c03-161">File format of the exported file.</span></span> <span data-ttu-id="71c03-162">El valor predeterminado es CSV</span><span class="sxs-lookup"><span data-stu-id="71c03-162">Default is CSV</span></span>     |    <span data-ttu-id="71c03-163">CSV/TSV</span><span class="sxs-lookup"><span data-stu-id="71c03-163">CSV/TSV</span></span>     |
|    <span data-ttu-id="71c03-164">CallbackURL</span><span class="sxs-lookup"><span data-stu-id="71c03-164">CallbackURL</span></span>     |    <span data-ttu-id="71c03-165">No</span><span class="sxs-lookup"><span data-stu-id="71c03-165">No</span></span>     |    <span data-ttu-id="71c03-166">Dirección URL de devolución de llamada HTTPS a la que se llamará en la generación de informes.</span><span class="sxs-lookup"><span data-stu-id="71c03-166">https callback URL to be called on report generation</span></span>     |    <span data-ttu-id="71c03-167">String</span><span class="sxs-lookup"><span data-stu-id="71c03-167">String</span></span>     |
|    <span data-ttu-id="71c03-168">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="71c03-168">CallbackMethod</span></span>    |    <span data-ttu-id="71c03-169">No</span><span class="sxs-lookup"><span data-stu-id="71c03-169">No</span></span>    |    <span data-ttu-id="71c03-170">Método HTTP que se va a usar para la devolución de llamada</span><span class="sxs-lookup"><span data-stu-id="71c03-170">Http method to be used for callback</span></span>    |    <span data-ttu-id="71c03-171">GET/POST</span><span class="sxs-lookup"><span data-stu-id="71c03-171">GET/POST</span></span>    |
|        |        |        |        |


<span data-ttu-id="71c03-172">**Respuesta**</span><span class="sxs-lookup"><span data-stu-id="71c03-172">**Response**</span></span>

<span data-ttu-id="71c03-173">La carga de respuesta tiene la estructura siguiente:</span><span class="sxs-lookup"><span data-stu-id="71c03-173">The response payload is structured as follows:</span></span>

<span data-ttu-id="71c03-174">Código de respuesta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="71c03-174">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="71c03-175">Ejemplo de carga de respuesta:</span><span class="sxs-lookup"><span data-stu-id="71c03-175">Response payload example:</span></span>

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
      "ExecuteNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      "RecurrenceCount": 0, 
      "CallbackUrl": "string", 
      "CallbackMethod": "string", 
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="71c03-176">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="71c03-176">**Glossary**</span></span>

<span data-ttu-id="71c03-177">En esta tabla se definen los elementos clave de la respuesta:</span><span class="sxs-lookup"><span data-stu-id="71c03-177">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="71c03-178">Parámetro</span><span class="sxs-lookup"><span data-stu-id="71c03-178">Parameter</span></span>    |    <span data-ttu-id="71c03-179">Descripción</span><span class="sxs-lookup"><span data-stu-id="71c03-179">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="71c03-180">ReportId</span><span class="sxs-lookup"><span data-stu-id="71c03-180">ReportId</span></span>     |    <span data-ttu-id="71c03-181">Identificador único universal (UUID) del informe que se actualiza</span><span class="sxs-lookup"><span data-stu-id="71c03-181">Universally unique identifier (UUID) of the report being updated</span></span>     |
|    <span data-ttu-id="71c03-182">ReportName</span><span class="sxs-lookup"><span data-stu-id="71c03-182">ReportName</span></span>     |    <span data-ttu-id="71c03-183">Nombre dado al informe en la carga útil de solicitud</span><span class="sxs-lookup"><span data-stu-id="71c03-183">Name given to the report in the request payload</span></span>     |
|    <span data-ttu-id="71c03-184">Descripción</span><span class="sxs-lookup"><span data-stu-id="71c03-184">Description</span></span>     |    <span data-ttu-id="71c03-185">Descripción dada al informe en la carga de solicitud</span><span class="sxs-lookup"><span data-stu-id="71c03-185">Description given to the report in the request payload</span></span>     |
|    <span data-ttu-id="71c03-186">QueryId</span><span class="sxs-lookup"><span data-stu-id="71c03-186">QueryId</span></span>     |    <span data-ttu-id="71c03-187">Id. de consulta pasado en el momento en que se creó el informe.</span><span class="sxs-lookup"><span data-stu-id="71c03-187">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="71c03-188">Consultar</span><span class="sxs-lookup"><span data-stu-id="71c03-188">Query</span></span>     |    <span data-ttu-id="71c03-189">Texto de la consulta que se ejecutará para este informe.</span><span class="sxs-lookup"><span data-stu-id="71c03-189">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="71c03-190">Usuario</span><span class="sxs-lookup"><span data-stu-id="71c03-190">User</span></span>     |    <span data-ttu-id="71c03-191">Identificador de usuario usado para crear el informe</span><span class="sxs-lookup"><span data-stu-id="71c03-191">User ID used to create the report</span></span>     |
|    <span data-ttu-id="71c03-192">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="71c03-192">CreatedTime</span></span>     |    <span data-ttu-id="71c03-193">Hora de creación del informe.</span><span class="sxs-lookup"><span data-stu-id="71c03-193">Time the report was created.</span></span> <span data-ttu-id="71c03-194">El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="71c03-194">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="71c03-195">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="71c03-195">ModifiedTime</span></span>     |    <span data-ttu-id="71c03-196">Hora en que se modificó el informe por última vez.</span><span class="sxs-lookup"><span data-stu-id="71c03-196">Time the report was last modified.</span></span> <span data-ttu-id="71c03-197">El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="71c03-197">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="71c03-198">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="71c03-198">ExecuteNow</span></span>     |    <span data-ttu-id="71c03-199">Marca ExecuteNow establecida en el momento en que se creó el informe</span><span class="sxs-lookup"><span data-stu-id="71c03-199">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="71c03-200">StartTime</span><span class="sxs-lookup"><span data-stu-id="71c03-200">StartTime</span></span>     |    <span data-ttu-id="71c03-201">Hora a la que se iniciará la ejecución del informe.</span><span class="sxs-lookup"><span data-stu-id="71c03-201">Time the report execution will begin.</span></span> <span data-ttu-id="71c03-202">El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="71c03-202">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="71c03-203">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="71c03-203">ReportStatus</span></span>     |    <span data-ttu-id="71c03-204">Estado de la ejecución del informe.</span><span class="sxs-lookup"><span data-stu-id="71c03-204">Status of the report execution.</span></span> <span data-ttu-id="71c03-205">Los valores posibles son en pausa, activo e inactivo.</span><span class="sxs-lookup"><span data-stu-id="71c03-205">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="71c03-206">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="71c03-206">RecurrenceInterval</span></span>     |    <span data-ttu-id="71c03-207">Intervalo de periodicidad proporcionado en la carga de solicitud</span><span class="sxs-lookup"><span data-stu-id="71c03-207">Recurrence interval provided in the request payload</span></span>     |
|    <span data-ttu-id="71c03-208">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="71c03-208">RecurrenceCount</span></span>     |    <span data-ttu-id="71c03-209">Recuento de periodicidad proporcionado en la carga de solicitud</span><span class="sxs-lookup"><span data-stu-id="71c03-209">Recurrence count provided in the request payload</span></span>     |
|    <span data-ttu-id="71c03-210">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="71c03-210">CallbackUrl</span></span>     |    <span data-ttu-id="71c03-211">Dirección URL de devolución de llamada proporcionada en la solicitud.</span><span class="sxs-lookup"><span data-stu-id="71c03-211">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="71c03-212">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="71c03-212">CallbackMethod</span></span>    |    <span data-ttu-id="71c03-213">Método de devolución de llamada proporcionado en la solicitud</span><span class="sxs-lookup"><span data-stu-id="71c03-213">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="71c03-214">Formato</span><span class="sxs-lookup"><span data-stu-id="71c03-214">Format</span></span>     |    <span data-ttu-id="71c03-215">Formato de los archivos de informe.</span><span class="sxs-lookup"><span data-stu-id="71c03-215">Format of the report files</span></span>     |
|    <span data-ttu-id="71c03-216">TotalCount</span><span class="sxs-lookup"><span data-stu-id="71c03-216">TotalCount</span></span>     |    <span data-ttu-id="71c03-217">Número de conjuntos de datos en la matriz de valores.</span><span class="sxs-lookup"><span data-stu-id="71c03-217">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="71c03-218">Message</span><span class="sxs-lookup"><span data-stu-id="71c03-218">Message</span></span>     |    <span data-ttu-id="71c03-219">Mensaje de estado de la ejecución de la API.</span><span class="sxs-lookup"><span data-stu-id="71c03-219">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="71c03-220">StatusCode</span><span class="sxs-lookup"><span data-stu-id="71c03-220">StatusCode</span></span>     |    <span data-ttu-id="71c03-221">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="71c03-221">Result Code.</span></span> <span data-ttu-id="71c03-222">Los valores posibles son 200, 400, 401, 403 y 500.</span><span class="sxs-lookup"><span data-stu-id="71c03-222">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |