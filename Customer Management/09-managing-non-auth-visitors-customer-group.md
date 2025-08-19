# Gestión del Customer Group de Visitantes No Autenticados

## Tabla de Contenidos
- [Introducción](#introducción)
- [Customer Group de Visitantes No Autenticados](#customer-group-de-visitantes-no-autenticados)
- [Configuración de Visibilidad de Contenido para Customers Invitados](#configuración-de-visibilidad-de-contenido-para-customers-invitados)
- [Permisos para el Customer Group de Visitantes No Autenticados](#permisos-para-el-customer-group-de-visitantes-no-autenticados)

## Introducción

Una vez que hayas configurado todas las opciones generales del sistema para tus customers invitados, puedes pasar al siguiente paso y definir las configuraciones necesarias para el customer group de invitados.

En la Sección 2.4, te presentamos el concepto de customer groups y su funcionalidad. Ahora, vamos a elaborar más sobre uno de los componentes del customer group. Con eso, nos referimos al customer group **Non-Authenticated Visitors**.

El customer group **Non-Authenticated Visitors** es el único customer group predeterminado pre-configurado que aparece en el sistema una vez que instalas la aplicación.

![Customer Group de Visitantes No Autenticados](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/non_authenticated_visitors_customer_group-1-768x211.png)

Otros grupos se agregan manualmente dependiendo de la necesidad y requisitos.

El customer group **Non-Authenticated Visitors** agrega automáticamente todos los customers anónimos y customer users de tu sitio web. Puedes asignar adicionalmente los customers requeridos a este grupo si es necesario.

El proceso de gestión de este customer group es idéntico al que hemos descrito previamente en las secciones sobre customer groups.

En resumen, puedes:

- **Editar los detalles del grupo**, como el nombre, owner, tax code, términos de pago
- **Agregar customers relacionados**
- **Asignar listas de precios de invitados** y establecer la opción de fallback requerida para que todos los usuarios no registrados de tu sitio web puedan ver los precios personalizados dirigidos específicamente a ellos.

Es importante mencionar aquí que la lógica de configuración de fallback de precios para usuarios no registrados difiere de la de los customers registrados:

**Non-Authenticated Visitors Customer Group Price List > Current Website PLs > Global PLs**. Significa que si no se encuentra un precio coincidente en la lista de precios creada para el customer group de invitados, la aplicación va más allá a las listas de precios configuradas en los niveles del sitio web y sistema para llenar el precio del producto faltante.

Mientras que para los usuarios registrados, la cadena de fallback es: **Current Customer PLs > Current Customer Group PLs > Current Website PLs > Global PLs**.

- **Editar elementos del menú frontend**, que te permiten personalizar la navegación, contenido y elementos del menú de tu storefront para tus customers invitados.
- **Editar configuración por customer group**.

![Viendo la Página del Customer Group No Autenticado](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/viewing_non_authenticated_customer_group_page-1-768x400.png)

## Configuración de Visibilidad de Contenido para Customers Invitados

Si quieres mostrar contenido diferente, producto, o incluso crear un nodo separado para que sea visible solo para customers invitados, debes establecer las restricciones de visibilidad requeridas al customer group **Non-Authenticated Visitors**, o como lo nombres en tu aplicación.

Para eso, sigue la misma lógica descrita para customer groups pero ten en cuenta que al establecer las restricciones al customer group **Non-Authenticated Visitors**, deshabilitas otros customer groups de ver este contenido, landing page, producto, categoría o nodo. Significa que la información para la cual estableces las restricciones (por ejemplo, el nodo del web catalog Guest Products) va a ser mostrada exclusivamente a usuarios invitados. Una vez que se registran una cuenta, ya no pueden ver esta página. Siempre puedes agregar otra condición para dirigirte a la audiencia que necesitas.

![Nodo del Web Catalog de Invitados](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/guest_web_catalog_node-1-768x326.png)

OroCommerce ha diseñado la funcionalidad de invitados para ser lo suficientemente flexible como para adaptarse a cualquier necesidad de negocio. Puedes habilitar el acceso de invitados para los períodos de baja producción y restringirlo nuevamente cuando la carga de trabajo se vuelve más pesada. Puedes personalizar fácilmente cada nivel matizado de interacción de usuario invitado y definir cómo los invitados ven los productos, crean listas de compras o hacen checkout.

## Permisos para el Customer Group de Visitantes No Autenticados

Ahora que has pasado por las configuraciones clave del customer group de invitados y tienes toda la configuración en su lugar, es tiempo de definir los permisos apropiados y niveles de acceso para usuarios no autenticados. De esta manera, puedes controlar qué pueden y no pueden hacer los customers invitados en tu sitio web, proporcionando que la función de invitados relacionada esté habilitada.

Por ejemplo, puedes activar la opción de lista de compras de invitados pero restringir la capacidad de eliminarla, o activar el checkout de invitados pero deshabilitar el uso de cupones a menos que un usuario invitado se registre. Puedes agregar el flujo de trabajo necesario para cubrir las necesidades de customers invitados, como un checkout alternativo o de una sola página, asignando los permisos requeridos. Estas y otras opciones de acceso están disponibles para cualquier personalización dependiendo de tus necesidades de negocio bajo **Customers > Customer User Roles** en la configuración del sistema.

![Roles de Customer User de Invitados](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/guest_customer_user_roles.png)

En la siguiente sección, vamos a discutir permisos y niveles de acceso que pueden ser personalizados para cada uno de tus customers tanto desde el storefront como desde el back-office.