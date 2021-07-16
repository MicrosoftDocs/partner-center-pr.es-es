---
title: 'Api de eliminación de consultas de informes: Ideas datos'
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para eliminar la consulta definida por el usuario en Centro de partners insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: e608068613edad1fca277ba5886c9c4bc962ffd2
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375884"
---
# <a name="delete-report-queries-api"></a><span data-ttu-id="fcd9e-103">Eliminación de API de consultas de informe</span><span class="sxs-lookup"><span data-stu-id="fcd9e-103">Delete report queries API</span></span>

<span data-ttu-id="fcd9e-104">Esta API elimina consultas definidas por el usuario.</span><span class="sxs-lookup"><span data-stu-id="fcd9e-104">This API deletes user-defined queries.</span></span>

<span data-ttu-id="fcd9e-105">**Sintaxis de la solicitud**</span><span class="sxs-lookup"><span data-stu-id="fcd9e-105">**Request syntax**</span></span>

|    <span data-ttu-id="fcd9e-106">Método</span><span class="sxs-lookup"><span data-stu-id="fcd9e-106">Method</span></span>    |    <span data-ttu-id="fcd9e-107">URI de solicitud</span><span class="sxs-lookup"><span data-stu-id="fcd9e-107">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="fcd9e-108">Delete</span><span class="sxs-lookup"><span data-stu-id="fcd9e-108">DELETE</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

<span data-ttu-id="fcd9e-109">**Encabezado de solicitud**</span><span class="sxs-lookup"><span data-stu-id="fcd9e-109">**Request header**</span></span>

|    <span data-ttu-id="fcd9e-110">Encabezado</span><span class="sxs-lookup"><span data-stu-id="fcd9e-110">Header</span></span>    |    <span data-ttu-id="fcd9e-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcd9e-111">Type</span></span>    |    <span data-ttu-id="fcd9e-112">Descripción</span><span class="sxs-lookup"><span data-stu-id="fcd9e-112">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="fcd9e-113">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcd9e-113">Authorization</span></span>    |    <span data-ttu-id="fcd9e-114">string</span><span class="sxs-lookup"><span data-stu-id="fcd9e-114">string</span></span>    |    <span data-ttu-id="fcd9e-115">Necesario.</span><span class="sxs-lookup"><span data-stu-id="fcd9e-115">Required.</span></span> <span data-ttu-id="fcd9e-116">Token Azure Active Directory acceso de Azure Active Directory (AAD) en el formulario`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="fcd9e-116">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="fcd9e-117">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fcd9e-117">Content-Type</span></span>    |    <span data-ttu-id="fcd9e-118">string</span><span class="sxs-lookup"><span data-stu-id="fcd9e-118">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="fcd9e-119">**Parámetro de ruta de acceso**</span><span class="sxs-lookup"><span data-stu-id="fcd9e-119">**Path parameter**</span></span>

|    <span data-ttu-id="fcd9e-120">Nombre de parámetro</span><span class="sxs-lookup"><span data-stu-id="fcd9e-120">Parameter Name</span></span>    |    <span data-ttu-id="fcd9e-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcd9e-121">Type</span></span>    |    <span data-ttu-id="fcd9e-122">Obligatorio</span><span class="sxs-lookup"><span data-stu-id="fcd9e-122">Required</span></span>    |    <span data-ttu-id="fcd9e-123">Descripción</span><span class="sxs-lookup"><span data-stu-id="fcd9e-123">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="fcd9e-124">queryId</span><span class="sxs-lookup"><span data-stu-id="fcd9e-124">queryId</span></span>     |    <span data-ttu-id="fcd9e-125">string</span><span class="sxs-lookup"><span data-stu-id="fcd9e-125">string</span></span>     |    <span data-ttu-id="fcd9e-126">No</span><span class="sxs-lookup"><span data-stu-id="fcd9e-126">No</span></span>    |    <span data-ttu-id="fcd9e-127">Filtrar para obtener los detalles de solo las consultas con el id. dado en el argumento</span><span class="sxs-lookup"><span data-stu-id="fcd9e-127">Filter to get details of only queries with the ID given in the argument</span></span>     |
|        |        |        |        |

<span data-ttu-id="fcd9e-128">**Parámetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="fcd9e-128">**Query parameter**</span></span>

<span data-ttu-id="fcd9e-129">Ninguno</span><span class="sxs-lookup"><span data-stu-id="fcd9e-129">None</span></span>

<span data-ttu-id="fcd9e-130">**Carga de solicitud**</span><span class="sxs-lookup"><span data-stu-id="fcd9e-130">**Request payload**</span></span>

<span data-ttu-id="fcd9e-131">Ninguno</span><span class="sxs-lookup"><span data-stu-id="fcd9e-131">None</span></span>

<span data-ttu-id="fcd9e-132">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="fcd9e-132">**Glossary**</span></span>

<span data-ttu-id="fcd9e-133">Ninguno</span><span class="sxs-lookup"><span data-stu-id="fcd9e-133">None</span></span>

<span data-ttu-id="fcd9e-134">**Respuesta**</span><span class="sxs-lookup"><span data-stu-id="fcd9e-134">**Response**</span></span>

<span data-ttu-id="fcd9e-135">La carga de respuesta tiene la estructura siguiente:</span><span class="sxs-lookup"><span data-stu-id="fcd9e-135">The response payload is structured as follows:</span></span>

<span data-ttu-id="fcd9e-136">Código de respuesta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="fcd9e-136">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="fcd9e-137">Ejemplo de carga de respuesta:</span><span class="sxs-lookup"><span data-stu-id="fcd9e-137">Response payload example:</span></span>

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

<span data-ttu-id="fcd9e-138">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="fcd9e-138">**Glossary**</span></span>

<span data-ttu-id="fcd9e-139">En esta tabla se definen los elementos clave de la respuesta:</span><span class="sxs-lookup"><span data-stu-id="fcd9e-139">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="fcd9e-140">Parámetro</span><span class="sxs-lookup"><span data-stu-id="fcd9e-140">Parameter</span></span>    |    <span data-ttu-id="fcd9e-141">Descripción</span><span class="sxs-lookup"><span data-stu-id="fcd9e-141">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="fcd9e-142">QueryId</span><span class="sxs-lookup"><span data-stu-id="fcd9e-142">QueryId</span></span>     |    <span data-ttu-id="fcd9e-143">UUID único de la consulta que se eliminó</span><span class="sxs-lookup"><span data-stu-id="fcd9e-143">Unique UUID of the query that was deleted</span></span>    |
|    <span data-ttu-id="fcd9e-144">Nombre</span><span class="sxs-lookup"><span data-stu-id="fcd9e-144">Name</span></span>     |    <span data-ttu-id="fcd9e-145">Nombre de la consulta eliminada.</span><span class="sxs-lookup"><span data-stu-id="fcd9e-145">Name of the query that was deleted</span></span>    |
|    <span data-ttu-id="fcd9e-146">Descripción</span><span class="sxs-lookup"><span data-stu-id="fcd9e-146">Description</span></span>     |    <span data-ttu-id="fcd9e-147">Descripción de la consulta eliminada.</span><span class="sxs-lookup"><span data-stu-id="fcd9e-147">Description of the deleted query</span></span>     |
|    <span data-ttu-id="fcd9e-148">Consultar</span><span class="sxs-lookup"><span data-stu-id="fcd9e-148">Query</span></span>     |    <span data-ttu-id="fcd9e-149">Cadena de consulta de informe de la consulta eliminada.</span><span class="sxs-lookup"><span data-stu-id="fcd9e-149">Report query string of the deleted query</span></span>    |
|    <span data-ttu-id="fcd9e-150">Tipo</span><span class="sxs-lookup"><span data-stu-id="fcd9e-150">Type</span></span>     |    <span data-ttu-id="fcd9e-151">Establezca en userDefined para las consultas creadas por el usuario.</span><span class="sxs-lookup"><span data-stu-id="fcd9e-151">Set to userDefined for user created queries</span></span>     |
|    <span data-ttu-id="fcd9e-152">Usuario</span><span class="sxs-lookup"><span data-stu-id="fcd9e-152">User</span></span>     |    <span data-ttu-id="fcd9e-153">Id. de usuario que creó la consulta.</span><span class="sxs-lookup"><span data-stu-id="fcd9e-153">User ID who created the query</span></span>     |
|    <span data-ttu-id="fcd9e-154">CreatedTime</span><span class="sxs-lookup"><span data-stu-id="fcd9e-154">CreatedTime</span></span>     |    <span data-ttu-id="fcd9e-155">Hora de creación de la consulta.</span><span class="sxs-lookup"><span data-stu-id="fcd9e-155">Time of creation of query</span></span>     |
|    <span data-ttu-id="fcd9e-156">TotalCount</span><span class="sxs-lookup"><span data-stu-id="fcd9e-156">TotalCount</span></span>     |    <span data-ttu-id="fcd9e-157">Número de conjuntos de datos en la matriz de valores.</span><span class="sxs-lookup"><span data-stu-id="fcd9e-157">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="fcd9e-158">Message</span><span class="sxs-lookup"><span data-stu-id="fcd9e-158">Message</span></span>     |    <span data-ttu-id="fcd9e-159">Mensaje de estado de la ejecución de la API.</span><span class="sxs-lookup"><span data-stu-id="fcd9e-159">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="fcd9e-160">StatusCode</span><span class="sxs-lookup"><span data-stu-id="fcd9e-160">StatusCode</span></span>     |    <span data-ttu-id="fcd9e-161">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="fcd9e-161">Result Code.</span></span> <span data-ttu-id="fcd9e-162">Los valores posibles son 200, 400, 401, 403 y 500.</span><span class="sxs-lookup"><span data-stu-id="fcd9e-162">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
