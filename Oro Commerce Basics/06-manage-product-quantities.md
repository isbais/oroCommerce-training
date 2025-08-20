# Gestionar Cantidades de Productos

## Tabla de Contenidos
- [Introducción](#introducción)
- [Unidades de Medición](#unidades-de-medición)
- [Gestión de Cantidades](#gestión-de-cantidades)
- [En el Inventory Registry](#en-el-inventory-registry)
- [Por Producto](#por-producto)
- [Resumen](#resumen)

## Introducción

La cantidad del producto es la cantidad de producto que se puede vender con su unidad de medición. La cantidad del producto podría ser un número entero o un número con una parte fraccionaria (un número de punto flotante). Si la cantidad debe ser un número entero o fraccionario, y cuántos dígitos se permiten en la parte fraccionaria, se define por la configuración de la unidad de medición seleccionada. Por ejemplo, por defecto "kilogram" permite ingresar hasta 3 números después del punto decimal, y "each" requiere una entrada de número entero.

## Unidades de Medición

Puedes gestionar fácilmente las cantidades de productos que tienes en stock tanto en el registro de inventory como por producto.

## Gestión de Cantidades

### En el Inventory Registry

Puedes filtrar el inventory de productos en el registro de inventory para limitar los registros al subconjunto que te gustaría actualizar. Puedes editar el **inventory status** y la cantidad en las columnas respectivas haciendo clic en el valor actual, escribiendo el nuevo y presionando Enter. La información actualizada se guarda automáticamente.

![Edición Inline de Inventory](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/inventory_inline_editing.png)

### Por Producto

También puedes gestionar cantidades para un solo producto en múltiples warehouses:

1. **Navega a Products > Products** en el menú principal. Se abre la lista de productos.
2. **Haz clic en el producto** para el que quieres gestionar el inventory. Se abre la página de vista del producto.
3. **Haz clic en More Actions** en la parte superior derecha y luego haz clic en **Manage Inventory**.
4. **Actualiza las cantidades del producto** y haz clic en **Save**.

Agregamos un warehouse para nuestro ejemplo, y así es como se ve la página cuando intentamos actualizar la cantidad de un solo producto:

![Inventory del Producto](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/product_inventory.png)

Si tienes más de un warehouse, todos se listarán en la columna **Warehouse** en la ventana de diálogo **Manage Inventory**.

## Resumen

En la siguiente sección, vamos a explicar cómo opera la gestión de precios en OroCommerce y mostrarte cómo agregar precios a los productos que has subido a tu master catalog.
