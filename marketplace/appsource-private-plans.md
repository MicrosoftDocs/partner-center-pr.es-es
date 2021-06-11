---
title: Planes privados en Microsoft AppSource
description: Configuración de planes privados en Microsoft AppSource (Azure Marketplace).
ms.service: marketplace-customer
ms.topic: how-to
author: Guyshu
ms.author: gushuchm
ms.date: 06/08/2021
robots: noindex
ms.openlocfilehash: a392859c1106c747e0e7c696927ef3b25262e411
ms.sourcegitcommit: a576c9606ade59cef7d0b2d5e1584016740d08eb
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/11/2021
ms.locfileid: "112008549"
---
# <a name="private-plans-in-microsoft-appsource"></a><span data-ttu-id="7604d-103">Planes privados en Microsoft AppSource</span><span class="sxs-lookup"><span data-stu-id="7604d-103">Private plans in Microsoft AppSource</span></span>

<span data-ttu-id="7604d-104">Los planes privados son la forma en que los publicadores proporcionan planes personalizados a clientes específicos.</span><span class="sxs-lookup"><span data-stu-id="7604d-104">Private plans are how publishers provide custom plans to specific customers.</span></span> <span data-ttu-id="7604d-105">Esta opción ya está disponible en Microsoft AppSource.</span><span class="sxs-lookup"><span data-stu-id="7604d-105">This option is now available in Microsoft AppSource.</span></span> <span data-ttu-id="7604d-106">Los planes privados se pueden vender en AppSource para ofertas  de software como servicio (SaaS) con la llamada a la acción Obtener ahora.</span><span class="sxs-lookup"><span data-stu-id="7604d-106">Private plans can be sold on AppSource for software as a service (SaaS) offers with the **Get it now** call-to-action.</span></span>

## <a name="ask-your-isv-for-a-private-plan"></a><span data-ttu-id="7604d-107">Pedir a su ISV un plan privado</span><span class="sxs-lookup"><span data-stu-id="7604d-107">Ask your ISV for a private plan</span></span>

<span data-ttu-id="7604d-108">Para que un plan privado esté disponible en AppSource, debe ponerse en contacto directamente con el ISV y negociar un precio personalizado y especificaciones técnicas.</span><span class="sxs-lookup"><span data-stu-id="7604d-108">For a private plan to be available to you in AppSource, you need to contact the ISV directly and negotiate a custom price and technical specifications.</span></span> <span data-ttu-id="7604d-109">Una vez acordados los términos del plan privado, el ISV creará un plan y lo asignará al identificador de inquilino de la organización, que deberá proporcionar.</span><span class="sxs-lookup"><span data-stu-id="7604d-109">Once the terms of the private plan are agreed to, the ISV will create a plan for you and assign it to your organization’s tenant ID, which you’ll need to provide.</span></span>

### <a name="finding-your-tenant-id"></a><span data-ttu-id="7604d-110">Búsqueda del identificador de inquilino</span><span class="sxs-lookup"><span data-stu-id="7604d-110">Finding your tenant ID</span></span>

1. <span data-ttu-id="7604d-111">En AppSource, en la esquina superior derecha, seleccione el icono de perfil de cuenta y, a continuación, **Ver inquilino.**</span><span class="sxs-lookup"><span data-stu-id="7604d-111">In AppSource, in the upper right corner, select your account profile icon and then **View tenant**.</span></span>
2. <span data-ttu-id="7604d-112">Copie el identificador de inquilino y proporcionelo al ISV.</span><span class="sxs-lookup"><span data-stu-id="7604d-112">Copy the tenant ID and provide it to the ISV.</span></span>

    :::image type="content" source="media/private-offers/find-tenant-id.png" alt-text="Muestra cómo buscar el identificador de inquilino.":::

## <a name="find-a-private-plan-in-appsource"></a><span data-ttu-id="7604d-114">Buscar un plan privado en AppSource</span><span class="sxs-lookup"><span data-stu-id="7604d-114">Find a private plan in AppSource</span></span>

<span data-ttu-id="7604d-115">Puede tardar hasta 48 horas después de que el ISV publique el nuevo plan privado antes de verlo en AppSource.</span><span class="sxs-lookup"><span data-stu-id="7604d-115">It can take up to 48 hours after the ISV publishes the new private plan before you see it in AppSource.</span></span> <span data-ttu-id="7604d-116">Para buscar planes privados asociados con el identificador de inquilino, seleccione **Planes privados** (icono de bloqueo) en la esquina superior derecha de AppSource.</span><span class="sxs-lookup"><span data-stu-id="7604d-116">To find private plans associated with your tenant ID, select **Private plans** (Lock icon) at the upper right of AppSource.</span></span>

:::image type="content" source="media/private-offers/lock-icon.png" alt-text="Muestra el icono de bloqueo (candado) en la barra de herramientas superior.":::

<span data-ttu-id="7604d-118">Si no ha iniciado sesión, aparecerá un mensaje que le pedirá que lo haga.</span><span class="sxs-lookup"><span data-stu-id="7604d-118">If you are not signed in, a message will prompt you to do so.</span></span> <span data-ttu-id="7604d-119">A continuación, puede comprar los planes privados asociados con el identificador de inquilino en la **pestaña Planes y** precios.</span><span class="sxs-lookup"><span data-stu-id="7604d-119">You can then purchase the private plans associated with your tenant ID on the **Plans + pricing** tab.</span></span>

:::image type="content" source="media/private-offers/plan-pricing-tab.png" alt-text="Muestra ofertas privadas en la pestaña plan y precios.":::

<span data-ttu-id="7604d-121">Si los planes privados no están disponibles para el inquilino, aparecerá un mensaje que indica que no tiene planes ni ofertas privados.</span><span class="sxs-lookup"><span data-stu-id="7604d-121">If private plans are not available for your tenant, a message will state that you don’t have any private plans or offers.</span></span>

## <a name="purchase-a-private-plan"></a><span data-ttu-id="7604d-122">Compra de un plan privado</span><span class="sxs-lookup"><span data-stu-id="7604d-122">Purchase a private plan</span></span>

<span data-ttu-id="7604d-123">Un ISV puede incluir uno o varios planes privados dentro de una oferta.</span><span class="sxs-lookup"><span data-stu-id="7604d-123">An ISV can include one or more private plans within an offer.</span></span> <span data-ttu-id="7604d-124">Cada oferta puede tener planes públicos y privados, pero los planes privados aparecen en una página de descripción de la oferta independiente a la que se accede desde el icono ofertas privadas (candado) en la esquina superior derecha de la página.</span><span class="sxs-lookup"><span data-stu-id="7604d-124">Each offer can have both public and private plans, but private plans appear under a separate offer listing page accessed from the Private offers icon (padlock) at the upper right of the page.</span></span>

<span data-ttu-id="7604d-125">Los planes privados disponibles se muestran en la **pestaña Planes y** precios. Los planes privados tienen un distintivo azul distintivo.</span><span class="sxs-lookup"><span data-stu-id="7604d-125">Available private plans display on the **Plans + pricing** tab. Private plans have a distinctive blue badge.</span></span>

:::image type="content" source="media/private-offers/private-plans-badge.png" alt-text="Muestra el distintivo azul de la oferta privada junto a las ofertas privadas.":::

<span data-ttu-id="7604d-127">Para comprar un plan seleccionado, seleccione **Obtenerlo ahora** y siga los pasos proporcionados.</span><span class="sxs-lookup"><span data-stu-id="7604d-127">To purchase a selected plan, select **Get it now** and follow the steps provided.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7604d-128">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="7604d-128">Next steps</span></span>

- [<span data-ttu-id="7604d-129">¿Qué es Microsoft AppSource?</span><span class="sxs-lookup"><span data-stu-id="7604d-129">What is Microsoft AppSource?</span></span>](appsource-overview.md)
