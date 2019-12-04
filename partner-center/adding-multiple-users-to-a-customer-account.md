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
ms.openlocfilehash: 2195d23074a3e7c397b5f557fd3bed9ec0cc518e
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721989"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="b2b20-104">Agregar varios usuarios a una cuenta de cliente</span><span class="sxs-lookup"><span data-stu-id="b2b20-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="b2b20-105">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="b2b20-105">**Applies to**</span></span>

- <span data-ttu-id="b2b20-106">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="b2b20-106">Partner Center</span></span>

<span data-ttu-id="b2b20-107">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="b2b20-107">**Appropriate roles**</span></span>

- <span data-ttu-id="b2b20-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="b2b20-108">Global admin</span></span>

<span data-ttu-id="b2b20-109">Puede agregar varios usuarios a la cuenta de un cliente a la vez, cargando un archivo de datos en el formato de archivo de valores separados por comas (. csv) al centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="b2b20-109">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="b2b20-110">Puede descargar un archivo de datos de ejemplo del centro de Partners y editarlo para su uso, o puede crear un nuevo archivo de datos con el modelo de datos definido a continuación.</span><span class="sxs-lookup"><span data-stu-id="b2b20-110">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="b2b20-111">Requisitos del archivo de datos</span><span class="sxs-lookup"><span data-stu-id="b2b20-111">Data file requirements</span></span>

<span data-ttu-id="b2b20-112">Para agregar varios usuarios a la cuenta de un cliente mediante el proceso de carga masiva, debe cumplir los siguientes requisitos:</span><span class="sxs-lookup"><span data-stu-id="b2b20-112">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="b2b20-113">Debes tener permisos de administrador global para la cuenta de cliente.</span><span class="sxs-lookup"><span data-stu-id="b2b20-113">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="b2b20-114">Cada usuario debe tener una dirección de correo electrónico exclusiva, anexa a los dominios de correo electrónico del cliente.</span><span class="sxs-lookup"><span data-stu-id="b2b20-114">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="b2b20-115">Puedes subir hasta 100 registros a la vez.</span><span class="sxs-lookup"><span data-stu-id="b2b20-115">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="b2b20-116">Si es necesario agregar más de 100 usuarios, crea y sube archivos de datos adicionales.</span><span class="sxs-lookup"><span data-stu-id="b2b20-116">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="b2b20-117">Todos los usuarios deben estar en la misma **ubicación** geográfica.</span><span class="sxs-lookup"><span data-stu-id="b2b20-117">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="b2b20-118">Escribe solo los datos que se describen a continuación.</span><span class="sxs-lookup"><span data-stu-id="b2b20-118">Enter only the data described below.</span></span> <span data-ttu-id="b2b20-119">Unos datos extraños hará que la carga sufra un error.</span><span class="sxs-lookup"><span data-stu-id="b2b20-119">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="b2b20-120">Escribe los siguientes datos en el archivo de datos:</span><span class="sxs-lookup"><span data-stu-id="b2b20-120">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="b2b20-121">**Nombre de columna**</span><span class="sxs-lookup"><span data-stu-id="b2b20-121">**Column name**</span></span> | <span data-ttu-id="b2b20-122">**Descripción**</span><span class="sxs-lookup"><span data-stu-id="b2b20-122">**Description**</span></span>                                                              | <span data-ttu-id="b2b20-123">**Única**</span><span class="sxs-lookup"><span data-stu-id="b2b20-123">**Limitation**</span></span>                             |
| <span data-ttu-id="b2b20-124">Nombre</span><span class="sxs-lookup"><span data-stu-id="b2b20-124">First name</span></span>      | <span data-ttu-id="b2b20-125">Nombre del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="b2b20-125">User's first name (optional field)</span></span>                                           | <span data-ttu-id="b2b20-126">Límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="b2b20-126">50-character limit</span></span>                         |
| <span data-ttu-id="b2b20-127">Apellidos</span><span class="sxs-lookup"><span data-stu-id="b2b20-127">Last name</span></span>       | <span data-ttu-id="b2b20-128">Los apellidos del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="b2b20-128">User's last name (optional field)</span></span>                                            | <span data-ttu-id="b2b20-129">Límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="b2b20-129">50-character limit</span></span>                         |
| <span data-ttu-id="b2b20-130">Nombre para mostrar</span><span class="sxs-lookup"><span data-stu-id="b2b20-130">Display name</span></span>    | <span data-ttu-id="b2b20-131">Nombre mostrado en el centro de Partners (campo obligatorio)</span><span class="sxs-lookup"><span data-stu-id="b2b20-131">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="b2b20-132">Límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="b2b20-132">50-character limit</span></span>                         |
| <span data-ttu-id="b2b20-133">Correo electrónico</span><span class="sxs-lookup"><span data-stu-id="b2b20-133">Email</span></span>           | <span data-ttu-id="b2b20-134">Dirección de correo electrónico empresarial del usuario en la empresa del cliente (campo obligatorio)</span><span class="sxs-lookup"><span data-stu-id="b2b20-134">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="b2b20-135">Cada usuario debe tener una dirección de correo electrónico exclusiva.</span><span class="sxs-lookup"><span data-stu-id="b2b20-135">Each user must have a unique email address</span></span> |
| <span data-ttu-id="b2b20-136">Actualización de estado</span><span class="sxs-lookup"><span data-stu-id="b2b20-136">Status update</span></span>   | <span data-ttu-id="b2b20-137">Se usa para indicar si el nuevo registro de usuario se ha creado correctamente o no.</span><span class="sxs-lookup"><span data-stu-id="b2b20-137">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="b2b20-138">\*\*deje\*vacío \*</span><span class="sxs-lookup"><span data-stu-id="b2b20-138">\*\*Leave empty\*\*</span></span>                        |

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="b2b20-139">Para crear varias cuentas de usuario</span><span class="sxs-lookup"><span data-stu-id="b2b20-139">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="b2b20-140">Crea un archivo de datos de valores separados por comas (.csv) con los datos que se han descrito anteriormente.</span><span class="sxs-lookup"><span data-stu-id="b2b20-140">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="b2b20-141">Guarda el archivo para que puedas acceder a él en un paso posterior.</span><span class="sxs-lookup"><span data-stu-id="b2b20-141">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="b2b20-142">Inicie sesión en el [Panel](https://partner.microsoft.com/dashboard)del centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="b2b20-142">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="b2b20-143">Desde el menú del Centro de partners, selecciona **Clientes** y, a continuación, elige un cliente de la lista.</span><span class="sxs-lookup"><span data-stu-id="b2b20-143">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="b2b20-144">Seleccione la pestaña **usuarios y licencias** del cliente y, a continuación, seleccione **cargar usuarios**.</span><span class="sxs-lookup"><span data-stu-id="b2b20-144">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="b2b20-145">En **Subir información de usuarios**, selecciona **Examinar**.</span><span class="sxs-lookup"><span data-stu-id="b2b20-145">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="b2b20-146">En el selector de archivos, selecciona el archivo de datos y, a continuación, selecciona **Abrir**.</span><span class="sxs-lookup"><span data-stu-id="b2b20-146">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="b2b20-147">Selecciona **Validar**.</span><span class="sxs-lookup"><span data-stu-id="b2b20-147">Select **Validate**.</span></span>

    <span data-ttu-id="b2b20-148">**Tenga** en cuenta  la mayoría de los errores de creación de cuentas están causados por problemas de archivos de datos, como información que falta, direcciones de correo electrónico con formato incorrecto o duplicado o demasiados registros en el archivo.</span><span class="sxs-lookup"><span data-stu-id="b2b20-148">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="b2b20-149">Una vez que el centro de Partners valida el archivo, seleccione la **Ubicación** geográfica para los nuevos usuarios.</span><span class="sxs-lookup"><span data-stu-id="b2b20-149">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="b2b20-150">Selecciona **Guardar**.</span><span class="sxs-lookup"><span data-stu-id="b2b20-150">Select **Save**.</span></span>
10. <span data-ttu-id="b2b20-151">Descarga la información de la contraseña temporal para los usuarios.</span><span class="sxs-lookup"><span data-stu-id="b2b20-151">Download the temporary password information for the users.</span></span>

<span data-ttu-id="b2b20-152">**IMPORTANTE:** Asegúrate de descargar el archivo con las contraseñas temporales ahora, ya no podrás hacerlo más adelante.</span><span class="sxs-lookup"><span data-stu-id="b2b20-152">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="b2b20-153">Los nuevos usuarios deben iniciar sesión en su nueva cuenta con las contraseñas temporales correspondientes a sus nuevas cuentas.</span><span class="sxs-lookup"><span data-stu-id="b2b20-153">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="b2b20-154">Los nuevos usuarios reciben asignación automática de permisos de **Puede usar licencias y servicios**.</span><span class="sxs-lookup"><span data-stu-id="b2b20-154">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



