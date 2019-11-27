---
title: Facturación para productos comerciales de Marketplace | Centro de Partners
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo funciona la facturación para los productos o las suscripciones de SaaS de ISV comprados para los clientes del Marketplace comercial en el centro de Partners.
author: MicheleHope
ms.author: v-mihope
keywords: suscripciones, productos, compras, Marketplace, terceros, ISV, facturación, facturas, conciliación, archivo de conciliación
ms.localizationpriority: medium
ms.openlocfilehash: bc4dcca3d8c3d454a17eca676d5fadd1dac202d3
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384911"
---
# <a name="billing-for-commercial-marketplace-products"></a>Facturación para productos comerciales de Marketplace

**Se aplica a**

- Centro de partners
- Partners del programa CSP

**Roles adecuados**

- Administrador global
- Administrador de facturación

Como asociado en el programa CSP, puede usar el centro de partners para comprar productos SaaS basados en licencias de publicadores ISV en Marketplace comercial. Después de hacerlo, puede tener acceso a una factura para estos tipos de compras. El período de facturación se inicia el primer día del mes natural y finaliza el último día del mes natural. Las facturas se ponen a disposición del 8 día del mes siguiente.

Puede acceder a las facturas desde el [Panel](https://partner.microsoft.com/dashboard/) del centro de Partners o mediante las [API del centro de Partners](https://docs.microsoft.com/partner-center/develop/).

Los asociados del programa CSP se facturan por las soluciones de Marketplace comercial de ISV compradas para un cliente cuando compran dichos productos desde el centro de Partners o desde el Azure Portal (mediante el inquilino de Azure anterior del cliente, adquirido por CSP).

>[!NOTE]
>Si los clientes usan su propio inquilino de Azure AD (no adquirido de un socio en el programa CSP), los clientes también pueden optar por comprar su propia solución SaaS de ISV directamente desde ([Microsoft AppSource](https://appsource.microsoft.com/) o [Azure Marketplace](https://azuremarketplace.microsoft.com/)). Si lo hacen, recibirán su propia factura directamente de Microsoft. Del mismo modo, si un asociado del programa CSP vende un inquilino de Azure AD al cliente y concede el [acceso basado en rol](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles) del cliente a ese inquilino (asignando cualquier rol al cliente además del **lector**), ese cliente también puede comprar ofertas de Marketplace comercial sin aprobación previa o notificación al asociado de CSP. En estos casos, Microsoft no enviará directamente a los asociados del programa CSP sobre las compras realizadas por sus clientes. Sin embargo, Microsoft ofrece un mecanismo de [Azure monitor](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) opcional que puede usar para establecer alertas o notificaciones sobre la actividad en una suscripción de Azure.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Acceder a la información de facturación para productos comerciales de Marketplace

El administrador global o el administrador de facturación de tu empresa recibirá un correo electrónico cuando una factura esté lista para ver. Para acceder a la factura y el archivo de conciliación más recientes para compras de productos comerciales de Marketplace:

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard/) del Centro de partners.

2. En el menú del Centro de partners, selecciona **Billing** (Facturación). 

    Verá dos pestañas en la parte superior de la página de facturación: compras **periódicas** y **periódicas y de una sola vez**. Cada pestaña permite acceder a los archivos de factura y conciliación (concil) de distintos productos de Marketplace:

    - Pestaña **periódica** : muestra los archivos de factura y de conciliación para las suscripciones relacionadas con Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, PowerBI Pro y Microsoft Azure.

    - Pestaña **compras periódicas y de un solo tiempo** : muestra los archivos de factura y de conciliación para Azure plan, reservas de Azure, software y productos de Marketplace comerciales.
  
3. Seleccione la pestaña **compras periódicas y una sola vez** . Si adquirió suscripciones para un cliente en una moneda distinta, verá una pestaña para cada moneda. Puede hacer algunas cosas fr: OM esta página:

    - Para ver la factura y el archivo de conciliación más recientes, seleccione **factura** o **archivo de conciliación**. (Si lo desea, también puede acceder a los datos más recientes de la factura y del archivo de conciliación mediante las [API del centro de Partners](https://docs.microsoft.com/partner-center/develop/).

    - Para ver las facturas y los archivos de conciliación anteriores, expanda la fila **historial de facturación** que aparece a continuación.

    - Para comprobar el saldo de cuenta Estimado o la factura en cualquier momento en función de la actividad de la cuenta más reciente, seleccione un vínculo debajo del encabezado **estimaciones** .  

    >[!NOTE]
    > Cuando publiquemos su factura el octavo día del mes, se incluirán los impuestos y otros cargos y créditos aplicables. Esto significa que la cantidad final debida podría diferir de lo que se ve durante el período de facturación.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Más información sobre las facturas y los archivos de conciliación para productos comerciales de Marketplace

En esta sección se ofrece más información acerca de los archivos de facturación y de conciliación para las suscripciones de SaaS comerciales de Marketplace compradas para clientes de publicadores de ISV de terceros.

Al seleccionar compras **periódicas y de una sola vez** desde la opción **facturación** del menú del centro de Partners, obtiene acceso a las facturas y a los archivos de conciliación para los cargos relacionados con las compras de Microsoft (de terceros) y ISV (de terceros). Estas compras pueden estar asociadas a:

- Suscripciones de SaaS (de los publicadores de Microsoft o ISV)

- Plan de Azure

- Reservas de Azure

- Otro software basado en suscripción (de publicadores de Microsoft o ISV)

Algunos ejemplos de estas compras pueden ser el software SUSE Linux (una suscripción de software) o una suscripción de producto de SaaS de Azure ISV.

>[!NOTE]
> Para obtener más información sobre cómo leer archivos de factura y de conciliación, consulte también [información general sobre facturación](billing.md).

### <a name="tips-on-reading-your-invoice"></a>Sugerencias para leer la factura

Cuando compre un producto SaaS basado en licencia de un publicador de ISV de terceros, solo verá los cargos por la cuota de licencia de la factura. Esto es así incluso cuando el producto SaaS del ISV usa (o consume) recursos subyacentes de la infraestructura de Azure. Esto se debe a que los cargos de uso de la infraestructura de Azure del cliente para el producto SaaS de un ISV se facturan directamente al ISV. (Los ISV verán los cargos de consumo de Azure asociados en su propio archivo de conciliación de factura clasificado por el uso de Azure).

La factura contendrá varias páginas:

- **Página 1 de la factura:** Contiene información general de Resumen de los detalles de facturación del asociado del programa CSP. Esto incluye un resumen de los cargos para el período de facturación, un número de factura, los términos de pago (neto 60 días) y los métodos de pago de facturación para pagar por cable o por cheque.

- **Página 2 (y las páginas posteriores) de la factura:** Se cobran los cargos de las compras de Microsoft propias y las compras de terceros (basadas en licencias) del Marketplace comercial. Puede identificar las compras basadas en licencias de ISV por la línea del **publicador** debajo de cada nombre de producto. El archivo de conciliación asociado ofrece más detalles de facturación para los cargos de factura concretos.

- **Última página de la factura:** Si se le cobra por los productos de Marketplace basados en licencia de un ISV, en esta página final se mostrarán más detalles sobre el nombre y la dirección del editor de ISV.

### <a name="tips-on-reading-your-reconciliation-file"></a>Sugerencias para leer el archivo de conciliación

El archivo de conciliación de **compras periódicas y de un solo tiempo** contiene varias columnas con detalles adicionales que se asignan a los cargos de la factura. La columna **PublisherName** muestra si la compra es de Microsoft o de un publicador de ISV de terceros.

Algunos cargos del archivo de conciliación pueden aparecer con un costo de $0. Esto puede deberse a una oferta de "evaluación gratuita" de ISV (normalmente 30 o 60 días) o a una oferta de traiga su propia licencia.

En el caso de ofertas de ISV de evaluación gratuita:

- El período de evaluación gratuita cubre el costo del producto SaaS basado en licencia del ISV durante ese tiempo. Tampoco se le cobrará por el uso de la infraestructura de Azure asociado a ese producto SaaS.  Sin embargo, si usa una oferta de ISV basada en el uso, la evaluación gratuita no incluye el costo del uso de la infraestructura de Azure subyacente. En este caso, los cargos de uso de la infraestructura de Azure aparecerán en un archivo de conciliación de Azure independiente.

- Al adquirir e implementar el producto de la versión de prueba gratuita de un ISV para su cliente, el cliente se inscribe automáticamente en la evaluación gratuita del anunciante de ISV. El período de evaluación gratuita finaliza automáticamente después del período definido por el publicador de ISV. Una vez finalizado el período, se cobrará al cliente. Esto significa que el archivo de conciliación puede mostrar dos filas para un producto que cumpla la prueba: uno que realice un seguimiento del período de prueba y otro que realice un seguimiento de la oferta de pago (que mostrará un costo de $0 hasta que finalice el período de prueba). Una vez finalizada la evaluación, la fila que muestra la oferta de pago empezará a mostrar los cargos. 

Para obtener más información sobre lo que representa cada columna, vea [usar los archivos de conciliación](use-the-reconciliation-files.md). Vea también [tipos de facturación en el centro de Partners](billing-different-types.md)

## <a name="next-steps"></a>Pasos siguientes

- [Administrar productos comerciales de Marketplace para clientes](csp-commercial-marketplace-manage.md)
- [Más información sobre la compatibilidad con productos comerciales de Marketplace](csp-commercial-marketplace-support.md)
