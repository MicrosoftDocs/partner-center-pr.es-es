---
title: Crear varios usuarios para una cuenta de cliente | Centro de partners
description: Puedes agregar varios usuarios a la vez a una cuenta de cliente, mediante la carga en el Centro de partners de un archivo de datos con el formato de archivo de valores separados por comas (.csv).
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
keywords: carga masiva, agregar varios usuarios a una cuenta de cliente, agregar usuarios del cliente, carga masiva de usuarios del cliente, cuenta del cliente, usuarios del cliente, usuarios
ms.localizationpriority: medium
ms.openlocfilehash: e7a5e7f9c0cebf81373c500dd3a552710fcf845a
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/31/2018
ms.locfileid: "2876975"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="3f275-104">Agregar varios usuarios a una cuenta de cliente</span><span class="sxs-lookup"><span data-stu-id="3f275-104">Add multiple users to a customer account</span></span>

**<span data-ttu-id="3f275-105">Se aplica a</span><span class="sxs-lookup"><span data-stu-id="3f275-105">Applies to</span></span>**

-  <span data-ttu-id="3f275-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="3f275-106">Partner Center</span></span>

<span data-ttu-id="3f275-107">Puedes agregar varios usuarios a la vez a una cuenta de cliente, cargando un archivo de datos con formato de archivo de valores separados por comas (.csv) en el panel partners.</span><span class="sxs-lookup"><span data-stu-id="3f275-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Dashboard.</span></span> <span data-ttu-id="3f275-108">Puedes descargar un archivo de datos de muestra desde el Panel de partners y después modificarlo para usarlo, o puedes crear un nuevo archivo de datos usando el modelo de datos que se define a continuación.</span><span class="sxs-lookup"><span data-stu-id="3f275-108">You can download a sample data file from the Partner Dashboard and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="3f275-109">Requisitos del archivo de datos:</span><span class="sxs-lookup"><span data-stu-id="3f275-109">Data file requirements</span></span>


<span data-ttu-id="3f275-110">Para agregar varios usuarios a la cuenta de un cliente mediante el proceso de carga masiva, es necesario cumplir los siguientes requisitos:</span><span class="sxs-lookup"><span data-stu-id="3f275-110">To add multiple users to a customer’s account using the bulk upload process, you’ll need to meet the following requirements:</span></span>

-   <span data-ttu-id="3f275-111">Debes tener permisos de administrador global para la cuenta de cliente.</span><span class="sxs-lookup"><span data-stu-id="3f275-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="3f275-112">Cada usuario debe tener una dirección de correo electrónico exclusiva, anexa a los dominios de correo electrónico del cliente.</span><span class="sxs-lookup"><span data-stu-id="3f275-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="3f275-113">Puedes subir hasta 100 registros a la vez.</span><span class="sxs-lookup"><span data-stu-id="3f275-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="3f275-114">Si es necesario agregar más de 100 usuarios, crea y sube archivos de datos adicionales.</span><span class="sxs-lookup"><span data-stu-id="3f275-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="3f275-115">Todos los usuarios deben estar en la misma **ubicación** geográfica.</span><span class="sxs-lookup"><span data-stu-id="3f275-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="3f275-116">Escribe solo los datos que se describen a continuación.</span><span class="sxs-lookup"><span data-stu-id="3f275-116">Enter only the data described below.</span></span> <span data-ttu-id="3f275-117">Unos datos extraños hará que la carga sufra un error.</span><span class="sxs-lookup"><span data-stu-id="3f275-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="3f275-118">Escribe los siguientes datos en el archivo de datos:</span><span class="sxs-lookup"><span data-stu-id="3f275-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **<span data-ttu-id="3f275-119">Nombre de columna</span><span class="sxs-lookup"><span data-stu-id="3f275-119">Column name</span></span>** | **<span data-ttu-id="3f275-120">Descripción</span><span class="sxs-lookup"><span data-stu-id="3f275-120">Description</span></span>**                                                              | **<span data-ttu-id="3f275-121">Limitaciones</span><span class="sxs-lookup"><span data-stu-id="3f275-121">Limitation</span></span>**                             |
| <span data-ttu-id="3f275-122">Nombre</span><span class="sxs-lookup"><span data-stu-id="3f275-122">First name</span></span>      | <span data-ttu-id="3f275-123">El nombre de pila del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="3f275-123">User’s first name (optional field)</span></span>                                           | <span data-ttu-id="3f275-124">Límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="3f275-124">50-character limit</span></span>                         |
| <span data-ttu-id="3f275-125">Apellidos</span><span class="sxs-lookup"><span data-stu-id="3f275-125">Last name</span></span>       | <span data-ttu-id="3f275-126">Los apellidos del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="3f275-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="3f275-127">Límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="3f275-127">50-character limit</span></span>                         |
| <span data-ttu-id="3f275-128">Nombre para mostrar</span><span class="sxs-lookup"><span data-stu-id="3f275-128">Display name</span></span>    | <span data-ttu-id="3f275-129">El nombre que aparece en el Panel de partners (campo obligatorio).</span><span class="sxs-lookup"><span data-stu-id="3f275-129">Name displayed in the Partner Dashboard (required field)</span></span>                            | <span data-ttu-id="3f275-130">Límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="3f275-130">50-character limit</span></span>                         |
| <span data-ttu-id="3f275-131">Correo electrónico</span><span class="sxs-lookup"><span data-stu-id="3f275-131">Email</span></span>           | <span data-ttu-id="3f275-132">La dirección de correo electrónico comercial del usuario en la compañía del cliente (campo obligatorio).</span><span class="sxs-lookup"><span data-stu-id="3f275-132">User’s business email address at customer company (required field)</span></span>           | <span data-ttu-id="3f275-133">Cada usuario debe tener una dirección de correo electrónico exclusiva.</span><span class="sxs-lookup"><span data-stu-id="3f275-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="3f275-134">Actualización de estado</span><span class="sxs-lookup"><span data-stu-id="3f275-134">Status update</span></span>   | <span data-ttu-id="3f275-135">Se usa para indicar si el nuevo registro de usuario se ha creado correctamente o no.</span><span class="sxs-lookup"><span data-stu-id="3f275-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="3f275-136">\*\*Dejar vacío\* \ *</span><span class="sxs-lookup"><span data-stu-id="3f275-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="3f275-137">Para crear varias cuentas de usuario</span><span class="sxs-lookup"><span data-stu-id="3f275-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="3f275-138">Crea un archivo de datos de valores separados por comas (.csv) con los datos que se han descrito anteriormente.</span><span class="sxs-lookup"><span data-stu-id="3f275-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="3f275-139">Guarda el archivo para que puedas acceder a él en un paso posterior.</span><span class="sxs-lookup"><span data-stu-id="3f275-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="3f275-140">Desde el menú **Panel**, selecciona **Clientes** y elige un cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="3f275-140">From the **Dashboard** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="3f275-141">Selecciona **Subir usuarios**.</span><span class="sxs-lookup"><span data-stu-id="3f275-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="3f275-142">En **Subir información de usuarios**, selecciona **Examinar**.</span><span class="sxs-lookup"><span data-stu-id="3f275-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="3f275-143">En el selector de archivos, selecciona el archivo de datos y, a continuación, selecciona **Abrir**.</span><span class="sxs-lookup"><span data-stu-id="3f275-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="3f275-144">Selecciona **Validar**.</span><span class="sxs-lookup"><span data-stu-id="3f275-144">Select **Validate**.</span></span>

    <span data-ttu-id="3f275-145">**Nota**: La mayoría de los errores de creación de cuentas se deben a problemas en los archivos de datos, lo que incluye la falta de información, unas direcciones de correo electrónico con formato incorrecto o duplicadas o un exceso de registros en el archivo.</span><span class="sxs-lookup"><span data-stu-id="3f275-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

7.  <span data-ttu-id="3f275-146">Cuando el Panel de partners haya validado el archivo, selecciona la **Ubicación** geográfica para los nuevos usuarios.</span><span class="sxs-lookup"><span data-stu-id="3f275-146">After the Partner Dashboard validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="3f275-147">Selecciona **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="3f275-147">Select **Save**.</span></span>
9.  <span data-ttu-id="3f275-148">Descarga la información de la contraseña temporal para los usuarios.</span><span class="sxs-lookup"><span data-stu-id="3f275-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="3f275-149">**IMPORTANTE:** Asegúrate de descargar el archivo con las contraseñas temporales ahora, ya no podrás hacerlo más adelante.</span><span class="sxs-lookup"><span data-stu-id="3f275-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="3f275-150">Los nuevos usuarios deben iniciar sesión en su nueva cuenta con las contraseñas temporales correspondientes a sus nuevas cuentas.</span><span class="sxs-lookup"><span data-stu-id="3f275-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="3f275-151">Los nuevos usuarios se les asignará automáticamente los permisos de **puede usar licencias y servicios** .</span><span class="sxs-lookup"><span data-stu-id="3f275-151">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



