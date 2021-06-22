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
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Solución de problemas de configuración de la cuenta o renovación de MPN

**Roles adecuados:** Administrador global | Administrador de asociados de MPN
 
Estas son algunas sugerencias para solucionar problemas comunes que surgen al configurar Centro de partners cuenta.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>¿Qué ocurre si va a migrar desde Partner Membership Center y no puede editar ningún campo de información de la empresa?

En los casos en los que la empresa ya tenga presencia en Centro de partners (por ejemplo, una cuenta de Proveedor de soluciones en la nube (CSP), se mostrará una pantalla de solo lectura. Esta pantalla mostrará toda la información sobre su empresa tal como existe en Centro de partners.

No puede cambiar los detalles en esta pantalla. Esto es por diseño y no un error.

Para continuar, seleccione **Aceptar** y, a continuación, **seleccione Continuar.**


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Si el departamento de TI ha desactivado el registro **para Centro de partners**

Verá este mensaje porque los usuarios virales están deshabilitados o porque el registro viral está deshabilitado en el inquilino Azure Active Directory (AD). El administrador global de la cuenta Azure AD puede habilitar las características necesarias mediante la ejecución del siguiente comando de PowerShell:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Para obtener más información, lea [Registro de autoservicio.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>Olvidó la contraseña.

Si ha olvidado la contraseña, en la página de inicio de sesión, seleccione **¿No puede acceder a su cuenta?**. Esta opción le permite restablecer la contraseña o pedir al administrador global que le asigne nuevas credenciales.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>En la pantalla "Cuéntenos sobre su empresa", recibe el error "Algo salió mal".

Este mensaje de error suele aparecer si usa accidentalmente caracteres especiales, espacios o código de país en el número de teléfono de la empresa. El valor especificado en el campo Número de teléfono solo puede contener un máximo de 10 caracteres.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>La compra de la tarjeta de crédito recibe un mensaje de error que indica que se ha rechazado el pedido. Compruebe su información"


Use siempre la dirección correspondiente a la tarjeta de crédito en lugar de la entidad legal. Además, asegúrese de que el código postal es correcto y corresponde a la dirección que usa.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Quiere cambiar del pago sin conexión al método de pago en línea. 

Deberá cancelar el pedido original y volver a comprar mediante el método de pago preferido.

Para cancelar un pedido:

1. En el panel Centro de partners, seleccione la pestaña **Ofertas de pertenencia.**

2. Seleccione **Cancelar pedido.**

3. Aparecerá una ventana de confirmación y debe confirmar para cancelar el pedido inicial.

## <a name="next-steps"></a>Pasos siguientes

- [Administrar la cuenta del Centro de partners](partner-center-account-setup.md)
- [Cómo leer el archivo de facturación y conciliación](read-your-bill.md)
