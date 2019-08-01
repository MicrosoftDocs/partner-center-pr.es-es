---
title: Confirmar la aceptación del cliente del contrato de cliente de Microsoft | Centro de Partners
ms.topic: article
ms.date: 04/16/2019
Description: Como Partner, debe obtener la aceptación del cliente del contrato de cliente de Microsoft antes de poder solicitar servicios y productos de Microsoft para ese cliente. Para ayudar a los asociados a satisfacer los requisitos de cumplimiento, Microsoft pide a los asociados que confirmen la aceptación proporcionando ciertos detalles sobre la persona que aceptó el contrato.
author: LauraBrenner
ms.author: labrenne
keywords: cliente, clientes, consentimiento, MCA, contrato de Microsoft Cloud, contrato de cliente de Microsoft, plantillas de contrato de cliente
ms.localizationpriority: medium
ms.openlocfilehash: 6ca8eb3acdee0114f01dbd5952e9c092859147a2
ms.sourcegitcommit: ee722dc2b9d82557d273738b64cec6d8cb435084
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/31/2019
ms.locfileid: "68681761"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-preview"></a>Confirmar la aceptación del cliente del contrato de cliente de Microsoft (versión preliminar)

Actualmente, antes de que un asociado de CSP pueda realizar un pedido en nombre de un cliente, el cliente debe aceptar y firmar el **acuerdo de Microsoft Cloud**aplicable. A continuación, el asociado debe confirmar su aceptación del cliente proporcionando información sobre el firmante a Microsoft. Si un cliente no confirma su aceptación del contrato de Microsoft Cloud:
- No podrás crear nuevos pedidos para este cliente.
- No podrás cambiar el número de puestos de suscripciones existentes en función de puestos para este cliente.

Para obtener más información sobre cómo confirmar la aceptación de un cliente del acuerdo de Microsoft Cloud mediante el panel del centro de Partners o la API, consulte [confirmar la aceptación del cliente del acuerdo de Microsoft Cloud](confirm-consent.md).

El 1 de octubre de 2019, Microsoft introducirá el **contrato de cliente de Microsoft** en el programa CSP para reemplazar el contrato de Microsoft Cloud. Para facilitar la migración de los asociados al nuevo contrato, se admitirá el contrato de Microsoft Cloud actual en el programa CSP hasta el 31 de enero de 2019. Para obtener más información sobre la escala de tiempo, vea la tabla siguiente:

| Date | Hito | Detalles |
|------------|------------|--------------------------------|
|01 de agosto de 2019|Versión preliminar de la experiencia del usuario disponible en el espacio aislado|Los asociados pueden confirmar la aceptación del cliente del acuerdo de cliente de Microsoft mediante el panel del centro de Partners en el entorno de espacio aislado de CSP. Asociados con acceso a la vista previa del entorno de espacio aislado de CSP que cambia la experiencia del usuario. Los asociados sin acceso al espacio aislado pueden obtener información sobre los cambios de este tema.|
|02 de septiembre de 2019|La versión preliminar de la API está disponible en el espacio aislado.|Los asociados pueden confirmar la aceptación del cliente del acuerdo de cliente de Microsoft mediante la API del centro de Partners en el entorno de espacio aislado de CSP. Los asociados de API pueden usar esta oportunidad para obtener una vista previa de los cambios de la API y comenzar a trabajar en la integración de API para admitir el nuevo contrato.|
|1 de octubre de 2019|Contrato de cliente de Microsoft disponible en producción|Microsoft presenta el contrato de cliente de Microsoft al programa CSP para reemplazar el contrato de Microsoft Cloud. Los asociados pueden confirmar la aceptación del cliente del acuerdo de cliente de Microsoft mediante el panel del centro de Partners y la API en producción. El contrato de Microsoft Cloud sigue siendo compatible con el programa de asociados de CSP. Sin embargo, se recomienda que los asociados empiecen a migrar al contrato de atención al cliente de Microsoft. Las nuevas compras y los cambios de recuento de puestos de las suscripciones existentes requerirán la confirmación del asociado del contrato de cliente de Microsoft o del contrato de Microsoft Cloud. Ciertas ofertas nuevas (por ejemplo, el nuevo plan de Azure) requerirán la confirmación del contrato de cliente de Microsoft.|
|31 de enero de 2019|Microsoft Cloud acuerdo quitado de la producción|El contrato de Microsoft Cloud ya no se acepta dentro del programa de asociados de CSP. Las nuevas compras y los cambios de número de puestos de las suscripciones existentes requerirán que el socio proporcione la confirmación del contrato de cliente de Microsoft. Este requisito se aplica a los clientes nuevos y a los clientes existentes que puedan haber aceptado previamente el contrato de Microsoft Cloud.|


## <a name="confirm-customer-acceptance-for-new-customers"></a>Confirmar la aceptación del cliente para nuevos clientes

Al crear un nuevo inquilino de cliente en el centro de Partners, siga estos pasos para confirmar la aceptación del cliente del contrato de cliente de Microsoft. Debe ser un agente de administración o un agente de ventas para realizar estos pasos.

1. Selecciona **Clientes** y luego **Nuevo cliente**.

2. En **información**de la cuenta, escriba la información de la empresa y su contacto principal.

3. En **contrato de Microsoft**, seleccione el **contrato de cliente de Microsoft**.

4. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.

5. Asegúrese de que la información de contacto del usuario principal mostrada sea correcta. Si no es correcta, seleccione **Actualizar** y escriba el **nombre**, los **apellidos**, la **dirección de correo electrónico**y el número de **teléfono** (opcional) de la persona que aceptó el contrato.

6. Selecciona **Siguiente** para continuar con los pasos restantes para crear el inquilino del cliente.

![Nuevo cliente](images/mcua1.png)

## <a name="confirm-customer-acceptance-for-existing-customers"></a>Confirmar la aceptación del cliente para clientes existentes

Para ello, debe ser un agente de administración o un agente de ventas:

1. Seleccione **clientes**. Busque y seleccione el cliente.

2. Seleccione la información de la **cuenta**.

3. En **contrato de cliente de Microsoft**, seleccione **Actualizar**.

4. Escriba el **nombre**, los **apellidos**, la **dirección de correo electrónico**y el **número de teléfono** (opcional) de la persona que aceptó el contrato. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.

5. Seleccione **Guardar** y continuar.

![Cliente existente](images/mcua2.png)

## <a name="retrieve-confirmation-of-customer-acceptance"></a>Recuperar confirmación de aceptación del cliente

Puede recuperar la confirmación de que un cliente existente ha aceptado el contrato de cliente de Microsoft mediante los pasos siguientes. Debes ser agente de administración o agente de ventas para poder hacer esto.

1. Selecciona **Clientes**y, a continuación, busca y selecciona el cliente que quieras ver.

2. Seleccione la información de la **cuenta**.

3. En **contrato de nube de Microsoft**, vea si el cliente tiene o no ha proporcionado la confirmación.


