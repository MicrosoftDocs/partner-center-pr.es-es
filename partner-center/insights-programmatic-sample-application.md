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
# <a name="sample-application"></a><span data-ttu-id="1b443-103">Aplicación de ejemplo</span><span class="sxs-lookup"><span data-stu-id="1b443-103">Sample Application</span></span>

<span data-ttu-id="1b443-104">Las aplicaciones de ejemplo se crean en lenguajes C# y JAVA y están disponibles en [GitHub](https://github.com/partneranalytics)</span><span class="sxs-lookup"><span data-stu-id="1b443-104">Sample applications are created in C# and JAVA languages and are available on [GitHub](https://github.com/partneranalytics)</span></span>

- [<span data-ttu-id="1b443-105">Aplicación de ejemplo de C#</span><span class="sxs-lookup"><span data-stu-id="1b443-105">C# Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [<span data-ttu-id="1b443-106">Aplicación de ejemplo de Java</span><span class="sxs-lookup"><span data-stu-id="1b443-106">JAVA Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

<span data-ttu-id="1b443-107">Puede inspirarse en la aplicación de ejemplo y compilar su propia aplicación en cualquier lenguaje.</span><span class="sxs-lookup"><span data-stu-id="1b443-107">You can choose to take inspiration from the sample application and build your own application in any language.</span></span>

<span data-ttu-id="1b443-108">La aplicación de ejemplo logra los siguientes objetivos:</span><span class="sxs-lookup"><span data-stu-id="1b443-108">The sample application achieves the following objectives:</span></span>

- <span data-ttu-id="1b443-109">Genera un token Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="1b443-109">Generates an Azure Active Directory (Azure AD) Token.</span></span>
- <span data-ttu-id="1b443-110">Obtiene los conjuntos de datos disponibles.</span><span class="sxs-lookup"><span data-stu-id="1b443-110">Gets available datasets.</span></span>
- <span data-ttu-id="1b443-111">Crea consultas definidas por el usuario.</span><span class="sxs-lookup"><span data-stu-id="1b443-111">Creates user defined queries.</span></span>
- <span data-ttu-id="1b443-112">Obtiene las consultas definidas por el usuario y del sistema.</span><span class="sxs-lookup"><span data-stu-id="1b443-112">Gets user defined and system queries.</span></span>
- <span data-ttu-id="1b443-113">Programa un informe.</span><span class="sxs-lookup"><span data-stu-id="1b443-113">Schedules a report.</span></span>

<span data-ttu-id="1b443-114">La aplicación de ejemplo no cubre el método de llamar a las API para otras funcionalidades.</span><span class="sxs-lookup"><span data-stu-id="1b443-114">The sample application doesn't cover the method of calling APIs for other functionalities.</span></span> <span data-ttu-id="1b443-115">Sin embargo, el proceso de llamada a otras API sigue siendo el mismo que se ha descrito anteriormente.</span><span class="sxs-lookup"><span data-stu-id="1b443-115">However, the process of calling other APIs remains the same as outlined above.</span></span>

## <a name="how-to-run-the-application"></a><span data-ttu-id="1b443-116">Procedimiento para ejecutar la aplicación</span><span class="sxs-lookup"><span data-stu-id="1b443-116">How to run the application</span></span>

- <span data-ttu-id="1b443-117">Clone el repositorio en un sistema local mediante este comando:</span><span class="sxs-lookup"><span data-stu-id="1b443-117">Clone the repository to a local system using this command:</span></span>

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> <span data-ttu-id="1b443-118">Para obtener más instrucciones, consulte el archivo ProgrammaticExportSampleAppMPN/README.md en GitHub [repositorio](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).</span><span class="sxs-lookup"><span data-stu-id="1b443-118">For more instructions, refer to the ProgrammaticExportSampleAppMPN/README.md file in the GitHub [repository](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).</span></span>

- <span data-ttu-id="1b443-119">Para ejecutar rápidamente la aplicación, actualice el identificador de cliente y el secreto de cliente en el **appsettings.Development.js**</span><span class="sxs-lookup"><span data-stu-id="1b443-119">To quickly run the app, update the client id and client secret in the **appsettings.Development.json**</span></span>

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="Ilustrar aplicaciones json de desarrollo de la asociación":::

<span data-ttu-id="1b443-121">Al ejecutar la aplicación, se iniciará un servidor web local y se abrirá una página (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span><span class="sxs-lookup"><span data-stu-id="1b443-121">Running the app will start a local web server and a page will open (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span></span>
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="Ilustrar la interfaz de usuario de la aplicación de ejemplo":::

<span data-ttu-id="1b443-123">Esta página realizará llamadas API al servidor web que se ejecuta en el equipo local, que a su vez realizará las llamadas de API de acceso mediante programación reales.</span><span class="sxs-lookup"><span data-stu-id="1b443-123">This page will make API calls to the webserver running on the local machine, which in turn will make the actual programmatic access API calls.</span></span>

## <a name="code-snippets"></a><span data-ttu-id="1b443-124">Fragmentos de código</span><span class="sxs-lookup"><span data-stu-id="1b443-124">Code Snippets</span></span>

<span data-ttu-id="1b443-125">La estructura básica del código C# para realizar llamadas API de acceso mediante programación es la siguiente:</span><span class="sxs-lookup"><span data-stu-id="1b443-125">The basic structure of the C# code for doing the programmatic access API calls is as follows:</span></span>
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Ilustrar fragmento de código":::

## <a name="next-steps"></a><span data-ttu-id="1b443-127">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="1b443-127">Next steps</span></span>

[<span data-ttu-id="1b443-128">API para acceder a los datos de análisis de Conclusiones de asociados</span><span class="sxs-lookup"><span data-stu-id="1b443-128">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)
