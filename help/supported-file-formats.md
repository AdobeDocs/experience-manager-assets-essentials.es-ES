---
title: Formatos de archivo compatibles
description: Formatos de archivo compatibles con los distintos casos de uso de [!DNL Assets Essentials]
role: User,Leader,Admin,Architect,Developer
contentOwner: AG
exl-id: bc44e98d-446e-41ff-b5b4-9dc324834630
source-git-commit: 02f28c00b387fbcac4cd917fab7763124fdd5d70
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 87%

---

# Compatibilidad de formatos de archivo en [!DNL Assets Essentials] {#file-format-support}

[!DNL Assets Essentials] admite una amplia gama de formatos de archivo y cada funcionalidad tiene compatibilidad variada con distintos tipos de archivo.

* ![icono de tipo de archivo de imagen](assets/image-icon.svg) Imágenes: JPG, PNG, GIF, TIFF y otros
* ![icono de tipo Creative Cloud](assets/creative-cloud-files.svg) Archivos de Creative Cloud: PSD, IA e INDD
* ![icono de tipo cámara](assets/camera-icon.svg) Archivos de Camera Raw: CR2/CR3, NEF, SRW/SRF y otros
* ![icono de tipo de archivo de documento](assets/document-icon.svg) Documentos: DOCX, PDF, PPTX y XLSX
* ![icono de tipo de archivo de vídeo](assets/video-icon.svg) Vídeos: MP4

[!DNL Assets Essentials] admite cualquier formato de archivo binario con servicios básicos como, por ejemplo, almacenamiento, carga, copia, movimiento, eliminación y adición de metadatos.

[!DNL Assets Essentials] también admite archivos RAW de cámara de una amplia gama de fabricantes líderes de cámaras, incluidos Canon (CR2/CR3), Nikon (NEF), Sony (SRW/SRF), Fujifilm (RAF), Olympus (ORF) y otros, con tecnología Adobe Camera Raw.

Los distintos tipos de archivo tienen diferentes grados de compatibilidad con los casos de uso y las funciones, como se describe a continuación. Utilice la leyenda para comprender el nivel de compatibilidad.

| Nivel de soporte | Descripción |
|-------------------|-------------------------|
| ✓ | Compatibilidad |
| ✓ ‡ | Compatible con condiciones |
| − | No aplicable |

## Adición, carga y visualización de recursos {#support-to-upload-view}

<!-- TBD: For AEM, AI files require the PDF option to be selected when saving the AI file.
-->

| Tipo de recurso | [Examinar](/help/navigate-view.md) | Copiar | [Cargar](/help/add-delete.md) | Crear | [Eliminar](/help/add-delete.md#delete-assets) | Detalles | Zoom de imagen | [Vistos recientemente](/help/navigate-view.md) |
|-------------------|----------|----------|----------|----------|----------|-------------------|------------|-----------------|
| Rasterización de imágenes | ✓ | ✓ | ✓ | - | ✓ | ✓ | ✓ | ✓ |
| Archivos RAW | ✓ | ✓ | ✓ | - | ✓ | ✓ | ✓ | ✓ |
| Carpetas | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | - | - |
| Vídeos MP4 | ✓ | ✓ | ✓ | - | ✓ | ✓ | - | ✓ |
| PDF | ✓ | ✓ | ✓ | - | ✓ | ✓ | - | ✓ |
| PSD, IA e INDD | ✓ | ✓ | ✓ | - | ✓ | ✓ | - | ✓ |
| Otros archivos binarios | ✓ | ✓ | ✓ | - | ✓ | ✓ | - | ✓ |

<!-- Hiding CC Libraries (considered beta) as per PM feedback.
| CC Libraries  | &#10003; | &minus;  | &#10003; | &#10003; | &#10003; | &#10003; | &minus;    | &minus;         |
-->

## Búsqueda, utilización y edición de recursos {#support-to-search-use-edit}

| Tipo de recurso | [Descargar](/help/manage-organize.md#download) | Arrastrar y colocar | [Editor de imágenes](/help/edit-images.md) | [Buscar](/help/search.md) | [Etiquetas inteligentes](/help/metadata.md#tags) | [Cambiar nombre](/help/manage-organize.md) | [Versiones](/help/manage-organize.md#versions-of-assets) |
|---------------|----------|---------------|--------------|----------|------------|----------|----------|
| Rasterización de imágenes | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Archivos RAW | ✓ | ✓ | - | ✓ | ✓ | ✓ | ✓ | ✓ |
| Carpetas | ✓ | ✓ | - | ✓ | - | ✓ | ✓ |
| Vídeos | ✓ | ✓ | - | ✓ | ✓ | ✓ | ✓ |
| Bibliotecas CC | - | - | - | - | - | ✓ | ✓ |
| PDF | ✓ | ✓ | - | ✓ | ✓ | ✓ | ✓ |
| PSD, IA e INDD | ✓ | ✓ | - | ✓ | ✓ | ✓ | ✓ |
| Otros archivos binarios | ✓ | ✓ | - | ✓ | - | ✓ | ✓ |


## Revisión de recursos y colaboración {#support-to-review-collaborate}

| Tipo de recurso | Anotar | Comentar | Crear tareas y revisar |
|---------------|----------|----------|-------------------------|
| Rasterización de imágenes | ✓ | ✓ | ✓ |
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
| Rasterización de imágenes | ✓ | ✓ | ✓ | ✓ | ✓ |
| Archivos RAW | ✓ | ✓ | ✓ | ✓ | ✓ |
| Carpetas | ✓ | - | ✓ | ✓ | ✓ |
| Vídeos | ✓ | - | ✓ | ✓ | ✓ |
| Bibliotecas CC | ✓ | - | - | - | - |
| PDF | ✓ | - | ✓ | ✓ | ✓ |
| PSD, IA e INDD | ✓ | - | ✓ | ✓ | ✓ |
| Otros archivos binarios | ✓ | - | ✓ | ✓ | ✓ |

Los usuarios de [!DNL Adobe Asset Link] pueden cargar y registrar archivos (cargar una nueva versión) en el repositorio de [!DNL Assets Essentials] desde las aplicaciones de escritorio de [!DNL Adobe Creative Cloud] admitidas.

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

## Siguientes pasos {#next-steps}

* Proporcione comentarios de producto mediante [!UICONTROL Comentarios] opción disponible en la interfaz de usuario de Assets Essentials

* Proporcione comentarios sobre la documentación usando [!UICONTROL Editar esta página] ![editar la página](assets/do-not-localize/edit-page.png) o [!UICONTROL Registrar un problema] ![crear un problema de GitHub](assets/do-not-localize/github-issue.png) disponible en la barra lateral derecha

* Contacto [Servicio de atención al cliente](https://experienceleague.adobe.com/?support-solution=General#support)
