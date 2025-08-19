# Introducción a la Funcionalidad de Gestión de Clientes de Oro

## Tabla de Contenidos
- [Introducción](#introducción)
- [Entidades Principales de Clientes](#entidades-principales-de-clientes)
- [Distinciones Conceptuales](#distinciones-conceptuales)
  - [Accounts](#accounts)
  - [Customers](#customers)
  - [Business Customers](#business-customers)
  - [Contacts](#contacts)
- [Resumen](#resumen)

## Introducción

El poder del comercio está en construir relaciones sólidas entre clientes y empresas. La gestión estándar de clientes abarca todos los sistemas, procesos y software necesarios para administrar estas relaciones, mantener y mejorar el vínculo comprador-vendedor. La construcción de relaciones es una inversión a largo plazo, pero los beneficios están garantizados si se hace correctamente.

La plataforma Oro ha cuidado bien la filosofía del cliente y ha desarrollado un sistema avanzado centrado en el cliente para vender, entregar, recopilar datos y apoyar a los clientes a lo largo de su viaje. Allí, puedes encontrar fácilmente todas las tareas, estimaciones, hitos, interacciones e información de contacto relacionada con tu cliente. Con OroCommerce, puedes gestionar tus clientes desde diferentes perspectivas, almacenar todo su historial de compras, valor de ventas de por vida, actividad de marketing, referencias a leads y oportunidades en un lugar fácilmente accesible. Es muy conveniente tener una sola ubicación para esta información agregada, ya que reduce considerablemente el tiempo dedicado a la gestión general de clientes.

Para trabajar con clientes en Oro, necesitas entender cómo Oro representa a los clientes, así como sus especificidades y distinciones, para asegurar que la información necesaria se muestre a la persona correcta. Estos datos también te permitirán rastrear información sobre empresas y personas y mantenerla actualizada.

Esta sección te ayudará a:

- Familiarizarte con los conceptos de **customer**, **customer user**, **customer groups**, **roles**, **accounts** y **contacts**.
- Aprender la diferencia conceptual y las relaciones entre ellos.

Para comenzar, te presentaremos un escenario de ejemplo que se ejecutará a lo largo del curso. Nuestro ejemplo se basa en una empresa estadounidense que vende ventanas, puertas y productos de seguridad para el hogar a clientes mayoristas, minoristas y visitantes. También te proporcionaremos varias tareas prácticas para ayudarte a retener mejor la información proporcionada y el material de aprendizaje.

## Entidades Principales de Clientes

Comencemos presentándote las principales entidades de clientes que residen bajo el menú principal **Customers** en el back-office de Oro.

Estas son:

- **Accounts**
- **Contacts**
- **Customers**
- **Customer Groups**
- **Customer Users**
- **Business Customers**

![Menú de Clientes](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/customer_menu-1-768x404.png)

Estas entidades representan personas y empresas en la aplicación Oro. Sin embargo, su disponibilidad en el menú depende del tipo de aplicación que uses y tus permisos de rol.

En las aplicaciones Oro, una **account** representa una empresa. Los **customers** representan negocios, divisiones y afiliadas que esta empresa puede tener. Típicamente, los customers tienen uno o más **customer users** asociados con ellos, mientras que los **business customers** pueden tener solo un contacto representativo. Estos son individuos dentro de la empresa que actúan en su nombre.

## Distinciones Conceptuales

Aunque la información en **Accounts**, **Contacts** y **Customers** puede parecer similar, hay algunas distinciones conceptuales:

### Accounts

Una **account** agrega datos de todos los canales y todas las fuentes (por ejemplo, **Contacts**, **Business Customers**, **Commerce Customers**), proporcionando una vista de 360 grados de toda la información sobre la empresa con la que trabajas. Todas las interacciones con un cliente particular se muestran en una sola página donde también puedes rastrear sus actividades de marketing, ventas a través de oportunidades, y asignar etiquetas correspondientes para organizar las accounts en categorías lógicas y subcategorías.

![Ejemplo de Account](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/account_record_example-1024x516.png)

### Customers

Un **customer** acumula la información sobre el negocio con el que tratas. Aquí, puedes ver los detalles de cada subsidiaria relacionada, **customer users** y su actividad de comercio electrónico. También puedes verificar los detalles de las solicitudes de cotización enviadas, cotizaciones y órdenes realizadas, así como todas las notas, intercambios de correo electrónico y otras cadenas de negociación.

![Ejemplo de Customer](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/customer_record_example-1024x465.png)

### Business Customers

Un **business customer** representa el negocio con el que estás interactuando pero que no requiere tener una cuenta en tu storefront. Un ejemplo sería una empresa de limpieza que proporciona servicios de limpieza diaria de oficinas a tu empresa. No compra nada de tu tienda, pero sus detalles deben registrarse en tu back-office para fines de rastreo de contactos y contabilidad. Otro caso es cuando operas un sistema ERP externo para procesar órdenes, cotizaciones y pagos, pero necesitas una forma de registrar tus clientes en tu aplicación. Aquí es donde la funcionalidad de business customer resulta útil. Ten en cuenta que la función de business customer no está habilitada por defecto. Si necesitas habilitarla para tu negocio, debes configurar un canal de ventas relacionado primero. Encontrarás más detalles en el tema dedicado **Business Customers** más abajo.

![Ejemplo de Business Customer](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/business_customers_example-1024x404.png)

### Contacts

Un **contact** se usa para asociar una persona con un **business customer** o **account** específico. Contiene la información personal del cliente, su posición en la empresa, información de dirección y otros datos relacionados.

![Ejemplo de Contact](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/contact_record_example-1024x595.png)

La principal diferencia entre un **contact** y un **customer user** es que un contact representa una persona que puede no usar el segmento Commerce (por ejemplo, el CEO de una empresa que no compra nada personalmente o el administrador de una empresa).

## Resumen

Esta fue una pequeña visión del concepto de gestión de clientes que se puede implementar en la plataforma Oro. En las próximas secciones, profundizaremos en cada entidad que participa en el proceso de gestión de clientes, enfocándonos en sus especificidades y características distintivas. También consideraremos las capacidades de la plataforma Oro que ayudan a construir un servicio al cliente integral, permitiendo que los clientes seleccionados tengan acceso completo o parcial a tu sitio web o sus páginas y contenido específicos.  

