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
# <a name="delete-report-queries-api"></a>Eliminación de API de consultas de informe

Esta API elimina consultas definidas por el usuario.

**Sintaxis de la solicitud**

|    Método    |    URI de solicitud    |
|    ----    |    ----    |
|    Delete    |    `https://api.partnercenter.microsoft.com/insights/v1/mpn/ScheduledQueries/{queryId}` |
|        |        |

**Encabezado de solicitud**

|    Encabezado    |    Tipo    |    Descripción    |
|    ----    |    ----    |    ----    |
|    Authorization    |    string    |    Necesario. Token Azure Active Directory acceso de Azure Active Directory (AAD) en el formulario`Bearer <token>`    |
|    Content-Type    |    string    |    `Application/JSON`    |
|        |        |        |

**Parámetro de ruta de acceso**

|    Nombre de parámetro    |    Tipo    |    Obligatorio    |    Descripción    |
|    ----    |    ----    |    ----    |    ----    |
|    queryId     |    string     |    No    |    Filtrar para obtener los detalles de solo las consultas con el id. dado en el argumento     |
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
|    QueryId     |    UUID único de la consulta que se eliminó    |
|    Nombre     |    Nombre de la consulta eliminada.    |
|    Descripción     |    Descripción de la consulta eliminada.     |
|    Consultar     |    Cadena de consulta de informe de la consulta eliminada.    |
|    Tipo     |    Establezca en userDefined para las consultas creadas por el usuario.     |
|    Usuario     |    Id. de usuario que creó la consulta.     |
|    CreatedTime     |    Hora de creación de la consulta.     |
|    TotalCount     |    Número de conjuntos de datos en la matriz de valores.     |
|    Message     |    Mensaje de estado de la ejecución de la API.     |
|    StatusCode     |    Código de resultado. Los valores posibles son 200, 400, 401, 403 y 500.     |
|        |        |
