---
title: Anuncios de marzo de 2021
description: Anuncios de marzo de 2021 para el Centro de partners de Microsoft, incluidas nuevas funcionalidades, promociones, ofertas, mercados o cambios en ofertas existentes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 04/02/2021
ms.openlocfilehash: 17b8082b8a42050892ff434010952d5f91a39431
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328073"
---
# <a name="march-2021-announcements"></a>Anuncios de marzo de 2021

En esta página se encuentran los anuncios del Centro de partners de Microsoft de marzo de 2021.

## <a name="readiness-changes-to-the-cloud-solution-provider-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="18"></a>Preparación: Los cambios en la API de validación de dirección de los clientes de Proveedor de soluciones en la nube (CSP) se pondrán en marcha en junio. La funcionalidad de pruebas ya está disponible.

### <a name="categories"></a>Categorías

- Fecha: 30/04/2021
- Preparación

### <a name="summary"></a>Resumen

Para ayudar a los partners y clientes a dirigir sus negocios basándose en la confianza, invitaremos a los partners a probar los cambios en la API de validación de direcciones para todos los países en todo el mundo.

### <a name="impacted-audience"></a>Audiencia afectada

Partners de facturación directa de CSP y proveedores indirectos que crean o actualizan los detalles actuales de dirección de los clientes.

### <a name="details"></a>Detalles

Microsoft funciona con confianza. Nos comprometemos a proporcionar un método compatible, seguro y protegido para la validación de la dirección de los clientes durante las operaciones de transacción con suscripciones de clientes en el programa CSP. A partir del 31 de marzo de 2021, hemos presentado cambios en la API de validación de direcciones, que invitamos a los partners a probar antes publicar los cambios en junio de 2021.

Los cambios solo afectan a la API de validación de direcciones. Las API de creación de clientes y actualización del perfil de facturación no se ven afectadas.

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

Una vez que se envía una dirección para su validación a través de la API de validación de direcciones, se devolverá el esquema de respuesta siguiente:

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

Eche un vistazo a esta respuesta de ejemplo. Tenga en cuenta que para EE. UU., si solo escribe cinco dígitos para el código postal, la respuesta devolverá un sufijo adicional de cuatro dígitos para la línea de código postal.

```csharp

"suggested_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Microsoft Way",
              "postal_Code": "98052-8300"
},
"original_address": {
              "Country": "US",
              "region": "WA",
              "city": "Redmond",
              "address_line1": "1 Micro Way",
              "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a>Pasos siguientes

- Comparta su id. de inquilino de espacio aislado con nuestro experto en la materia, Ali Khaki, para que se incluya en el piloto de prueba, de modo que pueda empezar a preparar la actualización.

- Si usa una solución de proveedor de panel de control (CPV), consulte a su CPV.

### <a name="questions"></a>¿Tiene alguna pregunta?

Si necesita soporte técnico para las operaciones con Microsoft, póngase en contacto con el grupo de Yammer del soporte técnico al partner.

### <a name="change-log"></a>Registro de cambios:

- 31 de marzo de 2020: Publicación original

- 30 de abril de 2021: Actualizaciones de la respuesta de ejemplo y los detalles del código postal

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a>Experiencia del nuevo Centro de administración de Exchange (EAC)

### <a name="categories"></a>Categorías

- Fecha: 29/03/2021
- Funcionalidades

### <a name="summary"></a>Resumen

A partir del 27 de abril de 2021, el Centro de administración de Exchange (EAC) implementará una nueva experiencia que mejorará la eficacia diaria de los usuarios.

### <a name="impacted-audience"></a>Audiencia afectada

Administradores delegados que acceden a Exchange a través del Centro de partners.

### <a name="details"></a>Detalles

A partir del 27 de abril de 2021, los asociados que naveguen a Exchange a través del Centro de partners se redirigirán al nuevo EAC.

Esta nueva experiencia está disponible actualmente como versión preliminar y los administradores pueden activarla seleccionando el botón de alternancia en la esquina superior derecha en el EAC clásico. También pueden navegar al nuevo EAC seleccionando el banner "Probar ahora" que se muestra en todas las páginas.

Entre las ventajas del nuevo EAC se incluyen:

- Se ha agregado información, informes y mecanismos de alerta para problemas relacionados con el flujo de correo. 

- Paneles personalizados para aumentar la productividad.

Para ayudarle a navegar por la nueva experiencia, puede encontrar vídeos en la sección **Entrenamiento y guía** en la nueva experiencia de EAC. Esto le proporcionará una visión general de cómo puede usar mejor el nuevo portal.

>[!NOTE]
>Con este cambio, la experiencia clásica de EAC no estará en desuso. Recibirá una notificación con antelación suficiente antes de que se implemente este cambio.

### <a name="next-steps"></a>Pasos siguientes

- Consulte los [recursos sobre este tema](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), donde puede ver capturas de pantallas de la nueva experiencia.

- Comparta esta información con las partes interesadas pertinentes de su organización. 

### <a name="questions"></a>¿Tiene preguntas?

Si tiene preguntas sobre estos cambios, consulte a las comunidades de Yammer correspondientes.

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a>Microsoft Operations: Presentación del calendario de lanzamiento del producto

### <a name="categories"></a>Categorías

- Fecha: 25/03/2021
- Ofertas / Modern Workplace

### <a name="summary"></a>Resumen

En respuesta a los comentarios de los asociados, Microsoft Operations simplificará las comunicaciones de los lanzamientos de productos.

### <a name="impacted-audience"></a>Audiencia afectada

Partners del programa Proveedor de soluciones en la nube (CSP)

### <a name="details"></a>Detalles

Microsoft se compromete a mejorar continuamente las experiencias de los asociados. Hemos recibido comentarios sobre el hecho de recibir demasiadas comunicaciones de Microsoft, incluidos anuncios duplicados de lanzamientos de productos.

En respuesta a sus comentarios, Microsoft ha simplificado la experiencia de preparación de los lanzamientos de productos para ofertas nuevas y existentes.

Ahora le proporcionamos una vista mensual única de los lanzamientos de productos publicados en la galería de recursos de preparación de operaciones. Esta [vista de calendario de lanzamientos de productos](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) mensual reemplazará las comunicaciones de lanzamiento de productos individuales en la galería de recursos de preparación de operaciones y en los anuncios del Centro de partners.

También puede acceder a este [calendario de lanzamientos de productos](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) desde [colecciones de la comunidad](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [vistas de calendario](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated) y [boletines de CSP](https://partner.microsoft.com/resources/collection/csp-monthly-update#/). Recibirá una notificación cuando publiquemos el calendario de lanzamientos de productos de cada mes con un anuncio en la galería de recursos de preparación de operaciones.

Todavía puede encontrar información sobre ofertas nuevas y existentes en la vista previa de la lista de precios y en los registros de cambios de la lista de precios, así como en blogs de productos, guías de licencia y páginas de marketing del producto.

El cambio se aplicará a los lanzamientos de los siguientes productos:

- Dynamics local
- Microsoft 365
- Microsoft Dynamics 365
- Windows
- Servidor  
- Herramientas
- Teams y Telco

Seguiremos enviando anuncios específicos de lanzamientos de productos que requieran detalles de preparación de operaciones.

### <a name="next-steps"></a>Pasos siguientes

Revise los recursos sobre este tema y comparta esta información con las partes interesadas adecuadas de su organización.

### <a name="questions"></a>¿Tiene alguna pregunta?

Si tiene alguna pregunta más sobre estas ofertas, consulte con las comunidades de Yammer correspondientes.

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a>Cambios en los requisitos de incorporación de clientes de CSP

### <a name="categories"></a>Categorías

- Fecha: 25/03/2021
- Funcionalidades

### <a name="summary"></a>Resumen

Como parte de nuestro compromiso para ayudar a los asociados y los clientes a llevar a cabo sus actividades empresariales basándose en la confianza, solicitaremos información adicional del cliente. Esto entrará en vigor el 25 de marzo de 2021.

### <a name="impacted-audience"></a>Audiencia afectada

Los asociados de CSP Direct Bill Partner y proveedores indirectos del Proveedor de soluciones en la nube (CSP) con clientes nuevos o existentes en los países que se indican en la sección siguiente.

### <a name="details"></a>Detalles

Microsoft funciona con confianza. Nos comprometemos a proporcionar un método compatible, seguro y protegido para la validación de clientes durante las operaciones de transacción con suscripciones de clientes en el programa CSP. El 25 de marzo de 2021, presentaremos mejoras en la interfaz de usuario y la API del Centro de partners que afectarán a los partners que cumplan los criterios siguientes:

1. El partner tiene una relación de factura directa con Microsoft (lo que significa que se trata de un partner de factura directa o de un proveedor indirecto).

2. El asociado hace negocios con clientes nuevos o existentes en los siguientes países:

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

Los asociados que cumplan los criterios tendrán que enviar el **identificador de registro de la compañía** (también conocido como **INN de la organización** del cliente) y el **número de teléfono** del cliente cuando incorporen clientes nuevos o modifiquen los detalles de clientes existentes. Estos partners también pueden escribir un **segundo nombre** opcional para el cliente.

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

Los asociados con clientes en el resto del mundo podrán, a partir del 25 de marzo de 2021, escribir el **identificador de registro de la compañía**, el **número de teléfono** y el **segundo nombre** de los clientes como detalles opcionales.

### <a name="next-steps"></a>Pasos siguientes

- Revise la documentación técnica y las preguntas más frecuentes en la [colección específica para asociados](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) a fin de obtener instrucciones más detalladas.

- Prepárese para incorporar los cambios mediante la API del Centro de partners y la experiencia de usuario web. Habrá API y SDK disponibles para realizar pruebas.

- Asegúrese de enviar los datos adicionales al incorporar clientes nuevos o modificar los datos de clientes existentes.

- Si usa una solución de proveedor de panel de control (CPV), consulte a su CPV.

### <a name="questions"></a>¿Tiene alguna pregunta?

Si tiene alguna pregunta relacionada con el identificador legal (también denominado INN o CIF/NIF), póngase en contacto con su asesor fiscal o con la agencia tributaria local. Microsoft no puede proporcionar orientación sobre cuestiones fiscales.

Si necesita soporte técnico con relación a sus operaciones con Microsoft, [abra una solicitud de servicio](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>Correcciones realizadas a la lista de precios de software perpetuo del 1 de marzo de 2021

### <a name="categories"></a>Categorías

- Fecha: 23/03/2021
- Ofertas/mercados

### <a name="impacted-audience"></a>Audiencia afectada

Proveedores indirectos y partners directos de facturación que realicen transacciones de software perpetuo en el programa Proveedor de soluciones en la nube 

### <a name="details"></a>Detalles

La lista de precios para el software perpetuo publicada el 1 de marzo de 2021 incluía mercados que no deberían estar allí. La lista de precios de software perpetuo se actualizó el 17 de marzo de 2021 con las correcciones. Estas correcciones solo se aplican a:

- Id. de producto: DF77X4D43RKT 
- Nombre del producto: actualización de Windows 10 Home a Pro para Microsoft 365 Empresa
- Mercados quitados o no admitidos: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW

Estos cambios solo se aplican al producto anterior. Otros productos no tenían correcciones. 

### <a name="next-steps-and-resources"></a>Pasos y recursos siguientes

- Los partners que realizan transacciones de software perpetuo deben descargar la lista de precios de software perpetuo más reciente.
- Consulte los [códigos de país de la región](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) para una asignación descriptiva de la abreviatura de dos letras a los países.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a>Versión del SDK en .NET Standard (v1.17.0)

### <a name="categories"></a>Categorías

- Fecha: 23/03/2021

- Funcionalidades
 
### <a name="impacted-audience"></a>Audiencia afectada

Partners de factura directa y proveedores indirectos que participan en el programa CSP y que usan el SDK de .NET del Centro de partners.

### <a name="details"></a>Detalles

A partir del 23 de marzo de 2020, los partners pueden empezar a descargar la versión de [MicrosoftPartnerCenter.NETSDK (galería de NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), junto con los [ejemplos de GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples) actualizados públicos del SDK del Centro de partners. Esta versión incluye actualizaciones para los métodos siguientes:

#### <a name="audit-updated-new-operation-types"></a>Auditoría actualizada: nuevos tipos de operación

Se han agregado nuevos [tipos de operación](https://docs.microsoft.com/partner-center/develop/auditing-resources) para saber cuándo el cliente ha aprobado y finalizado DAP.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Auditoría actualizada: nuevos tipos de recursos y operaciones

Se han agregado nuevos [tipos de recursos y operaciones](https://docs.microsoft.com/partner-center/develop/auditing-resources) para admitir el escenario de rol del directorio del cliente.

- Nuevo tipo de recurso "CustomerDirectoryRole"

- Tipos de operación "AddUserMember" y "RemoveUserMember"

#### <a name="sdk-updates-to-customer-accounts"></a>Actualizaciones del SDK para cuentas de cliente

- Compatibilidad con GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus

- GET /customers/{customer-tenant-id}/qualifications

- POST /customers/{customer_id}/qualifications?code={validationCode}

#### <a name="additional-changes"></a>Cambios adicionales

Los cambios siguientes se incluyen como parte del nuevo comercio y actualmente están disponibles por invitación solo para los partners que forman parte de la versión preliminar técnica de la experiencia del nuevo comercio de M365/D365. Los partners que no forman parte de la versión preliminar técnica del nuevo comercio no deberían notar los impactos y deberían ser compatibles con versiones anteriores.

- Cambios en el catálogo:

  - GET /products/{product-id}/skus/{sku-id}

- Compra y administración:
  - GET /customers/{customerId}/subscriptions
  - GET /customers/{customerId}/subscriptions/{subscriptionId}
  - PATCH /customers/{customerId}/subscriptions/{subscriptionId}
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>Pasos siguientes

- Descargue la versión más reciente de [MicrosoftPartnerCenter.NETSDK (galería de NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0).
- Descargue y revise los [ejemplos de GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples).

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>Oferta del marketplace comercial para CSP e incentivos de CSP para ofertas válidas en el año fiscal 2021

### <a name="categories"></a>Categorías

- Fecha: 18/03/2021
- Funcionalidades

### <a name="impacted-audience"></a>Audiencia afectada

Proveedores indirectos y partners de factura directa del programa Proveedor de soluciones en la nube 

### <a name="details"></a>Detalles

Los proveedores indirectos y los partners de factura directa del programa Proveedor de soluciones en la nube pueden vender ofertas de terceros y obtener un incentivo de descuento por cada oferta de terceros apta cuya transacción se realice en el Centro de partners o en Azure Portal. El incentivo será en forma de descuento en las ventas facturadas de las ofertas aptas y estará **disponible hasta el 30 de junio de 2021**.  

Obtenga más información sobre este incentivo de la oferta del marketplace comercial de CSP más abajo, y póngase en contacto con sus clientes hoy mismo para identificar las ofertas adecuadas para facilitar su éxito y transformación digital.

Nos hemos asociado con fabricantes de software independientes (ISV) para incorporar las soluciones de IaaS y SaaS más recientes al mercado de los clientes de Microsoft. Los editores de ISV tienen la opción de permitir las ventas de sus ofertas a través del canal de partners de Microsoft. Nuestras ofertas aptas para incentivos se dividen en dos categorías:

- Seleccione las ofertas de terceros de SaaS e IaaS con el estado de incentivo de venta conjunta de IP de Azure. 

- Aplicaciones SaaS integradas con Teams o al menos dos aplicaciones de productividad de Microsoft 365, como PowerPoint, Word, Excel, Outlook o SharePoint.

### <a name="next-steps-and-resources"></a>Pasos y recursos siguientes

- Obtenga información sobre la obtención de [incentivos para partners](https://partner.microsoft.com/membership/partner-incentives) por la venta de aplicaciones aptas del marketplace. Las nuevas ofertas se agregan mensualmente.  
- [Recursos de incentivos para partners de factura directa del Proveedor de soluciones en la nube](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Recursos de incentivos para proveedores indirectos del Proveedor de soluciones en la nube](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Revise esta [presentación](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) para obtener más información sobre cómo vender las aplicaciones del marketplace comercial. Consulte [aquí](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/) los recursos adicionales. 
- Explore el catálogo del marketplace comercial en el [Centro de partners](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) o en [Azure Portal](https://ms.portal.azure.com/#home).
- Use las [API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) para integrar aplicaciones en el marketplace de su empresa.
- Póngase en contacto con los fabricantes de software independientes con los que está interesado en tener relaciones comerciales.
- Los proveedores indirectos deben integrarse con las API y guiar a los revendedores en qué aplicaciones se deben vender.

### <a name="questions"></a>¿Alguna pregunta?  

Consulte [este artículo](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) para obtener información general sobre el marketplace comercial en el Centro de partners.

Si necesita más ayuda, puede crear una solicitud de soporte técnico en el Centro de partners. Obtenga más información en [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Actualización de nomenclatura de ofertas y de requisitos previos de Power BI Premium

### <a name="categories"></a>Categorías

- Fecha: 18/03/2021
- Funcionalidades

### <a name="summary"></a>Resumen

La lista final de precios del 1 de abril de 2021 se actualizará para agregar claridad a la información de nomenclatura o requisitos previos para las ofertas de Power BI Premium por usuario.

### <a name="impacted-audience"></a>Audiencia afectada

Partners directos e indirectos del programa Proveedor de soluciones en la nube (CSP)

### <a name="details"></a>Detalles

La lista final de precios del 1 de abril de 2021 se actualizará para agregar claridad a la información de nomenclatura o requisitos previos para las ofertas de Power BI Premium por usuario.

Hasta que se actualice la lista final de precios, use la información de esta sección para asegurarse de que se pida el producto correcto.

Los detalles siguientes muestran la SKU afectada y los detalles de los requisitos previos.

| Nombre para mostrar de la oferta en la versión preliminar de la lista de precios del 1 de marzo |  Nombre para mostrar de la oferta actualizada del 1 de abril de la lista final de precios| Id. de oferta |
| ------ | ----------- | ----------- |
| Complemento Power BI Premium por usuario (precios para personal de ONG)  |  Complemento de Power BI Premium por usuario **(Office)** (precios para personal de organizaciones sin ánimo de lucro)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Los clientes deben cumplir alguno de los siguientes requisitos previos para comprar esta oferta:

| Nombre para mostrar de la oferta | Id. de oferta |
| ------ | ----------- |
| Microsoft 365 E5 (precios para personal de organizaciones sin ánimo de lucro)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 sin audioconferencia (precios para personal de organizaciones sin ánimo de lucro)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (precios para personal de organizaciones sin ánimo de lucro)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Versión de evaluación de Office 365 E5 (precios para personal de organizaciones sin ánimo de lucro)|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Office 365 E5 sin audioconferencia (precios para personal de organizaciones sin ánimo de lucro)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

La siguiente oferta de Power BI Premium tiene un requisito previo para la compra:

| Nombre para mostrar de la oferta | Id. de oferta |
| ------ | ----------- |
|   Complemento Power BI Premium por usuario (precios para personal de ONG)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

Los clientes deben tener este requisito previo para comprar esta oferta:

| Nombre para mostrar de la oferta | Id. de oferta |
| ------ |----------|
| Power BI Pro (precios para personal de organizaciones sin ánimo de lucro)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Pasos siguientes

Revise los recursos sobre este tema y comparta esta información con las partes interesadas adecuadas de su organización.  

### <a name="questions"></a>¿Tiene alguna pregunta?

Si tiene preguntas sobre estas ofertas, consulte a las comunidades de Yammer correspondientes. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> Actualizaciones de precios de marzo de Microsoft 365 F3

### <a name="categories"></a>Categorías

- Fecha: 16/03/2021
- Ofertas/mercados

### <a name="summary"></a>Resumen

Se han corregido los precios incorrectos de marzo de 2021 para Microsoft 365 F3 en libras (GBP) y euros (EUR).

### <a name="impacted-audience"></a>Audiencia afectada

Los partners que compren Microsoft 365 F3 en GBP o EUR entre el 1 de marzo y el 17 de marzo de 2021 a través del programa Proveedor de soluciones en la nube (CSP).

### <a name="details"></a>Detalles

Microsoft ha solucionado los precios incorrectos para Microsoft 365 F3. Los precios incorrectos eran para GBP y EUR, y solo para las ofertas adquiridas entre el 1 de marzo y el 17 de marzo de 2021. A continuación, se muestran las ofertas y las monedas afectadas. 

| Nombre de la oferta | Moneda | Id. de oferta | Id. de material |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (ONG) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (comercial) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
Las listas de precios basados en licencias de la versión preliminar de marzo y abril se actualizaron el 16 de marzo, a las 17:00 horas (hora estándar del Pacífico).

### <a name="next-steps"></a>Pasos siguientes

- Los partners deben volver a descargar las listas de precios actuales basados en licencias, tanto de la versión preliminar de marzo como de abril, con las correcciones de precios, si procede.  
- Microsoft se pondrá en contacto con los partners afectados en las próximas semanas a través del correo electrónico para informarles sobre los siguientes pasos relacionados con la corrección de las transacciones afectadas.

### <a name="questions"></a>¿Tiene alguna pregunta?

Si tiene alguna pregunta, póngase en contacto con las comunidades de Yammer de CSP correspondientes.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> Actualización de la razón social de una empresa a través del Centro de partners

### <a name="categories"></a>Categorías

- Fecha: 16/03/2021
- Impulsar la eficiencia y la escala

### <a name="summary"></a>Resumen

A partir de marzo de 2021, los partners de Microsoft Partner Network (MPN) y los revendedores indirectos del Proveedor de soluciones en la nube (CSP) pueden actualizar la razón social de su empresa a través del Centro de partners.

### <a name="impacted-audience"></a>Audiencia afectada

Partners de MPN y revendedores indirectos de CSP (no aplicables a partners de facturación directa de CSP)

### <a name="details"></a>Detalles

A partir de marzo de 2021, los partners de MPN y los revendedores indirectos de CSP pueden actualizar la razón social de su empresa a través del Centro de partners por su cuenta y conforme a la normativa. Con esta nueva característica, los partners ya no tendrán que enviar una incidencia de soporte técnico del Centro de partners para actualizar el nombre de su empresa. Esto ahorrará una cantidad significativa de tiempo a los asociados al realizar estas actividades. 

Para más información, consulte [Actualización del perfil legal de la empresa](../update-your-partner-profile.md#update-your-legal-business-profile).

>[!NOTE]
>Asegúrese de que el nombre de la empresa en el perfil empresarial legal no tenga errores ortográficos ni abreviaturas, y de que coincida exactamente con los registros de inscripción formales de la empresa. Para obtener más información sobre cómo actualizar el perfil de la organización, consulte [Verificación del perfil de la organización](../update-your-partner-profile.md#update-your-legal-business-profile).

### <a name="next-steps"></a>Pasos siguientes

Comparta esta información en su organización para que el equipo adecuado pueda revisar y actualizar sus procesos.

### <a name="questions"></a>¿Alguna pregunta?

Si tiene alguna pregunta, póngase en contacto con las comunidades de Yammer de CSP correspondientes.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Actualización de la evolución del programa Proveedor de soluciones en la nube (CSP) y cambios en el programa Open License

### <a name="categories"></a>Categorías

- Fecha: 15/03/2021
- Funcionalidades

### <a name="summary"></a>Resumen

Se incorporarán nuevas ofertas de software perpetuo del sector comercial y público en el programa Proveedor de soluciones en la nube (CSP) y se realizarán cambios en el programa de licencias Open.

### <a name="impacted-audience"></a>Audiencia afectada

Distribuidores comerciales y revendedores administrados que venden productos a través del programa Open License, así como todos los partners de CSP que realizan transacciones con el software perpetuo

### <a name="details"></a>Detalles

En septiembre de 2020, Microsoft [anunció](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) una serie de pasos en nuestro recorrido de transformación digital para expandir las oportunidades de los partners en el programa CSP, incluida la disponibilidad del software local para los partners. Estos cambios permiten a los partners hacer crecer su empresa y ampliar su alcance, ya que aprovechan las licencias de software de CSP y las posicionan para que logren el éxito en el mundo actual en el que se da prioridad a la nube. También permiten transiciones de los clientes a la nube y ofrecen a los partners la flexibilidad necesaria para los entornos de nube híbrida de los clientes.

A fin de continuar con esta transformación digital, presentamos los siguientes cambios:

- 1 de julio de 2021: no se agregarán nuevas SKU, productos ni promociones a la lista de precios del programa Open License.

- 7 de julio de 2021: se agregarán dos ofertas comerciales (Get Genuine Windows y Visual Studio Professional) y ofertas del sector público (gobierno, educación y sin ánimo de lucro; consulte el [anuncio](./2020-december.md#9)) a la lista de precios del software perpetuo de CSP.  La lista de precios puede encontrarse en la sección Software de la página [Vender > Precios y ofertas](https://partnercenter.microsoft.com/pcv/sales) del Centro de partners y se volverá a publicar en esta fecha.

Para obtener detalles completos sobre la evolución del programa CSP y los cambios en el programa Open License, consulte **los siguientes pasos** .

### <a name="next-steps"></a>Pasos siguientes:

- Evolución del programa CSP: revise los materiales de preparación para el [software perpetuo del programa Proveedor de soluciones en la nube](https://partner.microsoft.com/resources/collection/software-in-csp#/). Use este [mapa de preparación](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) para localizar rápidamente la información adecuada para su rol.

- Cambios en el programa Open License: revise los materiales de preparación sobre la [evolución del programa CSP y los cambios en el programa Open License](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/). Use este [mapa de preparación](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) para localizar rápidamente la información adecuada para su rol.

### <a name="questions"></a>Preguntas

Si tiene alguna pregunta, póngase en contacto con las comunidades de Yammer de CSP correspondientes.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Actualización de un anuncio anterior: evaluaciones prémium, un complemento para el Administrador de cumplimiento

### <a name="categories"></a>Categorías

- Fecha: 15/03/2021
- Desarrollo de la empresa

### <a name="summary"></a>Resumen

Las ofertas de prueba no deben aparecer en la lista de precios y se quitarán.

### <a name="impacted-audience"></a>Audiencia afectada

Todos los partners que realizan transacciones a través del Proveedor de soluciones en la nube (CSP).

### <a name="details"></a>Detalles

Las ofertas de prueba no se deberían haber incluido en la lista de precios. Se quitarán de la lista de precios del 1 de mayo de 2021.

El anuncio original se encuentra [aquí](./2021-february.md#4).

### <a name="additional-resources"></a>Recursos adicionales

- [Seguridad y cumplimiento de Microsoft 365 E5](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Creación y administración de evaluaciones en el Administrador de cumplimiento de Microsoft: Cumplimiento de Microsoft 365](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Pasos siguientes

Revise los recursos sobre este tema y comparta esta información con las partes interesadas adecuadas de su organización.

### <a name="questions"></a>¿Tiene alguna pregunta?

Si tiene preguntas sobre estas ofertas, consúltelas a las comunidades de Yammer correspondientes.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Migre sus soluciones de comercialización (GTM) de One Commercial Partner (OCP) al marketplace comercial de Microsoft

### <a name="categories"></a>Categorías

- Fecha: 12/03/2021
- Funcionalidades

### <a name="summary"></a>Resumen

A partir del 29 de marzo de 2021, las funcionalidades de la herramienta de comercialización (GTM) de One Commercial Partner (OCP) se empezarán a ofrecer de forma limitada. Le recomendamos que migre sus soluciones al marketplace comercial en el Centro de partners.

### <a name="impacted-audience"></a>Audiencia afectada

Organizaciones que venden de forma conjunta las soluciones de GTM de OCP

### <a name="details"></a>Detalles

En diciembre de 2020, iniciamos nuestra transición de la herramienta de GTM de OCP de Microsoft al marketplace comercial de Microsoft en el Centro de partners. Este cambio amplía las funcionalidades del marketplace comercial, en el que puede presentar sus soluciones a millones de clientes, compartir de forma bidireccional las oportunidades con otros vendedores de Microsoft y partners y vender de manera conjunta soluciones innovadoras.

El siguiente hito de la transición tendrá lugar el 29 de marzo de 2021. Será en ese momento cuando las funcionalidades de GTM de OCP se ofrecerán de manera limitada y algunos campos pasarán a ser de solo lectura. Si actualmente vende de forma conjunta soluciones en la herramienta de GTM de OCP, le recomendamos que migre sus soluciones al marketplace comercial para aprovechar sus funcionalidades y simplificar la experiencia de publicación. 

Al cambiar al marketplace comercial, el Centro de partners se convertirá en el destino principal de la experiencia de publicación de venta conjunta. Desde allí podrá seguir desarrollando su empresa, ya que podrá conectar sus soluciones con nuestros clientes compartidos a través de los mismos canales y experiencias en el producto que usamos para los productos de Microsoft. [Obtenga información sobre el marketplace comercial](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).

### <a name="next-steps"></a>Pasos siguientes

- Si aún no ha trasladado sus soluciones, siga las instrucciones detalladas en la [guía de transición](/azure/marketplace/co-sell-solution-migration) o consulte el [tutorial detallado de vídeo](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) para completar todas las actividades de migración y empezar a publicar sus soluciones en el marketplace comercial.

- Si tiene preguntas sobre cómo será su experiencia con las funcionalidades limitadas de GTM de OCP, vea los [Requisitos de venta conjunta para publicar en las preguntas más frecuentes sobre el marketplace comercial de Microsoft](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf). (Consulte la sección "Funcionalidades limitadas de GTM de OCP a partir del 29 de marzo de 2021").

### <a name="questions"></a>¿Tiene alguna pregunta?

Póngase en contacto con el [soporte técnico](https://partner.microsoft.com/support/?stage=1) si tiene alguna pregunta o necesita más información.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Expansión de la nueva experiencia comercial en el programa Proveedor de soluciones en la nube (CSP) de Azure a Rusia

### <a name="categories"></a>Categorías

- Fecha: 10/03/2021
- Funcionalidades

### <a name="impacted-audience"></a>Audiencia afectada

Todos los partners de Rusia que realizan transacciones a través del programa Proveedor de soluciones en la nube (CSP).

### <a name="details"></a>Detalles

Nos complace anunciar que la **nueva experiencia de comercio en CSP para Azure en Rusia** estará disponible a partir del 10 de marzo de 2021. Esta experiencia simplificará y mejorará la forma en que los clientes compran y consumen los servicios de Azure. También proporcionará a los partners del programa CSP una vista coherente de los precios de Azure a través de los movimientos de ventas, los precios de USD para la coherencia global, la concordancia de las fechas de facturación y el acceso a Azure Cost Management.

### <a name="next-steps"></a>Pasos siguientes

Hay varios recursos disponibles que presentan la nueva experiencia de comercio de Azure y proporcionan información adicional. Busque las preguntas más frecuentes, los conjuntos de diapositivas, los vídeos, etc. más recientes en la [Galería de recursos de actualizaciones de programas de CSP](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>Suministro de descargas y claves de licencia de software del Centro de partners

### <a name="categories"></a>Categorías

- Fecha: 04/03/2021
- Funcionalidades

### <a name="summary"></a>Resumen

Se ha restablecido la funcionalidad de suministro de descargas y claves de licencia de software del Centro de partners.

### <a name="impacted-audience"></a>Audiencia afectada

Todos los partners que sean Proveedores de soluciones en la nube (CSP) que operen con pedidos de software de suscripción perpetua y de servidor a través del Centro de partners

### <a name="details"></a>Detalles

En respuesta a los comentarios de los partners, estamos restableciendo la funcionalidad de suministro del Centro de partners para obtener software y claves de licencia para los pedidos de software de suscripción perpetua y de servidor. Se restaurará a su estado previo antes de que se elimine el 19 de enero de 2021. (Vea el [anuncio](2020-september.md#17)).

Tenga en cuenta que las claves de licencia de software y los vínculos de descarga son recursos de propiedad intelectual valiosos y muy solicitados. Si se filtran, se pueden agotar rápidamente sus límites de activación, lo que puede provocar una experiencia negativa para clientes y partners.

### <a name="next-steps"></a>Pasos siguientes

Revise los siguientes recursos para obtener instrucciones de uso e información importante sobre la distribución de las claves de software:

- [Venta de software local a través del programa CSP](../csp-on-premise-software.md)
- [Nueva guía de operaciones comerciales del Centro de partners](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (consulte la sección **Guía sobre la distribución de claves de software**).

### <a name="questions"></a>¿Tiene alguna pregunta?

Si tiene alguna pregunta más sobre este aviso, consulte con las comunidades de Yammer correspondientes.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Migración de las ofertas de Partner Sales Connect (PSC) al Centro de partners

### <a name="categories"></a>Categorías

- Fecha: 04/03/2021
- Funcionalidades

### <a name="summary"></a>Resumen

Partner Sales Connect (PSC) se moverá a acceso de solo lectura a partir del 31 de marzo de 2021, por lo que le recomendamos que comience a migrar sus ofertas de PSC al Centro de partners.

### <a name="impacted-audience"></a>Audiencia afectada

Partners con ofertas en PSC

### <a name="details"></a>Detalles

Como parte de nuestro compromiso compartido con el crecimiento, la **venta conjunta con Microsoft** es el camino para que **le descubran, ofrezca sus conocimientos y amplíe su variedad de clientes** para obtener resultados positivos para estos. Con una oferta media que es **3,5 veces más rápida** que la normal, la administración de la experiencia de venta conjunta en el Centro de partners le permite vender a través de los canales de cliente directo, partner y vendedor de Microsoft, y administrar toda la canalización de referencia en una sola ubicación.

**PSC** pasará a **acceso de solo lectura** a partir del **31 de marzo de 2021**, por lo que le recomendamos que empiece el traslado al Centro de partners y acceda a estas mejoras en la funcionalidad: 

- **Enrutamiento más preciso** de las ofertas que comparte con Microsoft hacia el vendedor adecuado, en función del tipo de ayuda que necesite.
- **Validación de idoneidad de ofertas iniciales** para las soluciones aptas para incentivos y para cumplir los criterios del programa ISV Connect, al simplificar el proceso de aprobación y la atestación de prueba de ejecución (PoE) final.
- **Experiencia de usuario sin problemas** para administrar todas las oportunidades de venta conjunta y clientes potenciales cualificados para ventas en un solo lugar.

Además, recientemente hemos agregado nuevas características al Centro de partners para ayudarle en el traslado:

- [Operaciones masivas para las oportunidades de venta conjunta](../bulk-operations.md)
- [Característica de migración de ofertas](../psc-to-pc.md) (consulte la sección **Migración de contratos de PSC**).

Con la experiencia de venta conjunta en el Centro de partners, los equipos de ventas tendrán más tiempo para centrarse en fomentar la captación de clientes potenciales y oportunidades, cerrar acuerdos y crear relaciones duraderas con los clientes.

### <a name="next-steps"></a>Pasos siguientes

Use la [guía de transición](../psc-to-pc.md) del Centro de partners para conocer por los pasos necesarios para migrar sus ofertas de PSC al Centro de partners.

### <a name="questions"></a>¿Tiene alguna pregunta?

Si tiene más preguntas, póngase en contacto con [Soporte técnico](https://partner.microsoft.com/support/?stage=1).

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Nuevos productos y ofertas de Microsoft Dynamics 365 disponibles el 1 de abril de 2021

### <a name="categories"></a>Categorías

- Fecha: 04/03/2021
- Funcionalidades

### <a name="summary"></a>Resumen

El 1 de abril de 2021, Microsoft lanzará varios productos y ofertas nuevos para el programa Proveedor de soluciones en la nube (CSP).

### <a name="impacted-audience"></a>Audiencia afectada

Todos los partners que operan a través del programa Proveedor de soluciones en la nube (CSP)

### <a name="details"></a>Detalles

El 1 de abril de 2021, Microsoft lanzará los siguientes nuevos productos y ofertas:

- Power BI Premium por usuario
- Expansión geográfica y por segmento de USL de Customer Voice y Marketing

**Power BI Premium por usuario**

Microsoft presentará las primeras ofertas de Power BI Premium por usuario. Actualmente, Power BI Premium se vende solo en una construcción de capacidad. Power BI Premium por usuario proporciona acceso a las funcionalidades empresariales de business intelligence (BI) y análisis. Su oferta de licencias flexible e individual por puesto está dirigida a pequeñas y medianas empresas.

Revise los [detalles de la versión de Power BI](/power-platform-release-plan/2020wave2/power-bi/planned-features) para obtener más información sobre esta oferta.


**Detalles de la oferta**

Tenga en cuenta que el nombre de la oferta difiere ligeramente de la vista previa de la lista de precios.

| Nombre de la oferta | Id. de oferta |
| ------ |----------- |
| Power BI Premium por usuario | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium por usuario para profesores | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium por usuario para estudiantes | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium por usuario (precios para personal de ONG) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Complemento de Power BI Premium por usuario | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Complemento de Power BI Premium por usuario para profesores | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Complemento de Power BI Premium por usuario para estudiantes | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Complemento Power BI Premium por usuario (precios para personal de ONG) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Expansión geográfica y por segmento de USL de Customer Voice y Marketing**

Como seguimiento del lanzamiento de diciembre de 2020, se han cambiado las ofertas de USL de Dynamics 365 Customer Voice y Marketing para agregar nuevos países y más SKU de educación y ONG.

| Nombre de la oferta | Id. de oferta |
| ------ |----------- |
| USL de Dynamics 365 Customer Voice (precios para personal de ONG) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| USL de Dynamics 365 Customer Voice para profesores | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Para obtener más información sobre estas ofertas, visite las páginas siguientes:

- [Página principal de Dynamics 365 Customer Voice](https://dynamics.microsoft.com/customer-voice/overview/)
- [Página principal de Dynamics 365 Marketing](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Pasos siguientes

Revise los recursos sobre este tema y comparta esta información con las partes interesadas adecuadas de su organización.  

### <a name="questions"></a>¿Tiene alguna pregunta?

Si tiene preguntas sobre estas ofertas, consulte a las comunidades de Yammer correspondientes. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> Impresión universal de Microsoft ahora está disponible en algunos conjuntos de aplicaciones

### <a name="categories"></a>Categorías

- Fecha: 31/03/2021
- Funcionalidades

### <a name="summary"></a>Resumen

Impresión universal de Microsoft estará disponible para operaciones dentro de ciertos conjuntos de aplicaciones de Microsoft 365 y como complemento independiente a partir del 1 de marzo de 2021.

### <a name="impacted-audience"></a>Audiencia afectada

Todos los partners que operan a través del programa Proveedor de soluciones en la nube (CSP)

### <a name="details"></a>Detalles

[Impresión universal](https://aka.ms/universalprint) es un servicio de impresión de Microsoft 365 que elimina la necesidad de servidores de impresión locales, y permite que los dispositivos Windows impriman en impresoras registradas en Azure. Estará disponible para operar desde el 1 de marzo de 2021.

Los trabajadores se benefician de una impresión sin controladores, una detección de impresoras basada en ubicaciones y una experiencia de impresión intuitiva sin curva de aprendizaje. Los dispositivos que están unidos a Azure Active Directory (Azure AD) usan credenciales de Azure AD existentes para imprimir de forma segura. Los administradores administran la impresión mediante Azure Portal y pueden conectar fácilmente las impresoras con la compatibilidad nativa con Impresión universal. Impresión universal se puede implementar con impresoras no compatibles mediante el software del conector de Impresión universal.

Impresión universal se incluirá en un comienzo en Windows E3, A3, E5 y A5, y Microsoft 365 BP, F3, E3, A3, E5 y A5.  

**Detalles de la oferta**

Tenga en cuenta que el nombre de la oferta difiere ligeramente de la vista previa de la lista de precios.

| Nombre de la oferta | Id. de oferta | Id. de material |
| ------ |----------- |----------- |  
| Complemento de volumen de Impresión universal (500 trabajos): Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Complemento de volumen de Impresión universal (500 trabajos) para profesores: Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Complemento de volumen de Impresión universal (500 trabajos): Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| Complemento de volumen de Impresión universal (500 trabajos) para profesores: Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Pasos siguientes

Familiarícese con la lista de precios y la [Introducción a Impresión universal](/universal-print/fundamentals/universal-print-whatis). Comparta esta información con todos los contactos de su organización a quienes corresponda.

### <a name="questions"></a>¿Alguna pregunta?

Si tiene preguntas sobre estas ofertas, consulte a las comunidades de Yammer correspondientes.
