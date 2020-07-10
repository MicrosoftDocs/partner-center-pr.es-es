---
title: Ofrecer a los clientes versiones de evaluación de productos de Microsoft
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Permita que los clientes prueben los productos de suscripción de Microsoft durante 30 días. Regístrese para estas pruebas gratuitas en el catálogo, al igual que muchos otros servicios en línea.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3cb1b2104119a28b376301637e559df76392d65c
ms.sourcegitcommit: cba3c73520b8f72d0ba9ca3725f355cab79342c1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/09/2020
ms.locfileid: "86175992"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Ofrezca a los clientes versiones de evaluación gratuitas de los productos de Microsoft durante 30 días

**Se aplica a**

- Centro de partners

**Roles adecuados**
-   Administrador global 
-   Administrador de usuarios
-   Agente de ventas

Una buena manera de presentar a los clientes de nuevos productos de Microsoft es ofrecer pruebas gratuitas de 30 días. Puede registrarse para las pruebas en el catálogo del mismo modo que otros muchos servicios en línea. Todos los partners pueden participar.

## <a name="available-trial-offers"></a>Ofertas de evaluación disponibles

Puede encontrar todas las ofertas de evaluación pendientes en la página del **cliente** . En esta página se enumeran todas las suscripciones, incluidas las versiones de evaluación gratuitas y las suscripciones de pago. (Esta característica no está disponible actualmente en China).

Cada cliente tiene derecho a una evaluación gratuita por cada oferta disponible. Por ejemplo, puede obtener una evaluación gratuita de Microsoft 365 Empresa Standard y una evaluación gratuita para Office 365 E3. Sin embargo, si el cliente ya es propietario de la oferta, no puede usar una evaluación gratuita de la oferta.

### <a name="available-products"></a>Productos disponibles

Las evaluaciones gratuitas están disponibles para las ofertas basadas en licesen más completas y populares. Las nuevas ofertas de evaluación se pueden introducir mensualmente.

Los asociados pueden encontrar versiones de prueba en la lista de precios mensuales en la página **precios y ofertas** del centro de Partners. Las ofertas de evaluación incluirán "evaluación" en la columna **tipo de licencia secundario** de lista de precios.

Actualmente, no hay **ninguna evaluación gratuita** para ofertas de la administración pública, ofertas educativas ni ofertas de complementos.

## <a name="licenses-for-free-trial-offers"></a>Licencias para ofertas de evaluación gratuita

Todas las pruebas gratuitas proporcionan 25 licencias. No se puede cambiar este número durante la evaluación. No puede Agregar o quitar puestos en la evaluación gratuita. Una vez convertida la versión de prueba en una suscripción de pago, puede agregar más licencias a la suscripción.

Las licencias de prueba y puestos deben asignarse a los usuarios de la misma manera que se asigna la licencia de servicios de pago.

## <a name="sign-customers-up-for-trials"></a>Inicio de sesión de los clientes para versiones de prueba

Obtenga una versión de prueba para su cliente en el centro de Partners:

1. Desde **vender** en el centro de Partners, vaya a **Catálogo**. 
2. En el catálogo, desde **frecuencia de facturación**, haga clic en **oferta de evaluación**. Esto permite que solo aparezcan las pruebas gratuitas y se deshabilitan otras ofertas que no son gratuitas. Las pruebas se mostrarán en la pestaña de **pruebas** del catálogo.
3. Seleccione la evaluación gratuita que quiera ofrecer y, a continuación, seleccione **submit (enviar**). Todas las pruebas son durante treinta días durante los cuales no se le cobrará. También puede convertirla en una suscripción de pago en cualquier momento durante la prueba.

## <a name="converting-trials-to-paid-subscriptions"></a>Conversión de pruebas en suscripciones de pago

Una evaluación gratuita no se convierte automáticamente en una suscripción de pago. Después de treinta días, una evaluación gratuita se debe convertir en una suscripción de pago o [expirará](#expiring-offers). Las evaluaciones gratuitas no se pueden ampliar.

Deberá convertir la versión de prueba en una suscripción de pago. Para ello, puede [usar el centro de Partners](#convert-trials-using-partner-center) o [las API del centro de Partners](#convert-trials-using-apis).

> [!NOTE]
> Las evaluaciones gratuitas del cliente para el programa proveedor de soluciones en la nube (CSP) no se pueden convertir a otro inquilino de programa (como EA, Open o MOSP).

### <a name="convert-trials-using-partner-center"></a>Convertir pruebas mediante el centro de Partners

Puede convertir las pruebas en suscripciones de pago mediante el centro de Partners:

1. Vaya a la página de suscripción del cliente y seleccione la evaluación gratuita.
2. Seleccione **convertir evaluación en suscripción de pago**.
3. Escriba la cantidad de licencias deseada y la frecuencia de facturación y seleccione **aplicar**.
4. La facturación de la suscripción de pago comienza en la fecha de conversión y la suscripción se renueva en 12 meses a partir de la fecha de conversión. 

### <a name="convert-trials-using-apis"></a>Conversión de pruebas mediante API

Es posible que tenga que modificar las API para dar cabida a la conversión de una evaluación gratuita en una suscripción de pago. Para obtener más información, consulte la siguiente documentación para desarrolladores:

- [Convertir una suscripción de prueba en otra de pago](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Obtener una lista de ofertas de conversión de versiones de prueba](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Pruebas sin conversiones

No todas las pruebas se pueden convertir en suscripciones de pago. Los asociados pueden usar una versión de prueba que no tenga conversiones hasta la fecha de expiración. Los asociados pueden adquirir ofertas compatibles que admitan los mismos servicios que la oferta de evaluación.  Esto debe hacerse antes de que expire la evaluación para asegurarse de que los servicios de las ofertas recién compradas se alineen con los servicios de la versión de prueba. 

|**Versión de prueba**   |**Ofertas de pequeñas empresas compatibles**   |**Ofertas Enterprise compatibles**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Evaluación de la nube comercial de Microsoft Teams (Iniciado por el usuario)   |Microsoft 365 Empresa Basic, Microsoft 365 Empresa Standard, Microsoft 365 Empresa Premium   | F3 (anteriormente F1), Office 365 para empresas (E1, E3 y E5), M365 F1/F3, M365 Enterprise (E3)   |

>[!NOTE]
>Las ofertas anteriores tienen planes de servicio similares con una funcionalidad similar, pero puede haber algunas diferencias entre las ofertas.

### <a name="expiring-offers"></a>Ofertas que van a expirar

No recibirá ninguna notificación de las ofertas que expiren. Puede realizar un seguimiento de las fechas de expiración futuras mediante la vista de cliente del centro de Partners o consultando la API. Se recomienda supervisar esas fechas con frecuencia para poder realizar las acciones de seguimiento apropiadas con los clientes que se acercan a la fecha de caducidad.

Una vez que haya expirado una evaluación, un cliente que intente iniciar sesión en esa prueba verá un mensaje de expiración. Sin embargo, los datos se almacenan en línea con los estándares de retención de datos. Después de comprar una nueva suscripción con los mismos planes de servicio, se puede acceder a la información del cliente desde la suscripción que se acaba de activar.

## <a name="billing"></a>Facturación

La facturación anual y las evaluaciones gratuitas son las mismas en las nubes independientes y en la nube pública. La única diferencia es que las SKU de prueba están disponibles en el momento del lanzamiento.

## <a name="billing-for-free-trials"></a>Facturación para pruebas gratuitas

Las evaluaciones gratuitas se pueden usar para las suscripciones facturadas mensuales y anuales. Puede seleccionar la frecuencia de facturación al convertir la versión de prueba en una suscripción de pago.

La fecha de inicio de la suscripción se basa en la fecha de conversión. Si la evaluación gratuita se convierte en una oferta de pago con facturación anual, la fecha de renovación de la suscripción será a los doce meses a partir de la fecha de conversión. Si la evaluación gratuita se convierte en una oferta pagada con facturación mensual, la fecha de renovación de la suscripción será a los doce meses a partir de la fecha de facturación tras la fecha de conversión.

### <a name="invoices"></a>Facturas

No verá las pruebas gratuitas que aparecen en la factura o el archivo de conciliación basado en licencias. Las evaluaciones gratuitas solo aparecerán en la factura y el archivo de conciliación basado en licencias después de convertir una evaluación gratuita en una suscripción de pago. La suscripción convertida aparecerá de la misma manera que cualquier suscripción nueva.

### <a name="incentives"></a>Incentivos

Las evaluaciones gratuitas no afectan a los incentivos.

## <a name="support"></a>Soporte técnico

Para obtener soporte técnico sobre las pruebas gratuitas, envíe una solicitud de servicio a través del centro de Partners.
