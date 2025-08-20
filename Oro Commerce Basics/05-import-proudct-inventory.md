# Importar Niveles de Inventory de Productos

## Tabla de Contenidos
- [Introducción](#introducción)
- [Proceso de Importación](#proceso-de-importación)
- [Plantilla de Inventory Levels](#plantilla-de-inventory-levels)
- [Información de Ejemplo](#información-de-ejemplo)
- [Validación y Resultados](#validación-y-resultados)

## Introducción

Puedes importar **inventory statuses** (en stock, fuera de stock o descontinuado) y niveles (cantidad y unidad) para tus warehouses usando el archivo .csv que sigue la estructura de datos de detalles de inventory.

## Proceso de Importación

Para descargar la plantilla de exportación e importar una cantidad masiva de niveles o statuses de inventory:

1. **Navega a Inventory > Managed Inventory** en el menú principal. Se abre la lista de niveles de inventory.
2. **Haz clic en Import File** en la parte superior derecha.
3. **Haz clic en Export Template** para descargar un archivo .csv de muestra con los encabezados necesarios. Puedes importar tanto inventory statuses y niveles como solo inventory statuses.

![Importar Niveles de Inventory](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/import_inventory_levels-1536x566.png)

## Plantilla de Inventory Levels

Para nuestro ejemplo, hemos descargado una plantilla de **Detailed Inventory Levels**, como se ilustra a continuación:

![Plantilla de Inventory Levels](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/import_inventory_levels_template.png)

Basándote en el archivo descargado, crea tu información en masa en formato .csv.

## Información de Ejemplo

A continuación se muestra la captura de pantalla de la información que proporcionamos para nuestros productos de ejemplo:

![Plantilla de Inventory Levels Llenada](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/import_inventory_levels_template_filled-720x212-1.png)

Una vez que tu archivo esté listo, haz clic en **Choose File**, selecciona el archivo .csv preparado y haz clic en **Import File**.

## Validación y Resultados

**Nota:** También puedes validar tu archivo antes de subirlo para verificar si hay errores en él. Haz clic en **Validate** para verificar tus resultados de importación. Si hay **Records with errors**, corrígelos en el archivo .csv antes de comenzar la importación.

Los mensajes de estado interactivos informan sobre el progreso de la importación, y una vez que la importación esté completa, los cambios se reflejan en la lista después del refresh. También se entrega un mensaje de correo electrónico con el estado de la importación a tu buzón.
