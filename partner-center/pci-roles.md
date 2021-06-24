---
title: acceso basado en roles de Centro de partners Insights
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre los roles específicos necesarios para ver Centro de partners Insights. Estos incluyen los roles de Visor de informes ejecutivos y Visor de informes.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: fb06a863218446b0e88b38af242b4dac044560c0
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565311"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a>Control de acceso basado en rol al panel Centro de partners Insights

**Roles adecuados:** administrador global | Agente de administración | Visor de informes | Visor de informes ejecutivos

El panel insights usa dos nuevos roles en Centro de partners para administrar el acceso de los empleados a los informes: Visor de informes ejecutivos y Visor de informes.  Los usuarios del rol Visor de informes ejecutivos tienen acceso a todos los conjuntos de datos de informes, mientras que los usuarios del rol Visor de informes no tendrán acceso a conjuntos de datos confidenciales, como ingresos y datos personales de clientes o empleados.  

Al igual que con otros Centro de partners, el administrador global o el administrador de cuenta podrán asignar usuarios a esos roles en la página Administración de usuarios. Los roles pueden ser aplicables en toda la empresa o para ubicaciones Microsoft Partner Network (MPN) específicas. Los roles asignados para ubicaciones específicas de MPN limitan al usuario a ver los datos de informes asociados solo a las ubicaciones de MPN seleccionadas. El asociado puede seleccionar una o varias ubicaciones en la vista siguiente.

:::image type="content" source="images/pci/roles.png" alt-text="Muestra la configuración de roles de Centro de partners insights específica de la ubicación para el Visor de informes y el Visor de informes ejecutivos.":::

>[!Note]
> Los usuarios que sean administradores de asociados de MPN a partir del 20  de enero de 2020 se agregarán automáticamente al rol Visor de informes ejecutivos de toda la empresa para todas las ubicaciones de ese inquilino. Por lo tanto, estos usuarios pueden acceder a los informes como un visor de informes ejecutivos sin ninguna acción explícita requerida por el administrador global o el administrador de la cuenta. Los administradores globales y los administradores de cuentas pueden invalidar los roles asignados automáticamente de estos usuarios para aumentar o limitar aún más sus capacidades.

## <a name="next-steps"></a>Pasos siguientes

- Obtenga más información [sobre Centro de partners Insights](partner-center-insights.md) y sus distintos informes.
