---
title: 'Guía de inicio rápido: administración de Azure Marketplace privado con PowerShell'
description: En esta guía de inicio rápido se muestra cómo administrar ofertas en un Azure Marketplace privado mediante Azure PowerShell.
author: keferna
ms.author: keferna
ms.topic: quickstart
ms.prod: marketplace-customer
ms.devlang: azurepowershell
ms.date: 11/24/2020
ms.custom: devx-track-azurepowershell
ms.openlocfilehash: d0021be17ab12b6e549b0e5263772a4a1e42f8a3
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182348"
---
# <a name="quickstart-manage-a-private-azure-marketplace-using-powershell"></a><span data-ttu-id="d81ce-103">Guía de inicio rápido: administración de Azure Marketplace privado con PowerShell</span><span class="sxs-lookup"><span data-stu-id="d81ce-103">Quickstart: Manage a Private Azure Marketplace using PowerShell</span></span>

<span data-ttu-id="d81ce-104">En este artículo se describe cómo puede administrar ofertas en un Azure Marketplace privado mediante el módulo [AZ. Marketplace](/powershell/module/az.marketplace) de PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d81ce-104">This article describes how you can manage offers in a Private Azure Marketplace using the [Az.Marketplace](/powershell/module/az.marketplace) PowerShell module.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d81ce-105">Azure Marketplace privado se encuentra actualmente en versión preliminar pública.</span><span class="sxs-lookup"><span data-stu-id="d81ce-105">Private Azure Marketplace is currently in public preview.</span></span> <span data-ttu-id="d81ce-106">Esta versión preliminar se proporciona sin un acuerdo de nivel de servicio.</span><span class="sxs-lookup"><span data-stu-id="d81ce-106">This preview version is provided without a service level agreement.</span></span> <span data-ttu-id="d81ce-107">No se recomienda para las cargas de trabajo de producción.</span><span class="sxs-lookup"><span data-stu-id="d81ce-107">It's not recommended for production workloads.</span></span> <span data-ttu-id="d81ce-108">Es posible que algunas características no sean compatibles o que sus funcionalidades estén limitadas.</span><span class="sxs-lookup"><span data-stu-id="d81ce-108">Some features might not be supported or might have constrained capabilities.</span></span> <span data-ttu-id="d81ce-109">Para más información, consulte [Términos de uso complementarios de las Versiones Preliminares de Microsoft Azure](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span><span class="sxs-lookup"><span data-stu-id="d81ce-109">For more information, see [Supplemental Terms of Use for Microsoft Azure Previews](https://azure.microsoft.com/support/legal/preview-supplemental-terms/).</span></span>

## <a name="requirements"></a><span data-ttu-id="d81ce-110">Requisitos</span><span class="sxs-lookup"><span data-stu-id="d81ce-110">Requirements</span></span>

* <span data-ttu-id="d81ce-111">Si no tiene una suscripción a Azure, cree una cuenta [gratuita](https://azure.microsoft.com/free/) antes de empezar.</span><span class="sxs-lookup"><span data-stu-id="d81ce-111">If you don't have an Azure subscription, create a [free](https://azure.microsoft.com/free/) account before you begin.</span></span>

* <span data-ttu-id="d81ce-112">Si opta por usar Azure PowerShell en un entorno local:</span><span class="sxs-lookup"><span data-stu-id="d81ce-112">If you choose to use Azure PowerShell locally:</span></span>
  * <span data-ttu-id="d81ce-113">[Instale el módulo de PowerShell](/powershell/azure/install-az-ps).</span><span class="sxs-lookup"><span data-stu-id="d81ce-113">[Install the Az PowerShell module](/powershell/azure/install-az-ps).</span></span>
  * <span data-ttu-id="d81ce-114">Conéctese a su cuenta de Azure mediante el cmdlet [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span><span class="sxs-lookup"><span data-stu-id="d81ce-114">Connect to your Azure account using the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>
* <span data-ttu-id="d81ce-115">Si decide usar Azure Cloud Shell:</span><span class="sxs-lookup"><span data-stu-id="d81ce-115">If you choose to use Azure Cloud Shell:</span></span>
  * <span data-ttu-id="d81ce-116">Para más información, consulte [Introducción a Azure Cloud Shell](/azure/cloud-shell/overview).</span><span class="sxs-lookup"><span data-stu-id="d81ce-116">See [Overview of Azure Cloud Shell](/azure/cloud-shell/overview) for more information.</span></span>

  > [!IMPORTANT]
  > <span data-ttu-id="d81ce-117">Mientras el módulo de PowerShell **AZ. Marketplace** se encuentra en versión preliminar, debe instalarlo por separado mediante el `Install-Module` cmdlet.</span><span class="sxs-lookup"><span data-stu-id="d81ce-117">While the **Az.Marketplace** PowerShell module is in preview, you must install it separately using the `Install-Module` cmdlet.</span></span> <span data-ttu-id="d81ce-118">Una vez que este módulo de PowerShell esté disponible con carácter general, formará parte de las futuras versiones del módulo Az de PowerShell y estará disponible de forma predeterminada en Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="d81ce-118">After this PowerShell module becomes generally available, it will be part of future Az PowerShell module releases and available by default from within Azure Cloud Shell.</span></span>

  ```azurepowershell-interactive
  Install-Module -Name Az.Marketplace
  ```

* <span data-ttu-id="d81ce-119">Si tiene varias suscripciones a Azure, elija la suscripción adecuada en la que se debe facturar el recurso.</span><span class="sxs-lookup"><span data-stu-id="d81ce-119">If you have multiple Azure subscriptions, choose the appropriate subscription in which the resources should be billed.</span></span> <span data-ttu-id="d81ce-120">Seleccione una suscripción específica con el cmdlet [Set-AzContext](/powershell/module/az.accounts/set-azcontext).</span><span class="sxs-lookup"><span data-stu-id="d81ce-120">Select a specific subscription using the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span>

  ```azurepowershell-interactive
  Set-AzContext -SubscriptionId 00000000-0000-0000-0000-000000000000
  ```

## <a name="list-private-stores"></a><span data-ttu-id="d81ce-121">Enumerar almacenes privados</span><span class="sxs-lookup"><span data-stu-id="d81ce-121">List private stores</span></span>

<span data-ttu-id="d81ce-122">Para recuperar una lista de almacenes privados, use el cmdlet [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) .</span><span class="sxs-lookup"><span data-stu-id="d81ce-122">To retrieve a list of private stores, you use the [Get-AzMarketplacePrivateStore](/powershell/module/az.marketplace/get-azmarketplaceprivatestore) cmdlet.</span></span> <span data-ttu-id="d81ce-123">En el ejemplo siguiente se enumeran los almacenes privados que se crearon en el ámbito del inquilino.</span><span class="sxs-lookup"><span data-stu-id="d81ce-123">The following example lists private stores that were created under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStore
```

```Output
Availability   : enabled
PrivateStoreId : 00000000-0000-0000-0000-000000000000
ETag           : "00000000-0000-0000-0000-000000000000"
Id             : /providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000
Name           : 00000000-0000-0000-0000-000000000000
Type           : Microsoft.Marketplace/privateStores
```

## <a name="add-an-offer-to-a-private-marketplace"></a><span data-ttu-id="d81ce-124">Incorporación de una oferta a un Marketplace privado</span><span class="sxs-lookup"><span data-stu-id="d81ce-124">Add an offer to a private marketplace</span></span>

<span data-ttu-id="d81ce-125">Para agregar una oferta a una tienda privada, use el cmdlet [set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="d81ce-125">To add an offer to a private store, you use the [Set-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/set-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="d81ce-126">En el ejemplo siguiente se agrega la oferta especificada a un Marketplace privado para un almacén privado que se crea en el ámbito del inquilino.</span><span class="sxs-lookup"><span data-stu-id="d81ce-126">The following example adds the specified offer to a private marketplace for a private store that is created under the tenant scope.</span></span>

```azurepowershell-interactive
$Params = @{
  privateStoreId = '00000000-0000-0000-0000-000000000000'
  offerId = 'publisherid.offerid'
  SpecificPlanIdsLimitation =@('PublisherEnterpriseLinux72',
                               'PublisherEnterpriseLinux72-ARM',
                               'PublisherEnterpriseLinux73',
                               'PublisherEnterpriseLinux73-ARM',
                               'PublisherEnterpriseLinux73-ARM-pr'
  )
}
Set-AzMarketplacePrivateStoreOffer @Params
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {PublisherEnterpriseLinux72, PublisherEnterpriseLinux72-ARM,
PublisherEnterpriseLinux73, PublisherEnterpriseLinux73-ARM, PublisherEnterpriseLinux73-ARM-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="get-private-store-offers"></a><span data-ttu-id="d81ce-127">Obtener ofertas de tiendas privadas</span><span class="sxs-lookup"><span data-stu-id="d81ce-127">Get private store offers</span></span>

<span data-ttu-id="d81ce-128">Para obtener una o varias ofertas de almacén privado, use el cmdlet [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="d81ce-128">To get one or more private store offers, you use the [Get-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/get-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="d81ce-129">En el ejemplo siguiente se obtienen ofertas asociadas al almacén privado especificado que se agregaron en el ámbito del inquilino.</span><span class="sxs-lookup"><span data-stu-id="d81ce-129">The following example gets offers that are associated with the specified private store that were added under the tenant scope.</span></span>

```azurepowershell-interactive
Get-AzMarketplacePrivateStoreOffer -PrivateStoreId 00000000-0000-0000-0000-000000000000
```

```Output
UniqueOfferId             : publisherid.offerid
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {small, medium-with-upgraded-bandwidth, medium-with-upgraded-apps, large, large-pr,
small-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid.offerid
Name                      : publisherid.offerid
Type                      : Microsoft.Marketplace/privateStores/offers

UniqueOfferId             : publisherid1.offerid1
OfferDisplayName          :
PublisherDisplayName      :
ETag                      : "00000000-0000-0000-0000-000000000000"
PrivateStoreId            : 00000000-0000-0000-0000-000000000000
CreatedBy                 :
CreatedDate               : 01/01/0001 00:00:00
SpecificPlanIdsLimitation : {azure_managedservices_professional ,azure_managedservices_professional-pr}
Id                        :
/providers/Microsoft.Marketplace/privateStores/00000000-0000-0000-0000-000000000000/offers/
                            publisherid1.offerid1
Name                      : publisherid1.offerid1
Type                      : Microsoft.Marketplace/privateStores/offers
```

## <a name="remove-an-offer"></a><span data-ttu-id="d81ce-130">Quitar una oferta</span><span class="sxs-lookup"><span data-stu-id="d81ce-130">Remove an offer</span></span>

<span data-ttu-id="d81ce-131">Para quitar una oferta de una tienda privada, use el cmdlet [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) .</span><span class="sxs-lookup"><span data-stu-id="d81ce-131">To remove an offer from a private store, you use the [Remove-AzMarketplacePrivateStoreOffer](/powershell/module/az.marketplace/remove-azmarketplaceprivatestoreoffer) cmdlet.</span></span> <span data-ttu-id="d81ce-132">En el ejemplo siguiente se quita una oferta de un almacén privado que se creó en el ámbito del inquilino.</span><span class="sxs-lookup"><span data-stu-id="d81ce-132">The following example removes an offer from a private store that was created in the tenant scope.</span></span>

```azurepowershell-interactive
Remove-AzMarketplacePrivateStoreOffer -privateStoreId 00000000-0000-0000-0000-000000000000 -offerId publisherid.offerid
```

## <a name="next-steps"></a><span data-ttu-id="d81ce-133">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d81ce-133">Next steps</span></span>

<span data-ttu-id="d81ce-134">[Cree y administre Azure Marketplace privado](create-manage-private-azure-marketplace.md).</span><span class="sxs-lookup"><span data-stu-id="d81ce-134">[Create and manage Private Azure Marketplace](create-manage-private-azure-marketplace.md).</span></span>