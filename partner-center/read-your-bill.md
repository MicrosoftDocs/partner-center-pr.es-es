---
title: Cómo leer el archivo de conciliación & factura
ms.topic: article
ms.date: 06/05/2020
description: Obtenga información sobre los archivos de conciliación & factura. La factura muestra Centro de partners cargos en el programa, los productos y los clientes durante ese período mensual.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbdf85d20e15841189191d6b415b54c26378850e
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551204"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Comprender el archivo de facturación y conciliación: aprenda a encontrarlos en Centro de partners


**Roles adecuados:** administrador global | Administración de facturación | Agente de administración


La **factura** es un **resumen de todos los** cargos Centro de partners cliente (en todo el programa, todos los productos y todos los clientes). 

## <a name="find-your-bill-and-reconciliation-file"></a>Buscar el archivo de facturación y conciliación 

Puede encontrar la factura en la página Facturación del panel en Centro de partners. También puede encontrar el historial de facturación, las tendencias de gasto y los archivos de conciliación en esta página. 

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard/home) del Centro de partners. 

2. En el menú de la izquierda, seleccione **Facturación.** 

3. En la página de estado de facturación, selecciona una factura o un archivo de conciliación para ver información más detallada. 

Puede encontrar un vínculo a la factura más reciente en la parte superior de la página en Saldo de la cuenta a partir de la fecha de la última factura. 

Puede encontrar facturas anteriores en la sección Historial de facturación. Elija el año adecuado y, a continuación, seleccione la flecha desplegable situada junto al período de facturación adecuado. Seleccione el vínculo situado junto a Facturas (.pdf) para descargar la factura de ese período. 

## <a name="invoice-types"></a>Tipos de factura

Microsoft emitirá una factura por los cargos basados en licencias (como Office 365) y los cargos basados en el uso (como Azure) y una factura independiente para los cargos únicos (como instancias reservadas de Azure, Marketplace o el plan de Azure).

Por ejemplo,  

**Escenario 1 [moneda única]:** el partner tiene compras para ofertas 145P y licencias de Office 365,  

- El asociado recibirá un PDF de factura y dos archivos de conciliación que cubren los cargos de Office 365 y Azure (145p).  

**Escenario 2 [moneda única]:** el partner tiene compras para instancias reservadas de Azure, Marketplace o un plan de Azure junto con compras de 145p.

- El asociado recibirá un pdf de factura y un archivo de conciliación que cubre los cargos de Azure (145p). 

- El asociado recibirá otro PDF de factura y un archivo de conciliación que cubre los cargos de la instancia reservada (RI) de Azure, Marketplace y el plan de Azure. 

**Escenario 3 [moneda múltiple]:** el partner tiene compras para Instancias reservadas de Azure en DKK y el plan de Azure en EUR junto con compras de 145p en EUR.

- El asociado recibirá un pdf de factura y un archivo de conciliación que cubre los cargos de instancias reservadas de Azure en DKK. 

- El asociado recibirá un pdf de factura y un archivo de conciliación que cubre los cargos del plan de Azure en EUR. 

- El partner recibirá otro PDF de factura y un archivo de conciliación que cubre los cargos de la oferta de 145p en EUR (o moneda de facturación del asociado). 


## <a name="understanding-invoice-pdf"></a>Descripción del PDF de factura 

**Facturas por** uso y cargos basados en licencias: las facturas de los cargos de servicios como Office 365 y Azure estarán disponibles en un plazo de dos (2) días a partir de la fecha de facturación seleccionada [UTC].  

**Facturas de cargos únicos** y periódicos: las facturas de cargos por servicios como Azure RI, el plan de Azure y Marketplace estarán disponibles no más tarde del octavo de cada mes.  

A continuación se muestran algunos de los campos clave del documento PDF de factura:

**Número de factura:** identificador único para el documento de factura generado para el período de facturación correspondiente. 

**Período de** facturación: es el período durante el que tiene usos y servicios basados en licencias. 

**Fecha de factura:** fecha de facturación o fecha de aniversario en la que se genera la factura cada mes. 

**Fecha de vencimiento del** pago: la fecha en que se debe recibir el pago. 

**Cargos:** importe a pagar en la moneda de facturación para el período de facturación correspondiente. 

**Créditos:** créditos (como contrato de nivel de servicio )) o ajustes para los cambios realizados en las suscripciones (por ejemplo, aumentos o disminuciones de licencias). 

**Instrucciones de** pago: descripción de cómo pagar la factura en función de su región. Asegúrese siempre de incluir el número de factura al realizar un pago. 

Para obtener una descripción detallada de todos los campos del archivo de factura (incluidos los campos para cargos únicos), consulte [Campos de archivo de factura](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Información sobre los archivos de conciliación

 Los archivos de conciliación, que proporcionan una exploración en profundidad o detalles de los cargos, están disponibles para su descarga junto con el PDF de factura. Los archivos de conciliación incluyen identificadores de cliente e identificadores de suscripción que puede usar para crear facturas de cliente. Para obtener más información sobre los archivos de conciliación, [vea Cómo usar los archivos de conciliación](use-the-reconciliation-files.md). 

## <a name="next-steps"></a>Pasos siguientes

- [Cómo usar los archivos de conciliación](use-the-reconciliation-files.md)