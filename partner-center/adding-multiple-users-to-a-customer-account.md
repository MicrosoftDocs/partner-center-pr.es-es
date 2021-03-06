---
title: Agregar varios usuarios para una cuenta de cliente
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para agregar varios usuarios a la cuenta de un cliente, cargue un archivo de datos en Centro de partners con el formato de archivo de valores separados por comas (.csv).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150478"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a>Carga de un archivo .csv de usuarios en la cuenta de un cliente


**Roles apropiados**: administrador global

Agregue varios usuarios a la cuenta de un cliente a la vez, cargando un archivo de datos con el formato de archivo de valores separados por comas (.csv) en el Centro de partners. 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a>Creación del archivo de usuarios del cliente y carga en la cuenta de cliente

1. Crea un archivo de datos de valores separados por comas (.csv) con los datos que se han descrito anteriormente. Guarda el archivo para que puedas acceder a él en un paso posterior. Consulte [Campos para el archivo .csv para importar varios usuarios para una cuenta de cliente.](file-customer-users.md) 

2. Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.

3. Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.

4. Seleccione la pestaña Usuarios y licencias del cliente y, **a** continuación, **seleccione Cargar usuarios.**

5. En **Subir información de usuarios**, selecciona **Examinar**.

6. En el selector de archivos, selecciona el archivo de datos y, a continuación, selecciona **Abrir**.

7. Seleccione **Validar**.

    **Nota**: La mayoría de los errores de creación de cuentas se deben a problemas en los archivos de datos, lo que incluye la falta de información, unas direcciones de correo electrónico con formato incorrecto o duplicadas o un exceso de registros en el archivo.

8. Después de Centro de partners validar el archivo, seleccione la **ubicación geográfica** para los nuevos usuarios.
9. Seleccione **Guardar**.
10. Descargue la información de contraseña temporal de los usuarios.

    >[!IMPORTANT]
    > Asegúrese de descargar el archivo con las contraseñas temporales ahora, ya que no podrá hacerlo más adelante. Los nuevos usuarios deben iniciar sesión en su nueva cuenta con las contraseñas temporales correspondientes a sus nuevas cuentas.

11. A los nuevos usuarios se les asignan automáticamente permisos de **Puede usar licencias y servicios.** 

## <a name="next-steps"></a>Pasos siguientes

- [Conceder a los clientes permiso Centro de partners para comprar sus propios productos o servicios](give-customers-permission.md)
