---
title: 'Obtener todos los conjuntos de datos API: Ideas datos'
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para obtener detalles de todos los conjuntos de datos disponibles en Centro de partners insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 42ff7cc1f097e2423be5f1f7f9a7f62214d64949
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375871"
---
# <a name="get-all-datasets-api"></a><span data-ttu-id="63d5c-103">API de obtención de todos los conjuntos de datos</span><span class="sxs-lookup"><span data-stu-id="63d5c-103">Get all datasets API</span></span>

<span data-ttu-id="63d5c-104">La API Get all datasets obtiene todos los conjuntos de datos disponibles.</span><span class="sxs-lookup"><span data-stu-id="63d5c-104">The Get all datasets API gets all the available datasets.</span></span> <span data-ttu-id="63d5c-105">Los conjuntos de datos muestran las tablas, las columnas, las métricas y los intervalos de tiempo.</span><span class="sxs-lookup"><span data-stu-id="63d5c-105">Datasets list the tables, columns, metrics, and time ranges.</span></span>

<span data-ttu-id="63d5c-106">**Sintaxis de la solicitud**</span><span class="sxs-lookup"><span data-stu-id="63d5c-106">**Request syntax**</span></span>

|    <span data-ttu-id="63d5c-107">Método</span><span class="sxs-lookup"><span data-stu-id="63d5c-107">Method</span></span>    |    <span data-ttu-id="63d5c-108">URI de solicitud</span><span class="sxs-lookup"><span data-stu-id="63d5c-108">Request URI</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="63d5c-109">GET</span><span class="sxs-lookup"><span data-stu-id="63d5c-109">GET</span></span>    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledDataset?datasetName={Dataset Name}`     |
|        |        |

<span data-ttu-id="63d5c-110">**Encabezado de solicitud**</span><span class="sxs-lookup"><span data-stu-id="63d5c-110">**Request header**</span></span>

|    <span data-ttu-id="63d5c-111">Encabezado</span><span class="sxs-lookup"><span data-stu-id="63d5c-111">Header</span></span>    |    <span data-ttu-id="63d5c-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="63d5c-112">Type</span></span>    |    <span data-ttu-id="63d5c-113">Descripción</span><span class="sxs-lookup"><span data-stu-id="63d5c-113">Description</span></span>    |
|    ----    |    ----    |    ----    |
|    <span data-ttu-id="63d5c-114">Authorization</span><span class="sxs-lookup"><span data-stu-id="63d5c-114">Authorization</span></span>    |    <span data-ttu-id="63d5c-115">string</span><span class="sxs-lookup"><span data-stu-id="63d5c-115">string</span></span>    |    <span data-ttu-id="63d5c-116">Necesario.</span><span class="sxs-lookup"><span data-stu-id="63d5c-116">Required.</span></span> <span data-ttu-id="63d5c-117">Token Azure Active Directory acceso de Azure Active Directory (AAD) en el formulario`Bearer <token>`</span><span class="sxs-lookup"><span data-stu-id="63d5c-117">The Azure Active Directory (AAD) access token in the form `Bearer <token>`</span></span>    |
|    <span data-ttu-id="63d5c-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="63d5c-118">Content-Type</span></span>    |    <span data-ttu-id="63d5c-119">string</span><span class="sxs-lookup"><span data-stu-id="63d5c-119">string</span></span>    |    `Application/JSON`    |
|        |        |        |

<span data-ttu-id="63d5c-120">**Parámetro de ruta de acceso**</span><span class="sxs-lookup"><span data-stu-id="63d5c-120">**Path parameter**</span></span>

<span data-ttu-id="63d5c-121">Ninguno</span><span class="sxs-lookup"><span data-stu-id="63d5c-121">None</span></span>

<span data-ttu-id="63d5c-122">**Parámetro de consulta**</span><span class="sxs-lookup"><span data-stu-id="63d5c-122">**Query parameter**</span></span>

|    <span data-ttu-id="63d5c-123">Nombre de parámetro</span><span class="sxs-lookup"><span data-stu-id="63d5c-123">Parameter Name</span></span>    |    <span data-ttu-id="63d5c-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="63d5c-124">Type</span></span>    |    <span data-ttu-id="63d5c-125">Obligatorio</span><span class="sxs-lookup"><span data-stu-id="63d5c-125">Required</span></span>    |    <span data-ttu-id="63d5c-126">Descripción</span><span class="sxs-lookup"><span data-stu-id="63d5c-126">Description</span></span>    |
|    ----    |    ----    |    ----    |    ----    |
|    <span data-ttu-id="63d5c-127">datasetName</span><span class="sxs-lookup"><span data-stu-id="63d5c-127">datasetName</span></span>    |    <span data-ttu-id="63d5c-128">string</span><span class="sxs-lookup"><span data-stu-id="63d5c-128">string</span></span>    |    <span data-ttu-id="63d5c-129">No</span><span class="sxs-lookup"><span data-stu-id="63d5c-129">No</span></span>    |    <span data-ttu-id="63d5c-130">Filtro para obtener detalles de un solo conjunto de datos</span><span class="sxs-lookup"><span data-stu-id="63d5c-130">Filter to get details of only one dataset</span></span>    |
|        |        |        |        |

<span data-ttu-id="63d5c-131">**Carga de solicitud**</span><span class="sxs-lookup"><span data-stu-id="63d5c-131">**Request payload**</span></span>

<span data-ttu-id="63d5c-132">Ninguno</span><span class="sxs-lookup"><span data-stu-id="63d5c-132">None</span></span>

<span data-ttu-id="63d5c-133">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="63d5c-133">**Glossary**</span></span>

<span data-ttu-id="63d5c-134">Ninguno</span><span class="sxs-lookup"><span data-stu-id="63d5c-134">None</span></span>

<span data-ttu-id="63d5c-135">**Respuesta**</span><span class="sxs-lookup"><span data-stu-id="63d5c-135">**Response**</span></span>

<span data-ttu-id="63d5c-136">La carga de respuesta tiene la estructura siguiente:</span><span class="sxs-lookup"><span data-stu-id="63d5c-136">The response payload is structured as follows:</span></span>

<span data-ttu-id="63d5c-137">Código de respuesta: 200, 400, 401, 403, 404, 500</span><span class="sxs-lookup"><span data-stu-id="63d5c-137">Response code: 200, 400, 401, 403, 404, 500</span></span>

<span data-ttu-id="63d5c-138">Ejemplo de carga de respuesta:</span><span class="sxs-lookup"><span data-stu-id="63d5c-138">Response payload example:</span></span>

```json
{ 
   "Value":[ 
      { 
         "DatasetName ":"string", 
         "SelectableColumns":[ 
            "string" 
         ], 
         "AvailableMetrics":[ 
            "string" 
         ], 
         "AvailableDateRanges":[ 
            "string" 
         ], 
         "minimumRecurrenceInterval":0 
      } 
   ], 
   "TotalCount":0, 
   "Message":"<Error Message>", 
   "StatusCode": 0, 
} 
```

<span data-ttu-id="63d5c-139">**Glosario**</span><span class="sxs-lookup"><span data-stu-id="63d5c-139">**Glossary**</span></span>

<span data-ttu-id="63d5c-140">En esta tabla se definen los elementos clave de la respuesta:</span><span class="sxs-lookup"><span data-stu-id="63d5c-140">This table defines the key elements in the response:</span></span>

|    <span data-ttu-id="63d5c-141">Parámetro</span><span class="sxs-lookup"><span data-stu-id="63d5c-141">Parameter</span></span>    |    <span data-ttu-id="63d5c-142">Descripción</span><span class="sxs-lookup"><span data-stu-id="63d5c-142">Description</span></span>    |
|    ----    |    ----    |
|    <span data-ttu-id="63d5c-143">DatasetName</span><span class="sxs-lookup"><span data-stu-id="63d5c-143">DatasetName</span></span>     |    <span data-ttu-id="63d5c-144">Nombre del conjunto de datos que define este objeto de matriz.</span><span class="sxs-lookup"><span data-stu-id="63d5c-144">Name of the dataset that this array object defines</span></span>     |
|    <span data-ttu-id="63d5c-145">SelectableColumns</span><span class="sxs-lookup"><span data-stu-id="63d5c-145">SelectableColumns</span></span>     |    <span data-ttu-id="63d5c-146">Columnas sin procesar que se pueden especificar en las columnas de selección.</span><span class="sxs-lookup"><span data-stu-id="63d5c-146">Raw columns that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="63d5c-147">AvailableMetrics</span><span class="sxs-lookup"><span data-stu-id="63d5c-147">AvailableMetrics</span></span>     |    <span data-ttu-id="63d5c-148">Nombres de columna de agregación/métrica que se pueden especificar en las columnas de selección.</span><span class="sxs-lookup"><span data-stu-id="63d5c-148">Aggregation/metric column names that can be specified in the select columns</span></span>     |
|    <span data-ttu-id="63d5c-149">AvailableDateRanges</span><span class="sxs-lookup"><span data-stu-id="63d5c-149">AvailableDateRanges</span></span>     |    <span data-ttu-id="63d5c-150">Intervalo de fechas que se puede usar en las consultas de informe para el conjunto de datos.</span><span class="sxs-lookup"><span data-stu-id="63d5c-150">Date range that can be used in report queries for the dataset</span></span>     |
|    <span data-ttu-id="63d5c-151">minimumRecurrenceInterval</span><span class="sxs-lookup"><span data-stu-id="63d5c-151">minimumRecurrenceInterval</span></span>     |    <span data-ttu-id="63d5c-152">Valor mínimo de Intervalo de periodicidad</span><span class="sxs-lookup"><span data-stu-id="63d5c-152">Minimum value of Recurrence Interval</span></span>     |
|    <span data-ttu-id="63d5c-153">TotalCount</span><span class="sxs-lookup"><span data-stu-id="63d5c-153">TotalCount</span></span>     |    <span data-ttu-id="63d5c-154">Número de conjuntos de datos en la matriz de valores.</span><span class="sxs-lookup"><span data-stu-id="63d5c-154">Number of datasets in the Value array</span></span>     |
|    <span data-ttu-id="63d5c-155">Message</span><span class="sxs-lookup"><span data-stu-id="63d5c-155">Message</span></span>     |    <span data-ttu-id="63d5c-156">Mensaje de estado de la ejecución de la API.</span><span class="sxs-lookup"><span data-stu-id="63d5c-156">Status message from the execution of the API</span></span>     |
|    <span data-ttu-id="63d5c-157">StatusCode</span><span class="sxs-lookup"><span data-stu-id="63d5c-157">StatusCode</span></span>     |    <span data-ttu-id="63d5c-158">Código de resultado.</span><span class="sxs-lookup"><span data-stu-id="63d5c-158">Result Code.</span></span> <span data-ttu-id="63d5c-159">Los valores posibles son 200, 400, 401, 403 y 500.</span><span class="sxs-lookup"><span data-stu-id="63d5c-159">The possible values are 200, 400, 401, 403, 500</span></span>     |
|        |        |
