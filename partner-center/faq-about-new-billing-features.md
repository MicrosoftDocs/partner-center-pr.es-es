---
title: "Preguntas frecuentes sobre las nuevas características de facturación | Centro de partners"
Description: The following are frequently asked questions about Partner Center's annual billing and free trial features.
ms.assetid: 
author: MaggiePucciEvans
ms.openlocfilehash: cd6e267dd691529998cf43e7a21a3abac066e2d7
ms.sourcegitcommit: 6eec754e269e8744d4e09df64a690d0c74525dbb
ms.translationtype: HT
ms.contentlocale: es-ES
ms.lasthandoff: 02/14/2018
---
# <a name="faq-about-new-billing-features"></a>Preguntas frecuentes sobre las nuevas características de facturación

**Se aplica a**

-  Centro de partners
-  Centro de partners para Microsoft Cloud for US Government
-  Centro de partners para Microsoft Cloud Alemania

A continuación se incluyen algunas de las preguntas frecuentes relacionadas con las características de evaluación gratuita y facturación anual del Centro de partners. 

## <a name="in-this-section"></a>En esta sección

-   [Preguntas frecuentes sobre la facturación anual](#annualbillingfaq)

-   [Preguntas frecuentas sobre las evaluaciones gratuitas](#freetrialsfaq)

-   [Preguntas frecuentes sobre la alineación de facturación](#billingalignmentfaq)


## <a href="" id="annualbillingfaq"></a>Preguntas frecuentes sobre la facturación anual

Secciones:

[Información general y ventajas de la facturación anual](#overviewandbenefits)

[Cómo realizar un pedido y la facturación](#placingyourorder)

[Cambiar tu suscripción](#changingyoursubscription)

[Cálculo de precios](#pricingcalculation)

[Generación de informes](#reporting)

[Incentivos](#incentives)


<a href="" id="overviewandbenefits"></a>**Información general y ventajas de la facturación anual**

**P:** ¿Qué ha cambiado?

-   **R:** Como respuesta a las solicitudes recibidas, hemos incluido la opción de pagar determinadas suscripciones de CSP de forma anual o mensual. Esta nueva opción comenzó a estar disponible el 17 de octubre de 2017.

**P:**¿Quién puede participar?

-   **R:** Todos los tipos de partners y partners pueden sacar partido de la facturación anual. La facturación anual está disponible en todos los mercados donde CSP está disponible actualmente. 

**P:** ¿Qué tengo que tener en cuenta al pensar en la facturación anual?    

-   **R:** Deberías tener en cuenta cómo se verá afectado tu proceso de ventas. Estas son algunas sugerencias que te ayudarán a usar de forma eficaz la facturación anual. 
    - Actualiza las API para dar cabida a la característica de facturación anual, si corresponde. 
    - Revisa los cambios en la factura y el archivo de conciliación basada en licencia.
    - Asegúrate de que tu equipo esté informado.
    - Actualiza tus procesos internos según sea necesario.

**P:**¿Cuáles son las ventajas de la facturación anual? 

-   **R:** La facturación anual tiene las siguientes ventajas:

    - Una mayor flexibilidad en opciones de pago.

    - Una mejor alineación con la facturación de tus clientes.

    - Menor impacto de fluctuaciones de moneda.

    - Menores costos operativos de facturación.

**P:** ¿Qué ofertas tendrán la opción de facturación anual?

-   **R:** La mayoría de suscripciones basadas en licencia tienen la opción de facturación mensual o anual. Las suscripciones basadas en uso solo tienen la opción de facturación mensual. Podrás identificar las frecuencias de facturación disponibles para cada oferta con la columna J de la matriz de ofertas. Puedes encontrar la matriz de ofertas en la sección "Ver ofertas y precios" del Centro de partners. .

**P:** La facturación anual, ¿es por suscripción o por licencia?       

-   **R:** Tanto la facturación anual como la mensual son por suscripción.

**P:**¿Hay cambios necesarios en las API para dar soporte a la facturación anual?    

-   **R:** Para sacar partido de la facturación anual hay algunos cambios necesarios en las API. Encontrarás más información en los siguientes artículos:

    - https://partnercenter.microsoft.com/es-es/partner/developer

    - https://msdn.microsoft.com/es-es/library/partnercenter/microsoft.store.partnercenter.models.orders.order.billingcycle.aspx 

    - Código de muestra: https://msdn.microsoft.com/es-es/library/partnercenter/mt634667.aspx 

<a href="" id="placingyourorder"></a>**Cómo realizar un pedido y la facturación**

**P:** ¿Habrá una única oferta específica para los pedidos con facturación anual?   

-   **R:** No. Todas las frecuencias de facturación, incluida la opción de facturación anual, se asignan a la oferta como un atributo. Sin embargo, puedes cambiar el nombre de una oferta con un nombre más descriptivo de cliente para permitir la diferenciación.

**P:** ¿Cómo puedo seleccionar una facturación anual?

-   **R:** Al agregar una suscripción nueva, se te pedirá que selecciones una frecuencia de facturación. Puedes elegir la opción de facturación anual en este momento. Una vez que se selecciona la facturación anual se mostrarán todas las ofertas disponibles.

**P: ** ¿Si elijo facturación anual cuando se me facturará?    

-   **R:** Se facturará en la siguiente fecha de facturación. Por ejemplo, si la fecha de facturación es el 1 de febrero, siempre se te facturará el 1 de febrero. Por lo tanto, si compras una suscripción facturada anualmente el 29 de octubre de 2017 o el 15 de enero de 2018, se te facturará por la suscripción anual del 1 de febrero de 2018, en ambos casos. 

**P:** ¿Puedo dividir una suscripción para que una parte se facture mensualmente y la otra anualmente?  

-   **R:** No. Toda la suscripción debe tener la misma frecuencia de facturación. Toda la suscripción debe tener una facturación mensual o anual.

**P:** ¿Cuándo tiene lugar la renovación de una suscripción con facturación anual?     

-   **R:** La fecha de renovación será doce meses después de la fecha de inicio del servicio. El período de servicio comienza en la fecha en que se crea la suscripción.  Por ejemplo, una suscripción creada el 10 de enero de 2018, se renovará el 10 de enero de 2019.

**P:** ¿Cuándo se me facturará la renovación de una suscripción con facturación anual? 

-   **R:** Se te enviará una factura en la siguiente fecha de facturación después de la fecha de renovación de suscripción. Por ejemplo, si compras una suscripción con facturación anual el 15 de enero de 2018 y la fecha de facturación es el 20 de enero, tu suscripción se renovará en 15 de enero de 2019. La renovación se te facturará entonces el 20 de enero de 2019.

**P:** ¿Reciben las suscripciones con facturación anual un período gratuito?

-   **R:** No, las suscripciones con frecuencia de facturación anual no reciben un período gratuito. El plazo pagado de 12meses comienza en la fecha de compra. Difiere de las suscripciones con frecuencia de facturación mensual que reciben un período gratuito desde la fecha de compra hasta la próxima fecha de facturación.

**P:** ¿Puede un cliente tener varias suscripciones de la misma oferta cada una con diferentes frecuencias de facturación?    

-   **R:** Depende de la oferta. Hay algunas ofertas que están limitadas a una suscripción por cliente. Si la oferta no está limitada, un cliente puede tener varias suscripciones de la misma oferta con diferentes frecuencias de facturación. Puedes encontrar los detalles de todos los límites y restricciones de la oferta en la columna I de la matriz de ofertas. Puedes encontrar la matriz de ofertas en la sección "Ver ofertas y precios" del Centro de partners.

<a href="" id="changingyoursubscription"></a>**Cambiar tu suscripción**

**P:** ¿Puedo agregar una licencia nueva a una suscripción existente que tiene facturación anual?    

-   **R:** Sí. Puedes cambiar la cantidad de licencias de tus suscripciones en cualquier momento. Agregar licencias adicionales no afectará a la frecuencia de facturación. 

**P:**¿Puedo agregar licencias que tienen una facturación mensual a una suscripción existente que tiene facturación anual? 

-   **R:** Cuando adquieres una suscripción con facturación anual, cualquier licencia adicional seguirá la misma frecuencia de facturación. Si necesitas después adquirir liencias con facturación mensual, tendrás que adquirir una nueva suscripción.

**P:** ¿Es posible cambiar la frecuencia de facturación de una suscripción de mensual a anual y viceversa? 

-   **R:** No. Una vez que hayas seleccionado la frecuencia de facturación, no se puede cambiar. 

**P:** ¿La facturación anual está disponible para las ofertas de complementos?   

-   **R:** Sí. La suscripción de complemento tendrá automáticamente la misma frecuencia de facturación que suscripción principal.

**P:¿** Cómo funcionará la facturación anual al agregar o quitar licencias? 

-   **R:** Puedes agregar o quitar licencias en cualquier momento. Recibirás un crédito y una renovación prorrateada en tu próxima fecha de facturación después de cambiar el número de licencias. 

**P:** ¿Qué sucede si cancelo una suscripción con facturación anual?    

-   **R:** La política de cancelación es la misma que todas las frecuencias de facturación. Si se cancela la suscripción en los primeros 30 días del plazo pagado de 12meses, recibirás un crédito del 100 por ciento en la próxima fecha de facturación. Si se cancela la suscripción en después de 30 días del plazo pagado de 12meses, recibirás un crédito prorrateado en la próxima fecha de facturación.

**P:** ¿Puede un cliente trasladar una suscripción con facturación anual de un partner a otro partner?  

-   **R:** No. No se pueden mover suscripciones entre partners. El nuevo partner debe adquirir una nueva suscripción en nombre del cliente. Esto se aplica a las suscripciones facturadas mensualmente y anualmente.

**P:** ¿Puedo volver a activar una suscripción con facturación anual?

-   **R:** Sí, puede volver a activar la suscripción hasta 90 días desde la fecha de suspensión. Recibirás un cargo prorrateado en la siguiente fecha de facturación. La fecha de renovación de la suscripción permanece igual.

<a href="" id="pricingcalculation"></a>**Cálculo de precios**

**P:** ¿Qué sucede si el precio de una oferta ha cambiado durante el período de 12 meses de una suscripción facturada anualmente?    

-   **R:** El precio de la oferta en el momento de la compra se garantiza durante todo el período de suscripción de 12 meses. 

**P:** ¿Qué precio tendrá una suscripción cuando se renueva automáticamente después del período de suscripción de 12 meses?    

-   **R:** Cuando se renueva una suscripción, el precio se basará en la lista de precios actual en la fecha de renovación. El nuevo precio se garantiza durante el siguiente período de suscripción de 12meses.

**P:** ¿Cómo se calcula el crédito de una suscripción o licencia cancelada? ¿Se calcula por día o por mes?   

-   **R:** El crédito de la cancelación se calcula de la siguiente manera:

    - Crédito de cancelación = ((precio mensual*12)/365) *días que quedan en el período de 12 meses * número de licencias canceladas.

**P:** ¿Qué sucede si el precio de una oferta disminuye durante el período de 12 meses de una suscripción facturada anualmente? 

-   **R:** No hay ningún cambio. El precio está establecido para el período de 12 meses completo. Esto también ocurre en la facturación mensual.


<a href="" id="reporting"></a>**Generación de informes**

**P:** ¿Dónde puedo averiguar si una suscripción se factura anual o mensualmente?   

-   **R:** El archivo de conciliación basada en licencia incluirá la información sobre la frecuencia de facturación. Puedes encontrarla en la columna AA

**P:** ¿Qué cambios veré en el archivo de conciliación basada en licencia cuando la suscripción con facturación anual se adquiere o renueva?  

-   **R:** El primer cambio será una nueva fila en el archivo de conciliación basado en licencia en la primera fecha de facturación después de realizar la compra o una nueva suscripción. activado. Si no se realizan cambios en la suscripción, no aparecerán filas en los archivos de conciliación de los meses del dos al doce del período de suscripción. el próximo cambio en el archivo de conciliación aparecerá cuando se renueve la suscripción. Esto aparecerá en la primera fecha de facturación después de la renovación. Si se realiza un cambio en la suscripción durante el período de 12 meses, aparecerán un crédito y una renovación prorrateada en el siguiente archivo de conciliación después de realizar el cambio.

**P:** ¿Cómo la compra, el cambio o la cancelación de una suscripción anual aparecerán en la columna P de los archivos de uso?

-   **R:** El cargo de compra inicial aparece como "Tarifas prorrateadas al comprar". Los cambios en las licencias que dan lugar a crédito y renovación aparecen como "Prorrateo de instancia de ciclo". Los créditos de cancelación aparecen como "Cuota de cancelación".

**P:** Cuando se cancela una suscripción anual, ¿cómo se refleja en el archivo de conciliación?   

-   **R:** El archivo de conciliación contendrá un elemento de línea para un crédito de cancelación. Si la cancelación se produce en los primeros 30 días del período de 12 meses, la suscripción será abonada al 100 por ciento. Si la cancelación se produce después de los primeros 30 días, la suscripción se abonará de forma prorrateada.

**P:** ¿Qué aspecto tiene el archivo de conciliación cuando se agregan licencias a una suscripción que tiene facturación anual?  

-   **R:** El archivo de conciliación contendrá un crédito y una renovación prorrateada. Esto también ocurre en la suscripción con facturación mensual.

**P:** ¿Qué aspecto tiene el archivo de conciliación cuando se eliminan licencias de una suscripción con facturación anual? 

-   **R:** El archivo de conciliación contendrá un crédito y una renovación prorrateada.  Esto también ocurre en la suscripción con facturación mensual.

**P:** ¿El precio anual se muestra en la lista de precios? 

-   **R:** No. La lista de precios muestra el precio mensual. El precio anual se puede calcular multiplicando el precio mensual por doce.

**P:** ¿La matriz de ofertas tiene distintas entradas de ofertas que pueden facturarse anualmente?   

-   **R:**  No. Los identificadores de ofertas son los mismos que para todas las frecuencias de facturación. No hay identificadores de oferta exclusivos para la facturación anual.


<a href="" id="incentives"></a>**Incentivos**

**P:** ¿Con qué frecuencia se calculan los incentivos en las suscripciones anuales? 

-   **R:** Se calculan en función de los ingresos facturados. Los pagos de los incentivos ganados serán acordes con nuestra directiva que se encuentran en nuestras guías de incentivos de CSP. 

**P:** ¿Cómo se pagan los incentivos en las suscripciones facturadas anualmente?  

-   **R:** Actualmente todos los pagos de incentivos se realizan dos veces al año. Los pagos se realizan 45 días después del final de cada semestre.

**P:** Cuando se vende una suscripción facturada anualmente, ¿cómo se reconocerán los ingresos de dicha suscripción para el cálculo de los incentivos? ¿Se basará en los ingresos facturados o ajustados? 

-   **R:** Los cálculos para incentivos se basarán en los ingresos facturados.

**P:** ¿De qué modo se calculan las ganancias de incentivos en la suscripción facturada anualmente apta a través de los distintos tipos de incentivos de CSP (tasas de incentivos globales, tasas de aceleración local y campañas locales)?

-   **R:** Independientemente de cómo se factura una suscripción, ya sea mensual o anualmente, los partners obtienen incentivos de todas las transacciones aptas. Esto incluye la tasa de incentivos globales que se aplica a los ingresos facturados durante el período, el acelerador local de todas las regiones en las que existen aceleradores locales) y cualquier campaña global cuando corresponda.

**P:** ¿Con quién te puedes poner en contacto si tienes preguntas sobre los incentivos?

-   **R:** Ponte en contacto con el equipo de soporte técnico de incentivos regionales adecuado:

    - Norteamérica: ocina@microsoft.com

    - América Latina y Brasil: ocilatam@microsoft.com

    - EMEA: ociemea@microsoft.com

    - APOAC (excepto Japón): ociapgc@microsoft.com

    - Japón: ocijp@microsoft.com


**P:** ¿Qué sucede si suspendo mi suscripción? 

-   **R:** Si suspendes una suscripción, en el Centro de partners o a través de la API, antes de 30 días desde la fecha de compra, recibirás un crédito del 100%, independientemente de la frecuencia de facturación. 

    Con la facturación anual, tendría este aspecto:

    - Suscripción de compras del partner del 1 de enero = línea de facturación de cargo creada para el periodo de servicio 1/1 - 31/12.
    - Suspende la suscripción el 25 de enero = línea de facturación de crédito creada para el periodo de servicio 1/1 - 31/12.
    - Se reactiva el 29 de enero = línea de facturación de cargo creada para el periodo de servicio 1/29 - 31/12.

    Con la facturación mensual, tendría este aspecto:

    - Suscripción de compras del partner del 1 de enero = línea de facturación de cargo creada para el periodo de servicio 1/1 - 31/1.
    - Suspende la suscripción el 25 de enero = línea de facturación de crédito creada para el periodo de servicio 1/1 - 31/1.
    - Se reactiva el 29 de enero = línea de facturación de cargo creada para el periodo de servicio 1/29 - 31/1.



## <a href="" id="freetrialsfaq"></a>Preguntas frecuentes sobre evaluaciones gratuitas

**P:** ¿Qué son evaluaciones gratuitas?

-   **R:** Puedes ofrecer a tus clientes una evaluación gratuita de 30 días en determinados productos. Esto permite a los clientes evaluar el producto antes de comprarlo. Hay evaluaciones disponibles para los siguientes productos: 

    - Office 365 Empresa Premium  
    - Office 365 E3  
    - Office 365 E5 sin PSTN  
    - Office 365 E5 sin PSTN  
    - Enterprise Mobility & Security E5  
    - Plan Dynamics 365 Customer Engagement 1  
    - Dynamics 365 for Financials  
    
**P:** ¿Se elimina el período gratuito con la entrega de las evaluaciones gratuitas?

-   **R:** No, las suscripciones con facturación mensual seguirán teniendo un período gratuito. Sin embargo, no habrá ningún período gratuito para la facturación anual.

**P:** La alineación de facturación se ha retrasado hasta el primer trimestre de CY18. ¿Cómo afecta esto al período gratuito y a la facturación en general?

-   **R:** Las nuevas suscripciones con facturación mensual seguirán recibiendo un período gratuito y se alinean con la fecha de facturación del partner. Las suscripciones con facturación anual no ofrecerán un período gratuito y se alinean con la fecha de compra. Los partners seguirán recibiendo su factura y los archivos de conciliación en su fecha de facturación mensual, que contendrán la actividad de facturación de suscripciones mensuales y anuales.

**P:¿** ¿Cuándo se eliminará el período gratuito de las suscripciones con frecuencia de facturación mensual?

-   **A:** CY18 Q1.

**P: ¿** ¿Son la facturación anual y las evaluaciones gratuitas diferentes en la nube soberana frente a la nube pública?

-   **R:** No. Son iguales. La única diferencia serán las SKU de prueba que están disponibles en el momento de inicio.

**P:** ¿Cuándo esto estará disponible para las SKU enumeradas anteriormente?

-   **A:** 17 de octubre de 2017.

**P:** ¿Quién puede participar?

-   **R:** Todos los partners pueden participar. Sin embargo, no está disponible actualmente en China. Las evaluaciones gratuitas estarán disponibles para los clientes y partners chinos antes de finales de 2017. 

**P:** ¿Qué acciones debo realizar para sacar partido de estas evaluaciones gratuitas?

-   **R:** Considera cómo la evaluación gratuita puede incorporarse en tu ritmo de ventas y el impacto que tendrá en tus procesos internos. También puede ser necesario modificar las API para incluir la conversión de una evaluación gratuita a una suscripción de pago. Hay especificaciones técnicas detalladas para cambios de API en la vista Anuncios del Centro de partners.

**P:** ¿Veré la evaluación gratuita en mi factura y el archivo de conciliación?

-   **R:** No, las evaluaciones gratuitas no aparecerán en tu factura ni en el archivo de conciliación basado en licencia. Aparecerá en tu factura y en el archivo de conciliación basada en licencia después de convertir una evaluación de prueba en una suscripción de pago. La suscripción convertida aparecerá en la factura y en el archivo de conciliación basada en licencia de la misma forma que en cualquier otra suscripción nueva.

**P:** ¿Las evaluaciones de prueba afectan a los incentivos?

-   **R:** No. La evaluación gratuita no tiene ningún efecto en los incentivos.

**P:** ¿Estarán disponibles las evaluaciones gratuitas para los demás productos de Office y CSP adicionales en el futuro?

-   **R:** No lo sabemos aún. Proporcionamos evaluaciones gratuitas de estos productos porque son las ofertas de empresa más completas y populares. Podemos agregar ofertas adicionales de evaluación gratuita en el futuro.

**P:** ¿Puede un cliente tener más de una evaluación gratuita?

-   **R:** Cada cliente tiene derecho a una evaluación gratuita por oferta disponible.

**P:** ¿Hay límites para una evaluación gratuita?

-   **R:** Sí. La evaluación gratuita es para un máximo de 25 licencias. El número de licencias no se puede cambiar durante el período de prueba. Una vez que la evaluación se convierte en una suscripción de pago, puedes agregar licencias adicionales a la suscripción.

**P:** ¿Una evaluación gratuita se convierte automáticamente en una suscripción de pago?

-   **R:** No. Tendrás que convertir tú mismo la suscripción en el Centro de partners o a través de la API.

**P:** ¿Pueden usarse las evaluaciones gratuitas en suscripciones facturadas tanto mensualmente como anualmente?

-   **R:** Sí. Puedes elegir la frecuencia de facturación al convertir la evaluación gratuita en una suscripción de pago.

**P:** ¿La fecha de inicio de la suscripción se basará en la fecha de inicio de la evaluación gratuita o en la fecha en que se convierte en una suscripción de pago? 

-   **R:** La fecha de inicio se basa en la fecha del cambio. Si la evaluación gratuita se convierte en una oferta de pago con facturación anual, la fecha de renovación de suscripción será de doce meses desde la fecha de conversión. R: Si la evaluación gratuita se convierte en una oferta pagada con facturación mensual, la fecha de renovación de suscripción será de doce meses desde la fecha de facturación tras la fecha de conversión.

**P:** ¿Podemos agregar o quitar puestos durante la evaluación gratuita?

-   **R:** No. Las evaluaciones gratuitas tendrán 25 licencias de manera predeterminada y no se pueden actualizar.

**P:** ¿Hay pruebas para ofertas de complementos como ATP y RTC?

-   **R:** No hay evaluaciones gratuitas para ninguna oferta de complementos.

**P:** ¿Puedo ofrecer una evaluación gratuita de una oferta que ya posee un cliente?

-   **R:** No. Si la oferta ya pertenece al cliente no puede usarse para una evaluación gratuita.

**P:** ¿Podré ver todas mis ofertas de prueba pendientes?

-   **R:** Sí. La página de cliente muestra todas las suscripciones. Aquí se incluyen la suscripción de evaluación gratuita y la suscripción de pago.

**P:** ¿Se me notificará sobre evaluaciones gratuitas que van a caducar?

-   **R:** No. Puedes realizar un seguimiento de las fechas de caducidad próximas desde la vista del cliente en el Centro de partners, o puedes consultar la API. Se recomienda supervisar esas fechas con frecuencia para poder realizar las acciones de seguimiento apropiadas con los clientes que se acercan a la fecha de caducidad.

**P:** ¿Si un cliente ha tenido una evaluación gratuita para una oferta también puede usar otra evaluación para otra oferta? 

-   **R:** Sí. Los clientes pueden registrarse para una versión de evaluación por oferta. Por ejemplo, pueden obtener una evaluación gratuita para Office 365 Empresa Premium y una evaluación gratuita para Office 365 E3.

**P:** ¿Qué ocurre cuando finaliza el período de evaluación? ¿Mi cliente o yo recibiremos una notificación? ¿Qué notificaciones aparecen al intentar iniciar sesión en una versión de evaluación que ha caducado?

-   **R:** Una vez que ha caducado una evaluación, un cliente que intenta iniciar sesión en esa versión de evaluación verá un mensaje que indica que ha terminado el período de evaluación. No habrá notificaciones para indicar que una evaluación caduca pero como partner puedes realizar un seguimiento a través de la vista de clientes o a través de consultas en la API.

**P:** ¿Se puede extender una evaluación?

-   **R:** No. La versión de evaluación debe convertirse en una versión de pago o caducará después de 30 días.

**P:** Cuando una versión de evaluación caduca, ¿se puede acceder a la información de la versión de evaluación?

-   **R:** Sí. Los datos se almacenan en línea con estándares de retención de datos. Cuando hayas comprado una nueva suscripción con los mismos planes de servicio, se pueden acceder a los datos desde la suscripción recientemente activada.

**P:** ¿Las evaluaciones gratuitas están disponibles para ofertas de gobierno y educación?

-   **R:** En este momento no hay evaluaciones gratuitas para ofertas de gobierno y educación.

**P:** ¿Pueden convertirse las evaluaciones gratuitas de clientes del programa Proveedor de soluciones en la nube (CSP) en otras suscripciones de programa, tales como EA, Open o MOSP? 

-   **R:** No. No se pueden transferir las suscripciones de CSP a otro programa.

**P:** ¿Cómo puedo obtener soporte técnico en evaluaciones gratuitas? 

-   **R:** Envía una solicitud de servicio a través del Centro de partners.

## <a href="" id="billingalignmentfaq"></a>Alineación de facturación: finalización del período gratuito

El 20 de febrero, el Programa CSP implementará la "alineación de fechas de facturación" para las nuevas suscripciones con una frecuencia de facturación mensual. Esta "alineación de fechas de facturación" proporcionará a los partners más flexibilidad y capacidad de previsión para las ventas y facturación, así como para el aprovisionamiento y la administración de planes de clientes. Las suscripciones adquiridas antes del 20 de febrero obtienen un período gratuito a partir de la fecha de la compra hasta la fecha de facturación del partner. Las suscripciones adquiridas después del 20 de febrero ya no recibirán un período gratuito. El período pagado de 12 meses comenzará (alineará) en la fecha de la compra frente a la fecha de facturación del partner. Los partners ya no verán una "línea de facturación de 0$" que representa el período gratuito en el archivo de conciliación. No hay ningún cambio en las API, facturación o incentivos.  Los partners deben informar a sus equipos de ventas y de contabilidad de esta nueva lógica de facturación y asegurarse de que las operaciones se ajustan según sea necesario.  

Antes de implementar la alineación de fechas de facturación, hemos facturado y realizado el cargo en la fecha de aniversario de facturación del partner, la fecha en la que el partner se registró en el programa CSP; no en la fecha de aniversario de suscripción del cliente, la fecha en que el cliente adquirió su suscripción. Después del 20 de febrero, los partners recibirán el cargo en su fecha de aniversario de suscripción, lo que elimina este período gratuito.  Los partners seguirán recibiendo facturas en su fecha de aniversario de facturación, pero la fecha de vigencia de la factura será la fecha de aniversario de suscripción del cliente. 

Las suscripciones que se encuentran en el período gratuito el 20 de febrero no recibirán ningún cargo entre la fecha de compra y la fecha de facturación del partner. Además, no se realizará el cargo durante el primer mes del período de pago de 12 meses. Si usas un archivo de conciliación para realizar la verificación, ten en cuenta que el cargo de este primer mes dejará de estar visible en el archivo de conciliación.  

No hay ningún cambio en las API, facturación o incentivos como resultado de este cambio de lógica de facturación. Informa a los equipos de ventas y de contabilidad de esta nueva lógica de facturación y asegúrate de que ajustan las operaciones según sea necesario. Consulta las siguientes Preguntas frecuentes con escenarios de facturación detallados.  


**P1:** ¿Qué está cambiando con la fecha de facturación?

-   **R:** Las suscripciones basadas en licencia ya no tendrán un período gratuito. Actualmente, existe un período gratuito desde la fecha de compra hasta la fecha de facturación del partner.

**P2:** ¿Cuándo se eliminará el período gratuito?

- **R:** A partir del 20 de febrero de 2018, las nuevas suscripciones no tendrán un período gratuito.

**P3:** ¿Cuál será el impacto de las suscripciones en el período gratuito el 20 de febrero?

- **R:** Las suscripciones que están en el período gratuito el 20 de febrero de 2018 seguirán recibiendo un período gratuito desde la fecha de la compra hasta la fecha de facturación del partner. Estas licencias también recibirán un "período gratuito ampliado" y no se realizará el cargo durante el primer mes del período de pago de 12 meses. El "período gratuito ampliado" no se aplicará a licencias agregadas en el primer mes. Si aumentas la cantidad de licencias en el primer mes, se te cobrará por aquellas licencias agregadas en la siguiente factura/conciliación. Si el archivo de conciliación se usa para realizar la verificación, ten en cuenta que puede que el cargo de este primer mes no aparezca en el archivo de conciliación. Consulta los siguientes escenarios para obtener una explicación más detallada.

**P4:** ¿Cuándo comenzará el período de pago de 12 meses para una nueva suscripción?

- **R:** Actualmente, el período de pago comienza en la fecha de facturación del partner después de la fecha de compra. A partir del 20 de febrero de 2018, el período de pago para las nuevas suscripciones comenzará en la fecha de compra.

**P5:** ¿Cuándo se renovarán automáticamente las suscripciones?

- **R:** Las suscripciones se renuevan automáticamente 12 meses después de la primera fecha de facturación. Actualmente, esto significa que las suscripciones se renuevan automáticamente 12 meses después de la primera fecha de facturación del partner después de la fecha de compra. A partir del 20 de febrero de 2018, las nuevas suscripciones se renovarán automáticamente 12 meses después de la fecha de compra.

**P6:** ¿Y si adquiero la suscripción el día 29, 30 o 31 del mes?

- **R:** La suscripción estará disponible desde la fecha de compra, pero el período de pago de 12 meses no comenzará hasta el primer día del mes siguiente.

**P7:** ¿Qué ofertas se ven afectadas?

- **R:** La eliminación del período gratuito se aplica a todas las suscripciones basadas en licencia de CSP.

**P8:** ¿Cómo afecta esto al archivo de conciliación y facturación? 

- **R:** Ya no se verá la "línea de facturación de 0$" en el archivo de conciliación ni en el de facturación. Actualmente, la línea de facturación de $0 representa el período gratuito.

**P9:** ¿Cambiará la fecha de facturación?

- **R:** No, seguirás recibiendo el archivo de conciliación y facturación en la fecha de facturación existente.

**P10:** ¿Cambiarán las fechas de inicio y finalización de cargos mensuales para las suscripciones existentes?

- **R:** No, las fechas de inicio y finalización de cargos mensuales de las suscripciones existentes seguirán alineándose con la fecha de facturación. Sin embargo, las nuevas suscripciones se alinearán con la fecha de compra. Consulta el ejemplo que se indica a continuación.

**P11:** ¿Cambiará el cálculo de incentivos?

- **R:** No, no hay ningún cambio en los cálculos de incentivos.

**P12:** ¿Habrá algún cambio en las API?

- **R:** No, no hay ningún cambio en las API.

### <a name="common-scenarios"></a>Escenarios comunes


|**Escenarios**   |**Escenario 1: El período gratuito de suscripción finaliza antes del 20 de febrero de 2018**   |**Escenario 2: La suscripción se encuentra en el período gratuito el 20 de febrero de 2018**  | **Escenario 3: La suscripción se adquiere el 20 de febrero de 2018 o en una fecha posterior**   |
|----------|:------------|:--------------------|:------------|
|Fecha de compra |1 de febrero de 2018    | 1 de febrero de 2018    | 1 de junio de 2018     |
|Fecha de aprovisionamiento | 1 de febrero de 2018   |1 de febrero de 2018   |1 de junio de 2018   |
|Fecha de facturación   | Decimoquinto día de cada mes   |Vigésimo quinto día de cada mes   | Decimoquinto día de cada mes|
|Período gratuito   | 1 de febrero de 2018-14 de febrero de 2018|1 de febrero de 2018-24 de febrero de 2018   |Sin período gratuito|
|Cargo mes 1   | 15 de febrero de 2018-14 de marzo de 2018 | Las licencias vigentes el 24 de febrero de 2018 recibirán un período gratuito ampliado hasta el 24 de marzo de 2018. Se te cobrarán las licencias agregadas después del 24 de febrero de 2018. |1 de junio de 2018 - 30 de junio de 2018   |
|Cargo mes 2   | 15 de marzo de 2018 - 14 de abril de 2018|25 de marzo de 2018 - 24 de abril de 2018   |1 de julio de 2018 - 31 de julio de 2018|
|Comienza el período de pago   | 15 de febrero de 2018 | 25 de febrero de 2018| 1 de junio de 2018| 
|Finaliza el período de pago | 14 de febrero de 2019   |24 de febrero de 2019   | 31 de mayo de 2019  |
|Fecha de renovación | 15 de febrero de 2019 |25 de febrero de 2019   |1 de junio de 2019|

### <a name="scenario-4---new-purchase"></a>Escenario 4: Nueva compra

La fecha de facturación del partner es el decimoquinto día del mes. El 1 de junio de 2018 el partner adquiere una nueva suscripción. El precio de la suscripción es 30$ por licencia al mes. 

El 15 de junio el archivo de conciliación contendrá solo las siguientes líneas de facturación:

- Cargo de 30$ para el período de servicio comprendido entre el 1 y el 30 de junio

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------------|
|01/06/2018   |30/06/2018   |30 $   |1   |30$   |Tarifas prorrateadas al comprar |

### <a name="scenario-5a-suspend-and-reactivate-before-billing-date"></a>Escenario 5a: Suspender y volver a activar antes de la fecha de facturación

La fecha de facturación del partner es el decimoquinto día del mes. El 1 de junio de 2018 el partner adquiere una nueva suscripción. El precio de la suscripción es 30$ por licencia al mes. El 5 de junio de 2018, el partner suspende la suscripción. El 10 de junio de 2018, el partner vuelve a activar la suscripción. El 15 de junio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30$ para el período de servicio comprendido entre el 1 y el 30 de junio. 
- Crédito de cancelación de -30$ para el período de servicio comprendido entre el 5 y el 30 de junio. El crédito no se prorratea porque la suscripción se suspendió en los primeros 30 días. 
- Cargo de 30$ para el período de servicio comprendido entre el 10 y el 30 de junio. El cargo no se prorratea porque la suscripción se volvió a activar en los primeros 30 días. 

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01/06/2018   |30/06/2018   |30 $   |1   |30 $   |Tarifas prorrateadas al comprar |
|05/06/2018   |30/06/2018   |-30 $   |1   |30$   |Cuota de cancelación |
|10/06/2018   |30/06/2018   |30 $   |1   |30$   |Tarifa de activación |

Ten en cuenta que cuando se suspende una suscripción y vuelve a activarse, la fecha de renovación automática seguirá siendo 12meses desde la fecha de compra original.

### <a name="scenario-5b-suspend-and-reactivate-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Escenario 5b: Suspender y volver a activar después de la fecha de facturación pero menos de 30 días desde la fecha de la compra

La fecha de facturación del partner es el decimoquinto día del mes. El 1 de junio de 2018 el partner adquiere una nueva suscripción. El precio de la suscripción es 30$ por licencia al mes. El 20 de junio de 2018, el partner suspende la suscripción. El 25 de junio de 2018, el partner vuelve a activar la suscripción. El 15 de junio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30$ para el período de servicio comprendido entre el 1 y el 30 de junio. 

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01/06/2018   |30/06/2018   |30 $   |1   |30$   |Tarifas prorrateadas al comprar |

El 15 de julio el archivo de conciliación contendrá las siguientes líneas de facturación:
- Crédito de cancelación de -30$ para el período de servicio comprendido entre el 20 y el 30 de junio. El crédito no se prorratea porque la suscripción se suspendió en los primeros 30 días.
- Cargo de 30$ para el período de servicio comprendido entre el 25 y el 30 de junio. El cargo no se prorratea porque la suscripción se volvió a activar en los primeros 30 días.
- Cargo de 30$ para el período de servicio comprendido entre el 1 y el 31 de julio.

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20/06/2018   |30/06/2018   |-30 $   |1   |-30$   |Cuota de cancelación |
|25/06/2018   |30/06/2018   |30 $   |1   |30$   |Tarifa de activación |
|01/07/2018   |31/07/2018   |30 $   |1   |30$   |Tarifa de ciclo |

### <a name="scenario-5c-suspend-and-reactivate-different-license-quantity-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Escenario 5c: Suspender y volver a activar (otra cantidad de licencias) después de la fecha de facturación pero menos de 30 días desde la fecha de la compra

La fecha de facturación del partner es el decimoquinto día del mes. El 1 de junio de 2018 el partner adquiere una nueva suscripción. El precio de la suscripción es 30$ por licencia al mes. El 20 de junio de 2018, el partner suspende la suscripción. El 25 de junio de 2018, el partner vuelve a activar la suscripción con dos licencias. El 15 de junio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30$ para el período de servicio comprendido entre el 1 y el 30 de junio. 

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01/06/2018   |30/06/2018   |30 $   |1   |30$   |Tarifas prorrateadas al comprar |

El 15 de julio el archivo de conciliación contendrá las siguientes líneas de facturación:
- Crédito de cancelación de -30$ para el período de servicio comprendido entre el 20 y el 30 de junio. El crédito no se prorratea porque la suscripción se suspendió en los primeros 30 días.
- Cargo de 30$ para el período de servicio comprendido entre el 25 y el 30 de junio. El cargo no se prorratea porque la suscripción se suspendió en los primeros 30 días.
- Crédito de -30$ para el período de servicio comprendido entre el 1 y el 30 de junio. El partner vuelve a activar la suscripción con otra cantidad de licencias, lo que se traduce en un crédito y renovaciones prorrateadas.
- Renovación prorrateada de 24$ para el período de servicio comprendido entre el 1 y el 24 de junio. El partner tenía 1 licencia durante este período de servicio. Aunque se ha suspendido la suscripción desde el 20 de junio hasta el 24 de junio, el cliente seguirá recibiendo el cobro durante estos días. El precio unitario se calcula como sigue: (precio mensual o número de días en período de servicio total)*número de días en período de servicio prorrateado*número de licencias = (30/30)*24*1 = 24$.
- Renovación prorrateada de 12$ para el período de servicio comprendido entre el 25 y el 30 de junio. El partner tenía 2 licencias durante este período de servicio. El precio unitario se calcula como (30/30)*6*2= 12$.
- Cargo de 60$ para el período de servicio comprendido entre el 1 y el 31 de julio.

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20/06/2018   |30/06/2018   |-30 $   |1   |-30 $   |Cuota de cancelación |
|25/06/2018   |30/06/2018   |30 $   |1   |30$   |Tarifa de activación |
|01/06/2018   |30/06/2018   |-30 $   |1   |-30$   |Prorrateo de instancia de ciclo |
|01/06/2018   |24/06/2018   |24$   |1   |24$   |Prorrateo de instancia de ciclo |
|25/06/2018   |30/06/2018   |6$   |2   |12$   |Prorrateo de instancia de ciclo |
|01/07/2018   |31/07/2018   |30 $   |2   |60$   |Tarifa de ciclo |

### <a name="scenario-6-subscription-suspension-less-than-30-days-after-purchase-and-reactivation-more-than-30-days-after-purchase"></a>Escenario 6: Suspensión de una suscripción en menos de 30 días después de la compra y reactivación después de 30 días después de la compra 

La fecha de facturación del partner es el decimoquinto día del mes. El 1 de junio el partner adquiere una nueva suscripción de una licencia a 30$ al mes. El 5 de junio, el partner suspende la suscripción. El 15 de junio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30$ para el período de servicio comprendido entre el 1 y el 30 de junio
- Crédito de cancelación de -30$ para el período de servicio comprendido entre el 5 y el 30 de junio. El crédito no se prorratea porque la suscripción se suspendió en los primeros 30 días.

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|01/06/2018   |30/06/2018   |30 $   |1   |30$   |Tarifas prorrateadas al comprar
|05/06/2018   |30/06/2018   |-30 $   |1   |-30$   |Cuota de cancelación

El 10 de julio, el partner vuelve a activar la suscripción. El 15 de julio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de reactivación 21,30$ para el período de servicio comprendido entre el 10 y el 31 de julio. Las reactivaciones después de 30 días desde la fecha de compra se traducen en un cargo prorrateado. 

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|10/07/2018   |31/07/2018   |21,30$   |1   |21,30$   |Tarifa de activación |

El 15 de agosto el archivo de conciliación contendrá las siguientes líneas de facturación:
- Cargo de 30$ para el período de servicio comprendido entre el 1 y el 31 de agosto.

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/08/2018   |31/08/2018   |30$   |1   |30$   |Tarifa de ciclo |

Ten en cuenta que cuando se suspende una suscripción y vuelve a activarse, la fecha de renovación automática seguirá siendo 12meses desde la fecha de compra original. 

### <a name="scenario-7-subscription-suspension-and-reactivation-more-than-30-days-after-purchase"></a>Escenario 7: Suspensión y reactivación de una suscripción en más de 30 días después de la compra 
La fecha de facturación del partner es el decimoquinto día del mes. El 1 de junio el partner adquiere una nueva suscripción de una licencia a un precio de 30$ al mes. 

El 15 de junio el archivo de conciliación contendrá solo las siguientes líneas de facturación:

- Cargo de 30$ para el período de servicio comprendido entre el 1 y el 30 de junio.

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|01/06/2018   |30/06/2018   |30 $   |1   |30$   |Tarifas prorrateadas al comprar |

El partner suspende la suscripción el 5 de julio pero la vuelve a activar el 15 de julio. El 15 de julio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30$ para el período de servicio comprendido entre el 1 y el 31 de julio.
- Crédito de cancelación de -26,14$ para el período de servicio comprendido entre el 5 y el 31 de julio. Las cancelaciones después de 30 días desde la fecha de compra se traducen en un crédito prorrateado. Cálculo = (precio mensual/días en período de servicio total) x días del período de servicio prorrateado x cantidad de licencias x (-1) = (30/31) x 27 x 1 x (-1) =-26,14.
- Cargo de reactivación 21,30$ para el período de servicio comprendido entre el 10 y el 31 de julio. Las reactivaciones después de 30 días desde la fecha de compra se traducen en un cargo prorrateado. Cálculo = (30/31) x 22 x 1 = 21,30.

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/07/2018   |31/07/2018   |30 $  |1   |30$   |Tarifa de ciclo |
|05/07/2018   |31/07/2018   |   -26,14$   |1   |-26,14$|Cuota de cancelación |
|10/07/2018   |31/07/2018   |-21,30$   |1   |21,30$|Tarifa de activación |

El archivo de conciliación del 15 de agosto contendrá lo siguiente:
- Cargo de 30$ para el período de servicio comprendido entre el 1 y el 31 de agosto.

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/08/2018   |31/08/2018   |30$  |1   |30$   |Tarifa de ciclo |

### <a name="scenario-8-change-of-license-quantity"></a>Escenario 8: Cambiar cantidad de licencias 

La fecha de facturación del partner es el 15. El 1 de junio el partner adquiere una nueva suscripción por 30 $ al mes. El 10 de junio el partner aumenta la cantidad de licencias de 1a 2 licencias. El 15 de junio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30$ para el período de servicio comprendido entre el 1 y el 30 de junio. Aunque el partner aumentó la cantidad de licencias antes de la fecha de facturación del 15 de junio, el cambio no se reconoce en el sistema de facturación de Microsoft hasta el día de aniversario de suscripción el 1 de julio.

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/06/2018   |30/06/2018   |30 $   |1   |30$   |Tarifas prorrateadas al comprar |

El 1 de julio, el día de aniversario de la suscripción, el sistema de facturación de Microsoft reconocerá que la cantidad de licencias se cambió de 1a 2 el 10 de junio. El sistema de facturación generará un crédito y renovaciones prorrateadas para el período de servicio comprendido entre el 1 y el 9 de junio y el 10 y el 30 de junio. 

El archivo de conciliación del 15 de julio contendrá lo siguiente:

- Crédito de -30$ para el período de servicio comprendido entre el 1 y el 30 de junio.
- Renovación prorrateada de 9$ para el período de servicio comprendido entre el 1 y el 9 de junio. Se trata del período cuando el cliente tenía 1 licencia. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (30/30) x 9 x 1 = 9.
- Renovación prorrateada de 42$ para el período de servicio comprendido entre el 10 y el 30 de junio. Se trata del período cuando el cliente tenía 2 licencias. Cálculo = (30/30) x 21 x 2 = 42.
- Cargo de 60$ para el período de servicio comprendido entre el 1 y el 31 de julio.

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/06/2018   |30/06/2018   |-30 $   |1   |-30$|Prorrateo de instancia de ciclo |
|01/06/2018   |09/06/2018   |9 $   |1   |9$|Prorrateo de instancia de ciclo |
|10/06/2018   |30/06/2018   |21 $   |2   |42$|Prorrateo de instancia de ciclo |
|01/07/2018   |31/07/2018   |30 $   |2   |60$   |Tarifa de ciclo |

### <a name="scenario-9-add-on-subscriptions"></a>Escenario 9: Suscripciones de complemento

La fecha de facturación del partner es el decimoquinto día del mes. El 1 de junio el partner adquiere una nueva suscripción de una licencia a un precio de 30$ al mes. El 10 de junio el partner adquiere una nueva suscripción de complemento por 5$ al mes. La fecha de renovación de suscripción de complemento se alinea con la fecha de renovación de suscripción base que es el 1 de junio. 

El 10 de junio el partner adquiere una suscripción de complemento de una licencia a un precio de 5$ al mes. 

El 15 de junio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30$ para el período de servicio comprendido entre el 1 y el 30 de junio. Se trata de la suscripción base.
- Cargo prorrateado de 3,50$ para el período de servicio comprendido entre el 10 y el 30 de junio. Se trata de la suscripción de complemento. 

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/06/2018   |30/06/2018   |30 $   |1   |30$   |Tarifas prorrateadas al comprar |
|10/06/2018   |30/06/2018   |3,50USD   |1   |3,50$   |Tarifas prorrateadas al comprar |

El 15 de julio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30$ para el período de servicio comprendido entre el 1 y el 31 de julio. Se trata de la suscripción base.
- Cargo de 5$ para el período de servicio comprendido entre el 1 y el 31 de julio. Se trata de la suscripción de complemento.

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|-------|
|01/07/2018   |31/07/2018   |30 $   |1   |30$   |Tarifa de ciclo |
|01/07/2018   |31/07/2018   |5 $   |1   |5$   |Tarifa de ciclo |

Ten en cuenta que la suscripción de complemento tendrá una fecha de renovación automática de 1 de junio de 2019, que se alinea con la de suscripción base.

### <a name="scenario-10-new-purchase-on-the-29th-30th-or-31st"></a>Escenario 10: Nueva compra el 29, 30 o 31 

La fecha de facturación del partner es el decimoquinto día del mes. El 29 de mayo el partner adquiere una nueva suscripción de una licencia a un precio de 30$ al mes. Las suscripciones adquiridas el 29, 30 o 31 tendrán un período gratuito desde la fecha de compra hasta el primer día del mes siguiente. El día de aniversario de suscripción predeterminado será el 1. En este escenario, la suscripción recibirá un período gratuito desde el 29 de mayo hasta el 31 de mayo y el período de pago de 12meses comenzará el 1 de junio. 

El 15 de junio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30$ para el período de servicio comprendido entre el 1 y el 30 de junio.

|**Inicio del cargo**   |**Finalización del cargo**   |**Precio unitario**   |**Cantidad**   |**Importe**   |**Tipo de cargo** |
|-----------------|:-------------|:----------------|:------------|:------|------|
|01/06/2018   | 30/06/2018   |30 $   |1   |30$  |Tarifas prorrateadas al comprar |

Ten en cuenta que la suscripción se renovará automáticamente el 1 de junio de 2019.
