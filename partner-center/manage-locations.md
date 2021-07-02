---
title: Administración de las ubicaciones en tu cuenta de partner
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Aprenda a agregar una nueva ubicación y cómo se usa el identificador de MPN de ubicación en programas de incentivos, empresas de CSP, suscripciones y otras transacciones.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d30f250d6635758f3bef8e06c6f57ba0a0be744
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276831"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Administración de las ubicaciones de la cuenta de MPN y adición (eliminación) de una ubicación


**Roles adecuados**: Administrador global | Administrador de cuentas

Los identificadores de MPN de ubicación identifican cada ubicación específica de la empresa. Use el identificador de MPN de ubicación para inscribirse en programas de incentivos, para realizar transacciones de empresas del programa Proveedor de soluciones en la nube (CSP) y para otras transacciones comerciales. El identificador de MPN global se usa para actividades no transaccionales, como las solicitudes de soporte técnico.

## <a name="the-following-scenario-is-typical"></a>El escenario siguiente es típico:

Contoso tiene su cuenta global de partner (PGA) en el Reino Unido. La PGA indica la empresa legal registrada, cuyo identificador de MPN global se usa para administrar todos los negocios no transaccionales. Contoso también tiene cuentas de ubicación de partner (PLA) equivalentes a subsidiarias o divisiones en otras ubicaciones del Reino Unido, Francia y EE. UU. En la estructura de cuentas de MPN, estas PLA se representan como identificadores de MPN de ubicación únicos. Las PLA se usan para negocios transaccionales, como los programas de CSP o de incentivos. Los pagos están vinculados a ubicaciones específicas. 

>[!NOTE]
>Hay una relación 1-1 entre un inquilino de CSP y un identificador de ubicación de MPN.

:::image type="content" source="images/locations/locations1.png" alt-text="Estructura de ubicaciones de MPN.":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Requisitos previos para agregar una nueva cuenta para una empresa de CSP

Para agregar una nueva cuenta de empresa de CSP, empiece por asegurarse de cumplir los requisitos previos.

1. Debe tener un identificador de MPN de ubicación en el país en el que quiere hacer negocios de CSP. Para crear una nueva ubicación de MPN, lea "Agregar una ubicación de MPN" a continuación.
  
1. Para crear una nueva inscripción de CSP Indirect Reseller, lea [Trabajar con proveedores indirectos](indirect-reseller-tasks-in-partner-center.md#get-started). 

>[!NOTE] 
 >Recuerde iniciar sesión con las **nuevas** credenciales de la cuenta de CSP **nueva**. No use las credenciales existentes, ya que el Centro de partners reconocerá que ya tiene una cuenta.

2. Acepte el contrato Microsoft Partner Agreement y active la cuenta.

1. Si desea inscribirse como partner de facturación directa, consulte [Requisitos para partners de facturación directa](direct-partner-new-requirements.md).

## <a name="view-and-update-your-mpn-locations"></a>Visualización y actualización de las ubicaciones de MPN

1. Inicie sesión en el [panel](https://partner.microsoft.com/dashboard/home) del Centro de partners con las credenciales de la cuenta de MPN. (Las credenciales de MPN pueden ser diferentes de las credenciales del programa CSP). 
 
1. Desde el icono de **Configuración**, seleccione **Configuración de la cuenta**, **Perfil de la organización** y **Legal**. 

1. En la pestaña **Asociado**, compruebe que no hay ningún mensaje de error de banner que le pida que corrija las ubicaciones migradas desde PMC.  Si las ubicaciones no se configuraron correctamente en PMC y todavía no se han pasado al equipo, debe actualizarlas.

:::image type="content" source="images/locations/location-two.png" alt-text="Captura de pantalla que muestra cómo actualizar la ubicación.":::
 
4.  En la pantalla **Revisar ubicaciones de PMC**, seleccione **Actualizar**.
Actualice los campos siguientes:

- **Campo de nombre**: asegúrese de que el nombre de la ubicación de la compañía sea correcto. Si se muestra un error duplicado, intente cambiar de Contoso a Contoso, Inc., por ejemplo.

- **Campo de entidad jurídica**: asegúrese de que ha elegido la entidad jurídica a la que está asociada la ubicación.

- **Campos de línea de dirección 1 y 2**: asegúrese de que la dirección es correcta.

- **Campos de ciudad y estado o provincia**: asegúrese de que la combinación entre la ciudad y el estado o provincia sea correcta. Hay países en los que se aplicará el menú desplegable para elegir el estado o provincia y, en otros, el campo tendrá que insertarse manualmente.

- **Campo de código postal**: asegúrese de que el campo Código postal coincida con el país, la región, la ciudad o la dirección indicados.

- **Campos de información de contacto principal**: asegúrese de que se rellenan los campos de nombre y apellidos y que la dirección de correo electrónico indicada es un correo electrónico del trabajo y no uno personal (por ejemplo, @outlook.com, @live.com, etc.).

- **Campo de número de teléfono**: asegúrese de que el número de teléfono no incluya caracteres especiales, espacios ni código de país. El valor especificado en el campo de número de teléfono siempre contendrá un máximo de 10 caracteres.

5. Si no hay ningún mensaje de error, desde **Configuración**, seleccione **Configuración de la cuenta**, **Perfil de la organización** e **Identificadores**.

6. Busque el id. de MPN con el tipo "Ubicación" que coincida con el país de esta cuenta de CSP y úselo para completar la asociación.

7. Si no encuentra el id. de MPN de la ubicación que coincide con la cuenta de CSP que quiere usar, puede agregar una nueva ubicación que creará un nuevo id. de MPN. Consulte **Agregar una ubicación de MPN** a continuación.

## <a name="add-an-mpn-location"></a>Agregar una ubicación de MPN

1. Iniciar sesión con la cuenta de MPN en el Centro de partners. (Las credenciales de MPN pueden ser diferentes de las credenciales de CSP). La cuenta de MPN debe tener privilegios de Administrador global o de Administrador de cuentas. 

1. Desde el **icono de Configuración**, seleccione **Configuración de la cuenta** y, a continuación, elija **Perfil de la organización**.

2. Seleccione **Legal** y, a continuación, en la pestaña **Partner**, seleccione **Ubicaciones de la empresa** y haga clic en **Agregar una ubicación**.

3. Proporcione los detalles necesarios, como el nombre, la dirección y el contacto de la empresa correspondientes a la ubicación que desea agregar a la empresa.
 
1. Selecciona **Agregar ubicación**. Se creará un nuevo id. de MPN para la nueva ubicación, que puede usar para las transacciones y los incentivos del programa CSP.

:::image type="content" source="images/legal-biz.png" alt-text="Agregue una nueva razón social de la empresa.":::

> [!NOTE]
> Una vez agregada una ubicación en el Centro de partners, no se puede quitar. Verá **MPN** en el menú izquierdo del Centro de partners si ha usado el identificador de MPN correcto para iniciar sesión.

## <a name="add-the-registration-number-id"></a>Adición del identificador numérico de registro

Si es proveedor indirecto, partner de facturación directa o revendedor indirecto y hace negocios con clientes nuevos o existentes en los siguientes países, tiene que proporcionar los números de identificación del registro para su empresa. Si el país en el que hace negocios no aparece a continuación, la identificación del registro es opcional.

- Armenia 
- Azerbaiyán 
- Belarús 
- Brasil 
- Hungría 
- India 
- Iraq 
- Kazajistán 
- Kirguistán 
- Moldova 
- Myanmar 
- Polonia 
- Rusia 
- Arabia Saudí 
- Sudáfrica 
- Sudán del Sur  
- Tayikistán 
- Tailandia
- Turquía 
- Ucrania 
- Emiratos Árabes Unidos 
- Uzbekistán 
- Venezuela
- Vietnam 


Para obtener más información, lea [Información del id. de registro.](reg-number-id.md)

## <a name="delete-a-location"></a>Eliminación de una ubicación

Para eliminar una ubicación de la cuenta, deberá ponerse en contacto con el [servicio de soporte técnico para asociados](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b). Asegúrese de que comprende el impacto que tiene esta acción. Las ubicaciones eliminadas no se pueden recuperar y todo lo relacionado con ese id. de MPN específico ya no se reconocerá ni estará activo para la empresa.

## <a name="change-country-of-partner-global-account"></a>Cambiar el país de la cuenta global del asociado 

1. Iniciar sesión con la cuenta de MPN en el Centro de partners. (Las credenciales de MPN pueden ser diferentes de las credenciales de CSP). La cuenta de MPN debe tener privilegios de Administrador global o de Administrador de cuentas. 

2. En la pestaña **Partner**, diríjase a **Ubicaciones de la empresa** y compruebe la lista de ubicaciones para asegurarse de que se muestra la ubicación que quiere como entidad jurídica. 
 
1. Para agregar una ubicación, haga clic en **Agregar una ubicación** y, en el control flotante, proporcione los detalles necesarios, como el nombre, la dirección y el contacto principal de la empresa correspondientes a la ubicación que desea agregar a la empresa. 
 
1. Seleccione **Cambiar el país** junto a la lista desplegable **País o región** y siga los pasos que se indican. 

:::image type="content" source="images/lbp.png" alt-text="Control flotante de datos del perfil legal de la empresa.":::

5. Seleccione **Guardar**.

6. El país de la cuenta global de MPN se cambiará por el país del nuevo perfil legal.
  
## <a name="next-steps"></a>Pasos siguientes

- Obtenga más información acerca del [proceso de verificación](verification-responses.md).
