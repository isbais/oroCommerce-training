# Especificidades y Gestión de Customer Users

## Tabla de Contenidos
- [Introducción](#introducción)
- [Configuración de Customer User Settings](#configuración-de-customer-user-settings)
- [Creación de Customer User desde Storefront](#creación-de-customer-user-desde-storefront)
- [Creación de Customer User desde Back-Office](#creación-de-customer-user-desde-back-office)
- [Gestión de Customer User Details en Storefront](#gestión-de-customer-user-details-en-storefront)
- [Gestión de Customer User Details en Back-Office](#gestión-de-customer-user-details-en-back-office)

## Introducción

Un **customer user** es una persona, un empleado que actúa en nombre de una empresa determinada. Pueden tener diferentes permisos basados en su función en la organización del cliente. Usualmente, los customer users son gerentes de compras que registran sus cuentas en el storefront de la aplicación Oro y realizan las compras necesarias. Tus representantes de ventas también pueden registrar customer users desde el back-office. Ten en cuenta que los customer users no siempre tienen que representar una empresa o tener una cuenta. Pueden ser minoristas que compran un solo artículo para sí mismos o visitantes invitados que aún pueden crear una orden y comprar productos de tu tienda si tal comportamiento está habilitado en tu aplicación Oro.

## Configuración de Customer User Settings

Antes de comenzar a trabajar con customer users, primero debes configurar sus configuraciones básicas en la configuración del sistema. Estas configuraciones definen el comportamiento general del customer user en el storefront y te permiten controlar varias opciones de registro de customer user.

**Nota:** Si no tienes acceso a la configuración del sistema de la aplicación Oro, puedes pedir ayuda a un administrador.

![Configuración Global de Customer User](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/customer_user_global_config-1024x397.png)

Para modificar las configuraciones predeterminadas de customer user:

1. **Navega a la configuración del sistema** bajo **System > Configuration**. Aquí encontrarás todas las características del sistema (globales) que puedes personalizar específicamente para las necesidades de tu negocio. Configurar estas configuraciones significa que se aplican en todas las organizaciones, sitios web y usuarios en tu sistema. Las configuraciones de customer user se pueden modificar en tres niveles: global, organización y sitio web. En esta sección, nos enfocaremos solo en la configuración global, asumiendo que las mismas opciones también están disponibles para personalización en otros niveles.

   **Nota:** Para más detalles sobre los niveles de configuración utilizados en las aplicaciones Oro, consulta nuestra documentación en línea.

2. **Selecciona Commerce > Customer > Customer Users** en el menú de la izquierda.

3. **Alterna las opciones requeridas para:**
   - Habilitar o deshabilitar el registro de nuevos clientes desde la pantalla de inicio de sesión del storefront
   - Habilitar o deshabilitar el paso de confirmación por correo electrónico después del registro de usuario
   - Mostrar u ocultar el enlace de registro desde la pantalla de inicio de sesión del storefront
   - Mostrar u ocultar el campo de nombre de empresa en el formulario de registro en el storefront. Es útil para clientes individuales o minoristas que no representan ninguna empresa
   - Establecer las reglas para ingresar credenciales de usuario (sensible o insensible a mayúsculas), etc.

   **Nota:** Para obtener la lista completa de opciones y sus instrucciones detalladas, consulta nuestra documentación en línea.

4. **Una vez que las modificaciones necesarias estén completas, haz clic en Save settings** para aplicar los cambios. Para nuestro caso, hemos habilitado todas las opciones para ilustrar la extensión completa de la funcionalidad de customer user.

A partir de ahora, la configuración de tu sitio web seguirá las configuraciones que has aplicado para customer users.

Ahora puedes pasar al siguiente paso de crear un nuevo customer user.

Como hemos mencionado antes, un customer user puede ser creado de dos maneras, desde el storefront y desde el back-office.

## Creación de Customer User desde Storefront

Consideremos el primer caso: un gerente de compras de Twin Glass & Mirror establece la cuenta desde el storefront. Para hacerlo, necesitan hacer clic en **Sign Up** en la parte superior derecha de la página de tu tienda web.

![Botón de Registro](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/registration_button-1-768x325.png)

Una vez que el gerente completa el formulario de registro, proporcionando todos los detalles personales y de empresa requeridos, y lo envía, reciben una solicitud de confirmación por correo electrónico. Una vez que siguen con la acción solicitada, su cuenta se marca como confirmada.

![Formulario de Registro](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/registration_form-1-768x669.png)

La confirmación también puede ser procesada a través del back-office. Una vez que se envía una nueva aplicación, tu representante de ventas puede contactar a un potencial customer user y pedir más detalles, si es necesario, y luego confirmarlos en el sistema.

![Confirmar Customer User en Back-Office](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/confirm_customer_user_back_office-1-768x243.png)

Una vez confirmado, el customer user puede comenzar a interactuar con tu tienda web.

## Creación de Customer User desde Back-Office

Otra forma de crear un customer user es desde el back-office. Para nuestro caso, crearemos otro gerente de compras de la empresa Twin Glass & Mirror.

Para eso, navega a **Customers > Customer Users** en el menú principal y haz clic en **Create Customer User**. En la página que se abre, haz lo siguiente:

1. **Selecciona la casilla Enabled** para habilitar al usuario para iniciar sesión en el sistema y hacer su trabajo dentro de él al momento de la creación.

2. **Completa el Nombre del cliente** y otra información personal, como sigue:

![Crear Customer desde Back-Office Parte 1](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/create_customer_back_office_part1-1-768x525.png)

3. **Selecciona un customer** que este usuario representa. Para nuestro caso, seleccionaremos Twin Glass & Mirror. Este customer fue creado automáticamente cuando confirmamos al primer gerente de compras, Jerry Blackwill. Entonces, ahora podemos seleccionarlo de la lista. Si el customer al que pertenece el usuario no existe en el sistema, necesitarías crearlo primero, y luego proceder con agregar customer users a él.

   **Nota:** Discutiremos los customers en más detalle en las siguientes lecciones de esta sección.

![Crear Customer desde Back-Office Parte 2](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/create_customer_back_office_part_2-1-768x351.png)

4. **Asigna uno de tus representantes de ventas** para asistir a este cliente con su proceso de compra si surgen problemas. Un representante de ventas del cliente se aplica al customer user por defecto, pero puedes dejar este campo vacío, si es necesario, ya que es opcional.

5. **La opción Guest** indica si el customer user va a tener una cuenta o navegará por tu sitio web como invitado. Lo dejaremos deshabilitado, ya que pretendemos proporcionar a Felicity Haff una cuenta dedicada en el storefront.

6. **Selecciona las casillas Generate Password y Send Welcome Email** para notificar al customer user sobre la creación de su cuenta con una solicitud para restablecer la contraseña generada automáticamente con la suya propia.

7. **Selecciona el sitio web** del registro del customer user. Mientras que el customer user puede tener acceso a otros sitios web dentro de la misma organización, las notificaciones por correo electrónico concernientes a su cuenta de usuario apuntarán a este sitio web.

   **Nota:** Para más detalles sobre cómo gestionar varios sitios web, consulta nuestra documentación en línea.

8. **Selecciona una Localización Preferida** para el customer user. Este campo se muestra si más de una localización está habilitada para cualquiera de los sitios web de la organización actual. Si cambias el sitio web para el customer user, necesitarás seleccionar una nueva localización preferida.

9. **Agrega la dirección de facturación y envío** a los campos requeridos.

10. **En la sección Roles**, selecciona los roles que deben aplicarse al customer user. El rol tiene un cierto conjunto de permisos que definen qué pueden o no pueden hacer los customer users dentro del storefront de tu sitio web. Los roles se crean bajo **Customers > Customer User Roles**.

    **Nota:** Hay un módulo completo por delante (Sección 4) discutiendo un rol de customer user.

    En este punto, asegúrate de asignar al menos un rol a tu customer user. Si el customer user está deshabilitado, pueden ser guardados sin roles.

    Si seleccionas varios roles, los permisos otorgados se acumulan de todos los roles asignados.

    Para nuestro caso de uso, tenemos tres roles predefinidos. Estos son:

    - **Un administrador** que tiene los permisos de control más altos sobre el storefront del sitio web que les permiten crear otros customer users, asignar varios permisos a diferentes usuarios basados en sus responsabilidades laborales, ver órdenes, cotizaciones y solicitudes de cotización de todos los customer users bajo su organización. La lista de capacidades puede ser expandida o reducida, dependiendo de los requisitos de tu empresa para el rol particular.
    - **Un comprador** que opera su propia cuenta y puede ver solo los datos por los que es responsable, las listas de compras, órdenes y RFQs que han creado.
    - **Un visitante no autenticado** que navega por el storefront del sitio web como invitado. Las acciones que están permitidas para los usuarios invitados también dependen de tu estrategia de negocio, procesos y si apoyas el modelo B2C.

    **Nota:** Vamos a describir las características de invitado en detalle en la Sección 3 de este curso.

![Crear Customer desde Back-Office Parte 3](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/create_customer_back_office_part_3-1024x215.png)

11. **Haz clic en Save** para guardar tu nuevo customer user, Felicity Haff.

Para nuestro caso, le hemos asignado un rol de comprador, habilitándola para manejar solo sus propios registros.

Jerry Blackwill, el colega auto-registrado de Felicity Haff, también tiene asignado un rol de comprador. De esta manera, pueden hacer compras para la empresa Twin Glass & Mirror independientemente, sin acceder a los registros del otro.

Ten en cuenta que tal escenario se proporciona solo para propósitos de demostración. Tus roles pueden ser personalizados con cualquier permiso que tu negocio necesite.

Ahora, si verificas la cuadrícula de Customer Users, verás que ambos usuarios de Twin Glass & Mirror se muestran allí, junto con otros usuarios de las empresas con las que trabajas.

![Cuadrícula de Customer Users](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/customer_users_grid-1-768x300.png)

Tus representantes de ventas pueden entonces gestionar los detalles de estos usuarios, agregar los datos faltantes, ver sus solicitudes de cotización, cotizaciones, órdenes, listas de compras y otra actividad de marketing directamente desde el back-office. Las mismas acciones pueden ser tomadas por los customer users mismos desde sus cuentas del storefront. Los cambios que se hacen desde cualquiera de los dos lugares se reflejan en el otro, ya que la información entre tu storefront y back-office se sincroniza automáticamente.

Ahora echemos un vistazo más de cerca a cómo se puede gestionar la información de un customer user en ambos casos.

## Gestión de Customer User Details en Storefront

Iniciemos sesión en el storefront para revelar todo el alcance de capacidades disponibles para las cuentas registradas.

Para nuestro caso, iniciaremos sesión como Felicity Haff, una customer user recién creada. De esta manera, podemos ver cómo se muestra la información creada desde el back-office en el storefront.

Una vez que Felicity inicia sesión en el storefront de OroCommerce y navega a su menú de cuenta, podrá ver y gestionar su información de contacto personal, direcciones de facturación y envío, monitorear el estado de sus órdenes, cotizaciones, solicitudes de cotización y más.

![Página Principal del Perfil](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/profile_main_page-1-768x320.png)

El menú de cuenta predeterminado de cualquier customer user tiene las siguientes secciones:

- **My Profile** – consolida toda la información de contacto personal de los usuarios y las direcciones predeterminadas que usan para proporcionar ubicaciones de facturación y envío.

- **Address Book** – almacena tanto las direcciones de empresa como personales de un customer user. Dependiendo de los permisos del rol, un customer user puede o no ver y editar direcciones de empresa. En nuestro caso, Felicity puede ver las direcciones de la empresa Twin Glass & Mirror; sin embargo, está restringida de editarlas o eliminarlas.

![Sección del Menú Address Book](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/address_book_menu_section-1-768x470.png)

- **Users** – lista todos los miembros del equipo junto con otros empleados de la empresa del customer user y su información de contacto personal. Dependiendo de los permisos, tu customer user puede ver o ver y gestionar la información de los co-empleados. Aquí, también es posible agregar un nuevo customer user de tu organización haciendo clic en **+Create User**.

![Menú de Users para Admin](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/users_menu_for_admin-1-768x330.png)

Como nuestra Felicity tiene un rol de comprador, no puede gestionar la información de contacto de otros empleados o crear nuevos usuarios, así que su menú Users se ve así:

![Menú de Users para Comprador](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/users_menu_for_buyer-1-768x310.png)

- **Shopping Lists** almacena todas las listas actuales a las que un customer user puede acceder, mostrando solo aquellas que poseen por defecto. Con los permisos correctos, los usuarios pueden restablecer filtros, ver, actualizar, renombrar las listas de otros y completar el checkout por ellos.

![Sección de Shopping List para Admin](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/shopping_list_section_for_admin-1-768x435.png)

- **Requests for Quote** – almacena la información sobre todas las solicitudes de cotización enviadas de tu customer user. Aquí, pueden ver los detalles de las RFQs, verificar sus estados, imprimirlas o cancelarlas.

![Menú de RFQ](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/rfq_menu-1-768x343.png)

- **Order History** contiene todas las órdenes del cliente, tanto abiertas como enviadas. Los usuarios pueden ver detalles como número de orden, fecha de creación, dirección de envío, monto total, método de pago y estado. La cuadrícula de Open Orders lista órdenes incompletas, permitiendo a los usuarios reanudar el checkout si se interrumpe. Los usuarios pueden completar su compra haciendo clic en "Check Out" o eliminar órdenes inválidas. La cuadrícula de Past Orders muestra órdenes realizadas, donde los usuarios pueden revisar detalles y reenviar órdenes usando el enlace "Re-Order".

![Menú de Order History](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/order_history_menu-1-768x418.png)

**Nota:** Para más detalles sobre cómo revisar artículos ordenados, información de facturación y envío, y reordenar productos de órdenes anteriores, consulta nuestra documentación en línea.

- **Previously Purchased** muestra productos recién comprados para customer users, incluyendo sus precios. Los usuarios pueden agregar productos a listas de compras y filtrar por texto, nombre, SKU, precio y otros atributos. Por defecto, los productos se ordenan por recencia, con los más nuevos primero.

**Nota:** La visibilidad de esta sección puede ser gestionada por el administrador del sitio web.

- **Quotes** lista todas las cotizaciones de cliente creadas y enviadas. Los usuarios pueden ver, imprimir, aceptar y enviar cotizaciones para órdenes basadas en condiciones de RFQ negociadas. Declinar o cancelar cotizaciones requiere contactar representantes de ventas para manejarlo en el back-office. Una vez que las condiciones se acuerdan, la cotización puede ser transferida inmediatamente a una orden con la página de checkout pre-poblada. Si un usuario no está listo para completar su orden, se guardará en el menú Orders bajo la sección Open Orders, donde puedes localizarlos fácilmente.

**Nota:** Para más detalles sobre cómo aceptar una cotización ofrecida o enviar una cotización de invitado, consulta nuestra documentación en línea.

- **Saved Searches** permite a los clientes registrados guardar consultas de búsqueda con etiquetas personalizadas y recibir notificaciones para productos nuevos o reabastecidos. Los usuarios pueden ver, renombrar y gestionar notificaciones para sus búsquedas guardadas. Es importante notar que hay un límite pre-configurado para notificaciones de resultados de búsqueda establecido en el back-office. Las notificaciones por correo electrónico no se enviarán para búsquedas que contengan más productos que el límite establecido, y las nuevas consultas de búsqueda que excedan este límite no pueden tener notificaciones habilitadas.

![Crear Saved Search](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/create_saved_search-768x249.png)
![Lista de Saved Search](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/saved_search_list-768x361.png)

## Gestión de Customer User Details en Back-Office

Ahora eres consciente de que los customer users pueden gestionar sus cuentas, detalles de contacto, RFQs, órdenes y otras actividades desde el storefront. Los gerentes de ventas también pueden realizar estas acciones en el back-office.

Para acceder al perfil de Felicity Haff, ve a **Customers > Customer Users** en el back-office. Aquí, puedes gestionar información del usuario (nombre, dirección, teléfono), ver RFQs, órdenes, listas de compras y comunicaciones del cliente (correos electrónicos, notas, eventos). También puedes habilitar/deshabilitar al usuario, restablecer la contraseña, agregar aplicaciones OAuth e impersonar al usuario para solucionar problemas.

![Página de Customer User en Back-Office](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/customer_user_page_back_office-1-768x362.png)

La cuenta de Felicity ahora incluye RFQs, órdenes, consentimientos aceptados/declinados y listas de compras abiertas. Las secciones Activity, Marketing Activity y Additional Information registran interacciones del cliente, como negociaciones, llamadas, correos electrónicos, notas y eventos.

![Agregar Actividad de Customer User en Back-Office](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/customer_user_add_activity_back_office-1-768x316.png)

En la sección de aplicaciones OAuth, puedes agregar múltiples aplicaciones OAuth a tu customer user para proporcionar a estas aplicaciones acceso delegado seguro al storefront de OroCommerce. Las aplicaciones Oro soportan el tipo de autorización de credenciales OAuth 2.0 para habilitar la conexión de aplicaciones de terceros a la API web.

**Nota:** Para más detalles sobre cómo agregar una aplicación OAuth a tu customer user, generar credenciales y recuperar un token de acceso para conectarte a tu aplicación Oro, consulta nuestra documentación en línea.

Una característica adicional útil aquí es la posibilidad de iniciar sesión en el storefront en nombre de un customer user seleccionado y solucionar los problemas que el cliente ha enfrentado.

La característica está disponible para los usuarios del back-office con la capacidad de rol Login As Customer User.

**Nota:** Para más detalles sobre los roles de usuario del back-office, consulta nuestra documentación en línea. https://doc.oroinc.com/user/back-office/system/user-management/roles/admin-capabilities/#admin-capabilities

![Login as Customer User](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/login_as_customer_user-1.png)

Para impersonar a Felicity, haz clic en **Login as a User**; esto abre el storefront en una nueva pestaña. Después de completar cualquier acción, cierra sesión del modo de impersonación.

![Modo de Impersonación en Storefront](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/impersonation_mode_storefront-1-768x318.png)

Finalmente, puedes deshabilitar o eliminar tu usuario permanentemente haciendo clic en el botón requerido en la parte superior derecha de la página.

Ahora entiendes cómo crear y gestionar customer users en OroCommerce tanto desde el storefront como desde el back-office, con datos sincronizados entre los dos. A continuación, cubriremos los customers que representan empresas en la aplicación OroCommerce y sus características únicas.