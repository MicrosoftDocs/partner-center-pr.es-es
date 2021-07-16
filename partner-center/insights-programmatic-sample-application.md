---
title: Aplicación de ejemplo
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use la aplicación de ejemplo para compilar su propia aplicación para acceder mediante programación a los datos de conclusiones de asociados.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 6f334b9047c38e8b7763a4ba96d21d987c252682
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/16/2021
ms.locfileid: "114375854"
---
# <a name="sample-application"></a>Aplicación de ejemplo

Las aplicaciones de ejemplo se crean en lenguajes C# y JAVA y están disponibles en [GitHub](https://github.com/partneranalytics)

- [Aplicación de ejemplo de C#](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [Aplicación de ejemplo de Java](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

Puede inspirarse en la aplicación de ejemplo y compilar su propia aplicación en cualquier lenguaje.

La aplicación de ejemplo logra los siguientes objetivos:

- Genera un token Azure Active Directory (Azure AD).
- Obtiene los conjuntos de datos disponibles.
- Crea consultas definidas por el usuario.
- Obtiene las consultas definidas por el usuario y del sistema.
- Programa un informe.

La aplicación de ejemplo no cubre el método de llamar a las API para otras funcionalidades. Sin embargo, el proceso de llamada a otras API sigue siendo el mismo que se ha descrito anteriormente.

## <a name="how-to-run-the-application"></a>Procedimiento para ejecutar la aplicación

- Clone el repositorio en un sistema local mediante este comando:

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> Para obtener más instrucciones, consulte el archivo ProgrammaticExportSampleAppMPN/README.md en GitHub [repositorio](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).

- Para ejecutar rápidamente la aplicación, actualice el identificador de cliente y el secreto de cliente en el **appsettings.Development.js**

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Ilustrar aplicaciones json de desarrollo de la asociación":::

Al ejecutar la aplicación, se iniciará un servidor web local y se abrirá una página (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Ilustrar la interfaz de usuario de la aplicación de ejemplo":::

Esta página realizará llamadas API al servidor web que se ejecuta en el equipo local, que a su vez realizará las llamadas de API de acceso mediante programación reales.

## <a name="code-snippets"></a>Fragmentos de código

La estructura básica del código C# para realizar llamadas API de acceso mediante programación es la siguiente:
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Ilustrar fragmento de código":::

## <a name="next-steps"></a>Pasos siguientes

[API para acceder a los datos de análisis de Conclusiones de asociados](insights-programmatic-analytics-available-api.md)
