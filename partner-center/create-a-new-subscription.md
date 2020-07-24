---
title: Crear suscripciones de cliente en el centro de Partners
ms.topic: article
ms.date: 07/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprenda a vender sus suscripciones de clientes a productos publicados por Microsoft, así como a productos SaaS publicados por fabricantes de software independientes de terceros.
author: BillLinzbach
ms.author: BillLi
ms.custom: SEOAPR.20
ms.localizationpriority: medium
ms.openlocfilehash: 3e154fd217af8ca0f5d45c686467e671e5bd9a03
ms.sourcegitcommit: f8e8803b7d9fdf801ba181015a07dc6b570621c0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/22/2020
ms.locfileid: "86949841"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Crear, suspender o cancelar suscripciones de clientes

**Se aplica a**

- Centro de partners
- Centro de partners para Microsoft Cloud for US Government
- Partners de CSP

**Roles adecuados**

- Agente de administrador
- Administrador de facturación
- Administrador global
- Agente del departamento de soporte técnico
- Agente de ventas

Después de crear un registro del cliente en el Centro de partners, puedes venderle suscripciones a los productos del catálogo. Esto incluye productos publicados por Microsoft, así como productos de software como servicio (SaaS) publicados por fabricantes de software independientes (ISV) de terceros en el [Marketplace comercial](https://azuremarketplace.microsoft.com/marketplace).

Algunas ofertas se limitan a una suscripción por cliente. Para ver una lista de las ofertas restringidas, visita la página Precios y ofertas del Centro de partners.

> [!IMPORTANT]
> Como asociado en el programa CSP, solo puede comprar suscripciones de SaaS **basadas en licencias** de los publicadores ISV del centro de Partners. Esto significa que puede comprar cualquier oferta **de SaaS basada en licencia** que el publicador de ISV le haya puesto a su disposición, incluidas las [ofertas exclusivas](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) a las que tenga acceso. Para comprar o administrar otras ofertas comerciales de Marketplace de fabricantes de software independientes (como las ofertas basadas en **el uso, el uso**medido o las basadas en el consumo que impliquen aplicaciones, contenedores o máquinas virtuales de Azure), debe ir al [portal de administración de Azure](https://portal.azure.com/). Para obtener más información, consulte [comprar productos comerciales de Marketplace](csp-commercial-marketplace-purchase.md).

## <a name="create-a-new-subscription"></a>Crear una nueva suscripción

1. Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard).

2. Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.

3. Seleccione **Agregar suscripción**. En la pestaña **servicios en línea** se mostrarán todas las ofertas de SaaS de Marketplace disponibles.

4. Para ver solo determinados tipos de suscripciones, haz selecciones en los filtros disponibles:
   - **Publicador**: elija **Microsoft** para ver solo las ofertas de Microsoft o **Partner** para ver los productos comerciales de Marketplace publicados por ISV.
   - **Tipo de facturación**: seleccione el tipo de facturación de la suscripción que quiere usar: **licencia** o **uso**. Consulte [facturación basada en licencias](license-based-billing.md) para obtener información que le ayude a decidir entre la frecuencia de facturación mensual y anual.
   - **Categoría**: elija **empresa**, **pequeña empresa**o **prueba**. Para obtener información sobre las suscripciones de prueba, consulta [Ofrecer a los clientes pruebas de productos de Microsoft](offer-your-customers-trials-of-microsoft-products.md).

5. Seleccione las suscripciones de producto que desea comprar para su cliente. Los productos que se ven dependen del tipo de segmento de cliente (educación, gobierno, etc.) y de los filtros aplicados. Es posible que algunas ofertas que se muestran en Marketplace no siempre estén disponibles para un cliente específico o un asociado de CSP específico. Esto puede deberse a:

   - El cliente ya tiene una suscripción a ese producto y solo se permite uno.

   - Es posible que se haya suspendido la suscripción del cliente (en este caso, puede reactivar la suscripción en lugar de adquirir una nueva).

   - En el caso de las ofertas de SaaS de ISV, puede haber varias razones por las que la oferta no está disponible para su compra: es posible que el ISV no sea compatible con el país o la región de facturación del cliente. es posible que el ISV haya elegido no poner la oferta a disposición a través del programa CSP; o bien, es posible que el ISV haya realizado la oferta [exclusiva](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) para ciertos asociados de CSP. La oferta ISV también puede no ser transactable a través del centro de Partners (por ejemplo, contenedores o algunas ofertas basadas en el uso).  

6. Para cada suscripción que quiera agregar, escriba el número de licencias (si es necesario) y seleccione **Agregar al carro**.

7. Cuando haya terminado de agregar las suscripciones, seleccione **revisar** y revise el pedido.

8. Una vez que haya revisado los pedidos y estén listos para comprar estas suscripciones, seleccione **comprar**.

9. Después de comprar una suscripción para un cliente, ocurrirá lo siguiente:

    - Puede revisar o editar la suscripción seleccionando el nombre de la suscripción en la página de **suscripciones** de ese cliente. Desde aquí, puedes seleccionar licencias de complementos, si hay alguna disponible, cambiar la cantidad de licencias o suspender la suscripción.

    **Para las suscripciones de SaaS de ISV (basadas en licencias):**
    - Recibirá un vínculo al sitio del editor de ISV. Este vínculo le ayudará a completar la configuración de la implementación o la cuenta de la suscripción del cliente.
      
    >[!NOTE]
    > Ni usted ni su cliente recibirán un correo electrónico con instrucciones para completar el aprovisionamiento o la configuración de la cuenta para este tipo de suscripción de ISV).

    - Si su suscripción incluye una versión de evaluación gratuita de 30 días, el período de evaluación gratuita se aplicará automáticamente. Como asociado en el programa CSP, no puede renunciar al período de evaluación gratuita en las ofertas que compre para los clientes. Una vez finalizado el período de evaluación gratuita, se iniciará el período de la suscripción y la suscripción se convertirá en el estado de pago. La suscripción se renovará automáticamente según la misma programación.
   
## <a name="update-subscriptions-with-add-ons"></a>Actualizar suscripciones con complementos 

Para comprar un complemento, el cliente debe tener primero una suscripción base activa.  No se pueden comprar complementos a través del catálogo.

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

2. Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.

3. Selecciona la suscripción que deseas administrar.

4. Debajo de la sección **Estado** , se muestra una lista de complementos disponibles para la suscripción.  

5. Actualice la cantidad de licencias para cada complemento necesario. Haga clic en **Enviar** para enviar los cambios.

La capacidad de comprar complementos a través del centro de Partners solo está disponible para los proveedores directos de facturación e indirectos.
Solo se muestran los complementos válidos en función de los requisitos base y la disponibilidad regional. Consulte la matriz de la oferta del Reseller de la nube para obtener más información sobre precios y ofertas.  Al suspender la suscripción base, también se suspenderán los complementos asociados.

Las fechas de inicio de los complementos se alinean con la suscripción base y los cargos se calculan a partir de la fecha de inicio y la fecha de finalización del cargo con cargos prorrateados en la primera factura. Para obtener más información, consulte [facturación basada en licencias](license-based-billing.md).


## <a name="suspend-or-cancel-a-subscription"></a>Suspender o cancelar una suscripción

Los partners pueden suspender o cancelar una suscripción si el cliente lo solicita, o en casos de impago o fraude.

### <a name="suspend-a-subscription"></a>Suspender una suscripción

Si cambias el estado de una suscripción a **Suspendida**, los usuarios no podrán iniciar sesión ni acceder a los servicios.

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

2. Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.

3. Selecciona la suscripción que deseas administrar.

4. En la sección**Estado**, elija **Suspendida**. Haga clic en **Enviar** para enviar los cambios.

5. Se eliminarán todos los datos a menos que la suscripción se reactive en un plazo de 90 días o 90 días más el número de días entre el momento en el que se abrió la cuenta y el primer período de facturación (120 días como máximo).

Cuando se suspende una suscripción, la fecha que aparece debajo del botón **Suspendida** indica la fecha en que la suscripción expiraría automáticamente si no se vuelve a activar. 

### <a name="cancel-a-subscription"></a>Cancelación de una suscripción

Tiene la opción de cancelar las suscripciones de SaaS basadas en licencias de los publicadores de ISV de terceros en el [Marketplace comercial](csp-commercial-marketplace-overview.md)del centro de Partners. Siempre que se cancele el período de cancelación, recibirá un reembolso completo.

Para las ofertas de ISV facturadas mensualmente:

- Si cancela menos de 24 horas después de haber realizado el pedido, recibirá un crédito completo en la factura siguiente.

- Si cancela más de 24 horas después de haber realizado el pedido, la cancelación se programará para que se produzca durante la renovación.

Para las ofertas facturadas anualmente:

- Si cancela menos de 14 días después de realizar el pedido, recibirá un crédito completo en la factura siguiente.

- Si cancela más de 14 días después de realizar el pedido, la cancelación se programará para que se produzca durante la renovación.

Una vez finalizados estos períodos, ya no verá la opción de cancelar la suscripción.

> [!NOTE]
> Los servicios de ISV de terceros basados en uso y medidos (que usan máquinas virtuales o contenedores, por ejemplo) no son válidos para la devolución. Los servicios basados en el uso se pueden desaprovisionar como método de cancelación. Dado que los cargos se facturan después del uso, estos servicios no son válidos para un reembolso.

Para cancelar una suscripción de SaaS basada en licencia de un publicador de ISV, haga lo siguiente:

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

2. Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.

3. Busque la suscripción que desea cancelar.

4. En la columna **Estado** , seleccione **Cancelar**. Haga clic en **Enviar** para enviar los cambios.

5. Si aparece un cuadro de diálogo, rellene los detalles pertinentes y, a continuación, seleccione **submit (enviar**).

6. Para confirmar la cancelación, seleccione **sí, cancelar**.

> [!NOTE]
> También puede optar por cancelar una suscripción de Azure Marketplace mediante las API. Para ello, consulte [cancelación de una suscripción de Azure Marketplace](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Elegir si se va a renovar automáticamente una suscripción de Marketplace comercial

De forma predeterminada, las suscripciones activas se configuran para que se renueven automáticamente cuando expire el período de suscripción. En el caso de las [suscripciones a productos comerciales de Marketplace](csp-commercial-marketplace-overview.md), opcionalmente, puede optar por no renovar la suscripción automáticamente.

Para detener la renovación automática de una suscripción de Marketplace comercial activa:

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

2. Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.

3. Seleccione **Suscripciones**. Aquí se enumeran las suscripciones basadas en licencias que ha adquirido para el cliente.

4. En la columna **suscripción** , seleccione la suscripción que desea modificar.

5. En la página Detalles de la suscripción, busque la sección **Estado** y desactive la casilla **renovación automática** .

6. Seleccione **Submit** (Enviar).

## <a name="next-steps"></a>Pasos siguientes

- [Compra de productos de Marketplace comercial para tus clientes](csp-commercial-marketplace-purchase.md)

- [Administrar productos comerciales de Marketplace para sus clientes](csp-commercial-marketplace-manage.md)

- [Introducción a Marketplace comercial](csp-commercial-marketplace-overview.md)
