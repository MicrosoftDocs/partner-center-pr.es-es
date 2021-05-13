---
title: Cómo afectan las directivas fiscales al pago de Azure Marketplace
description: Obtenga información sobre cómo afectan las directivas fiscales al pago de Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: a93e94912f840e4cb69c3cc834f03af1b34f19aa
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856022"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a>Cómo afectan las directivas fiscales al pago de Azure Marketplace

**Roles adecuados:** Administrador global | Administrador de administración de | Agente de administración

## <a name="introduction"></a>Introducción

El marketplace comercial de Microsoft tiene alcance global. Las transacciones se producen a través de fronteras y, en función de dónde se encuentran el ISV y el cliente, las implicaciones fiscales pueden variar. Microsoft AppSource y Azure Marketplace usar la Centro de partners del perfil fiscal para determinar el país del ISV. Para determinar el país del cliente, use la información de facturación del cliente o, si el cliente está en la UE, usamos dos datos diferentes.

Para comprender mejor los escenarios [](tax-details-marketplace.md) siguientes, consulte la tabla Detalles fiscales, que muestra si Microsoft cobra y paga impuestos en nombre del publicador o si esa responsabilidad pertenece al publicador.

> [!NOTE]
> Todos los ejemplos de valores de venta y porcentajes fiscales de este tema son solo con fines ilustrativos, no con cifras exactas.

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a>Transacciones del publicador en el país fiscal administrado por Microsoft

**Escenario A:** transacciones que tienen lugar entre un publicador y un cliente en un país fiscal [administrado por Microsoft.](tax-details-marketplace.md#microsoft-managed-countries) Estas transacciones tendrán impuestos aplicables agregados en el momento de la venta y Microsoft envía ese impuesto al país aplicable. No se retiene ningún impuesto del pago y los cálculos de pago son exclusivos de impuestos.

Consulte [escenario D para](#foreign-publisher-transacts-with-us-customer) las transacciones entre un publicador que no es de EE. UU. y un cliente de EE. UU.

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a>Transacciones del publicador en un país fiscal administrado por Microsoft en el que el precio de Marketplace es un servicio imponible

**Escenario B:** transacciones que tienen lugar entre un publicador basado en Estados Unidos (tal y como se define en su información de perfil fiscal de Centro de partners) a un cliente en un país fiscal administrado por Microsoft donde el país impone un impuesto sobre la cuota de Marketplace (un servicio imponible). En este escenario, el impuesto sobre la tarifa del servicio de tienda se resta del pago del anunciante.

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Muestra el flujo de trabajo del escenario B del proceso de pago.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a>Transacciones del publicador en el país fiscal administrado por el publicador

**Escenario C:** transacciones que tienen lugar entre un publicador y un cliente en un país fiscal administrado por el publicador que no impone una retención de impuestos a los clientes. Los clientes no pagan ningún impuesto en el momento de la venta y es obligación del anunciante pagar todos los impuestos aplicables.

Para obtener más información sobre los precios específicos del país (por ejemplo, para compensar los próximos impuestos), consulte Planes y precios de ofertas [de marketplace comercial.](/azure/marketplace/plans-pricing#custom-prices)

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a>Transacciones del publicador externo con el cliente de EE. UU.

**Escenario D:** todos los anunciantes externos (tal y como se define en su información de perfil fiscal de Centro de partners) en países sin permiso de Estados Unidos (consulte el escenario [E)](#foreign-publisher-with-a-treaty-transacts-with-us-customer)que realiza una venta a un cliente basado en Estados Unidos (tal y como se define en su dirección de cuenta de cliente). El gobierno de EE. UU. requiere que Microsoft retenga los impuestos en nombre del anunciante. Los impuestos que se retienen del pago al publicador se calculan en función del precio de la oferta.

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Muestra el flujo de trabajo para el escenario D del proceso de pago.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a>Publicador externo con una transacción de transacción con un cliente de EE. UU.

**Escenario E:** todos los anunciantes externos (tal y como se define por su información de perfil fiscal de Centro de partners) en países con un tratado de Ee. UU. que realiza una venta a un cliente basado en Estados Unidos (tal y como se define en su dirección de cuenta de cliente). El gobierno de EE. UU. no requiere que Microsoft retenga los impuestos en nombre del anunciante.

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a>Un anunciante externo vende a un cliente registrado en el IVA de la UE en un país administrado por Microsoft (fuera de Irlanda)

**Escenario F:** todas las transacciones entre editores externos y clientes registrados en el IVA de la UE (fuera de Irlanda) en un Microsoft-Managed país. El cliente no paga impuestos por la venta.

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a>El anunciante externo vende a un cliente registrado en el IVA de la UE en un país administrado por Microsoft (en Irlanda)

**Escenario G:** todas las transacciones entre anunciantes externos y clientes registrados en el IVA de la UE (dentro de Irlanda) en un Microsoft-Managed país. El cliente paga el IVA de la caja y Microsoft paga este impuesto al gobierno de Irlanda.

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Muestra el flujo de trabajo para el escenario G del proceso de pago.":::

## <a name="next-steps"></a>Pasos siguientes

- [Preguntas más frecuentes sobre el publicador](/azure/marketplace/marketplace-faq-publisher-guide)
- [Instrucciones para crear perfiles fiscales y de pago](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)