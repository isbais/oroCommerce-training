# Organizar un Catálogo Web

## 📋 Tabla de Contenidos

- [Introducción](#introducción)
- [Crear una Landing Page](#crear-una-landing-page)
- [Crear Páginas de Categoría](#crear-páginas-de-categoría)
- [Crear una Product Collection](#crear-una-product-collection)
- [Agregar Sub Menús](#agregar-sub-menús)
- [Consejo Importante](#consejo-importante)

---

## Introducción

Ahora podemos organizar el contenido del catálogo en la estructura deseada, que definirá la apariencia y sensación de la navegación y menús en el **storefront** de OroCommerce.

El primer paso es crear elementos de menú de primer nivel, que se listan como encabezados de menú y enlazan a páginas de contenido específicas. Un buen primer paso es decidir sobre la página de contenido en la que los compradores aterrizarán cuando lleguen al storefront. Esto no necesariamente necesita ser una **landing page**; podría ser una **product page** o una **system page**.

Para nuestro ejemplo, vamos a crear un catálogo web que demuestre varias páginas de contenido, comenzando con la **landing page** y procediendo a las páginas de categorías de productos y colecciones de productos. La **landing page** reemplazará la página de aterrizaje predeterminada de OroCommerce ilustrada en la captura de pantalla anterior.

## Crear una Landing Page

Navega de vuelta al catálogo web bajo `Marketing > Web Catalogs` y haz clic en el nuevo catálogo para comenzar a editar sus páginas:

### Pasos para Crear la Landing Page:

1. **Haz clic** en `Edit Content Tree` en la parte superior derecha de la página del catálogo.
2. **Proporciona** un título significativo.
3. **Selecciona** la casilla `Rewrite Variant Title` si te gustaría personalizar el título de esta página. Por ejemplo, estamos agregando una **landing page** para el cliente, que se llama **Branded and Bulk Stationary**. Si escribimos este título y habilitamos la casilla, OroCommerce usa este nuevo nombre en lugar del creado para la **landing page**.
4. **En la sección SEO**, completa la **meta description** y **meta keywords** para ayudar a los motores de búsqueda a mostrar tu contenido web a la audiencia relevante.
5. **En la sección Restrictions**, define la visibilidad del catálogo web. Por defecto, el catálogo web se muestra para cualquier localización, en cualquier sitio web, y para cualquier cliente. Para hacer que OroCommerce aplique un catálogo web al **storefront** solo para la combinación particular de estos factores, crea una restricción seleccionando todos o algunos de los siguientes: **target localization**, **website**, y **customer** o **customer group**.
  
   > **Nota**: Por ejemplo, puedes tener una página especial con precios especiales disponibles para compras al por mayor. Podrías entonces crear una página que muestre la información de venta y la restrinja solo a grupos como clientes mayoristas o proveedores al por mayor. Si no hay restricciones, la página puede ser visible para cualquiera que pueda acceder al catálogo.

   > **Importante**: Ten en cuenta que solo un campo debe ser elegido para clientes a la vez, ya sea un **customer group** o un **customer**. Además, nunca dejes las restricciones para variantes no predeterminadas vacías. Esto puede causar una colisión de prioridad inesperada entre las variantes predeterminadas y no predeterminadas.

6. **En la sección Content Variant**, selecciona el tipo de contenido que se mostrará en el **storefront** de la lista a la derecha. Estamos seleccionando una **Landing Page**.

   Puedes crear una **landing page** de antemano bajo `Marketing > Landing Pages` en el menú principal o sin salir de la página del catálogo web haciendo clic en el ícono `+` junto al campo **Landing Page**. Más información sobre **landing pages** está disponible en la [biblioteca de documentación de OroCommerce](https://doc.oroinc.com/user/back-office/marketing/landing-pages/).

   ![Crear Landing Page](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/create-landing-page-2-1536x711.png)
      
7. **Haz clic** en `Save` cuando hayas terminado.

   Cuando regreses al **storefront** y recargues la página, la nueva **landing page** habrá reemplazado la página predeterminada de OroCommerce. Los únicos elementos de menú disponibles son **Resource Library**, **About**, y **Contact Us**. Volvamos a la **back-office** de OroCommerce para agregar nodos de contenido adicionales y trabajar a través de los elementos de menú de primer nivel.

   ![Storefront Vacío](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/empty-web-catalog-storefront-2-1536x764.png)

## Crear Páginas de Categoría

Ahora repetiremos el proceso para agregar páginas de categoría desde el **master catalog**. Queremos que estén en el mismo nivel, así que asegúrate de estar en el nodo de contenido de la página principal (ej., **Branded and Bulk Stationary**) en la **back-office** cuando agregues nuevos nodos de contenido.

### Pasos para Crear Páginas de Categoría:

1. **Haz clic** en `Create Content Node` en la parte superior derecha.
2. **Completa** los campos necesarios.
3. **En la sección Content Variants**, usa el menú desplegable para seleccionar `Add Category`. La página de categoría es un enlace directo a una categoría de producto de OroCommerce en el **master catalog** y lista todos los productos dentro de ella.

   ![Agregar Categoría](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/add-category-2-1536x712.png)

4. **Bajo la sección Category**, selecciona la categoría de producto. Para nuestro ejemplo, seleccionamos **Paper and Mailing** primero.

5. **Haz clic** en `Save`.

   Hemos creado de manera similar menús de primer nivel con el resto de las categorías del **master catalog** (**Writing Supplies**, **Desktop Accessories**, **Presentation Equipment**).

   Si quieres cambiar el orden de los elementos del menú, puedes **arrastrarlos y soltarlos** en la **back-office**.

   ![Drag and Drop](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/drag-n-drop-2-1536x394.png)

   Ahora echemos un vistazo a cómo se muestran todas las categorías en el **storefront**.

   > **Nota**: Hacer clic en el elemento de menú seleccionado te redirigirá a la página con los productos en esa categoría.

## Crear una Product Collection

Ahora, repetiremos el proceso para una **product collection** para el menú **Desktop Accessories**. Una **product collection** es un segmento basado en filtros que te ayuda a mostrar un conjunto personalizado de productos en el catálogo web.

### Pasos para Crear Product Collection:

1. **Haz clic** en el menú **Desktop Accessories**.  
2. **En la sección Content Variants**, usa el menú desplegable para seleccionar una **product collection**.

   ![Crear Product Collection](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/create-product-collection-1-1536x551.png)

3. **En la sección Product Collection**, puedes definir los elementos que se incluirán en la **product collection**. El **Segment Name** se genera automáticamente. Como puedes ver en la captura de pantalla, esta sección tiene pestañas para elementos que fueron agregados por el filtro, excluidos a propósito, o agregados manualmente.

4. **Para usar filtrado avanzado**, haz clic en `Advanced Filter`. Se muestra un diálogo de segmento. Puedes crear segmentos usando una variedad de filtros y condiciones. Para nuestro ejemplo, vamos a seleccionar todos los productos que están en stock pero tienen un inventario de menos de 500 elementos.

5. **Para esto**, arrastra la opción **field condition** a la caja de configuración y usa el menú desplegable para elegir un campo.

6. **Selecciona** `Product/Category/Products>Inventory Status`. Selecciona el valor del campo **In stock**.

7. **Arrastra** otra opción **field condition** a la caja de configuración, y usa el menú desplegable para elegir un campo.

8. **Selecciona** `Product/Product(Inventory Level) > Quantity`. Establece el valor del campo a menos de 500.

9. **Haz clic** en `Preview Results` para cargar la lista de productos coincidentes.

10. **Haz clic** en `Save` en la parte superior derecha de la página para guardar el nodo de contenido.

    ![Filtro Avanzado](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/product-collection-advanced-filter-1536x742.png)

    Cuando volvamos al **storefront** y hagamos clic en la pestaña **Desktop Accessories**, veremos los productos filtrados con la ayuda del filtro avanzado de hace un momento.

    ![Product Collection en Storefront](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/product-collection-storefront-1536x653.png)

## Agregar Sub Menús

Después de configurar el primer nivel del menú principal, puedes configurar el segundo nivel para él, así como muchos otros sub-niveles, dependiendo de la estructura que visualices para la tienda.

Puedes hacer esto creando un nodo de sub-menú en la **back-office**:

### Pasos para Agregar Sub Menús:

1. **Selecciona** el nodo padre en el que te gustaría colocar el nodo de sub-menú, y haz clic en `Create Content Node`. Para nuestro ejemplo, creemos un submenú para la categoría **Desktop Accessories**.
2. **Completa** los detalles en la sección General, como se describió anteriormente. Llamaremos al menú de segundo nivel **Organizers**.
3. **En la sección Content Variants**, agrega productos coincidentes, ya sea manualmente o usando el filtro avanzado.
4. **Haz clic** en `Save`.

   Cuando navegamos al **storefront**, el menú de segundo nivel que acabamos de crear aparece bajo **Desktop Accessories**.

   ![Sub Menú](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/sub-menu-1536x221.png)

   > **Consejo**: De esta manera, puedes crear tantos niveles bajo el menú de primer nivel como sea necesario para tu tienda.

## Consejo Importante

> **💡 HINT**: Usa la función **navigation root** ([documentación](https://doc.oroinc.com/user/back-office/marketing/web-catalogs/web-catalog-nav-tool-usecase/)) para seleccionar el nodo de contenido de tu elección como la raíz para construir el árbol de navegación en el **storefront**. Una vez que definas el alcance de la **navigation root** en la **system configuration** ([documentación](https://doc.oroinc.com/user/back-office/system/configuration/system/websites/global-routing/#sys-config-sysconfig-websites-routing)), el menú principal en el **storefront** debería mostrar los sub-menús solo desde el rango de **navigation root** seleccionado.

---

**Próximo paso**: Una vez que el catálogo web esté poblado con menús y productos, procedemos a las opciones de pago.

---

*Este documento forma parte de la guía de Oro Commerce Basics.*