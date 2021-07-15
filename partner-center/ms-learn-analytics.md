---
title: Centro de partners Ideas Microsoft Learn analytics
ms.topic: article
ms.date: 08/13/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Realice un seguimiento de los aprendices de su empresa mediante el aprovechamiento de datos en aprendizaje individual, módulos completados, rutas de aprendizaje completadas y mucho más.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e5d73582d3cfe0aa19483526d9b77e55a4c7e0a0
ms.sourcegitcommit: 70b8ebbe0d431c7a13529f9eabd1b24f40108a46
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 07/14/2021
ms.locfileid: "113989764"
---
# <a name="use-microsoft-learn-analytics-reports"></a>Uso de Microsoft Learn de análisis

**Roles adecuados:** administrador global | Administrador de asociados de MPN

El [Microsoft Learn](/learn/) proporciona información sobre los aprendices de la empresa, incluidos los módulos que han completado y las rutas de aprendizaje en las que se encuentran. El informe muestra el estado de cada aprendiz individual. Los administradores globales y los administradores de MPN de una empresa pueden ver los datos.

## <a name="how-to-read-the-report"></a>Cómo leer el informe

### <a name="summary-charts"></a>Gráficos de resumen

En estos gráficos se resumen las tendencias acumulativas mensuales y de recuento de personas entrenadas, las finalizaciones de módulos y las rutas de aprendizaje.

**Recuento de individuos entrenados:** recuento de todos los aprendices distintos que han completado al menos un módulo durante el intervalo de fechas seleccionado 

**Mini chart de tendencias de individuos entrenados:** recuento acumulado mes a mes de los aprendices activos 

**Recuento de finalizaciones de módulo:** recuento de finalizaciones de módulos por parte de los aprendices de la empresa del asociado durante el intervalo de fechas seleccionado.
Por ejemplo, si "Módulo 1" lo completan 15 personas y el "Módulo 2" lo han completado las mismas 15 personas, el número de finalizaciones del módulo será de 30. La fecha de finalización del módulo debe estar en el intervalo de fechas seleccionado.

**Mini chart de tendencia de finalizaciones de módulos:** recuento acumulado mes a mes de las finalizaciones del módulo 

Learning de finalizaciones **de rutas** de acceso: recuento de Learning las finalizaciones de rutas de acceso por parte de los aprendices de la empresa del asociado durante el intervalo de fechas seleccionado.
Por ejemplo, si 20 personas completan la ruta de acceso "Ruta 1" de Learning y la ruta de acceso de Learning "ruta 2" la han completado las mismas 20 personas, el recuento de finalización de la ruta de acceso de Learning será de 40. La Learning de finalización de la ruta de acceso debe estar dentro del intervalo de fechas seleccionado.

**Learning mini chart de tendencia de** finalizaciones de ruta de acceso: recuento acumulado mes a mes de las finalizaciones de la ruta de aprendizaje 

### <a name="trained-individuals-monthly-trend"></a>Tendencia mensual de los usuarios entrenados

Estos datos son la tendencia de los usuarios de la empresa que han completado un módulo por primera vez en ese mes. 

**Eje X es** mes para el filtro de tiempo seleccionado. 

**Eje Y es el** recuento de aprendices activos que se han registrado (finalización por primera vez de un módulo) durante ese mes. Esto no es acumulativo.

### <a name="module-completions-monthly-trend"></a>Tendencia mensual de finalizaciones de módulos

Estos datos son la tendencia de los módulos completados por todos los usuarios de la empresa durante ese mes. (no acumulativo) 

**Eje X es** mes para el filtro de tiempo seleccionado. 

**Eje Y es** el recuento de las finalizaciones del módulo durante ese mes. Esto no es acumulativo.

### <a name="learning-path-completions-monthly-trend"></a>Learning tendencia mensual de finalizaciones de rutas de acceso

Estos datos son la tendencia de las rutas de aprendizaje completadas por los usuarios de la empresa durante ese mes. (no acumulativo) 

**Eje X es** mes para el filtro de tiempo seleccionado. 

**Eje Y es el** recuento de finalizaciones de módulos en ese mes. Esto no es acumulativo.

### <a name="learning-path-completion-tabs"></a>Learning pestañas de finalización de rutas de acceso

#### <a name="module-tab"></a>Pestaña Módulo

Esta pestaña incluye un desglose de los módulos completados en su empresa por los cinco nombres de módulo principales. el producto al que está asociado el módulo; y el rol de usuario pertinente para el módulo.  

- Gráfico de anillos de finalizaciones de módulo: desglose de las finalizaciones del módulo (recuento mostrado en la sección de resumen) por los nombres de módulo.

El número mostrado en el centro del gráfico es el total de módulos completados

- Finalizaciones por rol: desglose de las finalizaciones del módulo por el rol del módulo. Si un módulo está asociado a varios roles, cada uno de los roles se agrega al recuento de finalizaciones de módulos.

El número que se muestra en el centro del gráfico es el número de roles distintos para las finalizaciones del módulo. 

- Finalizaciones por producto: desglose de las finalizaciones del módulo por el producto al que está asignado el módulo. Si un módulo está asociado a varios productos, cada uno de ellos se agrega al recuento de finalizaciones de módulos.    

El número que se muestra en el centro del gráfico es el número de productos distintos para las finalizaciones del módulo.  

#### <a name="learning-path-tab"></a>Learning de acceso

Esta pestaña incluye un desglose de las rutas de aprendizaje completadas en su empresa por los cinco nombres de módulo principales. el producto al que está asignada la ruta de aprendizaje; y el rol pertinente a esta ruta de aprendizaje.  

- Learning gráfico de anillos de finalizaciones de rutas de acceso: desglose de las finalizaciones Learning ruta de acceso (recuento mostrado en la sección de resumen) por nombre.

- Finalizaciones por rol: desglose de las finalizaciones de las rutas de aprendizaje por el rol. Si un módulo está asociado a varios roles, cada uno de los roles se agrega al recuento de finalizaciones de módulo.

- Finalizaciones por producto: desglose de las finalizaciones de las rutas de aprendizaje por el producto al que está asignada la ruta de aprendizaje. Si un módulo está asociado a varios productos, cada uno de ellos se agrega al recuento de finalizaciones de módulos.

### <a name="completions-by-learning-individuals"></a>Finalizaciones mediante el aprendizaje de individuos

Aquí se enumeran los usuarios entrenados de su empresa y los detalles de sus módulos completados y rutas de aprendizaje.

Microsoft Learn identifica a los aprendices con un identificador de objeto de usuario. En la **pestaña Módulos**, todos los aprendices se ordenan por los módulos completados. Se muestran con su nombre de Microsoft Learn nombre de usuario, identificador de objeto y número de módulos. Puede buscar con el nombre de usuario. 

En la **pestaña Learning** rutas de acceso de aprendizaje se muestran todos los aprendices ordenados por rutas de aprendizaje completadas, con el nombre para mostrar del aprendiz, el identificador de objeto y el número de módulos.

Para obtener los detalles de un aprendiz mediante el identificador de objeto de usuario: 

1. Inicie sesión en [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer ). (Debe ser el administrador global del inquilino de Azure AD empresa).

2. Copie el identificador de objeto de usuario en [el área resaltada](https://graph.microsoft.com/v1.0/users/a9633ad7-c8dc-4587-b119-0bc286b0711f) en Graph Explorer. 

## <a name="frequently-asked-questions-faq"></a>Preguntas más frecuentes

1. No puedo ver los detalles de learn de mi empresa.

   Este informe está disponible para los asociados que tienen una cuenta en Centro de partners. Si todavía está en Partner Membership Center, no podrá ver este informe.

2. Quién mi empresa puede ver este informe? 

   El administrador global y el administrador de MPN pueden ver el informe.

3. ¿Cómo puedo asegurarme de que todos nuestros usuarios asocien sus Microsoft Learn a su Centro de partners cuenta?

   *Después de que* el administrador global agrega un nuevo usuario, ese usuario debe ir a [Microsoft Learn](/learn/) para vincular su cuenta corporativa de Azure Active Directory (AD) o su cuenta de trabajo con su cuenta de Learn. Esto garantiza que Ideas Learning pestaña mostrará los cursos y las aptitudes adecuados.
   
   El usuario debe:
   
   1. Inicie sesión [Microsoft Learn](/learn/).
   2. Seleccione su imagen de perfil y, a **continuación, Mi perfil**.
   3. Haga clic en **Configuración**.
   4. En **Administración de cuentas,** agregue su cuenta de trabajo en **Cuentas vinculadas.**

4. ¿Puedo ver todos los usuarios de la empresa que inician sesión Microsoft Learn con una cuenta de MSA en este informe?

   Actualmente, la mejor manera de hacerlo es agregar estos usuarios al inquilino de Azure AD y, a continuación, agregarlos a Centro de partners para que puedan asociar su cuenta de Microsoft Learn a través de **Mi perfil** en Centro de partners. 

   Para los usuarios que solo usan su cuenta de MSA para el entrenamiento, en un futuro próximo, el equipo de Microsoft Learn les permitirá asociar su correo electrónico de trabajo a su perfil de Microsoft Learn. 

## <a name="next-steps"></a>Pasos siguientes

Para obtener más informes, [vea Centro de partners Ideas](partner-center-insights.md).

>[!NOTE] 
> Puede descargar los datos sin procesar que se están generando en este informe desde la sección Descargar informes del panel Ideas datos. [Más información](pci-download-reports.md) 
