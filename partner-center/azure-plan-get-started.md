---
title: Comienzo del traslado a un plan de Azure
description: Obtén información sobre cómo usar el plan de pago por uso de Azure, incluidos los primeros pasos, las precauciones de seguridad y cómo empezar.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: 5ad7bd7c99d7caa044877c98aac6dc5e3ce69420
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 09/22/2020
ms.locfileid: "91000579"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Comienzo del uso del plan de pago por uso de Azure

Microsoft ha introducido una nueva experiencia de comercio en el Centro de partners.  Gracias a esta nueva experiencia de comercio, los partners podrán obtener acceso a los servicios de Azure con tarifas de pago por uso para los clientes según lo indicado en el Acuerdo de cliente de Microsoft.

Este plan simplifica la experiencia de compra, ya que puedes tener varias suscripciones de Azure en un solo plan de Azure. Por ello, ya no es necesario enviar un pedido independiente por cada suscripción de Azure. Así pues, gracias a esta nueva experiencia comercial de Azure, hemos establecido un único principio global de precios que permitirá a los partners de CSP ofrecer Azure en función de los precios publicados.

Las necesidades de transformación digital de nuestros clientes requieren nuevas aptitudes de los partners. Muchos clientes buscan partners que proporcionen servicios más allá de las simples transacciones, para que su recorrido en la nube sea más sencillo y puedan obtener ayuda a la hora de usar los servicios de Azure de la forma más eficaz. Los partners de Microsoft desempeñan un papel fundamental en todas las fases del ciclo de vida del cliente. Estos tipos de servicios de partner son continuos e incluyen la supervisión de los servicios de Azure, la administración de directivas y gobernanza, el ajuste de la configuración y sus opciones, el soporte técnico y otros servicios. Asimismo, es necesario que un partner esté completamente familiarizado con el entorno de Azure del cliente y que tenga un gobierno y control continuo y apropiado de los recursos subyacentes que se administran. Los partners de facturación que proporcionan esta administración de operaciones en la nube las 24 horas del día y los 7 días de la semana, podrán recibir el **crédito que haya obtenido el partner por los servicios administrados** para realizar ese trabajo.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Asegúrate de que tus clientes hayan firmado el Acuerdo de cliente de Microsoft

A partir del 1 de octubre de 2019, el Acuerdo de cliente de Microsoft, un acuerdo perpetuo que simplifica y agiliza la experiencia de compra del cliente con un proceso totalmente digital, está disponible. Todos los clientes que quieran aprovechar la nueva experiencia comercial en CSP para Azure deben firmar el Acuerdo de Cliente de Microsoft.

Los partners que quieran realizar transacciones con el nuevo plan de Azure y hacer un nuevo pedido deberán confirmar la aceptación por parte del cliente del Acuerdo de cliente de Microsoft desde la API y el panel del Centro de partners en el entorno de producción.

A partir del 1 de febrero de 2020, se quitará el Contrato de Microsoft Cloud existente del programa de CSP. A partir de ese momento, se requerirá la confirmación (atestación) del partner de la aceptación por parte del cliente del nuevo Contrato de cliente de Microsoft para las demás ofertas, como Microsoft 365, Dynamics 365 y Azure. Los partners en CSP no podrán realizar un nuevo pedido para el cliente sin la atestación del Acuerdo de cliente de Microsoft.

Para obtener más detalles, consulta [Confirmar la aceptación del cliente del Acuerdo de Cliente de Microsoft](confirm-customer-agreement.md).

## <a name="security-and-access-control-practices"></a>Prácticas de seguridad y control de acceso

Para ayudar a proteger a los partners y clientes, presentamos un conjunto de requisitos de seguridad obligatorios para los asesores, proveedores de panel de control y asociados que participen en el programa Proveedor de soluciones en la nube.

Los partners que no implementen los requisitos de seguridad obligatorios no podrán realizar transacciones en el programa Proveedor de soluciones en la nube ni administrar los inquilinos del cliente que aprovechen los derechos de administrador delegado, una vez que se apliquen estos requisitos. Estamos en el proceso de establecer una fecha de aplicación técnica de los requisitos y se la notificaremos a los partners con información detallada.

## <a name="actions-to-take-to-implement-mfa"></a>Acciones que se deben llevar a cabo para implementar MFA

Dada la naturaleza de los partners, que tienen privilegios elevados, necesitamos asegurarnos de que cada usuario tenga que usar la MFA en todas y cada una de las autenticaciones. Esto se puede realizar de cualquiera de estas maneras:

- Mediante la implementación de Azure AD Premium y asegurándote de que se aplica la autenticación multifactor (MFA) a todos los usuarios.
- Implementar los [valores predeterminados de seguridad Azure AD](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Mediante la implementación de una solución de terceros y asegurándose de que se aplica MFA a todos los usuarios.

A partir del 1 de agosto de 2019, todos los partners tienen la obligación de aplicar la autenticación multifactor a todos los usuarios, incluidas las cuentas de servicio, en su inquilino de partner. Puedes encontrar información detallada sobre estos requisitos de seguridad en los [requisitos de seguridad para partners](partner-security-requirements.md).

Microsoft recomienda a los partners que usen el mecanismo RBAC diligentemente, siguiendo los procedimientos recomendados habilitadas a través de los [recursos de Azure Active Directory Privileged Identity Management](/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="read-more-about-the-azure-plan"></a>Obtén más información sobre el plan de Azure.

- [Compra del plan de Azure](purchase-azure-plan.md)

- [Comparar ofertas de Azure](compare-azure-offers.md)

- [Créditos obtenidos del partner: introducción](partner-earned-credit.md)

- Los cálculos del crédito que ha obtenido el partner (PEC) y los roles y permisos que son aptos para obtener créditos que haya obtenido ese partner están disponibles en la lista de precios del panel del Centro de partners (se requiere inicio de sesión).

## <a name="next-steps"></a>Pasos siguientes 

- [Cómo se determina el crédito que hay ganado el partner: detalles](partner-earned-credit-explanation.md)
- [Lista de precios del plan Azure explicada](azure-plan-price-list.md)
- [Transición del cliente al plan de Azure](azure-plan-transition.md)
- [Administrar suscripciones y recursos en el plan de Azure](azure-plan-manage.md)
- [Lista completa de países y regiones donde el plan Azure está disponible](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)