---
title: Transacciones de SaaS basadas en licencias de facturación
ms.topic: article
ms.date: 05/05/2020
description: Obtenga información sobre los escenarios de facturación comunes en el centro de partners para transacciones SaaS basadas en licencias.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
Keywords: facturación, pagos, compra única, compra periódica, suscripciones, puestos
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 02a50f5be3c19f179014fd7db4e1418ba025e874
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908193"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Escenarios comunes de facturación para las transacciones SaaS basadas en licencias en el centro de Partners

**Roles adecuados**

- Agente de administrador
- Administrador de facturación
- Agente del departamento de soporte técnico
- Agente de ventas


Estos ejemplos de [escenarios de facturación comunes](common-billing-scenarios.md) se aplican a las suscripciones de software como servicio (SaaS) basadas en licencias en el centro de Partners.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Convertir una suscripción de SaaS de evaluación gratuita en una suscripción de pago

En este escenario se describe la facturación de la renovación de una suscripción de SaaS de evaluación gratuita basada en licencias. La renovación convierte la evaluación gratuita en una suscripción de pago al final del período de evaluación gratuita.

En este ejemplo, adquirió una evaluación gratuita de una suscripción de SaaS (software como servicio) basada en licencias el 10 de junio. Esta evaluación gratuita se renueva automáticamente como una suscripción de pago cuando finaliza el período de evaluación gratuita.

Los archivos de conciliación incluirán los siguientes cargos:

| Fecha de compra | Fecha de inicio de la carga | Fecha de finalización del cargo | Precio unitario | Cantidad de unidad | Importe total | Tipo de cargo | Descripción de la suscripción |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | 10/06/2019 | 07/09/2019 | 0 $ | 1 | 0 $ | Nuevo | Evaluación gratuita |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | 2 $ | 1 | 2 $ | Renovación | Suscripción de pago |

## <a name="cancel-a-free-trial-saas-subscription"></a>Cancelar una suscripción de SaaS de evaluación gratuita

> [!TIP]
> Puede cancelar una suscripción SaaS de evaluación gratuita basada en licencias en cualquier momento, incluso durante el período de evaluación gratuita.

En este escenario, adquirió una suscripción SaaS de evaluación gratuita basada en licencias el 1 de julio y la canceló inmediatamente en el centro de Partners.

El archivo de conciliación incluirá los siguientes cargos:

| Fecha de compra | Fecha de inicio de la carga | Fecha de finalización del cargo | Precio unitario | Cantidad de unidad | Importe total | Tipo de cargo | Descripción de la suscripción |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | 10/06/2019 | 07/09/2019 | 0 $ | 11 | 0 $ | Nuevo | Evaluación gratuita |
| 10/06/2019 | 10/06/2019 | 07/09/2019 | 0 $ | 11 | 0 $ | Cancelar | Evaluación gratuita |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Convertir la suscripción de SaaS de medidor personalizado en otra SKU

En este escenario se describe cómo convertir una suscripción de SaaS de medidor personalizado de una referencia de almacén (SKU) a otra SKU para el mismo producto en la misma fecha.

En este escenario, adquirió una SKU (Silver) bajo un producto y la convirtió en otra SKU disponible (bronce) en este producto en la misma fecha.

El archivo de conciliación incluirá los siguientes cargos:

| Fecha de compra | SKU | Fecha de inicio de la carga | Fecha de finalización del cargo | Precio unitario | Cantidad de unidad | Importe total | Tipo de cargo | Descripción de la suscripción |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | Plata | 10/06/2019 | 10/06/2019 | 20 $ | 1 | 20 $ | Nuevo | Suscripción SaaS de medidor personalizado |
| 10/06/2019 | Plata | 10/06/2019 | 10/06/2019 | 20 $ | 1 | -$20 | Convert | Renovación prorrateada para la suscripción SaaS de medidor personalizado |
| 10/06/2019 | Bronce | 10/06/2019 | 10/06/2019 | 10 $ | 1 | 10 $ | Convert | Suscripción SaaS de medidor personalizado |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Compra y cancelación de una suscripción de SaaS de Customer meter en la misma fecha

En este escenario se describe la facturación de una suscripción de SaaS de Customer meter que ha adquirido y cancelado a través del Azure Portal en la misma fecha.

En este escenario, adquirió una suscripción de SaaS de medidor personalizado en el Azure Portal. A continuación, canceló la suscripción en la misma fecha.

| Fecha de compra | SKU | Fecha de inicio de la carga | Fecha de finalización del cargo | Precio unitario | Cantidad de unidad | Importe total | Tipo de cargo | Descripción de la suscripción |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | Bronce | 10/06/2019 | 10/06/2019 | 10 $ | 1 | 10 $ | Nuevo | Suscripción SaaS de medidor personalizado |
| 10/06/2019 | Bronce | 10/06/2019 | 10/06/2019 | 10 $ | 1 | -$10 | CancelImmediate | Suscripción SaaS de medidor personalizado |
