---
title: Vender clientes Microsoft Azure reservas
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Como proveedor de soluciones en la nube, puede comprar, vender o administrar las reservas de Azure para los clientes. Use el centro de Partners, el Azure Portal o la API del centro de Partners.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4524d810a036953e45fb94a72241734e02a2798f
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435734"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="1c3a1-104">Venda Microsoft Azure reservas a los clientes mediante el centro de Partners, el Azure Portal o las API</span><span class="sxs-lookup"><span data-stu-id="1c3a1-104">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="1c3a1-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="1c3a1-105">**Applies to**</span></span>

- <span data-ttu-id="1c3a1-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="1c3a1-106">Partner Center</span></span>
- <span data-ttu-id="1c3a1-107">Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="1c3a1-107">Microsoft Azure portal</span></span>
- <span data-ttu-id="1c3a1-108">Asociados en CSP</span><span class="sxs-lookup"><span data-stu-id="1c3a1-108">Partners in CSP</span></span>

<span data-ttu-id="1c3a1-109">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="1c3a1-109">**Appropriate roles**</span></span>

- <span data-ttu-id="1c3a1-110">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="1c3a1-110">Admin agent</span></span>
- <span data-ttu-id="1c3a1-111">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1c3a1-111">Global admin</span></span>
- <span data-ttu-id="1c3a1-112">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="1c3a1-112">Helpdesk agent</span></span>
- <span data-ttu-id="1c3a1-113">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="1c3a1-113">Sales agent</span></span>
- <span data-ttu-id="1c3a1-114">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="1c3a1-114">User management admin</span></span>

<span data-ttu-id="1c3a1-115">Los asociados del programa proveedor de soluciones en la nube (CSP) pueden ofrecer a sus clientes Microsoft Azure reservas.</span><span class="sxs-lookup"><span data-stu-id="1c3a1-115">Partners in the Cloud Solution Provider program (CSP) can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="1c3a1-116">Los clientes pueden obtener ahorros significativos cuando se reservan de antemano.</span><span class="sxs-lookup"><span data-stu-id="1c3a1-116">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="1c3a1-117">Las reservas de Azure ofrecen simplicidad y flexibilidad a los clientes de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="1c3a1-117">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="1c3a1-118">Términos de reserva de uno o tres años</span><span class="sxs-lookup"><span data-stu-id="1c3a1-118">One or three-year reservation terms</span></span>
- <span data-ttu-id="1c3a1-119">Fácil de empezar; Instalación completada en segundos</span><span class="sxs-lookup"><span data-stu-id="1c3a1-119">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="1c3a1-120">Cancelar o intercambiar instancias reservadas en cualquier momento para el reembolso ajustado</span><span class="sxs-lookup"><span data-stu-id="1c3a1-120">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="1c3a1-121">Administrar el uso de instancias reservadas en el nivel de Departamento individual o de la organización</span><span class="sxs-lookup"><span data-stu-id="1c3a1-121">Manage reserved instances usage at the organizational or individual department level</span></span> 

<span data-ttu-id="1c3a1-122">Las reservas de Azure pueden apelar a los clientes de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="1c3a1-122">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="1c3a1-123">Las reservas pueden ofrecer ahorros significativos en los precios de pago por uso (PAYG)</span><span class="sxs-lookup"><span data-stu-id="1c3a1-123">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="1c3a1-124">Mejores presupuestos y previsiones con el pago por adelantado de los términos de un año o de tres años</span><span class="sxs-lookup"><span data-stu-id="1c3a1-124">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="1c3a1-125">Capacidad informática con prioridad en la región de Azure más cercana a sus oficinas</span><span class="sxs-lookup"><span data-stu-id="1c3a1-125">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="1c3a1-126">Las reservas de Azure proporcionan la base para las soluciones de infraestructura de un extremo a otro cuando se combinan con software como Microsoft Windows Server y Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="1c3a1-126">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="1c3a1-127">Puede comprar, vender y administrar las reservas de Azure en el centro de Partners y en el Azure Portal, y mediante la API del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="1c3a1-127">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="1c3a1-128">También puede conceder a sus clientes permiso para comprar sus propias reservas de Azure a partir de una suscripción de Azure que haya adquirido.</span><span class="sxs-lookup"><span data-stu-id="1c3a1-128">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="1c3a1-129">Siga los vínculos siguientes para obtener información sobre cómo hacerlo.</span><span class="sxs-lookup"><span data-stu-id="1c3a1-129">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="1c3a1-130">Recursos de reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="1c3a1-130">Azure reservations resources</span></span>

|<span data-ttu-id="1c3a1-131">**Para información acerca de**</span><span class="sxs-lookup"><span data-stu-id="1c3a1-131">**For information about**</span></span>   |<span data-ttu-id="1c3a1-132">**Lee esto**</span><span class="sxs-lookup"><span data-stu-id="1c3a1-132">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="1c3a1-133">Documentación de reservas de Azure para sus clientes</span><span class="sxs-lookup"><span data-stu-id="1c3a1-133">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="1c3a1-134">¿Qué son las reservas de Azure?</span><span class="sxs-lookup"><span data-stu-id="1c3a1-134">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="1c3a1-135">Compra de reservas de Azure para sus clientes en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="1c3a1-135">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="1c3a1-136">Comprar reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="1c3a1-136">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="1c3a1-137">Administración de las reservas de Azure en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="1c3a1-137">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="1c3a1-138">Administración de las reservas de Azure en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="1c3a1-138">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="1c3a1-139">Determinación del tamaño correcto de la máquina virtual y comprobación del uso de la máquina virtual del cliente</span><span class="sxs-lookup"><span data-stu-id="1c3a1-139">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="1c3a1-140">Tamaño de máquina virtual para el uso máximo de reserva de Azure</span><span class="sxs-lookup"><span data-stu-id="1c3a1-140">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="1c3a1-141">Compra de reservas de Azure mediante la API del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="1c3a1-141">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="1c3a1-142">[Comprar Azure Reserved VM instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) en la documentación para desarrolladores del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="1c3a1-142">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="1c3a1-143">Otorgar a los clientes permiso para comprar sus propias reservas de Azure desde la suscripción de CSP.</span><span class="sxs-lookup"><span data-stu-id="1c3a1-143">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="1c3a1-144">Conceder permiso a los clientes para que compren sus propias reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="1c3a1-144">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
