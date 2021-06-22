---
title: Solución de problemas de configuración de la Centro de partners o de renovación de MPN
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Solucionar problemas al intentar inscribirse en Centro de partners. Las respuestas abordan desafíos con métodos de pago, olvidan las contraseñas y mucho más.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4fc1a43b4d525d9221ac7e4db56f5f278404e3f5
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431748"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a><span data-ttu-id="2f03c-104">Solución de problemas de configuración de la cuenta o renovación de MPN</span><span class="sxs-lookup"><span data-stu-id="2f03c-104">Troubleshoot account setup or MPN renewal issues</span></span>

<span data-ttu-id="2f03c-105">**Roles adecuados:** Administrador global | Administrador de asociados de MPN</span><span class="sxs-lookup"><span data-stu-id="2f03c-105">**Appropriate roles**: Global admin | MPN partner admin</span></span>
 
<span data-ttu-id="2f03c-106">Estas son algunas sugerencias para solucionar problemas comunes que surgen al configurar Centro de partners cuenta.</span><span class="sxs-lookup"><span data-stu-id="2f03c-106">Here are some suggestions for troubleshooting common issues that arise when setting up your Partner Center account.</span></span>

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a><span data-ttu-id="2f03c-107">¿Qué ocurre si va a migrar desde Partner Membership Center y no puede editar ningún campo de información de la empresa?</span><span class="sxs-lookup"><span data-stu-id="2f03c-107">What happens if you are migrating from Partner Membership Center and you can't edit any company information fields</span></span>

<span data-ttu-id="2f03c-108">En los casos en los que la empresa ya tenga presencia en Centro de partners (por ejemplo, una cuenta de Proveedor de soluciones en la nube (CSP), se mostrará una pantalla de solo lectura.</span><span class="sxs-lookup"><span data-stu-id="2f03c-108">In cases where your company already has a presence in Partner Center (for example, a Cloud Solution Provider (CSP) account) – you will be shown a read-only screen.</span></span> <span data-ttu-id="2f03c-109">Esta pantalla mostrará toda la información sobre su empresa tal como existe en Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="2f03c-109">This screen will display all the information about your company as it exists in Partner Center.</span></span>

<span data-ttu-id="2f03c-110">No puede cambiar los detalles en esta pantalla.</span><span class="sxs-lookup"><span data-stu-id="2f03c-110">You can't change the details on this screen.</span></span> <span data-ttu-id="2f03c-111">Esto es por diseño y no un error.</span><span class="sxs-lookup"><span data-stu-id="2f03c-111">This is by design and not an error.</span></span>

<span data-ttu-id="2f03c-112">Para continuar, seleccione **Aceptar** y, a continuación, **seleccione Continuar.**</span><span class="sxs-lookup"><span data-stu-id="2f03c-112">To proceed, select **Accept**, and then select **Continue**.</span></span>


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a><span data-ttu-id="2f03c-113">Si el departamento de TI ha desactivado el registro **para Centro de partners**</span><span class="sxs-lookup"><span data-stu-id="2f03c-113">If the IT department has turned off **Sign up for Partner Center**</span></span>

<span data-ttu-id="2f03c-114">Verá este mensaje porque los usuarios virales están deshabilitados o porque el registro viral está deshabilitado en el inquilino Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="2f03c-114">You see this message because viral users are disabled, or because Viral Sign-up is disabled on the Azure Active Directory (AD) tenant.</span></span> <span data-ttu-id="2f03c-115">El administrador global de la cuenta Azure AD puede habilitar las características necesarias mediante la ejecución del siguiente comando de PowerShell:</span><span class="sxs-lookup"><span data-stu-id="2f03c-115">The Global admin for your Azure AD account can enable required features by running the following PowerShell command:</span></span>

<span data-ttu-id="2f03c-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span><span class="sxs-lookup"><span data-stu-id="2f03c-116">**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**</span></span>

<span data-ttu-id="2f03c-117">Para obtener más información, lea [Registro de autoservicio.](/azure/active-directory/users-groups-roles/directory-self-service-signup)</span><span class="sxs-lookup"><span data-stu-id="2f03c-117">For more information, read [Self-service sign up](/azure/active-directory/users-groups-roles/directory-self-service-signup).</span></span>

## <a name="you-forgot-your-password"></a><span data-ttu-id="2f03c-118">Olvidó la contraseña.</span><span class="sxs-lookup"><span data-stu-id="2f03c-118">You forgot your password</span></span>

<span data-ttu-id="2f03c-119">Si ha olvidado la contraseña, en la página de inicio de sesión, seleccione **¿No puede acceder a su cuenta?**.</span><span class="sxs-lookup"><span data-stu-id="2f03c-119">If you have forgotten your password, on the sign-in page, select **Can't access your account?**.</span></span> <span data-ttu-id="2f03c-120">Esta opción le permite restablecer la contraseña o pedir al administrador global que le asigne nuevas credenciales.</span><span class="sxs-lookup"><span data-stu-id="2f03c-120">This option lets you reset your password or ask your Global admin to assign you new credentials.</span></span>

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a><span data-ttu-id="2f03c-121">En la pantalla "Cuéntenos sobre su empresa", recibe el error "Algo salió mal".</span><span class="sxs-lookup"><span data-stu-id="2f03c-121">On the “Tell us about your company” screen, you receive a “Something went wrong” error</span></span>

<span data-ttu-id="2f03c-122">Este mensaje de error suele aparecer si usa accidentalmente caracteres especiales, espacios o código de país en el número de teléfono de la empresa.</span><span class="sxs-lookup"><span data-stu-id="2f03c-122">This error message usually shows up if you inadvertently use special characters, spaces, or country code in your company phone number.</span></span> <span data-ttu-id="2f03c-123">El valor especificado en el campo Número de teléfono solo puede contener un máximo de 10 caracteres.</span><span class="sxs-lookup"><span data-stu-id="2f03c-123">The value entered in the Phone Number field can only contain a maximum of 10 characters.</span></span>


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a><span data-ttu-id="2f03c-124">La compra de la tarjeta de crédito recibe un mensaje de error que indica que se ha rechazado el pedido.</span><span class="sxs-lookup"><span data-stu-id="2f03c-124">Your credit card purchase is receiving an error message stating that “Your order was declined.</span></span> <span data-ttu-id="2f03c-125">Compruebe su información"</span><span class="sxs-lookup"><span data-stu-id="2f03c-125">Please verify your information”</span></span>


<span data-ttu-id="2f03c-126">Use siempre la dirección correspondiente a la tarjeta de crédito en lugar de la entidad legal.</span><span class="sxs-lookup"><span data-stu-id="2f03c-126">Always use the address corresponding to your credit card rather than your legal entity.</span></span> <span data-ttu-id="2f03c-127">Además, asegúrese de que el código postal es correcto y corresponde a la dirección que usa.</span><span class="sxs-lookup"><span data-stu-id="2f03c-127">Also, make sure the zip code is correct and corresponds to the address you use.</span></span>

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a><span data-ttu-id="2f03c-128">Quiere cambiar del pago sin conexión al método de pago en línea.</span><span class="sxs-lookup"><span data-stu-id="2f03c-128">You want to switch from offline payment to online payment method</span></span> 

<span data-ttu-id="2f03c-129">Deberá cancelar el pedido original y volver a comprar mediante el método de pago preferido.</span><span class="sxs-lookup"><span data-stu-id="2f03c-129">You will need to cancel the original order and repurchase using the preferred payment method.</span></span>

<span data-ttu-id="2f03c-130">Para cancelar un pedido:</span><span class="sxs-lookup"><span data-stu-id="2f03c-130">To cancel an order:</span></span>

1. <span data-ttu-id="2f03c-131">En el panel Centro de partners, seleccione la pestaña **Ofertas de pertenencia.**</span><span class="sxs-lookup"><span data-stu-id="2f03c-131">In the Partner Center dashboard, select the **Membership Offers** tab.</span></span>

2. <span data-ttu-id="2f03c-132">Seleccione **Cancelar pedido.**</span><span class="sxs-lookup"><span data-stu-id="2f03c-132">Select **Cancel order**</span></span>

3. <span data-ttu-id="2f03c-133">Aparecerá una ventana de confirmación y debe confirmar para cancelar el pedido inicial.</span><span class="sxs-lookup"><span data-stu-id="2f03c-133">A confirmation window will appear and you must confirm in order to cancel the initial order.</span></span>

## <a name="next-steps"></a><span data-ttu-id="2f03c-134">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="2f03c-134">Next steps</span></span>

- [<span data-ttu-id="2f03c-135">Administrar la cuenta del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="2f03c-135">Manage your Partner Center account</span></span>](partner-center-account-setup.md)
- [<span data-ttu-id="2f03c-136">Cómo leer el archivo de facturación y conciliación</span><span class="sxs-lookup"><span data-stu-id="2f03c-136">How to read your bill and recon file</span></span>](read-your-bill.md)
