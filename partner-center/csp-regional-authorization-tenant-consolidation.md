---
title: CSP regional authorization tenant consolidation | Partner Center
description: Use these instructions to consolidate tenants for different country/regions.
ms.assetid: 749B4C6A-26BE-4942-BDA8-F08C40DF048A
author: MaggiePucciEvans
ms.openlocfilehash: 06709900a4f98c44ef0ae8505928d7c901ee8473
ms.sourcegitcommit: c47f8e765def420017abe290f2f7327eab2cbba7
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 07/07/2017
---
# <a name="csp-regional-authorization-tenant-consolidation"></a>CSP regional authorization tenant consolidation

**Applies to**

-  Partner Center
-  Partner Center for Microsoft Cloud for US Government
-  Partner Center for Microsoft Cloud Germany

\[Some information relates to pre-released product which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.\]

Use these instructions to consolidate tenants for different country/regions.

**Nota**: Debes tener en cuenta todas las suscripciones y recuentos de puestos para tus clientes aprovisionados desde las cuentas de transición. Partners will be re-provisioning those same exact subscriptions with the same seat counts under the new Central CSP account as part of the migration process. Use the export list feature to help create a list of customers to move over to the centralized tenant. Partners choose to consolidate their tenants. Once consolidation is complete, Partners cannot revert to their previous state. Note that customer action is also be required.

 

## <a name="prepare-for-migration"></a>Prepare for migration


-   Log on to <https://partnercenter.microsoft.com> with the Transitioning (existing) account and take note of all customers and all of the services provisioned for those customers.

![regional customer list](images/regionalcustomer1.png)

## <a name="migrate-customer-accounts"></a>Migrate customer accounts


1.  Inicia sesión en <https://partnercenter.microsoft.com> con la cuenta de transición (la nueva cuenta) y navega hasta la lista de clientes desde el panel del centro de partners.

2.  Select Customer.

3.  Haz clic en **Solicitar una relación de revendedor**. You are presented with a default email message to present to your customers. This message contains a URL with the org ID unique to your new Partner Center account.

4.  **Acción de cliente:** Asegúrate de que todos los clientes activos que deseas migrar visitan esta dirección URL. When opening the URL, the customer is prompted to sign in to the Office 365 portal. The customer signs in using the same Org ID that they use to access the Azure and Office 365 admin portals.

5.  After signing in, the Global Admin for the customer account is prompted to submit an agreement to give delegated admin privileges to the new CSP account. If they agree, the customer selects the checkbox and agrees to authorize the relationship.

The customers will appear in the partner’s customer list after they have submitted the agreement, one by one.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrating Office 365 and non-Azure usage-based subscriptions


1.  Once your customer has signed the agreement, you can recreate their subscriptions under your Centralized Partner Tenant.

2.  En el panel del centro de partners, haz clic en **Clientes** en la barra de navegación izquierda.

3.  Open the company name for the customer you want to migrate.

4.  Haz clic en **Agregar suscripción**.

5.  Add the correct subscriptions and seat counts from the catalog. Verifica los datos con la información proporcionada en las cuentas de partner de **Transición desde**.

    ![screenshot of customer list](images/regionalcustomer2.png)

6.  Haz clic en **Enviar**.

Ahora los servicios se proporcionan al cliente desde la cuenta de partner de **Transición a**.

Repeat these steps to migrate subscriptions for all additional customers.

Before proceeding to the next section, ensure all customer subscriptions existing under the **Transitioning From** partner accounts are re-provisioned under the **Transitioning To** partner account.

**Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur. Support requests will be denied for credits due to any overlap in billing that occurs from not correctly setting the **Transitioning From** subscriptions to disabled.

 

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Disabling the Office 365 subscriptions under the Transitioning From partner account


Deshabilitar la suscripción de CSP de las cuentas de partner de **Transición desde** detiene toda facturación futura. You do not have to manually disable Azure subscriptions, because Azure subscriptions are automatically disabled during the migration process.

1.  Inicia sesión en <https://partnercenter.microsoft.com> con la cuenta de CSP de **Transición desde** y navega hasta la lista de clientes.

2.  Open the customer with subscriptions to disable, and then select the first offer to disable.
3.  Establece la suscripción en **suspendida**y, a continuación, haz clic en **enviar**.

    **Nota**: Suspender la suscripción garantiza que no se produce una facturación doble.

     

    La suscripción muestra **suspendida** en la lista de suscripciones.

4.  Repeat these steps for all subscriptions under the customer. Comprueba que todas muestran **suspendida.**

5.  Select the next customer on the list and repeat the process of disabling all subscriptions.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrating Azure usage-based subscriptions


Note that Azure usage-based CSP subscriptions do not need to be migrated manually as in the case with Office 365 CSP subscriptions. Microsoft Azure Support can migrate the Azure subscriptions as well as all deployed services or resources from the **Transitioning From** CSP reseller accounts to the **Transitioning To** CSP reseller account. There will be no disruption of service to the customer during this transition.

1.  Ensure that the customer accounts that need Azure subscriptions migrated have accepted the agreement to be associated with the new **Transitioning To** CSP account.
2.  Partners notify Microsoft which customer accounts that have Azure subscriptions are ready to migrate, and provides those customer’s company names.
3.  Microsoft migrates the Azure usage-based subscriptions and notifies the partner when the migration is complete.
4.  The partner confirms that the Azure subscription under the **Transitioning From** CSP reseller accounts now shows suspended in the Partner Center under the customer subscriptions section.
5.  The partner confirms that the Azure subscription under the **Transitioning To** CSP reseller account now shows a status of **active** in the Partner Center under the customer subscriptions section.

    **Nota**: Deshabilitar las suscripciones en el cliente no modifica la apariencia de dicho cliente en la lista de clientes. There is currently no option to remove customers from the list. Los partners deben evitar volver a agregar suscripciones a estos clientes en el futuro desde su cuenta de **Transición desde**.

     

6.  Repite estos pasos para todas las suscripciones de todos tus clientes para detener futuros cargos en las cuentas **Transición desde**. The partner will receive one final invoice with a credit for the number of unused days between the day of cancellation and the last day of the billing period. No future invoices will generate after that final billing period.

### <a name="notes"></a>Notes

-   Disabling the subscription from the **Transitioning From** CSP account does not impact end customer’s service provided the service was provisioned from the **Transitioning To** CSP account prior to the disable.

-   Subscriptions cannot be used by the customer and do not generate charges when suspended or cancelled.

-   There is currently no way to remove a customer from the Customers list completely.

-   **Note**  Partners must suspend subscriptions on the **Transitioning From** Partner Tenant account in Partner Center the same day that those subscriptions are transitioned to and set up under the **Transitioning To** Partner Tenant account in the Partner Center to ensure double billing does not occur. Microsoft will not support requests for credits due to any overlap in billing which occurs from not correctly setting the **Transitioning From** subscriptions to suspended.

     

### <a name="simplify-migration-using-export"></a>Simplify migration using Export

Si usas la **Función de exportación**, puedes capturar las suscripciones que necesites usar en tu nueva estructura consolidada:

1.  Haz clic en **Clientes** en el panel para ver la lista de clientes de la estructura existente.

2.  Open the desired customer name.

3.  En la página **Suscripciones**, haz clic en **Exportar suscripciones** para exportar los detalles de las suscripciones a un archivo de Excel.

4.  Use this list to recreate the subscriptions in your new consolidated tenant.

### <a name="api-registration"></a>API registration

Para obtener más información acerca del registro de API, visita esta [página web](https://go.microsoft.com/fwlink/?linkid=847990) (en inglés).

## <a name="partner-center-activity-log"></a>Partner Center Activity log


With the Activity log, partners can view a record of all customer-affecting changes made on their tenant. This helps partners track changes on a customer tenant.

**View the Activity log**

1.  En el panel del Centro de partners, haz clic en el vínculo **Registro de actividades**.
2.  En la página **Registro de actividades**, mira los cambios realizados en las cuentas de cliente. Para filtrar el registro de actividades por fecha, elige las fechas **Desde** y **A** para restringir los registros seleccionados en el registro. Para filtrar por cliente en el **Registro de actividades**, usa el cuadro de búsqueda.

**Export the Activity log**

-   Haz clic en **Exportar registro** para exportar los datos del registro de actividades a un archivo CSV.

    You can also export the customer list and the subscription list of a single customer (from the customer’s subscription page).

 

 



