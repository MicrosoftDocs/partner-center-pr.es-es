---
title: Actualización de la API de informe
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para actualizar los parámetros de informe en Centro de partners insights.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: c5ab1059e9be9b42918d268da6a6c1a3cbfe52af
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376090"
---
# <a name="update-report-api"></a>Actualización de la API de informe

Esta API ayuda a modificar un parámetro de informe.

**Sintaxis de la solicitud**

|    Método    |    URI de la solicitud    |
|    ----    |    ----    |
|    PUT    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledReport/{Report ID}`    |
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
|    reportId     |    string    |    No    |    Id. del informe que se está modificando     |
|        |        |        |        |

**Parámetro de consulta**

Ninguno

**Carga de solicitud**

```json
{ 
  "ReportName": "string", 
  "Description": "string", 
  "StartTime": "string", 
  "RecurrenceInterval": 0, 
  "RecurrenceCount": 0, 
  "Format": "string", 
  "CallbackUrl": "string",
 "CallbackMethod": "string"
}
```

**Glosario**

En esta tabla se indican las definiciones clave de los elementos de la respuesta.

|    Parámetro    |    Obligatorio    |    Descripción    |    Valores permitidos    |
|    ----    |    ----    |    ----    |    ----    |
|    ReportName     |    Sí     |    Nombre que se va a asignar al informe     |    String     |
|    Descripción     |    No     |    Descripción del informe creado     |    String     |
|    StartTime     |    Sí    |    Marca de tiempo después de la que comenzará la generación del informe     |    String     |
|    RecurrenceInterval     |    No     |    Frecuencia (en horas) con la que se debe generar el informe. El valor mínimo es 4.     |    Entero     |
|    RecurrenceCount     |    No     |    Números de informe que se generarán. El valor predeterminado es indefinido.     |    Entero     |
|    Formato     |    No    |    Formato del archivo exportado. El valor predeterminado es CSV     |    CSV/TSV     |
|    CallbackURL     |    No     |    Dirección URL de devolución de llamada HTTPS a la que se llamará en la generación de informes.     |    String     |
|    CallbackMethod    |    No    |    Método HTTP que se va a usar para la devolución de llamada    |    GET/POST    |
|        |        |        |        |


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
|    ReportId     |    Identificador único universal (UUID) del informe que se actualiza     |
|    ReportName     |    Nombre dado al informe en la carga útil de solicitud     |
|    Descripción     |    Descripción dada al informe en la carga de solicitud     |
|    QueryId     |    Id. de consulta pasado en el momento en que se creó el informe.     |
|    Consultar     |    Texto de la consulta que se ejecutará para este informe.     |
|    Usuario     |    Identificador de usuario usado para crear el informe     |
|    CreatedTime     |    Hora de creación del informe. El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.     |
|    ModifiedTime     |    Hora en que se modificó el informe por última vez. El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.     |
|    ExecuteNow     |    Marca ExecuteNow establecida en el momento en que se creó el informe    |
|    StartTime     |    Hora a la que se iniciará la ejecución del informe. El formato de la hora es aaaa-MM-ddTHH:mm:ssZ.     |
|    ReportStatus     |    Estado de la ejecución del informe. Los valores posibles son en pausa, activo e inactivo.     |
|    RecurrenceInterval     |    Intervalo de periodicidad proporcionado en la carga de solicitud     |
|    RecurrenceCount     |    Recuento de periodicidad proporcionado en la carga de solicitud     |
|    CallbackUrl     |    Dirección URL de devolución de llamada proporcionada en la solicitud.     |
|    CallbackMethod    |    Método de devolución de llamada proporcionado en la solicitud    |
|    Formato     |    Formato de los archivos de informe.     |
|    TotalCount     |    Número de conjuntos de datos en la matriz de valores.     |
|    Message     |    Mensaje de estado de la ejecución de la API.     |
|    StatusCode     |    Código de resultado. Los valores posibles son 200, 400, 401, 403 y 500.     |
|        |        |