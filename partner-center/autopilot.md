---
title: Personalizar la experiencia out-of-box de un dispositivo con los perfiles de Windows Autopilot | El centro de partners
description: Preconfigurar experiencia out-of-box de un dispositivo con perfiles Autopilot.
ms.topic: article
ms.date: 02/06/19
author: maggiepuccievans
ms.author: evansma
keywords: AutoPilot, autopilot de windows, autopilot de microsoft, implementación sin interacción, oobe, pantallas de inicio de sesión, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 46b8a74383585c630864079efa42b6e34412b91e
ms.sourcegitcommit: 80f3eb81f2e7605e77d19856827472f7830db419
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 02/22/2019
ms.locfileid: "9098832"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Personalizar la experiencia out-of-box de un dispositivo con los perfiles de Windows Autopilot

**Se aplica a:**

- Los partners de CSP directo factura, los proveedores indirectos y distribuidores indirectos

Si puedes administrar dispositivos de los clientes, puede que tengas personalizar la experiencia out-of-box (OOBE) para los usuarios del cliente. Puedes configurar previamente nuevos dispositivos con perfiles Autopilot de Windows antes de entregar los dispositivos a los clientes y aplicar los perfiles de nuevos a dispositivos de los clientes ya hayan comprado. En este artículo se explica cómo crear y aplicar los perfiles Autopilot a los dispositivos en el centro de partners.

Si no ya estás familiarizado con Autopilot, revisa la información de estos artículos:

- [Introducción a WindowsAutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Guía de referencia de implementación de AutoPilot](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Introducción

Con la característica Windows Autopilot en el centro de partners, puedes crear perfiles personalizados para aplicar a dispositivos de los clientes. La siguiente configuración de perfil estaba disponible en el momento en que se publicó este artículo:

- Omitir configuración de privacidad. Esta opción de configuración opcional del perfil de Autopilot permite a las organizaciones preguntar sobre la configuración de privacidad durante el proceso OOBE.

- Deshabilitar la creación de cuentas de administrador local en el dispositivo. Las organizaciones pueden decidir si el usuario configura el dispositivo debe tener acceso de administrador, una vez completado el proceso.

- Configurar automáticamente el dispositivo para el trabajo o escuela. Todos los dispositivos registrados con Autopilot automáticamente se considerarán trabajo o escuela dispositivos, por lo que esta pregunta no se le pida durante el proceso OOBE.

- Omitir páginas de configuración de registro de OEM, OneDrive y Cortana. Todos los dispositivos registrados con Autopilot omitirán automáticamente estas páginas durante el proceso de out-of-box rápida (OOBE).

- Omitir contrato de licencia de usuario final (CLUF). A partir de Windows 10, versión 1709, las organizaciones pueden decidir omitir la página del CLUF presentada durante el proceso de configuración rápida. Consulta [desestimación del CLUF de Windows Autopilot](#windows-autopilot-eula-dismissal) a continuación para obtener información importante a tener en cuenta acerca de la omisión de la página del CLUF durante la instalación de Windows.

Se aplican los permisos de administración de dispositivos y el perfil y limitaciones siguientes:

- Los partners de CSP pueden seguir administrar los perfiles de Autopilot para los clientes existentes con los que tienen relaciones de revendedor, incluso si los clientes han quitado los privilegios de administración delegada del partner.

- Puedes administrar los dispositivos existentes para los clientes que se han agregado por el usuario o por otro partner de CSP.

- No puedes administrar dispositivos que se haya cargado tu cliente a Microsoft Store para empresas o el Portal de Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Crear y administrar perfiles Autopilot en el centro de partners

En el centro de partners, puedes crear perfiles de implementación de Windows Autopilot y aplicarlos a los dispositivos.

>[!NOTE]
>Crear y aplicar los perfiles sólo los agentes de administración.

### <a name="create-a-new-autopilot-profile"></a>Crear un nuevo perfil de Autopilot

1. Selecciona **los clientes** en el menú del centro de partners y, a continuación, selecciona al cliente que vas a crear el perfil de Autopilot para.

2. En la página de detalles del cliente, selecciona **los dispositivos**.

3. En **los perfiles de Windows Autopilot** selecciona **Agregar nuevo perfil**.

4. Escribe el nombre y una descripción del perfil y, a continuación, configura las opciones de configuración rápida. Elegir entre:  

   - Omitir la configuración de privacidad en configuración

   - Deshabilitar la cuenta de administrador local en el programa de instalación
  
   - Omitir automáticamente las páginas durante la instalación<br>
        (Incluye *páginas de configuración de registro de OEM, OneDrive y omitir Cortana*y *Seleccionar automáticamente la configuración de trabajo o escuela* )
  
   - Omitir contrato de licencia de usuario final (CLUF)<br> 
       >[!IMPORTANT] 
       >Consulta [desestimación del CLUF de Windows Autopilot](#windows-autopilot-eula-dismissal) a continuación para obtener información importante a tener en cuenta acerca de la omisión de la página del CLUF durante la instalación de Windows.

5. Selecciona **Enviar** cuando hayas acabado.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Aplicar un perfil de Autopilot a dispositivos de los clientes

>[!NOTE]
>Las siguientes instrucciones se suponen que ya has agregado dispositivos del cliente al centro de partners y que puedes acceder a su lista de dispositivos. Si aún no ha agregado dispositivos del cliente, sigue las instrucciones de [Agregar dispositivos a una cuenta de cliente](#add-devices-to-a-customers-account) y, a continuación, sigue los pasos siguientes.

Después de crear un perfil de Autopilot para un cliente, se puede aplicar a los dispositivos del cliente.

1. Selecciona **los clientes** en el menú del centro de partners y, a continuación, selecciona al cliente que creó el perfil de Autopilot para.

2. En la página de detalles del cliente, selecciona **los dispositivos**.

3. En **los perfiles de aplicar a dispositivos** selecciona los dispositivos o grupos de dispositivos que quieres agregar perfiles para y, a continuación, seleccione **Aplicar perfil**. El perfil que aplica solo aparece en la columna **perfil** .

4. Sigue los pasos siguientes para comprobar que el perfil se aplicará correctamente en el dispositivo.

    a.  Conecta un dispositivo a la red y enciéndelo.

    b.  Comprueba que aparezcan las pantallas OOBE apropiadas (si es el caso).

    c.  Cuando se detiene el proceso OOBE, restablece el dispositivo a su configuración predeterminada de fábrica para prepararlo para un usuario nuevo.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Quitar un perfil de Autopilot de dispositivo de un cliente

1. Selecciona **los clientes** en el menú del centro de partners y, a continuación, selecciona al cliente que creó el perfil de Autopilot para.

2. En la página de detalles del cliente, selecciona **los dispositivos**.

3. En **los perfiles de aplicar a dispositivos de** seleccionar los dispositivos que quieres quitar el perfil y, a continuación, selecciona **quitar perfil**.

   >[!NOTE]
   >Quitar un perfil de un dispositivo no elimina el perfil de la lista. Si quieres eliminar un perfil, sigue las instrucciones de [actualización o eliminar un perfil de Autopilot](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Actualizar o eliminar un perfil de Autopilot

Si un cliente quiere cambiar la experiencia out-of-box después de que hayas enviado los dispositivos a ellos, puedes cambiar el perfil del centro de partners.

Cuando el dispositivo del cliente se conecta a internet, que descargue la versión más reciente del perfil durante el proceso OOBE. También, cada vez que un cliente restaura un dispositivo con la configuración predeterminada de fábrica, el dispositivo se vuelve a descargar la versión más reciente del perfil durante el proceso OOBE.

1. Selecciona **los clientes** en el menú del centro de partners y, a continuación, selecciona al cliente que quiere cambiar un perfil de Autopilot.

2. En la página de detalles del cliente, selecciona **los dispositivos**.

3. En **los perfiles de Windows Autopilot** selecciona el perfil que tengas que actualizar. Realice los cambios necesarios y, a continuación, selecciona **Enviar**.

Para eliminar el perfil, selecciona **eliminar el perfil** de la esquina superior derecha de la página.

### <a name="add-devices-to-a-customers-account"></a>Agregar dispositivos a una cuenta de cliente

>[!NOTE]
>Los agentes de ventas y los agentes de administración pueden agregar dispositivos a una cuenta de cliente.

Antes de que se pueden aplicar perfiles personalizados de Autopilot para dispositivos de los clientes, debe tener acceso a la lista de dispositivos del cliente.

Si vas a usar el nombre de OEM, el número de serie y la combinación de modelo, ten en cuenta estas limitaciones:

- Funciona tupla solo para dispositivos más recientes (4 k hash, por ejemplo) y no se admite para 128b hash (RS2 y dispositivos anteriores).

- El registro de tupla distingue mayúsculas de minúsculas, por lo que los datos en el archivo deben coincidir con el fabricante y modelo de nombres ***exactamente*** como proporcionada por el proveedor de OEM (proveedor de hardware).

Sigue estas instrucciones para agregar dispositivos a una cuenta de cliente en el centro de partners.

1. Selecciona **los clientes** en el menú del centro de partners y, a continuación, selecciona al cliente cuyos dispositivos que quieres administrar.

2. En la página de detalles del cliente, selecciona **los dispositivos**.

3. En **los perfiles de aplicar a dispositivos** selecciona **Agregar dispositivos**.

4. Escribe un nombre para la lista de dispositivos y, a continuación, selecciona **Examinar** para cargar la lista del cliente (en formato de archivo .csv) al centro de partners.

    >[!NOTE]
    >Debería haber recibido este archivo .csv con la compra del dispositivo. Si no recibes un archivo .csv, puedes crear una tú mismo siguiendo los pasos de [Agregar dispositivos a Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Carga el archivo .csv y, a continuación, selecciona **Guardar**.

Si recibes un mensaje de error al intentar cargar el archivo .csv, comprueba el formato del archivo. Puedes usar solo el hash de hardware o el nombre del OEM, número de serie y modelo (en ese orden de columna) o el identificador de producto de Windows. También puedes usar el archivo .csv de muestra proporcionado desde el vínculo situado junto a **Agregar dispositivos** para crear una lista de dispositivos.

## <a name="windows-autopilot-eula-dismissal"></a>Desestimación del CLUF de Windows Autopilot

### <a name="important-information"></a>INFORMACIÓN IMPORTANTE

Windows Autopilot te permite configurar instalaciones personalizadas de Windows en dispositivos que administras para tus clientes. Si autorizado no lo haces, el cliente, puedes suprimir u ocultar determinadas pantallas de configuración que normalmente se muestran a los usuarios al configurar Windows, incluida la pantalla de aceptación de términos (contrato de licencia de usuario final).

Al usar esta función, aceptas suprimir u ocultar cualquiera de las pantallas que está diseñada para proporcionar a los usuarios aviso o aceptación de los medios de términos que has obtenido consentimiento suficiente y la autorización del cliente para ocultar los términos y que, en nombre de el cliente (si una organización o un usuario individual como el caso de que puede ser), autorizas notificaciones y aceptas los términos aplicables al cliente. Esto incluye que estás de acuerdo con los términos y condiciones de la licencia o el anuncio que se presenta al usuario si no la suprimiste u ocultaste con esta herramienta. Tu cliente no puede usar el software de Windows en esos dispositivos si ha adquirido de manera válida una licencia para el software desde Microsoft o sus distribuidores con licencia.