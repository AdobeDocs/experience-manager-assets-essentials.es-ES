---
title: Integración de Assets Essentials con Adobe Workfront
description: Integre Assets Essentials con la aplicación Adobe Workfront para que pueda acceder al repositorio de Assets Essentials dentro de la aplicación Workfront.
source-git-commit: 7d49060ba2e02bd9c5caf9753ef56b5feed5b3df
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 19%

---


# Integración de Assets Essentials con Adobe Workfront {#integrate-assets-essentials-workfront}

![Preferencia para cambiar el tema oscuro y el claro](assets/cce-workfront.png)

## La historia hasta ahora

Después [configuración de Experience Manager Assets Essentials](adminster-aem-assets-essentials.md) y [integración de las aplicaciones Creative Cloud con Assets Essentials](integrate-assets-essentials-creative-cloud.md), puede continuar integrando la aplicación de Adobe Workfront con Assets Essentials.

## Objetivo

* **Audiencia**: Administradores de Adobe Workfront

* **Objetivo**: Integre Assets Essentials con la aplicación Adobe Workfront para que pueda acceder al repositorio de Assets Essentials dentro de la aplicación Workfront.

## Información general

[[!DNL Adobe Workfront]](https://www.workfront.com/) es una aplicación de administración de trabajo que le ayuda a administrar todo el ciclo de vida del trabajo en un solo lugar. La integración nativa entre [!DNL Adobe Workfront] y [!DNL Assets Essentials] permite a las organizaciones mejorar la velocidad de contenido y el tiempo de salida al mercado al conectar intrínsecamente el trabajo con la administración de recursos. En el contexto de la administración de su trabajo, los usuarios tienen acceso a los documentos e imágenes necesarios en la misma solución.

Ejecute las siguientes tareas para integrar Workfront con Experience Manager Assets Essentials:

* [Agregar usuarios a perfiles de producto de Workfront](#add-users-to-product-profiles)

* [Agregar usuarios a perfiles de producto de Assets Essentials](#add-workfront-users-assets-essentials-product-profiles)

* [Configuración de la integración de Experience Manager Assets Essentials](#configure-assets-essentials-integration)

## Agregar usuarios a perfiles de producto de Workfront {#add-users-to-product-profiles}

Para agregar usuarios a perfiles de producto de Workfront:

1. Acceso [Admin Console](https://adminconsole.adobe.com) para su organización, haga clic en **[!UICONTROL Productos]** en la barra superior, haga clic en **[!UICONTROL Workfront]** y haga clic en la primera instancia de la lista. No haga clic en la segunda y tercera instancias de la lista.

   ![Perfil de administrador de Admin Console](assets/workfront-instances.png)

   Admin Console muestra el único perfil de producto disponible.

1. Para agregar un usuario a un perfil de producto, haga clic en el perfil y luego en **[!UICONTROL Agregar usuario]**, proporcione los detalles del usuario y haga clic en **[!UICONTROL Guardar]**.

   ![Adición de perfil de administrador de usuarios](assets/add-users-workfront.png)

   Cuando añade un usuario, este recibe una invitación por correo electrónico para comenzar. Puede desactivar las invitaciones por correo electrónico en la configuración del perfil de producto en [!DNL Admin Console].

1. Para quitar un usuario de un grupo, haga clic en el grupo, seleccione un usuario existente y seleccione **[!UICONTROL Eliminar usuario]**.

Para obtener más información sobre cómo crear usuarios y administradores de sistemas en Workfront con Adobe Admin Console, consulte [Administrar usuarios en Adobe Admin Console](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FCreate_and_manage_users%2Fadmin-console.htm&amp;_LANG=enus).

## Agregar usuarios a perfiles de producto de Assets Essentials {#add-workfront-users-assets-essentials-product-profiles}

Asigne los usuarios de Workfront a uno de los siguientes perfiles de producto de Assets Essentials:

* **[!DNL Assets Essentials]Usuarios** tienen acceso a la interfaz de usuario completa de Assets Essentials. Estos usuarios pueden cargar, organizar, etiquetar y encontrar recursos digitales en la aplicación Assets Essentials. Además, los usuarios tienen acceso a la experiencia de selección de recursos incrustados en [!DNL Adobe Workfront] aplicación.
* **[!DNL Assets Essentials]Usuarios consumidores**: tener acceso a la experiencia de selección de recursos incrustados en [!DNL Adobe Workfront] aplicación.

Para obtener más información sobre cómo asignar usuarios a perfiles de producto de Assets Essentials, consulte [Asignación de usuarios a perfiles de producto de Assets Essentials](adminster-aem-assets-essentials.md#add-users-to-product-profiles).

## Configuración de la integración de Experience Manager Assets Essentials {#configure-assets-essentials-integration}

Después de agregar usuarios a los perfiles de producto de Workfront y Assets Essentials mediante el Admin Console, puede [configuración de la integración de Experience Manager Assets Essentials](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FDocuments%2FAdobe_Workfront_for_Experience_Manager_Assets_Essentials%2F_workfront-for-aem-asset-essentials.htm).

Después de configurar la integración, puede:

* [Vincular recursos y carpetas desde Experience Manager Assets Essentials](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FDocuments%2FAdobe_Workfront_for_Experience_Manager_Assets_Essentials%2Flink-to-aem.htm&amp;_LANG=enus)

* [Enviar un documento a Experience Manager Assets Essentials](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FDocuments%2FAdobe_Workfront_for_Experience_Manager_Assets_Essentials%2Fsend-to-aem.htm&amp;_LANG=enus)

* [Probar un recurso vinculado para Experience Manager Assets Essentials](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FDocuments%2FAdobe_Workfront_for_Experience_Manager_Assets_Essentials%2Fproof-linked-asset-aem.htm)

* [Ver o descargar un recurso vinculado desde Experience Manager Assets Essentials](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FDocuments%2FAdobe_Workfront_for_Experience_Manager_Assets_Essentials%2Fview-download-asset.htm)
