---
title: 'Obtener consultas de informe API: Ideas datos'
ms.topic: reference
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use esta API para obtener todas las consultas disponibles para su uso en la API de informe.
author: kshitishsahoo
ms.author: ksahoo
ms.localizationpriority: medium
ms.openlocfilehash: 3bf140576a19439990405cfef23190045e0a98be
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376127"
---
# <a name="get-report-queries-api"></a>Obtención de API de consultas de informe

La API Get report queries obtiene todas las consultas que están disponibles para su uso en informes. Obtiene todas las consultas del sistema y las definidas por el usuario de forma predeterminada.

**Sintaxis de la solicitud**

|    Método    |    URI de solicitud    |
|    ----    |    ----    |
|    GET    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries?queryId={QueryID}&queryName={QueryName}&includeSystemQueries={include_system_queries}&includeOnlySystemQueries={include_only_system_queries}`     |
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
|    queryId     |    string     |    No    |    Filtrar para obtener los detalles de solo las consultas con el id. dado en el argumento     |
|    queryName     |    string     |    No    |    Filtrar para obtener los detalles de solo las consultas con el nombre dado en el argumento     |
|    IncludeSystemQueries     |    boolean     |    No    |    Incluir consultas predefinidas por el sistema en la respuesta     |
|    IncludeOnlySystemQueries     |    boolean     |    No    |    Incluir solo las consultas del sistema en la respuesta     |
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

**Glosario**

En esta tabla se definen los elementos clave de la respuesta:

|    Parámetro    |    Descripción    |
|    ----    |    ----    |
|    QueryId     |    UUID único de la consulta.     |
|    Nombre     |    Nombre asignado a la consulta en el momento de la creación de la consulta.     |
|    Descripción     |    Descripción proporcionada durante la creación de la consulta.     |
|    Consultar     |    Cadena de consulta del informe.     |
|    Tipo     |    Se establece en userDefined para consultas creadas por el usuario y sistema para consultas predefinidas del sistema     |
|    Usuario     |    Id. de usuario que creó la consulta.     |
|    CreatedTime     |    Hora de creación de la consulta.     |
|    TotalCount     |    Número de conjuntos de datos en la matriz de valores.     |
|    Message     |    Mensaje de estado de la ejecución de la API.     |
|    StatusCode     |    Código de resultado. Los valores posibles son 200, 400, 401, 403 y 500.     |
|        |        |
