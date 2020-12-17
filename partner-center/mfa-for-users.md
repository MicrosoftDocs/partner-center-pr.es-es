---
title: Configurar los usuarios con la autenticación multifactor
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Obtenga información sobre cómo configurar a los empleados con MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 355258fd20f867052fa8598e688630005262bb16
ms.sourcegitcommit: ab2ca3c5990b7f920df4ecb9c611d5b1046ec111
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 12/16/2020
ms.locfileid: "97578296"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="1d529-103">Configurar los usuarios con la autenticación multifactor</span><span class="sxs-lookup"><span data-stu-id="1d529-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="1d529-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="1d529-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1d529-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1d529-105">Global admin</span></span>

<span data-ttu-id="1d529-106">Una mayor seguridad y protección de la privacidad se encuentran entre nuestras principales prioridades.</span><span class="sxs-lookup"><span data-stu-id="1d529-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="1d529-107">Sabemos que la mejor defensa es la prevención y que somos tan seguros como lo sea nuestro vínculo más débil.</span><span class="sxs-lookup"><span data-stu-id="1d529-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="1d529-108">Esta es la razón por la que necesitamos que todos los usuarios de nuestro ecosistema actúen y se aseguren de tener las protecciones de seguridad adecuadas.</span><span class="sxs-lookup"><span data-stu-id="1d529-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="1d529-109">Recomendamos encarecidamente que todos los partners habiliten la autenticación multifactor (MFA) para sus usuarios en su inquilino de partner.</span><span class="sxs-lookup"><span data-stu-id="1d529-109">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="1d529-110">Adición de la autenticación multifactor para los usuarios</span><span class="sxs-lookup"><span data-stu-id="1d529-110">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="1d529-111">Debe ser el administrador global de su empresa para poder completar esta tarea.</span><span class="sxs-lookup"><span data-stu-id="1d529-111">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="1d529-112">Es más fácil habilitar la MFA para los usuarios a medida que los agrega a su inquilino de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1d529-112">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="1d529-113">Inicie sesión en [Azure Portal](https://portal.azure.com) y, a continuación, vaya a **Administración de usuarios**.</span><span class="sxs-lookup"><span data-stu-id="1d529-113">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="1d529-114">Seleccione **Autenticación multifactor**.</span><span class="sxs-lookup"><span data-stu-id="1d529-114">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="1d529-115">Seleccione el usuario que desea habilitar y, a continuación, seleccione **Habilitar**.</span><span class="sxs-lookup"><span data-stu-id="1d529-115">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="1d529-116">Esto habilitará la MFA para este usuario.</span><span class="sxs-lookup"><span data-stu-id="1d529-116">This will enable MFA for this user.</span></span> <span data-ttu-id="1d529-117">Estar habilitado significa que al usuario se le pedirá que configure la comprobación de MFA cuando inicie sesión por primera vez.</span><span class="sxs-lookup"><span data-stu-id="1d529-117">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="1d529-118">A partir de ese momento, al iniciar sesión, se le pedirá que proporcione un código que se le enviará por correo electrónico o mensaje de texto (en función de la configuración).</span><span class="sxs-lookup"><span data-stu-id="1d529-118">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Especificación de cómo comprobar":::

>[!NOTE]
><span data-ttu-id="1d529-120">Para **exigir** que los usuarios utilicen MFA, puede seguir los mismos pasos descritos anteriormente y seleccionar **Exigir**.</span><span class="sxs-lookup"><span data-stu-id="1d529-120">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="1d529-121">Para obtener más información, lea [Habilitación de Azure Multi-Factor Authentication por usuario para proteger los eventos de inicio de sesión](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span><span class="sxs-lookup"><span data-stu-id="1d529-121">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="1d529-122">Todos los usuarios comienzan con un estado  **Deshabilitado**.</span><span class="sxs-lookup"><span data-stu-id="1d529-122">All users start out **Disabled**.</span></span> <span data-ttu-id="1d529-123">Cuando inscribe usuarios en Azure Multi-Factor Authentication por usuario, su estado cambia a  **Habilitado**.</span><span class="sxs-lookup"><span data-stu-id="1d529-123">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="1d529-124">Cuando los usuarios habilitados inician sesión y completan el proceso de registro, su estado cambia a  **Forzado**.</span><span class="sxs-lookup"><span data-stu-id="1d529-124">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="1d529-125">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="1d529-125">Next steps</span></span>

- [<span data-ttu-id="1d529-126">Asignación de roles y permisos a los usuarios</span><span class="sxs-lookup"><span data-stu-id="1d529-126">Assign roles and permissions to users</span></span>](permissions-overview.md)

