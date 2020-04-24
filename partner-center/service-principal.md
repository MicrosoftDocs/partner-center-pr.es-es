---
title: Entidad de servicio de Azure AD | Centro de partners
ms.topic: article
ms.date: 12/11/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Incorporación de una entidad de servicio al inquilino de Azure AD
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, Azure plan, service principal, Azure AD application
robots: ''
ms.localizationpriority: High
ms.openlocfilehash: bd74d09445d9a2f1745c518362b26f243f00a777
ms.sourcegitcommit: 449cb8c32880217ad7543712b02a84ae69869289
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2020
ms.locfileid: "75716896"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Incorporación de una aplicación de Azure AD (entidad de servicio) en el Centro de partners

En el programa de Marketplace comercial del Centro de partners, ahora puedes agregar una aplicación de Azure AD (entidad de servicio) como usuario en tu cuenta del Centro de partners. (Ya podías hacerlo anteriormente en la cuenta de Cloud Partner Portal pero, ahora que has migrado al Centro de partners, esa cuenta es de solo lectura). Ten en cuenta que entidad de servicio es sinónimo de aplicación de Azure AD.

## <a name="add-an-azure-ad-application-service-principal"></a>Incorporación de una aplicación de Azure AD (entidad de servicio)

1. En el panel del Centro de partners, selecciona **Configuración** y, a continuación, selecciona **Configuración de desarrollador**.

2. Selecciona **Usuarios** y, a continuación, **Agregar aplicaciones de Azure AD**.

3. Selecciona una aplicación de Azure AD existente o crea una nueva.

4. Si creas una nueva aplicación de Azure AD, incluye la siguiente información:  

  


**URL de respuesta**: Esta es la dirección URL en la que los usuarios pueden iniciar sesión para usar la aplicación de Azure AD. 

**URI de identificación de la aplicación**: Se trata de un identificador lógico para la aplicación de Azure AD que se muestra cuando envía una solicitud de inicio de sesión único a Azure AD. 

**Roles de seguridad**: Los roles **Administrador** (idéntico al rol "Propietario" en CPP) y **Desarrollador** (el mismo que el rol "Colaborador" en CPP) se aplican al programa de Marketplace comercial del Centro de partners y se pueden asociar a esta aplicación de Azure AD.  

  
