---
title: Administración y administración de usuarios
description: Casos de uso de administración, como la implementación y la administración de usuarios en [!DNL Assets Essentials].
role: Admin
exl-id: ef91126f-3aee-442b-b242-a6bf4034f3dc
source-git-commit: fb4ca5b3ab85f77cc1013c2d4743530f5d48e96d
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 88%

---

# Administración [!DNL Assets Essentials] y agregar usuarios {#administer}

[!DNL Adobe Experience Manager Assets Essentials] está aprovisionado por Adobe para sus clientes. Como parte del aprovisionamiento, [!DNL Assets Essentials] se añade a la organización de un cliente en [!DNL Adobe Admin Console]. Los administradores utilizarán [!DNL Admin Console] para administrar las autorizaciones de usuario a [!DNL Assets Essentials] y asignar administradores de aplicaciones para configurar permisos y formularios de metadatos en [!DNL Assets Essentials].

## Implementación automática de Assets Essentials {#automatic-deployment-assets-essentials}

Una vez aprovisionada la solución de Assets Essentials, el administrador recibe un correo electrónico de Adobe. El correo electrónico contiene un mensaje de bienvenida y un vínculo para empezar. Además, Adobe inicia el proceso para implementar Assets Essentials automáticamente. El proceso de implementación tarda una hora en completarse.

Desde el vínculo del correo electrónico, acceda a [Admin Console](https://adminconsole.adobe.com) e inicie sesión. Si tiene acceso de administrador a más de una cuenta de organización, seleccione la adecuada o cambie a ella con el conmutador de la barra superior. Una vez completado el proceso de implementación automática, la tarjeta de producto de [!DNL AEM Assets Essentials] es visible en [!DNL Admin Console].

![Implementación de Assets Essentials](assets/assets-essentials-deployment.png)

Los administradores deben realizar las siguientes tareas después de implementar correctamente la solución Assets Essentials:

* [Configurar grupos de usuarios, estructura de carpetas y asignar permisos](manage-permissions.md) para la solución. Seguir [prácticas recomendadas](permission-management-best-practices.md) para garantizar una configuración de permisos sencilla y eficaz.
* [Administrar el acceso de usuario](#add-users-to-essentials) de los miembros de la organización a [!DNL Assets Essentials].
* Opcionalmente, [ver el estado del servicio y los registros](#view-logs).

>[!NOTE]
>
>Si Assets Essentials está aprovisionado antes del 6 de enero de 2022, ejecute los [pasos de implementación en Cloud Manager](#deploy-essentials) antes de administrar el acceso de usuario de los miembros de la organización.


## Administración de usuarios {#add-users-to-essentials}

Un administrador gestiona qué usuarios tienen acceso a [!DNL Assets Essentials]. Los administradores utilizan [!DNL Adobe Admin Console] para añadir o quitar el acceso de usuario. [!DNL Assets Essentials] tiene disponibles los dos tipos siguientes de acceso de usuario.

* **[!DNL Assets Essentials]Administradores** tienen acceso administrativo a la aplicación. Además de todas las funcionalidades del usuario final, los administradores de aplicaciones de este grupo pueden administrar permisos para cualquier carpeta y grupo/usuario en todo el repositorio de aplicaciones.
* Los **[!DNL Assets Essentials] usuarios** tienen acceso a la interfaz de usuario completa. Estos usuarios pueden cargar, organizar, etiquetar y encontrar recursos digitales.
* Los **[!DNL Assets Essentials] usuarios consumidores**: tienen acceso a la experiencia de selección de recursos incrustada en el editor de plantillas de correo electrónico de [!DNL Adobe Journey Optimizer]. Para obtener más información, consulte [Uso de [!DNL Assets Essentials] en [!DNL Journey Optimizer]](https://experienceleague.adobe.com/docs/journey-optimizer/using/create-messages/assets-essentials.html?lang=es).

En [!DNL Admin Console], estos tres tipos de acceso están representados por tres [!UICONTROL Perfiles de producto]. Para añadir y eliminar miembros de su organización en cualquiera de los dos perfiles, siga estos pasos:

1. Acceda a la [!DNL Admin Console] para su organización, haga clic en **[!UICONTROL Productos]** en la barra superior, en **[!UICONTROL AEM Assets Essentials]** y, a continuación, en entorno de [!DNL Assets Essentials]. [!DNL Assets Essentials] tiene tres perfiles de producto que representan el acceso de los usuarios administradores, regulares y consumidores.

   ![Tres perfiles para tres tipos de usuarios](assets/admin-console-admin-profile.png)
   <!-- Need to update screenshot to include 3 profiles -->

   *Figura: Hay tres perfiles disponibles para agregar los tres tipos de usuarios.*

1. Para agregar un usuario a un grupo, haga clic en el grupo y seleccione **[!UICONTROL Añadir usuario]**, proporcione sus detalles y haga clic en **[!UICONTROL Guardar]**. Cuando añade un usuario, este recibe una invitación por correo electrónico para comenzar. Puede desactivar las invitaciones por correo electrónico en la configuración del perfil de producto en [!DNL Admin Console].

   ![Adición de un usuario a [!DNL Assets Essentials]](assets/adminconsole-add-user.png)

   *Imagen: adición de un usuario a [!DNL Assets Essentials] desde [!DNL Admin Console].*

1. Para quitar un usuario de un grupo, haga clic en el grupo, seleccione un usuario existente y seleccione **[!UICONTROL Eliminar usuario]**.

>[!TIP]
>
>En [!DNL Admin Console], puede administrar los usuarios por lotes mediante archivos CSV. Para obtener más información, consulte la [[!DNL Admin Console] documentación](https://helpx.adobe.com/es/enterprise/using/accounts.html).

## Visualización del estado del servicio y los registros de acceso {#view-logs}

Después del aprovisionamiento, los administradores implementan [!DNL Assets Essentials] solo una vez. Después de la implementación inicial, Adobe realiza el mantenimiento y las actualizaciones del servicio. Los administradores pueden usar la interfaz de usuario de [!DNL Cloud Manager] para comprobar el estado del servicio y descargar los registros de acceso recientes.

1. Cuando los usuarios informen de problemas, compruebe el estado del servicio de [!DNL Assets Essentials] en la interfaz **[!UICONTROL Información general del programa]**. Durante el funcionamiento normal de la solución, el estado es `Running`. Si [!DNL Cloud Manager] muestra cualquier otro estado, cree un ticket de asistencia en la sección de soporte de [!DNL Admin Console].

   ![El estado de [!DNL Assets Essentials] en [!DNL Cloud Manager]](assets/cloudmanager-manage-access-essentials.png)

   *Imagen: el estado normal de [!DNL Assets Essentials] en [!DNL Cloud Manager] es `Running`.*

1. Para descargar los registros de acceso recientes, haga clic en el ![icono de opciones](assets/do-not-localize/options-ellipses-icon.png), seleccione **[!UICONTROL Descargar registros]** y siga las instrucciones que aparecen en la pantalla. Puede auditar las solicitudes de acceso HTTPS mediante los registros.

   ![ Opción para descargar los registros de acceso](assets/cloudmanager-download-logs.png)

   *Imagen: opción para descargar los registros de acceso.*

## Implementación de [!DNL Assets Essentials] {#deploy-essentials}

>[!NOTE]
>
>Ejecute estos pasos solo si Assets Essentials está aprovisionado antes del 6 de enero de 2022.

Después del aprovisionamiento, el derecho de [!DNL Assets Essentials] se añade a su organización en [!DNL Admin Console]. Antes de que la solución esté disponible para el usuario, un administrador de la organización debe implementarla. El administrador realiza una implementación única utilizando la interfaz de usuario de [!DNL Cloud Manager]. Después de la implementación inicial, Adobe realiza el mantenimiento y las actualizaciones del servicio. Una vez aprovisionada la solución, el administrador recibe un correo electrónico de Adobe. El correo electrónico contiene un mensaje de bienvenida y un vínculo para empezar. Para llevar a cabo la implementación, siga estos pasos:

1. Desde el vínculo del correo electrónico, acceda a [Admin Console](https://adminconsole.adobe.com) e inicie sesión. Si tiene acceso de administrador a más de una cuenta de organización, seleccione la adecuada o cambie a ella con el conmutador de la barra superior. La tarjeta de producto para [!DNL Assets Essentials] puede verse en [!DNL Admin Console].

   Tarjeta de ![[!DNL Assets Essentials] en [!DNL Admin Console]](assets/essentials-in-admin-console.png)

   *Imagen: tarjeta de [!DNL Assets Essentials] en [!DNL Admin Console].*

   >[!NOTE]
   >
   >Si puede ver la tarjeta de **[!UICONTROL AEM Assets Essentials]** en la sección de productos en lugar de la de **[!UICONTROL AEM Assets Essentials: Cloud Manager]**, la implementación de Assets Essentials ya ha finalizado. Puede omitir los pasos restantes.

1. Añádase como administrador al perfil de producto de `AEM Assets Essentials - Cloud Manager` en [!DNL Admin Console]. En vez de a usted mismo, puede agregar a otro miembro de su organización o a más de un administrador.

1. Haga clic en ![añadir icono](assets/do-not-localize/add-icon.svg) para [!UICONTROL Seleccionar perfiles de producto] y, a continuación, seleccione [!UICONTROL Administrador de implementación: Assets Essentials] como el **[!UICONTROL perfil de producto]**. El usuario añadido en este paso recibe un correo electrónico de Adobe con acceso a [!DNL Cloud Manager] y puede llevar a cabo la implementación.

   ![Adición de un administrador y selección de un perfil de producto en [!DNL Admin Console]](assets/adminconsole-user1.png)

   *Imagen: adición de un administrador y selección de un perfil de producto en [!DNL Admin Console].*

1. Para acceder a [!DNL Cloud Manager], haga clic en el vínculo del correo electrónico con acceso a [!DNL Cloud Manager]. También puede acceder a [https://experience.adobe.com/#/cloud-manager/](https://experience.adobe.com/#/cloud-manager/) en su explorador.

1. En la interfaz de usuario de Cloud Manager, haga clic en **[!UICONTROL Añadir programa]** desde la esquina superior derecha.

1. Proporcione un nombre de su elección y, opcionalmente, cargue una imagen (representa el programa en [!DNL Cloud Manager]) y, a continuación, haga clic en **[!UICONTROL Crear]**. [!DNL Cloud Manager] tarda unos minutos en configurar el programa.

1. Cuando el programa esté listo, pase el puntero sobre el mosaico y haga clic en ![Añadir icono de entorno](assets/do-not-localize/add-environment-icon.png).

1. Para agregar el servicio [!DNL Assets Essentials] a su organización, haga clic en **[!UICONTROL Añadir entorno]**, seleccione un nombre y una región de implementación y haga clic en **[!UICONTROL Guardar]**. No puede cambiar la región de implementación más adelante. Intente hacer coincidir la región de implementación de [!DNL Assets Essentials] con la región de implementación de la otra solución con la que desea utilizar [!DNL Assets Essentials]. Esto sirve para garantizar el acceso de red lo más rápido posible a los recursos digitales y la menor latencia posible.

   ![Adición de un entorno en [!DNL Cloud Manager]](assets/cloudmanager-add-environment-for-essentials.png)

   *Imagen: adición de un entorno en [!DNL Cloud Manager] para empezar a usar [!DNL Assets Essentials].*

1. Después de varios minutos, cuando el entorno se haya creado correctamente, puede acceder a [!DNL Admin Console] y añadir los usuarios de su organización a la solución [!DNL Assets Essentials]. Haga clic en el ![icono de opciones](assets/do-not-localize/options-ellipses-icon.png) y seleccione la opción **[!UICONTROL Administrar acceso]**.

   ![Entorno listo en [!DNL Cloud Manager]](assets/cloudmanager-manage-access-essentials.png)

   *Imagen: un entorno en [!DNL Cloud Manager] que está listo para usarse.*

>[!MORELIKETHIS]
>
>* Ayuda de [[!DNL Admin Console] ](https://helpx.adobe.com/es/enterprise/using/admin-console.html)
>* Ayuda de [[!DNL Cloud Manager] ](https://experienceleague.adobe.com/docs/experience-manager-cloud-manager/using/introduction-to-cloud-manager.html?lang=es)
>* [Documentación de Adobe Journey Optimizer](https://experienceleague.adobe.com/docs/journey-optimizer/using/ajo-home.html?lang=es)
>* [Notas de la versión](release-notes.md)
>* [Introducción a [!DNL Assets Essentials]](get-started.md)

