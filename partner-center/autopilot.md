---
title: Simplificar la configuración del dispositivo con Autopilot de Windows | Centro de partners
ms.topic: article
ms.date: 10/29/2018
description: Agregar un perfil de implementación de AutoPilot de Windows en el Centro de partners para simplificar la configuración del dispositivo con AutoPilot de Windows
author: KPacquer
ms.author: kenpacq
keywords: autopilot, autopilot de windows, microsoft autopilot, implementación sin interacción, oobe, pantallas de inicio de sesión
ms.localizationpriority: medium
ms.openlocfilehash: 2c8e8953fbb79493a3704c9c8ea6982928c3fe92
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/29/2018
ms.locfileid: "5796658"
---
# <a name="simplify-device-setup-with-windows-autopilot"></a>Simplificar la configuración del dispositivo con AutoPilot de Windows 

AutoPilot de Windows simplifica y protege la configuración del dispositivo para los nuevos dispositivos de Windows 10 Pro desde el primer arranque en tan solo unos pasos. Para obtener más información, consulta [Introducción a AutoPilot de Windows](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot).

## <a name="features"></a>Características

*  **Deshabilitar los permisos de administrador local** para los usuarios finales que configuren los dispositivos
*  **Mostrar la página de inicio de sesión de una organización**. La organización puede predefinir una página de inicio de sesión que agrega el dispositivo como un dispositivo de trabajo y se une el dispositivo con Azure Active Directory.
*  **Inscribir el dispositivo en un Administrador de dispositivos móviles (MDM)**, como por ejemplo, Microsoft Intune, una vez que OOBE se ha completado.
*  **Simplificar la experiencia OOBE** para usar solo los pasos y las decisiones necesarias, utilizando un perfil de implementación de AutoPilot de Windows. 

## <a name="requirements"></a>Requisitos

*  Dispositivos preinstalados con Windows 10 Pro Creators Update (versión 1703 o posterior) o con Windows 10 Pro for Advanced PCs.
*  Identificador de dispositivo conocido como un hash del hardware (128 HWH o 4k HWH), normalmente proporcionado por un OEM. Usarás identificadores para asignar los perfiles de la organización en el centro de partners. 
*  Los dispositivos deben tener acceso a Internet. Cuando no se puede conectar el dispositivo, la experiencia OOBE se mostrará de forma predeterminada en las pantallas.
*  Inscribir el dispositivo en un MDM requiere Azure Active Directory Premium.

## <a name="add-organization-login-pages-to-oobe"></a>Agregar las páginas de inicio de sesión de la organización a OOBE

Para agregar las páginas específicas de la organización, agrega los dispositivos al [Azure AD Directory](https://go.microsoft.com/fwlink/?linkid=848958) de la organización y crea páginas de inicio de sesión.


## <a name="remove-windows-pages-from-oobe-with-a-windows-autopilot-deployment-profile"></a>Quitar páginas de Windows de OOBE con un perfil de implementación de AutoPilot de Windows

**Ejemplos de configuración de un perfil de implementación de AutoPilot de Windows**
*  Omitir la configuración de privacidad durante la instalación
*  Deshabilitar la cuenta de administrador local en el programa de instalación
*  Omitir automáticamente las páginas durante la instalación
   *  Seleccionar automáticamente la configuración de trabajo o centro docente
   *  Omitir páginas de configuración de registro de OEM, OneDrive y Cortana

### <a name="add-devices-and-apply-a-profile"></a>Agregar dispositivos y aplicar un perfil

Desde el centro de partners, puedes crear un perfil de implementación de Windows AutoPilot y aplicarlo a una lista de los dispositivos.

Para configurar los dispositivos, carga una lista de los dispositivos crea un perfil que se aplique a los dispositivos y aplícalo.

1.  Agrega la lista de dispositivos.

    Los agentes de ventas y los agentes de administración tienen acceso para agregar la lista de dispositivos al Centro de partners.
    
    Los revendedores indirectos pueden trabajar con su proveedor indirecto para agregarla.

    a.  Crea un archivo .csv con el script de PowerShell del tema: [Introducción a AutoPilot de Windows](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot). Este archivo .csv incluye información del dispositivo, como por ejemplo, el número de serie, nombre del OEM, nombre del modelo, id. del producto y el identificador del dispositivo. 

    b.  Desde el centro de partners, ve a **los clientes** > selecciona el cliente que recibe los dispositivos > **dispositivos > agregar dispositivos**.

    c.  Pon nombre al lote de dispositivos, por ejemplo, "equipos del departamento de ventas de Contoso, pedido de abril de 2017". 

    d.  Haz clic en **Examinar** > selecciona el archivo de información de dispositivo > **Validar**.

    **Nota:** Si recibes un mensaje de error después de intentar subir el archivo .csv, comprueba el formato del archivo. Después de agosto, puedes usar solo el Hash de Hardware o el nombre del OEM, número de serie y modelo en ese orden de columna o el id. del producto de Windows. También puedes usar el archivo .csv de muestra al que puedes tener acceso desde el vínculo situado junto a **Agregar dispositivos**.

2.  Crea un perfil que se pueda aplicar a los dispositivos. (Sólo los agentes de administración tienen acceso para crear y aplicar los perfiles en el centro de partners).

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

### <a name="you-can-remove-a-profile-from-a-device"></a>Puedes quitar un perfil de un dispositivo.
1. Selecciona el dispositivo (o el lote de dispositivos) del que quieras quitar el perfil. 

2. En el panel **Asignar y eliminar dispositivos**, selecciona **Quitar perfil**.

3. Ve al perfil que quieras quitar y elimínalo. El perfil se eliminará de todos los dispositivos.

Desde **Dispositivos**, selecciona el perfil. Aquí podrás modificar la configuración existente.

## <a name="windows-autopilot-eula-dismissal--important-information"></a>Desestimación del CLUF de Windows Autopilot: información importante

Esta herramienta te permite configurar instalaciones individuales de Windows en dispositivos que administras para tus clientes. Si tienes la autorización del cliente para hacerlo, puedes suprimir u ocultar determinadas pantallas de configuración que normalmente se muestran a los usuarios al configurar Windows, incluida la pantalla de aceptación de términos de licencia. 

Al usar esta función, aceptas suprimir u ocultar cualquiera de las pantallas que están diseñadas para proporcionar a los usuarios aviso o aceptación de términos significa que has obtenido el consentimiento y la autorización pertinentes el cliente para ocultar los términos y que en nombre del cliente (ya sea una organización o un usuario individual) autorizas notificaciones y aceptas los términos aplicables al cliente. Esto incluye que estás de acuerdo con los términos y condiciones de la licencia o el anuncio que se presenta al usuario si no la suprimiste u ocultaste con esta herramienta. Tu cliente no puede usar el software de Windows en esos dispositivos si ha adquirido de manera válida una licencia para el software desde Microsoft o sus distribuidores con licencia.


