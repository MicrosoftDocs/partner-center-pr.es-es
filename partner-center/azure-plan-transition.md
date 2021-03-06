---
title: Traslado de clientes de las ofertas actuales de Azure al plan de Azure
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtén información sobre cómo los partners de CSP pueden usar el Centro de partners para trasladar a los clientes de las ofertas de CSP de Azure existentes a los servicios de Azure en el plan de Azure.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: 770df3cff40b8cc51eab16fb95d0bd43967a5a69
ms.sourcegitcommit: 3ac88f7925bfe1df90e267ee5c1ee4d752ac92d4
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 06/29/2021
ms.locfileid: "113013274"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>Transición de clientes al plan de Azure desde ofertas de CSP de Azure existentes

**Se aplica a**: Centro de partners 

**Roles adecuados**: Agente de administración | Administrador de facturación | Administrador global | Agente de soporte técnico | Agente de ventas | Administrador de control de usuarios

En este artículo se explica cómo los partners de CSP pueden usar el Centro de partners para trasladar a los clientes de las ofertas de CSP de Azure existentes a los servicios de Azure en el plan de Azure. Los proveedores indirectos y los partners de facturación directa pueden realizar la transición a la nueva experiencia de comercio disponible en el programa Proveedor de soluciones en la nube de Microsoft (CSP) de Azure. (Los revendedores indirectos deberán trabajar a través de sus proveedores indirectos). Gracias a ello, los clientes tendrán una forma simplificada de comprar servicios en la nube, ya sea comprando a partners, vendedores de Microsoft o directamente en la web.

La funcionalidad de transición solo es para clientes que realicen la transición a la nueva experiencia comercial y que hayan firmado el Contrato de cliente de Microsoft. No se aplica a otras ofertas del programa CSP, como Office 365 o Dynamics 365.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Transición de ofertas de CSP existentes a un plan de Azure

Puedes hacer la transición de un cliente desde sus ofertas existentes de Azure en CSP hacia los servicios de Azure que se incluyen en el plan de Azure, en la nueva experiencia comercial del programa CSP mediante el Centro de partners. Para hacerlo, el partner y el cliente deben tener una relación de vendedor establecida a través del Centro de partners, y el cliente debe haber firmado el Contrato de cliente de Microsoft.

### <a name="select-transition-to-azure-plan"></a>Seleccionar la transición al plan de Azure

1. Selecciona el plan de Azure para su cliente.

2. Selecciona la **transición de facturación al plan de Azure**.

   :::image type="content" source="images/azure/transition1.png" alt-text="Captura de pantalla que muestra el informe con datos de suscripciones basadas en el uso con una opción seleccionable denominada: Transición de facturación de suscripciones de Azure al plan de Azure.":::

3. Selecciona **Continue** (Continuar)

   :::image type="content" source="images/azure/transition2.png" alt-text="Cuadro de diálogo titulado Transición al plan de Azure con implicaciones para leer sobre la transición y dos opciones para seleccionar, Continuar o Cancelar.":::

   Tu cliente cambiará al plan de Azure.

   **El flujo de trabajo de la transición automatiza los pasos de requisitos previos**:

   - Compra de planes de Azure
   - Un plan por cliente en escenarios de CSP directo  
   - Un plan por vendedor  

   Por ejemplo, un partner compra dos ofertas de Microsoft Azure e incluye dos POR diferentes en la compra. En este caso, el flujo de trabajo de la transición comprará dos planes de Azure (uno por cada vendedor) y asignará las suscripciones a Azure respectivas en los planes de Azure automáticamente.  

   **Asignación de la suscripción de Azure al plan de Azure**

   Después de comprar los planes de Azure, nuestro sistema asignará las suscripciones de Azure existentes a los planes de Azure. El progreso se puede ver en Azure Portal, así como en el Centro de partners.

4. Regresa a la página de **suscripciones**  del Centro de partners del cliente para actualizar el límite de presupuesto con su moneda local.

   :::image type="content" source="images/azure/transition3.png" alt-text="Vista parcial de la página de suscripciones del Centro de partners con los límites de presupuesto establecidos en la moneda local para un período de facturación.":::

   >[!NOTE]
   >El presupuesto que establezcas en el Centro de partners no se transferirá a Azure Portal. Recuerda que también debes establecer el presupuesto y la alerta en Azure Portal.

   Cuando pases al plan de Azure, ya no podrás comprar suscripciones de Azure para este cliente. Deberás crear las suscripciones según el plan de Azure en Azure Portal.

   >[!NOTE]
   > Todas las suscripciones de Azure compradas a través de RBAC en el plan de Azure se cobrarán y facturarán en la moneda local. No se usarán las tarifas de FX.

### <a name="track-your-transition-details"></a>Seguimiento de los detalles de la transición

Sigue el progreso de la transición en Azure Portal, así como en el Centro de partners.

:::image type="content" source="images/azure/details1.png" alt-text="Captura de pantalla que muestra la tabla con una lista de detalles de transición por suscripción: incluye el identificador de suscripción, la fecha de transición y el estado de la transición.":::

### <a name="billing-impact-to-partners"></a>Impacto de la facturación en los partners

Si realizas la transición de un cliente desde una oferta existente de Azure en CSP, se aplicarán los siguientes puntos de facturación:

- Se le cargará en su factura del programa CSP existente todo el uso hasta el momento de la salida de la suscripción de Azure original en el CSP.

- Si tenía derechos de acceso de administrador en la suscripción de CSP existente, continuará teniendo acceso cuando se migre esa suscripción.

Para realizar la transición de los Contratos Enterprise directos a las inscripciones de CSP y de servidor y de nube a los servicios de Azure, consulta [Obtener la propiedad de facturación de las suscripciones de Azure para Microsoft Partner Agreement](/azure/billing/mpa-request-ownership).

### <a name="audit-log"></a>Registro de auditoría

Para conciliar la facturación, consulta tu historial de suscripciones de "Microsoft Azure" (0145P) en la página **Suscripciones**.

La suscripción a "Microsoft Azure" (0145P) consta de dos partes:

1. Suscripción comercial
2. Suscripción de Azure (derecho)

Cuando se completa la transición, la suscripción de Azure se administra en función del nuevo plan de Azure, y la suscripción comercial se suspende para que no se notifique ningún uso adicional.  

>[!NOTE]
>Cuando la suscripción de Microsoft Azure (0145P) se compra en CSP, tanto la suscripción comercial como la de Azure (derecho) tienen el mismo valor. Solo en el caso de realizar cambios o transferencias en la propiedad de facturación difieren los valores.

### <a name="transition-issues"></a>Problemas de transición

No se prevé ningún problema durante las transiciones. Si se produce alguno, lo actualizaremos en el flujo de trabajo de la transición. No habrá ninguna interrupción mientras use Azure.  

## <a name="next-steps"></a>Pasos siguientes

- [Administrar suscripciones y recursos en el plan de Azure](azure-plan-manage.md)

- [Créditos obtenidos del partner: introducción](partner-earned-credit.md)
