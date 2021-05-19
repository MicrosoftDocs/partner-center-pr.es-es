---
title: Inscribirse como proveedor del Panel de control
description: Obtenga información sobre cómo inscribirse como Panel de control Proveedor de aplicaciones (CPV) en Centro de partners para que pueda integrar mejor los sistemas asociados de CSP con Centro de partners API.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 01/15/2021
ms.openlocfilehash: edc0ea8f0fda58f23cbce82bc7023a3277517cc3
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147146"
---
# <a name="enroll-as-a-control-panel-vendor-to-help-integrate-csp-partner-systems-with-partner-center-apis"></a><span data-ttu-id="8a965-103">Inscribirse como proveedor de panel de control para facilitar la integración de sistemas de partners de CSP con las API del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="8a965-103">Enroll as a Control Panel Vendor to help integrate CSP partner systems with Partner Center APIs</span></span>


<span data-ttu-id="8a965-104">**Roles apropiados**: administrador global</span><span class="sxs-lookup"><span data-stu-id="8a965-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="8a965-105">Un Panel de control Vendor (CPV) es un proveedor de software independiente que desarrolla aplicaciones para su uso por parte de asociados de Proveedor de soluciones en la nube (CSP) para permitirles integrar sus sistemas con Centro de partners API.</span><span class="sxs-lookup"><span data-stu-id="8a965-105">A Control Panel Vendor (CPV) is an independent software vendor that develops applications for use by Cloud Solution Provider (CSP) partners to enable them to integrate their systems with Partner Center APIs.</span></span> <span data-ttu-id="8a965-106">Un Panel de control proveedor no es un asociado de CSP con acceso directo al panel de Centro de partners o Centro de partners API.</span><span class="sxs-lookup"><span data-stu-id="8a965-106">A Control Panel vendor is not a CSP Partner with direct access to the Partner Center dashboard or Partner Center APIs.</span></span>

<span data-ttu-id="8a965-107">Tanto si es un proveedor de Panel de control (CPV) actual como un nuevo CPV que quiere trabajar con asociados de Microsoft, Microsoft ahora requiere que se inscriba en Centro de partners para registrar las aplicaciones y dar soporte técnico a Proveedor de soluciones en la nube asociados.</span><span class="sxs-lookup"><span data-stu-id="8a965-107">Whether you are a current Control Panel Vendor (CPV) or a new CPV who wants to work with Microsoft partners, Microsoft now requires you to enroll in Partner Center in order to register your applications and support Cloud Solution Provider partners.</span></span> <span data-ttu-id="8a965-108">Para crear una cuenta, un asociado de CPV puede usar un inquilino de asociado de CSP existente o un inquilino CPV existente o puede crear un nuevo inquilino como parte del proceso de incorporación.</span><span class="sxs-lookup"><span data-stu-id="8a965-108">To create an account, a CPV partner can either use an existing CSP partner tenant, or existing CPV tenant or can create a new tenant as part of onboarding process.</span></span> <span data-ttu-id="8a965-109">Si el asociado de CPV decide usar el inquilino de CSP existente, deberá crear aplicaciones multiinquilino independientes y registrarlas en Centro de partners para las actividades de CPV.</span><span class="sxs-lookup"><span data-stu-id="8a965-109">If the CPV partner chooses to use the existing CSP tenant, then they'll need to create separate multi-tenant applications and register them in Partner Center for CPV activities.</span></span> <span data-ttu-id="8a965-110">Una aplicación no se puede registrar como una aplicación CSP y CPV.</span><span class="sxs-lookup"><span data-stu-id="8a965-110">An application can't be registered as both a CSP and CPV application.</span></span> <span data-ttu-id="8a965-111">Una vez que se haya inscrito Centro de partners y registrado las aplicaciones, tendrá acceso a las API Centro de partners aplicaciones.</span><span class="sxs-lookup"><span data-stu-id="8a965-111">After you have enrolled in Partner Center and registered your applications, you will have access to the Partner Center APIs.</span></span>  <span data-ttu-id="8a965-112">Póngase en contacto con Microsoft a través Soporte técnico de Microsoft solicitud si necesita una cuenta de espacio aislado.</span><span class="sxs-lookup"><span data-stu-id="8a965-112">Contact Microsoft through a Microsoft Support request if you need a sandbox account.</span></span> <span data-ttu-id="8a965-113">Si ya tiene una cuenta de espacio aislado, siga usla.</span><span class="sxs-lookup"><span data-stu-id="8a965-113">If you already have a sandbox account, continue using it.</span></span> <span data-ttu-id="8a965-114">No necesitará un nuevo espacio aislado.</span><span class="sxs-lookup"><span data-stu-id="8a965-114">You won't need a new sandbox</span></span>

<span data-ttu-id="8a965-115">Revisión del [contrato Panel de control proveedor de Microsoft](https://go.microsoft.com/fwlink/?linkid=2055198)</span><span class="sxs-lookup"><span data-stu-id="8a965-115">Review the [Microsoft Control Panel Vendor agreement](https://go.microsoft.com/fwlink/?linkid=2055198)</span></span>


## <a name="working-in-partner-center"></a><span data-ttu-id="8a965-116">Uso del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="8a965-116">Working in Partner Center</span></span>

<span data-ttu-id="8a965-117">Una vez que se haya inscrito en Centro de partners experiencia de CPV y haya aceptado el contrato CPV, puede hacer lo siguiente:</span><span class="sxs-lookup"><span data-stu-id="8a965-117">Once you have enrolled in the Partner Center CPV experience and accepted the CPV agreement, you can:</span></span>

- <span data-ttu-id="8a965-118">Administrar aplicaciones multiinquilino (agregar aplicaciones para Azure Portal, registrar y anular el registro de aplicaciones en Centro de partners).</span><span class="sxs-lookup"><span data-stu-id="8a965-118">Manage multi-tenant applications (add applications to Azure portal, register, and unregister applications in Partner Center).</span></span>

    >[!Note] 
    ><span data-ttu-id="8a965-119">Las CPU deben registrar sus aplicaciones en Centro de partners para obtener autorización para Centro de partners API.</span><span class="sxs-lookup"><span data-stu-id="8a965-119">CPVs must register their applications in Partner Center in order to get authorized for Partner Center APIs.</span></span> <span data-ttu-id="8a965-120">Agregar aplicaciones a Azure Portal solo no autoriza a las aplicaciones de CPV para las Partner Center API.</span><span class="sxs-lookup"><span data-stu-id="8a965-120">Adding applications to the Azure portal alone does not authorize CPV applications for Partner Center APIs.</span></span> 

- <span data-ttu-id="8a965-121">Ver y administrar el perfil de CPV</span><span class="sxs-lookup"><span data-stu-id="8a965-121">View and manage your CPV profile</span></span> 

- <span data-ttu-id="8a965-122">Puedes ver y administrar los usuarios que necesitan acceso a las funcionalidades de CPV.</span><span class="sxs-lookup"><span data-stu-id="8a965-122">View and manage your users who need access to CPV capabilities.</span></span> <span data-ttu-id="8a965-123">El administrador global es el único rol que puede tener un CPV.</span><span class="sxs-lookup"><span data-stu-id="8a965-123">Global admin is the only role a CPV can have.</span></span>

## <a name="next-steps"></a><span data-ttu-id="8a965-124">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="8a965-124">Next steps</span></span>

<span data-ttu-id="8a965-125">-[Adición de inquilinos adicionales a Centro de partners cuenta](multi-tenant-account.md)</span><span class="sxs-lookup"><span data-stu-id="8a965-125">-[Add additional tenants to your Partner Center account](multi-tenant-account.md)</span></span>