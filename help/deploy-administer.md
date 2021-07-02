---
title: Implementar y administrar usuarios
description: Casos de uso de administración, como la implementación y la administración de usuarios en [!DNL Assets Essentials].
role: Administrator
source-git-commit: 6e482854e7cec3d8bc2fed786a2c6a685b3f8eed
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 2%

---


# Implementar [!DNL Assets Essentials] y agregar usuarios {#administer}

[!DNL Adobe Experience Manager Assets Essentials] está aprovisionado por Adobe para sus clientes. Como parte del aprovisionamiento, [!DNL Assets Essentials] se agrega a la organización de un cliente (organización de Adobe). El cliente también tiene acceso a [!DNL Experience Manager Cloud Manager] como herramienta de implementación y a [!DNL Admin Console] como herramienta de administración de usuarios.

Los administradores realizan las siguientes tareas:

* [ [!DNL Assets Essentials]](#deploy-essentials) Implementación para su organización.
* [Administre el ](#add-users-to-essentials) acceso de usuario de los miembros de la organización a  [!DNL Assets Essentials].
* De forma opcional, [vea el estado del servicio y los registros](#view-logs).

## Implementar [!DNL Assets Essentials] {#deploy-essentials}

Después del aprovisionamiento, se agrega el derecho [!DNL Assets Essentials] a la organización de Adobe y el administrador de una organización lo implementa. Los administradores de la organización realizan una implementación única utilizando la interfaz de usuario [!DNL Cloud Manager] . Después de la implementación inicial, Adobe realiza el mantenimiento y las actualizaciones del servicio. Para implementar, siga estos pasos:

1. Asegúrese de que el administrador recibe un correo electrónico del Adobe. El correo electrónico contiene un mensaje de bienvenida y un vínculo para empezar.

1. Desde el vínculo del correo electrónico, acceda a [Admin Console](https://adminconsole.adobe.com) e inicie sesión en él. Si tiene acceso de administrador a más de una cuenta de organización, seleccione la organización adecuada o cambie a ella con el conmutador de la barra superior. La tarjeta del producto para [!DNL Assets Essentials] se puede ver en [!DNL Admin Console].

   ![[!DNL Assets Essentials] tarjeta en  [!DNL Admin Console]](assets/essentials-in-admin-console.png)

   *Figura:  [!DNL Assets Essentials] en  [!DNL Admin Console].*

1. Añádese como administrador al producto `AEM Assets Essentials - Cloud Manager` en el [!DNL Cloud Manager]. En lugar de usted mismo, puede agregar otro miembro de su organización o puede agregar más de un administrador.

1. Haga clic en ![agregar icono](assets/do-not-localize/add-icon.svg) a [!UICONTROL Select product profiles] y, a continuación, seleccione [!UICONTROL Deployment Manager - Assets Essentials] como **[!UICONTROL product profile]**. El usuario añadido en este paso recibe un correo electrónico del Adobe con acceso a [!DNL Cloud Manager] y puede realizar la implementación.

   ![Añadir un administrador y seleccionar un perfil de producto en  [!DNL Admin Console]](assets/adminconsole-user1.png)

   *Figura: Añada un administrador y seleccione un perfil de producto en  [!DNL Admin Console].*

1. Para acceder a [!DNL Cloud Manager], haga clic en el vínculo del correo electrónico con acceso a [!DNL Cloud Manager]. También puede acceder a `https://experience.adobe.com/#/cloud-manager/` en su explorador.

1. En la interfaz de usuario de Cloud Manager, haga clic en **[!UICONTROL Add Program]** en la esquina superior derecha.

1. Proporcione un nombre de su elección y, opcionalmente, cargue una imagen (representa el programa en [!DNL Cloud Manager]) y, a continuación, haga clic en **[!UICONTROL Create]**. [!DNL Cloud Manager] tarda unos minutos en configurar el programa.

1. Cuando el programa esté listo, pase el puntero sobre el mosaico y haga clic en ![agregar icono de entorno](assets/do-not-localize/add-environment-icon.png).

1. Para agregar [!DNL Assets Essentials] servicio a su organización, haga clic en **[!UICONTROL Add Environment]**, seleccione un nombre y una región de implementación y haga clic en **[!UICONTROL Save]**. No puede cambiar la región de implementación más adelante. Intente hacer coincidir la región de implementación de [!DNL Assets Essentials] con la región de implementación de la otra solución con la que desea utilizar [!DNL Assets Essentials]. La coincidencia es garantizar el acceso de red más rápido posible a los recursos digitales y la menor latencia posible.

   ![Añadir un entorno en  [!DNL Cloud Manager]](assets/cloudmanager-add-environment-for-essentials.png)

   *Figura: Agregue un entorno en  [!DNL Cloud Manager] para empezar a usar  [!DNL Assets Essentials].*

1. Cuando el entorno se crea correctamente, puede acceder a [!DNL Admin Console] y agregar los usuarios de su organización a la solución [!DNL Assets Essentials]. Haga clic en ![options icon](assets/do-not-localize/options-ellipses-icon.png) y seleccione la opción **[!UICONTROL Manage Access]**.

   ![Entorno listo en  [!DNL Cloud Manager]](assets/cloudmanager-manage-access-essentials.png)

   *Figura: Un entorno en  [!DNL Cloud Manager] que esté listo para usar.*

## Administración de usuarios {#add-users-to-essentials}

Un administrador gestiona qué usuarios tienen acceso a [!DNL Assets Essentials]. Los administradores utilizan [!DNL Adobe Admin Console] para agregar o eliminar el acceso de los usuarios. [!DNL Assets Essentials] tiene disponibles los dos tipos siguientes de acceso de usuario.

* **[!DNL Assets Essentials]** Los usuarios tienen acceso a la interfaz de usuario completa. Estos usuarios pueden cargar, organizar, etiquetar y encontrar recursos digitales.
* **[!DNL Assets Essentials]Usuarios consumidores**: tienen acceso a la experiencia de selección de recursos incrustados en el editor de plantillas de  [!DNL Adobe Journey Optimizer] correo electrónico. Para obtener más información, consulte [Usar [!DNL Assets Essentials] en [!DNL Journey Optimizer]](https://experienceleague.adobe.com/docs/journey-optimizer/using/create-messages/assets-essentials.html).

En [!DNL Admin Console], estos dos tipos de acceso están representados por dos [!UICONTROL Product Profiles]. Para agregar y eliminar miembros de su organización a cualquiera de los dos perfiles, siga estos pasos:

1. Acceda a [!DNL Admin Console] para su organización, haga clic en **[!UICONTROL Products]** en la barra superior, haga clic en **[!UICONTROL AEM Assets Essentials]** y, a continuación, haga clic en [!DNL Assets Essentials] entorno. [!DNL Assets Essentials] tiene dos perfiles de producto que representan el acceso para los usuarios normales y los consumidores.

   ![Dos perfiles para dos tipos de usuarios](assets/adminconsole-user-types.png)

   *Figura: Hay dos perfiles disponibles para agregar los dos tipos de usuarios.*

1. Para agregar un usuario a un grupo, haga clic en el grupo, seleccione **[!UICONTROL Add User]**, proporcione los detalles del usuario y haga clic en **[!UICONTROL Save]**. Cuando agrega un usuario, el usuario recibe una invitación por correo electrónico para comenzar. Puede desactivar las invitaciones por correo electrónico en la configuración del perfil del producto en [!DNL Admin Console].

   ![Agregar un usuario a  [!DNL Assets Essentials]](assets/adminconsole-add-user.png)

   *Figura: Agregue un usuario a  [!DNL Assets Essentials] desde  [!DNL Admin Console].*

1. Para quitar un usuario de un grupo, haga clic en el grupo, seleccione un usuario existente y seleccione **[!UICONTROL Remove User]**.

>[!TIP]
>
>En [!DNL Admin Console], puede administrar los usuarios de forma masiva mediante archivos CSV. Para obtener más información, consulte [[!DNL Admin Console] documentación](https://helpx.adobe.com/enterprise/using/accounts.html).

## Ver el estado del servicio y los registros de acceso {#view-logs}

Después del aprovisionamiento, los administradores implementan [!DNL Assets Essentials] solo una vez. Después de la implementación inicial, Adobe realiza el mantenimiento y las actualizaciones del servicio. Los administradores pueden utilizar la interfaz de usuario [!DNL Cloud Manager] para comprobar el estado del servicio y descargar los registros de acceso recientes.

1. Cuando los usuarios informan de problemas, compruebe el estado del servicio de [!DNL Assets Essentials] en la interfaz **[!UICONTROL Program Overview]**. Durante el funcionamiento normal de la solución, el estado es `Running`. Si [!DNL Cloud Manager] muestra cualquier otro estado, cree un ticket de soporte en la sección de soporte [!DNL Admin Console].

   ![El estado de  [!DNL Assets Essentials] en  [!DNL Cloud Manager]](assets/cloudmanager-manage-access-essentials.png)

   *Figura: El estado normal de  [!DNL Assets Essentials] en  [!DNL Cloud Manager] es  `Running`.*

1. Para descargar los registros de acceso recientes, haga clic en ![icono de opciones](assets/do-not-localize/options-ellipses-icon.png), seleccione **[!UICONTROL Download Logs]** y siga las instrucciones que aparecen en la pantalla. Puede auditar las solicitudes de acceso HTTPS mediante los registros.

   ![ Opción para descargar los registros de acceso](assets/cloudmanager-download-logs.png)

   *Figura: Opción para descargar los registros de acceso.*

>[!MORELIKETHIS]
>
>* [[!DNL Admin Console] ayuda](https://helpx.adobe.com/enterprise/using/admin-console.html)
>* [[!DNL Cloud Manager] ayuda](https://experienceleague.adobe.com/docs/experience-manager-cloud-manager/using/introduction-to-cloud-manager.html?lang=es)
>* [Documentación de Adobe Journey Optimizer](https://experienceleague.adobe.com/docs/journey-optimizer/using/ajo-home.html)
>* [Notas de versión](release-notes.md)
* [Introducción a [!DNL Assets Essentials]](get-started.md)

