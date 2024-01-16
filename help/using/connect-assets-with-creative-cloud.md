---
title: Conectar AEM Assets a Creative Cloud
description: Obtenga información sobre cómo configurar y conectar AEM Assets a Creative Cloud. Conéctese a un derecho de Creative Cloud que se haya suministrado a una organización IMS diferente para utilizar fácilmente las integraciones de Creative Cloud más recientes en AEM Assets, incluidas las bibliotecas Express y Creative Cloud.
exl-id: 3d8d7429-ddf6-44cd-a6e7-ba2afcbaf52b
source-git-commit: 36f13972e7dc7b1546cdba0713a60f95f2bbc415
workflow-type: ht
source-wordcount: '286'
ht-degree: 100%

---

# Conectar AEM Assets a Creative Cloud  {#cross-org-entitlements}

Experience Manager Assets ofrece la posibilidad de conectarse a un derecho de Creative Cloud que se proporciona a una organización IMS diferente para utilizar fácilmente las integraciones de Creative Cloud más recientes en AEM Assets, incluidas las bibliotecas Express y Creative Cloud.

Si los productos de Creative Cloud y AEM Assets se suministran a organizaciones IMS independientes, puede conectarse a una organización de Creative Cloud diferente para poder ejecutar flujos de trabajo integrados entre las dos soluciones.

## Requisitos previos {#prerequisites}

* Derechos de administrador en Experience Manager Assets

* Derecho activo al Creative Cloud para el mismo ID de usuario utilizado en Creative Cloud y Experience Manager. Los derechos sobre los ID personales y federados con la misma dirección de correo electrónico se manejan como ID de usuario diferentes.

## Conexión a una nueva organización de Creative Cloud {#connect-to-creative-cloud-org}

Para conectarse a una nueva organización de Creative Cloud, ejecute los siguientes pasos:

1. Vaya a **[!UICONTROL Configuración]** > **[!UICONTROL Creative Cloud]**.

1. Seleccione la nueva organización de Creative Cloud mediante la lista desplegable **[!UICONTROL Seleccione el nuevo ID de organización de Creative Cloud]**. La lista muestra todas las organizaciones a las que tiene acceso. Seleccione la organización con derechos de Creative Cloud activos.

1. Haga clic en **[!UICONTROL Cambiar organizaciones]** para cambiar a la nueva organización.

   ![Derechos entre organizaciones](assets/cross-org-entitlements.png)

## Restricciones {#limitations}

* Puede conectar AEM Assets a una organización de Creative Cloud a la vez. No se admite la conexión a varias organizaciones de Creative Cloud a la vez.

* La organización de Creative Cloud a la que se conecta en AEM Assets se aplica a todos los usuarios de su organización.
