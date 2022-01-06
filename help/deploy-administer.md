---
title: Implementar y administrar usuarios
description: Casos de uso de administración, como la implementación y la administración de usuarios en [!DNL Assets Essentials].
role: Admin
exl-id: ef91126f-3aee-442b-b242-a6bf4034f3dc
source-git-commit: cbf75aaf05a0f3d798edf4d508325b28d9ca0dcb
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 1%

---

# Implementación [!DNL Assets Essentials] y agregar usuarios {#administer}

[!DNL Adobe Experience Manager Assets Essentials] está aprovisionado por Adobe para sus clientes. Como parte del aprovisionamiento, [!DNL Assets Essentials] se agrega a la organización de un cliente en [!DNL Adobe Admin Console]. Los clientes también tienen acceso a [!DNL Experience Manager Cloud Manager] como herramienta de implementación y para [!DNL Admin Console] para administrar las autorizaciones de usuario a [!DNL Assets Essentials] solución.

## Implementación automática de Assets Essentials {#automatic-deployment-assets-essentials}

Una vez aprovisionada la solución de Assets Essentials, el administrador recibe un correo electrónico del Adobe. El correo electrónico contiene un mensaje de bienvenida y un vínculo para empezar. Además, Adobe inicia el proceso para implementar Assets Essentials automáticamente. El proceso de implementación tarda una hora en completarse.

Desde el vínculo del correo electrónico, acceda a y inicie sesión en [Admin Console](https://adminconsole.adobe.com). Si tiene acceso de administrador a más de una cuenta de organización, seleccione la organización adecuada o cambie a ella con el conmutador de la barra superior. Una vez completado el proceso de implementación automática, la tarjeta de producto de [!DNL AEM Assets Essentials] es visible en la variable [!DNL Admin Console].

![Implementación de Assets Essentials](assets/assets-essentials-deployment.png)

Los administradores deben realizar las siguientes tareas después de implementar correctamente la solución Assets Essentials:

* [Administrar el acceso del usuario](#add-users-to-essentials) de los miembros de la organización a [!DNL Assets Essentials].
* Opcionalmente, [ver el estado y los registros del servicio](#view-logs).

>[!NOTE]
>
>Si Assets Essentials está aprovisionado antes del 06 de enero de 2022, ejecute el [pasos de implementación en Cloud Manager](#deploy-essentials) antes de administrar el acceso de los usuarios de los miembros de la organización.


## Administración de usuarios {#add-users-to-essentials}

Un administrador gestiona a qué usuarios tiene acceso [!DNL Assets Essentials]. Los administradores utilizan [!DNL Adobe Admin Console] para agregar o quitar el acceso del usuario. [!DNL Assets Essentials] tiene disponibles los dos tipos siguientes de acceso de usuario.

* **[!DNL Assets Essentials]Usuarios** tienen acceso a la interfaz de usuario completa. Estos usuarios pueden cargar, organizar, etiquetar y encontrar recursos digitales.
* **[!DNL Assets Essentials]Usuarios consumidores**: tener acceso a la experiencia de selección de recursos incrustados en [!DNL Adobe Journey Optimizer] editor de plantillas de correo electrónico. Para obtener más información, consulte [Uso [!DNL Assets Essentials] en [!DNL Journey Optimizer]](https://experienceleague.adobe.com/docs/journey-optimizer/using/create-messages/assets-essentials.html).

En [!DNL Admin Console], estos dos tipos de acceso están representados por dos [!UICONTROL Product Profiles]. Para agregar y eliminar miembros de su organización a cualquiera de los dos perfiles, siga estos pasos:

1. Acceso [!DNL Admin Console] para su organización, haga clic en **[!UICONTROL Products]** en la barra superior, haga clic en **[!UICONTROL AEM Assets Essentials]** y, a continuación, haga clic en [!DNL Assets Essentials] entorno. [!DNL Assets Essentials] tiene dos perfiles de producto que representan el acceso para los usuarios normales y los consumidores.

   ![Dos perfiles para dos tipos de usuarios](assets/adminconsole-user-types.png)

   *Figura: Hay dos perfiles disponibles para agregar los dos tipos de usuarios.*

1. Para agregar un usuario a un grupo, haga clic en el grupo y seleccione **[!UICONTROL Add User]**, proporcione los detalles del usuario y haga clic en **[!UICONTROL Save]**. Cuando agrega un usuario, el usuario recibe una invitación por correo electrónico para comenzar. Puede desactivar las invitaciones por correo electrónico en la configuración del perfil del producto en [!DNL Admin Console].

   ![Agregar un usuario a [!DNL Assets Essentials]](assets/adminconsole-add-user.png)

   *Figura: Agregar un usuario a [!DNL Assets Essentials] from [!DNL Admin Console].*

1. Para quitar un usuario de un grupo, haga clic en el grupo, seleccione un usuario existente y seleccione **[!UICONTROL Remove User]**.

>[!TIP]
>
>En [!DNL Admin Console], puede administrar los usuarios de forma masiva mediante archivos CSV. Para obtener más información, consulte [[!DNL Admin Console] documentación](https://helpx.adobe.com/enterprise/using/accounts.html).

## Ver el estado del servicio y los registros de acceso {#view-logs}

Después del aprovisionamiento, los administradores implementan [!DNL Assets Essentials] solo una vez. Después de la implementación inicial, Adobe realiza el mantenimiento y las actualizaciones del servicio. Los administradores pueden usar la variable [!DNL Cloud Manager] para comprobar el estado del servicio y descargar los registros de acceso recientes.

1. Cuando los usuarios informan de problemas, compruebe el estado de servicio de [!DNL Assets Essentials] en el **[!UICONTROL Program Overview]** interfaz. Durante el funcionamiento normal de la solución, el estado es `Running`. If [!DNL Cloud Manager] muestra cualquier otro estado, cree un ticket de asistencia en el [!DNL Admin Console] sección de soporte técnico.

   ![El estado de [!DNL Assets Essentials] en [!DNL Cloud Manager]](assets/cloudmanager-manage-access-essentials.png)

   *Figura: El estado normal de [!DNL Assets Essentials] en [!DNL Cloud Manager] es `Running`.*

1. Para descargar los registros de acceso recientes, haga clic en ![icono de opciones](assets/do-not-localize/options-ellipses-icon.png), seleccione **[!UICONTROL Download Logs]** y siga las instrucciones que aparecen en la pantalla. Puede auditar las solicitudes de acceso HTTPS mediante los registros.

   ![ Opción para descargar los registros de acceso](assets/cloudmanager-download-logs.png)

   *Figura: Opción para descargar los registros de acceso.*

## Implementar [!DNL Assets Essentials] {#deploy-essentials}

>[!NOTE]
>
>Ejecute estos pasos solo si Assets Essentials está aprovisionado antes del 6 de enero de 2022.

Después del aprovisionamiento, [!DNL Assets Essentials] se añade a su organización en [!DNL Admin Console]. Antes de que la solución esté disponible para el usuario, un administrador de la organización debe implementarla. El administrador realiza una implementación única utilizando [!DNL Cloud Manager] interfaz de usuario. Después de la implementación inicial, Adobe realiza el mantenimiento y las actualizaciones del servicio. Una vez aprovisionada la solución, el administrador recibe un correo electrónico del Adobe. El correo electrónico contiene un mensaje de bienvenida y un vínculo para empezar. Para implementar, siga estos pasos:

1. Desde el vínculo del correo electrónico, acceda a y inicie sesión en [Admin Console](https://adminconsole.adobe.com). Si tiene acceso de administrador a más de una cuenta de organización, seleccione la organización adecuada o cambie a ella con el conmutador de la barra superior. La tarjeta de producto para [!DNL Assets Essentials] es visible en la variable [!DNL Admin Console].

   ![[!DNL Assets Essentials] tarjeta en [!DNL Admin Console]](assets/essentials-in-admin-console.png)

   *Figura: [!DNL Assets Essentials] tarjeta en [!DNL Admin Console].*

   >[!NOTE]
   >
   >Si puede ver la **[!UICONTROL AEM Assets Essentials]** en la sección de productos en lugar de **[!UICONTROL AEM Assets Essentials - Cloud Manager]** , la implementación de Assets Essentials ya ha finalizado. Puede omitir los pasos restantes.

1. Agregue como administrador a `AEM Assets Essentials - Cloud Manager` perfil de producto en la variable [!DNL Admin Console]. En lugar de usted mismo, puede agregar otro miembro de su organización o puede agregar más de un administrador.

1. Haga clic en ![agregar icono](assets/do-not-localize/add-icon.svg) a [!UICONTROL Select product profiles]y, a continuación, seleccione [!UICONTROL Deployment Manager - Assets Essentials] como el **[!UICONTROL product profile]**. El usuario añadido en este paso recibe un correo electrónico del Adobe con acceso a [!DNL Cloud Manager] y pueden realizar la implementación.

   ![Añadir un administrador y seleccionar un perfil de producto en [!DNL Admin Console]](assets/adminconsole-user1.png)

   *Figura: Añadir un administrador y seleccionar un perfil de producto en [!DNL Admin Console].*

1. Para acceder a [!DNL Cloud Manager], haga clic en el vínculo del correo electrónico con acceso a [!DNL Cloud Manager]. También puede acceder a [https://experience.adobe.com/#/cloud-manager/](https://experience.adobe.com/#/cloud-manager/) en su navegador.

1. En la interfaz de usuario de Cloud Manager, haga clic en **[!UICONTROL Add Program]** desde la esquina superior derecha.

1. Proporcione un nombre de su elección y, opcionalmente, cargue una imagen (representa el programa en [!DNL Cloud Manager]) y, a continuación, haga clic en **[!UICONTROL Create]**. [!DNL Cloud Manager] tarda unos minutos en configurar el programa.

1. Cuando el programa esté listo, pase el puntero sobre el mosaico y haga clic en ![agregar icono de entorno](assets/do-not-localize/add-environment-icon.png).

1. Para agregar [!DNL Assets Essentials] servicio a su organización, haga clic en **[!UICONTROL Add Environment]**, seleccione un nombre y una región de implementación y haga clic en **[!UICONTROL Save]**. No puede cambiar la región de implementación más adelante. Intente coincidir con la región de implementación de [!DNL Assets Essentials] con la región de implementación de la otra solución con la que desea utilizar [!DNL Assets Essentials]. La coincidencia es garantizar el acceso de red más rápido posible a los recursos digitales y la menor latencia posible.

   ![Añadir un entorno en [!DNL Cloud Manager]](assets/cloudmanager-add-environment-for-essentials.png)

   *Figura: Añadir un entorno en [!DNL Cloud Manager] para empezar a usar [!DNL Assets Essentials].*

1. Después de varios minutos, cuando el entorno se crea correctamente, puede acceder a la variable [!DNL Admin Console] y agregar los usuarios de su organización a [!DNL Assets Essentials] solución. Haga clic en ![icono de opciones](assets/do-not-localize/options-ellipses-icon.png) y seleccione **[!UICONTROL Manage Access]** .

   ![Entorno listo en [!DNL Cloud Manager]](assets/cloudmanager-manage-access-essentials.png)

   *Figura: Un entorno en [!DNL Cloud Manager] que está listo para usar.*

>[!MORELIKETHIS]
>
>* [[!DNL Admin Console] ayuda](https://helpx.adobe.com/enterprise/using/admin-console.html)
>* [[!DNL Cloud Manager] ayuda](https://experienceleague.adobe.com/docs/experience-manager-cloud-manager/using/introduction-to-cloud-manager.html?lang=es)
>* [Documentación de Adobe Journey Optimizer](https://experienceleague.adobe.com/docs/journey-optimizer/using/ajo-home.html)
>* [Notas de la versión](release-notes.md)
>* [Introducción a [!DNL Assets Essentials]](get-started.md)

