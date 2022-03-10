---
title: Notas de la versión
description: Notas de la versión y problemas conocidos de [!DNL Assets Essentials]
role: User,Leader,Admin,Architect,Developer
contentOwner: AG
exl-id: a0e29eb6-336a-4f78-b7bd-ec1338c86775
source-git-commit: 4cced7aba92fd0f041842e5ef78d02f0a4f7ffe0
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 0%

---

# Notas de la versión de [!DNL Assets Essentials] {#release-notes}

La versión actual de [!DNL Assets Essentials] se publicó el 9 de marzo de 2022. Esta versión proporciona:

* [!DNL Assets Essentials] ahora le permite [generar un vínculo y compartir recursos con partes interesadas externas](share-links-for-assets.md), que no tienen acceso al [!DNL Assets Essentials] aplicación. Puede definir una fecha de caducidad para el vínculo y luego compartirlo con otras personas mediante el método de comunicación que prefiera, como el correo electrónico o los servicios de mensajería. Los destinatarios del vínculo pueden obtener una vista previa de los recursos y descargarlos.

* La variable [!DNL Assets Essentials] ahora incluye [un perfil de producto de administrador](deploy-administer.md#add-users-to-essentials) en Admin Console, además de los perfiles de producto de usuario normales y de consumidor existentes. Un administrador ahora puede asignar otros usuarios al perfil de producto del administrador.

* Assets Essentials ahora permite a los administradores [administrar los niveles de acceso para las carpetas disponibles en el repositorio](manage-permissions.md). Como administrador, puede crear grupos de usuarios y asignar permisos a esos grupos para administrar los niveles de acceso. También puede delegar los privilegios de administración de permisos a grupos de usuarios en el nivel de carpeta.

* Mejoras y correcciones de errores basadas en los comentarios de los clientes.

Además, [!DNL Adobe Asset Link] extensión para Creative Cloud (Photoshop, Illustrator y InDesign) publicada como [nueva versión 3.2](https://exchange.adobe.com/creativecloud.details.106875.adobe-asset-link-cep.html), con mejoras de rendimiento en el tiempo de inicio del panel y en la velocidad de descarga.


## Problemas conocidos {#known-issues}

La lista de problemas conocidos de [!DNL Assets Essentials] oferta se revisa y actualiza de forma continua:

* Ninguno

Si encuentra algún problema o incluso solicitudes de mejora, [proporcionar comentarios](#provide-feedback) al equipo.

## Versiones anteriores {#past-release}

### Versión 2022.1.0 {#january-2022}

[!DNL Assets Essentials] está disponible el 3 de febrero de 2022, con las siguientes actualizaciones:

* Mejoras de rendimiento para [!UICONTROL Crear carpeta] operación. <!-- CQ-4338818 -->

### Versión 2021.11.0 {#november-2021}

[!DNL Assets Essentials] está disponible el 16 de diciembre de 2021, con las siguientes actualizaciones:

* Adobe implementa Assets Essentials automáticamente después de completar el proceso de aprovisionamiento. Los administradores no necesitan realizar pasos adicionales para implementar Assets Essentials mediante [!DNL Cloud Manager] interfaz de usuario. Esta implementación automática estará disponible para los entornos aprovisionados después del 6 de enero de 2022.
* Hay nuevas versiones de los complementos de Creative Cloud que trabajan con Assets Essentials disponibles en Adobe Exchange: [Adobe Asset Link para Adobe XD v 2.1.0](https://exchange.adobe.com/creativecloud/plugindetails.html/app/cc/61d229b9) y [Adobe Asset Link para Photoshop / InDesign / Illustrator v 3.1.65](https://exchange.adobe.com/creativecloud.details.106875.adobe-asset-link-cep.html).
* Varias correcciones de errores y mejoras del producto, incluidos problemas conocidos previos (ahora las carpetas se muestran correctamente en el árbol de navegación izquierdo después de la carga<!-- CQ-4337638 -->, la carga de arrastrar y soltar permite al usuario seleccionar la carpeta actual o cualquier subcarpeta al soltar para la carga<!-- CQ-4327753 -->).

### Versión 2021.8.0 {#august2021}

[!DNL Assets Essentials] La versión 2021.8.0 se publicó el 30 de agosto de 2021, con las siguientes actualizaciones:

* Integraciones con [!DNL Adobe Workfront] that lets [!DNL Workfront] los usuarios administran sus recursos digitales en el contexto de la administración de su trabajo. Para obtener más información, consulte [integraciones con otras soluciones de Adobe](/help/integration.md).

### Versión 2021.7.0 {#july2021}

[!DNL Assets Essentials] La versión 2021.7.0 se publicó el 29 de julio de 2021, con las siguientes actualizaciones:

* Puede crear y administrar formularios de metadatos personalizados que se utilizarán para mostrar las propiedades de los metadatos a los usuarios en la pantalla de detalles de recursos de [!UICONTROL Forms de metadatos] opción bajo [!DNL Settings]. Consulte [formularios de metadatos](metadata.md#metadata-forms).
* Varias correcciones de errores y mejoras del producto, incluido un mejor rendimiento al cargar una carpeta anidada con muchas subcarpetas.

### Versión 2021.6.0 {#june2021}

La primera versión de [!DNL Assets Essentials], disponible el 21 de junio de 2021, ofrece funciones de administración de recursos ligeras. Admite las siguientes funciones principales y operaciones CRUD (crear, leer, actualizar y eliminar):

* Cargue y agregue recursos, incluidas carpetas anidadas. Obtenga una vista previa de los recursos y las versiones.
* Búsqueda de texto completo, filtros de búsqueda con matices y búsquedas guardadas para una detección rápida de recursos.
* Operaciones básicas de administración de recursos como actualizar, eliminar, descargar y administrar metadatos.
* [!DNL Assets Essentials] está disponible para [!DNL Adobe Journey Optimizer] para administrar los recursos al crear mensajes. Para obtener más información, consulte [integraciones con otras soluciones de Adobe](/help/integration.md).
