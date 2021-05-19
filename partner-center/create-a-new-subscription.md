---
title: Creación de suscripciones de cliente en Centro de partners
ms.topic: how-to
ms.date: 05/17/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo vender suscripciones a sus clientes para productos publicados por Microsoft, así como productos SaaS publicados por ISV de terceros.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 3269fa994d704c0a0dae067087bad8589a7ce031
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148211"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Crear, suspender o cancelar suscripciones de clientes

**Se aplica a**: Centro de partners | Centro de partners para Microsoft Cloud for US Government

**Roles adecuados:** agente de administración | Administrador de facturación | Administrador global | Agente de soporte técnico | Agente de ventas

Después de crear un registro del cliente en el Centro de partners, puedes venderle suscripciones a los productos del catálogo. Esto incluye los productos publicados por Microsoft y los productos de software como servicio (SaaS) publicados por proveedores de software independientes (ISV) de terceros en el [marketplace comercial.](https://azuremarketplace.microsoft.com/marketplace)

Algunas ofertas están limitadas a una suscripción por cliente. Para ver una lista de las ofertas restringidas, visita la página Precios y ofertas del Centro de partners.

>[!IMPORTANT]
> Como asociado del programa CSP,  puede comprar suscripciones **SaaS** basadas en licencias o de uso medidor a publicadores de ISV dentro de Centro de partners. Esto significa que puede comprar **cualquier** oferta **de** SaaS basada en licencia o [](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) con uso que el publicador de ISV haya puesto a su disposición, incluidas las ofertas exclusivas a las que tenga acceso. Para comprar o administrar otras ofertas de Marketplace comercial de ISV (como ofertas basadas en el uso que implican aplicaciones de Azure, contenedores o máquinas [virtuales),](https://portal.azure.com/)debe ir al Azure Portal .

## <a name="create-a-new-subscription"></a>Crear una nueva suscripción

1. Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard).

2. Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.

3. Seleccione **Agregar suscripción**. La **pestaña Servicios en** línea mostrará todas las ofertas de SaaS de Marketplace disponibles.

4. Para ver solo determinados tipos de suscripciones, haz selecciones en los filtros disponibles:
   - **Publicador:** elija **Microsoft** para ver solo las ofertas de Microsoft o **partner** para ver los productos de Marketplace comercial publicados por ISV.
   - **Tipo de facturación:** seleccione el tipo de facturación de suscripción que desea usar: **Licencia** o **Uso.** Consulte [Facturación basada en licencias](license-based-billing.md) para obtener información que le ayudará a decidir entre la frecuencia de facturación mensual y anual.
   - **Categoría:** elija **Enterprise,** **Small Business** o **Trial.** Para obtener información sobre las suscripciones de prueba, consulta [Ofrecer a los clientes pruebas de productos de Microsoft](offer-your-customers-trials-of-microsoft-products.md).

5. Seleccione las suscripciones de producto que desea comprar para el cliente. Los productos que vea dependen del tipo de segmento de cliente (educación, administración pública, etc.) y de los filtros que haya aplicado. Es posible que algunas ofertas que se muestran en Marketplace no estén siempre disponibles para un cliente específico o un asociado de CSP específico. Esto puede deberse a:

   - El cliente ya tiene una suscripción a ese producto y solo se permite una.

   - Es posible que la suscripción del cliente se haya suspendido (en este caso, puede reactivar la suscripción en lugar de comprar una nueva).

   - En el caso de las ofertas saaS de ISV, puede haber algunas razones por las que la oferta no está disponible para comprarse: es posible que el ISV no admita el país o región de facturación del cliente; es posible que el ISV haya decidido no hacer que la oferta esté disponible a través del programa CSP; o bien, es posible que el ISV haya hecho que la oferta [sea exclusiva](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) solo para determinados asociados de CSP. La oferta de ISV también puede no ser transaccionable a través de Centro de partners (por ejemplo, contenedores o algunas ofertas basadas en el uso).  

6. Para cada suscripción que quiera agregar, escriba el número de licencias (si es necesario) y **seleccione Agregar al carro.**

7. Cuando haya terminado de agregar suscripciones, seleccione **Revisar** y revisar el pedido.

8. Una vez que haya revisado los pedidos y esté listo para comprar estas suscripciones, seleccione **Comprar.**

9. Después de comprar una suscripción para un cliente, se producirá lo siguiente:

    - Puede revisar o editar la suscripción seleccionando el nombre de la suscripción en la página **Suscripciones de ese** cliente. Desde aquí, puedes seleccionar licencias de complementos, si hay alguna disponible, cambiar la cantidad de licencias o suspender la suscripción.

    **Para suscripciones SaaS de ISV (basadas en licencias y medidas):**
    - Recibirá un vínculo al sitio del publicador del ISV. Este vínculo debería ayudarle a completar la implementación o la configuración de la cuenta de la suscripción del cliente.
      
    >[!NOTE]
    > Ni usted ni el cliente recibirán un correo electrónico con instrucciones para completar la configuración o el aprovisionamiento de cuentas para este tipo de suscripción de ISV).

    - Si la suscripción incluye una evaluación gratuita de 30 días, el período de evaluación gratuita se aplicará automáticamente. Como asociado del programa CSP, no puede suspender el período de evaluación gratuita en las ofertas que compre para los clientes. Una vez que finalice el período de evaluación gratuita, se iniciará el período de suscripción y la suscripción se convertirá al estado de pago. La suscripción se renovará automáticamente según la misma programación.
   
## <a name="update-subscriptions-with-add-ons"></a>Actualizar suscripciones con complementos 

Para comprar un complemento, el cliente debe tener primero una suscripción base activa.  No se pueden comprar complementos a través del catálogo.

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

2. Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.

3. Selecciona la suscripción que deseas administrar.

4. Debajo **de la sección** Estado, se muestra una lista de complementos disponibles para la suscripción.  

5. Actualice la cantidad de licencias para cada complemento necesario. Haga clic en **Enviar** para enviar los cambios.

La capacidad de comprar complementos a través de Centro de partners solo está disponible para proveedores indirectos y de factura directa.
Solo se muestran complementos aptos en función de los requisitos base y la disponibilidad regional. Para más información sobre los precios y las ofertas, consulte la matriz de ofertas de revendedores en la nube. Al suspender la suscripción base, también se suspenderán los complementos asociados.

Las fechas de inicio de los complementos se alinean con la suscripción base y los cargos se calculan a partir de la fecha de inicio y la fecha de finalización del cargo con cargos prorrateados en la primera factura. Para más información, consulte [Facturación basada en licencias.](license-based-billing.md)


## <a name="suspend-or-cancel-a-subscription"></a>Suspender o cancelar una suscripción

Los partners pueden suspender o cancelar una suscripción si el cliente lo solicita, o en casos de impago o fraude.

### <a name="suspend-a-subscription"></a>Suspender una suscripción

Si cambias el estado de una suscripción a **Suspendida**, los usuarios no podrán iniciar sesión ni acceder a los servicios.

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

2. Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.

3. Selecciona la suscripción que deseas administrar.

4. En la sección **Estado**, elija **Suspendida**. Haga clic en **Enviar** para enviar los cambios.

5. Se eliminarán todos los datos a menos que la suscripción se reactive en un plazo de 90 días o 90 días más el número de días entre el momento en el que se abrió la cuenta y el primer período de facturación (120 días como máximo).

Cuando se suspende una suscripción, la fecha que aparece debajo del botón **Suspendida** indica la fecha en que la suscripción expiraría automáticamente si no se vuelve a activar. 

>[!NOTE]
>Las suscripciones de CSP no tienen un período expirado (la forma en que lo hacen las suscripciones web directas) durante el cual los servicios siguen funcionando, pero la suscripción no genera ningún cargo de facturación. Las suscripciones de CSP están activas o suspendidas (o totalmente eliminadas).

### <a name="cancel-a-subscription"></a>Cancelación de una suscripción

Puede cancelar suscripciones de SaaS basadas en licencias de publicadores de ISV de terceros dentro Centro de partners [marketplace comercial.](csp-commercial-marketplace-overview.md) Siempre y cuando cancele dentro del período de cancelación, recibirá un reembolso completo.

Para las ofertas de ISV facturadas mensualmente:

- Si cancela menos de 24 horas después de realizar el pedido, recibirá un crédito completo en la siguiente factura.

- Si cancela más de 24 horas después de realizar el pedido, la cancelación se programará para que se produzca en la renovación.

Para ofertas facturadas anualmente:

- Si cancela menos de 14 días después de realizar el pedido, recibirá un crédito completo en la siguiente factura.

- Si cancela más de 14 días después de realizar el pedido, la cancelación se programará para que se produzca en la renovación.

Una vez transcurridos estos períodos, ya no verá la opción de cancelar la suscripción.

> [!NOTE]
> Los servicios de ISV de terceros basados en el uso y de uso (que usan máquinas virtuales o contenedores, por ejemplo) no son aptos para la devolución. Los servicios basados en el uso se pueden cancelar el aprovisionamiento como método de cancelación. Dado que los cargos se facturan después del uso, estos servicios no son aptos para un reembolso.

Para cancelar una suscripción de SaaS basada en licencia de un publicador de ISV, haga lo siguiente:

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

2. Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.

3. Busque la suscripción que desea cancelar.

4. En la **columna Estado,** seleccione **Cancelar.** Haga clic en **Enviar** para enviar los cambios.

5. Si aparece un cuadro de diálogo, rellene los detalles pertinentes y seleccione **Enviar**.

6. Para confirmar la cancelación, seleccione **Sí, cancelar**.

> [!NOTE]
> También puede optar por cancelar una suscripción Azure Marketplace mediante las API. Para ello, consulte Cancel an Azure Marketplace subscription (Cancelar [una Azure Marketplace suscripción).](/partner-center/develop/cancel-an-azure-marketplace-subscription)

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Elegir si se va a renovar automáticamente una suscripción de Marketplace comercial

De forma predeterminada, las suscripciones activas se configuran para que se renueven automáticamente cuando expire el período de suscripción. En [el caso de las suscripciones a productos de Marketplace](csp-commercial-marketplace-overview.md)comercial, puede optar por no renovar automáticamente la suscripción.

Para impedir que una suscripción de Marketplace comercial activa se renueve automáticamente:

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

2. Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.

3. Seleccione **Suscripciones**. Aquí se enumeran todas las suscripciones basadas en licencias que haya adquirido para el cliente.

4. En la **columna** Suscripción, seleccione la suscripción que desea modificar.

5. En la página de detalles de la suscripción, busque la **sección Estado** y desactive la **casilla Renovación** automática.

6. Seleccione **Submit** (Enviar).

## <a name="next-steps"></a>Pasos siguientes

- [Compra de productos de Marketplace comercial para tus clientes](csp-commercial-marketplace-purchase.md)

- [Administración de productos de Marketplace comercial para sus clientes](csp-commercial-marketplace-manage.md)

- [Introducción a Marketplace comercial](csp-commercial-marketplace-overview.md)