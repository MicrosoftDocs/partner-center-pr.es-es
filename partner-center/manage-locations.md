---
title: Administración de las ubicaciones en tu cuenta de partner
ms.topic: article
ms.date: 10/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Aprenda a agregar una nueva ubicación y cómo se usa el identificador de MPN de ubicación en programas de incentivos, empresas de CSP, suscripciones y otras transacciones.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c4435227cdd5d777d11c79bf4adc63471ad925e9
ms.sourcegitcommit: 940dad4527f51781f6f966e196b3aa08389613a2
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 10/13/2020
ms.locfileid: "92006843"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Administración de las ubicaciones de la cuenta de MPN y adición de una nueva ubicación

**Se aplica a**

- Centro de partners

**Roles adecuados**

- Administrador global
- Administrador de cuentas

Los identificadores de MPN de ubicación identifican cada ubicación específica de la empresa. Use el identificador de MPN de ubicación para inscribirse en programas de incentivos, para realizar transacciones de empresas del programa Proveedor de soluciones en la nube (CSP) y para otras transacciones comerciales. El identificador de MPN global se usa para actividades no transaccionales, como las solicitudes de soporte técnico.

## <a name="the-following-is-a-typical-scenario"></a>El siguiente ejemplo es un escenario típico:

Contoso tiene su cuenta global de partner (PGA) en el Reino Unido. Se trata de su empresa legal registrada, cuyo identificador de MPN global se usa para administrar todos los negocios no transaccionales. Contoso también tiene cuentas de ubicación de partner (PLA) equivalentes a subsidiarias o divisiones en otras ubicaciones del Reino Unido, Francia y EE. UU. En la estructura de cuentas de MPN, estas PLA se representan como identificadores de MPN de ubicación únicos. Las PLA se usan para negocios transaccionales, como los programas de CSP o de incentivos. Los pagos están vinculados a ubicaciones específicas. 

>[!NOTE]
>Hay una relación 1-1 entre un inquilino de CSP y un identificador de ubicación de MPN.

:::image type="content" source="images/locations/locations1.png" alt-text="Estructura de ubicaciones de MPN":::

## <a name="prerequisites-in-order-to-add-a-new-location-for-a-csp-business"></a>Requisitos previos para agregar una nueva ubicación para una empresa de CSP

Para agregar una nueva ubicación de empresa de CSP, hay varios requisitos previos:

1. Debe tener un identificador de MPN de ubicación en el país en el que quiere hacer negocios.

1. Necesita un nuevo inquilino de Azure AD en la [región de la empresa](regional-authorization-overview.md) que aún no está inscrito en CSP. Créelo al inscribirse en CSP.
 
3. Use el nuevo inquilino de AAD para inscribirse en el programa CSP en la región.
Proporcione los detalles de la empresa legal, incluidos el nombre legal de la empresa, su dirección y los detalles del contacto principal. Esta cuenta se someterá a una verificación: asegúrese de agregar información válida.

>[!NOTE] 
 >Recuerde iniciar sesión con las **nuevas** credenciales para el **nuevo** inquilino de Azure AD. No use las credenciales existentes, ya que el Centro de partners reconocerá que ya tiene una cuenta.

4. Acepte el contrato Microsoft Partner Agreement y active la cuenta.

## <a name="add-a-location"></a>Agregar una ubicación

1. Inicie sesión con la cuenta de MPN en el Centro de partners. La cuenta de MPN debe tener privilegios de administrador global o de cuenta. 

1. En el **icono Configuración**, selecciona **Configuración de partners**.

2. Selecciona **Ubicaciones.**

3. Seleccione **Agregar una ubicación** e inserte los detalles de la dirección de la ubicación que quiera agregar a la empresa, así como un contacto principal para la ubicación.

> [!NOTE]
> Una vez agregada una ubicación en el Centro de partners, no se puede quitar. Verá **MPN** en el menú izquierdo del Centro de partners si ha usado el identificador de MPN correcto para iniciar sesión.

## <a name="change-global-partner-account-location"></a>Cambio de la ubicación de la cuenta de partner global

1. En la página **[Ubicaciones](https://partner.microsoft.com/pcv/accountsettings/locationsprofile)** , compruebe la lista de ubicaciones para asegurarse de que se muestra la ubicación que quiere como entidad jurídica. Si no es así, agrégala.

   :::image type="content" source="images/updatepartnerprofile2.png" alt-text="Estructura de ubicaciones de MPN":::

2. Selecciona **Perfil del partner** y luego **Update legal business profile** (Actualizar perfil de denominación legal de la empresa).

   :::image type="content" source="images/updatepartnerprofile1.png" alt-text="Estructura de ubicaciones de MPN":::

3. Selecciona la región, la entidad jurídica y **Enviar**.

   :::image type="content" source="images/updatepartnerprofile3.png" alt-text="Estructura de ubicaciones de MPN":::

## <a name="next-steps"></a>Pasos siguientes

- Obtenga más información acerca del [proceso de verificación](verification-responses.md).
