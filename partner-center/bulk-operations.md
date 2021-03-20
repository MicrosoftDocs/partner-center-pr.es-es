---
title: Exportación e importación masiva de oportunidades de venta conjunta a través de archivos de Excel/CSV en referencias
description: Aprenda a descargar, crear o actualizar oportunidades de venta conjunta mediante archivos de Excel (CSV) en el centro de Partners.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: 39a1370ad4e5da9120c74b46dfb0c20cd93df4e3
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712196"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Operaciones masivas para oportunidades de venta conjunta mediante archivos de valores separados por comas (CSV)

**Roles adecuados**

- Administrador de referencias
- Usuario de Referencias

Las operaciones masivas del centro de Partners ayudan a su empresa a exportar e importar datos de oportunidades de venta conjunta. Vaya a la página de **oportunidades de venta conjunta** para buscar los vínculos de **importación** y **exportación** en la parte superior derecha del encabezado de título de la página. Los usuarios con el **Administrador de referencias** y los permisos de usuario de **referencia** pueden usar esta funcionalidad.

> [!IMPORTANT]
> Las acciones crear/actualizar realizadas a través de la importación en bloque no son reversibles. Tenga cuidado al modificar o crear un gran número de registros. Solo se puede modificar un subconjunto de campos después de crear un trato. **No se permitirá ninguna acción una vez que el trato alcance un estado terminal como rechazado/expirado/ganada/perdida.**

## <a name="export-co-sell-opportunities"></a>Exportar oportunidades de venta conjunta

La siguiente información describe la funcionalidad de exportación:

- Puede exportar un **máximo de 5000 registros** haciendo clic en el botón **exportar** .
- Los acuerdos que se descargan se basarán en sus niveles de acceso. Los administradores de referencia y los usuarios de referencia pueden obtener resultados diferentes en función de su ámbito e inclusión como miembros del equipo en los acuerdos. Más información sobre [los permisos de referencias](permissions-overview.md#manage-referrals).
- La función de exportación tiene en cuenta la pestaña actual de la página oportunidades de venta conjunta y los filtros que se han aplicado.
- Se generará un archivo CSV con todos los datos basados en los filtros aplicados.
- Puede tardar hasta un minuto en descargar los registros.
- No es necesario esperar a que se complete la acción de descarga. Incluso si navega a otras páginas del centro de Partners, el archivo se descargará en cuanto se complete la función de exportación.
- Puede volver a usar el archivo descargado para modificar los detalles del trato y cargarlos para actualizar los registros.

## <a name="import-co-sell-opportunities"></a>Importar oportunidades de venta conjunta

- Puede crear o actualizar un **máximo de 1000 registros** mediante la funcionalidad de importación.
- Puede crear la plantilla desde cero descargando la plantilla desde la página importar del centro de Partners.
- También puede usar la funcionalidad de exportación para descargar los registros existentes y actualizarlos.
- Si el archivo tiene más de 1000 registros, no se puede procesar.
- Una vez procesado el archivo, se mostrará un resumen con el número de referencias que se han creado, actualizado y no procesado en la tarjeta del último archivo de proceso.
- Puede descargar los detalles de los registros procesados, corregir los errores y cargar el mismo archivo para crear o actualizar los registros en los que se produjo un error en la ejecución anterior. **Quite todos los registros correctos del archivo antes de cargar los registros corregidos que dieron error en la ejecución anterior.**
- Para agregar más soluciones, agregue columnas adicionales junto a la solución 1 y use el nombre de columna como solución X, donde X representa el número de la solución en el trato. Por ejemplo, solución 2, solución 3.
- Puede Agregar hasta 50 soluciones a un contrato.
- Para agregar más miembros del equipo, agregue columnas adicionales junto al miembro del equipo 1 y use el nombre de la columna como miembro del equipo X, donde X representa el número del miembro del equipo en el contrato. Por ejemplo, miembro del equipo 2, miembro del equipo 3.
- Puede Agregar hasta 50 miembros del equipo a un contrato.

> [!NOTE]
> No es necesario esperar a que se complete el procesamiento. Los detalles del último archivo procesado estarán disponibles para su descarga una vez completado el procesamiento. **Puede tardar hasta 10 minutos si está cargando archivos con registros 1000.**

> [!IMPORTANT]
> Lea todas las instrucciones detenidamente y compruebe el formato de cada columna de la tabla siguiente antes de crear o actualizar las ofertas mediante archivos CSV en el centro de Partners.

|**Nombre de la columna**|**¿Es obligatorio?**|**Descripción**|**Valores de ejemplo**|
|-----|:-----|:---------|:---|
Errors|No|Errores si se incluye en esta columna cualquier relación con las operaciones Create/Update w. r. t con las referencias. Si hay varios errores, todos ellos se enumerarán separados por un punto y coma.|Falta la solución de campo obligatorio 1|
IDENTIFICADOR de Engagement|No|El identificador de Engagement se genera mediante el sistema de referencias del centro de Partners de Microsoft. No es necesario para la creación de nueva referencia. Puede usar el identificador de interacción existente si está actualizando un registro.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Identificador de referencia|No|El identificador de referencia se genera mediante el sistema de referencias del centro de Partners de Microsoft. No es necesario para la creación de nueva referencia. Rellénelo con el identificador de referencia si va a actualizar un registro existente.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Nombre del trato|Sí|Nombre descriptivo del contrato para la referencia.|Contrato de primavera de Reino Unido
Nombre del cliente|Sí|Nombre de la empresa del cliente. Use el nombre legal de la organización para la coincidencia rápida en el lado de Microsoft.|Contoso Corporation
Línea de dirección de cliente 1|Sí|Dirección línea 1 de la empresa del cliente. |Una forma de Contoso
Línea de dirección de cliente 2|No|Dirección de la línea 2 de la empresa del cliente.|Calle 148
Ciudad del cliente|Sí|Ciudad en la que se encuentra la organización del cliente.|Redmond
Customer State (Estado del cliente)|No|Estado en el que se encuentra la organización del cliente.|Washington
Customer Postal Code (Código postal del cliente)|No|Código postal de la región donde se encuentra la organización del cliente.|98052
Customer Country (País del cliente)|Sí|País o región donde se encuentra la organización del cliente. Use los códigos de país de dos letras, como se mencionó [aquí]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes).|US
ID. de cliente D-U-N-S|No|Intente capturar el ID. de DUNS de la organización del cliente. Esto le ayudará a la coincidencia más rápida de la organización del cliente en el lado de Microsoft, lo que ayuda a asignar más rápido al vendedor. Puede obtener el identificador de DUNS gratis desde este [sitio web](https://www.dnb.com/duns-number/lookup.html).|81466849
Nombre de contacto del cliente|Depende|El nombre solo es obligatorio si necesita ayuda de Microsoft. El nombre del contacto principal de la organización del cliente que trabaja en este contrato.|John
Apellido de contacto del cliente|Depende|El apellido solo es obligatorio si necesita ayuda de Microsoft. Apellido del contacto principal de la organización del cliente que trabaja en este contrato.|Cliente
Número de teléfono de contacto del cliente|Depende|El número de teléfono solo es obligatorio si necesita ayuda de Microsoft. Número de teléfono del contacto principal de la organización del cliente que trabaja en este trato.|9999999999
Dirección de correo electrónico de contacto del cliente|Depende|La dirección de correo electrónico solo es obligatoria si necesita ayuda de Microsoft. Dirección de correo electrónico del contacto principal de la organización del cliente que trabaja en este contrato.|john.customer@contoso.com
Estado de referencia de asociado|Sí|Indica el estado del trato desde la perspectiva de la empresa. Obligatorio si intenta crear o modificar una referencia. Use **nuevo** si está intentando crear un nuevo trato. Los valores aceptados se documentan [aquí](/partner/develop/referral-resources#referralstatus).|Activo
Subestado de referencia de asociado|Sí|Indica el estado exacto de la transacción. Use **aceptado** si está intentando crear un nuevo trato. También es necesario si va a modificar una referencia existente. Los valores aceptados se documentan [aquí](/partner/develop/referral-resources#referralsubstatus).|Aceptado
Estado de referencia de Microsoft|Depende|Indica el estado de la solicitud de venta conjunta que envió a Microsoft para buscar ayuda. Este campo es de solo lectura. Se omitirá cualquier cambio realizado en este campo mientras se importan los datos.| Pending
Motivo de rechazo o pérdida|Depende| Solo se le pedirá que proporcione esta información si va a cambiar el subestado del campo a rechazado o perdido. Puede omitir esta columna en caso contrario. <br/> **Escriba un número basado en las opciones siguientes** <br/><br/> **1**-el presupuesto del proyecto no es adecuado  <br/> **2**-el cliente no respondió  <br/> **3**-el cliente eligió otro proveedor  <br/> **4** -no se cumplen los requisitos del cliente  <br/> **5** -no es un cliente <br/> **6**: la línea de tiempo propuesta es demasiado corta <br/> **7** -notificar como abuso, correo no deseado o phishing <br/> **8** -otros |6|
Fase de ventas|No|Este es el campo que indica la fase de ventas detallada de la referencia. Obtenga más información sobre las fases de ventas [aquí](./manage-co-sell-opportunities.md)|40
Valor de negocio estimado|Sí|"El valor del trato en función de las conversaciones iniciales con el cliente. Se puede cambiar hasta que el trato alcance uno de los Estados de terminal.| ganada o perdida ".|12563
Moneda|Sí|La moneda en la que se especifica el valor de trato. [Aquí](https://en.wikipedia.org/wiki/ISO_4217)puede encontrar los códigos de divisa.|USD
Fecha de cierre estimada|Sí|Fecha de cierre estimada del trato en función de las conversaciones iniciales con el cliente en el formato MM/DD/AAAA. <br/> **La fecha debe estar en la zona horaria UTC. Todas las fechas que se muestran en la interfaz de usuario del centro de Partners se basan en las zonas horarias localizadas. Puede haber una diferencia de +/-un día en la interfaz de usuario del centro de partners si está examinando la referencia para la que proporcionó la fecha en la zona horaria UTC.**|1/30/2020
IDENTIFICADOR DE CRM|No|Identificador de esta referencia específica en el sistema CRM, si existe. Se trata de un campo de entrada de texto de forma libre.|34234324-Sdfsdf-345345-SFD
ID. de campaña de marketing|No|Este campo indica la campaña de marketing, que resultó en esta referencia específica. Se usa normalmente para el cálculo de ROI|BingSummer2020
Notas|No|Notas detalladas que indican las actualizaciones relacionadas con la referencia|Esta es una nota de ejemplo
¿Necesita ayuda de Microsoft?|Sí|Esto es para indicar si desea que Microsoft le ayude a hacer esta solicitud de venta conjunta.|Sí
¿Qué ayuda específica de Microsoft?|Depende|Una de las seis maneras diferentes que Microsoft puede ayudarle. Esto solo es aplicable si elige sí en la pregunta "¿necesita ayuda de Microsoft? " <br/> **Escriba un número basado en las opciones siguientes** <br/><br/> **1**: propuesta de valor específica de la carga de trabajo  <br/> **2**-arquitectura técnica del cliente  <br/> **3**-prueba de concepto/demo  <br/> **4**-comillas y licencias  <br/> **5**-posterior-ventas de cliente correcta  <br/> **6**-general u otro|1|
Compartir con el equipo de ventas de Microsoft|Sí|Esto indica si desea compartir los detalles del trato con el equipo de ventas de Microsoft o no. Esto solo es aplicable si elige no en la pregunta "ayuda de Microsoft necesaria? "|Sí
Notas a Microsoft|No|Cualquier nota específica a Microsoft si necesita ayuda de Microsoft|Necesita ayuda con una POC para el cliente de Contoso
Consentimiento para compartir el contacto con el cliente y el socio|Sí|Consentimiento para compartir los detalles de contacto del cliente y los detalles de contacto de los empleados de la empresa que trabajan en el trato. **Los contratos no se crearán ni actualizarán si elige no para esta columna.** |Sí
Solución 1|Sí|IDENTIFICADOR de la solución (obligatorio), la moneda (opcional) en la que se especifica el valor del trato. Puede encontrar los códigos de divisa [aquí](https://en.wikipedia.org/wiki/ISO_4217), el precio de la SKU (opcional) y la cantidad de la SKU (opcional).  |SOL-1234-PQRS, USD, 10, 100
Miembro del equipo 1|Sí|Nombre, apellidos, número de móvil e identificador de correo electrónico del miembro del equipo correspondiente.| Bob, Partner, 999999, Bob.partner@Contoso.com

## <a name="next-steps"></a>Pasos siguientes

Puede usar estos conectores de venta conjunta del centro de partners para la venta conjunta con Microsoft desde los sistemas CRM.

- [Conector de venta conjunta para Dynamics 365 CRM: información general](connector-dynamics.md)
- [Conector de venta conjunta para Salesforce CRM: información general](connector-salesforce.md)
