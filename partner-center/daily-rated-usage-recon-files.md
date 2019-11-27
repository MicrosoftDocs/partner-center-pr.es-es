---
title: Archivos de conciliación de uso con clasificación diaria | Centro de Partners
ms.topic: article
ms.date: 11/21/2019
description: Comprenda los archivos de conciliación de uso clasificados diariamente en el centro de Partners.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 896f81b3a51e234065af7779d287b4023dd7163c
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389703"
---
# <a name="daily-rated-usage-reconciliation-files"></a>Archivos de conciliación de uso clasificados diariamente

Se aplica a:

- Centro de partners
- Centro de partners para Microsoft Cloud for US Government

En este tema se explica cómo leer archivos de conciliación de uso clasificados diariamente.

## <a name="fields-in-daily-rated-usage-reconciliation-files"></a>Campos en archivos de conciliación de uso clasificados diariamente

| Column | Descripción |
| ------ | ----------- |
| PartnerId | Identificador del asociado en formato GUID. |
| PartnerName | Nombre del asociado. |
| CustomerId | Identificador único de Microsoft para el cliente en formato GUID. |
| CustomerCompanyName | Nombre de la organización del cliente según se indica en el Centro de partners. *Esta columna es muy importante para conciliar la factura con la información del sistema.* |
| CustomerDomainName | El nombre de dominio del cliente. No está disponible para la actividad actual. |
| País del cliente | El país donde se encuentra el cliente. |
| MPNID | Identificador de MPN del asociado de CSP. |
| Reseller MPNID | Identificador de MPN del distribuidor de registro de la suscripción. No está disponible para la actividad actual. |
| InvoiceNumber | Número de factura donde aparece la transacción especificada. No está disponible para la actividad actual. |
| ProductId | Identificador del producto. |
| SkuId | Identificador de una SKU determinada. |
| AvailabilityId | Identificador de la disponibilidad de una SKU determinada. Esto muestra si la SKU está disponible para su compra en el país determinado, la moneda, el segmento del sector, etc. |
| Nombre de SKU | Título para un SKU concreto. |
| PublisherName | Nombre del publicador. |
| PublisherID | Identificador del publicador en formato GUID. No está disponible para la actividad actual. |
| Descripción de la suscripción | Nombre de la oferta de servicio adquirida por el cliente, según se define en la lista de precios. (Este campo es idéntico a **nombredeoferta**). |
| Id. de la suscripción | Identificador único de una suscripción en la plataforma de facturación de Microsoft. No se usa para la conciliación. *Este identificador no es el mismo que el **identificador de suscripción** en la consola de administración de socios comerciales.* |
| ChargeStartDate | Fecha de inicio del ciclo de facturación (excepto cuando se presentan fechas de datos de uso latente previamente no cargados del ciclo de facturación anterior). La hora siempre corresponde al comienzo del día, 0:00. |
| ChargeEndDate | Fecha final del ciclo de facturación (excepto cuando se presentan fechas de datos de uso latente previamente no cargados del ciclo de biling anterior). La hora siempre corresponde al fin del día, 23:59. |
| Fecha de uso | Fecha del uso del servicio. |
| Tipo de medidor | Tipo de medidor. |
| Categoría de medidor | El servicio de nivel superior para el uso. |
| ID. de medidor | Identificador del medidor que se está usando. |
| Subcategoría de medidor | El tipo de servicio de Azure, que puede afectar a la tarifa. |
| Nombre del medidor | Unidad de medida del medidor que se está consumiendo. |
| Región de medidor | Esta columna identifica la ubicación de un centro de datos dentro de la región para los servicios donde esto se aplica y rellena. |
| Unidad | Unidad del **nombre**del recurso. |
| Cantidad consumida | La cantidad de servicio consumido (como *Horas* o *GB*) durante el período de notificación. Incluye cualquier uso no facturado de períodos de informes anteriores. |
| Ubicación del recurso | > el centro de datos donde se está ejecutando el medidor. |
| Servicio consumido | El servicio de la plataforma Azure que ha usado. |
| URI de recurso | URI del recurso que se va a usar. |
| Tipo de cargo | Tipo de cargo o ajuste. No está disponible para la actividad actual. |
| Precio unitario | Precio por licencia, tal como se publicó en la lista de precios en el momento de la compra. Asegúrese de que este precio coincida con la información almacenada en el sistema de facturación durante la conciliación. |
| Cantidad | Número de licencias. Asegúrese de que este precio coincida con la información almacenada en el sistema de facturación durante la conciliación. |
| Tipo de unidad | Tipo de unidad en la que se carga el medidor. No está disponible para la actividad actual. |
| Impuesto previo de facturación | Importe total de facturación antes de los impuestos. |
| Moneda de facturación | La moneda en la región geográfica del cliente. |
| Precio pretax total | Los precios antes de que se agreguen los impuestos. |
| Moneda de precios | La moneda en la lista de precios. |
| Información de servicio 1 | El número de conexiones Service Bus aprovisionadas y utilizadas en un día determinado. |
| Información de servicio 2 | Campo heredado que captura los metadatos específicos del servicio opcionales. |
| Información adicional | Cualquier información adicional no incluida en otras columnas. |
