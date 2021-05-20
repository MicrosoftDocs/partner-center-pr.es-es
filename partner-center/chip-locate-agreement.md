---
title: Buscar el número de escritorios y el nivel de cuota
ms.topic: how-to
ms.date: 02/18/2021
description: Obtenga información sobre cómo usar la plataforma de incentivos de canal (CHIP) para encontrar la información de nivel de cuota y recuento de escritorio para un contrato.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 64dbbbae0087275fa8d0c5fd4f364079623efe63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148999"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Búsqueda del número de dispositivos de escritorio y el nivel de recargo de un contrato

**Roles adecuados:** contacto principal o administrador del programa

Puede iniciar sesión en [explore.ms](https://www.explore.ms/) revisar el contrato o descargar un archivo que proporcione los detalles del contrato para el número de escritorios y el nivel de cuota.

## <a name="to-locate-the-information"></a>Para buscar la información

### <a name="method-1--explorems"></a>Método 1: Explore.ms

1. Abra [explore.ms](https://www.explore.ms/) en Internet Explorer. 

>[!Note]
>No puede realizar esta función en Google Chrome ni en Microsoft Edge.

2. Inicie sesión con su cuenta de trabajo o educativa o con el identificador en directo.  

3. En el **campo Informes,** seleccione **Acuerdos**.

4. En la página resultante, escriba el número de contrato en el **campo Buscar** y, a continuación, **seleccione Seleccionar/Ordenar columnas**.

5. En la ventana emergente,  seleccione Recuento de escritorios de contrato en la lista de columnas disponibles y, a continuación, seleccione la flecha derecha para agregar la columna. Seleccione **Aceptar**.

6. Seleccione **Buscar.**

7. En la pantalla resultante, desplácese por los resultados para buscar la **columna Recuento de escritorios del** contrato. 

8. Use el recuento de escritorios para determinar el nivel de tarifa en función de la tabla de tarifas siguiente.  

| Nivel de cuota | Recuento de escritorios |
| ------ | :-----------: |
|  A | 0 – 2,399    |
|  B | 2,400 – 5,999    |
|  C | 6,000 – 14,999    |
|  D | 15,000+   |

>[!NOTE]
>Los niveles de incentivos empresariales se basan en el recuento de usuarios o de escritorio (lo que sea mayor) en las inscripciones del sector comercial y público (PS). En el caso de las inscripciones sin recuento natural de usuarios o escritorios asociados, Microsoft aplica un recuento de escritorios basado en el número de escritorios o el número de usuarios del EA que lo acompaña. <br><br>Si no hay ningún EA que lo acompaña, el nivel de tarifa se basa en el nivel de precios de la inscripción. El nivel de precios de la oferta también se puede ver en [www.explore.ms](https://www.explore.ms/). <br><br>Si hay varios niveles de grupo o precios en el EA/EAS existente, Microsoft pagará incentivos en el nivel de grupo o precios asignados más alto, siendo el nivel A el más bajo y el nivel D el más alto.

#### <a name="pool-and-pricing-levels"></a>Niveles de grupo y precios

Después de buscar el número de contrato en explore.ms los pasos descritos anteriormente, seleccione el número de contrato. Esto le llevará a la página de detalles del contrato, que mostrará **el** resumen del contrato y **las ofertas**. La sección de ofertas contiene los niveles de precios.

## <a name="method-2---chip"></a>Método 2: CHIP

1. Inicie sesión en CHIP y seleccione LSP Incentives (Incentivos de LSP).

2. En la **página Resumen de pago** de asociados, seleccione el  mes de informes que desea ver y, a continuación, seleccione Detalles de cálculo en la lista desplegable bajo Exportar **a Excel:**

:::image type="content" source="images/chip/chiplocate.png" alt-text="Buscar detalles del programa":::

3. Se iniciará la exportación y puede abrir el archivo o guardar o guardar como en un destino.

4. Cuando el informe esté abierto, vaya a la pestaña **DetailReport-FlatFile** en la parte inferior izquierda:

:::image type="content" source="images/chip/flatfile.png" alt-text="Descarga de archivos planos":::

Ahora puede buscar el número de contrato que busca en la columna J. y encontrará el número de escritorio asignado en la columna R, con la etiqueta Agreement_DesktopCount. También puede confirmar el nivel de tarifa de este contrato en la columna "AI" con la etiqueta Tier(Nivel).

## <a name="next-steps"></a>Pasos siguientes

- [Solución de problemas de acceso de CHIP](chip-access-trouble.md)
