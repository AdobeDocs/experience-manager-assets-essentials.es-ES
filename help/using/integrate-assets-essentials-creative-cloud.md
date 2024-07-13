---
title: Integración de Assets Essentials con aplicaciones de Creative Cloud
description: Integre Assets Essentials con aplicaciones de Creative Cloud para poder utilizar el panel integrado de Adobe Asset Link para conectarse al repositorio de  [!DNL Assets Essentials]  desde las aplicaciones de  [!DNL Adobe Creative Cloud]  de escritorio admitidas.
exl-id: 611fd958-3fd3-4c46-bee9-8b866b7dc208
source-git-commit: 65200f73a954e4ebf4fbd6dc3a819acc6e0beda4
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 100%

---

# Integración de Assets Essentials con aplicaciones de Creative Cloud {#integrate-assets-essentials-creative-cloud-applications}

![Preferencia para cambiar el tema oscuro y el claro](assets/cce-creative-cloud.png)

## La historia hasta ahora

Después de [configurar Experience Manager Assets Essentials](adminster-aem-assets-essentials.md) en este tutorial, puede aprovechar la experiencia para integrar las aplicaciones de Creative Cloud con Assets Essentials.

## Objetivo

* **Audiencia**: administradores de Creative Cloud

* **Objetivo**: integrar Assets Essentials con aplicaciones de Creative Cloud para que sus usuarios creativos puedan utilizar el panel integrado de Adobe Asset Link para conectarse al repositorio de [!DNL Assets Essentials] desde las aplicaciones de escritorio de [!DNL Adobe Creative Cloud] admitidas.

## Información general

El [panel integrado de Adobe Asset Link](https://www.adobe.com/es/creativecloud/business/enterprise/adobe-asset-link.html) permite a los profesionales creativos conectarse al repositorio de [!DNL Assets Essentials] desde las aplicaciones de escritorio de [!DNL Adobe Creative Cloud] admitidas. El panel está disponible para [!DNL Adobe Photoshop], [!DNL Adobe Illustrator], [!DNL Adobe InDesign] y [!DNL Adobe XD]. Simplifica el acceso a los recursos, lo que a su vez aumenta la velocidad del contenido.

Los usuarios de la aplicación de Creative Cloud solo pueden usar el panel en la aplicación de Adobe Asset Link cuando integren las aplicaciones de Creative Cloud con el repositorio de Experience Manager Assets Essentials.

Ejecute las siguientes tareas para integrar Assets Essentials con aplicaciones de Creative Cloud:

* [Cree un apoderamiento de directorios entre Creative Cloud y Admin Console de Experience Cloud](#directory-trusting-cc-assets-essentials-consoles)

* [Añada usuarios de Creative Cloud a perfiles de producto de Assets Essentials](#add-cc-users-assets-essentials-product-profiles)

* [Instale Adobe Asset Link](#install-asset-link)

* [Use Adobe Asset Link](#use-asset-link)

## Cree confianza de directorios entre Creative Cloud y Admin Consoles de Experience Cloud {#directory-trusting-cc-assets-essentials-consoles}

Si Creative Cloud se implementa en Adobe Admin Console independiente de la que se utiliza con Assets Essentials (solución de Experience Cloud), debe añadir una relación de confianza entre las dos consolas.

Para integrar aplicaciones de Creative Cloud y Assets Essentials, los usuarios disponibles en la Admin Console para Creative Cloud deben estar disponibles en la Admin Console para Experience Cloud. Si Creative Cloud y Assets Essentials se implementan en Admin Consoles separadas, se requiere una relación de confianza entre ellas para habilitar esto.

En la Admin Console de Experience Cloud, haga clic en **[!UICONTROL Configuración]** y utilice la pestaña **[!UICONTROL Directorios]** para crear un directorio y establecer una [confianza de directorios](https://helpx.adobe.com/es/enterprise/using/set-up-identity.html#directory-trusting) entre las dos Admin Consoles.

## Añada usuarios de Creative Cloud a perfiles de producto de Assets Essentials {#add-cc-users-assets-essentials-product-profiles}

Después de establecer la confianza de directorios entre la Admin Console de Creative Cloud y la de Experience Cloud, asigne los usuarios de Creative Cloud al perfil de producto **[!DNL Assets Essentials]Usuarios** en la tarjeta de producto de [!DNL Assets Essentials] en Admin Console de Experience Cloud. Permitirá a los usuarios de Creative Cloud acceder a Assets Essentials desde su panel de complementos de Adobe Asset Link; además, les permitirá acceder a la interfaz de usuario web completa de Assets Essentials para cargar, organizar, etiquetar y buscar recursos digitales mediante un explorador web.

Otros perfiles de producto de Assets Essentials: los Administradores de **[!DNL Assets Essentials]** y los Usuarios consumidores de **[!DNL Assets Essentials]** se utilizan para diferentes derechos de usuario (administradores y usuarios de aplicaciones que acceden a Assets Essentials a través de integraciones de Experience Cloud).

Para obtener más información sobre cómo asignar usuarios a perfiles de producto de Assets Essentials, consulte [Asignación de usuarios a perfiles de producto de Assets Essentials](adminster-aem-assets-essentials.md#add-users-to-product-profiles).

## Instale Adobe Asset Link {#install-asset-link}

El complemento [!DNL Adobe Asset Link] se puede instalar y poner a disposición de los usuarios creativos de dos formas:

* Los usuarios creativos pueden instalar el complemento desde su aplicación [!DNL Creative Cloud Desktop]
* El administrador de Creative Cloud puede añadir el complemento Asset Link a un paquete de Creative Cloud en Admin Console

La elección depende de las políticas de TI de la organización.

**La instalación mediante la aplicación de [!DNL Creative Cloud Desktop]** se describe [aquí](https://helpx.adobe.com/es/creative-cloud/kb/installingextensionsandaddons.html). Hay dos complementos disponibles y alojados en el Marketplace de [Adobe Exchange](https://exchange.adobe.com/), según la aplicación de Creative Cloud:

* Para [!DNL Adobe Photoshop], [!DNL Adobe Illustrator] y [!DNL Adobe InDesign]: [Adobe Asset Link CEP](https://exchange.adobe.com/creativecloud.details.106875.adobe-asset-link-cep.html)
* Para [!DNL Adobe XD]: [Adobe Asset Link](https://exchange.adobe.com/creativecloud/plugindetails.html/app/cc/61d229b9)

La **instalación con un paquete de Creative Cloud** la lleva a cabo el administrador de Creative Cloud en Admin Console, incluyendo el complemento Asset Link al crear un paquete de implementación, que luego se puede implementar en los equipos de usuario. En la pantalla Elegir complementos administrada, busque **Adobe Asset Link** en la sección **Complementos comerciales destacados**. Para obtener más información, consulte [Empaquetado de aplicaciones a través de Admin Console](https://helpx.adobe.com/es/enterprise/using/package-apps-admin-console.html).

## Use Adobe Asset Link {#use-asset-link}

Los usuarios creativos ahora pueden utilizar Adobe Asset Link con Photoshop, Illustrator, InDesign o XD. Para abrir el panel en InDesign o Illustrator, vaya a Windows > Extensiones > Adobe Asset Link. En Photoshop, vaya a Ventana > Extensiones (heredadas) > Adobe Asset Link.

Para obtener información sobre cómo configurar Adobe Asset Link para Adobe XD, haga clic [aquí](https://helpx.adobe.com/es/enterprise/using/adobe-asset-link-for-xd.html).

>[!NOTE]
>
>Cuando se trabaja con hardware Apple Silicon/M1, Adobe Photoshop debe iniciarse usando el modo de compatibilidad con Rosetta para garantizar que los usuarios creativos tengan acceso al panel Adobe Asset Link, ya que está construido con la tecnología de extensión CEP. Para obtener más información, consulte [Photoshop para Apple Silicon](https://helpx.adobe.com/es/photoshop/kb/photoshop-for-apple-silicon.html).


Utilice Adobe Asset Link para trabajar con los recursos almacenados en el repositorio de Assets Essentials y modificarlos. Puede llevar a cabo varias tareas, como las siguientes:

* Buscar y examinar recursos

* Carga de recursos

* Ordenar y filtrar recursos

* Colocar, descargar y arrastrar un recurso

* Desproteger y proteger un recurso

* Ver el historial de versiones y los detalles del archivo

Para obtener instrucciones sobre cómo llevar a cabo estas tareas, consulte [Administración de recursos mediante Adobe Asset Link](https://helpx.adobe.com/es/enterprise/using/manage-assets-using-adobe-asset-link.html).

## Siguientes pasos

Ahora que ha integrado las aplicaciones de Creative Cloud con Assets Essentials, [integre Adobe Workfront con Experience Manager Assets Essentials](integrate-assets-essentials-workfront.md).
