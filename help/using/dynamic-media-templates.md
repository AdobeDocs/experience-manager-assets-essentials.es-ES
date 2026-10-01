---
title: ¿Cómo administrar las plantillas de Dynamic Media?
description: Aprenda a crear plantillas de Dynamic Media con un editor de plantillas de WYSIWYG e incluya varias capas de imágenes y texto para crear rápidamente banners y folletos, y utilizarlos en aplicaciones descendentes.
hide: true
hidefromtoc: true
role: User
exl-id: 07de648e-4ae2-4524-8e05-3cf10bb6006d
source-git-commit: 10c0e2375ba16dfeeeeca8f0b816ca366254dd67
workflow-type: tm+mt
source-wordcount: '3017'
ht-degree: 99%
---
# Plantillas de Dynamic Media{#dynamic-media-templates}

| [Prácticas recomendadas de búsqueda](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/best-practices/search-best-practices) | [Prácticas recomendadas de metadatos](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/best-practices/metadata-best-practices) | [Centro de contenido](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/content-hub/product-overview) | [Documentación de desarrollador de AEM Assets](https://developer.adobe.com/experience-cloud/experience-manager-apis/) |
| ------------- | --------------------------- |---------|-----|

>[!CONTEXTUALHELP]
>id="assets_dm_templates"
>title="Administración de plantillas de Dynamic Media"
>abstract="Cree y personalice banners de imagen y texto sobre la marcha, con una interfaz de WYSIWYG fácil de usar, e incruste la URL de Dynamic Media en cualquier aplicación propia o de terceros para lograr experiencias muy atractivas. ¡Pruébelo!"
>additional-url="https://images-tv.adobe.com/mpcv3/4477/b74738ca-888c-4a37-9a9e-14fabd68ee45_1738206841.854x480at800_h264.mp4" text="Ver vídeo"

Cree plantillas de Dynamic Media con un editor de plantillas de WYSIWYG e incluya varias capas de imágenes y texto para crear rápidamente banners y folletos, y utilizarlos en aplicaciones descendentes. También puede añadir parámetros a las capas de imágenes y texto incluidos en la plantilla y utilice [URL de Dynamic Media](https://experienceleague.adobe.com/es/docs/commerce-admin/content-design/wysiwyg/storage/catalog-urls-dynamic-media) para actualizar los valores de esas capas en tiempo real.

Algunas de las funciones clave son las siguientes:

* **Editor de plantillas de Dynamic Media WYSIWYG:** cree banners personalizables con capas de texto e imagen.
* **Parametrización de capas:** defina pares dinámicos de clave-valor para las capas con el fin de habilitar las actualizaciones en tiempo real.
* **Compatibilidad con URL de Dynamic Media:** utilice las URL de Dynamic Media para plantillas, integrando valores personalizados de aplicaciones de origen o de terceros.
* **Control de visibilidad de la capa:** oculte o muestre de forma dinámica las capas según sea necesario.
* **Cambio de tamaño del texto inteligente:** ajuste automáticamente el tamaño del texto para ajustar las áreas designadas.

Algunas de las ventajas clave de las plantillas de Dynamic Media son:

* **Optimizar Personalization 1:1:** Adapte el contenido a las señales de clientes en tiempo real.
* **Reducción del esfuerzo manual:** automatice y acelere la creación y administración de contenido.
* **Garantía de experiencias omnicanal coherentes:** mantenga la coherencia de la marca en todos los canales.
* **Reutilización del contenido de forma eficaz:** evite el contenido de un solo uso y escale con plantillas dinámicas parametrizadas.
* **Mitigación de riesgos:** actualice precios, descuentos y vínculos en tiempo real.
* **Mejora de la participación del cliente:** impulse experiencias interactivas y relevantes para el contexto.

>[!NOTE]
>
>Los clientes con suscripciones al SKU de seguridad mejorada no pueden utilizar ninguna funcionalidad de Dynamic Media, incluidas las plantillas de Dynamic Media, en ese programa de Cloud Services.

## Antes de empezar{#prerequisites-for-dynamic-media-wysiwyg-template}

Para crear una plantilla de Dynamic Media, debe tener lo siguiente:

1. Acceso a Dynamic Media.
1. [Sincronización de las imágenes disponibles en su instancia de AEM Assets con Dynamic Media para usarlas para crear la plantilla](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/dynamicmedia/config-dm).
1. Se ha verificado lo siguiente en la IU táctil:
   * En la **[!UICONTROL página Editar configuración de Dynamic Media]**, el **[!UICONTROL modo de sincronización de Dynamic Media]** establecido en **[!UICONTROL Deshabilitado de forma predeterminada]** no se aplica a todas las carpetas de AEM (**[!UICONTROL Sincronizar todo el contenido]** no está marcado). Consulte [Configuración del servicio de nube de Dynamic Media](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/dynamicmedia/config-dm) para obtener más información.
   * **[!UICONTROL El modo de sincronización de Dynamic Media]** está establecido en **[!UICONTROL Habilitar para subcarpetas]** para la carpeta o subcarpeta de destino en la que guardará la plantilla después de crearla. Consulte [Configuración del servicio de nube de Dynamic Media](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/dynamicmedia/config-dm) para obtener más información.

## Crear una plantilla WYSIWYG de Dynamic Media{#how-to-create-dynamic-media-wysiwyg-template}

Para crear una plantilla de DM, siga estos pasos:

1. [Crear un lienzo en blanco](#create-a-canvas)
1. [Añadir imágenes al lienzo](#add-images-to-the-canvas)
1. [Añadir capas de texto al lienzo](#add-text-to-the-canvas)
1. [Editar o eliminar una capa](#edit-or-delete-a-layer)
1. [Parametrizar capas](#parameterise-a-layer)

### Crear un lienzo en blanco{#create-a-canvas}

Ejecute estos pasos para crear un lienzo en blanco:

1. Vaya a Assets Essentials y haga clic en **[!UICONTROL Recursos de Dynamic Media]** disponible en el panel izquierdo.

   ![Plantillas de Dynamic Media](/help/using/assets/DM-Assets1.png)

1. Haga clic en **[!UICONTROL Crear plantilla]** para guardar la plantilla en Recursos de Dynamic Media o vaya hasta una carpeta y haga clic en **[!UICONTROL Crear plantilla]** para guardar la plantilla en esa carpeta. Se muestra el cuadro de diálogo **[!UICONTROL Nueva plantilla]**.
   ![cómo crear plantillas dinámicas que se pueden personalizar en tiempo real](/help/using/assets/new-template.png)
   Para [crear una carpeta](/help/using/add-delete.md) en **[!UICONTROL Recursos de Dynamic Media]**, cree una carpeta en **[!UICONTROL Recursos]**. El árbol de carpetas de **[!UICONTROL Recursos]** se replica en **[!UICONTROL Recursos de Dynamic Media]**.
1. Especifique un nombre de plantilla, defina la anchura y altura del lienzo y haga clic en **[!UICONTROL Crear]**. Se muestra un lienzo en blanco con opciones de menú en ambos lados que se utilizan para crear la plantilla. Pase el puntero del ratón por encima de las opciones del menú para ver su ayuda contextual.
   ![plantilla personalizable en tiempo real](/help/using/assets/blank-canvas-page.png)

>[!NOTE]
>
> El intervalo de anchura y altura permitido es de 50 a 5000.

**Opciones de menú en el panel derecho:** utilice estas opciones para añadir las capas de imágenes y texto necesarias al lienzo.

* ![Plantillas de DM](/help/using/assets/add-image.svg): haga clic para añadir imágenes al lienzo.
* ![plantillas personalizables](/help/using/assets/add-text.svg): haga clic para añadir textos al lienzo.
* ![plantillas personalizables](/help/using/assets/show-layers-list.svg): haga clic para ver la lista de todas las capas (imagen y texto) del lienzo. Cada imagen y texto añadido al lienzo se representa como una capa independiente.

**Opciones de menú en el panel izquierdo:** utilice estas opciones para acciones comunes del editor tal como se menciona a continuación.

* ![Plantillas de DM](/help/using/assets/layer-selector.svg): seleccione una capa.
* ![crear una plantilla que se puede personalizar al instante](/help/using/assets/undo.svg): haga clic para deshacer la última acción o pulse **Ctrl** + **Z** (Windows) o **Cmd** + **Z** (Mac).
* ![plantilla para crear banners rápidamente](/help/using/assets/redo.svg): haga clic para rehacer la última acción o pulse **Ctrl** + **Y** (Windows) o **Cmd** + **Y** (Mac).
* ![plantilla para crear folletos rápidamente](/help/using/assets/zoomin.svg): haga clic para ampliar el lienzo o pulse **Ctrl** + **+** (Windows) o Cmd + **+** (Mac).
* ![plantilla para crear banners rápidamente](/help/using/assets/ZoomOut-1.svg): haga clic para reducir el lienzo o pulse **Ctrl** + **-** (Windows) o **Cmd** + **-** (Mac).
* Pulse **Retroceso** o **eliminar** para eliminar la capa seleccionada si no se está editando ningún texto o propiedad.

Haga clic en ![plantilla para crear folletos rápidamente](/help/using/assets/show-layers-list.svg) **>** más opciones (![](/help/using/assets/three-dots.svg)) en la capa Lienzo para editar las dimensiones del lienzo en cualquier momento mientras crea la plantilla.
![](/help/using/assets/edit-canvas1.png)

>[!NOTE]
>
> Las plantillas permiten un máximo de 20 capas, incluido el lienzo.

### Añadir imágenes al lienzo{#add-images-to-the-canvas}

Ejecute estos pasos para añadir imágenes al lienzo:

1. Haga clic en ![crear un banner al instante](/help/using/assets/add-image.svg) para mostrar el panel [Selector de recursos](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/asset-selector/overview-asset-selector). El panel muestra las imágenes de la instancia de AEM Assets que están sincronizadas con Dynamic Media.
1. Examine el panel o utilice palabras clave en la barra de búsqueda para encontrar una imagen específica.
1. Arrastre y suelte una imagen en el lienzo para utilizarla. Consulte el [**[!UICONTROL Panel de propiedades]**](#reposition-resize-delete-a-layer) para cambiar el tamaño o la posición de una capa en el lienzo.
   ![crear un banner en segundos](/help/using/assets/add-image-to-canvas.png)

### Añadir capas de texto al lienzo{#add-text-to-the-canvas}

Ejecute estos pasos para añadir capas de texto al lienzo:

1. Haga clic en ![creación de nuevos banners rápidamente](/help/using/assets/add-text.svg) para añadir una capa de texto al lienzo y abrir el panel Propiedades.
1. Seleccione la capa y haga clic en el texto para actualizarla.
1. Habilite **[!UICONTROL Redimensionado de texto inteligente]** en el panel Propiedades para ajustar automáticamente la longitud del texto y el tamaño de fuente para que se ajusten de manera óptima al área designada.
   ![mejores banners personalizables](/help/using/assets/add-text-layer.png)

Consulte el [**[!UICONTROL Panel de propiedades]**](#reposition-resize-delete-a-layer) para cambiar la posición, el tamaño, la rotación o la eliminación de la capa. Dé formato al texto según la fuente, el tamaño, el color, el estilo y la alineación deseados (en la capa) cambiando sus valores en los campos respectivos de la sección **[!UICONTROL Texto]** del panel.

>[!NOTE]
>
> Para utilizar una fuente distinta a la familia de fuentes predeterminada Adobe Sans F2, debe cargar y publicar el archivo de fuentes en AEM Assets y Dynamic Media. Si tiene fuentes antiguas en su instancia, asegúrese de [volver a procesar](/help/using/reprocessing.md) para verlas en el editor de plantillas.

### Editar o eliminar una capa {#edit-or-delete-a-layer}

Ejecute estos pasos para editar o eliminar una capa del lienzo:

1. Haga clic en ![plantillas con compatibilidad con las actualizaciones dinámicas](/help/using/assets/show-layers-list.svg) y seleccione la capa en el lienzo o en la lista Capas.
1. Haga clic en **más opciones** (![plantillas con compatibilidad con las actualizaciones en tiempo real](/help/using/assets/three-dots.svg)) para editar o eliminar la capa.
1. Haga clic en **[!UICONTROL Eliminar]** para eliminar la capa.
1. Haga clic en **[!UICONTROL Editar]** para editar la capa mediante el [**[!UICONTROL Panel de propiedades]**](#reposition-resize-delete-a-layer).
   ![creación rápida de banners](/help/using/assets/edit-delete-layer.png)

### Panel Propiedades{#properties-panel}

Para desplazarse al panel de propiedades de una capa:

1. Haga clic en ![creación rápida de contenido](/help/using/assets/show-layers-list.svg).
1. Seleccione la capa en la lista.

Este panel muestra la posición del punto central de la capa en el plano del lienzo (valores X e Y) y las dimensiones de la capa (anchura y altura) junto con las opciones de formato de texto.

![creación rápida de contenido](/help/using/assets/properties-panel.png)

En el panel de propiedades de una capa, seleccione otra capa del lienzo para ir hasta su panel de propiedades.


#### Cambiar la posición, el tamaño, la rotación o la eliminación de una capa{#reposition-resize-delete-a-layer}

Consulte estas acciones comunes de edición de capas para editar una capa de texto o de imagen:

* **Cambiar la posición de la capa:** arrastre la capa para moverla a cualquier lugar del lienzo. Esta acción actualiza los valores X e Y en el panel de propiedades.
* **Cambiar el tamaño de la capa:** seleccione la capa y arrastre sus controladores de bordes para cambiar su tamaño. Esta acción actualiza los valores W (anchura) y H (altura) en el panel de propiedades.
* **Rotar la capa:** arrastre el controlador cuadrado colocado verticalmente sobre la capa para girarlo alrededor de su centro. Esta acción actualiza los valores de ángulo en el panel de propiedades.
* **Eliminar la capa:** pulse **Retroceso** o **eliminar** y luego haga clic en **[!UICONTROL Confirmar]** para eliminar una capa seleccionada.

#### Opciones de formato de texto{#text-formatting-options-on-properties-panel}

Dé formato al texto según la fuente, el tamaño, el color, el estilo y la alineación deseados (en la capa) cambiando sus valores en los campos respectivos de la sección **[!UICONTROL Texto]** del panel.

**[!UICONTROL Redimensionado de texto inteligente]** Asegúrese de incluir **[!UICONTROL Redimensionado de texto inteligente]** ([Ajuste de texto](https://experienceleague.adobe.com/es/docs/dynamic-media-developer-resources/image-serving-api/image-serving-api/http-protocol-reference/text-formatting/r-copy-fitting)) para ajustar de forma óptima cualquier texto del área designada ajustando su tamaño y longitud de fuente de forma inteligente. Esta funcionalidad evita que el texto se desborde o minimiza los espacios adicionales en la parte inferior del texto.
![creación de contenido al instante](/help/using/assets/smart-text-resize.png)

### Parametrizar capas {#parameterise-a-layer}

Después de crear una plantilla con varias capas de imágenes y textos, parametrice las capas seleccionadas. Cuando se parametriza una capa o su propiedad, se le asigna un par clave-valor (también denominado parámetro). Este parámetro se puede incluir en la dirección URL de la plantilla para actualizar la posición, el tamaño o el contenido de la capa en tiempo real, lo que se traduce en la personalización de la plantilla al instante.

Para parametrizar una capa:

1. haga clic en ![creación instantánea de contenido](/help/using/assets/show-layers-list.svg), seleccione una capa y haga clic en **[!UICONTROL Parámetros]**. Se mostrará el panel **[!UICONTROL Parámetros]**
1. Active **[!UICONTROL Incluir parámetro]** para asignar parámetros a una propiedad. Consulte [esto](#parameterisation-options-or-allowed-parameters) para conocer el comportamiento de la propiedad después de la parametrización.
1. **Opcional:** cambie el nombre del parámetro. Un nombre de parámetro tiene un nombre de capa seguido de un sufijo. Para una capa seleccionada, todas sus propiedades parametrizadas comparten el mismo nombre de capa seguido de un sufijo variable. Cambie el nombre de la capa siguiendo la convención de nomenclatura semántica, de modo que cuando incluya el parámetro en la URL, el nombre del parámetro explique por sí mismo el contenido de la capa o su propósito.
1. Haga clic en **[!UICONTROL Guardar]**.
   ![creación instantánea de contenido](/help/using/assets/parameterise-a-layer.png)
   Para cambiar entre el panel Parámetro de una capa de imagen y de texto, seleccione la capa en el lienzo y haga clic en **[!UICONTROL Parámetros]**.

#### Opción del panel Parámetros {#parameterisation-options-or-allowed-parameters}

Las propiedades parametrizadas se pueden incluir como parámetros de URL en la URL de la plantilla para editar la plantilla en tiempo real mediante la URL.

**Parámetros de imagen:**

**X:** incluya este parámetro para mover la capa horizontalmente a lo largo de su línea central, paralela al eje X del plano de plantilla, cambiando el valor del parámetro en la dirección URL.
**Y:** incluya este parámetro para mover la capa verticalmente a lo largo de su línea central, paralela al eje Y del plano de la plantilla, cambiando el valor del parámetro en la dirección URL.
**Anchura:** incluya este parámetro para ajustar la anchura de la capa cambiando el valor del parámetro en la dirección URL.
**Altura:** incluya este parámetro para ajustar la altura de la capa cambiando el valor del parámetro en la dirección URL.
**Ocultar:** incluya este parámetro para ocultar o mostrar la capa en la plantilla usando 0 (mostrar) y 1 (ocultar).
**Origen:** incluya este parámetro para reemplazar la imagen de la capa por una nueva imagen cambiando la ruta de la imagen en el valor del parámetro en la dirección URL.

**Parámetros de formato de texto:**

Incluya los siguientes parámetros para editar el texto, su fuente, color y tamaño desde la URL al actualizar los valores de los parámetros en la URL.

**Texto:** incluya este parámetro para actualizar el texto de la dirección URL.
**Familia de fuentes:** incluya este parámetro para actualizar la fuente del texto desde la dirección URL.
**Tamaño de fuente:** incluya este parámetro para actualizar el tamaño de fuente del texto desde la dirección URL.
**Color del texto:** incluya este parámetro para actualizar el color de fuente del texto desde la dirección URL.

### Agrupar capas para controlar su visibilidad simultáneamente{#group-layers}

Otra forma de mantener las plantillas flexibles es utilizar un nombre de parámetro único para controlar varias capas. Esta estrategia es útil para el parámetro de visibilidad (ocultar o mostrar capas), para actualizar el diseño o los gráficos de una sola plantilla.

Siga estos pasos para asignar el mismo nombre a los parámetros de ocultación (![creación rápida de contenido](/help/using/assets/Visibility-icon.svg)) de varias capas, lo que le permite ocultarlos o mostrarlos simultáneamente.

1. Vaya al [**[!UICONTROL Panel de propiedades]**](#parameterise-a-layer) de una capa.
1. Active el parámetro **[!UICONTROL Ocultar]** si no está parametrizado anteriormente.
1. **Opcional:** cambie el nombre del parámetro Ocultar.
1. Copie el nombre del parámetro Ocultar.
1. Vaya al panel Parámetro de otras capas seleccionándolas en el lienzo y active su parámetro **[!UICONTROL Ocultar]** si no está parametrizado.
1. Reemplace su nombre de **[!UICONTROL parámetro Ocultar]** por el nombre copiado.
1. Haga clic en **[!UICONTROL Guardar]** para agrupar las capas.
1. Ejecute el paso 3 y luego el 4 en la sección [**[!UICONTROL Previsualizar y publicar]**](#preview-and-publish-template-and-copy-template-deliver-url) para ver los cambios.

## Vista previa y publicación de la plantilla para copiar la dirección URL de envío{#preview-and-publish-template-and-copy-template-deliver-url}

Siga estos pasos para previsualizar y publicar la plantilla y copiar la dirección URL de envío:

1. En la página de lienzo, haga clic en **[!UICONTROL Vista previa]**. También puede ir a **[!UICONTROL Assets Essentials]** **>** **[!UICONTROL Recursos de Dynamic Media]** **>**, buscar y seleccionar su plantilla **>**, hacer clic en **[!UICONTROL Editar plantilla]** **>** y hacer clic en **[!UICONTROL Vista previa]**. La página de vista previa muestra la plantilla, sus parámetros (capas y propiedades parametrizadas), el estado de publicación y la opción **[!UICONTROL Publicar]**.
1. Seleccione parámetros en el panel **[!UICONTROL Parámetros de plantilla]** para editar sus valores y actualizar instantáneamente el contenido, el tamaño, la posición o el formato de texto de la capa de plantilla correspondiente en la vista previa. Por ejemplo:
   1. Seleccione una capa de texto y edite su texto o
   1. Seleccione una capa de imagen, haga clic en ![creación de contenido sobre la marcha](/help/using/assets/add-image.svg), seleccione una imagen del selector de recursos y haga clic en **[!UICONTROL Actualizar]**.

   La plantilla se actualiza inmediatamente, mostrando el texto editado y reemplazando la imagen anterior por la nueva. Además, el valor del parámetro de imagen refleja la nueva ruta de la imagen. Asimismo, puede cambiar el tamaño de una capa ajustando sus valores, y los cambios se aplican a la plantilla en tiempo real.
1. Seleccione el parámetro ocultar de [capas agrupadas](#group-layers) en la lista para mostrarlas u ocultarlas juntas en la plantilla.
1. **Opcional:** cambie el valor del parámetro **[!UICONTROL Ocultar]** entre 0 y 1 y haga clic en **[!UICONTROL Actualizar]** para ver los cambios. Las capas con el mismo parámetro ocultar se ocultan o se muestran juntas. Asimismo, puede controlar la visibilidad de las capas desde la dirección URL.

   ![creación de contenido sobre la marcha](/help/using/assets/dm-templates-publish-status.png)
También puede activar **[!UICONTROL Incluir todos los parámetros]** para editar todos los valores de parámetros mostrados y ver las actualizaciones en la vista previa de la plantilla.
   <br>
1. Para publicar la plantilla en la página de vista previa, haga clic en **[!UICONTROL Publicar]** y confirme la publicación. Se muestra el mensaje Publicación completada y el estado de publicación se actualiza a Publicado.

>[!NOTE]
>
>La publicación de la plantilla requiere que las imágenes de la plantilla se publiquen primero.

### Copia de la URL de envío

Los parámetros seleccionados en la página **[!UICONTROL Vista previa]** se convierten en los parámetros de URL en la URL de la plantilla.

Para copiar la URL de la plantilla publicada que se muestra en la vista previa:

1. Haga clic en **[!UICONTROL Copiar URL]**. Se muestra el cuadro de diálogo **[!UICONTROL Copiar URL]**. Seleccione y copie la dirección URL mostrada. Observe que el primer parámetro de la dirección URL comienza después de un signo de interrogación **(?)** y un par clave-valor comienza con **$** y termina con **&amp;**. La clave y el valor están separados por un signo igual **(=)**, con la clave a la izquierda y el valor a la derecha.
1. Pegue esta dirección URL en la pestaña del explorador y vea la plantilla en directo. Personalice la plantilla en tiempo real actualizando el valor del parámetro requerido (valor de clave) en la dirección URL directamente, tal como se muestra en el [paso 2](#preview-and-publish-template-and-copy-template-deliver-url) de la sección **Previsualizar y publicar**.
1. Utilice esta URL para la comercialización rápida de sus productos o servicios. Puede compartir esta URL con sus clientes o integrarla en su sitio web o en cualquier aplicación de terceros descendente para mostrar el banner y realizar actualizaciones en tiempo real para reflejar las ofertas en curso.

Aprenda a crear una plantilla de Dynamic Media paso a paso en este vídeo.
>[!VIDEO](https://video.tv.adobe.com/v/3443281)

## Efectuar actualizaciones en tiempo real en la plantilla desde la URL{#update-the-template-from-the-url}

Editar parámetros directamente en la dirección URL puede ser una tarea tediosa. Para simplificar:

1. Copie la dirección URL y péguela en un bloc de notas.
1. Utilice Cmd+F (Mac) o Ctrl+F (Windows) para buscar y editar los valores de parámetro. Por ejemplo:
   * Reemplace las rutas de imagen de las capas de imagen.
   * Ajuste las dimensiones y posiciones de la capa (si está [parametrizada](#parameterise-a-layer)).
   * Edite el texto, la fuente, el color, el tamaño o la alineación de las capas de texto.
   * Cambie los valores de visibilidad entre 0 y 1.

Pegue esta URL actualizada en el explorador para ver los cambios.

## Edición de la plantilla{#edit-the-template}

Edite la plantilla siguiendo estos pasos:

1. En Assets Essentials, haga clic en **[!UICONTROL Recursos de Dynamic Media]**.
2. Navegue hasta la ubicación de la plantilla.
3. Seleccione la plantilla.
4. Haga clic en **[!UICONTROL Editar plantilla]**. El lienzo de la plantilla muestra la plantilla y la lista de todas sus capas en el panel Capas. Comience a editar la plantilla según sus necesidades.

## Puntos importantes a tener en cuenta {#important-points-to-note}

* Después de crear una plantilla con capas de imagen parametrizadas para actualizaciones dinámicas, asegúrese de que las imágenes destinadas a actualizaciones futuras compartan las mismas dimensiones que las imágenes parametrizadas. Esto garantiza que las imágenes se ajusten perfectamente dentro de las capas sin desbordarse ni dejar espacios vacíos. Actualmente, la plantilla no admite ajustes de dimensión automáticos para ajustar las imágenes a las capas.
* No se admiten subcadenas en una capa de texto. El usuario no puede aplicar propiedades de fuente diferentes en la subcadena de una capa de texto.
* Actualmente, la compatibilidad de varias empresas de Dynamic Media no está disponible con las plantillas de Dynamic Media.
* En caso de copia o movimiento, el selector de destino muestra todas las carpetas (incluidas las carpetas sincronizadas que no sean de Dynamic Media). Además, actualmente no muestra los recursos de plantilla de Dynamic Media (ambas son limitaciones del selector de destino).
* Cualquier operación de actualización en una carpeta (por ejemplo, Publicar o Eliminar) desde la sección de recursos afecta a las plantillas de Dynamic Media disponibles en esa carpeta.
* La papelera no funciona para las plantillas de Dynamic Media. Si un recurso se mueve a la papelera y, a continuación, se restaura, se restaura en AEM pero no en Dynamic Media. Lo mismo es válido para las plantillas de Dynamic Media.

## Ver también

1. Explorar [Dynamic Media y sus funcionalidades](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media)
1. Explorar [Dynamic Media con funcionalidades de OpenAPI](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/dynamic-media-open-apis-overview)
