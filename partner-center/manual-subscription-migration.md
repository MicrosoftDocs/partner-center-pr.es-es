---
title: Migración de suscripciones de Dynamics AX a Dynamics 365 | Centro de partners
ms.topic: article
ms.date: 10/29/2018
description: Microsoft presenta Dynamics 365, la próxima generación de aplicaciones empresariales inteligentes con las que tu organización podrá crecer, evolucionar y transformarse para satisfacer las necesidades de tus clientes y aprovechar nuevas oportunidades.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: e992a3cdfc0bbb01a303a8b00bfeda3cf60d1882
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/29/2018
ms.locfileid: "5797138"
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Migrar suscripciones de Dynamics AX a Dynamics 365

**Se aplica a**

-  Centro de partners

Microsoft presenta Dynamics 365, la próxima generación de aplicaciones empresariales inteligentes con las que tu organización podrá crecer, evolucionar y transformarse para satisfacer las necesidades de tus clientes y aprovechar nuevas oportunidades. Como parte del nuevo producto, el 1 de noviembre de 2016 Microsoft introdujo los planes de suscripción a Microsoft Dynamics para clientes. Son similares a los planes actuales, aunque no idénticos.

Las instrucciones de este documento describen el modo en el que los proveedores indirectos pueden cambiar las suscripciones actuales a Microsoft Dynamics AX y a Microsoft Dynamics CRM Online de los clientes a la nueva suscripción a Microsoft Dynamics 365. Las instrucciones también se aplican a otros productos de Microsoft que se actualizan a versiones nuevas, resultando necesario que los proveedores migren las suscripciones de clientes a una nueva SKU.

Los planes de Microsoft Dynamics CRM Online y AX se han retirado.  A partir del 1 de julio de 2017, ya no se pueden renovar los planes antiguos, y tampoco se renovarán automáticamente las suscripciones a E4 existentes cuando caduquen.

Cuando las suscripciones a CRM Online y AX finalicen, se cancelarán. Para garantizar que los clientes no vean interrumpidos sus servicios, planifica la transición de aquellos clientes cuyas suscripciones vayan a caducar a una opción de SKU compatible, como aparece a continuación. Recomendamos trasladar los clientes a las nuevas suscripciones antes de la fecha de finalización anual de la suscripción para evitar interrupciones en el servicio a los clientes. 

En la página de detalles de la suscripción, verá que el estado de las suscripciones que van a caducar ha cambiado de "Se renovará automáticamente el [fecha]" a "Expira el [fecha]". 

Si usas la API (CREST o el Centro de partners), puedes descubrir las suscripciones que van a caducar evaluando la fecha de finalización de la suscripción junto con la propiedad auto renew = False. Las suscripciones se establecieron en auto renew=False el 1 de julio de 2017. Puedes mover a los clientes a un plan nuevo en cualquier momento. 

**Cambios en las licencias de Microsoft Dynamics AX**

La línea de productos de Microsoft Dynamics AX se retiró a partir del 1 de noviembre de 2016. Para obtener más información sobre las nuevas opciones de licencias para Dynamics 365, revisa la [Guía de licencias](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf).

 Consulta la tabla siguiente para obtener más información sobre la asignación de licencias:

|**SKU retirado**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise SKU|Plan Microsoft Dynamics 365 for Unified Operations o Microsoft Dynamics 365 |
|Tarea|Microsoft Dynamics 365 for Activity
|Tarea/autoservicio|Microsoft Dynamics 365 for Team Members|
|Dispositivo|Dispositivo de Microsoft Dynamics 365 for Operations|

## <a name="microsoft-dynamics-crm-online-licensing-changes"></a>Cambios de licencias de Microsoft Dynamics CRM Online 

**Microsoft Dynamics CRM Online**

El plan actual de Microsoft Dynamics CRM Online se retiró el 1 de noviembre de 2016. Para obtener más información sobre las nuevas opciones de licencias para Microsoft Dynamics 365, revisa la [Guía de licencias](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf). Consulta [Información importante para los clientes de CRM Online](https://go.microsoft.com/fwlink/?linkid=831667) para conocer más detalles sobre nuevas opciones de licencias.

Consulta la tabla siguiente para obtener más información sobre la asignación de licencias:

|**SKU retirado**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise|Plan Dynamics 365 Enterprise Customer Engagement |
|Professional|Plan Dynamics 365 Enterprise Customer Engagement, Dynamics 365 for Sales o Dynamics 365 for Customer Service|
|Basic|Plan Dynamics 365 for Team Members, Dynamics 365 for Sales, Dynamics 365 for Customer Service o Dynamics 365 Enterprise Customer Engagement|
|Essential|Dynamics 365 for Team Members|
|Complemento de servicio de campo|Plan Dynamics 365 Enterprise Customer Engagement o Dynamics 365 for Field Service|
|Complemento de automatización de servicios de proyecto|Plan Dynamics 365 Enterprise Customer Engagement o Dynamics 365 for Project Service Automation|



## <a name="transition-customers-to-new-product-plans"></a>Clientes en transición a los nuevos planes de producto


Microsoft ofrece de forma continua nuevos productos y servicios a revendedores y proveedores. En estos casos, un revendedor podría tener que actualizar a los clientes con los nuevos servicios o migrar sus suscripciones de SKU que finalmente se apagarán. Migración de los clientes desde antiguas SKU a unas más recientes que requieren la siguiente secuencia:

-   [Comprar la nueva suscripción](#manual-subscription-migration-purchasenewsubsc);
-   [Reasignar licencias de usuario actual](#manual-subscription-migration-reassignlicenses);
-   [Cancelar la suscripción antigua](#manual-subscription-migration-cancelsubscriptions).

En los siguientes procedimientos, moverás a un cliente de Microsoft Dynamics AX o CRM Online a Dynamics 365.

En este ejemplo, el revendedor debe mover un cliente con una suscripción existente para Dynamics AX Enterprise a Dynamics 365 for Operations. El primer paso es comprar Dynamics 365 for Operations.  Repite estos pasos para un cliente de CRM Online que se mueva a Microsoft Dynamics 365.

<a href="" id="purchasenewsubsc"></a>

**Comprar la nueva suscripción**

1.  En el menú del **Centro de partners** , selecciona **los clientes**, selecciona al cliente que deseas mover y elige **Agregar suscripciones**.
2.  Selecciona la suscripción que quieras adquirir del catálogo (en este caso, Dynamics 365 para operaciones, Enterprise Edition), escribe el número de licencias y elige **Enviar**.

    El cliente ahora debería tener las suscripciones antigua y nueva; en este ejemplo, serían la antigua suscripción Dynamics AX Enterprise y la nueva suscripción de destino, Dynamics 365 para operaciones, Enterprise Edition.

<a href="" id="reassignlicenses"></a> El siguiente paso es reasignar todas las licencias de usuario existentes a la nueva suscripción.

**Reasignar licencias de usuario**

1.  En el menú del **Centro de partners** , selecciona **los clientes**, selecciona al cliente que deseas mover y elige **los usuarios y licencias**. La página Usuarios y licencias del cliente se abrirá.
2.  Para reasignar licencias de usuario, selecciona el usuario para reasignar y, a continuación, selecciona **Administrar licencias**.
3.  En la página **Administrar licencias**, desactiva la casilla de verificación de la licencia **Dynamics AX Enterprise** y selecciona la licencia **Dynamics 365 para operaciones**.
4.  Selecciona **Enviar**. Una página de confirmación enumera las nuevas asignaciones de licencias.
5.  Sigue los mismos pasos con otros usuarios del cliente que necesiten la reasignación de licencias.

<a href="" id="cancelsubscriptions"></a> Después de mover las licencias de usuario al nuevo servicio, puedes cancelar de forma segura la suscripción antigua al nivel superior del cliente.

**Cancelar la suscripción antigua**

1.  En el menú del **Centro de partners** , selecciona **los clientes**, selecciona al cliente que deseas mover y selecciona la suscripción que quieres Cancelar.
2.  En la página de detalles de suscripción, establece el **Estado** de la suscripción a **Suspendida**.
3.  Selecciona **Enviar**.

Se ha suspendido la suscripción antigua y la nueva suscripción está activa. Se cancelará el aprovisionamiento de la suscripción suspendida automáticamente después de 120 días. El cliente no incurre en costos adicionales para la suscripción antigua.

## <a name="additional-considerations"></a>Consideraciones adicionales


Si el cliente se mueve desde el canal abierto hasta el programa de servicios en la nube para un aprovisionamiento de suscripción adicional, también deberás migrar sus suscripciones existentes:

-   Si el cliente recibe su suscripción antigua a través del canal abierto, el movimiento al CSP en la nueva SKU es sencillo.
-   Si el cliente no se ha establecido aún como tu cliente, puedes invitarle. Para obtener información, consulta el tema de ayuda [Solicitar una relación con un cliente](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx).

Una vez que el cliente te acepte como su proveedor indirecto, los pasos de aprovisionamiento son prácticamente iguales que los descritos anteriormente: compras la nueva suscripción y, a continuación, asignas las licencias de usuario. La única diferencia implica la cancelación de suscripciones antiguas. Un nuevo proveedor no puede cancelar/suspender suscripciones adquiridas a través de otros canales. Si el cliente adquirió suscripciones anteriores en otro canal de ventas, como el canal abierto, el cliente deberá cancelarlas por sí mismo a través de dicho canal.

 

 



