---
title: Inscribirse en el programa proveedor de soluciones en la nube para Microsoft Cloud para el gobierno de EE. UU. | Centro de partners para Microsoft Cloud para el gobierno de EE. UU.
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Antes de inscribirse en el programa proveedor de soluciones en la nube para Microsoft Cloud para el gobierno de EE. UU., obtenga más información sobre los requisitos del programa CSP.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 9b9de82652543843b09dfdb00829c7911c20c572
ms.sourcegitcommit: faf7b1ac1653497f963b428bbfafcd821378adaa
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/05/2020
ms.locfileid: "82798373"
---
# <a name="enroll-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>Inscribirse en el programa proveedor de soluciones en la nube para Microsoft Cloud para el gobierno de EE. UU.

**Se aplica a**

- Centro de partners para Microsoft Cloud for US Government

**Roles adecuados**

- Administrador global

Los asociados de Microsoft ahora pueden vender soluciones y servicios en la nube de Microsoft a entidades federales, estatales, locales y de tribal de EE. UU. a través del programa proveedor de soluciones en la nube (CSP) para Microsoft Cloud para el gobierno de EE. UU. 

Microsoft Cloud para el gobierno de EE. UU. proporciona una instancia privada, dedicada y aislada de Microsoft Azure que cumple los requisitos del gobierno de EE. UU. para la seguridad, la privacidad y el cumplimiento de los datos. Su empresa debe cumplir los requisitos de elegibilidad de Microsoft para participar en el programa CSP para Microsoft Cloud para el gobierno de EE. UU. Para obtener más información, consulte [Partner Center for Microsoft Cloud para la administración pública de EE. UU.](partner-center-for-microsoft-us-govt-cloud.md)

## <a name="before-you-begin"></a>Antes de comenzar

Antes de que pueda inscribirse en el programa CSP para Microsoft Cloud para el gobierno de EE. UU., es necesario comprobar que su empresa cumple los requisitos para vender a entidades gubernamentales de EE. UU. Antes de comenzar el proceso de inscripción, complete el [formulario de validación de la nube de Microsoft Government](https://azuregov.microsoft.com/csp) para que podamos comprobar la elegibilidad de su empresa. Después de comprobar la elegibilidad de su empresa, le proporcionaremos un inquilino de Azure Active Directory (Azure AD) específico para el Microsoft Cloud para el gobierno de EE. UU.  

Para crear una cuenta del centro de Partners e inscribirse en CSP para Microsoft Cloud para el gobierno de EE. UU., deberá proporcionar la siguiente información (es posible que desee recopilar esta información antes de comenzar el proceso de inscripción):

-  Credenciales de administrador global para el nuevo inquilino de Azure AD de su organización para Microsoft Cloud para el gobierno de EE. UU.
-  IDENTIFICADOR de Microsoft Partner Network de su organización (MPN) 
-  Una dirección de negocio en el Estados Unidos

> [!IMPORTANT]  
> Si tiene una cuenta existente en el centro de Partners y desea inscribirse en CSP para Microsoft Cloud para el gobierno de EE. UU., debe crear una cuenta nueva e independiente específica para el mercado de la administración pública de Estados Unidos.

## <a name="how-to-enroll"></a>Cómo inscribirse 

### <a name="step-1---create-a-partner-center-account-for-microsoft-cloud-for-us-government"></a>Paso 1: creación de una cuenta del centro de partners para Microsoft Cloud para el gobierno de EE. UU.

1.  Inicia el proceso de inscripción [aquí](https://partnercenter.microsoft.com/register/resellerusgjoinnow). 

2.  Inicie sesión con las credenciales de administrador global del inquilino de Azure AD de su organización para Microsoft Cloud para el gobierno de EE. UU. Si su organización no tiene una cuenta para este portal, puede solicitar una completando el formulario de validación de la [nube de Microsoft Government](https://azuregov.microsoft.com/csp).


### <a name="step-2---apply-to-participate-in-the-cloud-solution-provider-program-for-microsoft-cloud-for-us-government"></a>Paso 2: aplicar a participar en el programa proveedor de soluciones en la nube para obtener Microsoft Cloud para el gobierno de EE. UU.

1.  Rellene la información que falte en el formulario de inscripción, incluidos el identificador de Microsoft Partner Network y los detalles de soporte al cliente de su organización. 

2.  Selecciona **Aceptar y continuar**. La revisión de la solicitud puede llevar varios días. Recibirás un mensaje cuando se haya completado la revisión.

    > [!IMPORTANT]  
    > Al seleccionar **Aceptar y continuar**, está confirmando que está autorizado a actuar en nombre de su organización y está aceptando permitir que Microsoft ejecute una comprobación de crédito en segundo plano antes de revisar la aplicación del proveedor de soluciones en la nube de su organización.


### <a name="step-3---sign-the-reseller-agreement-for-microsoft-cloud-for-us-government"></a>Paso 3: firma del acuerdo de revendedor para Microsoft Cloud para el gobierno de EE. UU.

1. Inicie sesión en el centro de partners para Microsoft Cloud para el gobierno de EE. UU. mediante el vínculo proporcionado en el correo electrónico de aprobación de la aplicación. 

2. En la página del **acuerdo** , lea los términos y, si está de acuerdo, seleccione **Aceptar y continúe** para firmar digitalmente el [acuerdo de revendedor para Microsoft Cloud para el gobierno de EE. UU.](https://go.microsoft.com/fwlink/p/?linkid=843364) Crear la cuenta puede tardar varias horas. Cierre la sesión del centro de partners para Microsoft Cloud para el gobierno de EE. UU. y vuelva a iniciarla más tarde.


### <a name="step-4---assign-users-to-the-admin-agent-role-in-the-microsoft-azure-admin-portal-for-microsoft-cloud-for-us-government"></a>Paso 4: asignación de usuarios al rol de agente de administración en el portal de administración de Microsoft Azure para Microsoft Cloud para el gobierno de EE. UU.

Microsoft Cloud para el gobierno de EE. UU. proporciona una instancia independiente de Microsoft Azure que cumple los estándares de cumplimiento, seguridad y privacidad de la administración pública. Para permitir que los administradores administren usuarios y licencias en el Microsoft Azure Portal, deberá asignar manualmente el rol de agente de administración.

> [!NOTE]  
> Después de asignar usuarios al rol del agente de administración, podrán tener acceso a la lista de clientes en la página **clientes** y [agregar nuevos clientes](add-a-new-customer.md).   

1.  Inicie sesión en el portal de administración de https://portal.azure.us/Microsoft Azure en.

2.  Asigne el rol agente de administración a los usuarios adecuados de la organización. Para ello, necesitará agregar estos usuarios al grupo de **AdminAgent** integrado. Consulte [Administración de los miembros de un grupo en Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-groups-members-azure-portal) para obtener información sobre cómo hacerlo.
 
## <a name="connect-with-us"></a>Conecta con nosotros

- ¿Tiene preguntas? Envíenos un correo electrónico aazgovcsp@microsoft.com

- Únase a nosotros en [Yammer](https://www.yammer.com/cloudpartnercommunity/#/threads/inGroup?type=in_group&feedId=11509777&view=all) 

## <a name="related-topics"></a>Temas relacionados

-  [Centro de partners para Microsoft Cloud for US Government](partner-center-for-microsoft-us-govt-cloud.md)

-  [Administración de usuarios y licencias en el Centro de partners para Microsoft Cloud for US Government](user-management-in-partner-center-for-microsoft-us-govt-cloud.md)


