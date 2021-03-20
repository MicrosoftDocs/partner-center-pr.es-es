---
title: Cómo afectan las directivas de impuestos al pago de Azure Marketplace
description: Obtenga información sobre cómo las directivas de impuestos afectan al pago de Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 19acb085b601212f1bf94316aab2b72c54aecc1a
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712960"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="07b8f-103">Cómo afectan las directivas de impuestos al pago de Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="07b8f-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="07b8f-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="07b8f-104">**Appropriate roles**</span></span>
-    <span data-ttu-id="07b8f-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="07b8f-105">Global admin</span></span>
-    <span data-ttu-id="07b8f-106">Administrador de usuarios</span><span class="sxs-lookup"><span data-stu-id="07b8f-106">User admin</span></span>
-    <span data-ttu-id="07b8f-107">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="07b8f-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="07b8f-108">Introducción</span><span class="sxs-lookup"><span data-stu-id="07b8f-108">Introduction</span></span>

<span data-ttu-id="07b8f-109">Microsoft Commercial Marketplace tiene alcance global.</span><span class="sxs-lookup"><span data-stu-id="07b8f-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="07b8f-110">Las transacciones se producen entre los bordes y, en función de dónde se encuentre el ISV y el cliente, las implicaciones fiscales pueden variar.</span><span class="sxs-lookup"><span data-stu-id="07b8f-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="07b8f-111">Microsoft AppSource y Azure Marketplace usan la información del perfil fiscal del centro de partners para determinar el país del ISV.</span><span class="sxs-lookup"><span data-stu-id="07b8f-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="07b8f-112">Para determinar el país del cliente, use la información de facturación del cliente o, si el cliente está en la UE, usamos dos fragmentos de información diferentes.</span><span class="sxs-lookup"><span data-stu-id="07b8f-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="07b8f-113">Para comprender mejor los escenarios siguientes, consulte la tabla de [detalles de impuestos](tax-details-marketplace.md) , que muestra si Microsoft recopila y paga impuestos en nombre del publicador o si esa responsabilidad pertenece al publicador.</span><span class="sxs-lookup"><span data-stu-id="07b8f-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="07b8f-114">Todos los ejemplos de ventas y los porcentajes de impuestos de este tema son solo para fines ilustrativos, no figuras exactas.</span><span class="sxs-lookup"><span data-stu-id="07b8f-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="07b8f-115">El publicador se comporta en el país de impuestos administrado por Microsoft</span><span class="sxs-lookup"><span data-stu-id="07b8f-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="07b8f-116">**Escenario A** : transacciones que tienen lugar entre un publicador y un cliente en un [país de impuestos administrado por Microsoft](tax-details-marketplace.md#microsoft-managed-countries).</span><span class="sxs-lookup"><span data-stu-id="07b8f-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="07b8f-117">Estas transacciones tendrán impuestos aplicables en el momento de la venta y Microsoft enviará dicho impuesto al país correspondiente.</span><span class="sxs-lookup"><span data-stu-id="07b8f-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="07b8f-118">No se retiene ningún impuesto del pago y los cálculos de pago son impuestos exclusivos.</span><span class="sxs-lookup"><span data-stu-id="07b8f-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="07b8f-119">Vea el [escenario D](#foreign-publisher-transacts-with-us-customer) para las transacciones entre un publicador que no es de Estados Unidos y un cliente de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="07b8f-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="07b8f-121">El publicador actúa en el país de impuestos administrado por Microsoft, donde la cuota de Marketplace es servicio gravable</span><span class="sxs-lookup"><span data-stu-id="07b8f-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="07b8f-122">**Escenario B** : las transacciones que tienen lugar entre un publicador basado en Estados Unidos (según se define en la información del perfil fiscal del centro de Partners) a un cliente en un país de impuestos administrado por Microsoft en el que el país impone un impuesto sobre la cuota de Marketplace (un servicio gravable).</span><span class="sxs-lookup"><span data-stu-id="07b8f-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="07b8f-123">En este escenario, el impuesto sobre la cuota de servicio de la tienda se resta del pago del anunciante.</span><span class="sxs-lookup"><span data-stu-id="07b8f-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago B.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="07b8f-125">El publicador actúa en el país de impuestos administrado por el publicador</span><span class="sxs-lookup"><span data-stu-id="07b8f-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="07b8f-126">**Escenario C** : las transacciones que tienen lugar entre un publicador y un cliente en un país de impuestos administrado por el publicador que no impone un impuesto de retención a los clientes.</span><span class="sxs-lookup"><span data-stu-id="07b8f-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="07b8f-127">Los clientes no pagan ningún impuesto en el punto de venta y es la obligación del anunciante de pagar todos los impuestos aplicables.</span><span class="sxs-lookup"><span data-stu-id="07b8f-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="07b8f-128">Para obtener más información sobre los precios específicos de cada país (por ejemplo, para desplazar la siguiente tributación), consulte [planes y precios de ofertas comerciales de Marketplace](/azure/marketplace/plans-pricing#custom-prices).</span><span class="sxs-lookup"><span data-stu-id="07b8f-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="07b8f-130">El publicador externo se comporta con el cliente de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="07b8f-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="07b8f-131">**Escenario D** : todos los publicadores externos (según se define en la información del perfil fiscal del centro de Partners) en países sin un tratado estadounidense (vea el [escenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) que realizan una venta a un cliente basado en Estados Unidos (según se define en la dirección de su cuenta de cliente).</span><span class="sxs-lookup"><span data-stu-id="07b8f-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="07b8f-132">El gobierno de EE. UU. requiere la retención de impuestos de Microsoft en nombre del publicador.</span><span class="sxs-lookup"><span data-stu-id="07b8f-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="07b8f-133">Los impuestos retenidos del pago al publicador se calculan en función del precio de la oferta.</span><span class="sxs-lookup"><span data-stu-id="07b8f-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago D.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="07b8f-135">Publicador externo con un tratado que se comporta con el cliente de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="07b8f-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="07b8f-136">**Escenario E** : todos los publicadores externos (según se define en la información del perfil fiscal del centro de Partners) en países con un Tratado de EE. UU. que realizan una venta a un cliente basado en EE. UU. (según se define en la dirección de su cuenta de cliente).</span><span class="sxs-lookup"><span data-stu-id="07b8f-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="07b8f-137">El gobierno de EE. UU. no requiere que Microsoft retenga impuestos en nombre del publicador.</span><span class="sxs-lookup"><span data-stu-id="07b8f-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="07b8f-139">El publicador externo vende a un cliente de IVA registrado de la UE en un país administrado por Microsoft (fuera de Irlanda)</span><span class="sxs-lookup"><span data-stu-id="07b8f-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="07b8f-140">**Escenario F** : todas las transacciones entre publicadores externos y clientes registrados en el IVA de la UE (fuera de Irlanda) en un Microsoft-Managed país.</span><span class="sxs-lookup"><span data-stu-id="07b8f-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="07b8f-141">El cliente no paga impuestos sobre la venta.</span><span class="sxs-lookup"><span data-stu-id="07b8f-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="07b8f-143">El publicador externo vende a un cliente de IVA registrado de la UE en un país administrado por Microsoft (en Irlanda)</span><span class="sxs-lookup"><span data-stu-id="07b8f-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="07b8f-144">**Escenario G** : todas las transacciones entre publicadores externos y clientes registrados en el IVA de la UE (dentro de Irlanda) en un Microsoft-Managed país.</span><span class="sxs-lookup"><span data-stu-id="07b8f-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="07b8f-145">El cliente paga el IVA irlandés y Microsoft paga este impuesto al Gobierno irlandés.</span><span class="sxs-lookup"><span data-stu-id="07b8f-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago G.":::

## <a name="next-steps"></a><span data-ttu-id="07b8f-147">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="07b8f-147">Next steps</span></span>

- [<span data-ttu-id="07b8f-148">Preguntas más frecuentes del publicador</span><span class="sxs-lookup"><span data-stu-id="07b8f-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="07b8f-149">Instrucciones para crear perfiles de pago y de impuestos</span><span class="sxs-lookup"><span data-stu-id="07b8f-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)