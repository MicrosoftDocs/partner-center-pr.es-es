---
title: Comprobar el estado del servicio de un cliente
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprenda a usar el centro de partners para comprobar el estado del servicio de un cliente cuando se produzca un problema con un servicio.
author: Kim-Davis
ms.author: kimnich
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: eba88c5380254929809d27ff2b877a5ee72df239
ms.sourcegitcommit: c4f2561fb7f224554c31e3af491de4ad65644158
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/23/2020
ms.locfileid: "87114811"
---
# <a name="check-service-health-for-a-customer-reporting-a-potential-service-problem-or-outage"></a><span data-ttu-id="b2e08-103">Comprobación del estado del servicio de un cliente que informa de un posible problema o interrupción del servicio</span><span class="sxs-lookup"><span data-stu-id="b2e08-103">Check service health for a customer reporting a potential service problem or outage</span></span>

<span data-ttu-id="b2e08-104">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="b2e08-104">**Applies to**</span></span>

- <span data-ttu-id="b2e08-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="b2e08-105">Partner Center</span></span>

<span data-ttu-id="b2e08-106">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="b2e08-106">**Appropriate roles**</span></span>

- <span data-ttu-id="b2e08-107">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="b2e08-107">Admin agent</span></span>
- <span data-ttu-id="b2e08-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="b2e08-108">Global admin</span></span>
- <span data-ttu-id="b2e08-109">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="b2e08-109">Helpdesk agent</span></span>
- <span data-ttu-id="b2e08-110">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="b2e08-110">Sales agent</span></span>

<span data-ttu-id="b2e08-111">Una de las primeras cosas que puedes hacer si un cliente está experimentando problemas con un servicio es comprobar el estado de dicho servicio.</span><span class="sxs-lookup"><span data-stu-id="b2e08-111">One of the first things you can do when a customer is experiencing problems with a service is to check the service health.</span></span> 

## <a name="check-service-health"></a><span data-ttu-id="b2e08-112">Comprobación del estado del servicio</span><span class="sxs-lookup"><span data-stu-id="b2e08-112">Check service health</span></span>

1. <span data-ttu-id="b2e08-113">Seleccione el **cliente** que tiene el problema en la **lista de clientes**.</span><span class="sxs-lookup"><span data-stu-id="b2e08-113">Select the **Customer** that is having the issue from the **Customer list**.</span></span>

2. <span data-ttu-id="b2e08-114">Seleccione **Administración de servicios** en el menú de la izquierda.</span><span class="sxs-lookup"><span data-stu-id="b2e08-114">Select **Service management** from the left menu.</span></span> <span data-ttu-id="b2e08-115">Se enumerarán los servicios aprovisionados para el cliente y el estado del servicio para cada uno de ellos.</span><span class="sxs-lookup"><span data-stu-id="b2e08-115">This will list the services provisioned for the customer and the service health for each.</span></span> <span data-ttu-id="b2e08-116">Los asociados pueden hacer clic en el servicio en el que están interesados para obtener más información.</span><span class="sxs-lookup"><span data-stu-id="b2e08-116">Partners can click the service they are interested in to get more information.</span></span> 

>[!NOTE] 
> <span data-ttu-id="b2e08-117">Los vínculos de estado del servicio en las páginas de **Administración de servicios** tomarán el asociado al centro de administración de M365 o al Azure portal como **Administrador Delegado**. Una vez que el asociado llega a un destino, el asociado puede ir a las páginas de estado del servicio en cualquier portal para obtener más detalles sobre la interrupción.</span><span class="sxs-lookup"><span data-stu-id="b2e08-117">Service health links on the **Service management** pages will take the partner to either the M365 admin center or the Azure portal as **delegated admin**. Once the partner gets to either destination, the partner can navigate to the service health pages in either portal for more details about the outage.</span></span>
 
<span data-ttu-id="b2e08-118">Durante una interrupción del servicio, Microsoft proporciona actualizaciones periódicas mientras trabaja para solucionar el problema.</span><span class="sxs-lookup"><span data-stu-id="b2e08-118">During a service outage, Microsoft provides regular updates as we work to address the problem.</span></span> <span data-ttu-id="b2e08-119">Estas notificaciones también se muestran en el Microsoft Azure Portal o en el centro de administración de Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b2e08-119">These notifications are also displayed on either the Microsoft Azure portal or the Microsoft 365 admin Center.</span></span>

<span data-ttu-id="b2e08-120">Si el problema persiste después del final de la interrupción del servicio, envíe una solicitud de servicio.</span><span class="sxs-lookup"><span data-stu-id="b2e08-120">If the problem persists after the end of the service outage, submit a service request.</span></span> <span data-ttu-id="b2e08-121">Consulta [Notificar problemas en nombre de un cliente](report-problems-on-behalf-of-a-customer.md).</span><span class="sxs-lookup"><span data-stu-id="b2e08-121">See [Report problems on behalf of a customer](report-problems-on-behalf-of-a-customer.md).</span></span>

<span data-ttu-id="b2e08-122">Microsoft 365 y Microsoft Azure proporcionan [API que los asociados pueden usar para recuperar el estado del servicio en tiempo real](get-automated-service-notifications-with-our-apis.md), las comunicaciones del centro de mensajes y los eventos de mantenimiento planeado.</span><span class="sxs-lookup"><span data-stu-id="b2e08-122">Microsoft 365 and Microsoft Azure each provide [APIs that partners can use to retrieve real-time service health](get-automated-service-notifications-with-our-apis.md), message center communications, and planned maintenance events.</span></span>

 

