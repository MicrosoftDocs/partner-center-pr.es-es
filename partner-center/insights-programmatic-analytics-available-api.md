---
title: Lista de API para acceder a los datos de Conclusiones de asociados
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Lista de API para acceder a los datos de conclusiones de asociados.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 71d04b6927e27b1d7a8d72bbdaa56b41cb113625
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376079"
---
# <a name="available-apis-for-partner-insights-analytics"></a><span data-ttu-id="96767-103">API disponibles para el análisis de Conclusiones de asociados</span><span class="sxs-lookup"><span data-stu-id="96767-103">Available APIs for partner insights analytics</span></span>

<span data-ttu-id="96767-104">A continuación se muestra la lista de API para el análisis de conclusiones de asociados y sus funcionalidades asociadas.</span><span class="sxs-lookup"><span data-stu-id="96767-104">Following are the list of APIs for partner insights analytics and their associated functionalities.</span></span>

## <a name="dataset-pull-apis"></a><span data-ttu-id="96767-105">API de extracción de conjuntos de datos</span><span class="sxs-lookup"><span data-stu-id="96767-105">Dataset pull APIs</span></span>

<span data-ttu-id="96767-106">***Tabla 1: API de extracción de conjuntos de datos***</span><span class="sxs-lookup"><span data-stu-id="96767-106">***Table 1: Dataset pull APIs***</span></span>

| <span data-ttu-id="96767-107">**API**</span><span class="sxs-lookup"><span data-stu-id="96767-107">**API**</span></span> | <span data-ttu-id="96767-108">**Funcionalidad**</span><span class="sxs-lookup"><span data-stu-id="96767-108">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="96767-109">Obtener todos los conjuntos de datos</span><span class="sxs-lookup"><span data-stu-id="96767-109">Get all datasets</span></span>](insights-programmatic-analytics-api-get-dataset.md) | <span data-ttu-id="96767-110">Obtiene todos los conjuntos de datos disponibles.</span><span class="sxs-lookup"><span data-stu-id="96767-110">Gets all the available datasets.</span></span> <span data-ttu-id="96767-111">Los conjuntos de datos muestran las tablas, las columnas, las métricas y los intervalos de tiempo.</span><span class="sxs-lookup"><span data-stu-id="96767-111">Datasets list the tables, columns, metrics, and time ranges.</span></span> |
|||

## <a name="query-management-apis"></a><span data-ttu-id="96767-112">API de administración de consultas</span><span class="sxs-lookup"><span data-stu-id="96767-112">Query management APIs</span></span>

<span data-ttu-id="96767-113">***Tabla 2: API de administración de consultas***</span><span class="sxs-lookup"><span data-stu-id="96767-113">***Table 2: Query management APIs***</span></span>

| <span data-ttu-id="96767-114">**API**</span><span class="sxs-lookup"><span data-stu-id="96767-114">**API**</span></span> | <span data-ttu-id="96767-115">**Funcionalidad**</span><span class="sxs-lookup"><span data-stu-id="96767-115">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="96767-116">Creación de consultas de informes</span><span class="sxs-lookup"><span data-stu-id="96767-116">Create Report Query</span></span>](insights-programmatic-access-paradigm.md#create-report-query-api) | <span data-ttu-id="96767-117">Crea consultas personalizadas que definen el conjunto de datos del que deben exportarse las columnas y métricas.</span><span class="sxs-lookup"><span data-stu-id="96767-117">Creates custom queries that define the dataset from which columns and metrics need to be exported.</span></span> |
| [<span data-ttu-id="96767-118">GET Report Query</span><span class="sxs-lookup"><span data-stu-id="96767-118">GET Report Query</span></span>](insights-programmatic-analytics-api-get-report-queries.md) | <span data-ttu-id="96767-119">Obtiene todas las consultas disponibles para su uso en informes.</span><span class="sxs-lookup"><span data-stu-id="96767-119">Gets all the queries available for use in reports.</span></span> <span data-ttu-id="96767-120">Obtiene todas las consultas definidas por el usuario y el sistema de manera predeterminada.</span><span class="sxs-lookup"><span data-stu-id="96767-120">Gets all the system and user-defined queries by default.</span></span> |
| [<span data-ttu-id="96767-121">DELETE Report Query</span><span class="sxs-lookup"><span data-stu-id="96767-121">DELETE Report Query</span></span>](insights-programmatic-analytics-api-delete-report-queries.md) | <span data-ttu-id="96767-122">Elimina consultas definidas por el usuario.</span><span class="sxs-lookup"><span data-stu-id="96767-122">Deletes user-defined queries.</span></span> |
|||

## <a name="report-management-apis"></a><span data-ttu-id="96767-123">API de administración de informes</span><span class="sxs-lookup"><span data-stu-id="96767-123">Report management APIs</span></span>

<span data-ttu-id="96767-124">***Tabla 3: API de administración de informes***</span><span class="sxs-lookup"><span data-stu-id="96767-124">***Table 3: Report management APIs***</span></span>

| <span data-ttu-id="96767-125">**API**</span><span class="sxs-lookup"><span data-stu-id="96767-125">**API**</span></span> | <span data-ttu-id="96767-126">**Funcionalidad**</span><span class="sxs-lookup"><span data-stu-id="96767-126">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="96767-127">Crear informe</span><span class="sxs-lookup"><span data-stu-id="96767-127">Create Report</span></span>](insights-programmatic-access-paradigm.md#create-report-api) | <span data-ttu-id="96767-128">Programa una consulta para que se ejecute en intervalos regulares.</span><span class="sxs-lookup"><span data-stu-id="96767-128">Schedules a query to be executed at regular intervals.</span></span> |
| [<span data-ttu-id="96767-129">TRY Report Query</span><span class="sxs-lookup"><span data-stu-id="96767-129">TRY Report Query</span></span>](insights-programmatic-analytics-api-try-report-queries.md) | <span data-ttu-id="96767-130">Ejecuta una instrucción de consulta de informe.</span><span class="sxs-lookup"><span data-stu-id="96767-130">Executes a Report query statement.</span></span> <span data-ttu-id="96767-131">Devuelve solo 10 registros que los asociados pueden usar para comprobar si los datos son los esperados.</span><span class="sxs-lookup"><span data-stu-id="96767-131">Returns only 10 records that a partner can use to verify if the data is as expected.</span></span> |
| [<span data-ttu-id="96767-132">Obtener un informe</span><span class="sxs-lookup"><span data-stu-id="96767-132">Get Report</span></span>](insights-programmatic-analytics-api-get-report.md) | <span data-ttu-id="96767-133">Obtiene todos los informes que se han programado.</span><span class="sxs-lookup"><span data-stu-id="96767-133">Get all the reports that have been scheduled.</span></span> |
| [<span data-ttu-id="96767-134">Actualización de informes</span><span class="sxs-lookup"><span data-stu-id="96767-134">Update Report</span></span>](insights-programmatic-analytics-api-update-report.md) | <span data-ttu-id="96767-135">Modifica un parámetro de informe.</span><span class="sxs-lookup"><span data-stu-id="96767-135">Modify a report parameter.</span></span> |
| [<span data-ttu-id="96767-136">Eliminación de informes</span><span class="sxs-lookup"><span data-stu-id="96767-136">Delete Report</span></span>](insights-programmatic-analytics-api-delete-report.md) | <span data-ttu-id="96767-137">Elimina todos los registros de ejecución de informes e informes.</span><span class="sxs-lookup"><span data-stu-id="96767-137">Deletes all the report and report execution records.</span></span> |
| [<span data-ttu-id="96767-138">Pausa de ejecuciones de informes</span><span class="sxs-lookup"><span data-stu-id="96767-138">Pause Report Executions</span></span>](insights-programmatic-analytics-api-pause-report-executions.md) | <span data-ttu-id="96767-139">Pausa la ejecución programada de informes.</span><span class="sxs-lookup"><span data-stu-id="96767-139">Pauses the scheduled execution of reports.</span></span> |
| [<span data-ttu-id="96767-140">Reanudación de ejecuciones de informes</span><span class="sxs-lookup"><span data-stu-id="96767-140">Resume Report Executions</span></span>](insights-programmatic-analytics-api-resume-report-executions.md) | <span data-ttu-id="96767-141">Reanuda la ejecución programada de un informe en pausa.</span><span class="sxs-lookup"><span data-stu-id="96767-141">Resumes the scheduled execution of a paused report.</span></span> |
|||

## <a name="report-execution-pull-apis"></a><span data-ttu-id="96767-142">API de extracción de ejecución de informes</span><span class="sxs-lookup"><span data-stu-id="96767-142">Report execution pull APIs</span></span>

<span data-ttu-id="96767-143">***Tabla 4: API de extracción de ejecución de informes***</span><span class="sxs-lookup"><span data-stu-id="96767-143">***Table 4: Report execution pull APIs***</span></span>

| <span data-ttu-id="96767-144">**API**</span><span class="sxs-lookup"><span data-stu-id="96767-144">**API**</span></span> | <span data-ttu-id="96767-145">**Funcionalidad**</span><span class="sxs-lookup"><span data-stu-id="96767-145">**Functionality**</span></span> |
| --- | --- |
| [<span data-ttu-id="96767-146">Obtención de ejecuciones de informes</span><span class="sxs-lookup"><span data-stu-id="96767-146">Get Report Executions</span></span>](insights-programmatic-access-paradigm.md#get-report-execution-api) | <span data-ttu-id="96767-147">Obtiene todas las ejecuciones que se han producido para un informe determinado.</span><span class="sxs-lookup"><span data-stu-id="96767-147">Get all the executions that have happened for a given report.</span></span> |
|||

## <a name="next-steps"></a><span data-ttu-id="96767-148">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="96767-148">Next steps</span></span>

- <span data-ttu-id="96767-149">Puede probar las API a través de la [dirección URL de la API de Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span><span class="sxs-lookup"><span data-stu-id="96767-149">You can try out the APIs through the [Swagger API URL](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).</span></span>