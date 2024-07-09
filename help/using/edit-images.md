---
title: Edición de imágenes
description: Edite imágenes mediante opciones que se sirven de [!DNL Adobe Express] y guarde imágenes actualizadas como versiones.
role: User
exl-id: fc21a6ee-bf23-4dbf-86b0-74695a315b2a
source-git-commit: a9ef92194f55da9ad5352adf4251c85e3abcdcd1
workflow-type: tm+mt
source-wordcount: '1138'
ht-degree: 99%

---

# Edición de imágenes en [!DNL Assets Essentials] {#edit-images-in-assets-essentials}

La interfaz de usuario de Asset Essentials permite la edición básica de imágenes, como cambiar el tamaño, quitar el fondo, realizar recortes y convertir entre los formatos JPEG y PNG. Además, permite realizar ediciones avanzadas integrándolas con Adobe Express. Después de editar una imagen, puede guardar la nueva como una nueva versión. El uso de versiones le ayuda a volver al recurso original más adelante, si es necesario. Para editar una imagen, [abra su previsualización](https://experienceleague.adobe.com/es/docs/experience-manager-assets-essentials/help/navigate-view#preview-assets) y haga clic en **Editar imagen**.

>[!NOTE]
>
>Puede editar imágenes de los tipos de archivo PNG y JPEG mediante Adobe Express.

<!--The editing actions that are available are Spot healing, Crop and straighten, Resize image, and Adjust image.-->

## Editar imágenes {#edit-images}

Para acceder a la interfaz de usuario de Asset Essentials utilice el vínculo de [IU de Asset Essentials](https://experience.adobe.com/#/assets) y seleccione el repositorio adecuado. Para obtener acceso, póngase en contacto con el administrador de su organización.
Para cualquier información de consulta adicional, consulte [Introducción a Adobe Experience Manager Assets Essentials](https://experienceleague.adobe.com/es/docs/experience-manager-assets-essentials/help/get-started), [comprensión de la interfaz de usuario](https://experienceleague.adobe.com/es/docs/experience-manager-assets-essentials/help/navigate-view), [casos de uso de Asset Essentials](https://experienceleague.adobe.com/es/docs/experience-manager-assets-essentials/help/get-started#use-cases) y [problemas conocidos](https://experienceleague.adobe.com/es/docs/experience-manager-assets-essentials/help/release-notes).

### Editar imágenes con el Adobe Express {#edit-images-using-adobe-express}

>[!CONTEXTUALHELP]
>id="assets_express_integration"
>title="Integración de Adobe Express"
>abstract="Herramientas de edición de imágenes sencillas e intuitivas con tecnología Adobe Express disponibles directamente en AEM Assets para aumentar la reutilización de contenidos y acelerar la velocidad del contenido."

Después de acceder a la IU de Essentials, haga clic en **Assets**, seleccione una imagen y haga clic en **Editar** en el carril superior. La nueva pantalla muestra las opciones de edición disponibles, como cambiar el tamaño, quitar el fondo, realizar recortes y convertir entre los formatos JPEG y PNG.

#### Cambiar tamaño de imagen {#resize-image-using-express}

Cambiar el tamaño de una imagen a un tamaño específico es un caso de uso popular. Assets Essentials le permite cambiar rápidamente el tamaño de las imágenes para adaptarlas a los tamaños de foto comunes, proporcionando nuevas resoluciones calculadas previamente para tamaños de foto específicos. Para cambiar el tamaño de la imagen mediante Assets Essentials, siga estos pasos:

1. Haga clic en **Cambiar tamaño de la imagen** en el panel izquierdo.
2. Seleccione la plataforma de medios sociales adecuada en la lista desplegable Cambiar tamaño y el tamaño de la imagen en las opciones que se muestran.
3. Escale la imagen, si es necesario, utilizando el campo **Escala de imagen**.
4. Haga clic en **Aplicar** para que tengan efecto los cambios.
   ![Edición de imágenes con Adobe Express](/help/using/assets/adobe-express-resize-image.png)

   La imagen editada está disponible para descargar. Puede guardar el recurso editado como una nueva versión del mismo recurso o guardarlo como uno nuevo.
   ![Guardar imagen con Adobe Express](/help/using/assets/adobe-express-resize-save.png)

#### Quitar fondo {#remove-background-using-express}

Puede quitar el fondo de una imagen siguiendo unos sencillos pasos, tal como se indica a continuación:

1. Haga clic en **Quitar fondo** en el panel izquierdo. Experience Manager Assets muestra la imagen sin fondo.
2. Haga clic en **[!UICONTROL Aplicar]** para que tengan efecto los cambios.
   ![Guardar imagen con Adobe Express](/help/using/assets/adobe-express-remove-background.png)

   La imagen editada está disponible para descargar. Puede guardar el recurso editado como una nueva versión del mismo recurso o guardarlo como uno nuevo.

#### Recortar imagen {#crop-image-using-express}

Transformar una imagen a un tamaño perfecto es fácil gracias al uso de las acciones rápidas de [!DNL Adobe Express] integradas.

1. Haga clic en **[!UICONTROL Recortar imagen]** en el panel izquierdo.
2. Arrastre los identificadores de las esquinas de la imagen para crear el recorte deseado.
3. Haga clic en **[!UICONTROL Aplicar]**.
   ![Guardar imagen con Adobe Express](/help/using/assets/adobe-express-crop-image.png)
La imagen recortada está disponible para descargar. Puede guardar el recurso editado como una nueva versión del mismo recurso o guardarlo como uno nuevo.

#### Convertir entre tipos de archivo de imagen {#convert-image-types-using-express}

Puede convertir rápidamente entre los formatos de imagen JPEG y PNG mediante Adobe Express. Ejecute los siguientes pasos:

1. Haga clic en **JPEG a PNG** o **PNG a JPEG** en el panel izquierdo.
   ![Convertir a PNG con Adobe Express](/help/using/assets/adobe-express-convert-image.png)
2. Haga clic en **[!UICONTROL Descargar]**.

#### Limitaciones {#limitations-adobe-express}

* Resolución de imagen admitida: mínimo de 50 píxeles, máximo de 6000 píxeles por dimensión.
* Tamaño máximo de archivo admitido: 17 MB.

### Edición de imágenes en el editor integrado de Adobe Express {#edit-images-in-adobe-express-embedded-editor}

Los usuarios con derechos para Express pueden utilizar el editor Express integrado desde la interfaz de usuario de Assets Essentials para editar fácilmente el contenido y crear contenido nuevo con GenAI desde Adobe Firefly. Esto mejora la reutilización de contenidos y acelera su velocidad. También puede utilizar elementos predefinidos para que su recurso tenga un aspecto impresionante o realizar acciones rápidas para editar la imagen con solo unos clics.
![express en la IU de essentials](/help/using/assets/express-in-essentials-ui.jpg)
Para editar imágenes con el editor integrado de Adobe Express, siga estos pasos:

1. Acceda a la IU de AEM Assets Essentials mediante el vínculo de [AEM IU de Asset Essentials](https://experience.adobe.com/#/assets) y seleccione el repositorio adecuado.
1. Haga clic en **Assets**, introduzca una carpeta y seleccione una imagen.
1. Haga clic en **Abrir en Adobe Express**. La imagen se abre en un lienzo exprés.
1. Realice los cambios necesarios en la imagen.
1. Si el proyecto requiere que se añadan más páginas, haga clic en **Añadir**, seleccione Assets, introduzca una carpeta, seleccione una imagen para llevarla a la página de lienzo y, a continuación, realice los cambios necesarios en la imagen.
1. Para guardar las imágenes, haga clic en **Guardar**. Aparece el cuadro de diálogo para guardar.

   >[!NOTE]
   >
   > **1. Para una sola página**
   >
   > **Guardar como versión:** esta función solo admite guardar un único recurso. Seleccione esta opción para exportar la imagen como una nueva versión (conservando el formato original) y guardarla en la misma carpeta.
   > **Guardar como nuevo recurso:** seleccione esta opción para exportar el recurso en un formato diferente al original y guardarlo en cualquier carpeta como un nuevo recurso.
   >  
   > **2. Para varias páginas**
   >
   > **Guardar como versión:** esta función solo admite guardar un único recurso. Si desea guardar una sola página de varias páginas, seleccione esta opción para guardar el recurso en su formato y ubicación originales.\
   > **Guardar como nuevo recurso:** con esta opción, exporte varios recursos o un único recurso a cualquier carpeta y guárdelos como nuevos recursos con su formato de archivo original o diferente.

1. En el cuadro de diálogo Guardar:
   1. Introduzca un nombre para el archivo en el campo **Guardar como**.
   1. Seleccione una carpeta de destino.
   1. Opcional: proporcione detalles como el nombre del proyecto o de la campaña, palabras clave, canales, lapso de tiempo y región.
1. Haga clic en **Guardar como versión** o **Guardar como nuevo recurso** para guardar los recursos.

#### Limitaciones de la edición de imágenes en Express Editor {#limitations-of-editing-images-in-the-express-editor}

* Tipo de archivo admitido: JPEG o PNG.
* Tamaño máximo de archivo admitido: 40 MB.
* Rango de anchura y altura admitido: entre 50 y 8000 píxeles.
* Vuelva a cargar la página para ver el nuevo recurso guardado más reciente en la carpeta de origen.

### Creación de nuevos recursos mediante Adobe Express {#create-new-assets-using-embedded-editor}

Assets Essenitals le permite crear una nueva plantilla desde cero utilizando el editor integrado de Adobe Express. Para crear un nuevo recurso con Adobe Express, ejecute los pasos siguientes:

1. Vaya a **Mi espacio de trabajo** y haga clic en **Crear** dentro del banner de Adobe Express que se muestra dentro de Adobe Express en la parte superior. El lienzo en blanco de Adobe Express se muestra en la interfaz de usuario de Assets Essentials.
1. Cree su contenido mediante [Plantillas](https://helpx.adobe.com/es/express/using/work-with-templates.html). En caso contrario, vaya a Sus cosas para modificar el contenido existente.
1. Una vez completada la edición, haga clic en **Guardar**.
1. Especifique la ruta de destino del recurso creado y haga clic en **Guardar como nuevo recurso**.

#### Limitaciones {#limitations}

* Solo puede modificar imágenes de los tipos de formato `JPEG` y `PNG`.
* El tamaño del recurso debe ser inferior a 40 MB.
* Puede guardar una imagen en los formatos `PDF`, `JPEG` o `PNG`.

<!--
## Edit images using [!DNL Adobe Photoshop Express] {#edit-using-photoshop-express}

<!--
After editing an image, you can save the new image as a new version. Versioning helps you to revert to the original asset later, if needed. To edit an image, [open its preview](/help/using/navigate-view.md#preview-assets) and click **[!UICONTROL Edit Image]** ![edit icon](assets/do-not-localize/edit-icon.png) from the rail on the right.

![Options to edit an image](assets/edit-image2.png)

*Figure: The options to edit images are powered by [!DNL Adobe Photoshop Express].*
-->
<!--
### Spot heal images {#spot-heal-images-using-photoshop-express}

If there are minor spots or small objects on an image, you can edit and remove the spots using the spot healing feature provided by Adobe Photoshop.

The brush samples the retouched area and makes the repaired pixels blend seamlessly into the rest of the image. Use a brush size that is only slightly larger than the spot you want to fix.

![Spot healing edit option](assets/edit-spot-healing.png)

<!-- 
TBD: See if we should give backlinks to PS docs for these concepts.
For more information about how Spot Healing works in Photoshop, see [retouching and repairing photos](https://helpx.adobe.com/photoshop/using/retouching-repairing-images.html). 
-->
<!--
### Crop and straighten images {#crop-straighten-images-using-photoshop-express}

Using the crop and straighten option that you can do basic cropping, rotate image, flip it horizontally or vertically, and crop it to dimensions suitable for popular social media websites.

To save your edits, click **[!UICONTROL Crop Image]**. After editing, you can save the new image as a version.

![Option to crop and straighten](assets/edit-crop-straighten.png)

Many default options let you crop your image to the best proportions that fit various social media profiles and posts.

### Resize image {#resize-image-using-photoshop-express}

You can view the common photo sizes in centimeters or inches to know the dimensions. By default, the resizing method retains the aspect ratio. To manually override the aspect ratio, click ![](assets/do-not-localize/lock-closed-icon.png).

Enter the dimensions and click **[!UICONTROL Resize Image]** to resize the image. Before you save the changes as a version, you can either undo all the changes done before saving by clicking [!UICONTROL Undo] or you can change the specific step in the editing process by clicking [!UICONTROL Revert].

![Options when resizing an image](assets/resize-image.png)

### Adjust image {#adjust-image-using-photoshop-express}

[!DNL Assets Essentials] lets you adjust the color, tone, contrast, and more, with just a few clicks. Click **[!UICONTROL Adjust image]** in the edit window. The following options are available in the right sidebar:

* **Popular**: [!UICONTROL High Contrast & Detail], [!UICONTROL Desaturated Contrast], [!UICONTROL Aged Photo], [!UICONTROL B&W Soft], and [!UICONTROL B&W Sepia Tone].
* **Color**: [!UICONTROL Natural], [!UICONTROL Bright], [!UICONTROL High Contrast], [!UICONTROL High Contrast & Detail], [!UICONTROL Vivid], and [!UICONTROL Matte].
* **Creative**: [!UICONTROL Desaturated Contrast], [!UICONTROL Cool Light], [!UICONTROL Turquoise & Red], [!UICONTROL Soft Mist], [!UICONTROL Vintage Instant], [!UICONTROL Warm Contrast], [!UICONTROL Flat & Green], [!UICONTROL Red Lift Matte], [!UICONTROL Warm Shadows], and [!UICONTROL Aged Photo].
* **B&W**: [!UICONTROL B&W Landscape], [!UICONTROL B&W High Contrast], [!UICONTROL B&W Punch], [!UICONTROL B&W Low Contrast], [!UICONTROL B&W Flat], [!UICONTROL B&W Soft], [!UICONTROL B&W Infrared], [!UICONTROL B&W Selenium Tone], [!UICONTROL B&W Sepia Tone], and [!UICONTROL B&W Split Tone].
* **Vignetting**: [!UICONTROL None], [!UICONTROL Light], [!UICONTROL Medium], and [!UICONTROL Heavy].

![Adjust image by editing](assets/adjust-image.png)

<!--
TBD: Insert a video of the available social media options.
-->

### Siguientes pasos {#next-steps}

* Proporcione comentarios de producto mediante la opción [!UICONTROL Comentarios] disponible en la interfaz de usuario de Assets Essentials

* Proporcione comentarios sobre la documentación usando [!UICONTROL Editar esta página] ![editar la página](assets/do-not-localize/edit-page.png) o [!UICONTROL Registrar una incidencia] ![crear una incidencia de GitHub](assets/do-not-localize/github-issue.png), disponibles en la barra lateral derecha

* Contacto con el [Servicio de atención al cliente](https://experienceleague.adobe.com/?support-solution=General&amp;lang=es#support)

>[!MORELIKETHIS]
>
>* [Visualización del historial de versiones de un recurso](/help/using/navigate-view.md)
