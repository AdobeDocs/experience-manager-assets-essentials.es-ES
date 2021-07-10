---
title: Formatos de archivo compatibles
description: Formatos de archivo compatibles con los distintos casos de uso de [!DNL Assets Essentials]
role: User,Leader,Admin,Architect,Developer
contentOwner: AG
source-git-commit: c63e9ab1054398dc055643f0dca6631bae881047
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 24%

---


# Compatibilidad con formatos de archivo en [!DNL Assets Essentials] {#file-format-support}

[!DNL Assets Essentials] admite una amplia gama de formatos de archivo y cada funcionalidad tiene compatibilidad variada con distintos tipos de archivo.

* ![tipo de archivo de imagen ](assets/do-not-localize/image-icon.png) iconImágenes: GIF, JPG, PNG y TIFF
* ![tipo de archivo de documento ](assets/do-not-localize/document-icon.png) iconoDocumentos: DOCX, PDF, PPTX y XLSX
* ![tipo de archivo de vídeo ](assets/do-not-localize/video-icon.png) iconVídeos: MP4

Los distintos tipos de archivo tienen diferentes grados de compatibilidad con los casos de uso y las funciones, como se describe a continuación. Utilice la leyenda para comprender el nivel de asistencia.

| Nivel de asistencia | Descripción |
|-------------------|-------------------------|
| ✓ | Compatible |
| ✓ | Compatible condicionalmente |
| - | No aplicable |

## Agregar, cargar y ver recursos {#support-to-upload-view}

<!-- TBD: For AEM, AI files require the PDF option to be selected when saving the AI file.
-->

| Tipo de recurso | [Examinar](/help/navigate-view.md) | Copiar | [Cargar](/help/add-delete.md) | Crear | [Eliminar](/help/add-delete.md#delete-assets) | Detalles | Zoom de imagen | [Vistos recientemente](/help/navigate-view.md) |
|-------------------|----------|----------|----------|----------|----------|-------------------|------------|-----------------|
| Imágenes rasterizadas | ✓ | ✓ | ✓ | - | ✓ | ✓ | ✓ | ✓ |
| Carpetas | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | - | - |
| Vídeos MP4 | ✓ | ✓ | ✓ | - | ✓ | ✓ | - | ✓ |
| PDF | ✓ | ✓ | ✓ | - | ✓ | ✓ | - | ✓ |
| PSD, AI e INDD | ✓ | ✓ | ✓ | - | ✓ | ✓ | - | ✓ |

<!-- Hiding CC Libraries (considered beta) as per PM feedback.
| CC Libraries  | &#10003; | &minus;  | &#10003; | &#10003; | &#10003; | &#10003; | &minus;    | &minus;         |
-->

## Buscar, utilizar y editar recursos {#support-to-search-use-edit}

| Tipo de recurso | [Descargar](/help/manage-organize.md#download) | Arrastrar y colocar | [Editor de imágenes](/help/edit-images.md) | [Buscar](/help/search.md) | [Etiquetas inteligentes](/help/metadata.md#tags) | [Cambiar nombre](/help/manage-organize.md) | [Versiones](/help/manage-organize.md#versions-of-assets) |
|---------------|----------|---------------|--------------|----------|------------|----------|----------|
| Imágenes rasterizadas | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Carpetas | ✓ | ✓ | - | ✓ | - | ✓ | - |
| Vídeos | ✓ | ✓ | - | ✓ | ✓ | ✓ | - |
| Bibliotecas CC | - | - | - | - | - | ✓ | - |
| PDF | ✓ | ✓ | - | ✓ | ✓ | ✓ | - |
| PSD | ✓ | ✓ | - | ✓ | ✓ | ✓ | - |
| AI | ✓ | ✓ | - | ✓ | ✓ | ✓ | - |
| INDD | ✓ | ✓ | - | ✓ | ✓ | ✓ | - |

## Revisar recursos y colaborar {#support-to-review-collaborate}

| Tipo de recurso | Anotar | Comentario | Crear tareas y revisar |
|---------------|----------|----------|-------------------------|
| Imágenes rasterizadas | ✓ | ✓ | ✓ |
| Carpetas | - | - | - |
| Vídeos | - | ✓ | ✓ |
| Bibliotecas CC | - | - | - |
| PDF | - | ✓ | ✓ |
| PSD | - | ✓ | ✓ |
| AI | - | ✓ | ✓ |
| INDD | - | ✓ | ✓ |

## Otras tareas de administración de recursos {#support-to-manage-assets}

| Tipo de recurso | [Metadatos](/help/metadata.md) | [Representaciones](/help/add-delete.md#renditions) | [Papelera](/help/add-delete.md#delete-assets) | Copiar | Mover |
|---------------|-------------------|------------|----------|----------|----------|
| Imágenes rasterizadas | ✓ | ✓ | ✓ | ✓ | ✓ |
| Carpetas | ✓ | - | ✓ | ✓ | ✓ |
| Vídeos | ✓ | - | ✓ | ✓ | ✓ |
| Bibliotecas CC | ✓ | - | - | - | - |
| PDF | ✓ | - | ✓ | ✓ | ✓ |
| PSD | ✓ | - | ✓ | ✓ | ✓ |
| AI | ✓ | - | ✓ | ✓ | ✓ |
| INDD | ✓ | - | ✓ | ✓ | ✓ |

Los usuarios de [!DNL Adobe Asset Link] pueden registrar las imágenes de trama en el repositorio [!DNL Assets Essentials] desde las aplicaciones de escritorio [!DNL Adobe Creative Cloud] soportadas.

<!-- TBD: Saving the template table separately for later use.
| Asset type    | Features |
|---------------|----------|
| Raster images |          |
| Folders       |          |
| Videos        |          |
| CC Libraries  |          |
| PDF files     |          |
| PSD           |          |
| AI            |          |
| INDD          |          |

>[!MORELIKETHIS]
>
>* []()
-->
