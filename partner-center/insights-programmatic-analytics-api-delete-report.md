---
title: 'Eliminación de la API de informe: Ideas datos'
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para eliminar cualquier informe de Centro de partners insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e060104f8f09f69c213ab1b22d4be08d58babced
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376138"
---
# <a name="delete-report-api"></a><span data-ttu-id="a464f-103">Eliminación de API de informe</span><span class="sxs-lookup"><span data-stu-id="a464f-103">Delete report API</span></span>

<span data-ttu-id="a464f-104">En la ejecución, esta API elimina todos los registros de ejecución de informes y de informes.</span><span class="sxs-lookup"><span data-stu-id="a464f-104">On execution, this API deletes all of the report and report execution records.</span></span>

<span data-ttu-id="a464f-105">**Sintaxis de la solicitud**</span><span class="sxs-lookup"><span data-stu-id="a464f-105">**Request syntax**</span></span>

|    <span data-ttu-id="a464f-106">Método</span><span class="sxs-lookup"><span data-stu-id="a464f-106">Method</span></span>    |    <span data-ttu-id="a464f-107">URI de solicitud</span><span class="sxs-lookup"><span data-stu-id="a464f-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="a464f-108">Delete</span><span class="sxs-lookup"><span data-stu-id="a464f-108">DELETE</span></span>    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

<span data-ttu-id="a464f-109">**Encabezado de solicitud**</span><span class="sxs-lookup"><span data-stu-id="a464f-109">**Request header**</span></span>

|    <span data-ttu-id="a464f-110">Encabezado</span><span class="sxs-lookup"><span data-stu-id="a464f-110">Header</span></span>    |    <span data-ttu-id="a464f-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="a464f-111">Type</span></span>    |    <span data-ttu-id="a464f-112">Descripción</span><span class="sxs-lookup"><span data-stu-id="a464f-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="a464f-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="a464f-113">Authorization</span></span>    |    <span data-ttu-id="a464f-114">string</span><span class="sxs-lookup"><span data-stu-id="a464f-114">string</span></span>    |    <span data-ttu-id="a464f-115">Necesario.</span><span class="sxs-lookup"><span data-stu-id="a464f-115">Required.</span></span> <span data-ttu-id="a464f-116">Token Azure Active Directory de acceso de Azure Active Directory (AAD) en el formulario`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="a464f-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="a464f-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a464f-117">Content-Type</span></span>    |    <span data-ttu-id="a464f-118">string</span><span class="sxs-lookup"><span data-stu-id="a464f-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="a464f-119">**Parámetro de ruta de acceso**</span><span class="sxs-lookup"><span data-stu-id="a464f-119">**Path parameter**</span></span>

|    <span data-ttu-id="a464f-120">Nombre de parámetro</span><span class="sxs-lookup"><span data-stu-id="a464f-120">Parameter Name</span></span>    |    <span data-ttu-id="a464f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a464f-121">Type</span></span>    |    <span data-ttu-id="a464f-122">Obligatorio</span><span class="sxs-lookup"><span data-stu-id="a464f-122">Required</span></span>    |    <span data-ttu-id="a464f-123">Descripción</span><span class="sxs-lookup"><span data-stu-id="a464f-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="a464f-124">reportId</span><span class="sxs-lookup"><span data-stu-id="a464f-124">reportId</span></span>     |    <span data-ttu-id="a464f-125">string</span><span class="sxs-lookup"><span data-stu-id="a464f-125">string</span></span>    |    <span data-ttu-id="a464f-126">No</span><span class="sxs-lookup"><span data-stu-id="a464f-126">No</span></span>    |    <span data-ttu-id="a464f-127">Identificador del informe que se va a eliminar</span><span class="sxs-lookup"><span data-stu-id="a464f-127">ID of the report being deleted</span></span>    |
|        |        |        |        |

<span data-ttu-id="a464f-128">**Parámetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="a464f-128">**Query parameter**</span></span>

<span data-ttu-id="a464f-129">Ninguno</span><span class="sxs-lookup"><span data-stu-id="a464f-129">None</span></span>

<span data-ttu-id="a464f-130">**Carga de solicitud**</span><span class="sxs-lookup"><span data-stu-id="a464f-130">**Request payload**</span></span>

<span data-ttu-id="a464f-131">Ninguno</span><span class="sxs-lookup"><span data-stu-id="a464f-131">None</span></span>

<span data-ttu-id="a464f-132">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="a464f-132">**Glossary**</span></span>

<span data-ttu-id="a464f-133">Ninguno</span><span class="sxs-lookup"><span data-stu-id="a464f-133">None</span></span>

<span data-ttu-id="a464f-134">**Respuesta**</span><span class="sxs-lookup"><span data-stu-id="a464f-134">**Response**</span></span>

<span data-ttu-id="a464f-135">La carga de respuesta tiene la estructura siguiente:</span><span class="sxs-lookup"><span data-stu-id="a464f-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="a464f-136">Código de respuesta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="a464f-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="a464f-137">Ejemplo de carga de respuesta:</span><span class="sxs-lookup"><span data-stu-id="a464f-137">Response payload example:</span></span>

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

<span data-ttu-id="a464f-138">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="a464f-138">**Glossary**</span></span>

<span data-ttu-id="a464f-139">En esta tabla se definen los elementos clave de la respuesta:</span><span class="sxs-lookup"><span data-stu-id="a464f-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="a464f-140">Parámetro</span><span class="sxs-lookup"><span data-stu-id="a464f-140">Parameter</span></span>    |    <span data-ttu-id="a464f-141">Descripción</span><span class="sxs-lookup"><span data-stu-id="a464f-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="a464f-142">ReportId</span><span class="sxs-lookup"><span data-stu-id="a464f-142">ReportId</span></span>     |    <span data-ttu-id="a464f-143">Identificador único universal (UUID) del informe eliminado.</span><span class="sxs-lookup"><span data-stu-id="a464f-143">Universally unique identifier (UUID) of the deleted report</span></span>     |
|    <span data-ttu-id="a464f-144">ReportName</span><span class="sxs-lookup"><span data-stu-id="a464f-144">ReportName</span></span>     |    <span data-ttu-id="a464f-145">Nombre dado al informe durante la creación.</span><span class="sxs-lookup"><span data-stu-id="a464f-145">Name given to the report during creation</span></span>     |
|    <span data-ttu-id="a464f-146">Descripción</span><span class="sxs-lookup"><span data-stu-id="a464f-146">Description</span></span>     |    <span data-ttu-id="a464f-147">Descripción proporcionada durante la creación del informe.</span><span class="sxs-lookup"><span data-stu-id="a464f-147">Description given during creation of the report</span></span>     |
|    <span data-ttu-id="a464f-148">QueryId</span><span class="sxs-lookup"><span data-stu-id="a464f-148">QueryId</span></span>     |    <span data-ttu-id="a464f-149">Id. de consulta pasado en el momento en que se creó el informe.</span><span class="sxs-lookup"><span data-stu-id="a464f-149">Query ID passed at the time the report was created</span></span>     |
|    <span data-ttu-id="a464f-150">Consultar</span><span class="sxs-lookup"><span data-stu-id="a464f-150">Query</span></span>     |    <span data-ttu-id="a464f-151">Texto de la consulta que se ejecutará para este informe.</span><span class="sxs-lookup"><span data-stu-id="a464f-151">Query text that will be executed for this report</span></span>     |
|    <span data-ttu-id="a464f-152">Usuario</span><span class="sxs-lookup"><span data-stu-id="a464f-152">User</span></span>     |    <span data-ttu-id="a464f-153">Identificador de usuario usado para crear el informe</span><span class="sxs-lookup"><span data-stu-id="a464f-153">User ID used to create the report</span></span>     |
|    <span data-ttu-id="a464f-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="a464f-154">CreatedTime</span></span>     |    <span data-ttu-id="a464f-155">Hora de creación del informe.</span><span class="sxs-lookup"><span data-stu-id="a464f-155">Time the report was created.</span></span> <span data-ttu-id="a464f-156">El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="a464f-156">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a464f-157">ModifiedTime</span><span class="sxs-lookup"><span data-stu-id="a464f-157">ModifiedTime</span></span>     |    <span data-ttu-id="a464f-158">Hora en que se modificó el informe por última vez.</span><span class="sxs-lookup"><span data-stu-id="a464f-158">Time the report was last modified.</span></span> <span data-ttu-id="a464f-159">El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="a464f-159">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a464f-160">ExecuteNow</span><span class="sxs-lookup"><span data-stu-id="a464f-160">ExecuteNow</span></span>     |    <span data-ttu-id="a464f-161">Marca ExecuteNow establecida en el momento en que se creó el informe</span><span class="sxs-lookup"><span data-stu-id="a464f-161">ExecuteNow flag set at the time the report was created</span></span>     |
|    <span data-ttu-id="a464f-162">StartTime</span><span class="sxs-lookup"><span data-stu-id="a464f-162">StartTime</span></span>     |    <span data-ttu-id="a464f-163">Hora a la que se iniciará la ejecución del informe.</span><span class="sxs-lookup"><span data-stu-id="a464f-163">Time the report execution will begin.</span></span> <span data-ttu-id="a464f-164">El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.</span><span class="sxs-lookup"><span data-stu-id="a464f-164">The time format is yyyy-MM-ddTHH:mm:ssZ</span></span>     |
|    <span data-ttu-id="a464f-165">ReportStatus</span><span class="sxs-lookup"><span data-stu-id="a464f-165">ReportStatus</span></span>     |    <span data-ttu-id="a464f-166">Estado de la ejecución del informe.</span><span class="sxs-lookup"><span data-stu-id="a464f-166">Status of the report execution.</span></span> <span data-ttu-id="a464f-167">Los valores posibles son en pausa, activo e inactivo.</span><span class="sxs-lookup"><span data-stu-id="a464f-167">The possible values are Paused, Active, and Inactive.</span></span>     |
|    <span data-ttu-id="a464f-168">RecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="a464f-168">RecurrenceInterval</span></span>     |    <span data-ttu-id="a464f-169">Intervalo de periodicidad proporcionado durante la creación del informe.</span><span class="sxs-lookup"><span data-stu-id="a464f-169">Recurrence interval provided during report creation</span></span>     |
|    <span data-ttu-id="a464f-170">RecurrenceCount</span><span class="sxs-lookup"><span data-stu-id="a464f-170">RecurrenceCount</span></span>     |    <span data-ttu-id="a464f-171">Recuento de periodicidad proporcionado durante la creación del informe.</span><span class="sxs-lookup"><span data-stu-id="a464f-171">Recurrence count provided during report creation</span></span>     |
|    <span data-ttu-id="a464f-172">CallbackUrl</span><span class="sxs-lookup"><span data-stu-id="a464f-172">CallbackUrl</span></span>     |    <span data-ttu-id="a464f-173">Dirección URL de devolución de llamada proporcionada en la solicitud.</span><span class="sxs-lookup"><span data-stu-id="a464f-173">Callback URL provided in the request</span></span>     |
|    <span data-ttu-id="a464f-174">CallbackMethod</span><span class="sxs-lookup"><span data-stu-id="a464f-174">CallbackMethod</span></span>    |    <span data-ttu-id="a464f-175">Método de devolución de llamada proporcionado en la solicitud</span><span class="sxs-lookup"><span data-stu-id="a464f-175">Callback method provided in the request</span></span>    |
|    <span data-ttu-id="a464f-176">Formato</span><span class="sxs-lookup"><span data-stu-id="a464f-176">Format</span></span>     |    <span data-ttu-id="a464f-177">Formato de los archivos de informe.</span><span class="sxs-lookup"><span data-stu-id="a464f-177">Format of the report files</span></span>     |
|    <span data-ttu-id="a464f-178">TotalCount</span><span class="sxs-lookup"><span data-stu-id="a464f-178">TotalCount</span></span>     |    <span data-ttu-id="a464f-179">Número de conjuntos de datos en la matriz de valores.</span><span class="sxs-lookup"><span data-stu-id="a464f-179">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="a464f-180">Message</span><span class="sxs-lookup"><span data-stu-id="a464f-180">Message</span></span>     |    <span data-ttu-id="a464f-181">Mensaje de estado de la ejecución de la API.</span><span class="sxs-lookup"><span data-stu-id="a464f-181">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="a464f-182">StatusCode</span><span class="sxs-lookup"><span data-stu-id="a464f-182">StatusCode</span></span>     |    <span data-ttu-id="a464f-183">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="a464f-183">Result Code.</span></span> <span data-ttu-id="a464f-184">Los valores posibles son 200, 400, 401, 403 y 500.</span><span class="sxs-lookup"><span data-stu-id="a464f-184">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
