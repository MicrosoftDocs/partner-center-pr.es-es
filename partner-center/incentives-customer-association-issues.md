---
title: Problemas de asociación de clientes
description: Obtenga información acerca de cómo solucionar los problemas que surgen al trabajar con las asociaciones de clientes de los asociados de registro (CPOR).
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: kim-davis
ms.author: kimnich
ms.localizationpriority: medium
ms.date: 06/29/2020
ms.openlocfilehash: cda0b9d29c351e5365a0ff291f66ee5e2fa91ae7
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949660"
---
# <a name="customer-association-issues"></a>Problemas de asociación de clientes

Se aplica a:

- Centro de partners

El contenido que aparece a continuación le ayudará a solucionar los problemas que pueden aparecer al trabajar con las asociaciones de clientes.

Roles adecuados:

- Administrador de facturación
- Administrador global
- Administrador de incentivos

## <a name="domain-tenant-mismatch"></a>Error de coincidencia de inquilino de dominio

En el flujo de notificaciones de asociación del socio de registro (CPOR), se le pedirá que proporcione el identificador y el subdominio del inquilino del cliente. Si recibe un error que indica que no coinciden, póngase en contacto con su cliente para asegurarse de que tiene los detalles correctos.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Errores de suscripción en el flujo de notificaciones de Asociación de CPOR

En el flujo de notificaciones de Asociación de CPOR, es posible que se le pida que proporcione una suscripción a un producto que está intentando reclamar a través de Business Applications (Dynamics 365). Solicitamos la suscripción, ya que estamos comprobando de forma dinámica que el producto y la suscripción pertenecen al inquilino que se va a solicitar. También estamos comprobando que la suscripción se encuentra en estado activo/en gracia.

Si recibe el error, podría deberse a varios motivos:

- El producto seleccionado no existe en el inquilino del cliente.
- La suscripción proporcionada no es para Dynamics
- La suscripción proporcionada es para CSP.
- El cliente todavía no ha activado o aprovisionado los productos para esa suscripción
- La suscripción ya se ha notificado.
- El identificador proporcionado no es un identificador de suscripción

Si tiene alguna pregunta sobre la precisión de su suscripción, trabaje con el cliente para asegurarse de que la suscripción es correcta y de que está usando el identificador de inquilino correcto.

Si esta ruta no ha resuelto el problema, póngase en contacto [con el servicio de soporte técnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="when-subscriptions-will-be-available-to-claim"></a>Cuándo estarán disponibles las suscripciones para la demanda

Al solicitar una suscripción, recibirá un error si aún no se ha aprovisionado la suscripción. Hay varios pasos que el cliente debe llevar a cabo para que la suscripción esté disponible para que la plataforma CPOR la seleccione y la ponga a disposición de la demanda. Si recibe un error al intentar reclamar una suscripción, póngase en contacto con su cliente para asegurarse de que se ha aprovisionado y de que la suscripción que va a notificar es correcta. Si ya ha tomado esta ruta, póngase en contacto [con el servicio de soporte técnico](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="which-activity-do-i-choose"></a>¿Qué actividad elijo?

La plataforma de reclamación de CPOR permite notificaciones de Asociación de CPOR relacionadas con Business Applications y Microsoft 365 áreas de la solución. A continuación se muestran las actividades que se aplican a cada área de solución. Seleccione la actividad correcta en función de las descripciones para evitar tener que reclamar en el futuro. La reivindicación de una actividad incorrecta puede dar lugar a pérdidas de elegibilidad y beneficios.


| Área de solución | Actividad | Aplicable para |
| ------ | ----------- | ----------- |
| Aplicaciones empresariales      | Soporte preventa   | Seleccione si influye en su compra de un producto válido y desea solicitar los incentivos de preventa. Esta opción solo es aplicable si el cliente compró estos productos a través del contrato de licencias por volumen o de web-Direct. |
|    |  Uso  | Seleccione esta información si desea impulsar la adopción y el uso de una carga de trabajo válida y desea aplicar los incentivos de uso. Esta opción solo es aplicable si el cliente compró estos productos a través del contrato de licencias por volumen o de web-Direct. |
|    | Asociación de ingresos   | Seleccione esta opción si influye en la selección de un producto válido como Influenciante empresarial. Esta opción es solo para la Asociación de ingresos, no para los pagos por incentivos. Esta opción solo es aplicable si el cliente compró estos productos a través del contrato de licencias por volumen o de web-Direct.   |
| Microsoft 365   | Uso   | Seleccione esta información si desea impulsar la adopción y el uso de una carga de trabajo válida y desea aplicar los incentivos de uso. |

## <a name="which-mpn-do-i-choose"></a>¿Qué MPN elegir?

En el flujo de notificaciones de Asociación de CPOR, se le pedirá que elija un MPN de empresa que se debe asociar al trabajo que está reclamando en el cliente final. Su empresa puede tener muchos MPNs, algunos de los cuales pueden inscribirse en programas de incentivos y otros asociados a un tipo de socio comercial como FRP FastTrack. El flujo de notificaciones de Asociación de CPOR identificará qué MPNs está inscrito en un programa de incentivos, pero no le indicará si es un tipo de asociado específico MPN. Es importante seleccionar el MPN correcto para evitar tener que reclamar en el futuro. La reivindicación de un MPN incorrecto puede dar lugar a una falta de elegibilidad y a una ganancia de incentivos.

Si no sabe qué MPN usar, póngase en contacto con el administrador global.

Si el MPN que quiere usar no está inscrito, puede administrarlo en la [pestaña Información general sobre incentivos](https://partner.microsoft.com/dashboard/incentives/enrollment/summary).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Elección de un producto frente a la entrada de una suscripción

Cuando se reclama y aprueba un producto de Dynamics, el asociado puede ver el identificador de la suscripción en la propia declaración de Asociación de CPOR. Cuando se solicita esta suscripción, está en estado activo o en período de gracia, pero puede haber una hora en la que la suscripción finaliza y las nuevas suscripciones se deben solicitar en una declaración de asociación CPOR independiente.

## <a name="competing-claims"></a>Notificaciones competitivas

Si va a crear una notificaciones de Asociación de CPOR para un cliente y sus productos que ya están asociados a otro asociado, su demanda pasará por el arbitraje:

1. Después de crear una nueva asociación de cliente, Microsoft comprobará los detalles de la asociación y la prueba de ejecución que se proporcionan para garantizar su precisión.

2. Si usted y otro socio reclaman al mismo cliente y producto o carga de trabajo, Microsoft revisará la documentación de prueba de ejecución de cada asociado para determinar qué socio comercial debe aprobar.

3. Es posible que se solicite información adicional a ambos asociados, lo que podría provocar retrasos en el procesamiento de la solicitud de asociación.

4. La demanda de la Asociación CPOR se seguirá revisando en un plazo de cinco días laborables, aunque su estado puede permanecer como _en revisión_ durante un período de tiempo más largo. Este escenario puede ocurrir cuando Microsoft trabaja con el asociado que posee actualmente el producto o la carga de trabajo. Si es así, se le notificará en la sección de comentarios de la notificación. 

>[!IMPORTANT]
>Si necesitamos información adicional para comprobar la Asociación de CPOR, nos pondremos en contacto con usted a través de la sección de comentarios de notificaciones de CPOR Association.
