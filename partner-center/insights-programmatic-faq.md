---
title: Preguntas comunes sobre el acceso mediante programación a Partner Insights
description: Obtenga respuestas a las preguntas más frecuentes sobre el acceso a los datos de conclusiones de asociados a través de la API.
ms.topic: troubleshooting
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: 5645a834c2b6a84920ba032198f7f62aa1487c47
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376058"
---
# <a name="programmatic-access-of-analytics-data-common-questions"></a>Acceso mediante programación a preguntas comunes sobre datos de análisis

En este artículo se abordan las preguntas más frecuentes sobre cómo acceder mediante programación a los datos de información de asociados en Centro de partners.

## <a name="api-responses"></a>Respuestas de API

¿Cuáles son los diferentes escenarios en los que se puede recibir una respuesta de API distinta de 200 (correcto)?

En esta tabla se describen las respuestas de API y qué hacer si se reciben.

|    Descripción del error     |    Código de error     |    Solución de problemas     |
|    ----    |    ----    |    ----    |
|    No autorizado     |    401     |    Se trata de una excepción de autenticación. Compruebe la corrección del token Azure Active Directory (AAD). El token de AAD es válido durante 60 minutos, después de lo cual tendría que volver a generar el token de AAD.     |
|    Nombre de tabla no válido     |    400     |    El nombre del conjunto de datos es incorrecto. Vuelva a comprobar el nombre del conjunto de datos llamando a la API "Obtener todos los conjuntos de datos".     |
|    Nombre de columna incorrecto     |    400     |    El nombre de la columna de la consulta es incorrecto. Vuelva a comprobar el nombre de columna mediante una llamada a la API "Obtener todos los conjuntos de datos" o haga referencia a los nombres de columna en las definiciones de datos.    |
|    Falta valor o es NULL     |    400     |    Es posible que falten parámetros obligatorios como parte de la carga de solicitud de la API.     |
|    Parámetros de informe no válidos     |    400     |    Asegúrese de que los parámetros de informe sean correctos. Por ejemplo, puede que esté dando un valor menor que 4 para el parámetro RecurrenceInterval.     |
|    El intervalo de periodicidad debe estar entre 4 y 2160     |    400     |    Asegúrese de que el valor del parámetro de solicitud RecurrenceInterval está entre 4 y 2160.     |
|    QueryId no válido     |    400     |    Vuelva a comprobar el QueryId generado.     |
|    Parámetros de informe no válidos para la creación: la hora de inicio del informe debe ser al menos 4 horas a partir de la hora UTC actual     |    400     |    El parámetro Start Time como parte de la carga de la solicitud no debe estar en el pasado. La hora de inicio del informe debe ser de al menos 4 horas después de la hora UTC actual.     |
|    No se encontró el valor solicitado 'string'     |    400     |    Compruebe si ha actualizado los parámetros de solicitud `callbackurl` o el formato.     |
|    No se encontró ningún elemento con los filtros especificados.     |    404     |    Compruebe el parámetro reportID que se usa en la API Get Report Executions.     |
|    No se han producido ejecuciones para las condiciones de filtro dadas. Compruebe el valor de reportId o executionId y vuelva a intentar la API después del tiempo de ejecución programado del informe.     |    404     |    Asegúrese de que el valor de reportId es correcto. Vuelva a intentar la API después del tiempo de ejecución programado del informe como se especifica en la carga de solicitud.     |
|    Se encontró un error interno al crear el informe. Id. de correlación <>     |    500     |    Asegúrese de que el formato de fecha de los campos *StartTime*, *QueryStartTime* y *QueryEndTime* sea correcto.     |
|    Servicio no disponible    |    500     |    Si recibe continuamente un servicio no disponible (error 5xx), abra una vale de soporte técnico.    |
|        |        |        |

## <a name="no-records"></a>Ningún registro

Recibo la respuesta 200 de la API al descargar el informe desde la ubicación segura. ¿Por qué no se obtienen registros?
Compruebe si la cadena de la consulta tiene uno de los valores permitidos para el encabezado de columna. Por ejemplo, esta consulta devolverá cero resultados:

```sql
SELECT CustomerTenantId, CustomerTpId, WorkloadName, Month, MonthlyActiveUsers 
FROM OfficeUsage 
WHERE IsDuplicateRowForPGA = 'False' 
ORDER BY CustomerTenantId DESC
```

En este ejemplo, los valores permitidos para `IsDuplicateRowForPGA` son 0 o 1. Consulte [definiciones de datos para](insights-data-definitions.md) ver todos los valores posibles de las distintas columnas.
