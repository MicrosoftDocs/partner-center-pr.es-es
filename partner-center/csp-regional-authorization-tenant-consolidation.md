---
title: "Consolidación de los inquilinos de autorización regional de CSP | Centro de partners"
description: "Usa estas instrucciones para consolidar los inquilinos para diferentes países o regiones."
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: 1d29dad279cacb63b59822efe407f26263c1a25b
ms.openlocfilehash: cc87659cd0412876a29a2f8fe48d005a84026509

---

# Consolidación de los inquilinos de autorización regional de CSP

**Se aplica a**

-  Centro de partners
-  Centro de partners para Microsoft Cloud Alemania

\[Parte de la información hace referencia a la versión preliminar del producto, que puede sufrir modificaciones importantes antes de que se publique la versión comercial. Microsoft no ofrece ninguna garantía, expresa o implícita, respecto a la información que se ofrece aquí.\]

Usa estas instrucciones para consolidar los inquilinos para diferentes países o regiones.

**Nota**: Debes tener en cuenta todas las suscripciones y recuentos de puestos para tus clientes aprovisionados desde las cuentas de transición. A los partners se les volverán a aprovisionar esas mismas suscripciones exactas con la misma cantidad de puestos en la nueva cuenta de Central CSP como parte del proceso de migración. Usa la característica de lista de exportación para ayudar a crear una lista de clientes que trasladar al inquilino centralizado. Los partners eligen si consolidar sus inquilinos. Una vez completada la consolidación, los partners no pueden volver a su estado anterior. Ten en cuenta que también son necesarias ciertas acciones por parte del cliente.

 

## Preparación para la migración


-   Inicia sesión en <https://partnercenter.microsoft.com> con la cuenta de transición (la cuenta existente) y tome nota de todos los clientes y todos los servicios aprovisionados para dichos clientes.

![lista de clientes regionales](images/regionalcustomer1.png)

## Migración de las cuentas de cliente


1.  Inicia sesión en <https://partnercenter.microsoft.com> con la cuenta de transición (la nueva cuenta) y navega hasta la lista de clientes desde el panel del centro de partners.

2.  Selecciona Cliente.

3.  Haz clic en **Solicitar una relación de revendedor**. Se te mostrará un mensaje de correo electrónico predeterminado que presentar a tus clientes. Este mensaje contiene una dirección URL con el identificador de organización exclusivo para tu nueva cuenta del centro de partners.

4.  **Acción de cliente:** Asegúrate de que todos los clientes activos que deseas migrar visitan esta dirección URL. Al abrir la dirección URL, al cliente se le pedirá que inicie sesión en el portal de Office 365. El cliente iniciará sesión usando el mismo identificador de organización que utilice para acceder a los portales de administración de Azure y de Office 365.

5.  Tras iniciar sesión, al administrador Global de la cuenta del cliente se le pedirá que envíe un contrato para conceder privilegios de administrador delegado a la nueva cuenta de CSP. Si acepta, el cliente seleccionará la casilla y autorizará la relación.

Los clientes aparecerán en la lista de clientes del partner después de enviar el acuerdo, uno por uno.

## Migración de suscripciones basadas en uso de Office 365 y que no sean de Azure


1.  Cuando el cliente haya firmado el contrato, puedes volver a crear sus suscripciones en tu inquilino de partner centralizado.

2.  En el panel del centro de partners, haz clic en **Clientes** en la barra de navegación izquierda.

3.  Abre el nombre de la compañía del cliente que deseas migrar.

4.  Haz clic en **Agregar suscripción**.

5.  Agrega las suscripciones y el número de puestos correctos desde el catálogo. Verifica los datos con la información proporcionada en las cuentas de partner de **Transición desde**.

    ![captura de pantalla de la lista de clientes](images/regionalcustomer2.png)

6.  Haz clic en **Enviar**.

Ahora los servicios se proporcionan al cliente desde la cuenta de partner de **Transición a**.

Repite estos pasos para migrar las suscripciones de todos los demás clientes.

Antes de pasar a la siguiente sección, asegúrate de todas las suscripciones de cliente existente en las cuentas de partner de **Transición desde** se vuelven a aprovisionar en la cuenta de partner de **Transición a**.

**Nota** Los partners deben suspender las suscripciones en la cuenta de inquilino de partner de **Transición desde** en el Centro de partners el mismo día que se realice la transición de dichas suscripciones y configurarlas en la cuenta de inquilino de partner de **Transición a** en el Centro de partners para asegurarse de que no se produce una facturación doble. Se denegarán las solicitudes de soporte técnico referentes a créditos debidas a cualquier superposición en la facturación que se produzca por no deshabilitar correctamente las suscripciones de **Transición desde**.

 

## Deshabilitar las suscripciones de Office 365 en la cuenta de partner de Transición desde


Deshabilitar la suscripción de CSP de las cuentas de partner de **Transición desde** detiene toda facturación futura. No es necesario deshabilitar manualmente las suscripciones de Azure, porque las suscripciones de Azure se deshabilitan automáticamente durante el proceso de migración.

1.  Inicia sesión en <https://partnercenter.microsoft.com> con la cuenta de CSP de **Transición desde** y navega hasta la lista de clientes.

2.  Abre al cliente cuyas suscripciones quieras deshabilitar y, a continuación, selecciona la primera oferta que deshabilitar.
3.  Establece la suscripción en **suspendida**y, a continuación, haz clic en **enviar**.

    **Nota**: Suspender la suscripción garantiza que no se produce una facturación doble.

     

    La suscripción muestra **suspendida** en la lista de suscripciones.

4.  Repite estos pasos para todas las suscripciones del cliente. Comprueba que todas muestran **suspendida.**

5.  Selecciona al siguiente cliente de la lista y repite el proceso de deshabilitar todas las suscripciones.

## Migración de suscripciones basadas en uso de Azure


Ten en cuenta que no es necesario migrar las suscripciones de CSP basadas en el uso de Azure de forma manual, como sucede con las suscripciones de CSP de Office 365. El soporte técnico de Microsoft Azure puede migrar las suscripciones de Azure, así como todos los servicios o los recursos implementados, desde las cuentas de revendedor de CSP de **Transición desde** a la cuenta de revendedor de CSP de **Transición a**. Durante esta transición, el cliente no experimentará ninguna interrupción del servicio.

1.  Asegúrate de que las cuentas de cliente que necesitan que se migren las suscripciones de Azure han aceptado el acuerdo que se asociará con la nueva cuenta de CSP de **Transición a**.
2.  Los partners notifican a Microsoft qué cuentas de cliente que tienen suscripciones de Azure están listas para migrar y proporciona los nombres de compañía de dichos clientes.
3.  Microsoft migra las suscripciones basadas en uso de Azure y notifica a los partners cuándo se ha completado la migración.
4.  El partner confirma que la suscripción de Azure en las cuentas de revendedor de CSP de **Transición desde** ahora muestra suspendida en el Centro de partners, en la sección de suscripciones del cliente.
5.  El partner confirma que la suscripción de Azure las cuenta de revendedor de CSP de **Transición a** ahora muestra un estado de **activa** en el Centro de partners, en la sección de suscripciones del cliente.

    **Nota**: Deshabilitar las suscripciones en el cliente no modifica la apariencia de dicho cliente en la lista de clientes. Actualmente no hay ninguna opción para quitar clientes de la lista. Los partners deben evitar volver a agregar suscripciones a estos clientes en el futuro desde su cuenta de **Transición desde**.

     

6.  Repite estos pasos para todas las suscripciones de todos tus clientes para detener futuros cargos en las cuentas **Transición desde**. El partner recibirá una factura final con un crédito por el número de días sin usar entre el día de la cancelación y el último día del período de facturación. Tras ese período de facturación final, no se generarán más futuras.

### Notas

-   Deshabilitar la suscripción desde la cuenta de CSP de **Transición desde** no afecta a servicio del cliente final, siempre que el servicio se haya aprovisionado desde la cuenta de CSP **Transición a** antes de la deshabilitación.

-   El cliente no puede usar las suscripciones y estas no generarán cargos cuando se suspendan o se cancelen.

-   Actualmente no hay ninguna manera de quitar por completo a un cliente de la lista de clientes.

-   **Nota** Los partners deben suspender las suscripciones en la cuenta de inquilino de partner de **Transición desde** en el Centro de partners el mismo día que se realice la transición de dichas suscripciones y configurarlas en la cuenta de inquilino de partner de **Transición a** en el Centro de partners para asegurarse de que no se produce una facturación doble. Microsoft no admitirá las solicitudes de soporte técnico referentes a créditos debidas a cualquier superposición en la facturación que se produzca por no deshabilitar correctamente las suscripciones de **Transición desde**.

     

### Simplificación de la migración mediante la exportación

Si usas la **Función de exportación**, puedes capturar las suscripciones que necesites usar en tu nueva estructura consolidada:

1.  Haz clic en **Clientes** en el panel para ver la lista de clientes de la estructura existente.

2.  Abre el nombre del cliente deseado.

3.  En la página **Suscripciones**, haz clic en **Exportar suscripciones** para exportar los detalles de las suscripciones a un archivo de Excel.

4.  Usa esta lista para volver a crear las suscripciones en el nuevo inquilino consolidado.

### Registro de API

Para obtener más información acerca del registro de API, visita esta [página web](https://msdn.microsoft.com/en-us/library/partnercenter/mt267552.aspx) (en inglés).

## Registro de actividades del Centro de partners


Con el registro de actividades, los partners pueden ver un registro de todos los cambios que afectan a los clientes en su inquilino. Esto ayuda a los partners a realizar un seguimiento de los cambios en un inquilino del cliente.

**Ver el registro de actividades**

1.  En el panel del Centro de partners, haz clic en el vínculo **Registro de actividades**.
2.  En la página **Registro de actividades**, mira los cambios realizados en las cuentas de cliente. Para filtrar el registro de actividades por fecha, elige las fechas **Desde** y **A** para restringir los registros seleccionados en el registro. Para filtrar por cliente en el **Registro de actividades**, usa el cuadro de búsqueda.

**Exportación del registro de actividades**

-   Haz clic en **Exportar registro** para exportar los datos del registro de actividades a un archivo CSV.

    También puedes exportar la lista de clientes y la lista de suscripciones de un cliente individual (desde la página de suscripción de dicho cliente).

 

 






<!--HONumber=Jan17_HO2-->


