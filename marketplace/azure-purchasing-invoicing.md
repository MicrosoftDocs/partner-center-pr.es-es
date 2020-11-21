---
title: Compra de software y soluciones desde Azure Marketplace
description: Obtenga información sobre las herramientas que simplifican y agilizan las compras y la administración de software en Azure Marketplace.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: b93ce1394326887b4265114c58527c36379101d9
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007371"
---
# <a name="azure-marketplace-purchasing"></a>Compras de Azure Marketplace

Azure Marketplace tiene numerosas herramientas y características que simplifican y simplifican el proceso de compra, facturación y administración de directivas de compra.

## <a name="simplified-procurement"></a>Adquisición simplificada

Azure Marketplace le ayuda a simplificar el proceso de adquisición a través de diferentes opciones de compra. Si compra productos con una tarjeta de crédito asociada a su cuenta de Azure, todas las compras se consolidarán en una sola factura y se facturarán a la tarjeta de crédito que elija. Si es un cliente de gran tamaño, puede comprar mediante una Contrato Enterprise. Con un contrato Enterprise, las compras de software se incluyen automáticamente en la factura de Azure. La factura contendrá los cargos de uso de Azure en primer lugar, seguidos de los de Azure Marketplace.

Al comprar a través de Azure Marketplace, elimina la complejidad de la administración de las relaciones y las facturas de los proveedores individuales. Obtendrá una factura mensual única y consolidada de Microsoft que incluye las compras de Azure Marketplace y los cargos de Azure.

## <a name="permission-to-purchase"></a>Permiso para comprar

Una vez que haya encontrado la aplicación de software correcta, la finalización de la compra es sencilla. Sin embargo, tendrá permisos adecuados en la suscripción de Azure. Dado que Azure funciona en un modelo de [Access Control basado en roles](https://docs.microsoft.com/azure/role-based-access-control/overview) (RBAC), la cuenta necesita permisos de **propietario** o **colaborador** de la suscripción para hacer una compra.

Antes de completar una compra, asegúrese de que el usuario tiene la configuración correcta en el inquilino de Azure. Esto ayudará a evitar errores durante la compra.

En la experiencia de Azure Marketplace en el Azure Portal, busque la aplicación que quiere comprar y seleccione **crear** o **configurar + suscribirse**. Se le pedirá que complete la información antes de poder usar la nueva solución.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Botón de creación de la oferta.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="El botón Configurar + suscribir.":::

Si desea implementar una solución desde la tienda en línea de Azure Marketplace, seleccione **obtenerla ahora** en la página Descripción del producto y, a continuación, inicie sesión con las credenciales de su cuenta de Azure.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="El cuadro de diálogo de inicio de sesión de Azure Marketplace.":::

Una vez que inicie sesión, se le redirigirá al producto en el Azure Portal para completar la compra.

## <a name="purchase-policy-management"></a>Administración de directivas de compra

Microsoft le permite administrar las compras de usuarios a través de su perfil de facturación como administrador de suscripciones de Azure. Elija una de las tres opciones:

- **Gratis + pago** : permite a los usuarios adquirir cualquier aplicación de software de Azure Marketplace.
- **Gratis** : permite a los usuarios implementar solo software gratuito de Azure Marketplace.
- **No** : impide que los usuarios implementen software desde Azure Marketplace.

Esta configuración se aplica a todos los usuarios con acceso a su suscripción de Azure, lo que le ofrece la capacidad de controlar la adquisición de ti a través de la Azure Portal.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Control de la adquisición de ti a través del Azure Portal":::

## <a name="cost-management"></a>Administración de costos

A medida que compra productos de Azure Marketplace, querrá obtener información que le ayude a administrar los costos. Azure Cost Management es una herramienta gratuita para ver información sobre los productos que ha adquirido. Puede usar Cost Management para ver detalles de los servicios con los que está gastando dinero a lo largo del tiempo y cómo esos costos realizan un seguimiento de los presupuestos que ha establecido. Además de establecer presupuestos, puede programar informes y analizar los costos de las suscripciones. Para obtener más información sobre Azure Cost Management, complete el módulo de Microsoft Learn en [análisis de costos y creación de presupuestos con Azure cost Management](https://docs.microsoft.com/learn/modules/analyze-costs-create-budgets-azure-cost-management/).

Puede ver los cargos y las facturas de Azure Marketplace en la herramienta de análisis de costos en Azure Cost Management.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Use Azure Cost Management para obtener información sobre los productos adquiridos.":::

## <a name="next-steps"></a>Pasos siguientes

- [Facturación y facturación](billing-invoicing.md)
