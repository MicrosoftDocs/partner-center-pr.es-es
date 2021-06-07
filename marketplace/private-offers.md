---
title: Ofertas privadas en Azure Marketplace
description: Obtenga información sobre las ofertas privadas en Azure Marketplace.
ms.service: marketplace-customer
ms.topic: article
author: Guyshu
ms.author: gushuchm
ms.date: 06/03/2021
ms.openlocfilehash: 55d0716b183e9e8905e631447e547396d6f55404
ms.sourcegitcommit: 9cb6bc9df20540f812b7932f88e520976c1aa85a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/06/2021
ms.locfileid: "111534181"
---
# <a name="private-plans-in-azure-marketplace"></a><span data-ttu-id="aabc1-103">Planes privados en Azure Marketplace</span><span class="sxs-lookup"><span data-stu-id="aabc1-103">Private plans in Azure Marketplace</span></span>

<span data-ttu-id="aabc1-104">Los planes privados son la forma en que los publicadores proporcionan planes personalizados a clientes específicos.</span><span class="sxs-lookup"><span data-stu-id="aabc1-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="aabc1-105">Los planes privados solo están disponibles para las ofertas de pago que se pueden adquirir e instalar directamente desde el Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="aabc1-105">Private plans are only available for paid offers that can be purchased and directly installed from the Azure portal.</span></span> <span data-ttu-id="aabc1-106">Los publicadores no pueden crear planes privados para servicios de consultoría, ningún servicio que tenga **Contacto** conmigo como llamada a la acción ni ningún servicio gratuito, independientemente de si se puede instalar desde el portal o no.</span><span class="sxs-lookup"><span data-stu-id="aabc1-106">Publishers cannot create private plans for consulting services, any service that has **Contact me** as a call-to-action, or any free service, regardless of whether it can be installed from the portal or not.</span></span>

## <a name="find-private-plans-in-the-azure-portal"></a><span data-ttu-id="aabc1-107">Busque planes privados en el Azure Portal</span><span class="sxs-lookup"><span data-stu-id="aabc1-107">Find private plans in the Azure portal</span></span>

<span data-ttu-id="aabc1-108">Cuando un asociado publica un plan privado, solo es visible para los usuarios aptos en la **sección Marketplace** de la Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="aabc1-108">When a partner publishes a private plan, it is visible only to eligible users in the **Marketplace** section of the Azure portal.</span></span> <span data-ttu-id="aabc1-109">Estos usuarios se definen mediante el identificador de suscripción o el identificador de inquilino, según el tipo de oferta.</span><span class="sxs-lookup"><span data-stu-id="aabc1-109">These users are defined by subscription ID or tenant ID, depending on the offer type.</span></span> <span data-ttu-id="aabc1-110">Si es apto para planes privados, hay dos maneras de encontrarlos en el portal.</span><span class="sxs-lookup"><span data-stu-id="aabc1-110">If you are eligible for private plans, there are two ways to find them in the portal.</span></span>

> [!NOTE]
> <span data-ttu-id="aabc1-111">Los planes privados se pueden buscar pero no se pueden filtrar (por categoría) en el Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="aabc1-111">Private plans are searchable but not filterable (by category) in the Azure portal.</span></span>

<span data-ttu-id="aabc1-112">En la Azure Portal, seleccione **+ Crear un recurso** o busque "Marketplace" para ir a la página **marketplace.**</span><span class="sxs-lookup"><span data-stu-id="aabc1-112">In the Azure portal, select **+ Create a resource** or search for “marketplace” to go to the **Marketplace** page.</span></span> <span data-ttu-id="aabc1-113">Si es apto para planes privados, verá el banner You **have private plans available (Tiene** planes privados disponibles) en la parte superior de la página.</span><span class="sxs-lookup"><span data-stu-id="aabc1-113">If you are eligible for private plans, you will see the **You have private plans available** banner on the top of the page.</span></span> <span data-ttu-id="aabc1-114">Seleccione **Ver ofertas privadas y planes para** ir a la página de planes privados.</span><span class="sxs-lookup"><span data-stu-id="aabc1-114">Select **View private offers + plans** to go to your private plans page.</span></span>

:::image type="content" source="media/private-offers/private-offers-banner.png" alt-text="Banner que se muestra cuando hay planes privados disponibles.":::

## <a name="review-private-plans"></a><span data-ttu-id="aabc1-116">Revisión de planes privados</span><span class="sxs-lookup"><span data-stu-id="aabc1-116">Review private plans</span></span>

<span data-ttu-id="aabc1-117">Un plan privado forma parte de varios planes de una oferta.</span><span class="sxs-lookup"><span data-stu-id="aabc1-117">A private plan is part of several plans in an offer.</span></span> <span data-ttu-id="aabc1-118">Cada oferta puede tener varios planes, tanto públicos como privados, pero los planes privados se muestran en una lista independiente de los planes públicos.</span><span class="sxs-lookup"><span data-stu-id="aabc1-118">Each offer can have multiple plans, both public and private, but private plans are shown under a separate listing from public plans.</span></span>

<span data-ttu-id="aabc1-119">Puede ver los planes privados disponibles en la **pestaña Planes,** marcados con un distintivo **privado** distintivo:</span><span class="sxs-lookup"><span data-stu-id="aabc1-119">You can see the available private plans under the **Plans** tab, marked with a distinctive **Private** badge:</span></span>

:::image type="content" source="media/private-offers/private-badge.png" alt-text="Página de planes marcada como Privada.":::

<span data-ttu-id="aabc1-121">Si tiene más de una suscripción, verá todos los planes privados disponibles para todas las suscripciones.</span><span class="sxs-lookup"><span data-stu-id="aabc1-121">If you have more than one subscription, you will see all private plans available for all your subscriptions.</span></span> <span data-ttu-id="aabc1-122">Al seleccionar **Crear**, se le enruta a la página de creación de recursos para empezar a configurar el recurso.</span><span class="sxs-lookup"><span data-stu-id="aabc1-122">When you select **Create**, you are routed to the resource creation page to start configuring your resource.</span></span>

<span data-ttu-id="aabc1-123">Si selecciona **Crear** y tiene varias suscripciones, pero no todas se agregan al plan privado, es posible que la suscripción predeterminada no sea la suscripción apta para este plan privado.</span><span class="sxs-lookup"><span data-stu-id="aabc1-123">If you select **Create** and have multiple subscriptions, but not all of them are added to the private plan, your default subscription may not be the subscription eligible for this private plan.</span></span> <span data-ttu-id="aabc1-124">En este caso, seleccione la suscripción correcta.</span><span class="sxs-lookup"><span data-stu-id="aabc1-124">In this case, select the correct subscription.</span></span>

:::image type="content" source="media/private-offers/select-correct-subscription.png" alt-text="Vínculo que muestra que hay más planes privados disponibles.":::

## <a name="next-steps"></a><span data-ttu-id="aabc1-126">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="aabc1-126">Next steps</span></span>

- [<span data-ttu-id="aabc1-127">¿Qué es Azure Marketplace?</span><span class="sxs-lookup"><span data-stu-id="aabc1-127">What is Azure Marketplace?</span></span>](azure-marketplace-overview.md)
