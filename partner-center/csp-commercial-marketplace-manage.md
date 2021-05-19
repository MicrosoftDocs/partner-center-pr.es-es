---
title: Administración de productos de Marketplace & ofertas
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Con Centro de partners, obtenga información sobre cómo los proveedores de soluciones en la nube pueden administrar las ofertas de ISV de terceros adquiridas para los clientes del marketplace comercial.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e1bb2752dad5325478496c83fc368943780d8afb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147911"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Administración de productos y ofertas de Marketplace comercial para sus clientes


**Roles adecuados:** administrador global | Agente de administración

Los asociados del programa Proveedor de soluciones en la nube (CSP) pueden usar el portal de Centro de partners para comprar muchas ofertas o suscripciones de SaaS de ISV para sus clientes desde el marketplace comercial. Una vez comprada una oferta, tiene varias maneras de administrarla.

## <a name="view-or-edit-a-subscription"></a>Visualización o edición de una suscripción

Después de comprar una suscripción a un publicador de ISV de terceros, puede revisarla o editarla como se muestra a continuación:

1. Inicie sesión en el panel Centro de partners [y,](https://partner.microsoft.com/dashboard)a continuación, **seleccione Clientes** en el menú de navegación izquierdo.

2. Seleccione un cliente adecuado y, a continuación, **seleccione Suscripciones.** Aquí se enumeran las suscripciones basadas en licencias que ha adquirido para el cliente.

3. En la **columna** Suscripción, seleccione la suscripción que desea ver o editar. Esto proporciona más información para configurar o aprovisionar la oferta. (Si se necesita más acción en la oferta, es posible que también vea un estado "Acción necesaria" en la columna Estado. Esto también puede ir acompañado de un vínculo al sitio del publicador del ISV).

4. Una vez que seleccione la suscripción que desea ver o editar, la página de detalles de la suscripción le permite editar la suscripción y hacer cosas como:

    - Cambio del alias de la suscripción

    - Agregar o disminuir el número de licencias de la suscripción

    - Cancelación de la suscripción

    - Desactivar la renovación automática

    - Agregue un identificador de MPN de revendedor indirecto, si procede.

> [!NOTE]
> Es posible que tenga que completar determinados pasos definidos por el publicador de ISV para poder realizar algunos cambios en una suscripción, como cancelar una suscripción.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Asignación de licencias y activación de una suscripción en nombre de un cliente

Cuando adquiere una oferta de software como servicio (SaaS) proporcionada por un publicador de fabricante de software independiente (ISV) en el marketplace comercial, el publicador de ISV ayuda a administrar el proceso de asignación de licencias y activación de la suscripción en nombre del cliente.

El publicador debe proporcionarle un vínculo personalizado y un código de autorización que identifique su compra específica.

1. Puede encontrar este vínculo personalizado en el publicador de ISV de varias maneras:

   - Puede ver el vínculo en la página de confirmación que aparece después de comprar una oferta de SaaS de ISV. Para encontrar este vínculo en la página, busque y seleccione **Ir al sitio del publicador.**

   - Puede ver el vínculo desde la página Suscripciones del cliente específico. Este vínculo del publicador aparece en la fila asociada a la oferta o suscripción de ISV adquirida para el cliente.

   - Puede recuperar [el vínculo mediante Centro de partners API](/partner-center/develop/get-activation-link-by-order-line-item).

   > [!NOTE]
   > Para ello en nombre del cliente, es posible que tenga que copiar el vínculo personalizado, pegarlo en un explorador privado y escribir las credenciales del cliente.

2. Una vez que esté en el sitio o sistema del publicador del ISV, el publicador le permitirá conocer los pasos adicionales que debe seguir para completar el proceso de instalación del cliente y aprovisionar o asignar licencias.

3. Como asociado del programa CSP que trabaja en nombre del cliente, usted es responsable de realizar las siguientes tareas:

    - Envíe la información necesaria al publicador.

    - Envíe cualquier dirección URL necesaria directamente al cliente (o comunique directamente los detalles sobre esta suscripción al cliente)

4. Una vez que proporcione la información necesaria al publicador, el publicador aprovisionará y asignará las licencias adecuadas. La facturación de la suscripción se iniciará solo después de que se produzcan los siguientes eventos:

    - El publicador de ISV ha asignado correctamente las licencias adecuadas

    - El publicador de ISV ha confirmado a Microsoft (a través de una API de suministro de SaaS independiente) que la configuración de la cuenta se ha completado correctamente.

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Cancelación de una suscripción de SaaS basada en licencia de un publicador de ISV

Al suscribirse a un producto SaaS basado en licencias ofrecido por un publicador de ISV dentro del marketplace comercial, tiene la opción de cancelar la suscripción dentro de su período de cancelación designado. Este período de cancelación cambia en función de si tiene una suscripción mensual o anual. También puedes elegir si deseas renovar la suscripción automáticamente o no.

Para obtener más información sobre los períodos de cancelación que se aplican, cómo cancelar o cómo renovar automáticamente una suscripción, consulte:

- [Cancelación de una suscripción](create-a-new-subscription.md#cancel-a-subscription)

- [Renovación automática de una suscripción de Marketplace comercial](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Adición o eliminación de licencias para una suscripción de SaaS

En el caso de las ofertas de Marketplace comercial de SaaS, puede agregar o quitar licencias de usuario para una suscripción de cliente.

1. Inicie sesión en el panel Centro de partners [y,](https://partner.microsoft.com/dashboard)a continuación, **seleccione Clientes** en el menú de navegación izquierdo.

2. Seleccione un cliente adecuado y, a continuación, **seleccione Suscripciones.** Aquí se enumeran las suscripciones basadas en licencias que ha adquirido para el cliente.

3. En la **columna** Suscripción, seleccione la suscripción que desea modificar.

4. En la página de detalles de la suscripción, busque **el campo Cantidad.** Aquí es donde puede aumentar o disminuir el número de licencias.

5. Cambie la cantidad y, a continuación, **seleccione Enviar**.

## <a name="manage-subscriptions-using-partner-center-apis"></a>Administración de suscripciones mediante las API del Centro de partners

También puede usar las API Centro de partners para realizar la administración del ciclo de vida y administrar las facturas de las suscripciones. Para más información, consulte [Creación de una suscripción para productos de Marketplace comercial.](/partner-center/develop/create-subscription-azure-marketplace-products)

## <a name="next-steps"></a>Pasos siguientes

- [Compra de ofertas de Marketplace comercial](csp-commercial-marketplace-purchase.md)
- [Más información sobre la facturación en marketplace comercial](csp-commercial-marketplace-billing.md)