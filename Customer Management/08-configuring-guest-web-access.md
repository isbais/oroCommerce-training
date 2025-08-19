# Configuración de Acceso Web para Invitados

## Tabla de Contenidos
- [Introducción](#introducción)
- [Configuración del Sistema](#configuración-del-sistema)
- [Funcionalidades de Invitados](#funcionalidades-de-invitados)
  - [Website Access](#website-access)
  - [Quick Order Form](#quick-order-form)
  - [Shopping List](#shopping-list)
  - [Request For Quote](#request-for-quote)
  - [Checkout](#checkout)
  - [Contacts](#contacts)
  - [Quotes](#quotes)

## Introducción

Trabajar con OroCommerce te permite adaptar la funcionalidad a tus necesidades específicas de negocio, ya sea B2B, B2C o ambos. Te damos una herramienta poderosa que se adapta a tus estrategias.

En secciones anteriores, cubrimos customers B2B y los beneficios de gestionar accounts desde el storefront. Sin embargo, tu negocio también puede dirigirse a customers B2C que hacen compras únicas. Los consumidores B2C típicamente son **guest customers**—visitantes no autenticados que llegan a tu sitio web y rápidamente hacen compras sin registrarse. OroCommerce soporta sus necesidades, permitiéndote personalizar contenido, productos, precios, descuentos y promociones específicamente para usuarios invitados.

Esta sección te guiará a través de habilitar la funcionalidad de invitados, permitiendo a usuarios no registrados acceso parcial o completo a características como navegar, ver productos, verificar precios, crear listas de compras, realizar órdenes y hacer checkout como invitados y registrarse después.

![Acceso Total](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/total_access-1.png)

O puedes restringir completamente el acceso de usuarios invitados al sitio web a menos que se registren.

![Sin Permisos](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/no_permissions-1-768x424.png)

## Configuración del Sistema

Antes de personalizar el contenido y establecer precios especiales de productos para tus usuarios invitados, primero necesitas habilitar varias características de invitados en la configuración del sistema para controlar la actividad de usuarios invitados en el storefront.

**Nota:** Si no tienes acceso a la configuración del sistema de la aplicación Oro, puedes pedir ayuda a un administrador.

La gestión flexible del acceso al sitio web te da la posibilidad de personalizar cada aspecto de tu storefront del sitio web para soportar la actividad de visitantes invitados, desde navegar el sitio web y agregar los productos seleccionados a una lista de compras hasta completar su orden.

Para eso:

1. **Navega a la configuración del sistema** bajo **System > Configuration**. Las configuraciones que se refieren a la funcionalidad de invitados se pueden modificar en tres niveles: global, organización y sitio web. Actualmente, nos enfocamos solo en la configuración global, implicando que las mismas opciones también están disponibles para personalización en otros niveles.

   **Nota:** Para más detalles sobre los niveles de configuración utilizados en las aplicaciones Oro, consulta nuestra documentación en línea: https://doc.oroinc.com/user/back-office/system/configuration/

2. **Una vez que llegues a la configuración del sistema**, escribe **guest** en la barra de búsqueda para reducir la lista de funciones de invitados.

![Funciones de Invitados](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/guest_functions-1-768x409.png)

Veamos a qué se refiere cada una de ellas.

## Funcionalidades de Invitados

### Website Access

La configuración habilita o deshabilita el acceso al sitio web para invitados para controlar la interacción de customers invitados con tu sitio web. Cuando esta opción está deshabilitada, la única página a la que los usuarios no registrados pueden acceder es la página de inicio de sesión.

### Quick Order Form

La configuración promueve compras rápidas a través del menú de acceso rápido en el storefront. Por defecto, el formulario de orden rápida está habilitado para customers registrados, mientras que el formulario de orden rápida para invitados está deshabilitado y no se muestra en el storefront. Puedes cambiar este comportamiento si es necesario. Ten en cuenta que para que se muestre el formulario de orden rápida, al menos una de las siguientes opciones también debe estar habilitada: lista de compras de invitados, RFQ de invitados o checkout de invitados.

![Habilitar Formulario de Orden Rápida para Invitados](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/enable_guest_quick_order_form-1-768x395.png)

### Shopping List

La configuración le da a un usuario invitado la posibilidad de comprar un producto agregándolo a la lista de compras. Ten en cuenta que solo 1 lista de compras está disponible para un customer invitado, y puede ser almacenada por hasta 30 días en un solo navegador.

### Request For Quote

La configuración habilita a usuarios anónimos a solicitar una cotización sobre los artículos de productos que les interesan desde la página de lista de compras y desde la página de detalles del producto. Para que la opción funcione correctamente, asegúrate de habilitar la característica de lista de compras de invitados mencionada antes.

### Checkout

La configuración soporta checkouts anónimos que no interrumpen la compra forzando a registrarse una cuenta. Sin embargo, los usuarios invitados aún pueden registrarse para una cuenta, si lo desean, después de completar el checkout. El proceso de checkout para usuarios invitados es idéntico al de los usuarios registrados. La única diferencia es que los usuarios invitados están obligados a ingresar sus datos manualmente ya que no hay información pre-llenada disponible en los formularios de checkout. Para una experiencia completa de checkout de invitados, se recomienda habilitar listas de compras de invitados, formulario de orden rápida de invitados y solicitudes de cotización de invitados.

Al proceder a través del checkout, los customers no autenticados pueden elegir si desean registrarse, iniciar sesión o continuar como invitados.

![Habilitar Checkout de Invitados](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/enable_guest_checkout-1-768x332.png)

### Contacts

La configuración te permite ingresar la información de contacto necesaria que se mostrará a visitantes no registrados. En lugar de proporcionar los contactos de tu empresa a todos los customers anónimos, puedes usar este campo para pedir registro y mostrar el contacto de tus representantes de ventas que pueden manejar cualquier problema de customers invitados.

![Habilitar Detalles de Contacto para Invitados](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/enable_guest_contact_details-1-768x684.png)

### Quotes

La configuración genera enlaces únicos que se usan para enviar cotizaciones a usuarios invitados proporcionando que el acceso al sitio web para invitados y el checkout de invitados estén habilitados para que los invitados vean y acepten las cotizaciones.

Una vez que una cotización está lista, puede ser enviada a la dirección de correo electrónico del customer invitado. El formulario de envío genera un enlace al que el usuario puede acceder para ver y aceptar la cotización si es necesario.

![Enviando Cotización de Invitado](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/sending_guest_quote-1-768x509.png)

El formulario de cotización para usuarios invitados se ve como sigue:

![Muestra de Cotización de Invitado](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/guest_quote_sample-1-768x466.png)

Por defecto, todas estas características de invitados están deshabilitadas en todos los niveles. Asegúrate de habilitar las requeridas para permitir que los customers invitados interactúen con tu sitio web, soliciten cotizaciones y realicen órdenes sin registrarse.

**Nota:** Para más detalles sobre cómo configurar cada característica de invitados individualmente, consulta nuestra documentación en línea: https://doc.oroinc.com/user/back-office/system/configuration/commerce/