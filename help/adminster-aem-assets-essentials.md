---
title: Administrar Experience Manager Assets Essentials
description: Configure el acceso a la aplicación de Assets Essentials mediante el Admin Console y, a continuación, administre las tareas que se pueden realizar después de iniciar sesión en la aplicación de Assets Essentials.
source-git-commit: 1f01dd340f79d1c2d9748232c2b1a589ae7f8545
workflow-type: tm+mt
source-wordcount: '1399'
ht-degree: 53%

---


# Administrar Experience Manager Assets Essentials {#administer-assets-essentials}

![Preferencia para cambiar el tema oscuro y el claro](assets/cce-assets.png)

## Objetivo

* **Audiencia**: Administradores de Assets Essentials

* **Objetivo**: Configure el acceso a la aplicación de Assets Essentials mediante el Admin Console y, a continuación, administre las tareas que se pueden realizar después de iniciar sesión en la aplicación de Assets Essentials.

## Información general {#overview}


[!DNL Adobe Experience Manager Assets Essentials] está aprovisionado por Adobe para sus clientes. Como parte del aprovisionamiento, [!DNL Assets Essentials] se añade a la organización de un cliente en [!DNL Adobe Admin Console]. Los administradores utilizan [!DNL Admin Console] para administrar las autorizaciones de usuario a [!DNL Assets Essentials] y asignar administradores de aplicaciones para configurar permisos y formularios de metadatos en [!DNL Assets Essentials].

El siguiente diagrama de flujo de datos ilustra la secuencia de tareas que un administrador debe realizar para configurar y administrar Assets Essentials:

![Flujo de administración de Assets Essentials](assets/permissions-management-cce-next.svg)

## Acceso al Admin Console {#access-admin-console}

Una vez aprovisionada la solución de Assets Essentials, el administrador recibe un correo electrónico de Adobe. El correo electrónico contiene un mensaje de bienvenida y un vínculo para empezar. Además, Adobe inicia el proceso para implementar Assets Essentials automáticamente. El proceso de implementación tarda una hora en completarse.

Desde el vínculo del correo electrónico, acceda a [Admin Console](https://adminconsole.adobe.com) e inicie sesión. Si tiene acceso de administrador a más de una cuenta de organización, seleccione la organización adecuada o cambie a ella mediante el [selector de organización](https://helpx.adobe.com/es/enterprise/using/admin-console.html). Una vez completado el proceso de implementación automática, la tarjeta de producto de [!DNL AEM Assets Essentials] es visible en [!DNL Admin Console].

![Implementación de Assets Essentials](assets/admin-console-cards.png)

## Administrar tareas de Admin Console {#manage-admin-console-tasks}

Realice las siguientes tareas en Admin Console:

* [Agregar usuarios a perfiles de producto](#add-users-to-product-profiles)

* [Adición de grupos de usuarios](#add-user-groups)

* [Adición de usuarios a grupos](#add-users-to-user-groups)

### Agregar usuarios a perfiles de producto {#add-users-to-product-profiles}

Agregue usuarios a perfiles de producto para que tengan acceso a la aplicación Assets Essentials.

Para agregar usuarios a perfiles de producto:

1. Acceso [Admin Console](https://adminconsole.adobe.com) para su organización, haga clic en **[!UICONTROL Productos]** en la barra superior, haga clic en **[!UICONTROL AEM Assets Essentials]** y, a continuación, haga clic en la instancia de [!DNL Assets Essentials]. El nombre de la instancia puede ser diferente al de la captura de pantalla siguiente.
   >[!NOTE]
   >
   >[!DNL Cloud Manager] es para uso especial de administrador, como comprobar el estado del servicio y obtener acceso a los registros del servicio, y no se puede utilizar para agregar usuarios al producto. Para obtener más información, consulte [guía de administración](deploy-administer.md#view-service-status-and-access-logs-view-logs).

   ![Perfil de administrador de Admin Console](assets/assets-essentials-instance.png)

   [!DNL Assets Essentials] tiene tres perfiles de producto que representan el acceso para los usuarios normales y consumidores y los administradores.

   ![Perfil de administrador de Admin Console](assets/admin-console-admin-profile.png)

1. Para agregar un usuario al producto, haga clic en uno de los tres perfiles de producto de Assets Essentials, seleccione **[!UICONTROL Agregar usuario]**, proporcione los detalles del usuario y haga clic en **[!UICONTROL Guardar]**.

   ![Adición de perfil de administrador de usuarios](assets/add-users-admin-profile.png)

   Cuando añade un usuario, este recibe una invitación por correo electrónico para comenzar. Puede desactivar las invitaciones por correo electrónico en la configuración del perfil de producto en [!DNL Admin Console].

1. Para quitar un usuario de un grupo, haga clic en el grupo, seleccione un usuario existente y seleccione **[!UICONTROL Eliminar usuario]**.

   >[!NOTE]
   >
   >Debe añadir un usuario al perfil de producto de Assets Essentials Administrator en el Admin Console para que pueda realizar tareas administrativas en la aplicación Assets Essentials. Estas tareas incluyen [Crear estructura de carpetas](#create-folder-structure), [Administrar permisos para carpetas](#manage-permissions-for-folders)y [Configuración de metadatos de Forms](#metadata-forms).

### Adición de grupos de usuarios {#add-user-groups}

Cree grupos de usuarios y luego asigne los usuarios a los grupos de usuarios. Estos grupos de usuarios estarán disponibles en la aplicación Assets Essentials para establecer permisos en las carpetas.

Puede añadir usuarios a grupos de usuarios (1) y [a perfiles de producto de Assets Essentials (2)](#add-admin-users). Sin embargo, no puede agregar grupos de usuarios directamente a los perfiles de producto de Assets Essentials (3).

![Adición de usuarios a grupos y perfiles de producto](assets/user-groups-product-profiles.svg)

Para obtener información sobre cómo administrar grupos de usuarios, consulte `Create user groups` y `Edit user groups`, disponibles en [Administración de grupos de usuarios](https://helpx.adobe.com/es/enterprise/using/user-groups.html).

>[!NOTE]
>
>Si Admin Console está configurada para aprovechar un sistema externo para administrar asignaciones de usuarios/grupos, como conectores de Azure o Google, la herramienta de sincronización de usuarios o la API de REST de User Management, los grupos y las asignaciones de usuarios se configuran automáticamente. Para obtener más información, consulte [Usuarios de Adobe Admin Console](https://helpx.adobe.com/es/enterprise/using/users.html).


### Adición de usuarios a grupos {#add-users-to-user-groups}

Después de crear grupos de usuarios, puede empezar a añadirles usuarios.

Para obtener información sobre cómo administrar la adición de usuarios a grupos de usuarios, consulte `Add users to groups`, disponible en [Administración de grupos de usuarios](https://helpx.adobe.com/es/enterprise/using/user-groups.html#add-users-to-groups).

## Administración de tareas de administración de Assets Essentials {#manage-assets-essentials-tasks}

Después de realizar las tareas de Admin Console, ahora puede realizar las siguientes tareas de administración en la aplicación Assets Essentials:

* [Creación de estructura de carpetas](#create-folder-structure)

* [Administración de permisos para carpetas](#manage-permissions-for-folders)

* [Configuración de metadatos de Forms](#metadata-forms)

>[!NOTE]
>
>Para poder administrar estas tareas, especialmente la administración de permisos, el usuario debe tener derechos de administración de aplicaciones; debe añadirse al [Perfil de producto Assets Essentials del administrador](#add-users-to-product-profiles).


### Creación de estructura de carpetas {#create-folder-structure}

Puede utilizar los siguientes métodos para crear una estructura de carpetas en el repositorio de Assets Essentials:

* Haga clic en la opción **[!UICONTROL Crear carpeta]**, disponible en la barra de herramientas, para crear una carpeta vacía.

* Haga clic en la opción **[!UICONTROL Añadir recursos]**, disponible en la barra de herramientas, para [cargar una estructura de carpetas disponible en el equipo local](add-delete.md).

Cree una estructura de carpetas que funcione bien con los objetivos empresariales de la organización. Si está cargando una estructura de carpetas existente en el repositorio de Assets Essentials, debe revisar la estructura. Para obtener más información, consulte [Prácticas recomendadas para la administración eficaz de permisos](permission-management-best-practices.md).

Tenga en cuenta los siguientes puntos cuando empiece a planificar la creación de una estructura de carpetas en el repositorio de Assets Essentials:

* Gobernanza futura: las carpetas controladas por los administradores y las [delegadas con permisos a otros usuarios como propietarios](manage-permissions.md##manage-permissions-folders).

* Escalable: la estructura de carpetas debe ajustarse a las necesidades futuras de su organización y ser fácilmente escalable.

* Tamaño: una carpeta no debe contener demasiados recursos. Esto puede conllevar problemas de uso y puede resultar difícil de administrar.

* Intuitiva: la estructura de carpetas debería ser fácil de examinar e intuitiva para los usuarios finales. Los usuarios deben poder identificar con facilidad dónde cargar un nuevo recurso en la estructura de carpetas.

Existen varios tipos de estructura de carpetas que puede utilizar para su organización. A continuación, se muestran algunos ejemplos de estructuras de carpetas típicas:

![Estructuras de carpeta típicas](assets/folder-structure.svg)

### Administración de permisos para carpetas {#manage-permissions-for-folders}

Assets Essentials permite a los administradores administrar los niveles de acceso para las carpetas disponibles en el repositorio. Como administrador, puede crear grupos de usuarios y asignar permisos a esos grupos para administrar los niveles de acceso. También puede delegar los privilegios de administración de permisos a grupos de usuarios en el nivel de carpeta.

>[!VIDEO](https://video.tv.adobe.com/v/341104)

Para obtener más información, consulte [Administrar permisos para carpetas](manage-permissions.md).

### Configuración de metadatos de Forms {#metadata-forms}

Assets Essentials proporciona muchos campos de metadatos estándar de forma predeterminada. Las organizaciones tienen requisitos de metadatos adicionales y necesitan más campos para agregar los específicos de su empresa. Los formularios de metadatos permiten a las empresas añadir campos de metadatos personalizados a la página [!UICONTROL Detalles] de un recurso. Los metadatos específicos de la empresa mejoran el control y el descubrimiento de sus recursos. Puede crear formularios desde cero o reutilizar uno existente.

Puede configurar formularios de metadatos para diferentes tipos de recursos (diferentes tipos de MIME). Utilice el mismo nombre de formulario que el tipo MIME del archivo. Essentials coincide automáticamente con el tipo MIME de los recursos cargados con el nombre del formulario y actualiza los metadatos de los recursos cargados en función de los campos del formulario.

Por ejemplo, si un formulario de metadatos por el nombre `PDF` o `pdf` existe, los documentos de PDF cargados contienen campos de metadatos tal como se definen en el formulario.

Assets Essentials utiliza la siguiente secuencia para buscar nombres de formulario de metadatos existentes para aplicar los campos de metadatos a los recursos cargados de un tipo en particular:

Subtipo MIME > Tipo MIME > `default` formulario > Formulario predeterminado

Por ejemplo, si existe un formulario de metadatos con el nombre `PDF` o `pdf`, los documentos PDF cargados contienen campos de metadatos tal como se definen en el formulario. Si un formulario de metadatos por el nombre `PDF` o `pdf` no existe, Assets Essentials coincide si hay un formulario de metadatos por nombre `application`. Si hay un formulario de metadatos por el nombre `application`, los documentos del PDF cargados contienen campos de metadatos tal como se definen en el formulario. Si Assets Essentials sigue sin encontrar un formulario de metadatos coincidente, busca la variable `default` formulario de metadatos para aplicar campos de metadatos definidos en el formulario a los documentos de PDF cargados. Si ninguno de estos pasos funciona, Assets Essentials aplica campos de metadatos definidos en el formulario predeterminado a todos los documentos de PDF cargados.

>[!IMPORTANT]
>
>El nuevo formulario de metadatos para un tipo de archivo específico reemplaza completamente el formulario de metadatos predeterminado que [!DNL Assets Essentials] proporciona. Si elimina o cambia el nombre de un formulario de metadatos, los campos de metadatos predeterminados volverán a estar disponibles para los nuevos recursos.

>[!VIDEO](https://video.tv.adobe.com/v/341275)

Para obtener más información sobre Metadata Forms, consulte [Metadatos de Forms en Assets Essentials](metadata.md#metadata-forms).

## Siguientes pasos

Ahora que ha configurado y administrado la aplicación de Assets Essentials, [integrar aplicaciones de Creative Cloud con la aplicación Experience Manager Assets Essentials](integrate-assets-essentials-creative-cloud.md).

