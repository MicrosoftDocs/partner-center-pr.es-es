---
title: Conceder permiso a los clientes para que compren sus propios servicios
description: Obtenga información sobre cómo los asociados de programas de CSP pueden permitir a los clientes comprar sus propios servicios, como las reservas de Azure, para una suscripción adquirida para ellos.
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
Keywords: suscripción, compra de autoservicio, RI de autoservicio, habilitar RI, deshabilitar RI, autoservicio, compra de clientes, permisos de cliente, instancia reservada de compra de clientes, reservas de Azure de clientes, activar autoservicio, desactivar autoservicio
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 625229eb9243bc6deb631a824e8197fd0565072a
ms.sourcegitcommit: 3849d49261f4f652bd7c0537ebe31558af427c5c
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2020
ms.locfileid: "83362613"
---
# <a name="how-to-give-customers-permission-to-buy-their-own-products-or-services"></a>Cómo dar permiso a los clientes para que compren sus propios productos o servicios

**Se aplica a**

- Centro de partners
- Partners del programa CSP

**Roles adecuados**

- Agente de administrador
- Agente de ventas

En este artículo se muestra cómo un asociado del programa proveedor de soluciones en la nube (CSP) puede conceder a un cliente permiso para comprar algunos servicios o recursos propios.

Los asociados en el programa CSP suelen usar el centro de Partners y su Marketplace comercial para comprar soluciones y servicios para sus clientes. Los asociados permiten a algunos clientes aprovisionar estos servicios directamente desde el Azure Portal.

A continuación se muestra un ejemplo. Supongamos que compra una suscripción a Azure plan para un cliente en el centro de Partners. A continuación, decide agregar otros recursos o servicios a esa suscripción en nombre del cliente. En este caso, puede Agregar reservas de Azure a la suscripción del cliente (por ejemplo, agregando instancias reservadas de máquina virtual). Después, puede permitir que el cliente aprovisione más recursos de reserva de Azure en el Azure Portal.

Ahora, con la característica de **permisos de cliente** , ofrece a los clientes más opciones de autoservicio con los recursos de Azure. Al activar los permisos para el cliente, permite a los clientes comprar sus propios recursos (como, por ejemplo, comprar sus propias reservas de Azure).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Información general de los permisos del cliente en el centro de Partners

Use la página **cuenta** de cliente para activar (o desactivar) los permisos de cliente. Actualmente, esta característica admite:

- **Reservas de Azure:** Activar este permiso permite al cliente adquirir sus propias reservas de Azure para una suscripción de Azure específica que haya adquirido.

Antes de activar los permisos del cliente, tenga en cuenta los siguientes puntos importantes:

- De forma predeterminada, los permisos de clientes se deshabilitan automáticamente (están desactivados) en el centro de Partners.

- Para poder activar (o desactivar) los permisos de un cliente, debe tener asignado el rol de agente de administración en el centro de Partners.

  Los asociados que tienen asignado el rol de agente de ventas o el agente del Departamento de soporte técnico tienen acceso de solo lectura y no pueden activar o desactivar los permisos de los clientes.

- Puede activar (habilitar) los permisos para cualquier cliente que elija.

- Puede activar (o desactivar) los permisos del cliente mediante el panel del centro de Partners o las [API del centro de Partners](https://docs.microsoft.com/partner-center/develop/manage-customers).

- Después de activar (habilitar) los permisos para un cliente específico, será responsable de pagar las compras posteriores realizadas por ese cliente. Si los clientes desean intercambiar, cancelar o renovar una compra realizada (o quieren cambiar el ámbito inicial de una reserva), no podrán hacerlo por sí mismos. Necesitan pedirle a usted, como asociado, que les ayude a intercambiar, cancelar y renovar las compras, o realizar cambios posteriores en el ámbito de una reserva.  

- Después de activar los permisos para un cliente específico, **no se** le notificará ninguna compra posterior realizada por el cliente.

- Las compras posteriores realizadas por el cliente aparecerán en el centro de Partners junto con las compras que haya realizado. Puede encontrar estas compras en la página del **historial de pedidos** del cliente, en su página **reservas** o en el [**registro de actividad**](activity-logs.md).

>[!NOTE]
> Para obtener información sobre los precios que pagará el cliente y cómo ayudar a los clientes a administrar sus compras, consulte [ayudar a los clientes a administrar las reservas que compren](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Conceder permiso a los clientes para que compren sus propias reservas de Azure

Las reservas de Azure son una excelente manera de comprar servicios de Azure a una tarifa con descuento. Para obtener más información sobre las ventajas de las reservas de Azure, consulte [¿Qué son Azure reservations?](https://docs.microsoft.com/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Ahora tiene la opción de comprar reservas de Azure en nombre de sus clientes, ya que es posible que ya lo haya hecho. O bien, puede dar permiso a los clientes para que compren sus propias reservas de Azure.

>[!NOTE]
> Después de dar permiso a los clientes para que compren sus propias reservas de Azure, ayúdeles a administrar las reservas que compren. Para obtener más información, consulte [ayudar a los clientes a administrar las reservas que compren](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Para permitir que los clientes compren sus propias reservas de Azure

1. Compruebe que el cliente tiene un plan de Azure o una suscripción global de Azure que ha adquirido en su nombre.

2. Compruebe que el cliente tiene asignado el rol de **propietario** para esta suscripción.

3. Habilite los permisos de clientes (Active esta característica) para comprar sus propias reservas **de**Azure.

Cada paso aparece a continuación.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Comprobar que el cliente tiene una suscripción de Azure existente

Antes de dar permiso a los clientes para que compren sus propias reservas de Azure, debe comprobar que el cliente tiene un plan de Azure o una suscripción global de Azure. Si el cliente no muestra ninguna suscripción de Azure actual en el centro de Partners, debe comprar una suscripción para ellos antes de activar los permisos de sus clientes.

- Para ver si un cliente ya tiene una suscripción de Azure, inicie sesión en el panel del centro de Partners y seleccione **CSP** seguido de **los clientes**. Seleccione el cliente específico de la lista. A continuación, seleccione **suscripciones** y busque las suscripciones basadas en el uso de Azure plan o Azure global.

- Si un cliente no tiene una suscripción de Azure existente, puede comprar una suscripción para ellos. Consulte [comprar el plan de Azure](purchase-azure-plan.md).

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Compruebe que se ha asignado al cliente el rol correcto en Azure

Después de comprobar que el cliente tiene una suscripción de Azure existente, también debe comprobar que los usuarios clave asociados a su cliente tienen asignado el rol de **propietario** correcto para esa suscripción de Azure. Este es el acceso basado en rol (RBAC) que el cliente necesita para comprar las reservas de Azure para una suscripción de Azure que haya adquirido.

Es posible que algunos asociados ya hayan asignado el rol de **propietario** a los clientes que desean administrar y aprovisionar activamente sus propios recursos de Azure. Si ya ha asignado el estado de **propietario** a un cliente para administrar las suscripciones anteriores que ha adquirido para ellos, puede omitir este paso.  

> [!IMPORTANT]
> Si a un cliente no se le ha asignado el rol de **propietario** , recibirá un error en el Azure portal que le impedirá comprar reservas de Azure.

Para comprobar que el cliente tiene asignado el rol de **propietario** para una suscripción de Azure:

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

2. Seleccione **CSP**y luego **clientes** y seleccione el cliente específico.

3. Seleccione **suscripciones** para ese cliente y busque la suscripción de Azure específica.

4. Seleccione el botón **administrar** junto a la suscripción de ese cliente. Al hacerlo, se abre el [Azure portal](https://portal.azure.com/).

5. Para asignar el rol de **propietario** a un usuario específico, siga estos pasos [para asignar un usuario como administrador](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Activar o desactivar los permisos de los clientes para adquirir sus propias reservas de Azure

Después de comprobar que el cliente tiene una suscripción de Azure existente y a los usuarios se les asigna el rol de **propietario** de esa suscripción, está listo para activar (habilitar) los permisos de cliente. También puede usar estos pasos para desactivar (deshabilitar) los permisos de los clientes. Puede habilitar o deshabilitar los permisos de cliente mediante el panel del centro de Partners o las [API del centro de Partners](https://docs.microsoft.com/partner-center/develop/manage-customers).

Para activar (o desactivar) los permisos del cliente en el centro de Partners:

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

2. En el menú de navegación izquierdo, seleccione **CSP**y luego **clientes**. Aparece una lista de clientes.

3. Seleccione un nombre de cliente específico.

4. Seleccione **cuenta** en el menú cliente. Aparece la página **cuenta** de cliente.

5. Busque el área de **permisos del cliente** en la parte inferior de la página.

   ![Página permisos del cliente en la cuenta](images/give-customers-permission-reservations.png)

6. En **reservas de Azure**, busque la opción **permitir al cliente comprar** .

7. Para activar los permisos del cliente, mueva el conmutador junto a esta opción a la posición **activada** . Para desactivar los permisos del cliente, mueva el conmutador a la posición de **apagado** .

>[!NOTE]
> Para obtener información sobre lo que sucede cuando se activan los permisos de un cliente para comprar sus propias reservas de Azure, consulte [información general de los permisos de los clientes en el centro de Partners](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).
>
>Al activar (o desactivar) los permisos del cliente, el registro de actividad registra cada acción. (Este registro es accesible cuando se selecciona el icono de engranaje en la parte superior del panel del centro de Partners). Al activar o desactivar los permisos de los clientes, la acción aparecerá como **crear permisos de compra de cliente** o **eliminar permisos de compra de cliente** en el registro de actividad.

## <a name="help-customers-manage-reservations-they-purchase"></a>Ayudar a los clientes a administrar las reservas que compren

Una vez que dé permiso a los clientes para que compren sus propias reservas de Azure, puede ayudarles a administrar mejor los recursos que compren. Los clientes pueden administrar muchos aspectos de las reservas de Azure directamente desde el [Azure portal](https://portal.azure.com/). Necesitará su ayuda para administrar algunos aspectos de las reservas de Azure que compren en su suscripción de CSP.  

Ayude a los clientes a comprender mejor la administración de estos aspectos de las reservas de Azure:

- Precios que los clientes pagarán por las reservas de Azure
- Cómo los clientes pueden optimizar el uso de las reservas de Azure
- ¿Qué sucede cuando los clientes compran reservas con un ámbito compartido?
- ¿Qué ocurre si los clientes desean cambiar, cancelar y renovar una reserva, o cambiar su ámbito?

**Precios que los clientes pagarán por sus reservas.** El cliente adquirirá reservas de Azure en función de una suscripción que haya comprado previamente en su cuenta de facturación de asociados de CSP. El precio del cliente para las reservas de Azure que compren en función de esta suscripción también lo establece el usuario. Este precio puede ser diferente del precio directo que el cliente ve en el Azure Portal.

**Cómo los clientes pueden optimizar el uso de una reserva.** Algunos clientes pueden beneficiarse de obtener más información sobre cómo optimizar el uso de una reserva o cómo asignar el ámbito inicial de una reserva durante su compra. Para obtener más información, pida a los clientes que lean [administrar las reservas de recursos de Azure]( https://docs.microsoft.com/azure/cost-management-billing/reservations/manage-reserved-vm-instance).

**¿Qué ocurre cuando un cliente adquiere una reserva con un ámbito compartido?** Cuando los clientes adquieren una reserva basada en una suscripción de CSP anterior y asignan un ámbito compartido a esa reserva, los descuentos que el CSP haya proporcionado al cliente se aplicarán al uso de coincidencias para todas las suscripciones que el asociado de CSP haya adquirido para ese cliente.

**¿Qué deben hacer los clientes si desean intercambiar, cancelar o renovar una compra realizada o cambiar el ámbito inicial de una reserva?** Los clientes deben pedir a sus asociados que les ayuden a cambiar el ámbito inicial de una reserva. También necesitan la ayuda de un asociado para intercambiar, cancelar o renovar una reserva. No pueden realizar estas tareas con reservas basadas en suscripciones adquiridas por un asociado de CSP.

## <a name="next-steps"></a>Pasos siguientes

- [Compre las reservas de Azure en nombre de sus clientes](azure-reservations-buying.md)

- [Centro de Partners: vender reservas de Microsoft](azure-reservations.md)

- [Administrar las reservas de Azure en nombre de sus clientes](azure-reservations-manage.md)
