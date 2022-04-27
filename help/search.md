---
title: Búsqueda y descubrimiento de recursos en [!DNL Assets Essentials]
description: Busque y descubra recursos en [!DNL Assets Essentials].
role: User
exl-id: be9597a3-056c-436c-a09e-15a03567c85a
source-git-commit: cd7af0c946a042430e62528fa6aa19bdab139f67
workflow-type: ht
source-wordcount: '389'
ht-degree: 100%

---

# Búsqueda de recursos en [!DNL Assets Essentials] {#search-assets}

[!DNL Assets Essentials] proporciona una búsqueda efectiva que funciona de forma predeterminada. La búsqueda es exhaustiva, ya que es de texto completo. La potente funcionalidad de búsqueda le permite descubrir rápidamente el recurso adecuado y ayudarle a mejorar la velocidad del contenido. [!DNL Assets Essentials] proporciona búsquedas de texto completo e incluso búsquedas mediante metadatos como etiquetas inteligentes, título, fecha de creación y copyright.

Para buscar recursos, haga lo siguiente:

* Haga clic en el cuadro de búsqueda que hay en la parte superior de la página. De forma predeterminada, busca dentro de la carpeta que está explorando actualmente. Realice una de las acciones siguientes:

   ![cuadro de búsqueda](assets/search-box.png)

   * Busque con una palabra clave y, si quiere, cambie la carpeta. Pulse Intro.

   * Empiece a trabajar con un recurso visualizado hace poco directamente buscándolo. Haga clic en el cuadro de búsqueda y seleccione un recurso visualizado recientemente en las sugerencias.

## Filtrado de los resultados de búsqueda {#refine-search-results}

Puede filtrar los resultados de búsqueda según los parámetros siguientes.

![Filtros de búsqueda](assets/filters1.png)

*Imagen: filtre los recursos buscados según varios parámetros.*

* Tipo de archivo: filtre los resultados de búsqueda según los tipos de archivos admitidos, es decir, `Images`, `Documents` y `Videos`.
* Tipo de MIME: filtre uno o varios formatos de archivo compatibles. <!-- TBD:  [supported file formats](/help/supported-file-formats.md). -->
* Tamaño de imagen: proporcione una o más de las dimensiones mínimas y máximas para filtrar imágenes. El tamaño se proporciona en dimensiones en píxeles y no es el tamaño de archivo de las imágenes.
* Fecha de creación: la fecha de creación del recurso tal como se indica en los metadatos. El formato de fecha estándar utilizado es `yyyy-mm-dd`.
* Fecha de modificación: fecha de la última modificación de los recursos. El formato de fecha estándar utilizado es `yyyy-mm-dd`.

Puede ordenar los recursos buscados en orden creciente o descendente de `Name`, `Relevancy`, `Size`, `Modified` y `Created`.

## Búsquedas guardadas {#saved-search}

La funcionalidad de búsqueda es bastante fácil de usar en [!DNL Assets Essentials]. Desde el cuadro de búsqueda, no solo puede escribir una palabra clave y pulsar la tecla Intro para ver los resultados, sino que también puede buscar rápidamente de nuevo las palabras clave consultadas recientemente con un solo clic.

También puede filtrar los resultados de búsqueda según criterios específicos en torno a los metadatos y el tipo de recursos. Para los filtros utilizados con frecuencia, a fin de mejorar la experiencia de búsqueda, [!DNL Assets Essentials] permite guardar los parámetros de búsqueda. A continuación, puede seleccionar la búsqueda guardada para buscar y aplicar el filtro con un solo clic.

Para crear una búsqueda guardada, busque algún recurso, aplique uno o varios filtros y haga clic en [!UICONTROL Guardar búsqueda] en el panel [!UICONTROL Filtros].

![Búsqueda guardada del panel Filtros](assets/saved-search.png)

<!-- TBD: Search behavior. Full-text search. Ranking and rank boosts. Hidden assets.
Report poor UX that users can only save a filtered search and not a simple search.
.
Are other supported files fully indexed and support full-text search? Eg. audio/videos files can at best have metadata indexed.
Anything about ranking of assets displayed in search results?

What about temporarily hiding an asset (suspending search on it) from the search results? If an asset is undergoing review collaboration, should it be used by others? Should it be hidden in search?

When userA is searching and userB add an asset that matches search results, will the asset display in search as soon as userA refreshes the page? Assuming indexing is near real-time. May not be so for bulk uploads.
-->
