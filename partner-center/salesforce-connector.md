---
title: El conector de venta conjunta para el centro de Partners de Salesforce CRM
ms.topic: article
ms.date: 05/22/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Usar el conector de CRM de Salesforce, obtener referencias de Microsoft
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: LauraBrenner
ms.author: labrenne
keywords: ''
ms.localizationpriority: medium
ms.openlocfilehash: ad39bdde92611066d0dd0c56d8b9133f4d9dcaa9
ms.sourcegitcommit: 97f1ff7386562cbb945bdfbcf15c85bc8303cac2
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/25/2020
ms.locfileid: "83825702"
---
# <a name="co-sell-connector-for-salesforce-crm---overview"></a>Conector de venta conjunta para Salesforce CRM: información general

### <a name="appropriate-roles"></a>Roles adecuados

- Administrador de referencias
- Administrador del sistema o Personalizador del sistema en CRM

El conector de la venta conjunta del centro de Partners permite que los vendedores covendan con Microsoft desde los sistemas CRM. No tendrán que estar capacitados para utilizar el centro de partners para administrar las ofertas de venta conjunta. Mediante el uso de conectores de venta conjunta, podrá crear una nueva referencia de venta conjunta para invitar a un vendedor de Microsoft, recibir referencias del vendedor de Microsoft, aceptar o rechazar las referencias, modificar los datos de los acuerdos, como el valor del negocio, la fecha de cierre, etc., así como recibir las actualizaciones de los vendedores de Microsoft en relación con la venta conjunta. Puede hacer todo esto mientras trabaja en el CRM de su elección en lugar de hacerlo en el centro de Partners. 

La solución se basa en la solución Microsoft Power Automate y usa las API del centro de Partners de Microsoft.


## <a name="before-you-install---pre-requisites"></a>Antes de instalar: requisitos previos

|**Temas**   |**Detalles**   |**Vínculos**   |
|--------------|--------------------|------|
|IDENTIFICADOR de Microsoft Partner Network |Necesita un ID. de MPN válido|Para unirse a [MPN](https://partner.microsoft.com/)|
|Venta conjunta lista|La solución de IP/servicios debe estar lista para su venta conjunta.|[Venda con Microsoft](https://partner.microsoft.com/membership/sell-with-microsoft)| 
|Cuenta del Centro de partners|El identificador de MPN asociado al inquilino del centro de Partners debe ser el mismo que el identificador de MPN asociado a la solución de venta conjunta. Compruebe que puede ver las referencias de venta conjunta en el portal del centro de Partners antes de implementar los conectores.|[Administración de la cuenta](create-user-accounts-and-set-permissions.md)|
|Roles de usuario del Centro de partners|El empleado que va a instalar y usar los conectores debe ser un administrador de referencias.|[Asignar roles y permisos de usuarios](create-user-accounts-and-set-permissions.md)|
|CRM de Salesforce|El rol de usuario CRM es administrador del sistema o Personalizador del sistema|[Asignación de roles en Dynamics 365](https://docs.microsoft.com/dynamics365/customerengagement/on-premises/customize/privileges-required-customization)|
|Cuenta de flujo de automatización de energía|Una cuenta activa de [Power Automatic](https://flow.microsoft.com) para el administrador del sistema CRM o el personalizador del sistema. Dicho usuario debe iniciar sesión en [Power automatizate](https://flow.microsoft.com) al menos una vez antes de la instalación.|

## <a name="install-partner-center-referrals-synchronization-for-salesforce-crm"></a>Instalación de la sincronización de referencias del centro de partners para Salesforce CRM

1. Vaya a [Power Automatic](https://flow.microsoft.com) y seleccione **entornos** en la esquina superior derecha. Se mostrarán las instancias de CRM disponibles.

2. Seleccione la instancia de CRM correspondiente en la lista desplegable de la esquina superior derecha. 

3. Seleccione **soluciones** en la barra de navegación izquierda.

4. Haga clic en el vínculo **abrir AppSource** en el menú superior.

![Abrir AppSource](images/cosellconnectors/openappsource.png)

5. Busque **conectores de referencias del centro de partners para Salesforce** en la pantalla emergente.  

6. Haga clic en el botón **obtener ahora** y **continúe**. 

7. Se abrirá la página en la que puede seleccionar el entorno de CRM (Dynamics 365) para instalar la aplicación.  Acepte los términos y condiciones. 

8. A continuación, se le dirigirá a la página **administrar soluciones** .  Vaya a "referencias del centro de Partners" con los botones de flecha de la parte inferior de la página. La **instalación programada** debe aparecer junto a la solución de referencias del centro de Partners. La instalación tardará 10-15 minutos. 

9. Una vez completada la instalación, vuelva a [Power Automatic](https://flow.microsoft.com) y seleccione **soluciones** en el área de navegación izquierda. Observe que la **sincronización de referencias del centro de partners para Salesforce** está disponible en la lista de soluciones.

10. Seleccione la **sincronización de referencias del centro de partners para Dynamics 365**. Están disponibles los siguientes flujos y entidades:

![CRMS disponibles](images/cosellconnectors/dynamics-available-crms.png)

## <a name="best-practice-test-before-you-go-live"></a>Procedimiento recomendado: prueba antes de la marcha

Antes de instalar, configurar y personalizar la solución Power Automate en el entorno de producción, asegúrese de probar la solución en una instancia de CRM provisional.

- Instale la solución Microsoft Power Automate en un entorno de ensayo o una instancia de CRM.
- Realice una copia de la solución y realice la configuración y las personalizaciones de flujo de automatización en el entorno de ensayo.
- Pruebe la solución en una instancia de ensayo o CRM. 
- En caso de éxito, importe como solución administrada a la instancia de producción. 

## <a name="configure-the-solution"></a>Configuración de la solución

1. Una vez que haya instalado la solución en la instancia de CRM, vuelva a [Power Automatic](https://flow.microsoft.com/).

2. En la lista desplegable de **entornos** de la esquina superior derecha, seleccione la instancia de CRM en la que instaló la solución Power Automatic.

3. Tendrá que crear conexiones que asocien las tres cuentas de usuario: 

- Usuario del centro de Partners con credenciales de administrador de referencias 
- Eventos del Centro de partners
- Administrador de CRM con la potencia que automatiza los flujos en la solución. 

    a. Seleccione **conexiones** en la barra de navegación izquierda y seleccione la solución "referencias del centro de Partners" en la lista.
    b. Cree una conexión haciendo clic en **crear una conexión**. 

    ![Crear conexión](images/cosellconnectors/createconnection.png)

    c. Busque **referencias del centro de Partners (versión preliminar)** en la barra de búsqueda de la esquina superior derecha.
    d. Cree una conexión para el usuario del centro de Partners con el rol de credenciales de administrador de referencias. e:.. A continuación, cree una conexión de eventos del centro de partners para el usuario del centro de Partners con las credenciales de administrador de referencias. formato. Cree una conexión para Common Data Service (entorno actual) para el usuario administrador de CRM.

4. Para asociar los flujos de alimentación automatizada con las conexiones, edite cada uno de los flujos de Power Automatic para conectarse a Common Data Service y a las referencias del centro de Partners. Guarde los cambios.

5. **Encienda** los flujos automatizar energía.

## <a name="next-steps"></a>Pasos siguientes

- [Uso de webhooks para obtener eventos de cambio de recursos](referral-connector-webhooks.md)

- [¿Más información sobre la plataforma Microsoft Power Automate?](https://docs.microsoft.com/power-automate/)

- [Administrar los clientes potenciales](manage-leads.md)

- [Administrar las oportunidades de venta conjunta](manage-co-sell-opportunities.md)
