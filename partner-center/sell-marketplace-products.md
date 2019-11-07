---
title: Vender suscripciones a productos de Marketplace comercial | Centro de partners
ms.topic: article
ms.date: 08/16/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Puedes usar el Centro de partners para vender tus suscripciones de cliente para productos de software como servicio (SaaS) publicados en Marketplace comercial por fabricantes de software independientes (ISV).
author: JnHs
ms.author: jenhayes
keywords: subscriptions, Marketplace, third party, ISV
ms.localizationpriority: medium
ms.openlocfilehash: bf3ad75f4bac84163efb4a67009a5d4d7f2261d5
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/06/2019
ms.locfileid: "73651636"
---
# <a name="sell-subscriptions-to-commercial-marketplace-products"></a>Vender suscripciones a productos de Marketplace comercial

**Se aplica a**

- Centro de partners

Puedes usar el Centro de partners para vender tus suscripciones de cliente a productos de software como servicio (SaaS) publicados en Marketplace comercial ([Microsoft AppSource](https://appsource.microsoft.com/) y [Azure Marketplace](https://azuremarketplace.microsoft.com/)) por fabricantes de software independientes (ISV). De esta manera puedes diferenciar tu negocio y ofrecer a tus clientes paquetes de software que den respuesta a sus necesidades empresariales específicas. Puedes administrar las licencias y suscripciones de estos productos de SaaS de Marketplace de la misma forma que lo haces con otros productos de Microsoft.

Para más información sobre Marketplace comercial, consulta las [Preguntas más frecuentes de Marketplace](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide).

> [!IMPORTANT]
> En el Centro de partners, solo se pueden adquirir suscripciones de Marketplace comercial de software como servicio (SaaS). Otros tipos de ofertas de Marketplace comercial (como aplicaciones, contenedores o VM de Azure) se administran a través de Azure Portal y se facturan según el consumo. Se requiere una suscripción de Azure existente para habilitar las soluciones de pago por uso a través de Azure Portal.

## <a name="view-marketplace-offers-and-pricing"></a>Visualización de ofertas y precios de Marketplace

Para ver todas las ofertas de Marketplace comercial disponibles, selecciona **Marketplace** en el menú de navegación izquierdo. De forma predeterminada, verá los productos de todos los tipos y categorías. Puedes filtrar por tipo o categoría, o utilizar el cuadro de búsqueda para buscar palabras clave específicas. Selecciona un producto para ver información sobre el anunciante y las SKU disponibles, incluido si se ofrece o no un período de evaluación gratuita.

> [!NOTE]
> Es posible que algunos productos disponibles en Marketplace comercial no se muestren aquí. Los ISV pueden decidir si ofrecen sus productos a los partners del Proveedor de soluciones en la nube (CSP) en el Centro de partners. Si ve un producto en el Marketplace comercial que le gustaría ofrecer a sus clientes a través del centro de Partners, busque la información de contacto del anunciante en la lista de productos y hágales saber que le interesa.

Los precios de los productos de Marketplace comercial pueden cambiar con frecuencia. Para más información sobre los precios actuales de todos los productos de Marketplace comercial, selecciona **Exportar lista de precios** en la esquina superior derecha de la página de **Marketplace**. Se generará una hoja de cálculo con todos los datos de precios. Esta información sobre los precios se actualiza todos los días, así que puedes consultarla con frecuencia para conocer los precios actuales.

> [!TIP]
> Si un producto de esta lista ofrece una evaluación gratuita, la hoja de cálculo incluirá dos filas para ese producto. Una fila mostrará un precio de cero, lo que indica que hay disponible una evaluación gratuita. La otra fila incluirá el precio y las condiciones que se aplicarán una vez finalizado el período de prueba.
>
> Si un producto de esta lista usa el modelo de [facturación limitado](https://docs.microsoft.com/azure/marketplace/partner-center-portal/saas-metered-billing), el campo term estará en blanco.

## <a name="purchase-commercial-marketplace-products-for-your-customers"></a>Compra de productos de Marketplace comercial para tus clientes

La compra de suscripciones para productos de SaaS de Marketplace comercial sigue el mismo proceso que la compra de suscripciones para productos de Microsoft. Debes seleccionar un cliente o agregar un cliente nuevo antes de comprar una suscripción.

Al agregar una suscripción para un cliente, puedes elegir ver solo las ofertas de Marketplace de fabricantes de software independiente seleccionando **Partner** en el filtro **Editor**. Para más información, consulta [Crear una suscripción nueva](create-a-new-subscription.md).

Tenga en cuenta que algunas de las ofertas que ve en la página de **Marketplace** pueden no estar disponibles para un cliente específico. La disponibilidad puede verse afectada por una serie de factores, incluido si el ISV es compatible con el país o la región de facturación del cliente.

> [!TIP]
> También puedes usar las [API del Centro de partners](https://docs.microsoft.com/partner-center/develop/) para crear suscripciones de Marketplace comercial para los clientes. Para más información, consulta [Create a subscription for commercial marketplace products](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products) (Crear una suscripción para los productos de Marketplace comercial).

Con las suscripciones a los productos de Marketplace comercial, tienes la opción de [cancelar la suscripción](https://docs.microsoft.com/partner-center/create-a-new-subscription#cancel-a-subscription) dentro del período de cancelación (24 horas para las suscripciones mensuales o 14 días para las anuales). También puedes [elegir si deseas renovar la suscripción automáticamente o no](https://docs.microsoft.com/partner-center/create-a-new-subscription#choose-whether-to-automatically-renew-an-azure-marketplace-subscription).

## <a name="license-activation-for-commercial-marketplace-products"></a>Activación de licencias para productos de Marketplace comercial

Para los tipos de ofertas de software como servicio, la asignación y la activación de licencias se administra a través del fabricante de software independiente que publicó el producto. Para completar este proceso, debe visitar el sitio del publicador, mediante un vínculo personalizado con un código de autorización que permita al anunciante identificar su compra específica. Puedes encontrar este vínculo en la página de confirmación que aparece después de comprar una oferta de SaaS y en la página **Suscripciones** (en la fila de esa oferta). También puedes [usar las API del Centro de partners para recuperar este vínculo](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item).

Al visitar el sitio del editor mediante este vínculo, verá qué información o acción adicional es necesaria para aprovisionar y asignar licencias, o bien completar el proceso de instalación. Los pasos necesarios pueden variar en función del anunciante y de la oferta. Eres el responsable de enviar toda la información necesaria (o enviar la dirección URL al cliente para proporcionar directamente esta información). Una vez que se haya proporcionado la información necesaria, el anunciante aprovisionará y asignará las licencias adecuadas. La facturación de la suscripción solo comenzará después de que se hayan asignado correctamente las licencias.

## <a name="access-billing-info-for-commercial-marketplace-products"></a>Acceso a la información de facturación de los productos de Marketplace comercial

En el caso de los productos de Marketplace comercial, el período de facturación se inicia el primer día del mes natural y finaliza el último día del mes natural. Haremos que la factura esté disponible en el octavo día del mes siguiente. Puedes acceder a estas facturas en el Centro de partners o mediante las API de este.

Para más información, consulta [Descripción de los tipos de facturación del Centro de partners](https://docs.microsoft.com/partner-center/billing-different-types#billing-for-one-time-and-select-recurring-charges).

## <a name="provide-support-for-customers-using-commercial-marketplace-products"></a>Proporcionar soporte técnico a los clientes que usan productos de Marketplace comercial

Al igual que con otros productos de Microsoft, deberías ser el primer punto de contacto para el cliente si tiene alguna pregunta sobre la administración de suscripciones y de la facturación. Para obtener soporte técnico, deberás ponerte en contacto con el anunciante. Microsoft no proporciona soporte para productos comerciales de Marketplace, pero le proporcionará información de contacto de soporte técnico del editor.

Para más información, consulta [Compatibilidad con productos de Marketplace comercial](https://docs.microsoft.com/partner-center/report-problems-on-behalf-of-a-customer#support-for-commercial-marketplace-products) y [Proporcionar soporte técnico a tus clientes](https://docs.microsoft.com/partner-center/customer-support).

## <a name="manage-subscriptions-using-partner-center-apis"></a>Administración de suscripciones mediante las API del Centro de partners

Para crear una suscripción para productos de Marketplace comercial, usa las API del Centro de partners. Para ello, primero debes obtener una lista de ofertas para un mercado y, a continuación, crear y enviar un pedido para una suscripción de Marketplace comercial específica. Por último, se recupera un vínculo de activación para la suscripción.

También puedes usar las API del Centro de partners para realizar la administración del ciclo de vida y de las facturas de estas suscripciones.

Para más información, consulta [Create a subscription for commercial marketplace products](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products) (Crear una suscripción para los productos de Marketplace comercial).