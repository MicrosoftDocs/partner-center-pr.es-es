---
title: Crear varios usuarios para una cuenta de cliente | Centro de partners
ms.topic: article
ms.date: 10/29/2018
description: Puedes agregar varios usuarios a la vez a una cuenta de cliente, mediante la carga en el Centro de partners de un archivo de datos con el formato de archivo de valores separados por comas (.csv).
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: carga masiva, agregar varios usuarios a una cuenta de cliente, agregar usuarios del cliente, carga masiva de usuarios del cliente, cuenta del cliente, usuarios del cliente, usuarios
ms.localizationpriority: medium
ms.openlocfilehash: 12bb42d4e1dcf5003ac8790be777c483f216fd6f
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2019
ms.locfileid: "57584248"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="fe3e3-104">Agregar varios usuarios a una cuenta de cliente</span><span class="sxs-lookup"><span data-stu-id="fe3e3-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="fe3e3-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="fe3e3-105">**Applies to**</span></span>

-  <span data-ttu-id="fe3e3-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="fe3e3-106">Partner Center</span></span>

<span data-ttu-id="fe3e3-107">Puede agregar varios usuarios a una cuenta de cliente al mismo tiempo, al cargar un archivo de datos en el formato de archivo de valores separados por comas (.csv) en el centro de partners.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="fe3e3-108">Puede descargar un archivo de datos de ejemplo desde el centro de partners y, a continuación, modificarlo para su uso, o puede crear un nuevo archivo de datos utilizando el modelo de datos que se definen a continuación.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-108">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="fe3e3-109">Requisitos del archivo de datos</span><span class="sxs-lookup"><span data-stu-id="fe3e3-109">Data file requirements</span></span>


<span data-ttu-id="fe3e3-110">Para agregar varios usuarios a la cuenta de un cliente mediante el proceso de carga masiva, es necesario cumplir los siguientes requisitos:</span><span class="sxs-lookup"><span data-stu-id="fe3e3-110">To add multiple users to a customer’s account using the bulk upload process, you’ll need to meet the following requirements:</span></span>

-   <span data-ttu-id="fe3e3-111">Debes tener permisos de administrador global para la cuenta de cliente.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="fe3e3-112">Cada usuario debe tener una dirección de correo electrónico exclusiva, anexa a los dominios de correo electrónico del cliente.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="fe3e3-113">Puedes subir hasta 100 registros a la vez.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="fe3e3-114">Si es necesario agregar más de 100 usuarios, crea y sube archivos de datos adicionales.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="fe3e3-115">Todos los usuarios deben estar en la misma **ubicación** geográfica.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="fe3e3-116">Escribe solo los datos que se describen a continuación.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-116">Enter only the data described below.</span></span> <span data-ttu-id="fe3e3-117">Unos datos extraños hará que la carga sufra un error.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="fe3e3-118">Escribe los siguientes datos en el archivo de datos:</span><span class="sxs-lookup"><span data-stu-id="fe3e3-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="fe3e3-119">**Nombre de columna**</span><span class="sxs-lookup"><span data-stu-id="fe3e3-119">**Column name**</span></span> | <span data-ttu-id="fe3e3-120">**Descripción**</span><span class="sxs-lookup"><span data-stu-id="fe3e3-120">**Description**</span></span>                                                              | <span data-ttu-id="fe3e3-121">**Limitación**</span><span class="sxs-lookup"><span data-stu-id="fe3e3-121">**Limitation**</span></span>                             |
| <span data-ttu-id="fe3e3-122">Nombre</span><span class="sxs-lookup"><span data-stu-id="fe3e3-122">First name</span></span>      | <span data-ttu-id="fe3e3-123">El nombre de pila del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="fe3e3-123">User’s first name (optional field)</span></span>                                           | <span data-ttu-id="fe3e3-124">Límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="fe3e3-124">50-character limit</span></span>                         |
| <span data-ttu-id="fe3e3-125">Apellidos</span><span class="sxs-lookup"><span data-stu-id="fe3e3-125">Last name</span></span>       | <span data-ttu-id="fe3e3-126">Los apellidos del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="fe3e3-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="fe3e3-127">Límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="fe3e3-127">50-character limit</span></span>                         |
| <span data-ttu-id="fe3e3-128">Nombre para mostrar</span><span class="sxs-lookup"><span data-stu-id="fe3e3-128">Display name</span></span>    | <span data-ttu-id="fe3e3-129">Nombre que aparece en el centro de partners (campo obligatorio)</span><span class="sxs-lookup"><span data-stu-id="fe3e3-129">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="fe3e3-130">Límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="fe3e3-130">50-character limit</span></span>                         |
| <span data-ttu-id="fe3e3-131">Correo electrónico</span><span class="sxs-lookup"><span data-stu-id="fe3e3-131">Email</span></span>           | <span data-ttu-id="fe3e3-132">La dirección de correo electrónico comercial del usuario en la compañía del cliente (campo obligatorio).</span><span class="sxs-lookup"><span data-stu-id="fe3e3-132">User’s business email address at customer company (required field)</span></span>           | <span data-ttu-id="fe3e3-133">Cada usuario debe tener una dirección de correo electrónico exclusiva.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="fe3e3-134">Actualización de estado</span><span class="sxs-lookup"><span data-stu-id="fe3e3-134">Status update</span></span>   | <span data-ttu-id="fe3e3-135">Se usa para indicar si el nuevo registro de usuario se ha creado correctamente o no.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="fe3e3-136">\*\*Deje en blanco\*\*</span><span class="sxs-lookup"><span data-stu-id="fe3e3-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="fe3e3-137">Para crear varias cuentas de usuario</span><span class="sxs-lookup"><span data-stu-id="fe3e3-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="fe3e3-138">Crea un archivo de datos de valores separados por comas (.csv) con los datos que se han descrito anteriormente.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="fe3e3-139">Guarda el archivo para que puedas acceder a él en un paso posterior.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="fe3e3-140">Desde el **centro de partners** menú, seleccione **clientes**, a continuación, elija un cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-140">From the **Partner Center** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="fe3e3-141">Selecciona **Subir usuarios**.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="fe3e3-142">En **Subir información de usuarios**, selecciona **Examinar**.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="fe3e3-143">En el selector de archivos, selecciona el archivo de datos y, a continuación, selecciona **Abrir**.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="fe3e3-144">Selecciona **Validar**.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-144">Select **Validate**.</span></span>

    <span data-ttu-id="fe3e3-145">**Tenga en cuenta**  mayoría de los errores de creación de cuenta está provocada por problemas de archivo de datos, incluida la falta de información, direcciones de correo electrónico con formato incorrecto o está duplicado o hay demasiados registros en el archivo.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

7.  <span data-ttu-id="fe3e3-146">Una vez que el centro de partners se valida el archivo, seleccione el geográfica **ubicación** para los nuevos usuarios.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-146">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="fe3e3-147">Selecciona **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-147">Select **Save**.</span></span>
9.  <span data-ttu-id="fe3e3-148">Descarga la información de la contraseña temporal para los usuarios.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="fe3e3-149">**IMPORTANTE:** Asegúrese de descargar el archivo con las contraseñas temporales ahora, ya no podrá hacerlo más tarde.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="fe3e3-150">Los nuevos usuarios deben iniciar sesión en su nueva cuenta con las contraseñas temporales correspondientes a sus nuevas cuentas.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="fe3e3-151">Los nuevos usuarios reciben asignación automática de permisos de **Puede usar licencias y servicios**.</span><span class="sxs-lookup"><span data-stu-id="fe3e3-151">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



