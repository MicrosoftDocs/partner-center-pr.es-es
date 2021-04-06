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
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441428"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="1d4c0-103">Agregar varios usuarios a una cuenta de cliente mediante la creación de un archivo. csv</span><span class="sxs-lookup"><span data-stu-id="1d4c0-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="1d4c0-104">**Roles adecuados**</span><span class="sxs-lookup"><span data-stu-id="1d4c0-104">**Appropriate roles**</span></span>

- <span data-ttu-id="1d4c0-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="1d4c0-105">Global admin</span></span>

<span data-ttu-id="1d4c0-106">Agregue varios usuarios a la cuenta de un cliente a la vez, cargando un archivo de datos en el formato de archivo de valores separados por comas (. csv) en el centro de Partners.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="1d4c0-107">Puede descargar un archivo de datos de ejemplo del centro de Partners y editarlo para su uso, o puede crear un nuevo archivo de datos con el modelo de datos definido a continuación.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-107">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="1d4c0-108">Requisitos del archivo de datos:</span><span class="sxs-lookup"><span data-stu-id="1d4c0-108">Data file requirements</span></span>

<span data-ttu-id="1d4c0-109">Para agregar varios usuarios a la cuenta de un cliente mediante el proceso de carga masiva, debe cumplir los siguientes requisitos:</span><span class="sxs-lookup"><span data-stu-id="1d4c0-109">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="1d4c0-110">Debes tener permisos de administrador global para la cuenta de cliente.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-110">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="1d4c0-111">Cada usuario debe tener una dirección de correo electrónico exclusiva, anexa a los dominios de correo electrónico del cliente.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-111">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="1d4c0-112">Puedes subir hasta 100 registros a la vez.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-112">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="1d4c0-113">Si es necesario agregar más de 100 usuarios, crea y sube archivos de datos adicionales.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-113">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="1d4c0-114">Todos los usuarios deben estar en la misma **ubicación** geográfica.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-114">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="1d4c0-115">Escribe solo los datos que se describen a continuación.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-115">Enter only the data described below.</span></span> <span data-ttu-id="1d4c0-116">Unos datos extraños hará que la carga sufra un error.</span><span class="sxs-lookup"><span data-stu-id="1d4c0-116">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="1d4c0-117">Escribe los siguientes datos en el archivo de datos:</span><span class="sxs-lookup"><span data-stu-id="1d4c0-117">Enter the following data in the data file:</span></span>

| <span data-ttu-id="1d4c0-118">**Nombre de la columna**</span><span class="sxs-lookup"><span data-stu-id="1d4c0-118">**Column name**</span></span> | <span data-ttu-id="1d4c0-119">**Descripción**</span><span class="sxs-lookup"><span data-stu-id="1d4c0-119">**Description**</span></span>  | <span data-ttu-id="1d4c0-120">**Limitación**</span><span class="sxs-lookup"><span data-stu-id="1d4c0-120">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="1d4c0-121">Nombre</span><span class="sxs-lookup"><span data-stu-id="1d4c0-121">First name</span></span>  | <span data-ttu-id="1d4c0-122">Nombre del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="1d4c0-122">User's first name (optional field)</span></span>  | <span data-ttu-id="1d4c0-123">límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="1d4c0-123">50-character limit</span></span>  |
| <span data-ttu-id="1d4c0-124">Apellido</span><span class="sxs-lookup"><span data-stu-id="1d4c0-124">Last name</span></span>  | <span data-ttu-id="1d4c0-125">Los apellidos del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="1d4c0-125">User's last name (optional field)</span></span>  | <span data-ttu-id="1d4c0-126">límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="1d4c0-126">50-character limit</span></span>  |
| <span data-ttu-id="1d4c0-127">Nombre para mostrar</span><span class="sxs-lookup"><span data-stu-id="1d4c0-127">Display name</span></span>    | <span data-ttu-id="1d4c0-128">Nombre mostrado en el centro de Partners (campo obligatorio)</span><span class="sxs-lookup"><span data-stu-id="1d4c0-128">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="1d4c0-129">límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="1d4c0-129">50-character limit</span></span>                         |
| <span data-ttu-id="1d4c0-130">Email</span><span class="sxs-lookup"><span data-stu-id="1d4c0-130">Email</span></span>   | <span data-ttu-id="1d4c0-131">Dirección de correo electrónico empresarial del usuario en la empresa del cliente (campo obligatorio)</span><span class="sxs-lookup"><span data-stu-id="1d4c0-131">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="1d4c0-132">Cada usuario debe tener una dirección de correo electrónico única</span><span class="sxs-lookup"><span data-stu-id="1d4c0-132">Each user must have a unique email address</span></span> |
| <span data-ttu-id="1d4c0-133">Actualización del estado</span><span class="sxs-lookup"><span data-stu-id="1d4c0-133">Status update</span></span>   | <span data-ttu-id="1d4c0-134">Se usa para indicar si el nuevo registro de usuario se creó correctamente</span><span class="sxs-lookup"><span data-stu-id="1d4c0-134">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="1d4c0-135">\*\*Dejar vacío\*\*</span><span class="sxs-lookup"><span data-stu-id="1d4c0-135">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="1d4c0-136">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="1d4c0-136">Next steps</span></span>

- [<span data-ttu-id="1d4c0-137">Procedimiento para agregar varios usuarios para un cliente</span><span class="sxs-lookup"><span data-stu-id="1d4c0-137">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)