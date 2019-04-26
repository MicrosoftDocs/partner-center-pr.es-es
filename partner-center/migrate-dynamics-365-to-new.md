---
title: Migración de Dynamics 365 Business Edition ofrece a las versiones más recientes | Centro de partners
ms.topic: article
ms.date: 12/12/2018
description: Ya no se pueden renovar las suscripciones de Dynamics 365 Business Edition.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
Keywords: Las ofertas de Dynamics 365, renovar las ofertas, nuevas SKU de Dynamics 365
ms.openlocfilehash: ca1823c4055e2d89edc5c49e900a1c255a94f59a
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134375"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrar ofertas de Dynamics 365 Business Edition a versiones más recientes 

**Se aplica a**

- Centro de partners

Efectivo el 1 de enero de 2019, los clientes con suscripciones de Dynamics 365 Business Edition ya no se pueden renovar en estas ofertas heredadas; las suscripciones existentes no se renovarán automáticamente cuando expiran. En la página de detalles de la suscripción, el estado de la suscripción cambiará a "Expira el [fecha]" de "Renueva automáticamente el [fecha]".

Para garantizar la continuidad de los clientes, debe realizar la transición aquellos con las suscripciones que van a expirar a una opción admitida, que se enumeran a continuación. Te recomendamos mover los clientes a las nuevas suscripciones antes de la fecha de finalización para evitar interrupciones en el servicio a los clientes.

Si usa la API (CREST o centro de partners), puede encontrar la renovación de suscripciones caducadas mediante la evaluación de la fecha de finalización de la suscripción, junto con el auto = False property. Las suscripciones en cuestión se establecerá en auto renovar = False, 1 de enero de 2019. Puedes mover a los clientes a un plan nuevo en cualquier momento. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>Las ediciones de Dynamics 365 Business va a retirar

- Dynamics 365 para Finance and Operations, edición Business
- Dynamics 365 for Team Members, edición Business

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Business Dynamics. UU.-las ofertas nuevo de Dynamics 365 Business Edition

Con las nuevas ofertas de Dynamics Business Central, los clientes pueden conectar sus finanzas, ventas, servicio y operaciones para optimizar los procesos empresariales, mejorar las interacciones del cliente y tomar mejores decisiones. Dynamics 365 Business Central está disponible a través solo asociados del programa proveedor de soluciones en la nube (CSP) y basado en la nube.
Dynamics 365 clientes Business Edition tienen derecho a recibir precios con descuento de transición para el nuevo Business Central ofrece hasta el 30 de junio de 2020.

## <a name="transition-customers-to-new-product-plans"></a>Clientes de transición hacia los nuevos planes de productos

 Mover a los clientes de SKU retiradas a los más recientes requiere los pasos siguientes en este orden:

- Comprar la nueva suscripción
- Reasignar licencias de usuario actuales
- Cancelar suscripción antigua

## <a name="purchase-the-new-plan-for-your-customer"></a>El nuevo plan de compra para su cliente

1. Seleccione **clientes** desde el panel de navegación izquierdo y, a continuación, seleccione el cliente que desea mover a la nueva suscripción.
2. Seleccione **Agregar suscripción**.
3. Selecciona la suscripción que quieras adquirir del catálogo (en este caso, una de las opciones que se indican más arriba), escribe el número de licencias y, a continuación, **Enviar**. 

El cliente tendrá ahora la suscripción antigua y una nueva. El siguiente paso es volver a asignar licencias a los usuarios del cliente.

1. Seleccione **clientes** desde el panel de navegación izquierdo y, a continuación, seleccione el cliente que está moviendo.
2. Selecciona **Usuarios y licencias**.
3. Para reasignar una licencia a un usuario, seleccione el usuario y, a continuación, seleccione **administrar licencias**. 
4. En el **administrar licencias** página, desactive el Dynamics 365 para Sales / Plan de compromiso del cliente de Basic (oferta completo) casilla de verificación de licencia y seleccione un nuevo plan de servicio para la suscripción que el cliente se mueve a. 
5. Selecciona **Enviar**. Hará esto para cada usuario que necesita la nueva licencia. 

Una vez que haya movido las licencias a través a la nueva suscripción puede cancelar la suscripción antigua. 

1. Seleccione **clientes** desde el panel de navegación izquierdo y, a continuación, seleccione el cliente que está moviendo.
2. En la página de detalles de suscripción, establezca la suscripción antigua **Suspended** y seleccione **enviar**.

Ahora se suspende la suscripción antigua y la nueva suscripción está activa. Se cancelará el aprovisionamiento de la suscripción suspendida automáticamente después de 120 días. Su cliente no incurrirá en ningún costo adicional para la suscripción antigua.