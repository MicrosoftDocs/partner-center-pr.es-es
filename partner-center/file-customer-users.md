---
title: Campos del archivo .csv para importar varios usuarios para una cuenta de cliente
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para agregar varios usuarios a una cuenta de cliente, cree un archivo de valores separados por comas (.csv) con los campos adecuados.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150988"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="d4d9e-103">Agregar varios usuarios a una cuenta de cliente mediante la creación de un archivo .csv</span><span class="sxs-lookup"><span data-stu-id="d4d9e-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="d4d9e-104">**Roles apropiados**: administrador global</span><span class="sxs-lookup"><span data-stu-id="d4d9e-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="d4d9e-105">Agregue varios usuarios a la cuenta de un cliente a la vez, cargando un archivo de datos con el formato de archivo de valores separados por comas (.csv) en el Centro de partners.</span><span class="sxs-lookup"><span data-stu-id="d4d9e-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="d4d9e-106">Puede descargar un archivo de datos de ejemplo de la Centro de partners y, a continuación, editarlo para su uso, o puede crear un nuevo archivo de datos mediante el modelo de datos definido a continuación.</span><span class="sxs-lookup"><span data-stu-id="d4d9e-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="d4d9e-107">Requisitos del archivo de datos:</span><span class="sxs-lookup"><span data-stu-id="d4d9e-107">Data file requirements</span></span>

<span data-ttu-id="d4d9e-108">Para agregar varios usuarios a la cuenta de un cliente mediante el proceso de carga masiva, deberá cumplir los siguientes requisitos:</span><span class="sxs-lookup"><span data-stu-id="d4d9e-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="d4d9e-109">Debes tener permisos de administrador global para la cuenta de cliente.</span><span class="sxs-lookup"><span data-stu-id="d4d9e-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="d4d9e-110">Cada usuario debe tener una dirección de correo electrónico exclusiva, anexa a los dominios de correo electrónico del cliente.</span><span class="sxs-lookup"><span data-stu-id="d4d9e-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="d4d9e-111">Puedes subir hasta 100 registros a la vez.</span><span class="sxs-lookup"><span data-stu-id="d4d9e-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="d4d9e-112">Si es necesario agregar más de 100 usuarios, crea y sube archivos de datos adicionales.</span><span class="sxs-lookup"><span data-stu-id="d4d9e-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="d4d9e-113">Todos los usuarios deben estar en la misma **ubicación** geográfica.</span><span class="sxs-lookup"><span data-stu-id="d4d9e-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="d4d9e-114">Escribe solo los datos que se describen a continuación.</span><span class="sxs-lookup"><span data-stu-id="d4d9e-114">Enter only the data described below.</span></span> <span data-ttu-id="d4d9e-115">Unos datos extraños hará que la carga sufra un error.</span><span class="sxs-lookup"><span data-stu-id="d4d9e-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="d4d9e-116">Escribe los siguientes datos en el archivo de datos:</span><span class="sxs-lookup"><span data-stu-id="d4d9e-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="d4d9e-117">**Nombre de la columna**</span><span class="sxs-lookup"><span data-stu-id="d4d9e-117">**Column name**</span></span> | <span data-ttu-id="d4d9e-118">**Descripción**</span><span class="sxs-lookup"><span data-stu-id="d4d9e-118">**Description**</span></span>  | <span data-ttu-id="d4d9e-119">**Limitación**</span><span class="sxs-lookup"><span data-stu-id="d4d9e-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="d4d9e-120">Nombre</span><span class="sxs-lookup"><span data-stu-id="d4d9e-120">First name</span></span>  | <span data-ttu-id="d4d9e-121">Nombre del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="d4d9e-121">User's first name (optional field)</span></span>  | <span data-ttu-id="d4d9e-122">límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="d4d9e-122">50-character limit</span></span>  |
| <span data-ttu-id="d4d9e-123">Apellido</span><span class="sxs-lookup"><span data-stu-id="d4d9e-123">Last name</span></span>  | <span data-ttu-id="d4d9e-124">Los apellidos del usuario (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="d4d9e-124">User's last name (optional field)</span></span>  | <span data-ttu-id="d4d9e-125">límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="d4d9e-125">50-character limit</span></span>  |
| <span data-ttu-id="d4d9e-126">Nombre para mostrar</span><span class="sxs-lookup"><span data-stu-id="d4d9e-126">Display name</span></span>    | <span data-ttu-id="d4d9e-127">Nombre que se muestra en la Centro de partners (campo obligatorio)</span><span class="sxs-lookup"><span data-stu-id="d4d9e-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="d4d9e-128">límite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="d4d9e-128">50-character limit</span></span>                         |
| <span data-ttu-id="d4d9e-129">Correo electrónico</span><span class="sxs-lookup"><span data-stu-id="d4d9e-129">Email</span></span>   | <span data-ttu-id="d4d9e-130">Dirección de correo electrónico empresarial del usuario en la empresa del cliente (campo obligatorio)</span><span class="sxs-lookup"><span data-stu-id="d4d9e-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="d4d9e-131">Cada usuario debe tener una dirección de correo electrónico única</span><span class="sxs-lookup"><span data-stu-id="d4d9e-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="d4d9e-132">Actualización del estado</span><span class="sxs-lookup"><span data-stu-id="d4d9e-132">Status update</span></span>   | <span data-ttu-id="d4d9e-133">Se usa para indicar si el nuevo registro de usuario se creó correctamente</span><span class="sxs-lookup"><span data-stu-id="d4d9e-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="d4d9e-134">\*\*Dejar vacío\*\*</span><span class="sxs-lookup"><span data-stu-id="d4d9e-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="d4d9e-135">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="d4d9e-135">Next steps</span></span>

- [<span data-ttu-id="d4d9e-136">Procedimiento para agregar varios usuarios para un cliente</span><span class="sxs-lookup"><span data-stu-id="d4d9e-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)