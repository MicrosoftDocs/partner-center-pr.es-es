---
title: Entidad de servicio de Azure AD
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Averigüe cómo agregar una entidad de servicio al inquilino de Azure AD. Esta acción implica la incorporación de una aplicación de Azure AD (entidad de servicio) en el Centro de partners.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d75c5c7311feaa3ca53139f2abf2702035b1069
ms.sourcegitcommit: 2e206627323ff175c0e0d10646cdba80e9881891
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/29/2020
ms.locfileid: "87365761"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Incorporación de una aplicación de Azure AD (entidad de servicio) en el Centro de partners

**Se aplica a**

- Centro de partners

**Roles adecuados**

- Administrador global

En el programa de Marketplace comercial del Centro de partners, ahora puedes agregar una aplicación de Azure AD (entidad de servicio) como usuario en tu cuenta del Centro de partners. (Antes podía hacerlo en la cuenta de Cloud Partner Portal, o CPP. Ahora que ha migrado al Centro de partners, la cuenta de CPP es de solo lectura).
 
>[!Note] 
>La entidad de servicio es sinónimo de aplicación de Azure AD.

## <a name="add-an-azure-ad-application-service-principal"></a>Incorporación de una aplicación de Azure AD (entidad de servicio)

1. En el panel del Centro de partners, selecciona **Configuración** y, a continuación, selecciona **Configuración de desarrollador**.

2. Selecciona **Usuarios** y, a continuación, **Agregar aplicaciones de Azure AD**.

3. Selecciona una aplicación de Azure AD existente o crea una nueva.

4. Si creas una nueva aplicación de Azure AD, incluye la siguiente información:  

   - **URL de respuesta**: dirección URL en la que los usuarios pueden iniciar sesión para usar la aplicación de Azure AD.

   - **URI de identificación de la aplicación**: identificador lógico para la aplicación de Azure AD que se muestra cuando envía una solicitud de inicio de sesión único a Azure AD.

   - **Roles de seguridad**: Los roles **Administrador** (idéntico al rol "Propietario" en CPP) y **Desarrollador** (el mismo que el rol "Colaborador" en CPP) se aplican al programa de Marketplace comercial del Centro de partners y se pueden asociar a esta aplicación de Azure AD.  

## <a name="next-steps"></a>Pasos siguientes

- [Información general sobre Marketplace comercial del Centro de partners](csp-commercial-marketplace-overview.md)