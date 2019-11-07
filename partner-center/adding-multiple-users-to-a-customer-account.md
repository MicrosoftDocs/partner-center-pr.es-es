---
title: Crear varios usuarios para una cuenta de cliente | Centro de partners
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Puedes agregar varios usuarios a la vez a una cuenta de cliente, mediante la carga en el Centro de partners de un archivo de datos con el formato de archivo de valores separados por comas (.csv).
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: carga masiva, agregar varios usuarios a una cuenta de cliente, agregar usuarios del cliente, carga masiva de usuarios del cliente, cuenta del cliente, usuarios del cliente, usuarios
ms.localizationpriority: medium
ms.openlocfilehash: 4062c36d9f5d394d9d25eb67265784d2a5b301cf
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/06/2019
ms.locfileid: "73653243"
---
# <a name="add-multiple-users-to-a-customer-account"></a>Agregar varios usuarios a una cuenta de cliente

**Se aplica a**

-  Centro de partners

Puede agregar varios usuarios a la cuenta de un cliente a la vez, cargando un archivo de datos en el formato de archivo de valores separados por comas (. csv) al centro de Partners. Puede descargar un archivo de datos de ejemplo del centro de Partners y editarlo para su uso, o puede crear un nuevo archivo de datos con el modelo de datos definido a continuación.

## <a href="" id="creatingtheimportcsvfile"></a>Requisitos del archivo de datos


Para agregar varios usuarios a la cuenta de un cliente mediante el proceso de carga masiva, debe cumplir los siguientes requisitos:

-   Debes tener permisos de administrador global para la cuenta de cliente.
-   Cada usuario debe tener una dirección de correo electrónico exclusiva, anexa a los dominios de correo electrónico del cliente.
-   Puedes subir hasta 100 registros a la vez. Si es necesario agregar más de 100 usuarios, crea y sube archivos de datos adicionales.
-   Todos los usuarios deben estar en la misma **ubicación** geográfica.
-   Escribe solo los datos que se describen a continuación. Unos datos extraños hará que la carga sufra un error.

Escribe los siguientes datos en el archivo de datos:

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **Nombre de columna** | **Descripción**                                                              | **Única**                             |
| Nombre      | Nombre del usuario (campo opcional)                                           | Límite de 50 caracteres                         |
| Apellidos       | Los apellidos del usuario (campo opcional)                                            | Límite de 50 caracteres                         |
| Nombre para mostrar    | Nombre mostrado en el centro de Partners (campo obligatorio)                            | Límite de 50 caracteres                         |
| Correo electrónico           | Dirección de correo electrónico empresarial del usuario en la empresa del cliente (campo obligatorio)           | Cada usuario debe tener una dirección de correo electrónico exclusiva. |
| Actualización de estado   | Se usa para indicar si el nuevo registro de usuario se ha creado correctamente o no. | \*\*deje\*vacío \*                        |

 

### <a href="" id="createmultipleuseraccounts"></a>Para crear varias cuentas de usuario

<a href="" id="creatingtheaccounts"></a>
1.  Crea un archivo de datos de valores separados por comas (.csv) con los datos que se han descrito anteriormente. Guarda el archivo para que puedas acceder a él en un paso posterior.
2.  En el menú del **centro de Partners** , seleccione **clientes**y, a continuación, elija un cliente de la lista.
3.  Selecciona **Subir usuarios**.
4.  En **Subir información de usuarios**, selecciona **Examinar**.
5.  En el selector de archivos, selecciona el archivo de datos y, a continuación, selecciona **Abrir**.
6.  Selecciona **Validar**.

    **Tenga** en cuenta  la mayoría de los errores de creación de cuentas están causados por problemas de archivos de datos, como información que falta, direcciones de correo electrónico con formato incorrecto o duplicado o demasiados registros en el archivo.

7.  Una vez que el centro de Partners valida el archivo, seleccione la **Ubicación** geográfica para los nuevos usuarios.
8.  Selecciona **Guardar**.
9.  Descarga la información de la contraseña temporal para los usuarios.

**IMPORTANTE:** Asegúrate de descargar el archivo con las contraseñas temporales ahora, ya no podrás hacerlo más adelante. Los nuevos usuarios deben iniciar sesión en su nueva cuenta con las contraseñas temporales correspondientes a sus nuevas cuentas.

10. Los nuevos usuarios reciben asignación automática de permisos de **Puede usar licencias y servicios**. 

 

 



