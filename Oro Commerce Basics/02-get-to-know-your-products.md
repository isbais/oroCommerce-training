# Conoce tus Productos

## Tabla de Contenidos
- [Introducción](#introducción)
- [Tipos de Productos](#tipos-de-productos)
- [Product Families](#product-families)
- [Recursos Adicionales](#recursos-adicionales)

## Introducción

Puedes crear tres tipos de productos en OroCommerce: **simple**, **configurable** y **product kit**. El tipo de producto seleccionado en el primer paso de la creación del producto determina la forma en que la información del producto se usa y gestiona posteriormente en la aplicación.

## Tipos de Productos

### Simple Product

Un **simple product** es un producto ordinario. Tiene un **SKU** único y el conjunto de detalles del producto que pueden variar según la **product family** a la que pertenece un producto. Puedes gestionar la información del inventario y el precio para un simple product. Un ejemplo de un simple product es un paquete de papel para copiadora que no tiene variaciones de color o tamaño.

### Configurable Product

Un **configurable product** agrupa varios simple products (variantes del configurable product) cuya información se superpone en su mayoría, excepto por varios atributos del producto que diferencian estos simple products. Como el configurable product y todas sus variantes comparten el mismo conjunto de atributos, deben compartir la **product family**.

Un ejemplo de un configurable product puede ser un paquete de papel para copiadora disponible en varios colores y tamaños. Este paquete puede contener 100, 300 o 500 hojas y venir en colores blanco, azul, verde o rojo. En el storefront, tal producto con todas sus variaciones de tamaño y color se muestra como un **matrix ordering form**. Puedes leer más sobre matrix forms en la sección correspondiente de la guía del storefront en la biblioteca de documentación de Oro.

### Product Kit

Un **product kit** es un surtido de productos, cada uno con sus **SKUs** individuales. Cada producto en este paquete de surtido puede ser obligatorio u opcional para que los compradores compren para proceder a través del checkout. Un ejemplo de un product kit sería una lámpara con una selección de accesorios opcionales para ella, como bombillas de repuesto de diferentes vatios.

## Product Families

Hemos mencionado anteriormente que los detalles del producto varían según la **product family**. En resumen, una product family es un conjunto de **product attributes** que almacenan información completa sobre productos de tipo similar. Entonces, por ejemplo, una grapadora y una impresora láser pueden compartir algunos atributos genéricos, como un nombre o una marca, y diferir en el conjunto de atributos restante. Para una grapadora, estos atributos pueden ser capacidad de hojas y tipo de tira, mientras que para una impresora, estos pueden ser velocidad, resolución o el tipo del puerto USB. Estos atributos pueden, por supuesto, crearse dependiendo de tus necesidades. También se puede agregar una nueva product family. Sin embargo, por defecto, OroCommerce viene con una product family predeterminada que almacena todos los **system attributes**. Estos system attributes son obligatorios para cualquier product family ya que contienen detalles esenciales del producto.

## Recursos Adicionales

Nuestra biblioteca de documentación contiene más información sobre **product families** y **attributes**. La biblioteca de medios de Oro también tiene un video sobre la creación de simple products en tu aplicación.
