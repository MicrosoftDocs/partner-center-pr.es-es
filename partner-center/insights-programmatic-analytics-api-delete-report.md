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
# <a name="delete-report-api"></a>Eliminación de API de informe

En la ejecución, esta API elimina todos los registros de ejecución de informes y de informes.

**Sintaxis de la solicitud**

|    Método    |    URI de solicitud    |
|    ----    |    ----    |
|    Delete    |    ` https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
|        |        |

**Encabezado de solicitud**

|    Encabezado    |    Tipo    |    Descripción    |
|    ----    |    ----    |    ----    |
|    Authorization    |    string    |    Necesario. Token Azure Active Directory de acceso de Azure Active Directory (AAD) en el formulario`Bearer <token>`    |
|    Content-Type    |    string    |    `Application/JSON`    |
|        |        |        |

**Parámetro de ruta de acceso**

|    Nombre de parámetro    |    Tipo    |    Obligatorio    |    Descripción    |
|    ----    |    ----    |    ----    |    ----    |
|    reportId     |    string    |    No    |    Identificador del informe que se va a eliminar    |
|        |        |        |        |

**Parámetro de consulta**

Ninguno

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

**Glosario**

En esta tabla se definen los elementos clave de la respuesta:

|    Parámetro    |    Descripción    |
|    ----    |    ----    |
|    ReportId     |    Identificador único universal (UUID) del informe eliminado.     |
|    ReportName     |    Nombre dado al informe durante la creación.     |
|    Descripción     |    Descripción proporcionada durante la creación del informe.     |
|    QueryId     |    Id. de consulta pasado en el momento en que se creó el informe.     |
|    Consultar     |    Texto de la consulta que se ejecutará para este informe.     |
|    Usuario     |    Identificador de usuario usado para crear el informe     |
|    CreatedTime     |    Hora de creación del informe. El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.     |
|    ModifiedTime     |    Hora en que se modificó el informe por última vez. El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.     |
|    ExecuteNow     |    Marca ExecuteNow establecida en el momento en que se creó el informe     |
|    StartTime     |    Hora a la que se iniciará la ejecución del informe. El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.     |
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
