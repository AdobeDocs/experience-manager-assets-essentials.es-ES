---
title: Reprocesamiento de recursos digitales
description: Obtenga información acerca de los distintos métodos de reprocesamiento de recursos digitales
role: User, Leader, Developer
exl-id: 8d84ecc2-e716-4e25-a0ec-87138ff2c499
TQID: https://experienceleague.adobe.com/08mkBUcjbm5OQaeWzBiLmhwJtCmtSU2Gm0bo9octzUs
product_v2:
  - id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
  - id: f8667931-f646-4dd3-af2a-b9d0cb8098ad
source-git-commit: f026b389ce582ece5d2ca8745d291b1ae50d657e
workflow-type: tm+mt
source-wordcount: 798
ht-degree: 0%

---

# Reprocesamiento de recursos digitales {#reprocessing-digital-assets}

Puede volver a procesar los recursos en una carpeta que ya tenga un perfil de metadatos existente cambiado a posteriori. Si desea que el ajuste preestablecido recién editado se vuelva a aplicar a los recursos existentes en la carpeta, debe volver a procesar la carpeta. Puede volver a procesar tantos recursos como sea necesario.

Vuelva a procesar los recursos en una carpeta si se da cualquiera de las dos situaciones siguientes:

* Desea ejecutar un ajuste preestablecido de conjunto por lotes en una carpeta de recursos existente que ya tenga recursos cargados en ella.
* Posteriormente, edite un ajuste preestablecido de conjunto de lotes existente que se haya aplicado anteriormente a una carpeta de recursos.

## Reprocesar recursos {#reprocessing-steps}

Para volver a procesar recursos en una carpeta:

1. En [!DNL Assets Essentials], en la página Assets, seleccione los recursos agregados recientemente o los recursos que desee volver a procesar.
En caso de que seleccione una carpeta:

   * El flujo de trabajo considera recursivamente todos los archivos de la carpeta seleccionada.
   * Si hay una o más subcarpetas con recursos en la carpeta principal seleccionada, el flujo de trabajo vuelve a procesar cada recurso en la jerarquía de carpetas.
   * Como práctica recomendada, evite ejecutar este flujo de trabajo en una jerarquía de carpetas que tenga más de 1000 recursos.

1. Seleccione **[!UICONTROL Volver a procesar Assets]**. Elija entre las dos opciones:

   ![Opciones de reprocesamiento de Assets](assets/reprocessing-options.png)

   * **[!UICONTROL Proceso completo]:** Seleccione esta opción cuando desee ejecutar el proceso general, incluidos el perfil predeterminado, el perfil personalizado, el procesamiento dinámico (si está configurado) y los flujos de trabajo posteriores al procesamiento.
   * **[!UICONTROL Avanzado]:** Seleccione esta opción para elegir el reprocesamiento avanzado.

     ![Opciones avanzadas de reprocesamiento de Assets](assets/reprocessing-options-advanced.png)

     Seleccione entre las siguientes opciones avanzadas:

      * **[!UICONTROL Representaciones de vista previa predeterminadas]:** Elija esta opción cuando desee volver a procesar las representaciones de vista previa de forma predeterminada.

      * **[!UICONTROL Metadatos]:** Elija esta opción cuando desee extraer información de metadatos y etiquetas inteligentes para los recursos seleccionados.

      * **[!UICONTROL Perfiles de procesamiento]:** Elija esta opción cuando desee volver a procesar un perfil seleccionado. Puede elegir la opción **[!UICONTROL Proceso completo]** para incluir el procesamiento predeterminado y el perfil personalizado asignado en el nivel de carpeta.
        <!--When assets are uploaded to a folder, [!DNL Assets Essentials] checks the containing folder's properties for a processing profile. If none is applied, a parent folder in the hierarchy is checked for a processing profile to apply.-->

      * **[!UICONTROL Flujo de trabajo de procesamiento posterior]:** Elija esta opción donde se requiera un procesamiento adicional de recursos que no se pueda lograr mediante los perfiles de procesamiento. Se pueden añadir a la configuración flujos de trabajo posteriores al procesamiento adicionales. El posprocesamiento le permite agregar un procesamiento completamente personalizado sobre el procesamiento configurable mediante microservicios de recursos.

Consulte [usar microservicios de recursos y perfiles de procesamiento](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/manage/asset-microservices-configure-and-use.html?lang=es) para obtener más información sobre los perfiles de procesamiento y el flujo de trabajo posterior al procesamiento.

![Opciones avanzadas de reprocesamiento de Assets2](assets/reprocessing-options-advanced-2.png)

Después de seleccionar las opciones apropiadas, haga clic en **[!UICONTROL Volver a procesar]**. Aparece el mensaje de éxito.

## Escenarios para reprocesar recursos digitales {#scenarios-reprocessing}

[!DNL Experience Manager] permite el reprocesamiento de recursos digitales para los siguientes componentes.

### Etiquetas inteligentes {#reprocessing-smart-tags}

Las organizaciones que trabajan con recursos digitales utilizan cada vez más vocabulario controlado por taxonomía en los metadatos de recursos. Básicamente, incluye una lista de palabras clave que los empleados, socios y clientes suelen utilizar para referirse a recursos digitales de una clase determinada y buscarlos. El etiquetado de recursos con vocabulario controlado por taxonomía garantiza que los recursos se identifiquen y recuperen fácilmente.

En comparación con los vocabularios de lenguajes naturales, el etiquetado de recursos digitales basado en la taxonomía empresarial ayuda a alinearlos con el negocio de una empresa y garantiza que los recursos más relevantes aparezcan en las búsquedas.

Más información sobre [Etiquetas inteligentes para recursos de vídeo](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/manage/smart-tags-video-assets.html?lang=en).

Más información sobre [Reprocesar etiquetas de color para imágenes existentes en DAM](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/manage/color-tag-images.html?lang=es#color-tags-existing-images).

### Recorte inteligente {#reprocessing-smart-crop}

Obtenga más información sobre [recorte inteligente de Dynamic Media](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/dynamicmedia/image-profiles.html?lang=es) que le permite aplicar un recorte específico (**[!UICONTROL recorte inteligente]** y recorte de píxeles) y una configuración perfeccionada a los recursos cargados.

### Metadatos {#reprocessing-metadata}

[!DNL Adobe Experience Manager Assets] guarda los metadatos de cada recurso. Permite una categorización y organización más sencillas de los recursos y ayuda a las personas que buscan un recurso específico. Con la capacidad de extraer metadatos de archivos cargados en Experience Manager Assets, la administración de metadatos se integra con el flujo de trabajo creativo. Con la capacidad de mantener y administrar metadatos con sus recursos, puede organizar y procesar recursos automáticamente en función de sus metadatos.

Más información sobre [Reprocesando perfiles de metadatos](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/manage/metadata-profiles.html?lang=es).

### Reprocesar recursos de Dynamic Media en una carpeta {#reprocessing-dynamic-media}

Puede volver a procesar los recursos en una carpeta que ya tenga un perfil de imagen de Dynamic Media existente o un perfil de vídeo de Dynamic Media que haya cambiado posteriormente. Para obtener más información, visite [volver a procesar los recursos de Dynamic Media en una carpeta.](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/admin/about-image-video-profiles.html?lang=es)

>[!NOTE]
>
>Debe configurar [!DNL Dynamic Media] en el entorno para habilitar el cuadro de diálogo Dynamic Media.
>

### Flujos de trabajo

Obtenga más información sobre [perfiles de procesamiento y flujos de trabajo posteriores al procesamiento](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/manage/asset-microservices-configure-and-use.html?lang=es).
