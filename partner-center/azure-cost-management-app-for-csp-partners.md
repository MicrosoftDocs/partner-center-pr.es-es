---
title: Azure Cost Management de Cloudyn para partners de CSP | Centro de partners
ms.topic: article
ms.date: 03/15/2019
description: Azure Cost Management de Cloudyn requiere acceso aprovisionado a la API del Centro de partners.
author: Janet
ms.author: janet
Keywords: Aplicación de administración de costos de Azure, administración de costos, Web Apps
robots: ''
ms.localizationpriority: medium
ms.openlocfilehash: 27ff91d9d42f08e44f812663f3d4409e1080d580
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820304"
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>Aplicación de administración de costos de Azure para partners de CSP de Azure  

**Se aplica a**

-  Centro de partners

[Obtener más información sobre Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Antes de empezar
Antes de poder usar Azure Cost Management, asegúrate de que cumples los siguientes requisitos:

- Eres partner en el programa de Proveedor de soluciones en la nube.
- Tienes la capacidad para crear una aplicación web de API del Centro de partners.

## <a name="overview"></a>Información general

Cloudyn es una aplicación web que le permite realizar un seguimiento y administrar la cantidad de clientes que usan Azure y los costos de ese uso. Puedes usarla a través de la API del Centro de partners.

## <a name="register-your-web-app-in-the-partner-center"></a>Registrar tu aplicación web en el Centro de partners
Al registrar una aplicación web de Azure Active Directory en el Centro de partners se habilita el acceso a la API del Centro de partners. 
1.  Inicia sesión en el [Centro de partners](https://partnercenter.microsoft.com/pcv/dashboard/overview) con una [cuenta de agente de administración o administrador global](create-user-accounts-and-set-permissions.md).
2.  En el **centro de Partners**, seleccione **configuración** &gt; de la cuenta **[Administración de aplicaciones](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)** .
3.  En la sección **Aplicación web**, haz clic en **Agregar nueva aplicación web**.
<br> **Nota**: Si ya ha creado una aplicación Web, puede omitir el paso 3.
4.  Copia y guarda el GUID de **ID de comercio** y el GUID de **ID de aplicación** para tu aplicación web. Necesitarás ambos identificadores para usar la versión de evaluación gratuita de 30 días de la aplicación Azure Cost Management.

## <a name="add-a-secret-key-to-your-app"></a>Agregar una clave secreta a la aplicación
1. En la lista desplegable situada junto al botón **Agregar clave**, selecciona una duración de 1 o 2 años.
2. Haz clic en **Agregar clave**. 
3. Copia y guarda el valor de la clave secreta. Lo necesitarás para la evaluación gratuita de 30 días.<br>
   > [!NOTE]  
   > Las claves secretas de aplicación son similares a las contraseñas con fechas de expiración más largas. Guarda el valor de clave en una ubicación segura para uso futuro.

## <a name="next-steps"></a>Pasos siguientes
Inicia una [evaluación gratuita de 30 días](https://go.microsoft.com/fwlink/?linkid=857895).
Necesitas la siguiente información para iniciar la prueba:
- Credenciales para conectarse al Centro de datos
- GUID de ID de comercio
- GUID de ID de aplicación
- Valor de clave secreta de aplicación
