---
title: Azure Cost Management de Cloudyn para partners de CSP | Centro de partners
description: Azure Cost Management de Cloudyn requiere acceso aprovisionado a la API del Centro de partners.
author: Janet
Keywords: Azure cost management app, manage costs, web apps
robots: ''
ms.openlocfilehash: 01553b850d5839d721de5406c3f1c63094f76bd6
ms.sourcegitcommit: 32f34476cbcae58651baab15d3f5591d6ef70d27
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/08/2018
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>Aplicación de administración de costos de Azure para partners de CSP de Azure  

**Se aplica a**

-  Centro de partners

[Obtener más información sobre Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Antes de comenzar
Antes de poder usar Azure Cost Management, asegúrate de que cumples los siguientes requisitos:
- Eres partner en el programa de Proveedor de soluciones en la nube.
- Tienes capacidad para crear una aplicación web de API del Panel de partners.

## <a name="overview"></a>Introducción

Azure Cost Management de Cloudyn es una aplicación web que permite realizar un seguimiento y administrar el número de clientes que están usando Azure y los costos de dicho uso. Puedes usarla a través de la API del Panel de partners.

## <a name="register-your-web-app-in-the-partner-dashboard"></a>Registrar tu aplicación web en el Panel de partners
Al registrar una aplicación web de Azure Active Directory en el Panel de partners, habilitas el acceso a la API del Panel de partners. 
1.  Inicia sesión en el [Panel de partners](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) con una [cuenta de agente de administración o de administrador global](create-user-accounts-and-set-permissions.md).
2.  En el **Panel**, selecciona **Configuración de la cuenta** &gt; **[Administración de aplicaciones](https://partnercenter.microsoft.com/en-us/pcv/apiintegration/appmanagement)**.
3.  En la sección **Aplicación web**, haz clic en **Agregar nueva aplicación web**.
<br> **Nota**: si ya has creado una aplicación web, puedes omitir el paso 3.
4.  Copia y guarda el GUID de **ID de comercio** y el GUID de **ID de aplicación** para tu aplicación web. Necesitarás ambos identificadores para usar la versión de evaluación gratuita de 30 días de la aplicación Azure Cost Management.

## <a name="add-a-secret-key-to-your-app"></a>Agregar una clave secreta a la aplicación
1.  En la lista desplegable situada junto al botón **Agregar clave**, selecciona una duración de 1 o 2 años.
2.  Haz clic en **Agregar clave**. 
3.  Copia y guarda el valor de la clave secreta. Lo necesitarás para la evaluación gratuita de 30 días.
<br>**Nota**: las claves secretas de la aplicación son como contraseñas con fechas de caducidad más largas. Guarda el valor de clave en una ubicación segura para uso futuro.

## <a name="next-steps"></a>Pasos siguientes
Inicia una [evaluación gratuita de 30 días](https://go.microsoft.com/fwlink/?linkid=857895).
Necesitas la siguiente información para iniciar la prueba:
- Credenciales de inicio de sesión del Panel de partners
- GUID de ID de comercio
- GUID de ID de aplicación
- Valor de clave secreta de aplicación
