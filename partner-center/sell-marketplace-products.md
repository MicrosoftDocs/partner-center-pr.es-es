---
title: Vender suscripciones a productos de Azure Marketplace | Centro de Partners
ms.topic: article
ms.date: 07/12/2019
description: Puede usar el centro de partners para vender sus suscripciones de clientes a productos de software como servicio (SaaS) publicados en Azure Marketplace por fabricantes de software independientes (ISV).
author: JnHs
ms.author: jenhayes
keywords: suscripciones, Marketplace, terceros, ISV
ms.localizationpriority: medium
ms.openlocfilehash: 4dda776e7ebdece3a8a15c3576b64d93d3e4158c
ms.sourcegitcommit: dd961f85bc790e56c70479a5926177454dd8e855
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/12/2019
ms.locfileid: "67854504"
---
# <a name="sell-subscriptions-to-azure-marketplace-products"></a>Vender suscripciones a productos de Azure Marketplace

**Se aplica a**

- Centro de partners

Puede usar el centro de partners para vender sus suscripciones de clientes a productos de software como servicio (SaaS) publicados en [Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace) por fabricantes de software independientes (ISV). Esto puede ayudar a diferenciar su negocio y proporcionar a los clientes paquetes de software que satisfagan sus necesidades empresariales específicas. Puede administrar licencias y suscripciones para estos productos de SaaS de Azure Marketplace de la misma forma que lo hace para los productos de Microsoft.

Para obtener más información sobre Azure Marketplace, consulte [preguntas más frecuentes sobre Azure Marketplace](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide).

## <a name="view-marketplace-offers-and-pricing"></a>Visualización de ofertas y precios de Marketplace

Para ver todas las ofertas disponibles, seleccione **Marketplace** en el menú de navegación izquierdo. De forma predeterminada, verá los productos de todos los tipos y categorías. Puede filtrar por tipo o categoría, o utilizar el cuadro Buscar para buscar palabras clave específicas. Seleccione un producto para ver información sobre el publicador y las SKU disponibles, incluido si se ofrece o no un período de evaluación gratuita.

> [!NOTE]
> Es posible que algunos productos que están disponibles en Azure Marketplace no se muestren aquí. Los ISV pueden decidir si ofrecen o no sus productos a los asociados del proveedor de soluciones en la nube (CSP) en el centro de Partners. Si ve un producto en Azure Marketplace que le gustaría ofrecer a sus clientes a través del centro de Partners, busque la información de contacto del anunciante en Azure Marketplace y háganoslo saber que está interesado.

Los precios de los productos de Azure Marketplace pueden cambiar con frecuencia. Para obtener información sobre los precios actuales de todos los productos de Marketplace, seleccione **Exportar lista de precios** en la esquina superior derecha de la página de **Marketplace** . Se generará una hoja de cálculo con todos los datos de precios. La información de precios se actualiza todos los días, por lo que puede comprobarla con la frecuencia que desee para obtener los precios actuales.

> [!TIP]
> Si un producto de esta lista ofrece una evaluación gratuita, la hoja de cálculo incluirá dos filas para ese producto. Una fila mostrará un precio de cero, lo que indica que hay disponible una evaluación gratuita. La otra fila incluirá el precio y el término que se aplicarán una vez finalizado el período de prueba.

## <a name="purchase-marketplace-products-for-your-customers"></a>Comprar productos de Marketplace para sus clientes

La compra de suscripciones para productos de SaaS de Azure Marketplace sigue el mismo proceso que la compra de suscripciones para productos de Microsoft. Al agregar una suscripción para un cliente, puede elegir ver solo las ofertas de Marketplace de ISV seleccionando **Partner** en el  filtro del publicador. Para obtener más información, consulte [crear una nueva suscripción](create-a-new-subscription.md).

> [!IMPORTANT]
> Solo puede comprar suscripciones de producto de software como servicio (SaaS) en el centro de Partners. Otros tipos de ofertas (como las aplicaciones, los contenedores o las máquinas virtuales de Azure) se administran a través del Azure Portal y se facturan según el consumo. Se requiere una suscripción de Azure existente para habilitar las soluciones de pago por uso a través de la Azure Portal.

Tenga en cuenta que algunas de las ofertas que ve en la página de **Marketplace** pueden no estar disponibles para un cliente específico. La disponibilidad puede verse afectada por una serie de factores, incluido si el ISV es compatible con el país o la región de facturación del cliente.

> [!TIP]
> También puede usar las [API del centro de Partners](https://docs.microsoft.com/partner-center/develop/) para crear suscripciones de Azure Marketplace para sus clientes. Para obtener más información, consulte [creación de una suscripción para productos de Azure Marketplace](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

Con las suscripciones a los productos de Azure Marketplace, tiene la opción de [cancelar la suscripción](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription) dentro del período de cancelación (24 horas para las suscripciones mensuales o 14 días para las suscripciones anuales). También puede [elegir si desea renovar la suscripción automáticamente](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription).

## <a name="license-activation-for-marketplace-products"></a>Activación de licencias para productos de Marketplace

En el caso de los tipos de oferta de software como servicio (SaaS), la asignación y la activación de licencias se administra a través del fabricante de software independiente (ISV) que publicó el producto. Para completar este proceso, debe visitar el sitio del publicador, mediante un vínculo personalizado con un código de autorización que permita al anunciante identificar su compra específica. Puede encontrar este vínculo en la página de confirmación que aparece después de comprar una oferta de SaaS y en  la página suscripciones (en la fila de esa oferta). También puede [usar las API del centro de partners para recuperar este vínculo](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item).

Al visitar el sitio del editor mediante este vínculo, verá qué información o acción adicional es necesaria para aprovisionar y asignar licencias, o bien completar el proceso de instalación. Los pasos necesarios pueden variar en función del publicador y la oferta. Usted es responsable de enviar la información necesaria (o enviar la dirección URL a su cliente para proporcionar directamente esta información). Una vez que se haya proporcionado la información necesaria, el publicador aprovisionará y asignará las licencias adecuadas. La facturación de la suscripción solo comenzará después de que se hayan asignado correctamente las licencias.

## <a name="access-billing-info-for-marketplace-products"></a>Acceder a la información de facturación de los productos de Marketplace

En el caso de los productos de Marketplace, el período de facturación se inicia el primer día del mes natural y finaliza el último día del mes natural. Haremos que la factura esté disponible en el octavo día del mes siguiente. Puede tener acceso a estas facturas en el centro de Partners o mediante las API del centro de Partners.

Para obtener más información, consulte [Descripción de los tipos de facturación en el centro de Partners](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges).

## <a name="provide-support-for-customers-using-marketplace-products"></a>Proporcionar soporte técnico a los clientes que usan productos de Marketplace

Al igual que con los productos de Microsoft, debe ser el primer punto de contacto para su cliente con preguntas sobre la administración de suscripciones y facturación. Para obtener soporte técnico, deberá ponerse en contacto con el publicador. Microsoft no proporciona soporte para los productos de Marketplace, pero le proporcionará información de contacto de soporte técnico del editor.

Para obtener más información, consulte [compatibilidad con productos de Azure Marketplace](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-azure-marketplace-products) y [proporcionar soporte técnico a los clientes](https://docs.microsoft.com/partner-center/customer-support).

## <a name="manage-subscriptions-using-partner-center-apis"></a>Administrar suscripciones mediante API del centro de Partners

Puede crear una suscripción para los productos de Azure Marketplace mediante las API del centro de partners mediante la obtención de una lista de ofertas para un mercado, la creación y el envío de un pedido de una suscripción de Azure Marketplace y la recuperación de un vínculo de activación. También puede usar las API del centro de partners para realizar la administración del ciclo de vida y administrar las facturas para estas suscripciones.

Para obtener más información, consulte [creación de una suscripción para productos de Azure Marketplace](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).