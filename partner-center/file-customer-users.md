---
title: Campos del archivo. csv para importar varios usuarios para una cuenta de cliente
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para agregar varios usuarios a una cuenta de cliente, cree un archivo de valores separados por comas (. csv) con los campos correspondientes.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 08/03/2020
ms.locfileid: "87528189"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="f0edd-103">Agregar varios usuarios a una cuenta de cliente mediante la creación de un archivo. csv</span><span class="sxs-lookup"><span data-stu-id="f0edd-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="f0edd-104">**Se aplica a**</span><span class="sxs-lookup"><span data-stu-id="f0edd-104">**Applies to**</span></span>

- <span data-ttu-id="f0edd-105">Centro de partners</span><span class="sxs-lookup"><span data-stu-id="f0edd-105">Partner Center</span></span>

<span data-ttu-id="f0edd-106">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="f0edd-106">**Appropriate roles**</span></span>

- <span data-ttu-id="f0edd-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="f0edd-107">Global admin</span></span>

<span data-ttu-id="f0edd-108">Agregue varios usuarios a la cuenta de un cliente a la vez, cargando un archivo de datos en el formato de archivo de valores separados por comas (. csv) en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="f0edd-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="f0edd-109">Puede descargar un archivo de datos de ejemplo del centro de Partners y editarlo para su uso, o puede crear un nuevo archivo de datos con el modelo de datos definido a continuación.</span><span class="sxs-lookup"><span data-stu-id="f0edd-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="f0edd-110">Requisitos del archivo de datos:</span><span class="sxs-lookup"><span data-stu-id="f0edd-110">Data file requirements</span></span>

<span data-ttu-id="f0edd-111">Para agregar varios usuarios a la cuenta de un cliente mediante el proceso de carga masiva, debe cumplir los siguientes requisitos:</span><span class="sxs-lookup"><span data-stu-id="f0edd-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="f0edd-112">Debes tener permisos de administrador global para la cuenta de cliente.</span><span class="sxs-lookup"><span data-stu-id="f0edd-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="f0edd-113">Cada usuario debe tener una dirección de correo electrónico exclusiva, anexa a los dominios de correo electrónico del cliente.</span><span class="sxs-lookup"><span data-stu-id="f0edd-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="f0edd-114">Puedes subir hasta 100 registros a la vez.</span><span class="sxs-lookup"><span data-stu-id="f0edd-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="f0edd-115">Si es necesario agregar más de 100 usuarios, crea y sube archivos de datos adicionales.</span><span class="sxs-lookup"><span data-stu-id="f0edd-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="f0edd-116">Todos los usuarios deben estar en la misma **ubicación** geográfica.</span><span class="sxs-lookup"><span data-stu-id="f0edd-116">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="f0edd-117">Escribe solo los datos que se describen a continuación.</span><span class="sxs-lookup"><span data-stu-id="f0edd-117">Enter only the data described below.</span></span> <span data-ttu-id="f0edd-118">Unos datos extraños hará que la carga sufra un error.</span><span class="sxs-lookup"><span data-stu-id="f0edd-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="f0edd-119">Escribe los siguientes datos en el archivo de datos:</span><span class="sxs-lookup"><span data-stu-id="f0edd-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="f0edd-120">**Nombre de la columna**</span><span class="sxs-lookup"><span data-stu-id="f0edd-120">**Column name**</span></span> | <span data-ttu-id="f0edd-121">**Descripción**</span><span class="sxs-lookup"><span data-stu-id="f0edd-121">**Description**</span></span>  | <span data-ttu-id="f0edd-122">**Limitación**</span><span class="sxs-lookup"><span data-stu-id="f0edd-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="f0edd-123">Nombre</span><span class="sxs-lookup"><span data-stu-id="f0edd-123">First name</span></span>  | <span data-ttu-id="f0edd-124">Nombre del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="f0edd-124">User's first name (optional field)</span></span>  | <span data-ttu-id="f0edd-125">límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="f0edd-125">50-character limit</span></span>  |
| <span data-ttu-id="f0edd-126">Apellidos</span><span class="sxs-lookup"><span data-stu-id="f0edd-126">Last name</span></span>  | <span data-ttu-id="f0edd-127">Los apellidos del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="f0edd-127">User's last name (optional field)</span></span>  | <span data-ttu-id="f0edd-128">límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="f0edd-128">50-character limit</span></span>  |
| <span data-ttu-id="f0edd-129">Nombre para mostrar</span><span class="sxs-lookup"><span data-stu-id="f0edd-129">Display name</span></span>    | <span data-ttu-id="f0edd-130">Nombre mostrado en el centro de Partners (campo obligatorio)</span><span class="sxs-lookup"><span data-stu-id="f0edd-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="f0edd-131">límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="f0edd-131">50-character limit</span></span>                         |
| <span data-ttu-id="f0edd-132">Correo electrónico</span><span class="sxs-lookup"><span data-stu-id="f0edd-132">Email</span></span>   | <span data-ttu-id="f0edd-133">Dirección de correo electrónico empresarial del usuario en la empresa del cliente (campo obligatorio)</span><span class="sxs-lookup"><span data-stu-id="f0edd-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="f0edd-134">Cada usuario debe tener una dirección de correo electrónico única</span><span class="sxs-lookup"><span data-stu-id="f0edd-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="f0edd-135">Actualización del estado</span><span class="sxs-lookup"><span data-stu-id="f0edd-135">Status update</span></span>   | <span data-ttu-id="f0edd-136">Se usa para indicar si el nuevo registro de usuario se ha creado correctamente o no.</span><span class="sxs-lookup"><span data-stu-id="f0edd-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="f0edd-137">\*\*Dejar vacío\*\*</span><span class="sxs-lookup"><span data-stu-id="f0edd-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="f0edd-138">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="f0edd-138">Next steps</span></span>

- [<span data-ttu-id="f0edd-139">Cómo agregar varios usuarios a un cliente</span><span class="sxs-lookup"><span data-stu-id="f0edd-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)