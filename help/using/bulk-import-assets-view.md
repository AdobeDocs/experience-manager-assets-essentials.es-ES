---
title: Importación masiva de recursos mediante Assets Essentials
description: Obtenga información sobre cómo importar recursos de forma masiva mediante la nueva interfaz de usuario de recursos (Assets Essentials). Permite a los administradores importar un gran número de recursos desde una fuente de datos a AEM Assets.
exl-id: 5f5fc15e-959b-48b6-834a-42b213512b49
source-git-commit: 4d4b239b0b75ac8a26a7c3001e5b28dcb6243f63
workflow-type: tm+mt
source-wordcount: '1812'
ht-degree: 100%

---

# Importación masiva de recursos mediante Assets Essentials   {#bulk-import-essentials}

>[!CONTEXTUALHELP]
>id="assets_bulk_import"
>title="Importación de recursos por lotes"
>abstract="Ahora los administradores pueden importar un gran número de recursos de una fuente de datos a Experience Manager Assets mediante Assets Essentials. Los administradores ya no tienen que cargar archivos o carpetas individuales a Experience Manager Assets. Los proveedores de almacenamiento en la nube admitidos para la importación por lotes son Azure, AWS, Google Cloud y Dropbox."
>additional-url="https://images-tv.adobe.com/mpcv3/4477/98bce651-721c-442e-98b8-c43e7708e44c_1698834577.854x480at800_h264.mp4" text="Ver vídeo"

La importación masiva en la vista de AEM Assets Essentials permite a los administradores importar un gran número de recursos desde una fuente de datos a AEM Assets. Los administradores ya no tienen que cargar archivos o carpetas individuales en Experience Manager Assets.

>[!NOTE]
>
>El importador masivo de Assets Essentials utiliza el mismo back-end que el del importador masivo de Assets as a Cloud Service. Sin embargo, Assets Essentials ofrece más fuentes de datos desde las que importar y una experiencia de usuario más optimizada.

Puede importar recursos desde las siguientes fuentes de datos:

* AWS
* Google Cloud
* Dropbox
* OneDrive
* Azure

## Requisitos previos {#prerequisites}

| Fuente de datos | Requisitos previos |
|-----|------|
| Azure | <ul> <li>Cuenta de almacenamiento de Azure </li> <li> Contenedor de blob de Azure <li> Clave de acceso de Azure o token SAS basado en el modo de autenticación </li></ul> |
| AWS | <ul> <li>Región de AWS </li> <li> Contenedor de AWS <li> Clave de acceso de AWS </li><li> Secreto de acceso de AWS </li></ul> |
| Google Cloud | <ul> <li>Contenedor de GCP </li> <li> Correo electrónico de la cuenta de servicio de GCP <li> Clave privada de la cuenta de servicio de GCP</li></ul> |
| Dropbox | <ul> <li>ID de cliente de Dropbox </li> <li> Secreto de cliente de Dropbox</li></ul> |
| OneDrive | <ul> <li>ID de inquilino de OneDrive </li> <li> ID de cliente de OneDrive</li><li> Secreto de cliente de OneDrive</li></ul> |

Además de estos requisitos previos basados en la fuente de datos, debe tener en cuenta el nombre de la carpeta de origen disponible en la fuente de datos que contiene todos los recursos que deben importarse en AEM Assets.

## Configuración de la aplicación para desarrolladores de Dropbox {#dropbox-developer-application}

Antes de importar recursos desde la cuenta de Dropbox a AEM Assets, cree y configure la aplicación para desarrolladores de Dropbox.

Ejecute los siguientes pasos:

1. Inicie sesión en su [cuenta de Dropbox](https://www.dropbox.com/developers) y haga clic en **[!UICONTROL Crear aplicaciones]**. <br>Si está utilizando una cuenta Enterprise de Dropbox, debe tener acceso a la función de administrador de contenido.

1. En la sección **[!UICONTROL Elegir una API]**, seleccione el único botón de opción disponible.

1. En la sección **[!UICONTROL Elija el tipo de acceso que desea]**, seleccione una de las siguientes opciones:

   * Seleccione **[!UICONTROL Carpeta de aplicación]**, si ha de acceder a una única carpeta creada dentro de su aplicación en su cuenta de Dropbox.

   * Seleccione **[!UICONTROL Dropbox completo]**, si ha de acceder a todos los archivos y carpetas de su cuenta de Dropbox.

1. Especifique un nombre para la aplicación y haga clic en **[!UICONTROL Crear aplicación]**.

1. En la pestaña **[!UICONTROL Configuración]** de la aplicación, añada https://experience.adobe.com a la sección **[!UICONTROL URI de redireccionamiento]**.

1. Copie los valores de los campos **[!UICONTROL Clave de aplicación]** y **[!UICONTROL Secreto de aplicación]**. Los valores son necesarios al configurar la herramienta de importación masiva en AEM Assets.

1. En la pestaña **[!UICONTROL Permisos]**, agregue los siguientes permisos dentro de la sección **[!UICONTROL Ámbitos individuales]**.

   * account_info.read

   * files.metadata.read

   * files.content.read

   * files.content.write

1. Haga clic en **[!UICONTROL Enviar]** para guardar los cambios.

## Configuración de la aplicación para desarrolladores de OneDrive {#onedrive-developer-application}

Antes de importar recursos desde la cuenta de OneDrive a AEM Assets, cree y configure la aplicación para desarrolladores de OneDrive.

<!-- Execute the following steps: -->

### Creación de una aplicación

1. Inicie sesión en su [Cuenta de OneDrive](https://portal.azure.com/#view/Microsoft_AAD_RegisteredApps/ApplicationsListBlade) y haga clic en **[!UICONTROL Nuevo registro]**.

1. Especifique un nombre para la aplicación, seleccione **[!UICONTROL Solo cuentas en este directorio organizativo (solo Adobe: inquilino único)]** de **[!UICONTROL Tipos de cuenta compatibles]**.

1. Ejecute los pasos siguientes para añadir URI de redireccionamiento:

   1. En el menú desplegable **[!UICONTROL Seleccione una plataforma]**, seleccione **[!UICONTROL Web]**.

   1. Añada https://experience.adobe.com a la sección **[!UICONTROL URI de redireccionamiento]**.
   <!-- Add the first URI and click **[!UICONTROL Configure]** to add it. You can add more by clicking **[!UICONTROL Add URI]** option available in the **[!UICONTROL Web]** section on the **[!UICONTROL Authentication]** page. -->

1. Haga clic en **[!UICONTROL Registrar]**. La aplicación se ha creado correctamente.

1. Copie los valores de los campos **[!UICONTROL ID (de cliente) de aplicación]** e **[!UICONTROL ID (de inquilino) de directorio]**. Los valores son necesarios al configurar la herramienta de importación masiva en AEM Assets.

1. Haga clic en **[!UICONTROL Añadir un certificado o secreto]** correspondiente a la opción **[!UICONTROL Credenciales del cliente]**.

1. Haga clic en **[!UICONTROL Nuevo secreto de cliente]**, proporcione la descripción del secreto del cliente, su vencimiento y haga clic en **[!UICONTROL Añadir]**.

1. Después de crear el secreto del cliente, copie el campo **[!UICONTROL Valor]** (No copie el campo ID de secreto). Es necesario al configurar la importación masiva en AEM Assets.

### Añadir permisos de API

Ejecute los siguientes pasos para agregar permisos de API para la aplicación:

1. Haga clic en **[!UICONTROL Permisos de API]** en el panel izquierdo y haga clic en **[!UICONTROL Agregar un permiso]**.
1. Haga clic en **[!UICONTROL Gráfico de Microsoft]** > **[!UICONTROL Permisos delegados]**. La sección **[!UICONTROL Seleccionar permiso]** muestra los permisos disponibles.
1. Seleccione el permiso `offline_access` de `OpenId permissions` y el permiso `Files.ReadWrite.All` de `Files`.
1. Haga clic en **[!UICONTROL Agregar permisos]** para guardar los permisos.

## Crear configuración de importación masiva{#create-bulk-import-configuration}

Siga estos pasos para crear una configuración de importación masiva en [!DNL Experience Manager Assets]:

1. Haga clic en **[!UICONTROL Importación masiva]** en el panel izquierdo y haga clic en **[!UICONTROL Crear importación]**.
1. Seleccione la fuente de datos. Las opciones disponibles incluyen **[!UICONTROL Azure]**, **[!UICONTROL AWS]**, **[!UICONTROL Google Cloud]**, **[!UICONTROL Dropbox]** y **[!UICONTROL OneDrive]**.
1. Especifique un nombre para la configuración de importación masiva en el campo **[!UICONTROL Nombre]**.
1. Especifique las credenciales específicas de la fuente de datos, tal como se menciona en [Requisitos previos](#prerequisites).
1. Proporcione el nombre de la carpeta raíz que contiene los recursos de la fuente de datos en el campo **[!UICONTROL Carpeta de origen]**.

   >[!NOTE]
   >
   >Si utiliza Dropbox como fuente de datos, especifique la ruta de la carpeta de origen en función de las siguientes reglas:
   >* Si selecciona **Dropbox completo** al crear la aplicación Dropbox, y la carpeta que contiene los recursos existe en `https://www.dropbox.com/home/bulkimport-assets`, especifique `bulkimport-assets` en el campo **[!UICONTROL Carpeta de origen]**.
   >* Si selecciona **Carpeta de aplicación** al crear la aplicación Dropbox, y la carpeta que contiene los recursos existe en `https://www.dropbox.com/home/Apps/BulkImportAppFolderScope/bulkimport-assets`, especifique `bulkimport-assets` en el campo **[!UICONTROL Carpeta de origen]**, donde `BulkImportAppFolderScope` hace referencia al nombre de la aplicación. `Apps` se añade automáticamente después de `home` en este caso.

1. (Opcional) Seleccione la opción **[!UICONTROL Eliminar archivo de origen tras importar]** para eliminar los archivos originales del almacén de datos de origen después de importar los archivos en [!DNL Experience Manager Assets].
1. Seleccione el **[!UICONTROL Modo de importación]**. Seleccione **[!UICONTROL Omitir]**, **[!UICONTROL Reemplazar]** o **[!UICONTROL Crear versión]**. El modo de omisión es el predeterminado y, en este modo, el ingestor omite la importación de un recurso si ya existe.
   ![Importar detalles de origen](assets/bulk-import-source-details.png)

1. (Opcional) Especifique el archivo de metadatos que desea importar, proporcionado en formato CSV, en el campo **[!UICONTROL Archivo de metadatos]**. El archivo fuente de metadatos debe estar en la carpeta de origen. Haga clic en **[!UICONTROL Siguiente]** para navegar a **[!UICONTROL Ubicación y filtros]**.
1. Especifique una ruta para definir una ubicación en DAM en la que se importarán los recursos mediante **[!UICONTROL Carpeta de destino de recursos]**. Por ejemplo, `/content/dam/imported_assets`.
1. (Opcional) En la sección **[!UICONTROL Elegir filtros]**, proporcione el tamaño mínimo de archivo de los recursos en MB para incluirlos en el proceso de ingesta en el campo **[!UICONTROL Filtrar por tamaño mínimo]**.
1. (Opcional) Proporcione el tamaño máximo de archivo de los recursos en MB para incluirlos en el proceso de ingesta en **[!UICONTROL Filtrar por tamaño máximo]**.
1. (Opcional) Seleccione los tipos MIME que desea incluir en el proceso de ingesta mediante el campo **[!UICONTROL Incluir tipo MIME]**. Puede seleccionar varios tipos MIME en este campo. Si no define un valor, todos los tipos MIME se incluyen en el proceso de ingesta.

1. (Opcional) Seleccione los tipos MIME que desea excluir en el proceso de ingesta mediante el campo **[!UICONTROL Excluir tipo MIME]**. Puede seleccionar varios tipos MIME en este campo. Si no define un valor, todos los tipos MIME se incluyen en el proceso de ingesta.

   ![Filtros de importación masiva](assets/bulk-import-location.png)

1. Haga clic en **[!UICONTROL Siguiente]**. Seleccione una de las siguientes opciones según su preferencia:

   * **[!UICONTROL Guardar importación]** para guardar la configuración por ahora y poder ejecutarla más adelante.
   * **[!UICONTROL Guardar y ejecutar importación]** para guardar la configuración y ejecutar la importación masiva.
   * **[!UICONTROL Guardar y programar importación]** para guardar la configuración y programar la importación masiva para más adelante. Puede elegir la frecuencia de la importación masiva y establecer la fecha y hora de la importación. La importación masiva se ejecutará en la fecha y hora establecidas en la frecuencia elegida.

   ![Ejecución de una importación masiva](assets/save-run.png)

1. Haga clic en **[!UICONTROL Guardar]** para ejecutar la opción seleccionada.

### Uso de nombres de archivo durante la importación masiva {#filename-handling-bulkimport-assets-view}

Al importar recursos o carpetas de forma masiva, [!DNL Experience Manager Assets] importa toda la estructura existente en el origen de importación. [!DNL Experience Manager] sigue las reglas integradas en cuanto a los caracteres especiales en los nombres de recursos y carpetas, por lo que estos nombres de archivo necesitan limpiarse. Tanto para el nombre de la carpeta como para el nombre del recurso, el título definido por el usuario permanece sin cambios y se almacena en `jcr:title`.

Durante la importación masiva, [!DNL Experience Manager] busque las carpetas existentes para evitar volver a importar los recursos y las carpetas, y compruebe también las reglas de limpieza aplicadas en la carpeta principal en la que se realiza la importación. Si las reglas de limpieza se aplican en la carpeta principal, se aplicarán las mismas reglas al origen de importación. Para la nueva importación, se aplican las siguientes reglas de limpieza para administrar los nombres de archivo de los recursos y las carpetas.

Para obtener más información sobre los nombres no permitidos, el uso de nombres de recursos y el uso de nombres de carpetas durante la importación masiva, consulte [Uso de nombres de archivo durante la importación masiva](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/manage/add-assets.html?lang=es#filename-handling-bulkimport).

## Ver configuraciones de importación masiva existentes {#view-import-configuration}

Para ver las importaciones masivas existentes, seleccione la opción **[!UICONTROL Importaciones masivas]** en el panel izquierdo. Aparece la página de importaciones masivas con la lista de **[!UICONTROL Importaciones ejecutadas]**. <br>
También puede ver las **[!UICONTROL Importaciones guardadas]** e **[!UICONTROL Importaciones programadas]** desde la opción desplegable.

![Guardar configuración de importación masiva](assets/bulk-import-options.png)

<!-- If you select to save and run the import, the import configuration displays in the **[!UICONTROL Executed Imports]** tab.

![Save bulk import configuration](assets/bulk-import-executed.png)

If you schedule an import, it displays in the **[!UICONTROL Scheduled Imports]** tab.  -->

## Editar configuración de importación masiva {#edit-import-configuration}

Para editar los detalles de configuración, haga clic en el ![icono Más](assets/do-not-localize/more-icon.svg) correspondiente al nombre de la configuración y haga clic en **[!UICONTROL Editar]**. No se puede editar el título de la configuración y la fuente de datos de importación mientras se realiza la operación de edición. Puede editar la configuración mediante las pestañas Importaciones ejecutadas, programadas o guardadas.

![Editar configuración de importación masiva](assets/edit-bulk-import.png)

## Programar importaciones únicas o recurrentes {#schedule-imports}

Para programar una importación masiva única o recurrente, ejecute los siguientes pasos:

1. Haga clic en el ![icono Más](assets/do-not-localize/more-icon.svg) correspondiente al nombre de configuración disponible en la pestaña **[!UICONTROL Importaciones ejecutadas]** o **[!UICONTROL Importaciones guardadas]** y haga clic en **[!UICONTROL Programación]**. También puede reprogramar una importación programada existente navegando hasta **[!UICONTROL Importaciones programadas]** y haciendo clic en **[!UICONTROL Programación]**.

1. Establezca una ingesta única o programe una programación horaria, diaria o semanal. Haga clic en **[!UICONTROL Enviar]**.

   ![Programar configuración de importación masiva](assets/bulk-import-schedule.png)

## Realizar una comprobación de estado de importación {#import-health-check}

Para validar la conexión con la fuente de datos, haga clic en el ![icono Más](assets/do-not-localize/more-icon.svg) correspondiente al nombre de la configuración y, a continuación, haga clic en **[!UICONTROL Comprobación]**. Si la conexión se realiza correctamente, Experience Manager Assets muestra el siguiente mensaje:

![Comprobación de estado de importación masiva](assets/bulk-import-health-check.png)

## Realice un ensayo antes de ejecutar una importación {#dry-run-bulk-import}

Haga clic en el ![icono Más](assets/do-not-localize/more-icon.svg) correspondiente al nombre de la configuración y haga clic en **[!UICONTROL Ensayo]** para invocar una ejecución de prueba para el trabajo de importación masiva. Experience Manager Assets muestra los siguientes detalles sobre el trabajo de importación masiva:

![Comprobación de estado de importación masiva](assets/bulk-import-dry-run.png)

## Ejecución de una importación masiva {#run-bulk-import}

Si ha guardado la importación al crear la configuración, puede ir la pestaña Importaciones guardadas, hacer clic en el ![icono Más](assets/do-not-localize/more-icon.svg) correspondiente a la configuración y hacer clic en **[!UICONTROL Ejecutar]**.

Del mismo modo, si necesita efectuar una importación ya ejecutada, vaya a la pestaña Importaciones ejecutadas, haga clic en el ![icono Más](assets/do-not-localize/more-icon.svg) correspondiente al nombre de configuración y haga clic en **[!UICONTROL Ejecutar]**.

## Detener o programar una importación en curso {#schedule-stop-ongoing-report}

Puede programar o detener una importación masiva en curso mediante el cuadro de diálogo de estado de importación masiva que aparece en la página de inicio Importación masiva durante una importación.

![Importación en curso](assets/bulk-import-progress.png)

También puede ver los recursos que se han importado en la carpeta de destino haciendo clic en **[!UICONTROL Ver recursos]**.


## Eliminar una configuración de importación masiva {#delete-bulk-import-configuration}

Haga clic en el ![icono Más](assets/do-not-localize/more-icon.svg) correspondiente al nombre de configuración existente en las pestañas **[!UICONTROL Importaciones ejecutadas]**, **[!UICONTROL Importaciones programadas]** o **[!UICONTROL Importaciones guardadas]** y haga clic en **[!UICONTROL Eliminar]** para borrar la configuración de importación masiva.

## Ir a los recursos después de realizar una importación masiva {#view-assets-after-bulk-import}

Para ver la ubicación de destino de los recursos donde se importan después de ejecutar el trabajo de importación masiva, haga clic en el ![icono Más](assets/do-not-localize/more-icon.svg) correspondiente al nombre de la configuración y, a continuación, haga clic en **[!UICONTROL Ver recursos]**.

## Vídeo: Importación masiva de recursos mediante Assets Essentials

>[!VIDEO](https://video.tv.adobe.com/v/3428012)
