---
title: Azure Cost Management de Cloudyn para partners de CSP | Centro de partners
description: Azure Cost Management de Cloudyn requiere acceso aprovisionado a la API del Centro de partners.
author: Janet
Keywords: Azure cost management app, manage costs, web apps
robots: 
ms.openlocfilehash: 3d122e0f88867d16df3713f79e735126b7f40dd4
ms.sourcegitcommit: 628443b08dde9d2f02553b46e669504c620c3da4
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/21/2017
---
# <a name="azure-cost-management-app-for-azure-csp-partners"></a>Aplicación de administración de costos de Azure para partners de CSP de Azure  

**Se aplica a**

-  Centro de partners

[Obtener más información sobre Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Antes de comenzar
Antes de poder usar Azure Cost Management, asegúrate de que cumples los siguientes requisitos:
- Eres partner en el programa de Proveedor de soluciones en la nube.
- Tienes la capacidad para crear una aplicación web de API del Centro de partners.

## <a name="overview"></a>Introducción

Azure Cost Management de Cloudyn es una aplicación web que permite realizar un seguimiento y administrar el número de clientes que están usando Azure y los costos de dicho uso. Puedes usarla a través de la API del Centro de partners.

## <a name="register-your-web-app-in-partner-center"></a>Registrar tu aplicación web en el Centro de partners
Al registrar una aplicación web de Azure Active Directory en el Centro de partners se habilita el acceso a la API del centro de partners. 
1.  Inicia sesión en [Centro de partners](https://partnercenter.microsoft.com/en-us/pcv/dashboard/overview) con una [cuenta de agente de administración o administrador global](create-user-accounts-and-set-permissions.md).
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
- Credenciales para conectarse al Centro de datos
- GUID de ID de comercio
- GUID de ID de aplicación
- Valor de clave secreta de aplicación
