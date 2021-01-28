---
title: Administración de las ubicaciones en tu cuenta de partner
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Aprenda a agregar una nueva ubicación y cómo se usa el identificador de MPN de ubicación en programas de incentivos, empresas de CSP, suscripciones y otras transacciones.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e39f264485e71c5a96916c224c0ea1a85c17a55b
ms.sourcegitcommit: fc1f9cb5a542bdc92d62d2a7e1ab2f4e69903e49
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 01/28/2021
ms.locfileid: "98925018"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Administración de las ubicaciones de la cuenta de MPN y adición de una nueva ubicación


**Roles adecuados**

- Administrador global
- Administrador de cuentas

Los identificadores de MPN de ubicación identifican cada ubicación específica de la empresa. Use el identificador de MPN de ubicación para inscribirse en programas de incentivos, para realizar transacciones de empresas del programa Proveedor de soluciones en la nube (CSP) y para otras transacciones comerciales. El identificador de MPN global se usa para actividades no transaccionales, como las solicitudes de soporte técnico.

## <a name="the-following-is-a-typical-scenario"></a>El siguiente ejemplo es un escenario típico:

Contoso tiene su cuenta global de partner (PGA) en el Reino Unido. Se trata de su empresa legal registrada, cuyo identificador de MPN global se usa para administrar todos los negocios no transaccionales. Contoso también tiene cuentas de ubicación de partner (PLA) equivalentes a subsidiarias o divisiones en otras ubicaciones del Reino Unido, Francia y EE. UU. En la estructura de cuentas de MPN, estas PLA se representan como identificadores de MPN de ubicación únicos. Las PLA se usan para negocios transaccionales, como los programas de CSP o de incentivos. Los pagos están vinculados a ubicaciones específicas. 

>[!NOTE]
>Hay una relación 1-1 entre un inquilino de CSP y un identificador de ubicación de MPN.

:::image type="content" source="images/locations/locations1.png" alt-text="Estructura de ubicaciones de MPN":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Requisitos previos para agregar una nueva cuenta para una empresa de CSP

Para agregar una nueva cuenta de empresa de CSP, empiece por asegurarse de cumplir los requisitos previos.

1. Debe tener un identificador de MPN de ubicación en el país en el que quiere hacer negocios de CSP. Para crear una nueva ubicación de MPN, lea "Agregar una ubicación de MPN" a continuación.
  
1. Para crear una nueva inscripción de CSP Indirect Reseller, lea [Trabajar con proveedores indirectos](indirect-reseller-tasks-in-partner-center.md#get-started). 

>[!NOTE] 
 >Recuerde iniciar sesión con las **nuevas** credenciales de la cuenta de CSP **nueva**. No use las credenciales existentes, ya que el Centro de partners reconocerá que ya tiene una cuenta.

2. Acepte el contrato Microsoft Partner Agreement y active la cuenta.

## <a name="add-an-mpn-location"></a>Agregar una ubicación de MPN

1. Iniciar sesión con la cuenta de MPN en el Centro de partners. (Las credenciales de MPN pueden ser diferentes de las credenciales del programa CSP). La cuenta de MPN debe tener privilegios de administrador global o de cuenta. 

1. Desde el **icono de Configuración**, seleccione **Configuración de la cuenta** y, a continuación, elija **Perfil de la organización**.

2. Seleccione **Legal** y, a continuación, en la pestaña **Partner**, seleccione **Ubicaciones de la empresa** y haga clic en **Agregar una ubicación**.

3. Proporcione los detalles necesarios, como el nombre, la dirección y el contacto de la empresa correspondientes a la ubicación que desea agregar a la empresa.
 
1. Haga clic en **Agregar ubicación**. Se creará un nuevo ID de MPN para la nueva ubicación, que puede utilizar para las transacciones y los incentivos del programa CSP.

:::image type="content" source="images/legal-biz.png" alt-text="Agregar un nuevo perfil legal de la empresa":::

> [!NOTE]
> Una vez agregada una ubicación en el Centro de partners, no se puede quitar. Verá **MPN** en el menú izquierdo del Centro de partners si ha usado el identificador de MPN correcto para iniciar sesión.

## <a name="change-country-of-partner-global-account"></a>Cambiar el país de la cuenta global del asociado 

1. Iniciar sesión con la cuenta de MPN en el Centro de partners. (Las credenciales de MPN pueden ser diferentes de las credenciales del programa CSP). La cuenta de MPN debe tener privilegios de administrador global o de cuenta. 

2. En la pestaña **Partner**, diríjase a **Ubicaciones de la empresa** y compruebe la lista de ubicaciones para asegurarse de que se muestra la ubicación que quiere como entidad jurídica. 
 
1. Para agregar una ubicación, haga clic en **Agregar una ubicación** y, en el control flotante, proporcione los detalles necesarios, como el nombre, la dirección y el contacto principal de la empresa correspondientes a la ubicación que desea agregar a la empresa. 
 
1. Seleccione **Cambiar el país** junto al menú desplegable **País o región** y siga los pasos que se indican. 

:::image type="content" source="images/lbp.png" alt-text="Control flotante de datos del perfil legal de la empresa":::

5. Haga clic en **Guardar**.

6. El país de la cuenta global de MPN se cambiará por el país del nuevo perfil legal.
  
## <a name="next-steps"></a>Pasos siguientes

- Obtenga más información acerca del [proceso de verificación](verification-responses.md).
