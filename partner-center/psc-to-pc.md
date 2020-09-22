---
title: Migrar de sales Partner Connect (PSC)
ms.topic: article
ms.date: 08/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Obtenga información acerca de cómo los asociados de Microsoft pueden migrar de Partner Sales Connect (PSC) al centro de Partners y crear o administrar los acuerdos enviados por los vendedores de Microsoft.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: dc131991826a6428d613aa34e2e99c19e3efde05
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/22/2020
ms.locfileid: "90999349"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Guía para la venta conjunta en el centro de Partners (PC) para los asociados que migran desde la conexión de ventas de asociados (PSC)

**Se aplica a**

- Centro de partners

**Roles adecuados**

- Administrador de cuentas
- Administrador de referencias
- Vendedor de sales Partner Connect (PSC)
- Administrador de ventas de asociados (PSC)
- Director de ventas de socio comercial (PSC)

Como sabe, su empresa perderá el acceso a PSC después del 31 de diciembre de 2020. Sin embargo, encontrará todo lo que desea hacer para crear ofertas de venta conjunta, administrar sus negocios y realizar acciones en los acuerdos enviados por los vendedores de Microsoft en el centro de Partners. Sin embargo, habrá diferencias y las siguientes instrucciones le ayudarán a hacer que la transición al centro de Partners sea más suave y directa.

>[!Important]
> Si está aquí porque vio un banner en PSC sobre la migración, está en el lugar correcto. Esta guía no es aplicable a los asociados de evaluación de soluciones (SA) y OEM IOT que administran sus contratos en PSC.

## <a name="before-you-move-things-you-need-to-know"></a>Antes de realizar el traslado, lo que necesita saber

### <a name="if-you-are-psc-admin"></a>Si es administrador de PSC

- Necesita un correo electrónico de trabajo para iniciar sesión en el [centro de Partners](https://partner.microsoft.com/).
- Configure su cuenta con la ayuda del administrador de la [cuenta](permissions-overview.md)del centro de Partners.
- Lea este documento para obtener información sobre cómo vender en el centro de Partners.
- Configure cuentas de usuario en el centro de partners para todos los usuarios de PSC (roles de administrador, administrador de transacciones y vendedor) y asígneles [roles de administrador de referencias](permissions-overview.md).

>[!Important]
> Asegúrese de que el identificador de MPN que se muestra en el banner de PSC está disponible en la lista de ubicaciones de MPN del centro de Partners. Para comprobarlo en el centro de Partners, vaya a "configuración de la cuenta" y "[ubicaciones](manage-locations.md)" en la lista para buscar la lista de todas las MPNs asociadas a la cuenta del centro de Partners.

 :::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Imagen que muestra el banner de PSC en el que los asociados pueden encontrar el ID. de MPN.":::

### <a name="if-you-are-psc-deal-manager-or-seller"></a>Si es un administrador de transacciones de PSC o un vendedor

- Necesita un correo electrónico de trabajo para iniciar sesión en el [centro de Partners](https://partner.microsoft.com/).
- Si usa una cuenta que no es de trabajo en PSC o el correo electrónico del trabajo es para una empresa distinta a la de la empresa asociada, póngase en contacto con el administrador de PSC para obtener ayuda de configuración de cuenta.
- Consulte con el administrador de PSC si la configuración de la cuenta del centro de Partners está completa independientemente de la cuenta que use para iniciar sesión en PSC.
- Compruebe si tiene acceso al centro de Partners y a la sección de referencias.
- Lea este documento para conocer los flujos de trabajo y los cambios en el centro de Partners.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Como administrador en PSC, estos son los pasos siguientes.

Si no ve la pestaña referencias:

- El [administrador global](permissions-overview.md) de su empresa puede concederle acceso a la pestaña referencias. Para buscar el administrador global, vaya a configuración de socio comercial en el icono de engranaje de la parte superior derecha del centro de Partners. Seleccione la página Administración de usuarios en el segundo nivel de la barra de navegación izquierda. Haga clic en la lista desplegable que muestra "todos los usuarios" en la parte superior derecha de la página y cambie a "administradores globales". La página mostrará a continuación todos los administradores globales con sus respectivos identificadores de correo electrónico. Póngase en contacto con ellos para obtener acceso "Administrador de referencia" para su cuenta profesional.

>[!Important]
> Si su rol solo está administrando usuarios en PSC, puede obtener el rol [Administrador de cuenta](permissions-overview.md#manage-mpn-membership-and-your-company) en el centro de Partners. Si su rol también incluye la administración de oportunidades de venta conjunta, debe obtener el rol de [Administrador de referencias](permissions-overview.md#manage-referrals) . Además, supongamos que un responsable de administración de cambios entre los administradores de PSC trabaja con el administrador de la cuenta del centro de Partners en lugar de que todos los administradores de PSC lleguen a los administradores de cuentas del equipo individualmente.

 :::image type="content" source="images/pscmigration/accountadmin.png" alt-text="Imagen que muestra los administradores de cuentas en la página de administración de usuarios de configuración de socios comerciales.":::

- Vaya a la pestaña referencias en el panel de navegación izquierdo y compruebe si puede tener acceso a las páginas.

>[!Note]
> Es posible que tenga que cerrar la sesión del centro de Partners y volver a iniciar sesión para actualizar las credenciales para el acceso a las páginas de referencias.

Una vez configurada la cuenta en el centro de Partners,

- Invite a todos los usuarios que tienen un rol "Deal Manager" o "vendedor" en PSC al centro de partners como paso siguiente.
- El [Administrador](permissions-overview.md#manage-mpn-membership-and-your-company) de la cuenta que le ayudó con el acceso a las referencias puede invitar a todos los usuarios.
- Al invitar a los usuarios, pídale al administrador de la cuenta que le asigne el rol de [Administrador de referencias](permissions-overview.md#manage-referrals) .
- Es posible que algunos de los usuarios de PSC estén usando una cuenta que no sea de trabajo o una cuenta de un dominio diferente del que está usando en el centro de Partners. Todos estos usuarios deben iniciar sesión en el centro de Partners con su cuenta profesional asociada al inquilino de Azure AD. El [administrador global](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) puede ayudarle con esto. Para buscar el administrador global, vaya a configuración de socio comercial en el icono de engranaje de la parte superior derecha del centro de Partners. Haga clic en la página Administración de usuarios en el segundo nivel de la barra de navegación izquierda. Haga clic en la lista desplegable que muestra "todos los usuarios" en la parte superior derecha de la página y cambie a "administradores globales".
- El administrador global puede crear una nueva cuenta de usuario en el inquilino de Azure AD o asignar acceso de usuario invitado a los demás usuarios de la cuenta de dominio.
- Una vez que las cuentas están configuradas para todos los administradores y usuarios de la empresa de PSC, deben iniciar sesión en el centro de Partners, ir a la pestaña referencia en el panel de navegación izquierdo y comprobar que pueden ver la página referencias.

Si su empresa tiene un PDM, cuando se configure la cuenta del centro de Partners y los usuarios hayan movido y tengan roles y permisos, puede trasladar las actividades de venta conjunta al centro de Partners. Informe a PDM para que realice el cambio en lugar de esperar hasta que se complete la fecha límite de la migración, lo que permitirá que todos los nuevos acuerdos fluyan al centro de Partners.
>[!Note]
>Una vez que haya realizado este cambio, solo podrá actuar en los contratos activos existentes en PSC. No puede crear nuevos acuerdos ni recibir ningún trato de los vendedores de Microsoft en PSC.

Si su empresa no tiene un PDM, asegúrese de que todos los usuarios configuran y comprueban todas las cuentas de usuario. Recibirá una notificación a través de un correo electrónico y un banner en PSC respecto a la fecha exacta en la que podrá empezar a vender en el centro de Partners. Recuerde que todavía tendrá que administrar las ofertas activas existentes en PSC.

>[!Important]
>Las ofertas activas no se migrarán al equipo. Tendrá hasta el 31 de diciembre de 2020 para cerrar y registrar los acuerdos.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Pasos siguientes para administradores de PSC, administradores de acuerdos de PSC y vendedores de PSC

Aprenda a vender en el centro de Partners.
Este es un paso importante, que le ayudará a prepararse para la venta conjunta en el centro de Partners. Comprenda los flujos de trabajo y los cambios en el centro de partners para que pueda vender de forma eficaz desde el primer día. Empiece por leer este documento completamente. También hay disponible un buen conjunto de recursos en la [Galería de experiencias de venta conjunta](https://aka.ms/cosellexperience).

## <a name="major-differences-between-psc-and-pc-workflows"></a>Principales diferencias entre los flujos de trabajo de PSC y PC

|**Escenario**|**Conexión de ventas de asociados**|**Centro de partners**|
|-----|:-----|:-----|
|Roles de usuario|PSC tiene roles de administrador, Director de transacciones y vendedor.|PC solo tiene el rol de [Administrador de referencia](permissions-overview.md#manage-referrals) que proporciona permiso de lectura y escritura para todos los contratos.|
|Invitar a Microsoft en un trato de venta conjunta|Iniciado por el vendedor de Microsoft, no hay ninguna pregunta explícita por parte del asociado.|El asociado tendrá que realizar una [solicitud explícita](manage-co-sell-opportunities.md#add-solutions) si se necesita ayuda de Microsoft para un vendedor. El vendedor de Microsoft tiene una opción para rechazar la solicitud.|
|Expiry|No hay ningún concepto de la expiración de un contrato.|Los acuerdos de entrada de asociados expiran en 14 días si no los acepta el socio. Lo mismo ocurre con los acuerdos salientes de los asociados en los que pueden entrar en el estado expirado si el vendedor de Microsoft no actúa en ellos en 14 días.|
|Detalles de vendedor de Microsoft|Visible en cuanto se crea un trato.|Los detalles de los vendedores de Microsoft se comparten con el socio comercial solo si el vendedor acepta explícitamente la invitación para la venta conjunta del socio.|
|[Canalización privada](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|No está disponible.|Los asociados pueden compartir su canalización sin ofrecer visibilidad a los vendedores de Microsoft.|
|Soluciones|Las soluciones que pertenecen a una sola lista de precios se pueden agregar a un contrato.|El asociado puede agregar [soluciones](manage-co-sell-opportunities.md#add-solutions) que pertenezcan a las listas siguientes. a) sus propias soluciones de soluciones b) del catálogo de Microsoft First Party (similar a la función de trato de transacciones en PSC) y c) soluciones de venta conjunta de otros asociados de terceros (similar al rol de negocio de ISV en PSC).|
|Asignación de trato|Solo el vendedor asignado puede ver los acuerdos y actuar sobre ellos.|Los miembros del equipo se pueden agregar a un trato para especificar las personas que trabajan en un trato, no hay ningún bloqueo de otros administradores de referencia que puedan ver o actuar en esos acuerdos.|
|Organización del cliente|Entrada de texto de forma libre.|Puede buscar la [organización del cliente](manage-co-sell-opportunities.md#select-your-customer) en la [base de datos D&B](https://www.dnb.com/) escribiendo solo unos pocos caracteres. El nombre y la dirección válidos se rellenan automáticamente en función de la elección.|
|Contacto del cliente|No es obligatorio.|No es obligatorio para el uso compartido de la canalización privada. Requerido si el vendedor de Microsoft está invitado a participar en una solicitud de venta conjunta.|
|API pública|No está disponible.|[API pública](/partner/develop/referrals) para administrar mediante programación las referencias del centro de Partners.|

## <a name="psc-and-partner-center-field-mapping"></a>Asignación de campos de centro de Partners y PSC

En esta sección se presenta la asignación exacta de los atributos entre PSC y el centro de Partners. Cada pantalla de PSC se compara con la vista correspondiente en la sección oportunidades de venta conjunta del centro de Partners. 

>[!Note]
>Siga los números de las burbujas amarillas de las capturas de pantallas de PSC para buscar el atributo equivalente en el centro de Partners. Las burbujas rojas indican que el archivado no está disponible en el centro de Partners.

**Página principal de PSC y vista predeterminada de las oportunidades de venta conjunta en el centro de Partners**

 :::image type="content" source="images/pscmigration/homepage.png" alt-text="Imagen que muestra las asignaciones de campos entre la Página principal de Partner Sales Connect y la vista predeterminada de las oportunidades de venta conjunta en el centro de Partners.":::

**Vista de cuadrícula de PSC y vista de trato del centro de Partners**

- No hay ninguna vista de lista en el centro de partners como la de PSC.  Todas las ofertas se enumeran en función de la última fecha de recepción o de creación con la información del cliente y el tipo de contrato. La primera vez que se trata la vista está seleccionada de forma predeterminada. La mayoría de los valores que se muestran en el formato de tabla de PSC están disponibles en la vista de detalle del trato en equipo.
- El rol de negocio no es un campo obligatorio en PC. No se muestra ni se captura en ninguno de los flujos de trabajo. Se deriva automáticamente en el lado de vendedor de Microsoft en función de las soluciones agregadas a la transacción.
- La fecha de la última modificación no se muestra en la página Detalles de referencia de PC. Los asociados pueden usar la funcionalidad de ordenación para ordenar los acuerdos en función de la fecha de la última actualización.

 :::image type="content" source="images/pscmigration/gridview.png" alt-text="Imagen que muestra las asignaciones de campos entre la vista de cuadrícula de conexión de ventas de socio (PSC) y la vista de trato del centro de Partners.":::

**Vista de detalles del contrato en PSC y en el centro de Partners**

- Los asociados pueden editar una relación haciendo clic en el botón Editar de la vista de detalles del contrato de socio comercial (6). Una vez que se hace clic en el botón Editar, todos los campos se convertirán en editables con la opción de guardar o cancelar las modificaciones realizadas en el contrato.
- No hay ninguna opción para cerrar el trato como duplicado en el centro de Partners.
- El resultado del cliente no está disponible en el centro de Partners. Todos los detalles relacionados con las interacciones de los clientes pueden actualizarse en la sección notas en PC.
- La fecha estimada de cierre de la solución solo está disponible para las ofertas de IOT OEM en el centro de Partners. No se muestra para ningún otro tipo de trato.
- El programa de licencias no es necesario en PC. Se inferirá automáticamente en función de las soluciones seleccionadas en el contrato.

>[!Note]
>Cualquier trato marcado como ganada o perdida no se puede editar. Tenga cuidado al trasladar un trato a uno de estos Estados de terminal.

 :::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Imagen que muestra las asignaciones de campos entre la vista de detalles del contrato de ventas de asociados (PSC) y la vista de detalles del centro de Partners.":::

**Vista "agregar productos" de PSC y la vista "agregar soluciones" del centro de Partners**

 :::image type="content" source="images/pscmigration/products.png" alt-text="Imagen en la que se muestran las asignaciones de campos entre la vista agregar productos del socio comercial de ventas (PSC) y el centro de Partners agregar vista de soluciones.":::

**Administración de usuarios en PSC y centro de Partners**

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Imagen que muestra las asignaciones de campos entre la Página principal de administración de usuarios de conexión de ventas de asociados (PSC) y la administración de usuarios del centro de Partners en la vista configuración de cuenta.":::

**Asignación de roles de usuario en PSC y centro de Partners**

- El rol equivalente para el administrador de PSC es el rol de administrador de cuenta en el centro de Partners.
- Solo hay un rol en el centro de partners para la administración de acuerdos de venta conjunta, que es el rol de administrador de referencia.

 :::image type="content" source="images/pscmigration/roles.png" alt-text="Imagen que muestra las asignaciones de campos entre la vista de asignación de roles de conexión de ventas (PSC) de asociados y la vista de asignación de roles del centro de Partners.":::

**Notificaciones en PSC y centro de Partners**

 :::image type="content" source="images/pscmigration/notifications.png" alt-text="Imagen que muestra la asignación entre las notificaciones de socio comercial (PSC) de asociados y la vista de notificaciones del centro de Partners.":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Cambio de PSC a Partner Center: preguntas más frecuentes

**Q1. ¿Qué debo hacer si no tengo acceso al centro de Partners?**

Puede ponerse en contacto con los administradores que aparecen en la página "sin acceso" para obtener los roles asignados. Necesitará el rol "[Administrador de referencias](permissions-overview.md#manage-referrals)" para el permiso de lectura y escritura en la sección referencias. Si solo está administrando perfiles de negocio, necesitará el rol "Administrador de Perfil de negocio" en el centro de Partners.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Imagen que muestra la experiencia de no acceso en el centro de Partners.":::

**Q2. ¿Quién puede concederme acceso a la sección de referencias del centro de Partners?**

El [Administrador](permissions-overview.md#manage-mpn-membership-and-your-company) de la cuenta puede concederle acceso a la pestaña referencias. Para buscar el administrador de la cuenta, vaya a configuración del socio comercial en el icono de engranaje de la parte superior derecha del centro de Partners. Haga clic en la página Administración de usuarios en el segundo nivel de la barra de navegación izquierda. Haga clic en la lista desplegable que muestra "todos los usuarios" en la parte superior derecha de la página y cambie a "Admins. de cuenta". La página mostrará todos los administradores de cuentas con sus respectivos identificadores de correo electrónico. Póngase en contacto con ellos para obtener acceso "Administrador de referencia" para su cuenta profesional.

**Q3. El botón + nuevo contrato está atenuado para nuestra cuenta. ¿Qué debo hacer para empezar a crear negocios?**

Esto solo ocurre si no hay ninguna solución de venta conjunta preparada conectada a la organización de MPN que está usando en el centro de Partners. Póngase en contacto con el PDM para obtener el identificador de MPN de sus soluciones corregidas o cree una incidencia de soporte técnico que mencione el problema "el nuevo botón de negocio está atenuado después de la migración de PSC".

**Cuatro. ¿Puedo asignar tratos a una persona específica de nuestra organización como PSC?**

Puede asignar miembros del equipo a un trato específico. No impide que otros administradores de referencia vean o actúen en esos acuerdos. 

**Q5. ¿Hay una vista de todas las ofertas asignadas a mí?**

Puede usar la característica favoritos, que es una pestaña de nivel de usuario. Puede marcar todos los acuerdos que tiene asignados como favoritos para obtener un acceso rápido a los negocios.

**Q6. ¿Hay una vista de solo lectura para los acuerdos?**

No, no hay ninguna vista de solo lectura de los contratos en la sección referencias. Todos los administradores de referencia tendrán acceso completo de lectura y escritura a todos los contratos.

**Q7. ¿Cómo puedo registrar un trato después de que lo gane?**

Si el trato cumple los siguientes criterios, se mostrará un elemento emergente para empezar a trabajar con el [registro](./register-deals.md).

- Existe una solución de incentivos que reúne el trato.
- El vendedor de Microsoft está invitado a participar en el trato o le ha invitado al trato.
- La tarjeta de Microsoft está en el estado aceptado o ganado en el centro de Partners.

**Q8. Aparece un mensaje de error al hacer clic en el botón "+ registro del nuevo contrato" en la sección registro de trato. ¿Cómo puedo registrar mis negocios?**

El "+ nuevo registro de trato" solo lo usarán los asociados registrados en el programa de conexión de ISV para registrar un trato sin ninguna oportunidad de venta conjunta correspondiente en el centro de Partners. Para el registro de acuerdos con una oportunidad de venta conjunta, se mostrará un mensaje emergente cuando el trato se marque como ganado y si cumple los criterios de registro del contrato.

**Q9. ¿Es obligatorio agregar una organización de cliente?**

Sí, la adición de una [organización de clientes](./manage-co-sell-opportunities.md#select-your-customer) es obligatoria en el centro de Partners. En primer lugar, busque la ubicación donde se encuentra el cliente. En función de los detalles que tenga; puede ser específico incluyendo el nombre exacto de la compilación o simplemente proporcionar los detalles de la ciudad. La búsqueda de la organización recuperará todas las entidades jurídicas que coincidan con el nombre especificado para que no tenga que escribir ningún detalle de dirección. Todos los detalles se rellenan automáticamente en función de la organización seleccionada.

**Q10. ¿Son obligatorios los detalles de contacto del cliente?**

Depende del [tipo de trato](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) que se va a crear. Si solo comparte su canalización y no requiere ayuda de la organización de ventas de Microsoft, puede elegir no proporcionar los detalles de contacto del cliente. Si va a realizar la venta conjunta en la que va a buscar ayuda de forma activa en el vendedor de Microsoft, deberá proporcionar los detalles de contacto del cliente. Debe obtener el consentimiento explícito del cliente antes de crear una solicitud de venta conjunta en el centro de Partners.

**Q11. ¿Cuántas soluciones se pueden agregar a un trato?**

Puede Agregar hasta 50 soluciones (análogas a ' productos ' en PSC) a un trato. A diferencia de PSC, puede combinar soluciones de sus propias soluciones de venta conjunta coincidentes, SKU de Microsoft First Party y otras soluciones coincidentes de terceros. No hay ningún rol de trato que deba seleccionarse o estar disponible en el centro de Partners. En el caso de las SKU de Microsoft, puede agregar opcionalmente la cantidad y el precio de cada SKU que se agregue a la transacción.

**Q12. ¿Cuándo puedo conocer los detalles de los vendedores de Microsoft después de crear un trato?**

A los vendedores de Microsoft se les asigna solo después de que coincidan con el requisito de ayuda exacto indicado al crear el trato con el rol de vendedor pertinente en el lado de Microsoft. Incluso después de la asignación, los vendedores de Microsoft tendrán una opción para aceptar o rechazar la invitación de venta conjunta. Solo si un vendedor acepta una invitación de venta conjunta, el trato se actualizará con los detalles de contacto del vendedor de Microsoft. El acuerdo de nivel de servicio para que los vendedores de Microsoft actúen en el trato es de 14 días. Es el mismo acuerdo de nivel de servicio que los asociados tienen que actuar en el trato antes de que pase al estado expirado.

**Q13. ¿Dónde puedo encontrar el identificador de oportunidad?**

El identificador de oportunidad en PSC es el mismo que el identificador de trato en PC. Puede encontrar el identificador de trato junto al nombre del trato al abrir cualquier trato.

**Q14. ¿Cómo puede mi PDM obtener acceso al equipo?**

El centro de Partners no es accesible desde el PDM directamente, a diferencia de PSC. Hay varias opciones para habilitar esa capacidad, que se mencionan a continuación.

- OCP Insights: si PDM solo está viendo los acuerdos & progreso relacionado con ellos, pueden usar el portal de OCP Insights para obtener la vista de la organización. Se trata de una herramienta interna que solo está disponible para PDM. Tenga en cuenta que OCP Insights no está disponible para los usuarios de su empresa.
- Usuario invitado en el centro de Partners: puede agregar su @microsoft.com cuenta de PDM como usuario invitado en el centro de Partners y asignarle el rol de administrador de referencias para que puedan ver y actuar en función de las referencias.
- Creación de un [nuevo usuario](./create-user-accounts-and-set-permissions.md#add-a-new-user) en el inquilino: puede crear un nuevo usuario en su propio inquilino y compartir esos detalles con el PDM para que puedan ver y actuar en las referencias similares a otros usuarios de referencia de su cuenta.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Recursos para ayudarle a crear y administrar sus ofertas en el centro de Partners

Si aún no ha leído los temas de ayuda de la venta conjunta, los siguientes recursos le ayudarán a administrar los acuerdos en el centro de Partners.

|**Para**   |**Lee esto**   |
|-----------------------|:-----------------------|
|Descripción de las pestañas y la navegación en la página de oportunidades de venta conjunta|[Navegar por la sección de venta conjunta](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|Selección de una organización de cliente en la lista D&B |[Seleccione su cliente](./manage-co-sell-opportunities.md#select-your-customer)|
|Modificación de los campos de la sección Detalles del contrato|[Detalles del trato](./manage-co-sell-opportunities.md#deal-details)|
|Agregar los miembros del equipo a un equipo de trato|[Agregar los empleados](./manage-co-sell-opportunities.md#add-team-members)|
|Respuesta a un trato de venta conjunta|[Administrar ofertas de venta conjunta](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Registre los acuerdos que ha ganado en el centro de Partners |[Registrar una nueva oferta](./register-deals.md)
|Obtenga información de referencia y descubra cómo están haciendo sus referencias |[Información de referencia](./referral-insights.md)
|Creación y administración de perfiles de negocio|[Administrar el perfil de negocio](./create-a-marketing-profile.md)
|Administración de clientes potenciales para su perfil de negocio |[Administrar los clientes potenciales](./manage-leads.md)|

## <a name="additional-resources"></a>Recursos adicionales

- [Ventas de asociados conectar con el centro de Partners libro](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) : libro para alinear los procesos de ventas y roles de los asociados con nuevos procesos de ventas a través del centro de Partners frente a la conexión de ventas de asociados.
- [Guía de funcionamiento de la venta conjunta del centro de Partners](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) : Guía para identificar un modelo operativo a través del centro de Partners con el fin de administrar oportunidades de ventas de clientes potenciales o de venta conjunta.
- [Baraja de administración de referencias](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) : instrucciones paso a paso para administrar clientes potenciales y oportunidades de venta conjunta a través del centro de Partners.
- [Publicación y administración en el Marketplace comercial](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) : instrucciones paso a paso para crear, administrar y publicar ofertas a través del centro de Partners en Marketplace comercial.
