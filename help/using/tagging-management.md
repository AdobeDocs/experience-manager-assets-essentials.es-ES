---
title: ¿Cómo se administran las etiquetas en la vista Recursos?
description: Obtenga información sobre cómo administrar etiquetas en la vista Recursos. Las etiquetas le ayudan a categorizar los recursos que se pueden examinar y buscar de forma más eficaz.
source-git-commit: 22786c182ac959739396f694f0a63d84efa28ae5
workflow-type: tm+mt
source-wordcount: '1422'
ht-degree: 0%

---

# Administración de etiquetas en la vista Recursos {#view-assets-and-details}


>[!CONTEXTUALHELP]
>id="assets_taxonomy_management"
>title="Administrar etiquetas"
>abstract="Las etiquetas le ayudan a categorizar los recursos que se pueden examinar y buscar de forma más eficaz. Los administradores tienen la capacidad de utilizar la estructura jerárquica de etiquetado, que facilita la aplicación de metadatos relevantes, la categorización de recursos, la compatibilidad con la búsqueda, la reutilización de etiquetas, la mejora de la capacidad de detección, etc."

Las etiquetas le ayudan a categorizar los recursos que se pueden examinar y buscar de forma más eficaz. El etiquetado ayuda a propagar la taxonomía adecuada a otros usuarios y flujos de trabajo.

Las listas planas de vocabularios controlados pueden volverse inmanejables con el tiempo. Los administradores tienen la capacidad de utilizar la estructura jerárquica de etiquetado, que facilita la aplicación de metadatos relevantes, la categorización de recursos, la compatibilidad con la búsqueda, la reutilización de etiquetas, la mejora de la capacidad de detección, etc.

Puede crear un área de nombres en el nivel raíz y crear una estructura jerárquica de subetiquetas dentro del área de nombres. Por ejemplo, puede crear un `Activities` en el nivel de raíz y tienen `Cycling`, `Hiking`, y `Running` etiquetas dentro del área de nombres. Puede tener más subetiquetas `Clothing` y `Shoes` dentro `Running`.

![Administración de etiquetas](assets/tags-hierarchy.png)

El etiquetado ofrece muchos beneficios, como:

* El etiquetado permite a los autores organizar fácilmente los recursos que no son similares a través de una taxonomía común. Los creadores pueden buscar y organizar recursos rápidamente mediante etiquetas comunes.

* Las etiquetas jerárquicas son extremadamente flexibles y son una excelente manera de organizar los términos de una manera lógica. Mediante áreas de nombres, etiquetas y subetiquetas, se pueden representar sistemas taxonómicos completos.

* Las etiquetas pueden evolucionar con el tiempo a medida que cambia el vocabulario de la organización.

* Las etiquetas administradas en la vista Administración permanecen sincronizadas con las etiquetas administradas en la vista Recursos, que garantiza la integridad y el control de los metadatos.

Para poder aplicar etiquetas a los recursos, primero debe crear un área de nombres y luego crear y agregarle etiquetas. También puede crear etiquetas y agregarlas a un área de nombres existente. Todas las etiquetas que cree en el nivel raíz se agregan automáticamente al espacio de nombres de etiquetas estándar. A continuación, puede agregar el campo Etiquetas al formulario de metadatos para que se muestre en la página Detalles del recurso. Después de configurar estos ajustes, puede empezar a aplicar etiquetas a los recursos.

>[!NOTE]
>
>Únicamente debe agregar el campo Etiquetas al formulario de metadatos si no está utilizando el formulario de metadatos predeterminado.

![Administración de etiquetas](assets/tagging-taxonomy-management.png)

En la vista de administración hay disponibles funcionalidades adicionales además de las mencionadas en este artículo, como combinar, cambiar el nombre, localizar y publicar etiquetas.

## Creación de un área de nombres {#creating-a-namespace}

Un área de nombres es un contenedor para etiquetas que solo puede existir en el nivel raíz. Puede comenzar a configurar la estructura jerárquica de etiquetas definiendo primero un nombre lógico para el área de nombres. Si no agrega una etiqueta a ninguna de las áreas de nombres existentes, la etiqueta se mueve a Etiquetas estándar automáticamente.

Siga estos pasos para crear un área de nombres:

1. Ir a `Taxonomy Management` bajo `Settings` para ver la lista de Áreas de nombres existentes. También puede ver la última fecha de modificación, el usuario que modificó el área de nombres o las etiquetas debajo de ella y el número de veces que la etiqueta se utiliza en un recurso.
1. Haga clic en `Create Namespace`.
1. Añadir `Title`, `Name`, y `Description` para el área de nombres. La entrada especificada en la variable `Title` El campo se muestra en la parte superior de la jerarquía. Por ejemplo, en la siguiente imagen, **Actividades** hace referencia al título del Área de nombres.

   ![Administración de etiquetas](assets/tags-hierarchy.png)

   <!--
    >[!NOTE]
    >You can use `Name` as a primary key if you are using any other metadata management tool is the source of truth for taxonomy values, you can use the name as a primary key.
    >
    -->

1. Haga clic en `Save`.

## Adición de etiquetas a un área de nombres {#adding-tags-to-namespace}

Ejecute los siguientes pasos para agregar etiquetas a un área de nombres:

1. Vaya a `Taxonomy Management`.
1. Seleccione el Área de nombres y haga clic en `Create` para crear la etiqueta en el nivel superior bajo el área de nombres. Si necesita crear una subetiqueta en una etiqueta que exista en un área de nombres, seleccione la etiqueta y haga clic en `Create`.
   ![Jerarquía de etiquetas](assets/hierarchy-of-tags.png)

   En este ejemplo, la imagen de la izquierda representa la etiqueta directamente debajo del área de nombres `automobile-four-wheeler` mostrado en la `Path` field. La imagen de la derecha es un ejemplo de subetiquetas añadidas dentro de una etiqueta, ya que hay más nombres de etiqueta, `jeep` y `jeep-meridian`, que se muestra en `Path` además del Área de nombres.
1. Especifique el título, el nombre y la descripción de la etiqueta y haga clic en `Save`.


   >[!NOTE]
   >
   >* El `Title` y `Name` Los campos de son obligatorios mientras que la variable `Description` es opcional.
   >* De forma predeterminada, la herramienta copia el texto que escriba en el campo Título y elimina los espacios en blanco o los caracteres especiales (. &amp; / \ : * ? [ ] | &quot; %) y lo almacena como el Nombre.
   >* Puede actualizar el `Title` más tarde, pero la variable `Name` El campo es de solo lectura.

## Adición de etiquetas a etiquetas estándar {#adding-tags-to-standard-tags}

Las etiquetas no estructuradas o las etiquetas que no tienen jerarquía se almacenan en `Standard Tags` namespace. Además, si desea agregar términos descriptivos adicionales sin afectar a la taxonomía controlada, puede almacenar ese valor en `Standard Tags`. Con el tiempo, puede mover estos valores a áreas de nombres estructuradas. Además, puede utilizar el `Standard Tags` área de nombres como entrada de forma libre para palabras clave.

Para crear una etiqueta estándar, haga clic en `Create Tag` en el nivel raíz. Especifique el título, el nombre y la descripción y haga clic en `Save`.

![Adición de etiquetas a etiquetas estándar](assets/adding-tags-to-standard-tags.png)

>[!NOTE]
>
>Si elimina `Standard Tags` espacio de nombre mediante la vista de administrador, las etiquetas creadas en el nivel raíz no se muestran en la lista de etiquetas disponibles.

## Mover etiquetas {#moving-tags}

Si almacena las etiquetas en una jerarquía incorrecta o si la taxonomía cambia con el tiempo, puede mover las etiquetas seleccionadas para mantener la integridad de los datos. Se deben tener en cuenta las siguientes condiciones al mover las etiquetas:

* Las etiquetas solo se pueden mover por debajo de áreas de nombres existentes o dentro de una jerarquía de etiquetas existente.
* Las etiquetas no se pueden mover a la raíz para convertirlas en un área de nombres.
* Al mover una etiqueta principal también se mueven todas las etiquetas secundarias almacenadas en la jerarquía.

Siga estos pasos para mover etiquetas de una ubicación a otra:

1. Seleccione la etiqueta o toda la jerarquía de etiquetas en el área de nombres correspondiente y haga clic en `Move`.
1. En el cuadro de diálogo Mover, seleccione la nueva etiqueta de destino o área de nombres con el `Select Tag` sección.
1. Haga clic en `Save`. La etiqueta se muestra en su nueva ubicación.

## Edición de etiquetas {#editing-tags}

Para editar el título de la etiqueta, seleccione la etiqueta y haga clic en `Edit`. Especifique el nuevo título y haga clic en `Save`.

>[!NOTE]
>
>* El `Name` de una etiqueta no se puede actualizar. La ruta raíz de una etiqueta también se basa en el nombre de la etiqueta. La ruta sigue siendo la misma aunque actualice el `Title` field.
>* Las operaciones adicionales, como combinar, localizar y publicar, están disponibles en la vista de administración.

## Eliminación de etiquetas {#deleting-tags}

Puede eliminar varias Áreas de nombres o etiquetas simultáneamente. La operación de eliminación no se puede deshacer.

Siga estos pasos para eliminar etiquetas:

1. Seleccione el área de nombres o la etiqueta y haga clic en `Delete`.
1. Haga clic en `Confirm`.

>[!NOTE]
>
>* Al eliminar la etiqueta principal o el área de nombres, también se eliminan las subetiquetas almacenadas en la jerarquía. Si necesita eliminar o actualizar el área de nombres principal, se recomienda [mover las etiquetas](#moving-tags) al nuevo destino antes de eliminar la jerarquía principal.
>* Al eliminar una etiqueta, también se eliminan todas sus referencias de los recursos.
>* No puede eliminar etiquetas estándar que existan en el nivel raíz.

## Adición del componente Etiquetas al formulario de metadatos {#adding-tags-to-metadata-form}

El componente de etiquetas se agrega al `default` formulario de metadatos automáticamente. Puede diseñar un [Metadatos de formulario](https://experienceleague.adobe.com/docs/experience-manager-assets-essentials/help/metadata.html?lang=en#metadata-forms) mediante una plantilla o desde cero. Si no utiliza una plantilla de formulario de metadatos existente, puede modificar el formulario de metadatos y agregar el componente de etiquetas. La asignación de propiedades de metadatos se rellena automáticamente y no se puede modificar en este momento. Los usuarios en la vista Administración pueden actualizar la asignación para almacenar valores de etiquetas utilizando áreas de nombres personalizadas y exponer solo subconjuntos de jerarquías mediante rutas raíz.

Vea este vídeo rápido para ver cómo agregar el componente Etiquetas al formulario de metadatos:

>[!VIDEO](https://video.tv.adobe.com/v/3420452)


### Adición de etiquetas a los recursos {#adding-tags-to-assets}

1. Vaya a la página de detalles del recurso y navegue hasta el `Tags` de Metadatos.
1. Seleccione el icono del selector de etiquetas que está junto al campo Etiquetas o empiece a escribir un nombre de etiqueta para ver los resultados sugeridos.

   ![Tagging-assets](assets/adding-tags-to-assets.png)

1. Seleccione una o varias etiquetas. La subetiqueta se selecciona automáticamente junto con la etiqueta principal o el área de nombres.
Las etiquetas modificadas en la vista Recursos también se aplican en la vista Administración.

## Restricciones {#limitations}

Las siguientes funciones avanzadas de taxonomía no están disponibles en la vista Recursos en este momento y solo se puede acceder a ellas desde la vista Administración:

* **Localización:** Cualquier localización debe realizarse en la vista Administrador.
* **Ruta raíz:** Las rutas raíz no se pueden configurar. Todas las áreas de nombres almacenadas en Administración de taxonomía se exponen en la propiedad Etiquetas de la vista Recursos.
* **Etiquetas estándar:** Las etiquetas Standard aplicadas en la vista Admin son visibles en la vista Assets. No puede agregar nuevas etiquetas estándar en la vista Recursos de la página Detalles del recurso. Los valores existentes almacenados en etiquetas estándar se aplican en la página Detalles de recursos.
* **Espacios de nombres personalizados:** Las etiquetas no se pueden asignar a áreas de nombres personalizadas.
* **Visualización de referencias:** Los administradores pueden ver el uso de etiquetas en la vista Recursos. Hace referencia a todos los recursos que utilizan activamente una etiqueta. Sin embargo, los administradores no pueden ver recursos individuales que utilicen la etiqueta en las referencias.

<!--
*   Overview
*   Benefits
*   Prerequisites and Permissions
*   Configuration
*   Managing Tags
    *   Creating a Namespace
    *   Adding Tags to a Namespace
    *   Adding Tags to Standard Tags
    *   Moving Tags
    *   Editing Tags
    *   Deleting Tags
*   Applying Tags
    *   Adding Tags to the Metadata form
    *   Adding Tags to Assets
*   Limitations
-->