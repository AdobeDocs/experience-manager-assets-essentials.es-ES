---
title: Administración de informes en Assets Essentials
description: Acceda a los datos de la sección de informes de Assets Essentials para evaluar el uso de productos y funciones y obtener perspectivas sobre las métricas de éxito clave.
exl-id: c7155459-05d9-4a95-a91f-a1fa6ae9d9a4
source-git-commit: 49b650b3efe5740eb1ce39b7dcf6f84e34e0e81a
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 37%

---

# Administrar informes {#manage-reports}

Los informes de recursos proporcionan a los administradores visibilidad de la actividad del entorno de Adobe Experience Manager Assets Essentials. Estos datos proporcionan información útil sobre cómo los usuarios interactúan con el contenido y el producto. Cualquier persona usuaria puede acceder al panel de Insights. Además, las personas asignadas al perfil de producto del rol de administrador pueden crear informes definidos por el usuario.

## Acceso a los informes {#access-reports}

Todos los usuarios asignados al [Perfil de producto de los administradores de Assets Essentials](deploy-administer.md) pueden acceder al tablero de Insights activas o crear informes definidos por el usuario en Assets Essentials.

Para acceder a los informes, vaya a **[!UICONTROL Informes]** debajo de **[!UICONTROL Configuración]**.

![Informes](assets/reports.png)
<!--
In the **[!UICONTROL Reports]** screen, various components are shown in the tabular format which includes the following:

* **Title**: Title of the report
* **Type**: Determines whether the report is uploaded or downloaded to the repository
* **Description**: Provide details of the report that was given during uploading/downloading the report
* **Status**: Determines whether the report is completed, under progress, or deleted.
* **Author**: Provides email of the author who has uploaded/downloaded the report.
* **Created**: Gives information of the date when the report was generated.
-->

## Crear un informe {#create-report}

El entorno de AEM Assets Essentials ofrece funcionalidades completas de creación de informes a través del panel Informes. Esta capacidad permite a los usuarios generar y descargar informes CSV que detallan las cargas y descargas de recursos en intervalos de tiempo especificados, desde intervalos únicos hasta intervalos diarios, semanales, mensuales o anuales.

**Para crear un informe:**

1. Vaya a **Informes** y haga clic en **Crear informe** (en la parte superior derecha). El cuadro de diálogo **crear informe** muestra los siguientes campos:
   ![create-report](/help/using/assets/executed-reports1.svg)

   **En la ficha Configuración:**

   1. **Tipo de informe:** Seleccione entre el tipo de carga y descarga.
   1. **Título:** Agregue un título al informe.
   1. **Descripción:** Agregue una descripción opcional al informe.
   1. **Seleccionar ruta de acceso a la carpeta:** Seleccione una ruta de acceso a la carpeta para generar el informe de los recursos cargados y descargados dentro de esa carpeta específica. Por ejemplo, si necesita el informe de recursos cargados en una carpeta, especifique la ruta a esa carpeta.
   1. **Seleccionar intervalo de fecha:** Seleccione el intervalo de fecha para ver la actividad de carga o descarga dentro de la carpeta.
   <br>

   >[!NOTE]
   >
   > Assets Essentials convierte todas las zonas horarias locales a la hora universal coordinada (UTC).

   **En la ficha Columnas:** Seleccione los nombres de columna que se mostrarán en el informe. En la tabla siguiente se explica el uso de todas las columnas:

   <table>
    <tbody>
     <tr>
      <th><strong>El nombre de la columna</strong></th>
      <th><strong>Descripción</strong></th>
      <th><strong>Tipo de informe</strong></th>
     </tr>
     <tr>
      <td>Título</td>
      <td>El título del recurso.</td>
      <td>Cargar y descargar</td>
     </tr>
     <tr>
      <td>Ruta </td>
      <td>Ruta de la carpeta en la que el recurso está disponible en Assets Essentials.</td>
      <td>Cargar y descargar</td>
     </tr>
     <tr>
      <td>Tipo MIME</td>
      <td>Tipo MIME del recurso.</td>
      <td>Cargar y descargar</td>
     </tr>
     <tr>
      <td>Tamaño</td>
      <td>El tamaño del recurso en bytes.</td>
      <td>Cargar y descargar</td>
     </tr>
     <tr>
      <td>Descargado por</td>
      <td>ID de correo electrónico del usuario que descargó el recurso.</td>
      <td>Descargar</td>
     </tr>
     <tr>
      <td>Fecha de descarga</td>
      <td>La fecha en la que se realiza la acción de descarga de recursos.</td>
      <td>Descargar</td>
     </tr>
     <tr>
      <td>Autor</td>
      <td>El autor del recurso.</td>
      <td>Cargar y descargar</td>
     </tr>
     <tr>
      <td>Fecha de creación</td>
      <td>La fecha en la que el recurso se carga en Assets Essentials.</td>
      <td>Cargar y descargar</td>
     </tr>
     <tr>
      <td>Fecha de modificación</td>
      <td>La fecha de la última modificación del recurso.</td>
      <td>Cargar y descargar</td>
     </tr>
     <tr>
      <td>Caducado</td>
      <td>Estado de caducidad del recurso.</td>
      <td>Cargar y descargar</td>
     </tr>
     <tr>
      <td>Descargado por (nombre de usuario)</td>
      <td>Nombre del usuario que descargó el recurso.</td>
      <td>Descargar</td>
     </tr>           
    </tbody>
   </table>

## Ver y descargar un informe existente {#View-and-download-existing-report}

Los informes existentes se muestran en la ficha **Informes ejecutados**. Haga clic en **Informes** y seleccione **Informes ejecutados** para ver todos los informes creados con el estado **completado**, lo que indica que están listos para descargarse. Para descargar el informe en formato CSV o eliminarlo, seleccione la fila del informe. Luego selecciona **Descargar CSV** o **Eliminar**.
![ver y descargar informes existentes](/help/using/assets/view-download-existing-report.png)

## Programar un informe {#schedule-report}

AEM En la interfaz de usuario de Essentials, **Programar informe** configura una generación automática de informes en intervalos futuros especificados, como diario, semanal, mensual o anual. Esta función ayuda a optimizar las necesidades recurrentes de creación de informes y garantiza actualizaciones de datos puntuales. Mientras **Crear informe** genera informes para fechas pasadas. Los informes completados se enumeran en **Informes ejecutados** y los informes próximos se encuentran en **Informes programados**.

Para programar un informe, siga los pasos a continuación:

1. Haga clic en Informes en el panel izquierdo y, a continuación, haga clic en Crear informe (desde la parte superior derecha).
1. El cuadro de diálogo del informe muestra la siguiente información:
   1. **Tipo de informe:** Seleccione entre el tipo de carga y descarga.
   1. **Título:** Agregue un título al informe.
   1. **Descripción**: agregue una descripción opcional al informe.
   1. **Seleccionar ruta de carpeta:** Seleccione una ruta de carpeta para generar un informe para los recursos que se cargarán o descargarán de esa carpeta específica en el futuro.
   1. Alternar **Programar informe:** Alternar para programar el informe para un momento posterior o para su repetición repetida.
      ![informe de programación](/help/using/assets/schedule-reports1.svg)

   1. **Elija la frecuencia:** Especifique el intervalo para generar el informe (por ejemplo, diario, semanal, mensual, anual o una vez) y establezca la fecha y la hora para ejecutar el informe junto con la fecha final para la periodicidad. AEM Para un informe único, seleccione el intervalo de fechas para el informe en el tipo de actividad seleccionado en el entorno de trabajo de la actividad de la actividad de la que se ha hecho clic en el botón de la opción de menú de una sola vez. Por ejemplo, si necesita un informe sobre los recursos descargados del 10 al 29 (fechas futuras) de un mes específico, seleccione estas fechas en el campo **Seleccionar intervalo de fecha**.

   >[!NOTE]
   >
   > Assets Essentials convierte todas las zonas horarias locales a la hora universal coordinada (UTC).

## Ver informes programados {#view-scheduled-reports}

Los informes programados se muestran en la ficha **Informes programados** de una manera organizada de manera sistemática. Todos los informes completados de cada informe programado se almacenan en una sola carpeta de informes. Haga clic en ![expandir contracción](/help/using/assets/expand-icon1.svg) para ver los informes completados. Por ejemplo, si ha programado un informe diario, todos los informes completados se agrupan en una carpeta. Esta organización simplifica tanto la navegación como la detección de informes. Para ver los informes programados, haga clic en **Informes** y luego haga clic en **Informes programados**. Se muestran todos los informes programados con su estado en curso o completado. Los informes completados están listos para descargarse.
![informe programado](/help/using/assets/scheduled-reports-tab.png)

## Editar y cancelar informes programados {#edit-cancel-scheduled-reports}

1. Vaya a la pestaña **Informes programados**.
1. Seleccione la fila del informe.
1. Haga clic en **Editar**.
1. Haga clic en **Cancelar programación** y, a continuación, haga clic en **Confirmar** para cancelar el informe programado. Para los informes cancelados, el siguiente tiempo de ejecución pasa a estar vacío y el estado se muestra cancelado.
   ![editar y cancelar informe programado](/help/using/assets/cancel-edit-scheduled-reports.png)

### Reanudar programación {#resume-schedule}

Para reanudar la programación cancelada, seleccione la fila del informe y haga clic en **Reanudar programación**. Cuando se reanuda, las siguientes entradas de tiempo de ejecución se muestran de nuevo y el estado es En curso.
![reanudar programación](/help/using/assets/resume-schedule.png)

>[!NOTE]
>
> Si reanuda un informe cancelado antes de la fecha de finalización programada, los informes desde la fecha de cancelación hasta la fecha de reanudación se generan automáticamente.

## Vista Insights {#view-live-statistics}

>[!CONTEXTUALHELP]
>id="assets_reports"
>title="Informes"
>abstract="El panel de información le permite ver las métricas de eventos en tiempo real de su entorno de Experience Manager Assets durante los últimos 30 días o 12 meses. La lista de eventos incluye el número de descargas, cargas, búsquedas principales, etc."

Assets Essentials le permite ver datos en tiempo real de su entorno de Assets Essentials con el tablero de Insights. Puede ver las métricas de eventos en tiempo real durante los últimos 30 días o 12 meses.

<!--![Toolbar options when you select an asset](assets/assets-essentials-live-statistics.png)-->

Haga clic en **[!UICONTROL Insights]** en el panel de navegación izquierdo para ver los siguientes gráficos generados automáticamente:

* **Descargas**: el número de activos descargados del entorno de Assets Essentials en los últimos 30 días o 12 meses representados mediante un gráfico de líneas.
  ![descargas](/help/using/assets/insights-downloads2341.svg)

* **Cargas**: el número de recursos cargados en el entorno de Assets Essentials en los últimos 30 días o 12 meses representados mediante un gráfico de líneas.
  ![cargas](/help/using/assets/insights-uplods2.svg)

<!--* **Asset Count by Size**: The division of count of assets based on their range of various sizes from 0 MB to 100 GB.-->

* **Uso de almacenamiento**: el uso de almacenamiento, en bytes, para el entorno Assets Essentials representado mediante un gráfico de barras.
  ![Uso de almacenamiento](/help/using/assets/insights-storage-usage1.svg)
  <!--* **Delivery**: The graph depicts the count of assets as the delivery dates.-->

<!--* **Asset Count by Asset Type**: Represents count of various MIME types of the available assets. For example, application/zip, image/png, video/mp4, application/postscripte.-->

* **Búsquedas principales**: vea los términos más buscados junto con el número de veces que se buscan en su entorno de Assets Essentials en los últimos 30 días o 12 meses representados en un formato tabular.
  ![Uso de almacenamiento](/help/using/assets/insights-top-search.svg)

  <!--
   ![Insights](assets/insights1.png)
   ![Insights](assets/insights2.png)
   -->

* **Recuento de recursos por tamaño:** segmenta el recuento total de recursos en su entorno de Assets essentials en diferentes intervalos de tamaño, resaltando el recuento y el porcentaje de recursos en cada intervalo de tamaño, representado por un gráfico de anillo.
  ![insights-assets-count-by-size](/help/using/assets/insights-assets-count-by-size.svg)

* **Recuento de recursos por tipo de recurso:** Segmenta el recuento total de recursos en su entorno de Assets essentials, destacando el recuento y el porcentaje de recursos en función de sus tipos de archivos, representados por un gráfico circular.
  ![insights-assets-count-by-size](/help/using/assets/insights-assest-count-by-asset-type1.svg)

