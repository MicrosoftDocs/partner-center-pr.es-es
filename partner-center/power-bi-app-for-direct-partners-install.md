---
title: Instale Centro de partners Analytics para Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Siga los pasos de este artículo para instalar y obtener una vista previa del Aplicación de análisis del Centro de partners para Power BI (para asociados directos en CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 15ee391d6b748b6499700aee321ff4abd85e75d2
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854492"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Instalación y versión preliminar de la Aplicación de análisis del Centro de partners para Microsoft Power BI


**Roles adecuados:** Administrador global | Administrador de administración de | Agente de ventas | Agente de administración

## <a name="before-you-begin"></a>Antes de empezar

Seleccione la aplicación más relevante para su negocio en la siguiente lista de aplicaciones Power BI disponibles:

- [Proveedor directo](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Proveedor indirecto](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Revendedor indirecto](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Antes de instalar la versión preliminar de Centro de partners Analytics, asegúrese de cumplir los siguientes requisitos.

- Elija la aplicación de Power BI correcta para su empresa.

- Tiene una licencia Power BI Pro.

- Tiene permisos para instalar aplicaciones de plantilla en el inquilino.

- Puede iniciar sesión en Power BI.

- Puede iniciar sesión como administrador global, agente de administración o administrador de facturación en el inquilino Azure Active Directory [(Azure AD) de la empresa.](azure-active-directory-tenants-and-partner-center.md)

## <a name="to-install-the-app"></a>Para instalar la aplicación

1. Seleccione el vínculo de origen de la aplicación dado (proveedor directo/proveedor indirecto/revendedor indirecto) en la sección anterior.

2. Seleccionar **Obtenerla ahora**. 

3. Acepte los términos y condiciones seleccionando **Continuar.**

4. En ¿Ya tiene una cuenta? seleccione **Iniciar sesión.**

5. En la página siguiente, escriba el nombre de Power BI y la contraseña y, a continuación, **seleccione Iniciar sesión.**

6. Instale el área de trabajo proporcionando el nombre del área de trabajo.

7. Puede encontrar las aplicaciones de plantilla instaladas en la sección Aplicaciones.

8. Seleccione **Aplicaciones** y elija las aplicaciones instaladas.

9. Se abre la pantalla Introducción a la nueva aplicación.

10. Para conectarse a los datos, seleccione **Conectar.**

11. En la **ventana emergente Conectarse a Centro de partners Analytics,** compruebe que el método de autenticación está establecido en  **oAuth2** o seleccione **oAuth2** en la lista si no lo está. 

> [!NOTE]  
>  Esta ventana puede tardar unos minutos en aparecer.

12. En la **página Centro de partners Analytics Connector,** inicie sesión con las credenciales de administrador global, agente de administración o administrador de facturación para el inquilino de Azure AD de la empresa y, a continuación, seleccione **Iniciar sesión.**
 
13. Cuando se le solicite acceso, seleccione **Aceptar.** 

Una vez que Centro de partners Analytics está conectado a Power BI, los datos comenzarán a cargarse. Dependiendo de la cantidad de datos, esto puede tardar hasta 10 minutos. 

Una vez que los datos terminen de cargarse, puede empezar a usar el panel de la aplicación Centro de partners Analytics y los informes de Power BI.

## <a name="next-steps"></a>Pasos siguientes

[Visualización de los datos empresariales con la aplicación Centro de partners Analytics para Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
