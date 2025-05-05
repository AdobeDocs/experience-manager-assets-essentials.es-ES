---
title: Integración de Content credentials
description: Los contentes credentials, integrados en AEM Assets y presentados en la interfaz de usuario de AEM Assets Essentials, pueden ofrecer contexto en el historial de un recurso, incluido cómo se creó y quién participó en su creación. Al igual que una etiqueta nutricional para el contenido digital, los Contentes credentials pueden ayudar a aumentar la transparencia y generar confianza con las audiencias.
role: User
source-git-commit: bb7a86c737f862411e2f06997d8b4d720d55a3c5
workflow-type: tm+mt
source-wordcount: '463'
ht-degree: 0%

---


# Credenciales de contenido {#content-credentials}

Las marcas están más preocupadas que nunca por la transparencia del contenido, la divulgación de la inteligencia artificial y la prevención de la manipulación de activos. La Iniciativa de autenticidad de contenido (CAI) del Adobe crea herramientas que cumplen con el estándar técnico de la [Coalición para la procedencia y autenticidad de contenido](https://c2pa.org/specifications/specifications/1.1/specs/C2PA_Specification.html#_trust_model) (C2PA). Los contentes credentials, que son un nuevo tipo de metadatos cifrados y a prueba de manipulaciones, pueden ayudar a los espectadores a comprender el linaje del contenido y garantizar la integridad de los recursos de la marca. Pueden incluir una amplia gama de datos de procedencia que ofrecen una perspectiva del historial de un recurso digital.

Esta información incluye:

* **Emisor o firmante:** Información acerca de la entidad o compañía que emitió la firma digital para certificar los certificados o firmas del recurso.
* **Fecha del problema:** Fecha en la que se aplicó la credencial de contenido al recurso.
* **Crédito y uso:** Información sobre el productor del recurso, incluidos el nombre, los identificadores de medios sociales u otra información relacionada con la identidad.
* **Proceso:** Registra las ediciones o modificaciones realizadas en el recurso.
* **Detalles del dispositivo:** Información sobre la aplicación o el dispositivo usado para crear o editar el recurso.
* **Herramienta de IA utilizada:** Si se utilizó IA generativa para editar o crear el recurso, se puede incluir el nombre del modelo utilizado.
* **Otra información relevante:** También se pueden incluir datos adicionales para ayudar a ofrecer más contexto sobre el historial de un recurso.

Para obtener una vista completa, [Verify](https://contentcredentials.org/verify) puede ofrecer una perspectiva más completa del historial de recursos.

Adobe Experience Manager Assets ahora es compatible con los Contentes credentials, lo que permite a los usuarios ver los Contentes credentials directamente en la interfaz de usuario de los Assets Essentials AEM de la interfaz de usuario de la interfaz de usuario de la interfaz de usuario de. Al observar los detalles del recurso, cualquier imagen con Contentes credentials (como las creadas con los servicios GenAI) muestra los detalles del manifiesto en un panel específico. Si el recurso se descarga, publica o comparte, las credenciales permanecen intactas con el recurso.

![recursos](/help/using/assets/content-credentials.png)

## Contentes credentials de acceso {#access-content-credentials}

1. Vaya a la interfaz de usuario de Assets Essentials y haga clic en **Assets** en el panel izquierdo.
1. Vaya a una carpeta y seleccione el recurso que desee.
1. Haga clic en **Detalles** y seleccione `Cr pin` en el panel situado más a la derecha. La pestaña Contentes credentials muestra la siguiente información sobre el recurso.
   1. **Imagen generada:** Fecha y hora de aplicación de los Contentes credentials.
   1. **Resumen de contenido:** Indica si AI ha generado el recurso parcial o totalmente, o cómo se ha editado.

      ![resumen de contenido](/help/using/assets/content-credentials1.png)
   1. **Proceso:** detalla la aplicación, el dispositivo y la herramienta de IA (como el Adobe Firefly) que se usó para generar el recurso, así como los cambios realizados posteriormente.

      ![proceso](/help/using/assets/CR-Process.png)
   1. **Acerca de estos Contentes credentials:** Nombre del emisor junto con la fecha y hora de emisión.

      ![emisor](/help/using/assets/CR-issuer.png)