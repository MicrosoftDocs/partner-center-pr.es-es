---
title: Consolidación de los inquilinos de autorización regional de CSP
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usa estas instrucciones para consolidar los inquilinos para diferentes países o regiones. Esto incluye los pasos para migrar las cuentas de cliente y las suscripciones de cliente.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: LauraBrenner
ms.author: labrenne
keywords: migración de clientes, aprovisionamiento, cuentas de inquilinos, consolidación de inquilinos
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: c2667bf19f73dfb2498cd6f706bd97b595f67a31
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679072"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Instrucciones para la consolidación de inquilinos de autorización regional de CSP

**Se aplica a**

-  Centro de partners
-  Centro de partners para Microsoft Cloud for US Government

**Roles adecuados**

- Administrador global
- Agente de administrador

\[Algunos datos se relacionan con productos de versiones preliminares que pueden modificarse sustancialmente antes de su lanzamiento comercial. Microsoft no ofrece ninguna garantía, expresa o implícita, con respecto a la información aquí proporcionada.\]

Usa estas instrucciones para consolidar los inquilinos para diferentes países o regiones.

>[!NOTE]  
>Debe tener en cuenta todas las suscripciones y los recuentos de puestos de sus clientes aprovisionados desde las cuentas de transición. Volverá a aprovisionar las mismas suscripciones exactas con los mismos recuentos de puestos en la nueva cuenta central de CSP como parte del proceso de migración. Usa la característica de lista de exportación para ayudar a crear una lista de clientes que trasladar al inquilino centralizado. Los partners eligen si consolidar sus inquilinos. Una vez completada la consolidación, los partners no pueden volver a su estado anterior. También es posible que se necesiten acciones del cliente.

## <a name="prepare-for-migration"></a>Preparación para la migración

- Inicie sesión en el **centro de Partners** con la cuenta de **transición** (existente) (aquella en la que va a realizar la transición) y Revise todos los clientes y todos los servicios aprovisionados para esos clientes.

   :::image type="content" source="images/regionalcustomer1.png" alt-text="lista de clientes regionales":::

## <a name="migrate-customer-accounts"></a>Migración de las cuentas de cliente

1. Inicie sesión en el **centro de Partners** con la cuenta de **transición** (nueva) (la que va a migrar) y vaya a la lista de clientes de **clientes**.

2. Selecciona Clientes.

3. Haz clic en **Solicitar una relación de revendedor**. Se te mostrará un mensaje de correo electrónico predeterminado que presentar a tus clientes. Este mensaje contiene una dirección URL con el identificador de organización exclusivo para tu nueva cuenta del centro de partners.

4. **Acción de cliente:** Asegúrate de que todos los clientes activos que deseas migrar visitan esta dirección URL. Al abrir la dirección URL, al cliente se le pedirá que inicie sesión en el portal de Office 365. El cliente iniciará sesión usando el mismo identificador de organización que utilice para acceder a los portales de administración de Azure y de Office 365.

5. Tras iniciar sesión, al administrador Global de la cuenta del cliente se le pedirá que envíe un contrato para conceder privilegios de administrador delegado a la nueva cuenta de CSP. Si acepta, el cliente seleccionará la casilla y autorizará la relación.

Los clientes aparecerán en la lista de clientes del asociado después de haber enviado el contrato, uno por uno.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migración de suscripciones basadas en uso de Office 365 y que no sean de Azure

1. Cuando el cliente haya firmado el contrato, puedes volver a crear sus suscripciones en tu inquilino de partner centralizado.

2. En **centro de Partners** , seleccione **clientes**.

3. Abre el nombre de la compañía del cliente que deseas migrar.

4. Seleccione **Agregar suscripción**.

5. Agrega las suscripciones y el número de puestos correctos desde el catálogo. Verifica los datos con la información proporcionada en las cuentas de partner de **Transición desde**.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="lista de clientes":::

6. Haga clic en **enviar.**

   Ahora los servicios se proporcionan al cliente desde la cuenta de partner de **Transición a**.

7. Repite estos pasos para migrar las suscripciones de todos los demás clientes.

Antes de pasar a la siguiente sección, asegúrate de todas las suscripciones de cliente existente en las cuentas de partner de **Transición desde** se vuelven a aprovisionar en la cuenta de partner de **Transición a**.

> [!NOTE]
> Los asociados deben suspender las suscripciones en la **transición de** la cuenta de inquilino de asociado del centro de Partners el mismo día en que se realiza la transición de esas suscripciones y se configuran en la cuenta de la **transición a** la cuenta de inquilino del asociado en el centro de partners para asegurarse de que no se produce la facturación doble. Se denegarán las solicitudes de soporte técnico referentes a créditos debidas a cualquier superposición en la facturación que se produzca por no deshabilitar correctamente las suscripciones de **Transición desde**.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Deshabilitar las suscripciones de Office 365 en la cuenta de partner de Transición desde

Deshabilitar la suscripción de CSP de las cuentas de partner de **Transición desde** detiene toda facturación futura. No es necesario deshabilitar manualmente las suscripciones de Azure, porque las suscripciones de Azure se deshabilitan automáticamente durante el proceso de migración.

1. Inicie sesión en el **centro de Partners** con la **transición de** la cuenta de CSP y navegue hasta la lista de clientes.

2. Abre al cliente cuyas suscripciones quieras deshabilitar y, a continuación, selecciona la primera oferta que deshabilitar.

3. Establece la suscripción en **suspendida**y, a continuación, haz clic en **enviar**.

   >[!Note]
   >Suspender la suscripción garantiza que no se produzca la facturación.

   La suscripción muestra **suspendida** en la lista de suscripciones.

4. Repite estos pasos para todas las suscripciones del cliente. Comprueba que todas muestran **suspendida.**

5. Selecciona al siguiente cliente de la lista y repite el proceso de deshabilitar todas las suscripciones.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migración de suscripciones basadas en uso de Azure

No es necesario migrar manualmente las suscripciones de CSP basadas en el uso de Azure como sucede con las suscripciones de Office 365 CSP. El soporte técnico de Microsoft Azure puede migrar las suscripciones de Azure, así como todos los servicios o los recursos implementados, desde las cuentas de revendedor de CSP de **Transición desde** a la cuenta de revendedor de CSP de **Transición a**. Durante esta transición, el cliente no experimentará ninguna interrupción del servicio.

1. Asegúrate de que las cuentas de cliente que necesitan que se migren las suscripciones de Azure han aceptado el acuerdo que se asociará con la nueva cuenta de CSP de **Transición a**.

2. Los asociados notifican a Microsoft qué cuentas de cliente que tienen suscripciones de Azure están listas para su migración y proporciona los nombres de la compañía de los clientes.

3. Microsoft migra las suscripciones basadas en uso de Azure y notifica a los partners cuándo se ha completado la migración.

4. El partner confirma que la suscripción de Azure en las cuentas de revendedor de CSP de **Transición desde** ahora muestra suspendida en el Centro de partners, en la sección de suscripciones del cliente.

5. El partner confirma que la suscripción de Azure las cuenta de revendedor de CSP de **Transición a** ahora muestra un estado de **activa** en el Centro de partners, en la sección de suscripciones del cliente.

   >[!Note]
   > Deshabilitar las suscripciones en el cliente no cambia la apariencia del cliente en la lista de clientes. Actualmente no hay ninguna opción para quitar clientes de la lista. Los partners deben evitar volver a agregar suscripciones a estos clientes en el futuro desde su cuenta de **Transición desde**.

6. Repite estos pasos para todas las suscripciones de todos tus clientes para detener futuros cargos en las cuentas **Transición desde**. El partner recibirá una factura final con un crédito por el número de días sin usar entre el día de la cancelación y el último día del período de facturación. Tras ese período de facturación final, no se generarán más futuras.

### <a name="additional-information"></a>Información adicional

- Deshabilitar la suscripción de la cuenta de la **transición de** CSP no afecta al servicio del cliente final, siempre que el servicio se haya aprovisionado desde la cuenta de **transición a** CSP antes de deshabilitar la suscripción.

- El cliente no puede usar las suscripciones y no genera cargos cuando se suspende o cancela.

- Actualmente no hay ninguna manera de quitar por completo a un cliente de la lista de clientes.

    >[!Note]
    > Los asociados deben suspender las suscripciones en la **transición de** la cuenta de inquilino del asociado en el centro de Partners el mismo día en el que se realiza la transición de esas suscripciones y se configuran en la cuenta de **transición a** inquilino del asociado en el centro de partners para asegurarse de que no se produce la facturación doble. Microsoft no admitirá solicitudes de créditos debido a cualquier superposición en la facturación que se produce cuando no se establece correctamente la **transición de** las suscripciones a suspendidas.

### <a name="simplify-migration-using-export"></a>Simplificación de la migración mediante la exportación

Si usas la **Función de exportación**, puedes capturar las suscripciones que necesites usar en tu nueva estructura consolidada:

1. Haga clic en **clientes** en el centro de partners para ver la lista de clientes de la estructura existente.

2. Abre el nombre del cliente deseado.

3. En la página **Suscripciones**, haz clic en **Exportar suscripciones** para exportar los detalles de las suscripciones a un archivo de Excel.

4. Usa esta lista para volver a crear las suscripciones en el nuevo inquilino consolidado.

### <a name="api-registration"></a>Registro de API

Para obtener más información sobre el registro de API, consulte [configuración del acceso de API en el centro de Partners](https://go.microsoft.com/fwlink/?linkid=847990).
