---
title: Administración de suscripciones y recursos en el plan de Azure | Centro de partners
ms.topic: article
ms.date: 10/04/2019
description: Compra de varias suscripciones de Azure sin tener que enviar pedidos individuales para cada suscripción
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.openlocfilehash: 5aa39cbecc7f468329c9a5234dd975c776a63ea6
ms.sourcegitcommit: dcc2a2077ef17255ecf7a2fa5fae6bbeefaa9eb0
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/07/2019
ms.locfileid: "71997865"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Administración de suscripciones y recursos en el plan de Azure

Al realizar la transición de un cliente al plan de Azure, se le asignan derechos de administrador con privilegios en Azure (derechos de propietario de la suscripción a través de administración en nombre de) de manera predeterminada.

 > [!NOTE]
 > El cliente puede eliminar los derechos de administrador en la suscripción de Azure en un nivel de suscripción, grupo de recursos o carga de trabajo. 

 Los partners pueden obtener administración y control operativo ininterrumpidos de los recursos de Azure de un cliente en CSP mediante el uso de diferentes opciones que se proporcionan a través de la característica de control de acceso basado en roles (RBAC). 

- **Administración en nombre de (AOBO)** : con AOBO, cualquier usuario con el rol de agente de administración en el inquilino del partner tendrá acceso de propietario de RBAC a las suscripciones de Azure que cree a través del programa CSP.

- **Azure Lighthouse**: AOBO no permite la flexibilidad de crear grupos distintos que funcionen con diferentes clientes ni habilitar diferentes roles para grupos o usuarios. Con Azure Lighthouse, puede asignar grupos diferentes a distintos clientes o roles. Dado que los usuarios tendrán el nivel de acceso adecuado a través de la administración de recursos delegados de Azure, puede reducir el número de usuarios que tienen el rol de agente de administración (y, por tanto, que tienen acceso total a AOBO). Esto ayuda a mejorar la seguridad al limitar el acceso innecesario a los recursos de los clientes. También ofrece más flexibilidad para administrar varios clientes a escala. Para obtener más información, consulte [Azure Lighthouse y el programa Proveedor de soluciones en la nube](https://docs.microsoft.com/azure/lighthouse/concepts/cloud-solution-provider).

-  **Usuarios invitados o de directorio o [Entidades de servicio](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)** : Puede delegar el acceso granular a las suscripciones de CSP agregando usuarios en el directorio del cliente o agregando usuarios invitados y asignando roles de RBAC específicos. 

Microsoft recomienda que los usuarios tengan los permisos mínimos que necesitan para realizar su trabajo como práctica de seguridad. Consulte [Recursos de Azure Active Directory Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure). 

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a>Vinculación del id. de partner (identificador de MPN) con las credenciales para administrar los recursos de Azure del cliente

En la tabla siguiente se muestran los métodos que se usan para asociar el id. de partner con diversas opciones de acceso RBAC.

|**Categoría**   |**Escenario**   |**Asociación del id. de MPN**|
|-----------------|:------------------------|:------------------|
|AOBO   |El proveedor indirecto o partner directo de CSP crea la suscripción del cliente, lo que convierte al proveedor indirecto o partner directo de CSP en el propietario predeterminado de la suscripción mediante AOBO. El partner directo de CSP o el proveedor indirecto proporcionan acceso de revendedor indirecto a la suscripción mediante AOBO.|Automática (no se requiere ningún trabajo por parte del partner)|
|Azure Lighthouse|El partner crea una nueva [oferta de Servicios administrados en Marketplace](https://docs.microsoft.com/azure/lighthouse/concepts/managed-services-offers). Esta oferta se acepta en la suscripción de CSP y el partner obtiene acceso a la suscripción de CSP.|Automática (no se requiere ningún trabajo por parte del partner)|
|Azure Lighthouse|El partner implementa la [plantilla de ARM](https://docs.microsoft.com/azure/lighthouse/how-to/onboard-customer) en la suscripción de Azure.|El partner debe asociar el id. de MPN con el usuario o la entidad de servicio en el inquilino del partner. Para obtener más información, consulte [Vinculación de un Id. de partner](https://docs.microsoft.com/en-us/azure/billing/billing-partner-admin-link-started).|
|Usuario invitado o de directorio|El partner crea un nuevo usuario o una entidad de servicio en el directorio del cliente y concede al usuario acceso a la suscripción de CSP. El partner crea un nuevo usuario o una entidad de servicio en el directorio del cliente. El partner agrega el usuario a un grupo y concede al grupo acceso a la suscripción de CSP.|El partner debe asociar el id. de MPN con el usuario o la entidad de servicio en el inquilino del cliente. Para obtener más información, consulte [Vinculación de un Id. de partner](https://docs.microsoft.com/en-us/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Confirmación de que tiene acceso de administrador

Necesita acceso de administrador para administrar los servicios del cliente y recibir los créditos obtenidos. Consulte [Partner earned credits](partner-earned-credit.md) (Créditos obtenidos del partner) para obtener información detallada sobre los créditos obtenidos. Tiene dos maneras de asegurarse de que sabe que tiene acceso de administrador.

- Revise el archivo de uso diario: esto se puede determinar mediante la revisión del precio unitario y el precio unitario efectivo en el archivo de uso diario y la confirmación de si se está aplicando un descuento. Si recibe el descuento, significa que es el administrador.

- Cree una alerta de Azure Monitor: puede crear una [alerta](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) de registro de actividad de Azure Monitor para que se le notifique cuando se quite el acceso de RBAC de la suscripción de CSP.

### <a name="create-an-azure-monitor-alert"></a>Creación de una alerta de Azure Monitor

1. Cree la alerta.

![Alerta de Azure](images/azure/azurealert1.png)

2. Seleccione el tipo de acción que quiere que lleve a cabo la alerta. Por ejemplo, si especifica que quiere un correo electrónico, recibirá un mensaje de correo electrónico en el que se le notificará si se elimina alguna asignación de roles.

![Configuración de la alerta](images/azure/azureconfigurealert2.png)

### <a name="aobo-removal"></a>Eliminación de AOBO

Los clientes pueden administrar el acceso a sus suscripciones si van a **Control de acceso** en Azure Portal. En la pestaña **Asignaciones de roles**, se selecciona **Eliminar acceso**. Si es así, puede:

- Hable con el cliente para ver si se puede restablecer el acceso de administrador.
- Use el acceso proporcionado a través del [control de acceso basado en roles (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview).
- Use el acceso proporcionado a través de [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).

El acceso basado en roles difiere del acceso de administrador. Los roles delimitan exactamente lo que puede y no puede hacer. El acceso de administrador es más amplio.

Para ver los roles que son válidos para obtener PEC (créditos obtenidos del partner), consulte [Roles y permisos para los créditos obtenidos del partner](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2).

**Para obtener más información**

- [Partner earned credit - overview](partner-earned-credit.md) (Créditos obtenidos del partner: introducción)

- [Partner earned credit for managed services](partner-earned-credit-explanation.md) (Créditos obtenidos del partner para servicios administrados)