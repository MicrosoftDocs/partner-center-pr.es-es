---
title: Cómo se calcula el crédito obtenido del socio | Centro de Partners
ms.topic: article
ms.date: 09/17/2019
description: Cómo se calcula el aspecto del crédito obtenido por el socio comercial del plan de Azure
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: eb0dd5ef22632a85ca0227cc9e988a88263e9ddf
ms.sourcegitcommit: 0195355f4526362f4d89f59ea643a5e422b6a9b2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/27/2019
ms.locfileid: "71318772"
---
# <a name="how-the-partner-earned-credit-pec-is-calculated"></a><span data-ttu-id="7163b-103">Cómo se calcula el crédito obtenido por el socio comercial (PEC)</span><span class="sxs-lookup"><span data-stu-id="7163b-103">How the partner earned credit (PEC) is calculated</span></span>


<span data-ttu-id="7163b-104">Los asociados que poseen la administración de operaciones de ti ininterrumpida de piezas o todo el entorno de Azure de sus clientes en CSP se recompensan con PEC.</span><span class="sxs-lookup"><span data-stu-id="7163b-104">Partners who own the 24x7 IT operations management of parts or the entire Azure environment of their customers in CSP are rewarded with PEC.</span></span> <span data-ttu-id="7163b-105">El PEC se proporciona como parte de la factura al socio comercial que tiene una relación de facturación directa con Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7163b-105">The PEC is provided as part of the invoice to the partner who has a direct billing relationship with Microsoft.</span></span> <span data-ttu-id="7163b-106">El crédito se calcula diariamente y se refleja en la factura mensual.</span><span class="sxs-lookup"><span data-stu-id="7163b-106">The credit is calculated daily and reflected in the monthly invoice.</span></span> <span data-ttu-id="7163b-107">De forma predeterminada, en CSP, a los asociados se les conceden los derechos de acceso necesarios a la suscripción del cliente, lo que les permite administrar y controlar las operaciones de forma ininterrumpida de los recursos de la suscripción.</span><span class="sxs-lookup"><span data-stu-id="7163b-107">By default, in CSP, partners are granted the necessary access rights to the customer’s subscription that allows them to have 24X7 operations management and control of the resources on the subscription.</span></span> <span data-ttu-id="7163b-108">En la sección siguiente se describen otras maneras en las que el cliente puede aprovisionar el acceso para el asociado de transacción.</span><span class="sxs-lookup"><span data-stu-id="7163b-108">Additional ways in which customer can provision access for transacting partner are described in the following section.</span></span>   


## <a name="important-eligibility-and-calculation-requirements"></a><span data-ttu-id="7163b-109">Requisitos importantes de elegibilidad y cálculo:</span><span class="sxs-lookup"><span data-stu-id="7163b-109">Important eligibility and calculation requirements:</span></span>

- <span data-ttu-id="7163b-110">Un asociado debe tener un acuerdo de MPN activo y un rol de la cuenta basada en reglas C (RBAC) válido para recibir el crédito obtenido para los recursos de Azure que administran.</span><span class="sxs-lookup"><span data-stu-id="7163b-110">A partner should have an active MPN agreement and a valid Rules Based Account C (RBAC) role to receive earned credit for the azure assets they manage.</span></span> <span data-ttu-id="7163b-111">Más información sobre [roles RBAC válidos]</span><span class="sxs-lookup"><span data-stu-id="7163b-111">Learn more about [valid RBAC roles]</span></span>

- <span data-ttu-id="7163b-112">El proveedor indirecto será válido para PEC si su revendedor indirecto o el revendedor indirecto, o ambos, tienen control operativo y administración ininterrumpida de los recursos de Azure del cliente en CSP.</span><span class="sxs-lookup"><span data-stu-id="7163b-112">The indirect provider will be eligible for PEC if either they or their indirect reseller or both have 24x7 operational control and management of the customer’s Azure resources in CSP.</span></span>

- <span data-ttu-id="7163b-113">PEC está asociado al consumo facturado (facturable) de la entidad de Azure del cliente en el CSP administrado por el asociado.</span><span class="sxs-lookup"><span data-stu-id="7163b-113">PEC is associated to billed (chargeable) consumption of customer’s Azure estate in CSP managed by the partner.</span></span> 

- <span data-ttu-id="7163b-114">PEC solo está disponible para los asociados de CSP que se facturan por Microsoft (proveedor indirecto y socio de facturación directo).</span><span class="sxs-lookup"><span data-stu-id="7163b-114">PEC is available only to partners in CSP who are billed by Microsoft (indirect provider and direct bill partner).</span></span>

- <span data-ttu-id="7163b-115">Servicios válidos: el crédito obtenido por el socio comercial es aplicable a todo el consumo de Azure de Azure 1PP proporcionado en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="7163b-115">Eligible Services: Partner earned credit is applicable to all Azure 1PP Azure consumption given on the price list.</span></span> <span data-ttu-id="7163b-116">Hay excepciones que incluyen, entre otras, 3PP y Azure Reservations.</span><span class="sxs-lookup"><span data-stu-id="7163b-116">There are exceptions including, but not limited to, 3PP and Azure Reservations.</span></span>

- <span data-ttu-id="7163b-117">PEC se calcula diariamente y se puede ver en el archivo de conciliación diaria.</span><span class="sxs-lookup"><span data-stu-id="7163b-117">PEC is calculated daily and can be viewed in the daily recon file.</span></span> <span data-ttu-id="7163b-118">Un asociado (proveedor o distribuidor (a través de su proveedor) debe tener acceso a todo el día (ininterrumpida) para asegurarse de que ganan PEC.</span><span class="sxs-lookup"><span data-stu-id="7163b-118">A partner (provider or reseller (through their provider) must have access for the entire day (24x7) to ensure they earn PEC.</span></span>

- <span data-ttu-id="7163b-119">PEC se gana al nivel de recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="7163b-119">PEC is earned down to the Azure resource level.</span></span> <span data-ttu-id="7163b-120">Si el asociado tiene acceso válido en el nivel de suscripción o de grupo de recursos, cada recurso que se aplica a la entidad superior ganará PEC.</span><span class="sxs-lookup"><span data-stu-id="7163b-120">If the partner has valid access at the subscription, or resource group level, each resource that role up to the higher entity will earn PEC.</span></span> 

- <span data-ttu-id="7163b-121">PEC se incluirá en la factura mensual del asociado.</span><span class="sxs-lookup"><span data-stu-id="7163b-121">PEC will be included on the partner's monthly invoice.</span></span> <span data-ttu-id="7163b-122">La factura es neta de cargos.</span><span class="sxs-lookup"><span data-stu-id="7163b-122">The invoice is net of charges.</span></span> <span data-ttu-id="7163b-123">Los detalles se muestran en el archivo de conciliación de factura.</span><span class="sxs-lookup"><span data-stu-id="7163b-123">The details are shown in the invoice recon file.</span></span>

<span data-ttu-id="7163b-124">Para obtener información sobre cómo obtener acceso para administrar las suscripciones de Azure y sobre cómo vincular el identificador de MPN a los roles de RBAC, consulte [Administración de suscripciones y recursos en el plan de Azure](azure-plan-manage.md).</span><span class="sxs-lookup"><span data-stu-id="7163b-124">For information on gaining access to manage Azure subscriptions and on how to link your MPN ID to RBAC roles, read [Manage subscriptions and resources under the Azure plan](azure-plan-manage.md).</span></span>

<span data-ttu-id="7163b-125">Para más información</span><span class="sxs-lookup"><span data-stu-id="7163b-125">For more information</span></span>

- [<span data-ttu-id="7163b-126">Plan de Azure: facturación</span><span class="sxs-lookup"><span data-stu-id="7163b-126">Azure plan - billing</span></span>](azure-plan-billing.md)

- [<span data-ttu-id="7163b-127">Lista de precios para la nueva experiencia de comercio en CSP</span><span class="sxs-lookup"><span data-stu-id="7163b-127">Price list for the new commerce experience in CSP </span></span>](azure-plan-price-list.md)