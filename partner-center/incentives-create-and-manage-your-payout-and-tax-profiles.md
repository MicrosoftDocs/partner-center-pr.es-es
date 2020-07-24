---
title: Crear y administrar perfiles de pago y impuestos en el Centro de partners
ms.topic: article
ms.date: 06/29/2020
description: Antes de que pueda pagar por su trabajo de incentivos, debe crear los perfiles de pago y fiscal.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: mseamons
ms.author: mseamons
ms.localizationpriority: medium
ms.openlocfilehash: ed8820065c8c009e64419e58fa11758a27f95d7e
ms.sourcegitcommit: c4f2561fb7f224554c31e3af491de4ad65644158
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/23/2020
ms.locfileid: "87114091"
---
# <a name="payout-and-tax-profiles-in-partner-center"></a>Perfiles fiscales y de pago en el centro de Partners

Se aplica a:

- Centro de partners

Antes de que pueda recibir el pago de sus programas de incentivos para una ubicación de MPN determinada, debe completar la inscripción; para ello, asocie un perfil de fiscal y de pago válido al programa y la ubicación MPN. Microsoft usará este perfil de pago e impuestos para emitir los pagos. Es posible que se le permita usar la transferencia electrónica bancaria o una nota de crédito para el pago, en función de las reglas del programa de incentivos. 

Roles adecuados:

- Administrador de incentivos
- Administrador de facturación
- Administrador global

## <a name="create-and-manage-payout-and-tax-profiles-in-partner-center"></a>Crear y administrar perfiles de pago y impuestos en el Centro de partners

Las secciones siguientes le guiarán a través del proceso de creación y administración de perfiles de pago y impuestos en el centro de Partners.

>[!IMPORTANT]
>Debe ser administrador de incentivos para crear o administrar perfiles de pago en el centro de Partners. Los roles de incentivos deben asignarse a cada ubicación de MPN en cada programa de incentivos. Para obtener más información acerca de cómo agregar administradores de incentivos en el centro de Partners, consulte [adición de usuarios de incentivos o administradores en el centro de Partners](https://support.microsoft.com/help/3011450/how-to-add-incentive-users-or-admins-in-partner-center).

## <a name="access-the-payout-and-tax-section-in-partner-center"></a>Acceder a la sección de impuestos y pago en el centro de Partners

1. Inicie sesión en el centro de partners mediante su cuenta de AAD (cuenta de la compañía) o la dirección de correo electrónico adecuada si se asignó alguna. 

   - Se pueden registrar varios dominios en una cuenta de AAD. Póngase en contacto con el administrador global para determinar qué dominios están asociados.
   - Si solo puede iniciar sesión con el **@onmicrosoft.com** dominio, póngase en contacto con el administrador de la cuenta para agregar dominios adicionales a la cuenta de AAD.
   - Si se le pide que seleccione una cuenta **profesional o educativa** o una cuenta **personal**, seleccione **cuenta profesional o educativa**.

2. Seleccione el icono de engranaje para abrir el menú de **configuración** y, a continuación, seleccione **configuración de socio comercial**.

3. En el menú configuración de la **cuenta** , seleccione **pago e impuestos**. 

## <a name="assign-payout-and-tax-profiles-to-individual-programs"></a>Asignación de perfiles de pago y impuestos a programas individuales

1. En el centro de Partners, seleccione el icono de engranaje para abrir el menú de **configuración** . 

2. Seleccione **configuración de socio comercial**, expanda la **sección pago y impuestos**y, a continuación, seleccione **asignación de perfil fiscal y de pago**. 
   
   Se mostrará una lista de los programas. Seleccione la flecha situada junto a un programa para ver los detalles del perfil. 

3. En el menú desplegable **Perfil de impuestos** , seleccione el perfil de impuestos que desee o seleccione la opción para crear un nuevo perfil. Al seleccionar la opción para crear un nuevo perfil, se le redirigirá adecuadamente.  Seleccione continuar en la ventana emergente. A continuación se proporciona el proceso para crear un nuevo perfil de impuestos.

4. Seleccione el **método de pago**.

   - Si seleccionó **transferencia bancaria electrónica** como método de pago, en la lista desplegable Perfil de pago, seleccione el perfil de pago que desee o seleccione la opción para crear un nuevo perfil. Al seleccionar la opción para crear un nuevo perfil, se le redirigirá adecuadamente.  Seleccione continuar en la ventana emergente. A continuación se proporciona el proceso para crear un nuevo perfil de pago.

   - Si ha seleccionado **Nota de crédito** como método de pago, complete la comprobación para confirmar que el número de SAP al que se hace referencia pertenece a su organización.

    >[!NOTE]
    >Si hay varias entidades comerciales de Microsoft en la lista, debe seleccionar un perfil de pago para cada entidad.

    >[!NOTE]
    >La disponibilidad del método de pago depende de las reglas del programa de incentivos.
    
5. Seleccione la **moneda**.

6. Cuando haya completado todos los campos de pago, seleccione **submit (enviar**).

## <a name="create-your-bank-profile"></a>Crear el perfil de Banco

Los perfiles de banco se crean en el nivel de organización, lo que permite asignar el mismo perfil de banco en varios programas de ID. de MPN y programas de incentivos dentro de una organización. Puede haber excepciones al aplicar el perfil de banca a distintos países, ya que se pueden aplicar diferentes reglas de banca y impuestos.

>[!NOTE]
>En las páginas siguientes, los campos con un asterisco son obligatorios. Si no sabe qué es un campo, seleccione el icono de información. 

1. En la página **detalles** , complete los siguientes campos: **nombre del perfil:** escriba un nombre único para identificar este perfil de pago.
    **Ubicación de la cuenta bancaria:** País en el que se encuentra el Banco de su empresa.
    **Método de pago:** El método de pago preferido es para el centro de Partners es transferencia bancaria electrónica.

2. Seleccione **Next** (Siguiente).

3. En la página **cuenta bancaria** , escriba su información. Los campos que se muestran en esta página variarán en función del país. 

4. Seleccione **Next** (Siguiente).

5. En la página **beneficiario** , escriba la información adecuada. El beneficiario es la persona de su empresa en la que el Banco se pondrá en contacto si necesita discutir su cuenta.

6. Una vez completados los campos, seleccione **Finalizar**y, a continuación, seleccione **confirmar** para crear el perfil de banco.

Se le redirigirá a la página de **perfiles de pago y impuestos** . El estado del nuevo perfil reflejará la **validación de Microsoft pendiente** hasta que se haya completado la validación. Esto puede tardar hasta 48 horas. Una vez completada la validación, el estado del perfil reflejará **aprobado** o **acción requerida**. Si se **requiere una acción**, repita los pasos anteriores y proporcione la información necesaria. 

## <a name="create-your-tax-profile"></a>Crear el perfil de impuestos

Utilice el procedimiento siguiente para proporcionar a Microsoft la información fiscal necesaria para su organización. Las páginas de esta sección son dinámicas y variarán según el país o la región. Si necesita ayuda para identificar la información fiscal correcta, póngase en contacto con los orígenes de gobierno correspondientes de su país.

En el caso de las empresas asociadas de la América, si necesita información sobre la finalización de los formularios W8 o W9, las siguientes direcciones le llevan al sitio de IRS:

- [http://www.irs.gov/pub/irs-pdf/iw8.pdf](http://www.irs.gov/pub/irs-pdf/iw8.pdf)
- [http://www.irs.gov/pub/irs-pdf/iw9.pdf](http://www.irs.gov/pub/irs-pdf/iw9.pdf)

>[!IMPORTANT]
> Especifique solo los detalles de su empresa. No escriba nunca detalles personales.

1. En la página **Perfil de negocio** , complete los campos obligatorios y, a continuación, seleccione **siguiente**. 

2. En la página **instalación** , seleccione la opción que se aplica a su compañía.

   - Seleccione la opción de la izquierda si su empresa se incorpora solo en el Estados Unidos, o si este perfil es para un individuo. 
   - Seleccione la opción de la derecha si su empresa se incorpora fuera del Estados Unidos y, a continuación, seleccione su país o región en la lista.

3. Seleccione **Next** (Siguiente). 

4. En la página **Estado de impuestos** , escriba la información necesaria y, a continuación, seleccione **siguiente**. Los campos de esta página variarán en función del país. los detalles. 

5. En la página de **documentación adicional** , los campos obligatorios y seleccione **siguiente**. 

6. Seleccione **examinar** para cargar los documentos requeridos por su país o región. Cuando se muestre el nombre del documento, seleccione **cargar**. 

7. Si necesita quitar el documento, seleccione **quitar**.

8. Para guardar y continuar, seleccione **Finalizar**.

9. Seleccione **confirmar** en el mensaje emergente. Volverá a la página de configuración de **pagos y impuestos** .

## <a name="payout-and-tax-profile-faqs"></a>Preguntas más frecuentes sobre el pago y el perfil fiscal

### <a name="why-do-i-need-to-provide-my-payout-andor-tax-details"></a>¿Por qué es necesario proporcionar los detalles de pago o de impuestos?

Con el fin de recibir pagos de los programas de incentivos de Microsoft, debe completar la inscripción proporcionando detalles de pago e impuestos válidos. Una inscripción se considera completa solo cuando Microsoft valida el pago y el perfil fiscal que proporcione.

### <a name="how-do-i-know-that-i-need-to-provideupdate-my-payout-andor-tax-details"></a>Cómo sabe que necesito proporcionar o actualizar los datos de pago o de impuestos?

Todos los asociados que se inscriben en un nuevo programa de incentivos deben proporcionar detalles de pago e impuestos válidos para completar la inscripción.

Es posible que también tenga que proporcionar información actualizada si cambian las reglas para el programa de incentivos, o si los aspectos del perfil expiran o se vuelven obsoletos. Si esto ocurre, la página de información general mostrará el estado **acción requerida-actualizar banco o Perfil de impuesto**.

### <a name="how-do-i-provide-update-my-payout-and-or-tax-details"></a>Cómo proporciono o actualizo mis datos de pago o fiscales?

Para obtener información detallada sobre cómo actualizar los detalles de pago y de impuestos en el centro de Partners, consulte [creación y administración de perfiles bancarios y de impuestos en el centro de Partners](https://support.microsoft.com/help/4524534/how-to-create-and-manage-bank-and-tax-profiles-in-partner-center) .

### <a name="why-dont-i-see-my-enrollments-when-i-go-to-assign-my-payout-and-tax-profile"></a>¿Por qué no veo mis inscripciones cuando me quiero asignar mi perfil de pago y fiscal?

Solo los administradores de incentivos de la ubicación de MPN pueden crear o administrar perfiles fiscales y de pago. Podría ser que no tuviera los permisos adecuados o que haya iniciado sesión con una cuenta que no tenga estos permisos. Póngase en contacto con el administrador de la organización para administrar los permisos bancarios y fiscales.

### <a name="where-can-i-see-the-payout-and-tax-profiles-for-my-organization-that-i-can-use"></a>¿Dónde puedo ver los perfiles fiscales y de pago de mi organización que puedo usar?

Use el procedimiento siguiente para ver los perfiles de pago y impuestos:

1. Inicie sesión en Centro de partners.

2. Seleccione el icono de engranaje para abrir el menú **Configuración**.

3. Seleccione **configuración de socio comercial**.

4. En **Configuración de cuenta**, seleccione **Pago e impuestos** y, a continuación, seleccione **Perfiles fiscales y de pago**. Verá todos los perfiles fiscales y de pago existentes junto con el estado y la capacidad de edición.

### <a name="my-organization-is-participating-in-multiple-incentive-programs-do-i-need-to-provide-my-payment-and-tax-profile-multiple-times"></a>Mi organización participa en varios programas de incentivos. ¿Es necesario proporcionar el perfil de pago y de impuestos varias veces?

Con los perfiles de pago, depende de usted. Los perfiles de pago se crean en el nivel de la organización, lo que permite asignar el mismo perfil bancario en varios programas de identificador de MPN y programas de incentivos dentro de una organización. En la mayoría de los casos, puede volver a usar un perfil existente o crear uno nuevo.

No obstante, puede haber excepciones al aplicar el perfil bancario a distintos países o regiones, ya que se pueden aplicar reglas bancarias o fiscales.

Los perfiles fiscales creados para una ubicación de MPN se reutilizan y se rellenan automáticamente cuando la misma ubicación de MPN participa en otro programa de incentivos. Pero puede haber excepciones. Por ejemplo, las reglas de pago de un nuevo programa de incentivos pueden requerir detalles adicionales para el perfil fiscal.  

### <a name="i-am-only-able-to-log-in-with-my-onmicrosoftcom-domain-what-should-i-do"></a>Solo puedo iniciar sesión con mi @onmicrosoft.com dominio. ¿Cuál debo hacer?

Póngase en contacto con el administrador de la cuenta para agregar dominios adicionales a la cuenta de AAD.
