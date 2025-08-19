# Roles de Customer User

## Tabla de Contenidos
- [Introducción](#introducción)
- [Concepto de Roles de Customer User](#concepto-de-roles-de-customer-user)
- [Gestión de Roles](#gestión-de-roles)
- [Roles Predefinidos](#roles-predefinidos)
- [Tipos de Roles](#tipos-de-roles)

## Introducción

Ahora que has aprendido los fundamentos de la gestión de clientes en las aplicaciones Oro, es tiempo de cubrir un último tema: **customer user roles**, permisos y niveles de acceso.

En esta sección, aprenderás cómo:

- **Crear y configurar customer user roles**, asignar los roles a customers para darles un área particular de responsabilidad.
- **Otorgar permisos y establecer los niveles de acceso requeridos** a ciertas acciones en el storefront para asegurar una interacción de customer user dentro del sitio web basada en sus funciones laborales.
- **Auto-gestionar customers** desde el storefront usando la información bajo el menú My Account.
- **Gestionar roles** en el back-office.

## Concepto de Roles de Customer User

Un **customer user role** es un conjunto de permisos y niveles de acceso predefinidos asignados a un customer user. Basado en las funciones laborales del customer (por ejemplo, un gerente de ventas, un miembro del equipo de marketing, o un administrador), los customer user roles aseguran que los usuarios de la aplicación estén autorizados a acceder solo a datos relevantes para sus responsabilidades laborales. Los roles también ayudan a definir qué pueden y no pueden hacer los usuarios dentro del sitio web. Ayudan a reducir el riesgo de error humano al permitirte delegar responsabilidades y permisos a ciertos usuarios únicamente.

Una vez que creas un customer, puedes asignarle un rol particular para darle a este customer un área requerida de responsabilidad. De esta manera, puedes restringir al customer de realizar ciertas acciones que exceden su jurisdicción, por ejemplo, ver y editar solicitudes de cotización de otros co-empleados o crear nuevas accounts. Mientras tanto, habilitar estas acciones para otros roles (por ejemplo, administradores, líderes de equipo) hace posible verificar y aprobar las RFQs, cotizaciones y órdenes creadas y realizadas por sus miembros del equipo, verificar los estados, ejecutar auditorías, crear nuevas cuentas de usuario y asignarles los roles requeridos.

Las capacidades de customer user role son vastas y diversas, lo que te permite adaptar las funciones del rol como necesites.

Los roles pueden ser auto-gestionados por un customer user desde su menú de cuenta en el storefront, bajo la sección **Roles**, siempre que tengan el acceso requerido.

![Roles de Customer User en Storefront](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/customer_user_roles_storefront-1-768x350.png)

Alternativamente, puedes gestionarlos desde el back-office de tu aplicación, bajo **Customers > Customer User Roles**.

![Roles de Customer User en Back-Office](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/customer_user_roles_back_office-1024x241.png)

## Roles Predefinidos

Por defecto, hay tres **customer user roles** predefinidos ofrecidos por OroCommerce. Estos son los roles típicos que pueden cubrir la mayoría de tus casos de negocio de customer.

- **Non-Authenticated Visitors** – el rol que define los permisos para todos tus customers no registrados. Si has habilitado una cierta característica de invitados en la configuración del sistema, pero no funciona en el storefront, la razón puede estar oculta aquí. Debes verificar si el permiso de característica correspondiente (por ejemplo, cotización o checkout) está otorgado para el rol. Este rol se muestra y solo puede ser gestionado desde el back-office ya que los customers invitados no tienen cuentas.
- **Buyer** – el rol habilita a sus usuarios a gestionar sus cuentas personales, ordenar productos y negociar las cotizaciones con gerentes de ventas.
- **Administrator** – el rol proporciona el nivel más alto de permisos a sus usuarios. Tales customers pueden acceder a todas las funciones administrativas dentro de un solo sitio. Controlan las actividades de todos los compradores de la empresa en el sitio web, pueden crear nuevos customer users y asignar un rol específico a cada uno de ellos.

## Tipos de Roles

Cada rol recién creado puede ser de tipo predefinido o personalizable. Cuando un rol se asigna a un customer determinado en los detalles del rol, se vuelve personalizable y está disponible solo para este customer específico. Si no se asigna ningún customer, el tipo de rol se vuelve predefinido, habilitando a cualquier customer a usarlo.

![Tipos de Roles](https://hive.oroinc.com/wp-content/uploads/sites/21/2021/02/role_types-1-768x268.png)

**Nota:** Los roles predefinidos no pueden ser editados directamente. Una vez que llegues a la página de edición y comiences a editar el rol, el sistema automáticamente copiará todos los datos originales y creará un nuevo rol idéntico, que luego puedes guardar bajo un nombre diferente. Todos los usuarios serán movidos del rol original a este nuevo rol después de que hagas clic en Save.

Si el rol es predefinido, tampoco puede ser eliminado. Tampoco puede ser eliminado si está asignado a un usuario/usuarios. Reasigna los usuarios asignados a un rol diferente para poder eliminarlo.

Para crear un nuevo rol, haz clic en **Create Customer User Role** en la parte superior derecha de la página y establece los permisos apropiados y niveles de acceso a los campos de entidad seleccionados.
