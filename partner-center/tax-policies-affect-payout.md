---
title: Cómo afectan las directivas fiscales al pago de Azure Marketplace
description: Obtenga información sobre cómo afectan las directivas fiscales al pago Azure Marketplace.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
author: mingshen-ms
ms.author: mingshen
ms.date: 02/09/2021
ms.openlocfilehash: 343db43633245030a5eba213cb5c8b79d09a7dee
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686320"
---
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="ec43e-103">Cómo afectan las directivas fiscales al pago de Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="ec43e-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="ec43e-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="ec43e-104">**Appropriate roles**</span></span>

- <span data-ttu-id="ec43e-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="ec43e-105">Global admin</span></span>
- <span data-ttu-id="ec43e-106">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="ec43e-106">User management admin</span></span>
- <span data-ttu-id="ec43e-107">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="ec43e-107">Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="ec43e-108">Introducción</span><span class="sxs-lookup"><span data-stu-id="ec43e-108">Introduction</span></span>

<span data-ttu-id="ec43e-109">El marketplace comercial de Microsoft tiene alcance global.</span><span class="sxs-lookup"><span data-stu-id="ec43e-109">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="ec43e-110">Las transacciones se producen a través de fronteras y, en función de dónde se encuentran el ISV y el cliente, las implicaciones fiscales pueden variar.</span><span class="sxs-lookup"><span data-stu-id="ec43e-110">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="ec43e-111">Microsoft AppSource y Azure Marketplace usar la Centro de partners del perfil fiscal para determinar el país del ISV.</span><span class="sxs-lookup"><span data-stu-id="ec43e-111">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="ec43e-112">Para determinar el país del cliente, use la información de facturación del cliente o, si el cliente está en la UE, usamos dos datos diferentes.</span><span class="sxs-lookup"><span data-stu-id="ec43e-112">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="ec43e-113">Para comprender mejor los escenarios [](tax-details-marketplace.md) siguientes, consulte la tabla Detalles fiscales, que muestra si Microsoft cobra y paga impuestos en nombre del publicador o si esa responsabilidad pertenece al publicador.</span><span class="sxs-lookup"><span data-stu-id="ec43e-113">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="ec43e-114">Todos los ejemplos de valores de venta y porcentajes fiscales de este tema son solo con fines ilustrativos, no con cifras exactas.</span><span class="sxs-lookup"><span data-stu-id="ec43e-114">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="ec43e-115">Transacciones del publicador en el país fiscal administrado por Microsoft</span><span class="sxs-lookup"><span data-stu-id="ec43e-115">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="ec43e-116">**Escenario A:** transacciones que tienen lugar entre un publicador y un cliente en un país fiscal [administrado por Microsoft.](tax-details-marketplace.md#microsoft-managed-countries)</span><span class="sxs-lookup"><span data-stu-id="ec43e-116">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="ec43e-117">Estas transacciones tendrán impuestos aplicables agregados en el momento de la venta y Microsoft envía ese impuesto al país aplicable.</span><span class="sxs-lookup"><span data-stu-id="ec43e-117">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="ec43e-118">No se retiene ningún impuesto del pago y los cálculos de pago son exclusivos de impuestos.</span><span class="sxs-lookup"><span data-stu-id="ec43e-118">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="ec43e-119">Consulte [escenario D para](#foreign-publisher-transacts-with-us-customer) las transacciones entre un publicador que no es de EE. UU. y un cliente de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="ec43e-119">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="ec43e-121">Transacciones del publicador en un país fiscal administrado por Microsoft en el que el precio de Marketplace es un servicio imponible</span><span class="sxs-lookup"><span data-stu-id="ec43e-121">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="ec43e-122">**Escenario B:** transacciones que tienen lugar entre un publicador basado en Estados Unidos (tal y como se define en su información de perfil fiscal de Centro de partners) a un cliente en un país fiscal administrado por Microsoft donde el país impone un impuesto sobre la cuota de Marketplace (un servicio imponible).</span><span class="sxs-lookup"><span data-stu-id="ec43e-122">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="ec43e-123">En este escenario, el impuesto sobre la tarifa del servicio de tienda se resta del pago del anunciante.</span><span class="sxs-lookup"><span data-stu-id="ec43e-123">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Muestra el flujo de trabajo del escenario B del proceso de pago.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="ec43e-125">Transacciones del publicador en el país fiscal administrado por el publicador</span><span class="sxs-lookup"><span data-stu-id="ec43e-125">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="ec43e-126">**Escenario C:** transacciones que tienen lugar entre un publicador y un cliente en un país fiscal administrado por el publicador que no impone una retención de impuestos a los clientes.</span><span class="sxs-lookup"><span data-stu-id="ec43e-126">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="ec43e-127">Los clientes no pagan ningún impuesto en el momento de la venta y es obligación del anunciante pagar todos los impuestos aplicables.</span><span class="sxs-lookup"><span data-stu-id="ec43e-127">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="ec43e-128">Para obtener más información sobre los precios específicos del país (por ejemplo, para compensar los próximos impuestos), consulte Planes y precios de ofertas [de marketplace comercial.](/azure/marketplace/plans-pricing#custom-prices)</span><span class="sxs-lookup"><span data-stu-id="ec43e-128">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="ec43e-130">Transacciones del publicador externo con el cliente de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="ec43e-130">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="ec43e-131">**Escenario D:** todos los anunciantes externos (tal y como se define en su información de perfil fiscal de Centro de partners) en países sin permiso de Ee. UU. (consulte el escenario [E)](#foreign-publisher-with-a-treaty-transacts-with-us-customer)que realiza una venta a un cliente basado en Estados Unidos (tal y como se define en su dirección de cuenta de cliente).</span><span class="sxs-lookup"><span data-stu-id="ec43e-131">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="ec43e-132">El gobierno de EE. UU. requiere que Microsoft retenga los impuestos en nombre del anunciante.</span><span class="sxs-lookup"><span data-stu-id="ec43e-132">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="ec43e-133">Los impuestos que se retienen del pago al publicador se calculan en función del precio de la oferta.</span><span class="sxs-lookup"><span data-stu-id="ec43e-133">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Muestra el flujo de trabajo para el escenario D del proceso de pago.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="ec43e-135">Publicador externo con una transacción de transacción con un cliente de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="ec43e-135">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="ec43e-136">**Escenario E:** todos los anunciantes externos (tal y como se define por su información de perfil fiscal de Centro de partners) en países con un tratado de Ee. UU. que realiza una venta a un cliente basado en Estados Unidos (tal y como se define en su dirección de cuenta de cliente).</span><span class="sxs-lookup"><span data-stu-id="ec43e-136">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="ec43e-137">El gobierno de EE. UU. no requiere que Microsoft retenga los impuestos en nombre del anunciante.</span><span class="sxs-lookup"><span data-stu-id="ec43e-137">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="ec43e-139">El anunciante externo vende a un cliente registrado en el IVA de la UE en un país administrado por Microsoft (fuera de Irlanda)</span><span class="sxs-lookup"><span data-stu-id="ec43e-139">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="ec43e-140">**Escenario F:** todas las transacciones entre editores externos y clientes registrados en el IVA de la UE (fuera de Irlanda) en un Microsoft-Managed país.</span><span class="sxs-lookup"><span data-stu-id="ec43e-140">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="ec43e-141">El cliente no paga impuestos por la venta.</span><span class="sxs-lookup"><span data-stu-id="ec43e-141">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="ec43e-143">El anunciante externo vende a un cliente registrado en el IVA de la UE en un país administrado por Microsoft (en Irlanda)</span><span class="sxs-lookup"><span data-stu-id="ec43e-143">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="ec43e-144">**Escenario G:** todas las transacciones entre anunciantes externos y clientes registrados en el IVA de la UE (dentro de Irlanda) en un Microsoft-Managed país.</span><span class="sxs-lookup"><span data-stu-id="ec43e-144">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="ec43e-145">El cliente paga el IVA imposiario y Microsoft paga este impuesto al gobierno de Irlanda.</span><span class="sxs-lookup"><span data-stu-id="ec43e-145">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Muestra el flujo de trabajo para el escenario G del proceso de pago.":::

## <a name="next-steps"></a><span data-ttu-id="ec43e-147">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="ec43e-147">Next steps</span></span>

- [<span data-ttu-id="ec43e-148">Preguntas más frecuentes sobre el publicador</span><span class="sxs-lookup"><span data-stu-id="ec43e-148">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="ec43e-149">Instrucciones para crear perfiles fiscales y de pago</span><span class="sxs-lookup"><span data-stu-id="ec43e-149">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)