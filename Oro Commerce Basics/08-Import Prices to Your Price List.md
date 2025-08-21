# Importar Precios a Tu Lista de Precios

## 📋 Tabla de Contenidos

- [Introducción](#introducción)
- [Lista de Precios Mayorista](#lista-de-precios-mayorista)
  - [Crear una Nueva Lista de Precios](#crear-una-nueva-lista-de-precios)
  - [Importar Precios desde Archivo CSV](#importar-precios-desde-archivo-csv)
  - [Gestionar la Lista de Precios](#gestionar-la-lista-de-precios)
- [Lista de Precios de Socios](#lista-de-precios-de-socios)
  - [Configurar Reglas de Cálculo de Precios](#configurar-reglas-de-cálculo-de-precios)
- [Recursos Adicionales](#recursos-adicionales)

---

## Introducción

Para nuestro ejemplo, vamos a crear 2 listas de precios simples, una para clientes mayoristas y otra para socios de la empresa. Más tarde, cuando la configuración del comercio esté completa y tengas clientes agregados al sistema, podrás agregar estas listas de precios a clientes y grupos de clientes específicos.

Vamos a comenzar creando primero la lista de precios mayorista. Debe tener los precios para clientes que compran artículos de papelería al por mayor, y que, por lo tanto, esperan etiquetas de precio más bajas. En el archivo .csv que hemos preparado, los artículos tendrán precios determinados para 10, 50, 100 y 200 artículos. Esto significa que, por ejemplo, si un cliente ordena 20 artículos, obtendrá el precio especificado para 10.

Veamos cómo crear una lista de precios y poblarla con precios mayoristas a continuación.

## Lista de Precios Mayorista

### Crear una Nueva Lista de Precios

Para agregar precios a productos, primero crea una nueva lista de precios:

1. **Navega** a `Sales > Price Lists` usando el menú principal.
2. **Haz clic** en `Create Price List` en la parte superior derecha.
3. En la sección **General**, proporciona la siguiente información:
   - **Name** — Escribe el nombre de la lista de precios. Para nuestro ejemplo, la hemos llamado `Wholesale Price List`.
   - **Currencies** — Selecciona una o más monedas que te gustaría habilitar para los precios en la lista de precios. El precio de cada moneda debe proporcionarse explícitamente, ya que no hay conversión automática.
   - **Active** — Establece la opción para habilitar la lista de precios. Mantén la lista de precios inactiva mientras redactas los precios. Desactiva la lista de precios para deshabilitar temporalmente los precios que contiene.
   - **Schedule** — Si es necesario, agrega un horario para la activación y desactivación de la lista de precios.
4. **Haz clic** en `Save and Close`.

![Crear Lista de Precios Mayorista](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/wholesale_price_list-720x382-1.png)

### Importar Precios desde Archivo CSV

Para cargar una gran cantidad de precios de productos en la lista de precios recién creada, usa la opción `Import File`. Aunque ya debes tener un archivo .csv con precios listo, se recomienda descargar la plantilla primero para asegurarte de que la información en el archivo esté estructurada correctamente y que el documento tenga encabezados apropiados. También ten en cuenta que las unidades y la moneda ya deben estar creadas en la consola de administración de la tienda antes de la importación de niveles de inventario.

#### Pasos para Importar:

1. **Abre** la lista de precios recién creada.
2. **Haz clic** en `Import File` en la parte superior derecha.

![Importar Archivo](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/wholesale_price_list_import-720x335-1.png)

3. **Haz clic** en `Export Template` para descargar un archivo .csv de muestra con los encabezados necesarios.
4. **Basándote** en el archivo descargado, crea tu información masiva en formato .csv. Una vez que tu archivo esté listo, haz clic en `Choose File` y selecciona el archivo .csv preparado.
5. En este punto no tenemos precios en la aplicación, por lo que puedes seleccionar cualquier estrategia para la importación. Hay dos estrategias disponibles:

   - **Add and Replace**: Sobrescribe los precios existentes con los mencionados en el archivo para el artículo de producto correspondiente. También agrega nuevos precios a los productos con valores vacíos.
   - **Reset and Add**: Elimina todos los precios existentes y agrega solo los listados en el archivo .csv.

6. **Haz clic** en `Import File`.

> **Nota**: También puedes validar tu archivo antes de subirlo para verificar si hay errores en él. Haz clic en `Validate` para verificar tus resultados de importación. Si hay algún `Record with errors`, corrígelos en el archivo .csv antes de comenzar la importación.

La siguiente captura de pantalla muestra los precios de productos de muestra agregados a la plantilla proporcionada.

![Plantilla de Importación](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/wholesale_price_list_import_template.png)

### Gestionar la Lista de Precios

Como puedes ver, la lista de precios mayorista tiene precios proporcionados para 10, 50, 100 y 200 productos. Una vez que la lista se suba a OroCommerce, la aplicación podrá usar la información dada y mostrar los precios a los clientes según los niveles en la lista de precios. La siguiente captura de pantalla muestra la lista de precios mayorista ya subida a OroCommerce.

![Lista de Precios Completada](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/wholesale_price_list_all-1-1536x488.png)

Usando filtros, puedes reducir la lista a productos específicos. También puedes ver, editar o eliminar productos particulares si usas el menú ilustrado a continuación.

![Gestionar Productos](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/wholesale_price_list_manage.png)

## Lista de Precios de Socios

Ahora vamos a crear la segunda lista de precios de una manera ligeramente diferente. Esta lista de precios debe tener precios para la misma cantidad de productos, pero serán 10% más bajos que los precios proporcionados en la lista de precios mayorista. La razón es un acuerdo donde nuestros socios compran más productos que los clientes mayoristas ordinarios a cambio de un descuento del 10%. Más tarde revenden estos artículos en sus tiendas.

Para este escenario, necesitamos crear una nueva lista de precios y luego agregar una regla de cálculo de precio de descuento del 10%:

### Configurar Reglas de Cálculo de Precios

1. **Crea y nombra** la lista (ej., `Partner Price List`), selecciona la moneda USD, y habilita la casilla `Active`.
2. En la sección **Price Assignment**, comienza escribiendo la siguiente fórmula:
   ```
   product.id in pricelist
   ```
3. **Selecciona** `Wholesale Price List` de la lista. La fórmula debería recoger el ID de la lista de precios asignado a la lista de precios en el sistema. En nuestro caso, el ID de `Wholesale Price List` es 2.
4. **A continuación**, selecciona `assignedProducts` del menú desplegable para completar la fórmula.

![Fórmula de Asignación 1](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/price-list-formula-1.png)

![Fórmula de Asignación 2](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/price-list-formula-2.png)

5. **A continuación**, haz clic en `+Add` en la sección **Price Calculation Rules**. Cada regla debe ser responsable de un nivel de precio. En nuestro ejemplo, los niveles de producto son 10, 50, 100 y 200 para la lista de precios mayorista. Por lo tanto, necesitamos 4 reglas, una para cada nivel.

6. **Para Price for Quantity**, establece el número de artículos, la unidad requerida y la moneda:
   - Nuestro primer nivel es **10**, la unidad es el **artículo**, y la moneda es **USD**.

7. **Para el campo Calculate As**, usa la siguiente fórmula:
   ```
   pricelist[2].prices.value * 0.9
   ```
   (donde 0.9 es el descuento del 10% del que hablamos anteriormente).

8. **Para el campo Condition**, usa la siguiente fórmula:
   ```
   pricelist[2].prices.quantity == 10
   ```
   (donde 10 es el primer nivel de cuatro).

9. **Proporciona** el número de prioridad.

![Regla de Precio](https://hive.oroinc.com/wp-content/uploads/sites/21/2018/06/price-rule.png)

**Repite** los mismos pasos para los niveles restantes (50, 100 y 200), asegurándote de cambiar los valores en las reglas en consecuencia. Una vez que hayas terminado, guarda la lista de precios. Ahora debería tener los precios listados con un descuento del 10% específicamente para tus socios B2C.

## Recursos Adicionales

También puedes ver un video en la biblioteca de medios de Oro sobre cómo usar [price calculation rules](https://hive.oroinc.com/lesson/import-prices-to-your-price-list/#:~:text=how%20to%20use-,price%20calculation%20rules,-.).

---

*Este documento forma parte de la guía de Oro Commerce Basics.*