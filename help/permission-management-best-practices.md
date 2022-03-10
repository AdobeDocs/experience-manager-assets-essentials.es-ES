---
title: ¿Cómo administrar de forma eficaz los permisos de carpeta?
description: Prácticas recomendadas para la administración eficaz de permisos
source-git-commit: fe716385939d18aa23d01dac5fe5f041541d2b31
workflow-type: tm+mt
source-wordcount: '398'
ht-degree: 0%

---

# Prácticas recomendadas para la administración eficaz de permisos {#best-practices-permissions-management}

Como administrador, antes de empezar a administrar los permisos de carpeta para el repositorio de Assets Essentials, existen varias prácticas recomendadas que puede implementar para que la infraestructura sea intuitiva para los administradores y los usuarios finales más adelante mientras gestiona las operaciones.

Puede incorporar estas prácticas recomendadas mientras:

* [Creación de grupos de usuarios en el Admin Console](#admin-console-best-practices)

* [Creación de una estructura de carpetas en el repositorio de Assets Essentials](#folder-structure-assets-essentials)

* [Administración de permisos en el repositorio de Assets Essentials](#folder-permissions)

## Admin Console {#admin-console-best-practices}

Identifique las necesidades de acceso en función de los grupos de usuarios de su organización. Planifique y cree grupos de usuarios para su organización y agregue usuarios a esos grupos de usuarios. Es más fácil administrar permisos de carpeta en función de grupos de usuarios y no de usuarios individuales.

## Estructura de carpetas del repositorio de Assets Essentials {#folder-structure-assets-essentials}

Tenga en cuenta los siguientes puntos cuando empiece a planificar la creación de una estructura de carpetas en el repositorio de Assets Essentials:

* Gobernanza futura: Las carpetas controladas por los administradores y las carpetas que [delegados para permisos para otros usuarios como propietarios](manage-permissions.md##manage-permissions-folders).

* Escalable: La estructura de carpetas debe ajustarse a las necesidades futuras de su organización y debe ser fácilmente escalable.

* Tamaño: Una carpeta no debe contener demasiados recursos. Esto puede conllevar problemas de uso y puede resultar difícil de administrar.

* Intuitivo: La estructura de carpetas debería ser fácil de examinar e intuitiva para los usuarios finales. Los usuarios deben poder identificar fácilmente dónde cargar un nuevo recurso en la estructura de carpetas.

Existen varios tipos de estructura de carpetas que puede utilizar para su organización. A continuación se muestran algunos ejemplos de estructuras de carpetas típicas:

* Basado en funciones y categorías

   ![Función y categorización](assets/function-categorization.png)

* Basado en campañas

   ![Basado en campañas](assets/campaign-based.png)

* Basado en la ubicación (o el canal) de la oferta

   ![Basado en la ubicación de la oferta](assets/offer-location.png)


## Permisos de carpeta {#folder-permissions}

Después de crear grupos de usuarios para su organización, agregar usuarios a esos grupos de usuarios y seleccionar y crear una estructura de carpetas en el repositorio de Assets Essentials que se adapte a las necesidades de su organización, puede empezar a administrar permisos de carpetas para su organización. Tenga en cuenta los siguientes puntos cuando empiece a administrar permisos de carpeta:

* Aplique permisos para grupos de usuarios, no para usuarios individuales. Esto resulta en una estructura de permisos más sencilla y eficaz.

* Mantenga la estructura de permisos tan sencilla como sea posible para lograr una eficacia operativa.

* Utilice Denegar permisos de acceso con cuidado y prefiera aplicar permisos positivos (Puede editar, Puede ver, Propietario) a la estructura de carpetas.

Para obtener ejemplos sobre cómo lograr una estructura de carpetas sencilla y eficaz, consulte [Administrar permisos en carpetas](manage-permissions.md##manage-permissions-folders).

