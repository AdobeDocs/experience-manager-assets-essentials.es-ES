---
title: Cargar recursos al repositorio
description: Cargar recursos a [!DNL Assets Essentials], ver estados de carga y resolver problemas de carga.
role: Business Practitioner
source-git-commit: e54cdf9b8ecb5d9ddc5b90a3ca82549c61b35074
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---


# Cargar recursos {#add-assets}

Para agregar nuevos recursos con los que trabajar, cargue algunos recursos desde el sistema de archivos local. <!-- TBD: Many of the [common file formats are supported](/help/supported-file-formats.md). -->

Puede utilizar los siguientes métodos para cargar uno o varios recursos o una carpeta que contenga recursos:

* Arrastre recursos o carpetas en la interfaz de usuario y siga las instrucciones que aparecen en la pantalla.
* Haga clic en la opción **[!UICONTROL Add Assets]** de la barra de herramientas y añada algunos archivos al cuadro de diálogo de carga.

<!-- TBD: Update this GIF
![Asset and nested folder upload demo](assets/do-not-localize/upload-assets.gif) -->

Puede utilizar cualquiera de estos métodos para cargar recursos después de crear una carpeta. Para crear una carpeta vacía, haga clic en **[!UICONTROL Create Folder]** en la barra de herramientas. Aunque [!DNL Assets Essentials] ofrece una potente funcionalidad de búsqueda de texto completo, también puede utilizar carpetas para organizar mejor sus recursos.

Una vez seleccionados los archivos, aparece un cuadro de diálogo de confirmación para añadir más archivos o para eliminar los archivos ya seleccionados. Para agregar más archivos a una selección, haga clic en **[!UICONTROL Browse]** y seleccione **[!UICONTROL Browse files]** o **[!UICONTROL Browse folders]**. Añada más archivos o carpetas de la misma carpeta o de otra carpeta.

Una vez que todos los archivos estén en cola, haga clic en **[!UICONTROL Upload]**.

![Cargar archivos y carpetas](assets/upload-browse-files-folders.png)

*Figura: Antes de cargar los recursos seleccionados, puede agregarlos o eliminarlos de la cola.*

>[!CAUTION]
>
>Utilice recursos que no tengan espacios en blanco en los nombres de archivo. Las respuestas a los comentarios no funcionan para estos activos.

## Ver el progreso y estado de la carga {#upload-progress}

Al cargar muchos recursos o carpetas anidadas en [!DNL Assets Essentials], es posible que algunos recursos no se carguen por varios motivos, como problemas de red y recursos duplicados.

Para realizar un seguimiento del progreso de carga, haga clic en la opción **[!UICONTROL Upload Progress]** de la barra de herramientas. Un panel muestra el progreso de carga de todos los recursos.

Para ver un subconjunto de recursos en función del progreso o estado de carga, utilice el filtro de la barra lateral **[!UICONTROL Upload Progress]**. Los distintos filtros muestran todos los recursos, las cargas completadas, las cargas en curso, los recursos en cola que se van a cargar, las cargas en pausa, los recursos duplicados y los recursos que no se han cargado.

![Filtrado del progreso de carga en función del estado de carga](assets/filter-upload-progress.png)

*Figura: Filtre los recursos que ha intentado cargar en función de su estado de carga o del progreso de carga.*

Inmediatamente después de cargar los recursos, [!DNL Assets Essentials] los procesa para generar miniaturas y procesar metadatos. Para muchos recursos, el procesamiento lleva algún tiempo. Si no ve una miniatura y ve un mensaje de procesamiento en la miniatura del marcador de posición, vuelva a comprobar la carpeta después de unos minutos.

![Procesamiento al cargar](assets/upload-processing.png)

## Representaciones de recursos {#renditions}

[!DNL Assets Essentials] procesa los recursos cargados casi en tiempo real y, para muchos tipos de archivo admitidos, genera representaciones. Creadas para imágenes, las representaciones son versiones cambiadas de tamaño de la imagen cargada. Puede descargar no solo el recurso, sino también las representaciones para utilizar una versión adecuada. Puede ver todas las representaciones de un recurso al [obtener una vista previa de un recurso](/help/navigate-view.md#preview-assets).

![Representaciones](assets/renditions-view-download.png)

## Administrar cargas fallidas {#resolve-upload-fails}

Si la carga de un recurso admitido falla por algún motivo, haga clic en **[!UICONTROL Retry]** en el panel [!UICONTROL Upload Progress].

![Reintentar una carga fallida](assets/upload-retry.png)

*Figura: Vuelva a intentarlo si un archivo compatible no se puede cargar por algún motivo.*

Si intenta cargar recursos duplicados, estos no se cargarán hasta que confirme explícitamente la carga. Al principio, los recursos duplicados se marcan como cargas fallidas. Para resolverlo, simplemente puede crear una versión, eliminar y reemplazar los recursos existentes o crear una copia duplicada cambiando el nombre del recurso. Puede resolver estos errores de un recurso a la vez o hacerlo de forma masiva para todos los duplicados fallidos de una sola vez.

![Administrar activos duplicados de uno en uno](assets/uploads-manage-duplicates.png)

*Figura: Para los recursos duplicados que no se cargan de forma predeterminada, resuelva el problema de uno en uno.*

![Administrar todas las cargas fallidas de forma masiva](assets/upload-progress-manage-failed-uploads.png)

*Figura: Para los recursos duplicados que no se cargan de forma predeterminada, resuelva los problemas de todos los recursos a la vez.*

>[!TIP]
>
>Puede cargar recursos en el repositorio de DAM directamente desde las aplicaciones de escritorio [!DNL Creative Cloud] . Consulte cómo [[!DNL Assets Essentials] se integra con [!DNL Adobe Asset Link]](/help/integration.md).

## Eliminar recursos o carpetas {#delete-assets}

Los usuarios pueden eliminar recursos o carpetas individuales que ya no sean necesarios. Para eliminar un recurso o una carpeta, realice una de las siguientes acciones:

* Utilice la opción disponible en la miniatura de un recurso o de una carpeta.

   ![Opciones en la miniatura de un recurso para administrar un recurso](assets/options-on-thumbnail.png)

* Seleccione un recurso o una carpeta y haga clic en **[!UICONTROL Delete]** ![eliminar icono](assets/do-not-localize/delete-icon.png) en la barra de herramientas.
