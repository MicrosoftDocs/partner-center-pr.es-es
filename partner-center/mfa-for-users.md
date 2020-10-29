---
title: Configurar los usuarios con la autenticación multifactor
ms.topic: how-to
ms.date: 10/23/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Obtenga información sobre cómo configurar a los empleados con MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 5e31fe8f65d8d676b7e0745f7747865493bbe3ee
ms.sourcegitcommit: 4a88db7e9e90b4fbb2ba82af38d7f77b016977f3
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/24/2020
ms.locfileid: "92526010"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="7667b-103">Configurar los usuarios con la autenticación multifactor</span><span class="sxs-lookup"><span data-stu-id="7667b-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="7667b-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="7667b-104">**Appropriate roles**</span></span>

- <span data-ttu-id="7667b-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="7667b-105">Global admin</span></span>

<span data-ttu-id="7667b-106">Una mayor seguridad y protección de la privacidad se encuentran entre nuestras principales prioridades.</span><span class="sxs-lookup"><span data-stu-id="7667b-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="7667b-107">Sabemos que la mejor defensa es la prevención y que somos tan seguros como lo sea nuestro vínculo más débil.</span><span class="sxs-lookup"><span data-stu-id="7667b-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="7667b-108">Esta es la razón por la que necesitamos que todos los usuarios de nuestro ecosistema actúen y se aseguren de tener las protecciones de seguridad adecuadas.</span><span class="sxs-lookup"><span data-stu-id="7667b-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="7667b-109">Para ayudar a proteger a los partners y clientes, presentamos un conjunto de requisitos de seguridad obligatorios para los asesores, proveedores de panel de control y asociados que participen en el programa Proveedor de soluciones en la nube.</span><span class="sxs-lookup"><span data-stu-id="7667b-109">To help safeguard partners and customers, we are introducing a set of mandatory security requirements for Advisors, Control Panel Vendors, and partners participating in the Cloud Solution Provider program.</span></span>

<span data-ttu-id="7667b-110">Los partners tienen la obligación de aplicar la autenticación multifactor (MFA) a todas las cuentas de usuario en su inquilino de partner.</span><span class="sxs-lookup"><span data-stu-id="7667b-110">Partners are required to enforce multi-factor authentication (MFA) for all user accounts in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="7667b-111">Adición de la autenticación multifactor para los usuarios</span><span class="sxs-lookup"><span data-stu-id="7667b-111">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="7667b-112">Debe ser el administrador global de su empresa para poder completar esta tarea.</span><span class="sxs-lookup"><span data-stu-id="7667b-112">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="7667b-113">Es más fácil habilitar la MFA para los usuarios a medida que los agrega a su inquilino de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7667b-113">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="7667b-114">Inicie sesión en [Azure Portal](https://portal.azure.com) y, a continuación, vaya a **Administración de usuarios** .</span><span class="sxs-lookup"><span data-stu-id="7667b-114">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management** .</span></span>
1. <span data-ttu-id="7667b-115">Seleccione **Autenticación multifactor** .</span><span class="sxs-lookup"><span data-stu-id="7667b-115">Select **Multi-factor authentication** .</span></span>
1. <span data-ttu-id="7667b-116">Seleccione el usuario que desea habilitar y, a continuación, seleccione **Habilitar** .</span><span class="sxs-lookup"><span data-stu-id="7667b-116">Select the user you want to enable and then select **Enable** .</span></span>

<span data-ttu-id="7667b-117">Esto habilitará la MFA para este usuario.</span><span class="sxs-lookup"><span data-stu-id="7667b-117">This will enable MFA for this user.</span></span> <span data-ttu-id="7667b-118">Estar habilitado significa que al usuario se le pedirá que configure la comprobación de MFA cuando inicie sesión por primera vez.</span><span class="sxs-lookup"><span data-stu-id="7667b-118">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="7667b-119">A partir de ese momento, al iniciar sesión, se le pedirá que proporcione un código que se le enviará por correo electrónico o mensaje de texto.</span><span class="sxs-lookup"><span data-stu-id="7667b-119">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message.</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Especificación de cómo comprobar":::

<span data-ttu-id="7667b-121">Para obligar a los usuarios a usar MFA, puede **aplicar** siguiendo los mismos pasos descritos anteriormente y seleccionar **Forzar** .</span><span class="sxs-lookup"><span data-stu-id="7667b-121">To force users to use MFA, you can **Enforce** using same steps as above and selecting **Enforce** .</span></span> <span data-ttu-id="7667b-122">Para obtener más información, lea [Habilitación de Azure Multi-Factor Authentication por usuario para proteger los eventos de inicio de sesión](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span><span class="sxs-lookup"><span data-stu-id="7667b-122">Learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="7667b-123">Todos los usuarios comienzan con un estado  **Deshabilitado** .</span><span class="sxs-lookup"><span data-stu-id="7667b-123">All users start out **Disabled** .</span></span> <span data-ttu-id="7667b-124">Cuando inscribe usuarios en Azure Multi-Factor Authentication por usuario, su estado cambia a  **Habilitado** .</span><span class="sxs-lookup"><span data-stu-id="7667b-124">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled** .</span></span> <span data-ttu-id="7667b-125">Cuando los usuarios habilitados inician sesión y completan el proceso de registro, su estado cambia a  **Forzado** .</span><span class="sxs-lookup"><span data-stu-id="7667b-125">When enabled users sign in and complete the registration process, their state changes to **Enforced** .</span></span> 

## <a name="next-steps"></a><span data-ttu-id="7667b-126">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="7667b-126">Next steps</span></span>

- [<span data-ttu-id="7667b-127">Asignación de roles y permisos a los usuarios</span><span class="sxs-lookup"><span data-stu-id="7667b-127">Assign roles and permissions to users</span></span>](permissions-overview.md)



