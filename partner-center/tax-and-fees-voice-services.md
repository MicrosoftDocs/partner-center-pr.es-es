---
title: Impuestos y tarifas del servicio RTC regional
description: Como asociado de Office 365 que realiza transacciones con Microsoft 365 Voice, puede estar sujeto a impuestos regionales, tarifas o requisitos normativos para los servicios RTC.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 80cb5503323f483c13c983375559baf70f9d0b6f
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854730"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Impuestos regionales, normativas para los servicios de red telefónica conmutada pública (PTSN)

**Roles adecuados:** Administrador global | Administrador de | Agente de administración

Los servicios públicos de red telefónica conmutada (RTC) en algunas jurisdicciones pueden estar sujetos a requisitos fiscales y normativos especiales que pueden afectar al orden y la facturación de los asociados. En el Estados Unidos, incluido Puerto Rico, los servicios RTC, que incluyen audioconferencia, planes de llamadas y créditos de comunicación, están sujetos a requisitos fiscales y normativos especiales. En el Estados Unidos y Puerto Rico, Microsoft precios los servicios RTC como tax-inclusive.  Los impuestos y las regulaciones únicos de RTC afectarán a los asociados de Office 365 que realicen transacciones Microsoft 365 voice.  Si un partner marca el precio de un servicio RTC de Microsoft, puede ser responsable del cálculo y de la remesa de impuestos y tasas de RTC.

## <a name="partner-recommendations"></a>Recomendaciones para asociados

Implique a su asesor fiscal y legal para comprender la responsabilidad de su organización con respecto a la regulación, los impuestos y las tarifas de los servicios RTC y otras posibles responsabilidades.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Presentación de facturas y archivo de conciliación de asociados

Las facturas de CSP y los archivos de conciliación de CSP de Estados Unidos, Puerto Rico y Canadá, que incluyen los servicios RTC de Skype Empresarial y Microsoft 365 Voice, proporcionarán elementos de línea independientes para los componentes RTC y no RTC.

Además, las facturas de CSP mostrarán la siguiente nota al pie:

* El precio mostrado es un cargo por audioconferencia y servicios de plan de llamada.  Los impuestos transaccionales aplicables se cobran exclusivamente del importe mostrado, excepto las ventas realizadas dentro del Estados Unidos.  En Estados Unidos, el precio que se muestra es tax inclusive, ya que incluye un cargo por los servicios de plan de llamada y audioconferencia y un cargo por los impuestos y tarifas que se deben cobrar.  Los servicios de audioconferencia y plan de llamada son atendidas por el asociado de Microsoft autorizado para proporcionarlos.  Consulte [Licencias por Volumen de Microsoft](https://go.microsoft.com/fwlink/?LinkId=690247) para más información.

## <a name="reconciliation-file-example"></a>Ejemplo de archivo de conciliación

Office 365 Enterprise E5 se presenta en el archivo de conciliación como dos elementos de línea con nombres idénticos e identificadores idénticos, pero cada elemento de línea tiene un precio unitario único (por ejemplo: 28,40 USD y 2,00 USD). Esto separa el componente Conferencia RTC de Skype Empresarial de la oferta de Office 365, para que puedas aplicar correctamente los impuestos.

**Ejemplo de conciliación #1 asociados (seleccionar columnas):**

|**ID_oferta_durable**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Tarifa de ciclo   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Tarifa de ciclo   |2.00   |

**Ejemplo de conciliación de asociados #2**

Microsoft 365 Business Voice disponible en Canadá tiene componentes imponibles rtcN adicionales que se consolidan en la factura de CSP (de forma similar a Office 365 E5, se presentan dos elementos de línea, uno para los componentes RTC y el otro para los componentes que no son RTC).  El archivo de conciliación de CSP para Microsoft 365 Business Voice mostrará todos los componentes imponibles de RTC individualmente (los componentes RTC individuales no se consolidarán en . CSV o herramienta de API).  La suma de los detalles del pedido y los importes facturados de los clientes que se encuentran en el archivo de conciliación coincidirá con la factura de CSP.

## <a name="additional-resources"></a>Recursos adicionales
Para más información, visite el sitio [de Microsoft 365 for Partners.](https://www.microsoft.com/microsoft-365/partners/)

