---
title: Administrar sus clientes
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Los registros de clientes se encuentran entre los recursos de información más importantes. Obtenga información sobre cómo ver, buscar, actualizar, & exportar información en la Centro de partners de clientes.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6e73aa98e0cfaf82521a5fe63e34ebf0b44363fb
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854509"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Administración de la lista de clientes: buscar, actualizar o exportar clientes en Centro de partners

**Se aplica a**: Centro de partners | Centro de partners para Microsoft Cloud for US Government

**Roles adecuados:** agente de administración | Administrador global

Los registros de cliente son unos de los recursos de información más importantes del Centro de partners. Puedes buscar en la base de datos de cuentas de cliente, exportar la base de datos de clientes completa o un subconjunto a un formato de archivo de valores separados por comas (.csv) compatible con Excel. También puedes exportar información de las suscripciones de un cliente a un archivo .csv.

Los registros de actividad también proporcionan datos exportables sobre transacciones y acciones de administración para los clientes. Para obtener más información, consulta [Ver los registros de actividades de los cliente](activity-logs.md).

## <a name="search-for-a-customer"></a>Buscar un cliente

1. En el **menú Centro de partners,** seleccione **Clientes.**
2. Para buscar un cliente, escriba el nombre del cliente o el nombre de dominio en el cuadro de búsqueda.
3. Selecciona la **flecha abajo** al final de una fila de cliente para ver el id. de Microsoft del cliente y los vínculos rápidos de suscripciones y servicios asociados.

## <a name="update-a-customers-company-name"></a>Actualizar el nombre de empresa de un cliente

En el **menú Centro de partners,** seleccione **Clientes.**
2. Para buscar un cliente, escriba el nombre del cliente o el nombre de dominio en el cuadro de búsqueda.
3. Selecciona la **flecha abajo** al final de una fila de cliente para ver el id. de Microsoft del cliente y los vínculos rápidos de suscripciones y servicios asociados.
4. En la información de **facturación del** cliente, actualice el nombre de la empresa. Al guardar el nuevo valor, se reflejará en la lista de clientes. Esta acción solo cambiará el nombre de la empresa de facturación y el valor de la lista de clientes. No se reflejará en ningún otro sitio.

## <a name="export-your-customer-list"></a>Exportar la lista de clientes

1. En el **menú Centro de partners,** seleccione **Clientes.**
2. Selecciona **Exportar clientes**.

   El Centro de partners convierte la lista de clientes completa en un archivo .csv y lo carga en la carpeta de descarga predeterminada de tu equipo. También puedes exportar subconjuntos de datos de clientes. Las columnas de datos incluyen lo siguiente:

   - **Identificador de Microsoft**;
   - **Nombre de la empresa**;
   - **Nombre de dominio principal**;
   - **Relación**: relación comercial del partner con cada cliente de la lista.

    De manera predeterminada, el Centro de partners exporta la lista de clientes completa, independientemente de longitud. También puedes buscar en la lista de cliente por nombre de la empresa o dominio y exportar ese subconjunto de datos.

3. Si es un proveedor indirecto, puede filtrar la lista de clientes por revendedor indirecto. Seleccione **Filtrar por revendedor indirecto** en la lista y, a continuación, elija un revendedor.


## <a name="export-customer-subscription-information"></a>Exportación de información de suscripción de cliente

1. En el **menú Centro de partners,** seleccione **Clientes.**

2. Selecciona el **Nombre de la empresa** para cualquier cliente. Se abrirá la página **Suscripciones** del cliente y se mostrará la lista completa de suscripciones de producto.

3. Selecciona **Exportar suscripciones**. El Centro de partners convierte los datos de suscripción del cliente en un archivo .csv y lo carga en la carpeta de descarga predeterminada de tu equipo. Las columnas de datos incluyen lo siguiente:
   - **Id. de suscripción**;
   - **Suscripción**: el nombre de producto para la suscripción;
   - **Cantidad**: número de licencias compradas;
   - **Status**;
   - **Revendedor**: el identificador del revendedor que posee y administra la suscripción.

> [!NOTE]  
> Para obtener más información sobre la administración de suscripciones, vea [Suscripciones de cliente.](customer-subscriptions.md)
