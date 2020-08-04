---
title: Campos del archivo. csv para importar varios usuarios para una cuenta de cliente
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para agregar varios usuarios a una cuenta de cliente, cree un archivo de valores separados por comas (. csv) con los campos correspondientes.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/03/2020
ms.locfileid: "87528189"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Agregar varios usuarios a una cuenta de cliente mediante la creación de un archivo. csv

**Se aplica a**

- Centro de partners

**Roles adecuados**

- Administrador global

Agregue varios usuarios a la cuenta de un cliente a la vez, cargando un archivo de datos en el formato de archivo de valores separados por comas (. csv) en el centro de Partners. Puede descargar un archivo de datos de ejemplo del centro de Partners y editarlo para su uso, o puede crear un nuevo archivo de datos con el modelo de datos definido a continuación.

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

## <a name="next-steps"></a>Pasos siguientes

- [Cómo agregar varios usuarios a un cliente](adding-multiple-users-to-a-customer-account.md)