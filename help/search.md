---
title: Buscar y descubrir recursos en [!DNL Assets Essentials]
description: Buscar y descubrir recursos en [!DNL Assets Essentials].
role: User
source-git-commit: 5bae37e18ac587aaacaa004e5ec02775888d7f9a
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 1%

---


# Buscar recursos en [!DNL Assets Essentials] {#search-assets}

[!DNL Assets Essentials] proporciona una búsqueda efectiva, que solo funciona de forma predeterminada. La búsqueda es completa, ya que es de texto completo. La potente funcionalidad de búsqueda le permite descubrir rápidamente el recurso adecuado y ayudarle a mejorar la velocidad de contenido. [!DNL Assets Essentials] proporciona búsquedas de texto completo e incluso búsquedas mediante metadatos como etiquetas inteligentes, título, fecha de creación y copyright.

Para buscar recursos,

* Haga clic en en el cuadro de búsqueda que hay en la parte superior de la página. De forma predeterminada, busca dentro de la carpeta que está explorando actualmente. Realice una de las acciones siguientes:

   ![cuadro de búsqueda](assets/search-box.png)

   * Busque con una palabra clave y, opcionalmente, cambie la carpeta . Pulse Retorno.

   * Empiece a trabajar con un recurso visualizado recientemente, buscándolo directamente. Haga clic en el cuadro de búsqueda y seleccione un recurso visualizado recientemente de las sugerencias.

## Filtrar los resultados de la búsqueda {#refine-search-results}

Puede filtrar los resultados de la búsqueda según los parámetros siguientes.

![Filtros de búsqueda](assets/filters1.png)

*Figura: Filtre los recursos buscados según varios parámetros.*

* Tipo de archivo: Filtre los resultados de la búsqueda por los tipos de archivos admitidos, `Images`, `Documents` y `Videos`.
* Tipo MIME: Filtre por uno o varios formatos de archivo compatibles. <!-- TBD:  [supported file formats](/help/supported-file-formats.md). -->
* Tamaño de la imagen: Proporcione una de las dimensiones mínimas y máximas para filtrar imágenes. El tamaño se proporciona en dimensiones en píxeles y no es el tamaño de archivo de las imágenes.
* Crear fecha: La fecha de creación del recurso tal como se indica en los metadatos. El formato de fecha estándar utilizado es `yyyy-mm-dd`.
* Fecha de modificación: Fecha de la última modificación de los recursos. El formato de fecha estándar utilizado es `yyyy-mm-dd`.

Puede ordenar los recursos buscados en orden creciente o descendente de `Name`, `Relevancy`, `Size`, `Modified` y `Created`.

## Búsquedas guardadas {#saved-search}

La funcionalidad de búsqueda es bastante fácil de usar en [!DNL Assets Essentials]. Desde el cuadro de búsqueda, no solo puede escribir una palabra clave y pulsar la tecla Retorno para ver los resultados, sino que también puede buscar rápidamente de nuevo las palabras clave buscadas recientemente en un solo clic.

También puede filtrar los resultados de búsqueda según criterios específicos en torno a metadatos y tipo de recursos. Para los filtros más utilizados, para mejorar la experiencia de búsqueda, [!DNL Assets Essentials] permite guardar los parámetros de búsqueda. A continuación, puede seleccionar la búsqueda guardada para buscar y aplicar el filtro con un solo clic.

Para crear una búsqueda guardada, busque algún recurso, aplique uno o más filtros y haga clic en [!UICONTROL Save Search] en el panel [!UICONTROL Filters].

![Búsqueda guardada del panel Filtros](assets/saved-search.png)

<!-- TBD: Search behavior. Full-text search. Ranking and rank boosts. Hidden assets.
Report poor UX that users can only save a filtered search and not a simple search.
.
Are other supported files fully indexed and support full-text search? Eg. audio/videos files can at best have metadata indexed.
Anything about ranking of assets displayed in search results?

What about temporarily hiding an asset (suspending search on it) from the search results? If an asset is undergoing review collaboration, should it be used by others? Should it be hidden in search?

When userA is searching and userB add an asset that matches search results, will the asset display in search as soon as userA refreshes the page? Assuming indexing is near real-time. May not be so for bulk uploads.
-->
