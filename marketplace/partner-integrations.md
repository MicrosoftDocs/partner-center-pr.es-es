---
title: Integraciones de asociados de Azure Marketplace
description: Obtenga información sobre Azure Marketplace soluciones que se integran con su entorno de Azure y obtenga un vínculo a las guías de implementación de asociados de Microsoft.
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: 56e72af367cdcb264cc444446c5fcbedcd880451
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276491"
---
# <a name="azure-marketplace-partner-integrations"></a>Integraciones de asociados de Azure Marketplace

Aprenda a integrar soluciones de asociados en su entorno de Azure. En este artículo se proporciona información general de cada solución y vínculos a guías de implementación detalladas. Las soluciones se enumeran en orden alfabético. 

## <a name="apache-kafka-on-confluent-cloud"></a>Apache Kafka en Confluent Cloud

![Nube confluente.](./media/partners/confluent-cloud.png)

Azure permite la integración con Confluent Cloud además de las aplicaciones en la nube. Los clientes confluentes suelen navegar entre la Azure Portal y la nube de Confluent. Por ejemplo, una vez que un usuario adquiere una oferta de Confluent Cloud en Azure Marketplace, se espera que configure una cuenta con Confluent Cloud. Este proceso agrega complejidad y tiempo, y requiere que los usuarios administren la configuración y los recursos entre los dos portales. Para reducir la carga de la administración entre plataformas, Microsoft, en colaboración con Confluent Cloud, ha creado una capa de aprovisionamiento integrada de Azure a Confluent Cloud. La solución está disponible en Azure Marketplace y proporciona una experiencia sin problemas para usar la oferta de nube de Confluent en Azure

La solución usa un proveedor de recursos habilitado en Azure para aprovisionar recursos de Confluent Cloud. Esto permite a los usuarios acceder al streaming de eventos en tiempo real a través de Azure Portal, CLI de Azure y LOS SDK de Azure. Confluent Cloud posee y ejecuta la aplicación SaaS, que incluye entornos, clústeres, temas, claves de API y conectores administrados.

La integración profunda con Confluent Cloud permite las siguientes funcionalidades:

- Aprovisionar un nuevo recurso de la organización de Confluent Cloud desde Azure Portal con una infraestructura totalmente administrada.
- Optimice el inicio de sesión único de Azure a Confluent Cloud con Azure Active Directory; no se necesita ninguna autenticación independiente desde Confluent Cloud Portal.
- Obtenga una facturación unificada de los cargos de consumo de Confluent Cloud a través de la facturación de la suscripción de Azure.
- Administre los recursos de Confluent Cloud desde Azure Portal  y realice un seguimiento de ellos en la página Todos los recursos, junto con los recursos de Azure.

[Guías de implementación de Confluent Cloud](https://docs.confluent.io/current/cloud/marketplace/index.html)

Para problemas relacionados con Confluent en Azure, vaya a [https://support.confluent.io](https://support.confluent.io) . Si es la primera vez que lo hace, restablezca la contraseña antes de iniciar sesión en el portal de soporte técnico de Confluent. Si no tiene una cuenta con Confluent, envíe un correo electrónico a [cloud-support@confluent.io](mailto:cloud-support@confluent.io) .

## <a name="datadog"></a>Datadog

![Logotipo de DataDog.](./media/partners/datadog.png)

Datadog proporciona herramientas de observabilidad y seguridad para que los usuarios de Azure comprendan el estado y el rendimiento de sus aplicaciones en entornos híbridos y de varias nubes. No obstante, la configuración de las integraciones necesarias a menudo requiere utilizar tanto Azure Portal como Datadog. Para simplificar la configuración y la administración de recursos en los portales, Microsoft ha trabajado con Datadog para crear una solución de Datadog integrada en Azure. Disponible a través Azure Marketplace, esta solución proporciona una experiencia sin problemas para que los clientes de Azure usen la solución de supervisión en la nube de Datadog.

Consulte la [Azure Monitor para](/azure/azure-monitor/platform/partners#datadog) obtener más información sobre esta solución y registrarse para obtener la versión preliminar pública.

## <a name="next-steps"></a>Pasos siguientes

- [Azure Marketplace en línea](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn: Creación de una cuenta de Azure](/learn/modules/create-an-azure-account/)
