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
# <a name="try-report-queries-api"></a>Prueba de la API de consultas de informe

Esta API ejecuta una instrucción de consulta de informe. La API devuelve solo 100 registros que usted como asociado puede usar para comprobar si los datos son los esperados.

> [!IMPORTANT]
> Esta API tiene un tiempo de espera de ejecución de consulta de 100 segundos. Si observa que la API tarda más, es muy probable que la consulta sea sintácticamente correcta o que haya recibido un código de error distinto de 200. La generación del informe real sucederá si la sintaxis de la consulta es correcta.

**Sintaxis de la solicitud**

|    Método    |    URI de solicitud    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/testQueryResult?<exportQuery={query text}|queryId={queryId}>`    |
|        |        |

**Encabezado de solicitud**

|    Encabezado    |    Tipo    |    Descripción    |
|    ----    |    ----    |    ----    |
|    Authorization    |    string    |    Necesario. Token Azure Active Directory acceso de Azure Active Directory (AAD) en el formulario`Bearer <token>`    |
|    Content-Type    |    string    |    `Application/JSON`    |
|        |        |        |

**Parámetro de ruta de acceso**

Ninguno

**Parámetro de consulta**

|    Nombre de parámetro    |    Tipo    |    Obligatorio    |    Descripción    |
|    ----    |    ----    |    ----    |    ----    |
|    exportQuery     |    string    |    No    |    Cadena de consulta de informe que se debe ejecutar     |
|    queryId     |    string    |    No    |    Identificador de consulta existente válido. Mutuamente excluyente con la cadena de consulta especificada en el parámetro exportQuery    |
|    startTime     |    string    |    No    |    Hora de inicio desde la que queremos los datos. Invalida el intervalo de tiempo especificado en la consulta.    |
|    endTime     |    string    |    No    |    Hora de finalización hasta la que queremos los datos. Invalida el intervalo de tiempo especificado en la consulta.    |
|        |        |        |        |

**Carga de solicitud**

Ninguno

**Glosario**

Ninguno

**Respuesta**

La carga de respuesta tiene la estructura siguiente:

Código de respuesta: 200, 400, 401, 403, 404, 500

Ejemplo de carga de respuesta:

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

**Glosario**

En esta tabla se definen los elementos clave de la respuesta:

|    Parámetro    |    Descripción    |
|    ----    |    ----    |
|    TotalCount     |    Número de conjuntos de datos en la matriz de valores.     |
|    Message     |    Mensaje de estado de la ejecución de la API.     |
|    StatusCode     |    Código de resultado. Los valores posibles son 200, 400, 401, 403 y 500.     |
|        |        |
