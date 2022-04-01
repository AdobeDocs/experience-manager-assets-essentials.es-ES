---
title: Administración de recursos digitales
description: Mueva, elimine, copie, cambie de nombre, actualice y convierta en versión los recursos en [!DNL Assets Essentials].
role: User,Leader
contentOwner: AG
exl-id: b01e98b9-0cc2-47c5-9f5b-79b8e6bef39f
source-git-commit: cd7af0c946a042430e62528fa6aa19bdab139f67
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 100%

---

# Administración de recursos {#manage-assets}

Puede realizar varias tareas de administración de activos digitales (DAM) fácilmente mediante la interfaz de usuario sencilla de usar de [!DNL Assets Essentials]. Una vez añadidos los recursos, puede buscarlos, descargarlos, moverlos, copiarlos, cambiarles el nombre, eliminarlos, actualizarlos y editarlos.

Use [!DNL Assets Essentials] para llevar a cabo las siguientes tareas de administración de recursos. Al seleccionar un recurso, aparecen las siguientes opciones en la barra de herramientas de la parte superior.

![Opciones de la barra de herramientas al seleccionar un recurso](assets/toolbar-image-selected.png)

*Imagen: opciones disponibles en la barra de herramientas de una imagen seleccionada.*

* ![icono de anular selección](assets/do-not-localize/close-icon.png) Anule la selección.
* ![icono de detalles](assets/do-not-localize/edit-in-icon.png) Haga clic para previsualizar un recurso y ver los metadatos detallados. Al previsualizar, puede ver las versiones y editar una imagen.
* ![icono de descarga](assets/do-not-localize/download-icon.png) Descargue el recurso seleccionado en el sistema de archivos local.
* ![icono de eliminación](assets/do-not-localize/delete-icon.png) Elimine el recurso o la carpeta seleccionados.
* ![icono de cierre de compra](assets/do-not-localize/checkout-icon.png) Cierre el recurso seleccionado.
* ![icono de copia](assets/do-not-localize/copy-icon.png) Copie el archivo o la carpeta seleccionados.
* ![icono de movimiento](assets/do-not-localize/move-icon.png) Mueva el recurso o la carpeta seleccionados a una ubicación diferente en la jerarquía del repositorio.
* ![icono de cambio de nombre](assets/do-not-localize/rename-icon.png) Cambie el nombre del recurso o la carpeta seleccionados. Utilice un nombre único, si no, el cambio de nombre producirá un error con una advertencia. Puede intentarlo de nuevo con un nombre nuevo.
* ![icono de asignación de tarea](assets/do-not-localize/review-delegate-icon.png) Asigne tareas a otros usuarios para colaborar en un recurso.

Puede ver las mismas opciones en las miniaturas de recursos.

![Opciones en la miniatura de un recurso para administrarlo](assets/options-on-thumbnail.png)

[!DNL Assets Essentials] muestra únicamente las opciones relevantes de la barra de herramientas que dependen del tipo de recurso seleccionado.

![Opciones de la barra de herramientas al seleccionar un recurso](assets/toolbar-folder-selected.png)

*Imagen: opciones disponibles en la barra de herramientas de una carpeta seleccionada.*

![Opciones de la barra de herramientas al seleccionar un recurso](assets/toolbar-pdf-selected.png)

*Imagen: opciones disponibles en la barra de herramientas de un archivo PDF seleccionado.*

## Descarga y distribución de recursos {#download}

Puede seleccionar uno o varios recursos, carpetas o una combinación de ambos y descargar la selección en el sistema de archivos local. Puede editar los recursos y volver a cargarlos o distribuirlos fuera de [!DNL Assets Essentials]. Además, puede [descargar las representaciones](/help/add-delete.md#renditions) de un recurso.

## Creación de versiones de recursos {#versions-of-assets}

<!-- 
TBD: query for engineering: How many versions are maintained. What happens when we reach that limit? Are old versions automatically removed? -->

[!DNL Assets Essentials] crea versiones de los recursos cuando se cargan de nuevo y se actualizan o editan. Puede ver el historial de versiones actuales y anteriores, así como restaurar una versión anterior de los recursos como la última versión, que se revierte a una anterior si es necesario. Las versiones de los recursos se crean en los siguientes casos:

* Cargue un nuevo recurso con el mismo nombre de archivo que uno existente y en la misma carpeta que este. [!DNL Assets Essentials] le solicita que sobrescriba el recurso anterior o que guarde el nuevo como una versión. Consulte [Carga de recursos duplicados](/help/add-delete.md#resolve-upload-fails).

   ![Creación de versiones al cargar](assets/uploads-manage-duplicates.png)

   *Imagen: al cargar un recurso con el mismo nombre que uno existente, puede crear una versión de este.*

* Edite una imagen y haga clic en **[!UICONTROL Guardar como versión]**. Consulte [Edición de imágenes](/help/edit-images.md).

   ![Guardar imagen editada como versión](assets/edit-image2.png)

   *Imagen: guardar imagen editada como versión.*

* Abra las versiones de un recurso existente. Haga clic en **[!UICONTROL Nueva versión]** y cargue una versión más reciente del recurso en el repositorio.

   ![Opción para cargar una nueva versión de un recurso desde el historial de versiones](assets/view-asset-versions2.png)

### Visualización de versiones de un recurso {#view-versions}

Al cargar una copia duplicada o modificada de un recurso, puede crear sus versiones. Las versiones le permiten revisar los recursos históricos y revertirlos a una versión anterior si es necesario.

Para ver las versiones, abra la previsualización de un recurso y haga clic en **[!UICONTROL Versiones]** ![Icono de versiones](assets/do-not-localize/versions-clock-icon.png) en la barra lateral derecha. Para previsualizar una versión específica, selecciónela. Para volver a ella, haga clic en **[!UICONTROL Crear más reciente]**.

También puede crear versiones a partir de la cronología de las versiones. Seleccione la última versión, haga clic en **[!UICONTROL Nueva versión]** y cargue una copia nueva del recurso desde el sistema de archivos local.

![Visualización de versiones de un recurso](assets/view-asset-versions1.png)

*Imagen: visualización de versiones de un recurso, reversión a una versión anterior o carga de otra versión nueva.*
