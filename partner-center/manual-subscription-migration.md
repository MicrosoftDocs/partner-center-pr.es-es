---
title: Migrate Dynamics AX subscriptions to Dynamics 365 | Partner Center
description: Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.openlocfilehash: 39f254488dab4335a24a5a36fc593d2e281adbf8
ms.sourcegitcommit: 2c948321945d0e61153f7d766a1a669782df4a54
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/24/2017
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Migrate Dynamics AX subscriptions to Dynamics 365

**Applies to**

-  Partner Center

Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities. Como parte del nuevo producto, el 1 de noviembre de 2016 Microsoft introdujo los planes de suscripción a Microsoft Dynamics para clientes. Son similares a los planes actuales, aunque no idénticos.

Las instrucciones de este documento describen el modo en el que los proveedores indirectos pueden cambiar las suscripciones actuales a Microsoft Dynamics AX y a Microsoft Dynamics CRM Online de los clientes a la nueva suscripción a Microsoft Dynamics 365. The instructions also apply to other Microsoft products that update to new versions, requiring providers to migrate customers’ subscriptions to a new SKU.

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


Microsoft continuously offers new products and services to resellers and providers. In these cases, a reseller may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down. Migrating customers from old SKUs to newer ones requires the following sequence:

-   [Purchase the new subscription](#manual-subscription-migration-purchasenewsubsc);
-   [Re-assign current user licenses](#manual-subscription-migration-reassignlicenses);
-   [Cancelar la suscripción antigua](#manual-subscription-migration-cancelsubscriptions).

En los siguientes procedimientos, moverás a un cliente de Microsoft Dynamics AX o CRM Online a Dynamics 365.

En este ejemplo, el revendedor debe mover un cliente con una suscripción existente para Dynamics AX Enterprise a Dynamics 365 for Operations. El primer paso es comprar Dynamics 365 for Operations.  Repite estos pasos para un cliente de CRM Online que se mueva a Microsoft Dynamics 365.

<a href="" id="purchasenewsubsc"></a>

**Comprar la nueva suscripción**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Add Subscriptions**.
2.  Select the subscription you want to purchase from the catalog (in this case, Dynamics 365 for Operations, Enterprise Edition), enter the number of licenses, and choose **Submit**.

    Your customer should now have both old and new subscriptions: in this example, the old Dynamics AX Enterprise, and the new ‘target’ subscription, Dynamics 365 for Operations, Enterprise Edition.

<a href="" id="reassignlicenses"></a> The next step is to reassign all existing user licenses to the new subscription.

**Reassign user licenses**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Users and licenses**. The customer’s Users and Licenses page opens.
2.  To re-assign user licenses, select the user to reassign and then select **Manage licenses**.
3.  On the **Manage licenses** page, clear the **Dynamics AX Enterprise** license check box and select the **Dynamics 365 for Operations** license.
4.  Select **Submit**. A confirmation page lists the new license assignments.
5.  Continue the same steps with any other customer users that need license reassignment.

<a href="" id="cancelsubscriptions"></a> After moving the user licenses to the new service, you can safely cancel the old subscription at the top Customer level.

**Cancel the old subscription**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and select the subscription you want to cancel.
2.  In the subscription details page, set the subscription **Status** to **Suspended**.
3.  Select **Submit**.

The old subscription is suspended, and the new subscription is active. The suspended subscription will automatically be de-provisioned after 120 days. The customer incurs no additional costs for the old subscription.

## <a name="additional-considerations"></a>Additional considerations


If your customer is moving from the Open Channel to the Cloud Services Program for further subscription provisioning, you will also need to migrate their existing subscriptions:

-   If the customer received their old subscription through the Open Channel, moving to the CSP on the new SKU is straightforward.
-   If the customer is not yet established as your customer, you can invite them. For information, see the [Request a relationship with a customer](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx) help topic.

After the customer accepts you as their indirect provider, the provisioning steps are mostly the same as described above: you purchase the new subscription, and then assign the user licenses. The only difference involves cancellation of old subscription(s). A new provider cannot cancel suspend/cancel subscriptions acquired via other channels. If the customer acquired prior subscriptions in another sales channel, such as the Open channel, the customer will need to cancel it themselves through that channel.

 

 



