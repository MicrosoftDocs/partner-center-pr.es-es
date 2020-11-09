---
title: Solución de problemas de configuración de la cuenta del centro de Partners o problemas de renovación de MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Solucionar problemas al intentar inscribirse en el centro de Partners. Responde a los desafíos relacionados con los métodos de pago, olvidar las contraseñas, etc.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6bf3e3af8e0d1d87a63f86e892d8bddcd74b6460
ms.sourcegitcommit: 0e142b4fbb044fe8dd2dbc7d13ab70a1a91b9f60
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/09/2020
ms.locfileid: "94381416"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="50681-104">Solucionar problemas de configuración de cuenta o de renovación de MPN</span><span class="sxs-lookup"><span data-stu-id="50681-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="50681-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="50681-105">**Applies to**</span></span>

- <span data-ttu-id="50681-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="50681-106">Partner Center</span></span>
 
<span data-ttu-id="50681-107">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="50681-107">**Appropriate roles**</span></span>

- <span data-ttu-id="50681-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="50681-108">Global admin</span></span>
- <span data-ttu-id="50681-109">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="50681-109">MPN partner admin</span></span> 
 
<span data-ttu-id="50681-110">Estas son algunas sugerencias para solucionar problemas comunes que surgen al configurar la cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="50681-110">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="50681-111">¿Qué ocurre si está migrando desde el centro de pertenencia de socios comerciales y no puede editar los campos de información de la compañía?</span><span class="sxs-lookup"><span data-stu-id="50681-111">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="50681-112">En los casos en los que su empresa ya tiene una presencia en el centro de Partners (por ejemplo, la cuenta de CSP), se mostrará una pantalla de solo lectura.</span><span class="sxs-lookup"><span data-stu-id="50681-112">In cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="50681-113">Esta pantalla mostrará toda la información acerca de la empresa tal como existe en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="50681-113">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="50681-114">No se pueden cambiar los detalles de esta pantalla.</span><span class="sxs-lookup"><span data-stu-id="50681-114">You can't change the details on this screen.</span></span> <span data-ttu-id="50681-115">Esto es así por diseño y no un error.</span><span class="sxs-lookup"><span data-stu-id="50681-115">This is by design and not an error.</span></span>

<span data-ttu-id="50681-116">Seleccione **Aceptar** y **continúe** para continuar.</span><span class="sxs-lookup"><span data-stu-id="50681-116">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="50681-117">Si el Departamento de ti ha desactivado **registrarse en el centro de Partners**.</span><span class="sxs-lookup"><span data-stu-id="50681-117">If the IT department has turned off **sign up for Partner Center**.</span></span>

<span data-ttu-id="50681-118">Verá este mensaje porque los usuarios virales están deshabilitados o porque se ha deshabilitado el registro viral en el inquilino de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50681-118">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="50681-119">El administrador global de su cuenta de Azure AD puede habilitar las características necesarias ejecutando el siguiente comando de PowerShell:</span><span class="sxs-lookup"><span data-stu-id="50681-119">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="50681-120">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="50681-120">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="50681-121">Para obtener más información, lea [el registro de autoservicio](/azure/active-directory/users-groups-roles/directory-self-service-signup) .</span><span class="sxs-lookup"><span data-stu-id="50681-121">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="50681-122">Olvidó su contraseña</span><span class="sxs-lookup"><span data-stu-id="50681-122">You forgot your password</span></span>

<span data-ttu-id="50681-123">Si ha olvidado la contraseña, seleccione el vínculo **¿no puede acceder a su cuenta?** en la página de inicio de sesión.</span><span class="sxs-lookup"><span data-stu-id="50681-123">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="50681-124">Esta opción le permite restablecer la contraseña o pedir al administrador global que le asigne nuevas credenciales.</span><span class="sxs-lookup"><span data-stu-id="50681-124">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="50681-125">En la pantalla de información general, recibirá un error que indica que se ha producido algún problema</span><span class="sxs-lookup"><span data-stu-id="50681-125">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="50681-126">Este mensaje de error suele mostrarse si utiliza accidentalmente caracteres especiales, espacios o código de país en el número de teléfono de la empresa.</span><span class="sxs-lookup"><span data-stu-id="50681-126">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="50681-127">El valor especificado en el campo número de teléfono solo puede contener un máximo de 10 caracteres.</span><span class="sxs-lookup"><span data-stu-id="50681-127">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="50681-128">La compra de la tarjeta de crédito recibe un mensaje de error que indica que "el pedido se ha rechazado.</span><span class="sxs-lookup"><span data-stu-id="50681-128">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="50681-129">Compruebe la información "</span><span class="sxs-lookup"><span data-stu-id="50681-129">Please verify your information”</span></span>


<span data-ttu-id="50681-130">Use siempre la dirección correspondiente a su tarjeta de crédito en lugar de la entidad legal.</span><span class="sxs-lookup"><span data-stu-id="50681-130">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="50681-131">Además, asegúrese de que el código postal sea correcto y corresponda a la dirección que use.</span><span class="sxs-lookup"><span data-stu-id="50681-131">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="50681-132">Quiere cambiar de pago sin conexión a método de pago en línea</span><span class="sxs-lookup"><span data-stu-id="50681-132">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="50681-133">Tendrá que cancelar el pedido original y volver a comprar con el método de pago preferido.</span><span class="sxs-lookup"><span data-stu-id="50681-133">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="50681-134">Para cancelar un pedido:</span><span class="sxs-lookup"><span data-stu-id="50681-134">To cancel an order:</span></span>

1. <span data-ttu-id="50681-135">Seleccione la pestaña **ofertas de pertenencia** en el panel.</span><span class="sxs-lookup"><span data-stu-id="50681-135">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="50681-136">Seleccione **Cancelar orden**</span><span class="sxs-lookup"><span data-stu-id="50681-136">Select **Cancel order**</span></span>

3. <span data-ttu-id="50681-137">Aparecerá una ventana de confirmación que debe confirmar para cancelar el pedido inicial.</span><span class="sxs-lookup"><span data-stu-id="50681-137">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="50681-138">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="50681-138">Next steps</span></span>

- [<span data-ttu-id="50681-139">Administrar la cuenta del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="50681-139">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="50681-140">Cómo leer el archivo de factura y concil</span><span class="sxs-lookup"><span data-stu-id="50681-140">How to read your bill and recon file</span></span>](read-your-bill.md)
