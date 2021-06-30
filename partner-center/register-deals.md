---
title: Registrar las ofertas
ms.topic: article
ms.date: 06/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Al registrar una oferta que ha ganado en Centro de partners, ayuda a Microsoft a proporcionarle más oportunidades en el futuro.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: medium
ms.openlocfilehash: eaa9bb6f8e57033669ef584e7c52c0d050a532e0
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080672"
---
# <a name="register-deals-youve-won-in-partner-center"></a>Registre las ofertas que ha ganado en Centro de partners

**Roles adecuados**: Administrador global

Para registrar las ofertas que has ganado en el Centro de partners, puedes proporcionar información adicional sobre el contrato. Esta información nos ayudará a proporcionarte más oportunidades en el futuro.

Hay dos rutas de acceso que conducen al registro de la oferta:

- Ha creado una nueva oferta en la sección **Oportunidades** de venta en colaboración y su oferta cumple los criterios para el registro de la oferta.
- Quiere notificar una oferta cerrada de ISV Connect, que no se ha vendido en colaboración con Microsoft.

## <a name="register-a-deal-originating-from-a-co-sell-opportunity"></a>Registro de una oferta que se origina en una oportunidad de venta en colaboración

Si desea registrar una oferta que se origina en una oportunidad de venta compartida, debe cumplir los siguientes requisitos de idoneidad:

- El tipo de oferta es la venta en colaboración o dirigida por asociados (ha elegido permitir que los vendedores de Microsoft puedan ver esta oferta).
- Hay al menos una solución apta para incentivos en el contrato. Una solución es apta para incentivos si contiene al menos una de las siguientes etiquetas:
  - Venta co-venta de IP de Azure
  - Business Applications Premium
  - Business Applications Estándar
- El estado de la oferta es "Won".
- Si el tipo de oferta es de venta en colaboración, Microsoft debe haber aceptado la invitación o marcado la oferta como ganada. Para ver el estado de Microsoft, consulte la tarjeta Microsoft debajo de los detalles de la oferta.

Si ha cumplido los requisitos de idoneidad, se le pedirá automáticamente  que registre su oferta con un botón Registrar ahora que se muestra en la barra de progreso de la oferta:

:::image type="content" source="images/register-deals.png" alt-text="Captura de pantalla que muestra la barra de progreso de la oferta.":::

> [!NOTE]
> Si el **elemento Registro de** la oferta no aparece en la barra de progreso de la oferta, la oferta no cumple todos los requisitos para el registro de la oferta.

Después de **hacer clic** en Registrar ahora, se le redirigirá a la página Registro de la oferta y se le pedirá que rellene un formulario con la información rellenada previamente para el cliente y la solución. Rellene el formulario con las instrucciones siguientes y haga clic **en Registrar.**

Tras el registro, se crearán uno o dos registros de registro de la oferta en función de la solución.

- Si la solución es apta para ISV Connect, se creará un registro de registro de la oferta de ISV Connect. Este registro de registro de la oferta se usará para la facturación.
- Si la solución es apta para los incentivos de venta co-venta de IP, se creará un registro de registro de la oferta de venta co-venta de IP. El equipo de revisión de la oferta de venta co-venta revisará y aprobará o rechazará este registro de registro de la oferta.

## <a name="report-a-closed-isv-connect-deal"></a>Notificar una oferta de ISV Connect cerrada

Para notificar una oferta de ISV Connect cerrada, vaya a la pestaña **Registro de** la oferta y haga clic en + Report **closed ISV Connect deal (+ Report closed ISV Connect deal**). Rellene los campos obligatorios y haga clic **en Registrar.** Este registro de registro de la oferta se usará para la facturación.

## <a name="fill-out-the-deal-registration-form"></a>Rellene el formulario de registro de la oferta.

> [!NOTE]
> Puede filtrar las ofertas por nombre de cliente, estado y tipo de oferta. Para ello, haga clic en el **botón Filtrar** situado en la parte superior de la página Registro de la oferta.

Tanto si ha llegado a tratar el registro de una oportunidad de venta en colaboración como si está informando de una oferta cerrada de ISV Connect, que no se ha vendido con Microsoft, se le pedirá que rellene los siguientes campos en el formulario de registro de la oferta.

- **Detalles del** cliente: escriba el **nombre de la compañía** del cliente y seleccione su país o **región.** A continuación, escribe su **Ciudad** y su **Estado o provincia**.
- **Solución:** seleccione la solución que se usará para la oferta. Si no ves la solución adecuada en la lista, ponte en contacto con el soporte técnico.
- **Tipo de contrato:** especifique si esta oferta es **un contrato** nuevo o **una renovación** de un contrato anterior.
- **Valor total del contrato:** el valor total esperado para la interacción. Este valor debe incluir todos los precios de software y servicio, pero no los costos de hardware. Asegúrate de seleccionar la moneda adecuada.
- **Valor de** la solución: el valor total de la solución en la nube que se usará para la oferta. Asegúrate de incluir todos los costos asociados con las tarifas de software y mantenimiento, pero no incluyas artículos reembolsables, tarifas de personalización no recurrentes ni cuotas de licencias de CSP directamente asociadas que abone Microsoft.
- **¿Se implementará la solución en Azure? Si no es así, elija Otro:** seleccione **Azure** u **Otros.**
- **¿Se ejecutará el consumo de la solución en** el inquilino del asociado o en el inquilino del **cliente?**: seleccione el inquilino **customer** o partner tenant .
- **Fecha de inicio del** contrato: la fecha en que se iniciará el contrato. Para las ofertas de pago por uso (PAYG), use la fecha de la primera factura. Por diseño, Centro de partners no le permitirá especificar una fecha de inicio anterior a la fecha de firma del contrato. Esto puede afectar a algunas ofertas, como las implementaciones de IP que se inician antes de la fecha de inicio de sesión. Para especificar correctamente estas ofertas, use la  fecha de firma del contrato para los campos fecha de inicio y fecha de inicio al enviar. (El contrato debe especificar explícitamente la duración de la oferta para que ACV se pueda calcular correctamente).
- **Fecha de finalización del** contrato: si el contrato finalizará en una fecha específica, seleccione **Tiene una fecha de finalización** y proporcione esa fecha. Si el contrato no tiene una fecha de finalización específica, seleccione **Perpetuos.** Para las ofertas de pago por uso (PAYG), use la fecha de la última factura o la más reciente.
- **Fecha de firma del** contrato: la fecha en la que la organización y el cliente firmaron el contrato final. Para las ofertas de pago por uso (PAYG), use la fecha de la primera factura.
- **Contacto de** registro: **el** **nombre,** los  **apellidos,** el número de teléfono y el correo electrónico de una persona de la organización con la que podemos ponerse en contacto si necesitamos más detalles sobre cualquiera de los datos que se proporcionan aquí.

Cuando haya completado todas las secciones de la página, haga clic en **Registrar.**

- Si la oferta es una oferta de ISV Connect, observará que el estado de la oferta es "Enviado, Completado". No es necesario realizar ninguna otra acción en este registro de la oferta. Este registro se usará para la facturación.
- Si la oferta es una oferta de venta en colaboración de IP, observará que el estado de la oferta es "Enviado". El equipo de revisión de la oferta de venta co-venta de Microsoft revisará la información que proporcionó en este registro de la oferta. El equipo de revisión le solicitará más acciones si es necesario, o aprobará o rechazará la oferta directamente.
- Si va a registrar una oferta que se origina en una oportunidad de venta en colaboración y ve que se han creado dos registros de registro de la oferta, significa que la solución de su oferta es apta tanto para ISV Connect como para la venta co-sell de IP. El registro de ISV Connect se va a usar para la facturación. El equipo de validación de la oferta de venta co-venta revisará el registro de venta co-venta de IP.

