---
title: Vender clientes Microsoft Azure reservas
ms.topic: article
ms.date: 06/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Como proveedor de soluciones en la nube, puede comprar, vender o administrar las reservas de Azure para los clientes. Use el centro de Partners, el Azure Portal o la API del centro de Partners.
author: BillLinzbach
ms.author: BillLi
keywords: Azure, reservas, administración, facturación, compra, Azure RI, instancias reservadas de Azure
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 93c6353922197270245b4b21f3bc210f26c7ec8f
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377649"
---
# <a name="sell-microsoft-azure-reservations-to-customers-using-partner-center-the-azure-portal-or-apis"></a><span data-ttu-id="93304-105">Venda Microsoft Azure reservas a los clientes mediante el centro de Partners, el Azure Portal o las API</span><span class="sxs-lookup"><span data-stu-id="93304-105">Sell Microsoft Azure reservations to customers using Partner Center, the Azure portal, or APIs</span></span>

<span data-ttu-id="93304-106">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="93304-106">**Applies to**</span></span>

- <span data-ttu-id="93304-107">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="93304-107">Partner Center</span></span>
- <span data-ttu-id="93304-108">Microsoft Azure Portal</span><span class="sxs-lookup"><span data-stu-id="93304-108">Microsoft Azure portal</span></span>
- <span data-ttu-id="93304-109">Asociados en CSP</span><span class="sxs-lookup"><span data-stu-id="93304-109">Partners in CSP</span></span>

<span data-ttu-id="93304-110">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="93304-110">**Appropriate roles**</span></span>

- <span data-ttu-id="93304-111">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="93304-111">Admin agent</span></span>
- <span data-ttu-id="93304-112">Administrador global</span><span class="sxs-lookup"><span data-stu-id="93304-112">Global admin</span></span>
- <span data-ttu-id="93304-113">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="93304-113">Helpdesk agent</span></span>
- <span data-ttu-id="93304-114">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="93304-114">Sales agent</span></span>
- <span data-ttu-id="93304-115">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="93304-115">User management admin</span></span>

<span data-ttu-id="93304-116">Los asociados del programa proveedor de soluciones en la nube (CSP) pueden ofrecer a sus clientes Microsoft Azure reservas.</span><span class="sxs-lookup"><span data-stu-id="93304-116">Partners in the Cloud Solution Provider program (CSP) can offer their customers Microsoft Azure reservations.</span></span> <span data-ttu-id="93304-117">Los clientes pueden obtener ahorros significativos cuando se reservan de antemano.</span><span class="sxs-lookup"><span data-stu-id="93304-117">Customers can gain significant savings when they reserve in advance.</span></span> <span data-ttu-id="93304-118">Las reservas de Azure ofrecen simplicidad y flexibilidad a los clientes de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="93304-118">Azure reservations offer customers simplicity and flexibility in the following ways:</span></span>

- <span data-ttu-id="93304-119">Términos de reserva de uno o tres años</span><span class="sxs-lookup"><span data-stu-id="93304-119">One or three-year reservation terms</span></span>
- <span data-ttu-id="93304-120">Fácil de empezar; Instalación completada en segundos</span><span class="sxs-lookup"><span data-stu-id="93304-120">Easy to get started; setup completed in seconds</span></span>
- <span data-ttu-id="93304-121">Cancelar o intercambiar instancias reservadas en cualquier momento para el reembolso ajustado</span><span class="sxs-lookup"><span data-stu-id="93304-121">Cancel or exchange reserved instances at any time for adjusted refund</span></span>
- <span data-ttu-id="93304-122">Administrar el uso de instancias reservadas en el nivel de Departamento individual o de la organización</span><span class="sxs-lookup"><span data-stu-id="93304-122">Manage reserved instances usage at the organizational or individual department level</span></span> 

<span data-ttu-id="93304-123">Las reservas de Azure pueden apelar a los clientes de las siguientes maneras:</span><span class="sxs-lookup"><span data-stu-id="93304-123">Azure reservations can appeal to customers in the following ways:</span></span>

- <span data-ttu-id="93304-124">Las reservas pueden ofrecer ahorros significativos en los precios de pago por uso (PAYG)</span><span class="sxs-lookup"><span data-stu-id="93304-124">Reservations can offer significant savings over pay-as-you-go (PAYG) pricing</span></span>
- <span data-ttu-id="93304-125">Mejores presupuestos y previsiones con el pago por adelantado de los términos de un año o de tres años</span><span class="sxs-lookup"><span data-stu-id="93304-125">Better budgeting and forecasting with upfront payment for one-year or three-year terms</span></span>
- <span data-ttu-id="93304-126">Capacidad informática con prioridad en la región de Azure más cercana a sus oficinas</span><span class="sxs-lookup"><span data-stu-id="93304-126">Prioritized computing capacity in the Azure region closest to their offices</span></span>
- <span data-ttu-id="93304-127">Las reservas de Azure proporcionan la base para las soluciones de infraestructura de un extremo a otro cuando se combinan con software como Microsoft Windows Server y Azure SQL Database</span><span class="sxs-lookup"><span data-stu-id="93304-127">Azure reservations provide the foundation for end to end infrastructure solutions when combined with software like Microsoft Windows Server and Azure SQL Database</span></span>

>[!NOTE]
> <span data-ttu-id="93304-128">Puede comprar, vender y administrar las reservas de Azure en el centro de Partners y en el Azure Portal, y mediante la API del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="93304-128">You can buy, sell, and manage Azure reservations in both the Partner Center and the Azure portal, and using the Partner Center API.</span></span> <span data-ttu-id="93304-129">También puede conceder a sus clientes permiso para comprar sus propias reservas de Azure a partir de una suscripción de Azure que haya adquirido.</span><span class="sxs-lookup"><span data-stu-id="93304-129">You can also give your customers permission to buy their own Azure reservations from an Azure subscription you purchased for them.</span></span> <span data-ttu-id="93304-130">Siga los vínculos siguientes para obtener información sobre cómo hacerlo.</span><span class="sxs-lookup"><span data-stu-id="93304-130">Follow the links below to learn how.</span></span>

## <a name="azure-reservations-resources"></a><span data-ttu-id="93304-131">Recursos de reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="93304-131">Azure reservations resources</span></span>

|<span data-ttu-id="93304-132">**Para información acerca de**</span><span class="sxs-lookup"><span data-stu-id="93304-132">**For information about**</span></span>   |<span data-ttu-id="93304-133">**Lee esto**</span><span class="sxs-lookup"><span data-stu-id="93304-133">**Read this**</span></span>    |
|:-----------------------------|:-----------------|
| <span data-ttu-id="93304-134">Documentación de reservas de Azure para sus clientes</span><span class="sxs-lookup"><span data-stu-id="93304-134">Azure reservations documentation for your customers</span></span> | [<span data-ttu-id="93304-135">¿Qué son las reservas de Azure?</span><span class="sxs-lookup"><span data-stu-id="93304-135">What are Azure reservations?</span></span>](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)
|<span data-ttu-id="93304-136">Compra de reservas de Azure para sus clientes en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="93304-136">Purchasing Azure reservations for your customers in Partner Center</span></span>   |[<span data-ttu-id="93304-137">Comprar reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="93304-137">Buy Azure reservations</span></span>](azure-reservations-buying.md)
|<span data-ttu-id="93304-138">Administración de las reservas de Azure en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="93304-138">Managing Azure reservations in Partner Center</span></span> | [<span data-ttu-id="93304-139">Administración de las reservas de Azure en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="93304-139">Managing Azure reservations in Partner Center</span></span>](azure-reservations-manage.md)
|<span data-ttu-id="93304-140">Determinación del tamaño correcto de la máquina virtual y comprobación del uso de la máquina virtual del cliente</span><span class="sxs-lookup"><span data-stu-id="93304-140">Determining the correct VM size and verifying customer VM usage</span></span>   |[<span data-ttu-id="93304-141">Tamaño de máquina virtual para el uso máximo de reserva de Azure</span><span class="sxs-lookup"><span data-stu-id="93304-141">VM sizing for maximum Azure reservation usage</span></span>](azure-usage.md)   |
|<span data-ttu-id="93304-142">Compra de reservas de Azure mediante la API del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="93304-142">Purchasing Azure reservations using the Partner Center API</span></span> | <span data-ttu-id="93304-143">[Comprar Azure Reserved VM instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) en la documentación para desarrolladores del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="93304-143">[Purchase Azure Reserved VM Instances](https://docs.microsoft.com/partner-center/develop/purchase-azure-reservations) in the Partner Center developer documentation</span></span>   |
|<span data-ttu-id="93304-144">Otorgar a los clientes permiso para comprar sus propias reservas de Azure desde la suscripción de CSP.</span><span class="sxs-lookup"><span data-stu-id="93304-144">Giving customers permission to buy their own Azure reservations from your CSP subscription.</span></span> | [<span data-ttu-id="93304-145">Conceder permiso a los clientes para que compren sus propias reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="93304-145">Give customers permission to buy their own Azure reservations</span></span>](give-customers-permission.md)   |
