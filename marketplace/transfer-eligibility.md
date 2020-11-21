---
title: 'Elegibilidad de transferencia: directrices para transferir una suscripción entre cuentas de facturación, Azure Marketplace'
description: Directrices para comprobaciones comerciales antes de transferir una suscripción entre cuentas de facturación en el Azure Portal.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007348"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a><span data-ttu-id="9103e-103">Transferir la idoneidad para una suscripción entre cuentas de facturación</span><span class="sxs-lookup"><span data-stu-id="9103e-103">Transfer eligibility for a subscription between billing accounts</span></span>

<span data-ttu-id="9103e-104">Puede [transferir una suscripción](/azure/cost-management-billing/understand/subscription-transfer) de una cuenta de facturación a otra en la sección facturación de la Azure portal.</span><span class="sxs-lookup"><span data-stu-id="9103e-104">You can [transfer a subscription](/azure/cost-management-billing/understand/subscription-transfer) from one billing account to another in the billing section of the Azure portal.</span></span> <span data-ttu-id="9103e-105">Antes de una transferencia, la suscripción se examina para los productos de terceros.</span><span class="sxs-lookup"><span data-stu-id="9103e-105">Prior to a transfer, the subscription is scanned for third-party products.</span></span> <span data-ttu-id="9103e-106">La transferencia se permite solo si se borran *todos* los productos para su transferencia (consulte los [criterios](#criteria-for-transfer-approval-or-denial) siguientes).</span><span class="sxs-lookup"><span data-stu-id="9103e-106">The transfer is permitted only if *all* products are cleared for transfer (see the [criteria](#criteria-for-transfer-approval-or-denial) below).</span></span> <span data-ttu-id="9103e-107">El sistema generará mensajes de error relevantes para las aplicaciones que no se han podido borrar para ayudarle a determinar los pasos siguientes.</span><span class="sxs-lookup"><span data-stu-id="9103e-107">The system will generate relevant error messages for the apps that failed to clear to help you determine next steps.</span></span>

> [!NOTE]
> <span data-ttu-id="9103e-108">Este artículo no se aplica a las ofertas de SaaS porque los recursos de SaaS se adjuntan a un inquilino, no a una suscripción.</span><span class="sxs-lookup"><span data-stu-id="9103e-108">This article does not apply to SaaS offers because SaaS resources are attached to a tenant, not a subscription.</span></span> <span data-ttu-id="9103e-109">Los recursos de SaaS se pueden transferir desde una cuenta de facturación a otra, pero esto se hace por recurso y por el soporte técnico de Azure como solicitud de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="9103e-109">SaaS resources are transferable from one billing account to another, but this is done per resource and by Azure support as a support request.</span></span>

## <a name="criteria-for-transfer-approval-or-denial"></a><span data-ttu-id="9103e-110">Criterios de aprobación o denegación de transferencia</span><span class="sxs-lookup"><span data-stu-id="9103e-110">Criteria for transfer approval or denial</span></span>

<span data-ttu-id="9103e-111">No se puede transferir una suscripción si cualquiera de sus aplicaciones de terceros cumple alguno de los siguientes criterios:</span><span class="sxs-lookup"><span data-stu-id="9103e-111">You cannot transfer a subscription if any of its third-party apps meet any of the following criteria:</span></span>

- <span data-ttu-id="9103e-112">La cuenta de destino es comercial y la aplicación deja de participar a través de asociados.</span><span class="sxs-lookup"><span data-stu-id="9103e-112">The target account is commercial and the app is opt-out to be sold via partners.</span></span>
- <span data-ttu-id="9103e-113">La aplicación es participación para los asociados seleccionados y la cuenta de destino no se encuentra en la lista de permitidos.</span><span class="sxs-lookup"><span data-stu-id="9103e-113">The app is opt-in for selected partners and the target account is not in the allow list.</span></span>
- <span data-ttu-id="9103e-114">La oferta era una oferta de vista previa en el pasado para las suscripciones seleccionadas o era una oferta privada y la suscripción ya no se encuentra en la lista de permitidos.</span><span class="sxs-lookup"><span data-stu-id="9103e-114">The offer was a preview offer in the past for selected subscriptions or was a private offer and the subscription is no longer in the allow list.</span></span>
- <span data-ttu-id="9103e-115">La nueva cuenta de facturación está en una región diferente de donde se vende la oferta y la oferta no se vende en esa región.</span><span class="sxs-lookup"><span data-stu-id="9103e-115">The new billing account is in a region different from where the offer is sold AND the offer is not to be sold in that region.</span></span>

<span data-ttu-id="9103e-116">Una transferencia bloqueada permanece en vigor hasta que se quita el recurso de la suscripción, tras lo cual se puede volver a intentar la transferencia.</span><span class="sxs-lookup"><span data-stu-id="9103e-116">A blocked transfer remains in effect until you remove the resource from the subscription, after which you can try the transfer again.</span></span>

## <a name="next-steps"></a><span data-ttu-id="9103e-117">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="9103e-117">Next steps</span></span>

[<span data-ttu-id="9103e-118">Obtener soporte técnico para Microsoft AppSource y Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="9103e-118">Get support for Microsoft AppSource and Azure Marketplace</span></span>](get-support.md)

