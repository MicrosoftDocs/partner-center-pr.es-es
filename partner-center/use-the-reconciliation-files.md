---
title: Usar los archivos de conciliación
ms.topic: article
ms.date: 06/08/2020
description: Obtenga información acerca de los archivos de conciliación en el centro de Partners y cómo interpretar las vistas detalladas del artículo de línea de los cargos de un ciclo de facturación determinado.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 05939dc5edaddeb2f74b3b75017e2062dff25e31
ms.sourcegitcommit: e243bc0ef337f5d92c5b208ce6bb9dc5f179b185
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/31/2020
ms.locfileid: "87468336"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="47bf4-103">Obtenga información sobre cómo leer los elementos de línea de los archivos de conciliación del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="47bf4-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="47bf4-104">Se aplica a:</span><span class="sxs-lookup"><span data-stu-id="47bf4-104">Applies to:</span></span>

- <span data-ttu-id="47bf4-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="47bf4-105">Partner Center</span></span>
- <span data-ttu-id="47bf4-106">Centro de partners para Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="47bf4-106">Partner Center for Microsoft Cloud for US Government</span></span>

<span data-ttu-id="47bf4-107">Puede descargar los archivos de conciliación del centro de partners para obtener una vista detallada de los elementos de línea de cada cargo en un ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="47bf4-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="47bf4-108">Los detalles de los elementos de línea incluyen los cargos de las suscripciones de cada cliente y eventos detallados (por ejemplo, una adición de licencias a mediados de la suscripción).</span><span class="sxs-lookup"><span data-stu-id="47bf4-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="47bf4-109">Roles adecuados:</span><span class="sxs-lookup"><span data-stu-id="47bf4-109">Appropriate roles:</span></span>

- <span data-ttu-id="47bf4-110">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="47bf4-110">Billing admin</span></span>
- <span data-ttu-id="47bf4-111">Administrador global</span><span class="sxs-lookup"><span data-stu-id="47bf4-111">Global admin</span></span>

<span data-ttu-id="47bf4-112">Para obtener información sobre cómo leer la **factura**, consulte [leer su](read-your-bill.md)factura.</span><span class="sxs-lookup"><span data-stu-id="47bf4-112">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="47bf4-113">Descripción de los campos de archivo de conciliación</span><span class="sxs-lookup"><span data-stu-id="47bf4-113">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="47bf4-114">Campos de archivos de conciliación basados en licencias</span><span class="sxs-lookup"><span data-stu-id="47bf4-114">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="47bf4-115">Campos de archivos de conciliación basados en el uso</span><span class="sxs-lookup"><span data-stu-id="47bf4-115">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="47bf4-116">Campos de archivo de conciliación de uso con clasificación diaria</span><span class="sxs-lookup"><span data-stu-id="47bf4-116">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="47bf4-117">Descripción de los tipos de carga en los archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="47bf4-117">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="47bf4-118">Para comprender los tipos de cargos de los archivos de conciliación (la columna **ChargeType** ), vea [reconciliar tipos de cargos de archivo](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="47bf4-118">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="47bf4-119">Corregir problemas de formato</span><span class="sxs-lookup"><span data-stu-id="47bf4-119">Fix formatting issues</span></span>

<span data-ttu-id="47bf4-120">En ocasiones, un archivo de conciliación puede contener problemas de formato.</span><span class="sxs-lookup"><span data-stu-id="47bf4-120">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="47bf4-121">Por ejemplo, este problema podría producirse si no se utiliza la configuración regional en-US.</span><span class="sxs-lookup"><span data-stu-id="47bf4-121">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="47bf4-122">Siga estos pasos para corregir los problemas de formato en los archivos de conciliación:</span><span class="sxs-lookup"><span data-stu-id="47bf4-122">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="47bf4-123">Abra el archivo de conciliación (en formato. csv) en Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="47bf4-123">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="47bf4-124">Seleccione la primera columna del archivo.</span><span class="sxs-lookup"><span data-stu-id="47bf4-124">Select the first column in the file.</span></span>
3. <span data-ttu-id="47bf4-125">Abra el **Asistente para convertir texto en columnas**.</span><span class="sxs-lookup"><span data-stu-id="47bf4-125">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="47bf4-126">En la cinta de opciones, seleccione **datos**y, a continuación, seleccione **texto en columnas**.</span><span class="sxs-lookup"><span data-stu-id="47bf4-126">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="47bf4-127">En el asistente, seleccione **tipo de archivo delimitado**.</span><span class="sxs-lookup"><span data-stu-id="47bf4-127">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="47bf4-128">Después, seleccione **Siguiente**.</span><span class="sxs-lookup"><span data-stu-id="47bf4-128">Then, select **Next**.</span></span>
5. <span data-ttu-id="47bf4-129">En el campo **delimitadores** , seleccione **coma**.</span><span class="sxs-lookup"><span data-stu-id="47bf4-129">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="47bf4-130">(Si la **pestaña** ya está seleccionada, puede dejar esta opción seleccionada). A continuación, seleccione **siguiente**.</span><span class="sxs-lookup"><span data-stu-id="47bf4-130">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="47bf4-131">En el campo **formato de datos de columna** , seleccione **Fecha: MDA**.</span><span class="sxs-lookup"><span data-stu-id="47bf4-131">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="47bf4-132">Después, seleccione **Siguiente**.</span><span class="sxs-lookup"><span data-stu-id="47bf4-132">Then, select **Next**.</span></span>
7. <span data-ttu-id="47bf4-133">En el campo **formato de datos de columna** , seleccione **texto** para todas las columnas de importe.</span><span class="sxs-lookup"><span data-stu-id="47bf4-133">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="47bf4-134">Después, seleccione **Finalizar**.</span><span class="sxs-lookup"><span data-stu-id="47bf4-134">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="47bf4-135">Descargar archivos de conciliación mediante programación</span><span class="sxs-lookup"><span data-stu-id="47bf4-135">Download reconciliation files programmatically</span></span>

<span data-ttu-id="47bf4-136">Los archivos de conciliación pueden ser muy grandes y a veces son difíciles de descargar.</span><span class="sxs-lookup"><span data-stu-id="47bf4-136">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="47bf4-137">Para descargar los archivos de conciliación mediante programación, vea [obtener artículos de línea de factura](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="47bf4-137">To download reconciliation files programmatically, see [Get invoice line items](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="47bf4-138">Impuestos de mapa o IVA</span><span class="sxs-lookup"><span data-stu-id="47bf4-138">Map taxes or VAT</span></span>

<span data-ttu-id="47bf4-139">Para asignar impuestos o impuestos sobre el valor añadido (IVA) a la factura:</span><span class="sxs-lookup"><span data-stu-id="47bf4-139">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="47bf4-140">Sume la columna **Tax** del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="47bf4-140">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="47bf4-141">Sume la columna **TaxAmount** del archivo basado en el uso.</span><span class="sxs-lookup"><span data-stu-id="47bf4-141">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="47bf4-142">Elemento de conciliación de elementos por asociado</span><span class="sxs-lookup"><span data-stu-id="47bf4-142">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="47bf4-143">Los asociados en el **modelo indirecto** pueden utilizar estos campos adicionales en los archivos de conciliación basados en la licencia y en el uso para que los revendan los archivos.</span><span class="sxs-lookup"><span data-stu-id="47bf4-143">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="47bf4-144">Identificador de MPN</span><span class="sxs-lookup"><span data-stu-id="47bf4-144">MPN ID</span></span> | <span data-ttu-id="47bf4-145">Descripción</span><span class="sxs-lookup"><span data-stu-id="47bf4-145">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="47bf4-146">Identificador de MPN</span><span class="sxs-lookup"><span data-stu-id="47bf4-146">MPN ID</span></span> | <span data-ttu-id="47bf4-147">Identificador Microsoft Partner Network (MPN) del asociado del proveedor de soluciones en la nube (CSP) (directo o indirecto).</span><span class="sxs-lookup"><span data-stu-id="47bf4-147">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="47bf4-148">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="47bf4-148">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="47bf4-149">[Identificador de MPN del distribuidor de registro de la suscripción](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="47bf4-149">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="47bf4-150">Este campo corresponde al ID. de distribuidor que se muestra para la suscripción específica del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="47bf4-150">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="47bf4-151">Solo aparece en los archivos de conciliación de partners en el modelo indirecto.</span><span class="sxs-lookup"><span data-stu-id="47bf4-151">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="47bf4-152">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="47bf4-152">Reseller MPN ID</span></span>

<span data-ttu-id="47bf4-153">Si un asociado de CSP vendió la suscripción directamente al cliente, su **identificador de MPN** aparece dos veces, como el **identificador de MPN** y el ID. de **MPN del reseller**.</span><span class="sxs-lookup"><span data-stu-id="47bf4-153">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="47bf4-154">Si un asociado de CSP tiene un revendedor sin **identificador de MPN**, este valor se establece en el **identificador de MPN** del asociado en su lugar.</span><span class="sxs-lookup"><span data-stu-id="47bf4-154">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="47bf4-155">Si el asociado de CSP quita un ID. de **revendedor de MPN**, este valor se establecerá en *-1*.</span><span class="sxs-lookup"><span data-stu-id="47bf4-155">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="47bf4-156">Para ver o actualizar el **ID. de revendedor MPN**:</span><span class="sxs-lookup"><span data-stu-id="47bf4-156">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="47bf4-157">Inicie sesión en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="47bf4-157">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="47bf4-158">En el menú del Centro de partners, selecciona **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="47bf4-158">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="47bf4-159">Elija el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="47bf4-159">Choose the customer from the list.</span></span>
4. <span data-ttu-id="47bf4-160">En el menú del cliente, seleccione **suscripciones**.</span><span class="sxs-lookup"><span data-stu-id="47bf4-160">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="47bf4-161">Elija la suscripción de la lista.</span><span class="sxs-lookup"><span data-stu-id="47bf4-161">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="47bf4-162">Selecciona **Actualizar** para cambiar el valor de **Revendedor (id. de MPN)**.</span><span class="sxs-lookup"><span data-stu-id="47bf4-162">Select **update** to change the **Reseller (MPN ID)**.</span></span>
