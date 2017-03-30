---
title: Cambiar suscripciones de Azure a otro partner | Centro de partners
description: "Un cliente puede cambiar el partner del programa Proveedor de soluciones en la nube que se usará para los servicios de Microsoft Azure. Sin embargo, este es un proceso manual que requiere acciones de partners y clientes."
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
ms.openlocfilehash: ec227dac6f8b0625120bf4b5d1bc76fbeaaae635
ms.sourcegitcommit: 772577c0538a5d5b05d45f0e669697209761ab03
translationtype: HT
---
# <a name="switch-azure-subscriptions-to-a-different-partner"></a>Cambiar las suscripciones de Azure a otro partner

**Se aplica a**

-  Centro de partners

Un cliente puede cambiar el partner del programa Proveedor de soluciones en la nube que se usará para los servicios de Microsoft Azure. Sin embargo, este es un proceso manual que requiere acciones de partners y clientes.

**Nota**  Actualmente no hay ningún proceso automático para clientes de Azure para cambiar de EA, Open u otros programas de licencias a CSP. Este es un proceso manual que requiere acciones de partners y clientes. Asimismo, por el momento no es posible cambiar los partners de las suscripciones de Proveedor de soluciones en la nube para las suscripciones de Office 365, Enterprise Mobility Suite o Microsoft DynamicsCRM.

 

**Cambia partners para suscripciones de Azure**

1.  Para transferir una suscripción de Azure a un partner nuevo, el cliente debe iniciar el proceso y ponerse en contacto con su partner de CSP actual de registro por escrito.

2.  El CSP de la suscripción debe realizar las siguientes tareas:

    Crear un vale de servicio de Azure desde el Centro de partners para solicitar una transferencia de suscripción:

    -   En el menu del panel del Centro de partners, selecciona **Clientes**, selecciona el cliente de la lista y, a continuación, selecciona **Administración de servicios**. En la sección **Vales de soporte**, selecciona la lista desplegable **Nuevo vale** y elige **Microsoft Azure**.

    -   Desde el portal de Azure, selecciona **Nueva solicitud de soporte técnico**.

        En el paso 1, elige **Administración de suscripciones** como tipo de problema, especifica el Id. de suscripción que quieres transferir y selecciona **Proveedor de soluciones en la nube** como el plan de soporte técnico.

        En el paso 2, selecciona **Impacto mínimo C** y elige **Otras preguntas generales** como el tipo de problema.

        Descarga el [formulario de transferencia de suscripción de CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip).

3.  Partner de CSP actual de la suscripción: rellena el [formulario de transferencia de suscripción de CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), fírmalo y, a continuación, envíalo al cliente. Para rellenar el formulario, necesitarás la siguiente información:

    -   Información de contacto del partner actual e Id. de Microsoft. En el menú del Centro de partners, selecciona **Configuración de la cuenta** &gt; **Perfil de la organización** y usa el **Id. de Microsoft**, **Nombre de la organización** y **Dirección** que se enumeran ahí.

    -   Id. Microsoft del cliente En el menú del Centro de partners, selecciona **Clientes** y, después, expande la lista del cliente para ver su **Id. Microsoft**.

    -   Id. de suscripción que se va a transferir. En el listado de clientes expandido, selecciona **Ver suscripciones** y, a continuación, expande la suscripción seleccionada para ver el **Id. de suscripción**.

4.  Cliente y CSP nuevo para la suscripción:

    Revisa el formulario, rellena la información sobre el nuevo partner y fírmalo. Comprueba que el nuevo cliente tiene un acuerdo contractual en vigor. Vuelve a enviar el formulario al partner de registro actual.

    *Importante*: si el nuevo partner de CSP no tiene una relación de revendedor con el cliente, debe establecer una antes de que se transfiera la suscripción. [Puedes encontrar información sobre cómo hacer esto aquí](https://int.msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx).

5.  Partner de CSP actual:

    Asegúrate de que el formulario incluye información de contacto para ambos administradores de partners. Soporte técnico de Microsoft se pondrá en contacto con ambos para comprobar la transferencia. Asegúrate de que las tres firmas estén en su lugar y, a continuación, adjunta el formulario rellenado a la solicitud de servicio existente mediante la opción **Carga de archivos**. Un ingeniero de soporte técnico de Microsoft se pondrá en contacto contigo en un plazo de 8 horas laborales para validar la recepción y la finalización.

6.  Nuevo partner de CSP:

    Actualiza la configuración de suscripción de Azure para quitar el partner antiguo de la cuenta. Para ver qué asignaciones de roles están aprovisionadas, ejecuta dos Commandlets de Powershell.

    -   Agrega el nuevo partner como el revendedor de la cuenta:

        **PS C:\\&gt; Add-AzureRMAccount -tenant "CustomerDomainName"**

        Para encontrar el valor de customerDomainName: en el menú del Centro de partners, selecciona **Clientes**. En la lista de clientes, selecciona el cliente. En el menú del cliente, selecciona **Cuenta** y usa el valor de **Nombre de dominio**.

    -   Observa los roles de la cuenta, incluidos los partners CSP anteriores:

        **PS C:\\&gt; Get-AzureRMRoleAssignment**

    Quita los permisos de acceso obsoletos para la suscripción y los recursos mediante la administración de la suscripción en Azure Portal. En el menú del Centro de partners, selecciona **Clientes**. Expande la lista del cliente y selecciona **Ver suscripciones**. En el menú del cliente, selecciona **Administración de servicios**. En **Microsoft Azure**, haz clic en el vínculo para ir al **Portal de administración de Microsoft Azure**.

 

 



