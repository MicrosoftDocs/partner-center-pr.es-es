---
title: Personalizar la experiencia de out-of-box de un dispositivo con perfiles de Windows Autopilot | Centro de partners
description: Preconfigurar la experiencia de out-of-box de un dispositivo con perfiles de Autopilot.
ms.topic: article
ms.date: 03/18/19
author: maggiepuccievans
ms.author: evansma
keywords: AutoPilot, autopilot de windows, autopilot de microsoft, una implementación sin retoques, oobe, pantallas de inicio de sesión, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: e940a7ccf79f6b43d3712a2f3ae2f9b150e1473e
ms.sourcegitcommit: f5dbd07185059aa5faddf1c5daa556f634ce97ee
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/19/2019
ms.locfileid: "58162225"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Personalizar la experiencia de out-of-box de un dispositivo con perfiles de Windows Autopilot

**Se aplica a**

- Asociados de CSP directo factura, los proveedores indirectos y revendedores indirectos

Si administra dispositivos de cliente, deberá personalizar la experiencia de out-of-box (OOBE) para los usuarios del cliente. Puede configurar previamente los nuevos dispositivos con perfiles de Windows Autopilot antes de entregar los dispositivos a los clientes y aplicar nuevos perfiles para dispositivos clientes ya han adquirido. En este artículo se explica cómo crear y aplicar los perfiles de Autopilot en dispositivos de centro de partners.

Si no ya está familiarizado con el piloto automático, revise la información en estos artículos:

- [Información general de Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Guía de referencia de implementación de AutoPilot](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Información general

Con la característica de Windows Autopilot en Centro de partners, puede crear perfiles personalizados para aplicar a los dispositivos cliente. La siguiente configuración del perfil estaba disponible en el momento en que se publicó este artículo:

- Omitir la configuración de privacidad. Esta configuración de perfil de Autopilot opcional permite a las organizaciones no preguntar sobre la configuración de privacidad durante el proceso de OOBE.

- Deshabilitar la creación de la cuenta de administrador local en el dispositivo. Las organizaciones pueden decidir si el usuario configura el dispositivo debe tener acceso de administrador, una vez completado el proceso.

- Configurar automáticamente dispositivos de empresa o centro educativo. Todos los dispositivos registrados con Autopilot automáticamente se considerará trabajo o educativas de los dispositivos, por lo que esta pregunta no se les pedirá durante el proceso de OOBE.

- Omitir las páginas de instalación del registro de OEM, OneDrive y Cortana. Todos los dispositivos registrados con Autopilot omitirá automáticamente estas páginas durante el proceso de configuración de-rápida (OOBE).

- Omitir el contrato de licencia de usuario final (CLUF). A partir de Windows 10 versión 1709, las organizaciones pueden decidir omitir la página del CLUF presentada durante el proceso OOBE. Consulte [despido de términos de licencia de Windows Autopilot](#windows-autopilot-eula-dismissal) a continuación para que obtener información importante a tener en cuenta acerca de la omisión de la página del CLUF Windows durante la instalación.

Se aplican los siguientes permisos de administración de perfil y el dispositivo y limitaciones:

- Los asociados de CSP pueden seguir administrar perfiles de Autopilot para los clientes existentes con los que tienen relaciones de distribuidor, incluso si los clientes han quitado privilegios de administración delegada del asociado.

- Puede administrar los dispositivos existentes para los clientes que se han agregado.

- No puede administrar dispositivos de que su cliente ha cargado en Microsoft Store para empresas o el Portal de Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Crear y administrar perfiles de Autopilot en Centro de partners

En el centro de partners, puede crear perfiles de Windows Autopilot deployment y aplicarlas a los dispositivos.

>[!NOTE]
>Solo los agentes de administración pueden crear y aplicar los perfiles.

### <a name="create-a-new-autopilot-profile"></a>Crear un nuevo perfil de Autopilot

1. Seleccione **clientes** desde el menú de centro de partners y, a continuación, seleccione el cliente que está creando el perfil de Autopilot para.

2. En la página de detalles del cliente, seleccione **dispositivos**.

3. En **perfiles de Windows Autopilot** seleccione **Agregar nuevo perfil**.

4. Escriba el nombre y una descripción del perfil y, a continuación, configure las opciones de bienvenida de Windows. Elegir entre:  

   - Omitir la configuración de privacidad en el programa de instalación

   - Deshabilitar la cuenta de administrador local en el programa de instalación
  
   - Omitir automáticamente las páginas durante la instalación<br>
        (Incluye *seleccionar automáticamente la configuración para el trabajo o escuela* y *páginas de configuración de registro de OEM, OneDrive y Skip Cortana*)
  
   - Omitir el contrato de licencia de usuario final (CLUF)<br> 
       >[!IMPORTANT] 
       >Consulte [despido de términos de licencia de Windows Autopilot](#windows-autopilot-eula-dismissal) a continuación para que obtener información importante a tener en cuenta acerca de la omisión de la página del CLUF Windows durante la instalación.

5. Selecciona **Enviar** cuando hayas acabado.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Un perfil de Autopilot se aplican a dispositivos de cliente

>[!NOTE]
>Las instrucciones siguientes se suponen que ya ha agregado los dispositivos del cliente al centro de partners y que puede tener acceso a su lista de dispositivos. Si aún no ha agregado los dispositivos del cliente, siga las instrucciones de [agregar dispositivos a una cuenta de cliente](#add-devices-to-a-customers-account) y, a continuación, siga los pasos siguientes.

Después de crear un perfil de Autopilot para un cliente, puede aplicarla a los dispositivos del cliente.

1. Seleccione **clientes** desde el menú de centro de partners y, a continuación, seleccione el cliente que creó para el perfil de Autopilot.

2. En la página de detalles del cliente, seleccione **dispositivos**.

3. En **perfiles se aplican a dispositivos** seleccione los dispositivos o grupos de dispositivos que desea agregar a los perfiles y, a continuación, seleccione **aplicar perfil**. El perfil que acaba de aplicar aparece en el **perfil** columna.

4. Siga los pasos siguientes para comprobar que el perfil se aplicará correctamente al dispositivo.

    a.  Conectar un dispositivo a la red y enciéndalo.

    b.  Comprueba que aparezcan las pantallas OOBE apropiadas (si es el caso).

    c.  Cuando se detiene el proceso OOBE, restablecer el dispositivo a la configuración predeterminada de fábrica para prepararlo para un usuario nuevo.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Quitar un perfil de Autopilot de dispositivo del cliente

1. Seleccione **clientes** desde el menú de centro de partners y, a continuación, seleccione el cliente que creó para el perfil de Autopilot.

2. En la página de detalles del cliente, seleccione **dispositivos**.

3. En **perfiles se aplican a dispositivos** seleccione los dispositivos que desea quitar el perfil de y, a continuación, seleccione **quitar perfil**.

   >[!NOTE]
   >Quitar un perfil de un dispositivo no elimina el perfil de la lista. Si desea eliminar un perfil, siga las instrucciones de [Update o delete de un perfil de Autopilot](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Actualizar o eliminar un perfil de Autopilot

Si un cliente quiere cambiar la configuración rápida después de haber enviado los dispositivos que les, puede cambiar el perfil en el centro de partners.

Cuando el dispositivo del cliente se conecta a internet, descargará la última versión de perfil durante el proceso de OOBE. Además, siempre que un cliente restaura un dispositivo a la configuración predeterminada de fábrica, el dispositivo nuevo descargará la última versión de perfil durante el proceso de OOBE.

1. Seleccione **clientes** en el menú de centro de partners y a continuación, seleccione el cliente que desea cambiar un perfil de Autopilot.

2. En la página de detalles del cliente, seleccione **dispositivos**.

3. En **perfiles de Windows Autopilot** seleccione el perfil que se debe actualizar. Realice los cambios necesarios y, a continuación, seleccione **enviar**.

Para eliminar este perfil, seleccione **eliminar perfil** desde la esquina superior derecha de la página.

### <a name="add-devices-to-a-customers-account"></a>Agregar dispositivos a una cuenta de cliente

>[!NOTE]
>Los agentes de ventas y los agentes de administración pueden agregar dispositivos a una cuenta de cliente.

Antes de aplicar los perfiles de Autopilot personalizados a los dispositivos de cliente, debe poder tener acceso a la lista de dispositivos del cliente.

Si tiene previsto usar el nombre, número de serie y combinación de modelos de OEM, tenga en cuenta estas limitaciones:

- Esta tupla solo funciona para los dispositivos más recientes (4 k hashes, por ejemplo) y no es compatible con hashes de 128b (RS2 y dispositivos anteriores).

- El registro de la tupla distingue mayúsculas de minúsculas, por lo que los datos en el archivo deben coincidir con los nombres de modelo y fabricante ***exactamente*** proporcionados por el proveedor OEM (proveedor de hardware).

Siga las instrucciones siguientes para agregar dispositivos a una cuenta de cliente en el centro de partners.

1. Seleccione **clientes** en el menú de centro de partners y, a continuación, seleccione el cliente cuyos dispositivos desea administrar.

2. En la página de detalles del cliente, seleccione **dispositivos**.

3. En **perfiles se aplican a dispositivos** seleccione **agregar dispositivos**.

4. Escriba un nombre para la lista de dispositivos y, a continuación, seleccione **examinar** para cargar la lista del cliente (en formato de archivo .csv) al centro de partners.

    >[!NOTE]
    >Debe haber recibido este archivo .csv con la compra de dispositivo. Si no ha recibido un archivo .csv, puede crear uno usted mismo, siga los pasos descritos en [agregar dispositivos a Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Cargue el archivo .csv y, a continuación, seleccione **guardar**.

Si recibe un mensaje de error al intentar cargar el archivo .csv, compruebe el formato del archivo. Puede usar solo, el hash del hardware o el nombre del OEM, número de serie y modelo (en ese orden de columna) o el identificador de producto de Windows. También puede usar el archivo .csv de ejemplo proporcionado en el vínculo junto a **agregar dispositivos** para crear una lista de dispositivos.

## <a name="windows-autopilot-eula-dismissal"></a>Despido de términos de licencia de Windows Autopilot

### <a name="important-information"></a>INFORMACIÓN IMPORTANTE

Windows Autopilot le permite configurar instalaciones personalizadas de Windows en dispositivos administrados para sus clientes. Si dispone de autorización para hacerlo por el cliente, puede suprimir u ocultar determinadas pantallas de instalación que normalmente se presentan a los usuarios al configurar Windows, incluida la pantalla de aceptación de términos de licencia (contrato de licencia de usuario final).

Mediante el uso de esta función, acepta al suprimir u ocultación de ninguna de las pantallas que está diseñada para proporcionar a los usuarios con notificación o aceptación de significa términos que haya obtenido suficiente consentimiento y autorización de su cliente para ocultar los términos y que usted, en nombre de el cliente (si una organización o un usuario individual en su caso puede ser), da su consentimiento para los avisos y aceptar cualquiera los términos que son aplicables a su cliente. Esto incluye que estás de acuerdo con los términos y condiciones de la licencia o el anuncio que se presenta al usuario si no la suprimiste u ocultaste con esta herramienta. Tu cliente no puede usar el software de Windows en esos dispositivos si ha adquirido de manera válida una licencia para el software desde Microsoft o sus distribuidores con licencia.