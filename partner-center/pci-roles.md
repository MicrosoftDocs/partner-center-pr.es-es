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
ms.openlocfilehash: a6af9c7d674d1956332a564628b6b2ea0b1796f6
ms.sourcegitcommit: 078eac1456f68585ff1003b21e5e1fe777af314b
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/28/2021
ms.locfileid: "108120790"
---
# <a name="role-based-access-control-to-the-partner-center-insights-dashboard"></a><span data-ttu-id="d1bb6-104">Control de acceso basado en rol al panel Centro de partners Insights</span><span class="sxs-lookup"><span data-stu-id="d1bb6-104">Role-based access control to the Partner Center Insights dashboard</span></span>

<span data-ttu-id="d1bb6-105">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="d1bb6-105">**Appropriate roles**</span></span>

- <span data-ttu-id="d1bb6-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d1bb6-106">Global admin</span></span>
- <span data-ttu-id="d1bb6-107">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="d1bb6-107">Admin agent</span></span>
- <span data-ttu-id="d1bb6-108">Visor de informes</span><span class="sxs-lookup"><span data-stu-id="d1bb6-108">Report viewer</span></span>
- <span data-ttu-id="d1bb6-109">Visor de informes ejecutivos</span><span class="sxs-lookup"><span data-stu-id="d1bb6-109">Executive report viewer</span></span>

<span data-ttu-id="d1bb6-110">El panel insights usa dos nuevos roles en Centro de partners para administrar el acceso de los empleados a los informes: Visor de informes ejecutivos y Visor de informes.</span><span class="sxs-lookup"><span data-stu-id="d1bb6-110">The Insights dashboard uses two new roles in Partner Center to manage employee access to the reports - Executive Report Viewer and Report Viewer.</span></span>  <span data-ttu-id="d1bb6-111">Los usuarios del rol Visor de informes ejecutivos tienen acceso a todos los conjuntos de datos de informes, mientras que los usuarios del rol Visor de informes no tendrán acceso a conjuntos de datos confidenciales, como los ingresos y los datos personales de clientes o empleados.</span><span class="sxs-lookup"><span data-stu-id="d1bb6-111">Users in the Executive Report Viewer role have access to all reporting datasets, while users in the Report Viewer role will not have access to sensitive data sets such as revenue and customer/employee personal data.</span></span>  

<span data-ttu-id="d1bb6-112">Al igual que con otros Centro de partners, el administrador global o el administrador de cuenta podrán asignar usuarios a esos roles en la página Administración de usuarios.</span><span class="sxs-lookup"><span data-stu-id="d1bb6-112">As with other Partner Center roles, the Global admin or the Account admin will be able to assign users to those roles on the User management page.</span></span> <span data-ttu-id="d1bb6-113">Los roles pueden ser aplicables en toda la empresa o para ubicaciones de MPN específicas.</span><span class="sxs-lookup"><span data-stu-id="d1bb6-113">The roles can be applicable across the entire company or for specific MPN location(s).</span></span> <span data-ttu-id="d1bb6-114">Los roles asignados para ubicaciones de MPN específicas limitan al usuario a ver los datos de informes asociados solo a las ubicaciones de MPN seleccionadas.</span><span class="sxs-lookup"><span data-stu-id="d1bb6-114">Roles assigned for specific MPN location(s) limit the user to viewing reporting data associated only with the selected MPN location(s).</span></span> <span data-ttu-id="d1bb6-115">El asociado puede seleccionar una o varias ubicaciones en la vista siguiente.</span><span class="sxs-lookup"><span data-stu-id="d1bb6-115">Partner can select one or multiple locations from the below view.</span></span>

:::image type="content" source="images/pci/roles.png" alt-text="Muestra la configuración de roles de Centro de partners insights específica de la ubicación para el Visor de informes y el Visor de informes ejecutivos.":::

>[!Note]
> <span data-ttu-id="d1bb6-117">Los usuarios que sean administradores de MPN a partir del 20 de enero  de 2020 se agregarán automáticamente al rol Visor de informes ejecutivos de toda la empresa para todas las ubicaciones de ese inquilino.</span><span class="sxs-lookup"><span data-stu-id="d1bb6-117">Users who are MPN admins as of Jan 20th, 2020 are automatically added to the company-wide **Executive Report Viewer** role for all locations for that tenant.</span></span> <span data-ttu-id="d1bb6-118">Por lo tanto, estos usuarios pueden acceder a los informes como un visor de informes ejecutivos sin ninguna acción explícita requerida por el administrador global o el administrador de la cuenta. Los administradores globales y los administradores de cuentas pueden invalidar los roles asignados automáticamente de estos usuarios para aumentar o limitar aún más sus capacidades.</span><span class="sxs-lookup"><span data-stu-id="d1bb6-118">These users are thus able to access the reports as an Executive Report viewer without any explicit action required by Global admin or Account admin. The Global admins and Account admins can override the auto-assigned roles of these users to further increase or limit their capabilities.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d1bb6-119">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d1bb6-119">Next steps</span></span>

- <span data-ttu-id="d1bb6-120">Obtenga más información [sobre Centro de partners Insights](partner-center-insights.md) y sus distintos informes.</span><span class="sxs-lookup"><span data-stu-id="d1bb6-120">Learn more about [Partner Center Insights](partner-center-insights.md) and its various reports.</span></span>
