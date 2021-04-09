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
ms.openlocfilehash: 12954a5f7eafb138794de879a41026ef54c65da7
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374400"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="d6ca3-103">Anuncios de marzo de 2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-103">March 2021 announcements</span></span>

<span data-ttu-id="d6ca3-104">En esta página se encuentran los anuncios del Centro de partners de Microsoft de marzo de 2021.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a><span data-ttu-id="d6ca3-105">La API de validación de direcciones de cliente de CSP actualizada ahora está disponible para pruebas</span><span class="sxs-lookup"><span data-stu-id="d6ca3-105">Updated CSP customer address validation API now available for testing</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-106">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-106">Categories</span></span>

- <span data-ttu-id="d6ca3-107">Fecha: 31/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-107">Date: 2021-03-31</span></span>
- <span data-ttu-id="d6ca3-108">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="d6ca3-108">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d6ca3-109">Resumen</span><span class="sxs-lookup"><span data-stu-id="d6ca3-109">Summary</span></span>

<span data-ttu-id="d6ca3-110">Como parte de nuestro compromiso para ayudar a los asociados y clientes a ejecutar su negocio en función de la confianza, invitaremos a los asociados de todo el mundo a probar los cambios en la API ValidateAddress.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-110">As part of our commitment to help partners and customers run their business based on trust, we will be inviting partners worldwide to test the changes to the ValidateAddress API.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-111">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-111">Impacted audience</span></span>

<span data-ttu-id="d6ca3-112">Todos los asociados de CSP Direct Bill Partner y proveedores indirectos que crean o actualizan los detalles de la dirección del cliente existente.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-112">All CSP direct bill partners and indirect providers who create new or update existing customer address details</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-113">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-113">Details</span></span>

<span data-ttu-id="d6ca3-114">Microsoft funciona con confianza.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-114">Microsoft runs on trust.</span></span> <span data-ttu-id="d6ca3-115">Nos comprometemos a proporcionar un método compatible, seguro y protegido para el envío de la validación de direcciones de clientes durante las operaciones de transacción con suscripciones de clientes en el programa CSP.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-115">We’re committed to providing a compliant, safe, and secure method of submitting customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="d6ca3-116">Hoy, 31 de marzo de 2021, hemos presentado cambios en la API ValidateAddress que nos gustaría invitarle a probar antes publicar los cambios de junio de 2021.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-116">Today, March 31, 2021, we have introduced changes to the ValidateAddress API that we’d like to invite you to test, prior to going live with the changes in June 2021.</span></span> 

<span data-ttu-id="d6ca3-117">Tenga en cuenta que estos cambios solo afectan a la API ValidateAddress.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-117">Note that these changes affect the ValidateAddress API only.</span></span> <span data-ttu-id="d6ca3-118">Las API CreateCustomer y UpdateBillingProfile no se ven afectadas.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-118">CreateCustomer and UpdateBillingProfile APIs are not affected.</span></span>

<span data-ttu-id="d6ca3-119">La respuesta devolverá uno de los siguientes mensajes de estado:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="d6ca3-120">Status</span><span class="sxs-lookup"><span data-stu-id="d6ca3-120">Status</span></span> | <span data-ttu-id="d6ca3-121">Descripción</span><span class="sxs-lookup"><span data-stu-id="d6ca3-121">Description</span></span> | <span data-ttu-id="d6ca3-122">Número de direcciones sugeridas devueltas</span><span class="sxs-lookup"><span data-stu-id="d6ca3-122">Number of suggested addresses returned</span></span> |
|----------|-------------|-------------------|
| <span data-ttu-id="d6ca3-123">VerifiedShippable</span><span class="sxs-lookup"><span data-stu-id="d6ca3-123">VerifiedShippable</span></span> | <span data-ttu-id="d6ca3-124">La dirección está comprobada y puede recibir envíos.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="d6ca3-125">Single</span><span class="sxs-lookup"><span data-stu-id="d6ca3-125">Single</span></span> |
| <span data-ttu-id="d6ca3-126">Verified</span><span class="sxs-lookup"><span data-stu-id="d6ca3-126">Verified</span></span> | <span data-ttu-id="d6ca3-127">La dirección está comprobada.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-127">Address is verified.</span></span> | <span data-ttu-id="d6ca3-128">Single</span><span class="sxs-lookup"><span data-stu-id="d6ca3-128">Single</span></span> |
| <span data-ttu-id="d6ca3-129">InteractionRequired</span><span class="sxs-lookup"><span data-stu-id="d6ca3-129">InteractionRequired</span></span> | <span data-ttu-id="d6ca3-130">Las direcciones sugeridas se han cambiado significativamente y necesitan la confirmación del usuario.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-130">Suggested address(es) has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="d6ca3-131">Single</span><span class="sxs-lookup"><span data-stu-id="d6ca3-131">Single</span></span> |
| <span data-ttu-id="d6ca3-132">StreetPartial</span><span class="sxs-lookup"><span data-stu-id="d6ca3-132">StreetPartial</span></span> | <span data-ttu-id="d6ca3-133">La calle indicada en la dirección es parcial y necesita más información.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="d6ca3-134">Varias: tres como máximo</span><span class="sxs-lookup"><span data-stu-id="d6ca3-134">Multiple—maximum of three</span></span>|
| <span data-ttu-id="d6ca3-135">PremisesPartial</span><span class="sxs-lookup"><span data-stu-id="d6ca3-135">PremisesPartial</span></span> | <span data-ttu-id="d6ca3-136">Los locales especificados (número de edificio, número de suite, etc.) son parciales y necesitan más información.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-136">The given premises (building number, suite number, etc.) is partial and needs more info.</span></span> | <span data-ttu-id="d6ca3-137">Varias: tres como máximo</span><span class="sxs-lookup"><span data-stu-id="d6ca3-137">Multiple—maximum of three</span></span> |
| <span data-ttu-id="d6ca3-138">Múltiple</span><span class="sxs-lookup"><span data-stu-id="d6ca3-138">Multiple</span></span> | <span data-ttu-id="d6ca3-139">Hay varios campos que son parciales en la dirección (también puede incluir StreetPartial y PremisesPartial).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-139">There are multiple fields that are partial in the address (potentially also including StreetPartial and PremisesPartial).</span></span> | <span data-ttu-id="d6ca3-140">Varias: tres como máximo</span><span class="sxs-lookup"><span data-stu-id="d6ca3-140">Multiple—maximum of three</span></span> |
| <span data-ttu-id="d6ca3-141">Ninguno</span><span class="sxs-lookup"><span data-stu-id="d6ca3-141">None</span></span> | <span data-ttu-id="d6ca3-142">La dirección es incorrecta.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-142">Address is incorrect.</span></span> | <span data-ttu-id="d6ca3-143">Ninguno</span><span class="sxs-lookup"><span data-stu-id="d6ca3-143">None</span></span> |
| <span data-ttu-id="d6ca3-144">NotValidated</span><span class="sxs-lookup"><span data-stu-id="d6ca3-144">NotValidated</span></span> | <span data-ttu-id="d6ca3-145">No se pudo enviar la dirección a través del proceso de validación.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-145">Address was not able to be sent through the validation process.</span></span>  | <span data-ttu-id="d6ca3-146">Ninguno</span><span class="sxs-lookup"><span data-stu-id="d6ca3-146">None</span></span> |

<span data-ttu-id="d6ca3-147">Una vez que se ha enviado una dirección que se va a validar a través de la API ValidateAddress, se devolverá el esquema de respuesta siguiente:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-147">Once an address has been submitted to be validated via the ValidateAddress API, the following response schema will be returned:</span></span>

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

<span data-ttu-id="d6ca3-148">Eche un vistazo a esta respuesta de ejemplo.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-148">Take a look at this sample response.</span></span> <span data-ttu-id="d6ca3-149">Tenga en cuenta que para EE. UU., si solo escribe cinco dígitos para el código postal, la respuesta devolverá un sufijo adicional de cuatro dígitos para la línea de código postal.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-149">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

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

### <a name="next-steps"></a><span data-ttu-id="d6ca3-150">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-150">Next steps</span></span>

- <span data-ttu-id="d6ca3-151">Comparta su id. de inquilino de espacio aislado con nuestro experto en la materia (SME), Ali Khaki, para que se incluya en el piloto de prueba, de modo que pueda empezar a preparar la actualización.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-151">Share your sandbox tenant ID with our subject matter expert (SME), Ali Khaki, to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="d6ca3-152">Si usa una solución de proveedor de panel de control (CPV), consulte a su CPV.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-152">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="d6ca3-153">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="d6ca3-153">Questions?</span></span>

<span data-ttu-id="d6ca3-154">Si tiene alguna pregunta o necesita soporte técnico para las operaciones con Microsoft, póngase en contacto con el grupo de Yammer del soporte técnico del asociado.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-154">If you have any questions or need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="d6ca3-155">Experiencia del nuevo Centro de administración de Exchange (EAC)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-155">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-156">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-156">Categories</span></span>

- <span data-ttu-id="d6ca3-157">Fecha: 29/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-157">Date: 2021-03-29</span></span>
- <span data-ttu-id="d6ca3-158">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="d6ca3-158">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d6ca3-159">Resumen</span><span class="sxs-lookup"><span data-stu-id="d6ca3-159">Summary</span></span>

<span data-ttu-id="d6ca3-160">A partir del 27 de abril de 2021, el Centro de administración de Exchange (EAC) implementará una nueva experiencia que mejorará la eficacia diaria de los usuarios.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-160">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-161">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-161">Impacted audience</span></span>

<span data-ttu-id="d6ca3-162">Administradores delegados que acceden a Exchange a través del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-162">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-163">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-163">Details</span></span>

<span data-ttu-id="d6ca3-164">A partir del 27 de abril de 2021, los asociados que naveguen a Exchange a través del Centro de partners se redirigirán al nuevo EAC.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-164">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="d6ca3-165">Esta nueva experiencia está disponible actualmente como versión preliminar y los administradores pueden activarla seleccionando el botón de alternancia en la esquina superior derecha en el EAC clásico.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-165">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="d6ca3-166">También pueden navegar al nuevo EAC seleccionando el banner "Probar ahora" que se muestra en todas las páginas.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-166">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="d6ca3-167">Entre las ventajas del nuevo EAC se incluyen:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-167">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="d6ca3-168">Se ha agregado información, informes y mecanismos de alerta para problemas relacionados con el flujo de correo.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-168">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="d6ca3-169">Paneles personalizados para aumentar la productividad.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-169">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="d6ca3-170">Para ayudarle a navegar por la nueva experiencia, puede encontrar vídeos en la sección **Entrenamiento y guía** en la nueva experiencia de EAC.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-170">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="d6ca3-171">Esto le proporcionará una visión general de cómo puede usar mejor el nuevo portal.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-171">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="d6ca3-172">Con este cambio, la experiencia clásica de EAC no estará en desuso.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-172">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="d6ca3-173">Recibirá una notificación con antelación suficiente antes de que se implemente este cambio.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-173">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d6ca3-174">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-174">Next steps</span></span>

- <span data-ttu-id="d6ca3-175">Consulte los [recursos sobre este tema](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), donde puede ver capturas de pantallas de la nueva experiencia.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-175">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="d6ca3-176">Comparta esta información con las partes interesadas pertinentes de su organización.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-176">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="d6ca3-177">¿Tiene preguntas?</span><span class="sxs-lookup"><span data-stu-id="d6ca3-177">Questions?</span></span>

<span data-ttu-id="d6ca3-178">Si tiene preguntas sobre estos cambios, consulte a las comunidades de Yammer correspondientes.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-178">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="d6ca3-179">Microsoft Operations: Presentación del calendario de lanzamiento del producto</span><span class="sxs-lookup"><span data-stu-id="d6ca3-179">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-180">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-180">Categories</span></span>

- <span data-ttu-id="d6ca3-181">Fecha: 25/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-181">Date: 2021-03-25</span></span>
- <span data-ttu-id="d6ca3-182">Ofertas / Modern Workplace</span><span class="sxs-lookup"><span data-stu-id="d6ca3-182">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="d6ca3-183">Resumen</span><span class="sxs-lookup"><span data-stu-id="d6ca3-183">Summary</span></span>

<span data-ttu-id="d6ca3-184">En respuesta a los comentarios de los asociados, Microsoft Operations simplificará las comunicaciones de los lanzamientos de productos.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-184">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-185">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-185">Impacted audience</span></span>

<span data-ttu-id="d6ca3-186">Partners del programa Proveedor de soluciones en la nube (CSP)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-186">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-187">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-187">Details</span></span>

<span data-ttu-id="d6ca3-188">Microsoft se compromete a mejorar continuamente las experiencias de los asociados.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-188">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="d6ca3-189">Hemos recibido comentarios sobre el hecho de recibir demasiadas comunicaciones de Microsoft, incluidos anuncios duplicados de lanzamientos de productos.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-189">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="d6ca3-190">En respuesta a sus comentarios, Microsoft ha simplificado la experiencia de preparación de los lanzamientos de productos para ofertas nuevas y existentes.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-190">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="d6ca3-191">Ahora le proporcionamos una vista mensual única de los lanzamientos de productos publicados en la galería de recursos de preparación de operaciones.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-191">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="d6ca3-192">Esta [vista de calendario de lanzamientos de productos](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) mensual reemplazará las comunicaciones de lanzamiento de productos individuales en la galería de recursos de preparación de operaciones y en los anuncios del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-192">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="d6ca3-193">También puede acceder a este [calendario de lanzamientos de productos](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) desde [colecciones de la comunidad](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [vistas de calendario](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated) y [boletines de CSP](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-193">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="d6ca3-194">Recibirá una notificación cuando publiquemos el calendario de lanzamientos de productos de cada mes con un anuncio en la galería de recursos de preparación de operaciones.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-194">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="d6ca3-195">Todavía puede encontrar información sobre ofertas nuevas y existentes en la vista previa de la lista de precios y en los registros de cambios de la lista de precios, así como en blogs de productos, guías de licencia y páginas de marketing del producto.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-195">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="d6ca3-196">El cambio se aplicará a los lanzamientos de los siguientes productos:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-196">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="d6ca3-197">Dynamics local</span><span class="sxs-lookup"><span data-stu-id="d6ca3-197">Dynamics on-premises</span></span>
- <span data-ttu-id="d6ca3-198">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d6ca3-198">Microsoft 365</span></span>
- <span data-ttu-id="d6ca3-199">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="d6ca3-199">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="d6ca3-200">Windows</span><span class="sxs-lookup"><span data-stu-id="d6ca3-200">Windows</span></span>
- <span data-ttu-id="d6ca3-201">Servidor</span><span class="sxs-lookup"><span data-stu-id="d6ca3-201">Server</span></span>  
- <span data-ttu-id="d6ca3-202">Herramientas</span><span class="sxs-lookup"><span data-stu-id="d6ca3-202">Tools</span></span>
- <span data-ttu-id="d6ca3-203">Teams y Telco</span><span class="sxs-lookup"><span data-stu-id="d6ca3-203">Teams and Telco</span></span>

<span data-ttu-id="d6ca3-204">Seguiremos enviando anuncios específicos de lanzamientos de productos que requieran detalles de preparación de operaciones.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-204">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d6ca3-205">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-205">Next steps</span></span>

<span data-ttu-id="d6ca3-206">Revise los recursos sobre este tema y comparta esta información con las partes interesadas adecuadas de su organización.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-206">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="d6ca3-207">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="d6ca3-207">Questions?</span></span>

<span data-ttu-id="d6ca3-208">Si tiene alguna pregunta más sobre estas ofertas, consulte con las comunidades de Yammer correspondientes.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-208">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="d6ca3-209">Cambios en los requisitos de incorporación de clientes de CSP</span><span class="sxs-lookup"><span data-stu-id="d6ca3-209">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-210">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-210">Categories</span></span>

- <span data-ttu-id="d6ca3-211">Fecha: 25/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-211">Date: 2021-03-25</span></span>
- <span data-ttu-id="d6ca3-212">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="d6ca3-212">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d6ca3-213">Resumen</span><span class="sxs-lookup"><span data-stu-id="d6ca3-213">Summary</span></span>

<span data-ttu-id="d6ca3-214">Como parte de nuestro compromiso para ayudar a los asociados y los clientes a llevar a cabo sus actividades empresariales basándose en la confianza, solicitaremos información adicional del cliente. Esto entrará en vigor el 25 de marzo de 2021.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-214">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-215">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-215">Impacted audience</span></span>

<span data-ttu-id="d6ca3-216">Los asociados de CSP Direct Bill Partner y proveedores indirectos del Proveedor de soluciones en la nube (CSP) con clientes nuevos o existentes en los países que se indican en la sección siguiente.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-216">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-217">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-217">Details</span></span>

<span data-ttu-id="d6ca3-218">Microsoft funciona con confianza.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-218">Microsoft runs on trust.</span></span> <span data-ttu-id="d6ca3-219">Nos comprometemos a proporcionar un método compatible, seguro y protegido para la validación de clientes durante las operaciones de transacción con suscripciones de clientes en el programa CSP.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-219">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="d6ca3-220">El 25 de marzo de 2021, presentaremos mejoras en la interfaz de usuario y la API del Centro de partners que afectarán a los partners que cumplan los criterios siguientes:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-220">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="d6ca3-221">El partner tiene una relación de factura directa con Microsoft (lo que significa que se trata de un partner de factura directa o de un proveedor indirecto).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-221">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="d6ca3-222">El asociado hace negocios con clientes nuevos o existentes en los siguientes países:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-222">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="d6ca3-223">Tailandia</span><span class="sxs-lookup"><span data-stu-id="d6ca3-223">Thailand</span></span>
    - <span data-ttu-id="d6ca3-224">Vietnam</span><span class="sxs-lookup"><span data-stu-id="d6ca3-224">Vietnam</span></span>
    - <span data-ttu-id="d6ca3-225">Turquía</span><span class="sxs-lookup"><span data-stu-id="d6ca3-225">Turkey</span></span>
    - <span data-ttu-id="d6ca3-226">Polonia</span><span class="sxs-lookup"><span data-stu-id="d6ca3-226">Poland</span></span>
    - <span data-ttu-id="d6ca3-227">Sudáfrica</span><span class="sxs-lookup"><span data-stu-id="d6ca3-227">South Africa</span></span>
    - <span data-ttu-id="d6ca3-228">India</span><span class="sxs-lookup"><span data-stu-id="d6ca3-228">India</span></span>
    - <span data-ttu-id="d6ca3-229">Brasil</span><span class="sxs-lookup"><span data-stu-id="d6ca3-229">Brazil</span></span>
    - <span data-ttu-id="d6ca3-230">Iraq</span><span class="sxs-lookup"><span data-stu-id="d6ca3-230">Iraq</span></span>
    - <span data-ttu-id="d6ca3-231">Myanmar</span><span class="sxs-lookup"><span data-stu-id="d6ca3-231">Myanmar</span></span>
    - <span data-ttu-id="d6ca3-232">Sudán del Sur</span><span class="sxs-lookup"><span data-stu-id="d6ca3-232">South Sudan</span></span>
    - <span data-ttu-id="d6ca3-233">Arabia Saudí</span><span class="sxs-lookup"><span data-stu-id="d6ca3-233">Saudi Arabia</span></span>
    - <span data-ttu-id="d6ca3-234">Emiratos Árabes Unidos</span><span class="sxs-lookup"><span data-stu-id="d6ca3-234">United Arab Emirates</span></span>
    - <span data-ttu-id="d6ca3-235">Venezuela</span><span class="sxs-lookup"><span data-stu-id="d6ca3-235">Venezuela</span></span>

<span data-ttu-id="d6ca3-236">Los asociados que cumplan los criterios tendrán que enviar el **identificador de registro de la compañía** (también conocido como **INN de la organización** del cliente) y el **número de teléfono** del cliente cuando incorporen clientes nuevos o modifiquen los detalles de clientes existentes.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-236">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="d6ca3-237">Estos partners también pueden escribir un **segundo nombre** opcional para el cliente.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-237">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="d6ca3-238">Tenga en cuenta que, al agregar el identificador de registro de la compañía, debe usar el id. de impuesto empresarial y no el identificador personal del cliente.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-238">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="d6ca3-239">Los partners que llevan a cabo actividades empresariales con clientes nuevos o existentes de los países siguientes ya se incorporaron con una versión anterior en noviembre de 2020.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-239">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="d6ca3-240">Armenia</span><span class="sxs-lookup"><span data-stu-id="d6ca3-240">Armenia</span></span>
- <span data-ttu-id="d6ca3-241">Azerbaiyán</span><span class="sxs-lookup"><span data-stu-id="d6ca3-241">Azerbaijan</span></span>
- <span data-ttu-id="d6ca3-242">Belarús</span><span class="sxs-lookup"><span data-stu-id="d6ca3-242">Belarus</span></span>
- <span data-ttu-id="d6ca3-243">Hungría</span><span class="sxs-lookup"><span data-stu-id="d6ca3-243">Hungary</span></span>
- <span data-ttu-id="d6ca3-244">Kazajistán</span><span class="sxs-lookup"><span data-stu-id="d6ca3-244">Kazakhstan</span></span>
- <span data-ttu-id="d6ca3-245">Kirguistán</span><span class="sxs-lookup"><span data-stu-id="d6ca3-245">Kyrgyzstan</span></span>
- <span data-ttu-id="d6ca3-246">Moldova</span><span class="sxs-lookup"><span data-stu-id="d6ca3-246">Moldova</span></span>
- <span data-ttu-id="d6ca3-247">Rusia</span><span class="sxs-lookup"><span data-stu-id="d6ca3-247">Russia</span></span>
- <span data-ttu-id="d6ca3-248">Tayikistán</span><span class="sxs-lookup"><span data-stu-id="d6ca3-248">Tajikistan</span></span>
- <span data-ttu-id="d6ca3-249">Ucrania</span><span class="sxs-lookup"><span data-stu-id="d6ca3-249">Ukraine</span></span>
- <span data-ttu-id="d6ca3-250">Uzbekistán</span><span class="sxs-lookup"><span data-stu-id="d6ca3-250">Uzbekistan</span></span>

<span data-ttu-id="d6ca3-251">Los asociados con clientes en el resto del mundo podrán, a partir del 25 de marzo de 2021, escribir el **identificador de registro de la compañía**, el **número de teléfono** y el **segundo nombre** de los clientes como detalles opcionales.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-251">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d6ca3-252">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-252">Next steps</span></span>

- <span data-ttu-id="d6ca3-253">Revise la documentación técnica y las preguntas más frecuentes en la [colección específica para asociados](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) a fin de obtener instrucciones más detalladas.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-253">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="d6ca3-254">Prepárese para incorporar los cambios mediante la API del Centro de partners y la experiencia de usuario web.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-254">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="d6ca3-255">Habrá API y SDK disponibles para realizar pruebas.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-255">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="d6ca3-256">Asegúrese de enviar los datos adicionales al incorporar clientes nuevos o modificar los datos de clientes existentes.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-256">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="d6ca3-257">Si usa una solución de proveedor de panel de control (CPV), consulte a su CPV.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-257">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="d6ca3-258">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="d6ca3-258">Questions?</span></span>

<span data-ttu-id="d6ca3-259">Si tiene alguna pregunta relacionada con el identificador legal (también denominado INN o CIF/NIF), póngase en contacto con su asesor fiscal o con la agencia tributaria local.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-259">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="d6ca3-260">Microsoft no puede proporcionar orientación sobre cuestiones fiscales.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-260">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="d6ca3-261">Si necesita soporte técnico con relación a sus operaciones con Microsoft, [abra una solicitud de servicio](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-261">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="d6ca3-262">Correcciones realizadas a la lista de precios de software perpetuo del 1 de marzo de 2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-262">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-263">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-263">Categories</span></span>

- <span data-ttu-id="d6ca3-264">Fecha: 23/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-264">Date: 2021-03-23</span></span>
- <span data-ttu-id="d6ca3-265">Ofertas/mercados</span><span class="sxs-lookup"><span data-stu-id="d6ca3-265">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-266">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-266">Impacted audience</span></span>

<span data-ttu-id="d6ca3-267">Proveedores indirectos y partners directos de facturación que realicen transacciones de software perpetuo en el programa Proveedor de soluciones en la nube</span><span class="sxs-lookup"><span data-stu-id="d6ca3-267">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="d6ca3-268">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-268">Details</span></span>

<span data-ttu-id="d6ca3-269">La lista de precios para el software perpetuo publicada el 1 de marzo de 2021 incluía mercados que no deberían estar allí.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-269">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="d6ca3-270">La lista de precios de software perpetuo se actualizó el 17 de marzo de 2021 con las correcciones.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-270">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="d6ca3-271">Estas correcciones solo se aplican a:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-271">These corrections were only applicable to:</span></span>

- <span data-ttu-id="d6ca3-272">Id. de producto: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="d6ca3-272">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="d6ca3-273">Nombre del producto: actualización de Windows 10 Home a Pro para Microsoft 365 Empresa</span><span class="sxs-lookup"><span data-stu-id="d6ca3-273">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="d6ca3-274">Mercados quitados o no admitidos: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span><span class="sxs-lookup"><span data-stu-id="d6ca3-274">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="d6ca3-275">Estos cambios solo se aplican al producto anterior.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-275">These changes only apply to the above product.</span></span> <span data-ttu-id="d6ca3-276">Otros productos no tenían correcciones.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-276">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="d6ca3-277">Pasos y recursos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-277">Next steps and resources</span></span>

- <span data-ttu-id="d6ca3-278">Los partners que realizan transacciones de software perpetuo deben descargar la lista de precios de software perpetuo más reciente.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-278">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="d6ca3-279">Consulte los [códigos de país de la región](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) para una asignación descriptiva de la abreviatura de dos letras a los países.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-279">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a><span data-ttu-id="d6ca3-280">Versión del SDK en .NET Standard (v1.17.0)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-280">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-281">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-281">Categories</span></span>

- <span data-ttu-id="d6ca3-282">Fecha: 23/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-282">Date: 2021-03-23</span></span>

- <span data-ttu-id="d6ca3-283">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="d6ca3-283">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-284">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-284">Impacted audience</span></span>

<span data-ttu-id="d6ca3-285">Partners de factura directa y proveedores indirectos que participan en el programa CSP y que usan el SDK de .NET del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-285">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-286">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-286">Details</span></span>

<span data-ttu-id="d6ca3-287">A partir del 23 de marzo de 2020, los partners pueden empezar a descargar la versión de [MicrosoftPartnerCenter.NETSDK (galería de NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), junto con los [ejemplos de GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples) actualizados públicos del SDK del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-287">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="d6ca3-288">Esta versión incluye actualizaciones para los métodos siguientes:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-288">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="d6ca3-289">Auditoría actualizada: nuevos tipos de operación</span><span class="sxs-lookup"><span data-stu-id="d6ca3-289">Audit Updated: New operation types</span></span>

<span data-ttu-id="d6ca3-290">Se han agregado nuevos [tipos de operación](https://docs.microsoft.com/partner-center/develop/auditing-resources) para saber cuándo el cliente ha aprobado y finalizado DAP.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-290">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="d6ca3-291">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="d6ca3-291">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="d6ca3-292">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="d6ca3-292">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="d6ca3-293">Auditoría actualizada: nuevos tipos de recursos y operaciones</span><span class="sxs-lookup"><span data-stu-id="d6ca3-293">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="d6ca3-294">Se han agregado nuevos [tipos de recursos y operaciones](https://docs.microsoft.com/partner-center/develop/auditing-resources) para admitir el escenario de rol del directorio del cliente.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-294">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="d6ca3-295">Nuevo tipo de recurso "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="d6ca3-295">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="d6ca3-296">Tipos de operación "AddUserMember" y "RemoveUserMember"</span><span class="sxs-lookup"><span data-stu-id="d6ca3-296">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="d6ca3-297">Actualizaciones del SDK para cuentas de cliente</span><span class="sxs-lookup"><span data-stu-id="d6ca3-297">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="d6ca3-298">Compatibilidad con GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span><span class="sxs-lookup"><span data-stu-id="d6ca3-298">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="d6ca3-299">GET /customers/{customer-tenant-id}/qualifications</span><span class="sxs-lookup"><span data-stu-id="d6ca3-299">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="d6ca3-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span><span class="sxs-lookup"><span data-stu-id="d6ca3-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="d6ca3-301">Cambios adicionales</span><span class="sxs-lookup"><span data-stu-id="d6ca3-301">Additional changes</span></span>

<span data-ttu-id="d6ca3-302">Los cambios siguientes se incluyen como parte del nuevo comercio y actualmente están disponibles por invitación solo para los partners que forman parte de la versión preliminar técnica de la experiencia del nuevo comercio de M365/D365.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-302">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="d6ca3-303">Los partners que no forman parte de la versión preliminar técnica del nuevo comercio no deberían notar los impactos y deberían ser compatibles con versiones anteriores.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-303">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="d6ca3-304">Cambios en el catálogo:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-304">Catalog Changes:</span></span>

  - <span data-ttu-id="d6ca3-305">GET /products/{product-id}/skus/{sku-id}</span><span class="sxs-lookup"><span data-stu-id="d6ca3-305">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="d6ca3-306">Compra y administración:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-306">Purchase and Manage:</span></span>
  - <span data-ttu-id="d6ca3-307">GET /customers/{customerId}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="d6ca3-307">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="d6ca3-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="d6ca3-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="d6ca3-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="d6ca3-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="d6ca3-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="d6ca3-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="d6ca3-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="d6ca3-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="d6ca3-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="d6ca3-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="d6ca3-313">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-313">Next Steps</span></span>

- <span data-ttu-id="d6ca3-314">Descargue la versión más reciente de [MicrosoftPartnerCenter.NETSDK (galería de NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-314">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="d6ca3-315">Descargue y revise los [ejemplos de GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-315">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="d6ca3-316">Oferta del marketplace comercial para CSP e incentivos de CSP para ofertas válidas en el año fiscal 2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-316">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-317">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-317">Categories</span></span>

- <span data-ttu-id="d6ca3-318">Fecha: 18/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-318">Date: 2021-03-18</span></span>
- <span data-ttu-id="d6ca3-319">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="d6ca3-319">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-320">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-320">Impacted audience</span></span>

<span data-ttu-id="d6ca3-321">Proveedores indirectos y partners de factura directa del programa Proveedor de soluciones en la nube</span><span class="sxs-lookup"><span data-stu-id="d6ca3-321">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="d6ca3-322">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-322">Details</span></span>

<span data-ttu-id="d6ca3-323">Los proveedores indirectos y los partners de factura directa del programa Proveedor de soluciones en la nube pueden vender ofertas de terceros y obtener un incentivo de descuento por cada oferta de terceros apta cuya transacción se realice en el Centro de partners o en Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-323">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="d6ca3-324">El incentivo será en forma de descuento en las ventas facturadas de las ofertas aptas y estará **disponible hasta el 30 de junio de 2021**.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-324">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="d6ca3-325">Obtenga más información sobre este incentivo de la oferta del marketplace comercial de CSP más abajo, y póngase en contacto con sus clientes hoy mismo para identificar las ofertas adecuadas para facilitar su éxito y transformación digital.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-325">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="d6ca3-326">Nos hemos asociado con fabricantes de software independientes (ISV) para incorporar las soluciones de IaaS y SaaS más recientes al mercado de los clientes de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-326">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="d6ca3-327">Los editores de ISV tienen la opción de permitir las ventas de sus ofertas a través del canal de partners de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-327">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="d6ca3-328">Nuestras ofertas aptas para incentivos se dividen en dos categorías:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-328">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="d6ca3-329">Seleccione las ofertas de terceros de SaaS e IaaS con el estado de incentivo de venta conjunta de IP de Azure.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-329">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="d6ca3-330">Aplicaciones SaaS integradas con Teams o al menos dos aplicaciones de productividad de Microsoft 365, como PowerPoint, Word, Excel, Outlook o SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-330">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="d6ca3-331">Pasos y recursos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-331">Next steps and resources</span></span>

- <span data-ttu-id="d6ca3-332">Obtenga información sobre la obtención de [incentivos para partners](https://partner.microsoft.com/membership/partner-incentives) por la venta de aplicaciones aptas del marketplace.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-332">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="d6ca3-333">Las nuevas ofertas se agregan mensualmente.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-333">New offers are added monthly.</span></span>  
- [<span data-ttu-id="d6ca3-334">Recursos de incentivos para partners de factura directa del Proveedor de soluciones en la nube</span><span class="sxs-lookup"><span data-stu-id="d6ca3-334">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="d6ca3-335">Recursos de incentivos para proveedores indirectos del Proveedor de soluciones en la nube</span><span class="sxs-lookup"><span data-stu-id="d6ca3-335">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="d6ca3-336">Revise esta [presentación](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) para obtener más información sobre cómo vender las aplicaciones del marketplace comercial.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-336">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="d6ca3-337">Consulte [aquí](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/) los recursos adicionales.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-337">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="d6ca3-338">Explore el catálogo del marketplace comercial en el [Centro de partners](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) o en [Azure Portal](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-338">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="d6ca3-339">Use las [API](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) para integrar aplicaciones en el marketplace de su empresa.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-339">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="d6ca3-340">Póngase en contacto con los fabricantes de software independientes con los que está interesado en tener relaciones comerciales.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-340">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="d6ca3-341">Los proveedores indirectos deben integrarse con las API y guiar a los revendedores en qué aplicaciones se deben vender.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-341">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="d6ca3-342">¿Alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="d6ca3-342">Questions?</span></span>  

<span data-ttu-id="d6ca3-343">Consulte [este artículo](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) para obtener información general sobre el marketplace comercial en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-343">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="d6ca3-344">Si necesita más ayuda, puede crear una solicitud de soporte técnico en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-344">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="d6ca3-345">Obtenga más información en [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-345">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="d6ca3-346">Actualización de nomenclatura de ofertas y de requisitos previos de Power BI Premium</span><span class="sxs-lookup"><span data-stu-id="d6ca3-346">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-347">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-347">Categories</span></span>

- <span data-ttu-id="d6ca3-348">Fecha: 18/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-348">Date: 2021-03-18</span></span>
- <span data-ttu-id="d6ca3-349">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="d6ca3-349">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d6ca3-350">Resumen</span><span class="sxs-lookup"><span data-stu-id="d6ca3-350">Summary</span></span>

<span data-ttu-id="d6ca3-351">La lista final de precios del 1 de abril de 2021 se actualizará para agregar claridad a la información de nomenclatura o requisitos previos para las ofertas de Power BI Premium por usuario.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-351">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-352">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-352">Impacted audience</span></span>

<span data-ttu-id="d6ca3-353">Partners directos e indirectos del programa Proveedor de soluciones en la nube (CSP)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-353">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-354">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-354">Details</span></span>

<span data-ttu-id="d6ca3-355">La lista final de precios del 1 de abril de 2021 se actualizará para agregar claridad a la información de nomenclatura o requisitos previos para las ofertas de Power BI Premium por usuario.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="d6ca3-356">Hasta que se actualice la lista final de precios, use la información de esta sección para asegurarse de que se pida el producto correcto.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-356">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="d6ca3-357">Los detalles siguientes muestran la SKU afectada y los detalles de los requisitos previos.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-357">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="d6ca3-358">Nombre para mostrar de la oferta en la versión preliminar de la lista de precios del 1 de marzo</span><span class="sxs-lookup"><span data-stu-id="d6ca3-358">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="d6ca3-359">Nombre para mostrar de la oferta actualizada del 1 de abril de la lista final de precios</span><span class="sxs-lookup"><span data-stu-id="d6ca3-359">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="d6ca3-360">Id. de oferta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-360">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="d6ca3-361">Complemento Power BI Premium por usuario (precios para personal de ONG)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-361">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="d6ca3-362">Complemento de Power BI Premium por usuario **(Office)** (precios para personal de organizaciones sin ánimo de lucro)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-362">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="d6ca3-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="d6ca3-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="d6ca3-364">Los clientes deben cumplir alguno de los siguientes requisitos previos para comprar esta oferta:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-364">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="d6ca3-365">Nombre para mostrar de la oferta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-365">Offer display name</span></span> | <span data-ttu-id="d6ca3-366">Id. de oferta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-366">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="d6ca3-367">Microsoft 365 E5 (precios para personal de organizaciones sin ánimo de lucro)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-367">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="d6ca3-368">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="d6ca3-368">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="d6ca3-369">Microsoft 365 E5 sin audioconferencia (precios para personal de organizaciones sin ánimo de lucro)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-369">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="d6ca3-370">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="d6ca3-370">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="d6ca3-371">Office 365 E5 (precios para personal de organizaciones sin ánimo de lucro)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-371">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="d6ca3-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="d6ca3-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="d6ca3-373">Versión de evaluación de Office 365 E5 (precios para personal de organizaciones sin ánimo de lucro)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-373">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="d6ca3-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="d6ca3-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="d6ca3-375">Office 365 E5 sin audioconferencia (precios para personal de organizaciones sin ánimo de lucro)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-375">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="d6ca3-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="d6ca3-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="d6ca3-377">La siguiente oferta de Power BI Premium tiene un requisito previo para la compra:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-377">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="d6ca3-378">Nombre para mostrar de la oferta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-378">Offer display name</span></span> | <span data-ttu-id="d6ca3-379">Id. de oferta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-379">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="d6ca3-380">Complemento Power BI Premium por usuario (precios para personal de ONG)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-380">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="d6ca3-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="d6ca3-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="d6ca3-382">Los clientes deben tener este requisito previo para comprar esta oferta:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-382">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="d6ca3-383">Nombre para mostrar de la oferta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-383">Offer display name</span></span> | <span data-ttu-id="d6ca3-384">Id. de oferta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-384">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="d6ca3-385">Power BI Pro (precios para personal de organizaciones sin ánimo de lucro)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-385">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="d6ca3-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="d6ca3-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="d6ca3-387">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-387">Next steps</span></span>

<span data-ttu-id="d6ca3-388">Revise los recursos sobre este tema y comparta esta información con las partes interesadas adecuadas de su organización.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-388">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="d6ca3-389">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="d6ca3-389">Questions?</span></span>

<span data-ttu-id="d6ca3-390">Si tiene preguntas sobre estas ofertas, consulte a las comunidades de Yammer correspondientes.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-390">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> <span data-ttu-id="d6ca3-391">Actualizaciones de precios de marzo de Microsoft 365 F3</span><span class="sxs-lookup"><span data-stu-id="d6ca3-391">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-392">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-392">Categories</span></span>

- <span data-ttu-id="d6ca3-393">Fecha: 16/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-393">Date: 2021-03-16</span></span>
- <span data-ttu-id="d6ca3-394">Ofertas/mercados</span><span class="sxs-lookup"><span data-stu-id="d6ca3-394">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="d6ca3-395">Resumen</span><span class="sxs-lookup"><span data-stu-id="d6ca3-395">Summary</span></span>

<span data-ttu-id="d6ca3-396">Se han corregido los precios incorrectos de marzo de 2021 para Microsoft 365 F3 en libras (GBP) y euros (EUR).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-396">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-397">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-397">Impacted audience</span></span>

<span data-ttu-id="d6ca3-398">Los partners que compren Microsoft 365 F3 en GBP o EUR entre el 1 de marzo y el 17 de marzo de 2021 a través del programa Proveedor de soluciones en la nube (CSP).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-398">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-399">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-399">Details</span></span>

<span data-ttu-id="d6ca3-400">Microsoft ha solucionado los precios incorrectos para Microsoft 365 F3.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-400">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="d6ca3-401">Los precios incorrectos eran para GBP y EUR, y solo para las ofertas adquiridas entre el 1 de marzo y el 17 de marzo de 2021.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-401">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="d6ca3-402">A continuación, se muestran las ofertas y las monedas afectadas.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-402">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="d6ca3-403">Nombre de la oferta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-403">Offer name</span></span> | <span data-ttu-id="d6ca3-404">Moneda</span><span class="sxs-lookup"><span data-stu-id="d6ca3-404">Currency</span></span> | <span data-ttu-id="d6ca3-405">Id. de oferta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-405">Offer ID</span></span> | <span data-ttu-id="d6ca3-406">Id. de material</span><span class="sxs-lookup"><span data-stu-id="d6ca3-406">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="d6ca3-407">Microsoft 365 F3 (ONG)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-407">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="d6ca3-408">GBP</span><span class="sxs-lookup"><span data-stu-id="d6ca3-408">GBP</span></span> | <span data-ttu-id="d6ca3-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="d6ca3-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="d6ca3-410">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="d6ca3-410">AAD-11626</span></span> |
| <span data-ttu-id="d6ca3-411">Microsoft 365 F3 (comercial)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-411">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="d6ca3-412">EUR</span><span class="sxs-lookup"><span data-stu-id="d6ca3-412">EUR</span></span>| <span data-ttu-id="d6ca3-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="d6ca3-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="d6ca3-414">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="d6ca3-414">AAA-89898</span></span> |
 
<span data-ttu-id="d6ca3-415">Las listas de precios basados en licencias de la versión preliminar de marzo y abril se actualizaron el 16 de marzo, a las 17:00 horas (hora estándar del Pacífico).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-415">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d6ca3-416">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-416">Next steps</span></span>

- <span data-ttu-id="d6ca3-417">Los partners deben volver a descargar las listas de precios actuales basados en licencias, tanto de la versión preliminar de marzo como de abril, con las correcciones de precios, si procede.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-417">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="d6ca3-418">Microsoft se pondrá en contacto con los partners afectados en las próximas semanas a través del correo electrónico para informarles sobre los siguientes pasos relacionados con la corrección de las transacciones afectadas.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-418">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="d6ca3-419">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="d6ca3-419">Questions?</span></span>

<span data-ttu-id="d6ca3-420">Si tiene alguna pregunta, póngase en contacto con las comunidades de Yammer de CSP correspondientes.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-420">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> <span data-ttu-id="d6ca3-421">Actualización de la razón social de una empresa a través del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="d6ca3-421">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-422">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-422">Categories</span></span>

- <span data-ttu-id="d6ca3-423">Fecha: 16/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-423">Date: 2021-03-16</span></span>
- <span data-ttu-id="d6ca3-424">Impulsar la eficiencia y la escala</span><span class="sxs-lookup"><span data-stu-id="d6ca3-424">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="d6ca3-425">Resumen</span><span class="sxs-lookup"><span data-stu-id="d6ca3-425">Summary</span></span>

<span data-ttu-id="d6ca3-426">A partir de marzo de 2021, los partners de Microsoft Partner Network (MPN) y los revendedores indirectos del Proveedor de soluciones en la nube (CSP) pueden actualizar la razón social de su empresa a través del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-426">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-427">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-427">Impacted audience</span></span>

<span data-ttu-id="d6ca3-428">Partners de MPN y revendedores indirectos de CSP (no aplicables a partners de facturación directa de CSP)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-428">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-429">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-429">Details</span></span>

<span data-ttu-id="d6ca3-430">A partir de marzo de 2021, los partners de MPN y los revendedores indirectos de CSP pueden actualizar la razón social de su empresa a través del Centro de partners por su cuenta y conforme a la normativa.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-430">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="d6ca3-431">Con esta nueva característica, los partners ya no tendrán que enviar una incidencia de soporte técnico del Centro de partners para actualizar el nombre de su empresa.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-431">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="d6ca3-432">Esto ahorrará una cantidad significativa de tiempo a los asociados al realizar estas actividades.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-432">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="d6ca3-433">Para más información, consulte [Actualización del perfil legal de la empresa](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-433">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="d6ca3-434">Asegúrese de que el nombre de la empresa en el perfil empresarial legal no tenga errores ortográficos ni abreviaturas, y de que coincida exactamente con los registros de inscripción formales de la empresa.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-434">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="d6ca3-435">Para obtener más información sobre cómo actualizar el perfil de la organización, consulte [Verificación del perfil de la organización](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-435">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="d6ca3-436">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-436">Next steps</span></span>

<span data-ttu-id="d6ca3-437">Comparta esta información en su organización para que el equipo adecuado pueda revisar y actualizar sus procesos.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-437">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="d6ca3-438">¿Alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="d6ca3-438">Questions?</span></span>

<span data-ttu-id="d6ca3-439">Si tiene alguna pregunta, póngase en contacto con las comunidades de Yammer de CSP correspondientes.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-439">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> <span data-ttu-id="d6ca3-440">Actualización de la evolución del programa Proveedor de soluciones en la nube (CSP) y cambios en el programa Open License</span><span class="sxs-lookup"><span data-stu-id="d6ca3-440">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-441">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-441">Categories</span></span>

- <span data-ttu-id="d6ca3-442">Fecha: 15/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-442">Date: 2021-03-15</span></span>
- <span data-ttu-id="d6ca3-443">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="d6ca3-443">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d6ca3-444">Resumen</span><span class="sxs-lookup"><span data-stu-id="d6ca3-444">Summary</span></span>

<span data-ttu-id="d6ca3-445">Se incorporarán nuevas ofertas de software perpetuo del sector comercial y público en el programa Proveedor de soluciones en la nube (CSP) y se realizarán cambios en el programa de licencias Open.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-445">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-446">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-446">Impacted audience</span></span>

<span data-ttu-id="d6ca3-447">Distribuidores comerciales y revendedores administrados que venden productos a través del programa Open License, así como todos los partners de CSP que realizan transacciones con el software perpetuo</span><span class="sxs-lookup"><span data-stu-id="d6ca3-447">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-448">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-448">Details</span></span>

<span data-ttu-id="d6ca3-449">En septiembre de 2020, Microsoft [anunció](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) una serie de pasos en nuestro recorrido de transformación digital para expandir las oportunidades de los partners en el programa CSP, incluida la disponibilidad del software local para los partners.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-449">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="d6ca3-450">Estos cambios permiten a los partners hacer crecer su empresa y ampliar su alcance, ya que aprovechan las licencias de software de CSP y las posicionan para que logren el éxito en el mundo actual en el que se da prioridad a la nube.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-450">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="d6ca3-451">También permiten transiciones de los clientes a la nube y ofrecen a los partners la flexibilidad necesaria para los entornos de nube híbrida de los clientes.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-451">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="d6ca3-452">A fin de continuar con esta transformación digital, presentamos los siguientes cambios:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-452">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="d6ca3-453">1 de julio de 2021: no se agregarán nuevas SKU, productos ni promociones a la lista de precios del programa Open License.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-453">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="d6ca3-454">7 de julio de 2021: se agregarán dos ofertas comerciales (Get Genuine Windows y Visual Studio Professional) y ofertas del sector público (gobierno, educación y sin ánimo de lucro; consulte el [anuncio](./2020-december.md#9)) a la lista de precios del software perpetuo de CSP.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-454">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="d6ca3-455">La lista de precios puede encontrarse en la sección Software de la página [Vender > Precios y ofertas](https://partnercenter.microsoft.com/pcv/sales) del Centro de partners y se volverá a publicar en esta fecha.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-455">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="d6ca3-456">Para obtener detalles completos sobre la evolución del programa CSP y los cambios en el programa Open License, consulte **los siguientes pasos** .</span><span class="sxs-lookup"><span data-stu-id="d6ca3-456">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d6ca3-457">Pasos siguientes:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-457">Next Steps:</span></span>

- <span data-ttu-id="d6ca3-458">Evolución del programa CSP: revise los materiales de preparación para el [software perpetuo del programa Proveedor de soluciones en la nube](https://partner.microsoft.com/resources/collection/software-in-csp#/).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-458">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="d6ca3-459">Use este [mapa de preparación](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) para localizar rápidamente la información adecuada para su rol.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-459">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="d6ca3-460">Cambios en el programa Open License: revise los materiales de preparación sobre la [evolución del programa CSP y los cambios en el programa Open License](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-460">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="d6ca3-461">Use este [mapa de preparación](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) para localizar rápidamente la información adecuada para su rol.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-461">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="d6ca3-462">Preguntas</span><span class="sxs-lookup"><span data-stu-id="d6ca3-462">Questions</span></span>

<span data-ttu-id="d6ca3-463">Si tiene alguna pregunta, póngase en contacto con las comunidades de Yammer de CSP correspondientes.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-463">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="d6ca3-464">Actualización de un anuncio anterior: evaluaciones prémium, un complemento para el Administrador de cumplimiento</span><span class="sxs-lookup"><span data-stu-id="d6ca3-464">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-465">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-465">Categories</span></span>

- <span data-ttu-id="d6ca3-466">Fecha: 15/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-466">Date: 2021-03-15</span></span>
- <span data-ttu-id="d6ca3-467">Desarrollo de la empresa</span><span class="sxs-lookup"><span data-stu-id="d6ca3-467">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="d6ca3-468">Resumen</span><span class="sxs-lookup"><span data-stu-id="d6ca3-468">Summary</span></span>

<span data-ttu-id="d6ca3-469">Las ofertas de prueba no deben aparecer en la lista de precios y se quitarán.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-469">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-470">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-470">Impacted audience</span></span>

<span data-ttu-id="d6ca3-471">Todos los partners que realizan transacciones a través del Proveedor de soluciones en la nube (CSP).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-471">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-472">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-472">Details</span></span>

<span data-ttu-id="d6ca3-473">Las ofertas de prueba no se deberían haber incluido en la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-473">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="d6ca3-474">Se quitarán de la lista de precios del 1 de mayo de 2021.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-474">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="d6ca3-475">El anuncio original se encuentra [aquí](./2021-february.md#4).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-475">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="d6ca3-476">Recursos adicionales</span><span class="sxs-lookup"><span data-stu-id="d6ca3-476">Additional resources</span></span>

- [<span data-ttu-id="d6ca3-477">Seguridad y cumplimiento de Microsoft 365 E5</span><span class="sxs-lookup"><span data-stu-id="d6ca3-477">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="d6ca3-478">Creación y administración de evaluaciones en el Administrador de cumplimiento de Microsoft: Cumplimiento de Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d6ca3-478">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="d6ca3-479">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-479">Next steps</span></span>

<span data-ttu-id="d6ca3-480">Revise los recursos sobre este tema y comparta esta información con las partes interesadas adecuadas de su organización.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-480">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="d6ca3-481">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="d6ca3-481">Questions?</span></span>

<span data-ttu-id="d6ca3-482">Si tiene preguntas sobre estas ofertas, consúltelas a las comunidades de Yammer correspondientes.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-482">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="d6ca3-483">Migre sus soluciones de comercialización (GTM) de One Commercial Partner (OCP) al marketplace comercial de Microsoft</span><span class="sxs-lookup"><span data-stu-id="d6ca3-483">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-484">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-484">Categories</span></span>

- <span data-ttu-id="d6ca3-485">Fecha: 12/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-485">Date: 2021-03-12</span></span>
- <span data-ttu-id="d6ca3-486">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="d6ca3-486">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d6ca3-487">Resumen</span><span class="sxs-lookup"><span data-stu-id="d6ca3-487">Summary</span></span>

<span data-ttu-id="d6ca3-488">A partir del 29 de marzo de 2021, las funcionalidades de la herramienta de comercialización (GTM) de One Commercial Partner (OCP) se empezarán a ofrecer de forma limitada.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-488">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="d6ca3-489">Le recomendamos que migre sus soluciones al marketplace comercial en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-489">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-490">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-490">Impacted audience</span></span>

<span data-ttu-id="d6ca3-491">Organizaciones que venden de forma conjunta las soluciones de GTM de OCP</span><span class="sxs-lookup"><span data-stu-id="d6ca3-491">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-492">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-492">Details</span></span>

<span data-ttu-id="d6ca3-493">En diciembre de 2020, iniciamos nuestra transición de la herramienta de GTM de OCP de Microsoft al marketplace comercial de Microsoft en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-493">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="d6ca3-494">Este cambio amplía las funcionalidades del marketplace comercial, en el que puede presentar sus soluciones a millones de clientes, compartir de forma bidireccional las oportunidades con otros vendedores de Microsoft y partners y vender de manera conjunta soluciones innovadoras.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-494">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="d6ca3-495">El siguiente hito de la transición tendrá lugar el 29 de marzo de 2021.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-495">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="d6ca3-496">Será en ese momento cuando las funcionalidades de GTM de OCP se ofrecerán de manera limitada y algunos campos pasarán a ser de solo lectura.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-496">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="d6ca3-497">Si actualmente vende de forma conjunta soluciones en la herramienta de GTM de OCP, le recomendamos que migre sus soluciones al marketplace comercial para aprovechar sus funcionalidades y simplificar la experiencia de publicación.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-497">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="d6ca3-498">Al cambiar al marketplace comercial, el Centro de partners se convertirá en el destino principal de la experiencia de publicación de venta conjunta.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-498">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="d6ca3-499">Desde allí podrá seguir desarrollando su empresa, ya que podrá conectar sus soluciones con nuestros clientes compartidos a través de los mismos canales y experiencias en el producto que usamos para los productos de Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-499">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="d6ca3-500">[Obtenga información sobre el marketplace comercial](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-500">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="d6ca3-501">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-501">Next steps</span></span>

- <span data-ttu-id="d6ca3-502">Si aún no ha trasladado sus soluciones, siga las instrucciones detalladas en la [guía de transición](/azure/marketplace/co-sell-solution-migration) o consulte el [tutorial detallado de vídeo](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) para completar todas las actividades de migración y empezar a publicar sus soluciones en el marketplace comercial.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-502">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="d6ca3-503">Si tiene preguntas sobre cómo será su experiencia con las funcionalidades limitadas de GTM de OCP, vea los [Requisitos de venta conjunta para publicar en las preguntas más frecuentes sobre el marketplace comercial de Microsoft](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-503">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="d6ca3-504">(Consulte la sección "Funcionalidades limitadas de GTM de OCP a partir del 29 de marzo de 2021").</span><span class="sxs-lookup"><span data-stu-id="d6ca3-504">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="d6ca3-505">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="d6ca3-505">Questions?</span></span>

<span data-ttu-id="d6ca3-506">Póngase en contacto con el [soporte técnico](https://partner.microsoft.com/support/?stage=1) si tiene alguna pregunta o necesita más información.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-506">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="d6ca3-507">Expansión de la nueva experiencia comercial en el programa Proveedor de soluciones en la nube (CSP) de Azure a Rusia</span><span class="sxs-lookup"><span data-stu-id="d6ca3-507">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-508">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-508">Categories</span></span>

- <span data-ttu-id="d6ca3-509">Fecha: 10/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-509">Date: 2021-03-10</span></span>
- <span data-ttu-id="d6ca3-510">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="d6ca3-510">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-511">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-511">Impacted audience</span></span>

<span data-ttu-id="d6ca3-512">Todos los partners de Rusia que realizan transacciones a través del programa Proveedor de soluciones en la nube (CSP).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-512">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-513">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-513">Details</span></span>

<span data-ttu-id="d6ca3-514">Nos complace anunciar que la **nueva experiencia de comercio en CSP para Azure en Rusia** estará disponible a partir del 10 de marzo de 2021.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-514">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="d6ca3-515">Esta experiencia simplificará y mejorará la forma en que los clientes compran y consumen los servicios de Azure.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-515">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="d6ca3-516">También proporcionará a los partners del programa CSP una vista coherente de los precios de Azure a través de los movimientos de ventas, los precios de USD para la coherencia global, la concordancia de las fechas de facturación y el acceso a Azure Cost Management.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-516">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d6ca3-517">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-517">Next steps</span></span>

<span data-ttu-id="d6ca3-518">Hay varios recursos disponibles que presentan la nueva experiencia de comercio de Azure y proporcionan información adicional.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-518">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="d6ca3-519">Busque las preguntas más frecuentes, los conjuntos de diapositivas, los vídeos, etc. más recientes en la [Galería de recursos de actualizaciones de programas de CSP](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-519">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="d6ca3-520">Suministro de descargas y claves de licencia de software del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="d6ca3-520">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-521">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-521">Categories</span></span>

- <span data-ttu-id="d6ca3-522">Fecha: 04/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-522">Date: 2021-03-04</span></span>
- <span data-ttu-id="d6ca3-523">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="d6ca3-523">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d6ca3-524">Resumen</span><span class="sxs-lookup"><span data-stu-id="d6ca3-524">Summary</span></span>

<span data-ttu-id="d6ca3-525">Se ha restablecido la funcionalidad de suministro de descargas y claves de licencia de software del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-525">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-526">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-526">Impacted audience</span></span>

<span data-ttu-id="d6ca3-527">Todos los partners que sean Proveedores de soluciones en la nube (CSP) que operen con pedidos de software de suscripción perpetua y de servidor a través del Centro de partners</span><span class="sxs-lookup"><span data-stu-id="d6ca3-527">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-528">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-528">Details</span></span>

<span data-ttu-id="d6ca3-529">En respuesta a los comentarios de los partners, estamos restableciendo la funcionalidad de suministro del Centro de partners para obtener software y claves de licencia para los pedidos de software de suscripción perpetua y de servidor.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-529">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="d6ca3-530">Se restaurará a su estado previo antes de que se elimine el 19 de enero de 2021.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-530">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="d6ca3-531">(Vea el [anuncio](2020-september.md#17)).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-531">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="d6ca3-532">Tenga en cuenta que las claves de licencia de software y los vínculos de descarga son recursos de propiedad intelectual valiosos y muy solicitados.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-532">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="d6ca3-533">Si se filtran, se pueden agotar rápidamente sus límites de activación, lo que puede provocar una experiencia negativa para clientes y partners.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-533">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d6ca3-534">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-534">Next steps</span></span>

<span data-ttu-id="d6ca3-535">Revise los siguientes recursos para obtener instrucciones de uso e información importante sobre la distribución de las claves de software:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-535">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="d6ca3-536">Venta de software local a través del programa CSP</span><span class="sxs-lookup"><span data-stu-id="d6ca3-536">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="d6ca3-537">[Nueva guía de operaciones comerciales del Centro de partners](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (consulte la sección **Guía sobre la distribución de claves de software**).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-537">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="d6ca3-538">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="d6ca3-538">Questions?</span></span>

<span data-ttu-id="d6ca3-539">Si tiene alguna pregunta más sobre este aviso, consulte con las comunidades de Yammer correspondientes.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-539">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="d6ca3-540">Migración de las ofertas de Partner Sales Connect (PSC) al Centro de partners</span><span class="sxs-lookup"><span data-stu-id="d6ca3-540">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-541">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-541">Categories</span></span>

- <span data-ttu-id="d6ca3-542">Fecha: 04/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-542">Date: 2021-03-04</span></span>
- <span data-ttu-id="d6ca3-543">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="d6ca3-543">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d6ca3-544">Resumen</span><span class="sxs-lookup"><span data-stu-id="d6ca3-544">Summary</span></span>

<span data-ttu-id="d6ca3-545">Partner Sales Connect (PSC) se moverá a acceso de solo lectura a partir del 31 de marzo de 2021, por lo que le recomendamos que comience a migrar sus ofertas de PSC al Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-545">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-546">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-546">Impacted audience</span></span>

<span data-ttu-id="d6ca3-547">Partners con ofertas en PSC</span><span class="sxs-lookup"><span data-stu-id="d6ca3-547">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-548">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-548">Details</span></span>

<span data-ttu-id="d6ca3-549">Como parte de nuestro compromiso compartido con el crecimiento, la **venta conjunta con Microsoft** es el camino para que **le descubran, ofrezca sus conocimientos y amplíe su variedad de clientes** para obtener resultados positivos para estos.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-549">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="d6ca3-550">Con una oferta media que es **3,5 veces más rápida** que la normal, la administración de la experiencia de venta conjunta en el Centro de partners le permite vender a través de los canales de cliente directo, partner y vendedor de Microsoft, y administrar toda la canalización de referencia en una sola ubicación.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-550">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="d6ca3-551">**PSC** pasará a **acceso de solo lectura** a partir del **31 de marzo de 2021**, por lo que le recomendamos que empiece el traslado al Centro de partners y acceda a estas mejoras en la funcionalidad:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-551">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="d6ca3-552">**Enrutamiento más preciso** de las ofertas que comparte con Microsoft hacia el vendedor adecuado, en función del tipo de ayuda que necesite.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-552">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="d6ca3-553">**Validación de idoneidad de ofertas iniciales** para las soluciones aptas para incentivos y para cumplir los criterios del programa ISV Connect, al simplificar el proceso de aprobación y la atestación de prueba de ejecución (PoE) final.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-553">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="d6ca3-554">**Experiencia de usuario sin problemas** para administrar todas las oportunidades de venta conjunta y clientes potenciales cualificados para ventas en un solo lugar.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-554">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="d6ca3-555">Además, recientemente hemos agregado nuevas características al Centro de partners para ayudarle en el traslado:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-555">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="d6ca3-556">Operaciones masivas para las oportunidades de venta conjunta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-556">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="d6ca3-557">[Característica de migración de ofertas](../psc-to-pc.md) (consulte la sección **Migración de contratos de PSC**).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-557">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="d6ca3-558">Con la experiencia de venta conjunta en el Centro de partners, los equipos de ventas tendrán más tiempo para centrarse en fomentar la captación de clientes potenciales y oportunidades, cerrar acuerdos y crear relaciones duraderas con los clientes.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-558">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="d6ca3-559">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-559">Next steps</span></span>

<span data-ttu-id="d6ca3-560">Use la [guía de transición](../psc-to-pc.md) del Centro de partners para conocer por los pasos necesarios para migrar sus ofertas de PSC al Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-560">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="d6ca3-561">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="d6ca3-561">Questions?</span></span>

<span data-ttu-id="d6ca3-562">Si tiene más preguntas, póngase en contacto con [Soporte técnico](https://partner.microsoft.com/support/?stage=1).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-562">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="d6ca3-563">Nuevos productos y ofertas de Microsoft Dynamics 365 disponibles el 1 de abril de 2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-563">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-564">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-564">Categories</span></span>

- <span data-ttu-id="d6ca3-565">Fecha: 04/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-565">Date: 2021-03-04</span></span>
- <span data-ttu-id="d6ca3-566">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="d6ca3-566">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d6ca3-567">Resumen</span><span class="sxs-lookup"><span data-stu-id="d6ca3-567">Summary</span></span>

<span data-ttu-id="d6ca3-568">El 1 de abril de 2021, Microsoft lanzará varios productos y ofertas nuevos para el programa Proveedor de soluciones en la nube (CSP).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-568">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-569">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-569">Impacted audience</span></span>

<span data-ttu-id="d6ca3-570">Todos los partners que operan a través del programa Proveedor de soluciones en la nube (CSP)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-570">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-571">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-571">Details</span></span>

<span data-ttu-id="d6ca3-572">El 1 de abril de 2021, Microsoft lanzará los siguientes nuevos productos y ofertas:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-572">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="d6ca3-573">Power BI Premium por usuario</span><span class="sxs-lookup"><span data-stu-id="d6ca3-573">Power BI Premium Per User</span></span>
- <span data-ttu-id="d6ca3-574">Expansión geográfica y por segmento de USL de Customer Voice y Marketing</span><span class="sxs-lookup"><span data-stu-id="d6ca3-574">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="d6ca3-575">**Power BI Premium por usuario**</span><span class="sxs-lookup"><span data-stu-id="d6ca3-575">**Power BI Premium Per User**</span></span>

<span data-ttu-id="d6ca3-576">Microsoft presentará las primeras ofertas de Power BI Premium por usuario.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-576">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="d6ca3-577">Actualmente, Power BI Premium se vende solo en una construcción de capacidad.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-577">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="d6ca3-578">Power BI Premium por usuario proporciona acceso a las funcionalidades empresariales de business intelligence (BI) y análisis.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-578">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="d6ca3-579">Su oferta de licencias flexible e individual por puesto está dirigida a pequeñas y medianas empresas.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-579">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="d6ca3-580">Revise los [detalles de la versión de Power BI](/power-platform-release-plan/2020wave2/power-bi/planned-features) para obtener más información sobre esta oferta.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-580">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="d6ca3-581">**Detalles de la oferta**</span><span class="sxs-lookup"><span data-stu-id="d6ca3-581">**Offer details**</span></span>

<span data-ttu-id="d6ca3-582">Tenga en cuenta que el nombre de la oferta difiere ligeramente de la vista previa de la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-582">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="d6ca3-583">Nombre de la oferta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-583">Offer name</span></span> | <span data-ttu-id="d6ca3-584">Id. de oferta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-584">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="d6ca3-585">Power BI Premium por usuario</span><span class="sxs-lookup"><span data-stu-id="d6ca3-585">Power BI Premium Per User</span></span> | <span data-ttu-id="d6ca3-586">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="d6ca3-586">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="d6ca3-587">Power BI Premium por usuario para profesores</span><span class="sxs-lookup"><span data-stu-id="d6ca3-587">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="d6ca3-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="d6ca3-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="d6ca3-589">Power BI Premium por usuario para estudiantes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-589">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="d6ca3-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="d6ca3-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="d6ca3-591">Power BI Premium por usuario (precios para personal de ONG)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-591">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="d6ca3-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="d6ca3-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="d6ca3-593">Complemento de Power BI Premium por usuario</span><span class="sxs-lookup"><span data-stu-id="d6ca3-593">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="d6ca3-594">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="d6ca3-594">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="d6ca3-595">Complemento de Power BI Premium por usuario para profesores</span><span class="sxs-lookup"><span data-stu-id="d6ca3-595">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="d6ca3-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="d6ca3-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="d6ca3-597">Complemento de Power BI Premium por usuario para estudiantes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-597">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="d6ca3-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="d6ca3-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="d6ca3-599">Complemento Power BI Premium por usuario (precios para personal de ONG)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-599">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="d6ca3-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="d6ca3-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="d6ca3-601">**Expansión geográfica y por segmento de USL de Customer Voice y Marketing**</span><span class="sxs-lookup"><span data-stu-id="d6ca3-601">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="d6ca3-602">Como seguimiento del lanzamiento de diciembre de 2020, se han cambiado las ofertas de USL de Dynamics 365 Customer Voice y Marketing para agregar nuevos países y más SKU de educación y ONG.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-602">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="d6ca3-603">Nombre de la oferta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-603">Offer name</span></span> | <span data-ttu-id="d6ca3-604">Id. de oferta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-604">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="d6ca3-605">USL de Dynamics 365 Customer Voice (precios para personal de ONG)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-605">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="d6ca3-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="d6ca3-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="d6ca3-607">USL de Dynamics 365 Customer Voice para profesores</span><span class="sxs-lookup"><span data-stu-id="d6ca3-607">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="d6ca3-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="d6ca3-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="d6ca3-609">Para obtener más información sobre estas ofertas, visite las páginas siguientes:</span><span class="sxs-lookup"><span data-stu-id="d6ca3-609">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="d6ca3-610">Página principal de Dynamics 365 Customer Voice</span><span class="sxs-lookup"><span data-stu-id="d6ca3-610">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="d6ca3-611">Página principal de Dynamics 365 Marketing</span><span class="sxs-lookup"><span data-stu-id="d6ca3-611">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="d6ca3-612">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-612">Next steps</span></span>

<span data-ttu-id="d6ca3-613">Revise los recursos sobre este tema y comparta esta información con las partes interesadas adecuadas de su organización.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-613">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="d6ca3-614">¿Tiene alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="d6ca3-614">Questions?</span></span>

<span data-ttu-id="d6ca3-615">Si tiene preguntas sobre estas ofertas, consulte a las comunidades de Yammer correspondientes.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-615">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> <span data-ttu-id="d6ca3-616">Impresión universal de Microsoft ahora está disponible en algunos conjuntos de aplicaciones</span><span class="sxs-lookup"><span data-stu-id="d6ca3-616">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="d6ca3-617">Categorías</span><span class="sxs-lookup"><span data-stu-id="d6ca3-617">Categories</span></span>

- <span data-ttu-id="d6ca3-618">Fecha: 31/03/2021</span><span class="sxs-lookup"><span data-stu-id="d6ca3-618">Date: 2021-03-33</span></span>
- <span data-ttu-id="d6ca3-619">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="d6ca3-619">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="d6ca3-620">Resumen</span><span class="sxs-lookup"><span data-stu-id="d6ca3-620">Summary</span></span>

<span data-ttu-id="d6ca3-621">Impresión universal de Microsoft estará disponible para operaciones dentro de ciertos conjuntos de aplicaciones de Microsoft 365 y como complemento independiente a partir del 1 de marzo de 2021.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-621">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="d6ca3-622">Audiencia afectada</span><span class="sxs-lookup"><span data-stu-id="d6ca3-622">Impacted audience</span></span>

<span data-ttu-id="d6ca3-623">Todos los partners que operan a través del programa Proveedor de soluciones en la nube (CSP)</span><span class="sxs-lookup"><span data-stu-id="d6ca3-623">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="d6ca3-624">Detalles</span><span class="sxs-lookup"><span data-stu-id="d6ca3-624">Details</span></span>

<span data-ttu-id="d6ca3-625">[Impresión universal](https://aka.ms/universalprint) es un servicio de impresión de Microsoft 365 que elimina la necesidad de servidores de impresión locales, y permite que los dispositivos Windows impriman en impresoras registradas en Azure.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-625">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="d6ca3-626">Estará disponible para operar desde el 1 de marzo de 2021.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-626">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="d6ca3-627">Los trabajadores se benefician de una impresión sin controladores, una detección de impresoras basada en ubicaciones y una experiencia de impresión intuitiva sin curva de aprendizaje.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-627">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="d6ca3-628">Los dispositivos que están unidos a Azure Active Directory (Azure AD) usan credenciales de Azure AD existentes para imprimir de forma segura.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-628">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="d6ca3-629">Los administradores administran la impresión mediante Azure Portal y pueden conectar fácilmente las impresoras con la compatibilidad nativa con Impresión universal.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-629">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="d6ca3-630">Impresión universal se puede implementar con impresoras no compatibles mediante el software del conector de Impresión universal.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-630">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="d6ca3-631">Impresión universal se incluirá en un comienzo en Windows E3, A3, E5 y A5, y Microsoft 365 BP, F3, E3, A3, E5 y A5.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-631">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="d6ca3-632">**Detalles de la oferta**</span><span class="sxs-lookup"><span data-stu-id="d6ca3-632">**Offer details**</span></span>

<span data-ttu-id="d6ca3-633">Tenga en cuenta que el nombre de la oferta difiere ligeramente de la vista previa de la lista de precios.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-633">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="d6ca3-634">Nombre de la oferta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-634">Offer name</span></span> | <span data-ttu-id="d6ca3-635">Id. de oferta</span><span class="sxs-lookup"><span data-stu-id="d6ca3-635">Offer ID</span></span> | <span data-ttu-id="d6ca3-636">Id. de material</span><span class="sxs-lookup"><span data-stu-id="d6ca3-636">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="d6ca3-637">Complemento de volumen de Impresión universal (500 trabajos): Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d6ca3-637">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="d6ca3-638">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="d6ca3-638">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="d6ca3-639">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="d6ca3-639">9BI-00004</span></span>   |
| <span data-ttu-id="d6ca3-640">Complemento de volumen de Impresión universal (500 trabajos) para profesores: Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d6ca3-640">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="d6ca3-641">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="d6ca3-641">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="d6ca3-642">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="d6ca3-642">9BK-00004</span></span>   |
| <span data-ttu-id="d6ca3-643">Complemento de volumen de Impresión universal (500 trabajos): Windows</span><span class="sxs-lookup"><span data-stu-id="d6ca3-643">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="d6ca3-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="d6ca3-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="d6ca3-645">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="d6ca3-645">9BI-00002</span></span>   |
| <span data-ttu-id="d6ca3-646">Complemento de volumen de Impresión universal (500 trabajos) para profesores: Windows</span><span class="sxs-lookup"><span data-stu-id="d6ca3-646">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="d6ca3-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="d6ca3-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="d6ca3-648">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="d6ca3-648">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="d6ca3-649">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d6ca3-649">Next steps</span></span>

<span data-ttu-id="d6ca3-650">Familiarícese con la lista de precios y la [Introducción a Impresión universal](/universal-print/fundamentals/universal-print-whatis).</span><span class="sxs-lookup"><span data-stu-id="d6ca3-650">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="d6ca3-651">Comparta esta información con todos los contactos de su organización a quienes corresponda.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-651">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="d6ca3-652">¿Alguna pregunta?</span><span class="sxs-lookup"><span data-stu-id="d6ca3-652">Questions?</span></span>

<span data-ttu-id="d6ca3-653">Si tiene preguntas sobre estas ofertas, consulte a las comunidades de Yammer correspondientes.</span><span class="sxs-lookup"><span data-stu-id="d6ca3-653">For any questions about these offers, check your relevant Yammer communities.</span></span>
