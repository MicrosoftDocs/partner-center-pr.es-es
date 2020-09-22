---
title: Consolidación de los inquilinos de autorización regional de CSP
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usa estas instrucciones para consolidar los inquilinos para diferentes países o regiones. Esto incluye los pasos para migrar las cuentas de cliente y las suscripciones de cliente.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 232eae10927d8ac38b4cce0842fbb8e4278f8d03
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000379"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Instrucciones para la consolidación de los inquilinos de autorización regional de CSP

**Se aplica a**

-  Centro de partners
-  Centro de partners para Microsoft Cloud for US Government

**Roles adecuados**

- Administrador global
- Agente de administrador

\[Algunos datos se relacionan con productos de versiones preliminares que pueden modificarse sustancialmente antes de su lanzamiento comercial. Microsoft no proporciona ninguna garantía, expresa o implícita, con respecto a la información proporcionada aquí.\]

Puede consolidar los inquilinos para su empresa. Usa estas instrucciones para consolidar los inquilinos para diferentes países o regiones.

>[!NOTE]  
>Debe tener en cuenta todas las suscripciones y los recuentos de licencias aprovisionados para cada uno de los clientes de la cuenta desde la que va a realizar la transición. Volverá a aprovisionar las mismas suscripciones exactas con los mismos recuentos de licencias en la nueva cuenta central de CSP como parte del proceso de migración. Usa la característica de lista de exportación para ayudar a crear una lista de clientes que trasladar al inquilino centralizado.  Una vez completada la consolidación, no se puede revertir al estado anterior del inquilino. También es posible que se necesiten acciones del cliente.

## <a name="prepare-for-migration"></a>Preparación para la migración

- Inicie sesión en el **centro de Partners**  mediante la cuenta de **transición** (la que va a pasar a la nueva cuenta) y Revise todos los clientes y todos los servicios aprovisionados para esos clientes.

- Cierre la sesión de esta cuenta.

## <a name="migrate-customer-accounts"></a>Migración de las cuentas de cliente

1. Inicie sesión en el **centro de Partners**  con la cuenta de **transición** (nueva) (aquella en la que va a realizar la transición de los clientes).

2. Seleccione **Clientes**.

3. Haz clic en **Solicitar una relación de revendedor**. Se le presentará un mensaje de correo electrónico predeterminado para enviarlo a sus clientes. Este mensaje contiene una dirección URL con el identificador de organización exclusivo para tu nueva cuenta del centro de partners.

4. **Acción de cliente:** Asegúrate de que todos los clientes activos que deseas migrar visitan esta dirección URL. Al abrir la dirección URL, al cliente se le pedirá que inicie sesión en el portal de Office 365. El cliente iniciará sesión usando el mismo identificador de organización que utilice para acceder a los portales de administración de Azure y de Office 365.

5. Después de iniciar sesión, se pide al administrador global de la **cuenta de cliente** que envíe un contrato que proporcione privilegios de administrador delegado a la nueva cuenta de CSP. Si acepta, el cliente seleccionará la casilla y autorizará la relación.

Los clientes aparecerán en la lista de clientes del asociado después de haber enviado el contrato, uno por uno.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migración de suscripciones basadas en uso de Office 365 y que no sean de Azure

1. Cuando el cliente haya firmado el contrato, puedes volver a crear sus suscripciones en tu inquilino de partner centralizado.

2. En **centro de Partners** , seleccione **clientes**.

3. Abre el nombre de la compañía del cliente que deseas migrar.

4. Seleccione **Agregar suscripción**.

5. Agregue las suscripciones y los recuentos de licencias correctos del catálogo. Verifica los datos con la información proporcionada en las cuentas de partner de **Transición desde**.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="lista de clientes":::

6. Haga clic en **enviar.**

   Ahora los servicios se proporcionan al cliente desde la cuenta de partner de **Transición a**.

7. Repite estos pasos para migrar las suscripciones de todos los demás clientes.

Antes de pasar a la siguiente sección, asegúrate de todas las suscripciones de cliente existente en las cuentas de partner de **Transición desde** se vuelven a aprovisionar en la cuenta de partner de **Transición a**.

> [!NOTE]
> Los asociados deben suspender las suscripciones en la **transición de** la cuenta de inquilino de asociado del centro de Partners el mismo día en que se realiza la transición de esas suscripciones y se configuran en la cuenta de la **transición a** la cuenta de inquilino del asociado en el centro de partners para asegurarse de que no se produce la facturación doble. Se denegarán los créditos de las solicitudes de soporte técnico debido a cualquier superposición en la facturación que se produzca cuando no se deshabilite correctamente la **transición de** las suscripciones.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Deshabilitar las suscripciones de Office 365 en la cuenta de partner de Transición desde

Deshabilitar la suscripción de CSP de las cuentas de partner de **Transición desde** detiene toda facturación futura. No tiene que deshabilitar manualmente las suscripciones de Azure, ya que las suscripciones de Azure se deshabilitan automáticamente durante el proceso de migración.

1. Inicie sesión en el **centro de Partners** con la **transición de** la cuenta de CSP y navegue hasta la lista de clientes.

2. Abre al cliente cuyas suscripciones quieras deshabilitar y, a continuación, selecciona la primera oferta que deshabilitar.

3. Establece la suscripción en **suspendida**y, a continuación, haz clic en **enviar**.

   >[!Note]
   >Suspender la suscripción garantiza que no se produzca la facturación.

   La suscripción muestra **Suspended** en la lista de suscripciones.

4. Repite estos pasos para todas las suscripciones del cliente. Comprueba que todas muestran **suspendida.**

5. Selecciona al siguiente cliente de la lista y repite el proceso de deshabilitar todas las suscripciones.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migración de suscripciones basadas en uso de Azure

A diferencia de las suscripciones de CSP de Office 365, no es necesario migrar manualmente las suscripciones de CSP basadas en el uso de Azure. Microsoft Azure soporte técnico migrará las suscripciones de Azure, así como todos los servicios o recursos implementados desde la **transición de** las cuentas de revendedores de CSP **a la cuenta** de revendedor de CSP. Durante esta transición, el cliente no experimentará ninguna interrupción del servicio.

1. Asegúrese de que las cuentas de cliente que tendrán las suscripciones de Azure migradas han aceptado el contrato que se va a asociar a la nueva cuenta **de transición a** CSP.

2. Notificará a Microsoft las cuentas de cliente que están preparadas para la migración y proporcionará los nombres de las compañías de los clientes.

3. Microsoft migra las suscripciones basadas en el uso de Azure y le notifica cuando se completa la migración.

4. Debe confirmar que la suscripción de Azure en la que se realiza la **transición de** la cuenta de revendedor de CSP ahora está marcada como **suspendida** en el centro de Partners en la sección suscripciones de clientes.

5. Confirme que la suscripción de Azure en la cuenta de **transición a** revendedor de CSP muestra ahora el estado **activo** en el centro de Partners en la sección suscripciones de clientes.

   >[!Note]
   > Deshabilitar las suscripciones en el cliente no cambia la apariencia del cliente en la lista de clientes. Actualmente no hay ninguna opción para quitar clientes de la lista. Los partners deben evitar volver a agregar suscripciones a estos clientes en el futuro desde su cuenta de **Transición desde**.

6. Repite estos pasos para todas las suscripciones de todos tus clientes para detener futuros cargos en las cuentas **Transición desde**. El partner recibirá una factura final con un crédito por el número de días sin usar entre el día de la cancelación y el último día del período de facturación. Tras ese período de facturación final, no se generarán más futuras.

### <a name="additional-information"></a>Información adicional

- Deshabilitar la suscripción de la cuenta de la **transición de** CSP no afecta al servicio del cliente final, siempre que el servicio se haya aprovisionado desde la cuenta de **transición a** CSP antes de deshabilitar la suscripción.

- El cliente no puede usar las suscripciones y no genera cargos cuando se suspende o cancela.

- Actualmente no hay ninguna manera de quitar un cliente completamente de la lista de **clientes** .
- 
    >[!Note]
    > Los asociados deben suspender las suscripciones en la **transición de** la cuenta de inquilino del asociado en el centro de Partners el mismo día en que se realiza la transición de las suscripciones y se configuran en la cuenta de **transición** para asegurarse de que no se produce la facturación doble. Microsoft no admitirá solicitudes de créditos debido a cualquier superposición en la facturación que se produce cuando no se establece correctamente la **transición de** las suscripciones a suspendidas.

### <a name="simplify-migration-using-export"></a>Simplificación de la migración mediante la exportación

Si usas la **Función de exportación**, puedes capturar las suscripciones que necesites usar en tu nueva estructura consolidada:

1. Haga clic en **clientes** en el centro de partners para ver la lista de clientes. 

2. Abre el nombre del cliente deseado.

3. En la página **Suscripciones**, haz clic en **Exportar suscripciones** para exportar los detalles de las suscripciones a un archivo de Excel.

4. Usa esta lista para volver a crear las suscripciones en el nuevo inquilino consolidado.

### <a name="api-registration"></a>Registro de API

Para obtener más información sobre el registro de API, consulte [configuración del acceso de API en el centro de Partners](/partner-center/develop/set-up-api-access-in-partner-center).

## <a name="next-steps"></a>Pasos siguientes

- [Configuración y administración de las cuentas de clientes para partners revendedores en el Centro de partners](customer-accounts.md)