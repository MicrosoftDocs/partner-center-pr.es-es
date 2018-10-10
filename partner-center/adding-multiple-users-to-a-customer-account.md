---
title: Crear varios usuarios para una cuenta de cliente | Centro de partners
description: Puedes agregar varios usuarios a la vez a una cuenta de cliente, mediante la carga en el Centro de partners de un archivo de datos con el formato de archivo de valores separados por comas (.csv).
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
keywords: carga masiva, agregar varios usuarios a una cuenta de cliente, agregar usuarios del cliente, carga masiva de usuarios del cliente, cuenta del cliente, usuarios del cliente, usuarios
ms.localizationpriority: medium
ms.openlocfilehash: 123c2c7b80398a860aa894449052502d41409c85
ms.sourcegitcommit: 123a7f53d633c27eb5f982926d856de47afb1042
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/09/2018
ms.locfileid: "4488821"
---
# <a name="add-multiple-users-to-a-customer-account"></a>Agregar varios usuarios a una cuenta de cliente

**Se aplica a**

-  Centro de partners

Puedes agregar varios usuarios a una cuenta de cliente al mismo tiempo, cargando un archivo de datos en el formato de archivo de valores separados por comas (.csv) en el centro de partners. Puedes descargar un archivo de datos de muestra desde el centro de partners y después modificarlo para usarlo, o puedes crear un nuevo archivo de datos mediante el modelo de datos que se define a continuación.

## <a href="" id="creatingtheimportcsvfile"></a>Requisitos del archivo de datos:


Para agregar varios usuarios a la cuenta de un cliente mediante el proceso de carga masiva, es necesario cumplir los siguientes requisitos:

-   Debes tener permisos de administrador global para la cuenta de cliente.
-   Cada usuario debe tener una dirección de correo electrónico exclusiva, anexa a los dominios de correo electrónico del cliente.
-   Puedes subir hasta 100 registros a la vez. Si es necesario agregar más de 100 usuarios, crea y sube archivos de datos adicionales.
-   Todos los usuarios deben estar en la misma **ubicación** geográfica.
-   Escribe solo los datos que se describen a continuación. Unos datos extraños hará que la carga sufra un error.

Escribe los siguientes datos en el archivo de datos:

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **Nombre de columna** | **Descripción**                                                              | **Limitaciones**                             |
| Nombre      | El nombre de pila del usuario (campo opcional)                                           | Límite de 50 caracteres                         |
| Apellidos       | Los apellidos del usuario (campo opcional)                                            | Límite de 50 caracteres                         |
| Nombre para mostrar    | Nombre que aparece en el centro de partners (campo obligatorio)                            | Límite de 50 caracteres                         |
| Correo electrónico           | La dirección de correo electrónico comercial del usuario en la compañía del cliente (campo obligatorio).           | Cada usuario debe tener una dirección de correo electrónico exclusiva. |
| Actualización de estado   | Se usa para indicar si el nuevo registro de usuario se ha creado correctamente o no. | \*\*Dejar vacío\* \ *                        |

 

### <a href="" id="createmultipleuseraccounts"></a>Para crear varias cuentas de usuario

<a href="" id="creatingtheaccounts"></a>
1.  Crea un archivo de datos de valores separados por comas (.csv) con los datos que se han descrito anteriormente. Guarda el archivo para que puedas acceder a él en un paso posterior.
2.  En el menú del **Centro de partners** , selecciona **los clientes**y luego elige a un cliente de la lista.
3.  Selecciona **Subir usuarios**.
4.  En **Subir información de usuarios**, selecciona **Examinar**.
5.  En el selector de archivos, selecciona el archivo de datos y, a continuación, selecciona **Abrir**.
6.  Selecciona **Validar**.

    **Nota**: La mayoría de los errores de creación de cuentas se deben a problemas en los archivos de datos, lo que incluye la falta de información, unas direcciones de correo electrónico con formato incorrecto o duplicadas o un exceso de registros en el archivo.

7.  Cuando el centro de partners haya validado el archivo, selecciona la **ubicación** geográfica para los nuevos usuarios.
8.  Selecciona **Guardar**.
9.  Descarga la información de la contraseña temporal para los usuarios.

**IMPORTANTE:** Asegúrate de descargar el archivo con las contraseñas temporales ahora, ya no podrás hacerlo más adelante. Los nuevos usuarios deben iniciar sesión en su nueva cuenta con las contraseñas temporales correspondientes a sus nuevas cuentas.

10. Los nuevos usuarios se les asignará automáticamente los permisos de **Usar licencias y servicios** . 

 

 



