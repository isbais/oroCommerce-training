# Importar Productos al Master Catalog

## Tabla de Contenidos
- [Introducción](#introducción)
- [Proceso de Importación](#proceso-de-importación)
- [Información del Producto](#información-del-producto)
- [Validación y Resultados](#validación-y-resultados)
- [Resultados de la Importación](#resultados-de-la-importación)

## Introducción

Puedes agregar productos a tu master catalog de OroCommerce en un par de clics. Como probablemente ya tienes una lista .csv de productos disponibles guardada, puedes ajustarla a la plantilla de OroCommerce y subirla a tu master catalog.

## Proceso de Importación

Para descargar la plantilla y subir tus productos en masa:

1. **Navega a Products > Products** en el menú principal. Se abre la lista de productos.
2. **Haz clic en Import File** en la parte superior derecha.
3. **En el diálogo de Import**, haz clic en Choose File, selecciona el archivo .csv requerido y haz clic en Import File.
4. **Haz clic en Export Template** para descargar un archivo .csv de muestra con los encabezados necesarios.
5. **Crea tu información en masa** en formato .csv basándote en el archivo descargado. Una vez que tu archivo esté listo, haz clic en Choose File, selecciona el archivo .csv preparado y haz clic en Import File.

![Importar Productos](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/import_products-720x343-1.png)

## Información del Producto

Para nuestro ejemplo, hemos llenado la plantilla con varios simple products y proporcionado la siguiente información para ellos:

- **SKU** (ej., WRT1)
- **Attribute.Family.code** (ej., default_family)
- **Status** (ej., enabled)
- **Type** (ej., simple)
- **Inventory_status.id** (ej., in_stock)
- **Category.default.title** (ej., Presentation Equipment)
- **Names.Default.Value** (ej., Flipchart Easel 110)
- **PrimaryUnitPrecision.precision** (ej., 1)

![Plantilla de Importación de Productos](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/ImportProducts-1.png)

## Validación y Resultados

**Nota:** También puedes validar tu archivo antes de subirlo para verificar si hay errores. Haz clic en Validate para verificar tus resultados de importación. Si hay Records con errores, corrígelos en el archivo .csv antes de comenzar la importación.

Los mensajes de estado interactivos informan sobre el progreso de la importación, y una vez que la importación esté completa, los cambios se reflejan en la lista después del refresh. Además, se entrega un mensaje de correo electrónico con el estado de la importación a tu buzón.

Una vez que los productos se importan, deberían estar disponibles en la lista de productos en tu aplicación y dentro de sus categorías respectivas.

![Productos Importados](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/imported-products-1536x549.png)

![Producto en Categoría](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/product-in-category-1536x581.png)

## Resultados de la Importación

Ten en cuenta que a menos que crees un web catalog para establecer la estructura y el diseño de tu sitio web, la estructura del master catalog se usará en el storefront. Como puedes ver en la captura de pantalla a continuación, las cuatro categorías que acabamos de agregar al master catalog ahora se muestran en el storefront porque no tenemos un web catalog creado para presentar los productos aún.
