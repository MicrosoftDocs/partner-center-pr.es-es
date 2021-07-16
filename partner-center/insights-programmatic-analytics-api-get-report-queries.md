---
title: 'Obtener consultas de informe API: Ideas datos'
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para obtener todas las consultas disponibles para su uso en la API de informe.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376127"
---
# <a name="get-report-queries-api"></a><span data-ttu-id="351ed-103">Obtención de API de consultas de informe</span><span class="sxs-lookup"><span data-stu-id="351ed-103">Get report queries API</span></span>

<span data-ttu-id="351ed-104">La API Get report queries obtiene todas las consultas que están disponibles para su uso en informes.</span><span class="sxs-lookup"><span data-stu-id="351ed-104">The Get report queries API gets all the queries that are available for use in reports.</span></span> <span data-ttu-id="351ed-105">Obtiene todas las consultas del sistema y las definidas por el usuario de forma predeterminada.</span><span class="sxs-lookup"><span data-stu-id="351ed-105">It gets all the system and user-defined queries by default.</span></span>

<span data-ttu-id="351ed-106">**Sintaxis de la solicitud**</span><span class="sxs-lookup"><span data-stu-id="351ed-106">**Request syntax**</span></span>

|    <span data-ttu-id="351ed-107">Método</span><span class="sxs-lookup"><span data-stu-id="351ed-107">Method</span></span>    |    <span data-ttu-id="351ed-108">URI de solicitud</span><span class="sxs-lookup"><span data-stu-id="351ed-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="351ed-109">GET</span><span class="sxs-lookup"><span data-stu-id="351ed-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
|        |        |

<span data-ttu-id="351ed-110">**Encabezado de solicitud**</span><span class="sxs-lookup"><span data-stu-id="351ed-110">**Request header**</span></span>

|    <span data-ttu-id="351ed-111">Encabezado</span><span class="sxs-lookup"><span data-stu-id="351ed-111">Header</span></span>    |    <span data-ttu-id="351ed-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="351ed-112">Type</span></span>    |    <span data-ttu-id="351ed-113">Descripción</span><span class="sxs-lookup"><span data-stu-id="351ed-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="351ed-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="351ed-114">Authorization</span></span>    |    <span data-ttu-id="351ed-115">string</span><span class="sxs-lookup"><span data-stu-id="351ed-115">string</span></span>    |    <span data-ttu-id="351ed-116">Necesario.</span><span class="sxs-lookup"><span data-stu-id="351ed-116">Required.</span></span> <span data-ttu-id="351ed-117">Token Azure Active Directory acceso de Azure Active Directory (AAD) en el formulario`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="351ed-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="351ed-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="351ed-118">Content-Type</span></span>    |    <span data-ttu-id="351ed-119">string</span><span class="sxs-lookup"><span data-stu-id="351ed-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="351ed-120">**Parámetro de ruta de acceso**</span><span class="sxs-lookup"><span data-stu-id="351ed-120">**Path parameter**</span></span>

<span data-ttu-id="351ed-121">Ninguno</span><span class="sxs-lookup"><span data-stu-id="351ed-121">None</span></span>

<span data-ttu-id="351ed-122">**Parámetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="351ed-122">**Query parameter**</span></span>

|    <span data-ttu-id="351ed-123">Nombre de parámetro</span><span class="sxs-lookup"><span data-stu-id="351ed-123">Parameter Name</span></span>    |    <span data-ttu-id="351ed-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="351ed-124">Type</span></span>    |    <span data-ttu-id="351ed-125">Obligatorio</span><span class="sxs-lookup"><span data-stu-id="351ed-125">Required</span></span>    |    <span data-ttu-id="351ed-126">Descripción</span><span class="sxs-lookup"><span data-stu-id="351ed-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="351ed-127">queryId</span><span class="sxs-lookup"><span data-stu-id="351ed-127">queryId</span></span>     |    <span data-ttu-id="351ed-128">string</span><span class="sxs-lookup"><span data-stu-id="351ed-128">string</span></span>     |    <span data-ttu-id="351ed-129">No</span><span class="sxs-lookup"><span data-stu-id="351ed-129">No</span></span>    |    <span data-ttu-id="351ed-130">Filtrar para obtener los detalles de solo las consultas con el id. dado en el argumento</span><span class="sxs-lookup"><span data-stu-id="351ed-130">Filter to get details of only queries with the ID given in the argument</span></span>     |
|    <span data-ttu-id="351ed-131">queryName</span><span class="sxs-lookup"><span data-stu-id="351ed-131">queryName</span></span>     |    <span data-ttu-id="351ed-132">string</span><span class="sxs-lookup"><span data-stu-id="351ed-132">string</span></span>     |    <span data-ttu-id="351ed-133">No</span><span class="sxs-lookup"><span data-stu-id="351ed-133">No</span></span>    |    <span data-ttu-id="351ed-134">Filtrar para obtener los detalles de solo las consultas con el nombre dado en el argumento</span><span class="sxs-lookup"><span data-stu-id="351ed-134">Filter to get details of only queries with the name given in the argument</span></span>     |
|    <span data-ttu-id="351ed-135">IncludeSystemQueries</span><span class="sxs-lookup"><span data-stu-id="351ed-135">IncludeSystemQueries</span></span>     |    <span data-ttu-id="351ed-136">boolean</span><span class="sxs-lookup"><span data-stu-id="351ed-136">boolean</span></span>     |    <span data-ttu-id="351ed-137">No</span><span class="sxs-lookup"><span data-stu-id="351ed-137">No</span></span>    |    <span data-ttu-id="351ed-138">Incluir consultas predefinidas por el sistema en la respuesta</span><span class="sxs-lookup"><span data-stu-id="351ed-138">Include predefined system queries in the response</span></span>     |
|    <span data-ttu-id="351ed-139">IncludeOnlySystemQueries</span><span class="sxs-lookup"><span data-stu-id="351ed-139">IncludeOnlySystemQueries</span></span>     |    <span data-ttu-id="351ed-140">boolean</span><span class="sxs-lookup"><span data-stu-id="351ed-140">boolean</span></span>     |    <span data-ttu-id="351ed-141">No</span><span class="sxs-lookup"><span data-stu-id="351ed-141">No</span></span>    |    <span data-ttu-id="351ed-142">Incluir solo las consultas del sistema en la respuesta</span><span class="sxs-lookup"><span data-stu-id="351ed-142">Include only system queries in the response</span></span>     |
|        |        |        |        |


<span data-ttu-id="351ed-143">**Carga de solicitud**</span><span class="sxs-lookup"><span data-stu-id="351ed-143">**Request payload**</span></span>

<span data-ttu-id="351ed-144">Ninguno</span><span class="sxs-lookup"><span data-stu-id="351ed-144">None</span></span>

<span data-ttu-id="351ed-145">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="351ed-145">**Glossary**</span></span>

<span data-ttu-id="351ed-146">Ninguno</span><span class="sxs-lookup"><span data-stu-id="351ed-146">None</span></span>

<span data-ttu-id="351ed-147">**Respuesta**</span><span class="sxs-lookup"><span data-stu-id="351ed-147">**Response**</span></span>

<span data-ttu-id="351ed-148">La carga de respuesta tiene la estructura siguiente:</span><span class="sxs-lookup"><span data-stu-id="351ed-148">The response payload is structured as follows:</span></span>

<span data-ttu-id="351ed-149">Código de respuesta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="351ed-149">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="351ed-150">Ejemplo de carga de respuesta:</span><span class="sxs-lookup"><span data-stu-id="351ed-150">Response payload example:</span></span>

```json
{ 
  "Value": [ 
    { 
      "QueryId": "string", 
      "Name": "string", 
      "Description": "string", 
      "Query": "string", 
      "Type": "string", 
      "User": "string", 
      "CreatedTime": "string", 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="351ed-151">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="351ed-151">**Glossary**</span></span>

<span data-ttu-id="351ed-152">En esta tabla se definen los elementos clave de la respuesta:</span><span class="sxs-lookup"><span data-stu-id="351ed-152">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="351ed-153">Parámetro</span><span class="sxs-lookup"><span data-stu-id="351ed-153">Parameter</span></span>    |    <span data-ttu-id="351ed-154">Descripción</span><span class="sxs-lookup"><span data-stu-id="351ed-154">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="351ed-155">QueryId</span><span class="sxs-lookup"><span data-stu-id="351ed-155">QueryId</span></span>     |    <span data-ttu-id="351ed-156">UUID único de la consulta.</span><span class="sxs-lookup"><span data-stu-id="351ed-156">Unique UUID of the query</span></span>     |
|    <span data-ttu-id="351ed-157">Nombre</span><span class="sxs-lookup"><span data-stu-id="351ed-157">Name</span></span>     |    <span data-ttu-id="351ed-158">Nombre asignado a la consulta en el momento de la creación de la consulta.</span><span class="sxs-lookup"><span data-stu-id="351ed-158">Name given to the query at the time of query creation</span></span>     |
|    <span data-ttu-id="351ed-159">Descripción</span><span class="sxs-lookup"><span data-stu-id="351ed-159">Description</span></span>     |    <span data-ttu-id="351ed-160">Descripción proporcionada durante la creación de la consulta.</span><span class="sxs-lookup"><span data-stu-id="351ed-160">Description given during creation of the query</span></span>     |
|    <span data-ttu-id="351ed-161">Consultar</span><span class="sxs-lookup"><span data-stu-id="351ed-161">Query</span></span>     |    <span data-ttu-id="351ed-162">Cadena de consulta del informe.</span><span class="sxs-lookup"><span data-stu-id="351ed-162">Report query string</span></span>     |
|    <span data-ttu-id="351ed-163">Tipo</span><span class="sxs-lookup"><span data-stu-id="351ed-163">Type</span></span>     |    <span data-ttu-id="351ed-164">Se establece en userDefined para consultas creadas por el usuario y sistema para consultas predefinidas del sistema</span><span class="sxs-lookup"><span data-stu-id="351ed-164">Set to userDefined for user created queries and system for predefined system queries</span></span>     |
|    <span data-ttu-id="351ed-165">Usuario</span><span class="sxs-lookup"><span data-stu-id="351ed-165">User</span></span>     |    <span data-ttu-id="351ed-166">Id. de usuario que creó la consulta.</span><span class="sxs-lookup"><span data-stu-id="351ed-166">User ID who created the query</span></span>     |
|    <span data-ttu-id="351ed-167">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="351ed-167">CreatedTime</span></span>     |    <span data-ttu-id="351ed-168">Hora de creación de la consulta.</span><span class="sxs-lookup"><span data-stu-id="351ed-168">Time of creation of query</span></span>     |
|    <span data-ttu-id="351ed-169">TotalCount</span><span class="sxs-lookup"><span data-stu-id="351ed-169">TotalCount</span></span>     |    <span data-ttu-id="351ed-170">Número de conjuntos de datos en la matriz de valores.</span><span class="sxs-lookup"><span data-stu-id="351ed-170">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="351ed-171">Message</span><span class="sxs-lookup"><span data-stu-id="351ed-171">Message</span></span>     |    <span data-ttu-id="351ed-172">Mensaje de estado de la ejecución de la API.</span><span class="sxs-lookup"><span data-stu-id="351ed-172">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="351ed-173">StatusCode</span><span class="sxs-lookup"><span data-stu-id="351ed-173">StatusCode</span></span>     |    <span data-ttu-id="351ed-174">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="351ed-174">Result Code.</span></span> <span data-ttu-id="351ed-175">Los valores posibles son 200, 400, 401, 403 y 500.</span><span class="sxs-lookup"><span data-stu-id="351ed-175">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
