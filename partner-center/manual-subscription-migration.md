---
title: "Migración de suscripciones de Dynamics AX a Dynamics 365 | Centro de partners"
description: "Microsoft presenta Dynamics 365, la próxima generación de aplicaciones empresariales inteligentes con las que tu organización podrá crecer, evolucionar y transformarse para satisfacer las necesidades de tus clientes y aprovechar nuevas oportunidades."
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
---

# Migración de suscripciones de Dynamics AX a Dynamics 365


Microsoft presenta Dynamics 365, la próxima generación de aplicaciones empresariales inteligentes con las que tu organización podrá crecer, evolucionar y transformarse para satisfacer las necesidades de tus clientes y aprovechar nuevas oportunidades. Como parte del nuevo producto, Microsoft presenta el 1 de noviembre de 2016 los planes de suscripción para clientes Microsoft Dynamics. Son similares, aunque no idénticos, a los planes actuales.

Las instrucciones de este documento describen cómo proveedores indirectos pueden cambiar suscripciones existentes de Microsoft Dynamics AX de los clientes a la nueva suscripción Microsoft Dynamics 365. Las instrucciones también se aplican a otros productos de Microsoft que se actualizan a versiones nuevas, resultando necesario que los proveedores migren las suscripciones de clientes a una nueva SKU.

**Cambios de licencias de Microsoft Dynamics AX**

Se retira la línea de productos de Microsoft Dynamics AX, con fecha de aplicación a partir del 1 de noviembre de 2016. Para obtener más información sobre las nuevas opciones de licencias para Dynamics 365, revisa a la próxima Guía de licencias que se publicará próximamente. Consulta la tabla siguiente para obtener más información sobre la asignación de licencias:

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Licencia de Dynamics AX retirada</strong></p></td>
<td><p><strong>Licencia de Dynamics 365</strong></p></td>
</tr>
<tr class="even">
<td><p>Dynamics AX Enterprise</p></td>
<td><p>Dynamics 365 Enterprise edition Plan 2</p>
<p>O Dynamics 365 para operaciones</p></td>
</tr>
<tr class="odd">
<td><p>Tarea de Dynamics AX</p></td>
<td><p>Dynamics 365 para miembro del equipo</p></td>
</tr>
<tr class="even">
<td><p>Dynamics AX funcional</p></td>
<td><p>Dynamics 365 para miembro del equipo</p></td>
</tr>
<tr class="odd">
<td><p>Dispositivo de Dynamics AX</p></td>
<td><p>Dynamics 365 para dispositivo de operaciones</p></td>
</tr>
</tbody>
</table>

 

**Microsoft Dynamics CRM Online**

El plan actual de Microsoft Dynamics CRM Online se retirará de forma definitiva 1 de noviembre de 2016. Consulta [Información importante para los clientes de CRM Online](https://go.microsoft.com/fwlink/?linkid=831667) para conocer más detalles sobre nuevas opciones de licencias.

## Clientes de transición hacia los nuevos planes de productos


Microsoft ofrece de forma continua nuevos productos y servicios a revendedores y proveedores. En estos casos, un revendedor podría tener que actualizar a los clientes con los nuevos servicios o migrar sus suscripciones de SKU que finalmente se apagarán. Migración de los clientes desde antiguas SKU a unas más recientes que requieren la siguiente secuencia:

-   [Comprar la nueva suscripción](#manual-subscription-migration-purchasenewsubsc);
-   [Reasignar licencias de usuario actual](#manual-subscription-migration-reassignlicenses);
-   [Cancelar la suscripción antigua](#manual-subscription-migration-cancelsubscriptions).

En los siguientes procedimientos, se mueve un cliente de Dynamics AX7 Enterprise a Dynamics 365 para operaciones.

<a href="" id="purchasenewsubsc"></a>
El revendedor debe mover un cliente con una suscripción existente para Dynamics AX Enterprise a Dynamics 365 para operaciones. El primer paso es comprar Dynamics 365 para operaciones.

**Comprar la nueva suscripción**

1.  En el menú **Panel**, selecciona **Clientes**, selecciona el cliente que deseas mover y elige **Agregar suscripciones**.
2.  Selecciona la suscripción que quieras adquirir del catálogo (en este caso, Dynamics 365 para operaciones, Enterprise Edition), escribe el número de licencias y elige **Enviar**.

    El cliente ahora debería tener las suscripciones antigua y nueva; en este ejemplo, serían la antigua suscripción Dynamics AX Enterprise y la nueva suscripción de destino, Dynamics 365 para operaciones, Enterprise Edition.

<a href="" id="reassignlicenses"></a>
El siguiente paso es reasignar todas las licencias de usuario existentes a la nueva suscripción.

**Reasignar licencias de usuario**

1.  En el menú **Panel**, selecciona **Clientes**, selecciona el cliente que deseas mover y elige **Usuarios y licencias**. La página Usuarios y licencias del cliente se abrirá.
2.  Para reasignar licencias de usuario, selecciona el usuario para reasignar y, a continuación, selecciona **Administrar licencias**.
3.  En la página **Administrar licencias**, desactiva la casilla de verificación de la licencia **Dynamics AX Enterprise** y selecciona la licencia **Dynamics 365 para operaciones**.
4.  Selecciona **Enviar**. Una página de confirmación enumera las nuevas asignaciones de licencias.
5.  Sigue los mismos pasos con otros usuarios del cliente que necesiten la reasignación de licencias.

<a href="" id="cancelsubscriptions"></a>
Después de mover las licencias de usuario al nuevo servicio, puedes cancelar de forma segura la suscripción antigua al nivel superior del cliente.

**Cancelar la suscripción antigua**

1.  En el menú **Panel**, selecciona **Clientes**, selecciona el cliente que deseas mover y selecciona la suscripción que quieres cancelar.
2.  En la página de detalles de suscripción, establece el **Estado** de la suscripción a **Suspendida**.
3.  Selecciona **Enviar**.

Se ha suspendido la suscripción antigua y la nueva suscripción está activa. Se cancelará el aprovisionamiento de la suscripción suspendida automáticamente después de 120 días. El cliente no incurre en costos adicionales para la suscripción antigua.

## Consideraciones adicionales


Si el cliente se mueve desde el canal abierto hasta el programa de servicios en la nube para un aprovisionamiento de suscripción adicional, también deberás migrar sus suscripciones existentes:

-   Si el cliente recibe su suscripción antigua a través del canal abierto, el movimiento al CSP en la nueva SKU es sencillo.
-   Si el cliente no se ha establecido aún como tu cliente, puedes invitarle. Para obtener información, consulta el tema de ayuda [Solicitar una relación con un cliente](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx).

Una vez que el cliente te acepte como su proveedor indirecto, los pasos de aprovisionamiento son prácticamente iguales que los descritos anteriormente: compras la nueva suscripción y, a continuación, asignas las licencias de usuario. La única diferencia implica la cancelación de suscripciones antiguas. Un nuevo proveedor no puede cancelar/suspender suscripciones adquiridas a través de otros canales. Si el cliente adquirió suscripciones anteriores en otro canal de ventas, como el canal abierto, el cliente deberá cancelarlas por sí mismo a través de dicho canal.

 

 





<!--HONumber=Jan17_HO2-->

