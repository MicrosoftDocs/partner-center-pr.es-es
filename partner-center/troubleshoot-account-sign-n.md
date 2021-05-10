---
title: Solución de problemas de configuración de la Centro de partners o de renovación de MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Solucione problemas al intentar inscribirse en Centro de partners. Las respuestas abordan los desafíos con los métodos de pago, las contraseñas y mucho más.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f34adc57e668caecb69af37afc72b5153f667335
ms.sourcegitcommit: 08a175c06ff4c6a2b12713f081adfa489e16e7a1
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/10/2021
ms.locfileid: "109686269"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="852fe-104">Solución de problemas de configuración de cuentas o renovación de MPN</span><span class="sxs-lookup"><span data-stu-id="852fe-104">Troubleshoot account setup or MPN renewal issues</span></span>


<span data-ttu-id="852fe-105">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="852fe-105">**Appropriate roles**</span></span>

- <span data-ttu-id="852fe-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="852fe-106">Global admin</span></span>
- <span data-ttu-id="852fe-107">Administrador de partners de MPN</span><span class="sxs-lookup"><span data-stu-id="852fe-107">MPN partner admin</span></span>
 
<span data-ttu-id="852fe-108">Estas son algunas sugerencias para solucionar problemas comunes que surgen al configurar la cuenta Centro de partners usuario.</span><span class="sxs-lookup"><span data-stu-id="852fe-108">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="852fe-109">¿Qué ocurre si va a migrar desde Partner Membership Center no puede editar ningún campo de información de empresa?</span><span class="sxs-lookup"><span data-stu-id="852fe-109">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="852fe-110">En los casos en los que la empresa ya tenga presencia en Centro de partners (por ejemplo, una cuenta de CSP): se mostrará una pantalla de solo lectura.</span><span class="sxs-lookup"><span data-stu-id="852fe-110">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="852fe-111">Esta pantalla mostrará toda la información sobre su empresa tal como existe en Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="852fe-111">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="852fe-112">No puede cambiar los detalles en esta pantalla.</span><span class="sxs-lookup"><span data-stu-id="852fe-112">You can't change the details on this screen.</span></span> <span data-ttu-id="852fe-113">Esto es por diseño y no un error.</span><span class="sxs-lookup"><span data-stu-id="852fe-113">This is by design and not an error.</span></span>

<span data-ttu-id="852fe-114">Seleccione **Aceptar** y **continuar** para continuar.</span><span class="sxs-lookup"><span data-stu-id="852fe-114">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="852fe-115">Si el departamento de TI ha desactivado **el registro para Centro de partners**</span><span class="sxs-lookup"><span data-stu-id="852fe-115">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="852fe-116">Verá este mensaje porque los usuarios virales están deshabilitados o porque el registro viral está deshabilitado en Azure AD inquilino.</span><span class="sxs-lookup"><span data-stu-id="852fe-116">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="852fe-117">El administrador global de la cuenta Azure AD puede habilitar las características necesarias mediante la ejecución del siguiente comando de PowerShell:</span><span class="sxs-lookup"><span data-stu-id="852fe-117">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="852fe-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="852fe-118">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="852fe-119">Para obtener más información, lea [Registro de autoservicio.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="852fe-119">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="852fe-120">Olvidó la contraseña.</span><span class="sxs-lookup"><span data-stu-id="852fe-120">You forgot your password</span></span>

<span data-ttu-id="852fe-121">Si ha olvidado la contraseña, seleccione el vínculo **¿No se puede acceder a su cuenta?** en la página de inicio de sesión.</span><span class="sxs-lookup"><span data-stu-id="852fe-121">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="852fe-122">Esta opción le permite restablecer la contraseña o pedir al administrador global que le asigne nuevas credenciales.</span><span class="sxs-lookup"><span data-stu-id="852fe-122">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="852fe-123">En la pantalla "Cuéntenos sobre su empresa", recibe el error "Algo salió mal".</span><span class="sxs-lookup"><span data-stu-id="852fe-123">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="852fe-124">Este mensaje de error suele aparecer si usa accidentalmente caracteres especiales, espacios o código de país en el número de teléfono de la empresa.</span><span class="sxs-lookup"><span data-stu-id="852fe-124">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="852fe-125">El valor especificado en el campo Número de teléfono solo puede contener un máximo de 10 caracteres.</span><span class="sxs-lookup"><span data-stu-id="852fe-125">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="852fe-126">La compra de la tarjeta de crédito recibe un mensaje de error que indica que se ha rechazado el pedido.</span><span class="sxs-lookup"><span data-stu-id="852fe-126">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="852fe-127">Compruebe su información"</span><span class="sxs-lookup"><span data-stu-id="852fe-127">Please verify your information”</span></span>


<span data-ttu-id="852fe-128">Use siempre la dirección correspondiente a la tarjeta de crédito en lugar de la entidad legal.</span><span class="sxs-lookup"><span data-stu-id="852fe-128">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="852fe-129">Además, asegúrese de que el código postal es correcto y corresponde a la dirección que usa.</span><span class="sxs-lookup"><span data-stu-id="852fe-129">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="852fe-130">Quiere cambiar del pago sin conexión al método de pago en línea.</span><span class="sxs-lookup"><span data-stu-id="852fe-130">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="852fe-131">Deberá cancelar el pedido original y volver a comprar mediante el método de pago preferido.</span><span class="sxs-lookup"><span data-stu-id="852fe-131">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="852fe-132">Para cancelar un pedido:</span><span class="sxs-lookup"><span data-stu-id="852fe-132">To cancel an order:</span></span>

1. <span data-ttu-id="852fe-133">Seleccione **la pestaña Ofertas de** pertenencia en el panel.</span><span class="sxs-lookup"><span data-stu-id="852fe-133">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="852fe-134">Seleccione **Cancelar pedido.**</span><span class="sxs-lookup"><span data-stu-id="852fe-134">Select **Cancel order**</span></span>

3. <span data-ttu-id="852fe-135">Aparecerá una ventana de confirmación y debe confirmar para cancelar el pedido inicial.</span><span class="sxs-lookup"><span data-stu-id="852fe-135">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="852fe-136">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="852fe-136">Next steps</span></span>

- [<span data-ttu-id="852fe-137">Administrar la cuenta del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="852fe-137">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="852fe-138">Cómo leer el archivo de facturación y conciliación</span><span class="sxs-lookup"><span data-stu-id="852fe-138">How to read your bill and recon file</span></span>](read-your-bill.md)
