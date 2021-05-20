---
title: Exportación e importación masiva de oportunidades de venta en bloque a través de archivos de Excel/CSV en referencias
description: Obtenga información sobre cómo descargar, crear o actualizar oportunidades de venta conjunto mediante archivos de Excel (CSV) en Centro de partners
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: af567b9b8b36841b6e6fd7e18a34e1c4b6b81f2e
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110149169"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Operaciones masivas para oportunidades de venta masiva mediante archivos de valores separados por comas (CSV)

**Roles adecuados:** administrador de referencias | Usuario de referencias

Las operaciones masivas Centro de partners ayudar a su empresa a exportar e importar datos de oportunidades de venta conjunto. Vaya a la página oportunidades de  venta  en colaboración para buscar los **vínculos** de importación y exportación en la parte superior derecha del banner del título de la página. Los usuarios con **permisos de administrador de referencias** y **usuario** de referencias pueden usar esta funcionalidad.

> [!IMPORTANT]
> Las acciones de creación y actualización realizadas a través de la importación masiva no son reversibles. Tenga cuidado al modificar o crear un gran número de registros. Solo se puede modificar un subconjunto de campos después de crear una oferta. **No se permitirá ninguna acción una vez que cualquier oferta alcance un estado terminal como Rechazado, Expirado, Ganado o Perdido.**

## <a name="export-co-sell-opportunities"></a>Exportación de oportunidades de venta en colaboración

En la siguiente información se describe la funcionalidad de exportación:

- Puede exportar un **máximo de 5000 registros haciendo** clic en el botón **exportar.**
- Las ofertas que se descargan se basarán en los niveles de acceso. Los administradores de referencias y los usuarios de referencia pueden obtener resultados diferentes en función de su ámbito e inclusión como miembros del equipo en las ofertas. Obtenga más información [sobre los permisos de referencia.](permissions-overview.md#manage-referrals)
- La función de exportación tiene en cuenta la pestaña actual en la página oportunidades de venta co-sell y los filtros que se han aplicado.
- Se generará un archivo CSV con todos los datos basados en los filtros aplicados.
- La descarga de los registros puede tardar hasta un minuto.
- No tiene que esperar a que se complete la acción de descarga. Incluso si navega a otras páginas de Centro de partners, el archivo se descargará en cuanto se complete la función de exportación.
- Puede reutilizar el archivo descargado para modificar los detalles de la oferta y cargarlo para actualizar los registros.

## <a name="import-co-sell-opportunities"></a>Importar oportunidades de venta en colaboración

- Puede crear o actualizar un **máximo de 1000 registros mediante** la funcionalidad de importación.
- Puede compilar la plantilla desde cero descargando la plantilla desde la página Importar de Centro de partners.
- También puede usar la funcionalidad Exportar para descargar los registros existentes y actualizarlos.
- Si el archivo tiene más de 1000 registros, no se puede procesar.
- Una vez procesado el archivo, se mostrará un resumen con el número de referencias que se crearon, actualizaron y no procesaron en la tarjeta del último archivo de proceso.
- Puede descargar los detalles de los registros procesados, corregir los errores y cargar el mismo archivo para crear o actualizar los registros con errores en la ejecución anterior. **Quite todos los registros correctos del archivo antes de cargar los registros corregidos que no se pudieron ejecutar en la ejecución anterior.**
- Para agregar más soluciones, agregue columnas adicionales junto a la solución 1 y use el nombre de columna como Solución X, donde X representa el número de la solución en la oferta. Por ejemplo, Solución 2, Solución 3.
- Puede agregar hasta 50 soluciones a una oferta.
- Para agregar más miembros del equipo, agregue columnas adicionales junto a Miembro del equipo 1 y use el nombre de columna como Miembro del equipo X, donde X representa el número del miembro del equipo en la oferta. Por ejemplo, Miembro del equipo 2, Miembro del equipo 3.
- Puede agregar hasta 50 miembros del equipo a una oferta.

> [!NOTE]
> No tiene que esperar a que se complete el procesamiento. Los detalles del último archivo procesado estarán disponibles para su descarga una vez completado el procesamiento. **Puede tardar hasta 10 minutos si carga archivos con 1000 registros.**

> [!IMPORTANT]
> Lea todas las instrucciones con cuidado y compruebe el formato de cada columna de la tabla siguiente antes de crear o actualizar ofertas mediante archivos CSV en Centro de partners.

|**Nombre de la columna**|**¿Es obligatorio?**|**Descripción**|**Valores de ejemplo**|
|-----|:-----|:---------|:---|
Errors|No|Errores si algún relacionado con las operaciones de creación/actualización w.r.t con las referencias se incluirá en esta columna. Si hay varios errores, todos ellos aparecerán separados por un punto y coma.|Falta el campo obligatorio Solución 1|
Identificador de interacción|No|El identificador de interacción lo genera el sistema de referencias del Centro de partners de Microsoft. No es necesario para la creación de nuevas referencias. Puede usar el identificador de interacción existente si va a actualizar un registro.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Identificador de referencia|No|El identificador de referencia lo genera el sistema de referencias del Centro de partners de Microsoft. No es necesario para la creación de una nueva referencia. Rellene con el identificador de referencia si va a actualizar un registro existente.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Nombre de la oferta|Sí|Nombre descriptivo de la oferta de referencia.|Acuerdo de spring del Reino Unido
Nombre del cliente|Sí|Nombre de la empresa del cliente. Use el nombre legal de la organización para la coincidencia rápida en el lado de Microsoft.|Contoso Corporation
Línea 1 de la dirección del cliente|Sí|Dirección de la línea 1 de la empresa del cliente. |One Contoso Way
Línea 2 de la dirección del cliente|No|Dirección de la línea 2 de la empresa del cliente.|CALLE NE 148
Ciudad del cliente|Sí|Ciudad donde se encuentra la organización del cliente.|Redmond
Customer State (Estado del cliente)|No|Estado donde se encuentra la organización del cliente.|Washington
Customer Postal Code (Código postal del cliente)|No|Código postal de la región donde se encuentra la organización del cliente.|98052
Customer Country (País del cliente)|Sí|País o región donde se encuentra la organización del cliente. Use los códigos de país de dos letras, como se [mencionó aquí.]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)|US
Id. de D-U-N-S del cliente|No|Intente capturar el identificador DE DUNS de la organización del cliente. Esto ayudará a una coincidencia más rápida de la organización del cliente en el lado de Microsoft, lo que ayuda a acelerar la asignación de vendedores. Puede obtener el identificador DE DUNS GRATIS desde este sitio [web.](https://www.dnb.com/duns-number/lookup.html)|81466849
Nombre del contacto con el cliente|Depende|El nombre solo es obligatorio si necesita ayuda de Microsoft. El nombre del contacto principal de la organización del cliente que trabaja en esta oferta.|John
Apellidos de contacto del cliente|Depende|Los apellidos solo son obligatorios si necesita ayuda de Microsoft. Apellidos del contacto principal de la organización del cliente que trabaja en esta oferta.|Customer
Número de teléfono de contacto del cliente|Depende|El número de teléfono solo es obligatorio si necesita ayuda de Microsoft. Número de teléfono del contacto principal de la organización del cliente que trabaja en esta oferta.|9999999999
Dirección de correo electrónico de contacto del cliente|Depende|La dirección de correo electrónico solo es obligatoria si necesita ayuda de Microsoft. Dirección de correo electrónico del contacto principal de la organización del cliente que trabaja en esta oferta.|john.customer@contoso.com
Estado de referencia de asociado|Sí|Indica el estado de la oferta desde la perspectiva de la empresa. Obligatorio si intenta crear o modificar una referencia. Use **Nuevo** si está intentando crear una nueva oferta. Los valores aceptados se [documentan aquí.](/partner/develop/referral-resources#referralstatus)|Active
Subestado de referencia de asociado|Sí|Indica el estado exacto de la oferta. Use **Aceptado** si está intentando crear una nueva oferta. También es necesario si va a modificar una referencia existente. Los valores aceptados se documentan [aquí.](/partner/develop/referral-resources#referralsubstatus)|Aceptado
Estado de referencia de Microsoft|Depende|Indica el estado de la solicitud de venta co-venta que envió a Microsoft en busca de ayuda. Este campo es de solo lectura. Cualquier cambio realizado en este campo al importar los datos se omitirá.| Pending
Motivo rechazado o perdido|Depende| Solo debe proporcionar esta información si va a cambiar el subes estado del campo a Rechazado o Perdido. De lo contrario, puede omitir esta columna. <br/> **Escriba un número en función de las opciones siguientes.** <br/><br/> **1**- El presupuesto del proyecto no es adecuado  <br/> **2**- El cliente no respondió  <br/> **3**- El cliente eligió otro proveedor  <br/> **4 -** No se cumplen los requisitos del cliente  <br/> **5** - No es un cliente <br/> **6**- La línea de tiempo propuesta era demasiado corta <br/> **7 -** Notificar como abuso, correo no deseado o suplantación de identidad (phishing) <br/> **8** - Otros |6|
Fase de ventas|No|Este es el campo para indicar la fase de ventas detallada de la referencia. Obtenga más información sobre las fases de [ventas aquí.](./manage-co-sell-opportunities.md)|40
Valor estimado de la oferta|Sí|Valor de la oferta en función de las conversaciones iniciales con el cliente. Esto se puede cambiar hasta que la oferta alcance uno de los estados terminales **ganados** o **perdidos.**|12563
Moneda|Sí|Moneda en la que se introduce el valor de la oferta. Puede encontrar los códigos de moneda [aquí.](https://en.wikipedia.org/wiki/ISO_4217)|USD
Fecha de cierre estimada|Sí|Fecha de cierre estimada de la oferta en función de las conversaciones iniciales con el cliente en el formato MM/DD/AÑO. <br/> **La fecha debe estar en zona horaria UTC. Todas las fechas que se muestran en Centro de partners interfaz de usuario se basan en zonas horarias localizadas. Puede haber una diferencia de +/- un día en la interfaz de usuario de Centro de partners si está viendo la referencia para la que proporcionó la fecha en zona horaria UTC.**|1/30/2020
Id. de CRM|No|Identificador de esta referencia específica en el sistema CRM, si lo hubiera. Se trata de un campo de entrada de texto de forma libre.|34234324-sdfsdf-345345-sfd
Id. de campaña de marketing|No|Este campo indica la campaña de marketing, que dio lugar a esta referencia específica. Normalmente se usa para el cálculo de ROI|BingSummer2020
Notas|No|Notas detalladas que indican las actualizaciones relacionadas con la referencia|Esta es una nota de ejemplo
¿Necesita ayuda de Microsoft?|Sí|Esto es para indicar si quiere que Microsoft le ayude a realizar esta solicitud de venta co-venta.|Sí
¿Qué ayuda específica de Microsoft?|Depende|Una de las seis maneras diferentes en que Microsoft puede ayudarle. Esto solo es aplicable si elige Sí para la pregunta "¿Se requiere ayuda de Microsoft? " <br/> **Escriba un número en función de las opciones siguientes.** <br/><br/> **1 -** Carga de trabajo: propuesta de valor específica  <br/> **2**- Arquitectura técnica del cliente  <br/> **3**- Prueba de concepto /Demo  <br/> **4 -** Comillas y licencias  <br/> **5 -** Publicación: éxito del cliente de ventas  <br/> **6**- General u otros|1|
Compartir con el equipo de ventas de Microsoft|Sí|Esto es para indicar si desea compartir los detalles del contrato con el equipo de ventas de Microsoft o no. Esto solo es aplicable si elige No para la pregunta "¿Se requiere ayuda de Microsoft? "|Sí
Notas para Microsoft|No|Cualquier nota específica para Microsoft si necesita ayuda de Microsoft|Necesita ayuda con una POC para el cliente de Contoso
Consentimiento para compartir contacto con el cliente o asociado|Sí|Consentimiento para compartir los detalles de contacto del cliente y los detalles de contacto de los empleados de la empresa que trabajan en el contrato. **Las ofertas no se crearán ni actualizarán si elige No para esta columna.** |Sí
Solución 1|Sí|Id. de solución (obligatorio), moneda (opcional) en la que se introduce el valor de la oferta. Puede encontrar los códigos de moneda [aquí,](https://en.wikipedia.org/wiki/ISO_4217)precio de la SKU (opcional) y cantidad de la SKU (opcional)  |SOL-1234-PQRS, USD, 10, 100
Miembro del equipo 1|Sí|Nombre, apellido, número de móvil e identificador de correo electrónico del miembro del equipo correspondiente.| Bob, partner, 999999, Bob.partner@Contoso.com

## <a name="next-steps"></a>Pasos siguientes

Puede usar estos conectores Centro de partners co-sell para la venta en colaboración con Microsoft desde dentro de sus sistemas CRM.

- [Conector de venta conjunto para Dynamics 365 CRM: información general](connector-dynamics.md)
- [Conector de venta conjunta para Salesforce CRM: información general](connector-salesforce.md)
