---
title: Problemas de asociación de clientes a incentivos
description: Obtenga información sobre cómo solucionar los problemas que se pueden encontrar al trabajar con asociaciones de clientes de asociados de registro reclamados (CPOR).
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.date: 09/11/2020
ms.openlocfilehash: 8f1c087911e6dd7e58182c99e2b97b7a6b2246d8
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110152178"
---
# <a name="issues-with-claimed-partner-of-record-cpor-customer-associations"></a>Problemas con las asociaciones de clientes de asociados de registro reclamados (CPOR)

**Roles adecuados:** Administrador de facturación | Administrador global | Administrador de incentivos

El contenido siguiente le ayudará a resolver los problemas que pueden llegar al trabajar con asociaciones de clientes.

## <a name="domain-tenant-mismatch"></a>Error de coincidencia entre dominio y inquilino

En el flujo de notificación de asociación del asociado de registro reclamado (CPOR), se le pedirá que proporcione el identificador de inquilino y el subdominio del cliente. Si recibe un error que indica que no coinciden, póngase en contacto con el cliente para asegurarse de que tiene los detalles correctos.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Errores de suscripción en el flujo de notificación de asociación de CPOR

En el flujo de notificación de asociación de CPOR, es posible que se le pida que proporcione una suscripción para un producto que está intentando reclamar a través de Business Applications (Dynamics 365). Solicitamos la suscripción porque estamos comprobando dinámicamente que el producto y la suscripción pertenecen al inquilino para el que se está reclamando. También estamos comprobando que la suscripción está activa o en estado de gracia.

Si recibe el error, podría deberse a varias razones:

- El producto seleccionado no existe en el inquilino del cliente.
- La suscripción proporcionada no es para Dynamics
- La suscripción proporcionada es para CSP.
- El cliente aún no ha activado ni aprovisionado los productos para esa suscripción.
- La suscripción ya se ha notificado.
- El identificador proporcionado no es un identificador de suscripción

Si tiene alguna pregunta sobre la precisión de la suscripción, trabaje con el cliente para asegurarse de que la suscripción es correcta y de que usa el identificador de inquilino correcto.

Si esta ruta no ha resuelto el problema, póngase en contacto con el [soporte técnico.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="when-subscriptions-will-be-available-to-claim"></a>Cuándo estarán disponibles las suscripciones para la notificación

Al reclamar una suscripción, recibirá un error si la suscripción aún no se ha aprovisionado. Hay varios pasos que el cliente debe seguir para que la suscripción esté disponible para que la plataforma CPOR la reclame y que esté disponible para la reclamación. Si recibe un error al intentar reclamar una suscripción, póngase en contacto con el cliente para asegurarse de que se ha aprovisionado y de que la suscripción que está reclamando es correcta. Si ya ha realizado esta ruta, póngase en contacto con el [soporte técnico.](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives)

## <a name="which-activity-do-i-choose"></a>¿Qué actividad se elige?

La plataforma de reclamación de CPOR permite notificaciones de asociación de CPOR relacionadas con Business Applications y Microsoft 365 de soluciones. A continuación se muestran las actividades que son aplicables a cada área de solución. Seleccione la actividad correcta en función de las descripciones para evitar tener que reclamar en el futuro. Reclamar con una actividad incorrecta puede dar lugar a la falta de elegibilidad y las ganancias de incentivos.


| Área de solución | Actividad | Aplicable a |
| ------ | ----------- | ----------- |
| Aplicaciones empresariales      | Preventa   | Seleccione si influyó en la compra de un producto apto y desea solicitar incentivos de venta previa. Esta opción solo es aplicable si el cliente compró estos productos mediante el contrato de licencia por volumen o Web-Direct. |
|    |  Uso  | Seleccione si impulsa su adopción y uso de una carga de trabajo apta y quiere solicitar incentivos de uso. Esta opción solo es aplicable si el cliente compró estos productos mediante el contrato de licencia por volumen o Web-Direct. |
|    | Asociación de ingresos   | Seleccione si ha influenciado su selección de un producto apto como influenciador empresarial. Esta opción es solo para la asociación de ingresos, no para los pagos de incentivos. Esta opción solo es aplicable si el cliente compró estos productos mediante el contrato de licencia por volumen o Web-Direct.   |
| Microsoft 365   | Uso   | Seleccione si impulsa su adopción y uso de una carga de trabajo apta y quiere solicitar incentivos de uso. |

## <a name="which-mpn-do-i-choose"></a>¿Qué MPN se elige?

En el flujo de notificación de asociación de CPOR, se le pedirá que elija un MPN de empresa que se debe asociar al trabajo que está reclamando al cliente final. Su empresa puede tener muchos MPN, algunos de los cuales pueden estar inscritos en programas de incentivos y otros asociados a un tipo de asociado, como FRP FastTrack. El flujo de notificación de asociación de CPOR identificará qué MPN están inscritos en un programa de incentivos, pero no le mostrará si es un MPN de tipo asociado específico. Es importante seleccionar el MPN correcto para evitar tener que reclamar en el futuro. La reclamación con un MPN incorrecto puede dar lugar a la falta de elegibilidad y las ganancias de incentivos.

Si no sabe qué MPN usar, póngase en contacto con el administrador global.

Si el MPN que quiere usar no está inscrito, puede administrarlo en la pestaña Información general de [incentivos](https://partner.microsoft.com/dashboard/incentives/enrollment/summary) (se requiere inicio de sesión).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Elección de un producto frente a la especificación de una suscripción

Cuando se reclama y aprueba un producto de Dynamics, el asociado puede ver el identificador de suscripción en la propia notificación de asociación de CPOR. Cuando se reclama esta suscripción, está activa o en estado de gracia, pero puede que haya un momento en el que la suscripción finalice y las nuevas suscripciones deban reclamarse en una notificación de asociación de CPOR independiente.

## <a name="competing-claims"></a>Notificaciones de la competencia

Si va a crear una reclamación de asociación de CPOR para un cliente y sus productos que ya están asociados a otro asociado, su reclamación pasará por el procedimiento de conciliación:

1. Después de crear una nueva asociación de cliente, Microsoft comprobará los detalles de la asociación y la prueba de ejecución que se proporcionan para garantizar su precisión.

2. Si usted y otro asociado reclaman el mismo cliente y producto o carga de trabajo, Microsoft revisará la documentación de prueba de ejecución de cada asociado para determinar qué asociado aprobar.

3. Es posible que se solicite información adicional a ambos asociados, lo que podría provocar retrasos en el procesamiento de la solicitud de asociación.

4. La notificación de asociación de CPOR se seguirá revisando  en un plazo de cinco días laborables, aunque su estado puede permanecer en Revisión durante un período de tiempo más largo. Este escenario puede ocurrir cuando Microsoft trabaja con el asociado que posee actualmente el producto o la carga de trabajo. Si es así, se le notificará en la sección de comentarios de la notificación. 

>[!IMPORTANT]
>Si necesitamos información adicional para comprobar la prueba de ejecución (PoE) de la asociación de CPOR, nos comunicaremos con usted a través de la sección de comentarios de notificación de asociación de CPOR.

## <a name="next-steps"></a>Pasos siguientes

- [Introducción a los incentivos](incentives-get-started-intro.md)
