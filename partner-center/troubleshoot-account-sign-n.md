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
ms.openlocfilehash: 9622f02039360e8ab39f459c9a2fe082ec70c854
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756742"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="7055d-104">Solucionar problemas de configuración de cuenta o de renovación de MPN</span><span class="sxs-lookup"><span data-stu-id="7055d-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="7055d-105">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="7055d-105">**Appropriate roles**</span></span>

- <span data-ttu-id="7055d-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="7055d-106">Global admin</span></span>
- <span data-ttu-id="7055d-107">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="7055d-107">MPN partner admin</span></span> 
 
<span data-ttu-id="7055d-108">Estas son algunas sugerencias para solucionar problemas comunes que surgen al configurar la cuenta del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="7055d-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="7055d-109">¿Qué ocurre si está migrando desde el centro de pertenencia de socios comerciales y no puede editar los campos de información de la compañía?</span><span class="sxs-lookup"><span data-stu-id="7055d-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="7055d-110">En los casos en los que su empresa ya tiene una presencia en el centro de Partners (por ejemplo, la cuenta de CSP), se mostrará una pantalla de solo lectura.</span><span class="sxs-lookup"><span data-stu-id="7055d-110">In cases where your company already has a presence in Partner Center (say CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="7055d-111">Esta pantalla mostrará toda la información acerca de la empresa tal como existe en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="7055d-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="7055d-112">No se pueden cambiar los detalles de esta pantalla.</span><span class="sxs-lookup"><span data-stu-id="7055d-112">You can't change the details on this screen.</span></span> <span data-ttu-id="7055d-113">Esto es así por diseño y no un error.</span><span class="sxs-lookup"><span data-stu-id="7055d-113">This is by design and not an error.</span></span>

<span data-ttu-id="7055d-114">Seleccione **Aceptar** y **continúe** para continuar.</span><span class="sxs-lookup"><span data-stu-id="7055d-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="7055d-115">Si el Departamento de ti ha desactivado **registrarse en el centro de Partners**.</span><span class="sxs-lookup"><span data-stu-id="7055d-115">If the IT department has turned off **sign up for Partner Center**.</span></span>

<span data-ttu-id="7055d-116">Verá este mensaje porque los usuarios virales están deshabilitados o porque se ha deshabilitado el registro viral en el inquilino de Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7055d-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="7055d-117">El administrador global de su cuenta de Azure AD puede habilitar las características necesarias ejecutando el siguiente comando de PowerShell:</span><span class="sxs-lookup"><span data-stu-id="7055d-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="7055d-118">**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="7055d-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="7055d-119">Para obtener más información, lea [el registro de autoservicio](/azure/active-directory/users-groups-roles/directory-self-service-signup) .</span><span class="sxs-lookup"><span data-stu-id="7055d-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="7055d-120">Olvidó su contraseña</span><span class="sxs-lookup"><span data-stu-id="7055d-120">You forgot your password</span></span>

<span data-ttu-id="7055d-121">Si ha olvidado la contraseña, seleccione el vínculo **¿no puede acceder a su cuenta?** en la página de inicio de sesión.</span><span class="sxs-lookup"><span data-stu-id="7055d-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="7055d-122">Esta opción le permite restablecer la contraseña o pedir al administrador global que le asigne nuevas credenciales.</span><span class="sxs-lookup"><span data-stu-id="7055d-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="7055d-123">En la pantalla de información general, recibirá un error que indica que se ha producido algún problema</span><span class="sxs-lookup"><span data-stu-id="7055d-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="7055d-124">Este mensaje de error suele mostrarse si utiliza accidentalmente caracteres especiales, espacios o código de país en el número de teléfono de la empresa.</span><span class="sxs-lookup"><span data-stu-id="7055d-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="7055d-125">El valor especificado en el campo número de teléfono solo puede contener un máximo de 10 caracteres.</span><span class="sxs-lookup"><span data-stu-id="7055d-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="7055d-126">La compra de la tarjeta de crédito recibe un mensaje de error que indica que "el pedido se ha rechazado.</span><span class="sxs-lookup"><span data-stu-id="7055d-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="7055d-127">Compruebe la información "</span><span class="sxs-lookup"><span data-stu-id="7055d-127">Please verify your information”</span></span>


<span data-ttu-id="7055d-128">Use siempre la dirección correspondiente a su tarjeta de crédito en lugar de la entidad legal.</span><span class="sxs-lookup"><span data-stu-id="7055d-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="7055d-129">Además, asegúrese de que el código postal sea correcto y corresponda a la dirección que use.</span><span class="sxs-lookup"><span data-stu-id="7055d-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="7055d-130">Quiere cambiar de pago sin conexión a método de pago en línea</span><span class="sxs-lookup"><span data-stu-id="7055d-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="7055d-131">Tendrá que cancelar el pedido original y volver a comprar con el método de pago preferido.</span><span class="sxs-lookup"><span data-stu-id="7055d-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="7055d-132">Para cancelar un pedido:</span><span class="sxs-lookup"><span data-stu-id="7055d-132">To cancel an order:</span></span>

1. <span data-ttu-id="7055d-133">Seleccione la pestaña **ofertas de pertenencia** en el panel.</span><span class="sxs-lookup"><span data-stu-id="7055d-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="7055d-134">Seleccione **Cancelar orden**</span><span class="sxs-lookup"><span data-stu-id="7055d-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="7055d-135">Aparecerá una ventana de confirmación que debe confirmar para cancelar el pedido inicial.</span><span class="sxs-lookup"><span data-stu-id="7055d-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="7055d-136">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="7055d-136">Next steps</span></span>

- [<span data-ttu-id="7055d-137">Administrar la cuenta del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="7055d-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="7055d-138">Cómo leer el archivo de factura y concil</span><span class="sxs-lookup"><span data-stu-id="7055d-138">How to read your bill and recon file</span></span>](read-your-bill.md)
