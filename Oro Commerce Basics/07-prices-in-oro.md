# Entender Precios en OroCommerce

## Tabla de Contenidos
- [Introducción](#introducción)
- [Gestión de Price Lists](#gestión-de-price-lists)
- [Definiciones Clave](#definiciones-clave)
- [Price Lists](#price-lists)
- [Currencies](#currencies)
- [Tier Price](#tier-price)
- [Combinando Price Lists](#combinando-price-lists)
- [Auto-generated Price Lists](#auto-generated-price-lists)
- [Price List Calculation](#price-list-calculation)
- [Recursos Adicionales](#recursos-adicionales)

## Introducción

La gestión de **price lists** es uno de los aspectos más importantes de cualquier negocio de e-Commerce y aún más para las empresas de e-Commerce Business to Business (B2B). Los negocios B2B requieren un alto nivel de flexibilidad para soportar los casos de uso más avanzados, incluyendo un enfoque altamente estructurado para la gestión de cuentas y procesos de ventas versátiles que a menudo se personalizan según las necesidades de **customer groups** específicos o cuentas grandes individuales. Es por eso que creamos OroCommerce con una de las características de gestión de price lists más avanzadas.

En general, la gestión de precios en OroCommerce te permite:

- Configurar precios de productos flexibles para diferentes sitios web, **customer groups** y clientes.
- Asignar precios para productos recién agregados automáticamente.
- Programar cambios de precio temporales o permanentes.
- Anular el precio asignado automáticamente con el valor ajustado manualmente.

## Gestión de Price Lists

Echa un vistazo rápido a las definiciones clave relacionadas con precios a continuación antes de pasar al lado práctico de agregar precios a tus productos.

## Definiciones Clave

### Price Lists

Una **price list** es una lista de cantidades de productos con sus precios en una o más **base currencies**. Las price lists se usan para determinar precios para productos del catálogo en el storefront. Por ejemplo, puedes tener una o múltiples price lists con precios ingresados en dólares estadounidenses y euros definiendo el pricing para todos tus clientes, una price list diferente con precios en dólares estadounidenses disponible solo para tus distribuidores estadounidenses de gran volumen, y otra price list con precios en euros disponible solo para algunos socios europeos seleccionados de tu empresa. También puedes crear una price list para clientes que compran a granel, dándoles un descuento del 10% debido a su estado de **Bulk Supplier**.

Una **calculated price list** (también llamada **combined price list**) es una representación interna de todos los precios disponibles para un cliente seleccionado (todos los **customer users**) en el storefront. Por ejemplo, cuando uno de tus clientes inicia sesión en el storefront, pueden ver precios tanto para el producto A como para el producto B, donde los precios del producto A se toman de la price list predeterminada disponible para todos, y los precios del producto B se toman de una price list personalizada que has creado para anular el pricing del producto B solo para este cliente específico. Aunque puedes ver todas las price lists y cambiar entre ellas en tu back-office de la tienda, tus clientes solo pueden ver esos precios en el storefront que les has hecho disponibles configurando price lists y sus configuraciones.

### Currencies

La **base currency** es la moneda de entrada de precio en una price list. Una **display currency** es una moneda que se usa para mostrar precios a un cliente. El storefront usa el valor exacto ingresado por el **price manager** cuando un cliente requiere precios en una display currency seleccionada y los precios en la misma base currency están disponibles en la calculated price list. Si la price list no tiene un precio en la moneda seleccionada, entonces se deben usar reglas adicionales de conversión de moneda.

### Tier Price

Un **tier price** es un precio determinado por el sistema para la cantidad de producto especificada. Por ejemplo, si configuras los siguientes precios en la price list:

- Producto A, 1 pieza, $100.00
- Producto A, 10 piezas, $90.00

El sistema usará $90.00 como precio por pieza cuando un cliente compre 10 o más piezas, y $100.00 como precio por pieza cuando un cliente compre 9 o menos piezas.

Los **price tiers** para un producto seleccionado pueden derivarse de la misma price list, o de diferentes price lists, si la **price tier merging** está habilitada. Revisa más información sobre price tier merging en el tema de configuración de price list en la biblioteca de documentación de Oro.

## Combinando Price Lists

La **price list priority** determina el orden en el que se deben combinar los precios de productos cuando hay precios para el mismo price tier en múltiples price lists disponibles para un cliente.

Por ejemplo:

- Especificaste $90.00 como precio unitario para 10 o más conjuntos del Producto A en la Price List 1, y $85.00 como precio unitario para 10 o más conjuntos del mismo Producto A en la Price List 2, y ambas price lists están disponibles para un cliente.
- Si la Price List 1 tiene una prioridad más alta que la Price List 2, el cliente verá $90.00 como precio unitario al comprar 10 o más conjuntos del Producto A.
- De lo contrario, el cliente verá $85.00 como precio unitario para 10 o más conjuntos del Producto A.

**Merge Allowed** es una configuración de price list que define si el sistema debe combinar price tiers del mismo producto de múltiples price lists. Esta configuración se muestra como opción **Merge Allowed** junto a los nombres de las price lists en las páginas de edición de cliente, customer group, sitio web, o en la página de configuraciones de pricing (**System Configuration > Catalog > Pricing**).

Por ejemplo, si especificaste un precio para 1 artículo del Producto A en la Price List 1, y el precio para 10 artículos del Producto A en la Price List 2, entonces, si tanto la Price List 1 como la Price List 2 están disponibles para un cliente, verán dos price tiers. El primer price tier será para artículos "1 a 9", y el segundo price tier será para "10 o más" artículos.

Si decidiste no fusionar price lists, y la Price List 2 tiene mayor prioridad que la Price List 1, entonces los clientes para quienes ambas price lists están disponibles, verán solo el price tier para "10 o más" artículos.

**Price list fallback** es una configuración que habilita el acceso a price lists de nivel superior. Por ejemplo, si el artículo de un cliente no está disponible en la price list configurada, puede recurrir a obtener el precio del grupo al que pertenece el cliente. Una price list puede no estar disponible debido a mantenimiento, o la promoción para el precio de venta ya no es válida.

Otro ejemplo:

En la configuración predeterminada, todos los **customer users** tienen acceso a todas las price lists asignadas a sus clientes y las price lists asignadas al **customer group** al que pertenece su cliente, así como a las price lists asignadas al sitio web que están navegando actualmente y las price lists predeterminadas configuradas a nivel del sistema.

Si deshabilitas la configuración de fallback a nivel del cliente y asignas una price list seleccionada a un cliente, esta price list se convierte en la única price list de la que los usuarios de este cliente verán los precios. En este caso, el pricing del customer group, el pricing del sitio web y el pricing predeterminado a nivel del sistema ya no estarán disponibles para los usuarios de este cliente.

Si deshabilitas la configuración de fallback a nivel del customer group, entonces todos los clientes que pertenecen a este customer group ya no tendrán acceso al pricing del sitio web y el pricing predeterminado a nivel del sistema.

## Auto-generated Price Lists

En OroCommerce, puedes configurar una price list que sea flexible, ajustable y que coincida exactamente con tu estrategia de pricing.

Con el **automated pricing** que puede depender de indicadores clave, como disponibilidad del producto, precio recomendado y costo de producción, obtienes la price list completa para miles y millones de artículos lista literalmente en ningún momento.

Los productos entran automáticamente en la price list siempre que coincidan con los criterios especiales: una **price list product assignment rule**. Puedes configurar reglas de pricing flexibles, por ejemplo, para cumplir con los requisitos de regulaciones de precios, mantener una price list internacional consciente de la ubicación, o para estimular la demanda y actualizar el precio siguiendo las tendencias de disponibilidad de stock.

## Price List Calculation

Para proporcionar una experiencia de usuario optimizada en el storefront y en el back-office, y mantener el nivel deseado de rendimiento del sistema, proporcionamos una forma de afinar el comportamiento del cálculo de price list.

OroCommerce realiza una parte no consumidora de recursos del recálculo de precios inmediatamente después de que el cambio de precio es enviado por el usuario en el back-office (por ejemplo, cuando un usuario envía el formulario de edición del producto, o agrega un precio a través de la gestión de price list, o modifica la prioridad de price list en una página de edición de cliente, etc.).

La parte consumidora de recursos del recálculo (por ejemplo, cuando la fórmula de auto-cálculo de precio depende del atributo del artículo que no está directamente relacionado con el producto) se difiere y ocurre en un horario que se define usando el valor **Offset Of Processing CPL Prices** en horas.

A partir de la versión 6.0, OroCommerce permite a los usuarios con permisos correspondientes ver toda la información de pricing en un lugar bajo la sección **Sales > Price Calculation Details** en el menú principal.

## Recursos Adicionales

Antes de continuar leyendo, también puedes revisar un video sobre cómo configurar price lists en tu aplicación en la biblioteca de medios de Oro, o leer sobre pricing en nuestra biblioteca de documentación.

Ahora procedemos a agregar precios a los productos subiendo la price list en masa a tu aplicación.
