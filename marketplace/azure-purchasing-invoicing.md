---
title: Compra de software y soluciones de Azure Marketplace
description: Obtenga información sobre las herramientas que simplifican y simplifican las compras y la administración de software en Azure Marketplace.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 06/22/2021
ms.openlocfilehash: 0e79674825f8ab28fa4b0e68dd01c9c1b7e8c27a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565192"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace compra

Azure Marketplace tiene numerosas herramientas y características que simplifican y simplifican el proceso de compra, facturación y administración de la directiva de compra.

## <a name="simplified-procurement"></a>Adquisición simplificada

Azure Marketplace le ayuda a simplificar el proceso de adquisición a través de diferentes opciones de compra. Si compra productos con una tarjeta de crédito asociada a su cuenta de Azure, todas las compras se consolidarán en una sola factura y se facturarán en la tarjeta de crédito que prefiera. Si es un cliente grande, puede comprar mediante un Contrato Enterprise. Con un EA, las compras de software se incluyen automáticamente en la factura de Azure. La factura contendrá los cargos de uso de Azure en primer lugar, seguidos de los de Azure Marketplace.

Al comprar a través de Azure Marketplace, se elimina la complejidad de administrar las relaciones y facturas de proveedores individuales. Obtiene una factura mensual única y consolidada de Microsoft que incluye tanto las compras de Azure Marketplace como los cargos de Azure.

## <a name="permission-to-purchase"></a>Permiso para comprar

Una vez que haya encontrado la aplicación de software adecuada, completar la compra es sencillo. Sin embargo, necesitará permisos adecuados dentro de la suscripción de Azure. Puesto que Azure funciona en un modelo de Access Control [basado](/azure/role-based-access-control/overview) en  rol  (RBAC), la cuenta necesita permisos de propietario o colaborador de la suscripción para realizar una compra.

Antes de completar una compra, asegúrese de que el usuario tiene la configuración correcta en el inquilino de Azure. Esto le ayudará a evitar errores durante la compra.

En la Azure Marketplace en la Azure Portal, busque la aplicación que desea  comprar y seleccione Crear o Configurar **+ suscribirse.** Se le pedirá que complete alguna información antes de poder usar la nueva solución.

> [!CAUTION]
> La aprobación en Marketplace privado no indica la adquisición de una solución.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="Botón Crear oferta.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="El botón Configurar y suscribirse.":::

Si quiere implementar una solución desde la tienda en  línea de Azure Marketplace, seleccione Obtenerla ahora en la página de descripción del producto y, a continuación, inicie sesión con las credenciales de la cuenta de Azure.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Cuadro Azure Marketplace de diálogo de inicio de sesión.":::

Una vez que inicie sesión, se le redirigirá al producto en el Azure Portal para completar la compra.

## <a name="purchase-policy-management"></a>Administración de directivas de compra

Microsoft le permite administrar las compras de usuarios a través de su perfil de facturación como administrador de suscripciones de Azure. Elija una de las tres opciones:

- **Gratis y de pago:** permite a los usuarios adquirir cualquier Azure Marketplace software.
- **Gratis:** permite a los usuarios implementar solo software gratuito desde Azure Marketplace.
- **No:** impide que los usuarios implemente software Azure Marketplace.

Esta configuración se aplica a todos los usuarios con acceso a su suscripción de Azure, lo que le ofrece la capacidad de controlar la adquisición de TI a través del Azure Portal.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Controlar la adquisición de IT a través del Azure Portal.":::

## <a name="cost-management"></a>Administración de costos

A medida que compra productos Azure Marketplace, quiere obtener información que le ayude a administrar los costos. Azure Cost Management es una herramienta gratuita para ver información sobre los productos que ha adquirido. Puede usar Cost Management ver los detalles de los servicios en los que está gastando dinero a lo largo del tiempo y cómo se realiza el seguimiento de esos costos con respecto a los presupuestos que ha establecido. Además de establecer presupuestos, puede programar informes y analizar los costos de la suscripción. Obtenga más información sobre Azure Cost Management completando el módulo Microsoft Learn análisis de costos y creación de [presupuestos con Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).

Puede ver los cargos y las facturas de Azure Marketplace en la herramienta de análisis de costos en Azure Cost Management.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Use Azure Cost Management para obtener información sobre los productos adquiridos.":::

## <a name="purchase-validation-checks"></a>Comprobaciones de validación de compra

La compra de una oferta mediante Azure Marketplace puede producir un error por diferentes motivos. Es más probable que el uso de la interfaz de línea de comandos (CLI) para una compra cause errores, ya que es posible que esté intentando comprar una oferta que no esté disponible o visible en Azure Marketplace. Estas son las comprobaciones que pueden provocar un error en una compra:

1. La suscripción pertenece a un Contrato Enterprise (EA) y el administrador de EA deshabilitado Azure Marketplace compras.
1. El administrador de EA ha habilitado las compras solo para las ofertas gratuitas y la oferta es una oferta de pago.
1. La oferta no se encuentra en Marketplace.
1. El proveedor de software independiente (ISV) dejó de vender la oferta, al menos en su región.
1. La suscripción que usa pertenece a una cuenta de facturación de una región en la que la oferta no está disponible.
1. La cuenta de suscripción o facturación no está asociada a un instrumento de pago válido (por ejemplo, una tarjeta de crédito válida).
1. La suscripción pertenece a un Proveedor de soluciones en la nube (CSP) y el ISV rechazó vender a través de un CSP.
1. Marketplace privado está habilitado para la suscripción y la oferta no está en la lista de ofertas permitidas.
1. La oferta es Privada/Versión preliminar para clientes específicos y la suscripción no está en la lista de clientes permitidos.

La compra de ofertas de Marketplace podría producir un error si entra en conflicto con los Azure Policy definidos por el administrador de Azure en su organización. Por ejemplo, no puede comprar Microsoft.SaaS si no está en la lista de permitidos **de su** organización. Para obtener más información, [consulte Azure Policy documentación](/azure/governance/policy/).

## <a name="next-steps"></a>Pasos siguientes

- [Facturación](billing-invoicing.md)