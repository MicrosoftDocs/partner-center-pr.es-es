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
ms.openlocfilehash: 40ba485cecce394dc81632d01f8774859690c522
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551612"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Agregue Servicios compartidos para asociados de Azure para que los asociados puedan comprar suscripciones de Azure para su propio uso

**Roles adecuados:** Administrador global | Agente de administración | Agente de ventas

Servicios compartidos para asociados de Azure (APSS) es un nuevo tipo de oferta para los asociados del programa Proveedor de soluciones en la nube (CSP), lo que permite a los asociados adquirir suscripciones de Azure para su propio uso.Crea la oportunidad de que los asociados usen un método uniforme para comprar, realizar un seguimiento y administrar Azure, además de la capacidad de consolidar sus contratos de licencias y reventa de Azure con Microsoft. Con APSS, los asociados ahora tienen la misma flexibilidad para usar suscripciones de Azure en CSP que en los programas Microsoft Contrato Enterprise y Web Direct, lo que abre escenarios como: crear entornos de desarrollo y pruebas, implementar cargas de trabajo internas y hospedar servicios compartidos o aplicaciones multiinquilino.  

## <a name="create-the-shared-services-tenant"></a>Creación del inquilino de servicios compartidos

1. Vaya a **Configuración Configuración** Configuración de  >  **la cuenta** Servicios  >  **compartidos.**

   :::image type="content" source="images/sharedservices2.png" alt-text="Configuración de la > servicios compartidos":::

2. Si aún no tiene un inquilino de servicios compartidos, seleccione **Crear servicios compartidos.**

   :::image type="content" source="images/sharedservices3.png" alt-text="Cree servicios compartidos.":::

3. Esto crea un inquilino de servicios compartidos y adquiere la CSP de Azure de Servicios compartidos, que se usará para los recursos compartidos y la carga de trabajo interna.

   :::image type="content" source="images/sharedservices5.png" alt-text="Cree el inquilino y compre la suscripción.":::

## <a name="about-the-azure--internalshared-services-offer"></a>Acerca de la Azure - Carga de trabajo interna/servicios compartidos de datos

- La Azure - Carga de trabajo interna/servicios compartidos es un nuevo tipo de oferta de Azure en CSP al que se accede Centro de partners que los asociados obtienen para su propio uso de Azure.

- Servicios compartidos para asociados de Azure suscripciones son aptas y se pueden usar para comprar LAS.

- La Azure - Carga de trabajo interna/servicios compartidos oferta solo se puede aplicar al inquilino de servicios compartidos.

- El uso principal de la Azure - Carga de trabajo interna/servicios compartidos suscripción es para que pueda usar Azure con fines de desarrollo propios. El inquilino compartido que usa para aprovisionar esta oferta no se puede usar para otros servicios como Office 365 o licencias de Dynamics.

- Puede cancelar la suscripción como cualquier otra suscripción. Vaya a la **configuración de Ver todo**  >  **servicios**  >  **compartidos.** Seleccione la Azure - Carga de trabajo interna/servicios compartidos suscripción y cancele.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Acceso a Servicios compartidos para asociados de Azure de consumo

Encontrará el consumo de Azure en la factura de CSP y el archivo de conciliación. Se incluirá como parte de Microsoft Azure línea en la factura. La información de consumo detallada estará disponible en el archivo de conciliación registrado en el inquilino que se creó para esta oferta.

## <a name="azure-partner-shared-services-pricing"></a>Servicios compartidos para asociados de Azure precios

Para ver el nuevo archivo de precios de APSS, vaya a **Precios** de venta y ofertas y seleccione la lista de precios del mes  >   actual. En las próximas semanas, también se lanzará una API de tarjeta de tarifa específica.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Ofertas y ofertas de Marketplace Servicios compartidos para asociados de Azure

A partir del 1 de marzo de 2019, APSS ya no admite ofertas de Marketplace.

|**Soporte técnico de Marketplace**   |**APSS compatible antes del 1 de marzo de 2019**|**Después del 1 de marzo de 2019**|
|---------------------------|:----------------------------|:-------------------|
|Traiga su propia licencia (BYOL) y servicios gratuitos   | Sí   | No|
|Otras ofertas de Marketplace de terceros   | No   |No|

Los asociados que tengan BYOL o servicios gratuitos implementados mediante APSS no se verán afectados; sin embargo, después del 1 de marzo de 2019 no podrán comprar nuevos byol ni servicios gratuitos.

Para aprovechar el catálogo completo de ofertas de Marketplace disponibles (no solo byol y servicios gratuitos), se recomienda que los asociados de CSP implementen servicios compartidos mediante suscripciones web directas de Azure.  Se recomienda a los asociados de CSP que han implementado byol de terceros y recursos de servicio gratuitos de Marketplace anteriormente y que desean seguir usándolos e implementar más ofertas de terceros para migrar la suscripción de APSS a web directa migrando suscripciones de [Azure](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)existentes.

Los asociados, que tienen previsto seguir usando la suscripción de APSS después del 1 de marzo de 2019 y desean implementar nuevos servicios [BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) de terceros o servicios gratuitos, pueden seguir las instrucciones de los ISV para implementarlos en sus suscripciones de APSS.

## <a name="next-steps"></a>Pasos siguientes

- [Venta de suscripciones de software a través de CSP](csp-software-subscriptions.md)