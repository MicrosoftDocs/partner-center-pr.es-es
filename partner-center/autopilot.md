---
title: "Agregar un perfil de implementaciones sin interacción para simplificar la configuración del dispositivo con Autopilot de Windows | Centro de partners"
description: "Agregar un perfil de implementaciones sin interacción en el Centro de partners para simplificar la configuración del dispositivo con Autopilot de Windows"
author: KPacquer
keywords: "autopilot, autopilot de windows, microsoft autopilot, ztd, sin interacción, oobe, pantallas de inicio de sesión"
robots: NOINDEX,NOFOLLOW
ms.openlocfilehash: c51d9204b352b548a4095e96944aacdbcde97fa2
ms.sourcegitcommit: c2a12d6a18b9631916f6dd8301a4752ecc03296b
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/19/2017
---
# <a name="add-a-zero-touch-deployment-profile-to-simplify-device-setup-with-windows-autopilot"></a>Agregar un perfil de implementaciones sin interacción para simplificar la configuración del dispositivo con Autopilot de Windows

Autopilot de Windows puede simplificar y proteger la instalación del dispositivo para los nuevos dispositivos de Windows 10 Pro desde el primer arranque en tan solo unos pasos. 

## <a name="features"></a>Características

*  **Deshabilitar los permisos de administrador local** para los usuarios finales que configuren los dispositivos
*  **Mostrar la página de inicio de sesión de una organización**. La organización puede predefinir una página de inicio de sesión que agrega el dispositivo como un dispositivo de trabajo y se une el dispositivo con Azure Active Directory.
*  **Inscribir el dispositivo en un MDM**, por ejemplo: Microsoft Intune, una vez que OOBE se ha completado.
*  **Simplificar la experiencia OOBE** para usar solo los pasos y las decisiones necesarias, utilizando un perfil de implementación sin interacción (ZTD). 

## <a name="requirements"></a>Requisitos

*  Dispositivos preinstalados con Windows 10 Pro Creators Update (versión 1703 o posterior)
*  Identificador de dispositivo conocido como un hash del hardware (128 HWH o 4k HWH), normalmente proporcionado por un OEM. Usarás los identificadores para asignar los perfiles de la organización en el Centro de partners.
*  Los dispositivos deben tener acceso a Internet. Cuando no se puede conectar el dispositivo, la experiencia OOBE se mostrará de forma predeterminada en las pantallas.
*  Inscribir el dispositivo en un MDM requiere Azure Active Directory Premium.

## <a name="add-organization-login-pages-to-oobe"></a>Agregar las páginas de inicio de sesión de la organización a OOBE

Para agregar las páginas específicas de la organización, agrega los dispositivos al [directorio de Azure AD](https://go.microsoft.com/fwlink/?linkid=848958) de la organización y crea páginas de inicio de sesión.


## <a name="remove--windows-pages-from-oobe-with-a-zero-touch-deployment-ztd-profile"></a>Quitar páginas de Windows de OOBE con un perfil de implementación sin interacción (ZTD)

### <a name="examples-of-settings-in-a-ztd-profile"></a>Ejemplos de configuración en un perfil ZTD
*  Omitir la configuración de privacidad durante la instalación
*  Deshabilitar la cuenta de administrador local en el programa de instalación
*  Omitir automáticamente las páginas durante la instalación
   *  Seleccionar automáticamente la configuración de trabajo o centro docente
   *  Omitir páginas de configuración de registro de OEM, OneDrive y Cortana

### <a name="add-devices-and-apply-a-profile"></a>Agregar dispositivos y aplicar un perfil

En el Centro de partners, puedes crear un perfil ZTD y aplicarlo a una lista de dispositivos.

Para configurar los dispositivos, sube una lista de los dispositivos al Centro de partners, crea un perfil que se aplique a los dispositivos y aplícala.

1.  Agrega la lista de dispositivo al Centro de partners. (Los agentes de ventas y los agentes de administración tienen acceso para agregar la lista de dispositivos al Centro de partners).

    a.  Solicitar el OEM un archivo .csv que enumera los nuevos dispositivos. Este archivo contiene el número de serie, el Id. del producto y el identificador de dispositivo generados desde la herramienta OEM Activation 3.0. 

    b.  Desde el panel del Centro de partners, ve a **Clientes** > selecciona el cliente que recibe los dispositivos > **Dispositivos > Agregar dispositivos**.

    c.  Pon nombre al lote de dispositivos, por ejemplo, "equipos del departamento de ventas de Contoso, pedido de abril de 2017". 

    d.  Haz clic en **Examinar** > selecciona el archivo de información de dispositivo > **Validar**.

2.  Crea un perfil que se pueda aplicar a los dispositivos. (Sólo los agentes de administración tienen acceso para crear y aplicar los perfiles en el Centro de partners).

    a.  Desde **Dispositivos**, haz clic en **Agregar nuevo perfil**.

    b.  Pon un nombre al perfil, por ejemplo, "perfil de Escritorio Contoso – Omitir el proceso OOBE por completo".

    c.  Configura las opciones de OOBE. Por ejemplo, activa **Omitir la configuración rápida en el programa de instalación**.

    d.  Haz clic en **Enviar**.

3.  Aplicar el perfil.

    a.  Desde **Dispositivos**, en el panel **Asignar y eliminar dispositivos**, selecciona los dispositivos que quieras configurar. Para seleccionar un lote completo, haz clic en la casilla de verificación junto al nombre del lote (por ejemplo, "equipos del departamento de ventas de Contoso, pedido de marzo de 2017").

    b.  Haz clic en **Aplicar perfil**y selecciona el perfil (por ejemplo, "perfil de Escritorio Contoso – omitir todos los OOBE"). Los dispositivos mostrarán el perfil en la columna Perfil.

4.  Opcional: Comprueba que tu perfil funciona.

    a.  Conecta un dispositivo a la red y enciéndelo.

    b.  Comprueba que aparezcan las pantallas OOBE apropiadas (si es el caso).

    c.  Para preparar el dispositivo para un usuario nuevo, completa la experiencia OOBE y, a continuación, restablece el dispositivo a la configuración predeterminada de fábrica.


## <a name="to-update-or-delete-a-profile"></a>Actualizar o eliminar un perfil 

Una vez que hayas asignado un perfil a un dispositivo, puedes actualizarlo, incluso si ya has entregado el dispositivo al cliente. Cuando el dispositivo se conecte a Internet, descarga la versión más reciente de tu perfil durante el proceso OOBE. Si el cliente restaura su dispositivo con la configuración predeterminada de fábrica, el dispositivo descargará de nuevo las últimas actualizaciones a tu perfil. 

###<a name="you-can-remove-a-profile-from-a-device"></a>Puedes quitar un perfil de un dispositivo.
1. Selecciona el dispositivo (o el lote de dispositivos) del que quieras quitar el perfil. 

2. En el panel **Asignar y eliminar dispositivos**, selecciona **Quitar perfil**.

3. Ve al perfil que quieras quitar y elimínalo. El perfil se eliminará de todos los dispositivos.


Desde **Dispositivos**, selecciona el perfil. Aquí podrás modificar la configuración existente.

