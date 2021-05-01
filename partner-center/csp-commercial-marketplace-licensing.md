---
title: Administración de licencias en ofertas de Marketplace
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Aprenda a configurar y administrar licencias para las ofertas del marketplace comercial de ISV.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f049ffda4c3d9476c09257fc814e5acac393cb54
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328022"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Administración de licencias en ofertas de Marketplace

**Roles adecuados**

- Administrador global
- Administrador de cuentas

Este artículo le guía por el proceso de configuración de una oferta en Centro de partners, su disponibilidad en Microsoft AppSource y, a continuación, la administración de licencias para esa oferta.  

>[!IMPORTANT]
>Las funcionalidades de este artículo están actualmente en versión preliminar pública.

## <a name="before-you-begin"></a>Antes de empezar

### <a name="commercial-marketplace-basics"></a>Conceptos básicos de Marketplace comercial

Antes de comenzar este proceso, debe familiarizarse con los conceptos básicos del marketplace comercial. Los artículos de la tabla siguiente le ayudarán a empezar a trabajar. 

| Tema  | Artículo  |
|-------|--------|
|Planes de Marketplace comercial | [Planes y precios de las ofertas del marketplace comercial](/azure/marketplace/plans-pricing)    |
|Ofertas de Marketplace comercial  | [Enumeración de tipos](/azure/marketplace/determine-your-listing-type)    |
|Cuentas de Marketplace comercial |  [Creación de una cuenta de Marketplace comercial en el Centro de partners](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a>Determinación del identificador de la oferta

En los procedimientos siguientes, se le pedirá que escriba un identificador de oferta. Tómese un tiempo para obtener un identificador de oferta adecuado, teniendo en cuenta los siguientes puntos:

- Se muestra a los clientes en la dirección web de la oferta de Marketplace y en las plantillas de Azure Resource Manager, si procede.
- El identificador de oferta en combinación con el del editor debe tener una longitud de menos de 40 caracteres.
- Use solo letras minúsculas y números. El identificador de la oferta puede incluir guiones y caracteres de subrayado, pero no espacios. Por ejemplo, si el identificador del publicador `testpublisherid` es y escribe , la dirección web de la oferta será `test-offer-1` `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .
- Este identificador no se puede cambiar después de seleccionar **Crear**.

### <a name="determine-your-offer-alias"></a>Determinación del alias de la oferta

El alias De oferta es el nombre que se usa para la oferta en Centro de partners. También necesitará un alias de oferta adecuado que siga las instrucciones siguientes:

- Este nombre no se usa en Marketplace y es diferente del nombre de la oferta y de otros valores que se muestran a los clientes.
- Este nombre no se puede cambiar después de seleccionar Crear.

## <a name="create-your-offer"></a>Creación de la oferta

El primer paso del proceso de licencia es crear la oferta de Marketplace comercial. 

1. Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).
2. En el menú de navegación izquierdo, seleccione **Marketplace comercial/Información general.**
3. En la parte superior de la página Información general, seleccione Nueva oferta y, a continuación, seleccione **Dynamics 365 for Customer Engagement & PowerApps.**
4. Escriba el **identificador de la oferta** y el alias de **la** oferta que creó anteriormente.
5. Seleccione **Crear** para generar la oferta y continuar.
6. Elija las opciones de licencia.

    - Para habilitar la administración de licencias para la oferta, seleccione **Habilitar la administración de licencias de aplicaciones a través de Microsoft**. Se trata de una configuración única y no se puede cambiar una vez publicada la oferta.

    - También puede permitir que los clientes ejecuten la funcionalidad base de la aplicación sin una licencia y ejecuten características Premium una vez que han adquirido una licencia. Para ello, seleccione **Permitir que los clientes instalen mi aplicación aunque no se asignen licencias.**

    - Si no desea que la oferta tenga habilitada la administración de licencias, seleccione Obtenerla **ahora (gratis),** Evaluación gratuita o Póngase **en contacto conmigo.**

## <a name="create-your-plan"></a>Crear el plan

En estos pasos definirá el plan o los planes que desea habilitar para la oferta.

1. En el menú de navegación izquierdo, seleccione **Información general del** plan y, a continuación, seleccione Crear nuevo **plan.**
2. Escriba un **id. de** plan y **un nombre de** plan y, a continuación, seleccione **Crear.**
3. En la **página Lista de** planes, escriba la descripción del **plan.**
4. Para guardar la descripción y finalizar más adelante, seleccione **Guardar borrador.**

5. Cuando haya terminado, seleccione **Revisar y publicar**. La información del plan se mostrará ahora en appsource.microsoft.com descripción de la oferta (sección planes).

6. Después de crear todos los planes para esta oferta, deberá copiar el identificador de servicio de cada plan. Seleccione **Información general del** plan en la parte superior de la página Lista de planes. Copie el identificador de servicio de cada plan en una ubicación segura.

## <a name="add-service-ids-to-your-solution"></a>Adición de los IDs de servicio a la solución

El siguiente paso consiste en actualizar la solución mediante la adición de los IDs de servicio para cada plan que acaba de copiar. Para obtener instrucciones sobre esto, consulte [Creación de un paquete de AppSource para la solución.](https://docs.microsoft.com/powerapps/developer/data-platform/create-package-app-appsource)

## <a name="upload-your-package-and-publish-your-offer"></a>Carga del paquete y publicación de la oferta

1. En el panel de navegación izquierdo, seleccione **Marketplace comercial** y, a continuación, **configuración técnica.**
2. En **Modelo de licencia base,** seleccione **Usuario**.
3. En **Paquete CRM,** escriba la dirección URL de la ubicación del paquete.
4. Use las demás pestañas del panel de navegación izquierdo para escribir cualquier otra información necesaria. Cuando haya terminado, seleccione **Revisar y publicar**.

Después de publicar la oferta, revisaremos y comprobaremos la información. Si hay algún problema con este proceso, se le notificará. Cuando se hayan resuelto todos los problemas, se le envía una notificación de que la oferta está disponible en AppSource. En ese momento, puede hacerlo en directo.

## <a name="make-your-offer-live-in-partner-center"></a>Hacer que la oferta se realice en Centro de partners

El procedimiento siguiente le guía por el proceso de hacer que su oferta se haga en AppSource. Para más información sobre este proceso, consulte [Introducción a las opciones de enumeración.](https://docs.microsoft.com/azure/marketplace/determine-your-listing-type)

>[!NOTE]
>Una vez publicada la oferta, se tardarán entre 4 y 6 horas en publicarse.

1. Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).
2. En el menú de navegación izquierdo, seleccione **Marketplace comercial/Información general.**
3. En la **página** Información general, busque la oferta que busca. Las ofertas listas para publicarse tendrán el estado Preview **(Versión preliminar).** Seleccione la oferta.
4. En la **página Información general de** la oferta, seleccione Ir a **.**
La oferta estará en directo en 4-6 horas.
5. Para ver la lista de ofertas en AppSource, seleccione el **vínculo AppSource** en la parte inferior de la página **Información general de la** oferta.

    - **Para las ofertas habilitadas** para licencia: si la oferta requiere una comprobación de licencia, los usuarios solo podrán escribir un cliente potencial haciendo clic en Ponerse en contacto conmigo **para** que pueda comunicarse con ellos.

    - **Para las ofertas habilitadas** para licencias con opción de instalación gratuita: si  la oferta no requiere una comprobación de licencia, los usuarios administradores verán un botón Obtenerla ahora además de Ponerse **en contacto conmigo.** Los usuarios que quieran probar la opción de instalación gratuita deben hacer clic en Obtenerla **ahora,** lo que les permitirá instalar la oferta en Power Platform Admin Center. Los usuarios pueden seguir utilizando **Ponerse** en contacto conmigo si tienen alguna pregunta o si quieren actualizar a un plan de pago.

## <a name="register-isv-connect-deal-in-deal-registration"></a>Registro de la oferta de ISV Connect en el registro de la oferta

Para poder asignar licencias a un cliente, cada venta debe registrarse en Centro de partners. Para ello, consulte Registro [de las ofertas.](register-deals.md)

## <a name="invite-the-customer"></a>Invitar al cliente

Use el procedimiento siguiente para invitar al cliente a participar en esta oferta.  

1. Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard/).
2. En el menú de navegación izquierdo, seleccione **Marketplace comercial/Información general.**
3. En el menú de navegación izquierdo, seleccione **Referencias** y, a continuación, seleccione **Registro de la oferta.**
4. Filtre **por Ofertas enviadas,** seleccione la **pestaña** En curso y, a continuación, seleccione la oferta que desee.
5. En la página de información general de esta oferta, seleccione **Administrar licencias.**
6. En la **ventana Administrar licencias,** seleccione el cliente en la **lista desplegable Detalles del** cliente. Si la relación con el cliente aún no existe, seleccione **+Invitar a un nuevo cliente a dar su consentimiento.**
7. Copie el vínculo que se muestra.
8. Envíe por correo electrónico este vínculo al administrador de facturación o al administrador global del cliente y haga que use este vínculo para acceder a admin.microsoft.com y aceptar y autorizar la relación que está estableciendo.

    >[!NOTE]
    >La relación no se establecerá hasta que el cliente realice este paso.

## <a name="activate-manage-and-remove-your-licenses"></a>Activación, administración y eliminación de licencias

Una vez que el cliente haya autorizado la relación con usted, puede empezar a agregar planes de la oferta y asignar licencias a cada plan.

1. En la ventana Administrar licencias de esta oferta, seleccione **+Agregar un plan.**
2. Complete los **campos Planes para esta solución** y Número de **licencias** y, a continuación, seleccione **Actualizar licencias.** Las licencias estarán disponibles en admin.microsoft.com para que los clientes las administren y asignen a los empleados.

    - Para cambiar el número de licencias de un plan  existente, escriba el nuevo número en el campo Número de licencias y seleccione **Actualizar licencias.**

    - Para desactivar o quitar licencias para una oferta,  seleccione el icono de papelera en el campo Acciones y, a continuación, **seleccione Actualizar licencias.**

## <a name="next-steps"></a>Pasos siguientes

[Recursos de licencias](support-resources-licensing.md)
