---
title: Cómo comprar una oferta de SaaS en Azure Portal
description: Obtenga información sobre cómo buscar y comprar una oferta de SaaS en Azure Portal.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/29/2021
ms.openlocfilehash: a124e4c5bb31a1fbb744bf2c5e1ea65a356bdd54
ms.sourcegitcommit: 1d09ccaaa54f167b0c63e99761172ebe84e89f2e
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/02/2021
ms.locfileid: "113221447"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Compra de una oferta de SaaS en Azure Portal

En este artículo se explican las distintas opciones y requisitos para buscar, probar y comprar una oferta de software como servicio (SaaS) de la Azure Portal.

## <a name="create-a-saas-subscription"></a>Creación de una suscripción de SaaS

Para comprar una suscripción de SaaS, necesita una cuenta de usuario de Azure con acceso a una suscripción de Azure adecuada. Esta suscripción se usará para la facturación, así como para la compartimentación de los recursos en la nube adquiridos. Para más información sobre las suscripciones de Azure, consulte [Creación de una suscripción de Azure adicional.](/azure/cost-management-billing/manage/create-subscription)

En la Azure Portal, seleccione la oferta de SaaS deseada en la **sección Marketplace.**

Una suscripción de software como servicio proporciona el derecho de usar un servicio durante un período de tiempo determinado a través de una suscripción en línea en lugar de la instalación local en equipos individuales. Una suscripción es un contrato para usar una o varias plataformas o servicios en la nube, para los que los cargos se acumulan en función de una cuota de licencia por usuario o del consumo de recursos basado en la nube. Una organización puede tener varias suscripciones de SaaS.

Las restricciones en las suscripciones de SaaS incluyen:

- No hay suscripciones de alumnos.
- No Visual Studio Enterprise suscripción.
- No hay suscripciones de crédito gratuitas.
- Para las ofertas de pago, se requiere un instrumento de pago.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS ofrece detección en Azure Portal

Una vez que Azure Portal, hay varias maneras de restringir la búsqueda para centrarse en las ofertas de SaaS.

### <a name="narrowing-your-search"></a>Restringir la búsqueda

En la página principal, en **Servicios de Azure,** seleccione **+ Crear un recurso** o **Marketplace.** O bien, use el acceso **directo G + N en** cualquier lugar de la plataforma.

- Limite los resultados a las ofertas de SaaS mediante el filtro **Tipo de** oferta y, a continuación, **seleccione SaaS.**
- Use la búsqueda global en el área de navegación superior para encontrar una oferta de SaaS específica.

Busque una [oferta de SaaS privada](/marketplace/private-offers) seleccionando el banner en la parte superior de la página principal de **Marketplace.** No todas las ofertas o planes están disponibles en todas las zonas geográficas y algunas solo pueden aparecer para determinados inquilinos.

La vista filtrada muestra cada oferta de SaaS disponible representada por un título. Seleccione uno para ver la página de detalles del producto. Incluye las secciones siguientes:

- Información general: detalles sobre el servicio, el marketing y los materiales de aprendizaje
- Planes y precios: cada oferta incluirá al menos un plan con diferentes términos y precios de facturación
- Información de uso y soporte técnico: incluye Publisher, id. de oferta e id. de plan
- Clasificación y revisiones de la oferta específica de SaaS

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Modelos de facturación disponibles (planes o SKU) para ofertas de SaaS

Cada oferta de SaaS tendrá uno o varios planes. Cada oferta tiene un modelo de precios asociado: tarifa plana o por usuario. Cada precio del plan es una tarifa periódica, que puede ser de cero dólares (los precios enumerados son solo para fines de ejemplo y no están diseñados para reflejar los costos reales). Esta tarifa es tarifa plana o precio por usuario. Tipos de planes disponibles:

- **Planes mensuales:** cuota mensual periódica; tarifa mensual plana o por usuario que se paga con periodicidad mensual. Cuando finalice el período, el plan se renovará automáticamente.
- **Planes anuales:** cuota anual periódica; tarifa anual plana o por usuario que se paga con periodicidad anual. Cuando finalice el período, el plan se renovará automáticamente.
- **Medidores personalizados:** junto con las tarifas periódicas, un plan de tarifa plana también puede incluir dimensiones de uso personalizado opcionales para el uso por encima del límite no incluido en la tarifa plana. Cada dimensión representa una unidad facturable. Se trata de un costo variable que cambia según el uso de las unidades de uso, como el ancho de banda, los vales o el correo electrónico procesado. Se le cobrará según el consumo de estas dimensiones mensualmente. Tenga en cuenta que el consumo de uso por encima del uso se inicia solo cuando se usan todas las unidades de uso medidas incluidas en la tarifa plana.
- **Evaluación gratuita:** en algunos casos, el plan incluye un período de prueba de un mes, durante el cual puede usar el software de forma gratuita.  Una vez que haya terminado el período de prueba, se le cobrará según el plan. Las ofertas de prueba no son compatibles con los medidores personalizados.

Estos modelos de precios están disponibles para planes públicos y privados.

## <a name="saas-purchase-experience"></a>Experiencia de compra de SaaS

1. En la página del producto, seleccione un plan que satisfaga sus necesidades y siga **configurando + suscribirse.**
2. Como parte del proceso de compra, se le redirigirá a la pestaña **Aspectos** básicos y se le hará lo siguiente:
    1. Defina qué *suscripción* desea usar para la facturación. La suscripción de Azure que use debe tener definido un método de compra válido. Debe tener el nivel de permiso adecuado o tener un grupo de recursos en esa suscripción con el nivel correcto de permisos. Además, su país de facturación debe ser un país donde la oferta esté disponible para su compra. Las suscripciones de Azure sin un método de pago válido (por ejemplo, una suscripción de MSDN) solo se pueden usar para comprar planes gratuitos.
    1. Elija o cree un **grupo de recursos al* que pertenecerá el recurso de SaaS.
    1. Escriba un *nombre para* la suscripción de SaaS para identificarlo fácilmente más adelante. Una vez comprado, no puede cambiar el nombre.
    1. En **Plan**, verá el plan seleccionado en la página detallada del producto (PDP). Si no ha realizado una selección activa en el PDP, verá el plan predeterminado. Puede cambiar la selección seleccionando el vínculo **Cambiar plan.** Seleccione el período de facturación correspondiente y, a continuación, elija otro plan. Es posible que pueda cambiar el plan después de la compra, si el publicador lo admite. Sin embargo, no podrá cambiar el plazo de mensual a anual o de anual a mensual.
    1. En los casos en los que el modelo de precios *es por usuario,* es posible que deba especificar el número de *usuarios*. El precio que vea cambiará en función de la suscripción, el plan y el término que haya seleccionado.
3. Continúe con **la pestaña** Etiquetas: las etiquetas son pares clave-valor definidos por el usuario, que se pueden colocar directamente en un recurso o un grupo de recursos.  Puede usar etiquetas para encontrar fácilmente el recurso de SaaS más adelante. Actualmente, Azure admite un máximo de 50 etiquetas por recurso y grupo de recursos. Las etiquetas se pueden colocar en un recurso en el momento de su creación, o bien se pueden agregar a un recurso existente.
4. Continúe con **Revisión y suscripción** para consultar los detalles de la oferta y el plan.
    1. Revise *Términos de uso,* *las modificaciones* y la directiva *de* privacidad del publicador y también para Azure Marketplace
    1. Es posible que se le pida que agregue los detalles de contacto.
    1. Revisión *de los aspectos básicos* y los detalles de las *etiquetas*
5. Tras la confirmación, seleccione **Suscribirse.**

## <a name="saas-subscription-and-configuration"></a>Suscripción y configuración de SaaS

Al seleccionar Suscribirse, aparece un mensaje que indica "La suscripción de SaaS está en curso". Este proceso debería tardar unos minutos y no cerrar la ventana hasta que finalice.

Una vez completada la suscripción, aparece un mensaje que indica que la suscripción de SaaS se ha completado y debe configurar la cuenta para empezar a disfrutar de la compra. También recibirá un correo electrónico en el que se le pedirá que active la nueva suscripción. Si no es el que va a configurar la cuenta de SaaS, reenvía este correo electrónico a la persona correspondiente.

Para completar el proceso y empezar a usar SaaS, es necesario empezar a configurar la suscripción. Al seleccionar el botón **Configurar cuenta ahora,** se le redirigirá al sitio web del publicador.

También puede comprobar el estado de la suscripción seleccionando el icono "campana" en la esquina superior derecha del encabezado.

Si no completa el proceso de configuración en un plazo de *30* días, esta suscripción de SaaS se eliminará *automáticamente.* La facturación se iniciará una vez configurada la cuenta en el sitio web del publicador.

Mensajes de error que podrían encontrarse durante el proceso:

- El nombre *del plan seleccionado no se* puede adquirir en una suscripción gratuita.
  - Actualice su cuenta y consulte https://aka.ms/UpgradeFreeSub para obtener más detalles.

- No se pudo realizar la compra porque no se pudo encontrar una tarjeta de crédito válida ni un método de pago asociado a su suscripción de Azure.
  - Use otra suscripción de Azure o agregue o actualice el método de pago o la tarjeta de crédito actual para esta suscripción y vuelva a intentarlo.

- El *nombre del plan seleccionado del*  nombre de la oferta por publicador de la oferta por publicador no está disponible para su compra según las reglas establecidas por el administrador de TI. 
  - Póngase en contacto con el administrador de TI.

- El *nombre del plan* seleccionado del  *plan* de oferta seleccionado por el publicador de la oferta no está disponible para su compra debido a la configuración de Marketplace privada realizada por el administrador de TI del inquilino.
  - Póngase en contacto con el administrador de TI.

- Error de compra porque el período de facturación solicitado está vacío o no es válido.
  - Intente comprar un plan o período de facturación diferente.

- Error en la compra porque no se pudo comprobar la firma del contrato legal.
  - Reintentar. Si el error persiste, intente realizar la compra con una suscripción de Azure diferente o póngase en contacto con el soporte técnico.

- Error en la compra de *offerID* por *publisherID* del publicador. Esta oferta no está disponible actualmente para la compra.
  - Vuelva a intentarlo más tarde. Si después de una hora sigue recibiendo este mensaje de error, póngase en contacto con el soporte técnico.  

- Error en la compra del *plan planID* de *offerID* por *publisherID* del publicador. Este plan no está disponible actualmente para la compra.
  - Vuelva a intentarlo más tarde. Si después de una hora sigue recibiendo este mensaje de error, póngase en contacto con el soporte técnico. 

- La dirección de *correo electrónico del cliente* con el id. de objeto *ObjectID* no tiene autorización para realizar la acción *DeploymentValidationAction* en el *ámbito ResourceGroup; DeploymentScope* o el ámbito no es válido.  
  - Recibirá este mensaje si no tiene los permisos adecuados en la suscripción o el grupo de recursos de Azure.  
    Si el acceso se concedió recientemente, actualice sus credenciales.  
    Para implementar recursos en un grupo de recursos, debe tener al menos acceso de colaborador. Compruebe el estado de acceso en **Grupos de recursos** y, a **continuación, Access Control**. Esto muestra quién es el "Propietario", a quien puede pedir que le asigne como "Colaborador".

- La suscripción usada para esta compra no permite las compras de Marketplace.  
  - Use otra suscripción o pida al administrador que cambie la definición de esta suscripción y vuelva a intentarlo.

## <a name="next-steps"></a>Pasos siguientes

- Si ya ha adquirido una oferta en Marketplace, vaya a [Facturación y facturación.](/marketplace/billing-invoicing)
- También puede obtener más información sobre las [opciones de planes privados.](/marketplace/private-offers)
