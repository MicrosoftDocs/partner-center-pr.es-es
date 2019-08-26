---
title: Confirmación de la aceptación por parte del cliente del Contrato de cliente de Microsoft | Centro de partners
ms.topic: article
ms.date: 04/16/2019
Description: Como partner, debes obtener la aceptación por parte de tu cliente del Contrato de cliente de Microsoft antes de pedir productos y servicios de Microsoft para dicho cliente. Para ayudar mejor a los partners a cumplir con los requisitos de cumplimiento, Microsoft les pide que confirmen la aceptación proporcionando ciertos detalles de la persona que ha aceptado el contrato.
author: LauraBrenner
ms.author: labrenne
keywords: customer, customers, consent, MCA, Microsoft Cloud Agreement, Microsoft Customer Agreement, customer agreement templates
ms.localizationpriority: medium
ms.openlocfilehash: 295c997baa43dd087552315d71d726a0f28c6ed1
ms.sourcegitcommit: 0712e68734f0b3e53821b490a6c32a6c991a6e49
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 08/21/2019
ms.locfileid: "69871771"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-preview"></a>Confirmación de la aceptación por parte del cliente del Contrato de cliente de Microsoft (versión preliminar)

Actualmente, para que un partner de CSP pueda realizar un pedido en nombre de un cliente, el cliente debe aceptar y firmar el **Contrato de Microsoft Cloud** aplicable. A continuación, el partner debe confirmar su aceptación proporcionando información sobre el firmante a Microsoft. Si un cliente no confirma su aceptación del Contrato de Microsoft Cloud:
- No podrás crear nuevos pedidos para este cliente.
- No podrás cambiar el número de puestos de las suscripciones basadas en puestos existentes para este cliente.

Para obtener más información sobre cómo confirmar la aceptación de un cliente del Contrato de Microsoft Cloud mediante la API o el panel del Centro de partners, consulta [Confirm customer acceptance of the Microsoft Cloud Agreement](confirm-consent.md) (Confirmar la aceptación del Contrato de Microsoft Cloud por parte del cliente).

El 1 de octubre de 2019, Microsoft introducirá el **Contrato de cliente de Microsoft** en el programa CSP para reemplazar el Contrato de Microsoft Cloud. Para facilitar la migración de los partners al nuevo contrato, se admitirá el Contrato de Microsoft Cloud actual en el programa CSP hasta el 31 de enero de 2019. Para obtener más detalles sobre la línea de tiempo, consulta la tabla siguiente:

| Fecha | Hito | Detalles |
|------------|------------|--------------------------------|
|01 de agosto de 2019|Versión preliminar de la experiencia del usuario disponible en el espacio aislado|Los partners pueden confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft desde el panel del Centro de partners del entorno del espacio aislado de CSP. Los partners con acceso al entorno de espacio aislado de CSP pueden acceder a una versión preliminar de los cambios en la experiencia del usuario. Los partners sin acceso al espacio aislado pueden obtener información sobre los cambios en este tema.|
|02 de septiembre de 2019|Hay una versión preliminar de la API disponible en el espacio aislado.|El partner puede confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft desde la API del Centro de partners del entorno del espacio aislado de CSP. Los partners de la API pueden usar esta oportunidad para acceder a una versión preliminar de los cambios de la API y comenzar a trabajar en la integración de la API para admitir el nuevo contrato.|
|01 de octubre de 2019|Contrato de cliente de Microsoft disponible en el entorno de producción|Microsoft introducirá el Contrato de cliente de Microsoft en el programa CSP para reemplazar el Contrato de Microsoft Cloud. Los partners pueden confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft desde la API y el panel del Centro de partners en el entorno de producción. El Contrato de Microsoft Cloud sigue siendo compatible con el programa de partners de CSP. Sin embargo, es recomendable que los partners inicien la migración al Contrato de cliente de Microsoft. Las nuevas compras y los cambios en el recuento de puestos de las suscripciones existentes requerirán la confirmación por parte del partner del Contrato de cliente de Microsoft o del Contrato de Microsoft Cloud. Ciertas ofertas nuevas (por ejemplo, el nuevo plan de Azure) requerirán la confirmación del Contrato de cliente de Microsoft.|
|31 de enero de 2019|El Contrato de Microsoft Cloud se quitó de la producción|El Contrato de Microsoft Cloud ya no se acepta en el programa para partners de CSP. Las nuevas compras y los cambios en el recuento de puestos de las suscripciones existentes requerirán que el partner confirme el Contrato de cliente de Microsoft. Este requisito se aplica a los clientes nuevos y a los clientes existentes que puedan haber aceptado previamente el Contrato de Microsoft Cloud.|


## <a name="confirm-customer-acceptance-for-new-customers"></a>Confirmar la aceptación de los clientes nuevos

Si creas un nuevo inquilino de cliente en el Centro de partners, sigue los pasos que se describen a continuación para confirmar la aceptación del cliente del Contrato de cliente de Microsoft. Para poder seguir estos pasos, debes ser agente de administración o de ventas.

1. Selecciona **Clientes** y, a continuación, **Nuevo cliente**.

2. En **Información de cuenta**, especifica los datos de la empresa y su contacto principal.

3. En **Contrato de Microsoft**, selecciona **Contrato de cliente de Microsoft**.

4. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.

5. Comprueba que la información de contacto del usuario principal que se muestra sea correcta. Si no lo es, selecciona **Actualizar** y escribe el **Nombre**, los **Apellidos**, la **Dirección de correo electrónico** y el ***Número de teléfono** (opcional) de la persona que ha aceptado el contrato.

6. Selecciona **Siguiente** para continuar con los pasos restantes para crear el inquilino del cliente.

![Cliente nuevo](images/mcua1.png)

## <a name="confirm-customer-acceptance-for-existing-customers"></a>Confirmar la aceptación de los clientes existentes

Debes ser agente de administración o de ventas para poder hacer esto:

1. Selecciona **Clientes**. Busca y selecciona el cliente.

2. Selecciona **Información de cuenta**.

3. En **Contrato de cliente de Microsoft**, selecciona **Actualizar**.

4. Escribe el **Nombre**, los **Apellidos**, la **Dirección de correo electrónico** y el **Número de teléfono** (opcional) de la persona que aceptó el contrato. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.

5. Selecciona **Guardar** y continúa.

![Cliente existente](images/mcua2.png)

## <a name="retrieve-confirmation-of-customer-acceptance"></a>Recuperar la confirmación de la aceptación del cliente

Sigue los pasos que se describen a continuación para recuperar la confirmación de que un cliente existente ha aceptado el Contrato de cliente de Microsoft. Debes ser agente de administración o agente de ventas para poder hacer esto.

1. Selecciona **Clientes** y, a continuación, busca y selecciona el cliente que quieras ver.

2. Selecciona **Información de cuenta**.

3. En **Contrato de cliente de Microsoft**, consulta si el cliente ha proporcionado la confirmación.


