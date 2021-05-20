---
title: Permitir que los clientes compren sus propios servicios en CSP
description: Obtenga información sobre cómo los asociados del programa CSP pueden permitir que los clientes compren sus propios servicios, como las reservas de Azure, para una suscripción comprada para ellos en Centro de partners.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9fabd6bd188c9d596128672d9fce3321db9b5432
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150767"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Conceder permiso a los Centro de partners para comprar sus propios productos o servicios

**Roles adecuados:** agente de administración | Agente de ventas

En este artículo se muestra cómo un asociado del programa Proveedor de soluciones en la nube (CSP) puede conceder a un cliente permiso para comprar algunos de sus propios servicios o recursos.

Los asociados del programa CSP a menudo usan Centro de partners y su marketplace comercial para comprar soluciones y servicios para sus clientes. A continuación, los asociados permiten que algunos clientes aprovisionen estos servicios directamente desde el Azure Portal.

A continuación se muestra un ejemplo. Supongamos que compra una suscripción al plan de Azure para un cliente de Centro de partners. A continuación, decide agregar otros recursos o servicios a esa suscripción en nombre del cliente. En este caso, puede agregar reservas de Azure a la suscripción del cliente (por ejemplo, agregar instancias reservadas de máquina virtual). A continuación, puede permitir que el cliente aprovisione aún más los recursos de reserva de Azure en el Azure Portal.

Ahora, con la **característica Permisos de** cliente, proporciona a los clientes más opciones de autoservicio con recursos de Azure. Al activar los permisos para el cliente, permite a los clientes comprar sus propios recursos (por ejemplo, comprar sus propias reservas de Azure).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Introducción a los permisos de cliente en Centro de partners

Use la página **Cuenta de** cliente para activar (o desactivar) los permisos de cliente. Actualmente, esta característica admite:

- **Reservas de Azure:** Activar este permiso permite al cliente comprar sus propias reservas de Azure para una suscripción de Azure específica que haya adquirido para ellos.

Antes de activar los permisos de cliente, tenga en cuenta estos puntos importantes:

- De forma predeterminada, los permisos de cliente se deshabilitan (desactivan) automáticamente en Centro de partners.

- Para poder activar (o desactivar) los permisos de un cliente, se le debe asignar el rol de Agente de administración en Centro de partners.

  Los asociados asignados al rol de agente de ventas o agente del departamento de soporte electrónico tienen acceso de solo lectura y no pueden activar o desactivar los permisos de los clientes.

- Puede activar (habilitar) los permisos para cualquier cliente que elija.

- Puede activar (o desactivar) los permisos de cliente mediante el panel de Centro de partners o [Centro de partners API](/partner-center/develop/manage-customers).

- Después de activar (habilitar) los permisos para un cliente específico, será responsable de pagar las compras posteriores realizadas por ese cliente. Si los clientes quieren intercambiar, cancelar o renovar una compra que han realizado (o quieren cambiar el ámbito inicial de una reserva), no podrán hacerlo ellos mismos. Deben pedirle, como asociado, que les ayude a intercambiar, cancelar y renovar compras, o realizar cambios posteriores en el ámbito de una reserva.  

- Después de activar los permisos para un  cliente específico, no se le notificará ninguna compra posterior realizada por el cliente.

- Las compras posteriores realizadas por el cliente aparecerán en Centro de partners junto con las compras realizadas por usted. Puede encontrar estas compras en la página Historial  de pedidos **del** cliente, su página Reservas o en el Registro [**de actividad**](activity-logs.md).

>[!NOTE]
> Para obtener información sobre los precios que el cliente pagará y cómo ayudar a los clientes a administrar sus compras, consulte Ayuda a los clientes a administrar [las reservas que compran.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Conceder a los clientes permiso para comprar sus propias reservas de Azure

Las reservas de Azure son una excelente manera de comprar servicios de Azure a una tarifa con descuento. Para más información sobre las ventajas de las reservas de Azure, consulte [¿Qué son las reservas de Azure?](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Ahora tiene la opción de comprar reservas de Azure en nombre de los clientes, como puede que ya lo haya hecho. O bien, puede conceder permiso a los clientes para comprar sus propias reservas de Azure.

>[!NOTE]
> Después de conceder permiso a los clientes para comprar sus propias reservas de Azure, ayúdelos a administrar las reservas que compren. Para obtener más información, consulte [Ayuda a los clientes a administrar las reservas que compran.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Para permitir que los clientes compren sus propias reservas de Azure

1. Compruebe que el cliente tiene un plan de Azure existente o una suscripción global de Azure que compró en su nombre.

2. Compruebe que al cliente se le ha asignado el **rol Propietario** para esta suscripción.

3. Habilite los permisos de los clientes (active **esta** característica) para comprar sus propias reservas de Azure.

Cada paso aparece a continuación.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Comprobación de que el cliente tiene una suscripción de Azure existente

Antes de conceder permiso a los clientes para comprar sus propias reservas de Azure, debe comprobar que el cliente tiene un plan de Azure existente o una suscripción global de Azure. Si el cliente no muestra ninguna suscripción de Azure actual en Centro de partners, debe comprar una suscripción para ellos antes de activar sus permisos de cliente.

- Para ver si un cliente ya tiene una suscripción de Azure, inicie sesión en el panel Centro de partners y, a continuación, seleccione **CSP** seguido de **Clientes.** Seleccione el cliente específico de la lista. A **continuación,** seleccione Suscripciones y busque las suscripciones basadas en el uso para el plan de Azure o Azure Global.

- Si un cliente no tiene una suscripción de Azure existente, puede comprar una suscripción para ellos. Consulte [Compra del plan de Azure.](purchase-azure-plan.md)

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Comprobación de que el cliente tiene asignado el rol correcto en Azure

Después de comprobar que el cliente tiene una suscripción de Azure existente, también debe  comprobar que a los usuarios clave asociados con el cliente se les ha asignado el rol de propietario correcto para esa suscripción de Azure. Este es el acceso basado en rol (RBAC) que el cliente necesita para comprar reservas de Azure para una suscripción de Azure que haya adquirido.

Es posible que algunos  asociados ya tengan asignado el rol propietario a los clientes que desean administrar y aprovisionar activamente sus propios recursos de Azure. Si ya ha asignado el **estado** de propietario a un cliente para administrar las suscripciones anteriores que ha adquirido para ellos, puede omitir este paso.  

> [!IMPORTANT]
> Si a un cliente  no se le ha asignado el rol propietario, recibirá un error en el Azure Portal impedirle comprar reservas de Azure.

Para comprobar que al cliente se le ha asignado el **rol propietario** de una suscripción de Azure:

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

2. Seleccione **CSP** y, a **continuación, Clientes** y seleccione el cliente específico.

3. Seleccione **Suscripciones** para ese cliente y busque la suscripción de Azure específica.

4. Seleccione el **botón** Administrar situado junto a la suscripción de ese cliente. Al hacerlo, se abre [el Azure Portal](https://portal.azure.com/).

5. Para asignar el **rol Propietario** a un usuario específico, siga estos pasos para asignar un usuario [como administrador.](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Activar o desactivar los permisos de los clientes para comprar sus propias reservas de Azure

Después de comprobar que el cliente tiene una  suscripción de Azure existente y a los usuarios se les asigna el rol propietario para esa suscripción, está listo para activar (habilitar) los permisos de cliente. También puede usar estos pasos para desactivar (deshabilitar) los permisos de cliente. Puede habilitar o deshabilitar los permisos de cliente mediante el panel de Centro de partners o [Centro de partners API](/partner-center/develop/manage-customers).

Para activar (o desactivar) los permisos de cliente en Centro de partners:

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

2. En el menú de navegación izquierdo, seleccione **CSP** y, a continuación, **Clientes.** Aparece una lista de clientes.

3. Seleccione un nombre de cliente específico.

4. Seleccione **Cuenta** en el menú del cliente. Aparece la **página Cuenta** de cliente.

5. Busque el **área Permisos de** cliente en la parte inferior de la página.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Permisos de cliente en la página Cuenta." border="true":::

6. En **Reservas de Azure,** busque la **opción Permitir que el cliente compre.**

7. Para activar los permisos de cliente, mueva el conmutador situado junto a esta opción a la **posición Activar.** Para desactivar los permisos de cliente, mueva el conmutador a la **posición Desactivado.**

>[!NOTE]
> Para saber qué más ocurre al activar los permisos de un cliente para comprar sus propias reservas de Azure, consulte Introducción a los permisos de cliente [en Centro de partners](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).
>
>Al activar (o desactivar) los permisos de cliente, el registro de actividad registra cada acción. (Este registro es accesible cuando se selecciona el icono de engranaje en la parte superior del Centro de partners panel). Al activar o desactivar los permisos de cliente,  la acción aparecerá como Crear permisos de compra del cliente o Eliminar permisos de compra del cliente en **el** registro de actividad.

## <a name="help-customers-manage-reservations-they-purchase"></a>Ayudar a los clientes a administrar las reservas que compran

Una vez que dé permiso a los clientes para comprar sus propias reservas de Azure, puede ayudarles a administrar mejor los recursos que compren. Los clientes pueden administrar muchos aspectos de las reservas de Azure directamente desde el [Azure Portal](https://portal.azure.com/). Necesitarán su ayuda para administrar algunos otros aspectos de las reservas de Azure que compran dentro de su suscripción de CSP.  

Ayude a los clientes a comprender más sobre la administración de estos aspectos de las reservas de Azure:

- Precios que los clientes pagarán por las reservas de Azure
- Cómo los clientes pueden optimizar el uso de las reservas de Azure
- ¿Qué ocurre cuando los clientes compran reservas con un ámbito compartido?
- ¿Qué ocurre si los clientes quieren cambiar, cancelar y renovar una reserva o cambiar su ámbito?

**Precios que los clientes pagarán por sus reservas.** El cliente comprará reservas de Azure en función de una suscripción que haya comprado anteriormente para ellas en su cuenta de facturación del asociado de CSP. El precio del cliente para las reservas de Azure que compre en función de esta suscripción también se establece por usted. Este precio puede ser diferente del precio de Web Direct que el cliente ve en el Azure Portal.

**Cómo los clientes pueden optimizar su uso de una reserva.** Algunos clientes pueden beneficiarse de aprender más sobre cómo optimizar el uso de una reserva o cómo asignar el ámbito inicial de una reserva durante su compra. Para más información, pida a los clientes que lean [Administración de reservas para recursos de Azure.](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)

**¿Qué ocurre cuando un cliente compra una reserva con un ámbito compartido?** Cuando los clientes compran una reserva basada en una suscripción de CSP anterior y asignan un ámbito compartido a esa reserva, los descuentos que el CSP haya dado al cliente se aplicarán al uso correspondiente para todas las suscripciones que el asociado de CSP haya adquirido para ese cliente.

**¿Qué deben hacer los clientes si quieren intercambiar, cancelar o renovar una compra que han realizado o cambiar el ámbito inicial de una reserva?** Los clientes deben pedir a su asociado que les ayude a cambiar el ámbito inicial de una reserva. También necesitan la ayuda de un asociado para intercambiar, cancelar o renovar una reserva. No pueden realizar estas tareas por sí mismos con reservas basadas en suscripciones adquiridas por un asociado de CSP.

## <a name="next-steps"></a>Pasos siguientes

- [Compra de reservas de Azure en nombre de los clientes](azure-reservations-buying.md)

- [Centro de partners: venta de reservas de Microsoft](azure-reservations.md)

- [Administración de reservas de Azure en nombre de los clientes](azure-reservations-manage.md)