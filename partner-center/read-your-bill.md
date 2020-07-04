---
title: Cómo leer el archivo de conciliación & de la factura
ms.topic: article
ms.date: 06/05/2020
description: Obtenga información sobre la factura & los archivos de conciliación. La factura muestra los cargos del centro de Partners en el programa, los productos y los clientes durante ese período mensual.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
keywords: facturación de suscripciones, facturación, facturación en el centro de Partners, facturación del centro de Partners, leer mi factura, factura, factura del centro de Partners, factura de CSP, ¿Dónde está mi factura?
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 40809fbca8ed81882e9b1d315fd5967143faff1e
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949320"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Descripción del archivo de conciliación y facturación: Obtenga información sobre cómo encontrarlos en el centro de Partners.

**Se aplica a**

- Centro de partners
- Centro de partners para Microsoft Cloud for US Government

**Roles adecuados**

- Administrador global
- Administrador de facturación
- Agente de administrador


La **factura** es un **Resumen de todos los cargos del centro de Partners** (en todo el programa, todos los productos y todos los clientes). 

## <a name="invoice-types"></a>Tipos de factura

Microsoft emitirá una factura por los cargos basados en licencia (como Office 365) y los cargos basados en el uso (como Azure) y una factura independiente por cargos de un solo uso (como Azure RI, Marketplace o Azure plan).

Por ejemplo,  

**Escenario 1 [moneda única]**: el asociado tiene compras para la oferta de 145P y licencias de O365,  

- El asociado obtendrá un PDF de factura y dos archivos de conciliación que cubren los cargos de O365 y Azure (145p).  

**Escenario 2 [sola moneda]**: el asociado tiene compras de Azure RI, Marketplace y/o Azure Plan junto con compras 145p.

- El asociado obtendrá un PDF de factura y un archivo de conciliación que cubra los cargos de Azure (145p). 

- El asociado recibirá otro PDF de factura y un archivo de conciliación que cubra sus cargos de Azure RI, Marketplace, Azure plan. 

**Escenario 3 [multimoneda]**: el asociado tiene compras de Azure RI en DKK y Azure plan en EUR junto con las compras de 145P en EUR.

- El asociado recibirá un PDF de factura y un archivo de conciliación que cubre los cargos de Azure RI en DKK. 

- El asociado recibirá un PDF de factura y un archivo de conciliación que cubre los cargos de Azure plan en EUR. 

- El asociado recibirá otro PDF de factura y un archivo de conciliación que cubra los cargos de la oferta 145p en euros (o en la moneda de facturación de los asociados). 

## <a name="find-your-bill"></a>Búsqueda de tu factura 

Puede encontrar la factura en la página facturación del panel del centro de Partners. También puede buscar el historial de facturación, las tendencias de gasto y los archivos de conciliación en esta página. 

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard/home) del Centro de partners. 

2. En el menú de la izquierda, seleccione **facturación**. 

3. En la página facturación, seleccione la factura que desea descargar. 

Puede encontrar un vínculo a la factura más reciente en la parte superior de la página en saldo de cuenta en la fecha de la última factura. 

Puede encontrar facturas anteriores en la sección historial de facturación. Elija el año adecuado y, a continuación, seleccione la flecha desplegable situada junto al período de facturación adecuado. Seleccione el vínculo situado junto a facturas (. pdf) para descargar la factura de ese período. 

## <a name="understanding-invoice-pdf"></a>Descripción de la factura PDF 

**Facturas de uso y cargos basados en licencias**: las facturas de cargos por servicios como Office 365 y Azure estarán disponibles en un plazo de dos (2) días a partir de la fecha de facturación seleccionada [UTC].  

**Facturas para cargos de onetime y recurrentes**: las facturas de cargos por servicios como Azure RI, Azure plan, Marketplace estarán disponibles a partir del 8 de cada mes.  

A continuación se muestran algunos de los campos clave del documento PDF de factura:

**Número de factura**: identificador único para el documento de factura generado para el período de facturación correspondiente. 

**Período de facturación**: este es el período durante el cual se tienen usos y servicios basados en licencias. 

**Fecha**de la factura: fecha de facturación o fecha de aniversario en la que se genera la factura cada mes. 

**Fecha de vencimiento del pago**: fecha en la que se debe recibir el pago. 

**Cargos**: la cantidad debida a la moneda de facturación para el período de facturación correspondiente. 

**Créditos**: créditos (como contrato de nivel de servicio) o ajustes para los cambios realizados en las suscripciones (por ejemplo, aumentos o disminuciones del asiento). 

**Instrucciones de pago**: Descripción de cómo pagar la factura, en función de su región. Asegúrese de incluir siempre el número de factura al realizar un pago. 

Para obtener una descripción detallada de todos los campos del archivo de factura (incluidos los campos de cargos de un solo tiempo), consulte [campos de archivo de factura](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Descripción de los archivos de conciliación

 Los archivos de conciliación, que proporcionan detalles detallados o desglosados de los cargos, están disponibles para su descarga junto con el PDF de factura. Los archivos de conciliación incluyen los identificadores de cliente y los identificadores de suscripción que puede usar para crear facturas de cliente. Consulte  [Cómo usar los archivos de conciliación](use-the-reconciliation-files.md) para obtener más detalles sobre los archivos de conciliación. 
