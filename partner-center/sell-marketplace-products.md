---
title: Vender suscripciones a productos de Azure Marketplace | Centro de partners
ms.topic: article
ms.date: 04/04/2019
description: Puede usar el centro de partners a vender a sus clientes las suscripciones a Software como servicio (SaaS) productos publican en Azure Marketplace por fabricantes de Software independientes (ISV).
author: JnHs
ms.author: jenhayes
keywords: las suscripciones, Marketplace, tercero, ISV
ms.localizationpriority: medium
ms.openlocfilehash: a086ab3a58e926d33c118690e7b171ba4f0fd18b
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133835"
---
# <a name="sell-subscriptions-to-azure-marketplace-products"></a>Vender suscripciones a productos de Azure Marketplace

**Se aplica a**

- Centro de partners

Puede usar el centro de partners a vender a sus clientes las suscripciones a Software como los productos de servicio (SaaS) publican en [Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace) por fabricantes de Software independientes (ISV). Esto puede ayudar a diferenciar su negocio y proporcionar a sus clientes con paquetes de software que abordar sus necesidades empresariales específicas. Administrar suscripciones para estos productos SaaS de Azure Marketplace y licencias tal como se hace para productos de Microsoft.

Para obtener más información sobre Azure Marketplace, consulte [preguntas más frecuentes de Azure Marketplace](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide).

## <a name="view-marketplace-offers-and-pricing"></a>Precios y ofertas de Marketplace de vista

Para ver todas las ofertas disponibles, seleccione **Marketplace** desde el menú de navegación izquierdo. De forma predeterminada, verá los productos de todos los tipos y categorías. Puede filtrar por categoría o de tipo, o utilice el cuadro de búsqueda para buscar palabras clave específicas. Seleccione un producto para ver información sobre el publicador y las SKU disponibles.

> [!NOTE]
> Algunos productos que están disponibles en Azure Marketplace no se muestren aquí. Los ISV pueden decidir si desea ofrecer sus productos a los asociados de proveedor de soluciones en la nube (CSP) en el centro de partners o no. Si ve un producto en Azure Marketplace que le gustaría para ofrecer a sus clientes a través del centro de partners, buscar información de contacto del publicador en Azure Marketplace y hágales saber que está interesado.

Precios de productos de Azure Marketplace pueden cambiar con frecuencia. Para obtener información de precios actual para todos los productos de Marketplace, seleccione **lista de precios de exportación** en la esquina superior derecha de la **Marketplace** página. Esto generará una hoja de cálculo con todos los datos de precios. Información sobre los precios se actualiza cada día, por lo que puede comprobar tan a menudo como desee obtener los precios actuales.

## <a name="purchase-marketplace-products-for-your-customers"></a>Comprar productos de Marketplace para sus clientes

Adquisición de suscripciones a productos SaaS de Azure Marketplace sigue el mismo proceso que la adquisición de suscripciones a productos de Microsoft. Al agregar una suscripción para un cliente, puede elegir ver solo Marketplace ofrece de ISV seleccionando **asociado** en el **Publisher** filtro. Para obtener más información, consulte [crear una nueva suscripción](create-a-new-subscription.md).

> [!IMPORTANT]
> Sólo puede adquirir un Software como una suscripción de producto de servicio (SaaS) en el centro de partners. Otros tipos de oferta (por ejemplo, las aplicaciones de Azure, contenedores o máquinas virtuales) se administra a través del portal de Azure y factura según el consumo. Se requiere una suscripción de Azure existente con el fin de habilitar las soluciones de pago por uso a través del portal de Azure.

Tenga en cuenta que algunos ofrece que ve en el **Marketplace** página puede no estar disponible para un cliente específico. Disponibilidad puede verse afectada por una serie de factores, incluido si el ISV es compatible con país o región de facturación del cliente.

> [!TIP]
> También puede usar [Partner Center API](https://docs.microsoft.com/partner-center/develop/) para crear suscripciones de Azure Marketplace para sus clientes. Para obtener más información, consulte [crear una suscripción para productos de Azure Marketplace](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

Con las suscripciones a productos de Azure Marketplace, tiene la opción de [cancelar la suscripción](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription) dentro del período de cancelación (24 horas para las suscripciones mensuales o 14 días para las suscripciones anuales). También puede [elegir automáticamente renovar la suscripción o no](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription).

## <a name="access-billing-info-for-marketplace-products"></a>Obtener acceso a información de facturación para los productos de Marketplace

Para los productos de Marketplace, el período de facturación se inicia el primer día del mes del calendario y termina en el último día del mes del calendario. Haremos la factura disponible 8 días del mes siguiente. Puede tener acceso a estas facturas en el centro de partners, o mediante el uso de API del centro de partners.

Para obtener más información, consulte [descripción de los tipos de facturación en el centro de partners](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges).

## <a name="provide-support-for-customers-using-marketplace-products"></a>Proporcionar soporte técnico para los clientes que usan productos de Marketplace

Al igual que con productos de Microsoft, debe ser el primer punto de contacto para el cliente para preguntas sobre la administración de suscripciones y facturación. Para obtener soporte técnico, deberá ponerse en contacto con el publicador. Microsoft no proporciona soporte técnico para productos de Marketplace, pero le proporcionará información de contacto de soporte técnico del publicador.

Para obtener más información, consulte [soporte técnico para productos de Azure Marketplace](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-azure-marketplace-products) y [proporcionar soporte técnico a sus clientes](https://docs.microsoft.com/partner-center/customer-support).

## <a name="manage-subscriptions-using-partner-center-apis"></a>Administrar suscripciones con la API del centro de partners

Puede crear una suscripción para productos de Azure Marketplace mediante la API del centro de partners por obtener una lista de ofertas para un mercado, crear y enviar un pedido para obtener una suscripción de Azure Marketplace, y recuperar un vínculo de activación. También puede usar Partner Center API para realizar la administración del ciclo de vida y administrar las facturas de estas suscripciones.

Para obtener más información, consulte [crear una suscripción para productos de Azure Marketplace](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).