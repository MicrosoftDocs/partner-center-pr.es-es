---
title: 'Facturación del plan de Azure: facturas y archivos de conciliación'
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprende a obtener acceso y a comprender la estructura del archivo de conciliación y facturación relacionado con la facturación del plan de Azure.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: c7c06f5ed7b147625afb5020f63ead411ef58fa8
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551527"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nueva experiencia comercial en CSP: facturación de Azure 

**Roles adecuados**: Agente de administración | Administrador de facturación | Administrador global

En este artículo se describe cómo acceder a la estructura del archivo de conciliación y facturación relacionado con la facturación del plan de Azure, así cómo comprenderla. La facturación del plan Azure es una experiencia de facturación simplificada que usa una fecha de facturación única alineada y un período de facturación basado en los meses del calendario.

## <a name="summary-of-billing-essentials"></a>Resumen de los elementos esenciales de la facturación

- **Fecha de facturación**: La factura y el archivo de conciliación estarán disponibles en el panel o API del Centro de partners antes del día 8 (medianoche, UTC).

- **Período de facturación**: El período de facturación de la factura coincidirá con el mes natural; por ejemplo, 10/1-10/31, 11/1-11/30.

- **Períodos del servicio de cargos**: Los cargos coincidirán con el mes natural. Por ejemplo, si el partner facturado agrega servicios de Azure a través de un plan de Azure el 15/10 y el cliente comienza a consumir los servicios de Azure el mismo 15/10, el partner facturado recibirá la factura o la conciliación el 8/11 referente al consumo del cliente durante el período de servicio del 15/10 al 31/10. La factura del próximo mes que se generará el 8/12 y contendrá todos los cargos del período de servicio del 1/11 al 11/31.

- **Plazo de pago de la factura**: Neto, 60 días.

- **Moneda de la factura** : A partir del 28 de enero de 2021, se facturará a los partners de la región de la UE/AELC y el Reino Unido que tengan nuevos clientes y clientes de CSP existentes que adquieran nuevas ofertas de comercio por primera vez y cuyos inquilinos se hayan creado antes del 11 de mayo de 2020 por esas compras en la moneda de la ubicación del partner. A los partners situados fuera de la región de la UE/AELC y el Reino Unido se les seguirá facturando en la moneda de la ubicación del partner.

- **Incentivos de partners**: Pagado a 45 días desde el final del mes de la factura.

## <a name="access-your-invoices-and-reconciliation-files"></a>Acceder a las facturas y los archivos de conciliación

El administrador global o el administrador de facturación de tu empresa recibirá un correo electrónico cuando una factura esté lista para ver.

Para acceder a la factura y al archivo de conciliación:

1. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard/) del Centro de partners.

2. En el menú del Centro de partners, selecciona **Billing** (Facturación).

3. Selecciona la pestaña de **Periódico** y **Una vez** y la moneda que te interese.

   :::image type="content" source="images/azure/billing3.png" alt-text="Facturación.":::

4. Selecciona **Factura** o **Archivo de conciliación**.  

   Para ver las facturas históricas y los archivos de conciliación, amplía la fila del historial de facturación a continuación.

## <a name="understanding-usage-data"></a>Explicación de los datos de uso 

1. El plan de Azure es el contenedor raíz o de nivel superior para el uso. Todo el uso está vinculado a un único plan de Azure.

2. En un plan, habrá una o varias suscripciones de Azure. Estos son los contenedores que se usan para la implementación y la administración de recursos. 

3. En una suscripción, los grupos de recursos se agregan a recursos de grupo. Cada recurso se implementa en un grupo de recursos. 

4. Entre los ejemplos de recursos se incluyen las máquinas virtuales y las cuentas de almacenamiento. 

5. Los recursos emiten medidores: Los medidores son medidas de consumo de un recurso, y un recurso puede emitir el uso de varios medidores. Los medidores se identifican mediante ProductId, SKUId y AvailabilityId. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Jerarquía de grupos de recursos de suscripción y medición

**Cuenta de Azure (inquilino)**

- Suscripción A
    - ResourceGroup 1
        - Máquina virtual (recurso)
            - Medidor de proceso
        - Virtual Network (recurso)
            - Sin medidor de facturación

    - ResourceGroup 2
        - Máquina virtual (recurso)
            - Medidor de proceso
        - Disco administrado SSD Premium (recurso)
            - Medidor de capacidad de almacenamiento
            - Medidor de operaciones de almacenamiento

- Suscripción B   -ResourceGroup 1       - Azure SQL (recurso)           - Medidor de DTU       - VPN Gateway (recurso)           - Medidor de VPN Gateway

    - ResourceGroup 2
        - Interfaz de Virtual Network (recurso)
            - Sin medidor de facturación

## <a name="read-the-invoice"></a>Leer la factura

1. La factura estará disponible el día ocho de cada mes a más tardar.

2. Los partners tienen 60 días para remitir el pago.

3. El período de facturación cubrirá un mes dado del calendario; por ejemplo del 1/10 al 31/10.

4. Los cargos son netos en cuanto a los ajustes (el importe es el valor neto del "crédito obtenido del partner por los servicios administrados").

5. Revisa el archivo de conciliación de facturas y el archivo de uso con clasificación diaria para obtener los detalles adicionales de facturación.

   :::image type="content" source="images/azure/invoice1.png" alt-text="Factura.":::

## <a name="read-the-invoice-reconciliation-file"></a>Lectura del archivo de conciliación de facturas

1. Cada combinación de medidor y plan de Azure puede tener hasta dos líneas de facturación en el archivo de conciliación.

2. Si el medidor puede tener en cuenta cualquier tipo de descuento o crédito (como los descuentos por nivel o el crédito obtenido del partner por los servicios administrados) durante todo el mes natural, el archivo de conciliación solo contendrá una línea de facturación. La columna **PriceAdjusmentDescription** hará referencia al descuento o al crédito obtenido.

3. Si no existen recursos para un medidor concreto que es apto para el descuento o el crédito obtenido del partner, el archivo de conciliación solo contendrá una línea de facturación y el precio por unidad vigente será el precio de venta al por menor (que es el precio por unidad).

4. Si el medidor (o cualquier recurso que este emita) es apto para el **crédito obtenido del partner para los servicios administrados** durante una parte del mes, el archivo de conciliación contendrá dos líneas de facturación. Una línea representará los días que el medidor haya calificado y la segunda línea representará los días que el medidor no calificó.

>[!NOTE]
>Puede conciliar el consumo de Azure en el archivo de conciliación de una sola compra. Para ello, vaya al archivo de conciliación de uso clasificado diariamente y busque su subscriptionID. Se mostrarán todos los costos asociados con su identificador del plan de Azure. Su SubscriptionID de Azure se muestra como EntitlementID.

## <a name="read-the-daily-usage-file"></a>Leer el archivo de uso diario

- Los medidores de suscripción en un plan de Azure se clasifican y se acumulan diariamente.

- **El crédito obtenido del partner por los servicios administrados**  se determina y se aplica diariamente.

- Cada medidor de suscripciones tendrá una fila por cada día del mes en el que se haya consumido.

- Consulta el ejemplo que aparece a continuación:

  - El medidor es apto para el **crédito obtenido del partner por los servicios administrados** del 1/7 al 3/7 (ten en cuenta que el precio unitario efectivo es el precio del minorista menos el crédito obtenido del partner).

  - El medidor no es apto para el **crédito obtenido del partner por los servicios administrados** del 4/7 al 7/7 (ten en cuenta que el precio unitario efectivo es el precio del minorista).

  - El medidor es apto para el **crédito obtenido del partner por los servicios administrados** del 8/7 al 31/7 (ten en cuenta que el precio unitario efectivo es el precio del minorista menos el crédito obtenido del partner).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-customer-currency"></a>Factura en la moneda del cliente

Los servicios de Azure a través de un plan de Azure tendrán un precio de USD y se facturarán en la moneda asignada en el país del cliente. Si la moneda de facturación no es USD, el tipo de cambio usado se mostrará en la última página de la factura. Los tipos de cambio se determinan mensualmente y se aplican a la factura siguiente. Para obtener una lista completa de las monedas de los países, consulta la [matriz de moneda del cliente y la disponibilidad de los países en cuanto a las nuevas ofertas comerciales](https://go.microsoft.com/fwlink/?linkid=2112354).

Microsoft aplica un tipo de cambio predeterminado a los precios en USD base para llegar a los cargos totales en los que se incurre por los servicios de Azure adquiridos o consumidos cada mes natural. El tipo de cambio mensual es el tipo de cambio medio publicado por Thomson Reuters (normalmente) dos días laborables antes del fin de mes anterior a las 16:00 GMT. 

**Por ejemplo,** el tipo de cambio de diciembre de Microsoft sería el tipo de cambio medio de Thomson Reuters el 29 de noviembre o una fecha aproximadamente para una moneda determinada. Dicho tipo se aplicará a todas las compras en esa moneda del 1 al 31 de diciembre. 

## <a name="azure-reservations"></a>Reservas de Azure


Si compra [reservas de Azure](azure-reservations.md) a través de un plan de Azure, puede elegir la facturación única o mensual.


## <a name="azure-spending"></a>Gastos de Azure

La experiencia existente de gasto de Azure se ha actualizado para admitir la nueva facturación del plan de Azure en el Centro de partners. Esto permite a los partners:

- Ver, administrar y recibir alertas del presupuesto establecido en un nivel de cliente. 

- Ver el total de gastos estimados en un plan de Azure (desglosado por nivel de recurso y medidor).

Dado que el modelo de facturación para los servicios de Azure a través de un plan de Azure es el consumo de pago posterior, para evitar recibir una factura más grande de lo previsto, los partners pueden aplicar un presupuesto mensual y realizar un seguimiento del porcentaje de uso. Se puede aplicar un presupuesto a un cliente o a varios clientes al mismo tiempo. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Gastos de Azure.":::

## <a name="next-steps"></a>Pasos siguientes

- Consulte cómo se calcula el crédito que obtiene el partner (PEC). Inicie sesión en el [panel](https://partner.microsoft.com/dashboard/) del Centro de partners y busque la lista de precios disponible.

- Obtenga información sobre la [compra del plan de Azure](purchase-azure-plan.md).

- Consulte la [lista de precios para la nueva experiencia comercial en CSP](azure-plan-price-list.md).
