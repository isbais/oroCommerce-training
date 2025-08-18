# Introducción a Master Catalog y Web Catalog en OroCommerce

Cuando pienses en organizar productos en colecciones o categorías (por tipo de producto, marca, precio, industria, etc.), necesitarás configurar tu **master catalog** o un **web catalog**.

En este módulo aprenderás a:

- Diferenciar entre las dos herramientas nativas: **master catalog** y **web catalog**.
- Construir nuevos web catalogs desde cero o modificar los predeterminados.
- Personalizar y enriquecer los web catalogs con nuevos menús para diferentes localizaciones, clientes o grupos de clientes.
- Configurar categorías en los web catalogs usando distintos **content variants**: system page, landing page, master catalog category o product collection.
- Usar **embedded filters** para crear condiciones especiales en tus product collections.
- Crear versiones ilimitadas, personalizadas y adaptadas de tu storefront mediante web catalogs.
- Trabajar con web catalogs en una aplicación **multi-org**.

---

## Diferencias clave entre Master Catalog y Web Catalog

Tanto el master catalog como el web catalog organizan productos similares en grupos y pueden mostrarse en el storefront como parte del menú principal. Sin embargo:

### Master catalog:
- Es el **repositorio único** de todos los productos de la organización.
- Solo puede existir **uno por organización**.
- Cada producto pertenece a una **sola categoría**.
- Su propósito es principalmente organizar, categorizar y almacenar.

### Web catalog:
- Puedes crear un **número ilimitado**.
- Permite seleccionar solo un rango de productos del master catalog para mostrarlos en el storefront.
- Los productos pueden asignarse a **múltiples nodos o categorías**.
- **Ejemplos de uso**:
  - Mostrar únicamente productos en stock en un submenú **Daily Living Aids**.
  - Mostrar productos con inventario < 10 en un submenú **Clearance**.
  - Aplicar filtros dinámicos para actualizar automáticamente los productos visibles.

![Master Catalog Example](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/eating_aids_master_catalog-1024x353.png)

![Web Catalog Example](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/daily_living_aids_web_catalog-1024x403.png)

![Clearance Low Inventory](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/clearance_low_inventory-1-1024x449.png)

---

## Ventajas del Web Catalog

El uso de web catalog ofrece mayor flexibilidad para:

- Crear **múltiples versiones** del storefront en una misma aplicación de OroCommerce.
- Definir **restricciones de visibilidad** por cliente, grupo de clientes, localización o sitio web.
- **Reutilizar** un mismo producto en diferentes categorías.
- **Ocultar** ciertos productos a públicos específicos.
- **Personalizar** con distintos tipos de páginas (system page, landing page, etc.).
- **Optimizar** la estructura para SEO.
- **Crear y modificar** product collections con filtros, añadir nodos de contenido y personalizar el menú.

---

## 📌 Conclusión:

- El **master catalog** es la base completa de todos los productos.
- El **web catalog** es la capa flexible que permite mostrar, segmentar y personalizar las vistas del catálogo para diferentes audiencias, ya sean **B2B** o **B2C**.

---

## Creación y asignación de un nuevo Web Catalog

Considerando el caso de uso de una tienda médica en EE.UU. que vende productos a distintas empresas a nivel nacional, crearemos un nuevo web catalog, lo asignaremos como predeterminado y añadiremos content variants relevantes a cada content node.

### Crear un Web Catalog

1. Navega a **Marketing > Web Catalogs** en el menú principal.
2. Haz clic en **Create Web Catalog**.

![Creating Web Catalog](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/creating_web_catalog-1024x365.png)

3. Asigna un nombre significativo y una descripción para diferenciarlo de otros web catalogs (ya que puedes tener múltiples).
4. Haz clic en **Save and Close** en la parte superior derecha.

En este punto, tu nuevo **basic web catalog** queda creado.

---

### Asignar un Web Catalog como Default

El siguiente paso es asignar este catálogo como el **default catalog** del storefront.

⚠️ **Nota**: Si no se asigna ningún web catalog, se utiliza el master catalog para definir el menú del storefront.

#### Pasos:

1. Navega a **System > Configuration** en el menú principal.
2. Selecciona **System Configuration > Websites > Routing** en el panel izquierdo.
3. En el campo **Web Catalog**, selecciona el nuevo catálogo en el dropdown (en este ejemplo, Medical Products).
4. Haz clic en **Save Settings**.

![Set Web Catalog as Default](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/set_web_catalog_as_default-1-1024x434.png)

---

### Visualizar el Web Catalog en el Storefront

Ahora, navega al OroCommerce storefront y recarga la página para ver el web catalog recién creado.

Lo que verás es una **home landing page en blanco**, sin contenido ni categorías de producto, excepto los ítems del menú **About** y **Contact Us**.

Estos elementos representan un **static custom storefront menu** (commerce_main_menu), que no forma parte ni del master catalog ni del web catalog, y que puede moverse a otra sección del storefront.

![Blank Storefront Page](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/blank_storefront_page-1-1024x343.png)

---

## 📌 Conclusión:

- Has creado un **web catalog básico**.
- Lo asignaste como **default** para tu storefront.
- Comprobaste su aparición inicial, listo para ser enriquecido con contenido, categorías y productos.


