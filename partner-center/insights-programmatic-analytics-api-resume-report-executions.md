---
title: 'Reanudar la API de ejecución de informes: Ideas datos'
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para reanudar la ejecución de cualquier informe en pausa en Centro de partners insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 1372823425f3aefd025ffc3441623c1ceee34e1e
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376111"
---
# <a name="resume-report-executions-api"></a><span data-ttu-id="cab68-103">API de reanudación de ejecuciones de informes</span><span class="sxs-lookup"><span data-stu-id="cab68-103">Resume report executions API</span></span>

<span data-ttu-id="cab68-104">En la ejecución, esta API reanuda la ejecución programada de un informe en pausa.</span><span class="sxs-lookup"><span data-stu-id="cab68-104">On execution, this API resumes the scheduled execution of a paused report.</span></span>

<span data-ttu-id="cab68-105">**Sintaxis de la solicitud**</span><span class="sxs-lookup"><span data-stu-id="cab68-105">**Request syntax**</span></span>

|    <span data-ttu-id="cab68-106">Método</span><span class="sxs-lookup"><span data-stu-id="cab68-106">Method</span></span>    |    <span data-ttu-id="cab68-107">URI de la solicitud</span><span class="sxs-lookup"><span data-stu-id="cab68-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="cab68-108">PUT</span><span class="sxs-lookup"><span data-stu-id="cab68-108">PUT</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/resume/{ReportID}`    |
|        |        |

<span data-ttu-id="cab68-109">**Encabezado de solicitud**</span><span class="sxs-lookup"><span data-stu-id="cab68-109">**Request header**</span></span>

|    <span data-ttu-id="cab68-110">Encabezado</span><span class="sxs-lookup"><span data-stu-id="cab68-110">Header</span></span>    |    <span data-ttu-id="cab68-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="cab68-111">Type</span></span>    |    <span data-ttu-id="cab68-112">Descripción</span><span class="sxs-lookup"><span data-stu-id="cab68-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="cab68-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="cab68-113">Authorization</span></span>    |    <span data-ttu-id="cab68-114">string</span><span class="sxs-lookup"><span data-stu-id="cab68-114">string</span></span>    |    <span data-ttu-id="cab68-115">Necesario.</span><span class="sxs-lookup"><span data-stu-id="cab68-115">Required.</span></span> <span data-ttu-id="cab68-116">Token Azure Active Directory de acceso de Azure Active Directory (AAD) en el formulario`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="cab68-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="cab68-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cab68-117">Content-Type</span></span>    |    <span data-ttu-id="cab68-118">string</span><span class="sxs-lookup"><span data-stu-id="cab68-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="cab68-119">**Parámetro de ruta de acceso**</span><span class="sxs-lookup"><span data-stu-id="cab68-119">**Path parameter**</span></span>

|    <span data-ttu-id="cab68-120">Nombre de parámetro</span><span class="sxs-lookup"><span data-stu-id="cab68-120">Parameter Name</span></span>    |    <span data-ttu-id="cab68-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="cab68-121">Type</span></span>    |    <span data-ttu-id="cab68-122">Obligatorio</span><span class="sxs-lookup"><span data-stu-id="cab68-122">Required</span></span>    |    <span data-ttu-id="cab68-123">Descripción</span><span class="sxs-lookup"><span data-stu-id="cab68-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="cab68-124">reportId</span><span class="sxs-lookup"><span data-stu-id="cab68-124">reportId</span></span>     |    <span data-ttu-id="cab68-125">string</span><span class="sxs-lookup"><span data-stu-id="cab68-125">string</span></span>    |    <span data-ttu-id="cab68-126">No</span><span class="sxs-lookup"><span data-stu-id="cab68-126">No</span></span>    |    <span data-ttu-id="cab68-127">Id. del informe que se está modificando</span><span class="sxs-lookup"><span data-stu-id="cab68-127">ID of the report being modified</span></span>     |
|        |        |        |        |

<span data-ttu-id="cab68-128">**Parámetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="cab68-128">**Query parameter**</span></span>

<span data-ttu-id="cab68-129">Ninguno</span><span class="sxs-lookup"><span data-stu-id="cab68-129">None</span></span>

<span data-ttu-id="cab68-130">**Carga de solicitud**</span><span class="sxs-lookup"><span data-stu-id="cab68-130">**Request payload**</span></span>

<span data-ttu-id="cab68-131">Ninguno</span><span class="sxs-lookup"><span data-stu-id="cab68-131">None</span></span>

<span data-ttu-id="cab68-132">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="cab68-132">**Glossary**</span></span>

<span data-ttu-id="cab68-133">Ninguno</span><span class="sxs-lookup"><span data-stu-id="cab68-133">None</span></span>

<span data-ttu-id="cab68-134">**Respuesta**</span><span class="sxs-lookup"><span data-stu-id="cab68-134">**Response**</span></span>

<span data-ttu-id="cab68-135">La carga de respuesta tiene la estructura siguiente:</span><span class="sxs-lookup"><span data-stu-id="cab68-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="cab68-136">Código de respuesta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="cab68-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="cab68-137">Ejemplo de carga de respuesta:</span><span class="sxs-lookup"><span data-stu-id="cab68-137">Response payload example:</span></span>

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

<span data-ttu-id="cab68-138">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="cab68-138">**Glossary**</span></span>

<span data-ttu-id="cab68-139">En esta tabla se definen los elementos clave de la respuesta:</span><span class="sxs-lookup"><span data-stu-id="cab68-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="cab68-140">Parámetro</span><span class="sxs-lookup"><span data-stu-id="cab68-140">Parameter</span></span>    |    <span data-ttu-id="cab68-141">Descripción</span><span class="sxs-lookup"><span data-stu-id="cab68-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="cab68-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="cab68-142">ReportId</span></span>     |    <span data-ttu-id="cab68-143">Identificador único universal (UUID) del informe reanudado.</span><span class="sxs-lookup"><span data-stu-id="cab68-143">Universally unique identifier (UUID) of the resumed report</span></span>     |
|    <span data-ttu-id="cab68-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="cab68-144">ReportName</span></span>     |    <span data-ttu-id="cab68-145">Nombre dado al informe durante la creación.</span><span class="sxs-lookup"><span data-stu-id="cab68-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="cab68-146">Descripción</span><span class="sxs-lookup"><span data-stu-id="cab68-146">Description</span></span>     |    <span data-ttu-id="cab68-147">Descripción proporcionada durante la creación del informe.</span><span class="sxs-lookup"><span data-stu-id="cab68-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="cab68-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="cab68-148">QueryId</span></span>     |    <span data-ttu-id="cab68-149">Id. de consulta pasado en el momento en que se creó el informe.</span><span class="sxs-lookup"><span data-stu-id="cab68-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="cab68-150">Consultar</span><span class="sxs-lookup"><span data-stu-id="cab68-150">Query</span></span>     |    <span data-ttu-id="cab68-151">Texto de la consulta que se ejecutará para este informe.</span><span class="sxs-lookup"><span data-stu-id="cab68-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="cab68-152">Usuario</span><span class="sxs-lookup"><span data-stu-id="cab68-152">User</span></span>     |    <span data-ttu-id="cab68-153">Identificador de usuario usado para crear el informe</span><span class="sxs-lookup"><span data-stu-id="cab68-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="cab68-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="cab68-154">CreatedTime</span></span>     |    <span data-ttu-id="cab68-155">Hora de creación del informe.</span><span class="sxs-lookup"><span data-stu-id="cab68-155">Time the report was created.</span></span> <span data-ttu-id="cab68-156">El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="cab68-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="cab68-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="cab68-157">ModifiedTime</span></span>     |    <span data-ttu-id="cab68-158">Hora en que se modificó el informe por última vez.</span><span class="sxs-lookup"><span data-stu-id="cab68-158">Time the report was last modified.</span></span> <span data-ttu-id="cab68-159">El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="cab68-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="cab68-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="cab68-160">ExecuteNow</span></span>     |    <span data-ttu-id="cab68-161">Marca ExecuteNow establecida en el momento en que se creó el informe</span><span class="sxs-lookup"><span data-stu-id="cab68-161">ExecuteNow flag set at the time the report was created</span></span>    |
|    <span data-ttu-id="cab68-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="cab68-162">StartTime</span></span>     |    <span data-ttu-id="cab68-163">Hora a la que se iniciará la ejecución del informe.</span><span class="sxs-lookup"><span data-stu-id="cab68-163">Time the report execution will begin.</span></span> <span data-ttu-id="cab68-164">El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="cab68-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="cab68-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="cab68-165">ReportStatus</span></span>     |    <span data-ttu-id="cab68-166">Estado de la ejecución del informe.</span><span class="sxs-lookup"><span data-stu-id="cab68-166">Status of the report execution.</span></span> <span data-ttu-id="cab68-167">Los valores posibles son en pausa, activo e inactivo.</span><span class="sxs-lookup"><span data-stu-id="cab68-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="cab68-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="cab68-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="cab68-169">Intervalo de periodicidad proporcionado durante la creación del informe.</span><span class="sxs-lookup"><span data-stu-id="cab68-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="cab68-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="cab68-170">RecurrenceCount</span></span>     |    <span data-ttu-id="cab68-171">Recuento de periodicidad proporcionado durante la creación del informe.</span><span class="sxs-lookup"><span data-stu-id="cab68-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="cab68-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="cab68-172">CallbackUrl</span></span>     |    <span data-ttu-id="cab68-173">Dirección URL de devolución de llamada proporcionada en la solicitud.</span><span class="sxs-lookup"><span data-stu-id="cab68-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="cab68-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="cab68-174">CallbackMethod</span></span>    |    <span data-ttu-id="cab68-175">Método de devolución de llamada proporcionado en la solicitud</span><span class="sxs-lookup"><span data-stu-id="cab68-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="cab68-176">Formato</span><span class="sxs-lookup"><span data-stu-id="cab68-176">Format</span></span>     |    <span data-ttu-id="cab68-177">Formato de los archivos de informe.</span><span class="sxs-lookup"><span data-stu-id="cab68-177">Format of the report files</span></span>     |
|    <span data-ttu-id="cab68-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="cab68-178">TotalCount</span></span>     |    <span data-ttu-id="cab68-179">Número de conjuntos de datos en la matriz de valores.</span><span class="sxs-lookup"><span data-stu-id="cab68-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="cab68-180">Message</span><span class="sxs-lookup"><span data-stu-id="cab68-180">Message</span></span>     |    <span data-ttu-id="cab68-181">Mensaje de estado de la ejecución de la API.</span><span class="sxs-lookup"><span data-stu-id="cab68-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="cab68-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="cab68-182">StatusCode</span></span>     |    <span data-ttu-id="cab68-183">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="cab68-183">Result Code.</span></span> <span data-ttu-id="cab68-184">Los valores posibles son 200, 400, 401, 403 y 500.</span><span class="sxs-lookup"><span data-stu-id="cab68-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
