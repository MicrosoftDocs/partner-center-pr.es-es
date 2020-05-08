---
title: Diferencias de facturación mensuales y anuales
ms.topic: article
ms.date: 05/06/2020
Description: Vea cómo la facturación mensual y anual difiere en el centro de Partners. También aprenderá a cambiar entre diferentes tipos de facturación y las implicaciones del cambio.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 841e7026651484b4b3c52ecc1e3c297af01f9f16
ms.sourcegitcommit: e9b627159745bcce53a8c2b1676f63f5249bba76
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/07/2020
ms.locfileid: "82908253"
---
# <a name="understand-the-difference-between-monthly-and-annual-billing-in-partner-center"></a>Comprenda la diferencia entre la facturación mensual y anual del centro de Partners


**Se aplica a**

- Centro de partners
- Centro de partners para Microsoft Cloud for US Government

**Roles adecuados**

- Agente de administrador
- Administrador de facturación
- Administrador global
- Administrador de incentivos
- Usuario de incentivos
- Agente del departamento de soporte técnico
- Agente de ventas

En este tema se explican las diferencias entre la **facturación mensual** y la **facturación anual** del centro de Partners, incluidas las ventajas y los casos de uso. Tiene la opción de pagar algunas suscripciones de proveedor de soluciones en la nube (CSP) mensual o anual.

## <a name="applicability"></a>Aplicabilidad

La mayoría de las suscripciones basadas en licencia tienen la opción de facturación mensual o anual. Las suscripciones basadas en uso solo tienen la opción de facturación mensual.

La facturación anual y mensual son **por suscripción**, ** *no* por licencia**.

### <a name="find-subscription-applicability"></a>Buscar aplicabilidad de suscripción

Puede identificar las frecuencias de facturación disponibles para cada oferta mediante el uso de la columna J en la matriz de la oferta. Puede encontrar la matriz de la oferta en la sección **Ver ofertas y precios** del centro de Partners.

### <a name="applicable-partners"></a>Asociados correspondientes

Todos los asociados y tipos de socios comerciales pueden elegir la facturación mensual o anual.

### <a name="applicable-markets"></a>Mercados aplicables

La facturación mensual y anual (para las ofertas correspondientes) está disponible en todos los mercados en los que el programa CSP está disponible actualmente.

## <a name="change-billing-frequency"></a>Cambio de la frecuencia de facturación

Puede cambiar entre facturación mensual y anual en cualquier momento. Puede que desee cambiar la frecuencia de facturación si cambian las necesidades de su empresa.

Cuando se cambia la frecuencia de facturación a anual, el término anual se actualiza para reflejar la fecha en que se cambió la frecuencia de facturación. También se establece una nueva fecha de renovación.

### <a name="monthly-to-annual-billing"></a>Facturación mensual

Cambiar de facturación mensual a facturación anual puede ser útil si tiene varias suscripciones que se facturan mensualmente. Al cambiar a la facturación anual, puede alinear las suscripciones con una fecha de facturación común.

### <a name="annual-to-monthly-billing"></a>Facturación anual a factura mensual

Cambiar de la facturación anual a la facturación mensual puede ser útil si desea ajustar las fechas de facturación a las de sus clientes individuales.

## <a name="annual-billing"></a>Facturación anual

La facturación anual tiene las siguientes ventajas:

- Una mayor flexibilidad en opciones de pago.
- Una mejor alineación con la facturación de tus clientes.
- Menor impacto de las fluctuaciones de moneda.
- Menores costos operativos de facturación.

### <a name="configure-annual-billing"></a>Configuración de la facturación anual

Si tiene previsto cambiar a la facturación anual del centro de Partners, asegúrese de considerar cómo se verá afectado el movimiento de ventas. Informe al equipo y actualice los procesos internos según sea necesario. También debe revisar los cambios en la factura y el archivo de conciliación basado en licencias. 

También necesitará [actualizar las API para la facturación anual](#required-api-changes).

#### <a name="required-api-changes"></a>Cambios necesarios de la API

Para poder aprovechar la facturación anual, deberá realizar algunos cambios en las API.

- [Propiedad order. BillingCycle](https://docs.microsoft.com/dotnet/api/microsoft.store.partnercenter.models.orders.order.billingcycle)
- [Crear un pedido](https://docs.microsoft.com/partner-center/develop/create-an-order)

Para obtener más información sobre las API del centro de Partners, consulte todos los [recursos y documentación para desarrolladores del centro de Partners](https://docs.microsoft.com/partner-center/develop/).

## <a name="placing-orders"></a>Realización de pedidos

El tipo de frecuencia de facturación, incluida la facturación anual, se asigna a la **oferta** como un atributo. No hay una oferta única para pedidos con facturación anual. Sin embargo, puede cambiar el nombre de una oferta con un nombre más descriptivo para diferenciar fácilmente.

### <a name="select-annual-billing"></a>Seleccionar facturación anual

Cuando agregue una nueva suscripción, se le pedirá que elija la frecuencia de facturación. Puedes elegir la opción de facturación anual en este momento. Al seleccionar la facturación anual, se mostrarán todas las ofertas disponibles.

### <a name="billing-time"></a>Tiempo de facturación

Se le facturará en la siguiente fecha de facturación. Por ejemplo, si la fecha de facturación es el día 1 del mes y compra una suscripción facturada anualmente el 29 de octubre de 2019, se le facturará el 1 de noviembre de 2019. Suponiendo que no realiza ningún cambio en la licencia, se le facturará de nuevo el 1 de noviembre de 2020. Si realiza un cambio de licencia, recibirá un crédito y se le refacturará en la siguiente fecha de facturación.

### <a name="annual-renewals"></a>Renovaciones anuales

La fecha de renovación de la suscripción será de 12 meses después de la fecha de inicio del servicio. El período de servicio comienza en la fecha en que se crea la suscripción.  Por ejemplo, una suscripción creada el 10 de enero de 2019, se renovará el 10 de enero de 2020.

Se te enviará una factura en la siguiente fecha de facturación después de la fecha de renovación de la suscripción. Por ejemplo, si compras una suscripción con facturación anual el 15 de enero de 2018 y la fecha de facturación es el 20 de enero, tu suscripción se renovará en 15 de enero de 2019. La renovación se te facturará entonces el 20 de enero de 2019.

### <a name="split-subscription-billing-frequency"></a>Frecuencia de facturación de suscripción dividida

No es posible dividir una **sola suscripción** para que una parte se facture mensualmente y la otra parte se facture anualmente. Toda la suscripción debe tener la misma frecuencia de facturación (facturación mensual o anual).

En el caso de los clientes con **varias suscripciones** de la misma oferta, puede que sea posible tener diferentes frecuencias de facturación por suscripción. Hay algunas ofertas que están limitadas a una suscripción por cliente. Si la oferta no está limitada, un cliente puede tener varias suscripciones de la misma oferta con diferentes frecuencias de facturación. Puedes encontrar los detalles de todos los límites y restricciones de las ofertas en la columna I de la matriz de ofertas. Puede encontrar la matriz de la oferta en la sección **Ver ofertas y precios** del centro de Partners.

### <a name="free-subscription-period"></a>Período de suscripción gratuito

Las suscripciones con una frecuencia de facturación anual no reciben un período gratuito. El plazo de pago de doce meses comienza en la fecha de compra. Difiere de las suscripciones con frecuencia de facturación mensual que reciben un período gratuito desde la fecha de compra hasta la próxima fecha de facturación.

### <a name="adding-and-removing-licenses"></a>Adición y eliminación de licencias

Puedes cambiar la cantidad de licencias de tus suscripciones en cualquier momento. Agregar licencias adicionales no afectará a la frecuencia de facturación.

Puedes agregar o quitar licencias en cualquier momento.  Recibirá un crédito y una factura prorrateada en la siguiente fecha de facturación después de cambiar el número de licencias.

Si la suscripción existente tiene una facturación anual, no es posible agregar licencias con facturación mensual a esa suscripción. Cuando adquieres una suscripción con facturación anual, cualquier licencia adicional seguirá la misma frecuencia de facturación. Si necesitas después adquirir licencias con facturación mensual, tendrás que adquirir una nueva suscripción.

### <a name="add-on-offers"></a>Ofertas de complementos

La suscripción a complementos tendrá automáticamente la misma frecuencia de facturación que la suscripción principal. La facturación anual está disponible para las ofertas de complementos. 

### <a name="cancelling-subscriptions"></a>Cancelar suscripciones

La directiva de cancelación es la misma para todas las frecuencias de facturación.

En el caso de la facturación anual, si la suscripción se cancela en los 30 primeros días del plazo de pago de doce meses, recibirá un crédito del 100 por ciento en la siguiente fecha de facturación. Si se cancela la suscripción después de 30 días del plazo de pago de doce meses, recibirá un crédito prorrateado en la siguiente fecha de facturación.

### <a name="moving-subscriptions-between-partners"></a>Mover suscripciones entre asociados

Los clientes no pueden trasladar las suscripciones entre de un asociado a otro. Esto se aplica a las suscripciones facturadas mensualmente y anualmente.

El nuevo partner debe adquirir una nueva suscripción en nombre del cliente. No es posible trasladar suscripciones entre asociados.

### <a name="reactivating-subscriptions"></a>Reactivación de suscripciones

Puede reactivar una suscripción durante un máximo de 90 días después de la fecha de suspensión. Recibirás un cargo prorrateado en la siguiente fecha de facturación. La fecha de renovación de la suscripción permanece igual.

## <a name="pricing"></a>Precios

### <a name="offer-pricing"></a>Precios de la oferta

El precio de la oferta en el momento de la compra se garantiza para el período de suscripción facturado completo (un mes para la facturación mensual, 12 meses para la facturación anual). Cuando se renueve una suscripción, el precio se basará en la lista de precios actual en la fecha de renovación. El nuevo precio se garantiza para el siguiente período de suscripción.

Si se reduce el precio de la oferta durante el período de facturación, la cantidad que se factura no cambia. El precio se establece para el período de facturación completo en el momento de la compra. Esto se aplica a la facturación mensual y anual.

### <a name="cancellation-credits"></a>Créditos de cancelación

El crédito para una licencia cancelada o una suscripción se calcula de la siguiente manera:

**Crédito de cancelación** = ((* * precio mensual * * * * 12)/ \* 365) **días restantes en el período** \* de doce meses de licencias canceladas.

## <a name="reconciliation-file"></a>Archivo de conciliación

### <a name="find-subscriptions-billing-frequency"></a>Buscar la frecuencia de facturación de la suscripción

La columna **AA** del archivo de conciliación le indicará si su suscripción se factura mensualmente o anualmente.

Para averiguar si puede cambiar una suscripción mensual a facturación anual, consulte [Find subscription aplicabilidad](#find-subscription-applicability).

### <a name="reconciliation-file-changes-for-annual-billing"></a>Cambios en el archivo de conciliación para la facturación anual

Al comprar o renovar una suscripción con una facturación anual, el archivo de conciliación basado en licencias cambiará como se indica a continuación:

- Habrá una nueva fila en el archivo de conciliación basada en licencias en la primera fecha de facturación después de la compra o de una nueva suscripción.

- Si no se realizan cambios en la suscripción, no habrá filas en los archivos de conciliación de los meses dos a 12 del período de suscripción. Si se realiza un cambio en la suscripción durante el período de doce meses, aparecerá un crédito y una factura prorrateada en el siguiente archivo de conciliación después de realizar el cambio.

- El siguiente cambio en el archivo de conciliación aparecerá cuando se renueve la suscripción. Esto aparecerá en la primera fecha de facturación después de la renovación.

### <a name="usage-file-changes-for-annual-billing"></a>Cambios en el archivo de uso para la facturación anual

Los siguientes cambios de suscripción facturados anualmente aparecen en la columna P del archivo de uso:

- **Tarifas de prorrateo al comprar**: la compra inicial de una suscripción anual.
- **Protasa de instancia de ciclo**: cambios de licencia que dan como resultado un crédito y una refacturación.
- **Cancelar cuota**: [cancelación de una suscripción anual](#cancellation-of-annual-subscription).

### <a name="cancellation-of-annual-subscription"></a>Cancelación de la suscripción anual

Cuando se cancela una suscripción facturada anualmente, el archivo de conciliación contendrá un elemento de línea para un crédito de cancelación.

Si se produce la cancelación en los primeros 30 días del período de doce meses, la suscripción se abonará en el 100 por ciento. Si la cancelación se produce después de los primeros 30 días, la suscripción será abonada de forma prorrateada.

### <a name="adding-licenses-to-annual-subscription"></a>Agregar licencias a la suscripción anual

Al agregar licencias a una suscripción, el archivo de conciliación contendrá un crédito y una factura prorrateada. Esto se aplica a las suscripciones facturadas mensualmente y anualmente.

### <a name="price-lists-for-annual-billing"></a>Listas de precios para la facturación anual

Las listas de precios del centro de Partners muestran los precios mensuales. No se muestra ningún precio anual. Puede calcular el precio anual multiplicando el precio mensual por 12.

### <a name="offer-matrix"></a>Matriz de la oferta

Los identificadores de oferta de la matriz de la oferta son los mismos para todas las frecuencias de facturación. No hay identificadores únicos para las ofertas que se pueden facturar anualmente.

## <a name="incentives"></a>Incentivos

### <a name="incentives-calculation"></a>Cálculo de incentivos

Los incentivos se calculan en función de los **ingresos facturados**, ** *no* **de los ingresos. Los pagos de los incentivos ganados serán acordes con nuestra directiva que se encuentran en nuestras guías de incentivos de CSP.

Cuando se vende una suscripción facturada anualmente, se reconocen los ingresos de la suscripción para el cálculo de los incentivos en función de los ingresos facturados.

### <a name="payout"></a>Pago

Actualmente, todos los pagos de incentivos se realizan dos veces al año. Los pagos se realizan 45 días después del final de cada semestre.

### <a name="rates"></a>Tarifas

Los asociados obtienen incentivos en todas las transacciones válidas, independientemente de cómo se facture una suscripción. Los beneficios de incentivos se calculan en función de la tasa de estímulo global (que se aplica a los ingresos facturados durante el período), el acelerador local (para todas las zonas geográficas en las que hay aceleradores locales) y cualquier campaña global (si procede).

### <a name="contacts"></a>Contactos

Si tiene preguntas sobre los incentivos, póngase en contacto con el equipo de soporte técnico de incentivos regionales adecuado:

| Region | Dirección de correo electrónico |
| ------ | ------------- |
| Norteamérica | <ocina@microsoft.com> |
|América Latina & Brasil | <ocilatam@microsoft.com> |
| EMEA | <ociemea@microsoft.com> |
| APOAC (excepto Japón) | <ociapgc@microsoft.com> |
| Japón | <ocijp@microsoft.com> |


### <a name="suspension"></a>Suspensivo

Si suspende una suscripción (en el centro de Partners o a través de las API) en un plazo de 30 días a partir de la compra, recibirá un crédito del 100%, independientemente de la frecuencia de facturación.

Para la facturación anual:

1. El socio compra la suscripción el 1 de enero. Se crea una línea de facturación de cargos para el período de servicio del 1 de enero al 31 de diciembre.
2. El socio suspende la suscripción el 25 de enero. Se crea una línea de facturación de crédito para el período de servicio del 1 de enero al 31 de diciembre.
3. El asociado vuelve a activar la suscripción el 29 de enero. Se crea una línea de facturación de cargos para el período de servicio del 29 de enero al 31 de diciembre.

Para facturación mensual:

1. El socio compra la suscripción el 1 de enero. Se crea una línea de facturación de cargos para el período de servicio del 1 de enero al 31 de enero.
2. El socio suspende la suscripción el 25 de enero. Se crea una línea de facturación de crédito para el período de servicio del 1 de enero al 31 de enero.
3. El asociado vuelve a activar la suscripción el 29 de enero. Se crea una línea de facturación de cargos para el período de servicio del 29 de enero al 31 de enero.
