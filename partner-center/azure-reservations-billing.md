---
title: Facturación de Azure Reservations | Centro de partners
ms.topic: article
ms.date: 10/29/2018
Description: Información sobre la facturación de las reservas de Azure.
author: LauraBrenner
ms.author: v-petand
keywords: Azure RI, instancias reservadas de azure, reservas, vm, administrar, facturación, comprar
robots: noindex, nofollow
ms.localizationpriority: medium
ms.openlocfilehash: b32c0da58cefea764f7f0cb3adb6d3a13faa46b5
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586908"
---
# <a name="microsoft-azure-reserved-vm-instances-billing"></a>Facturación de Microsoft Azure Reserved VM Instances

**Se aplica a**

-  Centro de partners
-  Microsoft Azure Portal
-  Partners de CSP

Los partners del programa de Proveedor de soluciones en la nube (CSP) pueden ofrecer a sus clientes instancias reservadas en máquinas virtuales de Microsoft Azure. Los clientes pueden reservar máquinas virtuales de antemano (para periodos de uno a tres años) y tener ahorros significativos en el uso de Azure.   

Tus clientes pagan por adelantado para Azure Reserved VM Instances. Al comprar Azure Reserved VM Instances en nombre de un cliente, recibirás facturas y archivos de conciliación para estos cargos únicos. 

>[!IMPORTANT]
>Si has comprado Azure Reserved VM Instances para un cliente en un mercado con una moneda diferente a la tuya, la divisa de facturación predeterminada se basa en el mercado del cliente, no en tu ubicación. Si tienes clientes en varios mercados, recibirás facturas y archivos de conciliación independientes para cada divisa en la que los clientes deben facturar, lo que te permite facturar a los clientes en la divisa adecuada. 

Para obtener acceso a las facturas de cargo único y archivos de conciliación, seleccione **facturación** desde el centro de partners y, a continuación, seleccione **una vez**. 

Para obtener más información general sobre facturación en el programa Proveedor de soluciones en la nube, consulta [Conceptos básicos sobre facturación](billing-basics.md).

## <a name="azure-reserved-vm-instance-invoice-file-definitions"></a>Definiciones de archivos de factura de Azure Reserved VM Instances

**Información general de facturación**

|**Field** |**Definición**|
|:----------------|:-----------------------------|
|US FEIN |El número de identificación fiscal federal. |
|Facturar a |La dirección de empresa legal que se usa por motivos fiscales. Para cambiar esta dirección, ve a Configuración de la cuenta > Perfil de facturación de partner. |
|Cargos |Todos los cargos actuales. |
|Créditos |Créditos para actividad de reembolso desde la compra inicial. |
|Descuentos |Descuentos que se pueden aplicar a Azure reservations u otros elementos del pedido del cliente. |
|Taxes |El total de impuestos para los cargos actuales según se suman en la sección de detalles a partir de la página 2 de la factura. |
|Total current charges |El importe debido en la divisa de facturación para el período de facturación, que se debe abonar antes de la fecha de vencimiento de pago. |
|Payment instructions |Describe cuándo y cómo pagar la factura, según tu región. Al realizar un pago, siempre incluye el número de factura. |
|N.º de factura |El número de la factura. |
|Invoice date |La fecha en que se generó tu factura. |
|Condiciones de pago |Para las compras de pago único siempre serán 60 días. |
|Payment due date |Fecha en la que debe recibirse tu pago. |


**Lista detallada de los cargos por única vez**

|**Field** |**Definición**|
|:----------------|:-----------------------------|
|Fecha |Fecha de compra. |
|Descripción |Nombre del producto. |
|Cantidad |Número de productos (reservas, por ejemplo) adquiridos. |
|Precio unitario |Precio por producto (reserva, por ejemplo). |
|Descuentos |Descuentos aplicables. |
|Importe antes de impuestos |Subtotal de las compras antes de impuestos. |
|Impuesto sobre ventas |Importe de impuestos. |
|Total |Total que se pagará. |


## <a name="azure-reserved-vm-instance-reconciliation-file-descriptions"></a>Definiciones de archivos de conciliación de Azure Reserved VM Instances

|**Field** |**Definición**|
|:----------------|:-----------------------------|
|PartnerId |Id. de partner, en formato de GUID. |
|CustomerId |Id. de Microsoft único, en formato GUID, usado para identificar al cliente. |
|CustomerName |Nombre de la organización del cliente según se indica en el Centro de partners. Esto es muy importante para conciliar la factura con la información del sistema. |
|CustomerDomainName |Nombre de dominio del cliente. |
|CustomerCountry |El país donde se encuentra el cliente. |
|InvoiceNumber |Número de factura donde aparece la transacción especificada. |
|MpnId |Id. de MPN del partner CSP (directo o indirecto). |
|Id. de MPN del revendedor |Solo aparece en los archivos de conciliación de partners en el modelo indirecto. Id. de MPN del revendedor de registro de la reserva. Corresponde al id. de revendedor indicado para la reserva específica en el Centro de partners. Si un partner CSP vendió la reserva directamente al cliente, su id. de MPN aparece dos veces, como id. de MPN y como id. de MPN del revendedor. Si un partner CSP tiene un revendedor sin un id. de MPN, este valor se establece en el id. de MPN del partner. Si el partner CSP quita un id. de revendedor, este valor se establece en -1. |
|OrderId |Identificador único de un pedido en la plataforma de facturación de Microsoft. Puede ser útil para identificar la reserva al ponerse en contacto con el soporte técnico, pero no para la reconciliación. |
|OrderDate |Fecha de realización del pedido. |
|ProductId |Identificador del producto. |
|SkuId  |Id. de un SKU concreto. |
|AvailabilityId |Id. de una disponibilidad concreta. "Disponibilidad" hace referencia a si un SKU concreto está o no disponible para su compra para el país, la moneda, el segmento industrial determinados, etc. |
|SkuName  |Título para un SKU concreto. |
|ProductName |Nombre del producto. |
|ChargeType |Tipo de cargo o ajuste. |
|UnitPrice |Precio por producto pedido. |
|Cantidad |Número de productos pedidos. |
|Subtotal |Total sin impuestos. Comprueba que el subtotal coincide con el total previsto, en el caso de un descuento. |
|TaxTotal |Total de todos los impuestos aplicables. |
|Total |Número total de esta compra. |
|Moneda |Tipo de moneda. Cada entidad de facturación tiene una sola moneda. Comprueba que coincide con la primera factura y repite la comprobación tras cualquier actualización importante de la plataforma de facturación. |
|DiscountDetails |Lista detallada de los descuentos relevantes. |


## <a name="manage-your-billing"></a>Administrar tu facturación

### <a name="view-your-current-billing-status-invoices-and-recon-files"></a>Ver el estado actual de facturación, facturas y archivos de conciliación

1.  En el centro de partners, seleccione **facturación** y, a continuación, **una vez** para ver el estado de facturación. 
2.  Selecciona una factura o un archivo de conciliación para ver información más detallada. 

### <a name="view-a-customers-order-history"></a>Ver el historial de pedidos de un cliente

1.  Seleccione **clientes** en el menú del centro de partners.
2.  En tu página **Clientes**, busca el cliente cuyo historial de pedidos quieres ver y, a continuación, selecciona la flecha abajo para expandir el registro del cliente. 
3.  Selecciona **Ver pedidos** para mostrar el historial de pedidos.

### <a name="create-a-credit-or-void-note"></a>Crear una nota nula o de crédito

En algún momento es posible que debas anular una factura y, a continuación, emitir una nueva. Por ejemplo, un cliente puede cambiar el nombre de su negocio y, a continuación, recibir una factura con el nombre anterior. 

Para anular una factura y que se emita una nueva, descargar el formulario en la página de facturación en ajustes.

## <a name="azure-reservations-resources"></a>Recursos de Azure Reservations
|**Para obtener información acerca de**   |**Lea este**    |
|:-----------------------------|:-----------------|
|Reservas de Azure en la introducción del CSP  | [Vende instancias reservadas de VM de Azure de Microsoft](azure-reservations.md)
|Compra de reservas de Azure para sus clientes en el centro de partners   |[Comprar reservas de Azure](azure-reservations-buying.md)
| Administración de las reservas de Azure en el centro de partners | [Administración de las reservas de Azure en el centro de partners](azure-reservations-manage.md)
|Compra de reservas de Azure en Azure Portal | [Pagar por adelantado máquinas virtuales con instancias reservadas de máquina virtual](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances) en la Ayuda de Azure |
|Administración de Azure Reservations en el Azure Portal   |[Administración de instancias reservadas de máquina virtual](https://docs.microsoft.com/azure/billing/billing-manage-reserved-vm-instance) en la Ayuda de Azure  |
|Compra de reservas de Azure usando la API del Centro de partners | [Purchase Azure Reserved VM Instances (Comprar Azure Reserved VM Instances)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) en la documentación de desarrolladores del Centro de partners

 
