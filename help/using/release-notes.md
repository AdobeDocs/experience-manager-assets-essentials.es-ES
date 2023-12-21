---
title: Notas de la versión
description: Notas de la versión y problemas conocidos de [!DNL Assets Essentials]
role: User,Leader,Admin,Architect,Developer
contentOwner: AK
exl-id: a0e29eb6-336a-4f78-b7bd-ec1338c86775
source-git-commit: 10d82a8a90e718272c9bb1c5b14db30785bb1ded
workflow-type: tm+mt
source-wordcount: '2617'
ht-degree: 88%

---

# Notas de la versión de [!DNL Assets Essentials] {#release-notes}

La versión actual de Assets Essentials se publicó el miércoles, 19 de diciembre de 2023.

Algunas de las funciones añadidas recientemente incluyen:

**Creación de imágenes de GenAI con Adobe Firefly**

Cree nuevas imágenes basadas en consultas de búsqueda con una integración de la función de Adobe Firefly de texto a imagen (requiere licencia de Adobe Firefly).

![Integración del Firefly de recursos](/help/using/assets/assets-firefly-integration.png)

**Buscar imágenes similares**

Ahora puede encontrar contenido fácilmente seleccionando una imagen y viendo imágenes similares en el repositorio de Experience Manager Assets.

**Editor de Adobes Express incrustados en AEM Assets**

Los usuarios con acceso a Express ahora disponen de herramientas integradas de edición y creación de imágenes desde Adobe Express y Adobe Firefly disponibles directamente en AEM Assets para mejorar la reutilización del contenido y acelerar la velocidad de contenido.

![asignar formulario de metadatos a una carpeta](/help/using/assets/adobe-express-aem-assets.png)

<!--

**Smart tags blocklist** 

Assets Essentials now enables you to define a list of blocked tags. These tags are automatically removed from the auto-generated smart tags when you upload assets to the repository. This capability performs tags governance and saves a lot of time as you can add a tag to the block list and Assets Essentials automatically excludes it from the list of tags for any of the assets that are added to the repository.

  ![storage usage insights](/help/using/assets/block-tags.png)

-->

**Informes de uso del almacenamiento en Insights**:

Los administradores ahora pueden ver los informes de uso del almacenamiento disponibles como parte de Insights.

![datos de uso de almacenamiento](/help/using/assets/storage-usage-insights.png)

**Configuración de la primera página principal de búsqueda**

Assets Essentials ahora le permite configurar la experiencia de la página principal para su organización. Si selecciona buscar primero como página principal, puede configurar la alineación de la barra de búsqueda, la imagen de fondo y el logotipo de su organización.

![buscar primera configuración](/help/using/assets/search-first-configuration.png)



**Mejoras basadas en los comentarios de los clientes**

Mejoras y correcciones de errores basadas en los comentarios de los clientes.


## Problemas conocidos {#known-issues}

La lista de problemas conocidos de la oferta de [!DNL Assets Essentials] se revisa y actualiza de forma continua:

<!--

* Assets Essentials does not support creating Private collections.

-->


* Las colecciones privadas están disponibles para el creador y los usuarios con privilegios de administrador. Como administrador, no puede delegar los permisos para acceder a la colección a otros usuarios.

* Como administrador, no puede delegar los permisos para acceder a la colección a otros usuarios.

Si encuentra algún problema o incluso si tiene solicitudes de mejora, [proporcione comentarios](#provide-feedback) al equipo.

## Versiones anteriores {#past-releases}

### Versión de octubre de 2023 {#october2023-release}

**Importación masiva de recursos desde la fuente de datos de OneDrive**

Los administradores ahora tienen la capacidad de [importar un gran número de recursos de OneDrive a AEM Assets](/help/using/bulk-import-assets-view.md). La lista actualizada de las fuentes de datos compatibles para la importación masiva incluye Azure, AWS, Google Cloud, Dropbox y OneDrive.

![asignar formulario de metadatos a una carpeta](/help/using/assets/bulk-import-source-details.png)

**Compatibilidad de derechos entre organizaciones para bibliotecas**

Experience Manager Assets ahora permite configurar el acceso a las bibliotecas de Creative Cloud en una organización IMS diferente. Permite un acceso más sencillo a los flujos de trabajo entre productos más recientes entre Creative Cloud y Experience Manager, y reduce el tiempo y el esfuerzo de los creativos.

### Versión de septiembre de 2023 {#september2023-release}

**Asignar un formulario de metadatos a una carpeta**

Ahora puede asignar un formulario de metadatos a una carpeta específica dentro de la implementación de Assets Essentials. Todos los recursos de la carpeta, incluidos los de las subcarpetas, muestran las propiedades definidas en el formulario de metadatos asignado.

![asignar formulario de metadatos a una carpeta](/help/using/assets/assign-to-folder.png)

**Importación masiva de recursos desde fuentes de datos**

Ahora los administradores tienen la capacidad de importar un gran número de archivos de una fuente de datos a AEM Assets. Los administradores ya no tienen que cargar archivos o carpetas individuales a AEM Assets. Las fuentes de datos admitidas para la importación masiva son Azure, AWS, Google Cloud y Dropbox.

![Importación masiva de recursos desde una fuente de datos](/help/using/assets/bulk-import.png)

**Herramientas de edición de imágenes con tecnología de Adobe Express**

Herramientas de edición de imágenes sencillas e intuitivas con tecnología Adobe Express disponibles directamente en AEM Assets para aumentar la reutilización de contenidos y acelerar la velocidad del contenido.

![Edición de imágenes con Adobe Express](/help/using/assets/edit-adobe-express.png)

**Flexibilidad al fijar elementos para el acceso rápido de Mi espacio de trabajo**

Capacidad para seleccionar y fijar elementos para usted, para toda su organización o para una lista de grupos, de modo que aparezcan en la sección Acceso rápido de Mi espacio de trabajo en función de su selección.

![Fijar elementos para grupos](assets/pin-items-for-groups.png)


### Versión de julio de 2023 {#july2023-release}

**Marco de trabajo de inteligencia artificial mejorado para las etiquetas inteligentes de imagen**

Experience Manager Assets ahora utiliza un marco de inteligencia artificial mejorado para las etiquetas inteligentes de imagen. Esta inteligencia de contenido mejora la relevancia y precisión de las etiquetas inteligentes disponibles para todos los recursos de imagen durante la ingesta.

**Configurar la visualización de columnas para la vista Lista de recursos**

Assets Essentials ahora permite seleccionar las columnas que se muestran en la vista Lista de recursos, como Estado, Formato, Dimensión, Tamaño, etc.

![Configuración de las columnas](/help/using/assets/configure-columns.png)

**Ordenar resultados de búsqueda según la relevancia**

Assets Essentials ahora ordena los resultados de la búsqueda según la relevancia de forma predeterminada. Puede ordenar los recursos buscados en orden creciente o descendente de `Name`, `Relevance`, `Size`, `Modified` y `Created`.

### Versión de junio de 2023 {#june2023-release}

**Etiquetado jerárquico de recursos para una experiencia de búsqueda más rápida**

Las listas planas de vocabularios controlados se vuelven inmanejables con el tiempo. Assets Essentials admite ahora la estructura de etiquetado jerárquica, que facilita la aplicación de metadatos relevantes, la categorización de recursos, la compatibilidad con la búsqueda, la reutilización de etiquetas, la mejora de la capacidad de detección, etc.

![Administración de etiquetado](assets/tags-hierarchy.png)

**Fijación de archivos, carpetas y colecciones para un acceso rápido**

Ahora puede fijar archivos, carpetas y colecciones para acceder más rápidamente a estos elementos cuando los necesite más adelante. Los elementos fijados se muestran en la sección **Acceso rápido** de Mi espacio de trabajo. Puede acceder a ellos mediante Mi espacio de trabajo en lugar de desplazarse a la ubicación en la que se guardan en el repositorio.

![Tareas en el espacio de trabajo](assets/quick-access.png)

**Filtrado de recursos en la carpeta Papelera**

Assets Essentials permite ahora filtrar los recursos disponibles en la carpeta Papelera. Puede aplicar filtros estándar o personalizados para buscar los recursos adecuados en la carpeta Papelera y restaurarlos o eliminarlos de forma permanente.

**Vistas previas de miniaturas para recursos 3D**

Assets Essentials genera ahora vistas previas de miniaturas para formatos de archivo 3D comunes, incluidos gLB, USDz, FBX, 3DS, OBJ y SBSAR. Cuando estos archivos se cargan en Assets Essentials, el sistema genera automáticamente las miniaturas de forma predeterminada.

![Tareas en el espacio de trabajo](assets/3d-preview.png)

**Ver los términos más buscados**

Assets Essentials ahora admite la visualización de los términos más buscados en la implementación de Assets Essentials mediante la sección **Insights** de Mi espacio de trabajo. También puede navegar hasta Insights detallados para ver las búsquedas principales durante los últimos 30 días o 12 meses.

![Tareas en el espacio de trabajo](assets/insights-top-searches.png)

**Mejoras en formularios de metadatos**

Assets Essentials permite ahora añadir texto de varios valores y componentes de propiedad de lista desplegable a los formularios de metadatos.

### Varias versiones en 2023 {#multiple-releases-2023}

La lista de funciones agregadas recientemente incluye las siguientes:

**Principales recursos descargados**

Mi espacio de trabajo ahora muestra los diez recursos más descargados para su entorno de Assets Essentials en la sección [!UICONTROL Contenido]. También puede ver el tipo de formato y el número de descargas de cada recurso de la lista.

**Actualizaciones masivas en los metadatos de recursos**

Las actualizaciones de metadatos masivas le permiten ejecutar simultáneamente actualizaciones de metadatos comunes en varios recursos. No es necesario actualizar los registros de forma individual y puede aplicar rápidamente propiedades a los recursos o carpetas a los que se accede mediante búsquedas.

**Mi espacio de trabajo con widgets configurables**

Assets ahora proporciona un espacio de trabajo personalizado, que sirve como solución integral para proporcionar un acceso práctico a las áreas clave de la interfaz de usuario de Assets y a la información más relevante para usted. Un acceso más rápido a estas opciones aumenta la velocidad de contenido y la eficacia de sus proyectos.

Mi espacio de trabajo incluye widgets para perspectivas, tareas y contenido. Puede configurar cómo se muestran estos widgets en el espacio de trabajo en función de sus preferencias.

**IU de administración de tareas dedicadas**

Assets Essentials ahora le permite administrar la lista de tareas que tiene asignadas, que ha creado y completado en una ubicación centralizada, utilizando la nueva opción **[!UICONTROL Tareas]** disponible en el panel de navegación izquierdo. También puede realizar las acciones adecuadas seleccionando una tarea para aprobarla o rechazarla, o abriendo los detalles de la tarea para aprobarla, rechazarla, editarla o eliminarla.

![Tareas en el espacio de trabajo](assets/tasks-workspace.png)

**Vínculos generados automáticamente para compartir archivos**

Assets Essentials ahora genera un vínculo automáticamente en cuanto elige compartir un recurso mediante la interfaz de usuario de Assets Essentials. El vínculo generado sigue siendo válido incluso si se cambia la fecha de caducidad.

![Tareas en el espacio de trabajo](assets/share-asset.png)


**Mejoras basadas en los comentarios de los clientes**

Mejoras y correcciones de errores basadas en los comentarios de los clientes.

### 2022.11.0 {#november-2022}

La versión de noviembre de [!DNL Assets Essentials] se publicó el 17 de noviembre de 2022.

Esta versión proporciona lo siguiente:

**Vista previa de documentos con el visualizador Document Cloud**

Assets Essentials ahora le permite cargar documentos en otros tipos de formato compatibles y previsualizarlos con el visualizador incluido en Document Cloud. Los tipos de formato compatibles son TXT, RTF, DOC, DOCX, PPT, PPTX, XLS y XLSX.

<!--

**View Smart Tags moderation reports**

Asset reporting now provides administrators with visibility into the Smart Tags promoted or deleted for an asset. You can specify a folder path and the report lists the Smart Tags promoted or deleted for all assets available at the folder path.

-->

<!--
**Read-only access to large number of users**

Assets Essentials allows administrators to provide read-only access to a large number of users for selected assets or folders in the repository. 
You can easily synchronize the user groups available on the external identity management of an organization with Adobe Admin Console and then manage permissions in Admin Console and Assets Essentials to provide the users with read-only access for selected assets or folders.

-->


**Nueva opción de guardado de metadatos**

Ahora hay disponible una nueva opción para guardar metadatos en la interfaz de usuario de Assets Essentials, para mejorar el control de los metadatos.

**Mejoras basadas en los comentarios de los clientes**

Mejoras y correcciones de errores basadas en los comentarios de los clientes.

**Adobe Asset Link, versión 3.3**

La versión 3.3 de [Adobe Asset Link](https://helpx.adobe.com/es/enterprise/using/adobe-asset-link.html) se publicó el 13 de diciembre de 2022 con las siguientes funciones:

* Compatibilidad con [Creative Cloud para equipos](https://www.adobe.com/es/creativecloud/business/teams.html) además de [Creative Cloud para empresas](https://www.adobe.com/es/creativecloud/business/enterprise.html) antes.

* Compatibilidad con las últimas aplicaciones de Adobe InDesign, Photoshop e Illustrator 2023.

* Compatibilidad para utilizar el complemento CEP de Adobe Asset Link en entornos con servidores proxy.

### 2022.8.0 {#august-2022}

La versión de [!DNL Assets Essentials] de agosto de se publicó el 22 de agosto de 2022.

Esta versión proporciona lo siguiente:

**Notificaciones para colecciones**

Las notificaciones de Assets Essentials ahora permiten supervisar las operaciones realizadas en los recursos, colecciones o carpetas disponibles en el repositorio. Debe seleccionar y suscribirse a las colecciones para las que se le envían las notificaciones. También puede configurar las operaciones para las que se le envían las notificaciones, como las de eliminación, uso compartido de vínculos, movimiento, cambio de nombre y actualización ejecutadas en las colecciones.

**Editar colecciones inteligentes**

Assets Essentials ahora también permite editar los criterios de búsqueda utilizados al crear una colección inteligente.  Guarde los nuevos criterios de búsqueda para actualizar el contenido de la colección de forma dinámica.

**Ver estadísticas activas de la cuenta de almacenamiento**

Assets Essentials ahora también le permite ver datos de la cuenta de almacenamiento en tiempo real de su entorno de Assets Essentials con el tablero Estadísticas activas. Puede ver las métricas de eventos en tiempo real durante los últimos 30 días o 12 meses.

**Ver informes de carga**

La creación de informes de activos ahora proporcionan a los administradores visibilidad de los activos cargados en la implementación de Adobe Experience Manager Assets Essentials. Los administradores ya tienen la capacidad de generar informes para los activos descargados de la implementación de Assets Essentials. Estos datos proporcionan información útil sobre cómo los usuarios interactúan con el contenido y el producto.

**Mejoras basadas en los comentarios de los clientes**

Mejoras y correcciones de errores basadas en los comentarios de los clientes.

### 2022.6.0 {#june-2022}

La versión de junio de [!DNL Assets Essentials] se publicó el 14 de julio de 2022.

Esta versión proporciona lo siguiente:

**Colecciones inteligentes**

Guarde los resultados de búsqueda como una colección inteligente para actualizar dinámicamente el contenido de la colección. Si hay recursos agregados al repositorio de Assets Essentials que se ajustan a los criterios de búsqueda definidos al [crear la colección inteligente](manage-collections.md#create-smart-collection), el contenido de la colección inteligente se actualiza automáticamente.

**Notificaciones**

Las notificaciones de Assets Essentials permiten [supervisar las operaciones realizadas en los recursos o carpetas disponibles en el repositorio](manage-notifications.md). Debe seleccionar y suscribirse al contenido para el que se le envían las notificaciones. También puede configurar las categorías a las que se envían las notificaciones.

**Creación de informes**

La creación de informes de recursos permiten a los administradores evaluar la actividad del usuario dentro de Adobe Experience Manager Assets Essentials. Los informes y el tablero de estadísticas activas proporcionan información útil sobre cómo los usuarios interactúan con los recursos disponibles en la implementación. [Utilice la información de los informes](manage-reports.md) para derivar métricas de éxito clave para medir la adopción de Recursos en su empresa y por parte de los clientes.

Vea los informes de descarga de recursos y el módulo del tablero de estadísticas activas para ver qué recursos se descargan y la frecuencia de las descargas.

### 2022.5.0 {#may-2022}

La versión de mayo de [!DNL Assets Essentials] se publicó el 16 de junio de 2022.

Esta versión proporciona lo siguiente:

**Mejoras en el estado de los activos**

* Assets Essentials ahora le permite [establecer una fecha de caducidad para un recurso](manage-organize.md#set-asset-status). Además, puede [filtrar recursos](search.md#refine-search-results) en función del `Expired` estado del activo y un intervalo de fechas de caducidad.

* Ahora puede ver el indicador de estado de los activos para todos los recursos disponibles en Papelera. Como resultado, puede tomar la decisión de restaurar un recurso en función de su estado.

**Mejoras en los filtros de búsqueda**

* Assets Essentials ahora le permite [filtrar recursos](search.md#refine-search-results) usando el `No Status` estado del activo.

<!--

* Assets Essentials now supports [using a wildcard operator (*) while using custom filters](search.md#custom-filters) to enable Assets Essentials to display assets in the results that partially match the search criteria.

-->

**Mejoras en las colecciones**

<!--

* Assets Essentials now enables you to [create Private collections](manage-collections.md#create-collection).

-->

* Assets Essentials ahora es compatible con la [descarga de una colección](manage-collections.md).

* Ahora puede editar el campo Metadatos de descripción de una colección.

**Mejoras en la documentación**

* Una nueva versión de [Documentación general de Assets Essentials](introduction.md) ya está disponible.

**Mejoras basadas en los comentarios de los clientes**

* Mejoras y correcciones de errores basadas en los comentarios de los clientes.

### 2022.4.0 {#april-2022}

La versión actual de [!DNL Assets Essentials] se publicó el 12 de mayo de 2022. Esta versión proporciona lo siguiente:

* [!DNL Assets Essentials] ahora admite la [creación de colecciones](manage-collections.md). Una colección es un conjunto de recursos dentro de Experience Manager Assets Essentials. Utilice las colecciones para compartir recursos entre los usuarios. A diferencia de las carpetas, una colección puede incluir recursos de distintas ubicaciones.

* Assets Essentials ahora también le permite [añadir filtros personalizados](search.md#custom-filters) a la interfaz de usuario. A continuación, puede aplicar esos filtros personalizados además de los filtros estándar para restringir los resultados de búsqueda.

* Assets Essentials ahora le permite [establecer el estado](manage-organize.md#set-asset-status) en los recursos disponibles en el repositorio. Establezca un estado de recurso para gobernar y administrar mejor el consumo descendente de recursos digitales.

* Mejoras y correcciones de errores basadas en los comentarios de los clientes.

#### Modo incógnito en Chrome {#incognito-mode}

Con esta versión, estamos optimizando el rendimiento del envío de la interfaz de usuario y de las funciones específicas de Assets Essentials (comentar sobre los recursos y la edición de imágenes) depende de que se habiliten el almacenamiento local del explorador y las cookies de terceros. El modo incógnito del explorador web Chrome bloquea las cookies de terceros de forma predeterminada: los usuarios tienen varias opciones para seguir accediendo a todas las funciones:

* Utilice los perfiles de Chrome en lugar del modo Incognito, cuando el usuario necesita separar las sesiones del navegador

* Desactive el `Block third-party cookies` en la pantalla del modo Incognito en Chrome

### 2022.2.0 {#march-2022}

[!DNL Assets Essentials] se publicó el 9 de marzo de 2022, con las siguientes actualizaciones:

* [!DNL Assets Essentials] ahora le permite [generar un vínculo y compartir recursos con partes interesadas externas](share-links-for-assets.md), que no tienen acceso a la aplicación [!DNL Assets Essentials]. Puede definir una fecha de caducidad para el vínculo y luego compartirlo con otras personas mediante el método de comunicación que prefiera, como el correo electrónico o los servicios de mensajería. Los destinatarios del vínculo pueden obtener una vista previa de los recursos y descargarlos.

* [!DNL Assets Essentials] ahora incluye [un perfil de producto de administrador](deploy-administer.md#add-users-to-essentials) en Admin Console, además de los perfiles de producto de usuarios normales y consumidores existentes. Un administrador ahora puede asignar otros usuarios al perfil de producto del administrador.

* Assets Essentials ahora permite a los administradores [administrar los niveles de acceso para las carpetas disponibles en el repositorio](manage-permissions.md). Como administrador, puede crear grupos de usuarios y asignar permisos a esos grupos para administrar los niveles de acceso. También puede delegar los privilegios de administración de permisos a grupos de usuarios en el nivel de carpeta.

* Mejoras y correcciones de errores basadas en los comentarios de los clientes.

Además, la extensión de [!DNL Adobe Asset Link] para Creative Cloud (Photoshop, Illustrator e InDesign) tiene una [nueva versión 3.2](https://exchange.adobe.com/creativecloud.details.106875.adobe-asset-link-cep.html), con mejoras de rendimiento en el tiempo de inicio del panel y en la velocidad de descarga.


### Versión 2022.1.0 {#january-2022}

[!DNL Assets Essentials] se publicó el 3 de febrero de 2022, con las siguientes actualizaciones:

* Mejoras de rendimiento para la operación [!UICONTROL Crear carpeta]. <!-- CQ-4338818 -->

### Versión 2021.11.0 {#november-2021}

[!DNL Assets Essentials] se publicó el 16 de diciembre de 2021, con las siguientes actualizaciones:

* Adobe implementa Assets Essentials automáticamente después de completar el proceso de aprovisionamiento. Los administradores no necesitan realizar pasos adicionales para implementar Assets Essentials mediante la interfaz de usuario de [!DNL Cloud Manager]. Esta implementación automática estará disponible para los entornos aprovisionados a partir del 6 de enero de 2022.
* Hay nuevas versiones de los complementos de Creative Cloud que funcionan con Assets Essentials disponibles en Adobe Exchange: [Adobe Asset Link para Adobe XD v. 2.1.0](https://exchange.adobe.com/creativecloud/plugindetails.html/app/cc/61d229b9) y [Adobe Asset Link para Photoshop/InDesign/Illustrator v. 3.1.65](https://exchange.adobe.com/creativecloud.details.106875.adobe-asset-link-cep.html).
* Varias correcciones de errores y mejoras del producto, incluidos problemas conocidos previos (ahora las carpetas se muestran correctamente en el árbol de navegación izquierdo después de la carga<!-- CQ-4337638 -->, la carga de arrastrar y soltar permite al usuario seleccionar la carpeta actual o cualquier subcarpeta al soltarla para la carga<!-- CQ-4327753 -->).

### Versión 2021.8.0 {#august2021}

[!DNL Assets Essentials] 2021.8.0 se publicó el 30 de agosto de 2021, con las siguientes actualizaciones:

* Integraciones con [!DNL Adobe Workfront] que permiten a los usuarios de [!DNL Workfront] administrar sus recursos digitales en el contexto de la administración de su trabajo.

### Versión 2021.7.0 {#july2021}

[!DNL Assets Essentials] 2021.7.0 se publicó el 29 de julio de 2021, con las siguientes actualizaciones:

* Puede crear y administrar formularios de metadatos personalizados que se utilizarán para mostrar las propiedades de los metadatos a los usuarios en la pantalla de detalles de recursos de la opción [!UICONTROL Formularios de metadatos], en [!DNL Settings]. Consulte [Formularios de metadatos](metadata.md#metadata-forms).
* Varias correcciones de errores y mejoras del producto, incluido un mejor rendimiento al cargar una carpeta anidada con muchas subcarpetas.

### Versión 2021.6.0 {#june2021}

La primera versión de [!DNL Assets Essentials], que se publicó el 21 de junio de 2021, ofrece funciones de administración de recursos ligeras. Admite las siguientes funciones principales y operaciones CRUD (crear, leer, actualizar y eliminar):

* Cargue y añada recursos, incluidas carpetas anidadas. Previsualice los recursos y las versiones.
* Búsqueda de texto completo, filtros de búsqueda con matices y búsquedas guardadas para una detección rápida de recursos.
* Operaciones básicas de administración de recursos como actualizar, eliminar, descargar y administrar metadatos.
* [!DNL Assets Essentials] está disponible para los usuarios de [!DNL Adobe Journey Optimizer] para administrar los recursos al crear mensajes.
