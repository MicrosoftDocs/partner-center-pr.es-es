---
title: 'Elegibilidad de transferencia: directrices para transferir una suscripción entre cuentas de facturación, Azure Marketplace'
description: Directrices para comprobaciones comerciales antes de transferir una suscripción entre cuentas de facturación en el Azure Portal.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 3a2415ab9833d5c574ad76d462f526a131c24f33
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/12/2021
ms.locfileid: "103412563"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Transferir la idoneidad para una suscripción entre cuentas de facturación

Puede [transferir una suscripción](/azure/cost-management-billing/understand/subscription-transfer) de una cuenta de facturación a otra en la sección facturación de la Azure portal. Antes de una transferencia, la suscripción se examina para los productos de terceros. La transferencia se permite solo si se borran *todos* los productos para su transferencia (consulte los [criterios](#criteria-for-transfer-approval-or-denial) siguientes). El sistema generará mensajes de error relevantes para las aplicaciones que no se han podido borrar para ayudarle a determinar los pasos siguientes.

> [!NOTE]
> Este artículo no se aplica a las ofertas de SaaS porque los recursos de SaaS se adjuntan a un inquilino, no a una suscripción. Los recursos de SaaS se pueden transferir desde una cuenta de facturación a otra, pero esto se hace por recurso y por el soporte técnico de Azure como solicitud de soporte técnico.

## <a name="criteria-for-transfer-approval-or-denial"></a>Criterios de aprobación o denegación de transferencia

No se puede transferir una suscripción si cualquiera de sus aplicaciones de terceros cumple alguno de los siguientes criterios:

- La cuenta de destino es comercial y la aplicación deja de participar a través de asociados.
- La aplicación es participación para los asociados seleccionados y la cuenta de destino no se encuentra en la lista de permitidos.
- La oferta era una oferta de vista previa en el pasado para las suscripciones seleccionadas o era una oferta privada y la suscripción ya no se encuentra en la lista de permitidos.
- La nueva cuenta de facturación está en una región diferente de donde se vende la oferta y la oferta no se vende en esa región.

Una transferencia bloqueada permanece en vigor hasta que se quita el recurso de la suscripción, tras lo cual se puede volver a intentar la transferencia.

## <a name="next-steps"></a>Pasos siguientes

[Obtener soporte técnico para Microsoft AppSource y Azure Marketplace](get-support.md)

