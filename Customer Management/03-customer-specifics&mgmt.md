# Especificidades y Gestión de Customers

## Tabla de Contenidos
- [Introducción](#introducción)
- [Configuración del Sistema](#configuración-del-sistema)
- [Creación de Customers](#creación-de-customers)
- [Organización de Jerarquía de Customers](#organización-de-jerarquía-de-customers)
- [Gestión de Customers](#gestión-de-customers)
- [Personalización del Menú Frontend para Customer](#personalización-del-menú-frontend-para-customer)
- [Configuración de Visibilidad de Contenido por Customer](#configuración-de-visibilidad-de-contenido-por-customer)
  - [Visibilidad de Productos](#visibilidad-de-productos)
  - [Visibilidad de Categorías del Master Catalog](#visibilidad-de-categorías-del-master-catalog)
  - [Visibilidad de Nodos de Contenido del Web Catalog](#visibilidad-de-nodos-de-contenido-del-web-catalog)
  - [Visibilidad de Landing Pages](#visibilidad-de-landing-pages)
  - [Visibilidad de Content Blocks](#visibilidad-de-content-blocks)

## Introducción

Mientras que los **customer users** son empleados que actúan en nombre de una empresa, los **customers** representan las mismas empresas para las que trabajan estos usuarios. Agregan todos los compradores relacionados con la misma organización de negocio. Los customers pueden ser agrupados en categorías con relaciones padre-hijo. Si, por ejemplo, una empresa tiene afiliadas en diferentes regiones o países, o ejecuta diferentes negocios, entonces puedes organizar tales customers en la jerarquía correspondiente. Esto puede simplificar significativamente tu proceso de gestión de clientes.

![Jerarquía de Customers](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/customers_hierarchy-1024x369.png)

## Configuración del Sistema

Similarmente a los customer users, el proceso de manejo de tus customers debe comenzar desde su configuración básica del sistema bajo **System > Configuration > Commerce > Customers**. Aquí, puedes configurar restricciones de visibilidad de productos y categorías, gestionar solicitudes de contacto y configurar consentimientos para back-office y storefront. Para hacer esto, navega a la configuración del sistema y habilita las configuraciones de customer requeridas. Una vez guardado, procede a los siguientes pasos de creación y gestión de customers.

![Configuración Global de Customer](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/global_customer_config-1-768x343.png)

Para comenzar a gestionar tus customers, navega a **Customers > Customers** en el menú principal. Aquí, puedes ver la lista de todos los customers disponibles con los que haces negocios.

![Lista de Customers](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/customers_list-1024x294.png)

Desde la cuadrícula All Customers, puedes crear nuevos customers, ver y editar detalles de customers, y exportar o importar customers haciendo clic en los botones relacionados.

## Creación de Customers

Los customers, así como los customer users, pueden ser creados de dos maneras, desde el storefront y back-office.

La primera forma es cuando un customer user registra una cuenta en el storefront. Ingresan el nombre de su empresa en el formulario de registro. Cuando el usuario es confirmado, el customer se agrega automáticamente a la lista de todos los customers. Este fue el caso con la empresa Twin Glass & Mirror cuando Jerry Blackwill, el primer gerente de compras, registró una cuenta a través del storefront. Tal forma de creación de customer carece de detalles, ya que el customer user solo menciona el nombre de la empresa. Usualmente significa que tus representantes de ventas tendrán que actualizar la información en el back-office para establecer los términos de pago necesarios y aplicar listas de precios si se requiere.

La segunda forma es cuando tus representantes de ventas crean customers en el back-office. Usualmente, se hace una vez que todas las condiciones de tus relaciones comerciales están confirmadas, y todos los acuerdos contractuales están firmados. De esta manera, sabes cómo configurar correctamente las configuraciones de tu customer, ya que los términos y condiciones pueden variar de customer a customer.

Para nuestro caso, actualicemos los detalles de la empresa Twin Glass & Mirror, suponiendo que hemos acordado venderles las puertas y ventanas con un 10% de descuento del precio predeterminado del sitio web bajo los términos de pago neto 10.

Para eso, navega a **Customers > Customers** en el menú principal, encuentra la empresa Twin Glass & Mirror en la lista, y haz clic en el ícono Edit al final de la fila para comenzar a editar la información.

![Editando Customer Parte 1](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/editing_customer_part1-1024x404.png)

En la sección General Information, proporciona los siguientes detalles:

1. **Selecciona el Owner** del customer. Por defecto, el campo está pre-poblado con el usuario que crea el customer, pero este valor puede ser cambiado a otro usuario del sistema haciendo clic en el menú hamburguesa y seleccionando un usuario de la lista.

2. **Selecciona una Account existente** para ayudar a rastrear acciones de ventas y métricas para el customer que es miembro de la organización de customer más grande. Cuando permanece vacío, una nueva account se crea para el nuevo customer automáticamente.

   **Nota:** Hablaremos más sobre accounts en la Sección 2.7.

3. **Completa el Name del customer**. En nuestro caso, fue poblado automáticamente junto con la confirmación del customer user.

4. **Opcionalmente, agrega un customer a un Customer Group** si ya tienes un grupo con las configuraciones y configuración que se ajusta al nuevo customer. Para nuestro caso, dejaremos este campo vacío ya que vamos a discutir customer groups en la siguiente sección.

5. **Selecciona un Parent Customer** si estás agregando una subsidiaria del customer existente. Como Twin Glass & Mirror es un customer padre en sí mismo, no seleccionaremos ninguno.

6. **Selecciona un Internal Customer Rating** ("1 de 5", "5 de 5") de la lista. Puede indicar rentabilidad potencial o cualquier otra puntuación o métrica acordada internamente.

7. **Asigna un Sales Representative** que asistirá a los customer users en el storefront.

8. **Selecciona un Tax Code** para etiquetar el esquema de tributación del grupo de customer.

9. **Agrega una Billing y Shipping Address**. Puedes agregar tantas como necesites. Todos los customer users que tienen el permiso para ver y editar direcciones de empresa pueden encontrar estas direcciones en su menú de cuenta en el storefront.

En la sección Price Lists, puedes construir una lista de precios agregada para cada sitio web que has configurado en OroCommerce. Usa pestañas para cambiar entre los sitios web, por ejemplo, Default, US, Australia, etc.

Para formar una lista de precios agregada:

1. **Selecciona la lista de precios** de la lista. Puedes agregar múltiples listas de precios, si es necesario, haciendo clic en **Add Price List** y luego estableciendo la prioridad arrastrando las listas hacia arriba o hacia abajo. Para nuestro caso, hemos seleccionado la lista de precios creada específicamente para este customer con el 10% de descuento acordado del precio predeterminado del artículo.

2. **Configura la opción de fallback** para proporcionar la fuente de precio si el precio no está disponible en las listas de precios configuradas directamente. Hay dos opciones disponibles:
   - **Customer group** – Significa que si no se encuentra un precio coincidente en las listas de precios creadas para el customer seleccionado, la aplicación va más allá a las listas de precios configuradas para el customer group para llenar el precio del producto faltante.
   - **Current customer only** – La aplicación busca el precio entre las listas de precios seleccionadas para el customer solo. Si no se encuentra precio, entonces no se muestra precio al customer en el storefront. Para nuestro caso, hemos establecido esta opción de fallback, ya que no hemos asignado nuestro customer a ningún customer group aún.

   **Nota:** Para más detalles sobre gestión de listas de precios y configuración de fallback, consulta nuestra extensa documentación en línea.

![Editando Customer Parte 2](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/editing_customer_part_2-1024x458.png)

En la sección Additional:

1. **Selecciona un Payment Term** para ser usado como una opción de pago disponible para los customer users durante el checkout. Para nuestro customer, hemos establecido el término de pago neto 10 como negociado previamente. Puedes dejar el campo vacío si no has confirmado los términos de pago con tu customer.

2. **Agrega el VAT ID** de tu customer, si es necesario. El VAT Id del customer debe ser capturado para su verificación de solvencia. El VAT Id debe ser válido, y la dirección de facturación debe coincidir con la proporcionada para el registro de VAT.

3. **Haz clic en Save** en la parte superior derecha para guardar los cambios que has hecho a tu customer.

Ahora, hemos completado la información faltante para nuestro customer Twin Glass & Mirror para hacerlo y sus customer users elegibles para compras a través del storefront según las condiciones y términos acordados.

## Organización de Jerarquía de Customers

Como hemos mencionado antes, puedes crear una jerarquía de unidades de negocio o divisiones de customer proporcionando una empresa padre al crear o editar los detalles de la empresa. Si asumimos que Twin Glass & Mirror tiene una división que vende ventanas en Canadá, entonces podemos crear un nuevo customer y vincularlo al padre.

Para esto:

1. **Haz clic en Create Customer** en la parte superior derecha de la página All Customers.

2. **Completa los detalles requeridos** siguiendo los pasos descritos en la sección anterior. Recuerda que tu customer hijo no necesariamente debe tener los mismos términos de pago, condiciones y descuentos de precio que tu customer padre. Puede tener configuraciones y configuración absolutamente únicas.

![Creando Customer Hijo](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/creating_child_customer-1-768x445.png)

3. **En la sección Parent Customer**, selecciona el requerido de la lista. Hemos seleccionado Twin Glass & Mirror.

4. **Haz clic en Save and Close**.

Una vez guardado, la empresa padre se muestra como un enlace bajo la sección General Information del customer hijo. Si haces clic en el enlace, serás redirigido a la página de tu customer padre.

![Enlace desde Customer Hijo a Padre](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/link_from_child_customer_to_parent-1-768x223.png)

Desde la página del customer padre, puedes ver todos los departamentos subsidiarios y divisiones conectados a él. Puedes crear un número ilimitado de customers hijos bajo el padre. Todos deben estar ubicados bajo la sección Subsidiaries.

## Gestión de Customers

Ahora averigüemos qué más podemos verificar y realizar desde la página de detalles del customer.

Cada página de customer agrega detalles sobre actividades, operaciones de eCommerce que sus customer users han realizado, el número de solicitudes enviadas, incluyendo cotizaciones, órdenes de venta y listas de compras. Proporciona acceso rápido a la estructura de la organización del customer, libreta de direcciones con vista previa del mapa, páginas de customer user, listas de precios habilitadas y un resumen de todas las cotizaciones, órdenes y listas. También puedes ver un resumen de las actividades de customer users navegando a la sección relevante.

![Ver Detalles del Customer](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/view_customer_details-1-768x250.png)

Adicionalmente, puedes actualizar los datos del customer si es necesario, ajustar sus configuraciones de configuración, personalizar el menú de storefront requerido, agregar archivos adjuntos, notas al customer, crear una subsidiaria, customer user, oportunidad, orden o cotización haciendo clic en el botón **More Actions** y seleccionando la acción requerida de la lista.

![Acciones del Customer](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/customer_actions-1-768x289.png)

## Personalización del Menú Frontend para Customer

Mientras que el proceso de editar detalles del customer o agregar notas puede parecer bastante directo, personalizar el menú frontend para un customer puede requerir explicación adicional.

El menú del storefront en OroCommerce constituye la navegación de tu storefront del sitio web, proporcionando una visión general de lo que ofreces, cómo contactarte, cómo acceder al carrito de compras y hacer una orden. Permite a los usuarios orientarse dentro de tu sitio web y acceder fácilmente a su cuenta, carrito de compras y otra información esencial a través de los enlaces distribuidos en diferentes lugares: junto al menú principal, en el pie de página, etc.

**Nota:** La configuración de menús está controlada por las capacidades Manage Menus y Access System Configuration bajo **System > User Management > Roles** en el menú del sistema del back-office.

Puedes modificar la configuración predeterminada para agregar nuevos elementos de menú, excluir algunos elementos de dispositivos específicos, o establecer las condiciones de visibilidad requeridas para un customer particular haciendo clic en **Edit Frontend Menu** en la parte superior derecha.

**Nota:** Actualmente, Frontend Menus incluye elementos de menú para todas las versiones de OroCommerce para propósitos de compatibilidad hacia atrás.

![Lista de Menú Frontend del Customer](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/customer_frontend_menu_list-1-768x504.png)

Usa pestañas para cambiar entre sitios web y modificar los elementos del menú para el sitio web al que el customer actual tiene acceso. Para Twin Glass & Mirror, vamos a usar el sitio web predeterminado, mientras que para la subsidiaria Canada BU, cambiaremos al sitio web de Canadá y configuraremos el menú del storefront allí.

![Configuración de Menú Frontend Canadá](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/frontent_menu_config_canada-1-768x234.png)

Cada elemento del menú es responsable de cierto contenido en tu sitio web. A continuación está la descripción ilustrativa de cada elemento en el storefront de muestra de OroCommerce para ayudarte a entender la diferencia entre cada elemento.

![Muestra del Menú Frontend](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/frontend_menu_sample-3-768x496.png)

Puedes personalizar cada menú para mostrar información específica. Por ejemplo, modifica el menú commerce_top_nav_refreshing_teal para mostrar el número de teléfono del representante de ventas, un chat en vivo y una opción de envío gratuito para un customer registrado, y solo la opción Contact Us para customers invitados.

![Actualizar Menú del Storefront](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/update_storefront_menu-768x339.png)

Los customers invitados que llegan a tu sitio web verán el siguiente menú de navegación superior:

![Menú Frontend para Invitados](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/frontend_menu_for_guests-1-768x302.png)

Sin embargo, una vez registrados, verán otro menú:

![Menú Frontend para Customers Registrados](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/frontend_menu_for_registered_customers-1-768x322.png)

**Nota:** Para más detalles sobre cómo gestionar menús frontend y configurar sus configuraciones en diferentes niveles, no solo por customer, consulta nuestra documentación en línea.

Una vez que hayas configurado los elementos del menú, puedes agregarlos a la configuración del tema seleccionado de tu sitio web, colocándolos en cualquier lugar en el encabezado del storefront.

![Configuración del Tema](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/theme_configuration-768x436.png)

**Nota:** Para más detalles sobre cómo personalizar la configuración del tema, consulta nuestra documentación en línea.

De esta manera, puedes personalizar y optimizar cualquier elemento del menú y tu navegación general del sitio para el uso conveniente de tus customers.

## Configuración de Visibilidad de Contenido por Customer

En OroCommerce, puedes controlar qué productos, categorías, nodos o landing pages son visibles para tus customers estableciendo restricciones de visualización. Este enfoque personalizado permite que cada customer vea descuentos, promociones y productos individuales cuando inician sesión.

Puedes gestionar la visibilidad de categorías del master catalog o productos individuales, así como establecer restricciones de visualización a varios contenidos, tales como:

### Visibilidad de Productos

La visibilidad de productos en OroCommerce determina si los customers pueden ver un producto en un sitio web particular. Esto es importante para personalizar tu storefront a diferentes sitios web, customers o customer groups.

Para gestionar la visibilidad de productos, ve a **Products > Products**, selecciona el producto, haz clic en **More actions** y elige **Manage Visibility**. Puedes establecer visibilidad por sitio web, customer group o customer individual.

![Gestionar Visibilidad de Producto](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/ProductManageVisibility-768x279.png)

Por defecto, la visibilidad del producto cae en las configuraciones de visibilidad de la categoría del master catalog asignada a menos que se especifique lo contrario.

![Visibilidad de Producto Predeterminada](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/default-product-visibility-768x202.png)

Puedes cambiar entre sitios web en la página de visibilidad del producto y aplicar los cambios necesarios.

Para nuevos sitios web, se aplican las siguientes configuraciones predeterminadas:

- **Visibility to All** define las configuraciones generales de visibilidad para el producto seleccionado en el sitio web elegido.
- **Product Visibility to Customer Groups** define configuraciones de visibilidad para el producto seleccionado para customer groups específicos.
- **Product Visibility to Customers** define configuraciones de visibilidad para el producto seleccionado para customers individuales.

Por defecto, los customers heredan la configuración de visibilidad del producto del customer group al que están asignados. Puedes cambiar este comportamiento seleccionando cualquier otro valor del menú desplegable.

Las opciones disponibles son:

- **Customer group** – Hereda la configuración de visibilidad del producto del customer group al que está asignado el customer seleccionado, lo que significa que coincide con las configuraciones definidas bajo la sección Product Visibility to Customer Groups para este producto. Es la opción predeterminada para cualquier nuevo customer.
- **Current product** – Hereda la configuración de visibilidad del producto predeterminada, lo que significa que coincide con las configuraciones definidas bajo la sección Visibility to All para este producto.
- **Category** – Hereda la configuración de la categoría del master catalog a la que está asignado el producto seleccionado. Significa que las configuraciones de visibilidad del producto actual igualan el valor definido en el campo Category Visibility to Customers de la categoría del master catalog relacionada.
- **Hidden** – El producto está oculto del storefront para el customer seleccionado.
- **Visible** – El producto es visible para el customer seleccionado en el storefront.

![Visibilidad de Producto a Customers](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/product-visibility-to-customers-768x792.png)

**Nota:** Para más detalles sobre cómo configurar y gestionar restricciones de visibilidad de productos en diferentes niveles, consulta nuestra documentación en línea.

### Visibilidad de Categorías del Master Catalog

El master catalog organiza los productos de tu tienda en categorías. Usando restricciones de visibilidad, puedes controlar qué categorías ven los customers y sus usuarios en el storefront. Puedes agrupar productos específicos en una categoría (por ejemplo, Productos con Descuento para Twin Glass & Mirror) y establecer restricciones de visibilidad para toda la categoría, personalizando su visualización para diferentes customers.

Para hacer esto, navega a **Products > Master Catalog**, selecciona la categoría y encuentra la sección Visibility. Aquí, puedes establecer restricciones de visibilidad para todos los visitantes del sitio web, customer groups específicos o customers individuales moviéndote de pestaña en pestaña.

Selecciona la opción necesaria de la lista:

- **Customer Group** — Hereda la configuración de visibilidad de la categoría del customer group al que está asignado el customer seleccionado, lo que significa que coincide con las configuraciones definidas bajo la sección Category Visibility to Customer Groups para esta categoría. Por defecto, esta configuración está pre-poblada para cualquier nuevo customer.
- **Visibility to All** — Hereda la configuración de visibilidad de la categoría predeterminada, lo que significa que coincide con las configuraciones definidas bajo la sección Category Visibility to All para esta categoría.
- **Parent Category** — Hereda la configuración de la categoría padre del master catalog. Significa que las configuraciones de visibilidad de la categoría actual igualan el valor definido en el campo Category Visibility to Customers de la categoría padre del master catalog. Esta opción está disponible solo para categorías no raíz.
- **Hidden** — La categoría está oculta del storefront para el customer seleccionado.
- **Visible** — La categoría es visible para el customer seleccionado en el storefront.

![Visibilidad del Master Catalog por Customer](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/master_catalog_visibility_per_customer-2-768x302.png)

Una vez que se selecciona la opción requerida, haz clic en **Save**.

**Nota:** Para más detalles sobre cómo configurar y gestionar la visibilidad de tu master catalog, consulta nuestra documentación en línea.

### Visibilidad de Nodos de Contenido del Web Catalog

Por defecto, el web catalog y sus nodos son visibles para todas las localizaciones, sitios web y customers. Sin embargo, puedes restringir nodos específicos para que sean visibles solo para ciertos customers. Por ejemplo, puedes limitar el nodo Timber Windows para que se muestre exclusivamente a Twin Glass & Mirror, evitando que otros customers lo vean.

Para configurar esto, ve a **Marketing > Web Catalog**, selecciona el web catalog requerido y haz clic en **Edit Content Tree**. Elige el nodo de contenido, desplázate a la sección Restrictions, desmarca **Inherit Parent** y selecciona el customer deseado (por ejemplo, Twin Glass & Mirror). Luego, guarda los cambios.

![Visibilidad de Nodo del Web Catalog por Customer](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/web_catalog_node_visibility_per_customer-1-768x299.png)

**Nota:** Para más detalles sobre cómo configurar y gestionar web catalogs, consulta nuestra extensa documentación en línea.

### Visibilidad de Landing Pages

Las restricciones de tus landing pages siguen la misma lógica de configuración que para los nodos de contenido del web catalog. Para hacer que aparezca una landing page en tu sitio web, primero debes agregarla como una variante de contenido a un nodo de contenido. Luego, establece las restricciones correspondientes en la sección Content Variants del nodo requerido, como se muestra a continuación.

![Visibilidad de Landing Page por Customer](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/landing_page_visibility_per_customer-1-768x363.png)

De esta manera, la página de bienvenida que se supone debe mostrarse a los customer users de la empresa Twin Glass & Mirror, se mostrará a ellos una vez que inicien sesión en sus cuentas en el storefront.

Puedes agregar un número ilimitado de landing pages y condiciones para mostrar contenido único a cada customer haciendo clic en el botón **Add** debajo del campo Restrictions.

**Nota:** Para más detalles sobre cómo crear y gestionar landing pages, consulta nuestra documentación en línea.

### Visibilidad de Content Blocks

La información mostrada en content blocks también puede ser restringida a ciertos customers y sus usuarios asignados.

Para hacer esto, navega a **Marketing > Content Blocks**, selecciona el bloque deseado y haz clic en **Edit**. En la sección Restrictions, elige el customer para la variante de contenido predeterminada. Si el bloque tiene múltiples variantes, aplica restricciones adicionales a cada variante no predeterminada para evitar conflictos. Asegúrate de que todas las variantes no predeterminadas tengan restricciones para prevenir colisiones de prioridad con el contenido predeterminado.

![Visibilidad de Content Block por Customer](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/content_block_visibility_per_customer-1-768x188.png)

**Nota:** Para más detalles sobre cómo crear y gestionar content blocks, consulta nuestra documentación en línea: https://doc.oroinc.com/user/concept-guides/content-management/content-blocks/