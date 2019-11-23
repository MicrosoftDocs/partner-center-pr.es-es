---
title: Ofrecer a los clientes versiones de prueba de productos Microsoft | Centro de partners
ms.topic: article
ms.date: 11/21/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Los clientes pueden probar productos de suscripción a Microsoft durante 30 días. You can sign up for these trials in the catalog just like many other online services.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: ca774233fa6d5314e57f1ab2eb2a73b6037223e5
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/22/2019
ms.locfileid: "74384831"
---
# <a name="offer-your-customers-trials-of-microsoft-products"></a>Ofrecer a los clientes pruebas de productos de Microsoft

Se aplica a:

- Centro de partners

Una buena manera de presentar a los clientes nuevos productos de Microsoft es ofrecer evaluaciones gratuitas de 30 días. Puedes registrarte en las versiones de prueba en el catálogo, al igual que para muchos otros servicios en línea. Todos los partners pueden participar.

## <a name="available-trial-offers"></a>Available trial offers

You can find all of your outstanding trial offers on the **Customer** page. This page lists all subscriptions, including free trials and paid subscriptions. (This feature is not currently available in China.)

Each customer is entitled to one free trial for each available offer. Por ejemplo, pueden obtener una prueba gratuita para Office 365 Empresa Premium y una prueba gratuita para Office 365 E3. However, if the customer already owns the offer, they can't use a free trial for that offer.

### <a name="available-products"></a>Available products

Hay evaluaciones gratuitas disponibles para los siguientes productos:

- Office 365 Empresa Premium
- Office 365 E3
- Office 365 E5 with PSTN
- Office 365 E5 without PSTN
- Enterprise Mobility & Security E5
- Plan Dynamics 365 Customer Engagement 1
- Dynamics 365 for Financials
- Microsoft 365 Empresa

Proporcionamos evaluaciones gratuitas de estos productos porque son las ofertas de empresa más completas y populares. Podemos agregar ofertas adicionales de evaluación gratuita en el futuro.

Currently, there are **no free trials** for government offers, education offers, or add-on offers.

## <a name="licenses-for-free-trial-offers"></a>Licenses for free trial offers

All free trials provide 25 licenses. You can't change this number during the trial. You can't add or remove seats in the free trial. After the trial is converted to a paid subscription, you can add additional licenses to the subscription.

You should assign trial licenses and seats just as you would for a paid service in Partner Center.

## <a name="sign-customers-up-for-trials"></a>Sign customers up for trials

To sign your customer up for a trial through Partner Center:

1. From **Sell** on the Partner Center, go to **Catalog**. 
2. En el catálogo, en **Frecuencia de facturación**, haz clic en **Oferta de prueba**. Esto permite mostrar solo evaluaciones gratuitas y oculta otras ofertas que no son gratuitas. Las pruebas aparecerán en la pestaña **Pruebas** del catálogo.
3. Selecciona la evaluación gratuita que quieras ofrecer y luego selecciona **enviar**. Todas las pruebas están activadas durante 30 días y no recibirás ningún cargo. También puedes convertirla en una suscripción de pago en cualquier momento durante el período de prueba.

## <a name="converting-trials-to-paid-subscriptions"></a>Converting trials to paid subscriptions

A free trial is not automatically converted to a paid subscription. After thirty days, a free trial must be converted to a paid subscription or it will [expire](#expiring-offers). Free trials can't be extended.

You'll need to convert the trial into a paid subscription yourself. You can do this [using the Partner Center](#convert-trials-using-partner-center) or [through the Partner Center APIs](#convert-trials-using-apis).

> [!NOTE]
> Customer free trials for the Cloud Solution Provider (CSP) program can't be converted to another program tenant (such as EA, Open or MOSP).

### <a name="convert-trials-using-partner-center"></a>Convert trials using Partner Center

You can convert trials to paid subscriptions using the Partner Center dashboard as follows:

1. Ve a la página de suscripción del cliente y selecciona la evaluación gratuita.
2. Selecciona **Conversión una prueba en suscripción de pago**.
3. Introduce la cantidad de licencias que desees y la frecuencia de facturación y selecciona **Aplicar**.
4. La facturación de la suscripción de pago comienza en la fecha de conversión y se renueva automáticamente doce meses después de la fecha de conversión. 

### <a name="convert-trials-using-apis"></a>Convert trials using APIs

You may need to alter your APIs to accommodate the conversion of a free trial to a paid subscription. For more information, see the following developer documentation:

- [Convertir una suscripción de prueba en otra de pago](https://docs.microsoft.com/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Obtener una lista de ofertas de conversión de versiones de prueba](https://docs.microsoft.com/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="expiring-offers"></a>Expiring offers

You will not be notified of expiring offers. You can track upcoming expiration dates using the customer view on Partner Center or by querying the API. Se recomienda supervisar esas fechas con frecuencia para poder realizar las acciones de seguimiento apropiadas con los clientes que se acercan a la fecha de caducidad.

After a trial has expired, a customer who attempts to log into that trial will see an expiry message. However, the data is stored in line with data retention standards. After you purchase a new subscription with the same service plans, your customer's information can be accessed again from the newly activated subscription.

## <a name="billing"></a>Facturación

Annual billing and free trials are the same in sovereign clouds and the public cloud. The only difference is the trial SKUs available at the time of launch.

## <a name="billing-for-free-trials"></a>Billing for free trials

Free trials can be used for both monthly and annually billed subscriptions. You can select the billing frequency when you convert the trial to a paid subscription.

The subscription start date is based on the conversion date. Si la evaluación gratuita se convierte en una oferta de pago con facturación anual, la fecha de renovación de la suscripción será a los doce meses a partir de la fecha de conversión. Si la evaluación gratuita se convierte en una oferta pagada con facturación mensual, la fecha de renovación de la suscripción será a los doce meses a partir de la fecha de facturación tras la fecha de conversión.

### <a name="invoices"></a>Facturas

You won't see free trials listed in your invoice or license-based reconciliation file. Free trials will only appear on your invoice and license-based reconciliation file after you convert a free trial to a paid subscription. The converted subscription will appear in the same way as any new subscription.

### <a name="incentives"></a>Incentivos

Free trials do not have an impact on incentives.

## <a name="support"></a>Soporte

For support on free trials, submit a service request through Partner Center.
