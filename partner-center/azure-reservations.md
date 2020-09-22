---
title: Vender clientes Microsoft Azure reservas
description: Como proveedor de soluciones en la nube, puede comprar, vender o administrar las reservas de Azure para los clientes. Use el centro de Partners, el Azure Portal o la API del centro de Partners.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 317d1f0295b79b79bf06f1091ae365bc7012b749
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000239"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="601e8-104">Venda Microsoft Azure reservas a los clientes mediante el centro de Partners, el Azure Portal o las API</span><span class="sxs-lookup"><span data-stu-id="601e8-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="601e8-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="601e8-105">**Applies to**</span></span>

- <span data-ttu-id="601e8-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="601e8-106">Partner Center</span></span>
- <span data-ttu-id="601e8-107">Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="601e8-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="601e8-108">Partners del programa CSP</span><span class="sxs-lookup"><span data-stu-id="601e8-108">Partners in the CSP program</span></span>

<span data-ttu-id="601e8-109">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="601e8-109">**Appropriate roles**</span></span>

- <span data-ttu-id="601e8-110">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="601e8-110">Admin agent</span></span>
- <span data-ttu-id="601e8-111">Administrador global</span><span class="sxs-lookup"><span data-stu-id="601e8-111">Global admin</span></span>
- <span data-ttu-id="601e8-112">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="601e8-112">Helpdesk agent</span></span>
- <span data-ttu-id="601e8-113">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="601e8-113">Sales agent</span></span>
- <span data-ttu-id="601e8-114">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="601e8-114">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="601e8-115">Este artículo se aplica únicamente a los asociados del programa proveedor de soluciones en la nube (CSP).</span><span class="sxs-lookup"><span data-stu-id="601e8-115">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="601e8-116">Los clientes que usen otros tipos de suscripciones (como, por ejemplo, pago por uso, individuo, contrato de cliente de Microsoft o suscripciones Contrato Enterprise), en su lugar, deberán leer [esta documentación](/azure/cost-management-billing/reservations)de las reservas de Azure.</span><span class="sxs-lookup"><span data-stu-id="601e8-116">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](/azure/cost-management-billing/reservations).</span></span>

<span data-ttu-id="601e8-117">Los asociados del programa CSP pueden ofrecer a sus clientes Microsoft Azure reservas.</span><span class="sxs-lookup"><span data-stu-id="601e8-117">Partners in the CSP program can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="601e8-118">Los clientes pueden obtener ahorros significativos cuando se reservan de antemano.</span><span class="sxs-lookup"><span data-stu-id="601e8-118">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="601e8-119">Las reservas de Azure ofrecen simplicidad y flexibilidad a los clientes de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="601e8-119">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="601e8-120">Términos de reserva de uno o tres años</span><span class="sxs-lookup"><span data-stu-id="601e8-120">One or three-year reservation terms</span></span>
- <span data-ttu-id="601e8-121">Fácil de empezar; Instalación completada en segundos</span><span class="sxs-lookup"><span data-stu-id="601e8-121">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="601e8-122">Cancelar o intercambiar instancias reservadas en cualquier momento para el reembolso ajustado</span><span class="sxs-lookup"><span data-stu-id="601e8-122">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="601e8-123">Administrar el uso de instancias reservadas en el nivel de Departamento individual o de la organización</span><span class="sxs-lookup"><span data-stu-id="601e8-123">Manage reserved instances usage at the organizational or individual department level</span></span>

<span data-ttu-id="601e8-124">Las reservas de Azure pueden apelar a los clientes de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="601e8-124">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="601e8-125">Las reservas pueden ofrecer ahorros significativos en los precios de pago por uso (PAYG)</span><span class="sxs-lookup"><span data-stu-id="601e8-125">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="601e8-126">Mejores presupuestos y previsiones con el pago por adelantado de los términos de un año o de tres años</span><span class="sxs-lookup"><span data-stu-id="601e8-126">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="601e8-127">Capacidad informática con prioridad en la región de Azure más cercana a sus oficinas</span><span class="sxs-lookup"><span data-stu-id="601e8-127">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="601e8-128">Las reservas de Azure proporcionan la base para las soluciones de infraestructura de un extremo a otro cuando se combinan con software como Microsoft Windows Server y Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="601e8-128">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="601e8-129">Puede comprar, vender y administrar las reservas de Azure en el centro de Partners y en el Azure Portal, y mediante la API del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="601e8-129">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="601e8-130">También puede conceder a sus clientes permiso para comprar sus propias reservas de Azure a partir de una suscripción de Azure que haya adquirido.</span><span class="sxs-lookup"><span data-stu-id="601e8-130">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="601e8-131">Siga los vínculos siguientes para obtener información sobre cómo hacerlo.</span><span class="sxs-lookup"><span data-stu-id="601e8-131">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="601e8-132">Recursos de reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="601e8-132">Azure reservations resources</span></span>

|<span data-ttu-id="601e8-133">**Para información acerca de**</span><span class="sxs-lookup"><span data-stu-id="601e8-133">**For information about**</span></span>   |<span data-ttu-id="601e8-134">**Lee esto**</span><span class="sxs-lookup"><span data-stu-id="601e8-134">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="601e8-135">Documentación de reservas de Azure para sus clientes</span><span class="sxs-lookup"><span data-stu-id="601e8-135">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="601e8-136">¿Qué es Azure Reservations?</span><span class="sxs-lookup"><span data-stu-id="601e8-136">What are Azure reservations?</span></span>](/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="601e8-137">Compra de reservas de Azure para sus clientes en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="601e8-137">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="601e8-138">Comprar reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="601e8-138">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="601e8-139">Administración de las reservas de Azure en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="601e8-139">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="601e8-140">Administración de las reservas de Azure en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="601e8-140">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="601e8-141">Determinación del tamaño correcto de la máquina virtual y comprobación del uso de la máquina virtual del cliente</span><span class="sxs-lookup"><span data-stu-id="601e8-141">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="601e8-142">Tamaño de máquina virtual para el uso máximo de reserva de Azure</span><span class="sxs-lookup"><span data-stu-id="601e8-142">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="601e8-143">Compra de reservas de Azure mediante la API del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="601e8-143">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="601e8-144">[Comprar Azure Reserved VM instances](/partner-center/develop/purchase-azure-reservations) en la documentación para desarrolladores del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="601e8-144">[Purchase Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="601e8-145">Otorgar a los clientes permiso para comprar sus propias reservas de Azure desde la suscripción de CSP.</span><span class="sxs-lookup"><span data-stu-id="601e8-145">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="601e8-146">Conceder permiso a los clientes para que compren sus propias reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="601e8-146">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |