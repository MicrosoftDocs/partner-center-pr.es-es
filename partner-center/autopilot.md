---
title: Personalización de la experiencia rápida de un dispositivo con perfiles de Windows AutoPilot | Centro de Partners
description: Preconfigurar la configuración rápida de un dispositivo con perfiles de AutoPilot.
ms.topic: article
ms.date: 03/18/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: maggiepuccievans
ms.author: evansma
keywords: AutoPilot, Windows AutoPilot, Microsoft AutoPilot, implementación sin interacción rápida, Oobe, pantallas de inicio de sesión, no actualizadas
ms.localizationpriority: medium
ms.openlocfilehash: 6ad6482c68da6c964414be3b7f036835934f049e
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653911"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Personalización de la experiencia rápida de un dispositivo con perfiles de Windows AutoPilot

**Se aplica a**

- CSP directo: factura, proveedores indirectos y distribuidores indirectos

Si administra los dispositivos del cliente, es posible que tenga que personalizar la experiencia rápida (OOBE) para los usuarios del cliente. Puede preconfigurar nuevos dispositivos con perfiles de Windows AutoPilot antes de entregar los dispositivos a los clientes y aplicar nuevos perfiles a los dispositivos que los clientes ya han comprado. 

Tenga en cuenta que los OEM han empezado a incluir una etiqueta de envío en el exterior del cuadro dispositivo AutoPilot que muestra el identificador de la clave de producto del dispositivo **(pkid)** .  Este código de barras bidimensional y legible proporciona a los asociados de nivel inferior una manera de registrar dispositivos para el piloto automático sin tener que volver a realizar la conversión unboxing de los dispositivos y cosechar el ID. de dispositivo mediante medios alternativos.

En este artículo se explica cómo crear y aplicar perfiles de AutoPilot a dispositivos del centro de Partners.

Si no está familiarizado con AutoPilot, revise la información de estos artículos:

- [Información general de Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Guía de referencia de implementación de AutoPilot](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Introducción

Con la característica de Windows AutoPilot del centro de Partners, puede crear perfiles personalizados para aplicarlos a los dispositivos del cliente. La siguiente configuración de perfil estaba disponible en el momento en que se publicó este artículo:

- Omitir la configuración de privacidad. Esta configuración de Perfil de AutoPilot opcional permite a las organizaciones no preguntar sobre la configuración de privacidad durante el proceso de OOBE.

- Deshabilite la creación de cuentas de administrador local en el dispositivo. Las organizaciones pueden decidir si el usuario que configura el dispositivo debe tener acceso de administrador una vez completado el proceso.

- Configure automáticamente el dispositivo para el trabajo o la escuela. Todos los dispositivos registrados con AutoPilot se considerarán automáticamente dispositivos de trabajo o escuela, por lo que no se le pedirá esta pregunta durante el proceso de OOBE.

- Omitir las páginas de configuración de registro de Cortana, OneDrive y OEM. Todos los dispositivos registrados con AutoPilot omitirán automáticamente estas páginas durante el proceso de la experiencia rápida (OOBE).

- Omitir contrato de licencia para el usuario final (CLUF). A partir de la versión 1709 de Windows 10, las organizaciones pueden decidir omitir la página del CLUF presentada durante el proceso de OOBE. Consulte [descartado de CLUF de Windows AutoPilot](#windows-autopilot-eula-dismissal) para obtener información importante que se debe tener en cuenta al omitir la página del CLUF durante la instalación de Windows.

Se aplican las siguientes limitaciones y permisos de administración de perfiles y dispositivos:

- Los asociados de CSP pueden seguir administrando los perfiles de AutoPilot para los clientes existentes con quienes tienen relaciones de reseller, incluso si los clientes han quitado los privilegios de administración delegada del socio.

- Puede administrar los dispositivos existentes para los clientes que ha agregado.

- No puede administrar los dispositivos que el cliente ha cargado en Microsoft Store para empresas o en el portal de Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Crear y administrar perfiles de AutoPilot en el centro de Partners

En el centro de Partners, puede crear perfiles de implementación de Windows AutoPilot y aplicarlos a los dispositivos.

>[!NOTE]
>Solo los agentes de administración pueden crear y aplicar perfiles.

### <a name="create-a-new-autopilot-profile"></a>Crear un nuevo perfil AutoPilot

1. Seleccione **clientes** en el menú del centro de Partners y, a continuación, seleccione el cliente para el que va a crear el perfil de AutoPilot.

2. En la página de detalles del cliente, seleccione **dispositivos**.

3. En **perfiles de Windows AutoPilot** , seleccione **Agregar nuevo perfil**.

4. Escriba el nombre y la descripción del perfil y, a continuación, establezca la configuración de OOBE. Elija entre:  

   - Omitir la configuración de privacidad en el programa de instalación

   - Deshabilitar la cuenta de administrador local en el programa de instalación
  
   - Omitir automáticamente las páginas durante la instalación<br>
        (Incluye *la configuración seleccionada automáticamente para el trabajo o la escuela* y *omitir las páginas de configuración de registro de Cortana, OneDrive y OEM*)
  
   - Omitir contrato de licencia para el usuario final (CLUF)<br> 
       >[!IMPORTANT] 
       >Consulte [descartado de CLUF de Windows AutoPilot](#windows-autopilot-eula-dismissal) para obtener información importante que se debe tener en cuenta al omitir la página del CLUF durante la instalación de Windows.

5. Selecciona **Enviar** cuando hayas acabado.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Aplicar un perfil de AutoPilot a los dispositivos del cliente

>[!NOTE]
>En las instrucciones siguientes se supone que ya ha agregado los dispositivos del cliente al centro de Partners y que puede acceder a su lista de dispositivos. Si aún no ha agregado los dispositivos del cliente, siga las instrucciones de [Agregar dispositivos a la cuenta de un cliente](#add-devices-to-a-customers-account) y, a continuación, siga los pasos que se indican a continuación.

Después de crear un perfil de AutoPilot para un cliente, puede aplicarlo a los dispositivos del cliente.

1. Seleccione **clientes** en el menú del centro de Partners y, a continuación, seleccione el cliente para el que ha creado el perfil AutoPilot.

2. En la página de detalles del cliente, seleccione **dispositivos**.

3. En **aplicar perfiles a dispositivos** , seleccione los dispositivos o grupos de dispositivos a los que quiere agregar perfiles y, a continuación, seleccione **aplicar perfil**. El perfil que acaba de aplicar aparece en la columna **perfil** .

4. Siga los pasos que se indican a continuación para comprobar que el perfil se aplicará correctamente al dispositivo.

    a.  Conectar un dispositivo a la red y activarlo.

    b.  Comprueba que aparezcan las pantallas OOBE apropiadas (si es el caso).

    c.  Cuando se detenga el proceso de OOBE, restablezca el dispositivo a su configuración predeterminada de fábrica para prepararlo para un nuevo usuario.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Quitar un perfil de AutoPilot del dispositivo de un cliente

1. Seleccione **clientes** en el menú del centro de Partners y, a continuación, seleccione el cliente para el que ha creado el perfil AutoPilot.

2. En la página de detalles del cliente, seleccione **dispositivos**.

3. En **aplicar perfiles a dispositivos** , seleccione los dispositivos de los que desea quitar el perfil y, a continuación, seleccione **quitar perfil**.

   >[!NOTE]
   >La eliminación de un perfil de un dispositivo no elimina el perfil de la lista. Si desea eliminar un perfil, siga las instrucciones de [actualización o eliminación de un perfil de AutoPilot](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Actualización o eliminación de un perfil de AutoPilot

Si un cliente desea cambiar la experiencia rápida después de haber enviado los dispositivos a ellos, puede cambiar el perfil en el centro de Partners.

Cuando el dispositivo del cliente se conecta a Internet, se descargará la versión más reciente del perfil durante el proceso de OOBE. Además, cada vez que un cliente restaura un dispositivo a su configuración predeterminada de fábrica, el dispositivo descargará la versión más reciente del perfil durante el proceso de OOBE.

1. Seleccione **clientes** en el menú del centro de Partners y, a continuación, seleccione el cliente que desea cambiar un perfil de AutoPilot.

2. En la página de detalles del cliente, seleccione **dispositivos**.

3. En **perfiles de Windows AutoPilot** , seleccione el perfil que necesita actualizar. Realice los cambios necesarios y, a continuación, seleccione **submit (enviar**).

Para eliminar este perfil, seleccione **eliminar perfil** en la esquina superior derecha de la página.

### <a name="add-devices-to-a-customers-account"></a>Agregar dispositivos a la cuenta de un cliente

>[!NOTE]
>Los agentes de ventas y los agentes de administración pueden agregar dispositivos a la cuenta de un cliente.

Para poder aplicar perfiles de AutoPilot personalizados a los dispositivos del cliente, debe tener acceso a la lista de dispositivos del cliente.

Si tiene previsto usar el nombre del OEM, el número de serie y la combinación de modelos, tenga en cuenta estas limitaciones:

- Esta tupla solo funciona para dispositivos más recientes (por ejemplo, hash 4k) y no se admite para los hashes 128B (RS2 y dispositivos anteriores).

- El registro de la tupla distingue entre mayúsculas y minúsculas, por lo que los datos del archivo deben coincidir ***exactamente*** con los nombres del modelo y del fabricante, tal como lo proporciona el proveedor de OEM (proveedor de hardware).

Siga las instrucciones que se indican a continuación para agregar dispositivos a la cuenta de un cliente en el centro de Partners.

1. Seleccione **customers (clientes** ) en el menú del centro de Partners y seleccione el cliente cuyos dispositivos desea administrar.

2. En la página de detalles del cliente, seleccione **dispositivos**.

3. En **aplicar perfiles a dispositivos** , seleccione **Agregar dispositivos**.

4. Escriba un nombre para la lista de dispositivos y, a continuación, seleccione **examinar** para cargar la lista de clientes (en formato de archivo. csv) en el centro de Partners.

    >[!NOTE]
    >Debe haber recibido este archivo. csv con la compra del dispositivo. Si no recibió un archivo. csv, puede crear uno usted mismo siguiendo los pasos descritos en [Agregar dispositivos a Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Cargue el archivo. csv y, a continuación, seleccione **Guardar**.

Si recibe un mensaje de error al intentar cargar el archivo. csv, compruebe el formato del archivo. Solo puede utilizar el hash de hardware, el nombre de OEM, el número de serie y el modelo (en ese orden de columna), o el identificador de producto de Windows. También puede usar el archivo. csv de ejemplo que se proporciona en el vínculo junto a **Agregar dispositivos** para crear una lista de dispositivos.

El archivo. csv debería tener un aspecto similar al siguiente:

> **Número de serie del dispositivo, ID. de producto de Windows, hash de hardware, nombre de fabricante, modelo de dispositivo**

> **{serialNumber},,, Microsoft Corporation, Surface Laptop**

Tenga en cuenta que "nombre del fabricante" y "modelo de dispositivo" distinguen mayúsculas de minúsculas.

Si no sabe qué valor poner para el modelo de nombre de fabricante y dispositivo, puede ejecutarlo en el dispositivo para recopilar los valores correctos:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Descartado de CLUF de Windows AutoPilot

### <a name="important-information"></a>INFORMACIÓN IMPORTANTE

Windows AutoPilot le permite configurar instalaciones personalizadas de Windows en los dispositivos que administra para sus clientes. Si el cliente tiene autorización para hacerlo, puede suprimir u ocultar determinadas pantallas de configuración que se suelen presentar a los usuarios al configurar Windows, incluida la pantalla de aceptación del CLUF (contrato de licencia para el usuario final).

Al usar esta función, acepta que la supresión y ocultación de las pantallas que están diseñadas para proporcionar a los usuarios aviso o aceptación de términos significa que ha obtenido el consentimiento y la autorización suficientes del cliente para ocultar términos y que usted, en nombre de su cliente (ya sea una organización o un usuario individual como caso), dar su consentimiento a cualquier aviso y aceptar los términos aplicables a su cliente. Esto incluye que estás de acuerdo con los términos y condiciones de la licencia o el anuncio que se presenta al usuario si no la suprimiste u ocultaste con esta herramienta. Tu cliente no puede usar el software de Windows en esos dispositivos si ha adquirido de manera válida una licencia para el software desde Microsoft o sus distribuidores con licencia.
