---
title: Agregar varios usuarios para una cuenta de cliente
ms.topic: article
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información sobre cómo agregar varios usuarios a la cuenta de un cliente a la vez. Cargue un archivo de datos en el centro de Partners con el formato de archivo de valores separados por comas (. csv).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a9a94ac9d9022b33c7f909a258b66daa4312ad13
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436314"
---
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a><span data-ttu-id="75e6c-104">Agregar varios usuarios a una cuenta de cliente: cargar un archivo de datos en el centro de Partners</span><span class="sxs-lookup"><span data-stu-id="75e6c-104">Add multiple users to a customer account - upload a data file to Partner Center</span></span>

<span data-ttu-id="75e6c-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="75e6c-105">**Applies to**</span></span>

- <span data-ttu-id="75e6c-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="75e6c-106">Partner Center</span></span>

<span data-ttu-id="75e6c-107">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="75e6c-107">**Appropriate roles**</span></span>

- <span data-ttu-id="75e6c-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="75e6c-108">Global admin</span></span>

<span data-ttu-id="75e6c-109">Puede agregar varios usuarios a la cuenta de un cliente a la vez, cargando un archivo de datos en el formato de archivo de valores separados por comas (. csv) al centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="75e6c-109">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="75e6c-110">Puede descargar un archivo de datos de ejemplo del centro de Partners y editarlo para su uso, o puede crear un nuevo archivo de datos con el modelo de datos definido a continuación.</span><span class="sxs-lookup"><span data-stu-id="75e6c-110">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="75e6c-111">Requisitos del archivo de datos:</span><span class="sxs-lookup"><span data-stu-id="75e6c-111">Data file requirements</span></span>

<span data-ttu-id="75e6c-112">Para agregar varios usuarios a la cuenta de un cliente mediante el proceso de carga masiva, debe cumplir los siguientes requisitos:</span><span class="sxs-lookup"><span data-stu-id="75e6c-112">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="75e6c-113">Debes tener permisos de administrador global para la cuenta de cliente.</span><span class="sxs-lookup"><span data-stu-id="75e6c-113">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="75e6c-114">Cada usuario debe tener una dirección de correo electrónico exclusiva, anexa a los dominios de correo electrónico del cliente.</span><span class="sxs-lookup"><span data-stu-id="75e6c-114">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="75e6c-115">Puedes subir hasta 100 registros a la vez.</span><span class="sxs-lookup"><span data-stu-id="75e6c-115">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="75e6c-116">Si es necesario agregar más de 100 usuarios, crea y sube archivos de datos adicionales.</span><span class="sxs-lookup"><span data-stu-id="75e6c-116">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="75e6c-117">Todos los usuarios deben estar en la misma **ubicación** geográfica.</span><span class="sxs-lookup"><span data-stu-id="75e6c-117">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="75e6c-118">Escribe solo los datos que se describen a continuación.</span><span class="sxs-lookup"><span data-stu-id="75e6c-118">Enter only the data described below.</span></span> <span data-ttu-id="75e6c-119">Unos datos extraños hará que la carga sufra un error.</span><span class="sxs-lookup"><span data-stu-id="75e6c-119">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="75e6c-120">Escribe los siguientes datos en el archivo de datos:</span><span class="sxs-lookup"><span data-stu-id="75e6c-120">Enter the following data in the data file:</span></span>

| <span data-ttu-id="75e6c-121">**Nombre de la columna**</span><span class="sxs-lookup"><span data-stu-id="75e6c-121">**Column name**</span></span> | <span data-ttu-id="75e6c-122">**Descripción**</span><span class="sxs-lookup"><span data-stu-id="75e6c-122">**Description**</span></span>  | <span data-ttu-id="75e6c-123">**Limitación**</span><span class="sxs-lookup"><span data-stu-id="75e6c-123">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="75e6c-124">Nombre</span><span class="sxs-lookup"><span data-stu-id="75e6c-124">First name</span></span>  | <span data-ttu-id="75e6c-125">Nombre del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="75e6c-125">User's first name (optional field)</span></span>  | <span data-ttu-id="75e6c-126">límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="75e6c-126">50-character limit</span></span>  |
| <span data-ttu-id="75e6c-127">Apellidos</span><span class="sxs-lookup"><span data-stu-id="75e6c-127">Last name</span></span>  | <span data-ttu-id="75e6c-128">Los apellidos del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="75e6c-128">User's last name (optional field)</span></span>  | <span data-ttu-id="75e6c-129">límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="75e6c-129">50-character limit</span></span>  |
| <span data-ttu-id="75e6c-130">Nombre para mostrar</span><span class="sxs-lookup"><span data-stu-id="75e6c-130">Display name</span></span>    | <span data-ttu-id="75e6c-131">Nombre mostrado en el centro de Partners (campo obligatorio)</span><span class="sxs-lookup"><span data-stu-id="75e6c-131">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="75e6c-132">límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="75e6c-132">50-character limit</span></span>                         |
| <span data-ttu-id="75e6c-133">Email</span><span class="sxs-lookup"><span data-stu-id="75e6c-133">Email</span></span>   | <span data-ttu-id="75e6c-134">Dirección de correo electrónico empresarial del usuario en la empresa del cliente (campo obligatorio)</span><span class="sxs-lookup"><span data-stu-id="75e6c-134">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="75e6c-135">Cada usuario debe tener una dirección de correo electrónico única</span><span class="sxs-lookup"><span data-stu-id="75e6c-135">Each user must have a unique email address</span></span> |
| <span data-ttu-id="75e6c-136">Actualización del estado</span><span class="sxs-lookup"><span data-stu-id="75e6c-136">Status update</span></span>   | <span data-ttu-id="75e6c-137">Se usa para indicar si el nuevo registro de usuario se ha creado correctamente o no.</span><span class="sxs-lookup"><span data-stu-id="75e6c-137">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="75e6c-138">\*\*Dejar vacío\*\*</span><span class="sxs-lookup"><span data-stu-id="75e6c-138">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="75e6c-139">Para crear varias cuentas de usuario</span><span class="sxs-lookup"><span data-stu-id="75e6c-139">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="75e6c-140">Crea un archivo de datos de valores separados por comas (.csv) con los datos que se han descrito anteriormente.</span><span class="sxs-lookup"><span data-stu-id="75e6c-140">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="75e6c-141">Guarda el archivo para que puedas acceder a él en un paso posterior.</span><span class="sxs-lookup"><span data-stu-id="75e6c-141">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="75e6c-142">Inicia sesión en el [panel](https://partner.microsoft.com/dashboard) del Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="75e6c-142">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="75e6c-143">Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="75e6c-143">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="75e6c-144">Seleccione la pestaña **usuarios y licencias** del cliente y, a continuación, seleccione **cargar usuarios**.</span><span class="sxs-lookup"><span data-stu-id="75e6c-144">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="75e6c-145">En **Subir información de usuarios**, selecciona **Examinar**.</span><span class="sxs-lookup"><span data-stu-id="75e6c-145">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="75e6c-146">En el selector de archivos, selecciona el archivo de datos y, a continuación, selecciona **Abrir**.</span><span class="sxs-lookup"><span data-stu-id="75e6c-146">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="75e6c-147">Seleccione **Validar**.</span><span class="sxs-lookup"><span data-stu-id="75e6c-147">Select **Validate**.</span></span>

    <span data-ttu-id="75e6c-148">**Nota:**    La mayoría de los errores de creación de cuentas están causados por problemas de archivos de datos, incluida la información que falta, direcciones de correo electrónico con formato incorrecto o duplicadas o demasiados registros en el archivo.</span><span class="sxs-lookup"><span data-stu-id="75e6c-148">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="75e6c-149">Una vez que el centro de Partners valida el archivo, seleccione la **Ubicación** geográfica para los nuevos usuarios.</span><span class="sxs-lookup"><span data-stu-id="75e6c-149">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="75e6c-150">Seleccione **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="75e6c-150">Select **Save**.</span></span>
10. <span data-ttu-id="75e6c-151">Descargue la información de contraseña temporal de los usuarios.</span><span class="sxs-lookup"><span data-stu-id="75e6c-151">Download the temporary password information for the users.</span></span>

<span data-ttu-id="75e6c-152">**IMPORTANTE:** Asegúrate de descargar el archivo con las contraseñas temporales ahora, ya no podrás hacerlo más adelante.</span><span class="sxs-lookup"><span data-stu-id="75e6c-152">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="75e6c-153">Los nuevos usuarios deben iniciar sesión en su nueva cuenta con las contraseñas temporales correspondientes a sus nuevas cuentas.</span><span class="sxs-lookup"><span data-stu-id="75e6c-153">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="75e6c-154">A los nuevos usuarios se les asignan permisos automáticamente **para utilizar licencias y servicios** .</span><span class="sxs-lookup"><span data-stu-id="75e6c-154">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



