---
title: Administración de metadatos
description: Administración de metadatos de recursos en [!DNL Assets Essentials]
role: User,Leader,Admin,Architect,Developer
contentOwner: AG
exl-id: cfc105d1-41fc-4418-9905-b2a28a348682
source-git-commit: 02f28c00b387fbcac4cd917fab7763124fdd5d70
workflow-type: ht
source-wordcount: '1026'
ht-degree: 100%

---

# Metadatos en [!DNL Assets Essentials] {#metadata}

Los metadatos son los datos o la descripción de los datos. Por ejemplo, las imágenes, como recurso, pueden contener información acerca de la cámara en la que se hizo clic o cualquier información de copyright. Esta información son los metadatos de la imagen. Los metadatos son esenciales para una administración eficiente de los recursos. Los metadatos son la recopilación de todos los datos disponibles para un recurso, pero es posible que no estén necesariamente contenidos en ese recurso.

Los metadatos le ayudan a categorizar los recursos y son útiles a medida que aumenta la cantidad de información digital. Es posible administrar algunos cientos de archivos basados únicamente en los nombres de archivo, miniaturas y memoria. Sin embargo, este enfoque no es escalable. Se queda corto cuando aumenta el número de personas involucradas y el número de recursos administrados.

Con la adición de metadatos, el valor de un recurso digital aumenta, ya que pasa a ser:

* Más accesible: los sistemas y los usuarios pueden encontrarlo fácilmente.
* Más fácil de administrar: puede encontrar recursos con el mismo conjunto de propiedades más fácilmente y aplicarles cambios.
* Completado: el recurso lleva más información y contexto con más metadatos.

Por estos motivos, Assets le proporciona los medios adecuados para crear, administrar e intercambiar metadatos para sus recursos digitales.

## Visualización de los metadatos {#view-metadata}

Para ver los metadatos de un recurso, navegue hasta él o búsquelo, selecciónelo y haga clic en **[!UICONTROL Detalles]** en la barra de herramientas.

![Visualización de los metadatos de un recurso](assets/metadata-view1.png)

*Imagen: para ver un recurso y sus metadatos, haga clic en **[!UICONTROL Detalles]** en la barra de herramientas o haga doble clic en él.*

Los metadatos básicos, como título, descripción y fecha de carga, están disponibles en la pestaña [!UICONTROL Básico]. La pestaña [!UICONTROL Avanzado] contiene metadatos más avanzados, como el modelo de cámara, los detalles de la lente y etiquetas geográficas. La pestaña [!UICONTROL Etiquetas] contiene etiquetas aplicadas automáticamente en función del contenido de la imagen.

## Actualización de metadatos {#update-metadata}

Puede actualizar algunos campos de metadatos manualmente. Los campos incluyen [!UICONTROL Título], [!UICONTROL Descripción], [!UICONTROL Autor] y [!UICONTROL Palabras clave].

## Etiquetas {#tags}

[!DNL Assets Essentials] utiliza inteligencia artificial proporcionada por [Adobe Sensei](https://www.adobe.com/es/sensei.html) para aplicar automáticamente las etiquetas relevantes a todos los recursos cargados. Estas etiquetas, que reciben el adecuado nombre de Etiquetas inteligentes, aumentan la velocidad del contenido de los proyectos al ayudarle a encontrar recursos relevantes con rapidez. Las etiquetas inteligentes son un ejemplo de metadatos que no están contenidos en la imagen.

Las etiquetas inteligentes se aplican en tiempo casi real y se generan en función del contenido de la imagen. Al cargar un recurso, la interfaz de usuario muestra [!UICONTROL Procesando] en la miniatura del recurso durante un tiempo. Una vez completado el procesamiento, puede [ver los metadatos](#view-metadata) y las etiquetas inteligentes.

![Visualización de las etiquetas inteligentes de un recurso](assets/metadata-view-tags.png)

*Imagen: para ver las etiquetas inteligentes de un recurso, haga clic en **[!UICONTROL Detalles]** en la barra de herramientas o haga doble clic en él.*

Las etiquetas inteligentes también contienen una puntuación de confianza en forma de porcentaje. Indica la confianza asociada a la etiqueta aplicada. Puede moderar las etiquetas inteligentes aplicadas automáticamente.

## Adición o actualización de etiquetas {#manually-tag}

Puede añadir más etiquetas a los recursos, además de las etiquetas inteligentes que se agregan automáticamente, usando el servicio inteligente [!DNL Adobe Sensei]. Abra un recurso para previsualizarlo, haga clic en [!UICONTROL Etiquetas] y escriba las palabras clave que desee en el campo [!UICONTROL Palabras clave]. Para añadir la etiqueta, pulse Intro. [!DNL Assets Essentials] indexa la palabra clave casi en tiempo real y su equipo puede buscar rápidamente los recursos actualizados con las nuevas palabras clave.

También puede quitar etiquetas de la sección [!UICONTROL Etiquetas inteligentes], que [!DNL Assets Essentials] añade automáticamente a todos los recursos cargados.

## Formularios de metadatos {#metadata-forms}

Assets Essentials proporciona muchos campos de metadatos estándar de forma predeterminada. Las organizaciones tienen requisitos de metadatos adicionales y necesitan más campos para agregar los específicos de su empresa. Los formularios de metadatos permiten a las empresas añadir campos de metadatos personalizados a la página [!UICONTROL Detalles] de un recurso. Los metadatos específicos de la empresa mejoran el control y el descubrimiento de sus recursos.

Puede configurar formularios de metadatos para diferentes tipos de recursos (diferentes tipos de MIME). Utilice el mismo nombre de formulario que el tipo MIME del archivo. Essentials hace coincidir automáticamente los recursos cargados con el nombre del formulario. Por ejemplo, si existe un formulario de metadatos con el nombre `PDF` o `pdf`, los documentos PDF cargados contienen campos de metadatos tal como se definen en el formulario. Puede crear formularios desde cero o reutilizar uno existente.

>[!IMPORTANT]
>
>El nuevo formulario de metadatos para un tipo de archivo específico reemplaza completamente el formulario de metadatos predeterminado que [!DNL Assets Essentials] proporciona. Si elimina o cambia el nombre de un formulario de metadatos, los campos de metadatos predeterminados volverán a estar disponibles para los nuevos recursos.

Para crear un formulario de metadatos, siga estos pasos:

1. En el carril izquierdo, haga clic en **[!UICONTROL Ajustes]** > **[!UICONTROL Formularios de metadatos]**.

   ![opción de formularios de metadatos en la barra lateral izquierda](assets/metadata-forms-sidebar.png)

1. Haga clic en **[!UICONTROL Crear]**, en el área superior derecha de la interfaz de usuario.
1. Proporcione un nombre al formulario y haga clic en **[!UICONTROL Crear]**.
1. Proporcione un nombre para la pestaña en **[!UICONTROL Ajustes]**, en el carril derecho.
1. De los **[!UICONTROL Componentes]** disponibles en el carril izquierdo, arrastre los necesarios a una pestaña del formulario. Arrastre los componentes en la secuencia deseada.

   ![opción de formularios de metadatos en la barra lateral izquierda](assets/metadata-form-new.png)

   *Imagen: interfaz de creación de formularios de metadatos con opciones para añadir componentes y para previsualizar el formulario.*

1. Para cada componente, proporcione un nombre en **[!UICONTROL Ajustes]**, en el carril derecho, y una asignación con las propiedades admitidas.
1. De forma opcional, para un componente, seleccione **[!UICONTROL Obligatorio]** para que el campo de metadatos sea obligatorio y **[!UICONTROL Solo lectura]** para que no se pueda editar en la página [!UICONTROL Detalles] del recurso.
1. Si lo desea, haga clic en **[!UICONTROL Previsualizar]** para previsualizar el formulario que está creando.
1. Opcionalmente, puede añadir más pestañas y los componentes necesarios en cada una.
1. Haga clic en **[!UICONTROL Guardar]** cuando haya completado el formulario.

Una vez creado un formulario, se aplica automáticamente cuando los usuarios cargan un recurso del tipo MIME correspondiente.

Para reutilizar un formulario existente y crear uno nuevo, seleccione un formulario de metadatos, haga clic en **[!UICONTROL Copiar]** en la barra de herramientas, proporcione un nombre y haga clic en **[!UICONTROL Confirmar]**. Puede editar un formulario de metadatos para cambiarlo. Al cambiar un formulario, se utiliza para los recursos cargados después del cambio. No cambia los recursos existentes.

## Siguientes pasos {#next-steps}

* [Vea un vídeo para administrar formularios de metadatos en Assets Essentials](https://experienceleague.adobe.com/docs/experience-manager-learn/assets-essentials/configuring/metadata-forms.html?lang=es)

* Proporcione comentarios de producto mediante la opción [!UICONTROL Comentarios] disponible en la interfaz de usuario de Assets Essentials

* Proporcione comentarios sobre la documentación usando [!UICONTROL Editar esta página] ![editar la página](assets/do-not-localize/edit-page.png) o [!UICONTROL Registrar una incidencia] ![crear una incidencia de GitHub](assets/do-not-localize/github-issue.png), disponibles en la barra lateral derecha.

* Contacto con el [Servicio de atención al cliente](https://experienceleague.adobe.com/?support-solution=General&amp;lang=es#support)

<!-- TBD: Cannot create a form using the second option. Documenting only the first option for now.
To reuse an existing form to create a new form, do one of these:

* Select a metadata form and click **[!UICONTROL Copy]** from the toolbar, provide a name, and click **[!UICONTROL Confirm]**.

* Click **[!UICONTROL Create]**, select **[!UICONTROL Use existing form structure as template]** option, and select an existing form. 
-->

<!-- TBD: Queries for PM and engg.

Can we edit the existing metadata in any form?

How to moderate smart tags?

Allow or deny list for smart tags?

What about Tags displayed just above Smart Tags in the UI?

Is there a detailed metadata tab. Where do the other details of an asset go?

How can one search based strictly on the metadata. Similar to AEM Assets GQL queries.
-->

<!-- TBD: Link to related articles if any.

>[!MORELIKETHIS]
>
>* [Search assets](search.md).
-->
