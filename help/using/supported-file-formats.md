---
title: Formatos de archivo compatibles
description: Formatos de archivo compatibles con los distintos casos de uso de [!DNL Assets Essentials]
role: User,Leader,Admin,Architect,Developer
contentOwner: AG
exl-id: bc44e98d-446e-41ff-b5b4-9dc324834630
source-git-commit: 243a41aef81cd1fdcbad8f4355fe2d888db394d1
workflow-type: ht
source-wordcount: '527'
ht-degree: 100%

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

| Tipo de recurso | [Examinar](/help/using/navigate-view.md) | Copiar | [Cargar](/help/using/add-delete.md) | Crear | [Eliminar](/help/using/add-delete.md#delete-assets) | Detalles | Zoom de imagen | [Vistos recientemente](/help/using/navigate-view.md) |
|-------------------|----------|----------|----------|----------|----------|-------------------|------------|-----------------|
| Rasterización de imágenes | ✓ | ✓ | ✓ | − | ✓ | ✓ | ✓ | ✓ |
| Archivos RAW | ✓ | ✓ | ✓ | − | ✓ | ✓ | ✓ | ✓ |
| Carpetas | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | − | − |
| Vídeos MP4 | ✓ | ✓ | ✓ | − | ✓ | ✓ ‡ | − | ✓ |
| PDF | ✓ | ✓ | ✓ | − | ✓ | ✓ | − | ✓ |
| PSD, IA, PSB e INDD | ✓ | ✓ | ✓ | − | ✓ | ✓ ‡ | − | ✓ |
| Otros archivos binarios | ✓ | ✓ | ✓ | − | ✓ | ✓ | − | ✓ |

<!-- Hiding CC Libraries (considered beta) as per PM feedback.
| CC Libraries  | &#10003; | &minus;  | &#10003; | &#10003; | &#10003; | &#10003; | &minus;    | &minus;         |
-->

## Búsqueda, utilización y edición de recursos {#support-to-search-use-edit}

| Tipo de recurso | [Descargar](/help/using/manage-organize.md#download) | Arrastrar y colocar | [Editor de imágenes](/help/using/edit-images.md) | [Buscar](/help/using/search.md) | [Etiquetas inteligentes](/help/using/metadata.md#tags) | [Cambiar nombre](/help/using/manage-organize.md) | [Versiones](/help/using/manage-organize.md#versions-of-assets) |
|---------------|----------|---------------|--------------|----------|------------|----------|----------|
| Rasterización de imágenes | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |
| Archivos RAW | ✓ | ✓ | − | ✓ | ✓ | ✓ | ✓ | ✓ |
| Carpetas | ✓ | ✓ | − | ✓ | − | ✓ | ✓ |
| Vídeos | ✓ | ✓ | − | ✓ | ✓ | ✓ | ✓ |
| Bibliotecas CC | − | − | − | − | − | ✓ | ✓ |
| PDF | ✓ | ✓ | − | ✓ | ✓ | ✓ | ✓ |
| PSD y PSB | ✓ | ✓ | − | ✓ | ✓ | ✓ | ✓ |
| IA e INDD | ✓ | ✓ | − | ✓ | − | ✓ | ✓ |
| Otros archivos binarios | ✓ | ✓ | − | ✓ | − | ✓ | ✓ |


## Revisión de recursos y colaboración {#support-to-review-collaborate}

| Tipo de recurso | Anotar | Comentar | Crear tareas y revisar |
|---------------|----------|----------|-------------------------|
| Rasterización de imágenes | ✓ | ✓ | ✓ |
| Archivos RAW | ✓ | ✓ | ✓ |
| Carpetas | − | − | − |
| Vídeos | − | ✓ | ✓ |
| Bibliotecas CC | − | − | − |
| PDF | − | ✓ | ✓ |
| PSD, PSB, IA e INDD | − | ✓ | ✓ |
| Otros archivos binarios | − | ✓ | ✓ |
| DOC | − | ✓ | ✓ |
| DOCX | − | ✓ | ✓ |
| PPT | − | ✓ | ✓ |
| PPTX | − | ✓ | ✓ |
| XLS | − | ✓ | ✓ |
| XLSX | − | ✓ | ✓ |
| TXT | − | ✓ | ✓ |
| RTF | − | ✓ | ✓ |

## Otras tareas de administración de recursos {#support-to-manage-assets}

| Tipo de recurso | [Metadatos](/help/using/metadata.md) | [Representaciones](/help/using/add-delete.md#renditions) | [Papelera](/help/using/add-delete.md#delete-assets) | Copiar | Mover |
|---------------|-------------------|------------|----------|----------|----------|
| Rasterización de imágenes | ✓ | ✓ | ✓ | ✓ | ✓ |
| Archivos RAW | ✓ | ✓ | ✓ | ✓ | ✓ |
| Carpetas | ✓ | − | ✓ | ✓ | ✓ |
| Vídeos | ✓ | − | ✓ | ✓ | ✓ |
| Bibliotecas CC | ✓ | − | − | − | − |
| PDF | ✓ | − | ✓ | ✓ | ✓ |
| IA e INDD | ✓ | − | ✓ | ✓ | ✓ |
| PSD y PSB | ✓ | ✓ | ✓ | ✓ | ✓ |
| Otros archivos binarios | ✓ | − | ✓ | ✓ | ✓ |

Los usuarios de [!DNL Adobe Asset Link] pueden cargar y registrar archivos (cargar una nueva versión) en el repositorio de [!DNL Assets Essentials] desde las aplicaciones de escritorio de [!DNL Adobe Creative Cloud] admitidas.

<!-- TBD: Saving the template table separately for later use.
| Asset type    | Features |
|---------------|----------|
| Raster images |          |
| Folders       |          |
| Videos        |          |
| CC Libraries  |          |
| PDF files     |          |
| PSD, PSB           |          |
| AI            |          |
| INDD          |          |

>[!MORELIKETHIS]
>
>* []()
-->

## Siguientes pasos {#next-steps}

* Proporcione comentarios de producto mediante la opción [!UICONTROL Comentarios] disponible en la interfaz de usuario de Assets Essentials

* Proporcione comentarios sobre la documentación usando [!UICONTROL Editar esta página] ![editar la página](assets/do-not-localize/edit-page.png) o [!UICONTROL Registrar una incidencia] ![crear una incidencia de GitHub](assets/do-not-localize/github-issue.png), disponibles en la barra lateral derecha

* Contacto con el [Servicio de atención al cliente](https://experienceleague.adobe.com/es?support-solution=General#support)
