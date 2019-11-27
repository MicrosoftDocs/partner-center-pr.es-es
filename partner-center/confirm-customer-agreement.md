---
title: Confirmación de la aceptación por parte del cliente del Contrato de cliente de Microsoft | Centro de partners
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Obtenga información sobre cómo confirmar la aceptación del cliente del contrato de cliente de Microsoft. Esto puede ser necesario para ordenar los productos y servicios de Microsoft para los clientes.
author: LauraBrenner
ms.author: labrenne
keywords: customer, customers, consent, MCA, Microsoft Cloud Agreement, Microsoft Customer Agreement, customer agreement templates
ms.localizationpriority: medium
ms.openlocfilehash: 9d362f581d0d318b1a457ba6a75db54713fce6bb
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252231"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Confirmar la aceptación del cliente del contrato de cliente de Microsoft

Actualmente, antes de que un asociado de CSP pueda realizar un pedido en nombre de un cliente, el cliente debe aceptar y firmar el **acuerdo de Microsoft Cloud**aplicable. A continuación, el asociado debe confirmar la aceptación por parte del cliente proporcionando información sobre el firmante a Microsoft. Si no se proporciona la confirmación:
- No podrá crear nuevos pedidos para este cliente.
- No podrá cambiar el número de puestos de las suscripciones basadas en puestos existentes para este cliente.

Para obtener más información sobre cómo confirmar la aceptación de un cliente del Contrato de Microsoft Cloud mediante la API o el panel del Centro de partners, consulta [Confirm customer acceptance of the Microsoft Cloud Agreement](confirm-consent.md) (Confirmar la aceptación del Contrato de Microsoft Cloud por parte del cliente).

El 1 de octubre de 2019, Microsoft introducirá el **Contrato de cliente de Microsoft** en el programa CSP para reemplazar el Contrato de Microsoft Cloud. Para facilitar la migración de los asociados al nuevo contrato, se admitirá el Contrato de Microsoft Cloud actual en el programa CSP hasta el 31 de enero de 2020. Para obtener más detalles sobre la línea de tiempo, consulta la tabla siguiente:

| Fecha | Hito | Detalles |
|------------|------------|--------------------------------|
|01 de agosto de 2019|Versión preliminar de la experiencia del usuario disponible en el espacio aislado|Los partners pueden confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft desde el panel del Centro de partners del entorno del espacio aislado de CSP. Los partners con acceso al entorno de espacio aislado de CSP pueden acceder a una versión preliminar de los cambios en la experiencia del usuario. Los partners sin acceso al espacio aislado pueden obtener información sobre los cambios en este tema.|
|03 de septiembre de 2019|Hay una versión preliminar de la API disponible en el espacio aislado.|El partner puede confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft desde la API del Centro de partners del entorno del espacio aislado de CSP. Los partners de la API pueden usar esta oportunidad para acceder a una versión preliminar de los cambios de la API y comenzar a trabajar en la integración de la API para admitir el nuevo contrato.|
|20 de septiembre de 2019|Hay una versión preliminar del SDK de .NET disponible en el espacio aislado.|El asociado puede confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft mediante el SDK de .NET del Centro de partners del entorno del espacio aislado de CSP. Los asociados de la API pueden usar esta oportunidad para acceder a una versión preliminar de los cambios del SDK de .NET y comenzar a trabajar en la integración de la API para admitir el nuevo contrato.|
|01 de octubre de 2019|Contrato de cliente de Microsoft disponible en el entorno de producción|Microsoft introducirá el Contrato de cliente de Microsoft en el programa CSP para reemplazar el Contrato de Microsoft Cloud. Los partners pueden confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft desde la API y el panel del Centro de partners en el entorno de producción. El Contrato de Microsoft Cloud sigue siendo compatible con el programa de partners de CSP. Sin embargo, es recomendable que los partners inicien la migración al Contrato de cliente de Microsoft. Las nuevas compras y los cambios en el recuento de puestos de las suscripciones existentes requerirán la confirmación por parte del partner del Contrato de cliente de Microsoft o del Contrato de Microsoft Cloud. Ciertas ofertas nuevas (por ejemplo, el nuevo plan de Azure) requerirán la confirmación del Contrato de cliente de Microsoft.|
|31 de enero de 2020|El Contrato de Microsoft Cloud se quitó de la producción|El Contrato de Microsoft Cloud ya no se acepta en el programa para partners de CSP. Las nuevas compras y los cambios en el recuento de puestos de las suscripciones existentes requerirán que el partner confirme el Contrato de cliente de Microsoft. Este requisito se aplica a los clientes nuevos y a los clientes existentes que puedan haber aceptado previamente el Contrato de Microsoft Cloud.|

## <a name="access-microsoft-customer-agreement-template"></a>Acceder a la plantilla de acuerdo de cliente de Microsoft
Los asociados pueden descargar manualmente la versión más reciente de la plantilla de contrato de cliente de Microsoft [aquí](https://aka.ms/customeragreement). Tenga en cuenta que el acuerdo de cliente de Microsoft es específico del país. Al solicitar la plantilla de contrato de cliente de Microsoft, asegúrese de seleccionar el país correcto en función de la ubicación del cliente. 

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Confirmar la aceptación del cliente mediante el SDK/API del centro de Partners
Los asociados pueden usar el SDK/API del centro de partners para confirmar la aceptación del cliente del contrato de cliente de Microsoft. Para obtener más información sobre la API/SDK, consulte:

- [Obtener los metadatos del acuerdo del Contrato de cliente de Microsoft](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [Confirmar la aceptación por parte del cliente del Contrato de cliente de Microsoft](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Obtener confirmación de la aceptación por parte del cliente del Contrato de cliente de Microsoft](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [Obtener un vínculo de descarga para la plantilla del Contrato de cliente de Microsoft](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)


## <a name="confirm-customer-acceptance-in-partner-center"></a>Confirmación de la aceptación por parte del cliente en el Centro de partners
Los asociados pueden confirmar la aceptación del cliente del acuerdo de cliente de Microsoft en el centro de partners para nuevos clientes y clientes existentes.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Confirmar la aceptación de los clientes nuevos

Si creas un nuevo inquilino de cliente en el Centro de partners, sigue los pasos que se describen a continuación para confirmar la aceptación del cliente del Contrato de cliente de Microsoft. Para poder seguir estos pasos, debes ser agente de administración o de ventas.

1. Selecciona **Clientes** y, a continuación, **Nuevo cliente**.

2. En **Información de cuenta**, especifica los datos de la empresa y su contacto principal.

3. En **Contrato de Microsoft**, selecciona **Contrato de cliente de Microsoft**.

4. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.

5. Comprueba que la información de contacto del usuario principal que se muestra sea correcta. Si no lo es, selecciona **Actualizar** y escribe el **Nombre**, los **Apellidos**, la **Dirección de correo electrónico** y el ***Número de teléfono** (opcional) de la persona que ha aceptado el contrato.

6. Selecciona **Siguiente** para continuar con los pasos restantes para crear el inquilino del cliente.

![Cliente nuevo](images/mcua1.png)

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Confirmar la aceptación de los clientes existentes

Debes ser agente de administración o de ventas para poder hacer esto:

1. Selecciona **Clientes**. Busca y selecciona el cliente.

2. Selecciona **Información de cuenta**.

3. En **Contrato de cliente de Microsoft**, selecciona **Actualizar**.

4. Escribe el **Nombre**, los **Apellidos**, la **Dirección de correo electrónico** y el **Número de teléfono** (opcional) de la persona que aceptó el contrato. En **Fecha de aceptación del contrato**, introduce la fecha adecuada. No puedes elegir para esto una fecha futura.

5. Selecciona **Guardar** y continúa.

![Cliente existente](images/mcua2.png)

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Recuperar la confirmación de la aceptación del cliente

Sigue los pasos que se describen a continuación para recuperar la confirmación de que un cliente existente ha aceptado el Contrato de cliente de Microsoft. Debes ser agente de administración o agente de ventas para poder hacer esto.

1. Selecciona **Clientes** y, a continuación, busca y selecciona el cliente que quieras ver.

2. Selecciona **Información de cuenta**.

3. En **Contrato de cliente de Microsoft**, consulta si el cliente ha proporcionado la confirmación.
