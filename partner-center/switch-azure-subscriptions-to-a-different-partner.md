---
title: Transferir suscripciones de Azure | Centro de partners
description: Un cliente puede cambiar el partner del programa Proveedor de soluciones en la nube que se usará para los servicios de Microsoft Azure. Sin embargo, este es un proceso manual que requiere acciones de partners y clientes.
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
keywords: suscripción de azure, alternar partner, cambiar partner, obtener nuevo partner, otro partner
ms.openlocfilehash: a4b9c0a320808f1d8a4a630a035660813a3f9c74
ms.sourcegitcommit: 93968695897114a68d5e948d13a36127a4079b6f
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/22/2018
ms.locfileid: "2088962"
---
# <a name="transfer-azure-subscriptions"></a>Transferir suscripciones de Azure 

**Se aplica a**

-  Centro de partners

Un cliente puede decidir cambiarse a un partner del Proveedor de soluciones en la nube u otro partner para los servicios de Microsoft Azure. Sin embargo, este es un proceso manual que requiere acciones del partner y del cliente.

**Nota**  Por el momento, no es posible cambiar los partners de las suscripciones del Proveedor de soluciones en la nube para las suscripciones de Office365, Enterprise Mobility Suite o Microsoft DynamicsCRM.



**Cambia partners para suscripciones de Azure**

1.  Para transferir una suscripción de Azure a un partner nuevo, el cliente debe iniciar el proceso y ponerse en contacto con su partner de registro actual por escrito. 

    >**Nota**<br> Es responsabilidad del partner actual crear el vale de servicio que inicia el proceso de transferencia. Microsoft no puede intervenir en nombre del cliente o del nuevo partner. El cliente debe tener previsto trabajar estrechamente con el partner actual para que la transición se realice sin problemas.

2.  El partner de la suscripción debe realizar las siguientes tareas:

    Crear un vale de servicio de Azure desde el Centro de partners para solicitar una transferencia de suscripción:

    -   En el menú del panel, selecciona **Clientes**, selecciona el cliente de la lista y, a continuación, selecciona **Administración de servicios**. En la sección **Vales de soporte**, selecciona la lista desplegable **Nuevo vale** y elige **Microsoft Azure**.

    -   Desde el portal de Azure, selecciona **Nueva solicitud de soporte técnico**.

        En el paso 1, elige **Administración de suscripciones** como tipo de problema, especifica el Id. de suscripción que quieres transferir y selecciona **Proveedor de soluciones en la nube** como el plan de soporte técnico.

        En el paso 2, selecciona **Impacto mínimo C** y elige **Otras preguntas generales** como el tipo de problema.

        Descarga el [formulario de transferencia de suscripción de CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip).

3.  Para el partner de la suscripción: rellena el [formulario de transferencia de suscripción de CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), fírmalo y luego envíalo al cliente. Para rellenar el formulario, necesitarás la siguiente información:

    -   Información de contacto del partner actual e Id. de Microsoft. En el menú del Centro de partners, selecciona **Configuración de la cuenta** &gt; **Perfil de la organización** y usa el **Id. de Microsoft**, **Nombre de la organización** y **Dirección** que se enumeran ahí.

    -   Id. Microsoft del cliente En el menú del Centro de partners, selecciona **Clientes** y, después, expande la lista del cliente para ver su **Id. Microsoft**.

    -   Id. de suscripción que se va a transferir. En el listado de clientes expandido, selecciona **Ver suscripciones** y luego expande la suscripción seleccionada para ver el **Id. de suscripción**.

    >**Nota**<br> Transferir una suscripción genera dos identificadores de suscripción que verás en la página **Editar suscripción** de la suscripción transferida: **1**- El identificador de suscripción del Centro de partners se usa para fines de facturación. 
    **2**- El id. de suscripción original de Azure se conserva y aparecerá en el Centro de partners, así como en el portal de administración de Azure. Este id. aparecerá en el archivo de conciliación.  **Al registrar vales de soporte técnico, deberás usar ambos id.**

4.  Para el cliente y el nuevo partner para la suscripción:

    Revisa el formulario, rellena la información sobre el nuevo partner y fírmalo. Comprueba que el nuevo cliente tiene un acuerdo contractual en vigor. Vuelve a enviar el formulario al partner de registro actual.

    *Importante*: si el nuevo partner de CSP no tiene una relación de revendedor con el cliente, debe establecer una antes de que se transfiera la suscripción. [Puedes encontrar información sobre cómo hacer esto aquí](request-a-relationship-with-a-customer.md).

5.  Partner actual:

    Asegúrate de que el formulario incluya información de contacto para ambos administradores de partners. Soporte técnico de Microsoft se pondrá en contacto con ambos para comprobar la transferencia. Asegúrate de que las tres firmas estén en su lugar y, a continuación, adjunta el formulario rellenado a la solicitud de servicio existente mediante la opción **Carga de archivos**. Un ingeniero de soporte técnico de Microsoft se pondrá en contacto contigo en un plazo de 8 horas laborales para validar la recepción y la finalización.

6.  Nuevo partner:

    Actualiza la configuración de suscripción de Azure para quitar el partner antiguo de la cuenta. Para ver qué asignaciones de roles están aprovisionadas, ejecuta dos Commandlets de Powershell.

    -   Agrega el nuevo partner como el revendedor de la cuenta:

        **PS C:\\&gt; Add-AzureRMAccount -tenant "CustomerDomainName"**

        Para encontrar el valor de customerDomainName: en el menú del Centro de partners, selecciona **Clientes**. En la lista de clientes, selecciona el cliente. En el menú del cliente, selecciona **Cuenta** y usa el valor de **Nombre de dominio**.

    -   Observa los roles de la cuenta, incluidos los partners CSP anteriores:

        **PS C:\\&gt; Get-AzureRMRoleAssignment**

7. Quitar permisos de acceso obsoletos

    -  En el menú del Centro de partners, selecciona **Clientes**. 
    -  Expande la lista del cliente y selecciona **Ver suscripciones**. 
    -  En el menú del cliente, selecciona **Administración de servicios**. 
    -  En **Microsoft Azure**, haz clic en el vínculo para ir al **Portal de administración de Microsoft Azure**.

 

 



