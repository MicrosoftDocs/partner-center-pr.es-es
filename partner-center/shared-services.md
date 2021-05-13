---
title: Agregar Servicios compartidos para asociados de Azure
description: Use Servicios compartidos para asociados de Azure para comprar suscripciones de Azure para su propio uso y para tener un método uniforme para comprar, realizar un seguimiento y administrar Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 929907c7c6f238fb84a13622227534797f0ac949
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855342"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Agregue Servicios compartidos para asociados de Azure para que los asociados puedan comprar suscripciones de Azure para su propio uso

**Roles adecuados:** Administrador global | Agente de administración | Agente de ventas

Los Servicios compartidos para partners de Azure son un nuevo tipo de oferta para partners en el programa CSP que les permite comprar suscripciones de Azure para el uso propio.Crea la oportunidad de que los asociados usen un método uniforme para comprar, realizar el seguimiento y administrar Azure, además de la capacidad de consolidar sus contratos de licencias y reventa de Azure con Microsoft. Con Servicios compartidos para asociados de Azure, los asociados ahora tienen la misma flexibilidad para usar suscripciones de Azure en CSP que en los programas Microsoft Contrato Enterprise y Web Direct, lo que abre escenarios como: crear entornos de desarrollo y pruebas, implementar cargas de trabajo internas y hospedar servicios compartidos o aplicaciones multiinquilino.  

## <a name="create-the-shared-services-tenant"></a>Creación del inquilino de servicios compartidos

1. Vaya a **Configuración Configuración** Configuración de  >  **la cuenta** Servicios  >  **compartidos.**

   :::image type="content" source="images/sharedservices2.png" alt-text="Configuración de la > servicios compartidos":::

2. Si aún no tiene un inquilino de servicios compartidos, haga clic **en Crear servicios compartidos.**

   :::image type="content" source="images/sharedservices3.png" alt-text="Creación de servicios compartidos":::

3. Esto crea un inquilino de servicios compartidos y adquiere la CSP de Azure de Servicios compartidos, que se usará para los recursos compartidos y la carga de trabajo interna.

   :::image type="content" source="images/sharedservices5.png" alt-text="Creación del inquilino y compra de la suscripción":::

## <a name="about-the-azure--internalshared-services-offer"></a>Acerca de la Azure - Carga de trabajo interna/servicios compartidos de datos

- La Azure - Carga de trabajo interna/servicios compartidos es un nuevo tipo de oferta de Azure en CSP al que se accede a través Centro de partners que los asociados obtienen para su propio uso de Azure.

- Servicios compartidos para asociados de Azure suscripciones son aptas y se pueden usar para comprar LAS.

- La Azure - Carga de trabajo interna/servicios compartidos oferta solo se puede aplicar al inquilino de servicios compartidos.

- El uso principal de la Azure - Carga de trabajo interna/servicios compartidos suscripción es para que pueda usar Azure con fines de desarrollo propios. El inquilino compartido que usa para aprovisionar esta oferta no se puede usar para otros servicios como Office 365 o licencias de Dynamics.

- Puede cancelar la suscripción como cualquier otra suscripción. Vaya a la **configuración Ver todo**  >  **configuración Servicios**  >  **compartidos**. Seleccione la Azure - Carga de trabajo interna/servicios compartidos suscripción y cancele la suscripción.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Acceso a Servicios compartidos para asociados de Azure detalles de consumo

Encontrará el consumo de Azure en la factura de CSP y el archivo de conciliación. Se incluirá como parte de Microsoft Azure línea en la factura. La información de consumo detallada estará disponible en el archivo de conciliación registrado en el inquilino que se creó para esta oferta.

## <a name="azure-partner-shared-services-pricing"></a>Servicios compartidos para asociados de Azure precios

Para ver el nuevo archivo de precios de Servicios compartidos para asociados de Azure, vaya a **Precios** y ofertas de venta y seleccione la lista de precios  >   del mes actual. En las próximas semanas, también se lanzará una API de tarjeta de tarifa específica.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Ofertas y ofertas de Marketplace Servicios compartidos para asociados de Azure

A partir del 1 de marzo de 2019, Servicios compartidos para asociados de Azure (APSS) ya no admite ofertas de Marketplace.

|**Soporte técnico de Marketplace**   |**APSS compatible antes del 1 de marzo de 2019**|**Después del 1 de marzo de 2019**|
|---------------------------|:----------------------------|:-------------------|
|Traiga su propia licencia (BYOL) y servicios gratuitos   | Sí   | No|
|Otras ofertas de Marketplace de terceros   | No   |No|

Los asociados que tengan BYOL o servicios gratuitos implementados mediante APSS no se verán afectados; sin embargo, después del 1 de marzo de 2019 no podrán adquirir nuevos servicios BYOL ni gratuitos.

Para aprovechar el catálogo completo de ofertas de Marketplace disponibles (no solo byol y servicios gratuitos), se recomienda que los asociados de CSP implementen servicios compartidos mediante suscripciones de Azure directas web.  Se recomienda a los asociados de CSP que han implementado byol de terceros y recursos de servicio gratuitos de Marketplace anteriormente y que desean seguir usándolos e implementar más ofertas de terceros para migrar la suscripción de APSS a web direct [Migrating Existing Azure Subscriptions](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)(Migración directa de suscripciones de Azure existentes).

Los asociados, que tienen previsto seguir usando la suscripción de APSS después del 1 de marzo de 2019 y desean implementar nuevos servicios [BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) de terceros o servicios gratuitos, pueden seguir las instrucciones de los ISV para implementarlos en sus suscripciones de APSS.

## <a name="next-steps"></a>Pasos siguientes

- [Venta de suscripciones de software a través de CSP](csp-software-subscriptions.md)