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
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Solucionar problemas de configuración de cuenta o de renovación de MPN

### <a name="applies-to"></a>Se aplica a

- Centro de partners
 
### <a name="appropriate-roles"></a>Roles adecuados

- Administrador global
- Administrador de partners de MPN 
 

Estas son algunas sugerencias para solucionar problemas comunes que surgen al configurar la cuenta del centro de Partners.

### <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>¿Qué ocurre si está migrando desde el centro de pertenencia de socios comerciales y no puede editar los campos de información de la compañía?

Esto se produce en los casos en los que su empresa ya tiene una presencia en el centro de Partners (por ejemplo, la cuenta de CSP), se mostrará una pantalla de solo lectura que mostrará toda la información sobre su empresa tal como existe en el centro de Partners.

No se pueden cambiar los detalles de esta pantalla. Esto es así por diseño y no un error.

Seleccione **Aceptar** y **continúe** para continuar.

### <a name="you-are-trying-to-enroll-or-to-migrate-from-partner-membership-center-and-you-receive-an-error-message-saying-that-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Está intentando inscribirse o migrar desde el centro de pertenencia del asociado y recibe un mensaje de error que indica que el Departamento de ti ha desactivado el **registro para el centro de Partners**. 

Verá este mensaje porque los usuarios virales están deshabilitados o se ha deshabilitado el registro viral en el inquilino de Azure AD. El administrador global de su cuenta de Azure AD puede habilitar las características necesarias ejecutando el siguiente comando de PowerShell:

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

Para obtener más información, lea [el registro de autoservicio](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-self-service-signup) .

### <a name="you-forgot-your-password"></a>Olvidó su contraseña

Si ha olvidado la contraseña, seleccione el vínculo **¿no puede acceder a su cuenta?** en la página de inicio de sesión para restablecer la contraseña o pida a su administrador global que le asigne nuevas credenciales.

### <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>En la pantalla "indíquenos sobre su empresa", recibe el error "se ha producido algún problema"

Esto suele ocurrir si utiliza accidentalmente caracteres especiales, espacios o código de país en el número de teléfono de la empresa. El valor especificado en el campo número de teléfono solo puede contener un máximo de 10 caracteres.

### <a name="you-are-trying-to-complete-the-purchase-via-credit-card-but-you-are-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Está intentando completar la compra a través de la tarjeta de crédito, pero recibe un mensaje de error que indica que "el pedido se ha rechazado. Compruebe la información "

Siempre debe insertar la dirección correspondiente a su tarjeta de crédito y que no corresponda a su entidad legal. Además, asegúrese de que el código postal sea correcto y corresponda a la dirección que use.

### <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Quiere cambiar de pago sin conexión a método de pago en línea 

Tendrá que cancelar el pedido original y volver a comprar con el método de pago preferido.

Para cancelar un pedido:

1. Seleccione la pestaña **ofertas de pertenencia** en el panel.

2. Seleccione **Cancelar orden**

3. Aparecerá una ventana de confirmación que debe confirmar para cancelar el pedido inicial.
