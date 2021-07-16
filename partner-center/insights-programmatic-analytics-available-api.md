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
# <a name="available-apis-for-partner-insights-analytics"></a>API disponibles para el análisis de Conclusiones de asociados

A continuación se muestra la lista de API para el análisis de conclusiones de asociados y sus funcionalidades asociadas.

## <a name="dataset-pull-apis"></a>API de extracción de conjuntos de datos

***Tabla 1: API de extracción de conjuntos de datos***

| **API** | **Funcionalidad** |
| --- | --- |
| [Obtener todos los conjuntos de datos](insights-programmatic-analytics-api-get-dataset.md) | Obtiene todos los conjuntos de datos disponibles. Los conjuntos de datos muestran las tablas, las columnas, las métricas y los intervalos de tiempo. |
|||

## <a name="query-management-apis"></a>API de administración de consultas

***Tabla 2: API de administración de consultas***

| **API** | **Funcionalidad** |
| --- | --- |
| [Creación de consultas de informes](insights-programmatic-access-paradigm.md#create-report-query-api) | Crea consultas personalizadas que definen el conjunto de datos del que deben exportarse las columnas y métricas. |
| [GET Report Query](insights-programmatic-analytics-api-get-report-queries.md) | Obtiene todas las consultas disponibles para su uso en informes. Obtiene todas las consultas definidas por el usuario y el sistema de manera predeterminada. |
| [DELETE Report Query](insights-programmatic-analytics-api-delete-report-queries.md) | Elimina consultas definidas por el usuario. |
|||

## <a name="report-management-apis"></a>API de administración de informes

***Tabla 3: API de administración de informes***

| **API** | **Funcionalidad** |
| --- | --- |
| [Crear informe](insights-programmatic-access-paradigm.md#create-report-api) | Programa una consulta para que se ejecute en intervalos regulares. |
| [TRY Report Query](insights-programmatic-analytics-api-try-report-queries.md) | Ejecuta una instrucción de consulta de informe. Devuelve solo 10 registros que los asociados pueden usar para comprobar si los datos son los esperados. |
| [Obtener un informe](insights-programmatic-analytics-api-get-report.md) | Obtiene todos los informes que se han programado. |
| [Actualización de informes](insights-programmatic-analytics-api-update-report.md) | Modifica un parámetro de informe. |
| [Eliminación de informes](insights-programmatic-analytics-api-delete-report.md) | Elimina todos los registros de ejecución de informes e informes. |
| [Pausa de ejecuciones de informes](insights-programmatic-analytics-api-pause-report-executions.md) | Pausa la ejecución programada de informes. |
| [Reanudación de ejecuciones de informes](insights-programmatic-analytics-api-resume-report-executions.md) | Reanuda la ejecución programada de un informe en pausa. |
|||

## <a name="report-execution-pull-apis"></a>API de extracción de ejecución de informes

***Tabla 4: API de extracción de ejecución de informes***

| **API** | **Funcionalidad** |
| --- | --- |
| [Obtención de ejecuciones de informes](insights-programmatic-access-paradigm.md#get-report-execution-api) | Obtiene todas las ejecuciones que se han producido para un informe determinado. |
|||

## <a name="next-steps"></a>Pasos siguientes

- Puede probar las API a través de la [dirección URL de la API de Swagger](https://api.partnercenter.microsoft.com/insights/v1/mpn/swagger/index.html).