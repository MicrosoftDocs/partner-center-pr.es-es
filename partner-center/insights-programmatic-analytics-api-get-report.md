---
title: 'Obtener la API de informe: Ideas datos'
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para obtener todos los identificadores de informe disponibles en Centro de partners insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 174a2f60a36cb46b287b787b177dd32236cef4eb
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376122"
---
# <a name="get-report-api"></a>Obtención de API de informe

Esta API obtiene todos los informes que se han programado.

**Sintaxis de la solicitud**

|    Método    |    URI de solicitud    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport?reportId={Report ID}&reportName={Report Name}&queryId={Query ID}` |
|        |        |

**Encabezado de solicitud**

|    Encabezado    |    Tipo    |    Descripción    |
|    ----    |    ----    |    ----    |
|    Authorization    |    string    |    Necesario. Token Azure Active Directory de acceso de Azure Active Directory (AAD) en el formulario`Bearer <token>`    |
|    Content-Type    |    string    |    `Application/JSON`    |
|        |        |        |

**Parámetro de ruta de acceso**

Ninguno

**Parámetro de consulta**

|    Nombre de parámetro    |    Tipo    |    Obligatorio    |    Descripción    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    string    |    No    |    Filtre para obtener detalles de solo los informes con el valor de reportId especificado en este argumento.     |
|    reportName     |    string    |    No    |    Filtre para obtener detalles de solo los informes con el valor reportName especificado en este argumento.     |
|    queryId     |    string    |    No    |    Filtre para obtener detalles de solo los informes con el valor de queryId especificado en este argumento.     |
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
      "executeNow": true, 
      "StartTime": "string", 
      "ReportStatus": "string", 
      "RecurrenceInterval": 0, 
      " RecurrenceCount": 0, 
      "CallbackUrl": "string",
      "CallbackMethod": null,
      "Format": "string" 
    } 
  ], 
  "TotalCount": 0, 
  "Message": "string", 
  "StatusCode": 0 
}
```

**Glosario**

En esta tabla se definen los elementos clave de la respuesta:

|    Parámetro    |    Descripción    |
|    ----    |    ----    |
|    ReportId     |    UUID único del informe que se creó.     |
|    ReportName     |    Nombre dado al informe en la carga útil de solicitud     |
|    Descripción     |    Descripción dada cuando se creó el informe.     |
|    QueryId     |    Id. de consulta pasado en el momento en que se creó el informe.     |
|    Consultar     |    Texto de la consulta que se ejecutará para este informe.     |
|    Usuario     |    Identificador de usuario usado para crear el informe     |
|    CreatedTime     |    Hora de creación del informe. El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.     |
|    ModifiedTime     |    Hora en que se modificó el informe por última vez. El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.     |
|    executeNow     |    Marca ExecuteNow establecida en el momento en que se creó el informe    |
|    StartTime     |    Se iniciará la ejecución de la hora. El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.     |
|    ReportStatus     |    Estado de la ejecución del informe. Los valores posibles son en pausa, activo e inactivo.     |
|    RecurrenceInterval     |    Intervalo de periodicidad proporcionado durante la creación del informe.     |
|    RecurrenceCount     |    Recuento de periodicidad proporcionado durante la creación del informe.     |
|    CallbackUrl     |    Dirección URL de devolución de llamada proporcionada en la solicitud.     |
|    CallbackMethod    |    Método de devolución de llamada proporcionado en la solicitud    |
|    Formato     |    Formato de los archivos de informe.     |
|    TotalCount     |    Número de conjuntos de datos en la matriz de valores.     |
|    Message     |    Mensaje de estado de la ejecución de la API.     |
|    StatusCode     |    Código de resultado. Los valores posibles son 200, 400, 401, 403 y 500.     |
|        |        |