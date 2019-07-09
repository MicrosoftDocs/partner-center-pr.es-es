---
title: Análisis de Microsoft Learn | Centro de partners
ms.topic: article
ms.date: 07/05/2019
description: Información sobre cómo entender el análisis de aprendizaje
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.openlocfilehash: 09d4ca14c1b407e9010ab26bccaf612f9caad732
ms.sourcegitcommit: bd83621eb29fafbda341ad41814a9ae5c1e78b00
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/08/2019
ms.locfileid: "67622533"
---
# <a name="microsoft-learn-analytics-report"></a>Informe de análisis de Microsoft Learn

El informe de Microsoft Learn le proporcionará información sobre los aprendices de la empresa incluidos los módulos que se ha completado y las rutas de acceso de aprendizaje que se encuentran en. El informe muestra el estado de cada factor individual. El administrador global y el administrador MPN para su empresa pueden ver los datos.

## <a name="how-to-read-the-report"></a>Cómo leer el informe

### <a name="summary-charts"></a>Gráficos de resumen

**Entrena el recuento de las personas**: Un recuento de todos los distintos factores que hayan completado al menos un módulo durante el intervalo de fechas seleccionado 

**Mini gráfico de tendencia de individuos entrenados**: Recuento acumulado de mes de los aprendices activos a mes 

**Número de finalizaciones de módulo**: Finalizaciones de recuento de módulo por los aprendices en la empresa del socio durante el intervalo de fechas seleccionado.
Por ejemplo, si "Módulo 1" se ha completado por 15 usuarios y el "módulo 2" se ha completado por las mismas 15 personas, el recuento de las finalizaciones de módulo será 30. La fecha de finalización de módulo debe estar en el intervalo de fechas seleccionado.

**Las finalizaciones de módulo mini gráfico de tendencia**: Recuento acumulado de mes de las finalizaciones de módulo a mes 

**Número de finalizaciones de ruta de acceso de aprendizaje**: Finalizaciones de ruta de acceso de recuento de aprendizaje por los aprendices en la empresa del socio durante el intervalo de fechas seleccionado.
Por ejemplo, si la ruta de aprendizaje "Ruta de acceso 1" se ha completado por 20 usuarios y la ruta de aprendizaje "ruta de acceso 2" se ha completado por las mismas 20 personas, el recuento de finalización de la ruta de aprendizaje será 40. La fecha de finalización de la ruta de acceso de aprendizaje debe estar dentro del intervalo de fechas seleccionado.

**Mini gráfico de tendencia de finalizaciones de ruta de acceso de aprendizaje**: Recuento acumulado de mes de aprendizaje a mes las finalizaciones de ruta de acceso 

### <a name="trained-individuals-monthly-trend"></a>Tendencia mensual de personas entrenado

**Eje x** es mes para el filtro de tiempo seleccionado. 

**Eje y** es el recuento de sistemas aprendices de activos que se han registrado (por primera vez la finalización de un módulo) durante ese mes. Esto no es acumulativo.

### <a name="module-completions-monthly-trend"></a>Tendencia mensual de finalizaciones de módulo

**Eje x** es mes para el filtro de tiempo seleccionado. 

**Eje y** es el recuento de las finalizaciones de módulo durante ese mes. Esto no es acumulativo.

### <a name="learning-path-completions-monthly-trend"></a>Tendencia mensual de finalizaciones de ruta de acceso de aprendizaje

**Eje x** es mes para el filtro de tiempo seleccionado. 

**Eje y** es el número de finalizaciones de módulo en ese mes. Esto no es acumulativo.

### <a name="learning-path-completion-tabs"></a>Pestañas de la finalización de ruta de acceso de aprendizaje 

- Ficha módulo

**Gráfico de anillos de finalizaciones de módulo**: desglose de las finalizaciones de módulo (mostrado en la sección de resumen de recuento) por los nombres de módulo.

Número que aparece en el centro del gráfico es los módulos total completados

**Las finalizaciones por rol**: desglose de las finalizaciones de módulo por el rol del módulo. Si un módulo está asociado a varios roles, cada uno de los roles se agrega al recuento de las finalizaciones de módulo.

Número que aparece en el centro del gráfico de anillos es el número de roles diferentes para las finalizaciones de módulo. 

**Las finalizaciones por producto**: desglose de las finalizaciones de módulo por el producto en el módulo está asignado a. Si un módulo está asociado a varios productos, cada uno de los productos se agrega al recuento de las finalizaciones de módulo.    

Número que se muestra en el centro del gráfico de anillos es el número de productos distintos para las finalizaciones de módulo.  

- Pestaña de la ruta de acceso de aprendizaje    

**Gráfico de anillos de finalizaciones de rutas de acceso de aprendizaje**: desglose de las finalizaciones de rutas de acceso de aprendizaje (mostrado en la sección de resumen de recuento) por su nombre.

**Las finalizaciones por rol**: desglose de lo aprendido las finalizaciones de rutas de acceso del rol. Si un módulo está asociado a varios roles, cada uno de los roles se agrega al recuento de las finalizaciones de módulo.

**Las finalizaciones por producto**: desglose de lo aprendido las finalizaciones de rutas de acceso que el producto al que se asigna la ruta de aprendizaje. Si un módulo está asociado a varios productos, cada uno de los productos se agrega al recuento de las finalizaciones de módulo.

### <a name="completions-by-learning-individuals"></a>Finalizaciones por individuos de aprendizaje

Microsoft Learn identifica aprendices con un identificador de objeto de usuario. En el **ficha módulos**, todos los aprendices se ordenan por los módulos que se completó. Se muestran con su nombre de usuario Microsoft Learn, Id. de objeto y el recuento de módulos. Puede buscar con nombre de usuario.

Para obtener detalles de un aprendiz utilizando el identificador de objeto de usuario: 

1. Inicie sesión en [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer ). (Debe ser administrador global del inquilino de Azure AD de su empresa).

2. Copie el identificador de objeto de usuario para el [área resaltada](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) en el Explorador de Graph. 

