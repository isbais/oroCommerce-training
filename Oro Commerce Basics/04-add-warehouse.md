# Agregar un Warehouse

## Tabla de Contenidos
- [Introducción](#introducción)
- [Funcionalidad de Inventory y Warehouse Management](#funcionalidad-de-inventory-y-warehouse-management)
- [Configuración del Sistema](#configuración-del-sistema)
- [Crear un Nuevo Warehouse](#crear-un-nuevo-warehouse)
- [Habilitar y Priorizar Warehouses](#habilitar-y-priorizar-warehouses)
- [Resumen](#resumen)

## Introducción

OroCommerce soporta operaciones esenciales relacionadas con la gestión y seguimiento de almacenamiento. Específicamente, la funcionalidad de **inventory** y **warehouse management** de OroCommerce mantiene un seguimiento de la disponibilidad de productos en uno o varios warehouses, muestra el inventario a compradores y representantes de ventas, y actualiza automáticamente el inventario cada vez que alguien realiza un pedido. Para empresas con niveles de stock más pequeños, estas características pueden ser suficientes. Si tu empresa requiere características avanzadas, como pronóstico de demanda, seguimiento automatizado de la calidad y consistencia de datos de productos, envío de ruta y verificación de carga de camión, puedes integrar fácilmente tu software externo de inventory y warehouse management con OroCommerce a través de nuestra potente API.

## Funcionalidad de Inventory y Warehouse Management

Por defecto, el inventario del producto está configurado para ser gestionado a través de OroCommerce, pero puedes deshabilitar esta opción para conectar tu sistema externo de elección.

Antes de continuar leyendo, también puedes revisar un video en la biblioteca de medios de Oro sobre cómo trabajar con inventory y warehouses en tu aplicación.

## Configuración del Sistema

En OroCommerce, las configuraciones relacionadas con inventory se encuentran bajo **System** en el menú principal en la sección relevante **Commerce > Inventory**. Allí, puedes cambiar la configuración predeterminada del sistema y personalizarla específicamente para las necesidades de tu negocio. En particular, puedes gestionar la configuración para **inventory statuses** permitidos, warehouses, **product options** y limitaciones de cantidad de pedido. Si quieres profundizar en inventory y warehouses en OroCommerce, revisa una guía completa de inventory en nuestra biblioteca de documentación.

Mientras tanto, volvamos al ejemplo que introdujimos anteriormente, el negocio estadounidense que vende artículos de papelería y oficina a varios negocios. Asumiendo que hay un warehouse físico que almacena todos los artículos para la venta, necesitamos agregar los detalles de este warehouse en la consola de gestión de OroCommerce.

## Crear un Nuevo Warehouse

Para crear un nuevo warehouse en tu aplicación Oro:

1. **Navega a Inventory > Warehouses** usando el menú principal.
2. **Haz clic en Create Warehouse**.
3. **Ingresa el nombre del warehouse**.
4. **Llena la dirección:**
   - Selecciona la casilla **Use Shipping Origin** para usar la dirección de origen de envío proporcionada en la configuración del sistema (**System > Configuration > Commerce > Shipping > Shipping Origin**).
   - Para usar una dirección de warehouse personalizada, ingresa el **Country**, **Region/State**, **Zip/Postal code**, **City** y dirección de la calle.
5. **Haz clic en Save**.

![Crear Warehouse](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/create_warehouse-1536x707.png)

Una vez que hayas creado el warehouse, necesitas habilitarlo en la configuración del sistema. Si tienes más de un warehouse, es posible que quieras priorizarlos para asegurar que OroCommerce use una estrategia para las actualizaciones de inventory que ocurren durante las operaciones de la tienda.

## Habilitar y Priorizar Warehouses

Para habilitar y priorizar warehouses:

1. **Navega a System > Configuration** en el menú principal.
2. **Selecciona Commerce > Inventory > Warehouses** en el menú de la izquierda.

![Configuración de Warehouse](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/warehouse_config-1536x682.png)

3. **Habilita tantos warehouses como necesites:**
   - Si es necesario, haz clic en **+Add Warehouse**.
   - Selecciona el nombre del warehouse de la lista **Choose a Warehouse**.
   - Usa drag and drop para priorizar los warehouses si tienes más de uno. Cuanto más alto esté el warehouse en la lista, mayor prioridad tiene. Los productos se ordenan y envían desde los warehouses de mayor prioridad primero.

4. **Puedes gestionar la lista de warehouses habilitados usando las siguientes acciones:**
   - Para deshabilitar un warehouse, haz clic en **x** a la derecha de la fila del warehouse junto al ícono de drag and drop.
   - Para limpiar el warehouse seleccionado, haz clic en **x** a la derecha del nombre del warehouse.
   - Para seleccionar un warehouse diferente de la lista, haz clic en **v** a la derecha del nombre del warehouse y selecciona un nuevo warehouse para habilitar.
   - Para ver la lista completa de warehouses en la tabla, haz clic en el signo de barra a la derecha del nombre del warehouse. La lista de warehouses se abre en una ventana emergente.

5. **Una vez que todos los warehouses estén habilitados y priorizados, haz clic en Save**.

Como se ilustra a continuación, hemos creado un warehouse principal y lo hemos habilitado en el sistema.

![Configuración de Warehouse Guardada](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/warehouse-config-saved-1536x362.png)

## Resumen

Entonces, en este punto, tenemos el master catalog y las categorías creadas, los productos subidos, el warehouse habilitado. Ahora es el momento de importar los niveles de inventario de productos y ver cómo podemos gestionar el inventory para los productos.
