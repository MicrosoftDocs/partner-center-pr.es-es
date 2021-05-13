---
title: Solución de problemas de configuración de la Centro de partners o de renovación de MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Solución de problemas al intentar inscribirse en Centro de partners. Las respuestas abordan desafíos con métodos de pago, olvidan las contraseñas y mucho más.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a5e8a292ad8593dc0b94179d5f0ee418344ef9af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854696"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="43564-104">Solución de problemas de configuración de la cuenta o renovación de MPN</span><span class="sxs-lookup"><span data-stu-id="43564-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="43564-105">**Roles adecuados:** Administrador global | Administrador de asociados de MPN</span><span class="sxs-lookup"><span data-stu-id="43564-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="43564-106">Estas son algunas sugerencias para solucionar problemas comunes que surgen al configurar Centro de partners cuenta.</span><span class="sxs-lookup"><span data-stu-id="43564-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="43564-107">¿Qué ocurre si va a migrar desde Partner Membership Center y no puede editar ningún campo de información de la empresa?</span><span class="sxs-lookup"><span data-stu-id="43564-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="43564-108">En los casos en los que la empresa ya tenga presencia en Centro de partners (por ejemplo, una cuenta de CSP): se mostrará una pantalla de solo lectura.</span><span class="sxs-lookup"><span data-stu-id="43564-108">In cases where your company already has a presence in Partner Center (for example, a CSP account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="43564-109">Esta pantalla mostrará toda la información sobre su empresa tal como existe en Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="43564-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="43564-110">No puede cambiar los detalles en esta pantalla.</span><span class="sxs-lookup"><span data-stu-id="43564-110">You can't change the details on this screen.</span></span> <span data-ttu-id="43564-111">Esto es por diseño y no un error.</span><span class="sxs-lookup"><span data-stu-id="43564-111">This is by design and not an error.</span></span>

<span data-ttu-id="43564-112">Seleccione **Aceptar** y **continuar** para continuar.</span><span class="sxs-lookup"><span data-stu-id="43564-112">Select **Accept** and **Continue** to proceed.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="43564-113">Si el departamento de TI ha desactivado el registro **para Centro de partners**</span><span class="sxs-lookup"><span data-stu-id="43564-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="43564-114">Verá este mensaje porque los usuarios virales están deshabilitados o porque el registro viral está deshabilitado en Azure AD inquilino.</span><span class="sxs-lookup"><span data-stu-id="43564-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure AD tenant.</span></span> <span data-ttu-id="43564-115">El administrador global de la cuenta Azure AD puede habilitar las características necesarias mediante la ejecución del siguiente comando de PowerShell:</span><span class="sxs-lookup"><span data-stu-id="43564-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="43564-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="43564-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="43564-117">Para obtener más información, lea [Registro de autoservicio.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="43564-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="43564-118">Olvidó la contraseña.</span><span class="sxs-lookup"><span data-stu-id="43564-118">You forgot your password</span></span>

<span data-ttu-id="43564-119">Si ha olvidado la contraseña, seleccione el vínculo **¿No se puede acceder a su cuenta?** en la página de inicio de sesión.</span><span class="sxs-lookup"><span data-stu-id="43564-119">If you have forgotten your password, select the **Can't access your account?** link on the sign-in page.</span></span> <span data-ttu-id="43564-120">Esta opción le permite restablecer la contraseña o pedir al administrador global que le asigne nuevas credenciales.</span><span class="sxs-lookup"><span data-stu-id="43564-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="43564-121">En la pantalla "Cuéntenos sobre su empresa", recibe el error "Algo salió mal".</span><span class="sxs-lookup"><span data-stu-id="43564-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="43564-122">Este mensaje de error suele aparecer si usa accidentalmente caracteres especiales, espacios o código de país en el número de teléfono de la empresa.</span><span class="sxs-lookup"><span data-stu-id="43564-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="43564-123">El valor especificado en el campo Número de teléfono solo puede contener un máximo de 10 caracteres.</span><span class="sxs-lookup"><span data-stu-id="43564-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="43564-124">La compra con tarjeta de crédito recibe un mensaje de error que indica que "Se rechazó el pedido.</span><span class="sxs-lookup"><span data-stu-id="43564-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="43564-125">Compruebe su información"</span><span class="sxs-lookup"><span data-stu-id="43564-125">Please verify your information”</span></span>


<span data-ttu-id="43564-126">Use siempre la dirección correspondiente a la tarjeta de crédito en lugar de la entidad legal.</span><span class="sxs-lookup"><span data-stu-id="43564-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="43564-127">Además, asegúrese de que el código postal es correcto y corresponde a la dirección que usa.</span><span class="sxs-lookup"><span data-stu-id="43564-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="43564-128">Quiere cambiar del pago sin conexión al método de pago en línea.</span><span class="sxs-lookup"><span data-stu-id="43564-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="43564-129">Deberá cancelar el pedido original y volver a comprar mediante el método de pago preferido.</span><span class="sxs-lookup"><span data-stu-id="43564-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="43564-130">Para cancelar un pedido:</span><span class="sxs-lookup"><span data-stu-id="43564-130">To cancel an order:</span></span>

1. <span data-ttu-id="43564-131">Seleccione **la pestaña Ofertas** de pertenencia en el panel.</span><span class="sxs-lookup"><span data-stu-id="43564-131">Select **Membership Offers** tab in the Dashboard.</span></span>

2. <span data-ttu-id="43564-132">Seleccione **Cancelar pedido.**</span><span class="sxs-lookup"><span data-stu-id="43564-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="43564-133">Aparecerá una ventana de confirmación y debe confirmar para cancelar el pedido inicial.</span><span class="sxs-lookup"><span data-stu-id="43564-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="43564-134">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="43564-134">Next steps</span></span>

- [<span data-ttu-id="43564-135">Administrar la cuenta del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="43564-135">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="43564-136">Cómo leer el archivo de facturación y conciliación</span><span class="sxs-lookup"><span data-stu-id="43564-136">How to read your bill and recon file</span></span>](read-your-bill.md)
