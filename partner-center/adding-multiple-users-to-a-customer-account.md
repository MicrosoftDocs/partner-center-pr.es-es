---
title: Crear varios usuarios para una cuenta de cliente | Centro de partners
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información acerca de cómo agregar varios usuarios a la cuenta de un cliente a la vez, cargando un archivo de datos en el formato de archivo de valores separados por comas (. csv) en el centro de Partners.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: carga masiva, agregar varios usuarios a una cuenta de cliente, agregar usuarios del cliente, carga masiva de usuarios del cliente, cuenta del cliente, usuarios del cliente, usuarios
ms.localizationpriority: medium
ms.openlocfilehash: 5c9de7ed78a0494790b447d1755d5eef70a89cca
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253179"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="56f68-104">Agregar varios usuarios a una cuenta de cliente</span><span class="sxs-lookup"><span data-stu-id="56f68-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="56f68-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="56f68-105">**Applies to**</span></span>

-  <span data-ttu-id="56f68-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="56f68-106">Partner Center</span></span>

<span data-ttu-id="56f68-107">Puede agregar varios usuarios a la cuenta de un cliente a la vez, cargando un archivo de datos en el formato de archivo de valores separados por comas (. csv) al centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="56f68-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="56f68-108">Puede descargar un archivo de datos de ejemplo del centro de Partners y editarlo para su uso, o puede crear un nuevo archivo de datos con el modelo de datos definido a continuación.</span><span class="sxs-lookup"><span data-stu-id="56f68-108">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="56f68-109">Requisitos del archivo de datos</span><span class="sxs-lookup"><span data-stu-id="56f68-109">Data file requirements</span></span>


<span data-ttu-id="56f68-110">Para agregar varios usuarios a la cuenta de un cliente mediante el proceso de carga masiva, debe cumplir los siguientes requisitos:</span><span class="sxs-lookup"><span data-stu-id="56f68-110">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

-   <span data-ttu-id="56f68-111">Debes tener permisos de administrador global para la cuenta de cliente.</span><span class="sxs-lookup"><span data-stu-id="56f68-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="56f68-112">Cada usuario debe tener una dirección de correo electrónico exclusiva, anexa a los dominios de correo electrónico del cliente.</span><span class="sxs-lookup"><span data-stu-id="56f68-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="56f68-113">Puedes subir hasta 100 registros a la vez.</span><span class="sxs-lookup"><span data-stu-id="56f68-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="56f68-114">Si es necesario agregar más de 100 usuarios, crea y sube archivos de datos adicionales.</span><span class="sxs-lookup"><span data-stu-id="56f68-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="56f68-115">Todos los usuarios deben estar en la misma **ubicación** geográfica.</span><span class="sxs-lookup"><span data-stu-id="56f68-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="56f68-116">Escribe solo los datos que se describen a continuación.</span><span class="sxs-lookup"><span data-stu-id="56f68-116">Enter only the data described below.</span></span> <span data-ttu-id="56f68-117">Unos datos extraños hará que la carga sufra un error.</span><span class="sxs-lookup"><span data-stu-id="56f68-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="56f68-118">Escribe los siguientes datos en el archivo de datos:</span><span class="sxs-lookup"><span data-stu-id="56f68-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="56f68-119">**Nombre de columna**</span><span class="sxs-lookup"><span data-stu-id="56f68-119">**Column name**</span></span> | <span data-ttu-id="56f68-120">**Descripción**</span><span class="sxs-lookup"><span data-stu-id="56f68-120">**Description**</span></span>                                                              | <span data-ttu-id="56f68-121">**Única**</span><span class="sxs-lookup"><span data-stu-id="56f68-121">**Limitation**</span></span>                             |
| <span data-ttu-id="56f68-122">Nombre</span><span class="sxs-lookup"><span data-stu-id="56f68-122">First name</span></span>      | <span data-ttu-id="56f68-123">Nombre del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="56f68-123">User's first name (optional field)</span></span>                                           | <span data-ttu-id="56f68-124">Límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="56f68-124">50-character limit</span></span>                         |
| <span data-ttu-id="56f68-125">Apellidos</span><span class="sxs-lookup"><span data-stu-id="56f68-125">Last name</span></span>       | <span data-ttu-id="56f68-126">Los apellidos del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="56f68-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="56f68-127">Límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="56f68-127">50-character limit</span></span>                         |
| <span data-ttu-id="56f68-128">Nombre para mostrar</span><span class="sxs-lookup"><span data-stu-id="56f68-128">Display name</span></span>    | <span data-ttu-id="56f68-129">Nombre mostrado en el centro de Partners (campo obligatorio)</span><span class="sxs-lookup"><span data-stu-id="56f68-129">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="56f68-130">Límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="56f68-130">50-character limit</span></span>                         |
| <span data-ttu-id="56f68-131">Correo electrónico</span><span class="sxs-lookup"><span data-stu-id="56f68-131">Email</span></span>           | <span data-ttu-id="56f68-132">Dirección de correo electrónico empresarial del usuario en la empresa del cliente (campo obligatorio)</span><span class="sxs-lookup"><span data-stu-id="56f68-132">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="56f68-133">Cada usuario debe tener una dirección de correo electrónico exclusiva.</span><span class="sxs-lookup"><span data-stu-id="56f68-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="56f68-134">Actualización de estado</span><span class="sxs-lookup"><span data-stu-id="56f68-134">Status update</span></span>   | <span data-ttu-id="56f68-135">Se usa para indicar si el nuevo registro de usuario se ha creado correctamente o no.</span><span class="sxs-lookup"><span data-stu-id="56f68-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="56f68-136">\*\*deje\*vacío \*</span><span class="sxs-lookup"><span data-stu-id="56f68-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="56f68-137">Para crear varias cuentas de usuario</span><span class="sxs-lookup"><span data-stu-id="56f68-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="56f68-138">Crea un archivo de datos de valores separados por comas (.csv) con los datos que se han descrito anteriormente.</span><span class="sxs-lookup"><span data-stu-id="56f68-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="56f68-139">Guarda el archivo para que puedas acceder a él en un paso posterior.</span><span class="sxs-lookup"><span data-stu-id="56f68-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="56f68-140">En el menú del **centro de Partners** , seleccione **clientes**y, a continuación, elija un cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="56f68-140">From the **Partner Center** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="56f68-141">Selecciona **Subir usuarios**.</span><span class="sxs-lookup"><span data-stu-id="56f68-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="56f68-142">En **Subir información de usuarios**, selecciona **Examinar**.</span><span class="sxs-lookup"><span data-stu-id="56f68-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="56f68-143">En el selector de archivos, selecciona el archivo de datos y, a continuación, selecciona **Abrir**.</span><span class="sxs-lookup"><span data-stu-id="56f68-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="56f68-144">Selecciona **Validar**.</span><span class="sxs-lookup"><span data-stu-id="56f68-144">Select **Validate**.</span></span>

    <span data-ttu-id="56f68-145">**Tenga** en cuenta  la mayoría de los errores de creación de cuentas están causados por problemas de archivos de datos, como información que falta, direcciones de correo electrónico con formato incorrecto o duplicado o demasiados registros en el archivo.</span><span class="sxs-lookup"><span data-stu-id="56f68-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

7.  <span data-ttu-id="56f68-146">Una vez que el centro de Partners valida el archivo, seleccione la **Ubicación** geográfica para los nuevos usuarios.</span><span class="sxs-lookup"><span data-stu-id="56f68-146">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="56f68-147">Selecciona **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="56f68-147">Select **Save**.</span></span>
9.  <span data-ttu-id="56f68-148">Descarga la información de la contraseña temporal para los usuarios.</span><span class="sxs-lookup"><span data-stu-id="56f68-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="56f68-149">**IMPORTANTE:** Asegúrate de descargar el archivo con las contraseñas temporales ahora, ya no podrás hacerlo más adelante.</span><span class="sxs-lookup"><span data-stu-id="56f68-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="56f68-150">Los nuevos usuarios deben iniciar sesión en su nueva cuenta con las contraseñas temporales correspondientes a sus nuevas cuentas.</span><span class="sxs-lookup"><span data-stu-id="56f68-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="56f68-151">Los nuevos usuarios reciben asignación automática de permisos de **Puede usar licencias y servicios**.</span><span class="sxs-lookup"><span data-stu-id="56f68-151">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



