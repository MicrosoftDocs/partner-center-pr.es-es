---
title: Instalación del análisis del centro de partners para Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Siga los pasos de este artículo para instalar y obtener una vista previa de la aplicación de análisis del centro de partners para Power BI (para asociados directos en CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852583
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e8a8558bad11f641737507f4d76405e9825df516
ms.sourcegitcommit: 2a980b50cf177753c15ebfd7770e14cf6d486cf7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/22/2020
ms.locfileid: "83795873"
---
# <a name="install-and-preview-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Instalación y versión preliminar de la Aplicación de análisis del Centro de partners para Microsoft Power BI

**Se aplica a**

- Centro de partners

**Roles adecuados**
-   Administrador global
-   Administrador de usuarios
-   Agente de ventas
-   Agente de administrador

## <a name="before-you-begin"></a>Antes de comenzar

Seleccione la aplicación más relevante para su empresa en la siguiente lista de aplicaciones Power BI disponibles:
- [Partner directo](https://app.powerbi.com/groups/me/getdata/services/direct-providers-partner-analytics)

- [Socio indirecto](https://app.powerbi.com/groups/me/getdata/services/indirect-providers-partner-analytics)

- [Revendedor indirecto](https://app.powerbi.com/groups/me/getdata/services/indirect-seller-partner-analytics)

Antes de instalar la versión preliminar de la aplicación de análisis del centro de Partners, asegúrese de cumplir los siguientes requisitos.

- Elija la aplicación de Power BI correcta para su empresa.

- Tiene una suscripción activa a Microsoft Power BI Professional o Microsoft Power BI Premium.

- Puede iniciar sesión en Power BI.

- Puede iniciar sesión como administrador global, agente de administración o administrador de facturación en [el inquilino de Azure Active Directory de su empresa (Azure ad)](azure-active-directory-tenants-and-partner-center.md).

## <a name="to-install-the-app"></a>Para instalar la aplicación

1. Inicie [el proceso de instalación](https://app.powerbi.com/getdata/services/partneranalytics?cpcode=PartnerCenterAnalytics&getDataForceConnect=true&alwaysPromptForContentProviderCreds=true).

2. En **¿ya tiene una cuenta?** , seleccione **iniciar sesión**. 

3. En la página siguiente, escriba el nombre de usuario y la contraseña de Power BI y, a continuación, seleccione **iniciar sesión**. 

4. En la ventana emergente **conectarse al centro de Partners** , compruebe que el **método de autenticación** está establecido en **OAuth2** o seleccione **OAuth2** en la lista si no lo está. 

> [!NOTE]  
>  Esta ventana puede tardar unos minutos en aparecer.

5. En la página del **conector del centro de Partners** , inicie sesión con las credenciales de administrador global, agente de administración o de facturación del inquilino de Azure ad de su empresa y, a continuación, seleccione **iniciar sesión**.
 
6. Cuando se le pida acceso, seleccione **Aceptar**. 

Una vez que el servicio de análisis de Partner Center está conectado a Power BI, los datos comenzarán a cargarse. En función de la cantidad de datos, esto puede tardar hasta 10 minutos. 

Una vez que los datos terminen de cargarse, puede empezar a usar el panel de la aplicación del centro de Partners y los informes en Power BI.

## <a name="next-steps"></a>Pasos siguientes

[Vea los datos empresariales con la aplicación de análisis del centro de partners para Microsoft Power BI](power-bi-app-for-direct-partners-use.md)
