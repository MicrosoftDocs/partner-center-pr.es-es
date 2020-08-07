---
title: Reservas de Azure & suscripciones de servidor
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre las oportunidades del proveedor de soluciones en la nube para adquirir, aprovisionar y administrar las reservas de Azure y las suscripciones de servidor para los clientes.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5b8a9cf07f8dace47346c68ade3707d6b12a1532
ms.sourcegitcommit: b79504dbfc335aca995f370e15a654829acdaaff
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/06/2020
ms.locfileid: "87900096"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="30f89-103">Adquisición, aprovisionamiento, & administración de instancias reservadas de máquina virtual de Azure (RI) + suscripciones de servidor para clientes</span><span class="sxs-lookup"><span data-stu-id="30f89-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="30f89-104">Se aplica a:</span><span class="sxs-lookup"><span data-stu-id="30f89-104">Applies to:</span></span>

- <span data-ttu-id="30f89-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="30f89-105">Partner Center</span></span>

<span data-ttu-id="30f89-106">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="30f89-106">**Appropriate roles**</span></span>

- <span data-ttu-id="30f89-107">Agente de administrador</span><span class="sxs-lookup"><span data-stu-id="30f89-107">Admin agent</span></span>
- <span data-ttu-id="30f89-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="30f89-108">Global admin</span></span>
- <span data-ttu-id="30f89-109">Agente del departamento de soporte técnico</span><span class="sxs-lookup"><span data-stu-id="30f89-109">Helpdesk agent</span></span>
- <span data-ttu-id="30f89-110">Agente de ventas</span><span class="sxs-lookup"><span data-stu-id="30f89-110">Sales agent</span></span>
- <span data-ttu-id="30f89-111">Administrador del control de usuarios</span><span class="sxs-lookup"><span data-stu-id="30f89-111">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="30f89-112">Este artículo se aplica únicamente a los asociados del programa proveedor de soluciones en la nube (CSP).</span><span class="sxs-lookup"><span data-stu-id="30f89-112">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="30f89-113">Los clientes que usen otros tipos de suscripciones (como, por ejemplo, pago por uso, individuo, contrato de cliente de Microsoft o suscripciones Contrato Enterprise), en su lugar, deberán leer [esta documentación](https://docs.microsoft.com/azure/cost-management-billing/reservations)de las reservas de Azure.</span><span class="sxs-lookup"><span data-stu-id="30f89-113">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="30f89-114">¿Qué es Azure Reservations?</span><span class="sxs-lookup"><span data-stu-id="30f89-114">What are Azure Reservations?</span></span>

<span data-ttu-id="30f89-115">Azure Reservations ayudarle a ahorrar dinero al pagar por adelantado de una máquina virtual de un año o tres años, SQL Database capacidad de proceso, Azure Cosmos DB el rendimiento u otros recursos de Azure.</span><span class="sxs-lookup"><span data-stu-id="30f89-115">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="30f89-116">El pago adelantado le permite obtener un descuento en los recursos que utiliza.</span><span class="sxs-lookup"><span data-stu-id="30f89-116">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="30f89-117">Las reservas pueden reducir significativamente la máquina virtual, el proceso de SQL Database, Azure Cosmos DB y otros costos de recursos hasta un 72% en comparación con los precios de pago por uso.</span><span class="sxs-lookup"><span data-stu-id="30f89-117">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="30f89-118">Reservations ofrece un descuento en la facturación y no afecta al estado del entorno de ejecución de los recursos.</span><span class="sxs-lookup"><span data-stu-id="30f89-118">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="30f89-119">Para obtener más información, consulte [¿Qué son Azure reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="30f89-119">For more information see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="30f89-120">¿Por qué los clientes deben comprar una reserva?</span><span class="sxs-lookup"><span data-stu-id="30f89-120">Why should customers buy a reservation?</span></span>

<span data-ttu-id="30f89-121">Si los clientes tienen máquinas virtuales, Azure Cosmos DB o bases de datos SQL que se ejecutan durante largos períodos de tiempo, la compra de una reserva les proporciona la opción más rentable.</span><span class="sxs-lookup"><span data-stu-id="30f89-121">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="30f89-122">Por ejemplo, si un cliente ejecuta continuamente cuatro instancias de un servicio sin una reserva, se cobran según las tarifas de pago por uso.</span><span class="sxs-lookup"><span data-stu-id="30f89-122">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="30f89-123">Si compran una reserva para esos recursos, obtienen inmediatamente el descuento de la reserva.</span><span class="sxs-lookup"><span data-stu-id="30f89-123">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="30f89-124">Ya no se aplicarán a los recursos las tarifas de pago por uso.</span><span class="sxs-lookup"><span data-stu-id="30f89-124">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="30f89-125">Nueva oferta atractiva de Azure en CSP</span><span class="sxs-lookup"><span data-stu-id="30f89-125">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="30f89-126">Al trasladar Azure Reservations y suscripciones de servidor a su programa de CSP, Microsoft está habilitando mejor a sus asociados para abordar rápidamente la demanda de los clientes para ofrecer soluciones más rentables que permitan cargas de trabajo de nube persistentes altamente predecibles.</span><span class="sxs-lookup"><span data-stu-id="30f89-126">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="30f89-127">El programa CSP permite a los asociados adquirir, aprovisionar y administrar Azure Reservations y suscripciones de servidor en nombre de clientes comerciales a través del centro de Partners de Microsoft y Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="30f89-127">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="30f89-128">Incluso proporcionamos a los asociados en nuestras opciones del programa CSP sobre cómo se pueden adquirir las reservas de Azure.</span><span class="sxs-lookup"><span data-stu-id="30f89-128">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="30f89-129">Los asociados de CSP pueden [comprar reservas de Azure en nombre de un cliente](azure-reservations-buying.md) o pueden [permitir que el cliente compre sus propias reservas](give-customers-permission.md) de una suscripción de Azure anterior que el asociado ha adquirido para ellas.</span><span class="sxs-lookup"><span data-stu-id="30f89-129">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="30f89-130">Azure Reservations ofrecer a los clientes la flexibilidad de la virtualización para una amplia gama de soluciones informáticas, como desarrollo y pruebas, ejecutar aplicaciones y ampliar el centro de datos.</span><span class="sxs-lookup"><span data-stu-id="30f89-130">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="30f89-131">Con [Azure Reserved VM instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) por ejemplo, los clientes comerciales ahora pueden ahorrar hasta un 72% en comparación con los precios de las máquinas virtuales de Azure de pago por uso, simplemente comprando, o "reservando", la máquina virtual durante un período de 1 o 3 años.</span><span class="sxs-lookup"><span data-stu-id="30f89-131">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="30f89-132">Los clientes de Windows Server con Ventaja híbrida de Azure, incluido con software Assurance, podrán ahorrar hasta un 80% en comparación con los precios de pago por uso.</span><span class="sxs-lookup"><span data-stu-id="30f89-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="30f89-133">Con una combinación sin comparación de precios atractivos y una flexibilidad de implementación incomparable, los clientes verán el mejor valor general cuando elijan Azure Reservations:</span><span class="sxs-lookup"><span data-stu-id="30f89-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="30f89-134">Reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="30f89-134">Azure reservations</span></span>

- <span data-ttu-id="30f89-135">Azure Reserved VM Instances</span><span class="sxs-lookup"><span data-stu-id="30f89-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="30f89-136">Reservas de base de SQL</span><span class="sxs-lookup"><span data-stu-id="30f89-136">SQL DB Reservations</span></span>
- <span data-ttu-id="30f89-137">Instancia administrada de SQL</span><span class="sxs-lookup"><span data-stu-id="30f89-137">SQL Managed Instance</span></span>
- <span data-ttu-id="30f89-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="30f89-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="30f89-139">Azure SQL Data Warehouse</span><span class="sxs-lookup"><span data-stu-id="30f89-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="30f89-140">Servicios de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="30f89-140">App Services</span></span>
- <span data-ttu-id="30f89-141">Azure Databricks reservas unitarias</span><span class="sxs-lookup"><span data-stu-id="30f89-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="30f89-142">Disco administrado</span><span class="sxs-lookup"><span data-stu-id="30f89-142">Managed Disk</span></span>
- <span data-ttu-id="30f89-143">Blob en bloques</span><span class="sxs-lookup"><span data-stu-id="30f89-143">Block blob</span></span>
- <span data-ttu-id="30f89-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="30f89-144">MySQL</span></span>
- <span data-ttu-id="30f89-145">Explorador de datos de Azure</span><span class="sxs-lookup"><span data-stu-id="30f89-145">Azure Data explorer</span></span>
- <span data-ttu-id="30f89-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="30f89-146">MariaDB</span></span>
- <span data-ttu-id="30f89-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="30f89-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="30f89-148">Suscripciones de servidor</span><span class="sxs-lookup"><span data-stu-id="30f89-148">Server subscriptions</span></span>

- <span data-ttu-id="30f89-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="30f89-149">Windows Server</span></span>
- <span data-ttu-id="30f89-150">Cal de Servicios de Escritorio remoto (RDS)</span><span class="sxs-lookup"><span data-stu-id="30f89-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="30f89-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="30f89-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="30f89-152">Suscripciones anuales de ISV de Linux</span><span class="sxs-lookup"><span data-stu-id="30f89-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="30f89-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="30f89-153">SUSE Linux</span></span>
- <span data-ttu-id="30f89-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="30f89-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="30f89-155">Red Hat OpenShift en Azure</span><span class="sxs-lookup"><span data-stu-id="30f89-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="30f89-156">Suscripciones anuales de ISV</span><span class="sxs-lookup"><span data-stu-id="30f89-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="30f89-157">Azure VMware Solution by CloudSimple</span><span class="sxs-lookup"><span data-stu-id="30f89-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="30f89-158">Introducción</span><span class="sxs-lookup"><span data-stu-id="30f89-158">Getting started</span></span>

<span data-ttu-id="30f89-159">Para entender cómo puede posicionar Azure Reservations con sus clientes y ponerse en marcha de manera operativa lo más rápido posible, se recomienda el siguiente enfoque para revisar los materiales de preparación:</span><span class="sxs-lookup"><span data-stu-id="30f89-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="30f89-160">Revise las presentaciones de información general y los seminarios web asociados para la propuesta de valor y la posición de los clientes.</span><span class="sxs-lookup"><span data-stu-id="30f89-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="30f89-161">Revisar y comprender la guía de operaciones de comercio moderno</span><span class="sxs-lookup"><span data-stu-id="30f89-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="30f89-162">Revise las preguntas más frecuentes sobre las suscripciones de RI y de servidor de Azure</span><span class="sxs-lookup"><span data-stu-id="30f89-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="30f89-163">Descripción de las actualizaciones de Azure Reservations y suscripciones de servidor en la [API del centro de Partners (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="30f89-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="30f89-164">Recursos</span><span class="sxs-lookup"><span data-stu-id="30f89-164">Resources</span></span>

<span data-ttu-id="30f89-165">A continuación se muestra una lista completa de recursos que le ayudarán a incorporar rápidamente Azure Reservations a través del centro de Partners:</span><span class="sxs-lookup"><span data-stu-id="30f89-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="30f89-166">Preparación de ventas</span><span class="sxs-lookup"><span data-stu-id="30f89-166">Sales readiness</span></span>

- [<span data-ttu-id="30f89-167">Azure Reservations y suscripciones de servidor con Ventaja híbrida de Azure información general</span><span class="sxs-lookup"><span data-stu-id="30f89-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="30f89-168">Hoja de ventas</span><span class="sxs-lookup"><span data-stu-id="30f89-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="30f89-169">Preguntas más frecuentes sobre asociados para Azure Reservations</span><span class="sxs-lookup"><span data-stu-id="30f89-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="30f89-170">Preguntas más frecuentes sobre asociados de Azure Reservations y SQL DB</span><span class="sxs-lookup"><span data-stu-id="30f89-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="30f89-171">Licencia de acceso de cliente (CAL) de Servicios de Escritorio remoto (RDS) (anuncio)</span><span class="sxs-lookup"><span data-stu-id="30f89-171">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="30f89-172">Azure Reserved VM Instances (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="30f89-172">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="30f89-173">Suscripciones de servidor</span><span class="sxs-lookup"><span data-stu-id="30f89-173">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="30f89-174">Información general de SQL Database en Azure</span><span class="sxs-lookup"><span data-stu-id="30f89-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="30f89-175">Reservas de base de SQL (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="30f89-175">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="30f89-176">Azure Cosmos DB (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="30f89-176">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="30f89-177">Instancia administrada SQL (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="30f89-177">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="30f89-178">SUSE y Red Hat Enterprise Linux (Azure Portal)</span><span class="sxs-lookup"><span data-stu-id="30f89-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="30f89-179">Red Hat Linux en Azure</span><span class="sxs-lookup"><span data-stu-id="30f89-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="30f89-180">SUSE Linux en Azure</span><span class="sxs-lookup"><span data-stu-id="30f89-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="30f89-181">Linux en Azure</span><span class="sxs-lookup"><span data-stu-id="30f89-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="30f89-182">Información general sobre precios de Azure</span><span class="sxs-lookup"><span data-stu-id="30f89-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="30f89-183">Calculadora de precios de Azure</span><span class="sxs-lookup"><span data-stu-id="30f89-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="30f89-184">Azure Databricks reservas unitarias</span><span class="sxs-lookup"><span data-stu-id="30f89-184">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="30f89-185">Listas de precios de CSP: las listas de precios **Microsoft Azure instancias reservadas** y **suscripciones de software** se encuentran en la página precios del centro de Partners [&](https://partner.microsoft.com/pcv/sales) .</span><span class="sxs-lookup"><span data-stu-id="30f89-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="30f89-186">Cursos</span><span class="sxs-lookup"><span data-stu-id="30f89-186">Training</span></span>

<span data-ttu-id="30f89-187">Regístrese para ver [seminarios web de preparación de licencias comerciales](https://commercial-licensing.eventbuilder.com/FY2019_ALL) y eventos a petición.</span><span class="sxs-lookup"><span data-stu-id="30f89-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="30f89-188">Los eventos de preparación de licencias a petición incluyen temas como los siguientes:</span><span class="sxs-lookup"><span data-stu-id="30f89-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="30f89-189">Servicios en línea de CSP, Azure CSP y actualizaciones de licencias generales, incluido Azure (2018 de noviembre)</span><span class="sxs-lookup"><span data-stu-id="30f89-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="30f89-190">Capacidad reservada de SQL DB & flexibilidad de tamaño de instancia (2018 de agosto)</span><span class="sxs-lookup"><span data-stu-id="30f89-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="30f89-191">Suscripciones de servidor en CSP (2018 de julio)</span><span class="sxs-lookup"><span data-stu-id="30f89-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="30f89-192">Información general de Azure Reservations en CSP (2018 de mayo)</span><span class="sxs-lookup"><span data-stu-id="30f89-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="30f89-193">Otro aprendizaje útil incluye el [módulo de licencias de Azure en Partner University](https://aka.ms/azure_partner_licensing).</span><span class="sxs-lookup"><span data-stu-id="30f89-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="30f89-194">Operaciones</span><span class="sxs-lookup"><span data-stu-id="30f89-194">Operations</span></span>

- <span data-ttu-id="30f89-195">[Guía de operaciones de comercio moderno](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (actualizada): una guía completa sobre directivas clave y aspectos operativos como acuerdos, pedidos a través del centro de Partners, factura, detalles de la lista de precios, incentivos, archivo de conciliación, API/SDK, espacio aislado y servicios compartidos de asociados de Azure.</span><span class="sxs-lookup"><span data-stu-id="30f89-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="30f89-196">Moderno ofrece la matriz de la moneda del cliente y la disponibilidad del país</span><span class="sxs-lookup"><span data-stu-id="30f89-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="30f89-197">Vender Microsoft Azure instancias reservadas</span><span class="sxs-lookup"><span data-stu-id="30f89-197">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="30f89-198">Comprar reservas de Microsoft Azure en nombre de los clientes</span><span class="sxs-lookup"><span data-stu-id="30f89-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="30f89-199">Administrar las reservas de Azure en nombre de sus clientes</span><span class="sxs-lookup"><span data-stu-id="30f89-199">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="30f89-200">Facturación de las reservas de Azure</span><span class="sxs-lookup"><span data-stu-id="30f89-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="30f89-201">Cambio de tamaño de la máquina virtual para el uso máximo de reserva</span><span class="sxs-lookup"><span data-stu-id="30f89-201">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="30f89-202">API del centro de Partners (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="30f89-202">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="30f89-203">Servicios de Escritorio remoto</span><span class="sxs-lookup"><span data-stu-id="30f89-203">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="30f89-204">Ventaja híbrida de Azure</span><span class="sxs-lookup"><span data-stu-id="30f89-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="30f89-205">El [ventaja híbrida de Azure](https://azure.microsoft.com/pricing/hybrid-benefit) le ayuda a obtener más valor de las licencias de Windows Server y a ahorrar hasta un \* 47% en las máquinas virtuales.</span><span class="sxs-lookup"><span data-stu-id="30f89-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="30f89-206">Puedes usar la ventaja con las licencias de las ediciones Standard y Datacenter de Windows Server cubiertas con Software Assurance.</span><span class="sxs-lookup"><span data-stu-id="30f89-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="30f89-207">En función de la edición, puede convertir o volver a usar las licencias para ejecutar máquinas virtuales de Windows Server en Azure y pagar una tarifa de proceso base inferior (tarifas de máquinas virtuales Linux).</span><span class="sxs-lookup"><span data-stu-id="30f89-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="30f89-208">Consulte también [ventaja híbrida de Azure preguntas más frecuentes](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="30f89-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="30f89-209">\* El ahorro real puede variar en función de la región, el tipo de instancia o el uso.</span><span class="sxs-lookup"><span data-stu-id="30f89-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
