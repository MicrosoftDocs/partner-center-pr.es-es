---
title: Anuncios de abril de 2021
description: Anuncios de abril de 2021 para el Centro de partners de Microsoft, incluidas nuevas funcionalidades, promociones, ofertas, mercados o cambios en ofertas existentes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: 798dcb1570a0f6dfc94c7b45fc3c2e152f55cbe5
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702831"
---
# <a name="april-2021-announcements"></a>Anuncios de abril de 2021

En esta página se encuentran los anuncios del Centro de partners de Microsoft de abril de 2021.

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a>Preparación: Se ha actualizado la API de validación de direcciones de clientes de CSP que se publicará en junio. La funcionalidad de pruebas ya está disponible.

### <a name="categories"></a>Categorías

- Fecha: 30/04/2021
- Preparación

### <a name="summary"></a>Resumen

Para ayudar a los partners y clientes a dirigir sus negocios basándose en la confianza, invitaremos a los partners a probar los cambios en la API de validación de direcciones para todos los países en todo el mundo.

### <a name="impacted-audience"></a>Audiencia afectada

Partners de facturación directa de CSP y proveedores indirectos que crean o actualizan los detalles actuales de dirección de los clientes.

### <a name="details"></a>Detalles

Microsoft funciona con confianza. Nos comprometemos a proporcionar un método compatible, seguro y protegido para la validación de la dirección de los clientes durante las operaciones de transacción con suscripciones de clientes en el programa CSP. A partir del 31 de marzo de 2021, hemos introducido cambios en la API de validación de direcciones. Invitamos a los partners a probar la API antes de la publicación a finales de junio de 2021. 

Tenga en cuenta que estos cambios solo afectan a la API de validación de direcciones. Las API de creación de clientes y actualización del perfil de facturación no se ven afectadas. Aunque la dirección sugerida no tiene que usarse actualmente con la API de creación de clientes, se recomienda encarecidamente.

La respuesta devolverá uno de los siguientes mensajes de estado:

| Status     | Descripción |    Número de direcciones sugeridas devueltas |
|-------|---------------|-------------------|
|Verified shippable | La dirección está comprobada y puede recibir envíos. | Single |
|Verified | La dirección está comprobada. | Single |
|Interaction required | La dirección sugerida se ha cambiado significativamente y se necesita la confirmación del usuario. | Single |
|Street partial | La calle indicada en la dirección es parcial y necesita más información. | Varias: tres como máximo |
|Premises partial | Los locales especificados (número de edificio, número de suite, etc.) son parciales y se necesita más información. | Varias: tres como máximo |
|Múltiple | La dirección tiene varios campos que son parciales (también puede incluir Street partial y Premises partial). | Varias: tres como máximo |
|Ninguno | La dirección es incorrecta. | Ninguno |
|No validado | No se pudo enviar la dirección a través del proceso de validación. | Ninguno |

Los códigos postales de EE. UU. devolverán cuatro dígitos adicionales más un guion, por ejemplo, 12345-6789.

### <a name="next-steps"></a>Pasos siguientes

- Revise la documentación técnica y las preguntas más frecuentes en la [colección específica para asociados](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) a fin de obtener instrucciones más detalladas.
- Prepárese para incorporar los cambios mediante la API del Centro de partners y la experiencia de usuario web. 
- Comparta su id. de inquilino de espacio aislado con nuestro experto en la materia, Ali Khaki, para que se incluya en el piloto de prueba, de modo que pueda empezar a preparar la actualización. 
- Si usa una solución de proveedor de panel de control (CPV), consulte a su CPV.

### <a name="questions"></a>¿Tiene alguna pregunta?

Si necesita soporte técnico para las operaciones con Microsoft, póngase en contacto con el grupo de Yammer de soporte técnico al partner o abra una [solicitud de servicio](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a>Nueva ubicación para la documentación de Swagger de las API del Centro de partners

### <a name="categories"></a>Categorías

- Fecha: 26/04/2021
- Funcionalidades

### <a name="summary"></a>Resumen

Los documentos de Swagger de las API del Centro de partners se han migrado desde el [sitio de documentación de Swagger anterior](https://apidocs.microsoft.com/services/partnercenter) a un [nuevo sitio de documentación de Swagger](https://docs.microsoft.com/rest/api/partner-center-rest/).

### <a name="impacted-audience"></a>Audiencia afectada

Partners de factura directa y proveedores indirectos que participan en el programa Proveedor de soluciones en la nube (CSP) y que usan las API del Centro de partners.

### <a name="details"></a>Detalles

A partir del 26 de abril de 2021, la documentación de Swagger de las API del Centro de partners, incluido el contenido de la API REST, se encuentra en un [nuevo sitio](https://docs.microsoft.com/rest/api/partner-center-rest/). El sitio antiguo dejará de ser accesible después de varias semanas.

### <a name="benefits"></a>Ventajas

La documentación de Swagger de las API del Centro de partners proporciona una función **Pruébalo**. Para usar esta función, deberá tener un token de portador, que puede generar siguiendo los pasos indicados en [Autenticación del Centro de partners](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication).

### <a name="next-steps"></a>Pasos siguientes

Comparta esta información en su organización para que el equipo adecuado pueda revisar y actualizar sus procesos.

### <a name="questions"></a>¿Tiene alguna pregunta?

Si tiene preguntas sobre estas ofertas, consúltelas a las comunidades de Yammer correspondientes.

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a>Directiva del período de devolución de software para Proveedor de soluciones en la nube (CSP) y aviso de expiración del vínculo de descarga

### <a name="categories"></a>Categorías

- Fecha: 21/04/2021
- Funcionalidades

### <a name="summary"></a>Resumen

Hay cambios en la directiva del período de devolución de software para CSP y en la expiración del vínculo de descarga.

### <a name="impacted-audience"></a>Audiencia afectada

Partners que realizan transacciones con ofertas de software perpetuo o suscripciones de software en CSP

### <a name="details"></a>Detalles

Tenga en cuenta las siguientes notificaciones importantes relacionadas con las compras de software perpetuo y suscripciones de software a través del Centro de partners:

#### <a name="software-return-period-policy"></a>Directiva del período de devolución de software

A partir del 1 de junio de 2021, el período de devolución de las ofertas de software en CSP, como se indica en el Microsoft Partner Agreement (MPA), cambiará de 60 días desde la fecha de pedido a 30 días desde la fecha de pedido.

Después de enviar un pedido para una oferta de software, los partners tendrán 30 días a partir de la fecha de pedido para enviar cualquier modificación de dicho pedido:

- Toda licencia de software perpetuo devuelta dentro del período de devolución de 30 días recibirá un crédito completo del precio de compra pagado.

- Todo producto de suscripción de software devuelto dentro del período de devolución de 30 días recibirá un crédito prorrateado del precio de compra pagado.

Este mensaje es la continuación de los comunicados enviados por correo electrónico en diciembre de 2020 y abril de 2021 a todos los partners de CSP con respecto al período de devolución y otras actualizaciones al MPA. Consulte esos avisos para obtener detalles completos sobre los cambios que afectan al MPA.

#### <a name="software-download-link-expiry"></a>Expiración del vínculo de descarga de software

A partir del 3 de junio de 2021, los vínculos de descarga de software para las compras de productos de software perpetuo y suscripciones de software a través del Centro de partners tendrán una fecha de expiración de cinco días a partir de la descarga inicial. El período de expiración se aplicará a todas las compras anteriores al 3 de junio de 2021, así como a partir del 3 de junio de 2021 en adelante.

### <a name="next-steps"></a>Pasos siguientes

Revise las [Preguntas frecuentes sobre el período de devolución de CSP y la expiración del vínculo de descarga](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), e informe de estos cambios a todos los equipos pertinentes de su organización:

### <a name="questions"></a>¿Tiene alguna pregunta?

Si tiene preguntas sobre estas ofertas, consúltelas a las comunidades de Yammer correspondientes.

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a>Programa Open License: transición de revendedores al programa Proveedor de soluciones en la nube (CSP)

### <a name="categories"></a>Categorías

- Fecha: 19/04/2021
- Hacer crecer el negocio

### <a name="summary"></a>Resumen

En esta comunicación se detalla cómo prepararse para los cambios que se van a realizar próximamente en el programa Open License.

### <a name="impacted-audience"></a>Audiencia afectada

Asociados de Open License y CSP

### <a name="details"></a>Detalles

En 2020, Microsoft [anunció](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) que las licencias perpetuas de software estarán disponibles ampliamente para asociados y clientes a través del programa Proveedor de soluciones en la nube (CSP). El primer hito se alcanzó en enero de 2021, cuando las ofertas perpetuas de software comerciales se pusieron disponibles. El siguiente hito clave se realizará en julio de 2021, cuando las ofertas del [sector público](https://aka.ms/openlicensepublicsector) estén disponibles. También se ha [comunicado](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) que, a partir del 1 de enero de 2022, no se pueden realizar nuevas compras ni renovaciones de licencias de software de Software Assurance o servicios en línea a través del programa Open License.

La transición del software perpetuo al programa CSP en la nueva experiencia comercial ayudará a los asociados a ampliar las oportunidades de ofrecer diversas soluciones y servicios administrados. Esto también acelerará la transición de los clientes a la nube.  Para ayudar a garantizar una transición sin problemas para nuestros asociados y clientes, hemos realizado estos ajustes y materiales para acelerar esta transformación digital:

#### <a name="april-2021"></a>Abril de 2021

[Ya disponible](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): materiales de transición de Open License a CSP para revendedores.

#### <a name="july-2021"></a>Julio de 2021

##### <a name="csp"></a>CSP

- 1 de julio: licencias perpetuas de software disponibles para los clientes del sector público.

- 7 de julio: licencias perpetuas de software de Visual Studio Pro y Get Genuine Windows Agreement disponibles para todos los segmentos.

##### <a name="open-value"></a>Open Value

- 1 de julio: SKU adicionales disponibles en el programa Open Value para centros educativos y organizaciones sin ánimo de lucro, que proporcionan ofertas similares al programa Open License.

##### <a name="open-license"></a>Open License

- 1 de julio: Microsoft ya no lanzará nuevas ofertas en el programa Open License.

#### <a name="january-2022"></a>Enero de 2022

- A partir del 1 de enero de 2022, no se pueden realizar nuevas compras ni renovaciones mediante el programa Open License.

### <a name="next-steps"></a>Pasos siguientes

#### <a name="csp-indirect-providers"></a>Proveedores indirectos de CSP

Dedique los próximos meses a ayudar a los revendedores de Open License a orientarse en el programa CSP mediante la asistencia a eventos de la comunidad de asociados y el uso de los materiales de transición de Open License a CSP para revendedores:

- [Materiales de transición de Open License a CSP para revendedores](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): presentación de información general personalizable, plantilla de correo electrónico, guía de incorporación de revendedores indirectos de CSP y mucho más para ayudarle a impulsar la adopción de los revendedores a gran escala.

- [Eventos de la comunidad de asociados de CSP](https://globalpbocomm.eventbuilder.com/GlobalCSP) hospedados por Microsoft Business Operations.  Únase a las distintas sesiones para obtener información sobre los conceptos básicos de CSP (aspectos básicos de CSP) o mantenerse al día y hacer preguntas sobre el software en CSP (sesiones de preguntas y respuestas).

- (Próximamente) Sesión de entrenamiento centrada en revendedores indirectos de CSP hospedada por Microsoft Business Operations.

#### <a name="open-license-resellers"></a>Revendedores de Open License

- Si su organización no está actualmente inscrita en el programa CSP, póngase en contacto con el distribuidor para obtener información sobre cómo empezar. Conéctese con un proveedor indirecto [aquí](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).

- Si su organización ya está inscrita en el programa CSP, obtenga más información sobre el software perpetuo en CSP [aquí](https://partner.microsoft.com/resources/collection/software-in-csp).

### <a name="questions"></a>¿Tiene alguna pregunta?

Si tiene alguna pregunta más sobre estas ofertas, consulte con las comunidades de Yammer correspondientes.

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a>Ya disponible: guía de preparación para la promoción global

### <a name="categories"></a>Categorías

- Fecha: 16/04/2021
- Capacidades

### <a name="summary"></a>Resumen

La preparación de lanzamiento ha publicado una nueva [guía global de preparación para la promoción](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) en la galería de recursos de preparación de operaciones. En esta guía se proporciona una vista consolidada de todas las [promociones globales](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/) activas.

### <a name="impacted-audience"></a>Audiencia afectada

Todos los asociados de licencias por volumen (VL), lista de precios de Dynamics (DPL) y Proveedor de soluciones en la nube (CSP)

### <a name="details"></a>Detalles

Los asociados de Microsoft han compartido con nosotros la necesidad de proporcionar una vista consolidada de todas las promociones globales con detalles de soporte técnico. Querían que esta guía consolidada le ayudara a usar promociones con la confianza de que toda la información disponible fuese fácilmente accesible en una ubicación central y cómoda.

A partir de abril de 2021, Microsoft actualizará esta guía mensualmente y estará disponible en una colección dedicada de preparación para la promoción global en la galería de recursos de preparación de operaciones.

Los vínculos a esta guía también se incluirán en las colecciones siguientes:

- [Colección de calendario de lanzamientos](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), que proporciona una vista centralizada de los próximos cambios y lanzamientos.

- [Colecciones de la comunidad](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), que contienen materiales de apoyo para nuestras llamadas mensuales de asociados, que resaltan los próximos cambios y temas oportunos de interés operativo.

- [Boletines de asociados](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), como la actualización mensual de CSP.

Como recordatorio mensual, también publicaremos un anuncio del Centro de partners con cada nuevo problema de la guía de preparación para la promoción global.

### <a name="next-steps"></a>Pasos siguientes

Al principio de cada mes, encontrará la [guía de preparación para la promoción global](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) más reciente en la [galería de recursos de preparación de operaciones](https://partner.microsoft.com/resources).

Comparta esta información con los contactos adecuados de sus organizaciones y háganos saber lo útil que es la guía a través del artículo "¿Ha sido útil esta página?" situado al final de cada página.

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a>Actualización y recordatorios de la comunidad de Proveedor de soluciones en la nube (CSP) de abril

### <a name="categories"></a>Categorías

- Fecha: 16/04/2021
- Comunidad | Invitaciones y recordatorios

### <a name="summary"></a>Resumen

Los recursos de la comunidad de CSP están disponibles a petición y se actualizan mensualmente para mantenerlo informado y preparado para el cambio en el programa CSP.

### <a name="impacted-audience"></a>Audiencia afectada

Proveedores indirectos o asociados de factura directa de CSP

### <a name="details"></a>Detalles

Este mes, los recursos incluyen los siguientes temas clave:

- [Actualización a la evolución del programa CSP y cambios en el programa Open License](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [Cambios en los requisitos de incorporación de clientes de CSP en determinadas regiones](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [Nuevo formato para la nueva factura de comercio en PDF en el programa CSP](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

Dentro de la [colección de la comunidad de CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), encontrará:

- El [boletín de actualización mensual de CSP](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global) descargable, que agrega anuncios, actualizaciones, eventos y recordatorios recientes de CSP en un documento fácil de leer.

- El [calendario de anuncios de CSP](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), que proporciona una vista de escala de tiempo de los próximos cambios que afectan al programa.

- El nuevo [calendario de lanzamientos de productos](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), donde puede ver las próximas ofertas y lanzamientos de productos.

- [Recursos de actualización de lanzamientos de CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) con contenido fácil de consumir en los cambios operativos clave.

- [Actualizadores y recordatorios](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) sobre temas clave de CSP que reciben interés y consultas.

#### <a name="csp-community-call-qas"></a>Preguntas y respuestas de llamadas de la comunidad de CSP

Las preguntas y respuestas de llamadas de la comunidad están disponibles para ayudarle con preguntas relacionadas con los próximos cambios. Regístrese ahora para las preguntas y respuestas de llamadas de la comunidad que tendrán lugar en abril, mayo y junio. Se centrarán en los lanzamientos más recientes, los actualizadores importantes y los recordatorios.

[Regístrese aquí](https://globalpbocomm.eventbuilder.com/GlobalCSP).

### <a name="next-steps"></a>Pasos siguientes

Revise los recursos de la comunidad y regístrese para las preguntas y respuestas de llamadas de la comunidad.

Para asegurarse de que obtiene el máximo partido de las preguntas y respuestas de llamadas de la comunidad, revise el contenido de la comunidad a petición y envíe sus preguntas hasta 48 horas antes de la llamada.

### <a name="questions"></a>¿Tiene alguna pregunta?

Las preguntas y respuestas de llamadas de la comunidad de CSP mensuales son el mejor lugar para las preguntas relacionadas con los cambios en el programa CSP. Cada mes, revise el material y envíe sus preguntas de antemano para que podamos dedicar la sesión a los temas más importantes para usted.

Para obtener más información, póngase en contacto con el [soporte técnico](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).

________________
## <a name="final-reminder-deprecation-of-get-qualification-on-may-6-2021"></a><a name="4"></a>Recordatorio final: Desuso de calificación GET para el 6 de mayo de 2021

### <a name="categories"></a>Categorías

- Fecha: 04/05/2021

- Funcionalidades

### <a name="impacted-audience"></a>Audiencia afectada

Asociados que venden ofertas académicas, sin ánimo de lucro y de Government Community Cloud (GCC) a través del programa Proveedor de soluciones en la nube mediante la API del Centro de partners.

### <a name="details"></a>Detalles

Este anuncio es un seguimiento de las [mejoras publicadas en diciembre](https://docs.microsoft.com/partner-center/announcements/2020-december#1) en el Centro de partners. Como parte de ese lanzamiento, se han implementado nuevas API de calificación GET y POST y, como resultado, **la calificación GET existente se retirará el 6 de mayo de 2021**. En ese momento, deberá haber pasado a las nuevas API de POST del Centro de partners. Las nuevas API de POST le permitirán comprar ofertas para educación, mientras que las nuevas API de GET le permitirán comprar ofertas sin ánimo de lucro y GCC previamente calificadas.

### <a name="next-steps"></a>Pasos siguientes

- **Actualice las nuevas API** para conseguir una transición correcta y oportuna.

- **Revise los nuevos cambios en la API del Centro de partners y consulte la Guía** sobre los recursos de preparación de operaciones: [Mejoras en el proceso de validación de clientes de Educación del Centro de partners](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).

- Comparta esta información con los equipos adecuados de su organización y con sus revendedores para ayudarlos a prepararse para estos cambios.

### <a name="questions"></a>¿Tiene alguna pregunta?

Si tiene alguna pregunta relacionada con esta notificación, póngase en contacto con el [soporte técnico del Centro de partners](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).

### <a name="change-log"></a>Registro de cambios

- 4 de mayo de 2021: recordatorio final de la próxima entrada en desuso de la calificación GET

- 9 de abril de 2021: recordatorio de la próxima entrada en desuso de la calificación GET 

- Febrero: escalas de tiempo actualizadas y que dejarán en desuso las calificaciones GET y PUT.

- Enero: recordatorio de la próxima entrada en desuso de las calificaciones de GET & PUT

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a>Nuevo formato para la nueva factura de comercio en PDF en CSP

### <a name="categories"></a>Categorías

- Fecha: 05/04/2021
- Funcionalidades

### <a name="summary"></a>Resumen

Microsoft presenta un nuevo formato para la nueva factura de comercio en PDF en el programa Proveedor de soluciones en la nube (CSP) para mostrar la información de facturación por detalle del producto en lugar de la descripción de la SKU.

### <a name="impacted-audience"></a>Audiencia afectada

Partners que realizan transacciones mediante el programa CSP

### <a name="details"></a>Detalles

A partir de mayo de 2021, Microsoft presenta un nuevo formato para la nueva factura de comercio en PDF en el programa CSP para mostrar la información de facturación por detalle del producto en lugar de la descripción de la SKU. Con esta nueva actualización, agregaremos los elementos de línea por tipo de producto, al tiempo que se muestran todos los productos en una línea individual.

Los asociados observarán que este cambio entra en vigor en su factura de mayo del período de facturación entre el 1 y el 30 de abril de 2021. Las ofertas afectadas son instancia reservada de Microsoft Azure, suscripciones de Azure (plan de Azure) y Marketplace.

Las solicitudes de refacturación de crédito realizadas después de actualizar el formato de la factura se generará en el nuevo formato.

#### <a name="partner-benefits"></a>Ventajas para partners

Esta actualización ofrece las siguientes mejoras en la experiencia de facturación para asociados:

- Tamaño de factura reducido al tiempo que se conservan los datos críticos

- Alineación del formato a los estándares del sector para facturas compactas y fáciles de usar 

Los elementos siguientes no se verán afectados:

- Página de resumen de facturación en la factura en PDF

- API de facturación existentes

- Archivos de conciliación (los archivos de conciliación se pueden usar para recuperar datos granulares). 

- Facturas de cargos de uso y basadas en licencias

### <a name="next-steps"></a>Pasos siguientes

Revise la información sobre este tema en la [galería de recursos de preparación de operaciones](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) en el sitio web para asociados de Microsoft. Para más información sobre facturación e impuestos, así como recursos de facturación, facturas, facturación de CSP e impuestos, visite la [sección de facturación](https://docs.microsoft.com/partner-center/billing) del Centro de partners.

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a>Cambios en los requisitos de incorporación de clientes de Proveedor de soluciones en la nube (CSP)

### <a name="categories"></a>Categorías

- Fecha: 02/04/2021
- Ofertas/mercados

### <a name="summary"></a>Resumen

Como parte de nuestro compromiso para ayudar a los asociados y los clientes a llevar a cabo sus actividades empresariales basándose en la confianza, solicitaremos información adicional del cliente. Esto entrará en vigor el 25 de marzo de 2021.

### <a name="impacted-audience"></a>Audiencia afectada

Partners de factura directa y proveedores indirectos de CSP con clientes nuevos o existentes en los países que se indican en la sección siguiente

### <a name="details"></a>Detalles

Microsoft funciona con confianza. Nos comprometemos a proporcionar un método compatible, seguro y protegido para la validación de clientes durante las operaciones de transacción con suscripciones de clientes en el programa CSP. El 25 de marzo de 2021, presentaremos mejoras en la interfaz de usuario y la API del Centro de partners que afectarán a los partners que cumplan los criterios siguientes:

- El partner tiene una relación de factura directa con Microsoft (lo que significa que se trata de un partner de factura directa o de un proveedor indirecto).

- El asociado hace negocios con clientes nuevos o existentes en los siguientes países:

    - Tailandia
    - Vietnam
    - Turquía
    - Polonia
    - Sudáfrica
    - India
    - Brasil
    - Iraq
    - Myanmar
    - Sudán del Sur
    - Arabia Saudí
    - Emiratos Árabes Unidos
    - Venezuela

Los asociados que cumplan los criterios tendrán que enviar el identificador de registro de la compañía (también conocido como INN de la organización del cliente) y el número de teléfono del cliente la próxima vez que actualicen o creen una suscripción para ese cliente. Estos partners también pueden escribir un segundo nombre opcional para el cliente.

Tenga en cuenta que, al agregar el identificador de registro de la compañía, debe usar el id. de impuesto empresarial y no el identificador personal del cliente.

Los partners que llevan a cabo actividades empresariales con clientes nuevos o existentes de los países siguientes ya se incorporaron con una versión anterior en noviembre de 2020.

- Armenia
- Azerbaiyán
- Belarús
- Hungría
- Kazajistán
- Kirguistán
- Moldova
- Rusia
- Tayikistán
- Ucrania
- Uzbekistán

Los asociados con clientes en el resto del mundo podrán, a finales de marzo de 2021, escribir el identificador de registro de la compañía, el número de teléfono y el segundo nombre de los clientes como detalles opcionales.

### <a name="next-steps"></a>Pasos siguientes

- Revise la documentación técnica y las preguntas más frecuentes en la [colección específica para partners](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) a fin de obtener instrucciones más detalladas.
- Prepárese para incorporar los cambios mediante la API del Centro de partners y la experiencia de usuario web. Habrá API y SDK disponibles para realizar pruebas.
- Asegúrese de enviar los datos adicionales al incorporar clientes nuevos o modificar los datos de clientes existentes.
- Si usa una solución de proveedor de panel de control (CPV), consulte a su CPV.

### <a name="questions"></a>¿Tiene alguna pregunta?

Si tiene alguna pregunta relacionada con el identificador de registro de la compañía (también denominado INN o CIF/NIF), póngase en contacto con su asesor fiscal o con la agencia tributaria local. Microsoft no puede proporcionar orientación sobre cuestiones fiscales.

Si necesita soporte técnico con relación a sus operaciones con Microsoft, [abra una solicitud de servicio](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a>Ver ofertas y lanzamientos de productos de este mes

### <a name="categories"></a>Categorías

- Fecha: 01/04/2021
- Funcionalidades
 
### <a name="summary"></a>Resumen

Ya se ha publicado el calendario de lanzamientos de productos de abril de 2021.

### <a name="impacted-audience"></a>Audiencia afectada

Todos los partners que operan a través del programa Proveedor de soluciones en la nube (CSP)

### <a name="details"></a>Detalles

El [calendario de lanzamientos de productos](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) de abril de 2021 ya está disponible en la galería de recursos de preparación de operaciones. Vea los próximos lanzamientos de productos y ofertas aquí.

### <a name="next-steps"></a>Pasos siguientes

Revise el [calendario de lanzamientos de productos](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) y comparta esta información con las partes interesadas adecuadas de su organización.  

### <a name="questions"></a>¿Tiene alguna pregunta?

Si tiene alguna pregunta más sobre estas ofertas, consulte con las comunidades de Yammer correspondientes.
