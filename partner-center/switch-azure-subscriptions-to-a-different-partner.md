---
title: Transferir suscripciones de Azure | Centro de partners
ms.topic: article
ms.date: 10/29/2018
description: Un cliente puede cambiar el partner del programa Proveedor de soluciones en la nube que se usará para los servicios de Microsoft Azure. Sin embargo, este es un proceso manual que requiere acciones de partners y clientes.
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
ms.author: evansma
keywords: suscripción de azure, alternar partner, cambiar partner, obtener nuevo partner, otro partner
ms.localizationpriority: medium
ms.openlocfilehash: f9df7ac6c1e30f9e0d9d62c5e0c18aae529c472a
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584358"
---
# <a name="transfer-azure-subscriptions"></a>Transferir suscripciones de Azure 

**Se aplica a**

-  Centro de partners

Un cliente puede decidir cambiarse a un partner del Proveedor de soluciones en la nube u otro partner para los servicios de Microsoft Azure. Sin embargo, este es un proceso manual que requiere acciones del partner y del cliente.

>[!Note]  
>En este momento sólo Direct o proveedores indirectos pueden transferir suscripciones.
>Por el momento, no es posible cambiar los partners de las suscripciones de Proveedor de soluciones en la nube para las suscripciones de Office 365, Enterprise Mobility Suite o Microsoft Dynamics CRM.



**Asociados de conmutador para suscripciones de Azure**

1. Para transferir una suscripción de Azure a un socio nuevo, el cliente debe iniciar el proceso y ponerse en contacto con su partner de registro actual por escrito. 
>[!Note]
>Es responsabilidad del partner actual crear el vale de servicio que inicia el proceso de transferencia. Microsoft no puede intervenir en nombre del cliente o del nuevo partner. El cliente debe tener previsto trabajar estrechamente con el partner actual para que la transición se realice sin problemas.

2. El partner de la suscripción debe realizar las siguientes tareas:

Crear un vale de servicio de Azure desde el Centro de partners para solicitar una transferencia de suscripción:
-   En el menú del centro de partners, seleccione **clientes**, seleccione el cliente de la lista y, a continuación, seleccione **administración de servicios**. En la sección **Vales de soporte**, selecciona la lista desplegable **Nuevo vale** y elige **Microsoft Azure**.

-   Desde el portal de Azure, selecciona **Nueva solicitud de soporte técnico**.

En el paso 1, elige **Administración de suscripciones** como tipo de problema, especifica el Id. de suscripción que quieres transferir y selecciona **Proveedor de soluciones en la nube** como el plan de soporte técnico.

En el paso 2, selecciona **Impacto mínimo C** y elige **Otras preguntas generales** como el tipo de problema.

Descarga el [formulario de transferencia de suscripción de CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip).

3. El asociado de la suscripción: Rellene el [formulario de transferencia de suscripción de CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), fírmelo y, a continuación, enviarla al cliente. Para rellenar el formulario, necesitarás la siguiente información:

- Información de contacto del partner actual e Id. de Microsoft. En el menú del centro de partners, seleccione **configuración de la cuenta** &gt; **perfil organización**y usar el **Microsoft ID**, **nombre de la organización** , y **dirección** en la lista.

- Id. Microsoft del cliente En el menú del Centro de partners, selecciona **Clientes** y, después, expande la lista del cliente para ver su **Id. Microsoft**.

- Id. de suscripción que se va a transferir. En el listado de clientes expandido, selecciona **Ver suscripciones** y, a continuación, expande la suscripción seleccionada para ver el **Id. de suscripción**.

>[!Note]
>Transferir una suscripción da como resultado dos suscripción identificadores que verá en el **Editar suscripción** página de la suscripción transferida: **1**-el identificador de suscripción de Partner Center se utiliza para fines de facturación. 
**2**- El identificador de suscripción original de Azure se conserva y aparecerá en el Centro de partners, así como en el portal de administración de Azure. Este identificador aparecerán en el archivo de conciliación.  **Cuando el registro de incidencias de soporte técnico, deberá usar ambos identificadores.**

4. Para el cliente y el nuevo partner para la suscripción:

Revisa el formulario, rellena la información sobre el nuevo partner y fírmalo. Comprueba que el nuevo cliente tiene un acuerdo contractual en vigor. Vuelve a enviar el formulario al partner de registro actual.

*Importantes*: Si el nuevo asociado de CSP no tiene una relación de revendedor con el cliente, debe establecer una de ellas antes de la suscripción que se transfieren. [Puedes encontrar información sobre cómo hacer esto aquí](request-a-relationship-with-a-customer.md).

>[!Note]
>El nuevo asociado de CSP y el inquilino del cliente deben estar en el mismo país. 

5. Partner actual:

Asegúrate de que el formulario incluye información de contacto para ambos administradores de partners. Soporte técnico de Microsoft se pondrá en contacto con ambos para comprobar la transferencia. Asegúrate de que las tres firmas estén en su lugar y, a continuación, adjunta el formulario rellenado a la solicitud de servicio existente mediante la opción **Carga de archivos**. Un ingeniero de soporte técnico de Microsoft se pondrá en contacto contigo en un plazo de 8 horas laborales para validar la recepción y la finalización.

6. Nuevo partner:

Actualiza la configuración de suscripción de Azure para quitar el partner antiguo de la cuenta. Para ver qué asignaciones de roles están aprovisionadas, ejecuta dos commandlets de Powershell.

-   Agrega el nuevo asociado como el revendedor de la cuenta:

**PS C:\\&gt; Add-AzureRMAccount-"CustomerDomainName" del inquilino**

Para encontrar el valor de customerDomainName: en el menú del Centro de partners, selecciona **Clientes**. En la lista de clientes, selecciona el cliente. En el menú del cliente, selecciona **Cuenta** y usa el valor de **Nombre de dominio**.

-   Observa los roles de la cuenta, incluidos los asociados de CSP anteriores:

**PS C:\\&gt; Get-AzureRMRoleAssignment**

7. Quitar permisos de acceso obsoletos

-  En el menú del Centro de partners, selecciona **Clientes**. 
-  Expande la lista del cliente y selecciona **Ver suscripciones**. 
-  En el menú del cliente, selecciona **Administración de servicios**. 
-  En **Microsoft Azure**, haz clic en el vínculo para ir al **Portal de administración de Microsoft Azure**.

 

 



