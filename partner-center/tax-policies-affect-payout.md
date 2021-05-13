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
# <a name="how-tax-policies-affect-payout-for-azure-marketplace"></a><span data-ttu-id="2f34a-103">Cómo afectan las directivas fiscales al pago de Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="2f34a-103">How tax policies affect payout for Azure Marketplace</span></span>

<span data-ttu-id="2f34a-104">**Roles adecuados:** Administrador global | Administrador de administración de | Agente de administración</span><span class="sxs-lookup"><span data-stu-id="2f34a-104">**Appropriate roles**: Global admin | User management admin | Admin agent</span></span>

## <a name="introduction"></a><span data-ttu-id="2f34a-105">Introducción</span><span class="sxs-lookup"><span data-stu-id="2f34a-105">Introduction</span></span>

<span data-ttu-id="2f34a-106">El marketplace comercial de Microsoft tiene alcance global.</span><span class="sxs-lookup"><span data-stu-id="2f34a-106">The Microsoft commercial marketplace has global reach.</span></span> <span data-ttu-id="2f34a-107">Las transacciones se producen a través de fronteras y, en función de dónde se encuentran el ISV y el cliente, las implicaciones fiscales pueden variar.</span><span class="sxs-lookup"><span data-stu-id="2f34a-107">Transactions occur across borders and depending on where the ISV and the customer are located, tax implications can vary.</span></span> <span data-ttu-id="2f34a-108">Microsoft AppSource y Azure Marketplace usar la Centro de partners del perfil fiscal para determinar el país del ISV.</span><span class="sxs-lookup"><span data-stu-id="2f34a-108">Microsoft AppSource and Azure Marketplace use the Partner Center Tax Profile Information to determine the ISV's country.</span></span> <span data-ttu-id="2f34a-109">Para determinar el país del cliente, use la información de facturación del cliente o, si el cliente está en la UE, usamos dos datos diferentes.</span><span class="sxs-lookup"><span data-stu-id="2f34a-109">To determine the customer's country, either use the customer's billing information or, if the customer is in the EU, we use two different pieces of information.</span></span>

<span data-ttu-id="2f34a-110">Para comprender mejor los escenarios [](tax-details-marketplace.md) siguientes, consulte la tabla Detalles fiscales, que muestra si Microsoft cobra y paga impuestos en nombre del publicador o si esa responsabilidad pertenece al publicador.</span><span class="sxs-lookup"><span data-stu-id="2f34a-110">To better understand the following scenarios, refer to the [Tax details](tax-details-marketplace.md) table, which shows whether Microsoft collects and pays taxes on behalf of the publisher or if that responsibility belongs to the publisher.</span></span>

> [!NOTE]
> <span data-ttu-id="2f34a-111">Todos los ejemplos de valores de venta y porcentajes fiscales de este tema son solo con fines ilustrativos, no con cifras exactas.</span><span class="sxs-lookup"><span data-stu-id="2f34a-111">All examples sale values and tax percentages in this topic are for illustrative purposes only, not exact figures.</span></span>

## <a name="publisher-transacts-in-microsoft-managed-tax-country"></a><span data-ttu-id="2f34a-112">Transacciones del publicador en el país fiscal administrado por Microsoft</span><span class="sxs-lookup"><span data-stu-id="2f34a-112">Publisher Transacts in Microsoft-managed Tax Country</span></span>

<span data-ttu-id="2f34a-113">**Escenario A:** transacciones que tienen lugar entre un publicador y un cliente en un país fiscal [administrado por Microsoft.](tax-details-marketplace.md#microsoft-managed-countries)</span><span class="sxs-lookup"><span data-stu-id="2f34a-113">**Scenario A** – Transactions that take place between a publisher and a customer in a [Microsoft-managed tax country](tax-details-marketplace.md#microsoft-managed-countries).</span></span> <span data-ttu-id="2f34a-114">Estas transacciones tendrán impuestos aplicables agregados en el momento de la venta y Microsoft envía ese impuesto al país aplicable.</span><span class="sxs-lookup"><span data-stu-id="2f34a-114">These transactions will have applicable tax added at the time of sale and Microsoft sends that tax to the applicable country.</span></span> <span data-ttu-id="2f34a-115">No se retiene ningún impuesto del pago y los cálculos de pago son exclusivos de impuestos.</span><span class="sxs-lookup"><span data-stu-id="2f34a-115">No taxes are withheld from payout and payout calculations are tax exclusive.</span></span>

<span data-ttu-id="2f34a-116">Consulte [escenario D para](#foreign-publisher-transacts-with-us-customer) las transacciones entre un publicador que no es de EE. UU. y un cliente de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="2f34a-116">See [Scenario D](#foreign-publisher-transacts-with-us-customer) for transactions between a non-US publisher and a US customer.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-a.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago A.":::

## <a name="publisher-transacts-in-microsoft-managed-tax-country-where-marketplace-fee-is-taxable-service"></a><span data-ttu-id="2f34a-118">Transacciones del publicador en un país fiscal administrado por Microsoft en el que el precio de Marketplace es un servicio imponible</span><span class="sxs-lookup"><span data-stu-id="2f34a-118">Publisher Transacts in Microsoft-managed Tax Country where Marketplace Fee is Taxable Service</span></span>

<span data-ttu-id="2f34a-119">**Escenario B:** transacciones que tienen lugar entre un publicador basado en Estados Unidos (tal y como se define en su información de perfil fiscal de Centro de partners) a un cliente en un país fiscal administrado por Microsoft donde el país impone un impuesto sobre la cuota de Marketplace (un servicio imponible).</span><span class="sxs-lookup"><span data-stu-id="2f34a-119">**Scenario B** – Transactions that take place between a US-based publisher (as defined by their Partner Center Tax Profile Information) to a customer in a Microsoft-managed tax country where the country imposes a tax on the Marketplace Fee (a taxable service).</span></span> <span data-ttu-id="2f34a-120">En este escenario, el impuesto sobre la tarifa del servicio de tienda se resta del pago del anunciante.</span><span class="sxs-lookup"><span data-stu-id="2f34a-120">In this scenario, the tax on the store service fee is subtracted from the publisher's payout.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-b.png" alt-text="Muestra el flujo de trabajo del escenario B del proceso de pago.":::

## <a name="publisher-transacts-in-publisher-managed-tax-country"></a><span data-ttu-id="2f34a-122">Transacciones del publicador en el país fiscal administrado por el publicador</span><span class="sxs-lookup"><span data-stu-id="2f34a-122">Publisher Transacts in Publisher-managed Tax Country</span></span>

<span data-ttu-id="2f34a-123">**Escenario C:** transacciones que tienen lugar entre un publicador y un cliente en un país fiscal administrado por el publicador que no impone una retención de impuestos a los clientes.</span><span class="sxs-lookup"><span data-stu-id="2f34a-123">**Scenario C** – Transactions that take place between a publisher and a customer in a publisher-managed tax country that does not impose a withholding tax on customers.</span></span> <span data-ttu-id="2f34a-124">Los clientes no pagan ningún impuesto en el momento de la venta y es obligación del anunciante pagar todos los impuestos aplicables.</span><span class="sxs-lookup"><span data-stu-id="2f34a-124">Customers pay no tax at the point of sale and it is the publisher's obligation to pay all applicable taxes.</span></span>

<span data-ttu-id="2f34a-125">Para obtener más información sobre los precios específicos del país (por ejemplo, para compensar los próximos impuestos), consulte Planes y precios de ofertas [de marketplace comercial.](/azure/marketplace/plans-pricing#custom-prices)</span><span class="sxs-lookup"><span data-stu-id="2f34a-125">For more information on country-specific pricing (for example, to offset upcoming taxation) see [Plans and pricing for commercial marketplace offers](/azure/marketplace/plans-pricing#custom-prices).</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-c.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago C.":::

## <a name="foreign-publisher-transacts-with-us-customer"></a><span data-ttu-id="2f34a-127">Transacciones del publicador externo con el cliente de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="2f34a-127">Foreign Publisher Transacts with US Customer</span></span>

<span data-ttu-id="2f34a-128">**Escenario D:** todos los anunciantes externos (tal y como se define en su información de perfil fiscal de Centro de partners) en países sin permiso de Estados Unidos (consulte el escenario [E)](#foreign-publisher-with-a-treaty-transacts-with-us-customer)que realiza una venta a un cliente basado en Estados Unidos (tal y como se define en su dirección de cuenta de cliente).</span><span class="sxs-lookup"><span data-stu-id="2f34a-128">**Scenario D** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries without a US treaty (see [Scenario E](#foreign-publisher-with-a-treaty-transacts-with-us-customer)) making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="2f34a-129">El gobierno de EE. UU. requiere que Microsoft retenga los impuestos en nombre del anunciante.</span><span class="sxs-lookup"><span data-stu-id="2f34a-129">US government requires that Microsoft withhold tax on behalf of the publisher.</span></span> <span data-ttu-id="2f34a-130">Los impuestos que se retienen del pago al publicador se calculan en función del precio de la oferta.</span><span class="sxs-lookup"><span data-stu-id="2f34a-130">Tax withheld from payout to publisher is calculated based on offer price.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-d.png" alt-text="Muestra el flujo de trabajo para el escenario D del proceso de pago.":::

## <a name="foreign-publisher-with-a-treaty-transacts-with-us-customer"></a><span data-ttu-id="2f34a-132">Publicador externo con una transacción de transacción con un cliente de EE. UU.</span><span class="sxs-lookup"><span data-stu-id="2f34a-132">Foreign publisher with a Treaty Transacts with US customer</span></span>

<span data-ttu-id="2f34a-133">**Escenario E:** todos los anunciantes externos (tal y como se define por su información de perfil fiscal de Centro de partners) en países con un tratado de Ee. UU. que realiza una venta a un cliente basado en Estados Unidos (tal y como se define en su dirección de cuenta de cliente).</span><span class="sxs-lookup"><span data-stu-id="2f34a-133">**Scenario E** – All foreign publishers (as defined by their Partner Center Tax Profile Information) in countries with a US treaty making a sale to a US-based customer (as defined by their customer account address).</span></span> <span data-ttu-id="2f34a-134">El gobierno de EE. UU. no requiere que Microsoft retenga los impuestos en nombre del anunciante.</span><span class="sxs-lookup"><span data-stu-id="2f34a-134">US government does not require Microsoft to withhold tax on behalf of the publisher.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-e.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago E.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-outside-ireland"></a><span data-ttu-id="2f34a-136">Un anunciante externo vende a un cliente registrado en el IVA de la UE en un país administrado por Microsoft (fuera de Irlanda)</span><span class="sxs-lookup"><span data-stu-id="2f34a-136">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (outside Ireland)</span></span>

<span data-ttu-id="2f34a-137">**Escenario F:** todas las transacciones entre editores externos y clientes registrados en el IVA de la UE (fuera de Irlanda) en un Microsoft-Managed país.</span><span class="sxs-lookup"><span data-stu-id="2f34a-137">**Scenario F** – All transactions between foreign publishers and EU VAT-registered customers (outside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="2f34a-138">El cliente no paga impuestos por la venta.</span><span class="sxs-lookup"><span data-stu-id="2f34a-138">The customer does not pay tax on the sale.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-f.png" alt-text="Muestra el flujo de trabajo para el escenario de proceso de pago F.":::

## <a name="foreign-publisher-sells-to-an-eu-vat-registered-customer-in-a-microsoft-managed-country-in-ireland"></a><span data-ttu-id="2f34a-140">El anunciante externo vende a un cliente registrado en el IVA de la UE en un país administrado por Microsoft (en Irlanda)</span><span class="sxs-lookup"><span data-stu-id="2f34a-140">Foreign publisher sells to an EU VAT-registered customer in a Microsoft-managed country (in Ireland)</span></span>

<span data-ttu-id="2f34a-141">**Escenario G:** todas las transacciones entre anunciantes externos y clientes registrados en el IVA de la UE (dentro de Irlanda) en un Microsoft-Managed país.</span><span class="sxs-lookup"><span data-stu-id="2f34a-141">**Scenario G** – All transactions between foreign publishers and EU VAT-registered customers (inside Ireland) in a Microsoft-Managed country.</span></span> <span data-ttu-id="2f34a-142">El cliente paga el IVA de la caja y Microsoft paga este impuesto al gobierno de Irlanda.</span><span class="sxs-lookup"><span data-stu-id="2f34a-142">The customer pays Irish VAT and Microsoft pays this tax to the Irish government.</span></span>

:::image type="content" source="images/tax-policies/payout-scenario-g.png" alt-text="Muestra el flujo de trabajo para el escenario G del proceso de pago.":::

## <a name="next-steps"></a><span data-ttu-id="2f34a-144">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="2f34a-144">Next steps</span></span>

- [<span data-ttu-id="2f34a-145">Preguntas más frecuentes sobre el publicador</span><span class="sxs-lookup"><span data-stu-id="2f34a-145">Publisher FAQ</span></span>](/azure/marketplace/marketplace-faq-publisher-guide)
- [<span data-ttu-id="2f34a-146">Instrucciones para crear perfiles fiscales y de pago</span><span class="sxs-lookup"><span data-stu-id="2f34a-146">Instructions to create payment and tax profiles</span></span>](./set-up-your-payout-account.md?context=%2fazure%2fmarketplace%2fcontext%2fcontext#create-a-payment-profile)