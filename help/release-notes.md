---
title: Notas de la versión
description: Notas de la versión y problemas conocidos de [!DNL Assets Essentials]
role: User,Leader,Admin,Architect,Developer
contentOwner: AK
exl-id: a0e29eb6-336a-4f78-b7bd-ec1338c86775
source-git-commit: f273e1e3c8a290e0beee0423da00c63013062c43
workflow-type: tm+mt
source-wordcount: '1117'
ht-degree: 80%

---

# Notas de la versión de [!DNL Assets Essentials] {#release-notes}

La versión actual de [!DNL Assets Essentials] está disponible el 14 de julio de 2022.

Esta versión proporciona lo siguiente:

**Colecciones inteligentes**

Guarde los resultados de búsqueda como una colección inteligente para actualizar dinámicamente el contenido de la colección. Si hay recursos agregados al repositorio de Assets Essentials que se ajustan a los criterios de búsqueda definidos al [creación de la colección inteligente](manage-collections.md#create-smart-collection), el contenido de la colección inteligente se actualiza automáticamente.

**Notificaciones**

Las notificaciones de Assets Essentials le permiten [supervisar las operaciones realizadas en los recursos o carpetas disponibles en el repositorio](manage-notifications.md). Debe seleccionar y suscribirse al contenido para el que se le envían las notificaciones. También puede configurar las categorías a las que se envían las notificaciones.

**Informes**

Los informes de recursos permiten a los administradores evaluar la actividad del usuario dentro de Adobe Experience Manager Assets Essentials. El panel de informes y estadísticas activas proporciona información útil sobre cómo los usuarios interactúan con los recursos disponibles en la implementación. [Utilizar la información de los informes](manage-reports.md) para obtener métricas de éxito clave para medir la adopción de activos dentro de su empresa y por parte de los clientes.

Vea los informes de descarga de recursos y el módulo del tablero de estadísticas activas para ver qué recursos se descargan y la frecuencia de las descargas.

**Mejoras basadas en los comentarios de los clientes**

Mejoras y correcciones de errores basadas en los comentarios de los clientes.


## Problemas conocidos {#known-issues}

La lista de problemas conocidos de la oferta de [!DNL Assets Essentials] se revisa y actualiza de forma continua:

<!--

* Assets Essentials does not support creating Private collections.

-->


* Assets Essentials no admite la edición de colecciones inteligentes.

* Las colecciones privadas están disponibles para el creador y los usuarios con privilegios de administrador. Como administrador, no puede delegar los permisos para acceder a la colección a otros usuarios.

Si encuentra algún problema o incluso si tiene solicitudes de mejora, [proporcione comentarios](#provide-feedback) al equipo.

## Versiones anteriores {#past-release}

### 2022.5.0 {#may-2022}

La versión actual de [!DNL Assets Essentials] se publicó el 16 de junio de 2022.

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

* Integraciones con [!DNL Adobe Workfront] que permiten a los usuarios de [!DNL Workfront] administrar sus recursos digitales en el contexto de la administración de su trabajo. Para obtener más información, consulte [integraciones con otras soluciones de Adobe](/help/integration.md).

### Versión 2021.7.0 {#july2021}

[!DNL Assets Essentials] 2021.7.0 se publicó el 29 de julio de 2021, con las siguientes actualizaciones:

* Puede crear y administrar formularios de metadatos personalizados que se utilizarán para mostrar las propiedades de los metadatos a los usuarios en la pantalla de detalles de recursos de la opción [!UICONTROL Formularios de metadatos], en [!DNL Settings]. Consulte [Formularios de metadatos](metadata.md#metadata-forms).
* Varias correcciones de errores y mejoras del producto, incluido un mejor rendimiento al cargar una carpeta anidada con muchas subcarpetas.

### Versión 2021.6.0 {#june2021}

La primera versión de [!DNL Assets Essentials], que se publicó el 21 de junio de 2021, ofrece funciones de administración de recursos ligeras. Admite las siguientes funciones principales y operaciones CRUD (crear, leer, actualizar y eliminar):

* Cargue y añada recursos, incluidas carpetas anidadas. Previsualice los recursos y las versiones.
* Búsqueda de texto completo, filtros de búsqueda con matices y búsquedas guardadas para una detección rápida de recursos.
* Operaciones básicas de administración de recursos como actualizar, eliminar, descargar y administrar metadatos.
* [!DNL Assets Essentials] está disponible para los usuarios de [!DNL Adobe Journey Optimizer] para administrar los recursos al crear mensajes. Para obtener más información, consulte [Integraciones con otras soluciones de Adobe](/help/integration.md).
