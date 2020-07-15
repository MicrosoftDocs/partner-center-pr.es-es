---
title: Agregar varios usuarios para una cuenta de cliente
ms.topic: article
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo agregar varios usuarios a la cuenta de un cliente a la vez. Cargue un archivo de datos en el centro de Partners con el formato de archivo de valores separados por comas (. csv).
author: parthpandyaMSFT
ms.author: parthp
keywords: carga masiva, adición de varios usuarios a la cuenta de un cliente, adición de usuarios del cliente, carga masiva de usuarios del cliente, cuenta del cliente, usuarios del cliente, usuarios
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 72a1bf634950ac5a445dca894e3925abcae5f645
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377279"
---
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a>Agregar varios usuarios a una cuenta de cliente: cargar un archivo de datos en el centro de Partners

**Se aplica a**

- Centro de partners

**Roles adecuados**

- Administrador global

Puede agregar varios usuarios a la cuenta de un cliente a la vez, cargando un archivo de datos en el formato de archivo de valores separados por comas (. csv) al centro de Partners. Puede descargar un archivo de datos de ejemplo del centro de Partners y editarlo para su uso, o puede crear un nuevo archivo de datos con el modelo de datos definido a continuación.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Requisitos del archivo de datos:

Para agregar varios usuarios a la cuenta de un cliente mediante el proceso de carga masiva, debe cumplir los siguientes requisitos:

- Debes tener permisos de administrador global para la cuenta de cliente.
- Cada usuario debe tener una dirección de correo electrónico exclusiva, anexa a los dominios de correo electrónico del cliente.
- Puedes subir hasta 100 registros a la vez. Si es necesario agregar más de 100 usuarios, crea y sube archivos de datos adicionales.
- Todos los usuarios deben estar en la misma **ubicación** geográfica.
- Escribe solo los datos que se describen a continuación. Unos datos extraños hará que la carga sufra un error.

Escribe los siguientes datos en el archivo de datos:

| **Nombre de la columna** | **Descripción**  | **Limitación**  |
|:-------- |:------  |:----- |
| Nombre  | Nombre del usuario (campo opcional)  | límite de 50 caracteres  |
| Apellidos  | Los apellidos del usuario (campo opcional)  | límite de 50 caracteres  |
| Nombre para mostrar    | Nombre mostrado en el centro de Partners (campo obligatorio)                            | límite de 50 caracteres                         |
| Correo electrónico   | Dirección de correo electrónico empresarial del usuario en la empresa del cliente (campo obligatorio)           | Cada usuario debe tener una dirección de correo electrónico única |
| Actualización del estado   | Se usa para indicar si el nuevo registro de usuario se ha creado correctamente o no. | \*\*Dejar vacío\*\*                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a>Para crear varias cuentas de usuario

<a href="" id="creatingtheaccounts"></a>

1. Crea un archivo de datos de valores separados por comas (.csv) con los datos que se han descrito anteriormente. Guarda el archivo para que puedas acceder a él en un paso posterior.

2. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

3. Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.

4. Seleccione la pestaña **usuarios y licencias** del cliente y, a continuación, seleccione **cargar usuarios**.

5. En **Subir información de usuarios**, selecciona **Examinar**.

6. En el selector de archivos, selecciona el archivo de datos y, a continuación, selecciona **Abrir**.

7. Seleccione **Validar**.

    **Nota:**    La mayoría de los errores de creación de cuentas están causados por problemas de archivos de datos, incluida la información que falta, direcciones de correo electrónico con formato incorrecto o duplicadas o demasiados registros en el archivo.

8. Una vez que el centro de Partners valida el archivo, seleccione la **Ubicación** geográfica para los nuevos usuarios.
9. Seleccione **Guardar**.
10. Descargue la información de contraseña temporal de los usuarios.

**IMPORTANTE:** Asegúrate de descargar el archivo con las contraseñas temporales ahora, ya no podrás hacerlo más adelante. Los nuevos usuarios deben iniciar sesión en su nueva cuenta con las contraseñas temporales correspondientes a sus nuevas cuentas.

10. A los nuevos usuarios se les asignan permisos automáticamente **para utilizar licencias y servicios** . 

 

 



