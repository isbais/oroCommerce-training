# Storefront Menu Components

El **storefront menu** en OroCommerce permite a los usuarios orientarse dentro de tu sitio web y acceder fácilmente a su cuenta, **shopping cart** y otra información esencial a través de enlaces distribuidos en diferentes lugares: junto al menú principal, en el **footer**, en el **featured menu**, etc.

## Funcionalidad del Storefront Menu

La funcionalidad del **storefront menu** consiste en varios **components** suministrados con las configuraciones necesarias para crear la navegación del **storefront** de tu sitio web y permitir a los visitantes saber dónde están, a dónde pueden ir y dónde ya han estado.

Puedes modificar la **default configuration** para agregar nuevos **menu items**, excluir algunos elementos de dispositivos específicos, establecer condiciones de visibilidad para ciertos **customer groups**, o ajustar la **default configuration** según valores de configuración particulares.

## Acceso a los Menu Items

Para acceder a los **storefront menu items**, navega a **System > Frontend Menus** en el **back-office**.

Por defecto, OroCommerce proporciona los siguientes **menu items**:

![Storefront Menu Items Back Office](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/storefront_menu_items_back_office-1.png)

> **Nota**: Actualmente, **Frontend Menus** incluye **menu items** tanto para **Refreshing Teal** como para la versión 5.1 y anteriores para soportar todas las versiones de OroCommerce.

A continuación se muestra la visualización de cada **menu item** en el **storefront**:

![Storefront Menu Items Representation](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/storefront_menu_items_representation-1-1024x740.png)

> **Nota**: Para familiarizarte más con cada **frontend menu component**, lee la guía relacionada en nuestra documentación en línea.

## Configuración de Niveles

Puedes configurar cada **menu element** en cinco niveles: **global**, **organization**, **website**, **customer group** y **customer**. Siempre mantén un ojo en la **fallback logic**, lo que significa que los valores establecidos en un nivel inferior (ej: nivel **customer**) siempre prevalecerán y sobrescribirán la configuración establecida en un nivel superior.

![Frontend Menu Config](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/frontend_menu_config-1024x609.png)

## Integración con el Theme

Una vez que hayas configurado los **menu items**, puedes agregarlos a la opción de configuración del **theme** seleccionado de tu sitio web, colocándolos en cualquier lugar del **storefront header**. En la siguiente sección, elaboraremos este tema en detalle.

