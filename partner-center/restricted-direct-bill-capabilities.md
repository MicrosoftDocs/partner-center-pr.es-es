---
title: Funcionalidades de facturación directa restringidas
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre Proveedor de soluciones en la nube asociados de facturación directa (CSP) y qué hacer para evitar que las funcionalidades se restringen. Averigón si las funcionalidades se han restringido.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e5bc33101809a805ba591be5a9b51d8dfff2397b
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551425"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Funcionalidades de factura directa restringidas y los requisitos necesarios para los asociados de factura directa de CSP

**Roles apropiados**: administrador global

## <a name="overview"></a>Información general

Los asociados de factura directa deben cumplir los nuevos [requisitos](direct-partner-new-requirements.md) para permanecer en el programa Proveedor de soluciones en la nube asociados de facturación directa (CSP). De lo contrario, su acceso a las capacidades de factura directa se restringirá con el tiempo y ya no podrán realizar tareas específicas, como nuevas compras para sus clientes.

> [!Note]
> Microsoft informará a los asociados de factura directa que no cumplan los nuevos requisitos del programa de asociados de facturación directa de CSP cuando se restringirán sus funcionalidades de factura directa. Esto se aplica a todos los asociados de facturación directa, independientemente de si han optado por la transición del asociado de facturación directa a [revendedores indirectos](transition-direct-to-indirect.md) o no.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Cómo saber si las funcionalidades de factura directa se han restringido

Para confirmar si se ha restringido el acceso desde el inquilino del asociado de factura directa a las funcionalidades de facturación directa, siga estos pasos.

1. Inicie sesión en el [panel del Centro de partners](https://partner.microsoft.com/dashboard).

2. Vaya a **Configuración de la cuenta** Perfil  >  **legal.**

3. En **Información del programa,** busque Proveedor de soluciones en la nube de Microsoft **estado**.

4. Si el estado del programa tiene un valor **restringido,** significa que se ha restringido el acceso del inquilino del asociado de factura directa a las funcionalidades de facturación directa.

## <a name="affected-direct-bill-capabilities"></a>Funcionalidades de factura directa afectadas

Si se han restringido las funcionalidades de facturación directa, ya no podrá realizar nuevas compras para los clientes en Centro de partners. Esta restricción incluye:

- Suscripciones de Azure

- Suscripciones basadas en licencias

- Agregue nuevos complementos a las suscripciones basadas en licencias existentes.

- Realice compras únicas de software y productos de reserva (por ejemplo, suscripciones de software, software perpetuo e instancias reservadas de máquina virtual de Azure).

Tampoco puede usar la oferta de [servicios compartidos de asociados](shared-services.md) de Azure en el programa CSP para comprar nuevas suscripciones de Azure para su propio uso.

Las suscripciones de factura directa existentes no se ven afectadas. Siguen siendo válidos y se han renuevo de forma automática. Microsoft le seguirá facturando directamente hasta que se cancelen. Todavía puede administrar las suscripciones existentes de las maneras siguientes:

- Suspender suscripciones existentes

- Ajuste del recuento de licencias de las suscripciones basadas en licencias existentes

- Ajuste el número de licencias de los complementos existentes a una suscripción. 

    >[!Note]
    >No puede agregar nuevos complementos a las suscripciones existentes, ya que se tratan como una nueva compra.

- Implemente nuevos recursos de Azure y administre los recursos de Azure existentes en las suscripciones de Azure existentes. Esto incluye los recursos, que están disponibles a través de Azure Marketplace y Visual Studio suscripciones.

Además de las nuevas compras, no puede acceder a las siguientes funcionalidades de facturación directa en Centro de partners:

- No puede crear nuevos inquilinos de cliente. La **opción Crear cliente** en la **página** Clientes Centro de partners no estará disponible.

- No se puede generar una invitación al cliente que solicita una relación de revendedor directo. La **opción Solicitar una relación de** revendedor en **la** página Clientes Centro de partners no estará disponible.

    >[!NOTE]
    >Como parte de la transición de un asociado de factura directa a un revendedor indirecto, si ya ha inscrito el inquilino del asociado de facturación directa como revendedor indirecto, puede generar la invitación al cliente que solicita una relación de revendedor indirecto en su lugar.

- No puede crear un nuevo inquilino de espacio aislado. Cada inquilino de asociado de factura directa puede crear un inquilino de espacio aislado para la integración de la API de factura directa. Si no ha creado uno anteriormente, no puede hacerlo después de que se haya restringido la funcionalidad del asociado de facturación directa.  

## <a name="next-steps"></a>Pasos siguientes

- [Información adicional sobre cómo convertirse en revendedor indirecto](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [Nuevos requisitos de asociados directos del CSP](direct-partner-new-requirements.md)
