---
title: Buscar el número de equipos de escritorio y el nivel de cuota
ms.topic: how-to
ms.date: 02/18/2021
description: Aprenda a usar la plataforma de incentivos de canal (CHIP) para encontrar la información de recuento de equipos de escritorio y tarifas de un acuerdo.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e433b44f158c3e4cefe22027e7f7d3b845991308
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756119"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Búsqueda del número de dispositivos de escritorio y el nivel de recargo de un contrato

**Roles adecuados**

- Contacto principal o administrador de programas

Puede iniciar sesión en [Explore.ms](https://www.explore.ms/) para revisar el contrato o descargar un archivo que proporcione los detalles del contrato para el recuento de equipos de escritorio y el nivel de cuota.

## <a name="to-locate-the-information"></a>Para buscar la información

### <a name="method-1--explorems"></a>Método 1: Explore.ms

1. Abra [Explore.ms](https://www.explore.ms/) en Internet Explorer. 

>[!Note]
>No se puede realizar esta función en Google Chrome ni en Microsoft Edge.

2. Inicie sesión con su cuenta profesional o educativa o Live ID.  

3. En el campo **informes** , seleccione **contratos**.

4. En la página resultante, escriba el número de contrato en el campo de **búsqueda** y, a continuación, seleccione **seleccionar/ordenar columnas**.

5. En la ventana emergente, seleccione el **acuerdo recuento de equipos de escritorio** en la lista columnas disponibles y, a continuación, seleccione la flecha derecha para agregar la columna. Seleccione **Aceptar**.

6. Seleccione **Buscar.**

7. En la pantalla resultante, desplácese por los resultados para buscar la columna **contrato de Desktop Count** . 

8. Use el recuento de escritorios para determinar el nivel de cuota según la tabla de tarifas que aparece a continuación.  

| Nivel de tarifa | Recuento de equipos de escritorio |
| ------ | :-----------: |
|  A | de 0 a 2.399    |
|  B | 2.400 – 5.999    |
|  C | 6.000 – 14.999    |
|  D | 15000 +   |

>[!NOTE]
>Los niveles de incentivo empresariales se basan en el número de equipos de escritorio o de usuarios (el que sea mayor) en las inscripciones de sectores comerciales y públicos (PS). En el caso de las inscripciones sin un número de usuario o de escritorio asociado natural, Microsoft aplica un recuento de equipos de escritorio en función del número de equipos de escritorio o el recuento de usuarios del EA que lo acompaña. <br><br>Si no hay ningún EA acompañante, el nivel de cuota se basa en el nivel de precios de la inscripción. El nivel de precios del contrato también se puede ver en [www.Explore.ms](https://www.explore.ms/). <br><br>Si hay varios grupos o niveles de precios en el EA/EAS existente, Microsoft pagará incentivos con el mayor nivel de precios y grupos asignados, y el nivel A será el más bajo y el nivel D será el más alto.

#### <a name="pool-and-pricing-levels"></a>Grupos y niveles de precios

Después de buscar el número de contrato en explore.ms siguiendo los pasos descritos anteriormente, seleccione el número de contrato. Esto le llevará a la página de detalles del contrato, que mostrará las **ofertas** y el **Resumen del contrato** . La sección de ofertas contiene los niveles de precios.

## <a name="method-2---chip"></a>Método 2: CHIP

1. Inicie sesión en CHIP y seleccione incentivos de LSP.

2. En la página **Resumen de pago de socios** , seleccione el mes de informes que desea ver y, a continuación, seleccione detalles de **cálculo** en la lista desplegable de **exportar a Excel**:

:::image type="content" source="images/chip/chiplocate.png" alt-text="Buscar detalles del programa":::

3. La exportación se iniciará y podrá abrir el archivo o guardar o guardar como para un destino.

4. Cuando el informe esté abierto, vaya a la pestaña **DetailReport-FlatFile** en la parte inferior izquierda:

:::image type="content" source="images/chip/flatfile.png" alt-text="Descarga de archivos planos":::

Ahora puede buscar el número de contrato que está buscando en la columna J. y encontrará el recuento de escritorios asignados en la columna R, con la etiqueta Agreement_DesktopCount. También puede confirmar el nivel de cuota de este contrato en la columna ' AI ' con la etiqueta nivel.

## <a name="next-steps"></a>Pasos siguientes

- [Solucionar problemas de acceso a CHIPs](chip-access-trouble.md)
