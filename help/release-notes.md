---
title: Notas de la versión
description: Notas de la versión y problemas conocidos de [!DNL Assets Essentials]
role: User,Leader,Admin,Architect,Developer
contentOwner: AG
source-git-commit: eda2ba0d271310d0e87f904dc7622583a80d002e
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 1%

---


# Notas de la versión de [!DNL Assets Essentials] {#release-notes}

La versión actual de [!DNL Assets Essentials] se publicó el 30 de agosto de 2021. Proporciona integraciones con [!DNL Adobe Workfront] que permiten a los usuarios [!DNL Workfront] administrar sus recursos digitales en el contexto de la administración de su trabajo. Consulte [integraciones con otras soluciones de Adobe](/help/integration.md).

Para obtener más información sobre la solución, consulte la [introducción a [!DNL Assets Essentials]](introduction.md). Para empezar a usar las funciones, consulte [Introducción](/help/get-started.md).

## Problemas conocidos {#known-issues}

La lista de problemas conocidos de la oferta [!DNL Assets Essentials] se revisa y actualiza de forma continua:

* Para cargar una carpeta o recursos, cuando arrastra los elementos a una carpeta con subcarpetas en el repositorio, la carga se envía automáticamente a una de las subcarpetas. La solución es hacer clic en la opción [!DNL Upload assets] y arrastrarla al cuadro de diálogo. <!-- CQ-4327753 -->
* Después de cargar la carpeta, a veces las nuevas carpetas pueden aparecer incorrectamente en el carril izquierdo en lugar de mostrarse en la vista de árbol. La solución es actualizar el explorador. <!-- CQ-4323534 -->

<!--
* Use assets that do not have whitespace in the file names. The replies to comments do not work for such assets.
-->

Si encuentra algún problema o incluso solicitudes de mejora, [proporcione comentarios](#provide-feedback) al equipo.

## Versiones anteriores {#past-release}

### Versión 2021.7.0 {#july2021}

[!DNL Assets Essentials] La versión 2021.7.0 se publicó el 29 de julio de 2021, con las siguientes actualizaciones:

* Puede crear y administrar formularios de metadatos personalizados que se utilizarán para mostrar las propiedades de los metadatos a los usuarios en la pantalla de detalles del recurso, en la opción [!UICONTROL Metadata Forms] de [!DNL Settings]. Consulte [formularios de metadatos](metadata.md#metadata-forms).
* Varias correcciones de errores y mejoras del producto, incluido un mejor rendimiento al cargar una carpeta anidada con muchas subcarpetas.

### Versión 2021.6.0 {#june2021}

La primera versión de [!DNL Assets Essentials], disponible el 21 de junio de 2021, ofrece funciones de administración de recursos ligeras. Admite las siguientes funciones principales y operaciones CRUD (crear, leer, actualizar y eliminar):

* Cargue y agregue recursos, incluidas carpetas anidadas. Obtenga una vista previa de los recursos y las versiones.
* Búsqueda de texto completo, filtros de búsqueda con matices y búsquedas guardadas para una detección rápida de recursos.
* Operaciones básicas de administración de recursos como actualizar, eliminar, descargar y administrar metadatos.
* [!DNL Assets Essentials] está disponible para  [[!DNL Adobe Journey Optimizer]](https://experienceleague.adobe.com/docs/journey-optimizer/using/create-messages/assets-essentials.html).
