---
title: Usar los archivos de conciliación
ms.topic: article
ms.date: 03/26/2021
description: Obtenga información acerca de los archivos de conciliación en el centro de Partners y cómo interpretar las vistas detalladas del artículo de línea de los cargos de un ciclo de facturación determinado.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4a6a1455304f12e364d71e666cbd548821f8be55
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633903"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="36c1d-103">Obtenga información sobre cómo leer los elementos de línea de los archivos de conciliación del centro de Partners</span><span class="sxs-lookup"><span data-stu-id="36c1d-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="36c1d-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="36c1d-104">**Appropriate roles**</span></span>

- <span data-ttu-id="36c1d-105">Administrador de facturación</span><span class="sxs-lookup"><span data-stu-id="36c1d-105">Billing admin</span></span>
- <span data-ttu-id="36c1d-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="36c1d-106">Global admin</span></span>

<span data-ttu-id="36c1d-107">Puede descargar los archivos de conciliación del centro de partners para obtener una vista detallada de los elementos de línea de cada cargo en un ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="36c1d-107">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="36c1d-108">Los detalles de los elementos de línea incluyen los cargos de las suscripciones de cada cliente y eventos detallados (por ejemplo, una adición de licencias a mediados de la suscripción).</span><span class="sxs-lookup"><span data-stu-id="36c1d-108">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="36c1d-109">Para obtener información sobre cómo leer la **factura**, consulte [leer su](read-your-bill.md)factura.</span><span class="sxs-lookup"><span data-stu-id="36c1d-109">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="36c1d-110">Descripción de los campos de archivo de conciliación</span><span class="sxs-lookup"><span data-stu-id="36c1d-110">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="36c1d-111">Campos de archivos de conciliación basados en licencias</span><span class="sxs-lookup"><span data-stu-id="36c1d-111">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="36c1d-112">Campos de archivos de conciliación basados en el uso</span><span class="sxs-lookup"><span data-stu-id="36c1d-112">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="36c1d-113">Campos de archivos de conciliación de uso con clasificación diaria</span><span class="sxs-lookup"><span data-stu-id="36c1d-113">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="36c1d-114">Campos de archivo de conciliación de CSP de compra única</span><span class="sxs-lookup"><span data-stu-id="36c1d-114">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="36c1d-115">Descripción de los tipos de carga en los archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="36c1d-115">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="36c1d-116">Para comprender los tipos de cargos de los archivos de conciliación (la columna **ChargeType** ), vea [reconciliar tipos de cargos de archivo](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="36c1d-116">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="36c1d-117">Corregir problemas de formato</span><span class="sxs-lookup"><span data-stu-id="36c1d-117">Fix formatting issues</span></span>

<span data-ttu-id="36c1d-118">En ocasiones, un archivo de conciliación puede contener problemas de formato.</span><span class="sxs-lookup"><span data-stu-id="36c1d-118">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="36c1d-119">Por ejemplo, este problema podría producirse si no se utiliza la configuración regional en-US.</span><span class="sxs-lookup"><span data-stu-id="36c1d-119">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="36c1d-120">Siga estos pasos para corregir los problemas de formato en los archivos de conciliación:</span><span class="sxs-lookup"><span data-stu-id="36c1d-120">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="36c1d-121">Abra el archivo de conciliación (en formato. csv) en Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="36c1d-121">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="36c1d-122">Seleccione la primera columna del archivo.</span><span class="sxs-lookup"><span data-stu-id="36c1d-122">Select the first column in the file.</span></span>
3. <span data-ttu-id="36c1d-123">Abra el **Asistente para convertir texto en columnas**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-123">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="36c1d-124">En la cinta de opciones, seleccione **datos** y, a continuación, seleccione **texto en columnas**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-124">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="36c1d-125">En el asistente, seleccione **tipo de archivo delimitado**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-125">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="36c1d-126">Después, seleccione **Siguiente**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-126">Then, select **Next**.</span></span>
5. <span data-ttu-id="36c1d-127">En el campo **delimitadores** , seleccione **coma**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-127">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="36c1d-128">(Si la **pestaña** ya está seleccionada, puede dejar esta opción seleccionada). A continuación, seleccione **siguiente**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-128">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="36c1d-129">En el campo **formato de datos de columna** , seleccione **Fecha: MDA**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-129">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="36c1d-130">Después, seleccione **Siguiente**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-130">Then, select **Next**.</span></span>
7. <span data-ttu-id="36c1d-131">En el campo **formato de datos de columna** , seleccione **texto** para todas las columnas de importe.</span><span class="sxs-lookup"><span data-stu-id="36c1d-131">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="36c1d-132">A continuación, seleccione **Finish** (Finalizar).</span><span class="sxs-lookup"><span data-stu-id="36c1d-132">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="36c1d-133">Descargar archivos de conciliación mediante programación</span><span class="sxs-lookup"><span data-stu-id="36c1d-133">Download reconciliation files programmatically</span></span>

<span data-ttu-id="36c1d-134">Los archivos de conciliación pueden ser muy grandes y a veces son difíciles de descargar.</span><span class="sxs-lookup"><span data-stu-id="36c1d-134">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="36c1d-135">Para descargar los archivos de conciliación mediante programación, vea [obtener artículos de línea de factura](/partner-center/develop/get-invoiceline-items).</span><span class="sxs-lookup"><span data-stu-id="36c1d-135">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="36c1d-136">Si el archivo supera el límite de filas de Excel</span><span class="sxs-lookup"><span data-stu-id="36c1d-136">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="36c1d-137">Si es capaz de descargar un archivo de conciliación pero no lo abre en Microsoft Excel, probablemente significa que el archivo contiene más filas de las que Excel permitirá.</span><span class="sxs-lookup"><span data-stu-id="36c1d-137">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="36c1d-138">Si esto ocurre, puede usar cualquiera de los procedimientos siguientes para abrir el archivo.</span><span class="sxs-lookup"><span data-stu-id="36c1d-138">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="36c1d-139">Abra un archivo de conciliación en Power BI</span><span class="sxs-lookup"><span data-stu-id="36c1d-139">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="36c1d-140">Descargue el archivo de conciliación como lo haría normalmente.</span><span class="sxs-lookup"><span data-stu-id="36c1d-140">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="36c1d-141">Descargue, instale y abra una instancia de Power BI.</span><span class="sxs-lookup"><span data-stu-id="36c1d-141">Download, install, and open an instance of Power BI.</span></span>
3. <span data-ttu-id="36c1d-142">En la pestaña **Inicio** de Power BI, seleccione **obtener datos**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-142">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="36c1d-143">En la lista de **orígenes de datos comunes**, seleccione **Text/CSV**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-143">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="36c1d-144">Cuando se le solicite, abra el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="36c1d-144">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="36c1d-145">Apertura de un archivo de conciliación en una tabla dinámica de Excel</span><span class="sxs-lookup"><span data-stu-id="36c1d-145">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="36c1d-146">Descargue el archivo de conciliación como lo haría normalmente.</span><span class="sxs-lookup"><span data-stu-id="36c1d-146">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="36c1d-147">Abra un archivo nuevo en Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="36c1d-147">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="36c1d-148">En la pestaña **datos** , seleccione **obtener datos**, seleccione **desde archivo** y, a continuación, seleccione **texto/CSV**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-148">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="36c1d-149">Cuando se le solicite, abra el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="36c1d-149">When prompted, open your recon file.</span></span> <span data-ttu-id="36c1d-150">Los datos aparecerán.</span><span class="sxs-lookup"><span data-stu-id="36c1d-150">Your data will appear.</span></span>
5. <span data-ttu-id="36c1d-151">En el menú desplegable **cargar** , seleccione **cargar en** y, a continuación, haga clic en **Aceptar**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-151">In the **Load** dropdown menu, select **Load to**, and then **OK**.</span></span>
6. <span data-ttu-id="36c1d-152">En el cuadro de diálogo **importar datos** , seleccione **Informe de tabla dinámica** para abrir el archivo.</span><span class="sxs-lookup"><span data-stu-id="36c1d-152">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="36c1d-153">Impuestos de mapa o IVA</span><span class="sxs-lookup"><span data-stu-id="36c1d-153">Map taxes or VAT</span></span>

<span data-ttu-id="36c1d-154">Para asignar impuestos o impuestos sobre el valor añadido (IVA) a la factura:</span><span class="sxs-lookup"><span data-stu-id="36c1d-154">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="36c1d-155">Sume la columna **Tax** del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="36c1d-155">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="36c1d-156">Sume la columna **TaxAmount** del archivo basado en el uso.</span><span class="sxs-lookup"><span data-stu-id="36c1d-156">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="36c1d-157">Elemento de conciliación de elementos por asociado</span><span class="sxs-lookup"><span data-stu-id="36c1d-157">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="36c1d-158">Los asociados en el **modelo indirecto** pueden utilizar estos campos adicionales en los archivos de conciliación basados en la licencia y en el uso para que los revendan los archivos.</span><span class="sxs-lookup"><span data-stu-id="36c1d-158">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="36c1d-159">Identificador de MPN</span><span class="sxs-lookup"><span data-stu-id="36c1d-159">MPN ID</span></span> | <span data-ttu-id="36c1d-160">Descripción</span><span class="sxs-lookup"><span data-stu-id="36c1d-160">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="36c1d-161">Identificador de MPN</span><span class="sxs-lookup"><span data-stu-id="36c1d-161">MPN ID</span></span> | <span data-ttu-id="36c1d-162">Identificador Microsoft Partner Network (MPN) del asociado del proveedor de soluciones en la nube (CSP) (directo o indirecto).</span><span class="sxs-lookup"><span data-stu-id="36c1d-162">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="36c1d-163">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="36c1d-163">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="36c1d-164">[Identificador de MPN del distribuidor de registro de la suscripción](#reseller-mpn-id).</span><span class="sxs-lookup"><span data-stu-id="36c1d-164">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="36c1d-165">Este campo corresponde al ID. de distribuidor que se muestra para la suscripción específica del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="36c1d-165">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="36c1d-166">Solo aparece en los archivos de conciliación de partners en el modelo indirecto.</span><span class="sxs-lookup"><span data-stu-id="36c1d-166">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="36c1d-167">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="36c1d-167">Reseller MPN ID</span></span>

<span data-ttu-id="36c1d-168">Si un asociado de CSP vendió la suscripción directamente al cliente, su **identificador de MPN** aparece dos veces, como el **identificador de MPN** y el ID. de **MPN del reseller**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-168">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="36c1d-169">Si un asociado de CSP tiene un revendedor sin **identificador de MPN**, este valor se establece en el **identificador de MPN** del asociado en su lugar.</span><span class="sxs-lookup"><span data-stu-id="36c1d-169">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="36c1d-170">Si el asociado de CSP quita un ID. de **revendedor de MPN**, este valor se establecerá en *-1*.</span><span class="sxs-lookup"><span data-stu-id="36c1d-170">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="36c1d-171">Para ver o actualizar el **ID. de revendedor MPN**:</span><span class="sxs-lookup"><span data-stu-id="36c1d-171">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="36c1d-172">Inicie sesión en el Centro de datos.</span><span class="sxs-lookup"><span data-stu-id="36c1d-172">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="36c1d-173">En el menú del Centro de partners, selecciona **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-173">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="36c1d-174">Elija el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="36c1d-174">Choose the customer from the list.</span></span>
4. <span data-ttu-id="36c1d-175">En el menú del cliente, seleccione **suscripciones**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-175">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="36c1d-176">Elija la suscripción de la lista.</span><span class="sxs-lookup"><span data-stu-id="36c1d-176">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="36c1d-177">Selecciona **Actualizar** para cambiar el valor de **Revendedor (id. de MPN)**.</span><span class="sxs-lookup"><span data-stu-id="36c1d-177">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="36c1d-178">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="36c1d-178">Next steps</span></span>

- [<span data-ttu-id="36c1d-179">Cómo leer el archivo de conciliación & de la factura</span><span class="sxs-lookup"><span data-stu-id="36c1d-179">How to read your bill & recon file</span></span>](read-your-bill.md) 