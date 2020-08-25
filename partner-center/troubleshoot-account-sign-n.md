---
title: Solución de problemas de configuración de la cuenta del centro de Partners o problemas de renovación de MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Solucionar problemas de inscripción en el centro de Partners
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a516d569791356c4ba967b8835268562d1597a16
ms.sourcegitcommit: 9bbad472a86086eec684f3b7f4568fdf152f625e
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/25/2020
ms.locfileid: "88848952"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="1215d-103">Solucionar problemas de configuración de cuenta o de renovación de MPN</span><span class="sxs-lookup"><span data-stu-id="1215d-103">Troubleshoot account setup or MPN renewal issues</span></span>

### <a name="applies-to"></a><span data-ttu-id="1215d-104">Se aplica a</span><span class="sxs-lookup"><span data-stu-id="1215d-104">Applies to</span></span>

- <span data-ttu-id="1215d-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="1215d-105">Partner Center</span></span>
 
### <a name="appropriate-roles"></a><span data-ttu-id="1215d-106">Roles adecuados</span><span class="sxs-lookup"><span data-stu-id="1215d-106">Appropriate roles</span></span>

- <span data-ttu-id="1215d-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1215d-107">Global admin</span></span>
- <span data-ttu-id="1215d-108">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="1215d-108">MPN partner admin</span></span> 
 

<span data-ttu-id="1215d-109">Estas son algunas sugerencias para solucionar problemas comunes que surgen al configurar la cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="1215d-109">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

### <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="1215d-110">¿Qué ocurre si está migrando desde el centro de pertenencia de socios comerciales y no puede editar los campos de información de la compañía?</span><span class="sxs-lookup"><span data-stu-id="1215d-110">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="1215d-111">Esto se produce en los casos en los que su empresa ya tiene una presencia en el centro de Partners (por ejemplo, la cuenta de CSP), se mostrará una pantalla de solo lectura que mostrará toda la información sobre su empresa tal como existe en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="1215d-111">This occurs in cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen which will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="1215d-112">No se pueden cambiar los detalles de esta pantalla.</span><span class="sxs-lookup"><span data-stu-id="1215d-112">You cannot change the details on this screen.</span></span> <span data-ttu-id="1215d-113">Esto es así por diseño y no un error.</span><span class="sxs-lookup"><span data-stu-id="1215d-113">This is by design and not an error.</span></span>

<span data-ttu-id="1215d-114">Seleccione **Aceptar** y **continúe** para continuar.</span><span class="sxs-lookup"><span data-stu-id="1215d-114">Select **Accept** and **Continue** to proceed.</span></span>

### <a name="you-are-trying-to-enroll-or-to-migrate-from-partner-membership-center-and-you-receive-an-error-message-saying-that-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="1215d-115">Está intentando inscribirse o migrar desde el centro de pertenencia del asociado y recibe un mensaje de error que indica que el Departamento de ti ha desactivado el **registro para el centro de Partners**.</span><span class="sxs-lookup"><span data-stu-id="1215d-115">You are trying to enroll or to migrate from Partner Membership Center and you receive an error message saying that the IT department has turned off **sign up for Partner Center**.</span></span> 

<span data-ttu-id="1215d-116">Verá este mensaje porque los usuarios virales están deshabilitados o se ha deshabilitado el registro viral en el inquilino de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1215d-116">You see this message because viral users are disabled, or Viral Sign up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="1215d-117">El administrador global de su cuenta de Azure AD puede habilitar las características necesarias ejecutando el siguiente comando de PowerShell:</span><span class="sxs-lookup"><span data-stu-id="1215d-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="1215d-118">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="1215d-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="1215d-119">Para obtener más información, lea [el registro de autoservicio](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup) .</span><span class="sxs-lookup"><span data-stu-id="1215d-119">For more information, read [Self-service sign up](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

### <a name="you-forgot-your-password"></a><span data-ttu-id="1215d-120">Olvidó su contraseña</span><span class="sxs-lookup"><span data-stu-id="1215d-120">You forgot your password</span></span>

<span data-ttu-id="1215d-121">Si ha olvidado la contraseña, seleccione el vínculo **¿no puede acceder a su cuenta?** en la página de inicio de sesión para restablecer la contraseña o pida a su administrador global que le asigne nuevas credenciales.</span><span class="sxs-lookup"><span data-stu-id="1215d-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page to reset your password, or ask your Global admin to assign you new credentials.</span></span>

### <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="1215d-122">En la pantalla "indíquenos sobre su empresa", recibe el error "se ha producido algún problema"</span><span class="sxs-lookup"><span data-stu-id="1215d-122">On the “Tell us about your company” screen you receive a “Something went wrong” error</span></span>

<span data-ttu-id="1215d-123">Esto suele ocurrir si utiliza accidentalmente caracteres especiales, espacios o código de país en el número de teléfono de la empresa.</span><span class="sxs-lookup"><span data-stu-id="1215d-123">This usually happens if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="1215d-124">El valor especificado en el campo número de teléfono solo puede contener un máximo de 10 caracteres.</span><span class="sxs-lookup"><span data-stu-id="1215d-124">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>

### <a name="you-are-trying-to-complete-the-purchase-via-credit-card-but-you-are-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="1215d-125">Está intentando completar la compra a través de la tarjeta de crédito, pero recibe un mensaje de error que indica que "el pedido se ha rechazado.</span><span class="sxs-lookup"><span data-stu-id="1215d-125">You are trying to complete the purchase via credit card, but you are receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="1215d-126">Compruebe la información "</span><span class="sxs-lookup"><span data-stu-id="1215d-126">Please verify your information”</span></span>

<span data-ttu-id="1215d-127">Siempre debe insertar la dirección correspondiente a su tarjeta de crédito y que no corresponda a su entidad legal.</span><span class="sxs-lookup"><span data-stu-id="1215d-127">You should always insert the address corresponding to your credit card and not corresponding to your legal entity.</span></span> <span data-ttu-id="1215d-128">Además, asegúrese de que el código postal sea correcto y corresponda a la dirección que use.</span><span class="sxs-lookup"><span data-stu-id="1215d-128">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

### <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="1215d-129">Quiere cambiar de pago sin conexión a método de pago en línea</span><span class="sxs-lookup"><span data-stu-id="1215d-129">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="1215d-130">Tendrá que cancelar el pedido original y volver a comprar con el método de pago preferido.</span><span class="sxs-lookup"><span data-stu-id="1215d-130">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="1215d-131">Para cancelar un pedido:</span><span class="sxs-lookup"><span data-stu-id="1215d-131">To cancel an order:</span></span>

1. <span data-ttu-id="1215d-132">Seleccione la pestaña **ofertas de pertenencia** en el panel.</span><span class="sxs-lookup"><span data-stu-id="1215d-132">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="1215d-133">Seleccione **Cancelar orden**</span><span class="sxs-lookup"><span data-stu-id="1215d-133">Select **Cancel order**</span></span>

3. <span data-ttu-id="1215d-134">Aparecerá una ventana de confirmación que debe confirmar para cancelar el pedido inicial.</span><span class="sxs-lookup"><span data-stu-id="1215d-134">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>
