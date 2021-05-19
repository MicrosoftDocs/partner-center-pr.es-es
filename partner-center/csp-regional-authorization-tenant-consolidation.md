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
ms.openlocfilehash: d2168dcd60b8675a21960918dab49b778025fa51
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147588"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Instrucciones para la consolidación de los inquilinos de autorización regional de CSP

**Se aplica a**: Centro de partners | Centro de partners para Microsoft Cloud for US Government

**Roles adecuados:** administrador global | Agente de administración

\[Parte de la información está relacionada con el producto publicado previamente que puede modificarse considerablemente antes de su lanzamiento comercial. Microsoft no otorga ninguna garantía, explícita o implícita, con respecto a la información proporcionada aquí.\]

Puede consolidar los inquilinos para su negocio. Usa estas instrucciones para consolidar los inquilinos para diferentes países o regiones.

>[!NOTE]  
>Debe tener en cuenta todos los recuentos de licencias y suscripciones aprovisionadas para cada uno de los clientes de la cuenta desde la que va a realizar la transición. Volverá a aprovisionar esas mismas suscripciones exactas con los mismos recuentos de licencias en la nueva cuenta de CSP central como parte del proceso de migración. Usa la característica de lista de exportación para ayudar a crear una lista de clientes que trasladar al inquilino centralizado.  Una vez completada la consolidación, no se puede revertir al estado de inquilino anterior. También puede ser necesaria la acción del cliente.

## <a name="prepare-for-migration"></a>Preparación para la migración

- Inicie sesión en **Centro de partners** con  la cuenta de transición (la que realizará la transición a la nueva cuenta) y revise todos los clientes y todos los servicios aprovisionados para esos clientes.

- Cerrar sesión en esta cuenta.

## <a name="migrate-customer-accounts"></a>Migración de las cuentas de cliente

1. Inicie sesión en **Centro de partners**  con **la cuenta de** transición (nueva) (a la que va a realizar la transición de los clientes).

2. Seleccione **Clientes**.

3. Seleccione **Solicitar una relación de revendedor.** Se le muestra un mensaje de correo electrónico predeterminado para enviarlo a los clientes. Este mensaje contiene una dirección URL con el identificador de organización exclusivo para tu nueva cuenta del centro de partners.

4. **Acción de cliente:** Asegúrate de que todos los clientes activos que deseas migrar visitan esta dirección URL. Al abrir la dirección URL, al cliente se le pedirá que inicie sesión en el portal de Office 365. El cliente iniciará sesión usando el mismo identificador de organización que utilice para acceder a los portales de administración de Azure y de Office 365.

5. Después de iniciar sesión,  se solicita al administrador global de la cuenta de cliente que envíe un contrato que concede privilegios de administrador delegado a la nueva cuenta de CSP. Si acepta, el cliente seleccionará la casilla y autorizará la relación.

Los clientes aparecerán en la lista de clientes del asociado después de haber enviado el contrato, uno por uno.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migración de suscripciones basadas en uso de Office 365 y que no sean de Azure

1. Cuando el cliente haya firmado el contrato, puedes volver a crear sus suscripciones en tu inquilino de partner centralizado.

2. En **Centro de partners**, seleccione **Clientes.**

3. Abre el nombre de la compañía del cliente que deseas migrar.

4. Seleccione **Agregar suscripción**.

5. Agregue las suscripciones y los recuentos de licencias correctos desde el catálogo. Verifica los datos con la información proporcionada en las cuentas de partner de **Transición desde**.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="lista de clientes":::

6. Seleccione **Enviar.**

   Ahora los servicios se proporcionan al cliente desde la cuenta de partner de **Transición a**.

7. Repite estos pasos para migrar las suscripciones de todos los demás clientes.

Antes de pasar a la siguiente sección, asegúrate de todas las suscripciones de cliente existente en las cuentas de partner de **Transición desde** se vuelven a aprovisionar en la cuenta de partner de **Transición a**.

> [!NOTE]
> Los asociados deben  suspender las suscripciones de la cuenta Transición desde el inquilino del asociado  en Centro de partners el mismo día en que esas suscripciones se han pasado y configurado en la cuenta Transición al inquilino del asociado del Centro de partners para asegurarse de que no se produce la doble facturación. Se denegarán las solicitudes de soporte técnico para los créditos debido a cualquier superposición en la facturación que se produzca al no deshabilitar correctamente las suscripciones **De** transición.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Deshabilitar las suscripciones de Office 365 en la cuenta de partner de Transición desde

Deshabilitar la suscripción de CSP de las cuentas de partner de **Transición desde** detiene toda facturación futura. No tiene que deshabilitar manualmente las suscripciones de Azure, ya que las suscripciones de Azure se deshabilitan automáticamente durante el proceso de migración.

1. Inicie sesión en el **Centro de partners** con la **cuenta Transitioning From** CSP (Transición desde CSP) y vaya a la lista de clientes.

2. Abre al cliente cuyas suscripciones quieras deshabilitar y, a continuación, selecciona la primera oferta que deshabilitar.

3. Establezca la suscripción en **suspendida y,** a continuación, **seleccione Enviar**.

   >[!Note]
   >La suspensión de la suscripción garantiza que no se produzca la doble facturación.

   La suscripción se **muestra suspendida en** la lista de suscripciones.

4. Repite estos pasos para todas las suscripciones del cliente. Comprueba que todas muestran **suspendida.**

5. Selecciona al siguiente cliente de la lista y repite el proceso de deshabilitar todas las suscripciones.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migración de suscripciones basadas en uso de Azure

A diferencia de las suscripciones de CSP de Office 365, no es necesario migrar manualmente las suscripciones de CSP basadas en el uso de Azure. Microsoft Azure soporte técnico migrará las suscripciones de Azure y todos los servicios o recursos implementados desde la transición de las cuentas de revendedor de **CSP** a la cuenta de revendedor de **Transición** a CSP. Durante esta transición, el cliente no experimentará ninguna interrupción del servicio.

1. Asegúrese de que las cuentas de cliente que tendrán suscripciones de Azure migradas hayan aceptado el contrato para asociarse a la nueva cuenta de CSP **de** transición a .

2. Notificará a Microsoft qué cuentas de cliente están listas para migrar y proporcionará los nombres de la empresa de esos clientes.

3. Microsoft migra las suscripciones basadas en el uso de Azure y le notifica cuando se completa la migración.

4. Debe confirmar que la suscripción de Azure en la cuenta  de revendedor de **Transición** desde CSP ahora está marcada como suspendida en Centro de partners en la sección suscripciones del cliente.

5. Confirme que la suscripción de Azure en la cuenta  de revendedor de **Transición** a CSP ahora muestra el estado activo en Centro de partners en la sección suscripciones de cliente.

   >[!Note]
   > Deshabilitar las suscripciones en el cliente no cambia la apariencia del cliente en la lista Clientes. Actualmente no hay ninguna opción para quitar clientes de la lista. Los partners deben evitar volver a agregar suscripciones a estos clientes en el futuro desde su cuenta de **Transición desde**.

6. Repite estos pasos para todas las suscripciones de todos tus clientes para detener futuros cargos en las cuentas **Transición desde**. El partner recibirá una factura final con un crédito por el número de días sin usar entre el día de la cancelación y el último día del período de facturación. Tras ese período de facturación final, no se generarán más futuras.

### <a name="additional-information"></a>Información adicional

- Deshabilitar la suscripción de la cuenta de **CSP** de transición desde no afecta al servicio del cliente final, siempre y cuando el servicio se aprovisionó desde la cuenta de **CSP** de transición a antes de deshabilitar la suscripción.

- El cliente no puede usar las suscripciones y no generan cargos cuando se suspenden o cancelan.

- Actualmente no hay ninguna manera de quitar completamente un cliente de la **lista Clientes.**
- 
    >[!Note]
    > Los asociados deben  suspender las suscripciones en la cuenta de inquilino de transición desde el  asociado en Centro de partners el mismo día en que esas suscripciones se transiciónn a la cuenta de transición a y configurarse en ella para asegurarse de que no se produce la doble facturación. Microsoft no admitirá solicitudes de crédito debido a cualquier superposición en  la facturación que se produzca al no establecer correctamente la transición de suscripciones a suspendidas.

### <a name="simplify-migration-using-export"></a>Simplificación de la migración mediante la exportación

Si usas la **Función de exportación**, puedes capturar las suscripciones que necesites usar en tu nueva estructura consolidada:

1. Seleccione **Clientes** en Centro de partners para ver la lista de clientes. 

2. Abre el nombre del cliente deseado.

3. En la **página Suscripciones,** seleccione **Exportar suscripciones para** exportar los detalles de las suscripciones a un archivo de Excel.

4. Usa esta lista para volver a crear las suscripciones en el nuevo inquilino consolidado.

### <a name="api-registration"></a>Registro de API

Para obtener más información sobre el registro de API, consulte [Configuración del acceso de API en Centro de partners](/partner-center/develop/set-up-api-access-in-partner-center).

## <a name="next-steps"></a>Pasos siguientes

- [Proveedor de soluciones en la nube mercados regionales del programa y monedas donde puede vender ofertas de CSP](regional-authorization-overview.md)
