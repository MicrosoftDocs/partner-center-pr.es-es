---
title: Roles, permisos para el crédito obtenido por el socio comercial
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información acerca de los roles y los permisos de los asociados para poder ganar créditos obtenidos por asociados (PEC). Estos difieren de los roles para trabajar en el centro de Partners.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f48774cb830ceb575a84177efb57431afdcb9b25
ms.sourcegitcommit: 5fc28f6f81eaebb84e1faa71848afb504e181f37
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/11/2020
ms.locfileid: "90011745"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>Roles y permisos coincidentes para ganar el crédito obtenido por el socio

Los roles siguientes se asignan a los niveles de permisos que determinan si un asociado es válido para créditos obtenidos por el socio.

>[!Important]
>Estos roles y permisos no son los mismos que los roles y permisos que un usuario necesita para trabajar en el centro de Partners.

|**Rol**   |**Descripción**   |**PEC válido**   |
|-----------------|:------------------|:--------------|
|Propietario  |Puede administrar todo, incluido el acceso a los recursos.|Sí|
|Colaborador |Administra todo, excepto el acceso a los recursos.|Sí|
|Lector|Puede ver todo, pero no realizar cambios.|No|
|ACRDelete|Eliminar artefacto|Sí|
|ACRImageSigner|Firmante de imagen de ACR|Sí|
|ACRPull|extracción de ACR|Sí|
|AcrPush|inserción de ACR|Sí|
|AcrQuarantineReader|Lector de datos de cuarentena de ACR|No|
|AcrQuarantineWriter| Escritura de datos de cuarentena de ACR|Sí|
|Colaborador de servicio de administración de API|Puede administrar servicios y las API.|Sí|
|Rol del operador del servicio API Management|Puede administrar el servicio, pero no las API.|Sí|
|Rol de lector del servicio API Management|Acceso de solo lectura al servicio y las API.|No|
|Colaborador de componentes de Application Insights|Administra componentes de Application Insights|Sí|
|Depurador de instantáneas de Application Insights|Concede permiso al usuario para ver y descargar las instantáneas de depuración que se recopilan con Snapshot Debugger de Application Insights. Tenga en cuenta que estos permisos no se incluyen en los roles Propietario ni Colaborador.|Sí|
Operador de trabajos de Automation | Permite crear y administrar trabajos con los runbooks de Automation. | Sí | 
Operador de Automation | Los operadores de automatización pueden iniciar, detener, suspender y reanudar trabajos. | Sí | 
Operador de runbooks de Automation | Permite leer las propiedades de runbook para poder crear trabajos del runbook. | Sí | 
Colaborador de Avere | Puede crear y administrar un clúster de Avere vFXT. | Sí | 
Operador de Avere | Lo usa el clúster de Avere vFXT para su administración. | Sí | 
Propietario de los datos de Azure Event Hubs | Concede acceso total a los recursos de Azure Event Hubs. | Sí | 
Receptor de datos de Azure Event Hubs | Concede acceso de recepción a los recursos de Azure Event Hubs. | Sí | 
Emisor de datos de Azure Event Hubs | Concede acceso de emisión a los recursos de Azure Event Hubs. | Sí | 
Rol de administrador de clúster de Azure Kubernetes Service | Enumerar la acción de credenciales administrativas del clúster. | Sí | 
Rol de usuario de clúster de Azure Kubernetes Service | Enumerar la acción de credenciales de usuario del clúster. | Sí | 
Azure Maps Data Reader (versión preliminar) | Concede acceso de lectura a los datos de los mapas de una cuenta de Azure Maps. | No | 
Propietario de los datos de Azure Service Bus | Concede acceso total a los recursos de Azure Service Bus. | Sí | 
Receptor de datos de Azure Service Bus | Concede acceso de recepción a los recursos de Azure Service Bus. | Sí | 
Emisor de datos de Azure Service Bus | Concede acceso de emisión a los recursos de Azure Service Bus. | Sí | 
Propietario del registro de Azure Stack | Permite administrar los registros de Azure Stack. | Sí | 
Colaborador de copias de seguridad | Permite administrar el servicio de copias de seguridad, pero no puede crear almacenes ni conceder acceso a otros usuarios | Sí | 
Operador de copias de seguridad | Permite administrar los servicios de copias de seguridad, excepto la eliminación de copias de seguridad, la creación de almacenes y la concesión de acceso a otros usuarios | Sí | 
Lector de copias de seguridad | Puede ver servicios de copia de seguridad, pero no puede realizar cambios. | No | 
Lector de facturación | Permite acceso de lectura a los datos de facturación. | No | 
Colaborador de BizTalk | Permite administrar los servicios de BizTalk, pero no acceder a ellos. | Sí | 
Acceso al nodo de miembro de la cadena de bloques (versión preliminar) | Permite acceder a los nodos de miembro de la cadena de bloques. | Sí | 
Colaborador de plano técnico | Puede administrar las definiciones del plano técnico, pero no asignarlas. | Sí | 
Operador del plano técnico | Puede asignar los planos técnicos publicados existentes, pero no puede crear nuevos. Nota: Esto solo funciona si la asignación se realiza con una identidad administrada asignada por el usuario. | Sí | 
Colaborador de punto de conexión de CDN | Puede administrar puntos de conexión de CDN, pero no conceder acceso a otros usuarios. | Sí | 
Lector de punto de conexión de CDN | Puede ver puntos de conexión de CDN, pero no hacer cambios. | No | 
Colaborador de perfil de CDN | Puede administrar perfiles de CDN y sus puntos de conexión, pero no conceder acceso a otros usuarios. | Sí | 
Lector de perfil de CDN | Puede ver perfiles de CDN y sus puntos de conexión, pero no hacer cambios. | No | 
Colaborador de la red clásica | Permite administrar las redes clásicas, pero no acceder a ellas. | Sí | 
Colaborador de cuentas de almacenamiento clásico | Permite administrar cuentas de almacenamiento clásicas, pero no acceder a ellas. | Sí | 
Rol de servicio de operador de claves de cuentas de almacenamiento clásicas | Los operadores de claves de cuentas de almacenamiento clásicas pueden enumerar y regenerar claves en cuentas de almacenamiento clásicas | Sí | 
Colaborador de la máquina virtual clásica | Permite administrar máquinas virtuales clásicas, pero no acceder a ellas, ni tampoco a la red virtual ni a la cuenta de almacenamiento a las que están conectadas. | Sí | 
Colaborador de Cognitive Services | Le permite crear, leer, actualizar, eliminar y administrar las claves de Cognitive Services. | Sí | 
Lector de datos de Cognitive Services (versión preliminar) | Permite leer los datos de Cognitive Services. | No | 
Usuario de Cognitive Services | Le permite leer y mostrar las claves de Cognitive Services. | No | 
Rol de lector de cuentas de Cosmos DB | Puede leer los datos de cuentas de Azure Cosmos DB. Vea Colaborador de cuenta de DocumentDB para administrar cuentas de Azure Cosmos DB. | No | 
Operador de Cosmos DB | Permite administrar las cuentas de Azure Cosmos DB, pero no acceder a los datos que contienen. Evita el acceso a las claves de cuenta y a las cadenas de conexión. | Sí | 
CosmosBackupOperator | Puede enviar una solicitud de restauración para una base de datos de Cosmos DB o un contenedor de una cuenta | Sí | 
Colaborador de Cost Management | Puede ver los costos y administrar la configuración de estos (por ejemplo, presupuestos, exportaciones) | Sí | 
Lector de Cost Management | Puede ver los datos de costo y la configuración (por ejemplo, presupuestos, exportaciones) | No | 
Colaborador de Data Box | Permite administrarlo todo en el servicio Data Box, excepto dar acceso a otros usuarios. | Sí | 
Lector de Data Box | Permite administrar el servicio Data Box excepto la creación o edición de detalles de pedido y dar acceso a otros usuarios. | No | 
Colaborador de Factoría de datos | Crea y administra factorías de datos, así como recursos secundarios dentro de ellas. | Sí | 
Desarrollador de Data Lake Analytics | Le permite enviar, supervisar y administrar sus propios trabajos, pero no crear ni eliminar cuentas de Data Lake Analytics. | Sí | 
Purgador de datos | Puede purgar datos de análisis. | Sí | 
Usuario de DevTest Labs | Permite conectarse a sus máquinas virtuales, así como iniciarlas, reiniciarlas y apagarlas, en su instancia de Azure DevTest Labs. | Sí | 
Colaborador de zona DNS | Permite administrar zonas y conjuntos de registros DNS en Azure DNS, pero no controlar los usuarios que tienen acceso. | Sí | 
Colaborador de cuenta de DocumentDB | Puede administrar cuentas de Azure Cosmos DB. Azure Cosmos DB se llamaba anteriormente DocumentDB. | Sí | 
Colaborador de EventGrid EventSubscription | Permite administrar las operaciones de suscripción de eventos de EventGrid. | Sí | 
Lector de EventGrid EventSubscription | Permite leer las suscripciones de eventos de EventGrid. | No | 
Operador de clústeres de HDInsight | Permite leer y modificar las configuraciones de clúster de HDInsight. | Sí | 
Colaborador de Domain Services para HDInsight | Puede leer, crear, modificar y eliminar operaciones relacionadas con Domain Services para HDInsight Enterprise Security Package | Sí | 
Colaborador de la cuenta de Sistemas inteligentes | Permite administrar las cuentas de Intelligent Systems, pero no acceder a ellas. | Sí | 
Colaborador de almacén de claves | Le permite administrar almacenes de claves, pero no acceder a ellos. | Sí | 
Creador de laboratorio | Le permite crear, administrar y eliminar los laboratorios administrados en sus cuentas de Azure Lab. | Sí | 
Colaborador de Log Analytics | Un colaborador de Log Analytics puede leer todos los datos de supervisión y editar la configuración de supervisión. La edición de la configuración de supervisión incluye la posibilidad de añadir la extensión de máquina virtual a las máquinas virtuales, leer las claves de las cuentas de almacenamiento para poder configurar la recopilación de registros de Azure Storage, crear y configurar cuentas de Automation, añadir soluciones y configurar Azure Diagnostics en todos los recursos de Azure. | Sí | 
Lector de Log Analytics | Un lector de Log Analytics puede ver y buscar todos los datos de supervisión, así como consultar la configuración de supervisión, incluida la de Azure Diagnostics en todos los recursos de Azure. | No | 
Colaborador de aplicación lógica | Le permite administrar aplicaciones lógicas, pero no cambiar el acceso a ellas. | Sí | 
Operador de aplicación lógica | Le permite leer, habilitar y deshabilitar aplicaciones lógicas, pero no permite editarlas ni actualizarlas. | Sí | 
Rol de operador de aplicación administrada | Permite leer y realizar acciones en los recursos de aplicación administrada. | Sí | 
Lector de aplicaciones administradas | Le permite leer los recursos de una aplicación administrada y solicitar acceso JIT. | No | 
Colaborador de identidad administrada | Le permite crear, leer, actualizar y eliminar identidades asignadas por el usuario. | Sí | 
Operador de identidad administrada | Le permite leer y asignar identidades asignadas por el usuario. | Sí | 
Colaborador de grupo de administración | Rol de colaborador de grupo de administración | Sí | 
Lector de grupo de administración | Rol de lector de grupo de administración | No | 
Colaborador de supervisión | Puede leer todos los datos de supervisión y editar la configuración de supervisión. Consulte también Introducción a roles, permisos y seguridad con Azure Monitor. | Sí | 
Supervisión del publicador de métricas | Permite publicar las métricas de los recursos de Azure. | Sí | 
Lector de supervisión | Puede leer todos los datos de supervisión (métricas, registros, etc.). Consulte también Introducción a roles, permisos y seguridad con Azure Monitor. | No | 
Colaborador de la red | Permite administrar redes, pero no acceder a ellas. | Sí | 
Colaborador de la cuenta de NewRelic APM | Le permite administrar las aplicaciones y cuentas de Application Performance Management de New Relic, pero no acceder a ellas. | Sí | 
Lector y acceso a los datos | Permite ver todo el contenido, pero no eliminar ni crear una cuenta de almacenamiento ni un recurso incluido. También permitirá el acceso de lectura o escritura para todos los datos incluidos en una cuenta de almacenamiento a través del acceso a las claves de la cuenta de almacenamiento. | Sí | 
Colaborador de la memoria caché de Redis | Permite administrar cachés de Redis, pero no acceder a ellas. | Sí | 
Colaborador de la directiva de recursos (versión preliminar) | (Versión preliminar) Los usuarios repuestos de EA, con derechos para crear o modificar la directiva de recursos, crean incidencias de soporte técnico y leen los recursos o la jerarquía. | Sí | 
Colaborador de colecciones de trabajos de Scheduler | Permite administrar colecciones de trabajos de Scheduler, pero no acceder a ellas. | Sí | 
Colaborador del servicio de búsqueda | Permite administrar los servicios de Búsqueda, pero no acceder a ellos. | Sí | 
Administrador de seguridad | Solo en Security Center: puede ver las directivas de seguridad, ver los estados de seguridad, editar las directivas de seguridad, ver alertas y recomendaciones, y descartar alertas y recomendaciones | Sí | 
Administrador de seguridad (heredado) | Se trata de un rol heredado. En su lugar, use el Administrador de seguridad. | Sí | 
Lector de seguridad | Solo en Security Center: puede ver las recomendaciones y alertas, ver las directivas de seguridad y ver los estados de seguridad, pero no puede realizar cambios | No | 
Colaborador de Site Recovery | Permite administrar el servicio Site Recovery, excepto la creación de almacenes y la asignación de roles. | Sí | 
Operador de Site Recovery | Permite realizar una conmutación por error o una conmutación por recuperación, pero no otras operaciones de administración de Site Recovery. | Sí | 
Lector de Site Recovery | Permite visualizar el estado de Site Recovery, pero no realizar otras operaciones de administración. | No | 
Colaborador de la cuenta de Spatial Anchors | Permite administrar los anclajes espaciales en su cuenta, pero no eliminarlos. | Sí | 
Propietario de la cuenta de Spatial Anchors | Permite administrar los anclajes espaciales en su cuenta y eliminarlos. | Sí | 
Lector de la cuenta de Spatial Anchors | Permite encontrar y leer propiedades de los anclajes espaciales en la cuenta. | No | 
Colaborador de Base de datos de SQL | Permite administrar las bases de datos de SQL, pero no acceder a ellas. Además, no puede administrar sus directivas relacionadas con la seguridad ni los servidores SQL primarios. | Sí | 
Colaborador de Instancia administrada de SQL | Permite administrar las instancias administradas de SQL y requiere configuración de red, pero no puede conceder acceso a otros usuarios. | Sí | 
Administrador de seguridad SQL | Permite administrar las directivas relacionadas con seguridad de bases de datos y servidores SQL, pero no acceder a ellas. | Sí | 
Colaborador de SQL Server | Permite administrar bases de datos y servidores SQL, pero no acceder a ellos, ni a sus directivas relacionadas con la seguridad. | Sí | 
Colaborador de la cuenta de almacenamiento | Permite la administración de cuentas de almacenamiento. Proporciona acceso a la clave de cuenta, que puede usarse para tener acceso a datos a través de la autorización de clave compartida. | Sí | 
Rol de servicio de operador de claves de cuentas de almacenamiento | Permite enumerar y regenerar claves de acceso de la cuenta de almacenamiento. | Sí | 
Colaborador de datos de blobs de almacenamiento | Lee, escribe y elimina blobs y contenedores de Azure Storage. Para aprender qué acciones son necesarias para una operación de datos determinada, consulte Permissions for calling blob and queue data operations (Permisos para llamar a operaciones de datos de blob y de cola). | Sí | 
Propietario de datos de blobs de almacenamiento | Proporciona acceso total a los contenedores de blobs y los datos de Azure Storage, incluida la asignación de control de acceso POSIX. Para aprender qué acciones son necesarias para una operación de datos determinada, consulte Permissions for calling blob and queue data operations (Permisos para llamar a operaciones de datos de blob y de cola). | Sí | 
Lector de datos de blobs de almacenamiento | Lee y enumera blobs y contenedores de Azure Storage. Para aprender qué acciones son necesarias para una operación de datos determinada, consulte Permissions for calling blob and queue data operations (Permisos para llamar a operaciones de datos de blob y de cola). | No | 
Delegador de Blob Storage | Obtiene una clave de delegación de usuarios, que se puede usar a continuación para crear una firma de acceso compartido para un contenedor o un blob firmado con credenciales de Azure AD. Para más información, vea Creación de SAS de delegación de usuarios. | Sí | 
Colaborador de recursos compartidos de SMB de datos de archivos de Storage | Permite el acceso de lectura, escritura y eliminación a los recursos compartidos de archivos de Azure Storage mediante SMB. | Sí | 
Colaborador elevado de recursos compartidos de SMB de datos de archivos de Storage | Permite el acceso de lectura, escritura, eliminación y modificación de permisos NTFS a los recursos compartidos de archivos de Azure Storage mediante SMB. | Sí | 
Lector de recursos compartidos de SMB de datos de archivos de Storage | Permite el acceso de lectura a los recursos compartidos de archivos de Azure mediante SMB. | No | 
Colaborador de datos de la cola de Storage | Lee, escribe y elimina los mensajes de la cola y a la cola de Azure Storage. Para aprender qué acciones son necesarias para una operación de datos determinada, consulte Permissions for calling blob and queue data operations (Permisos para llamar a operaciones de datos de blob y de cola). | Sí | 
Procesador de mensajes de datos de la cola de Storage | Consulta, recupera y elimina un mensaje de una cola de Azure Storage. Para aprender qué acciones son necesarias para una operación de datos determinada, consulte Permissions for calling blob and queue data operations (Permisos para llamar a operaciones de datos de blob y de cola). | Sí | 
Emisor de mensajes de datos de la cola de Storage | Agrega mensaje a una cola de Azure Storage. Para aprender qué acciones son necesarias para una operación de datos determinada, consulte Permissions for calling blob and queue data operations (Permisos para llamar a operaciones de datos de blob y de cola). | Sí | 
Lector de datos de la cola de Storage | Lee y enumera los mensajes de la cola y las colas de Azure Storage. Para aprender qué acciones son necesarias para una operación de datos determinada, consulte Permissions for calling blob and queue data operations (Permisos para llamar a operaciones de datos de blob y de cola). | No | 
Colaborador de la solicitud de soporte técnico | Permite crear y administrar solicitudes de soporte técnico. | Sí | 
Colaborador de Traffic Manager | Le permite administrar perfiles de Traffic Manager, pero no controlar los usuarios que tienen acceso a ellos. | Sí | 
Administrador de acceso de usuario | Permite administrar el acceso de usuario a los recursos de Azure. | Sí | 
Inicio de sesión de administrador de Virtual Machine | Visualización de máquinas virtuales en el portal e inicio de sesión como administrador | Sí | 
Colaborador de la máquina virtual | Permite administrar máquinas virtuales, pero no acceder a ellas, ni tampoco a la red virtual ni la cuenta de almacenamiento a las que están conectadas. | Sí | 
Inicio de sesión de usuario de Virtual Machine | Visualización de máquinas virtuales en el portal e inicio de sesión como usuario normal. | Sí | 
Colaborador de plan web | Permite administrar los planes web para sitios web, pero no acceder a ellos. | Sí | 
Colaborador de sitio web | Le permite administrar sitios web (no planes Web), pero no acceder a ellos. | Sí |
