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
ms.openlocfilehash: d26d1af994ae9a3f951ee9428ee6fd092b2c91d8
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328056"
---
# <a name="april-2021-announcements"></a><span data-ttu-id="204bd-103">Anuncios de abril de 2021</span><span class="sxs-lookup"><span data-stu-id="204bd-103">April 2021 announcements</span></span>

<span data-ttu-id="204bd-104">En esta página se encuentran los anuncios del Centro de partners de Microsoft de abril de 2021.</span><span class="sxs-lookup"><span data-stu-id="204bd-104">This page provides the announcements for Microsoft Partner Center for April 2021.</span></span>

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a><span data-ttu-id="204bd-105">Preparación: Se ha actualizado la API de validación de direcciones de clientes de CSP que se publicará en junio. La funcionalidad de pruebas ya está disponible.</span><span class="sxs-lookup"><span data-stu-id="204bd-105">Readiness: Updated CSP customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="204bd-106">Categorías</span><span class="sxs-lookup"><span data-stu-id="204bd-106">Categories</span></span>

- <span data-ttu-id="204bd-107">Fecha: 30/04/2021</span><span class="sxs-lookup"><span data-stu-id="204bd-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="204bd-108">Preparación</span><span class="sxs-lookup"><span data-stu-id="204bd-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="204bd-109">Resumen</span><span class="sxs-lookup"><span data-stu-id="204bd-109">Summary</span></span>

<span data-ttu-id="204bd-110">Para ayudar a los partners y clientes a dirigir sus negocios basándose en la confianza, invitaremos a los partners a probar los cambios en la API de validación de direcciones para todos los países en todo el mundo.</span><span class="sxs-lookup"><span data-stu-id="204bd-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="204bd-111">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="204bd-111">Impacted audience</span></span>

<span data-ttu-id="204bd-112">Partners de facturación directa de CSP y proveedores indirectos que crean o actualizan los detalles actuales de dirección de los clientes.</span><span class="sxs-lookup"><span data-stu-id="204bd-112">CSP direct bill partners and indirect providers who create new or update existing customers’ address details</span></span>

### <a name="details"></a><span data-ttu-id="204bd-113">Detalles</span><span class="sxs-lookup"><span data-stu-id="204bd-113">Details</span></span>

<span data-ttu-id="204bd-114">Microsoft funciona con confianza.</span><span class="sxs-lookup"><span data-stu-id="204bd-114">Microsoft runs on trust.</span></span> <span data-ttu-id="204bd-115">Nos comprometemos a proporcionar un método compatible, seguro y protegido para la validación de la dirección de los clientes durante las operaciones de transacción con suscripciones de clientes en el programa CSP.</span><span class="sxs-lookup"><span data-stu-id="204bd-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="204bd-116">A partir del 31 de marzo de 2021, hemos introducido cambios en la API de validación de direcciones.</span><span class="sxs-lookup"><span data-stu-id="204bd-116">As of March 31, 2021, we have introduced changes to the Validate Address API.</span></span> <span data-ttu-id="204bd-117">Invitamos a los partners a probar la API antes de la publicación a finales de junio de 2021.</span><span class="sxs-lookup"><span data-stu-id="204bd-117">We invite partners to test the API prior to the  go-live at the end of June 2021.</span></span> 

<span data-ttu-id="204bd-118">Tenga en cuenta que estos cambios solo afectan a la API de validación de direcciones.</span><span class="sxs-lookup"><span data-stu-id="204bd-118">Note that these changes affect the Validate Address API only.</span></span> <span data-ttu-id="204bd-119">Las API de creación de clientes y actualización del perfil de facturación no se ven afectadas.</span><span class="sxs-lookup"><span data-stu-id="204bd-119">Create Customer and Update Billing Profile APIs aren’t affected.</span></span> <span data-ttu-id="204bd-120">Aunque la dirección sugerida no tiene que usarse actualmente con la API de creación de clientes, se recomienda encarecidamente.</span><span class="sxs-lookup"><span data-stu-id="204bd-120">Although the suggested address doesn’t currently have to be used with the Create Customer API, it’s highly recommended.</span></span>

<span data-ttu-id="204bd-121">La respuesta devolverá uno de los siguientes mensajes de estado:</span><span class="sxs-lookup"><span data-stu-id="204bd-121">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="204bd-122">Status</span><span class="sxs-lookup"><span data-stu-id="204bd-122">Status</span></span>     | <span data-ttu-id="204bd-123">Descripción</span><span class="sxs-lookup"><span data-stu-id="204bd-123">Description</span></span> |    <span data-ttu-id="204bd-124">Número de direcciones sugeridas devueltas</span><span class="sxs-lookup"><span data-stu-id="204bd-124">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="204bd-125">Verified shippable</span><span class="sxs-lookup"><span data-stu-id="204bd-125">Verified shippable</span></span> | <span data-ttu-id="204bd-126">La dirección está comprobada y puede recibir envíos.</span><span class="sxs-lookup"><span data-stu-id="204bd-126">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="204bd-127">Single</span><span class="sxs-lookup"><span data-stu-id="204bd-127">Single</span></span> |
|<span data-ttu-id="204bd-128">Verified</span><span class="sxs-lookup"><span data-stu-id="204bd-128">Verified</span></span> | <span data-ttu-id="204bd-129">La dirección está comprobada.</span><span class="sxs-lookup"><span data-stu-id="204bd-129">Address is verified.</span></span> | <span data-ttu-id="204bd-130">Single</span><span class="sxs-lookup"><span data-stu-id="204bd-130">Single</span></span> |
|<span data-ttu-id="204bd-131">Interaction required</span><span class="sxs-lookup"><span data-stu-id="204bd-131">Interaction required</span></span> | <span data-ttu-id="204bd-132">La dirección sugerida se ha cambiado significativamente y se necesita la confirmación del usuario.</span><span class="sxs-lookup"><span data-stu-id="204bd-132">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="204bd-133">Single</span><span class="sxs-lookup"><span data-stu-id="204bd-133">Single</span></span> |
|<span data-ttu-id="204bd-134">Street partial</span><span class="sxs-lookup"><span data-stu-id="204bd-134">Street partial</span></span> | <span data-ttu-id="204bd-135">La calle indicada en la dirección es parcial y necesita más información.</span><span class="sxs-lookup"><span data-stu-id="204bd-135">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="204bd-136">Varias: tres como máximo</span><span class="sxs-lookup"><span data-stu-id="204bd-136">Multiple—maximum of three</span></span> |
|<span data-ttu-id="204bd-137">Premises partial</span><span class="sxs-lookup"><span data-stu-id="204bd-137">Premises partial</span></span> | <span data-ttu-id="204bd-138">Los locales especificados (número de edificio, número de suite, etc.) son parciales y se necesita más información.</span><span class="sxs-lookup"><span data-stu-id="204bd-138">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="204bd-139">Varias: tres como máximo</span><span class="sxs-lookup"><span data-stu-id="204bd-139">Multiple—maximum of three</span></span> |
|<span data-ttu-id="204bd-140">Múltiple</span><span class="sxs-lookup"><span data-stu-id="204bd-140">Multiple</span></span> | <span data-ttu-id="204bd-141">La dirección tiene varios campos que son parciales (también puede incluir Street partial y Premises partial).</span><span class="sxs-lookup"><span data-stu-id="204bd-141">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="204bd-142">Varias: tres como máximo</span><span class="sxs-lookup"><span data-stu-id="204bd-142">Multiple—maximum of three</span></span> |
|<span data-ttu-id="204bd-143">Ninguno</span><span class="sxs-lookup"><span data-stu-id="204bd-143">None</span></span> | <span data-ttu-id="204bd-144">La dirección es incorrecta.</span><span class="sxs-lookup"><span data-stu-id="204bd-144">Address is incorrect.</span></span> | <span data-ttu-id="204bd-145">Ninguno</span><span class="sxs-lookup"><span data-stu-id="204bd-145">None</span></span> |
|<span data-ttu-id="204bd-146">No validado</span><span class="sxs-lookup"><span data-stu-id="204bd-146">Not validated</span></span> | <span data-ttu-id="204bd-147">No se pudo enviar la dirección a través del proceso de validación.</span><span class="sxs-lookup"><span data-stu-id="204bd-147">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="204bd-148">Ninguno</span><span class="sxs-lookup"><span data-stu-id="204bd-148">None</span></span> |

<span data-ttu-id="204bd-149">Los códigos postales de EE. UU. devolverán cuatro dígitos adicionales más un guion, por ejemplo, 12345-6789.</span><span class="sxs-lookup"><span data-stu-id="204bd-149">US post codes will return an additional four digits + hyphen, for example, 12345-6789.</span></span>

### <a name="next-steps"></a><span data-ttu-id="204bd-150">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="204bd-150">Next steps</span></span>

- <span data-ttu-id="204bd-151">Revise la documentación técnica y las preguntas más frecuentes en la [colección específica para asociados](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) a fin de obtener instrucciones más detalladas.</span><span class="sxs-lookup"><span data-stu-id="204bd-151">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="204bd-152">Prepárese para incorporar los cambios mediante la API del Centro de partners y la experiencia de usuario web.</span><span class="sxs-lookup"><span data-stu-id="204bd-152">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> 
- <span data-ttu-id="204bd-153">Comparta su id. de inquilino de espacio aislado con nuestro experto en la materia, Ali Khaki, para que se incluya en el piloto de prueba, de modo que pueda empezar a preparar la actualización.</span><span class="sxs-lookup"><span data-stu-id="204bd-153">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span> 
- <span data-ttu-id="204bd-154">Si usa una solución de proveedor de panel de control (CPV), consulte a su CPV.</span><span class="sxs-lookup"><span data-stu-id="204bd-154">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="204bd-155">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="204bd-155">Questions?</span></span>

<span data-ttu-id="204bd-156">Si necesita soporte técnico para las operaciones con Microsoft, póngase en contacto con el grupo de Yammer de soporte técnico al partner o abra una [solicitud de servicio](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="204bd-156">If you need support for your operations with Microsoft, reach out to your partner support Yammer group or open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a><span data-ttu-id="204bd-157">Nueva ubicación para la documentación de Swagger de las API del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="204bd-157">New location for Partner Center API Swagger documentation</span></span>

### <a name="categories"></a><span data-ttu-id="204bd-158">Categorías</span><span class="sxs-lookup"><span data-stu-id="204bd-158">Categories</span></span>

- <span data-ttu-id="204bd-159">Fecha: 26/04/2021</span><span class="sxs-lookup"><span data-stu-id="204bd-159">Date: 2021-04-26</span></span>
- <span data-ttu-id="204bd-160">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="204bd-160">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="204bd-161">Resumen</span><span class="sxs-lookup"><span data-stu-id="204bd-161">Summary</span></span>

<span data-ttu-id="204bd-162">Los documentos de Swagger de las API del Centro de partners se han migrado desde el [sitio de documentación de Swagger anterior](https://apidocs.microsoft.com/services/partnercenter) a un [nuevo sitio de documentación de Swagger](https://docs.microsoft.com/rest/api/partner-center-rest/).</span><span class="sxs-lookup"><span data-stu-id="204bd-162">Partner Center API Swagger documents have been migrated from the [previous Swagger Documentation site](https://apidocs.microsoft.com/services/partnercenter) to a [new Swagger Documentation site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="204bd-163">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="204bd-163">Impacted audience</span></span>

<span data-ttu-id="204bd-164">Partners de factura directa y proveedores indirectos que participan en el programa Proveedor de soluciones en la nube (CSP) y que usan las API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="204bd-164">Direct bill partners and Indirect Providers participating in the Cloud Solution Provider (CSP) program who are using the Partner Center APIs</span></span>

### <a name="details"></a><span data-ttu-id="204bd-165">Detalles</span><span class="sxs-lookup"><span data-stu-id="204bd-165">Details</span></span>

<span data-ttu-id="204bd-166">A partir del 26 de abril de 2021, la documentación de Swagger de las API del Centro de partners, incluido el contenido de la API REST, se encuentra en un [nuevo sitio](https://docs.microsoft.com/rest/api/partner-center-rest/).</span><span class="sxs-lookup"><span data-stu-id="204bd-166">As of April 26, 2021 the Partner Center API Swagger documentation, including Rest API content, is located on a [new site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span> <span data-ttu-id="204bd-167">El sitio antiguo dejará de ser accesible después de varias semanas.</span><span class="sxs-lookup"><span data-stu-id="204bd-167">The old site will be inaccessible after several weeks.</span></span>

### <a name="benefits"></a><span data-ttu-id="204bd-168">Ventajas</span><span class="sxs-lookup"><span data-stu-id="204bd-168">Benefits</span></span>

<span data-ttu-id="204bd-169">La documentación de Swagger de las API del Centro de partners proporciona una función **Pruébalo**.</span><span class="sxs-lookup"><span data-stu-id="204bd-169">The Partner Center API Swagger documentation will provide a **Try It** function.</span></span> <span data-ttu-id="204bd-170">Para usar esta función, deberá tener un token de portador, que puede generar siguiendo los pasos indicados en [Autenticación del Centro de partners](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication).</span><span class="sxs-lookup"><span data-stu-id="204bd-170">To use this function, you’ll need to have a Bearer Token, which you can generate by following the steps listed in [Partner Center Authentication](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication).</span></span>

### <a name="next-steps"></a><span data-ttu-id="204bd-171">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="204bd-171">Next steps</span></span>

<span data-ttu-id="204bd-172">Comparta esta información en su organización para que el equipo adecuado pueda revisar y actualizar sus procesos.</span><span class="sxs-lookup"><span data-stu-id="204bd-172">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="204bd-173">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="204bd-173">Questions?</span></span>

<span data-ttu-id="204bd-174">Si tiene preguntas sobre estas ofertas, consúltelas a las comunidades de Yammer correspondientes.</span><span class="sxs-lookup"><span data-stu-id="204bd-174">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a><span data-ttu-id="204bd-175">Directiva del período de devolución de software para Proveedor de soluciones en la nube (CSP) y aviso de expiración del vínculo de descarga</span><span class="sxs-lookup"><span data-stu-id="204bd-175">Cloud Solution Provider (CSP) software return period policy and download link expiry notice</span></span>

### <a name="categories"></a><span data-ttu-id="204bd-176">Categorías</span><span class="sxs-lookup"><span data-stu-id="204bd-176">Categories</span></span>

- <span data-ttu-id="204bd-177">Fecha: 21/04/2021</span><span class="sxs-lookup"><span data-stu-id="204bd-177">Date: 2021-04-21</span></span>
- <span data-ttu-id="204bd-178">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="204bd-178">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="204bd-179">Resumen</span><span class="sxs-lookup"><span data-stu-id="204bd-179">Summary</span></span>

<span data-ttu-id="204bd-180">Hay cambios en la directiva del período de devolución de software para CSP y en la expiración del vínculo de descarga.</span><span class="sxs-lookup"><span data-stu-id="204bd-180">There are changes to the CSP software return period policy and download link expiry.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="204bd-181">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="204bd-181">Impacted audience</span></span>

<span data-ttu-id="204bd-182">Partners que realizan transacciones con ofertas de software perpetuo o suscripciones de software en CSP</span><span class="sxs-lookup"><span data-stu-id="204bd-182">Partners transacting perpetual software or software subscription offers in CSP</span></span>

### <a name="details"></a><span data-ttu-id="204bd-183">Detalles</span><span class="sxs-lookup"><span data-stu-id="204bd-183">Details</span></span>

<span data-ttu-id="204bd-184">Tenga en cuenta las siguientes notificaciones importantes relacionadas con las compras de software perpetuo y suscripciones de software a través del Centro de partners:</span><span class="sxs-lookup"><span data-stu-id="204bd-184">Note the following important notifications regarding perpetual software and software subscription purchases through Partner Center:</span></span>

#### <a name="software-return-period-policy"></a><span data-ttu-id="204bd-185">Directiva del período de devolución de software</span><span class="sxs-lookup"><span data-stu-id="204bd-185">Software return period policy</span></span>

<span data-ttu-id="204bd-186">A partir del 1 de junio de 2021, el período de devolución de las ofertas de software en CSP, como se indica en el Microsoft Partner Agreement (MPA), cambiará de 60 días desde la fecha de pedido a 30 días desde la fecha de pedido.</span><span class="sxs-lookup"><span data-stu-id="204bd-186">From June 1, 2021, the return period for software offers in CSP, as stated in the Microsoft Partner Agreement (MPA), will change from 60 days from order date to 30 days from order date.</span></span>

<span data-ttu-id="204bd-187">Después de enviar un pedido para una oferta de software, los partners tendrán 30 días a partir de la fecha de pedido para enviar cualquier modificación de dicho pedido:</span><span class="sxs-lookup"><span data-stu-id="204bd-187">After an order for a software offer is submitted, partners will have 30 days from the order date to submit any revisions to such order:</span></span>

- <span data-ttu-id="204bd-188">Toda licencia de software perpetuo devuelta dentro del período de devolución de 30 días recibirá un crédito completo del precio de compra pagado.</span><span class="sxs-lookup"><span data-stu-id="204bd-188">Any perpetual software license returned within the 30-day return period will receive a full credit of the paid purchase price.</span></span>

- <span data-ttu-id="204bd-189">Todo producto de suscripción de software devuelto dentro del período de devolución de 30 días recibirá un crédito prorrateado del precio de compra pagado.</span><span class="sxs-lookup"><span data-stu-id="204bd-189">Any software subscription product returned within the 30-day return period will receive a prorated credit of the paid purchase price.</span></span>

<span data-ttu-id="204bd-190">Este mensaje es la continuación de los comunicados enviados por correo electrónico en diciembre de 2020 y abril de 2021 a todos los partners de CSP con respecto al período de devolución y otras actualizaciones al MPA.</span><span class="sxs-lookup"><span data-stu-id="204bd-190">This message is a follow-up to our email communications sent on December 2020 and April 2021 to all CSP partners regarding the return period and other updates to the MPA.</span></span> <span data-ttu-id="204bd-191">Consulte esos avisos para obtener detalles completos sobre los cambios que afectan al MPA.</span><span class="sxs-lookup"><span data-stu-id="204bd-191">Refer to those notices for full details regarding changes affecting the MPA.</span></span>

#### <a name="software-download-link-expiry"></a><span data-ttu-id="204bd-192">Expiración del vínculo de descarga de software</span><span class="sxs-lookup"><span data-stu-id="204bd-192">Software download link expiry</span></span>

<span data-ttu-id="204bd-193">A partir del 3 de junio de 2021, los vínculos de descarga de software para las compras de productos de software perpetuo y suscripciones de software a través del Centro de partners tendrán una fecha de expiración de cinco días a partir de la descarga inicial.</span><span class="sxs-lookup"><span data-stu-id="204bd-193">From June 3, 2021, the software download links for perpetual software and software subscription product purchases through Partner Center will have an expiration date of five days from the initial download.</span></span> <span data-ttu-id="204bd-194">El período de expiración se aplicará a todas las compras anteriores al 3 de junio de 2021, así como a partir del 3 de junio de 2021 en adelante.</span><span class="sxs-lookup"><span data-stu-id="204bd-194">The expiry period will apply to all purchases before June 3, 2021, as well as on or after June 3, 2021.</span></span>

### <a name="next-steps"></a><span data-ttu-id="204bd-195">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="204bd-195">Next steps</span></span>

<span data-ttu-id="204bd-196">Revise las [Preguntas frecuentes sobre el período de devolución de CSP y la expiración del vínculo de descarga](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), e informe de estos cambios a todos los equipos pertinentes de su organización:</span><span class="sxs-lookup"><span data-stu-id="204bd-196">Review the [CSP return period and download link expiry FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), and inform all appropriate teams within your organization of these changes:</span></span>

### <a name="questions"></a><span data-ttu-id="204bd-197">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="204bd-197">Questions?</span></span>

<span data-ttu-id="204bd-198">Si tiene preguntas sobre estas ofertas, consúltelas a las comunidades de Yammer correspondientes.</span><span class="sxs-lookup"><span data-stu-id="204bd-198">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a><span data-ttu-id="204bd-199">Programa Open License: transición de revendedores al programa Proveedor de soluciones en la nube (CSP)</span><span class="sxs-lookup"><span data-stu-id="204bd-199">Open Licensing program: Transitioning resellers to the Cloud Solution Provider (CSP) program</span></span>

### <a name="categories"></a><span data-ttu-id="204bd-200">Categorías</span><span class="sxs-lookup"><span data-stu-id="204bd-200">Categories</span></span>

- <span data-ttu-id="204bd-201">Fecha: 19/04/2021</span><span class="sxs-lookup"><span data-stu-id="204bd-201">Date: 2021-04-19</span></span>
- <span data-ttu-id="204bd-202">Hacer crecer el negocio</span><span class="sxs-lookup"><span data-stu-id="204bd-202">Grow Your Business</span></span>

### <a name="summary"></a><span data-ttu-id="204bd-203">Resumen</span><span class="sxs-lookup"><span data-stu-id="204bd-203">Summary</span></span>

<span data-ttu-id="204bd-204">En esta comunicación se detalla cómo prepararse para los cambios que se van a realizar próximamente en el programa Open License.</span><span class="sxs-lookup"><span data-stu-id="204bd-204">This communication details how to prepare for the changes that are coming soon to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="204bd-205">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="204bd-205">Impacted audience</span></span>

<span data-ttu-id="204bd-206">Asociados de Open License y CSP</span><span class="sxs-lookup"><span data-stu-id="204bd-206">CSP and Open License partners</span></span>

### <a name="details"></a><span data-ttu-id="204bd-207">Detalles</span><span class="sxs-lookup"><span data-stu-id="204bd-207">Details</span></span>

<span data-ttu-id="204bd-208">En 2020, Microsoft [anunció](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) que las licencias perpetuas de software estarán disponibles ampliamente para asociados y clientes a través del programa Proveedor de soluciones en la nube (CSP).</span><span class="sxs-lookup"><span data-stu-id="204bd-208">In 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) that perpetual software licenses will be broadly available to partners and customers through the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="204bd-209">El primer hito se alcanzó en enero de 2021, cuando las ofertas perpetuas de software comerciales se pusieron disponibles.</span><span class="sxs-lookup"><span data-stu-id="204bd-209">The first milestone was reached in January 2021, when commercial perpetual software offers became available.</span></span> <span data-ttu-id="204bd-210">El siguiente hito clave se realizará en julio de 2021, cuando las ofertas del [sector público](https://aka.ms/openlicensepublicsector) estén disponibles.</span><span class="sxs-lookup"><span data-stu-id="204bd-210">The next key milestone will happen in July 2021, when [public sector](https://aka.ms/openlicensepublicsector) offers become available.</span></span> <span data-ttu-id="204bd-211">También se ha [comunicado](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) que, a partir del 1 de enero de 2022, no se pueden realizar nuevas compras ni renovaciones de licencias de software de Software Assurance o servicios en línea a través del programa Open License.</span><span class="sxs-lookup"><span data-stu-id="204bd-211">We also [communicated](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) that effective January 1, 2022, no new software license purchases or renewals of Software Assurance or online services can be made through the Open License program.</span></span>

<span data-ttu-id="204bd-212">La transición del software perpetuo al programa CSP en la nueva experiencia comercial ayudará a los asociados a ampliar las oportunidades de ofrecer diversas soluciones y servicios administrados.</span><span class="sxs-lookup"><span data-stu-id="204bd-212">The transition of perpetual software to the CSP program in the new commerce experience will help partners to expand the opportunities to offer diverse solutions and managed services.</span></span> <span data-ttu-id="204bd-213">Esto también acelerará la transición de los clientes a la nube.</span><span class="sxs-lookup"><span data-stu-id="204bd-213">This will also accelerate customers’ transition to the cloud.</span></span>  <span data-ttu-id="204bd-214">Para ayudar a garantizar una transición sin problemas para nuestros asociados y clientes, hemos realizado estos ajustes y materiales para acelerar esta transformación digital:</span><span class="sxs-lookup"><span data-stu-id="204bd-214">To help ensure a smooth transition for both our partners and customers, we’ve made these adjustments and materials to accelerate this digital transformation:</span></span>

#### <a name="april-2021"></a><span data-ttu-id="204bd-215">Abril de 2021</span><span class="sxs-lookup"><span data-stu-id="204bd-215">April 2021</span></span>

<span data-ttu-id="204bd-216">[Ya disponible](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): materiales de transición de Open License a CSP para revendedores.</span><span class="sxs-lookup"><span data-stu-id="204bd-216">[Now available](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Open License-to-CSP transition materials for resellers</span></span>

#### <a name="july-2021"></a><span data-ttu-id="204bd-217">Julio de 2021</span><span class="sxs-lookup"><span data-stu-id="204bd-217">July 2021</span></span>

##### <a name="csp"></a><span data-ttu-id="204bd-218">CSP</span><span class="sxs-lookup"><span data-stu-id="204bd-218">CSP</span></span>

- <span data-ttu-id="204bd-219">1 de julio: licencias perpetuas de software disponibles para los clientes del sector público.</span><span class="sxs-lookup"><span data-stu-id="204bd-219">July 1: Perpetual software licenses available to public sector customers</span></span>

- <span data-ttu-id="204bd-220">7 de julio: licencias perpetuas de software de Visual Studio Pro y Get Genuine Windows Agreement disponibles para todos los segmentos.</span><span class="sxs-lookup"><span data-stu-id="204bd-220">July 7: Visual Studio Pro and Get Genuine Windows Agreement  perpetual software licenses available to all segments</span></span>

##### <a name="open-value"></a><span data-ttu-id="204bd-221">Open Value</span><span class="sxs-lookup"><span data-stu-id="204bd-221">Open Value</span></span>

- <span data-ttu-id="204bd-222">1 de julio: SKU adicionales disponibles en el programa Open Value para centros educativos y organizaciones sin ánimo de lucro, que proporcionan ofertas similares al programa Open License.</span><span class="sxs-lookup"><span data-stu-id="204bd-222">July 1: Additional SKUs available in the Open Value program for education and nonprofit, providing similar offers to the Open License program</span></span>

##### <a name="open-license"></a><span data-ttu-id="204bd-223">Open License</span><span class="sxs-lookup"><span data-stu-id="204bd-223">Open License</span></span>

- <span data-ttu-id="204bd-224">1 de julio: Microsoft ya no lanzará nuevas ofertas en el programa Open License.</span><span class="sxs-lookup"><span data-stu-id="204bd-224">July 1: Microsoft will no longer launch new offers in the Open License program.</span></span>

#### <a name="january-2022"></a><span data-ttu-id="204bd-225">Enero de 2022</span><span class="sxs-lookup"><span data-stu-id="204bd-225">January 2022</span></span>

- <span data-ttu-id="204bd-226">A partir del 1 de enero de 2022, no se pueden realizar nuevas compras ni renovaciones mediante el programa Open License.</span><span class="sxs-lookup"><span data-stu-id="204bd-226">January 1: No new purchases or renewals can be made through the Open License program</span></span>

### <a name="next-steps"></a><span data-ttu-id="204bd-227">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="204bd-227">Next steps</span></span>

#### <a name="csp-indirect-providers"></a><span data-ttu-id="204bd-228">Proveedores indirectos de CSP</span><span class="sxs-lookup"><span data-stu-id="204bd-228">CSP indirect providers</span></span>

<span data-ttu-id="204bd-229">Dedique los próximos meses a ayudar a los revendedores de Open License a orientarse en el programa CSP mediante la asistencia a eventos de la comunidad de asociados y el uso de los materiales de transición de Open License a CSP para revendedores:</span><span class="sxs-lookup"><span data-stu-id="204bd-229">Use the coming months to help Open License resellers orient into the CSP program by attending partner community events and using the Open License-to-CSP transition materials for resellers:</span></span>

- <span data-ttu-id="204bd-230">[Materiales de transición de Open License a CSP para revendedores](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): presentación de información general personalizable, plantilla de correo electrónico, guía de incorporación de revendedores indirectos de CSP y mucho más para ayudarle a impulsar la adopción de los revendedores a gran escala.</span><span class="sxs-lookup"><span data-stu-id="204bd-230">[Open License-to-CSP transition materials for resellers](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—Customizable overview presentation, email template, CSP indirect reseller onboarding guide, and more to help you drive the adoption for your resellers at scale.</span></span>

- <span data-ttu-id="204bd-231">[Eventos de la comunidad de asociados de CSP](https://globalpbocomm.eventbuilder.com/GlobalCSP) hospedados por Microsoft Business Operations.</span><span class="sxs-lookup"><span data-stu-id="204bd-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) hosted by Microsoft Business Operations.</span></span>  <span data-ttu-id="204bd-232">Únase a las distintas sesiones para obtener información sobre los conceptos básicos de CSP (aspectos básicos de CSP) o mantenerse al día y hacer preguntas sobre el software en CSP (sesiones de preguntas y respuestas).</span><span class="sxs-lookup"><span data-stu-id="204bd-232">Join the various sessions to learn CSP basics (CSP Fundamentals) or stay up to date, and ask questions regarding Software in CSP (Q&A Sessions).</span></span>

- <span data-ttu-id="204bd-233">(Próximamente) Sesión de entrenamiento centrada en revendedores indirectos de CSP hospedada por Microsoft Business Operations.</span><span class="sxs-lookup"><span data-stu-id="204bd-233">(Coming soon) CSP indirect reseller–focused training session hosted by Microsoft Business Operations.</span></span>

#### <a name="open-license-resellers"></a><span data-ttu-id="204bd-234">Revendedores de Open License</span><span class="sxs-lookup"><span data-stu-id="204bd-234">Open License resellers</span></span>

- <span data-ttu-id="204bd-235">Si su organización no está actualmente inscrita en el programa CSP, póngase en contacto con el distribuidor para obtener información sobre cómo empezar.</span><span class="sxs-lookup"><span data-stu-id="204bd-235">If your organization isn’t currently enrolled in the CSP program, contact your distributor for information on how to get started.</span></span> <span data-ttu-id="204bd-236">Conéctese con un proveedor indirecto [aquí](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span><span class="sxs-lookup"><span data-stu-id="204bd-236">Connect with an indirect provider [here](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span></span>

- <span data-ttu-id="204bd-237">Si su organización ya está inscrita en el programa CSP, obtenga más información sobre el software perpetuo en CSP [aquí](https://partner.microsoft.com/resources/collection/software-in-csp).</span><span class="sxs-lookup"><span data-stu-id="204bd-237">If your organization is already enrolled in the CSP program, learn more about perpetual software in CSP [here](https://partner.microsoft.com/resources/collection/software-in-csp).</span></span>

### <a name="questions"></a><span data-ttu-id="204bd-238">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="204bd-238">Questions?</span></span>

<span data-ttu-id="204bd-239">Si tiene alguna pregunta más sobre estas ofertas, consulte con las comunidades de Yammer correspondientes.</span><span class="sxs-lookup"><span data-stu-id="204bd-239">For further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a><span data-ttu-id="204bd-240">Ya disponible: guía de preparación para la promoción global</span><span class="sxs-lookup"><span data-stu-id="204bd-240">Now live: Global promo readiness guide</span></span>

### <a name="categories"></a><span data-ttu-id="204bd-241">Categorías</span><span class="sxs-lookup"><span data-stu-id="204bd-241">Categories</span></span>

- <span data-ttu-id="204bd-242">Fecha: 16/04/2021</span><span class="sxs-lookup"><span data-stu-id="204bd-242">Date: 2021-04-16</span></span>
- <span data-ttu-id="204bd-243">Capacidades</span><span class="sxs-lookup"><span data-stu-id="204bd-243">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="204bd-244">Resumen</span><span class="sxs-lookup"><span data-stu-id="204bd-244">Summary</span></span>

<span data-ttu-id="204bd-245">La preparación de lanzamiento ha publicado una nueva [guía global de preparación para la promoción](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) en la galería de recursos de preparación de operaciones.</span><span class="sxs-lookup"><span data-stu-id="204bd-245">Launch Readiness has published a new [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) on the Operations Readiness resource gallery.</span></span> <span data-ttu-id="204bd-246">En esta guía se proporciona una vista consolidada de todas las [promociones globales](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/) activas.</span><span class="sxs-lookup"><span data-stu-id="204bd-246">This guide provides a consolidated view of all active [global promotions](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="204bd-247">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="204bd-247">Impacted audience</span></span>

<span data-ttu-id="204bd-248">Todos los asociados de licencias por volumen (VL), lista de precios de Dynamics (DPL) y Proveedor de soluciones en la nube (CSP)</span><span class="sxs-lookup"><span data-stu-id="204bd-248">All Volume Licensing (VL), Dynamics Price List (DPL), and Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="204bd-249">Detalles</span><span class="sxs-lookup"><span data-stu-id="204bd-249">Details</span></span>

<span data-ttu-id="204bd-250">Los asociados de Microsoft han compartido con nosotros la necesidad de proporcionar una vista consolidada de todas las promociones globales con detalles de soporte técnico.</span><span class="sxs-lookup"><span data-stu-id="204bd-250">Microsoft partners have shared with us the need to provide a consolidated view of all global promotions with supporting details.</span></span> <span data-ttu-id="204bd-251">Querían que esta guía consolidada le ayudara a usar promociones con la confianza de que toda la información disponible fuese fácilmente accesible en una ubicación central y cómoda.</span><span class="sxs-lookup"><span data-stu-id="204bd-251">You wanted this consolidated guide to help you use promotions with the confidence that all the available information will be readily accessible in a central and convenient location.</span></span>

<span data-ttu-id="204bd-252">A partir de abril de 2021, Microsoft actualizará esta guía mensualmente y estará disponible en una colección dedicada de preparación para la promoción global en la galería de recursos de preparación de operaciones.</span><span class="sxs-lookup"><span data-stu-id="204bd-252">Beginning in April 2021, Microsoft will update this guide on a monthly basis, and it will be available in a dedicated Global Promo Readiness Guide collection in the Operations Readiness resource gallery.</span></span>

<span data-ttu-id="204bd-253">Los vínculos a esta guía también se incluirán en las colecciones siguientes:</span><span class="sxs-lookup"><span data-stu-id="204bd-253">Links to this guide will also be included in the following collections:</span></span>

- <span data-ttu-id="204bd-254">[Colección de calendario de lanzamientos](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), que proporciona una vista centralizada de los próximos cambios y lanzamientos.</span><span class="sxs-lookup"><span data-stu-id="204bd-254">[Launch calendar collection](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), which provides a centralized view of upcoming changes and launches.</span></span>

- <span data-ttu-id="204bd-255">[Colecciones de la comunidad](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), que contienen materiales de apoyo para nuestras llamadas mensuales de asociados, que resaltan los próximos cambios y temas oportunos de interés operativo.</span><span class="sxs-lookup"><span data-stu-id="204bd-255">[Community collections](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), which contain supporting materials for our monthly partner calls, highlighting upcoming changes and timely topics of operational interest.</span></span>

- <span data-ttu-id="204bd-256">[Boletines de asociados](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), como la actualización mensual de CSP.</span><span class="sxs-lookup"><span data-stu-id="204bd-256">[Partner newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), such as CSP Monthly Update</span></span>

<span data-ttu-id="204bd-257">Como recordatorio mensual, también publicaremos un anuncio del Centro de partners con cada nuevo problema de la guía de preparación para la promoción global.</span><span class="sxs-lookup"><span data-stu-id="204bd-257">As a monthly reminder, we will also publish a Partner Center announcement with each new issue of the global promo readiness guide.</span></span>

### <a name="next-steps"></a><span data-ttu-id="204bd-258">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="204bd-258">Next steps</span></span>

<span data-ttu-id="204bd-259">Al principio de cada mes, encontrará la [guía de preparación para la promoción global](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) más reciente en la [galería de recursos de preparación de operaciones](https://partner.microsoft.com/resources).</span><span class="sxs-lookup"><span data-stu-id="204bd-259">At the start of each month, you will find the latest [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources).</span></span>

<span data-ttu-id="204bd-260">Comparta esta información con los contactos adecuados de sus organizaciones y háganos saber lo útil que es la guía a través del artículo "¿Ha sido útil esta página?"</span><span class="sxs-lookup"><span data-stu-id="204bd-260">Share this information with the appropriate contacts in your organizations and let us know how helpful the guide is through the “Was this page helpful?”</span></span> <span data-ttu-id="204bd-261">situado al final de cada página.</span><span class="sxs-lookup"><span data-stu-id="204bd-261">button at the end of each page.</span></span>

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a><span data-ttu-id="204bd-262">Actualización y recordatorios de la comunidad de Proveedor de soluciones en la nube (CSP) de abril</span><span class="sxs-lookup"><span data-stu-id="204bd-262">April Cloud Solution Provider (CSP) community update and reminders</span></span>

### <a name="categories"></a><span data-ttu-id="204bd-263">Categorías</span><span class="sxs-lookup"><span data-stu-id="204bd-263">Categories</span></span>

- <span data-ttu-id="204bd-264">Fecha: 16/04/2021</span><span class="sxs-lookup"><span data-stu-id="204bd-264">Date: 2021-04-16</span></span>
- <span data-ttu-id="204bd-265">Comunidad | Invitaciones y recordatorios</span><span class="sxs-lookup"><span data-stu-id="204bd-265">Community | Invites and reminders</span></span>

### <a name="summary"></a><span data-ttu-id="204bd-266">Resumen</span><span class="sxs-lookup"><span data-stu-id="204bd-266">Summary</span></span>

<span data-ttu-id="204bd-267">Los recursos de la comunidad de CSP están disponibles a petición y se actualizan mensualmente para mantenerlo informado y preparado para el cambio en el programa CSP.</span><span class="sxs-lookup"><span data-stu-id="204bd-267">CSP community resources are available on demand and updated monthly to keep you informed and prepared for change in the CSP program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="204bd-268">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="204bd-268">Impacted audience</span></span>

<span data-ttu-id="204bd-269">Proveedores indirectos o asociados de factura directa de CSP</span><span class="sxs-lookup"><span data-stu-id="204bd-269">CSP direct bill partners and indirect providers</span></span>

### <a name="details"></a><span data-ttu-id="204bd-270">Detalles</span><span class="sxs-lookup"><span data-stu-id="204bd-270">Details</span></span>

<span data-ttu-id="204bd-271">Este mes, los recursos incluyen los siguientes temas clave:</span><span class="sxs-lookup"><span data-stu-id="204bd-271">This month, the resources include the following key topics:</span></span>

- [<span data-ttu-id="204bd-272">Actualización a la evolución del programa CSP y cambios en el programa Open License</span><span class="sxs-lookup"><span data-stu-id="204bd-272">Update to CSP program evolution and Open License program changes</span></span>](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [<span data-ttu-id="204bd-273">Cambios en los requisitos de incorporación de clientes de CSP en determinadas regiones</span><span class="sxs-lookup"><span data-stu-id="204bd-273">Changes to CSP customer onboarding requirements in certain regions</span></span>](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [<span data-ttu-id="204bd-274">Nuevo formato para la nueva factura de comercio en PDF en el programa CSP</span><span class="sxs-lookup"><span data-stu-id="204bd-274">New format for the new commerce PDF invoice in the CSP program</span></span>](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

<span data-ttu-id="204bd-275">Dentro de la [colección de la comunidad de CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), encontrará:</span><span class="sxs-lookup"><span data-stu-id="204bd-275">Within the [CSP community collection](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), you’ll find:</span></span>

- <span data-ttu-id="204bd-276">El [boletín de actualización mensual de CSP](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global) descargable, que agrega anuncios, actualizaciones, eventos y recordatorios recientes de CSP en un documento fácil de leer.</span><span class="sxs-lookup"><span data-stu-id="204bd-276">The downloadable [CSP Monthly Update newsletter](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), which aggregates recent CSP announcements, updates, events, and reminders in an easy-to-read document.</span></span>

- <span data-ttu-id="204bd-277">El [calendario de anuncios de CSP](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), que proporciona una vista de escala de tiempo de los próximos cambios que afectan al programa.</span><span class="sxs-lookup"><span data-stu-id="204bd-277">The [CSP Announcement Calendar](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), which provides a timeline view of upcoming changes affecting the program.</span></span>

- <span data-ttu-id="204bd-278">El nuevo [calendario de lanzamientos de productos](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), donde puede ver las próximas ofertas y lanzamientos de productos.</span><span class="sxs-lookup"><span data-stu-id="204bd-278">The new [product launch calendar](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), where you can view upcoming product launches and offers.</span></span>

- <span data-ttu-id="204bd-279">[Recursos de actualización de lanzamientos de CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) con contenido fácil de consumir en los cambios operativos clave.</span><span class="sxs-lookup"><span data-stu-id="204bd-279">[CSP launch update resources](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) with easy-to-consume content on key operational changes.</span></span>

- <span data-ttu-id="204bd-280">[Actualizadores y recordatorios](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) sobre temas clave de CSP que reciben interés y consultas.</span><span class="sxs-lookup"><span data-stu-id="204bd-280">[Refreshers and reminders](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) on key CSP topics receiving interest and queries.</span></span>

#### <a name="csp-community-call-qas"></a><span data-ttu-id="204bd-281">Preguntas y respuestas de llamadas de la comunidad de CSP</span><span class="sxs-lookup"><span data-stu-id="204bd-281">CSP Community Call Q&As</span></span>

<span data-ttu-id="204bd-282">Las preguntas y respuestas de llamadas de la comunidad están disponibles para ayudarle con preguntas relacionadas con los próximos cambios.</span><span class="sxs-lookup"><span data-stu-id="204bd-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span></span> <span data-ttu-id="204bd-283">Regístrese ahora para las preguntas y respuestas de llamadas de la comunidad que tendrán lugar en abril, mayo y junio.</span><span class="sxs-lookup"><span data-stu-id="204bd-283">Register now for CSP Community Call Q&As that are taking place in April, May, and June.</span></span> <span data-ttu-id="204bd-284">Se centrarán en los lanzamientos más recientes, los actualizadores importantes y los recordatorios.</span><span class="sxs-lookup"><span data-stu-id="204bd-284">These will focus on the latest launches, important refreshers, and reminders.</span></span>

<span data-ttu-id="204bd-285">[Regístrese aquí](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span><span class="sxs-lookup"><span data-stu-id="204bd-285">[Register here](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span></span>

### <a name="next-steps"></a><span data-ttu-id="204bd-286">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="204bd-286">Next steps</span></span>

<span data-ttu-id="204bd-287">Revise los recursos de la comunidad y regístrese para las preguntas y respuestas de llamadas de la comunidad.</span><span class="sxs-lookup"><span data-stu-id="204bd-287">Review the community resources and register for the Community Call Q&A.</span></span>

<span data-ttu-id="204bd-288">Para asegurarse de que obtiene el máximo partido de las preguntas y respuestas de llamadas de la comunidad, revise el contenido de la comunidad a petición y envíe sus preguntas hasta 48 horas antes de la llamada.</span><span class="sxs-lookup"><span data-stu-id="204bd-288">To ensure that you get the most from the Community Call Q&A, review the on-demand community content and submit your questions up to 48 hours before the call.</span></span>

### <a name="questions"></a><span data-ttu-id="204bd-289">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="204bd-289">Questions?</span></span>

<span data-ttu-id="204bd-290">Las preguntas y respuestas de llamadas de la comunidad de CSP mensuales son el mejor lugar para las preguntas relacionadas con los cambios en el programa CSP.</span><span class="sxs-lookup"><span data-stu-id="204bd-290">The monthly CSP Community Call Q&A is the best place for questions related to changes in the CSP program.</span></span> <span data-ttu-id="204bd-291">Cada mes, revise el material y envíe sus preguntas de antemano para que podamos dedicar la sesión a los temas más importantes para usted.</span><span class="sxs-lookup"><span data-stu-id="204bd-291">Each month, review the material and submit your questions in advance so that we can spend the session on the topics that are most important to you.</span></span>

<span data-ttu-id="204bd-292">Para obtener más información, póngase en contacto con el [soporte técnico](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span><span class="sxs-lookup"><span data-stu-id="204bd-292">For more information, contact [Support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span></span>

________________
## <a name="reminder-deprecation-of-get-qualification-on-may-4-2021"></a><a name="4"></a><span data-ttu-id="204bd-293">Recordatorio: desuso de calificación GET para el 4 de mayo de 2021</span><span class="sxs-lookup"><span data-stu-id="204bd-293">Reminder: Deprecation of GET qualification on May 4, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="204bd-294">Categorías</span><span class="sxs-lookup"><span data-stu-id="204bd-294">Categories</span></span>

- <span data-ttu-id="204bd-295">Fecha: 09/04/2021</span><span class="sxs-lookup"><span data-stu-id="204bd-295">Date: 2021-04-09</span></span>
- <span data-ttu-id="204bd-296">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="204bd-296">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="204bd-297">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="204bd-297">Impacted audience</span></span>

<span data-ttu-id="204bd-298">Asociados que venden ofertas académicas, sin ánimo de lucro y de Government Community Cloud (GCC) a través del programa Proveedor de soluciones en la nube mediante la API del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="204bd-298">Partners selling Academic, Nonprofit, and Government Community Cloud (GCC) offers through the Cloud Solution Provider program using the Partner Center API</span></span>

### <a name="details"></a><span data-ttu-id="204bd-299">Detalles</span><span class="sxs-lookup"><span data-stu-id="204bd-299">Details</span></span>

<span data-ttu-id="204bd-300">Este anuncio es un seguimiento de las [mejoras publicadas en diciembre](https://docs.microsoft.com/partner-center/announcements/2020-december#1) en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="204bd-300">This announcement is a follow-up to the Partner Center [enhancements released in December](https://docs.microsoft.com/partner-center/announcements/2020-december#1).</span></span> <span data-ttu-id="204bd-301">Como parte de ese lanzamiento, se han implementado nuevas API de calificación GET y POST, y como resultado, la calificación GET existente se retirará el 4 de mayo de 2021.</span><span class="sxs-lookup"><span data-stu-id="204bd-301">As part of that release, new GET and POST Qualifications APIs were deployed and, as a result, the existing GET qualification will be retired by May 4, 2021.</span></span> <span data-ttu-id="204bd-302">En ese momento, tendrá que haber realizado la transición para usar las nuevas API POST del Centro de partners, para poder comprar ofertas educativas y las nuevas API de calificación GET para adquirir ofertas sin ánimo de lucro y GCC calificadas previamente.</span><span class="sxs-lookup"><span data-stu-id="204bd-302">By that time, you’ll need to have transitioned to using the new POST Partner Center APIs in purchase Education offers, and the new GET qualifications API to purchase prequalified Nonprofit and GCC offers.</span></span>

### <a name="next-steps"></a><span data-ttu-id="204bd-303">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="204bd-303">Next steps</span></span>

- <span data-ttu-id="204bd-304">Actualice las nuevas API para conseguir una transición correcta y oportuna.</span><span class="sxs-lookup"><span data-stu-id="204bd-304">Update to the new APIs for a successful and timely transition.</span></span>

- <span data-ttu-id="204bd-305">Revise los nuevos cambios en la API del Centro de partners y consulte la Guía sobre los recursos de preparación de operaciones: [Mejoras en el proceso de validación de clientes de Educación del Centro de partners](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span><span class="sxs-lookup"><span data-stu-id="204bd-305">Review the new Partner Center API changes and Guide in the Operations Readiness resources: [Partner Center Education customer validation process enhancements](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span></span>

- <span data-ttu-id="204bd-306">Comparta esta información con los equipos adecuados de su organización y con sus revendedores para ayudarlos a prepararse para estos cambios.</span><span class="sxs-lookup"><span data-stu-id="204bd-306">Share this information with the appropriate teams within your organization and with your resellers to help them prepare for these changes.</span></span>

### <a name="questions"></a><span data-ttu-id="204bd-307">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="204bd-307">Questions?</span></span>

<span data-ttu-id="204bd-308">Si tiene alguna pregunta relacionada con esta notificación, póngase en contacto con el [soporte técnico del Centro de partners](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span><span class="sxs-lookup"><span data-stu-id="204bd-308">For any questions related to this notification, contact [Partner Center support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span></span>

### <a name="change-log"></a><span data-ttu-id="204bd-309">Registro de cambios</span><span class="sxs-lookup"><span data-stu-id="204bd-309">Change log</span></span>

- <span data-ttu-id="204bd-310">Abril: recordatorio de la próxima entrada en desuso de la calificación GET</span><span class="sxs-lookup"><span data-stu-id="204bd-310">April: Reminder of upcoming deprecation of GET qualification</span></span> 
- <span data-ttu-id="204bd-311">Febrero: escalas de tiempo actualizadas y que dejarán en desuso las calificaciones GET y PUT.</span><span class="sxs-lookup"><span data-stu-id="204bd-311">February: Updated timelines for deprecation of GET & PUT qualifications</span></span>
- <span data-ttu-id="204bd-312">Enero: recordatorio de la próxima entrada en desuso de las calificaciones de GET & PUT</span><span class="sxs-lookup"><span data-stu-id="204bd-312">January: Reminder of upcoming deprecations of GET & PUT qualifications</span></span>

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a><span data-ttu-id="204bd-313">Nuevo formato para la nueva factura de comercio en PDF en CSP</span><span class="sxs-lookup"><span data-stu-id="204bd-313">New format for the new commerce PDF invoice in CSP</span></span>

### <a name="categories"></a><span data-ttu-id="204bd-314">Categorías</span><span class="sxs-lookup"><span data-stu-id="204bd-314">Categories</span></span>

- <span data-ttu-id="204bd-315">Fecha: 05/04/2021</span><span class="sxs-lookup"><span data-stu-id="204bd-315">Date: 2021-04-05</span></span>
- <span data-ttu-id="204bd-316">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="204bd-316">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="204bd-317">Resumen</span><span class="sxs-lookup"><span data-stu-id="204bd-317">Summary</span></span>

<span data-ttu-id="204bd-318">Microsoft presenta un nuevo formato para la nueva factura de comercio en PDF en el programa Proveedor de soluciones en la nube (CSP) para mostrar la información de facturación por detalle del producto en lugar de la descripción de la SKU.</span><span class="sxs-lookup"><span data-stu-id="204bd-318">Microsoft is introducing a new format for the new commerce PDF invoice in the Cloud Solution Provider (CSP) program to display billing details by product detail instead of SKU description.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="204bd-319">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="204bd-319">Impacted audience</span></span>

<span data-ttu-id="204bd-320">Partners que realizan transacciones mediante el programa CSP</span><span class="sxs-lookup"><span data-stu-id="204bd-320">Partners transacting through the CSP program</span></span>

### <a name="details"></a><span data-ttu-id="204bd-321">Detalles</span><span class="sxs-lookup"><span data-stu-id="204bd-321">Details</span></span>

<span data-ttu-id="204bd-322">A partir de mayo de 2021, Microsoft presenta un nuevo formato para la nueva factura de comercio en PDF en el programa CSP para mostrar la información de facturación por detalle del producto en lugar de la descripción de la SKU.</span><span class="sxs-lookup"><span data-stu-id="204bd-322">Starting May 2021, Microsoft is introducing a new format for the new commerce PDF invoice in the CSP program to display billing details by product detail instead of SKU description.</span></span> <span data-ttu-id="204bd-323">Con esta nueva actualización, agregaremos los elementos de línea por tipo de producto, al tiempo que se muestran todos los productos en una línea individual.</span><span class="sxs-lookup"><span data-stu-id="204bd-323">With this new update, we will be aggregating the line items by product type while displaying every product on an individual line.</span></span>

<span data-ttu-id="204bd-324">Los asociados observarán que este cambio entra en vigor en su factura de mayo del período de facturación entre el 1 y el 30 de abril de 2021.</span><span class="sxs-lookup"><span data-stu-id="204bd-324">Partners will notice this change coming into effect in their May invoice for the billing period between April 1, 2021 and April 30, 2021.</span></span> <span data-ttu-id="204bd-325">Las ofertas afectadas son instancia reservada de Microsoft Azure, suscripciones de Azure (plan de Azure) y Marketplace.</span><span class="sxs-lookup"><span data-stu-id="204bd-325">The affected offers are Microsoft Azure Reserved Instance, Azure subscriptions (Azure plan), and Marketplace.</span></span>

<span data-ttu-id="204bd-326">Las solicitudes de refacturación de crédito realizadas después de actualizar el formato de la factura se generará en el nuevo formato.</span><span class="sxs-lookup"><span data-stu-id="204bd-326">Any credit-rebill requests made after the invoice format has been updated will be generated in the new format.</span></span>

#### <a name="partner-benefits"></a><span data-ttu-id="204bd-327">Ventajas para partners</span><span class="sxs-lookup"><span data-stu-id="204bd-327">Partner benefits</span></span>

<span data-ttu-id="204bd-328">Esta actualización ofrece las siguientes mejoras en la experiencia de facturación para asociados:</span><span class="sxs-lookup"><span data-stu-id="204bd-328">This update will offer the following improvements to the invoicing experience for partners:</span></span>

- <span data-ttu-id="204bd-329">Tamaño de factura reducido al tiempo que se conservan los datos críticos</span><span class="sxs-lookup"><span data-stu-id="204bd-329">Reduced invoice size while retaining critical data</span></span>

- <span data-ttu-id="204bd-330">Alineación del formato a los estándares del sector para facturas compactas y fáciles de usar</span><span class="sxs-lookup"><span data-stu-id="204bd-330">Alignment of the format to the industry standards for compact and user-friendly invoices</span></span> 

<span data-ttu-id="204bd-331">Los elementos siguientes no se verán afectados:</span><span class="sxs-lookup"><span data-stu-id="204bd-331">The following elements will not be affected:</span></span>

- <span data-ttu-id="204bd-332">Página de resumen de facturación en la factura en PDF</span><span class="sxs-lookup"><span data-stu-id="204bd-332">Billing summary page on the invoice PDF</span></span>

- <span data-ttu-id="204bd-333">API de facturación existentes</span><span class="sxs-lookup"><span data-stu-id="204bd-333">Existing invoicing APIs</span></span>

- <span data-ttu-id="204bd-334">Archivos de conciliación (los archivos de conciliación se pueden usar para recuperar datos granulares).</span><span class="sxs-lookup"><span data-stu-id="204bd-334">Reconciliation files (Recon files can be used for retrieving granular data.)</span></span> 

- <span data-ttu-id="204bd-335">Facturas de cargos de uso y basadas en licencias</span><span class="sxs-lookup"><span data-stu-id="204bd-335">Usage and license-based charges invoices</span></span>

### <a name="next-steps"></a><span data-ttu-id="204bd-336">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="204bd-336">Next steps</span></span>

<span data-ttu-id="204bd-337">Revise la información sobre este tema en la [galería de recursos de preparación de operaciones](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) en el sitio web para asociados de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="204bd-337">Review the information about this topic in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) on the Microsoft partner website.</span></span> <span data-ttu-id="204bd-338">Para más información sobre facturación e impuestos, así como recursos de facturación, facturas, facturación de CSP e impuestos, visite la [sección de facturación](https://docs.microsoft.com/partner-center/billing) del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="204bd-338">For more information about billing and tax topics including billing resources, invoices, CSP billing, and taxes, visit the [Billing section](https://docs.microsoft.com/partner-center/billing) in Partner Center.</span></span>

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a><span data-ttu-id="204bd-339">Cambios en los requisitos de incorporación de clientes de Proveedor de soluciones en la nube (CSP)</span><span class="sxs-lookup"><span data-stu-id="204bd-339">Changes to the Cloud Solution Provider (CSP) customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="204bd-340">Categorías</span><span class="sxs-lookup"><span data-stu-id="204bd-340">Categories</span></span>

- <span data-ttu-id="204bd-341">Fecha: 02/04/2021</span><span class="sxs-lookup"><span data-stu-id="204bd-341">Date: 2021-04-02</span></span>
- <span data-ttu-id="204bd-342">Ofertas/mercados</span><span class="sxs-lookup"><span data-stu-id="204bd-342">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="204bd-343">Resumen</span><span class="sxs-lookup"><span data-stu-id="204bd-343">Summary</span></span>

<span data-ttu-id="204bd-344">Como parte de nuestro compromiso para ayudar a los asociados y los clientes a llevar a cabo sus actividades empresariales basándose en la confianza, solicitaremos información adicional del cliente. Esto entrará en vigor el 25 de marzo de 2021.</span><span class="sxs-lookup"><span data-stu-id="204bd-344">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="204bd-345">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="204bd-345">Impacted audience</span></span>

<span data-ttu-id="204bd-346">Partners de factura directa y proveedores indirectos de CSP con clientes nuevos o existentes en los países que se indican en la sección siguiente</span><span class="sxs-lookup"><span data-stu-id="204bd-346">CSP direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="204bd-347">Detalles</span><span class="sxs-lookup"><span data-stu-id="204bd-347">Details</span></span>

<span data-ttu-id="204bd-348">Microsoft funciona con confianza.</span><span class="sxs-lookup"><span data-stu-id="204bd-348">Microsoft runs on trust.</span></span> <span data-ttu-id="204bd-349">Nos comprometemos a proporcionar un método compatible, seguro y protegido para la validación de clientes durante las operaciones de transacción con suscripciones de clientes en el programa CSP.</span><span class="sxs-lookup"><span data-stu-id="204bd-349">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="204bd-350">El 25 de marzo de 2021, presentaremos mejoras en la interfaz de usuario y la API del Centro de partners que afectarán a los partners que cumplan los criterios siguientes:</span><span class="sxs-lookup"><span data-stu-id="204bd-350">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

- <span data-ttu-id="204bd-351">El partner tiene una relación de factura directa con Microsoft (lo que significa que se trata de un partner de factura directa o de un proveedor indirecto).</span><span class="sxs-lookup"><span data-stu-id="204bd-351">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

- <span data-ttu-id="204bd-352">El asociado hace negocios con clientes nuevos o existentes en los siguientes países:</span><span class="sxs-lookup"><span data-stu-id="204bd-352">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="204bd-353">Tailandia</span><span class="sxs-lookup"><span data-stu-id="204bd-353">Thailand</span></span>
    - <span data-ttu-id="204bd-354">Vietnam</span><span class="sxs-lookup"><span data-stu-id="204bd-354">Vietnam</span></span>
    - <span data-ttu-id="204bd-355">Turquía</span><span class="sxs-lookup"><span data-stu-id="204bd-355">Turkey</span></span>
    - <span data-ttu-id="204bd-356">Polonia</span><span class="sxs-lookup"><span data-stu-id="204bd-356">Poland</span></span>
    - <span data-ttu-id="204bd-357">Sudáfrica</span><span class="sxs-lookup"><span data-stu-id="204bd-357">South Africa</span></span>
    - <span data-ttu-id="204bd-358">India</span><span class="sxs-lookup"><span data-stu-id="204bd-358">India</span></span>
    - <span data-ttu-id="204bd-359">Brasil</span><span class="sxs-lookup"><span data-stu-id="204bd-359">Brazil</span></span>
    - <span data-ttu-id="204bd-360">Iraq</span><span class="sxs-lookup"><span data-stu-id="204bd-360">Iraq</span></span>
    - <span data-ttu-id="204bd-361">Myanmar</span><span class="sxs-lookup"><span data-stu-id="204bd-361">Myanmar</span></span>
    - <span data-ttu-id="204bd-362">Sudán del Sur</span><span class="sxs-lookup"><span data-stu-id="204bd-362">South Sudan</span></span>
    - <span data-ttu-id="204bd-363">Arabia Saudí</span><span class="sxs-lookup"><span data-stu-id="204bd-363">Saudi Arabia</span></span>
    - <span data-ttu-id="204bd-364">Emiratos Árabes Unidos</span><span class="sxs-lookup"><span data-stu-id="204bd-364">United Arab Emirates</span></span>
    - <span data-ttu-id="204bd-365">Venezuela</span><span class="sxs-lookup"><span data-stu-id="204bd-365">Venezuela</span></span>

<span data-ttu-id="204bd-366">Los asociados que cumplan los criterios tendrán que enviar el identificador de registro de la compañía (también conocido como INN de la organización del cliente) y el número de teléfono del cliente la próxima vez que actualicen o creen una suscripción para ese cliente.</span><span class="sxs-lookup"><span data-stu-id="204bd-366">Partners who meet the criteria will have to submit a customer's company registration ID (also known as the customer's organization INN) and phone number when they next update or create a subscription for that customer.</span></span> <span data-ttu-id="204bd-367">Estos partners también pueden escribir un segundo nombre opcional para el cliente.</span><span class="sxs-lookup"><span data-stu-id="204bd-367">These partners can also enter an optional middle name for the customer.</span></span>

<span data-ttu-id="204bd-368">Tenga en cuenta que, al agregar el identificador de registro de la compañía, debe usar el id. de impuesto empresarial y no el identificador personal del cliente.</span><span class="sxs-lookup"><span data-stu-id="204bd-368">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="204bd-369">Los partners que llevan a cabo actividades empresariales con clientes nuevos o existentes de los países siguientes ya se incorporaron con una versión anterior en noviembre de 2020.</span><span class="sxs-lookup"><span data-stu-id="204bd-369">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="204bd-370">Armenia</span><span class="sxs-lookup"><span data-stu-id="204bd-370">Armenia</span></span>
- <span data-ttu-id="204bd-371">Azerbaiyán</span><span class="sxs-lookup"><span data-stu-id="204bd-371">Azerbaijan</span></span>
- <span data-ttu-id="204bd-372">Belarús</span><span class="sxs-lookup"><span data-stu-id="204bd-372">Belarus</span></span>
- <span data-ttu-id="204bd-373">Hungría</span><span class="sxs-lookup"><span data-stu-id="204bd-373">Hungary</span></span>
- <span data-ttu-id="204bd-374">Kazajistán</span><span class="sxs-lookup"><span data-stu-id="204bd-374">Kazakhstan</span></span>
- <span data-ttu-id="204bd-375">Kirguistán</span><span class="sxs-lookup"><span data-stu-id="204bd-375">Kyrgyzstan</span></span>
- <span data-ttu-id="204bd-376">Moldova</span><span class="sxs-lookup"><span data-stu-id="204bd-376">Moldova</span></span>
- <span data-ttu-id="204bd-377">Rusia</span><span class="sxs-lookup"><span data-stu-id="204bd-377">Russia</span></span>
- <span data-ttu-id="204bd-378">Tayikistán</span><span class="sxs-lookup"><span data-stu-id="204bd-378">Tajikistan</span></span>
- <span data-ttu-id="204bd-379">Ucrania</span><span class="sxs-lookup"><span data-stu-id="204bd-379">Ukraine</span></span>
- <span data-ttu-id="204bd-380">Uzbekistán</span><span class="sxs-lookup"><span data-stu-id="204bd-380">Uzbekistan</span></span>

<span data-ttu-id="204bd-381">Los asociados con clientes en el resto del mundo podrán, a finales de marzo de 2021, escribir el identificador de registro de la compañía, el número de teléfono y el segundo nombre de los clientes como detalles opcionales.</span><span class="sxs-lookup"><span data-stu-id="204bd-381">Partners with customers in the rest of the world will have the ability at the end of March 2021 to enter the company registration ID, phone number, and middle name for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="204bd-382">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="204bd-382">Next steps</span></span>

- <span data-ttu-id="204bd-383">Revise la documentación técnica y las preguntas más frecuentes en la [colección específica para partners](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) a fin de obtener instrucciones más detalladas.</span><span class="sxs-lookup"><span data-stu-id="204bd-383">Review the technical documentation and frequently asked questions in the dedicated [partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="204bd-384">Prepárese para incorporar los cambios mediante la API del Centro de partners y la experiencia de usuario web.</span><span class="sxs-lookup"><span data-stu-id="204bd-384">Prepare to incorporate the changes using Partner Center API and web user experience.</span></span> <span data-ttu-id="204bd-385">Habrá API y SDK disponibles para realizar pruebas.</span><span class="sxs-lookup"><span data-stu-id="204bd-385">API/SDKs will be available for testing.</span></span>
- <span data-ttu-id="204bd-386">Asegúrese de enviar los datos adicionales al incorporar clientes nuevos o modificar los datos de clientes existentes.</span><span class="sxs-lookup"><span data-stu-id="204bd-386">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>
- <span data-ttu-id="204bd-387">Si usa una solución de proveedor de panel de control (CPV), consulte a su CPV.</span><span class="sxs-lookup"><span data-stu-id="204bd-387">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="204bd-388">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="204bd-388">Questions?</span></span>

<span data-ttu-id="204bd-389">Si tiene alguna pregunta relacionada con el identificador de registro de la compañía (también denominado INN o CIF/NIF), póngase en contacto con su asesor fiscal o con la agencia tributaria local.</span><span class="sxs-lookup"><span data-stu-id="204bd-389">Contact your tax advisor or local tax office if you have any questions related to the company registration ID (also called INN or TIN).</span></span> <span data-ttu-id="204bd-390">Microsoft no puede proporcionar orientación sobre cuestiones fiscales.</span><span class="sxs-lookup"><span data-stu-id="204bd-390">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="204bd-391">Si necesita soporte técnico con relación a sus operaciones con Microsoft, [abra una solicitud de servicio](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="204bd-391">If you need support with your operations with Microsoft, open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a><span data-ttu-id="204bd-392">Ver ofertas y lanzamientos de productos de este mes</span><span class="sxs-lookup"><span data-stu-id="204bd-392">View this month’s product launches and offers</span></span>

### <a name="categories"></a><span data-ttu-id="204bd-393">Categorías</span><span class="sxs-lookup"><span data-stu-id="204bd-393">Categories</span></span>

- <span data-ttu-id="204bd-394">Fecha: 01/04/2021</span><span class="sxs-lookup"><span data-stu-id="204bd-394">Date: 2021-04-01</span></span>
- <span data-ttu-id="204bd-395">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="204bd-395">Capabilities</span></span>
 
### <a name="summary"></a><span data-ttu-id="204bd-396">Resumen</span><span class="sxs-lookup"><span data-stu-id="204bd-396">Summary</span></span>

<span data-ttu-id="204bd-397">Ya se ha publicado el calendario de lanzamientos de productos de abril de 2021.</span><span class="sxs-lookup"><span data-stu-id="204bd-397">The April 2021 product launch calendar is now published.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="204bd-398">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="204bd-398">Impacted audience</span></span>

<span data-ttu-id="204bd-399">Todos los partners que operan a través del programa Proveedor de soluciones en la nube (CSP)</span><span class="sxs-lookup"><span data-stu-id="204bd-399">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="204bd-400">Detalles</span><span class="sxs-lookup"><span data-stu-id="204bd-400">Details</span></span>

<span data-ttu-id="204bd-401">El [calendario de lanzamientos de productos](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) de abril de 2021 ya está disponible en la galería de recursos de preparación de operaciones.</span><span class="sxs-lookup"><span data-stu-id="204bd-401">The April 2021 [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) is now available in the Operations readiness resource gallery.</span></span> <span data-ttu-id="204bd-402">Vea los próximos lanzamientos de productos y ofertas aquí.</span><span class="sxs-lookup"><span data-stu-id="204bd-402">View the upcoming product launches and offers here.</span></span>

### <a name="next-steps"></a><span data-ttu-id="204bd-403">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="204bd-403">Next steps</span></span>

<span data-ttu-id="204bd-404">Revise el [calendario de lanzamientos de productos](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) y comparta esta información con las partes interesadas adecuadas de su organización.</span><span class="sxs-lookup"><span data-stu-id="204bd-404">Review the [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), and share the information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="204bd-405">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="204bd-405">Questions?</span></span>

<span data-ttu-id="204bd-406">Si tiene alguna pregunta más sobre estas ofertas, consulte con las comunidades de Yammer correspondientes.</span><span class="sxs-lookup"><span data-stu-id="204bd-406">For any further questions about these offers, check your relevant Yammer communities.</span></span>
