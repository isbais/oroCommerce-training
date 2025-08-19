# Gestión de Content Blocks

Los **content blocks** son fracciones de tu página web o piezas de contenido (ej: texto, botones, widgets, videos, imágenes o enlaces) que creas para ser mostrados en tu sitio web. Cada **content block** es un componente independiente que puedes insertar en una o varias páginas.

A diferencia de los **content widgets**, que tienen representaciones visuales y configuraciones predefinidas, los **content blocks** son fragmentos de contenido en blanco que diseñas desde cero. Se usan comúnmente cuando necesitas reutilizar el mismo segmento de contenido en múltiples páginas del sitio, por ejemplo: dirección de la empresa, página de términos y condiciones o página de certificaciones.

También puedes especificar **restricciones de visibilidad** para cada **content block** o variante de contenido estableciendo la **localization**, el **website**, el **customer** o el **customer group** de destino. De esta forma, el **content block** solo se mostrará en el **storefront** si se cumplen las condiciones configuradas.

---

## 📌 Caso de uso

Crearemos un **content block** con las condiciones de devolución y reembolso para ropa médica (zuecos, uniformes, batas de laboratorio, etc.).

- El **content block** será visible para clientes **B2B**
- Los usuarios **B2C** deberán registrarse primero para ver los detalles
- Como las condiciones son las mismas para toda la ropa médica, aplicaremos este **content block** en todas las descripciones de productos relacionados

---

## Pasos para crear un Content Block

1. **Navegar** a **Marketing > Content Blocks** en el menú principal
2. **Clic** en **Create Content Block**
3. **En la sección General**, agregar:
   - **Owner** del bloque
   - **Alias** (identificador único para usar en el layout)
   - **Title**
   - **Activar el bloque** marcando **Enabled**
4. **En la sección Content Variants**, hacer clic en **Add Content** para mostrar el campo **WYSIWYG**
5. **Agregar el contenido requerido** (ejemplo: política de devoluciones y reembolsos para clientes **B2B**)

![Content Block Return Policy](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/content_block_return_policy-1024x464.png)

6. **Definir restricciones de visibilidad** en la sección **Restrictions**. En este caso, seleccionamos **B2B customers** en el campo **Customer Group**

![B2B Restrictions](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/B2B_restrictions.png)

7. **Como planeamos mostrar una solicitud de registro** a visitantes **B2C** en lugar de la política de devoluciones, añadimos otra **content variant** dentro del mismo bloque
8. **Clic en Add Content** nuevamente e ingresar la información requerida. Para variantes no default, debes aplicar restricciones. En este caso, seleccionamos **Non-Authenticated Visitors** en el campo **Customer Group**

![Content Block for B2C](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/content_block_for-B2C-1-1024x523.png)

9. **Clic en Save** para guardar el **content block**

---

## 📌 Variantes y Traducciones

Puedes añadir un número ilimitado de **content variants** a un mismo **content block**, proveer traducciones (alemán, francés, chino, etc.) y definir restricciones de **localization** para mostrar el contenido en diferentes idiomas según el **website** y la **localization** de destino.

---

## 📌 Insertar un Content Block en un producto

1. **Navega** a **Products > Products** en el menú principal y selecciona un producto (ejemplo: **7NM98 – Men's Slip On Clogs**)
2. **Inserta el Content Block** en la sección **Description**
3. **Guarda los cambios**

![Insert Content Block to Product](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/insert_content_block_to_product-1-1024x503.png)

- **En el storefront**, un usuario registrado verá:

![View Content Block B2B](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/view_content_block_b2b-1024x853.png)

- **Mientras que un usuario no registrado** verá:

![View Content Block as B2C](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/view_content_block_as_b2c-1-1024x581.png)