---
title: Acceso basado en roles de Partner Center Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre los roles específicos necesarios para ver los informes de Partner Center Insights. Entre ellos se incluyen los roles del visor de informes ejecutivo y el visor de informes.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 980c086a2ab1ee0a21592ceb1e2e018c0e1159ae
ms.sourcegitcommit: bcd0c09d3acd5eae4fbfca7ea6614a54d203eff6
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/04/2020
ms.locfileid: "89490613"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Control de acceso basado en roles al panel de información del centro de Partners

El panel Insights usa dos nuevos roles en el centro de partners para administrar el acceso de los empleados a los informes: visor de informes ejecutivos y visor de informes.  Los usuarios del rol Executive Report Viewer tienen acceso a todos los conjuntos de datos de informes, mientras que los usuarios del rol visor de informes no tendrán acceso a conjuntos de datos confidenciales como los ingresos y los datos personales de clientes y empleados.  

Al igual que con otras funciones del centro de Partners, el administrador global o el administrador de la cuenta podrán asignar usuarios a esos roles en la página de administración de usuarios. Los roles pueden ser aplicables en toda la empresa o en ubicaciones específicas de MPN. Los roles asignados a ubicaciones específicas de MPN limitan al usuario a ver los datos de informes asociados solo con las ubicaciones de MPN seleccionadas. El asociado puede seleccionar una o varias ubicaciones en la vista siguiente.

:::image type="content" source="images/pci/roles.png" alt-text="Muestra la configuración de roles del centro de Partners de la ubicación específica para el visor de informes y el visor de informes ejecutivos.":::

>[!Note]
> Los usuarios que son administradores de MPN a partir del 20 de enero de 2020 se agregan automáticamente al rol de **visor de informes Ejecutivo** de toda la compañía para todas las ubicaciones de ese inquilino. Por lo tanto, estos usuarios pueden tener acceso a los informes como un visor de informes ejecutivo sin ninguna acción explícita requerida por el administrador global o el administrador de la cuenta. Los administradores globales y los administradores de cuentas pueden invalidar los roles asignados automáticamente de estos usuarios para aumentar o reducir aún más sus capacidades.

## <a name="next-steps"></a>Pasos siguientes

- Obtenga más información sobre los [detalles del centro de Partners](partner-center-insights.md) y sus diversos informes.
