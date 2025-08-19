# Especificidades y Gestión de Customer Groups

## Tabla de Contenidos
- [Introducción](#introducción)
- [Creación de Customer Group](#creación-de-customer-group)
- [Gestión de Customer Groups](#gestión-de-customer-groups)

## Introducción

Ahora que eres consciente de cómo crear customers y customer users, podemos pasar a los **customer groups** que constituyen una parte integral de la gestión de clientes en OroCommerce.

Un **customer group** agrega customers que son similares de alguna manera. Por ejemplo, puedes crear varios grupos para distinguir entre customers minoristas y mayoristas o entre partners y customers externos, customers B2B y B2C, etc. También puedes organizar customers en customer groups independientemente de la jerarquía pero basados en parámetros de uso comunes, tales como impuestos, términos de pago, listas de precios, ubicación, industria, número de empleados, y así sucesivamente. Esto te ayudará a comercializar a cada grupo de manera efectiva y apropiada.

![Customer Groups](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/customer_groups.png)

Dentro de un customer group, puedes establecer opciones específicas para ser aplicadas a todos los customers y customer users que pertenecen a este grupo, asignar descuentos especiales y precios para productos. También puedes restringir el acceso a productos basado en a qué grupo pertenece un customer.

Combinar customers en grupos puede facilitar considerablemente su gestión y configuración interna. En lugar de aplicar configuraciones a cada customer individualmente, puedes hacerlo mucho más rápido configurando las configuraciones para todo el grupo, a menos que se requieran configuraciones personales para un customer particular.

Ahora acerquémonos al proceso de crear un customer group. Para nuestro caso, crearemos un grupo llamado Silver Partners. Este grupo combinará todos los customers con competencia plateada, principalmente nuevos customers con un período de partnership de hasta 1 año.

## Creación de Customer Group

Para crear un nuevo customer group:

1. **Navega a Customers > Customer Groups** en el menú principal. Desde esta página, puedes crear un nuevo customer group, ver detalles del customer group, y editar o eliminar customer groups existentes.

![Lista de Todos los Customer Groups](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/all_customer_groups_list-1-768x309.png)

2. **Haz clic en Create Customer Group** en la parte superior derecha de la página.

3. **En la página que se abre, completa el Name del customer**. En nuestro caso, es Silver Partners.

![Crear Customer Group](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/create_customer_group-1024x417.png)

4. **Selecciona Tax Code** que etiquetará el esquema de tributación del customer group.

5. **En la sección Customers**, selecciona los customers para agregar al customer group. En nuestro caso, agregaremos el customer Twin Glass & Mirror junto con su subsidiaria, y Partner C.

6. **En la sección Price Lists**, agrega las listas de precios necesarias y establece la prioridad para ellas como hemos hecho previamente para customers. Configura la opción de fallback para proporcionar la fuente de precio si el precio no está disponible en las listas de precios configuradas directamente. A diferencia de las opciones disponibles para customers, los customer groups tienen lo siguiente:

   - **Website** – Significa que si no se encuentra un precio coincidente en las listas de precios creadas para el customer group seleccionado, la aplicación va más allá a las listas de precios configuradas para el sitio web al que pertenece este customer group para llenar el precio del producto faltante.
   - **Current customer group only** – La aplicación busca el precio entre las listas de precios seleccionadas para el customer group solo. Si no se encuentra precio, entonces no se muestra precio al customer en el storefront.

   Cambia entre las pestañas del sitio web para configurar las configuraciones para cada sitio web individualmente.

![Crear Customer Group Parte 2](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/create_customer_group_part2-1024x411.png)

Como puedes ver, hemos agregado la Silver Partners Price List a nuestro grupo. Esta lista de precios pretende proporcionar un 20% de descuento a sus customers asignados. Sin embargo, como puedes recordar la configuración para el customer Twin Glass & Mirror, le hemos asignado una lista de precios que ofrece solo un 10% de descuento del precio predeterminado.

![Editando Customer Parte 2](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/editing_customer_part_2-1024x458.png)

Si has estado siguiendo esta sección cuidadosamente, ahora podrás adivinar qué precio de producto obtendrá Felicity Haff en su storefront con esta configuración, si el customer al que está asignada tiene la lista de precios Twin Glass & Mirror, mientras que el customer group al que está asignada tiene la lista de precios Silver Partners. ¡Esta es tu oportunidad de hacer una conjetura!

Ahora verifiquemos si estabas correcto.

La lógica de configuración de fallback predeterminada para los customer users registrados es: **Current Customer PLs > Current Customer Group PLs > Current Website PLs > Global PLs**. Significa que si no se encuentra un precio coincidente en la lista de precios creada para el customer seleccionado, la aplicación va más allá a las listas de precios configuradas para el customer group, luego al pricing del sitio web, y el pricing predeterminado a nivel del sistema para llenar el precio del producto faltante.

En nuestro caso, el pricing predeterminado se ve como sigue:

![Pricing de Producto Predeterminado](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/default_product_pricing-1-768x429.png)

Una vez que Felicity Haff inicia sesión en el storefront, va a ver el pricing con un 10% de descuento según la lista de precios asignada a su customer.

![Lista de Precios Twin Glass & Mirror](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/twin_glass__mirror_price_list-1-768x525.png)

Si cambiamos la opción de fallback de la lista de precios del customer Twin Glass & Mirror a customer group y removemos la lista de precios Twin Glass & Mirror, los precios serán tomados de la lista de precios asignada al customer group relacionado.

![Fallback a Customer Group](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/fallback_to_customer_group-1-768x273.png)

En este caso, si recargamos la página del storefront de Felicity, veremos los precios con un 20% de descuento en lugar del 10% anterior.

![Lista de Precios Silver Partners](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/silver_partners_price_list-1-768x518.png)

Una vez que hayas terminado con establecer la opción de pricing, pasemos al último paso de la configuración del customer group.

7. **En la sección Additional**, selecciona un **Payment term** para ser usado como una opción de pago disponible para los customer users durante el checkout.

8. **Haz clic en Save** en la esquina superior derecha para guardar tu customer group Silver Partners.

## Gestión de Customer Groups

Ahora que tu customer group Silver Partners está creado, es tiempo de ilustrar cómo puedes gestionarlo.

Desde una página de customer group, puedes acceder a la información agregada sobre todos los customers asignados a este grupo, condiciones relacionadas con pagos e impuestos, listas de precios habilitadas para el customer group, configuraciones de fallback y otras actividades de eCommerce. Para eso, solo navega a la sección requerida para ver la información que deseas.

También puedes actualizar datos del customer group, agregar notas, personalizar menús del storefront, configuración del customer group y eliminar grupos innecesarios.

![Ver Detalles del Customer Group](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/view_customer_group_details-1-768x392.png)

También puedes personalizar y personalizar el contenido de tu storefront para cada customer group estableciendo las restricciones de visibilidad necesarias, similar a lo que hemos hecho con customers (visibilidad de productos, visibilidad de categorías del master catalog y nodos de contenido del web catalog, etc.)

Solo hay una regla para recordar cuando configuras las restricciones. Solo un campo debe ser elegido para customers a la vez, ya sea un customer group o un customer.

![Visibilidad de Nodo del Web Catalog por Customer Group](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/web_catalog_node_visibility_customer_group-768x275.png)

Puedes seguir las instrucciones paso a paso proporcionadas en la sección anterior para aprender cómo individualizar contenido para un customer group, ya que el proceso es el mismo que para customers.

Con todas estas características, puedes configurar fácilmente el comportamiento necesario del storefront de tu sitio web para cada customer, customer user o customer group.