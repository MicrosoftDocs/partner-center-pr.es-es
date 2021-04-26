---
title: Transferencia de una suscripción de Azure a otro asociado
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprenda a cambiar el asociado del Proveedor de soluciones en la nube asociado a las suscripciones de Azure de un cliente.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: b21bfcae4472763c19481ad506ae1c72d238e8f0
ms.sourcegitcommit: 26e6b470756aa9c1b3b0b919301b0eb38a335a52
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/26/2021
ms.locfileid: "108002914"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Aprenda cómo transferir las suscripciones de Azure de un cliente a otro asociado.

**Se aplica a**

- Centro de partners para Microsoft Cloud for US Government

**Roles adecuados**

- Administrador global

En este artículo se describe cómo un cliente puede cambiar sus servicios Microsoft Azure de un Proveedor de soluciones en la nube (CSP) a otro.

Para cambiar los servicios o suscripciones de Azure de un cliente a otro asociado, siga estos pasos manuales. Tanto el asociado como el cliente deben completar los pasos.

>[!Note]  
>Actualmente, solo los proveedores directos o indirectos pueden transferir suscripciones.
>No se pueden cambiar los asociados Proveedor de soluciones en la nube suscripciones asociadas con el plan de Azure, Office 365, Enterprise Mobility Suite o suscripciones de Microsoft Dynamics CRM.

## <a name="switch-partners-for-azure-subscriptions"></a>Cambia partners para suscripciones de Azure

1. Para transferir una suscripción de Azure a un socio nuevo, el cliente debe iniciar el proceso y ponerse en contacto con su partner de registro actual por escrito.

   >[!Note]
   > Es responsabilidad del asociado actual crear el vale de servicio que inicia el proceso de transferencia. Microsoft no puede intervención en nombre del cliente o del nuevo asociado. El cliente debe planear trabajar en estrecha colaboración con el asociado actual para que la transición se realice sin problemas.

2. El asociado de la suscripción debe realizar las siguientes tareas:

   Crear un vale de servicio de Azure desde el Centro de partners para solicitar una transferencia de suscripción:

   1. En el Centro de partners, seleccione **Clientes,** seleccione el cliente en la lista y, a continuación, **seleccione Administración de servicios.**

   2. En la sección **Vales de soporte**, selecciona la lista desplegable **Nuevo vale** y elige **Microsoft Azure**.
   
   3. En la [Azure Portal](https://portal.azure.com), seleccione **Nueva solicitud de soporte técnico.**
   
   4. En el paso 1, elija **Administración** de suscripciones como tipo de problema, especifique el identificador de suscripción que desea transferir y elija Proveedor de soluciones en la nube **como** plan de soporte técnico.
   
   5. En el paso 2, seleccione **Impacto mínimo** de C y elija **Otras** preguntas generales como tipo de problema.
   
   6. Descargue el [formulario de transferencia de suscripciones de CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC).

3. Asociado de la suscripción: rellene el formulario de transferencia de suscripción [de CSP,](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)regístrelo y envíelo al cliente. 

   Para rellenar el formulario, necesitarás la siguiente información:

   - Información de contacto del partner actual e Id. de Microsoft. En el menú del Centro de partners, selecciona **Configuración de la cuenta** &gt; **Perfil de la organización** y usa el **Id. de Microsoft**, **Nombre de la organización** y **Dirección** que se enumeran ahí.

   - Identificador de Microsoft del cliente. En el menú del Centro de partners, selecciona **Clientes** y, después, expande la lista del cliente para ver su **Id. Microsoft**.

   - Id. de suscripción que se va a transferir. En el listado de clientes expandido, selecciona **Ver suscripciones** y, a continuación, expande la suscripción seleccionada para ver el **Id. de suscripción**.

   >[!Note]
   >La transferencia de una suscripción da como resultado  dos identificadores de suscripción que verá en la página Editar suscripción de la suscripción transferida: **1:** el identificador de suscripción Centro de partners se usa con fines de facturación. **2**- El identificador de suscripción de Azure original se conserva y aparecerá en Centro de partners, así como en el Portal de administración de Azure. Este identificador aparecerá en el archivo de conciliación.  **Al registrar vales de soporte técnico, debe usar ambos.**

4. El cliente y el nuevo asociado de la suscripción:

   Revisa el formulario, rellena la información sobre el nuevo partner y fírmalo. Comprueba que el nuevo cliente tiene un acuerdo contractual en vigor. Vuelve a enviar el formulario al partner de registro actual.

   *Importante:* Si el nuevo asociado de CSP no tiene una relación de revendedor con el cliente, debe establecer una antes de transferir la suscripción. [Puedes encontrar información sobre cómo hacer esto aquí](request-a-relationship-with-a-customer.md).

   >[!Note]
   >El nuevo asociado de CSP y el inquilino del cliente deben estar en el mismo país. 

5. Asociado actual:

   Asegúrese de que el formulario incluye información de contacto para ambos administradores de asociados. Soporte técnico de Microsoft contacto con ambos administradores para comprobar la transferencia. Asegúrese de que tiene las tres firmas. A continuación, **use la opción Carga** de archivos para adjuntar el formulario completado a la solicitud de servicio existente. Un ingeniero de soporte técnico de Microsoft se pondrá en contacto con usted en un plazo de ocho horas laborables para validar la recepción y la finalización.

6. Nuevo asociado:

   Actualiza la configuración de suscripción de Azure para quitar el partner antiguo de la cuenta. Para ver qué asignaciones de roles se aprovisionan, ejecute dos Commandlets de PowerShell.

   - Agrega el nuevo asociado como el revendedor de la cuenta:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > El identificador de inquilino **del cliente** aparece en Centro de partners como el identificador de Microsoft **del cliente.** Para buscar el identificador de Microsoft (id. de inquilino) de un cliente específico, inicie sesión en Centro de partners [panel](https://partner.microsoft.com/dashboard). A **continuación, seleccione** Clientes en el menú. Busque el cliente en la lista. Seleccione la flecha abajo para expandir la lista del cliente. Verá información sobre el nombre de dominio del cliente *y* el identificador de **Microsoft del cliente.** Use el identificador de **Microsoft** de 16 dígitos en el commandlet de PowerShell.

   - Observa los roles de la cuenta, incluidos los asociados de CSP anteriores:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Quitar permisos de acceso obsoletos:

   - En el menú del Centro de partners, selecciona **Clientes**.
   - Busque el cliente en la lista. Seleccione (haga doble clic) en el nombre de la compañía. Esta acción abre la página **Suscripciones del** cliente.
   - En el menú de detalles del cliente, seleccione **Administración de servicios.**
   - En **Microsoft Azure**, seleccione el vínculo para ir **al** Portal de administración de Microsoft Azure .

## <a name="next-steps"></a>Pasos siguientes

- Descargue el [formulario de transferencia de suscripciones de CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).

- Obtenga información sobre [la compatibilidad con varios asociados.](multipartner.md)

- [compatibilidad con varios asociados.](multipartner.md)
- [compatibilidad con varios canales.](multichannel.md)
- [Transferir suscripciones de Azure](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)