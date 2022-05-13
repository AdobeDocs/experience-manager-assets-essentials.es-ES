---
title: Integración de Assets Essentials con aplicaciones de Creative Cloud
description: Integre Assets Essentials con aplicaciones de Creative Cloud para que pueda utilizar el panel integrado de vínculos de recursos de Adobe para conectarse a [!DNL Assets Essentials] repositorio desde el [!DNL Adobe Creative Cloud] aplicaciones de escritorio.
source-git-commit: f4e56fc6bb76eeb2770b18be88b7da1a1829069c
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 4%

---


# Integración de Assets Essentials con aplicaciones de Creative Cloud {#integrate-assets-essentials-creative-cloud-applications}

![Preferencia para cambiar el tema oscuro y el claro](assets/cce-creative-cloud.png)

## La historia hasta ahora

Después [configuración de Experience Manager Assets Essentials](adminster-aem-assets-essentials.md) en este tutorial, puede aprovechar la experiencia para integrar las aplicaciones de Creative Cloud con Assets Essentials.

## Objetivo

* **Audiencia**: Administradores Creative Cloud

* **Objetivo**: Integre Assets Essentials con aplicaciones de Creative Cloud para que sus usuarios creativos puedan utilizar el panel integrado de vínculos de Adobe Asset para conectarse a [!DNL Assets Essentials] repositorio desde el [!DNL Adobe Creative Cloud] aplicaciones de escritorio.

## Información general

[Panel en la aplicación de vínculo de recursos de Adobe](https://www.adobe.com/creativecloud/business/enterprise/adobe-asset-link.html) permite a los profesionales creativos conectarse a [!DNL Assets Essentials] repositorio desde el [!DNL Adobe Creative Cloud] aplicaciones de escritorio. El panel está disponible para [!DNL Adobe Photoshop], [!DNL Adobe Illustrator], [!DNL Adobe InDesign] y [!DNL Adobe XD]. Simplifica el acceso a los recursos, lo que a su vez ayuda a aumentar la velocidad de contenido.

Los usuarios de la aplicación de Creative Cloud solo pueden usar el panel en la aplicación de Asset Link de Adobe cuando integren las aplicaciones de Creative Cloud con el repositorio de Experience Manager Assets Essentials.

Ejecute las siguientes tareas para integrar Assets Essentials con aplicaciones de Creative Cloud:

* [Creación de la confianza de directorios entre el Creative Cloud y el Admin Console del Experience Cloud](#directory-trusting-cc-assets-essentials-consoles)

* [Agregar usuarios de Creative Cloud a perfiles de producto de Assets Essentials](#add-cc-users-assets-essentials-product-profiles)

* [Instalación de Asset Link de Adobe](#install-asset-link)

* [Uso del vínculo de recursos de Adobe](#use-asset-link)

## Creación de la confianza de directorios entre Admin Console Creative Cloud y Experience Cloud {#directory-trusting-cc-assets-essentials-consoles}

Si el Creative Cloud se implementa en una Consola de administración de Adobe independiente de la que se utiliza con Assets Essentials (solución de Experience Cloud), debe agregar una relación de confianza entre las dos consolas.

Para integrar aplicaciones de Creative Cloud y Assets Essentials, los usuarios disponibles en Admin Console para Creative Cloud deben estar disponibles en Admin Console para Experience Cloud. Si Creative Cloud y Assets Essentials se implementan en Admin Console separados, se requiere una relación de confianza entre ellos para habilitar esto.

En el Admin Console del Experience Cloud, haga clic en **[!UICONTROL Configuración]** y utilice el **[!UICONTROL Directorios]** pestaña para crear un directorio para establecer [confianza de directorios](https://helpx.adobe.com/enterprise/using/set-up-identity.html#directory-trusting) entre los dos Admin Console.

## Agregar usuarios de Creative Cloud a perfiles de producto de Assets Essentials {#add-cc-users-assets-essentials-product-profiles}

Después de establecer la confianza de directorios entre el Admin Console del Creative Cloud y el Admin Console del Experience Cloud, asigne los usuarios del Creative Cloud al **[!DNL Assets Essentials]Usuarios** perfil de producto en [!DNL Assets Essentials] tarjeta de producto en el Admin Console del Experience Cloud. Permitirá a los usuarios Creative Cloud acceder a Assets Essentials desde su panel de complementos de Asset Link de Adobe; además, les permitirá acceder a la interfaz de usuario web completa de Assets Essentials para cargar, organizar, etiquetar y buscar recursos digitales mediante un explorador web.

Otros perfiles de producto de Assets Essentials: **[!DNL Assets Essentials]Administradores** y **[!DNL Assets Essentials]Usuarios consumidores** : se utilizan para diferentes derechos de usuario (administradores de aplicaciones y usuarios que acceden a Assets Essentials a través de integraciones de Experience Cloud).

Para obtener más información sobre cómo asignar usuarios a perfiles de producto de Assets Essentials, consulte [Asignación de usuarios a perfiles de producto de Assets Essentials](adminster-aem-assets-essentials.md#add-users-to-product-profiles).

## Instalación de Asset Link de Adobe {#install-asset-link}

[!DNL Adobe Asset Link] el complemento se puede instalar y poner a disposición de los usuarios creativos de dos formas:

* Los usuarios creativos pueden instalar el complemento desde sus [!DNL Creative Cloud Desktop] aplicación
* El administrador de Creative Cloud puede agregar el complemento Asset Link a un paquete de Creative Cloud en Admin Console

La elección depende de las políticas de TI de la organización.

**Instalación mediante [!DNL Creative Cloud Desktop] aplicación** se describe [here](https://helpx.adobe.com/creative-cloud/kb/installingextensionsandaddons.html). Hay dos complementos disponibles y alojados en [Adobe Exchange](https://exchange.adobe.com/) mercado, según la aplicación de Creative Cloud:

* Para [!DNL Adobe Photoshop], [!DNL Adobe Illustrator]y [!DNL Adobe InDesign]: [Adobe Asset Link CEP](https://exchange.adobe.com/creativecloud.details.106875.adobe-asset-link-cep.html)
* Para [!DNL Adobe XD]: [Vínculo de recurso de Adobe](https://exchange.adobe.com/creativecloud/plugindetails.html/app/cc/61d229b9)

**Instalación con un paquete de Creative Cloud** lo realiza el administrador Creative Cloud en Admin Console, incluyendo el complemento Asset Link al crear un paquete de implementación, que luego se puede implementar en los equipos de usuario. En la pantalla Elegir complementos administrada, busque **Vínculo de recurso de Adobe** en el **Complementos comerciales destacados** para obtener más información. Para obtener más información, consulte [empaquetar aplicaciones a través del Admin Console](https://helpx.adobe.com/enterprise/using/package-apps-admin-console.html).

## Uso del vínculo de recursos de Adobe {#use-asset-link}

Los usuarios creativos ahora pueden utilizar Adobe Asset Link con Photoshop, Illustrator, InDesign o XD. Para abrir el panel en InDesign o Illustrator, vaya a Windows > Extensiones > Adobe Asset Link. En Photoshop, vaya a Ventana > Extensiones (heredadas) > Adobe Asset Link.

Para obtener información sobre cómo configurar Adobe Asset Link para Adobe XD, haga clic en [here](https://helpx.adobe.com/enterprise/using/adobe-asset-link-for-xd.html).

>[!NOTE]
>
>Cuando se trabaja con hardware Apple Silicon / M1, Adobe Photoshop debe iniciarse usando el modo de compatibilidad con Rosetta para garantizar que los usuarios creativos tengan acceso al panel Adobe Asset Link, ya que está construido con la tecnología de extensión CEP. Para obtener más información, consulte [Photoshop para Apple Silicon](https://helpx.adobe.com/photoshop/kb/photoshop-for-apple-silicon.html).


Utilice Adobe Asset Link para trabajar con los recursos almacenados en el repositorio de Assets Essentials y modificarlos. Puede realizar varias tareas, como:

* Buscar y examinar recursos

* Carga de recursos

* Ordenar y filtrar recursos

* Colocar, descargar y arrastrar un recurso

* Desproteger y proteger un recurso

* Ver el historial de versiones y los detalles de archivos

Para obtener instrucciones sobre cómo realizar estas tareas, consulte [Administrar recursos mediante el vínculo de recursos de Adobe](https://helpx.adobe.com/in/enterprise/using/manage-assets-using-adobe-asset-link.html).

## Siguientes pasos

Ahora que ha integrado las aplicaciones de Creative Cloud con Assets Essentials, [integrar Adobe Workfront con Experience Manager Assets Essentials](integrate-assets-essentials-workfront.md).
