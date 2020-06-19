---
title: Solicitar un crédito de contrato de nivel de servicio de Microsoft
ms.topic: article
ms.date: 04/28/2020
description: Obtenga información sobre las ventajas, restricciones y procedimientos para solicitar un crédito de contrato de nivel de servicio (SLA) de Microsoft si los clientes experimentan una interrupción del servicio.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 27a444bc5f923b1d2ad18bfe47cf70b365751e42
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/18/2020
ms.locfileid: "84992014"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Cómo y cuándo solicitar un crédito de contrato de nivel de servicio (SLA) de Microsoft

Puede solicitar **créditos de contrato de nivel de servicio (SLA)** de Microsoft si un servicio que está proporcionando para sus clientes tiene una interrupción.

## <a name="sla-credit-calculation"></a>Cálculo del contrato de nivel de servicio

Los créditos de contrato de nivel de servicio de Microsoft se determinan en función de los servicios afectados. Por ejemplo, si el cliente tiene un conjunto de Office 365 pero solo se ha producido una interrupción de SharePoint, el crédito del contrato de nivel de servicio se aprueba solo para SharePoint y no para el plan completo del cliente.

*Los créditos se prorratean en función del servicio afectado y de la duración de la interrupción.* Para ver los tipos de escenarios que reúnen los créditos del contrato de nivel de servicio, consulte el [documento de SLA consolidado de servicios en línea](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37). Esta información se aplica también a los servicios que se venden a través del programa proveedor de soluciones en la nube.

## <a name="request-an-sla-credit"></a>Solicitar un crédito de contrato de nivel de servicio

*El asociado del proveedor de soluciones en la nube (CSP) debe enviar la demanda y toda la información necesaria hasta el final del mes natural siguiente al mes en el que se produjo el incidente.* Por ejemplo, si el incidente se produjo el 15 de febrero, Microsoft debe recibir la demanda y toda la información necesaria antes del 31 de marzo. Los clientes finales y los distribuidores indirectos no pueden enviar notificaciones de crédito del contrato de nivel de servicio. el proveedor indirecto o el asociado directo de factura debe enviar notificaciones en su nombre.

### <a name="required-information"></a>Información necesaria

Antes de [enviar una solicitud de crédito del contrato](#submit-sla-credit-request) de nivel de servicio a Microsoft, debe recopilar la siguiente información para incluirla en la incidencia de soporte técnico:

- GUID del inquilino del cliente
- ¿El [identificador del incidente de interrupción](#outage-incident-identifier)?
- ¿Las suscripciones afectadas se han adquirido a través de CSP? (*sí* o *no*)

#### <a name="outage-incident-identifier"></a>Identificador de incidente de interrupción

Puede encontrar el identificador del incidente de interrupción en la página **Service Health** del centro de administración de Microsoft 365. El **identificador del incidente de interrupción** es un número precedido por una abreviatura de dos letras que indica el servicio afectado (por ejemplo, *EX25194* para una interrupción de Exchange Online). En la tabla siguiente se describen las abreviaturas de servicio comunes:

| Abreviatura de dos letras | Servicio de Microsoft |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Protección de Exchange Online |
| SB | Skype empresarial online (anteriormente, Lync Online) |
| SO | Suscripción a Office |
| PB | Power BI para Office 365 |
| SP | SharePoint Online |
| Cherokee | Yammer Enterprise |
| MO | Error del portal |

### <a name="submit-sla-credit-request"></a>Enviar solicitud de crédito del contrato de nivel de servicio

Para enviar la solicitud de crédito del contrato de nivel de servicio a Microsoft a través del panel del centro de Partners:

1. Inicia sesión en el panel del Centro de partners.
2. En el menú de la izquierda, elija **solicitudes de servicio**y, a continuación, seleccione **solicitudes de soporte técnico de asociados**.
3. En la página **solicitud de socio comercial** , elija **nueva solicitud**.
4. En la página **iniciar la solicitud** , busque la sección **CSP-clientes, pedidos y suscripciones**. En esta sección, elija **seleccionar un tipo de problema**y, a continuación, seleccione **solicitudes de crédito de servicios de cliente**.
5. En la página **soluciones recomendadas** , en **¿necesita más ayuda?**, elija **sí**.
6. En la página **detalles** , rellene la sección **detalles del problema** . En el cuadro de texto **detalles** , asegúrese de escribir la [información necesaria](#required-information) que recopiló anteriormente.
7. Elija **submit (enviar** ) para enviar la solicitud de crédito del contrato de nivel de servicio.
