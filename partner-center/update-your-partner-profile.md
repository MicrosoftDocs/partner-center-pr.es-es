---
title: Comprobación del perfil de la empresa
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtén información sobre cómo comprobar la información de tu empresa, como el contacto principal, la dirección y la información del programa. También puedes actualizar el domicilio legal y la dirección de facturación.
author: parthpandyaMSFT
ms.author: parthp
ms.topic: how-to
ms.date: 04/12/2021
ms.localizationpriority: medium
ms.custom: contperf-fy21q4
ms.openlocfilehash: 9f9a055ce3bfbff568287267b74b04e8f9d03ad1
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080629"
---
# <a name="verify-or-update-your-company-profile-information"></a>Comprobar o actualizar la información del perfil de empresa 

**Roles apropiados**: administrador global | administrador de cuentas de MPN

La primera vez que inicies sesión en el Centro de partners como administrador global, tienes que confirmar que todos los detalles de la compañía son correctos. Estos incluyen el contacto principal, la denominación y la dirección legal de la empresa y la información del programa. Si tu empresa tiene más de una ubicación, revisa los datos de ubicación para comprobar su precisión. Como administrador global, administrador de facturación o agente de administración, también podrás ver y actualizar la información de facturación y de impuestos.

> [!NOTE]
> Debe ser el administrador global para actualizar la dirección de facturación.

Tu perfil de partner está formado por la información legal de la empresa, el nombre y el correo electrónico de contacto principal, los programas en los que participa la empresa y, si procede, las demás compañías que incluye la denominación legal de tu empresa. Asegúrese de que el nombre y la dirección de la compañía del perfil legal de la empresa no tengan errores ortográficos ni abreviaturas, y de que coincidan exactamente con los registros de inscripción formales de la compañía. Si trabaja como un solo propietario, debe usar el nombre de su empresa como razón social.


## <a name="locate-the-legal-business-profile"></a>Búsqueda del perfil legal de la empresa

1. En el Centro de partners, seleccione el icono **Configuración** y, a continuación, **Configuración de la cuenta**.
 
1. Seleccione **Perfil de la organización**. 

2. Revise los valores **Perfil legal de la empresa**, **Información de contacto principal** e **Información del programa**.

Si ha combinado otras compañías bajo la denominación legal de su empresa, también puede revisar su información. 

## <a name="update-your-legal-business-profile"></a>Actualización del perfil legal de la empresa 

Actualice la razón social y el domicilio social de su empresa en el Centro de partners.

>[!Important]
>- En el caso de las cuentas de Microsoft Partner Network (MPN), el administrador global y el de cuentas pueden actualizar la razón social de la empresa.
>- En el caso de las cuentas de revendedores indirectos de Proveedor de soluciones en la nube (CSP), solo el administrador global puede actualizar la razón social de la empresa. 
>- Los asociados de factura directa y los proveedores indirectos no pueden cambiar la razón social de la compañía si el estado de verificación de la cuenta es **Autorizado**. Si necesita cambiar el nombre, tendrá que [crear una incidencia de soporte técnico](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=eb74583c-61b3-2124-bffc-00920e0ae772).



1. En Centro de partners, seleccione **Configuración**, **Configuración de la cuenta** y, a continuación, **Perfil de la organización**.

2. Seleccione **Legal** y, a continuación, el perfil legal de la empresa (asociado o revendedor) que quiere actualizar.

1. Haga clic en **Actualizar** junto al nombre o la dirección de la compañía, y cambie los detalles.
 
1. Cuando seleccione **Enviar**, se reevaluará su identidad legal. Solo revaluamos lo que ha cambiado.

1. Si se produce un error en la comprobación, obtenga información acerca de cómo [corregir el problema](verification-responses.md).

>[!Important]
>Si es un asociado de CSP, no puede cambiar el país asociado a su domicilio social. El país del domicilio social está ligado a tu inquilino y a los servicios, así como a la moneda en la que realizas las transacciones. Para obtener información sobre las actualizaciones de país de MPN, lea  [actualizaciones del país de MPN](manage-locations.md#change-country-of-partner-global-account).


### <a name="who-can-update-legal-business-name-and-when"></a>Quién puede actualizar la razón social de la empresa y cuándo

|**Program**|**Quién puede actualizar el nombre de la empresa**|**Cuando se puede actualizar (estado)**|**Permitido**|
|---------------------|:-------------------------------|:------------|:-----------------|
MPN|Administrador global; administrador de la cuenta|Autorizado, pendiente, rechazado| Permitido|
|CSP: revendedor indirecto|Administrador global|Autorizado, pendiente, rechazado| Permitido|


## <a name="update-your-mpn-global-business-account"></a>Actualización de la cuenta empresarial global de MPN

Si durante la migración de Partner Membership Center al Centro de partners se identificó una cuenta empresarial equivocada como razón social de la empresa, puede cambiarla a la cuenta empresarial correcta.

Para realizar estas actualizaciones, debe ser un administrador global o de la cuenta. Aprenda a [administrar las cuentas de ubicación globales de MPN](manage-locations.md)


## <a name="update-your-mpn-id-associated-with-your-csp-account"></a>Actualización del id. de MPN asociado a la cuenta de CSP

Para actualizar el id. de MPN asociado a la cuenta de CSP:

1. Inicie sesión en el [panel](https://partner.microsoft.com/dashboard/home) del Centro de partners como administrador global con las credenciales de su cuenta de CSP y seleccione **Configuración**. (Las credenciales MPN y CSP pueden ser diferentes).
 
1. Seleccione **Identificadores** en **Configuración de cuenta**.

1. En la sección **CSP**, use el vínculo **Actualizar** para actualizar el identificador de MPN asociado a su cuenta de CSP. 


## <a name="update-your-csp-legal-billing-address"></a>Actualización de la dirección de facturación legal de CSP

Si es el administrador global, puede cambiar la dirección que aparece en la factura en **Payout and tax profile** (Perfil de pago y fiscal). Actualmente, no puede cambiar el nombre de la empresa en la factura debido a una limitación con el sistema de facturación.

:::image type="content" source="images/billing-profile.png" alt-text="Captura de pantalla del área donde se agrega la información de facturación.":::

|**Campo**  |**Descripción**|  
|---------------------|:------------------|
|Nombre de la compañía de facturación|Nombre de la compañía que aparece en la información de facturación de la factura de CSP.  Esta información no es editable en el Centro de partners.  Para actualizarla, debe crear una incidencia de soporte técnico.|
|Dirección de facturación|Dirección de facturación que se muestra en la factura de CSP. Se puede actualizar desde el [perfil de facturación](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial).|
|Contacto de facturación|Detalles del contacto de facturación (nombre, apellidos, número principal) de la cuenta de CSP.  Se puede actualizar desde el [perfil de facturación](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial).|
|Número de pedido de compra|Número de pedido de compra que se muestra en la factura del partner. Se puede actualizar desde el [perfil de facturación](https://partner.microsoft.com/dashboard/account/v3/accountsettings/billingprofile#commercial).|
|Id. fiscal de la compañía|Las empresas de algunos países pueden proporcionar su [número de IVA (valor añadido) o el equivalente local](./organization-tax-info.md). Para actualizar el CIF o IVA, debe ser un administrador global, un administrador de facturación o un agente de administración.|
|Divisa de facturación|La moneda de facturación de la cuenta de CSP viene determinada por el país legal de la cuenta de CSP.  Esta información no se puede cambiar una vez creada la cuenta de CSP.|

## <a name="next-steps"></a>Pasos siguientes

- [Comprobar el estado de la verificación](verification-responses.md)

- [Administrar ubicaciones de MPN](manage-locations.md)
