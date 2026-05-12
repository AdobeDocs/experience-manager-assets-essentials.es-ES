---
title: Integración de Content Credentials
description: Content Credentials, integrado en AEM Assets y destacado en la interfaz de usuario de AEM Assets Essentials, puede ofrecer contexto en el historial de un recurso, incluido cómo se creó y quién participó en su creación. Al igual que una etiqueta nutricional para el contenido digital, Content Credentials puede ayudar a aumentar la transparencia y generar confianza con las audiencias.
role: User
exl-id: 703f74a6-24d4-4181-8174-9ff4a90ee7aa
TQID: https://experienceleague.adobe.com/witCqgAh8EKfD-hdn8efjZ-M4sypX44KB2ELs3ECInI
product_v2: id: fd1f54a9-f50c-467d-8956-cebbaf4f3eb8
feature_v2: id: ec4263d9-bf7c-44c7-b3f1-3e664861c8f2
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
source-git-commit: f026b389ce582ece5d2ca8745d291b1ae50d657e
workflow-type: tm+mt
source-wordcount: 474
ht-degree: 13%

---

# Content Credentials {#content-credentials}

Las marcas están más preocupadas que nunca por la transparencia del contenido, la divulgación de la inteligencia artificial y la prevención de la manipulación de activos. Content Authenticity Initiative (CAI) en Adobe crea herramientas compatibles con el estándar técnico de [Coalición para la procedencia y autenticidad del contenido](https://c2pa.org/specifications/specifications/1.1/specs/C2PA_Specification.html#_trust_model) (C2PA). Credenciales de contenido, un nuevo tipo de metadatos cifrados y a prueba de manipulaciones, puede ayudar a los visores a comprender el linaje del contenido y garantizar la integridad de los activos de la marca. Pueden incluir una amplia gama de datos de procedencia que ofrecen información del historial de un recurso digital.

Esta información incluye:

* **Emisor o firmante:** Información acerca de la entidad o compañía que emitió la firma digital para certificar los certificados o firmas del recurso.
* **Fecha del problema:** Fecha en la que se aplicó Content Credential al recurso.
* **Crédito y uso:** Información sobre el productor del recurso, incluidos el nombre, los identificadores de medios sociales u otra información relacionada con la identidad.
* **Proceso:** Registra las ediciones o modificaciones realizadas en el recurso.
* **Detalles del dispositivo:** Información sobre la aplicación o el dispositivo usado para crear o editar el recurso.
* **Herramienta de IA utilizada:** Si se utilizó IA generativa para editar o crear el recurso, se puede incluir el nombre del modelo utilizado.
* **Otra información relevante:** También se pueden incluir datos adicionales para ayudar a ofrecer más contexto sobre el historial de un recurso.

Para obtener una vista completa, [Verify](https://contentcredentials.org/verify) puede ofrecer una insight más completa en el historial de recursos.

Adobe Experience Manager Assets ahora es compatible con Content Credentials, lo que permite a los usuarios ver Content Credentials directamente en la interfaz de usuario de Assets Essentials de AEM. Al observar los detalles del recurso, cualquier imagen con Content Credentials (como las creadas con los servicios GenAI) muestra los detalles del manifiesto en un panel dedicado. Si el recurso se descarga, publica o comparte, las credenciales permanecen intactas con el recurso.

![recursos](/help/using/assets/content-credentials.png)

## Acceso a Content Credentials {#access-content-credentials}

1. Vaya a la interfaz de usuario de Assets Essentials y haga clic en **Assets** desde el panel izquierdo.
1. Vaya a una carpeta y seleccione el recurso que desee.
1. Haga clic en **Detalles** y seleccione `Cr pin` en el panel situado más a la derecha. La pestaña Content Credentials muestra la siguiente información sobre el recurso.
   1. **Imagen generada:** Fecha y hora en que se aplicó Content Credentials.
   1. **Resumen de contenido:** Indica si AI ha generado el recurso parcial o totalmente, o cómo se ha editado.
      ![resumen de contenido](/help/using/assets/content-credentials1.png)
   1. **Proceso:** detalla la aplicación, el dispositivo y la herramienta de IA (como Adobe Firefly) utilizados para generar el recurso, así como los cambios realizados posteriormente.
      ![proceso](/help/using/assets/CR-Process.png)
   1. **Acerca de este Content Credentials:** Nombre del emisor junto con la fecha y hora de emisión.
      ![emisor](/help/using/assets/CR-issuer.png)
