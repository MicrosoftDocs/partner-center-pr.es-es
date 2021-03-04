---
title: Cómo afectan las directivas de impuestos al pago de Azure Marketplace
description: Obtenga información sobre cómo las directivas de impuestos afectan al pago de Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 3630824c839ccd9f54f3e8e5199a573b5824bb91
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/03/2021
ms.locfileid: "101758544"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Cómo afectan las directivas de impuestos al pago de Azure Marketplace

**Roles adecuados**
-    Administrador global
-    Administrador de usuarios
-    Agente de administrador

## <a name="introduction"></a>Introducción

Microsoft Commercial Marketplace tiene alcance global. Las transacciones se producen entre los bordes y, en función de dónde se encuentre el ISV y el cliente, las implicaciones fiscales pueden variar. Microsoft AppSource y Azure Marketplace usan la información del perfil fiscal del centro de partners para determinar el país del ISV. Para determinar el país del cliente, use la información de facturación del cliente o, si el cliente está en la UE, usamos dos fragmentos de información diferentes.

Para comprender mejor los escenarios siguientes, consulte la tabla de [detalles de impuestos](tax-details-marketplace.md) , que muestra si Microsoft recopila y paga impuestos en nombre del publicador o si esa responsabilidad pertenece al publicador.

> [!NOTE]
> Todos los ejemplos de ventas y los porcentajes de impuestos de este tema son solo para fines ilustrativos, no figuras exactas.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>El publicador se comporta en el país de impuestos administrado por Microsoft

**Escenario A** : transacciones que tienen lugar entre un publicador y un cliente en un [país de impuestos administrado por Microsoft](tax-details-marketplace.md#microsoft-managed-countries). Estas transacciones tendrán impuestos aplicables en el momento de la venta y Microsoft enviará dicho impuesto al país correspondiente. No se retiene ningún impuesto del pago y los cálculos de pago son impuestos exclusivos.

Vea el [escenario D](#foreign-publisher-transacts-with-us-customer) para las transacciones entre un publicador que no es de Estados Unidos y un cliente de EE. UU.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>El publicador actúa en el país de impuestos administrado por Microsoft, donde la cuota de Marketplace es servicio gravable

**Escenario B** : las transacciones que tienen lugar entre un publicador basado en Estados Unidos (según se define en la información del perfil fiscal del centro de Partners) a un cliente en un país de impuestos administrado por Microsoft en el que el país impone un impuesto sobre la cuota de Marketplace (un servicio gravable). En este escenario, el impuesto sobre la cuota de servicio de la tienda se resta del pago del anunciante.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>El publicador actúa en el país de impuestos administrado por el publicador

**Escenario C** : las transacciones que tienen lugar entre un publicador y un cliente en un país de impuestos administrado por el publicador que no impone un impuesto de retención a los clientes. Los clientes no pagan ningún impuesto en el punto de venta y es la obligación del anunciante de pagar todos los impuestos aplicables.

Para obtener más información sobre los precios específicos de cada país (por ejemplo, para desplazar la siguiente tributación), consulte [planes y precios de ofertas comerciales de Marketplace](https://docs.microsoft.com/azure/marketplace/plans-pricing#custom-prices).

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>El publicador externo se comporta con el cliente de EE. UU.

**Escenario D** : todos los publicadores externos (según se define en la información del perfil fiscal del centro de Partners) en países sin un tratado estadounidense (vea el [escenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) que realizan una venta a un cliente basado en Estados Unidos (según se define en la dirección de su cuenta de cliente). El gobierno de EE. UU. requiere la retención de impuestos de Microsoft en nombre del publicador. Los impuestos retenidos del pago al publicador se calculan en función del precio de la oferta.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Publicador externo con un tratado que se comporta con el cliente de EE. UU.

**Escenario E** : todos los publicadores externos (según se define en la información del perfil fiscal del centro de Partners) en países con un Tratado de EE. UU. que realizan una venta a un cliente basado en EE. UU. (según se define en la dirección de su cuenta de cliente). El gobierno de EE. UU. no requiere que Microsoft retenga impuestos en nombre del publicador.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>El publicador externo vende a un cliente de IVA registrado de la UE en un país administrado por Microsoft (fuera de Irlanda)

**Escenario F** : todas las transacciones entre publicadores externos y clientes registrados en el IVA de la UE (fuera de Irlanda) en un Microsoft-Managed país. El cliente no paga impuestos sobre la venta.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>El publicador externo vende a un cliente de IVA registrado de la UE en un país administrado por Microsoft (en Irlanda)

**Escenario G** : todas las transacciones entre publicadores externos y clientes registrados en el IVA de la UE (dentro de Irlanda) en un Microsoft-Managed país. El cliente paga el IVA irlandés y Microsoft paga este impuesto al Gobierno irlandés.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago G.":::

## <a name="next-steps"></a>Pasos siguientes

- [Preguntas más frecuentes del publicador](https://docs.microsoft.com/azure/marketplace/marketplace-faq-publisher-guide)
- [Instrucciones para crear perfiles de pago y de impuestos](https://docs.microsoft.com/partner-center/set-up-your-payout-account?context=/azure/marketplace/context/context#create-a-payment-profile)
