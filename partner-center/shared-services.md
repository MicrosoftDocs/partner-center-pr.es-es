---
title: Agregar Servicios compartidos para asociados de Azure
description: Use los servicios compartidos de asociados de Azure para comprar suscripciones de Azure para su propio uso y para tener un método uniforme de compra, seguimiento y administración de Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 49b5bd1c9a7cd4c56f2fac28a45cc8a4b922b9b0
ms.sourcegitcommit: 2d11dbdcc2b1e64ad16d29182824984517470a63
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/24/2020
ms.locfileid: "92333764"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Agregue los servicios compartidos de asociados de Azure para que los asociados puedan comprar suscripciones de Azure para su propio uso.

**Se aplica a**

- Centro de partners
 
**Roles adecuados**

- Administrador global
- Agente de administrador
- Agente de ventas

Los Servicios compartidos para partners de Azure son un nuevo tipo de oferta para partners en el programa CSP que les permite comprar suscripciones de Azure para el uso propio.Crea la oportunidad de que los asociados usen un método uniforme para comprar, realizar el seguimiento y administrar Azure, además de la capacidad de consolidar sus contratos de licencia y reventa de Azure con Microsoft. Con los servicios compartidos de asociados de Azure, ahora los asociados tienen la misma flexibilidad para usar las suscripciones de Azure en CSP que en los programas de Microsoft Contrato Enterprise y Web Direct, lo que abre escenarios como compilar entornos de desarrollo y pruebas, implementar cargas de trabajo internas y hospedar servicios compartidos o aplicaciones de varios inquilinos.  

## <a name="create-the-shared-services-tenant"></a>Crear el inquilino de servicios compartidos

1. Vaya a **configuración**configuración de la  >  **cuenta**  >  **servicios compartidos**.

   :::image type="content" source="images/sharedservices2.png" alt-text="Configuración de la cuenta > servicios compartidos":::

2. Si aún no tiene un inquilino de servicios compartidos, haga clic en **crear servicios compartidos**.

   :::image type="content" source="images/sharedservices3.png" alt-text="Configuración de la cuenta > servicios compartidos":::

3. Esto crea un inquilino de servicios compartidos y compra la suscripción de servicios compartidos de CSP de Azure, que se usará para los recursos compartidos y la carga de trabajo interna.

   :::image type="content" source="images/sharedservices5.png" alt-text="Configuración de la cuenta > servicios compartidos":::

## <a name="about-the-azure--internalshared-services-offer"></a>Acerca de la oferta de Azure-Carga de trabajo interna/servicios compartidos

- El Azure-Carga de trabajo interna/servicios compartidos suscripción es un nuevo tipo de oferta de Azure en CSP al que se tiene acceso a través del centro de partners que los asociados obtienen para su propio uso de Azure.

- Azure-Carga de trabajo interna/servicios compartidos oferta no es válida para descuentos e incentivos.

- La oferta de Azure-Carga de trabajo interna/servicios compartidos solo se puede aplicar al inquilino de servicios compartidos.

- El uso principal de la suscripción Azure-Carga de trabajo interna/servicios compartidos es para que pueda usar Azure para sus propios propósitos de desarrollo. El inquilino compartido que se usa para aprovisionar esta oferta no se puede usar para otros servicios como licencias de Office 365 o Dynamics.

- Puede cancelar la suscripción como cualquier otra suscripción. Vaya a la **configuración**  >  **vista todos los**  >  **servicios compartidos**. Seleccione el Azure-Carga de trabajo interna/servicios compartidos suscripción y cancélelo.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Obtener acceso a los detalles de consumo de servicios compartidos de Azure Partner

Encontrará el consumo de Azure en la factura de CSP y en el archivo de conciliación. Se incluirá como parte de Microsoft Azure elemento de línea de la factura. La información detallada sobre el consumo estará disponible en el archivo de conciliación registrado en el inquilino que se creó para esta oferta.

## <a name="azure-partner-shared-services-pricing"></a>Precios de los servicios compartidos de asociados de Azure

Para ver el nuevo archivo de precios de los servicios compartidos de asociados de Azure, vaya a **vender**  >  **precios y ofertas** y seleccione la lista de precios del mes actual. En las próximas semanas, también se publicará una API de tarjeta de tarifas específica.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Ofertas de Marketplace y servicios compartidos de asociados de Azure

A partir del 1 de marzo de 2019, los servicios compartidos de asociados de Azure (APSS) ya no admiten ofertas de Marketplace.

|**Soporte técnico de Marketplace**   |**APSS admitido antes del 1 de marzo de 2019**|**Después del 1 de marzo de 2019**|
|---------------------------|:----------------------------|:-------------------|
|Traiga su propia licencia (BYOL) y servicios gratuitos   | Sí   | No|
|Otras ofertas de Marketplace de terceros   | No   |No|

Los asociados que tienen servicios BYOL o gratis implementados con APSS no se verán afectados; sin embargo, después del 1 de marzo de 2019, no podrán adquirir nuevos servicios de BYOL o gratis.

Para aprovechar el catálogo completo de ofertas de Marketplace disponibles (no solo BYOL y servicios gratuitos), recomendamos que los asociados de CSP implementen servicios compartidos con suscripciones de Azure directas de Web.  Los asociados de CSP que han implementado BYOL de terceros y recursos de servicio gratis desde Marketplace previamente y desean seguir utilizándolos e implementar más ofertas de terceros se recomiendan para migrar la suscripción de APSS a web Direct y [migrar las suscripciones de Azure existentes](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).

Los asociados, que planean seguir usando la suscripción a APSS después del 1 de marzo de 2019 y desean implementar nuevos [servicios de BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) de terceros o servicios gratuitos, pueden seguir las instrucciones de los ISV para implementarlos en sus suscripciones de APSS.