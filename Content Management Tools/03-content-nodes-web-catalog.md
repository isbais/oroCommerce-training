# Content Nodes y Web Catalog en OroCommerce

## 📋 Índice

1. [Introducción a Content Nodes](#introducción-a-content-nodes)
2. [Estructura del Menú de Navegación](#estructura-del-menú-de-navegación)
3. [Agregando una Landing Page (Homepage)](#agregando-una-landing-page-homepage)
4. [Configuración del Content Node Principal](#configuración-del-content-node-principal)
5. [Agregando una System Page (All Products Page)](#agregando-una-system-page-all-products-page)
6. [Configuración de Restricciones y Herencia](#configuración-de-restricciones-y-herencia)
7. [Agregando una Master Catalog Category](#agregando-una-master-catalog-category)
8. [Agregando una Product Collection: Brand](#agregando-una-product-collection-brand)
9. [Agregando una Product Collection: Deals & Promotions](#agregando-una-product-collection-deals--promotions)

---

## Introducción a Content Nodes

OroCommerce representa los **web catalogs** como una estructura de **product collection** organizada en un **content tree** con sus categorías y subcategorías, que se denominan **content nodes**. Este **content tree** define la apariencia y sensación de tu menú del **storefront**. El **content tree** comienza desde el **root content node**, seguido por los elementos del menú de primer nivel que representan los **menu headers**. Todos los **root nodes** están anidados bajo el **homepage node**. Una vez que configures el primer nivel del menú principal, puedes configurar el segundo, tercero y otros sub-niveles, dependiendo de la estructura que visualices para la tienda.

Considerando nuestro escenario con la tienda médica que vende productos médicos, transporte, nutrición y ropa, hemos decidido dividir los productos por categoría, marca y productos con descuentos. Esto debería facilitar la navegación de los clientes a través de mucha información en nuestro sitio web.

Para nuestra tienda médica, los **menu headers** de ejemplo pueden ser los siguientes:

- **Product Category**
- **Brand**
- **Deals & Promotions**

Todos los **content (parent) nodes** pueden anidar varios niveles de sus **child nodes**, como en el ejemplo a continuación:

```
Product Category
    Wheelchairs & Transport Chairs
        Wheelchairs
        Transport Chairs
        Support Cushions
    Medical Scrubs & Clothing
        Uniforms
        Footwear
        Patient Clothing
    Bedding & Accessories
    Medical Nutrition
    Daily Living Aids

Brand
    Drive Medical
    Essential Medical
    Boost
    Hormel

Deals & Promotions
```

Cada menú puede duplicar productos bajo diferentes categorías, lo cual no sería posible a través del **master catalog**. Puedes crear tantos **subnodes** como quieras, sin embargo, no todos ellos pueden ser visibles en el **storefront**. Para personalizar la granularidad de visibilidad del **node**, pide asistencia a tu desarrollador.

---

## Agregando una Landing Page (Homepage)

Comenzaremos desde el **root content node**, que es tu **homepage** que da la bienvenida a tus clientes una vez que llegan a tu tienda en línea. Se configura por el primer **node** creado en el **web catalog**.

Entonces, vamos a crearlo navegando a **Marketing > Web Catalogs** en el **back-office** y haciendo clic en el nuevo catálogo (en nuestro caso, es Medical Products) para comenzar a editar sus páginas:

### Pasos para crear el Content Node Principal:

1. **Haz clic en Edit Content Tree** en la parte superior derecha de la página del catálogo.

![Edit Content Tree Button](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/edit_content_tree_button-1024x245.png)

En la página que se abre, crea tu primer **content node**, que será tu **homepage**.

![Blank Homepage Node](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/blank_homepage_node_-1024x451.png)

2. **Proporciona un título significativo** (por ejemplo, Medical Products)

3. **Selecciona la casilla Rewrite Variant Title** para sobrescribir el título nativo del contenido alternativo que estás mapeando a este **catalog node**. Por ejemplo, si estás agregando una **landing page** que tiene su título (por ejemplo, Homepage), entonces esta página mostrará este título en el **storefront**. Sin embargo, si habilitas **Rewrite Variant Title**, cambiarás el nombre del título de la página de Homepage a Medical Products.

4. **En la sección SEO**, completa el **meta title**, **description** y **keywords** para ayudar a los motores de búsqueda a mostrar tu contenido web a la audiencia relevante. La optimización SEO es un tema amplio para hablar, así que lo cubriremos en detalle en el Módulo 5 de este curso.

5. **En la sección Restrictions**, define la visibilidad del **web catalog**. Por defecto, el **web catalog** se muestra para cualquier **localization**, en cualquier **website** y para cualquier **customer**. Para hacer que OroCommerce aplique un **web catalog** al **storefront** solo para la combinación particular de estos factores, crea una restricción seleccionando todos o algunos de los siguientes: **target localization**, **website** y **customer** o **customer group**.

6. **En la sección Content Variant**, selecciona el tipo de páginas que puedes agregar a tu **content node**. Los **content variants** definen la información que quieres mostrar a tus clientes cuando llegan a esta página (**content node**). Las páginas pueden ser de los siguientes tipos:

    - **System page** – una de las muchas páginas estándar prediseñadas para el **storefront** de OroCommerce (página de Sign In, página de Open Orders, página de Request a Quote, etc.)
    - **Product page** – un enlace directo a los detalles del producto
    - **All Products page** – una colección de todos los productos, generalmente agregada para catálogos más pequeños con no más de unos pocos cientos de productos
    - **Product Collection page** – una colección dinámica de productos que filtraste/seleccionaste manualmente o en masa para ser mostrados en esta página
    - **Category page** – un enlace directo a productos de una categoría del **master catalog**
    - **Landing page** – un enlace directo a una página de contenido personalizada
    - **Resource library** – si descargas una **Resource Library Extension**, puedes agregar contenido multimedia, como noticias, banners, videos de reseñas de productos, especificaciones de seguridad, etc.

![Content Variants](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/content_variants-1-1024x420.png)

7. **Estamos seleccionando una Landing Page** haciendo clic en **Add Landing Page**.

8. **Usa el dropdown** junto al campo **Landing Page** para seleccionar la página requerida de la lista de **landing pages** disponibles. Hemos seleccionado la **homepage**, que será nuestra página de bienvenida. Ten en cuenta que en instalaciones limpias de aplicaciones Oro, la **homepage** por defecto está en blanco, por lo que necesitas prediseñarla primero para poder usarla. Para crear una **landing page** de antemano, ve a **Marketing > Landing Pages** en el menú principal, o haz clic en el ícono **+** junto al campo **Landing Page** sin salir de la página del **web catalog**.

![Landing Page List](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/landing_page_list-1024x443.png)

![Add Landing Page](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/add_landing_page-1024x403.png)

9. **Habilita la opción Do Not Render Title** si no quieres que el título de la **landing page** se muestre en el **storefront**.

10. **Haz clic en Save** para guardar tus cambios.

Tu primer **content node** está listo.

![Available Actions](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/available_actions-1024x371.png)

Ahora puedes:

- **Preview** el **content node** directamente desde la página del **web catalog** haciendo clic en **Preview**. Esto abrirá otra pestaña en tu navegador, mostrando tu página del **storefront** en modo **preview**. El modo te permite navegar por otras páginas también. El panel de configuración en la parte superior de la página te permite cambiar entre **websites**, **localizations**, **customer groups** y **customers** para asegurar que la página se muestre correctamente basada en diferentes ámbitos de restricción aplicados.

> **Nota**: La capacidad de hacer **preview** de **web catalog nodes** está controlada por los permisos **Storefront Preview** definidos para el rol seleccionado en la configuración del sistema. Para más detalles sobre la gestión de roles del **back-office**, consulta nuestra documentación en línea.

![Preview Mode](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/preview_mode-1-1024x863.png)

Alternativamente, puedes regresar a tu **storefront** y recargar la página. Verás la **landing page** de la **homepage** (Homepage) que acabamos de configurar con un **image slider**, **featured menu** y **featured categories**. Estas y otras capacidades de **landing page** serán cubiertas en el Módulo 3, más adelante en el curso.

- **Delete** el **content node**. Ten en cuenta que cuando eliminas el **content node**, también eliminas todos los **child nodes** dentro de él.
- **Return** a la lista de todos los **web catalogs** haciendo clic en **Cancel**.
- **Click Create Content Node** para continuar construyendo el **content tree**. Esta acción crea el **child content node** para el que estás viendo actualmente. Siempre puedes mover el **node** arrastrándolo y soltándolo en el lugar requerido.

Ahora que has agregado un **root content node** a tu **web catalog**, agrégalo al campo **Navigation Root** en la configuración del sistema (**System Configuration > Websites > Routing**) como un **root content node** para el **storefront**. Los futuros **sub-menu nodes** que crearemos bajo este **parent node** serán visibles en el **storefront**.

![Root Content Node](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/root_content_node-1024x335.png)

> **Nota**: Cuando no se asigna ningún **web catalog**, el sistema usa el **master catalog** para definir la navegación del **storefront**. En este caso, la **homepage** del **website** debe definirse en el campo **Homepage**.

![Master Catalog Homepage](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/master_catalog_homepage-1024x515.png)

Ahora continuemos construyendo la navegación del menú de tu **storefront**, comenzando con los elementos del menú de primer nivel.

---

## Agregando una System Page (All Products Page)

Una **system page** es la página estándar preconfigurada y prediseñada que es proporcionada por OroCommerce **out-of-the-box**. Los tipos de **system page** incluyen, pero no se limitan a:

- La página **All Products** (recomendada exclusivamente para catálogos pequeños con no más de unos pocos cientos de productos; de lo contrario, el rendimiento del navegador podría verse afectado)
- La página **Quick Order Form**
- La página **User Registration**
- La página **User Account Profile**
- La página **Request for Quotes**
- La página **Contact Us**

Para nuestra tienda de muestra, hemos esbozado el siguiente **menu tree**:

```
Product Category
    Wheelchairs & Transport Chairs
        Wheelchairs
        Transport Chairs
        Support Cushions
    Medical Scrubs & Clothing
        Uniforms
        Footwear
        Patient Clothing
    Bedding & Accessories
    Medical Nutrition
    Daily Living Aids

Brand
    Drive Medical
    Essential Medical
    Boost
    Hormel

Deals & Promotions
```

donde **Product Category**, **Brand** y **Deals & Promotions** son los elementos del menú de primer nivel.

La página **Product Category** introducirá una lista de todos los productos disponibles del **master catalog** agrupados por categoría. Sin embargo, recuerda que esta **system page** es recomendada exclusivamente para catálogos pequeños para evitar afectar el rendimiento de tu navegador.

> **Nota**: A diferencia de otras **system pages**, la página **All Products** necesita ser habilitada de antemano en la configuración del sistema en el nivel requerido — globalmente (**System Configuration > Commerce > Catalog > Special Pages**) o por **website**.

![All Products System](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/AllProductsSystem.png)

### Para crear el content node:

1. **Haz clic en el parent node** en el que te gustaría colocar el **sub-menu node**, y luego haz clic en **Create Content Node**. Para nuestro ejemplo, es el **parent node** Medical Products.

2. **Completa los detalles** en las secciones **General** y **SEO**, como se describió anteriormente, nombrando el **sub-node** Product Category.

3. **Todas las restricciones** que establezcas para el **parent node** serán heredadas por sus **child nodes**. Para modificarlas, desmarca la opción **Inherit Parent** y proporciona las nuevas condiciones para el **node** requerido.

![Inherited Restrictions](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/inherited_restrictions-1-1024x495.png)

4. **En la sección Content Variants**, haz clic en **Add System Page** y selecciona la **system page** requerida de la lista de páginas disponibles.

![All Products Page](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/all_products_page-1024x356.png)

5. **Haz clic en Save** y verifica tu menú de navegación del **storefront** con el elemento de menú **Product Category** recién creado agregado a él. La página ahora muestra todos los productos en tu **master catalog** agrupados por categorías.

![All Products Page Storefront](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/all_products_page_storefront-952x1024.png)

En la siguiente sección, agregaremos varios niveles de **child nodes** con enlaces a categorías del **master catalog**.

---

## Agregando una Master Catalog Category

En esta sección, continuaremos construyendo el **content tree** del **web catalog**, creando los siguientes **sub-menu nodes** bajo el elemento de menú **Product Category**:

```
Product Category
    Wheelchairs & Transport Chairs
        Wheelchairs
        Transport Chairs
        Support Cushions
    Medical Scrubs & Clothing
        Uniforms
        Footwear
        Patient Clothing
        Bedding & Accessories
    Medical Nutrition
    Daily Living Aids
```

### Pasos para crear sub-nodes:

1. **Crea un nuevo sub-node**, completa los detalles en las secciones **General**, **SEO** y **Restrictions**, como se describió anteriormente. Llamaremos al menú de segundo nivel **Wheelchairs & Transport Chairs**.

2. **En la sección Content Variants**, usa el dropdown para seleccionar **Add Category**. La página de categoría es un enlace directo a una categoría de producto de OroCommerce en el **master catalog** y lista todos los productos dentro de ella.

3. **Bajo la sección Category**, selecciona la categoría de producto. Para usar la búsqueda, comienza a escribir el nombre de la categoría en el cuadro. Usa **>** y **v** para expandir/contraer el **tree node**. Para nuestro ejemplo, estamos seleccionando **Wheelchairs & Transport Chairs** primero.

Tu categoría del **master catalog** no tiene que tener el mismo nombre que tu **content node** del **web catalog**. Depende de ti cómo organizar tus productos internamente y mostrarlos externamente.

![Master Category Content Variant](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/master_category_content_variant-1024x645.png)

4. **Selecciona la opción requerida** en el campo **Sub-Categories**. Hay dos opciones disponibles:

    - **Include, show as filter** – Se usa para incluir todos los productos asignados a las subcategorías de la categoría maestra seleccionada, además de los productos que ya están asignados directamente. Las subcategorías del primer nivel con al menos un producto se mostrarán como un filtro de categoría en el **storefront** de OroCommerce.

![Include Show as Filter](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/include_show_as_filter-1-1024x485.png)

    - **Do not include** – Se usa para incluir solo los productos asignados a la categoría maestra seleccionada. Si la categoría tiene una subcategoría, sus elementos de producto no se mostrarán.

![Do Not Include](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/do_not_include-1-1024x388.png)

En nuestro caso, hemos seleccionado incluir todos los productos de **Support Cushions**, **Wheelchairs** y **Transportation** bajo el **parent content node** **Wheelchairs & Transport Chairs**.

5. **Haz clic en Save**.

6. **Continúa creando** el resto de los **content nodes** requeridos con las categorías del **master catalog** (**Medical Scrubs & Clothing**, **Bedding & Accessories**, **Medical Nutrition**, **Daily Living Aids**).

![Complete Content Tree](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/complete_content_tree-1.png)

Recuerda que puedes arrastrar y soltar elementos del menú en el **back-office** en un orden diferente.

![Drag and Drop Menu Items](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/drag_and_drop_menu_items-1024x435.png)

Ahora, echemos un vistazo a cómo se muestran todas las categorías en el **storefront**.

![Product Category Storefront](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/product_category_storefront-2-1024x448.png)

De esta manera, puedes crear tantos niveles bajo el menú de primer nivel como sea necesario para tu tienda.

---

## Agregando una Product Collection: Brand

En esta sección, completaremos el **content tree** inicialmente planificado, poblando los menús **Product Brand** y **Deals & Promotions** con las subcategorías relacionadas. Para esto, usaremos un **content variant** de **product collection** para nuestros **content nodes**.

**Product collection** es un segmento basado en filtros que te ayuda a mostrar un conjunto personalizado y dinámico de productos en el **web catalog** de manera similar al contenido de categoría. Significa que puedes establecer cualquier condición para filtrar todo tu rango de productos y mostrar solo los productos que coincidan con tu filtro.

![Product Collection Content Variant](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/product_collection_content_variant-1024x435.png)

Para nuestro caso, hemos decidido filtrar los registros:

- **por la marca** que les fue asignada mientras se creaban o editaban productos (bajo el nodo **Brand**)
- **por los productos con descuentos** (bajo **Deals & Promotions**)

### Para esto:

1. **Asegúrate de estar en el homepage node** (comencemos con **Brand**) cuando crees un **content node** para la **product collection**.

2. **Crea varios nodes** con marcas (**Drive Medical**, **Essential Medical**, **Boost** y **Hormel**) para que coincidan con las marcas de productos que se crean en el sistema bajo **Products > Product Brands**.

![Product Brands](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/product_brands-1024x248.png)

3. **En la sección Content Variants**, usa el dropdown para seleccionar una **product collection**.

4. **En la sección Product Collection**, puedes definir los elementos que se incluirán en la **product collection**. El **Segment Name** se genera automáticamente. Esta sección tiene pestañas para elementos que fueron agregados por el filtro, excluidos a propósito o agregados manualmente.

5. **Puedes agregar los productos requeridos manualmente**, seleccionándolos uno por uno de la lista dropdown.

![Add Products Manually](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/add_products_manually-1024x451.png)

6. **O puedes usar la funcionalidad de filtrado avanzado** para aplicar las condiciones necesarias. Haz clic en **Advanced Filter** para mostrar el diálogo de segmento con filtros. Puedes crear segmentos usando una variedad de filtros y condiciones. Para nuestro ejemplo, vamos a seleccionar todos los productos que pertenecen a la marca **Drive Medical**.

> **Nota**: Para más detalles sobre cómo crear marcas y asignarlas a productos, consulta nuestra documentación en línea.

7. **Para esto, arrastra la opción de condición de campo** al cuadro de configuración y usa el dropdown para elegir un campo.

8. **Selecciona Product/Brand>Id**. Proporciona el valor que iguale el número de ID de la marca necesaria. En nuestro caso, es 1, que representa **Drive Medical**.

9. **Haz clic en Preview Results** para cargar la lista de productos coincidentes.

![Use Advanced Filters to Add Products](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/use_advanced_filters_to_add_products-1024x617.png)

10. **Haz clic en Save** en la parte superior derecha de la página para guardar el **content node**.

Repite el proceso para llenar el nodo **Brand** con el resto de los nombres de marcas de productos (**Essential Medical**, **Boost**, **Hormel**).

![Brand Storefront](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/brand_storefront-1024x321.png)

---

## Agregando una Product Collection: Deals & Promotions

Esta sección está destinada a agrupar los productos a los que puedes aplicar algunos descuentos en el checkout bajo el menú principal **Deals & Promotions**. Hemos decidido agrupar los productos de la siguiente manera:

```
Deals & Promotions
    Medical Scrubs & Clothing 
    Bedding & Accessories
    Medical Nutrition
    Wheelchairs & Transport Chairs
    Daily Living Aids
    Walkers & Rollators
```

Estas **product collections** deben basarse en el segmento de promoción relacionado creado individualmente por categoría.

> **Nota**: Para más detalles sobre segmentos de promoción, consulta nuestra biblioteca de documentación.

Para nuestro caso, hemos creado preliminarmente varios segmentos de promoción bajo **Marketing > Promotions > Promotions**. Cada segmento incluye los productos de la categoría correspondiente con algunas condiciones extra-aplicadas.

Por ejemplo, la promoción **Medical Scrubs & Clothing** ofrece un descuento de $20 en todas las blusas de scrub que están actualmente en stock. Otra ropa que está listada bajo la categoría maestra **Medical Scrubs & Clothing** está excluida de la promoción.

![Medical Scrubs Promotion](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/medical_scrubs_promotion-1024x676.png)

Ahora puedes aplicar este segmento a la **product collection** requerida usando el **Advanced Filter**.

### Para esto:

1. **Arrastra la opción Apply Segment** al cuadro de configuración y usa el dropdown para elegir el segmento **Promotion Matching Products**.

2. **Haz clic en Preview Results** para cargar la lista de productos coincidentes.

3. **Puedes agregar más condiciones** junto al segmento de promoción, si es necesario, arrastrando la opción requerida al cuadro y seleccionando los valores necesarios.

![Applying Promotion Segment to Node](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/applying_promotion_segment_to_node-1024x667.png)

Para completar el **content tree** de **Deals & Promotions**, procede con agregar otros segmentos de promoción al resto de los **content nodes**.

> **Nota**: Cuando completes poblar el **web catalog** con todos los **content nodes** requeridos, puedes decidir qué sección del **web catalog** mostrar en tu sitio web. Eso se hace a través de la configuración del **navigation root** bajo **System Configuration > Websites > Routing**. Allí, puedes seleccionar categorías relevantes que quieres que se incluyan, en lugar de todo el **content tree** del **web catalog**. Por ejemplo, puedes construir el menú principal comenzando desde el **content node** **Medical Scrubs & Clothing** y sus **child nodes**.

![Navigation Root](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/Navigation_root-1-1024x404.png)

Finalmente, hemos completado el **content tree** que inicialmente visualizamos para nuestra tienda, con todos los niveles de primer, segundo y sub-menús más profundos.

---

## Web Catalogs en una Aplicación Multi-Org

La **edición Enterprise** de OroCommerce te permite crear y gestionar múltiples **organizations** dentro de tu aplicación. Cada **organization** en una aplicación **multi-org** de Oro es un espacio en blanco con un **inventory**, **catalogs**, **products**, y las opciones de configuración de la **organization** que pueden o no heredar de la **system configuration**.

### Características principales:

- **Organizaciones independientes**: Cada organización tiene su propio inventario, catálogos y productos
- **Web catalogs únicos**: Los web catalogs y products no se replican de una organization a otra
- **Gestión centralizada**: Solo la **global organization** puede gestionar web catalogs y products de diferentes organizations

### La Global Organization

La única **organization** que puede gestionar **web catalogs** y **products** de diferentes organizations en el **back-office** se llama **global**. Los **users** en la **global organization**, siempre que tengan niveles de acceso **Global** en su rol, pueden acceder y controlar todos los datos del sistema en todas las **organizations** dentro de una instancia de la aplicación.

![Multiple Organizations](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/multiple_organizations.png)

### Navegación entre Organizaciones

Si tienes acceso a más de una **organization**, puedes alternar entre ellas usando el **selector** en la parte superior izquierda de tu página de **back-office**.

> **Nota**: Para más detalles sobre la gestión de **organization**, consulta nuestra documentación en línea.

---

## 📋 Resumen del Módulo

Ahora que has adquirido el conocimiento fundamental sobre la gestión de **web catalog**, que constituye la navegación de tu **storefront** y organiza tus colecciones de **products** en categorías estructuradas, puedes avanzar hacia herramientas más avanzadas que ayudan a trabajar con el contenido de tu sitio web.

### Lo que has aprendido:

✅ **Diferencias entre Master Catalog y Web Catalog**  
✅ **Creación y configuración de Web Catalogs**  
✅ **Estructura de Content Nodes y Content Tree**  
✅ **Configuración de Landing Pages y System Pages**  
✅ **Integración con Master Catalog Categories**  
✅ **Creación de Product Collections con filtros avanzados**  
✅ **Configuración de promociones y descuentos**  
✅ **Gestión en aplicaciones Multi-Org**

### Próximos pasos:

En el siguiente módulo, exploraremos las **Landing Pages** y el **WYSIWYG Builder** para crear contenido dinámico y atractivo para tu **storefront**.