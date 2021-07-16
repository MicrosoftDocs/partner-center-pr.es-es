---
title: Prueba de la API de consultas de informe
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para probar la consulta y validar los resultados en Centro de partners insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 13ad6fe385a4d31390b6806d863da3f647105b2c
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376095"
---
# <a name="try-report-queries-api"></a><span data-ttu-id="97e4c-103">Prueba de la API de consultas de informe</span><span class="sxs-lookup"><span data-stu-id="97e4c-103">Try report queries API</span></span>

<span data-ttu-id="97e4c-104">Esta API ejecuta una instrucción de consulta de informe.</span><span class="sxs-lookup"><span data-stu-id="97e4c-104">This API executes a Report query statement.</span></span> <span data-ttu-id="97e4c-105">La API devuelve solo 100 registros que usted como asociado puede usar para comprobar si los datos son los esperados.</span><span class="sxs-lookup"><span data-stu-id="97e4c-105">The API returns only 100 records that you as a partner can use to verify if the data is as you expected.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="97e4c-106">Esta API tiene un tiempo de espera de ejecución de consulta de 100 segundos.</span><span class="sxs-lookup"><span data-stu-id="97e4c-106">This API has a query execution timeout of 100 seconds.</span></span> <span data-ttu-id="97e4c-107">Si observa que la API tarda más, es muy probable que la consulta sea sintácticamente correcta o que haya recibido un código de error distinto de 200.</span><span class="sxs-lookup"><span data-stu-id="97e4c-107">If you notice the API is taking more than 100 seconds, it is highly likely that the query is syntactically correct or else you would have received an error code other than 200.</span></span> <span data-ttu-id="97e4c-108">La generación del informe real sucederá si la sintaxis de la consulta es correcta.</span><span class="sxs-lookup"><span data-stu-id="97e4c-108">The actual report generation will pass if the query syntax is correct.</span></span>

<span data-ttu-id="97e4c-109">**Sintaxis de la solicitud**</span><span class="sxs-lookup"><span data-stu-id="97e4c-109">**Request syntax**</span></span>

|    <span data-ttu-id="97e4c-110">Método</span><span class="sxs-lookup"><span data-stu-id="97e4c-110">Method</span></span>    |    <span data-ttu-id="97e4c-111">URI de solicitud</span><span class="sxs-lookup"><span data-stu-id="97e4c-111">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="97e4c-112">GET</span><span class="sxs-lookup"><span data-stu-id="97e4c-112">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

<span data-ttu-id="97e4c-113">**Encabezado de solicitud**</span><span class="sxs-lookup"><span data-stu-id="97e4c-113">**Request header**</span></span>

|    <span data-ttu-id="97e4c-114">Encabezado</span><span class="sxs-lookup"><span data-stu-id="97e4c-114">Header</span></span>    |    <span data-ttu-id="97e4c-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="97e4c-115">Type</span></span>    |    <span data-ttu-id="97e4c-116">Descripción</span><span class="sxs-lookup"><span data-stu-id="97e4c-116">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="97e4c-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="97e4c-117">Authorization</span></span>    |    <span data-ttu-id="97e4c-118">string</span><span class="sxs-lookup"><span data-stu-id="97e4c-118">string</span></span>    |    <span data-ttu-id="97e4c-119">Necesario.</span><span class="sxs-lookup"><span data-stu-id="97e4c-119">Required.</span></span> <span data-ttu-id="97e4c-120">Token Azure Active Directory acceso de Azure Active Directory (AAD) en el formulario`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="97e4c-120">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="97e4c-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="97e4c-121">Content-Type</span></span>    |    <span data-ttu-id="97e4c-122">string</span><span class="sxs-lookup"><span data-stu-id="97e4c-122">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="97e4c-123">**Parámetro de ruta de acceso**</span><span class="sxs-lookup"><span data-stu-id="97e4c-123">**Path parameter**</span></span>

<span data-ttu-id="97e4c-124">Ninguno</span><span class="sxs-lookup"><span data-stu-id="97e4c-124">None</span></span>

<span data-ttu-id="97e4c-125">**Parámetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="97e4c-125">**Query parameter**</span></span>

|    <span data-ttu-id="97e4c-126">Nombre de parámetro</span><span class="sxs-lookup"><span data-stu-id="97e4c-126">Parameter Name</span></span>    |    <span data-ttu-id="97e4c-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="97e4c-127">Type</span></span>    |    <span data-ttu-id="97e4c-128">Obligatorio</span><span class="sxs-lookup"><span data-stu-id="97e4c-128">Required</span></span>    |    <span data-ttu-id="97e4c-129">Descripción</span><span class="sxs-lookup"><span data-stu-id="97e4c-129">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="97e4c-130">exportQuery</span><span class="sxs-lookup"><span data-stu-id="97e4c-130">exportQuery</span></span>     |    <span data-ttu-id="97e4c-131">string</span><span class="sxs-lookup"><span data-stu-id="97e4c-131">string</span></span>    |    <span data-ttu-id="97e4c-132">No</span><span class="sxs-lookup"><span data-stu-id="97e4c-132">No</span></span>    |    <span data-ttu-id="97e4c-133">Cadena de consulta de informe que se debe ejecutar</span><span class="sxs-lookup"><span data-stu-id="97e4c-133">Report query string that needs to be executed</span></span>     |
|    <span data-ttu-id="97e4c-134">queryId</span><span class="sxs-lookup"><span data-stu-id="97e4c-134">queryId</span></span>     |    <span data-ttu-id="97e4c-135">string</span><span class="sxs-lookup"><span data-stu-id="97e4c-135">string</span></span>    |    <span data-ttu-id="97e4c-136">No</span><span class="sxs-lookup"><span data-stu-id="97e4c-136">No</span></span>    |    <span data-ttu-id="97e4c-137">Identificador de consulta existente válido.</span><span class="sxs-lookup"><span data-stu-id="97e4c-137">A valid existing query ID.</span></span> <span data-ttu-id="97e4c-138">Mutuamente excluyente con la cadena de consulta especificada en el parámetro exportQuery</span><span class="sxs-lookup"><span data-stu-id="97e4c-138">Mutually exclusive with query string specified in exportQuery parameter</span></span>    |
|    <span data-ttu-id="97e4c-139">startTime</span><span class="sxs-lookup"><span data-stu-id="97e4c-139">startTime</span></span>     |    <span data-ttu-id="97e4c-140">string</span><span class="sxs-lookup"><span data-stu-id="97e4c-140">string</span></span>    |    <span data-ttu-id="97e4c-141">No</span><span class="sxs-lookup"><span data-stu-id="97e4c-141">No</span></span>    |    <span data-ttu-id="97e4c-142">Hora de inicio desde la que queremos los datos.</span><span class="sxs-lookup"><span data-stu-id="97e4c-142">Start time from which we want the data.</span></span> <span data-ttu-id="97e4c-143">Invalida el intervalo de tiempo especificado en la consulta.</span><span class="sxs-lookup"><span data-stu-id="97e4c-143">It overrides timespan specified in the query</span></span>    |
|    <span data-ttu-id="97e4c-144">endTime</span><span class="sxs-lookup"><span data-stu-id="97e4c-144">endTime</span></span>     |    <span data-ttu-id="97e4c-145">string</span><span class="sxs-lookup"><span data-stu-id="97e4c-145">string</span></span>    |    <span data-ttu-id="97e4c-146">No</span><span class="sxs-lookup"><span data-stu-id="97e4c-146">No</span></span>    |    <span data-ttu-id="97e4c-147">Hora de finalización hasta la que queremos los datos.</span><span class="sxs-lookup"><span data-stu-id="97e4c-147">End time till which we want the data.</span></span> <span data-ttu-id="97e4c-148">Invalida el intervalo de tiempo especificado en la consulta.</span><span class="sxs-lookup"><span data-stu-id="97e4c-148">It overrides timespan specified in the query</span></span>    |
|        |        |        |        |

<span data-ttu-id="97e4c-149">**Carga de solicitud**</span><span class="sxs-lookup"><span data-stu-id="97e4c-149">**Request payload**</span></span>

<span data-ttu-id="97e4c-150">Ninguno</span><span class="sxs-lookup"><span data-stu-id="97e4c-150">None</span></span>

<span data-ttu-id="97e4c-151">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="97e4c-151">**Glossary**</span></span>

<span data-ttu-id="97e4c-152">Ninguno</span><span class="sxs-lookup"><span data-stu-id="97e4c-152">None</span></span>

<span data-ttu-id="97e4c-153">**Respuesta**</span><span class="sxs-lookup"><span data-stu-id="97e4c-153">**Response**</span></span>

<span data-ttu-id="97e4c-154">La carga de respuesta tiene la estructura siguiente:</span><span class="sxs-lookup"><span data-stu-id="97e4c-154">The response payload is structured as follows:</span></span>

<span data-ttu-id="97e4c-155">Código de respuesta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="97e4c-155">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="97e4c-156">Ejemplo de carga de respuesta:</span><span class="sxs-lookup"><span data-stu-id="97e4c-156">Response payload example:</span></span>

```json
Top 100 rows of query execution 
{ 
  "Value": [ 
    { 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0, 
} 
```

<span data-ttu-id="97e4c-157">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="97e4c-157">**Glossary**</span></span>

<span data-ttu-id="97e4c-158">En esta tabla se definen los elementos clave de la respuesta:</span><span class="sxs-lookup"><span data-stu-id="97e4c-158">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="97e4c-159">Parámetro</span><span class="sxs-lookup"><span data-stu-id="97e4c-159">Parameter</span></span>    |    <span data-ttu-id="97e4c-160">Descripción</span><span class="sxs-lookup"><span data-stu-id="97e4c-160">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="97e4c-161">TotalCount</span><span class="sxs-lookup"><span data-stu-id="97e4c-161">TotalCount</span></span>     |    <span data-ttu-id="97e4c-162">Número de conjuntos de datos en la matriz de valores.</span><span class="sxs-lookup"><span data-stu-id="97e4c-162">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="97e4c-163">Message</span><span class="sxs-lookup"><span data-stu-id="97e4c-163">Message</span></span>     |    <span data-ttu-id="97e4c-164">Mensaje de estado de la ejecución de la API.</span><span class="sxs-lookup"><span data-stu-id="97e4c-164">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="97e4c-165">StatusCode</span><span class="sxs-lookup"><span data-stu-id="97e4c-165">StatusCode</span></span>     |    <span data-ttu-id="97e4c-166">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="97e4c-166">Result Code.</span></span> <span data-ttu-id="97e4c-167">Los valores posibles son 200, 400, 401, 403 y 500.</span><span class="sxs-lookup"><span data-stu-id="97e4c-167">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
