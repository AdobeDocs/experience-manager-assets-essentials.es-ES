---
title: Formatos de archivo compatibles
description: Formatos de archivo compatibles con los distintos casos de uso de [!DNL Assets Essentials]
role: User,Leader,Admin,Architect,Developer
contentOwner: AG
source-git-commit: e791ef4ffdfdad907b5e868b3f3eab0c597ae4cd
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 26%

---


# Compatibilidad con formatos de archivo en [!DNL Assets Essentials] {#file-format-support}

[!DNL Assets Essentials] admite una amplia gama de formatos de archivo y cada funcionalidad tiene compatibilidad variada con distintos tipos de archivo.

* ![tipo de archivo de imagen ](assets/do-not-localize/image-icon.png) iconImágenes: GIF, JPG, PNG y TIFF
* ![tipo de archivo de documento ](assets/do-not-localize/document-icon.png) iconoDocumentos: DOCX, PDF, PPTX y XLSX
* ![tipo de archivo de vídeo ](assets/do-not-localize/video-icon.png) iconVídeos: MP4

Los distintos tipos de archivo tienen diferentes grados de compatibilidad con los casos de uso y las funciones, como se describe a continuación. Utilice la leyenda para comprender el nivel de asistencia.

| Nivel de asistencia | Descripción |
|---------------|-------------------------|
| ✓ | Compatible |
| * | Compatible condicionalmente |
| - | No aplicable |

* Otras tareas de administración de recursos:

## Agregar, cargar y ver recursos {#support-to-upload-view}

<!-- TBD: For AEM, AI files require the PDF option to be selected when saving the AI file.
-->

| Tipo de recurso | Examinar | Copiar | Cargar | Crear | Eliminar | Detalles | Zoom de imagen | Vistos recientemente |
|---------------|----------|----------|----------|----------|----------|----------|------------|-----------------|
| Imágenes rasterizadas | ✓ | ✓ | ✓ | - | ✓ | ✓ | ✓ | ✓ |
| Carpetas | ✓ | ✓ | ✓ | ✓ | ✓ | ✓ | - | - |
| Vídeos | ✓ | ✓ | ✓ | - | ✓ | * | - | ✓ |
| Bibliotecas CC | ✓ | - | ✓ | ✓ | ✓ | ✓ | - | - |
| PDF | ✓ | ✓ | ✓ | - | ✓ | ✓ | - | ✓ |
| PSD | ✓ | ✓ | ✓ | - | ✓ | * | - | ✓ |
| AI | ✓ | ✓ | ✓ | - | ✓ | * | - | ✓ |
| INDD | ✓ | ✓ | ✓ | - | ✓ | * | - | ✓ |

## Buscar, utilizar y editar recursos {#support-to-search-use-edit}

| Tipo de recurso | Descargar | Arrastrar y colocar | Editor de imágenes | Búsqueda   | Etiquetas inteligentes | Cambiar nombre | Versiones |
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

| Tipo de recurso | Metadatos | Representaciones | Papelera | Copiar | Mover | [!DNL Adobe Asset Link] check-in |
|---------------|----------|------------|----------|----------|----------|----------------------------------|
| Imágenes rasterizadas | * | ✓ | ✓ | ✓ | ✓ | ✓ |
| Carpetas | * | - | ✓ | ✓ | ✓ | - |
| Vídeos | * | - | ✓ | ✓ | ✓ | - |
| Bibliotecas CC | * | - | - | - | - | - |
| PDF | * | - | ✓ | ✓ | ✓ | - |
| PSD | * | - | ✓ | ✓ | ✓ | - |
| AI | * | - | ✓ | ✓ | ✓ | - |
| INDD | * | - | ✓ | ✓ | ✓ | - |

<!-- TBD: Saving template table separately.
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
