---
title: Azure Cost Management por Cloudyn para CSP
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo registrar la aplicación Web de Cloudyn y usar una clave secreta para ella en el centro de partners para que pueda usar la aplicación para realizar un seguimiento del uso y los costos de Azure de los clientes.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4ea156ef0932fe1af20f3e3c4b9be1a5f931cdde
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435914"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a>Realice un seguimiento del uso y los costos de Azure de los clientes con la aplicación Azure cost Management para asociados de CSP  

**Se aplica a**

- Centro de partners
- Partners del programa Proveedor de soluciones en la nube

**Roles adecuados**

- Administrador global
- Agente de administrador

[Obtener más información sobre Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Antes de empezar
Antes de poder usar Azure Cost Management, asegúrese de cumplir los siguientes requisitos:

- Usted es un asociado en el programa proveedor de soluciones en la nube.
- Tiene la capacidad de crear una aplicación Web de API del centro de Partners.

## <a name="overview"></a>Información general

Cloudyn es una aplicación web que le permite realizar un seguimiento y administrar la cantidad de clientes que usan Azure y los costos de ese uso. Se usa a través de la API del centro de Partners.

## <a name="register-your-web-app-in-the-partner-center"></a>Registro de la aplicación web en el centro de Partners
Al registrar una aplicación Web de Azure Active Directory en el centro de Partners, se habilita el acceso a la API del centro de Partners. 
1.  Inicie sesión en [el centro de Partners](https://partnercenter.microsoft.com/pcv/dashboard/overview) con una [cuenta de administrador global o de agente de administración](create-user-accounts-and-set-permissions.md).
2.  En el **centro de Partners**, seleccione Configuración de la **cuenta** &gt; **[Administración de aplicaciones](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.
3.  En la sección **aplicación web** , haga clic en **Agregar nueva aplicación web**.
<br> **Nota**: Si ya ha creado una aplicación Web, puede omitir el paso 3.
4.  Copie y guarde el GUID de ID. de **Commerce** y el GUID de ID. de **aplicación** para la aplicación Web. Necesitará ambos identificadores para usar la evaluación gratuita de 30 días de la aplicación Azure cost Management.

## <a name="add-a-secret-key-to-your-app"></a>Agregar una clave secreta a la aplicación
1. En el menú desplegable situado junto al botón **Agregar clave** , seleccione una duración de 1 o 2 años.
2. Haga clic en **Agregar clave**. 
3. Copie y guarde el valor de la clave secreta. Lo necesitará para la evaluación gratuita de 30 días.<br>
   > [!NOTE]  
   > Las claves secretas de aplicación son similares a las contraseñas con fechas de expiración más largas. Guarde el valor de clave en una ubicación segura para su uso futuro.

## <a name="next-steps"></a>Pasos siguientes
Inicie una [evaluación gratuita de 30 días](https://go.microsoft.com/fwlink/?linkid=857895).
Necesita los siguientes detalles para iniciar la versión de prueba:
- Credenciales de inicio de sesión del centro de Partners
- GUID de ID. de Commerce
- GUID de ID. de aplicación
- Valor de clave secreta de aplicación
