---
title: Ofrecer a los clientes pruebas de productos de Microsoft
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Permitir que los clientes prueben productos de suscripción de Microsoft durante 30 días. Regístrese para obtener estas pruebas gratuitas en el catálogo como muchas otras servicios en línea.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d6fda82464b9abc30714798a2ee3999d8f93db5
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151141"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Proporcionar a los clientes pruebas gratuitas de 30 días de productos de Microsoft

**Roles adecuados:** Administrador global | Administrador de administración de | Agente de ventas

Una buena manera de presentar a los clientes a los nuevos productos de Microsoft es ofrecer pruebas gratuitas de 30 días. Puede registrarse para obtener las pruebas del catálogo como muchas otras servicios en línea. Todos los partners pueden participar.

## <a name="available-trial-offers"></a>Ofertas de prueba disponibles

Puede encontrar todas las ofertas de evaluación pendientes en la **página** Cliente. En esta página se enumeran todas las suscripciones, incluidas las pruebas gratuitas y las suscripciones de pago. (Esta característica no está disponible actualmente en China).

Cada cliente tiene derecho a una evaluación gratuita para cada oferta disponible. Por ejemplo, pueden obtener una evaluación gratuita para Microsoft 365 Business Standard y una evaluación gratuita para Office 365 E3. Sin embargo, si el cliente ya posee la oferta, no puede usar una evaluación gratuita para esa oferta.

### <a name="available-products"></a>Productos disponibles

Hay pruebas gratuitas disponibles para las ofertas más completas y populares basadas en licesen. Las nuevas ofertas de prueba se pueden presentar mensualmente.

Los asociados pueden encontrar pruebas en la lista de precios mensuales en la **página precios y** ofertas de Centro de partners. Las ofertas de prueba tendrán "PRUEBA" en la columna Tipo **de licencia secundaria** de la lista de precios.

Actualmente, **no hay pruebas gratuitas para** las ofertas gubernamentales, las ofertas educativas ni las ofertas de complementos.

## <a name="licenses-for-free-trial-offers"></a>Licencias para ofertas de evaluación gratuita

Todas las pruebas gratuitas proporcionan 25 licencias. No se puede cambiar este número durante la evaluación. No se pueden agregar ni quitar licencias en la evaluación gratuita. Después de convertir la versión de prueba en una suscripción de pago, puede agregar más licencias a la suscripción.

Las licencias de prueba deben asignarse a los usuarios de la misma manera que se asignan las licencias de servicios de pago.

## <a name="sign-customers-up-for-trials"></a>Registro de clientes para obtener pruebas

Obtenga una prueba para el cliente en Centro de partners:

1. En **Sell** (Vender) Centro de partners, vaya a **Catalog (Catálogo).** 
2. En el catálogo, en **Frecuencia de facturación,** seleccione **Oferta de prueba.** Esto permite que solo aparezcan las pruebas gratuitas y deshabilita otras ofertas que no son gratuitas. Las pruebas se mostrarán en la **pestaña Trials (Pruebas)** del catálogo.
3. Seleccione la evaluación gratuita que desea ofrecer y, a continuación, **seleccione Enviar**. Todas las pruebas son durante 30 días durante los cuales no se le facturará. También puede convertirlo en una suscripción de pago en cualquier momento durante la evaluación.

## <a name="converting-trials-to-paid-subscriptions"></a>Conversión de pruebas en suscripciones de pago

Una evaluación gratuita no se convierte automáticamente en una suscripción de pago. Después de 30 días, se debe convertir una evaluación gratuita en una suscripción de pago o [expirará](#expiring-offers). No se pueden ampliar las pruebas gratuitas.

Tendrá que convertir la versión de prueba en una suscripción de pago usted mismo. Puede hacerlo mediante [el Centro de partners](#convert-trials-using-partner-center) o a través de [Centro de partners API](#convert-trials-using-apis).

> [!NOTE]
> Las pruebas gratuitas del cliente Proveedor de soluciones en la nube programa de Proveedor de soluciones en la nube (CSP) no se pueden convertir a otro inquilino del programa (como EA, Open o MOSP).

### <a name="convert-trials-using-partner-center"></a>Conversión de pruebas mediante Centro de partners

Puede convertir las pruebas en suscripciones de pago Centro de partners:

1. Vaya a la página de suscripción del cliente y seleccione la evaluación gratuita.
2. Seleccione **Convertir la versión de prueba en una suscripción de pago.**
3. Escriba la cantidad de licencias deseada y la frecuencia de facturación y seleccione **Aplicar.**
4. La facturación de la suscripción de pago comienza en la fecha de conversión y la suscripción se renueva automáticamente 12 meses a partir de la fecha de conversión. 

### <a name="convert-trials-using-apis"></a>Conversión de pruebas mediante API

Es posible que tenga que modificar las API para adaptarse a la conversión de una evaluación gratuita en una suscripción de pago. Para más información, consulte la siguiente documentación para desarrolladores:

- [Convertir una suscripción de prueba en otra de pago](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Obtener una lista de ofertas de conversión de versiones de prueba](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Pruebas sin conversiones

No todas las pruebas se pueden convertir en suscripciones de pago. Los asociados pueden usar una prueba que no tenga conversiones hasta la fecha de expiración. Los partners pueden comprar ofertas compatibles que admitan los mismos servicios que la oferta de prueba.  Esto debe hacerse antes de que expire la versión de prueba para asegurarse de que los servicios de las ofertas recién adquiridas se alinean con los servicios de la prueba. 

|**Versión de prueba**   |**Ofertas compatibles para pequeñas empresas**   |**Ofertas empresariales compatibles**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Prueba de la nube comercial de Microsoft Teams (iniciada por el usuario)   |Microsoft 365 Business Basic, Microsoft 365 Business Standard, Microsoft 365 Business Premium   | F3 (anteriormente F1), Office 365 for Enterprise (E1, E3 y E5), Microsoft 365 F1/F3, Microsoft 365 Enterprise (E3)   |

>[!NOTE]
>Las ofertas anteriores tienen planes de servicio similares con una funcionalidad similar, pero puede haber algunas diferencias entre las ofertas.

### <a name="expiring-offers"></a>Ofertas que expiran

No se le notificará de las ofertas que expiran. Puede realizar un seguimiento de las próximas fechas de expiración mediante la vista del cliente Centro de partners o consultando la API. Se recomienda supervisar esas fechas con frecuencia para poder realizar las acciones de seguimiento apropiadas con los clientes que se acercan a la fecha de caducidad.

Una vez que haya expirado una evaluación, un cliente que intente iniciar sesión en esa versión de prueba verá un mensaje de expiración. Sin embargo, los datos se almacenan de acuerdo con los estándares de retención de datos. Después de comprar una nueva suscripción con los mismos planes de servicio, se puede acceder de nuevo a la información del cliente desde la suscripción recién activada.

## <a name="billing"></a>Facturación

La facturación anual y las pruebas gratuitas son las mismas en las nubes soberanas y en la nube pública. La única diferencia son las SKU de prueba disponibles en el momento del inicio.

## <a name="billing-for-free-trials"></a>Facturación de las pruebas gratuitas

Las pruebas gratuitas se pueden usar para suscripciones facturadas mensuales y anuales. Puede seleccionar la frecuencia de facturación al convertir la versión de prueba en una suscripción de pago.

La fecha de inicio de la suscripción se basa en la fecha de conversión. Si la evaluación gratuita se convierte en una oferta de pago con facturación anual, la fecha de renovación de la suscripción será de 12 meses a partir de la fecha de conversión. Si la evaluación gratuita se convierte en una oferta pagada con facturación mensual, la fecha de renovación de la suscripción será a los doce meses a partir de la fecha de facturación tras la fecha de conversión.

### <a name="invoices"></a>Facturas

No verá las pruebas gratuitas en el archivo de conciliación basado en la factura o la licencia. Las pruebas gratuitas solo aparecerán en el archivo de conciliación basado en la factura y la licencia después de convertir una evaluación gratuita en una suscripción de pago. La suscripción convertida aparecerá de la misma manera que cualquier suscripción nueva.

### <a name="incentives"></a>Incentivos

Las pruebas gratuitas no afectan a los incentivos.

## <a name="support"></a>Soporte técnico

Para obtener soporte técnico sobre las pruebas gratuitas, envíe una solicitud de servicio a través Centro de partners.