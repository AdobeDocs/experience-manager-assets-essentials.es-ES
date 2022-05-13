---
title: Configuración de Assets Essentials para Creative Cloud Pro con soluciones de administración de trabajo
description: 'Este tutorial presenta un recorrido de administrador para permitir que la aplicación de Assets Essentials se integre con las aplicaciones de escritorio de Creative Cloud y con la aplicación de Adobe Workfront. Las aplicaciones de escritorio de Creative Cloud incluyen Adobe Photoshop, Adobe Illustrator, Adobe InDesign y Adobe XD. '
source-git-commit: f4e56fc6bb76eeb2770b18be88b7da1a1829069c
workflow-type: tm+mt
source-wordcount: '900'
ht-degree: 12%

---


# Assets Essentials para Creative Cloud Pro con soluciones de administración de trabajo {#creative-cloud-enterprise-user-journeys}

![Preferencia para cambiar el tema oscuro y el claro](assets/cce-next-banner-landing-page.png)

## Introducción {#introduction}

Creative Cloud Pro para empresas con soluciones de administración del trabajo integra herramientas creativas, de contenido y de administración del trabajo para aumentar su capacidad de producir contenido creativo y lograr rápidamente los objetivos empresariales. La solución incluye los siguientes componentes:

* Creative Cloud Pro

* Adobe Workfront

* Experience Manager Assets Essentials

Este tutorial presenta un recorrido de administrador para permitir que la aplicación de Assets Essentials se integre con las aplicaciones de escritorio de Creative Cloud y con la aplicación de Adobe Workfront. Las aplicaciones de escritorio de Creative Cloud incluyen Adobe Photoshop, Adobe Illustrator, Adobe InDesign y Adobe XD.

## Tipos de implementación {#deployment-types}

Como la solución está formada por aplicaciones y servicios tanto de Creative Cloud como de Adobe Experience Cloud, se pueden implementar en uno o dos Admin Console de Adobe para su empresa.

En caso de implementación en dos Admin Console, se requiere un paso de configuración adicional:

* Los servicios y las aplicaciones de Creative Cloud (Creative Cloud para enterprise Pro y módulos opcionales) se administran en [Adobe Admin Console para su implementación de Creative Cloud](https://chl-author-preview.corp.adobe.com/content/help/en/enterprise/admin-guide.html).

* Adobe Workfront y Adobe Experience Manager Assets Essentials se administran en [Adobe Admin Console para soluciones de Experience Cloud](https://experienceleague.adobe.com/docs/core-services/interface/administration/admin-getting-started.html).

Para integrar aplicaciones de Creative Cloud y Assets Essentials, los usuarios disponibles en Admin Console para Creative Cloud deben estar disponibles en Admin Console para Experience Cloud. Para que los usuarios estén disponibles en el Admin Console del Experience Cloud, cree un directorio para establecer [confianza de directorios](https://helpx.adobe.com/enterprise/using/set-up-identity.html#directory-trusting) entre las dos consolas de administración.

![Usuarios de Creative Cloud](assets/creative-cloud-users.svg)

Como se muestra en el diagrama, los usuarios del Creative Cloud están disponibles automáticamente en el Admin Console del Experience Cloud en función de una relación de confianza entre las dos consolas. A continuación, puede agregar los usuarios a los perfiles de producto de Assets Essentials. Como resultado, los usuarios Creative Cloud pueden acceder a la aplicación Adobe Asset Link que puede interactuar con el repositorio de Assets Essentials. Para obtener más información, consulte [Integración de Assets Essentials con aplicaciones de Creative Cloud](integrate-assets-essentials-creative-cloud.md).

## recorridos de documentación del Experience Manager {#documentation-journeys}

Un Recorrido de documentación vincula muchos temas y características diferentes y tal vez complejos al proporcionar una narrativa que ayuda al lector, que puede ser nuevo en Assets Essentials, a comprender y resolver un problema comercial de principio a fin, mientras asume un conocimiento previo mínimo del tema o Assets Essentials.

Los Recorridos de documentación están diseñados en torno a los principios de las prácticas recomendadas, basados en las últimas investigaciones de Adobe, la experiencia de implementación comprobada de los consultores de Adobe y los comentarios de los proyectos de los clientes.

## Requisitos previos

* [Acceso a Adobe Admin Console para soluciones de Experience Cloud](https://experienceleague.adobe.com/docs/core-services/interface/administration/admin-getting-started.html)

* [Acceso a Adobe Admin Console para Creative Cloud para la implementación empresarial](https://helpx.adobe.com/enterprise/admin-guide.html)

## Administrar Experience Manager Assets Essentials {#administer-assets-essentials}

![Preferencia para cambiar el tema oscuro y el claro](assets/cce-assets.png)

Adobe Experience Manager Assets Essentials es una nueva edición ligera de Adobe Experience Manager Assets. Assets Essentials proporciona una colaboración y administración unificadas de recursos con una interfaz de usuario simplificada y coherente. La facilidad de uso permite que equipos más creativos y de marketing almacenen, descubran y distribuyan recursos digitales.

Adobe Experience Manager Assets Essentials se aprovisiona por Adobe para sus clientes. Como parte del aprovisionamiento, Assets Essentials se añade a la organización de un cliente en Adobe Admin Console.

Los administradores utilizan el Admin Console para administrar las autorizaciones de usuario para el producto de Assets Essentials:

* Adición de grupos de usuarios

* Agregar usuarios a grupos de usuarios

* Agregar usuarios a perfiles de producto de Assets Essentials

Después de administrar las autorizaciones de usuario en Admin Console, los administradores pueden utilizar la aplicación de Assets Essentials para:

* Cree una estructura de carpetas para satisfacer mejor las necesidades de la organización

* Administrar permisos a la estructura de carpetas

* Configuración de formularios de metadatos

[![Véase la Guía](https://helpx.adobe.com/content/dam/help/en/marketing-cloud/how-to/digital-foundation/_jcr_content/main-pars/image_1250343773/see-the-guide-sm.png)](adminster-aem-assets-essentials.md)

## Integración de aplicaciones de Creative Cloud con Experience Manager Assets Essentials {#administer-creative-cloud-applications}

![Preferencia para cambiar el tema oscuro y el claro](assets/cce-creative-cloud.png)

[Panel en la aplicación de vínculo de recursos de Adobe](https://www.adobe.com/creativecloud/business/enterprise/adobe-asset-link.html) permite a los profesionales creativos conectarse a [!DNL Assets Essentials] repositorio desde el [!DNL Adobe Creative Cloud] aplicaciones de escritorio. El panel está disponible para [!DNL Adobe Photoshop], [!DNL Adobe Illustrator], [!DNL Adobe InDesign] y [!DNL Adobe XD]. Simplifica el acceso a los recursos, lo que a su vez aumenta la velocidad de contenido.

Este tutorial le guía para integrar [!DNL Adobe Photoshop], [!DNL Adobe Illustrator], [!DNL Adobe InDesign]y [!DNL Adobe XD] aplicaciones con Experience Manager Assets Essentials.

Objetivos:

* Creación de la confianza de directorios entre Admin Console Creative Cloud y Experience Cloud

* Agregar usuarios de Creative Cloud a perfiles de producto de Assets Essentials

* Instalación de Asset Link de Adobe

* Uso del vínculo de recursos de Adobe

[![Véase la Guía](https://helpx.adobe.com/content/dam/help/en/marketing-cloud/how-to/digital-foundation/_jcr_content/main-pars/image_1250343773/see-the-guide-sm.png)](integrate-assets-essentials-creative-cloud.md)

## Integrar Adobe Workfront con Experience Manager Assets Essentials {#administer-adobe-workfront}

![Preferencia para cambiar el tema oscuro y el claro](assets/cce-workfront.png)

[[!DNL Adobe Workfront]](https://www.workfront.com/) es una aplicación de administración de trabajo que le ayuda a administrar todo el ciclo de vida del trabajo en un solo lugar. La integración nativa entre [!DNL Adobe Workfront] y [!DNL Assets Essentials] permite a las organizaciones mejorar la velocidad de contenido y el tiempo de salida al mercado al conectar intrínsecamente el trabajo con la administración de recursos. En el contexto de la administración de su trabajo, los usuarios tienen acceso a los documentos e imágenes necesarios en la misma solución.

Este tutorial le guía para administrar Adobe Workfront y luego integrarlo con Experience Manager Assets Essentials.

Objetivos:

* Agregar usuarios a perfiles de producto de Workfront

* Agregar usuarios a perfiles de producto de Assets Essentials

* Configuración de la integración de Experience Manager Assets Essentials

[![Véase la Guía](https://helpx.adobe.com/content/dam/help/en/marketing-cloud/how-to/digital-foundation/_jcr_content/main-pars/image_1250343773/see-the-guide-sm.png)](integrate-assets-essentials-workfront.md)


