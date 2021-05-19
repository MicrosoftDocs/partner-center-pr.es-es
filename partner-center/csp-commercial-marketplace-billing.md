---
title: Facturación de productos de Marketplace comercial
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo funciona la facturación de los productos o suscripciones saaS de ISV adquiridos para los clientes del marketplace comercial en Centro de partners.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c25d4ab3077c6a0f648c767472e8b7b60ef53a9c
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148030"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Facturación de productos y suscripciones de Marketplace comercial en Centro de partners


**Roles adecuados:** Administrador global | Administrador de facturación

Como asociado del programa CSP, puede usar Centro de partners para comprar productos SaaS basados en licencias de publicadores de ISV en marketplace comercial. Después de hacerlo, puede acceder a una factura para estos tipos de compras. El período de facturación comienza el primer día del mes natural y finaliza el último día del mes natural. Las facturas están disponibles el día 8 del mes siguiente.

Puede acceder a las facturas desde el Centro de partners [o](https://partner.microsoft.com/dashboard/) mediante Centro de partners [API](/partner-center/develop/).

Los partners del programa CSP se facturan por las soluciones de marketplace comercial de ISV adquiridas para un cliente cuando compran esos productos desde Centro de partners o desde Azure Portal (mediante el inquilino de Azure adquirido por CSP anterior del cliente).

>[!NOTE]
>Si los clientes usan su propio inquilino de Azure AD (no uno comprado a un asociado en el programa CSP), los clientes también pueden optar por comprar su propia solución SaaS de ISV directamente desde ([Microsoft AppSource](https://appsource.microsoft.com/) [o Azure Marketplace](https://azuremarketplace.microsoft.com/)). Si lo hacen, recibirán su propia factura directamente de Microsoft. Del mismo modo, si un asociado del programa CSP vende una suscripción de Azure o el nuevo plan de Azure al cliente y concede al cliente (o revendedor [indirecto)](/azure/role-based-access-control/built-in-roles) acceso basado en roles a ese inquilino (asignando cualquier rol al cliente además de **Lector),** ese cliente (o revendedor indirecto) también puede comprar ofertas de Marketplace comercial sin aprobación previa ni notificación al asociado de CSP. En estos casos, Microsoft no notificará directamente a los partners del programa CSP las compras realizadas por sus clientes. Sin embargo, Microsoft ofrece un Azure Monitor [opcional](/azure/azure-monitor/platform/alerts-activity-log) que puede usar para establecer alertas o notificaciones sobre la actividad en una suscripción de Azure.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Acceso a la información de facturación de productos de Marketplace comercial

El administrador global o el administrador de facturación de tu empresa recibirá un correo electrónico cuando una factura esté lista para ver. Para acceder al archivo de factura y conciliación más reciente para las compras de productos de Marketplace comercial:

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard/) del Centro de partners.

2. En el menú del Centro de partners, selecciona **Billing** (Facturación). 

    Verá dos pestañas en la parte superior  de la página Facturación: Periódicas y periódicas **y compras únicas.** Cada pestaña le permite acceder a los archivos de factura y conciliación (conciliación) de diferentes productos de Marketplace:

    - **Pestaña** Periódica: muestra los archivos de facturación y conciliación de las suscripciones relacionadas con Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro y Microsoft Azure.

    - **Pestaña Compras periódicas y únicas:** muestra los archivos de factura y conciliación del plan de Azure, las reservas de Azure, el software y los productos de Marketplace comercial.
  
3. Seleccione la **pestaña Compras periódicas y únicas.** Si ha adquirido suscripciones para un cliente en una moneda diferente, verá una pestaña para cada moneda. Puede hacer algunas cosas desde esta página:

    - Para ver la factura y el archivo de conciliación más recientes, seleccione **Factura** o **Archivo de conciliación.** (Si lo desea, también puede acceder a la factura más reciente y volver a crear archivos de datos [mediante Centro de partners API](/partner-center/develop/).

    - Para ver las facturas anteriores y los archivos de conciliación, expanda la fila **Historial de facturación** a continuación.

    - Para comprobar el saldo estimado de la cuenta o la factura en cualquier momento en función de la actividad de la cuenta más reciente, seleccione un vínculo en el encabezado **Estimaciones.**  

    >[!NOTE]
    > Cuando publiquemos la factura el día 8 del mes, incluirá los impuestos y cualquier otro cargo y crédito aplicable. Esto significa que el importe final debido puede diferir de lo que se ve durante el período de facturación.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Más información sobre facturas y archivos de conciliación para productos de Marketplace comercial

En esta sección se ofrece más información sobre los archivos de conciliación y factura para las suscripciones SaaS del marketplace comercial adquiridas para los clientes de publicadores de ISV de terceros.

Al seleccionar  Compras periódicas y únicas en la opción Facturación en el menú Centro de partners, obtendrá acceso a facturas y archivos de conciliación por los cargos relacionados con las compras de Microsoft (de terceros) e ISV (terceros).  Estas compras pueden estar asociadas a:

- Suscripciones de SaaS (de publicadores de Microsoft o ISV)

- Plan de Azure

- Reservas de Azure

- Otro software basado en suscripciones (de Microsoft o publicadores de ISV)

Algunos ejemplos de estas compras pueden ser el software SUSE Linux (una suscripción de software) o una suscripción de producto SaaS de Azure ISV.

>[!NOTE]
> Para obtener más información sobre cómo leer los archivos de factura y conciliación, consulte también Información general [de facturación.](billing.md)

### <a name="tips-on-reading-your-invoice"></a>Sugerencias para leer la factura

Al comprar un producto SaaS basado en licencia de un publicador de ISV de terceros, solo verá cargos por el precio de licencia en la factura. Esto es así incluso cuando el producto SaaS del ISV usa (o consume) recursos de infraestructura de Azure subyacentes. Esto se debe a que los cargos de uso de la infraestructura de Azure del cliente para el producto SaaS de un ISV se facturan directamente al ISV. (Los ISV verán los cargos de consumo de Azure asociados en su propio archivo de conciliación de facturas de uso diario de Azure).

La factura contendrá varias páginas:

- **Página 1 de la factura:** Contiene información general de resumen de los detalles de facturación del asociado del programa CSP. Esto incluye un resumen de los cargos del período de facturación, un número de factura, los términos de pago (60 días netos) y los métodos de pago de facturación para pagar por transferencia o mediante comprobación.

- **Página 2 (y las páginas posteriores) de la factura:** Detalla los cargos por las compras de Microsoft de terceros y las compras de ISV de terceros (basadas en licencias) del marketplace comercial. Puede identificar las compras basadas en licencias de ISV por la línea **del** publicador debajo de cada nombre de producto. El archivo de conciliación asociado ofrece más detalles de facturación para cargos de factura específicos.

- **Página final de la factura:** Si se le han cobrado productos de Marketplace basados en licencias desde un ISV, en esta página final se mostrarán más detalles sobre el nombre y la dirección del publicador del ISV.

### <a name="tips-on-reading-your-reconciliation-file"></a>Sugerencias para leer el archivo de conciliación

El **archivo de conciliación de** compras periódicas y únicas contiene varias columnas con detalles adicionales que se asignan a los cargos de la factura. La **columna PublisherName** muestra si la compra es de Microsoft o de un publicador de ISV de terceros.

Algunos cargos en el archivo de conciliación pueden aparecer con un costo de 0 USD. Esto puede deberse a una oferta de "evaluación gratuita" de ISV (normalmente 30 o 60 días) o a una oferta de traiga su propia licencia.

En el caso de las ofertas de ISV de evaluación gratuita:

- El período de evaluación gratuita cubre el costo del producto SaaS basado en licencias del ISV durante ese tiempo. Tampoco se le cobrará por el uso asociado de la infraestructura de Azure de ese producto SaaS.  Sin embargo, si usa una oferta de ISV basada en el uso, la evaluación gratuita no incluye el costo del uso subyacente de la infraestructura de Azure. En este caso, los cargos de uso de la infraestructura de Azure aparecerán en un archivo de conciliación de Azure independiente.

- Al comprar e implementar el producto apto para evaluación gratuita de un ISV para el cliente, el publicador de ISV inscribirá automáticamente al cliente en la evaluación gratuita. El período de evaluación gratuita finaliza automáticamente después del período definido por el publicador de ISV. Una vez que finalice el período, se cobrará al cliente. Esto significa que el archivo de conciliación puede mostrar dos filas para un producto apto para evaluación: una que realiza un seguimiento del período de prueba y otra que realiza el seguimiento de la oferta de pago (que mostrará un costo de 0 USD hasta que finalice el período de prueba). Una vez que finalice la evaluación, la fila que muestra la oferta de pago comenzará a mostrar los cargos. 

Para obtener más información sobre lo que representa cada columna, vea [Usar los archivos de conciliación](use-the-reconciliation-files.md). Consulte también [Tipos de facturación en Centro de partners](./billing-basics.md)

## <a name="next-steps"></a>Pasos siguientes

- [Administración de productos de Marketplace comercial para clientes](csp-commercial-marketplace-manage.md)
- [Más información sobre el soporte técnico para productos de Marketplace comercial](csp-commercial-marketplace-support.md)