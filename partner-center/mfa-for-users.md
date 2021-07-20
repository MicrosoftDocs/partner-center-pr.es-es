---
title: Configurar los usuarios con la autenticación multifactor
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Obtenga información sobre cómo configurar a los empleados con MFA.
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9cdb83c8b58b75606275c9773cba79eba75d5d0d
ms.sourcegitcommit: 7cc83714e17337b472727819243f98c84ae181ba
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/22/2021
ms.locfileid: "112450814"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="f5c22-103">Configurar los usuarios con la autenticación multifactor</span><span class="sxs-lookup"><span data-stu-id="f5c22-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="f5c22-104">**Roles apropiados**: administrador global</span><span class="sxs-lookup"><span data-stu-id="f5c22-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="f5c22-105">Una mayor seguridad y protección de la privacidad se encuentran entre nuestras principales prioridades.</span><span class="sxs-lookup"><span data-stu-id="f5c22-105">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="f5c22-106">Sabemos que la mejor defensa es la prevención y que somos tan seguros como lo sea nuestro vínculo más débil.</span><span class="sxs-lookup"><span data-stu-id="f5c22-106">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="f5c22-107">Esta es la razón por la que necesitamos que todos los usuarios de nuestro ecosistema actúen y se aseguren de tener las protecciones de seguridad adecuadas.</span><span class="sxs-lookup"><span data-stu-id="f5c22-107">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="f5c22-108">Recomendamos encarecidamente que todos los partners habiliten la autenticación multifactor (MFA) para sus usuarios en su inquilino de partner.</span><span class="sxs-lookup"><span data-stu-id="f5c22-108">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="f5c22-109">Adición de la autenticación multifactor para los usuarios</span><span class="sxs-lookup"><span data-stu-id="f5c22-109">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="f5c22-110">Debe ser el administrador global de su empresa para poder completar esta tarea.</span><span class="sxs-lookup"><span data-stu-id="f5c22-110">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="f5c22-111">Es más fácil habilitar la MFA para los usuarios a medida que los agrega a su inquilino de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f5c22-111">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="f5c22-112">Inicie sesión en [Azure Portal](https://portal.azure.com) y, a continuación, vaya a **Administración de usuarios**.</span><span class="sxs-lookup"><span data-stu-id="f5c22-112">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="f5c22-113">Seleccione **Autenticación multifactor**.</span><span class="sxs-lookup"><span data-stu-id="f5c22-113">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="f5c22-114">Seleccione el usuario que desea habilitar y, a continuación, seleccione **Habilitar**.</span><span class="sxs-lookup"><span data-stu-id="f5c22-114">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="f5c22-115">Esto habilitará la MFA para este usuario.</span><span class="sxs-lookup"><span data-stu-id="f5c22-115">This will enable MFA for this user.</span></span> <span data-ttu-id="f5c22-116">Estar habilitado significa que al usuario se le pedirá que configure la comprobación de MFA cuando inicie sesión por primera vez.</span><span class="sxs-lookup"><span data-stu-id="f5c22-116">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="f5c22-117">A partir de ese momento, al iniciar sesión, se le pedirá que proporcione un código que se le enviará por correo electrónico o mensaje de texto (en función de la configuración).</span><span class="sxs-lookup"><span data-stu-id="f5c22-117">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/multi-factor-authentication/security-verification.png" alt-text="Especificación de cómo comprobar.":::

>[!NOTE]
><span data-ttu-id="f5c22-119">Para **exigir** que los usuarios utilicen MFA, puede seguir los mismos pasos descritos anteriormente y seleccionar **Exigir**.</span><span class="sxs-lookup"><span data-stu-id="f5c22-119">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="f5c22-120">Para obtener más información, lea [Habilitación de Azure Multi-Factor Authentication por usuario para proteger los eventos de inicio de sesión](/azure/active-directory/authentication/howto-mfa-userstates).</span><span class="sxs-lookup"><span data-stu-id="f5c22-120">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="f5c22-121">Todos los usuarios comienzan con un estado  **Deshabilitado**.</span><span class="sxs-lookup"><span data-stu-id="f5c22-121">All users start out **Disabled**.</span></span> <span data-ttu-id="f5c22-122">Cuando inscribe usuarios en Azure Active Directory Multi-Factor Authentication por usuario, su estado cambia a  **Habilitado**.</span><span class="sxs-lookup"><span data-stu-id="f5c22-122">When you enroll users in per-user Azure Active Directory Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="f5c22-123">Cuando los usuarios habilitados inician sesión y completan el proceso de registro, su estado cambia a  **Forzado**.</span><span class="sxs-lookup"><span data-stu-id="f5c22-123">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="f5c22-124">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="f5c22-124">Next steps</span></span>

- [<span data-ttu-id="f5c22-125">Asignación de roles y permisos a los usuarios</span><span class="sxs-lookup"><span data-stu-id="f5c22-125">Assign roles and permissions to users</span></span>](permissions-overview.md)