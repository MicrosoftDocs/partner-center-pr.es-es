---
title: Instalación del análisis del centro de partners para Power BI
ms.topic: article
ms.date: 07/10/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Siga los pasos de este artículo para instalar y obtener una vista previa de la aplicación de análisis del centro de partners para Power BI (para asociados directos en CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 754b3310918df9b38129cf1374ae3731d9d8062e
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215856"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Instalación y versión preliminar de la Aplicación de análisis del Centro de partners para Microsoft Power BI


**Roles adecuados**
-   Administrador global
-   Administrador de usuarios
-   Agente de ventas
-   Agente de administrador

## <a name="before-you-begin"></a>Antes de empezar

Seleccione la aplicación más relevante para su empresa en la siguiente lista de aplicaciones Power BI disponibles:
- [Proveedor directo](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.direct_provider_partner_analytics)

- [Proveedor indirecto](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_provider_partner_analytics)

- [Revendedor indirecto](https://appsource.microsoft.com/product/power-bi/partnercenteranalytics.indirect_reseller_partner_analytics)

Antes de instalar la versión preliminar de la aplicación de análisis del centro de Partners, asegúrese de cumplir los siguientes requisitos.

- Elija la aplicación de Power BI correcta para su empresa.

- Tiene una licencia de Power BI Pro.

- Tiene permisos para instalar aplicaciones de plantilla en el inquilino.

- Puede iniciar sesión en Power BI.

- Puede iniciar sesión como administrador global, agente de administración o administrador de facturación en [el inquilino de Azure Active Directory de su empresa (Azure ad)](azure-active-directory-tenants-and-partner-center.md).

## <a name="to-install-the-app"></a>Para instalar la aplicación

1. Haga clic en el vínculo de origen de la aplicación dado (proveedor directo/proveedor indirecto/Revendedor indirecto) en la sección anterior.

2. Haga clic en **obtenerla ahora**. 

3. Para aceptar los términos y condiciones, haga clic en **continuar**.

4. ¿Ya tiene una cuenta? Seleccione **iniciar sesión**.

5. En la página siguiente, escriba el nombre de usuario y la contraseña de Power BI y, a continuación, seleccione iniciar sesión.

6. Instale el área de trabajo proporcionando el nombre del área de trabajo.

7. Puede encontrar las aplicaciones de plantilla instaladas en la sección aplicaciones.

8. Haga clic en aplicaciones y elija las aplicaciones instaladas.

9. Se abre la pantalla de introducción a la nueva aplicación.

10. Para conectarse a los datos, haga clic en **conectar**.

11. En la ventana emergente **conectarse al centro de Partners** , compruebe que el **método de autenticación** está establecido en **OAuth2** o seleccione **OAuth2** en la lista si no lo está. 

> [!NOTE]  
>  Esta ventana puede tardar unos minutos en aparecer.

12. En la página del **conector del centro de Partners** , inicie sesión con las credenciales de administrador global, agente de administración o de facturación del inquilino de Azure ad de su empresa y, a continuación, seleccione **iniciar sesión**.
 
13. Cuando se le pida acceso, seleccione **Aceptar**. 

Una vez que el servicio de análisis de Partner Center está conectado a Power BI, los datos comenzarán a cargarse. En función de la cantidad de datos, esto puede tardar hasta 10 minutos. 

Una vez que los datos terminen de cargarse, puede empezar a usar el panel de la aplicación del centro de Partners y los informes en Power BI.

## <a name="next-steps"></a>Pasos siguientes

[Vea los datos empresariales con la aplicación de análisis del centro de partners para Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
