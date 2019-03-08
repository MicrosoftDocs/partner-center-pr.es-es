---
title: Preguntas frecuentes sobre las nuevas características de facturación | Centro de partners
ms.topic: article
ms.date: 10/29/2018
Description: A continuación se incluyen algunas de las preguntas frecuentes relacionadas con las características de evaluación gratuita y facturación anual del Centro de partners.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: de8b450edace9aea1fbf5321159f41bf26420488
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/05/2019
ms.locfileid: "57587228"
---
# <a name="faq-about-new-billing-features"></a>Preguntas frecuentes sobre las nuevas características de facturación

**Se aplica a**

-  Centro de partners
-  Centro de partners para Microsoft Cloud for US Government


A continuación se incluyen algunas de las preguntas frecuentes relacionadas con las características de evaluación gratuita y facturación anual del Centro de partners. 

## <a name="in-this-section"></a>En esta sección

-   [Preguntas más frecuentes de facturación anual](#annualbillingfaq)

-   [Evaluaciones gratuitas de preguntas más frecuentes](#freetrialsfaq)

-   [Alineación de facturación preguntas más frecuentes](#billingalignmentfaq)


## <a href="" id="annualbillingfaq"></a>Preguntas más frecuentes de facturación anual

Secciones:

[Información general y las ventajas de facturación anual](#overviewandbenefits)

[El pedido y escenarios de facturación](#placingyourorder)

[Cambiar la suscripción](#changingyoursubscription)

[Cálculo de precios](#pricingcalculation)

[Reporting](#reporting)

[Incentivos](#incentives)


<a href="" id="overviewandbenefits"></a>**Información general y las ventajas de facturación anual**

**P: ¿** ¿Qué ha cambiado?

-   **R:** En respuesta a las solicitudes, hemos introducido la opción de pagar para determinadas suscripciones de CSP en anual o mensual. Esta nueva opción comenzó a estar disponible el 17 de octubre de 2017.

**P: ¿** ¿Quién puede participar?

-   **R:** Pueden hacer uso de todos los asociados y tipos de socios de facturación anual. La facturación anual está disponible en todos los mercados donde CSP está disponible actualmente. 

**P: ¿** ¿Qué es necesario tener en cuenta al pensar en facturación anual?    

-   **R:** Debe considerar cómo se verá afectada su movimiento de ventas. Estas son algunas sugerencias que te ayudarán a usar de forma eficaz la facturación anual. 
    - Actualiza las API para dar cabida a la característica de facturación anual, si corresponde. 
    - Revisa los cambios en la factura y el archivo de conciliación basada en licencia.
    - Asegúrate de que tu equipo esté informado.
    - Actualiza tus procesos internos según sea necesario.

**P: ¿** ¿Cuáles son las ventajas de facturación anual? 

-   **R:** Facturación anual tiene las siguientes ventajas:

    - Una mayor flexibilidad en opciones de pago.

    - Una mejor alineación con la facturación de tus clientes.

    - Menor impacto de fluctuaciones de moneda.

    - Menores costos operativos de facturación.

**P: ¿** ¿Qué ofertas tendrán la opción para la facturación anual?

-   **R:** Las suscripciones basadas en una licencia más tienen la opción para la opción de facturación mensual o anual. Las suscripciones basadas en uso solo tienen la opción de facturación mensual. Podrás identificar las frecuencias de facturación disponibles para cada oferta con la columna J de la matriz de ofertas. Puedes encontrar la matriz de ofertas en la sección "Ver ofertas y precios" del Centro de partners. .

**P: ¿** ¿Es la facturación anual por suscripción o licencia?       

-   **R:** Facturación anual y mensual son por suscripción.

**P: ¿** ¿Existen cambios necesarios para las API para admitir la facturación anual?    

-   **R:** Para poder beneficiarse de facturación anual existe es algunos cambios necesarios para las API. Encontrarás más información en los siguientes artículos:

    - https://partnercenter.microsoft.com/en-us/partner/developer

    - https://msdn.microsoft.com/en-us/library/partnercenter/microsoft.store.partnercenter.models.orders.order.billingcycle.aspx 

    - Código de muestra: https://msdn.microsoft.com/en-us/library/partnercenter/mt634667.aspx 

<a href="" id="placingyourorder"></a>**El pedido y escenarios de facturación**

**P: ¿** ¿Habrá una única oferta específicamente para los pedidos con la facturación anual?   

-   **R:** No. Todas las frecuencias de facturación, incluida la opción de facturación anual, se asignan a la oferta como un atributo. Sin embargo, puedes cambiar el nombre de una oferta con un nombre más descriptivo de cliente para permitir la diferenciación.

**P: ¿** ¿Cómo se puede seleccionar facturación anual?

-   **R:** Al agregar una nueva suscripción, que se le pedirá que elija la frecuencia de facturación. Puedes elegir la opción de facturación anual en este momento. Una vez que se selecciona la facturación anual se mostrarán todas las ofertas disponibles.

**P: ¿** ¿Si se elige la facturación anual cuándo se cobrará?    

-   **R:** Se le facturará en su próxima fecha de facturación. Por ejemplo, si la fecha de facturación es el 1, y compras una suscripción con facturación anual el 29 de octubre de 2017, se te facturará el 1 de noviembre de 2017. Suponiendo que no hagas ningún cambio en la licencia, se te facturará de nuevo el 1 de noviembre de 2018. Si haces un cambio en la licencia, recibirás un crédito y una renovación en la próxima fecha de facturación. 

**P: ¿** ¿Puedo dividir una suscripción para que una parte se factura mensualmente y la otra se cobra anualmente?  

-   **R:** No. Toda la suscripción debe tener la misma frecuencia de facturación. Toda la suscripción debe tener una facturación mensual o anual.

**P: ¿** ¿Cuándo es la renovación de suscripción con la facturación anual?     

-   **R:** La fecha de renovación será doce meses después de que el servicio de la fecha de inicio. El período de servicio comienza en la fecha en que se crea la suscripción.  Por ejemplo, una suscripción creada el 10 de enero de 2018, se renovará el 10 de enero de 2019.

**P: ¿** ¿Cuándo se cobrará la renovación de una suscripción con la facturación anual? 

-   **R:** Se le facturará en la próxima fecha de facturación después de la fecha de renovación de suscripción. Por ejemplo, si compras una suscripción con facturación anual el 15 de enero de 2018 y la fecha de facturación es el 20 de enero, tu suscripción se renovará en 15 de enero de 2019. La renovación se te facturará entonces el 20 de enero de 2019.

**P: ¿** ¿Las suscripciones con la facturación anual reciben un período gratuito?

-   **R:** No, las suscripciones con la frecuencia de facturación anual no reciben un periodo gratis. El plazo pagado de 12 meses comienza en la fecha de compra. Difiere de las suscripciones con frecuencia de facturación mensual que reciben un período gratuito desde la fecha de compra hasta la próxima fecha de facturación.

**P: ¿** ¿Un cliente puede tener varias suscripciones de la oferta misma cada con distintas frecuencias de facturación?    

-   **R:** Depende de la oferta. Hay algunas ofertas que están limitadas a una suscripción por cliente. Si la oferta no está limitada, un cliente puede tener varias suscripciones de la misma oferta con diferentes frecuencias de facturación. Puedes encontrar los detalles de todos los límites y restricciones de la oferta en la columna I de la matriz de ofertas. Puedes encontrar la matriz de ofertas en la sección "Ver ofertas y precios" del Centro de partners.

<a href="" id="changingyoursubscription"></a>**Cambiar la suscripción**

**P: ¿** ¿Puedo agregar una nueva licencia a una suscripción existente que tiene la facturación anual?    

-   **R:** Sí. Puedes cambiar la cantidad de licencias de tus suscripciones en cualquier momento. Agregar licencias adicionales no afectará a la frecuencia de facturación. 

**P: ¿** ¿Puedo agregar licencias que tienen la facturación mensual a una suscripción existente que tiene la facturación anual? 

-   **R:** Una vez que compra una suscripción con la facturación anual, las licencias adicionales seguirá la misma frecuencia de facturación. Si necesitas después adquirir liencias con facturación mensual, tendrás que adquirir una nueva suscripción.

**P: ¿** ¿Puedo cambiar la frecuencia de facturación para una suscripción de mensual, anual y viceversa? 

-   **R:** Sí. Consulte **para cambiar la frecuencia de facturación de un servicio en línea** en [conceptos básicos de facturación](https://docs.microsoft.com/en-us/partner-center/billing-basics).

**P: ¿** ¿Está disponible para las ofertas de complemento facturación anual?   

-   **R:** Sí. La suscripción de complemento tendrá automáticamente la misma frecuencia de facturación que suscripción principal.

**P: ¿** ¿Cómo funcionará la facturación anual al agregar o quitar licencias? 

-   **R:** Puede agregar o quitar licencias en cualquier momento. Recibirás un crédito y una renovación prorrateada en tu próxima fecha de facturación después de cambiar el número de licencias. 

**P: ¿** ¿Qué ocurre si cancelo una suscripción con funciona la facturación anual?    

-   **R:** La directiva de cancelación es el mismo para todas las frecuencias de facturación. Si se cancela la suscripción en los primeros 30 días del plazo pagado de 12 meses, recibirás un crédito del 100 por ciento en la próxima fecha de facturación. Si se cancela la suscripción en después de 30 días del plazo pagado de 12 meses, recibirás un crédito prorrateado en la próxima fecha de facturación.

**P: ¿** ¿Un cliente puede mover una suscripción con la facturación anual de un socio a otro asociado?  

-   **R:** No. No se pueden mover suscripciones entre partners. El nuevo partner debe adquirir una nueva suscripción en nombre del cliente. Esto se aplica a las suscripciones facturadas mensualmente y anualmente.

**P: ¿** ¿Volver a activar una suscripción con la facturación anual?

-   **R:** Sí, puede reactivar la suscripción de hasta 90 días desde la fecha de suspensión. Recibirás un cargo prorrateado en la siguiente fecha de facturación. La fecha de renovación de la suscripción permanece igual.

<a href="" id="pricingcalculation"></a>**Cálculo de precios**

**P: ¿** ¿Qué ocurre si el precio de una oferta es cambia parte de la forma hasta el período de 12 meses de una suscripción de facturación anual?    

-   **R:** Para el período de suscripción de 12 meses completa garantiza que el precio de oferta en el momento de la compra. 

**P: ¿** ¿Qué precio de una suscripción será cuando renueva automáticamente tras un período de suscripción de 12 meses?    

-   **R:** Cuando se renueva una suscripción, el precio se basará en la lista de precios actual en la fecha de renovación. El nuevo precio se garantiza durante el siguiente período de suscripción de 12 meses.

**P: ¿** ¿Cómo se calcula el crédito para una licencia cancelada o una suscripción? ¿Se calcula por día o por mes?   

-   **R:** Crédito de cancelación se calcula como sigue:

    - Crédito de cancelación = ((precio mensual*12)/365) *días que quedan en el período de 12 meses * número de licencias canceladas.

**P: ¿** ¿Qué ocurre si una parte de oferta precio disminuye durante el período de 12 meses de una suscripción de facturación anual? 

-   **R:** No hay ningún cambio. El precio está establecido para el período de 12 meses completo. Esto también ocurre en la facturación mensual.


<a href="" id="reporting"></a>**Reporting**

**P: ¿** ¿Dónde puedo averiguar si una suscripción se factura mensual o anualmente?   

-   **R:** El archivo de conciliación en licencias incluirá la información sobre la frecuencia de facturación. Puedes encontrarla en la columna AA

**P: ¿** ¿Qué cambios verán en el archivo de conciliación en licencias al suscripción con la facturación anual es adquirida o renovada?  

-   **R:** El primer cambio será una nueva fila en el archivo de conciliación en licencias de la primera fecha de facturación después de la compra o una nueva suscripción. activado. Si no se realizan cambios en la suscripción, no aparecerán filas en los archivos de conciliación de los meses del dos al doce del período de suscripción. el próximo cambio en el archivo de conciliación aparecerá cuando se renueve la suscripción. Esto aparecerá en la primera fecha de facturación después de la renovación. Si se realiza un cambio en la suscripción durante el período de 12 meses, aparecerán un crédito y una renovación prorrateada en el siguiente archivo de conciliación después de realizar el cambio.

**P: ¿** ¿Cómo aparece la compra de, el cambio o cancelación de una suscripción anual en P de la columna de los archivos de uso?

-   **R:** El cargo de la compra inicial aparece como "cuotas Prorate cuando compra." Los cambios en las licencias que dan lugar a crédito y renovación aparecen como "Prorrateo de instancia de ciclo". Los créditos de cancelación aparecen como "Cuota de cancelación".

**P: ¿** ¿Cuando se cancela una suscripción anual, cómo esto aparece en el archivo de conciliación?   

-   **R:** El archivo de conciliación contendrá un elemento de línea para un crédito de cancelación. Si la cancelación se produce en los primeros 30 días del período de 12 meses, la suscripción será abonada al 100 por ciento. Si la cancelación se produce después de los primeros 30 días, la suscripción será abonada de forma prorrateada.

**P: ¿** ¿Cómo lo aparece en el archivo de conciliación si las licencias se agregan a una suscripción que tiene la facturación anual?  

-   **R:** El archivo de conciliación contendrá un crédito y la renovación prorrateado. Esto también ocurre en la suscripción con facturación mensual.

**P: ¿** ¿Cómo aparecer lion el archivo de conciliación si se quitan las licencias de una suscripción con la facturación anual? 

-   **R:** El archivo de conciliación contendrá un crédito y la renovación prorrateado.  Esto también ocurre en la suscripción con facturación mensual.

**P: ¿** ¿Es el precio anual se muestra en la lista de precios? 

-   **R:** No. La lista de precios muestra el precio mensual. El precio anual se puede calcular multiplicando el precio mensual por doce.

**P: ¿** ¿La matriz de la oferta tiene entradas diferentes para las ofertas que se pueden facturar anualmente.?   

-   **R:**  No. Los identificadores de ofertas son los mismos que para todas las frecuencias de facturación. No hay identificadores de oferta exclusivos para la facturación anual.


<a href="" id="incentives"></a>**Incentivos**

**P: ¿** ¿Con qué frecuencia se calculan los incentivos en suscripciones anuales? 

-   **R:** Calculamos en los ingresos facturado. Los pagos de los incentivos ganados serán acordes con nuestra directiva que se encuentran en nuestras guías de incentivos de CSP. 

**P: ¿** ¿Cómo se pagan incentivos en las suscripciones anuales facturados?  

-   **R:** Actualmente, todos los pagos por incentivos se realizan dos veces por año. Los pagos se realizan 45 días después del final de cada semestre.

**P: ¿** Cuando se vende una suscripción de facturación anual, cómo los ingresos de la suscripción se reconoce para el cálculo de incentivos. ¿Se basará en los ingresos facturados o ajustados? 

-   **R:** Incentivos cálculos se basan en los ingresos facturado.

**P:** ¿De qué modo se calculan las ganancias de incentivos en la suscripción facturada anualmente apta a través de los distintos tipos de incentivos de CSP (tasas de incentivos globales, tasas de aceleración local y campañas locales)?

-   **R:** Independientemente de cómo se factura una suscripción, si mensual o anualmente, socios ganar incentivos en todas las transacciones elegibles. Esto incluye la tasa de incentivos globales que se aplica a los ingresos facturados durante el período, el acelerador local de todas las regiones en las que existen aceleradores locales) y cualquier campaña global cuando corresponda.

**P: ¿** ¿Quién puede contacto si tiene preguntas acerca de los incentivos?

- **R:** Póngase en contacto con el equipo de soporte técnico adecuado de incentivos regionales:

  - Norteamérica: ocina@microsoft.com

  - América Latina y Brasil: ocilatam@microsoft.com

  - EMEA: ociemea@microsoft.com

  - APOAC (excepto Japón): ociapgc@microsoft.com

  - Japón: ocijp@microsoft.com


**P: ¿** ¿Qué ocurre si suspende mi suscripción? 

-   **R:** Si suspende una suscripción, en el centro de partners, o a través de API, dentro de 30 días de la compra, recibirá un crédito de 100%, independientemente de la frecuencia de facturación. 

    Con la facturación anual, tendría este aspecto:

    - Suscripción de compras del partner del 1 de enero = línea de facturación de cargo creada para el periodo de servicio 1/1 - 31/12.
    - Suspende la suscripción el 25 de enero = línea de facturación de crédito creada para el periodo de servicio 1/1 - 31/12.
    - Se reactiva el 29 de enero = línea de facturación de cargo creada para el periodo de servicio 1/29 - 31/12.

    Con la facturación mensual, tendría este aspecto:

    - Suscripción de compras del partner del 1 de enero = línea de facturación de cargo creada para el periodo de servicio 1/1 - 31/1.
    - Suspende la suscripción el 25 de enero = línea de facturación de crédito creada para el periodo de servicio 1/1 - 31/1.
    - Se reactiva el 29 de enero = línea de facturación de cargo creada para el periodo de servicio 1/29 - 31/1.



## <a href="" id="freetrialsfaq"></a>Evaluaciones gratuitas de preguntas más frecuentes

**Q1:** ¿Cuáles son las evaluaciones gratuitas?

-   **R:** Puede ofrecer una evaluación gratuita de 30 días de determinados productos a sus clientes. Esto permite a los clientes evaluar el producto antes de comprarlo. Hay pruebas gratuitas disponibles para los siguientes productos: 

    - Office 365 Empresa Premium (a partir del 17 de octubre de 2017)
    - Office 365 E3 (a partir del 17 de octubre de 2017)
    - Office 365 E5 con RTC (a partir del 17 de octubre de 2017)
    - Office 365 E5 sin RTC (a partir del 17 de octubre de 2017)
    - Enterprise Mobility + Security E5 (a partir del 17 de octubre de 2017)
    - Dynamics 365 Customer Engagement Plan 1 (a partir del 17 de octubre de 2017)
    - Dynamics 365 for Financials (a partir del 17 de octubre de 2017)
    - Microsoft 365 Empresa (a partir del 1 de marzo de 2018)
    
**P2:** ¿Son la facturación anual y libres ensayos diferentes en una nube soberana frente a la nube pública?

-   **R:** No. Son iguales. La única diferencia serán las SKU de prueba que están disponibles en el momento de inicio.

**Q3:** ¿Quién puede participar?

-   **R:** Todos los asociados pueden participar. Sin embargo, actualmente no está disponible en China. 

**Q4:** ¿Qué debo hacer para habilitarme para beneficiarse de estas evaluaciones gratuitas??

-   **R:** Tenga en cuenta cómo se puede incorporar la evaluación gratuita en el movimiento de venta y el impacto en los procesos internos. También puede ser necesario modificar las API para incluir la conversión de una evaluación gratuita a una suscripción de pago. Hay especificaciones técnicas detalladas para cambios de API en la vista Anuncios del Centro de partners.

**Q5:** ¿Veré la evaluación gratuita en mi archivo de conciliación y la factura?

-   **R:** No, no aparecerá en su factura o el archivo de conciliación en licencias gratuitas. Aparecerá en tu factura y en el archivo de conciliación basada en licencia después de convertir una evaluación de prueba en una suscripción de pago. La suscripción convertida aparecerá en la factura y en el archivo de conciliación basada en licencia de la misma forma que en cualquier otra suscripción nueva.

**Q6:** ¿Las evaluaciones gratuitas tienen un impacto en los incentivos?

-   **R:** No. La prueba gratuita no tiene ningún efecto en los incentivos.

**Q7:** ¿Las evaluaciones gratuitas estarán disponibles para otros productos de Office en el futuro?

-   **R:** Proporcionamos evaluaciones gratuitas de estos productos porque son las ofertas de empresa más completas y populares. Podemos agregar ofertas adicionales de evaluación gratuita en el futuro.

**Q8:** ¿Puede un cliente tiene más de una evaluación gratuita?

-   **R:** Cada cliente tiene derecho a una evaluación gratuita por oferta disponible.

**Q9:** ¿Existen límites para una evaluación gratuita?

-   **R:** Sí. La evaluación gratuita es para un máximo de 25 licencias. El número de licencias no se puede cambiar durante el período de prueba. Una vez que la prueba se convierte en una suscripción de pago, puedes agregar licencias adicionales a la suscripción.

**Q10:** ¿Es una evaluación gratuita se convierten automáticamente en una suscripción de pago?

-   **R:** No. Tendrás que convertir tú mismo la suscripción en el Centro de partners o a través de la API.

**Q11:** ¿Las evaluaciones gratuitas se pueden usar para las suscripciones de facturación mensuales y anuales?

-   **R:** Sí. Puedes elegir la frecuencia de facturación al convertir la evaluación gratuita en una suscripción de pago.

**Q12:** ¿La fecha de inicio de la suscripción se basará la fecha inicia el evaluación gratuita o la fecha en que se convierte en una suscripción de pago? 

-   **R:** La fecha de inicio se basa en la fecha de conversión. Si la evaluación gratuita se convierte en una oferta de pago con facturación anual, la fecha de renovación de suscripción será de doce meses desde la fecha de conversión. R: Si la evaluación gratuita se convierte en una oferta pagada con facturación mensual, la fecha de renovación de suscripción será de doce meses desde la fecha de facturación tras la fecha de conversión.

**Q13:** ¿Podemos agregar o quitar puestos durante la evaluación gratuita?

-   **R:** No. Las pruebas gratuitas tendrán 25 licencias de manera predeterminada y no se pueden actualizar.

**Q14:** ¿Hay evaluaciones para las ofertas de complemento como ATP y PSTN?

-   **R:** No hay ningún gratuitas para cualquier oferta de complemento en este momento.

**Q15:** ¿Se puede proporcionar una evaluación gratuita de una oferta que ya posee un cliente?

-   **R:** No. Si la oferta ya pertenece al cliente, no puede usarse para una prueba gratuita.

**Q16:** ¿Podré ver todas mis ofertas de prueba pendientes?

-   **R:** Sí. La página de cliente muestra todas las suscripciones. Esto incluye las suscripciones de pruebas gratuitas y las suscripciones de pago.

**Q17:** ¿Se notificará sobre evaluaciones gratuitas que caducan?

-   **R:** No. Puedes realizar un seguimiento de las fechas de caducidad próximas desde la vista del cliente en el Centro de partners, o puedes consultar la API. Se recomienda supervisar esas fechas con frecuencia para poder realizar las acciones de seguimiento apropiadas con los clientes que se acercan a la fecha de caducidad.

**Q18:** ¿Si un cliente ha tenido una evaluación gratuita para una oferta puede también usan otra prueba para una oferta diferente? 

-   **R:** Sí. Los clientes pueden registrarse para una versión de evaluación por oferta. Por ejemplo, pueden obtener una prueba gratuita para Office 365 Empresa Premium y una prueba gratuita para Office 365 E3.

**Q19:** ¿Qué ocurre cuando finaliza el período de prueba? ¿Mi cliente o yo recibiremos una notificación? ¿Qué notificaciones aparecen al intentar iniciar sesión en una versión de evaluación que ha caducado?

-   **R:** Una vez que una versión de evaluación ha expirado, un cliente intenta iniciar sesión en esa versión de prueba verán un mensaje que indica que la versión de evaluación ha expirado. No habrá notificaciones para indicar que una prueba caduca, pero, como partner, puedes realizar un seguimiento a través de la vista de clientes o a través de consultas en la API.

**Q20:** ¿Una versión de prueba se puede extender?

-   **R:** No. La versión de prueba debe convertirse en una versión de pago o caducará después de 30 días.

**Q21:** ¿Cuando una versión de evaluación expira, puede la información de la versión de prueba obtenerse?

-   **R:** Sí. Los datos se almacenan en línea con estándares de retención de datos. Cuando hayas comprado una nueva suscripción con los mismos planes de servicio, se puede acceder a los datos del cliente desde la suscripción recientemente activada.

**Q22:** ¿Son gratuitas disponibles para el gobierno y ofrece la educación?

-   **R:** No hay ningún gratuitas para el gobierno y educación se ofrece en este momento.

**Q23:** ¿Las evaluaciones gratuitas de cliente para el programa proveedor de soluciones en la nube (CSP) se pueden convertir a otros inquilinos de programa, por ejemplo, EA, abierto o MOSP? 

-   **R:** No. Las suscripciones no pueden transferirse de CSP a otro programa.

**Q24:** ¿Cómo puedo obtener soporte técnico en las evaluaciones gratuitas? 

-   **R:** Envíe una solicitud de servicio a través del centro de partners.

## <a href="" id="billingalignmentfaq"></a>Alineación - libre final del periodo de facturación

A partir del 21 de febrero de 2018, el programa Proveedor de soluciones en la nube (CSP) comenzará a implementar la "alineación de fechas de facturación" para las nuevas suscripciones con frecuencia de facturación mensual. Esta "alineación de fechas de facturación" proporcionará a los partners más flexibilidad y capacidad de previsión para las ventas y facturación, así como para el aprovisionamiento y la administración de planes de clientes. 

**ACTUALIZAR EL 23 DE FEBRERO:**  Anteriormente habíamos anunciado una fecha de implementación del 20 de febrero, pero nuestra implementación real se ha retrasado ligeramente y se ha escalonado por categoría de producto.  Revisa el gráfico a continuación para conocer la fecha de implementación por categoría de producto. 

|**Categoría de producto**   |**Día de la implementación**   |
|-----------------|:-------------|
|Office  |21 de febrero   |
|Windows, Minecraft   |22 de febrero   |
|Office 365 China   |23 de febrero   |
|Dynamics/Intune   |23 de febrero   |

Las suscripciones adquiridas antes de la fecha de implementación (véase el gráfico anterior) se benefician de un período gratuito desde la fecha de compra hasta la fecha de facturación del partner. Las suscripciones adquiridas después de la fecha de implementación ya no recibirán un período gratuito. El período pagado de 12 meses comenzará (se alineará) en la fecha de la compra, en lugar de con la facturación del partner. Los partners ya no verán una "línea de facturación de 0 $" que representa el período gratuito en el archivo de conciliación. No hay ningún cambio en las API, la facturación o los incentivos.  Los partners deben informar a sus equipos de ventas y contabilidad de esta nueva lógica de facturación y asegurarse de que las operaciones se ajusten según sea necesario.  

Antes de implementar la alineación de fechas de facturación, hemos facturado y realizado el cargo en la fecha de aniversario de facturación del partner, la fecha en la que el partner se registró en el programa CSP; no en la fecha de aniversario de suscripción del cliente, la fecha en que el cliente adquirió su suscripción. Después de la fecha de implementación, los partners recibirán el cargo en su fecha de aniversario de suscripción, lo que elimina este período gratuito.  Los partners seguirán recibiendo facturas en su fecha de aniversario de facturación, pero la fecha de vigencia de la factura será la fecha de aniversario de suscripción del cliente. 

Las suscripciones que se encuentran en el período gratuito en la fecha de implementación no recibirán ningún cargo entre la fecha de compra y la fecha de facturación del partner. Además, no se realizará el cargo durante el primer mes del período de pago de 12 meses. Si usas un archivo de conciliación para realizar la verificación, ten en cuenta que el cargo de este primer mes dejará de estar visible en el archivo de conciliación.  

**Q1:** ¿Qué va a cambiar con la fecha de facturación?

-   **R:** Las suscripciones basadas en licencias dejará de tener un período gratuito. Actualmente, existe un período gratuito desde la fecha de compra hasta la fecha de facturación del partner.

**P2:** ¿Cuando se quita el período gratuito?

- **R:** A partir de la fecha de implementación que se indican en la tabla siguiente, las suscripciones nuevas no recibirá un periodo gratis.

|**Categoría de producto**   |**Día de la implementación**   |
|-----------------|:-------------|
|Office  |21 de febrero   |
|Windows, Minecraft   |22 de febrero   |
|Office 365 China   |23 de febrero   |
|Dynamics/Intune   |23 de febrero   |

**Q3:** ¿Cuál será el impacto en las suscripciones en el período en la fecha de implementación gratuita?

- **R:** Las suscripciones que están en el período en la fecha de implementación gratuita seguirá recibiendo un período gratuita desde la fecha de compra a la fecha de facturación asociado. Estas licencias también recibirán un "período gratuito ampliado" y no se realizará el cargo durante el primer mes del período de pago de 12 meses. El "período gratuito ampliado" no se aplicará a licencias agregadas en el primer mes. Si aumentas la cantidad de licencias en el primer mes, se te cobrará por aquellas licencias agregadas en la siguiente factura/conciliación. Si el archivo de conciliación se usa para realizar la verificación, ten en cuenta que puede que el cargo de este primer mes no aparezca en el archivo de conciliación. Consulta los siguientes escenarios para obtener una explicación más detallada.

**Q4:** ¿Cuándo comenzará el período de pago de 12 meses para una nueva suscripción?

- **R:** Actualmente, el período de pago comienza en la fecha siguiente a la fecha de compra de facturación del asociado. A partir de la fecha de implementación, el período de pago para las nuevas suscripciones comenzará en la fecha de compra.

**Q5:** ¿Cuándo se las suscripciones de renovación automática?

- **R:** Las suscripciones renuevan automáticamente 12 meses después de la primera fecha de facturación. Actualmente, esto significa que las suscripciones se renuevan automáticamente 12 meses después de la primera fecha de facturación del partner después de la fecha de compra. A partir de la fecha de implementación, las nuevas suscripciones se renovarán automáticamente 12 meses después de la fecha de compra.

**Q6:** ¿Qué ocurre si comprar la suscripción el día 29, 30 o 31 de un mes?

- **R:** La suscripción estará disponible desde la fecha de compra, pero no se inicia el período de pago de 12 meses hasta el primer día del mes siguiente.

**Q7:** ¿Qué ofertas se ven afectados?

- **R:** La eliminación de período gratuita se aplica a todas las suscripciones de CSP basados en licencia.

**Q8:** ¿Cómo esto afecta el archivo de conciliación y la factura? 

- **R:** Ya no verá la "línea de facturación de 0 $" en la factura o el archivo de conciliación. Actualmente, la línea de facturación de $0 representa el período gratuito.

**Q9:** ¿Cambiará mi facturación fecha?

- **R:** No, se seguirá recibiendo el archivo de conciliación y la factura en su fecha de facturación existente.

**Q10:** ¿El cargo mensual iniciará y finalizar el cambio de fechas para las suscripciones existentes?

- **R:** No, existente suscripción mensual gratuita inicial y final se seguirán las fechas para alinearse con su fecha de facturación. Sin embargo, las nuevas suscripciones se alinearán con la fecha de compra. Ver un ejemplo abajo.

**Q11:** ¿Cambiará el cálculo de incentivos?

- **R:** No, no hay ningún cambio en los cálculos de incentivos.

**Q12:** ¿Habrá un cambio en las API?

- **R:** No, no hay ningún cambio a las API.

### <a name="common-scenarios"></a>Escenarios comunes


|**Escenarios**   |**Escenario 1: Período de suscripción gratuita finaliza antes de la fecha de implementación**   |**Escenario 2: Suscripción está dentro del período libre en la fecha de implementación**  | **Escenario 3: Suscripción adquirida en o después de la fecha de implementación**   |
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

La fecha de facturación del partner es el decimoquinto día del mes. El 1 de junio de 2018 el partner adquiere una nueva suscripción. El precio de la suscripción es 30 $ por licencia al mes. 

El 15 de junio el archivo de conciliación contendrá solo las siguientes líneas de facturación:

- Cargo de 30 $ para el período de servicio comprendido entre el 1 y el 30 de junio

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|--------------|
|01/06/2018   |30/6/2018   |30 $   |1   |30 $   |Tarifas prorrateadas al comprar |

### <a name="scenario-5a-suspend-and-reactivate-before-billing-date"></a>Escenario 5a: Suspensión y reactivación antes de la fecha de facturación

La fecha de facturación del partner es el decimoquinto día del mes. El 1 de junio de 2018 el partner adquiere una nueva suscripción. El precio de la suscripción es 30 $ por licencia al mes. El 5 de junio de 2018, el partner suspende la suscripción. El 10 de junio de 2018, el partner vuelve a activar la suscripción. El 15 de junio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30 $ para el período de servicio comprendido entre el 1 y el 30 de junio. 
- Crédito de cancelación de -30 $ para el período de servicio comprendido entre el 5 y el 30 de junio. El crédito no se prorratea porque la suscripción se suspendió en los primeros 30 días. 
- Cargo de 30 $ para el período de servicio comprendido entre el 10 y el 30 de junio. El cargo no se prorratea porque la suscripción se volvió a activar en los primeros 30 días. 

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01/06/2018   |30/6/2018   |30 $   |1   |30 $   |Tarifas prorrateadas al comprar |
|05/06/2018   |30/6/2018   |-30 $   |1   |30 $   |Cuota de cancelación |
|10/06/2018   |30/6/2018   |30 $   |1   |30 $   |Tarifa de activación |

Ten en cuenta que cuando se suspende una suscripción y vuelve a activarse, la fecha de renovación automática seguirá siendo 12 meses desde la fecha de compra original.

### <a name="scenario-5b-suspend-and-reactivate-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Escenario 5b: Suspenda y reactive después de la fecha de facturación, pero menos de 30 días desde la fecha de compra

La fecha de facturación del partner es el decimoquinto día del mes. El 1 de junio de 2018 el partner adquiere una nueva suscripción. El precio de la suscripción es 30 $ por licencia al mes. El 20 de junio de 2018, el partner suspende la suscripción. El 25 de junio de 2018, el partner vuelve a activar la suscripción. El 15 de junio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30 $ para el período de servicio comprendido entre el 1 y el 30 de junio. 

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01/06/2018   |30/6/2018   |30 $   |1   |30 $   |Tarifas prorrateadas al comprar |

El 15 de julio el archivo de conciliación contendrá las siguientes líneas de facturación:
- Crédito de cancelación de -30 $ para el período de servicio comprendido entre el 20 y el 30 de junio. El crédito no se prorratea porque la suscripción se suspendió en los primeros 30 días.
- Cargo de 30 $ para el período de servicio comprendido entre el 25 y el 30 de junio. El cargo no se prorratea porque la suscripción se volvió a activar en los primeros 30 días.
- Cargo de 30 $ para el período de servicio comprendido entre el 1 y el 31 de julio.

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20/06/2018   |30/6/2018   |-30 $   |1   |-30 $   |Cuota de cancelación |
|25/06/2018   |30/6/2018   |30 $   |1   |30 $   |Tarifa de activación |
|01/07/2018   |31/7/2018   |30 $   |1   |30 $   |Tarifa de ciclo |

### <a name="scenario-5c-suspend-and-reactivate-different-license-quantity-after-billing-date-but-less-than-30-days-from-purchase-date"></a>Escenario 5c: Suspenda y reactive (cantidad de licencias distinto) después de la fecha de facturación, pero menos de 30 días desde la fecha de compra

La fecha de facturación del partner es el decimoquinto día del mes. El 1 de junio de 2018 el partner adquiere una nueva suscripción. El precio de la suscripción es 30 $ por licencia al mes. El 20 de junio de 2018, el partner suspende la suscripción. El 25 de junio de 2018, el partner vuelve a activar la suscripción con dos licencias. El 15 de junio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30 $ para el período de servicio comprendido entre el 1 y el 30 de junio. 

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|01/06/2018   |30/6/2018   |30 $   |1   |30 $   |Tarifas prorrateadas al comprar |

El 15 de julio el archivo de conciliación contendrá las siguientes líneas de facturación:
- Crédito de cancelación de -30 $ para el período de servicio comprendido entre el 20 y el 30 de junio. El crédito no se prorratea porque la suscripción se suspendió en los primeros 30 días.
- Cargo de 30 $ para el período de servicio comprendido entre el 25 y el 30 de junio. El cargo de reactivación no se prorratea porque la suscripción se volvió a activar en los primeros 30 días. El cargo también se basa en la cantidad de licencias original de 1.
- Crédito de -6 $ para el período de servicio comprendido entre el 25 y el 30 de junio. El cargo de reactivación solo le cobró por 1 licencia durante el período de servicio del 25 y el 30 de junio, cuando tenía 2 licencias. El crédito de -6 $ revierte el cargo incorrecto para el período de servicio del 25 al 30 de junio.
- Renovación prorrateada de 12 $ para el período de servicio comprendido entre el 25 y el 30 de junio. El partner tenía 2 licencias durante este período de servicio. El precio unitario se calcula como (30/30)*6*2= 12 $.
- Cargo de 60 $ para el período de servicio comprendido entre el 1 y el 31 de julio.

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|:------ |--------|
|20/06/2018   |30/6/2018   |-30 $   |1   |-30 $   |Cuota de cancelación |
|25/06/2018   |30/6/2018   |30 $   |1   |30 $   |Tarifa de activación |
|25/06/2018   |30/6/2018   |-6 $   |1   |-6 $   |Prorrateo de instancia de ciclo |
|25/06/2018   |30/6/2018   |6 $   |2   |12 $   |Prorrateo de instancia de ciclo |
|01/07/2018   |31/7/2018   |30 $   |2   |60 $   |Tarifa de ciclo |

### <a name="scenario-6-subscription-suspension-less-than-30-days-after-purchase-and-reactivation-more-than-30-days-after-purchase"></a>Escenario 6: Suspenda la suscripción menos de 30 días después de la compra y reactivación de más de 30 días después de la compra 

La fecha de facturación del partner es el decimoquinto día del mes. El 1 de junio el partner adquiere una nueva suscripción de una licencia a 30 $ al mes. El 5 de junio, el partner suspende la suscripción. El 15 de junio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30 $ para el período de servicio comprendido entre el 1 y el 30 de junio
- Crédito de cancelación de -30 $ para el período de servicio comprendido entre el 5 y el 30 de junio. El crédito no se prorratea porque la suscripción se suspendió en los primeros 30 días.

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|01/06/2018   |30/6/2018   |30 $   |1   |30 $   |Tarifas prorrateadas al comprar
|05/06/2018   |30/6/2018   |-30 $   |1   |-30 $   |Cuota de cancelación

El 10 de julio, el partner vuelve a activar la suscripción. El 15 de julio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de reactivación 21,30 $ para el período de servicio comprendido entre el 10 y el 31 de julio. Las reactivaciones después de 30 días desde la fecha de compra se traducen en un cargo prorrateado. 

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|10/7/2018   |31/7/2018   |21,30 $   |1   |21,30 $   |Tarifa de activación |

El 15 de agosto el archivo de conciliación contendrá las siguientes líneas de facturación:
- Cargo de 30 $ para el período de servicio comprendido entre el 1 y el 31 de agosto.

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/08/2018   |31/8/2018   |30 $   |1   |30 $   |Tarifa de ciclo |

Ten en cuenta que cuando se suspende una suscripción y vuelve a activarse, la fecha de renovación automática seguirá siendo 12 meses desde la fecha de compra original. 

### <a name="scenario-7-subscription-suspension-and-reactivation-more-than-30-days-after-purchase"></a>Escenario 7: Suspensión y reactivación de una suscripción en más de 30 días después de la compra 
La fecha de facturación del partner es el decimoquinto día del mes. El 1 de junio el partner adquiere una nueva suscripción de una licencia a un precio de 30 $ al mes. 

El 15 de junio el archivo de conciliación contendrá solo las siguientes líneas de facturación:

- Cargo de 30 $ para el período de servicio comprendido entre el 1 y el 30 de junio.

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|---------|
|01/06/2018   |30/6/2018   |30 $   |1   |30 $   |Tarifas prorrateadas al comprar |

El partner suspende la suscripción el 5 de julio pero la vuelve a activar el 15 de julio. El 15 de julio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30 $ para el período de servicio comprendido entre el 1 y el 31 de julio.
- Crédito de cancelación de -26,14 $ para el período de servicio comprendido entre el 5 y el 31 de julio. Las cancelaciones después de 30 días desde la fecha de compra se traducen en un crédito prorrateado. Cálculo = (precio mensual/días en período de servicio total) x días del período de servicio prorrateado x cantidad de licencias x (-1) = (30/31) x 27 x 1 x (-1) =-26,14.
- Cargo de reactivación 21,30 $ para el período de servicio comprendido entre el 10 y el 31 de julio. Las reactivaciones después de 30 días desde la fecha de compra se traducen en un cargo prorrateado. Cálculo = (30/31) x 22 x 1 = 21,30.

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/07/2018   |31/7/2018   |30 $  |1   |30 $   |Tarifa de ciclo |
|05/07/2018   |31/7/2018   |   -26,14 $   |1   |-26,14 $|Cuota de cancelación |
|10/7/2018   |31/7/2018   |-21,30 $   |1   |21,30 $|Tarifa de activación |

El archivo de conciliación del 15 de agosto contendrá lo siguiente:
- Cargo de 30 $ para el período de servicio comprendido entre el 1 y el 31 de agosto.

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/08/2018   |31/8/2018   |30 $  |1   |30 $   |Tarifa de ciclo |

### <a name="scenario-8-change-of-license-quantity"></a>Escenario 8: Cambiar la cantidad de licencias 

La fecha de facturación del partner es el 15. El 1 de junio el partner adquiere una nueva suscripción por 30 $ al mes. El 10 de junio el partner aumenta la cantidad de licencias de 1 a 2 licencias. El 15 de junio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30 $ para el período de servicio comprendido entre el 1 y el 30 de junio. Aunque el partner aumentó la cantidad de licencias antes de la fecha de facturación del 15 de junio, el cambio no se reconoce en el sistema de facturación de Microsoft hasta el día de aniversario de suscripción el 1 de julio.

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/06/2018   |30/6/2018   |30 $   |1   |30 $   |Tarifas prorrateadas al comprar |

El 1 de julio, el día de aniversario de la suscripción, el sistema de facturación de Microsoft reconocerá que la cantidad de licencias se cambió de 1 a 2 el 10 de junio. El sistema de facturación generará un crédito y renovaciones prorrateadas para el período de servicio comprendido entre el 1 y el 9 de junio y el 10 y el 30 de junio. 

El archivo de conciliación del 15 de julio contendrá lo siguiente:

- Crédito de -30 $ para el período de servicio comprendido entre el 1 y el 30 de junio.
- Renovación prorrateada de 9 $ para el período de servicio comprendido entre el 1 y el 9 de junio. Se trata del período cuando el cliente tenía 1 licencia. Cálculo = (precio mensual/total de días en período de servicio total) x días del período de servicio prorrateado x número de licencias = (30/30) x 9 x 1 = 9.
- Renovación prorrateada de 42 $ para el período de servicio comprendido entre el 10 y el 30 de junio. Se trata del período cuando el cliente tenía 2 licencias. Cálculo = (30/30) x 21 x 2 = 42.
- Cargo de 60 $ para el período de servicio comprendido entre el 1 y el 31 de julio.

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/06/2018   |30/6/2018   |-30 $   |1   |-30 $|Prorrateo de instancia de ciclo |
|01/06/2018   |09/06/2018   |9 $   |1   |9 $|Prorrateo de instancia de ciclo |
|10/06/2018   |30/6/2018   |21 $   |2   |42 $|Prorrateo de instancia de ciclo |
|01/07/2018   |31/7/2018   |30 $   |2   |60 $   |Tarifa de ciclo |

### <a name="scenario-9-add-on-subscriptions"></a>Escenario 9: Suscripciones de complemento

La fecha de facturación del partner es el decimoquinto día del mes. El 1 de junio el partner adquiere una nueva suscripción de una licencia a un precio de 30 $ al mes. El 10 de junio el partner adquiere una nueva suscripción de complemento por 5 $ al mes. La fecha de renovación de suscripción de complemento se alinea con la fecha de renovación de suscripción base que es el 1 de junio. 

El 10 de junio el partner adquiere una suscripción de complemento de una licencia a un precio de 5 $ al mes. 

El 15 de junio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30 $ para el período de servicio comprendido entre el 1 y el 30 de junio. Se trata de la suscripción base.
- Cargo prorrateado de 3,50 $ para el período de servicio comprendido entre el 10 y el 30 de junio. Se trata de la suscripción de complemento. 

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|--------|
|01/06/2018   |30/6/2018   |30 $   |1   |30 $   |Tarifas prorrateadas al comprar |
|10/06/2018   |30/6/2018   |3,50 USD   |1   |3,50 USD   |Tarifas prorrateadas al comprar |

El 15 de julio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30 $ para el período de servicio comprendido entre el 1 y el 31 de julio. Se trata de la suscripción base.
- Cargo de 5 $ para el período de servicio comprendido entre el 1 y el 31 de julio. Se trata de la suscripción de complemento.

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|-------|
|01/07/2018   |31/7/2018   |30 $   |1   |30 $   |Tarifa de ciclo |
|01/07/2018   |31/7/2018   |5 $   |1   |5 $   |Tarifa de ciclo |

Ten en cuenta que la suscripción de complemento tendrá una fecha de renovación automática de 1 de junio de 2019, que se alinea con la de suscripción base.

### <a name="scenario-10-new-purchase-on-the-29th-30th-or-31st"></a>Escenario 10: Compra a través de los días 29, 30 o 31 

La fecha de facturación del partner es el decimoquinto día del mes. El 29 de mayo el partner adquiere una nueva suscripción de una licencia a un precio de 30 $ al mes. Las suscripciones adquiridas el 29, 30 o 31 tendrán un período gratuito desde la fecha de compra hasta el primer día del mes siguiente. El día de aniversario de suscripción predeterminado será el 1. En este escenario, la suscripción recibirá un período gratuito desde el 29 de mayo hasta el 31 de mayo y el período de pago de 12 meses comenzará el 1 de junio. 

El 15 de junio el archivo de conciliación contendrá las siguientes líneas de facturación:

- Cargo de 30 $ para el período de servicio comprendido entre el 1 y el 30 de junio.

|**Inicio de cargo**   |**Final de cargo**   |**Precio por unidad**   |**Cantidad**   |**Cantidad**   |**Tipo de gasto** |
|-----------------|:-------------|:----------------|:------------|:------|------|
|29/5/2018   | 30/6/2018   |30 $   |1   |30 $  |Tarifas prorrateadas al comprar |

Ten en cuenta que la suscripción se renovará automáticamente el 1 de junio de 2019.
