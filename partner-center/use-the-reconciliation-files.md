---
title: Uso de los archivos de conciliación
ms.topic: article
ms.date: 03/26/2021
description: Obtenga información sobre los archivos de conciliación Centro de partners y cómo interpretar las vistas detalladas de elementos de línea de los cargos de un ciclo de facturación determinado.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431569"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a><span data-ttu-id="e630e-103">Obtenga información sobre cómo leer los elementos de línea en los archivos Centro de partners conciliación</span><span class="sxs-lookup"><span data-stu-id="e630e-103">Learn how to read the line items in your Partner Center reconciliation files</span></span>

<span data-ttu-id="e630e-104">**Roles adecuados:** Administrador de facturación | Administrador global</span><span class="sxs-lookup"><span data-stu-id="e630e-104">**Appropriate roles**: Billing admin | Global admin</span></span>

<span data-ttu-id="e630e-105">Puede descargar los archivos de conciliación Centro de partners obtener una vista detallada de cada cargo en un ciclo de facturación.</span><span class="sxs-lookup"><span data-stu-id="e630e-105">You can download your reconciliation files from Partner Center for a detailed, line-item view of each charge in a billing cycle.</span></span> <span data-ttu-id="e630e-106">Los detalles del elemento de línea incluyen cargos por las suscripciones de cada cliente y eventos detallados (por ejemplo, una adición a medio plazo de licencias a una suscripción).</span><span class="sxs-lookup"><span data-stu-id="e630e-106">Line-item details include charges for each customer's subscriptions, and detailed events (such as a mid-term addition of licenses to a subscription).</span></span>

<span data-ttu-id="e630e-107">Para obtener información sobre cómo leer la **factura,** vea [Leer la factura.](read-your-bill.md)</span><span class="sxs-lookup"><span data-stu-id="e630e-107">For information on how to read your **invoice**, see [Read your bill](read-your-bill.md).</span></span>

## <a name="understand-reconciliation-file-fields"></a><span data-ttu-id="e630e-108">Información sobre los campos del archivo de conciliación</span><span class="sxs-lookup"><span data-stu-id="e630e-108">Understand reconciliation file fields</span></span>

- [<span data-ttu-id="e630e-109">Campos de archivos de conciliación basados en licencias</span><span class="sxs-lookup"><span data-stu-id="e630e-109">License-based reconciliation file fields</span></span>](license-based-recon-files.md)
- [<span data-ttu-id="e630e-110">Campos de archivos de conciliación basados en el uso</span><span class="sxs-lookup"><span data-stu-id="e630e-110">Usage-based reconciliation file fields</span></span>](usage-based-recon-files.md)
- [<span data-ttu-id="e630e-111">Campos de archivos de conciliación de uso con clasificación diaria</span><span class="sxs-lookup"><span data-stu-id="e630e-111">Daily-rated usage reconciliation file fields</span></span>](daily-rated-usage-recon-files.md)
- [<span data-ttu-id="e630e-112">Campos de archivo de conciliación de CSP de compra única</span><span class="sxs-lookup"><span data-stu-id="e630e-112">One-time purchase CSP reconciliation file fields</span></span>](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a><span data-ttu-id="e630e-113">Información sobre los tipos de cargos en los archivos de conciliación</span><span class="sxs-lookup"><span data-stu-id="e630e-113">Understand charge types in reconciliation files</span></span>

<span data-ttu-id="e630e-114">Para comprender los tipos de cargos en los archivos de conciliación (la **columna ChargeType),** vea [Tipos de cargos de archivo de conciliación](recon-file-charge-types.md).</span><span class="sxs-lookup"><span data-stu-id="e630e-114">To understand the types of charges in reconciliation files (the **ChargeType** column), see [Reconciliation file charge types](recon-file-charge-types.md).</span></span>

## <a name="fix-formatting-issues"></a><span data-ttu-id="e630e-115">Corrección de problemas de formato</span><span class="sxs-lookup"><span data-stu-id="e630e-115">Fix formatting issues</span></span>

<span data-ttu-id="e630e-116">En ocasiones, un archivo de conciliación puede contener problemas de formato.</span><span class="sxs-lookup"><span data-stu-id="e630e-116">Occasionally, a reconciliation file might contain formatting issues.</span></span> <span data-ttu-id="e630e-117">Por ejemplo, este problema puede producirse si no se usa la configuración regional en-US.</span><span class="sxs-lookup"><span data-stu-id="e630e-117">For example, this issue might occur if the en-US locale is not used.</span></span>

<span data-ttu-id="e630e-118">Siga estos pasos para corregir cualquier problema de formato en los archivos de conciliación:</span><span class="sxs-lookup"><span data-stu-id="e630e-118">Follow these steps for fix any formatting issues in your reconciliation files:</span></span>

1. <span data-ttu-id="e630e-119">Abra el archivo de conciliación (.csv formato) en Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="e630e-119">Open the reconciliation file (in .csv format) in Microsoft Excel.</span></span>
2. <span data-ttu-id="e630e-120">Seleccione la primera columna del archivo.</span><span class="sxs-lookup"><span data-stu-id="e630e-120">Select the first column in the file.</span></span>
3. <span data-ttu-id="e630e-121">Abra el **Asistente para convertir texto en columnas**.</span><span class="sxs-lookup"><span data-stu-id="e630e-121">Open the **Convert Text to Columns Wizard**.</span></span> <span data-ttu-id="e630e-122">En la cinta de opciones, **seleccione Datos** y, a continuación, seleccione Texto **a columnas.**</span><span class="sxs-lookup"><span data-stu-id="e630e-122">On the ribbon, select **Data**, then select **Text to Columns**.</span></span>
4. <span data-ttu-id="e630e-123">En el asistente, seleccione **Tipo de archivo delimitado**.</span><span class="sxs-lookup"><span data-stu-id="e630e-123">In the wizard, select **Delimited file type**.</span></span> <span data-ttu-id="e630e-124">Después, seleccione **Siguiente**.</span><span class="sxs-lookup"><span data-stu-id="e630e-124">Then, select **Next**.</span></span>
5. <span data-ttu-id="e630e-125">En el **campo Delimitadores,** seleccione **Coma**.</span><span class="sxs-lookup"><span data-stu-id="e630e-125">In the **Delimiters** field, select **Comma**.</span></span> <span data-ttu-id="e630e-126">(Si **tab** ya está seleccionado, puede dejar esta opción seleccionada). A continuación, **seleccione Siguiente.**</span><span class="sxs-lookup"><span data-stu-id="e630e-126">(If **Tab** is already selected, you can leave this option selected.) Then, select **Next**.</span></span>
6. <span data-ttu-id="e630e-127">En el **campo Formato de datos de** columna, seleccione **Date:MDY**.</span><span class="sxs-lookup"><span data-stu-id="e630e-127">In the **Column data format** field, select **Date:MDY**.</span></span> <span data-ttu-id="e630e-128">Después, seleccione **Siguiente**.</span><span class="sxs-lookup"><span data-stu-id="e630e-128">Then, select **Next**.</span></span>
7. <span data-ttu-id="e630e-129">En el campo **Formato de datos de** columna, seleccione Texto **para** todas las columnas de cantidad.</span><span class="sxs-lookup"><span data-stu-id="e630e-129">In the **Column data format** field, select **Text** for all amount columns.</span></span> <span data-ttu-id="e630e-130">A continuación, seleccione **Finish** (Finalizar).</span><span class="sxs-lookup"><span data-stu-id="e630e-130">Then, select **Finish**.</span></span>

## <a name="download-reconciliation-files-programmatically"></a><span data-ttu-id="e630e-131">Descarga de archivos de conciliación mediante programación</span><span class="sxs-lookup"><span data-stu-id="e630e-131">Download reconciliation files programmatically</span></span>

<span data-ttu-id="e630e-132">Los archivos de conciliación pueden ser muy grandes y a veces son difíciles de descargar.</span><span class="sxs-lookup"><span data-stu-id="e630e-132">Reconciliation files can be very large and are sometimes difficult to download.</span></span> <span data-ttu-id="e630e-133">Para descargar archivos de conciliación mediante programación, vea [Obtener elementos de línea de factura.](/partner-center/develop/get-invoiceline-items)</span><span class="sxs-lookup"><span data-stu-id="e630e-133">To download reconciliation files programmatically, see [Get invoice line items](/partner-center/develop/get-invoiceline-items).</span></span>

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a><span data-ttu-id="e630e-134">Si el archivo supera el límite de filas en Excel</span><span class="sxs-lookup"><span data-stu-id="e630e-134">If your file exceeds the row limit in Excel</span></span>

<span data-ttu-id="e630e-135">Si puede descargar un archivo de conciliación pero no abrirlo en Microsoft Excel, probablemente significa que el archivo contiene más filas de las que excel permitirá.</span><span class="sxs-lookup"><span data-stu-id="e630e-135">If you’re able to download a reconciliation file but not open it in Microsoft Excel, it probably means the file contains more rows than Excel will allow.</span></span> <span data-ttu-id="e630e-136">Si esto sucede, puede usar cualquiera de los procedimientos siguientes para abrir el archivo.</span><span class="sxs-lookup"><span data-stu-id="e630e-136">If this happens, you can use either of the procedures below to open the file.</span></span>

### <a name="open-a-recon-file-in-power-bi"></a><span data-ttu-id="e630e-137">Abra un archivo de conciliación en Power BI</span><span class="sxs-lookup"><span data-stu-id="e630e-137">Open a recon file in Power BI</span></span>

1. <span data-ttu-id="e630e-138">Descargue el archivo de conciliación como lo haría normalmente.</span><span class="sxs-lookup"><span data-stu-id="e630e-138">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="e630e-139">Descargue, instale y abra una instancia de Microsoft Power BI.</span><span class="sxs-lookup"><span data-stu-id="e630e-139">Download, install, and open an instance of Microsoft Power BI.</span></span>
3. <span data-ttu-id="e630e-140">En la Power BI **Inicio,** seleccione **Obtener datos.**</span><span class="sxs-lookup"><span data-stu-id="e630e-140">On the Power BI **Home** tab, select **Get data**.</span></span>
4. <span data-ttu-id="e630e-141">En la lista de **orígenes de datos comunes,** seleccione **Texto/CSV.**</span><span class="sxs-lookup"><span data-stu-id="e630e-141">In the list of **Common data sources**, select **Text/CSV**.</span></span>
5. <span data-ttu-id="e630e-142">Cuando se le solicite, abra el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="e630e-142">When prompted, open your recon file.</span></span>

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a><span data-ttu-id="e630e-143">Abrir un archivo de conciliación en una tabla dinámica de Excel</span><span class="sxs-lookup"><span data-stu-id="e630e-143">Open a recon file in an Excel pivot table</span></span>

1. <span data-ttu-id="e630e-144">Descargue el archivo de conciliación como lo haría normalmente.</span><span class="sxs-lookup"><span data-stu-id="e630e-144">Download the reconciliation file as you normally would.</span></span>
2. <span data-ttu-id="e630e-145">Abra un nuevo archivo en Microsoft Excel.</span><span class="sxs-lookup"><span data-stu-id="e630e-145">Open a new file in Microsoft Excel.</span></span>
3. <span data-ttu-id="e630e-146">En la **pestaña Datos,** seleccione **Obtener datos,** **Desde archivo** y, a continuación, **texto/CSV.**</span><span class="sxs-lookup"><span data-stu-id="e630e-146">On the **Data** tab, select **Get data**, select **From file**, and then select **Text/CSV**.</span></span>
4. <span data-ttu-id="e630e-147">Cuando se le solicite, abra el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="e630e-147">When prompted, open your recon file.</span></span> <span data-ttu-id="e630e-148">Aparecerán los datos.</span><span class="sxs-lookup"><span data-stu-id="e630e-148">Your data will appear.</span></span>
5. <span data-ttu-id="e630e-149">En el **menú desplegable** Cargar, seleccione **Cargar en** y, a continuación, **seleccione Aceptar.**</span><span class="sxs-lookup"><span data-stu-id="e630e-149">In the **Load** dropdown menu, select **Load to**, and then select **OK**.</span></span>
6. <span data-ttu-id="e630e-150">En el **cuadro de diálogo Importar** datos, seleccione Informe de tabla **dinámica** para abrir el archivo.</span><span class="sxs-lookup"><span data-stu-id="e630e-150">In the **Import Data** dialog box, select **PivotTable Report** to open your file.</span></span>

## <a name="negative-amount-displayed"></a><span data-ttu-id="e630e-151">Cantidad negativa mostrada</span><span class="sxs-lookup"><span data-stu-id="e630e-151">Negative amount displayed</span></span>

<span data-ttu-id="e630e-152">Es posible que vea una cantidad negativa en el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="e630e-152">You may see a negative amount in your reconciliation file.</span></span> <span data-ttu-id="e630e-153">Este problema se produce normalmente por uno de los siguientes motivos:</span><span class="sxs-lookup"><span data-stu-id="e630e-153">This is probably caused by one of the following things:</span></span>

- <span data-ttu-id="e630e-154">Ha cancelado o reducido recientemente el número de licencias.</span><span class="sxs-lookup"><span data-stu-id="e630e-154">You recently canceled or reduced your number of licenses</span></span>
- <span data-ttu-id="e630e-155">Ha recibido crédito para un contrato de licencia de servicio (SLA) o para el consumo de Azure.</span><span class="sxs-lookup"><span data-stu-id="e630e-155">You received credit for either a service license agreement (SLA) or for Azure consumption</span></span>

<span data-ttu-id="e630e-156">Para obtener más información acerca de esta transacción, revise su atributo de tipo de carga en el archivo de conciliación.</span><span class="sxs-lookup"><span data-stu-id="e630e-156">To get more information about this transaction, review its charge type attribute in your reconciliation file.</span></span>

## <a name="map-taxes-or-vat"></a><span data-ttu-id="e630e-157">Asignación de impuestos o IVA</span><span class="sxs-lookup"><span data-stu-id="e630e-157">Map taxes or VAT</span></span>

<span data-ttu-id="e630e-158">Para asignar impuestos o impuestos al valor agregado (IVA) a la factura:</span><span class="sxs-lookup"><span data-stu-id="e630e-158">To map Taxes or value-added tax (VAT) to your invoice:</span></span>

- <span data-ttu-id="e630e-159">Sumar la **columna** Impuestos del archivo basado en licencia.</span><span class="sxs-lookup"><span data-stu-id="e630e-159">Sum the **Tax** column from the license-based file.</span></span>
- <span data-ttu-id="e630e-160">Sumar **la columna TaxAmount** del archivo basado en uso.</span><span class="sxs-lookup"><span data-stu-id="e630e-160">Sum the **TaxAmount** column from the usage-based file.</span></span>

## <a name="itemize-reconciliation-files-by-partner"></a><span data-ttu-id="e630e-161">Elementos de los archivos de conciliación por asociado</span><span class="sxs-lookup"><span data-stu-id="e630e-161">Itemize reconciliation files by partner</span></span>

<span data-ttu-id="e630e-162">Los asociados **del modelo indirecto** pueden usar estos campos adicionales en los archivos de conciliación basados en licencias y basados en el uso para especificar los archivos por revendedor.</span><span class="sxs-lookup"><span data-stu-id="e630e-162">Partners in the **indirect model** can use these additional fields in both license-based and usage-based reconciliation files to itemize the files by reseller.</span></span>

| <span data-ttu-id="e630e-163">Identificador de MPN</span><span class="sxs-lookup"><span data-stu-id="e630e-163">MPN ID</span></span> | <span data-ttu-id="e630e-164">Descripción</span><span class="sxs-lookup"><span data-stu-id="e630e-164">Description</span></span> |
| ------ | ----------- |
| <span data-ttu-id="e630e-165">Identificador de MPN</span><span class="sxs-lookup"><span data-stu-id="e630e-165">MPN ID</span></span> | <span data-ttu-id="e630e-166">Identificador Microsoft Partner Network (MPN) del asociado de Proveedor de soluciones en la nube (CSP) (directo o indirecto).</span><span class="sxs-lookup"><span data-stu-id="e630e-166">The Microsoft Partner Network (MPN) identifier of the Cloud Solution Provider (CSP) partner (direct or indirect).</span></span> |
| [<span data-ttu-id="e630e-167">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="e630e-167">Reseller MPN ID</span></span>](#reseller-mpn-id) | <span data-ttu-id="e630e-168">Identificador [de MPN del revendedor del registro de la suscripción.](#reseller-mpn-id)</span><span class="sxs-lookup"><span data-stu-id="e630e-168">The [MPN identifier of the reseller of record for the subscription](#reseller-mpn-id).</span></span> <span data-ttu-id="e630e-169">Este campo corresponde al identificador de revendedor que aparece para la suscripción específica en Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="e630e-169">This field corresponds to the reseller ID listed for the specific subscription in Partner Center.</span></span> <span data-ttu-id="e630e-170">Solo aparece en los archivos de conciliación de partners en el modelo indirecto.</span><span class="sxs-lookup"><span data-stu-id="e630e-170">Only appears on reconciliation files for partners in the indirect model.</span></span> |

### <a name="reseller-mpn-id"></a><span data-ttu-id="e630e-171">Id. de MPN del revendedor</span><span class="sxs-lookup"><span data-stu-id="e630e-171">Reseller MPN ID</span></span>

<span data-ttu-id="e630e-172">Si un asociado de CSP vende la suscripción directamente al cliente, su identificador **de MPN** aparece dos veces, como el identificador de **MPN** y el identificador **de MPN del revendedor.**</span><span class="sxs-lookup"><span data-stu-id="e630e-172">If a CSP partner sold the subscription directly to the customer, their **MPN ID** is listed twice, as both the **MPN ID** and the **Reseller MPN ID**.</span></span>

<span data-ttu-id="e630e-173">Si un asociado de CSP tiene un revendedor sin identificador **de MPN,** este valor se establece en el identificador **de MPN del** asociado en su lugar.</span><span class="sxs-lookup"><span data-stu-id="e630e-173">If a CSP partner has a reseller with no **MPN ID**, this value is set to the partner's **MPN ID** instead.</span></span>

<span data-ttu-id="e630e-174">Si el asociado de CSP quita un **id. de MPN de revendedor,** este valor se establecerá en *-1.*</span><span class="sxs-lookup"><span data-stu-id="e630e-174">If the CSP partner removes a **Reseller MPN ID**, this value will be set to *-1*.</span></span>

<span data-ttu-id="e630e-175">Para ver o actualizar el identificador **de MPN del revendedor:**</span><span class="sxs-lookup"><span data-stu-id="e630e-175">To view or update the **Reseller MPN ID**:</span></span>

1. <span data-ttu-id="e630e-176">Inicie sesión en el Centro de datos.</span><span class="sxs-lookup"><span data-stu-id="e630e-176">Sign in to Partner Center.</span></span>
2. <span data-ttu-id="e630e-177">En el menú del Centro de partners, selecciona **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="e630e-177">In the Partner Center menu, select **Customers**.</span></span>
3. <span data-ttu-id="e630e-178">Elija el cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="e630e-178">Choose the customer from the list.</span></span>
4. <span data-ttu-id="e630e-179">En el menú del cliente, seleccione **Suscripciones.**</span><span class="sxs-lookup"><span data-stu-id="e630e-179">In the customer menu, select **Subscriptions**.</span></span>
5. <span data-ttu-id="e630e-180">Elija la suscripción de la lista.</span><span class="sxs-lookup"><span data-stu-id="e630e-180">Choose the subscription from the list.</span></span>
6. <span data-ttu-id="e630e-181">Selecciona **Actualizar** para cambiar el valor de **Revendedor (id. de MPN)**.</span><span class="sxs-lookup"><span data-stu-id="e630e-181">Select **update** to change the **Reseller (MPN ID)**.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e630e-182">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="e630e-182">Next steps</span></span>

- [<span data-ttu-id="e630e-183">Cómo leer el archivo de conciliación & facturación</span><span class="sxs-lookup"><span data-stu-id="e630e-183">How to read your bill & recon file</span></span>](read-your-bill.md) 