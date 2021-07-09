---
title: Solicitar un crédito de contrato de nivel de servicio de Microsoft
ms.topic: article
ms.date: 03/31/2021
description: Conozca las ventajas, restricciones y procedimientos para solicitar un crédito de contrato de nivel de servicio (SLA) a Microsoft si los clientes experimentan una interrupción del servicio.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 3a0bb85143efe3d4135b56985b9a04e2dbe5e4cc
ms.sourcegitcommit: 57442bbbef15a70bd9a042642140cbf2c8608b09
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/09/2021
ms.locfileid: "113519438"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Cómo y cuándo solicitar un crédito de contrato de nivel de servicio (SLA) a Microsoft

**Roles adecuados:** agente de administración | Administrador global

Puede solicitar créditos de contrato de nivel de servicio **(SLA)** a Microsoft si un servicio que está proporcionando a los clientes tiene una interrupción.

## <a name="sla-credit-calculation"></a>Cálculo del crédito del Acuerdo de Nivel de Servicio

Los créditos del Acuerdo de Nivel de Servicio de Microsoft se determinan en función de los servicios que se han afectado. Por ejemplo, si el cliente tiene un conjunto de Office 365 pero solo ha experimentado una interrupción SharePoint, el crédito del Acuerdo de Nivel de Servicio solo se aprueba para SharePoint y no para todo el plan del cliente.

*Los créditos se prorratea según el servicio afectado y la duración de la interrupción.* Para ver los tipos de escenarios que reúnen los requisitos para los créditos del Acuerdo de Nivel de Servicio, consulte el documento de Acuerdo de Nivel de [Servicio consolidado de Online Services](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37). Esta información también se aplica a los servicios vendidos a Proveedor de soluciones en la nube programa (CSP).


## <a name="request-an-sla-credit"></a>Solicitud de un crédito del Acuerdo de Nivel de Servicio

*El asociado de CSP debe enviar la notificación y toda la información necesaria al final del mes natural siguiente al mes en el que se produjo el incidente.* Por ejemplo, si el incidente se produjo el 15 de febrero, Microsoft debe recibir la notificación y toda la información necesaria antes del 31 de marzo. Los clientes finales y revendedores indirectos no pueden enviar notificaciones de crédito del Acuerdo de Nivel de Servicio. el proveedor indirecto o el asociado de facturación directa deben enviar notificaciones en su nombre.

> [!NOTE]
> Por lo general, los incidentes de asesoramiento no son aptos para créditos del Acuerdo de Nivel de Servicio. Un incidente publicado en Service Health Dashboard indica que  un inquilino puede estar afectado y representa la mejor información que Microsoft tiene en el momento de la publicación. Los datos de la página de mantenimiento representan la disponibilidad general de un servicio. El impacto, la mitigación y la resolución de un servicio individual pueden variar. Puede revisar la última publicación del incidente y la revisión posterior al incidente para obtener más detalles. Para [más información, consulte Comprobación Microsoft 365 estado del](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) servicio.

### <a name="required-information"></a>Información necesaria

El nombre del cliente, el identificador de inquilino, el número de vale de partner y la marca de fecha y hora creada por el vale no son suficientes para que se procese una notificación.

Antes de enviar una solicitud de crédito  del [Acuerdo](#submit-sla-credit-request) de Nivel de Servicio a Microsoft, debe recopilar toda la información siguiente para incluirla en la vale de soporte técnico:

- GUID del inquilino del cliente
- El identificador [de incidente de interrupción](#outage-incident-identifier)?
- Evidencia de que el cliente se ha afectado por la interrupción y ha solicitado un crédito del Acuerdo de Nivel de Servicio.
- ¿Se compraron las suscripciones afectadas a través de CSP? (*sí* o *no*)

#### <a name="evidence-that-proves-customer-impact"></a>Evidencia que demuestra el impacto en el cliente

- Información sobre el tiempo y la duración del tiempo de inactividad
- Número y ubicación de los usuarios afectados (si procede)
- Descripciones de los intentos de resolver el incidente en el momento de la aparición
- Un correo electrónico del cliente afectado que solicita soporte técnico y, posteriormente, crédito
- El número de incidencia de soporte técnico y los detalles del contacto del cliente con respecto a la resolución del impacto en el servicio


#### <a name="outage-incident-identifier"></a>Identificador de incidente de interrupción

Puede encontrar el identificador del incidente de interrupción en la **Service Health** del Centro de administración de Microsoft 365. El **identificador de incidente de** interrupción es un número precedido por una abreviatura de dos letras que indica el servicio afectado (por ejemplo, *EX25194* para una interrupción Exchange Online de servicio). En la tabla siguiente se describen las abreviaturas de servicio comunes:

| Abreviatura de dos letras | Servicio de Microsoft |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online Protection |
| SB | Skype Empresarial Online (anteriormente Lync Online) |
| SO | Suscripción a Office |
| PB | Power BI para Office 365 |
| SP | SharePoint Online |
| YA | Yammer Enterprise |
| MO | Error del portal |

### <a name="submit-sla-credit-request"></a>Envío de una solicitud de crédito del Acuerdo de Nivel de Servicio

Para enviar la solicitud de crédito del Acuerdo de Nivel de Servicio a Microsoft a través Centro de partners panel:

1. Inicie sesión en el panel del Centro de partners.
2. En el menú de la izquierda, elija **Solicitudes de servicio y,** a continuación, **seleccione Solicitudes de soporte técnico para asociados.**
3. En la **página Solicitud de asociado,** elija **Nueva solicitud.**
4. En la **página Iniciar la solicitud,** busque la sección **CSP : clientes, pedidos y suscripciones.** En esta sección, elija **Seleccionar un tipo de problema y,** a continuación, seleccione Solicitudes de crédito de servicios al **cliente.**
5. En la **página Soluciones recomendadas,** en **¿Necesita más ayuda?**, elija **Sí.**
6. En la **página Detalles,** rellene la sección **Detalles del** problema. En el **cuadro de** texto Detalles, asegúrese de escribir la [información necesaria](#required-information) que ha recopilado anteriormente.
7. Elija **Enviar para** enviar la solicitud de crédito del Acuerdo de Nivel de Servicio.

## <a name="next-steps"></a>Pasos siguientes

- [Informe de problemas en nombre del cliente](report-problems-on-behalf-of-a-customer.md)
