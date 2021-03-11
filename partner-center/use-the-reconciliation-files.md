---
title: Usar los archivos de conciliación
ms.topic: article
ms.date: 03/10/2021
description: Obtenga información acerca de los archivos de conciliación en el centro de Partners y cómo interpretar las vistas detalladas del artículo de línea de los cargos de un ciclo de facturación determinado.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e6b9e466402d71c988729052bd72ba2346a9d977
ms.sourcegitcommit: 868f90c54f26a037eee29749c207a7316bb4b475
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/11/2021
ms.locfileid: "103022781"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="d7eb9-103">Obtenga información sobre cómo leer los elementos de línea de los archivos de conciliación del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="d7eb9-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="d7eb9-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="d7eb9-104">**Appropriate roles**</span></span>

- <span data-ttu-id="d7eb9-105">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="d7eb9-105">Billing admin</span></span>
- <span data-ttu-id="d7eb9-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="d7eb9-106">Global admin</span></span>

<span data-ttu-id="d7eb9-107">Puede descargar los archivos de conciliación del centro de partners para obtener una vista detallada de los elementos de línea de cada cargo en un ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="d7eb9-108">Los detalles de los elementos de línea incluyen los cargos de las suscripciones de cada cliente y eventos detallados (por ejemplo, una adición de licencias a mediados de la suscripción).</span><span class="sxs-lookup"><span data-stu-id="d7eb9-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="d7eb9-109">Para obtener información sobre cómo leer la **factura**, consulte [leer su](read-your-bill.md)factura.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="d7eb9-110">Descripción de los campos de archivo de conciliación</span><span class="sxs-lookup"><span data-stu-id="d7eb9-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="d7eb9-111">Campos de archivos de conciliación basados en licencias</span><span class="sxs-lookup"><span data-stu-id="d7eb9-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="d7eb9-112">Campos de archivos de conciliación basados en el uso</span><span class="sxs-lookup"><span data-stu-id="d7eb9-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="d7eb9-113">Campos de archivos de conciliación de uso con clasificación diaria</span><span class="sxs-lookup"><span data-stu-id="d7eb9-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="d7eb9-114">Campos de archivo de conciliación de CSP de compra única</span><span class="sxs-lookup"><span data-stu-id="d7eb9-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="d7eb9-115">Descripción de los tipos de carga en los archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="d7eb9-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="d7eb9-116">Para comprender los tipos de cargos de los archivos de conciliación (la columna **ChargeType** ), vea [reconciliar tipos de cargos de archivo](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="d7eb9-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="d7eb9-117">Corregir problemas de formato</span><span class="sxs-lookup"><span data-stu-id="d7eb9-117">Fix formatting issues</span></span>

<span data-ttu-id="d7eb9-118">En ocasiones, un archivo de conciliación puede contener problemas de formato.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="d7eb9-119">Por ejemplo, este problema podría producirse si no se utiliza la configuración regional en-US.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="d7eb9-120">Siga estos pasos para corregir los problemas de formato en los archivos de conciliación:</span><span class="sxs-lookup"><span data-stu-id="d7eb9-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="d7eb9-121">Abra el archivo de conciliación (en formato. csv) en Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="d7eb9-122">Seleccione la primera columna del archivo.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="d7eb9-123">Abra el **Asistente para convertir texto en columnas**.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="d7eb9-124">En la cinta de opciones, seleccione **datos** y, a continuación, seleccione **texto en columnas**.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="d7eb9-125">En el asistente, seleccione **tipo de archivo delimitado**.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="d7eb9-126">Después, seleccione **Siguiente**.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="d7eb9-127">En el campo **delimitadores** , seleccione **coma**.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="d7eb9-128">(Si la **pestaña** ya está seleccionada, puede dejar esta opción seleccionada). A continuación, seleccione **siguiente**.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="d7eb9-129">En el campo **formato de datos de columna** , seleccione **Fecha: MDA**.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="d7eb9-130">Después, seleccione **Siguiente**.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="d7eb9-131">En el campo **formato de datos de columna** , seleccione **texto** para todas las columnas de importe.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="d7eb9-132">A continuación, seleccione **Finish** (Finalizar).</span><span class="sxs-lookup"><span data-stu-id="d7eb9-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="d7eb9-133">Descargar archivos de conciliación mediante programación</span><span class="sxs-lookup"><span data-stu-id="d7eb9-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="d7eb9-134">Los archivos de conciliación pueden ser muy grandes y a veces son difíciles de descargar.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="d7eb9-135">Para descargar los archivos de conciliación mediante programación, vea [obtener artículos de línea de factura](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="d7eb9-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="d7eb9-136">Impuestos de mapa o IVA</span><span class="sxs-lookup"><span data-stu-id="d7eb9-136">Map taxes or VAT</span></span>

<span data-ttu-id="d7eb9-137">Para asignar impuestos o impuestos sobre el valor añadido (IVA) a la factura:</span><span class="sxs-lookup"><span data-stu-id="d7eb9-137">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="d7eb9-138">Sume la columna **Tax** del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-138">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="d7eb9-139">Sume la columna **TaxAmount** del archivo basado en el uso.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-139">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="d7eb9-140">Elemento de conciliación de elementos por asociado</span><span class="sxs-lookup"><span data-stu-id="d7eb9-140">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="d7eb9-141">Los asociados en el **modelo indirecto** pueden utilizar estos campos adicionales en los archivos de conciliación basados en la licencia y en el uso para que los revendan los archivos.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-141">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="d7eb9-142">Identificador de MPN</span><span class="sxs-lookup"><span data-stu-id="d7eb9-142">MPN ID</span></span> | <span data-ttu-id="d7eb9-143">Descripción</span><span class="sxs-lookup"><span data-stu-id="d7eb9-143">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="d7eb9-144">Identificador de MPN</span><span class="sxs-lookup"><span data-stu-id="d7eb9-144">MPN ID</span></span> | <span data-ttu-id="d7eb9-145">Identificador Microsoft Partner Network (MPN) del asociado del proveedor de soluciones en la nube (CSP) (directo o indirecto).</span><span class="sxs-lookup"><span data-stu-id="d7eb9-145">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="d7eb9-146">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="d7eb9-146">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="d7eb9-147">[Identificador de MPN del distribuidor de registro de la suscripción](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="d7eb9-147">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="d7eb9-148">Este campo corresponde al ID. de distribuidor que se muestra para la suscripción específica del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-148">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="d7eb9-149">Solo aparece en los archivos de conciliación de partners en el modelo indirecto.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-149">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="d7eb9-150">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="d7eb9-150">Reseller MPN ID</span></span>

<span data-ttu-id="d7eb9-151">Si un asociado de CSP vendió la suscripción directamente al cliente, su **identificador de MPN** aparece dos veces, como el **identificador de MPN** y el ID. de **MPN del reseller**.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-151">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="d7eb9-152">Si un asociado de CSP tiene un revendedor sin **identificador de MPN**, este valor se establece en el **identificador de MPN** del asociado en su lugar.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-152">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="d7eb9-153">Si el asociado de CSP quita un ID. de **revendedor de MPN**, este valor se establecerá en *-1*.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-153">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="d7eb9-154">Para ver o actualizar el **ID. de revendedor MPN**:</span><span class="sxs-lookup"><span data-stu-id="d7eb9-154">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="d7eb9-155">Inicie sesión en el Centro de datos.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-155">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="d7eb9-156">En el menú del Centro de partners, selecciona **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-156">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="d7eb9-157">Elija el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-157">Choose the customer from the list.</span></span>
4. <span data-ttu-id="d7eb9-158">En el menú del cliente, seleccione **suscripciones**.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-158">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="d7eb9-159">Elija la suscripción de la lista.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-159">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="d7eb9-160">Selecciona **Actualizar** para cambiar el valor de **Revendedor (id. de MPN)**.</span><span class="sxs-lookup"><span data-stu-id="d7eb9-160">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d7eb9-161">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d7eb9-161">Next steps</span></span>

- [<span data-ttu-id="d7eb9-162">Cómo leer el archivo de conciliación & de la factura</span><span class="sxs-lookup"><span data-stu-id="d7eb9-162">How to read your bill & recon file</span></span>](read-your-bill.md) 