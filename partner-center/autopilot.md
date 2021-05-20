---
title: Personalización de la experiencia de configuración de un dispositivo
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Antes de entregar el nuevo dispositivo de un cliente, puede usar perfiles de Windows Autopilot para personalizar o configurar previamente la experiencia de configuración (OOBE) del dispositivo.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 5294495403be729adecb5a7814ade4f9d454a0f6
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149832"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Usar perfiles de Windows Autopilot en dispositivos nuevos para personalizar la experiencia rápida de un cliente

**Roles adecuados:** agente de administración | Administrador global | Agente de ventas | Administrador de administración de usuarios

Si administra dispositivos de cliente, es posible que tenga que personalizar la experiencia personalizada (OOBE) para los usuarios del cliente. Puede configurar previamente nuevos dispositivos con Windows Autopilot antes de entregar los dispositivos a los clientes y aplicar nuevos perfiles a los dispositivos que los clientes ya han adquirido. 

Tenga en cuenta que los OEM han empezado a incluir una etiqueta de envío en el exterior de la caja del dispositivo Autopilot que muestra el identificador de clave de producto **(PKID) del dispositivo.**  Este código de barras 1 dimensional y legible proporciona a los asociados de nivel inferior una manera de registrar dispositivos para Autopilot sin tener que desboxear los dispositivos y recolección del identificador de dispositivo por medios alternativos.

En este artículo se explica cómo crear y aplicar perfiles de Autopilot a dispositivos de Centro de partners.

Si aún no está familiarizado con Autopilot, revise la información de estos artículos:

- [Información general de Windows AutoPilot](/windows/deployment/windows-10-auto-pilot)
- [Guía de referencia de implementación de Autopilot](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Información general

Con la Windows Autopilot en Centro de partners, puede crear perfiles personalizados para aplicarlos a los dispositivos del cliente. La siguiente configuración de perfil estaba disponible en el momento en que se publicó este artículo:

- Omitir la configuración de privacidad. Esta configuración de perfil opcional de Autopilot permite a las organizaciones no preguntar sobre la configuración de privacidad durante el proceso de OOBE.

- Deshabilite la creación de cuentas de administrador local en el dispositivo. Las organizaciones pueden decidir si el usuario que configura el dispositivo debe tener acceso de administrador una vez completado el proceso.

- Configure automáticamente el dispositivo para el trabajo o la escuela. Todos los dispositivos registrados con Autopilot se considerarán automáticamente dispositivos de trabajo o educativos, por lo que esta pregunta no se hará durante el proceso de OOBE.

- Omita las páginas de configuración de registro de Cortana, OneDrive y OEM. Todos los dispositivos registrados con Autopilot omitirán automáticamente estas páginas durante el proceso de configuración automática (OOBE).

- Omitir el Contrato de licencia del usuario final (CLUF). A partir Windows 10 versión 1709, las organizaciones pueden decidir omitir la página del CLUF presentada durante el proceso de OOBE. Consulte [Windows Autopilot licencia del CLUF](#windows-autopilot-eula-dismissal) a continuación para obtener información importante a tener en cuenta sobre la omisión de la página clufór durante la instalación de Windows.

Se aplican las siguientes limitaciones y permisos de administración de perfiles y dispositivos:

- Los asociados de CSP pueden seguir administrando los perfiles de Autopilot para los clientes existentes con quienes tienen relaciones de revendedor, incluso si los clientes han quitado los privilegios de administración delegada del asociado.

- Puede administrar los dispositivos existentes para los clientes que ha agregado.

- No puede administrar los dispositivos que el cliente ha cargado en Microsoft Store para empresas o en el portal de Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Creación y administración de perfiles de Autopilot en Centro de partners

En Centro de partners, puede crear perfiles de Windows Autopilot y aplicarlos a los dispositivos.

>[!NOTE]
>Solo los agentes de administración pueden crear y aplicar perfiles.

### <a name="create-a-new-autopilot-profile"></a>Creación de un nuevo perfil de Autopilot

1. Seleccione **Clientes** en el Centro de partners y, a continuación, seleccione el cliente para el que va a crear el perfil de Autopilot.

2. En la página de detalles del cliente, seleccione **Dispositivos.**

3. En **Windows Autopilot perfiles,** seleccione **Agregar nuevo perfil.**

4. Escriba el nombre y la descripción del perfil y, a continuación, configure los valores de OOBE. Elija de entre las siguientes opciones:  

   - Omitir la configuración de privacidad en la configuración

   - Deshabilitación de la cuenta de administrador local en la instalación
  
   - Omitir páginas automáticamente en la configuración<br>
        (Incluye *Seleccionar automáticamente la configuración para el trabajo* o la escuela y omitir las páginas de configuración de registro de *Cortana, OneDrive y OEM)*
  
   - Omitir el contrato de licencia del usuario final (CLUF)<br> 
       >[!IMPORTANT] 
       >Consulte [Windows Autopilot licencia del CLUF](#windows-autopilot-eula-dismissal) a continuación para obtener información importante a tener en cuenta sobre la omisión de la página clufór durante la instalación de Windows.

5. Seleccione **Enviar** cuando haya terminado.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Aplicación de un perfil de Autopilot a dispositivos de cliente

>[!NOTE]
>En las instrucciones siguientes se supone que ya ha agregado los dispositivos del cliente a Centro de partners y que puede acceder a su lista de dispositivos. Si aún no ha agregado los dispositivos del cliente, siga las instrucciones de Adición de dispositivos a la cuenta de un cliente y, [a](#add-devices-to-a-customers-account) continuación, siga los pasos que se indican a continuación.

Después de crear un perfil de Autopilot para un cliente, puede aplicarlo a los dispositivos del cliente.

1. Seleccione **Clientes** en el menú Centro de partners y, a continuación, seleccione el cliente para el que creó el perfil de Autopilot.

2. En la página de detalles del cliente, seleccione **Dispositivos.**

3. En **Aplicar perfiles a dispositivos,** seleccione los dispositivos o grupos de dispositivos a los que desea agregar perfiles y, a continuación, **seleccione Aplicar perfil.** El perfil que acaba de aplicar aparece en la **columna** Perfil.

4. Siga estos pasos para comprobar que el perfil se aplicará correctamente al dispositivo.

    a.  Conecte un dispositivo a la red y encándalo.

    b.  Compruebe que aparecen las pantallas de OOBE adecuadas (si las hay).

    c.  Cuando se detenga el proceso de OOBE, restablezca el dispositivo a su configuración predeterminada de fábrica para prepararlo para un nuevo usuario.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Eliminación de un perfil de Autopilot del dispositivo de un cliente

1. Seleccione **Clientes** en el menú Centro de partners y, a continuación, seleccione el cliente para el que creó el perfil de Autopilot.

2. En la página de detalles del cliente, seleccione **Dispositivos.**

3. En **Aplicar perfiles a dispositivos,** seleccione los dispositivos de los que desea quitar el perfil y, a continuación, **seleccione Quitar perfil.**

   >[!NOTE]
   >La eliminación de un perfil de un dispositivo no elimina el perfil de la lista. Si desea eliminar un perfil, siga las instrucciones de [Actualización o eliminación de un perfil de Autopilot.](#update-or-delete-an-autopilot-profile)

### <a name="update-or-delete-an-autopilot-profile"></a>Actualización o eliminación de un perfil de Autopilot

Si un cliente desea cambiar la experiencia lista para usar después de haberle enviado los dispositivos, puede cambiar el perfil en Centro de partners.

Cuando el dispositivo del cliente se conecte a Internet, descargará la versión más reciente del perfil durante el proceso de OOBE. Además, cada vez que un cliente restaura un dispositivo a su configuración predeterminada de fábrica, el dispositivo descargará de nuevo la versión más reciente del perfil durante el proceso de OOBE.

1. Seleccione **Clientes** en el Centro de partners y, a continuación, seleccione el cliente que quiere que cambie un perfil de Autopilot.

2. En la página de detalles del cliente, seleccione **Dispositivos.**

3. En **Windows Autopilot perfiles,** seleccione el perfil que necesita actualizar. Realice los cambios necesarios y, a continuación, **seleccione Enviar**.

Para eliminar este perfil, seleccione **Eliminar perfil** en la esquina superior derecha de la página.

### <a name="add-devices-to-a-customers-account"></a>Agregar dispositivos a la cuenta de un cliente

>[!NOTE]
>Los agentes de ventas y los agentes de administración pueden agregar dispositivos a la cuenta de un cliente.

Para poder aplicar perfiles personalizados de Autopilot a los dispositivos del cliente, debe poder acceder a la lista de dispositivos del cliente.

Si tiene previsto usar el nombre de OEM, el número de serie y la combinación de modelos, tenga en cuenta estas limitaciones:

- Esta tupla solo funciona para dispositivos más recientes (hashes de 4k, por ejemplo) y no se admite para hashes 128b (RS2 y dispositivos anteriores).

- El registro de tupla distingue mayúsculas de minúsculas, por  lo que los datos del archivo deben coincidir exactamente con los nombres de modelo y fabricante proporcionados por el proveedor oem (proveedor de hardware).

Siga las instrucciones siguientes para agregar dispositivos a la cuenta de un cliente en Centro de partners.

1. Seleccione **Clientes** en el Centro de partners y, a continuación, seleccione el cliente cuyos dispositivos desea administrar.

2. En la página de detalles del cliente, seleccione **Dispositivos.**

3. En **Aplicar perfiles a dispositivos,** **seleccione Agregar dispositivos.**

4. Escriba un nombre para la  lista de dispositivos y, a continuación, seleccione Examinar para cargar la lista del cliente (en formato de archivo .csv) para Centro de partners.

    >[!NOTE]
    >Debería haber recibido este archivo .csv con la compra del dispositivo. Si no recibió un archivo .csv, puede crear uno usted mismo siguiendo los pasos descritos en Incorporación de dispositivos a [Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Cargue el archivo .csv y seleccione **Guardar.**

Si recibe un mensaje de error al intentar cargar el archivo .csv, compruebe el formato del archivo. Solo puede utilizar el hash de hardware, el nombre de OEM, el número de serie y el modelo (en ese orden de columna), o el identificador de producto de Windows. También puede usar el archivo .csv de ejemplo proporcionado en el vínculo junto a **Agregar dispositivos** para crear una lista de dispositivos.

El archivo .csv debe tener un aspecto parecido al siguiente:

> **Número de serie del dispositivo, id. de producto de Windows, hash de hardware, nombre del fabricante, modelo de dispositivo**

> **{serialNumber},,,Microsoft Corporation,Surface Laptop**

>[!NOTE]
> "Nombre de fabricante" y "Modelo de dispositivo" distinguen mayúsculas de minúsculas.

Si no sabe qué valor se debe colocar para el nombre del fabricante y el modelo de dispositivo, puede ejecutarlo en el dispositivo para recopilar los valores correctos:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot del CLUF

### <a name="important-information"></a>INFORMACIÓN IMPORTANTE

Windows Autopilot permite configurar instalaciones personalizadas de Windows en dispositivos que administra para los clientes. Si el cliente lo autoriza, puede suprimir u ocultar determinadas pantallas de configuración que normalmente se presentan a los usuarios al configurar Windows, incluida la pantalla de aceptación del CLUF (Contrato de licencia del usuario final).

Al usar esta función, acepta que suprimir u ocultar las pantallas diseñadas para proporcionar a los usuarios el aviso o la aceptación de los términos significa que ha obtenido el consentimiento y la autorización suficientes del cliente para ocultar los términos, y que usted, en nombre del cliente (ya sea una organización o un usuario individual según sea el caso), da su consentimiento a los avisos y acepta los términos aplicables a su cliente. Esto incluye el acuerdo con los términos y condiciones de la licencia o el aviso que se presentaría al usuario si no lo suprimió u ocultó mediante esta herramienta. El cliente no puede usar el software de Windows en esos dispositivos si el cliente no ha adquirido válidamente una licencia para el software de Microsoft o sus distribuidores con licencia.