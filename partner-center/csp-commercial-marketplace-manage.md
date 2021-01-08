---
title: Administrar productos de Marketplace & ofertas
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Con el centro de Partners, obtenga información sobre cómo los proveedores de soluciones en la nube pueden administrar ofertas de ISV de terceros compradas para clientes del Marketplace comercial.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5e6ca188aeb50cec6f847afb08be4a9d62b36984
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979683"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Administrar productos y ofertas comerciales de Marketplace para sus clientes


**Roles adecuados**

- Administrador global
- Agente de administrador

Los asociados del programa proveedor de soluciones en la nube (CSP) pueden usar el portal del centro de partners para comprar muchas ofertas o suscripciones de SaaS de ISV para sus clientes del Marketplace comercial. Una vez que compre una oferta, tendrá varias maneras de administrarla.

## <a name="view-or-edit-a-subscription"></a>Ver o editar una suscripción

Después de comprar una suscripción de un publicador de ISV de terceros, puede revisarla o editarla de la siguiente manera:

1. Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard)del centro de Partners y seleccione **customers (clientes** ) en el menú de navegación izquierdo.

2. Seleccione un cliente adecuado y, a continuación, seleccione **suscripciones**. Aquí se enumeran las suscripciones basadas en licencias que ha adquirido para el cliente.

3. En la columna **suscripción** , seleccione la suscripción que desea ver o editar. Esto le proporciona más información para configurar o aprovisionar la oferta. (Si se necesita más acción en la oferta, también puede ver el estado "acción necesaria" en la columna Estado. También puede ir acompañado de un vínculo al sitio del anunciante de ISV).

4. Una vez que seleccione la suscripción que desea ver o editar, la página de detalles de la suscripción le permite editar la suscripción y hacer cosas como:

    - Cambiar el alias de la suscripción

    - Agregar o disminuir el número de licencias de la suscripción

    - Cancelación de la suscripción

    - Desactivar la renovación automática

    - Agregar un ID. de revendedor de MPN indirecto, si procede

> [!NOTE]
> Es posible que tenga que completar determinados pasos definidos por el publicador de ISV para poder realizar algunos cambios en una suscripción, como cancelar una suscripción.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Asignar licencias y activar una suscripción en nombre de un cliente

Cuando se adquiere una oferta de software como servicio (SaaS) proporcionada por un publicador de proveedor de software independiente (ISV) en el Marketplace comercial, el publicador de ISV ayuda a administrar el proceso de asignación de licencias y la activación de la suscripción en nombre del cliente.

El publicador debe proporcionarle un vínculo personalizado y un código de autorización que identifique su compra específica.

1. Puede encontrar este vínculo personalizado en el publicador de ISV de varias maneras:

   - Puede ver el vínculo de la página de confirmación que aparece después de comprar una oferta de SaaS de ISV. Para encontrar este vínculo en la página, busque y seleccione **ir al sitio del editor**.

   - Puede ver el vínculo desde la página suscripciones del cliente específico. Este vínculo de publicador aparece en la fila asociada a la oferta de ISV o a la suscripción adquirida para el cliente.

   - Puede [recuperar el vínculo mediante las API del centro de Partners](/partner-center/develop/get-activation-link-by-order-line-item).

   > [!NOTE]
   > Para ello en nombre del cliente, es posible que tenga que copiar el vínculo personalizado, pegarlo en un explorador privado y especificar las credenciales del cliente.

2. Una vez que se encuentre en el sitio o el sistema del publicador de ISV, el publicador le informará de los pasos adicionales que debe seguir para completar el proceso de configuración del cliente y aprovisionar o asignar licencias.

3. Como asociado en el programa CSP que trabaja en nombre de su cliente, usted es responsable de realizar las siguientes tareas:

    - Envíe cualquier información necesaria al publicador.

    - Envíe cualquier dirección URL necesaria directamente a su cliente (o comunique directamente los detalles sobre esta suscripción a su cliente)

4. Una vez que proporcione la información necesaria al publicador, el publicador aprovisionará y asignará las licencias adecuadas. La facturación de la suscripción se iniciará solo después de que se produzcan los siguientes eventos:

    - El publicador de ISV ha asignado correctamente las licencias adecuadas

    - El publicador de ISV ha confirmado a Microsoft (a través de una API de cumplimiento de SaaS independiente) que la configuración de la cuenta se ha completado correctamente.

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Cancelar una suscripción de SaaS basada en licencia de un publicador de ISV

Al suscribirse a un producto SaaS basado en licencia ofrecido por un publicador de ISV en el Marketplace comercial, tiene la opción de cancelar la suscripción dentro del período de cancelación designado. Este período de cancelación cambia en función de si tiene una suscripción mensual o anual. También puedes elegir si deseas renovar la suscripción automáticamente o no.

Para obtener más información sobre los períodos de cancelación que se aplican, cómo cancelar o cómo renovar automáticamente una suscripción, consulte:

- [Cancelación de una suscripción](create-a-new-subscription.md#cancel-a-subscription)

- [Renovación automática de una suscripción de Marketplace comercial](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Adición o eliminación de licencias para una suscripción de SaaS

En el caso de las ofertas de Marketplace comercial de SaaS, puede Agregar o quitar licencias de usuario para una suscripción de cliente.

1. Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard)del centro de Partners y seleccione **customers (clientes** ) en el menú de navegación izquierdo.

2. Seleccione un cliente adecuado y, a continuación, seleccione **suscripciones**. Aquí se enumeran las suscripciones basadas en licencias que ha adquirido para el cliente.

3. En la columna **suscripción** , seleccione la suscripción que desea modificar.

4. En la página Detalles de la suscripción, busque el campo **cantidad** . Aquí es donde puede aumentar o disminuir el número de licencias.

5. Cambie la cantidad y, a continuación, seleccione **submit (enviar**).

## <a name="manage-subscriptions-using-partner-center-apis"></a>Administración de suscripciones mediante las API del Centro de partners

También puede usar las API del centro de partners para realizar la administración del ciclo de vida y administrar las facturas de las suscripciones. Para obtener más información, consulte [crear una suscripción para productos de Marketplace comerciales](/partner-center/develop/create-subscription-azure-marketplace-products).

## <a name="next-steps"></a>Pasos siguientes

- [Comprar ofertas comerciales de Marketplace](csp-commercial-marketplace-purchase.md)
- [Más información sobre la facturación en el Marketplace comercial](csp-commercial-marketplace-billing.md)