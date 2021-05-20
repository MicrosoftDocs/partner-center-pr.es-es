---
title: 'Facturación: transacciones SaaS basadas en licencias'
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre los escenarios comunes de facturación Centro de partners para transacciones de software como servicio (SaaS) basadas en licencias.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 764d5a3cb0dc6f409e5272d4119424396caff53b
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148642"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Escenarios comunes de facturación para transacciones SaaS basadas en licencias en Centro de partners

**Roles adecuados:** agente de administración | Administrador de facturación | Agente del departamento de soporte técnico | Agente de ventas


Estos [escenarios comunes de facturación de](common-billing-scenarios.md) ejemplo son aplicables a las suscripciones de software como servicio (SaaS) basadas en licencias en Centro de partners.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Conversión de una suscripción de SaaS de evaluación gratuita en una suscripción de pago

En este escenario se describe la facturación para la renovación de una suscripción de SaaS de evaluación gratuita basada en licencias. La renovación convierte la evaluación gratuita en una suscripción de pago al final del período de evaluación gratuita.

En este ejemplo, adquirió una evaluación gratuita de una suscripción de SaaS (software como servicio) basada en licencia el 10 de junio. Esta evaluación gratuita se renueva automáticamente como una suscripción de pago cuando finaliza el período de evaluación gratuita.

Los archivos de conciliación incluirán los cargos siguientes:

| Fecha de compra | Fecha de inicio del cargo | Fecha de finalización del cargo | Precio unitario | Cantidad de unidades | Importe total | Tipo de cargo | Descripción de la suscripción |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | 10/06/2019 | 07/09/2019 | 0 $ | 1 | 0 $ | Nuevo | Evaluación gratuita |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | 2 $ | 1 | 2 $ | Renovación | Suscripción de pago |

## <a name="cancel-a-free-trial-saas-subscription"></a>Cancelación de una suscripción de SaaS de evaluación gratuita

> [!TIP]
> Puede cancelar una suscripción de SaaS de evaluación gratuita basada en licencia en cualquier momento, incluso durante el período de evaluación gratuita.

En este escenario, adquirió una suscripción de SaaS de evaluación gratuita basada en licencia el 1 de julio y, a continuación, la canceló inmediatamente en Centro de partners.

El archivo de conciliación incluirá los cargos siguientes:

| Fecha de compra | Fecha de inicio del cargo | Fecha de finalización del cargo | Precio unitario | Cantidad de unidades | Importe total | Tipo de cargo | Descripción de la suscripción |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | 10/06/2019 | 07/09/2019 | 0 $ | 11 | 0 $ | Nuevo | Evaluación gratuita |
| 10/06/2019 | 10/06/2019 | 07/09/2019 | 0 $ | 11 | 0 $ | Cancelar | Evaluación gratuita |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>Conversión de una suscripción saaS de medidor personalizado a otra SKU

En este escenario se describe cómo convertir una suscripción de SaaS de medidor personalizado de una unidad de mantenimiento de existencias (SKU) a otra SKU para el mismo producto, en la misma fecha.

En este escenario, ha adquirido una SKU (Silver) en un producto y la ha convertido en otra SKU disponible (Bronze) en este producto en la misma fecha.

El archivo de conciliación incluirá los cargos siguientes:

| Fecha de compra | SKU | Fecha de inicio del cargo | Fecha de finalización del cargo | Precio unitario | Cantidad de unidades | Importe total | Tipo de cargo | Descripción de la suscripción |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | Plata | 10/06/2019 | 10/06/2019 | 20 $ | 1 | 20 $ | Nuevo | Suscripción de SaaS de medidor personalizado |
| 10/06/2019 | Plata | 10/06/2019 | 10/06/2019 | 20 $ | 1 | -$20 | Convert | Refacturación prorrateada para la suscripción de SaaS de medidor personalizado |
| 10/06/2019 | Bronce | 10/06/2019 | 10/06/2019 | 10 $ | 1 | 10 $ | Convert | Suscripción de SaaS de medidor personalizado |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Compra y cancelación de una suscripción de SaaS de medidor de clientes en la misma fecha

En este escenario se describe la facturación de una suscripción de SaaS de medidor de clientes que compró y canceló a través del Azure Portal en la misma fecha.

En este escenario, ha adquirido una suscripción de SaaS de medidor personalizado en el Azure Portal. A continuación, canceló la suscripción en la misma fecha.

| Fecha de compra | SKU | Fecha de inicio del cargo | Fecha de finalización del cargo | Precio unitario | Cantidad de unidades | Importe total | Tipo de cargo | Descripción de la suscripción |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 10/06/2019 | Bronce | 10/06/2019 | 10/06/2019 | 10 $ | 1 | 10 $ | Nuevo | Suscripción de SaaS de medidor personalizado |
| 10/06/2019 | Bronce | 10/06/2019 | 10/06/2019 | 10 $ | 1 | -$10 | CancelImmediate | Suscripción de SaaS de medidor personalizado |
