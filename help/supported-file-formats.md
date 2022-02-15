---
title: Formatos de archivo compatibles
description: Formatos de archivo compatibles con los distintos casos de uso de [!DNL Assets Essentials]
role: User,Leader,Admin,Architect,Developer
contentOwner: AG
exl-id: bc44e98d-446e-41ff-b5b4-9dc324834630
source-git-commit: b9d333a862cca6227ef386ae8dadf431c2fb6d71
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 16%

---

# Los formatos de archivo son compatibles con [!DNL Assets Essentials] {#file-format-support}

[!DNL Assets Essentials] admite una amplia gama de formatos de archivo y cada funcionalidad tiene compatibilidad variada con distintos tipos de archivo.

* ![icono de tipo de archivo de imagen](assets/image-icon.svg) Imágenes: JPG, PNG, GIF, TIFF y otros
* ![icono de tipo nube creativa](assets/creative-cloud-files.svg) archivos Creative Cloud: PSD, IA e INDD
* ![icono de tipo cámara](assets/camera-icon.svg) archivos Camera Raw: CR2/CR3, NEF, SRW/SRF y otros
* ![icono de tipo de archivo de documento](assets/document-icon.svg) Documentos: DOCX, PDF, PPTX y XLSX
* ![icono de tipo de archivo de vídeo](assets/video-icon.svg) Vídeos: MP4

[!DNL Assets Essentials] admite cualquier formato de archivo binario con servicios básicos como, por ejemplo, almacenamiento, carga, copia, movimiento, eliminación y adición de metadatos.

[!DNL Assets Essentials] también admite archivos RAW de cámara de una amplia gama de fabricantes líderes de cámaras, incluidos Canon (CR2/CR3), Nikon (NEF), Sony (SRW/SRF), Fujifilm (RAF), Olympus (ORF) y otros, con tecnología Adobe Camera Raw.

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
| Archivos RAW | ✓ | ✓ | ✓ | - | ✓ | ✓ | ✓ | ✓ |
| Carpetas | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | - | - |
| Vídeos MP4 | ✓ | ✓ | ✓ | - | ✓ | ✓ | - | ✓ |
| PDF | ✓ | ✓ | ✓ | - | ✓ | ✓ | - | ✓ |
| PSD, IA e INDD | ✓ | ✓ | ✓ | - | ✓ | ✓ | - | ✓ |
| Otros archivos binarios | ✓ | ✓ | ✓ | - | ✓ | ✓ | - | ✓ |

<!-- Hiding CC Libraries (considered beta) as per PM feedback.
| CC Libraries  | &#10003; | &minus;  | &#10003; | &#10003; | &#10003; | &#10003; | &minus;    | &minus;         |
-->

## Buscar, utilizar y editar recursos {#support-to-search-use-edit}

| Tipo de recurso | [Descargar](/help/manage-organize.md#download) | Arrastrar y colocar | [Editor de imágenes](/help/edit-images.md) | [Buscar](/help/search.md) | [Etiquetas inteligentes](/help/metadata.md#tags) | [Cambiar nombre](/help/manage-organize.md) | [Versiones](/help/manage-organize.md#versions-of-assets) |
|---------------|----------|---------------|--------------|----------|------------|----------|----------|
| Imágenes rasterizadas | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Archivos RAW | ✓ | ✓ | - | ✓ | ✓ | ✓ | ✓ | ✓ |
| Carpetas | ✓ | ✓ | - | ✓ | - | ✓ | ✓ |
| Vídeos | ✓ | ✓ | - | ✓ | ✓ | ✓ | ✓ |
| Bibliotecas CC | - | - | - | - | - | ✓ | ✓ |
| PDF | ✓ | ✓ | - | ✓ | ✓ | ✓ | ✓ |
| PSD, IA e INDD | ✓ | ✓ | - | ✓ | ✓ | ✓ | ✓ |
| Otros archivos binarios | ✓ | ✓ | - | ✓ | - | ✓ | ✓ |


## Revisar recursos y colaborar {#support-to-review-collaborate}

| Tipo de recurso | Anotar | Comentario | Crear tareas y revisar |
|---------------|----------|----------|-------------------------|
| Imágenes rasterizadas | ✓ | ✓ | ✓ |
| Archivos RAW | ✓ | ✓ | ✓ |
| Carpetas | - | - | - |
| Vídeos | - | ✓ | ✓ |
| Bibliotecas CC | - | - | - |
| PDF | - | ✓ | ✓ |
| PSD, IA e INDD | - | ✓ | ✓ |
| Otros archivos binarios | - | ✓ | ✓ |

## Otras tareas de administración de recursos {#support-to-manage-assets}

| Tipo de recurso | [Metadatos](/help/metadata.md) | [Representaciones](/help/add-delete.md#renditions) | [Papelera](/help/add-delete.md#delete-assets) | Copiar | Mover |
|---------------|-------------------|------------|----------|----------|----------|
| Imágenes rasterizadas | ✓ | ✓ | ✓ | ✓ | ✓ |
| Archivos RAW | ✓ | ✓ | ✓ | ✓ | ✓ |
| Carpetas | ✓ | - | ✓ | ✓ | ✓ |
| Vídeos | ✓ | - | ✓ | ✓ | ✓ |
| Bibliotecas CC | ✓ | - | - | - | - |
| PDF | ✓ | - | ✓ | ✓ | ✓ |
| PSD, IA e INDD | ✓ | - | ✓ | ✓ | ✓ |
| Otros archivos binarios | ✓ | - | ✓ | ✓ | ✓ |

Usuarios de [!DNL Adobe Asset Link] puede cargar y registrar archivos (cargar una nueva versión) en el [!DNL Assets Essentials] del repositorio admitido [!DNL Adobe Creative Cloud] aplicaciones de escritorio.

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
