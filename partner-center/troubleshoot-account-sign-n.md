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
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Solucionar problemas de configuración de cuenta o de renovación de MPN

**Se aplica a**

- Centro de partners
 
**Roles adecuados**

- Administrador global
- Administrador de partners de MPN 
 
Estas son algunas sugerencias para solucionar problemas comunes que surgen al configurar la cuenta del centro de Partners.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>¿Qué ocurre si está migrando desde el centro de pertenencia de socios comerciales y no puede editar los campos de información de la compañía?

En los casos en los que su empresa ya tiene una presencia en el centro de Partners (por ejemplo, la cuenta de CSP), se mostrará una pantalla de solo lectura. Esta pantalla mostrará toda la información acerca de la empresa tal como existe en el centro de Partners.

No se pueden cambiar los detalles de esta pantalla. Esto es así por diseño y no un error.

Seleccione **Aceptar** y **continúe** para continuar.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Si el Departamento de ti ha desactivado **registrarse en el centro de Partners**.

Verá este mensaje porque los usuarios virales están deshabilitados o porque se ha deshabilitado el registro viral en el inquilino de Azure AD. El administrador global de su cuenta de Azure AD puede habilitar las características necesarias ejecutando el siguiente comando de PowerShell:

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

Para obtener más información, lea [el registro de autoservicio](/azure/active-directory/users-groups-roles/directory-self-service-signup) .

## <a name="you-forgot-your-password"></a>Olvidó su contraseña

Si ha olvidado la contraseña, seleccione el vínculo **¿no puede acceder a su cuenta?** en la página de inicio de sesión. Esta opción le permite restablecer la contraseña o pedir al administrador global que le asigne nuevas credenciales.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>En la pantalla de información general, recibirá un error que indica que se ha producido algún problema

Este mensaje de error suele mostrarse si utiliza accidentalmente caracteres especiales, espacios o código de país en el número de teléfono de la empresa. El valor especificado en el campo número de teléfono solo puede contener un máximo de 10 caracteres.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>La compra de la tarjeta de crédito recibe un mensaje de error que indica que "el pedido se ha rechazado. Compruebe la información "


Use siempre la dirección correspondiente a su tarjeta de crédito en lugar de la entidad legal. Además, asegúrese de que el código postal sea correcto y corresponda a la dirección que use.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>Quiere cambiar de pago sin conexión a método de pago en línea 

Tendrá que cancelar el pedido original y volver a comprar con el método de pago preferido.

Para cancelar un pedido:

1. Seleccione la pestaña **ofertas de pertenencia** en el panel.

2. Seleccione **Cancelar orden**

3. Aparecerá una ventana de confirmación que debe confirmar para cancelar el pedido inicial.

## <a name="next-steps"></a>Pasos siguientes

- [Administrar la cuenta del Centro de partners](partner-center-account-setup.md)
- [Cómo leer el archivo de factura y concil](read-your-bill.md)
